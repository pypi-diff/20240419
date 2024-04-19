# Comparing `tmp/phtml5-0.0.0.tar.gz` & `tmp/phtml5-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phtml5-0.0.0.tar", last modified: Wed Mar  6 15:21:12 2024, max compression
+gzip compressed data, was "phtml5-1.0.0.tar", last modified: Fri Apr 19 18:11:36 2024, max compression
```

## Comparing `phtml5-0.0.0.tar` & `phtml5-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 15:21:12.920093 phtml5-0.0.0/
--rw-rw-rw-   0        0        0      292 2024-03-06 15:21:12.920597 phtml5-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-03-06 15:15:11.000000 phtml5-0.0.0/README.md
--rw-rw-rw-   0        0        0       99 2023-10-12 17:43:15.000000 phtml5-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      427 2024-03-06 15:21:12.920597 phtml5-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-05-25 14:43:52.000000 phtml5-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-06 15:21:12.911013 phtml5-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-06 15:21:12.915073 phtml5-0.0.0/src/phtml5/
--rw-rw-rw-   0        0        0      737 2024-03-06 14:57:00.000000 phtml5-0.0.0/src/phtml5/__init__.py
--rw-rw-rw-   0        0        0     1239 2024-03-06 14:10:24.000000 phtml5-0.0.0/src/phtml5/htmlelement.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:03:18.000000 phtml5-0.0.0/src/phtml5/py.typed
--rw-rw-rw-   0        0        0    35959 2024-03-06 14:57:13.000000 phtml5-0.0.0/src/phtml5/tags.py
-drwxrwxrwx   0        0        0        0 2024-03-06 15:21:12.919088 phtml5-0.0.0/src/phtml5.egg-info/
--rw-rw-rw-   0        0        0      292 2024-03-06 15:21:12.000000 phtml5-0.0.0/src/phtml5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-03-06 15:21:12.000000 phtml5-0.0.0/src/phtml5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 15:21:12.000000 phtml5-0.0.0/src/phtml5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-06 15:21:12.000000 phtml5-0.0.0/src/phtml5.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-03-06 15:21:12.000000 phtml5-0.0.0/src/phtml5.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 18:11:36.233531 phtml5-1.0.0/
+-rw-rw-rw-   0        0        0      292 2024-04-19 18:11:36.233531 phtml5-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2024-03-06 15:15:11.000000 phtml5-1.0.0/README.md
+-rw-rw-rw-   0        0        0       99 2023-10-12 17:43:15.000000 phtml5-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      444 2024-04-19 18:11:36.235073 phtml5-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-05-25 14:43:52.000000 phtml5-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 18:11:36.219685 phtml5-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 18:11:36.227412 phtml5-1.0.0/src/phtml5/
+-rw-rw-rw-   0        0        0     1448 2024-04-19 18:06:21.000000 phtml5-1.0.0/src/phtml5/__init__.py
+-rw-rw-rw-   0        0        0     1239 2024-03-06 14:10:24.000000 phtml5-1.0.0/src/phtml5/htmlelement.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:03:18.000000 phtml5-1.0.0/src/phtml5/py.typed
+-rw-rw-rw-   0        0        0    36403 2024-04-19 18:06:21.000000 phtml5-1.0.0/src/phtml5/tags.py
+drwxrwxrwx   0        0        0        0 2024-04-19 18:11:36.232530 phtml5-1.0.0/src/phtml5.egg-info/
+-rw-rw-rw-   0        0        0      292 2024-04-19 18:11:36.000000 phtml5-1.0.0/src/phtml5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-19 18:11:36.000000 phtml5-1.0.0/src/phtml5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 18:11:36.000000 phtml5-1.0.0/src/phtml5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 18:07:52.000000 phtml5-1.0.0/src/phtml5.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-04-19 18:11:36.000000 phtml5-1.0.0/src/phtml5.egg-info/top_level.txt
```

### Comparing `phtml5-0.0.0/README.md` & `phtml5-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `phtml5-0.0.0/src/phtml5/htmlelement.py` & `phtml5-1.0.0/src/phtml5/htmlelement.py`

 * *Files identical despite different names*

### Comparing `phtml5-0.0.0/src/phtml5/tags.py` & `phtml5-1.0.0/src/phtml5/tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 def style(_class: str | None = None, **kwargs: Any) -> Style:
     arguments = { 'class': _class }
     return Style('style', arguments | kwargs, [])
 
 class Summary(HTMLElement):
 
-    def __call__(self: Summary, *args: Phrasingcontent | Headingcontent | list[Phrasingcontent | Headingcontent]) -> Summary:
+    def __call__(self: Summary, *args: Phrasingcontent | Headingcontent | str | list[Phrasingcontent | Headingcontent | str]) -> Summary:
         return Summary(self._tag, self._attributes, self.get_children_from_args(args))
 
 def summary(_class: str | None = None, **kwargs: Any) -> Summary:
     arguments = { 'class': _class }
     return Summary('summary', arguments | kwargs, [])
 
 class Script(HTMLElement):
@@ -70,15 +70,15 @@
 
 def script(_class: str | None = None, **kwargs: Any) -> Script:
     arguments = { 'class': _class }
     return Script('script', arguments | kwargs, [])
 
 class Noscript(HTMLElement):
 
-    def __call__(self: Noscript, *args: Flowcontent | list[Flowcontent]) -> Noscript:
+    def __call__(self: Noscript, *args: Flowcontent | str | list[Flowcontent | str]) -> Noscript:
         return Noscript(self._tag, self._attributes, self.get_children_from_args(args))
 
 def noscript(_class: str | None = None, **kwargs: Any) -> Noscript:
     arguments = { 'class': _class }
     return Noscript('noscript', arguments | kwargs, [])
 
 class Body(HTMLElement):
@@ -106,15 +106,15 @@
 
 def nav(_class: str | None = None, **kwargs: Any) -> Nav:
     arguments = { 'class': _class }
     return Nav('nav', arguments | kwargs, [])
 
 class Article(HTMLElement):
 
-    def __call__(self: Article, *args: Flowcontent | list[Flowcontent]) -> Article:
+    def __call__(self: Article, *args: Flowcontent | str | list[Flowcontent | str]) -> Article:
         return Article(self._tag, self._attributes, self.get_children_from_args(args))
 
 def article(_class: str | None = None, **kwargs: Any) -> Article:
     arguments = { 'class': _class }
     return Article('article', arguments | kwargs, [])
 
 class Aside(HTMLElement):
@@ -124,60 +124,60 @@
 
 def aside(_class: str | None = None, **kwargs: Any) -> Aside:
     arguments = { 'class': _class }
     return Aside('aside', arguments | kwargs, [])
 
 class H1(HTMLElement):
 
-    def __call__(self: H1, *args: Phrasingcontent | list[Phrasingcontent]) -> H1:
+    def __call__(self: H1, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> H1:
         return H1(self._tag, self._attributes, self.get_children_from_args(args))
 
 def h1(_class: str | None = None, **kwargs: Any) -> H1:
     arguments = { 'class': _class }
     return H1('h1', arguments | kwargs, [])
 
 class H2(HTMLElement):
 
-    def __call__(self: H2, *args: Phrasingcontent | list[Phrasingcontent]) -> H2:
+    def __call__(self: H2, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> H2:
         return H2(self._tag, self._attributes, self.get_children_from_args(args))
 
 def h2(_class: str | None = None, **kwargs: Any) -> H2:
     arguments = { 'class': _class }
     return H2('h2', arguments | kwargs, [])
 
 class H3(HTMLElement):
 
-    def __call__(self: H3, *args: Phrasingcontent | list[Phrasingcontent]) -> H3:
+    def __call__(self: H3, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> H3:
         return H3(self._tag, self._attributes, self.get_children_from_args(args))
 
 def h3(_class: str | None = None, **kwargs: Any) -> H3:
     arguments = { 'class': _class }
     return H3('h3', arguments | kwargs, [])
 
 class H4(HTMLElement):
 
-    def __call__(self: H4, *args: Phrasingcontent | list[Phrasingcontent]) -> H4:
+    def __call__(self: H4, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> H4:
         return H4(self._tag, self._attributes, self.get_children_from_args(args))
 
 def h4(_class: str | None = None, **kwargs: Any) -> H4:
     arguments = { 'class': _class }
     return H4('h4', arguments | kwargs, [])
 
 class H5(HTMLElement):
 
-    def __call__(self: H5, *args: Phrasingcontent | list[Phrasingcontent]) -> H5:
+    def __call__(self: H5, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> H5:
         return H5(self._tag, self._attributes, self.get_children_from_args(args))
 
 def h5(_class: str | None = None, **kwargs: Any) -> H5:
     arguments = { 'class': _class }
     return H5('h5', arguments | kwargs, [])
 
 class H6(HTMLElement):
 
-    def __call__(self: H6, *args: Phrasingcontent | list[Phrasingcontent]) -> H6:
+    def __call__(self: H6, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> H6:
         return H6(self._tag, self._attributes, self.get_children_from_args(args))
 
 def h6(_class: str | None = None, **kwargs: Any) -> H6:
     arguments = { 'class': _class }
     return H6('h6', arguments | kwargs, [])
 
 class Hgroup(HTMLElement):
@@ -214,15 +214,15 @@
 
 def address(_class: str | None = None, **kwargs: Any) -> Address:
     arguments = { 'class': _class }
     return Address('address', arguments | kwargs, [])
 
 class P(HTMLElement):
 
-    def __call__(self: P, *args: Phrasingcontent | list[Phrasingcontent]) -> P:
+    def __call__(self: P, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> P:
         return P(self._tag, self._attributes, self.get_children_from_args(args))
 
 def p(_class: str | None = None, **kwargs: Any) -> P:
     arguments = { 'class': _class }
     return P('p', arguments | kwargs, [])
 
 class Br(HTMLElement):
@@ -230,15 +230,15 @@
 
 def br(_class: str | None = None, **kwargs: Any) -> Br:
     arguments = { 'class': _class }
     return Br('br', arguments | kwargs, [])
 
 class Pre(HTMLElement):
 
-    def __call__(self: Pre, *args: Phrasingcontent | list[Phrasingcontent]) -> Pre:
+    def __call__(self: Pre, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Pre:
         return Pre(self._tag, self._attributes, self.get_children_from_args(args))
 
 def pre(_class: str | None = None, **kwargs: Any) -> Pre:
     arguments = { 'class': _class }
     return Pre('pre', arguments | kwargs, [])
 
 class Dialog(HTMLElement):
@@ -248,15 +248,15 @@
 
 def dialog(_class: str | None = None, **kwargs: Any) -> Dialog:
     arguments = { 'class': _class }
     return Dialog('dialog', arguments | kwargs, [])
 
 class Blockquote(HTMLElement):
 
-    def __call__(self: Blockquote, *args: Flowcontent | list[Flowcontent]) -> Blockquote:
+    def __call__(self: Blockquote, *args: Flowcontent | str | list[Flowcontent | str]) -> Blockquote:
         return Blockquote(self._tag, self._attributes, self.get_children_from_args(args))
 
 def blockquote(_class: str | None = None, **kwargs: Any) -> Blockquote:
     arguments = { 'class': _class }
     return Blockquote('blockquote', arguments | kwargs, [])
 
 class Ol(HTMLElement):
@@ -275,15 +275,15 @@
 
 def ul(_class: str | None = None, **kwargs: Any) -> Ul:
     arguments = { 'class': _class }
     return Ul('ul', arguments | kwargs, [])
 
 class Li(HTMLElement):
 
-    def __call__(self: Li, *args: Flowcontent | list[Flowcontent]) -> Li:
+    def __call__(self: Li, *args: Flowcontent | str | list[Flowcontent | str]) -> Li:
         return Li(self._tag, self._attributes, self.get_children_from_args(args))
 
 def li(_class: str | None = None, **kwargs: Any) -> Li:
     arguments = { 'class': _class }
     return Li('li', arguments | kwargs, [])
 
 class Dl(HTMLElement):
@@ -293,33 +293,33 @@
 
 def dl(_class: str | None = None, **kwargs: Any) -> Dl:
     arguments = { 'class': _class }
     return Dl('dl', arguments | kwargs, [])
 
 class Dt(HTMLElement):
 
-    def __call__(self: Dt, *args: Phrasingcontent | list[Phrasingcontent]) -> Dt:
+    def __call__(self: Dt, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Dt:
         return Dt(self._tag, self._attributes, self.get_children_from_args(args))
 
 def dt(_class: str | None = None, **kwargs: Any) -> Dt:
     arguments = { 'class': _class }
     return Dt('dt', arguments | kwargs, [])
 
 class Dd(HTMLElement):
 
-    def __call__(self: Dd, *args: Flowcontent | list[Flowcontent]) -> Dd:
+    def __call__(self: Dd, *args: Flowcontent | str | list[Flowcontent | str]) -> Dd:
         return Dd(self._tag, self._attributes, self.get_children_from_args(args))
 
 def dd(_class: str | None = None, **kwargs: Any) -> Dd:
     arguments = { 'class': _class }
     return Dd('dd', arguments | kwargs, [])
 
 class A(HTMLElement):
 
-    def __call__(self: A, *args: Flowcontent | list[Flowcontent]) -> A:
+    def __call__(self: A, *args: Flowcontent | str | list[Flowcontent | str]) -> A:
         return A(self._tag, self._attributes, self.get_children_from_args(args))
 
 def a(_class: str | None = None, **kwargs: Any) -> A:
     arguments = { 'class': _class }
     return A('a', arguments | kwargs, [])
 
 class Em(HTMLElement):
@@ -356,15 +356,15 @@
 
 def cite(_class: str | None = None, **kwargs: Any) -> Cite:
     arguments = { 'class': _class }
     return Cite('cite', arguments | kwargs, [])
 
 class Q(HTMLElement):
 
-    def __call__(self: Q, *args: Phrasingcontent | list[Phrasingcontent]) -> Q:
+    def __call__(self: Q, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Q:
         return Q(self._tag, self._attributes, self.get_children_from_args(args))
 
 def q(_class: str | None = None, **kwargs: Any) -> Q:
     arguments = { 'class': _class }
     return Q('q', arguments | kwargs, [])
 
 class Dfn(HTMLElement):
@@ -446,15 +446,15 @@
 
 def i(_class: str | None = None, **kwargs: Any) -> I:
     arguments = { 'class': _class }
     return I('i', arguments | kwargs, [])
 
 class B(HTMLElement):
 
-    def __call__(self: B, *args: Phrasingcontent | list[Phrasingcontent]) -> B:
+    def __call__(self: B, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> B:
         return B(self._tag, self._attributes, self.get_children_from_args(args))
 
 def b(_class: str | None = None, **kwargs: Any) -> B:
     arguments = { 'class': _class }
     return B('b', arguments | kwargs, [])
 
 class Main(HTMLElement):
@@ -489,33 +489,33 @@
 
 def progress(_class: str | None = None, **kwargs: Any) -> Progress:
     arguments = { 'class': _class }
     return Progress('progress', arguments | kwargs, [])
 
 class Meter(HTMLElement):
 
-    def __call__(self: Meter, *args: Phrasingcontent | list[Phrasingcontent]) -> Meter:
+    def __call__(self: Meter, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Meter:
         return Meter(self._tag, self._attributes, self.get_children_from_args(args))
 
 def meter(_class: str | None = None, **kwargs: Any) -> Meter:
     arguments = { 'class': _class }
     return Meter('meter', arguments | kwargs, [])
 
 class Time(HTMLElement):
 
-    def __call__(self: Time, *args: Phrasingcontent | list[Phrasingcontent]) -> Time:
+    def __call__(self: Time, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Time:
         return Time(self._tag, self._attributes, self.get_children_from_args(args))
 
 def time(_class: str | None = None, **kwargs: Any) -> Time:
     arguments = { 'class': _class }
     return Time('time', arguments | kwargs, [])
 
 class Ruby(HTMLElement):
 
-    def __call__(self: Ruby, *args: Phrasingcontent | Rt | Rp | list[Phrasingcontent | Rt | Rp]) -> Ruby:
+    def __call__(self: Ruby, *args: Phrasingcontent | Rt | Rp | str | list[Phrasingcontent | Rt | Rp | str]) -> Ruby:
         return Ruby(self._tag, self._attributes, self.get_children_from_args(args))
 
 def ruby(_class: str | None = None, **kwargs: Any) -> Ruby:
     arguments = { 'class': _class }
     return Ruby('ruby', arguments | kwargs, [])
 
 class Rt(HTMLElement):
@@ -552,42 +552,42 @@
 
 def bdo(_class: str | None = None, **kwargs: Any) -> Bdo:
     arguments = { 'class': _class }
     return Bdo('bdo', arguments | kwargs, [])
 
 class Span(HTMLElement):
 
-    def __call__(self: Span, *args: Phrasingcontent | list[Phrasingcontent]) -> Span:
+    def __call__(self: Span, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Span:
         return Span(self._tag, self._attributes, self.get_children_from_args(args))
 
 def span(_class: str | None = None, **kwargs: Any) -> Span:
     arguments = { 'class': _class }
     return Span('span', arguments | kwargs, [])
 
 class Ins(HTMLElement):
 
-    def __call__(self: Ins, *args: Phrasingcontent | list[Phrasingcontent]) -> Ins:
+    def __call__(self: Ins, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Ins:
         return Ins(self._tag, self._attributes, self.get_children_from_args(args))
 
 def ins(_class: str | None = None, **kwargs: Any) -> Ins:
     arguments = { 'class': _class }
     return Ins('ins', arguments | kwargs, [])
 
 class Figure(HTMLElement):
 
-    def __call__(self: Figure, *args: Flowcontent | Legend | Figcaption | list[Flowcontent | Legend | Figcaption]) -> Figure:
+    def __call__(self: Figure, *args: Flowcontent | Legend | Figcaption | str | list[Flowcontent | Legend | Figcaption | str]) -> Figure:
         return Figure(self._tag, self._attributes, self.get_children_from_args(args))
 
 def figure(_class: str | None = None, **kwargs: Any) -> Figure:
     arguments = { 'class': _class }
     return Figure('figure', arguments | kwargs, [])
 
 class Figcaption(HTMLElement):
 
-    def __call__(self: Figcaption, *args: Flowcontent | list[Flowcontent]) -> Figcaption:
+    def __call__(self: Figcaption, *args: Flowcontent | str | list[Flowcontent | str]) -> Figcaption:
         return Figcaption(self._tag, self._attributes, self.get_children_from_args(args))
 
 def figcaption(_class: str | None = None, **kwargs: Any) -> Figcaption:
     arguments = { 'class': _class }
     return Figcaption('figcaption', arguments | kwargs, [])
 
 class Img(HTMLElement):
@@ -618,15 +618,15 @@
 
 def embed(_class: str | None = None, **kwargs: Any) -> Embed:
     arguments = { 'class': _class }
     return Embed('embed', arguments | kwargs, [])
 
 class Object(HTMLElement):
 
-    def __call__(self: Object, *args: Param | list[Param]) -> Object:
+    def __call__(self: Object, *args: Param | str | list[Param | str]) -> Object:
         return Object(self._tag, self._attributes, self.get_children_from_args(args))
 
 def object(_class: str | None = None, **kwargs: Any) -> Object:
     arguments = { 'class': _class }
     return Object('object', arguments | kwargs, [])
 
 class Param(HTMLElement):
@@ -634,15 +634,15 @@
 
 def param(_class: str | None = None, **kwargs: Any) -> Param:
     arguments = { 'class': _class }
     return Param('param', arguments | kwargs, [])
 
 class Details(HTMLElement):
 
-    def __call__(self: Details, *args: Legend | Flowcontent | list[Legend | Flowcontent]) -> Details:
+    def __call__(self: Details, *args: Legend | Flowcontent | str | list[Legend | Flowcontent | str]) -> Details:
         return Details(self._tag, self._attributes, self.get_children_from_args(args))
 
 def details(_class: str | None = None, **kwargs: Any) -> Details:
     arguments = { 'class': _class }
     return Details('details', arguments | kwargs, [])
 
 class Command(HTMLElement):
@@ -659,15 +659,15 @@
 
 def menu(_class: str | None = None, **kwargs: Any) -> Menu:
     arguments = { 'class': _class }
     return Menu('menu', arguments | kwargs, [])
 
 class Legend(HTMLElement):
 
-    def __call__(self: Legend, *args: Flowcontent | Phrasingcontent | list[Flowcontent | Phrasingcontent]) -> Legend:
+    def __call__(self: Legend, *args: Flowcontent | Phrasingcontent | str | list[Flowcontent | Phrasingcontent | str]) -> Legend:
         return Legend(self._tag, self._attributes, self.get_children_from_args(args))
 
 def legend(_class: str | None = None, **kwargs: Any) -> Legend:
     arguments = { 'class': _class }
     return Legend('legend', arguments | kwargs, [])
 
 class Div(HTMLElement):
@@ -684,24 +684,24 @@
 
 def source(_class: str | None = None, **kwargs: Any) -> Source:
     arguments = { 'class': _class }
     return Source('source', arguments | kwargs, [])
 
 class Audio(HTMLElement):
 
-    def __call__(self: Audio, *args: Source | list[Source]) -> Audio:
+    def __call__(self: Audio, *args: Source | str | list[Source | str]) -> Audio:
         return Audio(self._tag, self._attributes, self.get_children_from_args(args))
 
 def audio(_class: str | None = None, **kwargs: Any) -> Audio:
     arguments = { 'class': _class }
     return Audio('audio', arguments | kwargs, [])
 
 class Video(HTMLElement):
 
-    def __call__(self: Video, *args: Source | list[Source]) -> Video:
+    def __call__(self: Video, *args: Source | str | list[Source | str]) -> Video:
         return Video(self._tag, self._attributes, self.get_children_from_args(args))
 
 def video(_class: str | None = None, **kwargs: Any) -> Video:
     arguments = { 'class': _class }
     return Video('video', arguments | kwargs, [])
 
 class Hr(HTMLElement):
@@ -709,33 +709,33 @@
 
 def hr(_class: str | None = None, **kwargs: Any) -> Hr:
     arguments = { 'class': _class }
     return Hr('hr', arguments | kwargs, [])
 
 class Form(HTMLElement):
 
-    def __call__(self: Form, *args: Flowcontent | list[Flowcontent]) -> Form:
+    def __call__(self: Form, *args: Flowcontent | str | list[Flowcontent | str]) -> Form:
         return Form(self._tag, self._attributes, self.get_children_from_args(args))
 
 def form(_class: str | None = None, **kwargs: Any) -> Form:
     arguments = { 'class': _class }
     return Form('form', arguments | kwargs, [])
 
 class Fieldset(HTMLElement):
 
-    def __call__(self: Fieldset, *args: Legend | Flowcontent | list[Legend | Flowcontent]) -> Fieldset:
+    def __call__(self: Fieldset, *args: Legend | Flowcontent | str | list[Legend | Flowcontent | str]) -> Fieldset:
         return Fieldset(self._tag, self._attributes, self.get_children_from_args(args))
 
 def fieldset(_class: str | None = None, **kwargs: Any) -> Fieldset:
     arguments = { 'class': _class }
     return Fieldset('fieldset', arguments | kwargs, [])
 
 class Label(HTMLElement):
 
-    def __call__(self: Label, *args: Phrasingcontent | list[Phrasingcontent]) -> Label:
+    def __call__(self: Label, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Label:
         return Label(self._tag, self._attributes, self.get_children_from_args(args))
 
 def label(_class: str | None = None, **kwargs: Any) -> Label:
     arguments = { 'class': _class }
     return Label('label', arguments | kwargs, [])
 
 class Input(HTMLElement):
@@ -743,15 +743,15 @@
 
 def input(_class: str | None = None, **kwargs: Any) -> Input:
     arguments = { 'class': _class }
     return Input('input', arguments | kwargs, [])
 
 class Button(HTMLElement):
 
-    def __call__(self: Button, *args: Phrasingcontent | list[Phrasingcontent]) -> Button:
+    def __call__(self: Button, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Button:
         return Button(self._tag, self._attributes, self.get_children_from_args(args))
 
 def button(_class: str | None = None, **kwargs: Any) -> Button:
     arguments = { 'class': _class }
     return Button('button', arguments | kwargs, [])
 
 class Select(HTMLElement):
@@ -800,15 +800,15 @@
 
 def keygen(_class: str | None = None, **kwargs: Any) -> Keygen:
     arguments = { 'class': _class }
     return Keygen('keygen', arguments | kwargs, [])
 
 class Output(HTMLElement):
 
-    def __call__(self: Output, *args: Phrasingcontent | list[Phrasingcontent]) -> Output:
+    def __call__(self: Output, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Output:
         return Output(self._tag, self._attributes, self.get_children_from_args(args))
 
 def output(_class: str | None = None, **kwargs: Any) -> Output:
     arguments = { 'class': _class }
     return Output('output', arguments | kwargs, [])
 
 class Canvas(HTMLElement):
@@ -916,24 +916,24 @@
 
 def tr(_class: str | None = None, **kwargs: Any) -> Tr:
     arguments = { 'class': _class }
     return Tr('tr', arguments | kwargs, [])
 
 class Th(HTMLElement):
 
-    def __call__(self: Th, *args: Phrasingcontent | list[Phrasingcontent]) -> Th:
+    def __call__(self: Th, *args: Phrasingcontent | str | list[Phrasingcontent | str]) -> Th:
         return Th(self._tag, self._attributes, self.get_children_from_args(args))
 
 def th(_class: str | None = None, **kwargs: Any) -> Th:
     arguments = { 'class': _class }
     return Th('th', arguments | kwargs, [])
 
 class Td(HTMLElement):
 
-    def __call__(self: Td, *args: Flowcontent | list[Flowcontent]) -> Td:
+    def __call__(self: Td, *args: Flowcontent | str | list[Flowcontent | str]) -> Td:
         return Td(self._tag, self._attributes, self.get_children_from_args(args))
 
 def td(_class: str | None = None, **kwargs: Any) -> Td:
     arguments = { 'class': _class }
     return Td('td', arguments | kwargs, [])
 
 Metadatacontent = Base | Command | Link | Meta | Noscript | Script | Style | Title
```

