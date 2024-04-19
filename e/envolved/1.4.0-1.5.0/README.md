# Comparing `tmp/envolved-1.4.0.tar.gz` & `tmp/envolved-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envolved-1.4.0.tar", max compression
+gzip compressed data, was "envolved-1.5.0.tar", max compression
```

## Comparing `envolved-1.4.0.tar` & `envolved-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2095 2024-03-02 19:00:13.745648 envolved-1.4.0/LICENSE
--rw-r--r--   0        0        0     1942 2024-03-02 19:00:13.745648 envolved-1.4.0/README.md
--rw-r--r--   0        0        0      463 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/__init__.py
--rw-r--r--   0        0        0       22 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/_version.py
--rw-r--r--   0        0        0      290 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/basevar.py
--rw-r--r--   0        0        0     2254 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/describe/__init__.py
--rw-r--r--   0        0        0     4303 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/describe/flat.py
--rw-r--r--   0        0        0     4068 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/describe/nested.py
--rw-r--r--   0        0        0     1114 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/describe/util.py
--rw-r--r--   0        0        0     5623 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/envparser.py
--rw-r--r--   0        0        0    16304 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/envvar.py
--rw-r--r--   0        0        0      371 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/exceptions.py
--rw-r--r--   0        0        0     2635 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/factory_spec.py
--rw-r--r--   0        0        0      228 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/infer_env_var.py
--rw-r--r--   0        0        0    12531 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/parsers.py
--rw-r--r--   0        0        0        0 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/py.typed
--rw-r--r--   0        0        0      823 2024-03-02 19:00:13.745648 envolved-1.4.0/envolved/utils.py
--rw-r--r--   0        0        0     3591 2024-03-02 19:00:13.745648 envolved-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 envolved-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2095 2024-04-19 19:03:13.106566 envolved-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1942 2024-04-19 19:03:13.106566 envolved-1.5.0/README.md
+-rw-r--r--   0        0        0      463 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/_version.py
+-rw-r--r--   0        0        0      290 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/basevar.py
+-rw-r--r--   0        0        0     2254 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/describe/__init__.py
+-rw-r--r--   0        0        0     4303 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/describe/flat.py
+-rw-r--r--   0        0        0     4068 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/describe/nested.py
+-rw-r--r--   0        0        0     1114 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/describe/util.py
+-rw-r--r--   0        0        0     4080 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/envparser.py
+-rw-r--r--   0        0        0    17963 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/envvar.py
+-rw-r--r--   0        0        0      371 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/exceptions.py
+-rw-r--r--   0        0        0     2635 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/factory_spec.py
+-rw-r--r--   0        0        0      228 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/infer_env_var.py
+-rw-r--r--   0        0        0    13917 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/parsers.py
+-rw-r--r--   0        0        0        0 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/py.typed
+-rw-r--r--   0        0        0      823 2024-04-19 19:03:13.110566 envolved-1.5.0/envolved/utils.py
+-rw-r--r--   0        0        0     3580 2024-04-19 19:03:13.110566 envolved-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 envolved-1.5.0/PKG-INFO
```

### Comparing `envolved-1.4.0/LICENSE` & `envolved-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/README.md` & `envolved-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/envolved/describe/__init__.py` & `envolved-1.5.0/envolved/describe/__init__.py`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/envolved/describe/flat.py` & `envolved-1.5.0/envolved/describe/flat.py`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/envolved/describe/nested.py` & `envolved-1.5.0/envolved/describe/nested.py`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/envolved/describe/util.py` & `envolved-1.5.0/envolved/describe/util.py`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/envolved/envparser.py` & `envolved-1.5.0/envolved/envparser.py`

 * *Files 24% similar despite different names*

```diff
@@ -55,21 +55,19 @@
 
     def __init__(self):
         self.lock = Lock()
         self.reload()
 
 
 class AuditingEnvParser(ReloadingEnvParser):
-    environ_case_insensitive: MutableMapping[str, Set[str]]
-
     def __init__(self):
         super().__init__()
         sys.addaudithook(self.audit_hook)
 
-    def audit_hook(self, event: str, args: Tuple[Any, ...]):  # pragma: no cover
+    def audit_hook(self, event: str, args: Tuple[Any, ...]):
         if event == "os.putenv":
             if not args:
                 return
             key = args[0]
             if isinstance(key, bytes):
                 try:
                     key = key.decode("ascii")
@@ -116,57 +114,19 @@
         if ret is None:
             # someone messed with the env without triggering the auditing hook
             self.reload()
             return self.get(case_sensitive, key)
         return ret
 
 
-class NonAuditingEnvParser(ReloadingEnvParser):
-    def get(self, case_sensitive: bool, key: str) -> str:
-        if case_sensitive:
-            return getenv_unsafe(key)
-
-        def out_of_date() -> str:
-            self.reload()
-            return get_case_insensitive(retry_allowed=False)
-
-        lowered = key.lower()
-
-        def get_case_insensitive(retry_allowed: bool) -> str:
-            if retry_allowed and lowered not in self.environ_case_insensitive:
-                # if a retry is allowed, and no candidates are available, we need to retry
-                return out_of_date()
-            candidates = self.environ_case_insensitive[lowered]
-            if key in candidates:
-                preferred_key = key
-            elif retry_allowed and has_env(key):
-                # key is not a candidate, but it is in the env
-                return out_of_date()
-            elif len(candidates) == 1:
-                (preferred_key,) = candidates
-            elif retry_allowed:
-                return out_of_date()
-            else:
-                raise CaseInsensitiveAmbiguityError(candidates)
-            ret = getenv(preferred_key)
-            if ret is None:
-                assert retry_allowed
-                return out_of_date()
-            return ret
-
-        return get_case_insensitive(retry_allowed=True)
-
-
 EnvParser: Type[BaseEnvParser]
 if name == "nt":
     # in windows, all env vars are uppercase
     EnvParser = CaseInsensitiveEnvParser
-elif sys.version_info >= (3, 8):  # adding audit hooks is only supported in python 3.8+
-    EnvParser = AuditingEnvParser
 else:
-    EnvParser = NonAuditingEnvParser
+    EnvParser = AuditingEnvParser
 
 
 env_parser = EnvParser()
 """
 A global parser used by environment variables
 """
```

### Comparing `envolved-1.4.0/envolved/envvar.py` & `envolved-1.5.0/envolved/envvar.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,21 @@
 
 class Discard(Enum):
     discard = auto()
 
 
 discard = Discard.discard
 
+
+class Unchanged(Enum):
+    unchanged = auto()
+
+
+unchanged = Unchanged.unchanged
+
 Description = Union[str, Sequence[str]]
 
 
 @dataclass
 class Factory(Generic[T]):
     callback: Callable[[], T]
 
@@ -130,15 +137,21 @@
         return _EnvVarResult(value, exists=True)
 
     @abstractmethod
     def _get(self, **kwargs: Any) -> T:
         pass
 
     @abstractmethod
-    def with_prefix(self: Self, prefix: str) -> Self:
+    def with_prefix(
+        self: Self,
+        prefix: str,
+        *,
+        default: Union[T, Factory[T], Missing, Discard, Unchanged] = unchanged,
+        description: Union[Description, None, Unchanged] = unchanged,
+    ) -> Self:
         pass
 
     @abstractmethod
     def _get_children(self) -> Iterable[EnvVar]:
         pass
 
     def _get_descendants(self) -> Iterable[EnvVar]:
@@ -190,23 +203,43 @@
         except CaseInsensitiveAmbiguityError as cia:
             raise RuntimeError(f"environment error: cannot choose between environment variables {cia.args[0]}") from cia
 
         if self.strip_whitespaces:
             raw_value = raw_value.strip()
         return self.type(raw_value, **kwargs)
 
-    def with_prefix(self, prefix: str) -> SingleEnvVar[T]:
+    def with_prefix(
+        self,
+        prefix: str,
+        *,
+        default: Union[T, Factory[T], Missing, Discard, Unchanged] = unchanged,
+        description: Union[Description, None, Unchanged] = unchanged,
+        type: Union[Type[T], Parser[T], Unchanged] = unchanged,
+        case_sensitive: Union[bool, Unchanged] = unchanged,
+        strip_whitespaces: Union[bool, Unchanged] = unchanged,
+    ) -> SingleEnvVar[T]:
+        if default is unchanged:
+            default = self.default
+        if description is unchanged:
+            description = self.description
+        type_ = type
+        if type_ is unchanged:
+            type_ = self.type
+        if case_sensitive is unchanged:
+            case_sensitive = self.case_sensitive
+        if strip_whitespaces is unchanged:
+            strip_whitespaces = self.strip_whitespaces
         return register_env_var(
             SingleEnvVar(
                 prefix + self._key,
-                self.default,
-                type=self.type,
-                description=self.description,
-                case_sensitive=self.case_sensitive,
-                strip_whitespaces=self.strip_whitespaces,
+                default,
+                type=type_,
+                description=description,
+                case_sensitive=case_sensitive,
+                strip_whitespaces=strip_whitespaces,
                 validators=self._validators,
             )
         )
 
     def _get_children(self) -> Iterable[EnvVar[Any]]:
         return ()
 
@@ -288,22 +321,39 @@
                     raise SkipDefault(errs[0])
                 if isinstance(self.on_partial, Factory):
                     return self.on_partial.callback()
                 return self.on_partial  # type: ignore[return-value]
             raise errs[0]
         return self._type(*pos_values, **kw_values)
 
-    def with_prefix(self, prefix: str) -> SchemaEnvVar[T]:
+    def with_prefix(
+        self,
+        prefix: str,
+        *,
+        default: Union[T, Factory[T], Missing, Discard, Unchanged] = unchanged,
+        description: Union[Unchanged, None, Description] = unchanged,
+        type: Union[Type[T], Parser[T], Unchanged] = unchanged,
+        on_partial: Union[T, Missing, AsDefault, Discard, Factory[T], Unchanged] = unchanged,
+    ) -> SchemaEnvVar[T]:
+        if default is unchanged:
+            default = self.default
+        if description is unchanged:
+            description = self.description
+        type_ = type
+        if type_ is unchanged:
+            type_ = self.type
+        if on_partial is unchanged:
+            on_partial = self.on_partial
         return register_env_var(
             SchemaEnvVar(
                 {k: v.with_prefix(prefix) for k, v in self._args.items()},
-                self.default,
-                type=self._type,
-                description=self.description,
-                on_partial=self.on_partial,
+                default,
+                type=type_,
+                description=description,
+                on_partial=on_partial,
                 validators=self._validators,
                 pos_args=tuple(v.with_prefix(prefix) for v in self._pos_args),
             )
         )
 
     def _get_children(self) -> Iterable[EnvVar[Any]]:
         return chain(self._args.values(), self._pos_args)
```

### Comparing `envolved-1.4.0/envolved/factory_spec.py` & `envolved-1.5.0/envolved/factory_spec.py`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/envolved/parsers.py` & `envolved-1.5.0/envolved/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import re
 from enum import Enum, auto
-from functools import lru_cache
 from itertools import chain
 from sys import version_info
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
@@ -134,107 +133,122 @@
     for k, v in pairs:
         if k in ret:
             raise ValueError(f"duplicate key {k}")
         ret[k] = v
     return ret
 
 
+def strip_opener_idx(x: str, opener: Pattern[str]) -> int:
+    opener_match = opener.match(x)
+    if not opener_match:
+        raise ValueError("position 0, expected opener")
+    return opener_match.end()
+
+
+def strip_closer_idx(x: str, closer: Needle, pos: int) -> int:
+    if isinstance(closer, str):
+        if len(closer) + pos > len(x) or not x.endswith(closer):
+            raise ValueError("expected string to end in closer")
+        return len(x) - len(closer)
+    else:
+        assert isinstance(closer, Pattern)
+        # now we have a problem, as the standard re module doesn't support reverse matches
+        closer_matches = closer.finditer(x, pos)
+        closer_match = None
+        for closer_match in closer_matches:  # noqa: B007
+            # we iterate to find the last match
+            pass
+        if not closer_match:
+            raise ValueError("expected string to end in closer")
+        else:
+            while closer_match.end() != len(x):
+                # finditer could have missed an overlapping match, if there is an overlapping match
+                # it will be found after the start of the last match (but before its end)
+                closer_match = closer.search(x, closer_match.start() + 1)
+                # if there is a match, it's an overlapping match, but it doesn't neccessarily end at
+                # the end of the string
+                if not closer_match:
+                    raise ValueError("expected string to end in closer")
+        return closer_match.start()
+
+
+def strip_opener_and_closer(x: str, opener: Pattern[str], closer: Needle) -> str:
+    start_idx = strip_opener_idx(x, opener)
+    end_idx = strip_closer_idx(x, closer, start_idx)
+
+    if start_idx != 0 or end_idx != len(x):
+        return x[start_idx:end_idx]
+    return x
+
+
+def value_parser_func(value_type: Union[ParserInput[V], Mapping[K, ParserInput[V]]]) -> Callable[[K], Parser[V]]:
+    if isinstance(value_type, Mapping):
+        value_parsers = {k: parser(v) for k, v in value_type.items()}
+
+        def get_value_parser(key: K) -> Parser[V]:
+            try:
+                return value_parsers[key]
+            except KeyError:
+                # in case the mapping has a default value or the like
+                return parser(value_type[key])
+    else:
+        _value_parser = parser(value_type)
+
+        def get_value_parser(key: K) -> Parser[V]:
+            return _value_parser
+
+    return get_value_parser
+
+
 class CollectionParser(Generic[G, E]):
     """
     A parser that splits a string by a delimiter, and parses each part individually.
     """
 
     def __init__(
         self,
         delimiter: Needle,
         inner_parser: ParserInput[E],
         output_type: Callable[[Iterator[E]], G] = list,  # type: ignore[assignment]
         opener: Needle = empty_pattern,
-        closer: Needle = empty_pattern,
+        closer: Needle = "",
         *,
         strip: bool = True,
     ):
-        """
-        :param delimiter: The delimiter to split by.
-        :param inner_parser: The inner parser to apply to each element.
-        :param output_type: The aggregator function of all the parsed elements.
-        :param opener: Optional opener that must be present at the start of the string.
-        :param closer: Optional closer that must be present at the end of the string.
-        """
         self.delimiter_pattern = needle_to_pattern(delimiter)
         self.inner_parser = parser(inner_parser)
         self.output_type = output_type
         self.opener_pattern = needle_to_pattern(opener)
-        self.closer_pattern = needle_to_pattern(closer)
+        self.closer = closer
         self.strip = strip
 
     def __call__(self, x: str) -> G:
-        opener_match = self.opener_pattern.match(x)
-        if not opener_match:
-            raise ValueError("position 0, expected opener")
-        x = x[opener_match.end() :]
-        raw_elements = self.delimiter_pattern.split(x)
-        closer_matches = self.closer_pattern.finditer(raw_elements[-1])
-
-        closer_match = None
-        for closer_match in closer_matches:  # noqa: B007
-            pass
-        if not closer_match:
-            raise ValueError("expected string to end in closer")
-        elif closer_match.end() != len(raw_elements[-1]):
-            raise ValueError(
-                "expected closer to match end of string, got unexpected suffix: "
-                + raw_elements[-1][closer_match.end() :]
-            )
-
-        raw_elements[-1] = raw_elements[-1][: closer_match.start()]
-        raw_items = iter(raw_elements)
+        x = strip_opener_and_closer(x, self.opener_pattern, self.closer)
+        raw_items = iter(self.delimiter_pattern.split(x))
         if self.strip:
             raw_items = (r.strip() for r in raw_items)
         elements = (self.inner_parser(r) for r in raw_items)
         return self.output_type(elements)
 
     @classmethod
     def pair_wise_delimited(
         cls,
         pair_delimiter: Needle,
         key_value_delimiter: Needle,
         key_type: ParserInput[K],
         value_type: Union[ParserInput[V], Mapping[K, ParserInput[V]]],
         output_type: Callable[[Iterator[Tuple[K, V]]], G] = _duplicate_avoiding_dict,  # type: ignore[assignment]
-        *,
         key_first: bool = True,
         strip_keys: bool = True,
         strip_values: bool = True,
         **kwargs: Any,
     ) -> Parser[G]:
-        """
-        Create a collectionParser that aggregates to key-value pairs.
-        :param pair_delimiter: The separator between different key-value pairs.
-        :param key_value_delimiter: The separator between each key and value.
-        :param key_type: The parser for key elements.
-        :param value_type: The parser for value elements. Can also be a mapping, parsing each key under a different
-         parser.
-        :param output_type: The tuple aggregator function. Defaults to a duplicate-checking dict.
-        :param key_first: If set to false, will evaluate the part behind the key-value separator as a value.
-        :param kwargs: forwarded to `CollectionParser.__init__`
-        """
         key_value_delimiter = needle_to_pattern(key_value_delimiter)
         key_parser = parser(key_type)
-        get_value_parser: Callable[[K], Parser]
-        if isinstance(value_type, Mapping):
-
-            @lru_cache(None)
-            def get_value_parser(key: K) -> Parser[V]:
-                return parser(value_type[key])
-        else:
-            _value_parser = parser(value_type)
-
-            def get_value_parser(key: K) -> Parser[V]:
-                return _value_parser
+        get_value_parser = value_parser_func(value_type)
 
         def combined_parser(s: str) -> Tuple[K, V]:
             split = key_value_delimiter.split(s, maxsplit=2)
             if len(split) != 2:
                 raise ValueError(f"expecting key-value pair, got {s}")
             k, v = split
             if not key_first:
@@ -246,14 +260,46 @@
             key = key_parser(k)
             value = get_value_parser(key)(v)
             return key, value
 
         return cls(pair_delimiter, combined_parser, output_type, **kwargs)  # type: ignore[arg-type]
 
 
+def find_iter_contingient(x: str, pattern: Pattern[str]) -> Iterator[re.Match[str]]:
+    start_idx = 0
+    while start_idx < len(x):
+        match = pattern.match(x, start_idx)
+        if match is None:
+            raise ValueError(f"could not match pattern {pattern} at position {start_idx}")
+        start_idx = match.end()
+        yield match
+
+
+class FindIterCollectionParser(Generic[G, E]):
+    def __init__(
+        self,
+        element_pattern: Pattern[str],
+        element_func: Callable[[re.Match[str]], E],
+        output_type: Callable[[Iterator[E]], G] = list,  # type: ignore[assignment]
+        opener: Needle = empty_pattern,
+        closer: Needle = "",
+    ):
+        self.prefix_pattern = element_pattern
+        self.element_func = element_func
+        self.output_type = output_type
+        self.opener_pattern = needle_to_pattern(opener)
+        self.closer = closer
+
+    def __call__(self, x: str) -> G:
+        x = strip_opener_and_closer(x, self.opener_pattern, self.closer)
+        raw_matches = find_iter_contingient(x, self.prefix_pattern)
+        elements = (self.element_func(r) for r in raw_matches)
+        return self.output_type(elements)
+
+
 class NoFallback(Enum):
     no_fallback = auto()
 
 
 no_fallback = NoFallback.no_fallback
 
 CasesInput = Union[Iterable[Tuple[Needle, T]], Mapping[str, T], Type[Enum]]
```

### Comparing `envolved-1.4.0/envolved/utils.py` & `envolved-1.5.0/envolved/utils.py`

 * *Files identical despite different names*

### Comparing `envolved-1.4.0/pyproject.toml` & `envolved-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [tool.poetry]
 name = "envolved"
-version = "1.4.0"
+version = "1.5.0"
 description = ""
 authors = ["ben avrahami <avrahami.ben@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bentheiii/envolved"
 packages = [
     {include="envolved"},
     {include="envolved/py.typed"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typing-extensions = [
-    {version="<4.8.0", python=">=3.7, <3.8"},
-    {version="*", python=">=3.8"},
-]
+python = "^3.8"
+typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 mypy = {version="*", python=">=3.8"} 
 pytest-cov = "^4.1.0"
 ruff = {version="*", python=">=3.8"} 
 pydantic = "^2.5.2"
@@ -35,15 +32,15 @@
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 output-format = "full"
 [tool.ruff.lint]
 exclude = ["docs/**"]
 # https://beta.ruff.rs/docs/rules/
 select = ["I", "E", "W", "F", "N", "S", "BLE", "COM", "C4", "ISC", "ICN", "G", "PIE", "T20", "PYI", "Q", "SLF", "SIM",
           "ERA", "PGH", "PLC", "PLE", "PLR", "PLW", "RUF", "PT", "UP", "B", "ANN", "ASYNC", "FBT003", "A", "INP",
@@ -104,7 +101,11 @@
     "B018",  # useless expression
     "FBT",  # boolean params
     "A",  # builtin shadowing
     "INP",  # implicit namespace packages
     "PTH",  # use pathlib
     "PERF",  # performance anti-patterns
 ]
+
+"type_checking/**" = [
+    "INP001",  # implicit namespace packages
+]
```

### Comparing `envolved-1.4.0/PKG-INFO` & `envolved-1.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: envolved
-Version: 1.4.0
+Version: 1.5.0
 Summary: 
 Home-page: https://github.com/bentheiii/envolved
 License: MIT
 Author: ben avrahami
 Author-email: avrahami.ben@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: typing-extensions (<4.8.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: typing-extensions ; python_version >= "3.8"
+Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/bentheiii/envolved
 Description-Content-Type: text/markdown
 
 # Envolved
 Envolved is a library to make environment variable parsing powerful and effortless.
 
 documentation: https://envolved.readthedocs.io/en/latest/
```

