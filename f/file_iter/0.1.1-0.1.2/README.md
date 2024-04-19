# Comparing `tmp/file_iter-0.1.1.tar.gz` & `tmp/file_iter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_iter-0.1.1.tar", max compression
+gzip compressed data, was "file_iter-0.1.2.tar", max compression
```

## Comparing `file_iter-0.1.1.tar` & `file_iter-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2024-04-05 19:06:27.300345 file_iter-0.1.1/LICENSE
--rw-r--r--   0        0        0     1894 2024-04-12 14:11:20.845268 file_iter-0.1.1/README.md
--rw-r--r--   0        0        0      106 2024-04-06 16:59:35.449657 file_iter-0.1.1/file_iter/__init__.py
--rw-r--r--   0        0        0     9552 2024-04-12 14:17:04.345030 file_iter-0.1.1/file_iter/file_iter.py
--rw-r--r--   0        0        0      915 2024-04-11 21:42:53.651502 file_iter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 file_iter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-05 19:06:27.300345 file_iter-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1894 2024-04-12 14:11:20.845268 file_iter-0.1.2/README.md
+-rw-r--r--   0        0        0      146 2024-04-19 13:24:01.364289 file_iter-0.1.2/file_iter/__init__.py
+-rw-r--r--   0        0        0    10041 2024-04-19 13:24:01.364289 file_iter-0.1.2/file_iter/file_iter.py
+-rw-r--r--   0        0        0      986 2024-04-19 13:24:01.364289 file_iter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 file_iter-0.1.2/PKG-INFO
```

### Comparing `file_iter-0.1.1/LICENSE` & `file_iter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `file_iter-0.1.1/README.md` & `file_iter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `file_iter-0.1.1/file_iter/file_iter.py` & `file_iter-0.1.2/file_iter/file_iter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,137 +1,140 @@
+"""A Swiss Army knife iterator for files (or any iterator of strings)."""
+
 import itertools
 from collections import deque
 from pathlib import Path
 from typing import Any, Callable, Iterable, Iterator, Literal, overload
 
 _marker: Any = object()
 
 
 class FileIter(Iterator[str]):
     """
-    A Swiss Army knife iterator for files (or any iterator of strings)
+    A Swiss Army knife iterator for files (or any iterator of strings).
 
     - Strips lines
     - Keeps track of the current line: `current_line`
     - Keeps track of the line number: `position`
         - Specify position if entering in the middle of a file: `FileIter(f, position=10)`
     - Peek at the next line: `peek()`
     - Jump ahead `n` lines `jump(n)`
     - Check if empty: `isempty()`
     - Filter out unimportant lines:
         - Always filter: `FileIter(f, filter_func=is_data)`
         - Filter only single next(): `filter_next(filter_func)`
 
-    >>> def is_data(line: str) -> bool:
+    >>> def is_data(line:  str) -> bool:
     ...    return len(line) > 0 and (line[0] != "#")
-    >>> my_iter = FileIter(
+    >>> file_iter = FileIter(
     ...     ["Hello", "", "# comment", "World", "How", "are", "you?"],
     ...     filter_func=is_data
     ... )
-    >>> next(my_iter)
+    >>> next(file_iter)
     'Hello'
-    >>> my_iter.peek()  # peek does not respect filter_func
+    >>> file_iter.peek()  # peek does not respect filter_func
     ''
-    >>> next(my_iter)  # skips "" and "# comment"
+    >>> next(file_iter)  # skips "" and "# comment"
     'World'
-    >>> my_iter.position
+    >>> file_iter.position
     3
-    >>> my_iter.current_line
+    >>> file_iter.current_line
     'World'
-    >>> my_iter.jump(3)  # jump does not respect filter_func
+    >>> file_iter.jump(3)  # jump does not respect filter_func
     'you?'
-    >>> my_iter.position
+    >>> file_iter.position
     6
-    >>> my_iter.isempty()
+    >>> file_iter.isempty()
     True
-    >>> my_iter.peek(default="default")
+    >>> file_iter.peek(default="default")
     'default'
     """
 
     def __init__(
         self,
         iterable: Iterable[str],
         position: int = -1,
         filter_func: Callable[[str], bool] | None = None,
     ) -> None:
         """
+        Initialize the FileIter object.
+
         :param iterable: an iterable object
         :param position: the current position in the iterable
         :param filter_func: a function that checks if the line is useful, otherwise skips
         :return: an iterator object
         """
         self._it = iter(iterable)
         self._cache: deque[str] = deque()
         self._current_line: str = _marker
         self._filter_func = filter_func
         self._position = position
 
     def __iter__(self) -> Iterator[str]:
+        """Iterate over self."""
         return self
 
     def __next__(self) -> str:
         """
-        Get the next element in the iterator
+        Get the next element in the iterator.
 
         Applies the filter function if it exists
-        >>> my_iter = FileIter(["", "# comment", "data"], filter_func=is_data)
-        >>> next(my_iter)
+        >>> file_iter = FileIter(["", "# comment", "data"], filter_func=is_data)
+        >>> next(file_iter)
         'data'
-        >>> my_iter.position
+        >>> file_iter.position
         2
-        >>> my_iter = FileIter(["", "# no", "", "# data"], filter_func=is_data)
-        >>> for line in my_iter:
+        >>> file_iter = FileIter(["", "# no", "", "# data"], filter_func=is_data)
+        >>> for line in file_iter:
         ...     print(line)
         """
         if self._filter_func is None:
             return self._next()
 
         while not (self._filter_func(self._next())):
             pass
 
         return self._current_line
 
     def _next(self) -> str:
         """
-        Return the next line and update the position
+        Return the next line and update the position.
 
         Updates the line number only if successful
         """
         line = self._cache.popleft() if self._cache else next(self._it)
         self._current_line = line.strip()
         self._position += 1
         return self._current_line
 
     @overload
-    def filtered_next(self, filter_func: Callable[[str], bool]) -> str:
-        ...
+    def filtered_next(self, filter_func: Callable[[str], bool]) -> str: ...
 
     @overload
     def filtered_next(
         self, filter_func: Callable[[str], bool], default: object
-    ) -> str | object:
-        ...
+    ) -> str | object: ...
 
     def filtered_next(
         self,
         filter_func: Callable[[str], bool],
         default: str | object = _marker,
     ) -> str | object:
         """
-        Get the next element in the iterator that passes the filter function
+        Get the next element in the iterator that passes the filter function.
 
         :param filter_func: a function that checks if the line is valid
 
-        >>> my_iter = FileIter(["", "# comment", "hello"])
-        >>> my_iter.filtered_next(is_data)
+        >>> file_iter = FileIter(["", "# comment", "hello"])
+        >>> file_iter.filtered_next(is_data)
         'hello'
-        >>> my_iter = FileIter(["", "# no", "", "# data"])
-        >>> my_iter.filtered_next(is_data, default="default")
+        >>> file_iter = FileIter(["", "# no", "", "# data"])
+        >>> file_iter.filtered_next(is_data, default="default")
         'default'
-        >>> my_iter.filtered_next(is_data)
+        >>> file_iter.filtered_next(is_data)
         Traceback (most recent call last):
         ...
         StopIteration
         """
         try:
             while not filter_func(next(self)):
                 pass
@@ -140,108 +143,106 @@
             if default is _marker:
                 raise
             return default
 
     @property
     def position(self) -> int:
         """
-        Get the current position in the iterator
+        Get the current position in the iterator.
 
         Note: -1 indicates the iterator has not been read yet
 
-        >>> my_iter = FileIter(["a", "b", "c"])
-        >>> my_iter.position
+        >>> file_iter = FileIter(["a", "b", "c"])
+        >>> file_iter.position
         -1
-        >>> next(my_iter), next(my_iter)
+        >>> next(file_iter), next(file_iter)
         ('a', 'b')
-        >>> my_iter.position
+        >>> file_iter.position
         1
         """
         return self._position
 
     @property
     def current_line(self) -> str:
         """
-        Get the current line in the iterator
+        Get the current line in the iterator.
 
-        >>> my_iter = FileIter(["a", "b", "c"])
-        >>> my_iter.current_line
+        >>> file_iter = FileIter(["a", "b", "c"])
+        >>> file_iter.current_line
         Traceback (most recent call last):
         ...
         ValueError: Have not read any lines yet
-        >>> next(my_iter), next(my_iter)
+        >>> next(file_iter), next(file_iter)
         ('a', 'b')
-        >>> my_iter.current_line
+        >>> file_iter.current_line
         'b'
         """
         if self._current_line is _marker:
             raise ValueError("Have not read any lines yet")
 
         return self._current_line
 
     def jump(self, num: int) -> str:
         """
-        Jump forward the specified number of elements in the iterator
+        Jump forward the specified number of elements in the iterator.
 
         Note: jump does not respect the filter function
 
         :param num: the number of elements to jump forward
         :return: the line n-steps forward
 
-        >>> my_iter = FileIter(["a", "b", "c"])
-        >>> next(my_iter)
+        >>> file_iter = FileIter(["a", "b", "c"])
+        >>> next(file_iter)
         'a'
-        >>> my_iter.jump(2)
+        >>> file_iter.jump(2)
         'c'
-        >>> my_iter.position
+        >>> file_iter.position
         2
-        >>> my_iter.jump(-1)
+        >>> file_iter.jump(-1)
         Traceback (most recent call last):
         ...
         IndexError: Can only jump forward
         """
         if num < 1:
             raise IndexError("Can only jump forward")
 
         for _ in itertools.islice(self, num - 1):
             pass
 
         return next(self)
 
     @overload
-    def peek(self) -> str:
-        ...
+    def peek(self) -> str: ...
 
     @overload
-    def peek(self, default: object) -> object | str:
-        ...
+    def peek(self, default: object) -> object | str: ...
 
     def peek(self, default: object = _marker) -> object | str:
         """
-        Get the next element in the iterator without consuming it
+        Get the next element in the iterator without consuming it.
 
         Note: peek does not respect the filter function
 
         :param default: the value to return if the iterator is empty
         :return: the next element in the iterator
 
-        >>> my_iter = FileIter(["a", "b", "c"], filter_func=lambda x: x != "b")
-        >>> my_iter.peek()
+        >>> file_iter = FileIter(["a", "b", "c"], filter_func=lambda x: x != "b")
+        >>> file_iter.peek()
         'a'
-        >>> my_iter.position
+        >>> file_iter.position
         -1
-        >>> next(my_iter), my_iter.position
+        >>> next(file_iter), file_iter.position
         ('a', 0)
-        >>> my_iter.peek(), my_iter.position
+        >>> file_iter.peek(), file_iter.position
         ('b', 0)
-        >>> next(my_iter)
+        >>> next(file_iter)
         'c'
-        >>> my_iter.peek("default")
+        >>> file_iter.peek("default")
         'default'
-        >>> my_iter.peek()
+        >>> file_iter.peek()
         Traceback (most recent call last):
         ...
         StopIteration
         """
         if not self._cache:
             try:
                 self._cache.append(next(self._it))
@@ -249,87 +250,91 @@
                 if default is _marker:
                     raise
                 return default
         return self._cache[0]
 
     def isempty(self) -> bool:
         """
-        Check if the iterator is empty
+        Check if the iterator is empty.
 
-        >>> my_iter = FileIter(["a", "b", "c"])
-        >>> my_iter.isempty()
+        >>> file_iter = FileIter(["a", "b", "c"])
+        >>> file_iter.isempty()
         False
-        >>> next(my_iter), next(my_iter), next(my_iter)
+        >>> next(file_iter), next(file_iter), next(file_iter)
         ('a', 'b', 'c')
-        >>> my_iter.isempty()
+        >>> file_iter.isempty()
         True
         """
         try:
             self.peek()
             return False
         except StopIteration:
             return True
 
 
 class FileIterContextManager:
-    """
-    Manage opening and closing a file for iteration
+    r"""
+    Manage opening and closing a file for iteration.
 
     See FileIter for more information
     Note: contextlib.contextmanager is not used to avoid mypy issues
 
     >>> from tempfile import NamedTemporaryFile
     >>> with NamedTemporaryFile("w") as f:
-    ...     _ = f.write("Hello\\n# comment\\n\\nWorld")
+    ...     _ = f.write("Hello\n# comment\n\nWorld")
     ...     _ = f.seek(0)
     ...
-    ...     with FileIterContextManager(f.name, filter_func=is_data) as my_iter:
-    ...         for line in my_iter:
-    ...             print(line, my_iter.position)
+    ...     with FileIterContextManager(f.name, filter_func=is_data) as file_iter:
+    ...         for line in file_iter:
+    ...             print(line, file_iter.position)
     Hello 0
     World 3
     >>> with NamedTemporaryFile("w") as f:  # doctest: +ELLIPSIS
     ...     name = f.name
-    ...     _ = f.write("Hello\\n# comment\\n\\nWorld")
+    ...     _ = f.write("Hello\n# comment\n\nWorld")
     ...     _ = f.seek(0)
     ...
-    ...     with FileIterContextManager(f.name, filter_func=is_data) as my_iter:
-    ...         my_iter.jump(-1)
+    ...     with FileIterContextManager(f.name, filter_func=is_data) as file_iter:
+    ...         _ = next(file_iter), next(file_iter)
+    ...         file_iter.jump(-1)
     Traceback (most recent call last):
     ...
     IndexError: Can only jump forward
-    Error reading ... at line=-1
+    Error reading ... at line=3
     """
 
     def __init__(
         self,
         filename: str | Path,
         position: int = -1,
         filter_func: Callable[[str], bool] | None = None,
     ) -> None:
         self.filename = Path(filename)
-        self.position = position
+        self.start_position = position
         self.filter_func = filter_func
 
     def __enter__(self) -> FileIter:
+        """Open the file and return a FileIter object."""
         self.file = open(self.filename)
-        return FileIter(self.file, self.position, self.filter_func)
+        self.file_iter = FileIter(self.file, self.start_position, self.filter_func)
+        return self.file_iter
 
     def __exit__(
         self, exc_type: type | None, exc_value: Exception | None, traceback: Any | None
     ) -> Literal[False]:
+        """Close the file and indicate the position if there is an exception."""
         if exc_value is not None:
-            exc_value.add_note(f"Error reading {self.filename} at line={self.position}")
+            exc_value.add_note(f"Error reading {self.filename} at line={self.file_iter.position}")
         self.file.close()
         return False
 
 
 def is_data(line: str) -> bool:
     """
-    Check if the line contains data (presumes it has been stripped)
+    Check if the line contains data (presumes it has been stripped).
 
     >>> is_data("hello")
     True
     >>> is_data("# comment")
     False
     >>> is_data("")
     False
```

### Comparing `file_iter-0.1.1/pyproject.toml` & `file_iter-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [tool.poetry]
 name = "file_iter"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Swiss Army knife iterator for files (or any iterator of strings)"
 authors = ["Jonathon Vandezande"]
 keywords = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jevandezande/file_iter"
 
 [tool.poetry.dependencies]
 python = ">=3.12"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "*"
 pre-commit = "*"
-ruff = ">=0.3.0"
+ruff = ">=0.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov = "*"
 
 [tool.ruff]
 line-length = 100
 
 [tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
+    "D",  # pydocstyle
 ]
 
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
 [tool.mypy]
 files = ["file_iter"]
 strict = true
 pretty = true
 
 [tool.pytest.ini_options]
 testpaths = ["file_iter"]
```

### Comparing `file_iter-0.1.1/PKG-INFO` & `file_iter-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_iter
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Swiss Army knife iterator for files (or any iterator of strings)
 Home-page: https://github.com/jevandezande/file_iter
 License: MIT
 Author: Jonathon Vandezande
 Requires-Python: >=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

