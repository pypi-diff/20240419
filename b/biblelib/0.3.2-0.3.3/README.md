# Comparing `tmp/biblelib-0.3.2.tar.gz` & `tmp/biblelib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.3.2.tar", max compression
+gzip compressed data, was "biblelib-0.3.3.tar", max compression
```

## Comparing `biblelib-0.3.2.tar` & `biblelib-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.2/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.2/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.2/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.2/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.2/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.2/biblelib/book/__init__.py
--rw-r--r--   0        0        0    14365 2024-02-22 22:47:18.883690 biblelib-0.3.2/biblelib/book/book.py
--rw-r--r--   0        0        0     4746 2023-07-29 01:03:41.398182 biblelib-0.3.2/biblelib/book/books.tsv
--rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.2/biblelib/sources.py
--rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.2/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5834 2024-02-02 00:49:16.545913 biblelib-0.3.2/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.2/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     7217 2024-02-02 00:50:41.685079 biblelib-0.3.2/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.2/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.2/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.2/biblelib/unit/pericope.py
--rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.2/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.2/biblelib/unit/unit.py
--rw-r--r--   0        0        0     5179 2024-02-21 01:50:22.890112 biblelib-0.3.2/biblelib/unit/unitrange.py
--rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.2/biblelib/unit/verse.py
--rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.2/biblelib/versification/Enumerator.py
--rw-r--r--   0        0        0     1443 2024-03-14 22:13:58.993984 biblelib-0.3.2/biblelib/versification/Mapper.py
--rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.2/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0     1733 2024-03-11 19:05:21.601106 biblelib-0.3.2/biblelib/versification/VrefReader.py
--rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.2/biblelib/versification/__init__.py
--rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.2/biblelib/versification/eng-nt-vref.txt
--rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.2/biblelib/versification/eng-ot-vref.txt
--rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.2/biblelib/versification/eng-protestant-vref.txt
--rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.2/biblelib/versification/org-nt-vref.txt
--rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.2/biblelib/versification/org-ot-vref.txt
--rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.2/biblelib/versification/org-protestant-vref.txt
--rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.2/biblelib/versification/rso-nt-vref.txt
--rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.2/biblelib/versification/rso-ot-vref.txt
--rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.2/biblelib/versification/rso-protestant-vref.txt
--rw-r--r--   0        0        0      959 2024-03-14 17:56:36.859595 biblelib-0.3.2/biblelib/word/__init__.py
--rw-r--r--   0        0        0    22893 2024-03-14 19:40:11.109037 biblelib-0.3.2/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.3.2/biblelib/word/mappings.py
--rw-r--r--   0        0        0     1300 2024-03-14 22:18:40.721545 biblelib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.3/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.3/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.3/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.3/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.3/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.3/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.3/biblelib/book/book.py
+-rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.3/biblelib/book/books.tsv
+-rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.3/biblelib/sources.py
+-rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.3/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5834 2024-02-02 00:49:16.545913 biblelib-0.3.3/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.3/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     7217 2024-02-02 00:50:41.685079 biblelib-0.3.3/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.3/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.3/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.3/biblelib/unit/pericope.py
+-rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.3/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.3/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     5945 2024-04-19 20:18:36.271104 biblelib-0.3.3/biblelib/unit/unitrange.py
+-rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.3/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.3/biblelib/versification/Enumerator.py
+-rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.3/biblelib/versification/Mapper.py
+-rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.3/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.3/biblelib/versification/VrefReader.py
+-rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.3/biblelib/versification/__init__.py
+-rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.3/biblelib/versification/eng-nt-vref.txt
+-rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.3/biblelib/versification/eng-ot-vref.txt
+-rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.3/biblelib/versification/eng-protestant-vref.txt
+-rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.3/biblelib/versification/org-nt-vref.txt
+-rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.3/biblelib/versification/org-ot-vref.txt
+-rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.3/biblelib/versification/org-protestant-vref.txt
+-rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.3/biblelib/versification/rso-nt-vref.txt
+-rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.3/biblelib/versification/rso-ot-vref.txt
+-rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.3/biblelib/versification/rso-protestant-vref.txt
+-rw-r--r--   0        0        0      959 2024-03-14 17:56:36.859595 biblelib-0.3.3/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    22893 2024-04-18 23:52:17.261353 biblelib-0.3.3/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.3.3/biblelib/word/mappings.py
+-rw-r--r--   0        0        0     1324 2024-04-19 20:25:13.001522 biblelib-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.3/PKG-INFO
```

### Comparing `biblelib-0.3.2/LICENSE.md` & `biblelib-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/LICENSE.md~` & `biblelib-0.3.3/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/README.md` & `biblelib-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/book/ReadMe.md` & `biblelib-0.3.3/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/book/book.py` & `biblelib-0.3.3/biblelib/book/book.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """
 
 from collections import UserDict
 from csv import DictReader
 from dataclasses import dataclass, field
 from pathlib import Path
 import re
-from typing import Union
+from typing import Any, Union
 
 
 # This directory: where books.tsv is also located.
 BOOKSPATH = Path(__file__).parent
 
 
 @dataclass
@@ -60,14 +60,15 @@
         logosID (int): the index number of this book in the Logos
             bible datatype. Provides a standard ordinal index for
             ordering.
         usfmnumber (str): the USFM string for this book. 1-2
             characters: single-digit strings are not zero-padded.
         usfmname (str): the three-character USFM name for this book
         osisID (str): the OSIS identifier for this book
+        biblia (str): biblia.com abbreviaton for this book
         name (str): the common English name for this book
         altname (str): a longer or alternate English name, or empty string
 
     Todo:
         Add canon information.
 
     """
@@ -76,14 +77,15 @@
     # first to support ordinal sorting
     logosID: int
     # despite the name, this is a 1-2 character string
     usfmnumber: str
     # three characters
     usfmname: str
     osisID: str
+    biblia: str
     name: str
     altname: str = ""
     _canon_traditions: tuple = ("Catholic", "Jewish", "Protestant")
     # keep this in sync with the attributes below
     _fieldnames: tuple = ("logosID", "usfmnumber", "usfmname", "osisID", "name", "altname")
     # canon-specific
     ordinal: int = field(init=False)
@@ -98,33 +100,33 @@
         """Return a hash code.
 
         Instances are populated with static data, so they're
         functionally immutable (but don't change attribute values!).
         """
         return hash(self.osisID)
 
-    def __eq__(self, o) -> bool:
+    def __eq__(self, o: Any) -> bool:
         """Return True if self is == to other, else False, based on ordinals."""
-        return self.ordinal == o.ordinal
+        return bool(self.ordinal == o.ordinal)
 
-    def __ge__(self, o) -> bool:
+    def __ge__(self, o: Any) -> bool:
         """Return True if self is >= other, else False, based on ordinals."""
-        return self.ordinal >= o.ordinal
+        return bool(self.ordinal >= o.ordinal)
 
-    def __gt__(self, o) -> bool:
+    def __gt__(self, o: Any) -> bool:
         """Return True if self is > other, else False, based on ordinals."""
-        return self.ordinal > o.ordinal
+        return bool(self.ordinal > o.ordinal)
 
-    def __le__(self, o) -> bool:
+    def __le__(self, o: Any) -> bool:
         """Return True if self is <= other, else False, based on ordinals."""
-        return self.ordinal <= o.ordinal
+        return bool(self.ordinal <= o.ordinal)
 
-    def __lt__(self, o) -> bool:
+    def __lt__(self, o: Any) -> bool:
         """Return True if self is < other, else False, based on ordinals."""
-        return self.ordinal < o.ordinal
+        return bool(self.ordinal < o.ordinal)
 
     @property
     def usfmnumberalt(self) -> str:
         """Return an alternate USFM number, based on Matt="41" rather than "40".
 
         In some filenames associated with Paratext and legacy data,
         Matt is "41" and subsequent book numbers are one higher,
@@ -166,14 +168,24 @@
 
         Example:
             >>> Books()["MRK"].logosURI
             'https://ref.ly/logosref/bible.62'
         """
         return f"https://ref.ly/logosref/{self.render('logosID')}"
 
+    @property
+    def bibliaURI(self) -> str:
+        """Return a URI to open this book at biblia.com.
+
+        Example:
+            >>> Books()["MRK"].logosURI
+            'https://biblia.com/books/nrsv/Mk'
+        """
+        return f"https://biblia.com/books/nrsv/{self.render('biblia')}"
+
     # other URIs to consider
     # YouVersion
     # Bible Gateway
     # Ref.ly? Different Bible book abbreviations, not sure how important
 
 
 class Books(UserDict):
@@ -186,14 +198,15 @@
     source: Path = BOOKSPATH / "books.tsv"
     mappingfields: set = set(Book._fieldnames)
     canon: str = "Protestant"
     logosmap: dict = {}
     namemap: dict = {}
     nameregexp: re.Pattern = re.compile("")
     osismap: dict = {}
+    bibliamap: dict = {}
     usfmnumbermap: dict = {}
     # some minor standardization: this is not an extensible approach,
     # and long form names should use a different approach
     quickfixes = {"Psalm": "Psalms", "Song of Solomon": "Song of Songs"}
 
     def __init__(self, sourcefile: str = "", canon: str = "Protestant") -> None:
         """Initialize a Books instance.
@@ -260,28 +273,30 @@
                 logosID = int(logosID[6:])
             else:
                 logosID = int(logosID)
         if not self.logosmap:
             # initialize on demand
             self.logosmap = {b.logosID: b for _, b in self.data.items()}
         assert logosID in self.logosmap, f"Invalid logosID {logosID}"
-        return self.logosmap[logosID]
+        bookinst: Book = self.logosmap[logosID]
+        return bookinst
 
     def fromname(self, bookname: str) -> Book:
         """Return the book instance for a book name.
 
         Args:
             bookname: the full name  to use in looking up the Book,
                 like "Matthew".
         """
         # some minor standardization: this is not an extensible
         # approach, and long form names should use a different
         # approach
         bookname = self.quickfixes.get(bookname, bookname)
-        return self.namemap[bookname]
+        bookinst: Book = self.namemap[bookname]
+        return bookinst
 
     def _ensure_osismap(self) -> dict[str, str]:
         """Generate the OSIS map if needed."""
         if not self.osismap:
             # initialize on demand
             self.osismap = {b.osisID: b for _, b in self.data.items()}
         return self.osismap
@@ -290,15 +305,34 @@
         """Return the book instance for an OSIS identifier.
 
         Args:
             osisID: the OSIS identifier to use in looking up the Book,
                 like "Matt".
         """
         self._ensure_osismap()
-        return self.osismap[osisID]
+        bookinst: Book = self.osismap[osisID]
+        return bookinst
+
+    def _ensure_bibliamap(self) -> dict[str, str]:
+        """Generate the Biblia map if needed."""
+        if not self.bibliamap:
+            # initialize on demand
+            self.bibliamap = {b.biblia: b for _, b in self.data.items()}
+        return self.bibliamap
+
+    def frombiblia(self, biblia: str) -> Book:
+        """Return the book instance for a Biblia identifier.
+
+        Args:
+            biblia: the Biblia identifier to use in looking up the Book,
+                like "Matt".
+        """
+        self._ensure_bibliamap()
+        bookinst: Book = self.bibliamap[biblia]
+        return bookinst
 
     def fromusfmnumber(self, usfmnumber: str, legacynumbering: bool = False) -> Book:
         """Return the book instance for a USFM number.
 
         Args:
             usfmnumber: the USFM book number to use in looking up the Book,
                 like "40".
```

### Comparing `biblelib-0.3.2/biblelib/book/books.tsv` & `biblelib-0.3.3/biblelib/book/books.tsv`

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,121 @@
-logosID	usfmnumber	usfmname	osisID	name	altname
-1	1	GEN	Gen	Genesis
-2	2	EXO	Exod	Exodus
-3	3	LEV	Lev	Leviticus
-4	4	NUM	Num	Numbers
-5	5	DEU	Deut	Deuteronomy
-6	6	JOS	Josh	Joshua
-7	7	JDG	Judg	Judges
-8	8	RUT	Ruth	Ruth
-9	9	1SA	1Sam	1 Samuel
-10	10	2SA	2Sam	2 Samuel
-11	11	1KI	1Kgs	1 Kings
-12	12	2KI	2Kgs	2 Kings
-13	13	1CH	1Chr	1 Chronicles
-14	14	2CH	2Chr	2 Chronicles
-15	15	EZR	Ezra	Ezra
-16	16	NEH	Neh	Nehemiah
-17	17	EST	Esth	Esther
-18	18	JOB	Job	Job
-19	19	PSA	Ps	Psalms
-20	20	PRO	Prov	Proverbs
-21	21	ECC	Eccl	Ecclesiastes
-22	22	SNG	Song	Song of Songs	Song of Solomon
-23	23	ISA	Isa	Isaiah
-24	24	JER	Jer	Jeremiah
-25	25	LAM	Lam	Lamentations	The Lamentations of Jeremiah
-26	26	EZK	Ezek	Ezekiel
-27	27	DAN	Dan	Daniel
-28	28	HOS	Hos	Hosea
-29	29	JOL	Joel	Joel
-30	30	AMO	Amos	Amos
-31	31	OBA	Obad	Obadiah
-32	32	JON	Jonah	Jonah
-33	33	MIC	Mic	Micah
-34	34	NAM	Nah	Nahum
-35	35	HAB	Hab	Habakkuk
-36	36	ZEP	Zeph	Zephaniah
-37	37	HAG	Hag	Haggai
-38	38	ZEC	Zech	Zechariah
-39	39	MAL	Mal	Malachi
+logosID	usfmnumber	usfmname	osisID	biblia	name	altname
+1	1	GEN	Gen	Ge	Genesis
+2	2	EXO	Exod	Ex	Exodus
+3	3	LEV	Lev	Le	Leviticus
+4	4	NUM	Num	Nu	Numbers
+5	5	DEU	Deut	Dt	Deuteronomy
+6	6	JOS	Josh	Jos	Joshua
+7	7	JDG	Judg	Jdg	Judges
+8	8	RUT	Ruth	Ru	Ruth
+9	9	1SA	1Sam	1Sa	1 Samuel
+10	10	2SA	2Sam	2Sa	2 Samuel
+11	11	1KI	1Kgs	1Ki	1 Kings
+12	12	2KI	2Kgs	2Ki	2 Kings
+13	13	1CH	1Chr	1Ch	1 Chronicles
+14	14	2CH	2Chr	2Ch	2 Chronicles
+15	15	EZR	Ezra	Ezr	Ezra
+16	16	NEH	Neh	Ne	Nehemiah
+17	17	EST	Esth	Es	Esther
+18	18	JOB	Job	Job	Job
+19	19	PSA	Ps	Ps	Psalms
+20	20	PRO	Prov	Pr	Proverbs
+21	21	ECC	Eccl	Ec	Ecclesiastes
+22	22	SNG	Song	So	Song of Songs	Song of Solomon
+23	23	ISA	Isa	Is	Isaiah
+24	24	JER	Jer	Je	Jeremiah
+25	25	LAM	Lam	La	Lamentations	The Lamentations of Jeremiah
+26	26	EZK	Ezek	Eze	Ezekiel
+27	27	DAN	Dan	Da	Daniel
+28	28	HOS	Hos	Ho	Hosea
+29	29	JOL	Joel	Joe	Joel
+30	30	AMO	Amos	Am	Amos
+31	31	OBA	Obad	Ob	Obadiah
+32	32	JON	Jonah	Jon	Jonah
+33	33	MIC	Mic	Mic	Micah
+34	34	NAM	Nah	Na	Nahum
+35	35	HAB	Hab	Hab	Habakkuk
+36	36	ZEP	Zeph	Zep	Zephaniah
+37	37	HAG	Hag	Hag	Haggai
+38	38	ZEC	Zech	Zec	Zechariah
+39	39	MAL	Mal	Mal	Malachi
 # gap in the USFM numbering sequence here because of the legacy
 # issue of MAT as 41 rather than 40.
-40	68	TOB	Tob	Tobit
-41	69	JDT	Jdt	Judith
-42	70	ESG	EsthGr	Esther Greek
-43	71	WIS	Wis	Wisdom of Solomon
-44	72	SIR	Sir	Sirach
-45	73	BAR	Bar	Baruch
-46	74	LJE	EpJer	Letter of Jeremiah
-47	75	S3Y	PrAzar	Song of the 3 Young Men
-48	76	SUS	Sus	Susanna
-49	77	BEL	Bel	Bel and the Dragon
-50	78	1MA	1Macc	1 Maccabees
-51	79	2MA	2Macc	2 Maccabees
-52	82	1ES	1Esd	1 Esdras (Greek)
-53	84	MAN	PrMan	Prayer of Manasseh
-54	85	PS2	AddPs	Psalm 151
-55	80	3MA	3Macc	3 Maccabees
-56	83	2ES	2Esd	2 Esdras (Latin)
-57	81	4MA	4Macc	4 Maccabees
-58	86	ODA	Odes	Odae/Odes
-59	87	PSS	PssSol	Psalms of Solomon
-60	C3	LAO	EpLao	Letter to the Laodiceans
+# Need to add Biblia abbreviations for Deuterocanon
+40	68	TOB	Tob	aaa	Tobit
+41	69	JDT	Jdt	bbb	Judith
+42	70	ESG	EsthGr	ccc	Esther Greek
+43	71	WIS	Wis	ddd	Wisdom of Solomon
+44	72	SIR	Sir	eee	Sirach
+45	73	BAR	Bar	fff	Baruch
+46	74	LJE	EpJer	ggg	Letter of Jeremiah
+47	75	S3Y	PrAzar	hhh	Song of the 3 Young Men
+48	76	SUS	Sus	iii	Susanna
+49	77	BEL	Bel	jjj	Bel and the Dragon
+50	78	1MA	1Macc	kkk	1 Maccabees
+51	79	2MA	2Macc	lll	2 Maccabees
+52	82	1ES	1Esd	mmm	1 Esdras (Greek)
+53	84	MAN	PrMan	nnn	Prayer of Manasseh
+54	85	PS2	AddPs	ooo	Psalm 151
+55	80	3MA	3Macc	ppp	3 Maccabees
+56	83	2ES	2Esd	qqq	2 Esdras (Latin)
+57	81	4MA	4Macc	rrr	4 Maccabees
+58	86	ODA	Odes	sss	Odae/Odes
+59	87	PSS	PssSol	ttt	Psalms of Solomon
+60	C3	LAO	EpLao	uuu	Letter to the Laodiceans
 # Some filenames and legacy data have USFM number for MAT as 41,
 # and +1 for subsequent NT books: use usfmnumberalt for that. But
 # most common current practice is MAT = 40.
-61	40	MAT	Matt	Matthew	The Gospel according to Matthew
-62	41	MRK	Mark	Mark	The Gospel according to Mark
-63	42	LUK	Luke	Luke	The Gospel according to Luke
-64	43	JHN	John	John	The Gospel according to John
-65	44	ACT	Acts	Acts	The Acts of the Apostles
-66	45	ROM	Rom	Romans	The Letter of Paul to the Romans
-67	46	1CO	1Cor	1 Corinthians	The First Letter of Paul to the Corinthians
-68	47	2CO	2Cor	2 Corinthians	The Second Letter of Paul to the Corinthians
-69	48	GAL	Gal	Galatians	The Letter of Paul to the Galatians
-70	49	EPH	Eph	Ephesians	The Letter of Paul to the Ephesians
-71	50	PHP	Phil	Philippians	The Letter of Paul to the Philippians
-72	51	COL	Col	Colossians	The Letter of Paul to the Colossians
-73	52	1TH	1Thess	1 Thessalonians	The First Letter of Paul to the Thessalonians
-74	53	2TH	2Thess	2 Thessalonians	The Second Letter of Paul to the Thessalonians
-75	54	1TI	1Tim	1 Timothy	The First Letter of Paul to Timothy
-76	55	2TI	2Tim	2 Timothy	The Second Letter of Paul to Timothy
-77	56	TIT	Titus	Titus	The Letter of Paul to Titus
-78	57	PHM	Phlm	Philemon	The Letter of Paul to Philemon
-79	58	HEB	Heb	Hebrews	The Letter to the Hebrews
-80	59	JAS	Jas	James	The Letter of James
-81	60	1PE	1Pet	1 Peter	The First Letter of Peter
-82	61	2PE	2Pet	2 Peter	The Second Letter of Peter
-83	62	1JN	1John	1 John	The First Letter of John
-84	63	2JN	2John	2 John	The Second Letter of John
-85	64	3JN	3John	3 John	The Third Letter of John
-86	65	JUD	Jude	Jude	The Letter of Jude
-87	66	REV	Rev	Revelation	The Revelation to John
-88	B7	ENO	1En	Enoch
+61	40	MAT	Matt	Mt	Matthew	The Gospel according to Matthew
+62	41	MRK	Mark	Mk	Mark	The Gospel according to Mark
+63	42	LUK	Luke	Lk	Luke	The Gospel according to Luke
+64	43	JHN	John	Jn	John	The Gospel according to John
+65	44	ACT	Acts	Ac	Acts	The Acts of the Apostles
+66	45	ROM	Rom	Ro	Romans	The Letter of Paul to the Romans
+67	46	1CO	1Cor	1Co	1 Corinthians	The First Letter of Paul to the Corinthians
+68	47	2CO	2Cor	2Co	2 Corinthians	The Second Letter of Paul to the Corinthians
+69	48	GAL	Gal	Ga	Galatians	The Letter of Paul to the Galatians
+70	49	EPH	Eph	Eph	Ephesians	The Letter of Paul to the Ephesians
+71	50	PHP	Phil	Php	Philippians	The Letter of Paul to the Philippians
+72	51	COL	Col	Col	Colossians	The Letter of Paul to the Colossians
+73	52	1TH	1Thess	1Th	1 Thessalonians	The First Letter of Paul to the Thessalonians
+74	53	2TH	2Thess	2Th	2 Thessalonians	The Second Letter of Paul to the Thessalonians
+75	54	1TI	1Tim	1Ti	1 Timothy	The First Letter of Paul to Timothy
+76	55	2TI	2Tim	2Ti	2 Timothy	The Second Letter of Paul to Timothy
+77	56	TIT	Titus	Tt	Titus	The Letter of Paul to Titus
+78	57	PHM	Phlm	Phm	Philemon	The Letter of Paul to Philemon
+79	58	HEB	Heb	Heb	Hebrews	The Letter to the Hebrews
+80	59	JAS	Jas	Jas	James	The Letter of James
+81	60	1PE	1Pet	1Pe	1 Peter	The First Letter of Peter
+82	61	2PE	2Pet	2Pe	2 Peter	The Second Letter of Peter
+83	62	1JN	1John	1Jn	1 John	The First Letter of John
+84	63	2JN	2John	2Jn	2 John	The Second Letter of John
+85	64	3JN	3John	3Jn	3 John	The Third Letter of John
+86	65	JUD	Jude	Jud	Jude	The Letter of Jude
+87	66	REV	Rev	Re	Revelation	The Revelation to John
+88	B7	ENO	1En		Enoch
 # Logos also has 2 Baruch (99)??
 # LBD: 'The Syriac Apocalypse of Baruch proper consists of 2
 # Baruch 1–77, while 2 Baruch 78–87 form the Letter of Baruch.'
 # I'm guessing USFM doesn't distinguish?
-96	B4	2BA	2Bar	2 Baruch (Apocalypse)	The Apocalypse of Baruch
-97	B5	LBA	EpBar	Letter of Baruch
-98	B2	DAG	DanGr	Daniel Greek
+96	B4	2BA	2Bar	vvv	2 Baruch (Apocalypse)	The Apocalypse of Baruch
+97	B5	LBA	EpBar	www	Letter of Baruch
+98	B2	DAG	DanGr	xxx	Daniel Greek
 # (99, '2 Baruch'),
-100	A4	EZA	4Ezra	Ezra Apocalypse
+100	A4	EZA	4Ezra	yyy	Ezra Apocalypse
 # # no Logos number AFAIK: arbitrarily numbered from 200
-200	A5	5EZ	5Ezra	5 Ezra
-201	A6	6EZ	6Ezra	6 Ezra
-202	B3	PS3	5ApocSyrPss	Psalms 152-155
-203	B6	JUB	Jub	Jubilees
-204	B8	1MQ	1Meq	1 Meqabyan/Mekabis	Book of Mekabis of Benjamin
-205	B9	2MQ	2Meq	2 Meqabyan/Mekabis	Book of Mekabis of Moab
-206	C0	3MQ	3Meq	3 Meqabyan/Mekabis	Book of Meqabyan
-207	C1	REP	Rep	Reproof
-208	C2	4BA	4Bar	4 Baruch
+200	A5	5EZ	5Ezra	zzz	5 Ezra
+201	A6	6EZ	6Ezra	aab	6 Ezra
+202	B3	PS3	5ApocSyrPss	aac	Psalms 152-155
+203	B6	JUB	Jub	aad	Jubilees
+204	B8	1MQ	1Meq	aae	1 Meqabyan/Mekabis	Book of Mekabis of Benjamin
+205	B9	2MQ	2Meq	aaf	2 Meqabyan/Mekabis	Book of Mekabis of Moab
+206	C0	3MQ	3Meq	aag	3 Meqabyan/Mekabis	Book of Meqabyan
+207	C1	REP	Rep	aah	Reproof
+208	C2	4BA	4Bar	aai	4 Baruch
 # more from Logos, per
 # https://wiki.logos.com/Logos_Bible_Book_Names, but not in
 # USFM/OSIS? These seems to be from DSS5
 # `logosref:bibleNN` doesn't navigate for more in Logos for NN > 87
 # (89, 'Plea for Deliverance'),
 # (90, 'Apostrophe to Zion'),
 # (91, 'Eschatalogical Hymn'),
```

### Comparing `biblelib-0.3.2/biblelib/sources.py` & `biblelib-0.3.3/biblelib/sources.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/__init__.py` & `biblelib-0.3.3/biblelib/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/book.py` & `biblelib-0.3.3/biblelib/unit/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/bookchapters.tsv` & `biblelib-0.3.3/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/chapter.py` & `biblelib-0.3.3/biblelib/unit/chapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/chapters.tsv` & `biblelib-0.3.3/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/chapterverses.tsv` & `biblelib-0.3.3/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/pericope.py` & `biblelib-0.3.3/biblelib/unit/pericope.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/tempchapter.py` & `biblelib-0.3.3/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/unit.py` & `biblelib-0.3.3/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/unit/unitrange.py` & `biblelib-0.3.3/biblelib/unit/unitrange.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 >>> onechap = VerseRange(start=BCVID("41001040"), end=BCVID("41002002"))
 >>> onechap.enumerate()
 [Verse(identifier='BCVID('41001040')'), Verse(identifier='BCVID('41001041')'), ... Verse(identifier='BCVID('41002002')')]
 
 
 """
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import re
 
 from biblelib.book import Books
 from biblelib.word import BID, BCID, BCVID, simplify
 from .chapter import Chapter
 from .verse import Verse
 from .unit import pad
@@ -60,20 +60,35 @@
 
 @dataclass
 class VerseRange:
     """Manage a range of verses."""
 
     startid: BCVID
     endid: BCVID
+    # these are computed from startid and endid
+    ID: str = field(init=False)
+    book: BID = field(init=False)
+    chapter: BCID = field(init=False)
 
     def __post_init__(self) -> None:
         """Check initialization values."""
-        assert simplify(self.startid, BID) == simplify(
-            self.endid, BID
-        ), f"Startid {self.startid} and endid (self.endid) must be in the same book."
+        # enforce typs: a little hacky to change init values like this.
+        # It would be less hacky to have a factory method that does this.
+        if self.startid.__class__.__name__ != "BCVID":
+            self.startid = BCVID(self.startid.to_bcvid)
+        if self.endid.__class__.__name__ != "BCVID":
+            self.endid = BCVID(self.endid.to_bcvid)
+        self.ID = self.startid.ID + "-" + self.endid.ID
+        self.book: BID = BID(self.startid.to_bid)
+        self.chapter: BCID = BCID(self.startid.to_bcid)
+        assert self.book == BID(
+            self.endid.to_bid
+        ), f"Startid {self.startid} and endid {self.endid} must be in the same book."
+        # note this allows a vacuous range with the same start and
+        # end: does that make sense?
         assert self.startid <= self.endid, f"Startid {self.startid} must precede endid {self.endid}."
 
     def enumerate(self) -> list[Verse]:
         """Return a list of Verse instances enumerating the verses in the range.
 
         Enumerations include the ending Verse value (unlike range).
         """
```

### Comparing `biblelib-0.3.2/biblelib/unit/verse.py` & `biblelib-0.3.3/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/Enumerator.py` & `biblelib-0.3.3/biblelib/versification/Enumerator.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/ReadMe.md` & `biblelib-0.3.3/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/VrefReader.py` & `biblelib-0.3.3/biblelib/versification/VrefReader.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     def __init__(self, scheme: str, canon: str, asbcv: bool = True) -> None:
         """Read a .vref file.
 
         With asbcv=True (the default), converts references from USFM
         to BCV: otherwise they remain as USFM.
 
         """
+        assert scheme in self.schemes, f"Unsupported scheme: {scheme}"
+        assert canon in self.canons, f"Unsupported canon: {canon}"
         self.scheme = scheme
         self.canon = canon
         self.vref_file: str = self.get_vref_file(scheme, canon)
         r = requests.get(self.vref_file)
         assert r.status_code == 200, f"Failed to get content from {self.vref_file}"
         vref_usfm: list[str] = r.text.split("\n")
         if asbcv:
```

### Comparing `biblelib-0.3.2/biblelib/versification/eng-nt-vref.txt` & `biblelib-0.3.3/biblelib/versification/eng-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/eng-ot-vref.txt` & `biblelib-0.3.3/biblelib/versification/eng-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/eng-protestant-vref.txt` & `biblelib-0.3.3/biblelib/versification/eng-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/org-nt-vref.txt` & `biblelib-0.3.3/biblelib/versification/org-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/org-ot-vref.txt` & `biblelib-0.3.3/biblelib/versification/org-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/org-protestant-vref.txt` & `biblelib-0.3.3/biblelib/versification/org-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/rso-nt-vref.txt` & `biblelib-0.3.3/biblelib/versification/rso-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/rso-ot-vref.txt` & `biblelib-0.3.3/biblelib/versification/rso-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/versification/rso-protestant-vref.txt` & `biblelib-0.3.3/biblelib/versification/rso-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/word/__init__.py` & `biblelib-0.3.3/biblelib/word/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/biblelib/word/bcvwpid.py` & `biblelib-0.3.3/biblelib/word/bcvwpid.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     # class is mutable because of post_init, but otherwise logically immutable
     # note that, for subclasses, hash(self) != hash(self.ID). I do not
     # know why, but dataclass hash functions are special.
     def __hash__(self) -> int:
         """Return a hash value."""
         return hash(self.ID)
 
+    @property
+    def to_bid(self) -> str:
+        """Return the book ID."""
+        return self.book_ID
+
 
 @dataclass(repr=False, unsafe_hash=True)
 class BID(_Base):
     """Identifies a book identifier.
 
     Also a base class for other BCV identifiers.
     """
@@ -161,14 +166,19 @@
 
     def __post_init__(self) -> None:
         """Compute other values on initialization."""
         super().__post_init__()
         self.chapter_ID = self.ID[2:5]
         # also test that they're all digits, in the right range, etc.
 
+    @property
+    def to_bcid(self) -> str:
+        """Return string for the book and chapter ID."""
+        return self.book_ID + self.chapter_ID
+
     def includes(self, other: Any) -> bool:
         """Return True if other is included in the scope of self.
 
         Simply based on substring matching. Any instance includes
         itself therefore.
 
         """
@@ -222,14 +232,19 @@
 
     def __post_init__(self) -> None:
         """Compute other values on initialization."""
         super().__post_init__()
         self.verse_ID = self.ID[5:8]
         # also test that they're all digits, in the right range, etc.
 
+    @property
+    def to_bcvid(self) -> str:
+        """Return string for the book, chapter, and verse ID."""
+        return self.book_ID + self.chapter_ID + self.verse_ID
+
     def includes(self, other: Any) -> bool:
         """Return True if other is included in the scope of self.
 
         Simply based on substring matching. Any instance includes
         itself therefore.
 
         """
@@ -383,29 +398,14 @@
 
     # not sure this is a proper USFM-ification
     def to_usfm(self) -> str:
         """Return a USFM representation."""
         usfmbook = BOOKS.fromusfmnumber(self.book_ID).usfmname
         return f"{usfmbook} {int(self.chapter_ID)}:{int(self.verse_ID)}"
 
-    @property
-    def to_bid(self) -> str:
-        """Return the book ID."""
-        return self.book_ID
-
-    @property
-    def to_bcid(self) -> str:
-        """Return string for the book and chapter ID."""
-        return self.book_ID + self.chapter_ID
-
-    @property
-    def to_bcvid(self) -> str:
-        """Return string for the book, chapter, and verse ID."""
-        return self.book_ID + self.chapter_ID + self.verse_ID
-
 
 # @dataclass
 # class MarbleID(BCVWPID:
 #     """Like a standard BCVWPID, but with an extra leading digit for books.
 
 #     Format is BBBCCCVVVWWWP."""
```

### Comparing `biblelib-0.3.2/biblelib/word/mappings.py` & `biblelib-0.3.3/biblelib/word/mappings.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.2/pyproject.toml` & `biblelib-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.3.2"
+version = "0.3.3"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 # apparently text files are also shipped?
 # include = [
@@ -19,15 +19,16 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 pydantic = "^2.3.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+black = "^24.3.0"
 pytest = "^7.1.2"
 mkdocs = "^1.3.0"
 mkdocs-material = "^8.3.8"
 mkdocstrings = "^0.18.1"
 mypy = "^0.961"
 #pre-commit = "^2.20.0"
 tox = "^3.25.1"
```

### Comparing `biblelib-0.3.2/PKG-INFO` & `biblelib-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.3.2
+Version: 0.3.3
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

