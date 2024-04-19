# Comparing `tmp/profasta-0.0.4.tar.gz` & `tmp/profasta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profasta-0.0.4.tar", last modified: Fri Feb 16 12:17:20 2024, max compression
+gzip compressed data, was "profasta-0.0.5.tar", last modified: Fri Apr 19 15:01:50 2024, max compression
```

## Comparing `profasta-0.0.4.tar` & `profasta-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 12:17:20.500391 profasta-0.0.4/
--rw-rw-rw-   0        0        0     1096 2024-01-31 15:54:36.000000 profasta-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0     5364 2024-02-16 12:17:20.499394 profasta-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3404 2024-02-16 10:32:36.000000 profasta-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-16 12:17:20.480446 profasta-0.0.4/profasta/
--rw-rw-rw-   0        0        0      315 2024-02-16 12:15:28.000000 profasta-0.0.4/profasta/__init__.py
--rw-rw-rw-   0        0        0     6231 2024-02-16 12:15:28.000000 profasta-0.0.4/profasta/db.py
--rw-rw-rw-   0        0        0     1695 2024-02-16 10:32:36.000000 profasta-0.0.4/profasta/decoy.py
--rw-rw-rw-   0        0        0     3325 2024-02-16 10:32:36.000000 profasta-0.0.4/profasta/io.py
--rw-rw-rw-   0        0        0    11488 2024-02-16 10:32:36.000000 profasta-0.0.4/profasta/parser.py
-drwxrwxrwx   0        0        0        0 2024-02-16 12:17:20.498397 profasta-0.0.4/profasta.egg-info/
--rw-rw-rw-   0        0        0     5364 2024-02-16 12:17:20.000000 profasta-0.0.4/profasta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-02-16 12:17:20.000000 profasta-0.0.4/profasta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 12:17:20.000000 profasta-0.0.4/profasta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-16 12:17:20.000000 profasta-0.0.4/profasta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-16 12:17:20.000000 profasta-0.0.4/profasta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1004 2024-02-14 11:01:10.000000 profasta-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-16 12:17:20.500391 profasta-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-01-12 15:48:17.000000 profasta-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:01:50.633344 profasta-0.0.5/
+-rw-rw-rw-   0        0        0     1096 2024-01-31 15:54:36.000000 profasta-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0     6141 2024-04-19 15:01:50.632346 profasta-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4083 2024-04-19 15:00:38.000000 profasta-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 15:01:50.618384 profasta-0.0.5/profasta/
+-rw-rw-rw-   0        0        0      315 2024-04-19 15:00:38.000000 profasta-0.0.5/profasta/__init__.py
+-rw-rw-rw-   0        0        0     8288 2024-04-19 15:00:38.000000 profasta-0.0.5/profasta/db.py
+-rw-rw-rw-   0        0        0     1875 2024-04-19 15:00:38.000000 profasta-0.0.5/profasta/decoy.py
+-rw-rw-rw-   0        0        0     3451 2024-04-19 15:00:38.000000 profasta-0.0.5/profasta/io.py
+-rw-rw-rw-   0        0        0    11831 2024-04-19 15:00:38.000000 profasta-0.0.5/profasta/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:01:50.631349 profasta-0.0.5/profasta.egg-info/
+-rw-rw-rw-   0        0        0     6141 2024-04-19 15:01:50.000000 profasta-0.0.5/profasta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-19 15:01:50.000000 profasta-0.0.5/profasta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:01:50.000000 profasta-0.0.5/profasta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-19 15:01:50.000000 profasta-0.0.5/profasta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 15:01:50.000000 profasta-0.0.5/profasta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1029 2024-04-19 15:00:38.000000 profasta-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:01:50.633344 profasta-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-01-12 15:48:17.000000 profasta-0.0.5/setup.py
```

### Comparing `profasta-0.0.4/LICENSE.md` & `profasta-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `profasta-0.0.4/PKG-INFO` & `profasta-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profasta
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for working with protein containing FASTA files.
 Author-email: "David M. Hollenstein" <hollenstein.david@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 David M. Hollenstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,17 +31,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
+Provides-Extra: dev
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # ProFASTA
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fhollenstein%2Fprofasta%2Fmain%2Fpyproject.toml)
+[![pypi](https://img.shields.io/pypi/v/profasta)](https://pypi.org/project/profasta)
+[![unit-tests](https://github.com/hollenstein/profasta/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/hollenstein/profasta/actions/workflows/python-package.yml)
 
 ## Introduction
 ProFASTA is a Python library for working with FASTA files containing protein records. Unlike other packages, ProFASTA prioritizes simplicity, while aiming to provide a set of useful features required in the field of proteomics based mass spectrometry. 
 
 The library is still in early development and the interface might change over time. At the current stage ProFASTA provides functionality for parsing and writing FASTA files, as well as for providing access to protein records imported from FASTA files.
 
 ProFASTA is developed as part of the computational toolbox for the [Mass Spectrometry Facility](https://www.maxperutzlabs.ac.at/research/facilities/mass-spectrometry-facility) at the Max Perutz Labs (University of Vienna).
@@ -55,22 +61,24 @@
 
 ## Usage example
 The following code snippet shows how to import a FASTA file containing UniProt protein entries, retrieve a protein record by its UniProt accession number and print its gene name:
 
 ```python
 >>> import profasta
 >>> 
->>> fasta_path = "./example_data/uniprot_hsapiens_10entries.fasta"
+>>> fasta_path = "./examples/uniprot_hsapiens_10entries.fasta"
 >>> db = profasta.db.ProteinDatabase()
 >>> db.add_fasta(fasta_path, header_parser="uniprot")
 >>> protein_record = db["O75385"]
 >>> print(protein_record.header_fields["gene_name"])
 ULK1
 ```
 
+For more examples how to use the ProFASTA library please refer to the [code snippets](examples/code_snippets.ipynb) Jupyter notebook.
+
 ## Requirements
 Python >= 3.9
 
 ## Installation
 The following command will install the latest version of ProFASTA and its dependencies from PyPi, the Python Packaging Index:
 
 ```
@@ -87,16 +95,19 @@
 **Main requirements**
 - [x] parse FASTA file
 - [x] parse FASTA header
     - [x] built-in parser that never fails
     - [x] built-in parser for uniprot format
     - [x] allow user defined parser
 - [x] write FASTA file
-    -[x] allow custom FASTA header generation
+    - [x] allow custom FASTA header generation
     
 **Additional features**
 - [x] read multiple FASTA files and write a combined file
 - [x] add protein records to an existing FASTA file
 - [x] generate decoy protein records by reversing the sequence
     - [x] add decoy protein records to an existing FASTA file
 - [ ] validate FASTA file / FASTA records
 
+## Contributors
+
+- Juraj Ahel - [@xeniorn](https://github.com/xeniorn)
```

### Comparing `profasta-0.0.4/README.md` & `profasta-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # ProFASTA
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fhollenstein%2Fprofasta%2Fmain%2Fpyproject.toml)
+[![pypi](https://img.shields.io/pypi/v/profasta)](https://pypi.org/project/profasta)
+[![unit-tests](https://github.com/hollenstein/profasta/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/hollenstein/profasta/actions/workflows/python-package.yml)
 
 ## Introduction
 ProFASTA is a Python library for working with FASTA files containing protein records. Unlike other packages, ProFASTA prioritizes simplicity, while aiming to provide a set of useful features required in the field of proteomics based mass spectrometry. 
 
 The library is still in early development and the interface might change over time. At the current stage ProFASTA provides functionality for parsing and writing FASTA files, as well as for providing access to protein records imported from FASTA files.
 
 ProFASTA is developed as part of the computational toolbox for the [Mass Spectrometry Facility](https://www.maxperutzlabs.ac.at/research/facilities/mass-spectrometry-facility) at the Max Perutz Labs (University of Vienna).
@@ -17,22 +20,24 @@
 
 ## Usage example
 The following code snippet shows how to import a FASTA file containing UniProt protein entries, retrieve a protein record by its UniProt accession number and print its gene name:
 
 ```python
 >>> import profasta
 >>> 
->>> fasta_path = "./example_data/uniprot_hsapiens_10entries.fasta"
+>>> fasta_path = "./examples/uniprot_hsapiens_10entries.fasta"
 >>> db = profasta.db.ProteinDatabase()
 >>> db.add_fasta(fasta_path, header_parser="uniprot")
 >>> protein_record = db["O75385"]
 >>> print(protein_record.header_fields["gene_name"])
 ULK1
 ```
 
+For more examples how to use the ProFASTA library please refer to the [code snippets](examples/code_snippets.ipynb) Jupyter notebook.
+
 ## Requirements
 Python >= 3.9
 
 ## Installation
 The following command will install the latest version of ProFASTA and its dependencies from PyPi, the Python Packaging Index:
 
 ```
@@ -49,16 +54,19 @@
 **Main requirements**
 - [x] parse FASTA file
 - [x] parse FASTA header
     - [x] built-in parser that never fails
     - [x] built-in parser for uniprot format
     - [x] allow user defined parser
 - [x] write FASTA file
-    -[x] allow custom FASTA header generation
+    - [x] allow custom FASTA header generation
     
 **Additional features**
 - [x] read multiple FASTA files and write a combined file
 - [x] add protein records to an existing FASTA file
 - [x] generate decoy protein records by reversing the sequence
     - [x] add decoy protein records to an existing FASTA file
 - [ ] validate FASTA file / FASTA records
 
+## Contributors
+
+- Juraj Ahel - [@xeniorn](https://github.com/xeniorn)
```

### Comparing `profasta-0.0.4/profasta/db.py` & `profasta-0.0.5/profasta/db.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,23 @@
     AbstractDatabaseEntry (Protocol): Interface for representing a protein entry.
     DatabaseEntry: Representation of a protein entry.
     ProteinDatabase: A database for managing protein entries derived from FASTA files.
 """
 
 from __future__ import annotations
 from dataclasses import dataclass
+import logging
 from pathlib import Path
 from typing import Any, Iterator, Optional, Protocol
 
 from profasta.parser import get_parser, get_writer
 import profasta.io
 
+logger = logging.getLogger(__name__)
+
 
 class AbstractDatabaseEntry(Protocol):
     """A protein entry derived from a protein record in a FASTA file."""
 
     identifier: str
     header: str
     sequence: str
@@ -47,59 +50,93 @@
 
     The Python indexing operator `[]` provides access to the protein entries by their
     identifier. Iterating over the database yields the identifiers of all protein
     entries.
 
     Attributes:
         db: Dictionary mapping protein identifiers to protein entries.
-        imported_fasta_files: List of FASTA files that have been imported into the
+        added_fasta_files: List of FASTA files that have been imported into the
             database.
+        skipped_fasta_entries: Dictionary mapping added FASTA names to lists of FASTA
+            entry headers that could not be parsed by the header parser, and thus were
+            not added to the database.
     """
 
     db: dict[str, AbstractDatabaseEntry]
-    imported_fasta_files: list[str]
+    added_fasta_files: list[str]
+    skipped_fasta_entries: dict[str, list]
 
     def __init__(self):
         self.db = {}
-        self.imported_fasta_files = []
+        self.added_fasta_files = []
+        self.skipped_fasta_entries = {}
 
     def add_fasta(
         self,
         path: str,
         header_parser: str,
         fasta_name: Optional[str] = None,
         overwrite: bool = False,
+        skip_invalid: bool = False,
     ):
         """Add protein entries from a FASTA file to the database.
 
         Args:
             path: The path to the FASTA file.
             header_parser: The name of the parser to use for parsing the FASTA headers.
                 The parser must be registered in the global parser registry.
             fasta_name: Optional name for the FASTA file. If not provided, the filename
                 will be used instead.
             overwrite: If True, overwrite an existing entry with the same identifier.
                 If False and an entry with the same identifier already exists, a
                 KeyError will be raised.
+            skip_invalid: If True, entries with a non-parsable header are skipped. If
+                False, a ValueError is raised when an entry is encountered which header
+                could not be parsed by the header_parser. Headers of skipped entries are
+                stored in the skipped_fasta_entries attribute.
         """
-        if fasta_name is None:
-            fasta_name = Path(path).name
-        self.imported_fasta_files.append(fasta_name)
-
+        fasta_name = fasta_name if fasta_name is not None else Path(path).name
         parser = get_parser(header_parser)
+        parsed_protein_entries: list[DatabaseEntry] = []
+        skipped_entry_headers: list[str] = []
+
         with open(path, "r") as file:
             for fasta_record in profasta.io.parse_fasta(file):
-                parsed_header = parser.parse(fasta_record.header)
+                try:
+                    parsed_header = parser.parse(fasta_record.header)
+                except ValueError as error:
+                    if skip_invalid:
+                        skipped_entry_headers.append(fasta_record.header)
+                        continue
+                    else:
+                        raise ValueError(
+                            f"FASTA header could not be parsed with the "
+                            f"'{header_parser}' parser: '{fasta_record.header}'"
+                        ) from error
                 protein_entry = DatabaseEntry(
                     parsed_header.identifier,
                     parsed_header.header,
                     fasta_record.sequence,
                     parsed_header.header_fields,
                 )
-                self.add_entry(protein_entry, overwrite)
+                parsed_protein_entries.append(protein_entry)
+
+        self.added_fasta_files.append(fasta_name)
+        self.skipped_fasta_entries[fasta_name] = skipped_entry_headers
+        for protein_entry in parsed_protein_entries:
+            self.add_entry(protein_entry, overwrite)
+
+        if skipped_entry_headers:
+            num_skipped = len(skipped_entry_headers)
+            num_total = num_skipped + len(parsed_protein_entries)
+            logger.warning(
+                f"Skipped {num_skipped}/{num_total} entries while adding "
+                f"'{fasta_name}' to a ProteinDatabase because their headers could not "
+                f"be parsed:"
+            )
 
     def add_entry(self, protein_entry: AbstractDatabaseEntry, overwrite: bool = False):
         """Add a protein entry to the database.
 
         Args:
             protein_entry: The protein entry to add.
             overwrite: If True, overwrite an existing entry with the same identifier.
@@ -147,14 +184,23 @@
         with open(path, file_open_mode) as file:
             profasta.io.write_fasta(file, fasta_records, line_width)
 
     def get(self, identifier: str, default: Any = None) -> DatabaseEntry | Any:
         """Get a protein entry by its identifier or return a default value."""
         return self.db.get(identifier, default)
 
+    def keys(self):
+        return self.db.keys()
+
+    def values(self):
+        return self.db.values()
+
+    def items(self):
+        return self.db.items()
+
     def __getitem__(self, identifier) -> AbstractDatabaseEntry:
         return self.db[identifier]
 
     def __contains__(self, identifier) -> bool:
         return identifier in self.db
 
     def __iter__(self) -> Iterator[str]:
```

### Comparing `profasta-0.0.4/profasta/decoy.py` & `profasta-0.0.5/profasta/decoy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Functions for creating decoy databases.
+
+Functions:
+    create_decoy_db: Create a decoy database by reversing the sequences of the input
+        database records.
+"""
+
 from copy import deepcopy
 from profasta.db import ProteinDatabase
 
 
 def create_decoy_db(
     db: ProteinDatabase, keep_nterm: bool = False, keep_nterm_methionine: bool = True
 ) -> ProteinDatabase:
@@ -16,24 +23,24 @@
 
     Returns:
         The decoy database.
     """
     decoy_db = ProteinDatabase()
     for protein in db:
         decoy_entry = deepcopy(db[protein])
-        decoy_entry.sequence = reverse_sequence(
+        decoy_entry.sequence = _reverse_sequence(
             decoy_entry.sequence,
             keep_nterm=keep_nterm,
             keep_nterm_methionine=keep_nterm_methionine,
         )
         decoy_db.add_entry(decoy_entry)
     return decoy_db
 
 
-def reverse_sequence(
+def _reverse_sequence(
     sequence: str, keep_nterm: bool = False, keep_nterm_methionine: bool = True
 ) -> str:
     """Create a decoy sequence by reversing the input sequence.
 
     Args:
         sequence: The input sequence.
         keep_nterm: If True, keep the N-terminal residue in the same position. Default
```

### Comparing `profasta-0.0.4/profasta/io.py` & `profasta-0.0.5/profasta/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,29 +42,31 @@
 
 def parse_fasta(file_object: IO[str]) -> Generator[FastaRecord, None, None]:
     """Parse a FASTA file object and yield FastaRecords.
 
     Lines starting with ">" are header lines, all others are sequence lines.
     Each header line is followed by one or multiple sequence lines. Multiple sequence
     lines are joined by removing new line characters into one single sequence string.
+    Sequence strings are converted to uppercase and spaces and trailing "*" characters
+    are removed.
 
     Args:
         file_object: A file object to parse.
 
     Yields:
         Yields FastaRecords.
     """
     fasta_text = file_object.read()
     if not fasta_text.startswith("\n"):
         fasta_text = "\n" + fasta_text
 
     for block in fasta_text.split("\n>")[1:]:
         lines = block.split("\n")
         header = lines[0].strip()
-        sequence = "".join(lines[1:]).replace(" ", "")
+        sequence = "".join(lines[1:]).replace(" ", "").rstrip("*").upper()
         yield FastaRecord(header, sequence)
 
 
 def write_fasta(
     file_object: IO[str],
     fasta_records: Iterable[AbstractFastaRecord],
     line_width: int = -1,
```

### Comparing `profasta-0.0.4/profasta/parser.py` & `profasta-0.0.5/profasta/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 header parsers and writers are registered in a global registry, which can be accessed
 via the `get_parser` and `get_writer` functions and the name of the parser or writer.
 New parsers and writers must be registered via the `register_parser` and
 `register_writer` functions before they become available in the other modules.
 
 Classes:
     AbstractParsedHeader (Protocol): Interface for representing a parsed FASTA header.
+    AbstractHeaderParser (Protocol): Interface for a FASTA header parser.
+    AbstractHeaderWriter (Protocol): Interface for a FASTA header writer.
     ParsedHeader: Representation of a parsed FASTA header.
-    HeaderParser (Protocol): Interface for a FASTA header parser.
-    HeaderWriter (Protocol): Interface for a FASTA header writer.
     DefaultParser: Default FASTA header parser.
     UniprotParser: Parser for Uniprot FASTA headers.
     UniprotLikeParser: Parser for less strict Uniprot like FASTA headers.
     DefaultWriter: Default FASTA header writer.
     UniprotWriter: Parser for Uniprot FASTA writer.
     UniprotLikeWriter: Parser for less strict Uniprot like FASTA writer.
 
@@ -49,56 +49,59 @@
     """
 
     identifier: str
     header: str
     header_fields: dict[str, str]
 
 
-@dataclass
-class ParsedHeader:
-    """Parsed FASTA header.
-
-    Attributes:
-        identifier: The unique identifier of the FASTA entry.
-        header: The FASTA header, not containing the starting ">" character.
-        header_fields: The parsed header fields as a dictionary.
-    """
-
-    identifier: str
-    header: str
-    header_fields: dict[str, str] = field(default_factory=dict)
-
-
-class HeaderParser(Protocol):
+class AbstractHeaderParser(Protocol):
     """Abstract header parser."""
 
     @classmethod
     def parse(self, header: str) -> AbstractParsedHeader:
-        """Parse a FASTA header string into a ParsedHeader object."""
+        """Parse a FASTA header string into a ParsedHeader object.
+
+        Raises:
+            ValueError: If the header could not be parsed.
+        """
         ...
 
 
-class HeaderWriter(Protocol):
+class AbstractHeaderWriter(Protocol):
     """Abstract header writer."""
 
     @classmethod
     def write(self, parsed_header: AbstractParsedHeader) -> str:
         """Write a FASTA header string from a ParsedHeader object."""
         ...
 
 
+@dataclass
+class ParsedHeader:
+    """Parsed FASTA header.
+
+    Attributes:
+        identifier: The unique identifier of the FASTA entry.
+        header: The FASTA header, not containing the starting ">" character.
+        header_fields: The parsed header fields as a dictionary.
+    """
+
+    identifier: str
+    header: str
+    header_fields: dict[str, str] = field(default_factory=dict)
+
+
 class DefaultParser:
     """Default FASTA header parser.
 
     The `parse` method returns a ParsedHeader object with the identifier being the
     first whitespace-separated word of the header. The rest of the header is stored
     in the "description" field of the `header_fields` dictionary, which might be an
-    empty string.
-
-    The `write` method returns the original `header` string from the parsed_header.
+    empty string. This parser is guaranteed to work for any FASTA header string and
+    never fail.
     """
 
     @classmethod
     def parse(cls, header: str) -> ParsedHeader:
         """Parse a FASTA header string into a ParsedHeader object."""
         split_header = header.split(maxsplit=1)
         _id = split_header[0]
@@ -155,15 +158,19 @@
         "GN": "gene_name",
         "PE": "protein_existence",
         "SV": "sequence_version",
     }
 
     @classmethod
     def parse(cls, header: str) -> ParsedHeader:
-        """Parse a FASTA header string into a ParsedHeader object."""
+        """Parse a FASTA header string into a ParsedHeader object.
+
+        Raises:
+            ValueError: If the header could not be parsed.
+        """
         match = cls.header_pattern.match(header)
         if match is None:
             raise ValueError(f"Header does not match the UniProt pattern: {header}")
         fields = match.groupdict()
 
         for key in ["OS", "OX", "GN", "PE", "SV"]:
             if fields[key] is None:
@@ -221,15 +228,19 @@
         "GN": "gene_name",
         "PE": "protein_existence",
         "SV": "sequence_version",
     }
 
     @classmethod
     def parse(cls, header: str) -> ParsedHeader:
-        """Parse a FASTA header string into a ParsedHeader object."""
+        """Parse a FASTA header string into a ParsedHeader object.
+
+        Raises:
+            ValueError: If the header could not be parsed.
+        """
         split_header = header.split(maxsplit=1)
         try:
             db, _id, entry = split_header[0].split("|")
         except ValueError:
             raise ValueError(
                 f"Header does not match the minimal UniProt like pattern: {header}"
             )
@@ -290,40 +301,40 @@
             field_name = cls.tag_names[key]
             if field_name not in fields:
                 continue
             header_entries.append(f"{key}={fields[field_name]}")
         return " ".join(header_entries)
 
 
-def register_parser(name: str, parser: HeaderParser):
+def register_parser(name: str, parser: AbstractHeaderParser):
     """Register a custom parser by name."""
     PARSER_REGISTRY[name] = parser
 
 
-def get_parser(parser_name: str) -> HeaderParser:
+def get_parser(parser_name: str) -> AbstractHeaderParser:
     """Get a registered parser by name."""
     return PARSER_REGISTRY[parser_name]
 
 
-def register_writer(name: str, parser: HeaderWriter):
+def register_writer(name: str, parser: AbstractHeaderWriter):
     """Register a custom writer by name."""
     WRITER_REGISTRY[name] = parser
 
 
-def get_writer(parser_name: str) -> HeaderWriter:
+def get_writer(parser_name: str) -> AbstractHeaderWriter:
     """Get a registered writer by name."""
     return WRITER_REGISTRY[parser_name]
 
 
-PARSER_REGISTRY: dict[str, HeaderParser] = {
+PARSER_REGISTRY: dict[str, AbstractHeaderParser] = {
     "default": DefaultParser,
     "uniprot": UniprotParser,
     "uniprot_like": UniprotLikeParser,
 }
 
 
-WRITER_REGISTRY: dict[str, HeaderWriter] = {
+WRITER_REGISTRY: dict[str, AbstractHeaderWriter] = {
     "default": DefaultWriter,
     "decoy": DecoyWriter,
     "uniprot": UniprotWriter,
     "uniprot_like": UniprotLikeWriter,
 }
```

### Comparing `profasta-0.0.4/profasta.egg-info/PKG-INFO` & `profasta-0.0.5/profasta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profasta
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library for working with protein containing FASTA files.
 Author-email: "David M. Hollenstein" <hollenstein.david@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 David M. Hollenstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,17 +31,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
+Provides-Extra: dev
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # ProFASTA
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fhollenstein%2Fprofasta%2Fmain%2Fpyproject.toml)
+[![pypi](https://img.shields.io/pypi/v/profasta)](https://pypi.org/project/profasta)
+[![unit-tests](https://github.com/hollenstein/profasta/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/hollenstein/profasta/actions/workflows/python-package.yml)
 
 ## Introduction
 ProFASTA is a Python library for working with FASTA files containing protein records. Unlike other packages, ProFASTA prioritizes simplicity, while aiming to provide a set of useful features required in the field of proteomics based mass spectrometry. 
 
 The library is still in early development and the interface might change over time. At the current stage ProFASTA provides functionality for parsing and writing FASTA files, as well as for providing access to protein records imported from FASTA files.
 
 ProFASTA is developed as part of the computational toolbox for the [Mass Spectrometry Facility](https://www.maxperutzlabs.ac.at/research/facilities/mass-spectrometry-facility) at the Max Perutz Labs (University of Vienna).
@@ -55,22 +61,24 @@
 
 ## Usage example
 The following code snippet shows how to import a FASTA file containing UniProt protein entries, retrieve a protein record by its UniProt accession number and print its gene name:
 
 ```python
 >>> import profasta
 >>> 
->>> fasta_path = "./example_data/uniprot_hsapiens_10entries.fasta"
+>>> fasta_path = "./examples/uniprot_hsapiens_10entries.fasta"
 >>> db = profasta.db.ProteinDatabase()
 >>> db.add_fasta(fasta_path, header_parser="uniprot")
 >>> protein_record = db["O75385"]
 >>> print(protein_record.header_fields["gene_name"])
 ULK1
 ```
 
+For more examples how to use the ProFASTA library please refer to the [code snippets](examples/code_snippets.ipynb) Jupyter notebook.
+
 ## Requirements
 Python >= 3.9
 
 ## Installation
 The following command will install the latest version of ProFASTA and its dependencies from PyPi, the Python Packaging Index:
 
 ```
@@ -87,16 +95,19 @@
 **Main requirements**
 - [x] parse FASTA file
 - [x] parse FASTA header
     - [x] built-in parser that never fails
     - [x] built-in parser for uniprot format
     - [x] allow user defined parser
 - [x] write FASTA file
-    -[x] allow custom FASTA header generation
+    - [x] allow custom FASTA header generation
     
 **Additional features**
 - [x] read multiple FASTA files and write a combined file
 - [x] add protein records to an existing FASTA file
 - [x] generate decoy protein records by reversing the sequence
     - [x] add decoy protein records to an existing FASTA file
 - [ ] validate FASTA file / FASTA records
 
+## Contributors
+
+- Juraj Ahel - [@xeniorn](https://github.com/xeniorn)
```

### Comparing `profasta-0.0.4/pyproject.toml` & `profasta-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ]
 keywords = ["fasta", "bioinformatics", "mass spectrometry", "proteomics"]
 requires-python = ">=3.9"
 dynamic = ["version"]
 
 [project.optional-dependencies]
 tests = ["pytest"]
+dev = ["nox", "pytest"]
 
 [project.urls]
 repository = "https://github.com/hollenstein/profasta"
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

