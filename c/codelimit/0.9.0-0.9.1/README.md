# Comparing `tmp/codelimit-0.9.0.tar.gz` & `tmp/codelimit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelimit-0.9.0.tar", max compression
+gzip compressed data, was "codelimit-0.9.1.tar", max compression
```

## Comparing `codelimit-0.9.0.tar` & `codelimit-0.9.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    32423 2024-04-18 08:41:12.145831 codelimit-0.9.0/LICENSE
--rw-r--r--   0        0        0     2697 2024-04-18 08:41:12.145831 codelimit-0.9.0/README.md
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/__init__.py
--rwxr-xr-x   0        0        0     2253 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/__main__.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/__init__.py
--rw-r--r--   0        0        0     1457 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/app.py
--rw-r--r--   0        0        0     1942 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/check.py
--rw-r--r--   0        0        0     1457 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/report.py
--rw-r--r--   0        0        0     1303 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/scan.py
--rw-r--r--   0        0        0     1211 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/commands/upload.py
--rw-r--r--   0        0        0     1627 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/CheckResult.py
--rw-r--r--   0        0        0     2303 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Codebase.py
--rw-r--r--   0        0        0      503 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/CodebseEntry.py
--rw-r--r--   0        0        0      566 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Configuration.py
--rw-r--r--   0        0        0      559 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Language.py
--rw-r--r--   0        0        0      643 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/LanguageTotals.py
--rw-r--r--   0        0        0     1166 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Location.py
--rw-r--r--   0        0        0      186 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/Measurement.py
--rw-r--r--   0        0        0     1581 2024-04-18 08:41:12.145831 codelimit-0.9.0/codelimit/common/ScanResultTable.py
--rw-r--r--   0        0        0     1406 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/ScanTotals.py
--rw-r--r--   0        0        0     7181 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/Scanner.py
--rw-r--r--   0        0        0      331 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFile.py
--rw-r--r--   0        0        0      873 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFileEntry.py
--rw-r--r--   0        0        0      535 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFolder.py
--rw-r--r--   0        0        0      255 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/SourceFolderEntry.py
--rw-r--r--   0        0        0     1333 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/Token.py
--rw-r--r--   0        0        0     1256 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/TokenRange.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/Expression.py
--rw-r--r--   0        0        0      453 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/Pattern.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/__init__.py
--rw-r--r--   0        0        0      263 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/Automata.py
--rw-r--r--   0        0        0      450 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/DFA.py
--rw-r--r--   0        0        0      444 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/NFA.py
--rw-r--r--   0        0        0      876 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/State.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/automata/__init__.py
--rw-r--r--   0        0        0     3825 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/matcher.py
--rw-r--r--   0        0        0      721 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Atom.py
--rw-r--r--   0        0        0      389 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Concat.py
--rw-r--r--   0        0        0      702 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/OneOrMore.py
--rw-r--r--   0        0        0      182 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Operator.py
--rw-r--r--   0        0        0      701 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Optional.py
--rw-r--r--   0        0        0      854 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/Union.py
--rw-r--r--   0        0        0      714 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/ZeroOrMore.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/operator/__init__.py
--rw-r--r--   0        0        0      521 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/predicate/Identity.py
--rw-r--r--   0        0        0      336 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/predicate/Predicate.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/predicate/__init__.py
--rw-r--r--   0        0        0     2032 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/gsm/utils.py
--rw-r--r--   0        0        0     1013 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/lexer_utils.py
--rw-r--r--   0        0        0     1583 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/Report.py
--rw-r--r--   0        0        0     1343 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/ReportReader.py
--rw-r--r--   0        0        0      162 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/ReportUnit.py
--rw-r--r--   0        0        0     5087 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/ReportWriter.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/report/__init__.py
--rw-r--r--   0        0        0      155 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/Header.py
--rw-r--r--   0        0        0     1227 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/Scope.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/__init__.py
--rw-r--r--   0        0        0     5506 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/scope/scope_utils.py
--rw-r--r--   0        0        0     2083 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/source_utils.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/__init__.py
--rw-r--r--   0        0        0     1404 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Balanced.py
--rw-r--r--   0        0        0      875 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Choice.py
--rw-r--r--   0        0        0      659 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Keyword.py
--rw-r--r--   0        0        0      444 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Name.py
--rw-r--r--   0        0        0      635 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Operator.py
--rw-r--r--   0        0        0      629 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/Symbol.py
--rw-r--r--   0        0        0      364 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/TokenPredicate.py
--rw-r--r--   0        0        0      628 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/TokenValue.py
--rw-r--r--   0        0        0        0 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_matching/predicate/__init__.py
--rw-r--r--   0        0        0     1621 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/token_utils.py
--rw-r--r--   0        0        0     5762 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/common/utils.py
--rw-r--r--   0        0        0     3139 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/github_auth.py
--rw-r--r--   0        0        0      926 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/C.py
--rw-r--r--   0        0        0      858 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/Cpp.py
--rw-r--r--   0        0        0      707 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/Java.py
--rw-r--r--   0        0        0     1086 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/JavaScript.py
--rw-r--r--   0        0        0     3018 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/Python.py
--rw-r--r--   0        0        0     1610 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/TypeScript.py
--rw-r--r--   0        0        0      178 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/languages/__init__.py
--rw-r--r--   0        0        0     1911 2024-04-18 08:41:12.149831 codelimit-0.9.0/codelimit/utils.py
--rw-r--r--   0        0        0       18 2024-04-18 08:41:37.982332 codelimit-0.9.0/codelimit/version.py
--rw-r--r--   0        0        0     1124 2024-04-18 08:41:37.982332 codelimit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 codelimit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    32423 2024-04-18 21:26:50.771452 codelimit-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2710 2024-04-18 21:26:50.771452 codelimit-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/__init__.py
+-rwxr-xr-x   0        0        0     2253 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/commands/__init__.py
+-rw-r--r--   0        0        0     1457 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/commands/app.py
+-rw-r--r--   0        0        0     1942 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/commands/check.py
+-rw-r--r--   0        0        0     1457 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/commands/report.py
+-rw-r--r--   0        0        0     1303 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/commands/scan.py
+-rw-r--r--   0        0        0     1211 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/commands/upload.py
+-rw-r--r--   0        0        0     1627 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/CheckResult.py
+-rw-r--r--   0        0        0     2303 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Codebase.py
+-rw-r--r--   0        0        0      503 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/CodebseEntry.py
+-rw-r--r--   0        0        0      566 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Configuration.py
+-rw-r--r--   0        0        0      559 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Language.py
+-rw-r--r--   0        0        0      643 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/LanguageTotals.py
+-rw-r--r--   0        0        0     1166 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Location.py
+-rw-r--r--   0        0        0      186 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Measurement.py
+-rw-r--r--   0        0        0     1581 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/ScanResultTable.py
+-rw-r--r--   0        0        0     1406 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/ScanTotals.py
+-rw-r--r--   0        0        0     7184 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Scanner.py
+-rw-r--r--   0        0        0      331 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/SourceFile.py
+-rw-r--r--   0        0        0      873 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/SourceFileEntry.py
+-rw-r--r--   0        0        0      535 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/SourceFolder.py
+-rw-r--r--   0        0        0      255 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/SourceFolderEntry.py
+-rw-r--r--   0        0        0     1333 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/Token.py
+-rw-r--r--   0        0        0     1256 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/TokenRange.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/Expression.py
+-rw-r--r--   0        0        0      453 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/Pattern.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/automata/Automata.py
+-rw-r--r--   0        0        0      450 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/automata/DFA.py
+-rw-r--r--   0        0        0      444 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/automata/NFA.py
+-rw-r--r--   0        0        0      876 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/automata/State.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/automata/__init__.py
+-rw-r--r--   0        0        0     3825 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/matcher.py
+-rw-r--r--   0        0        0      721 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/Atom.py
+-rw-r--r--   0        0        0      389 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/Concat.py
+-rw-r--r--   0        0        0      702 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/OneOrMore.py
+-rw-r--r--   0        0        0      182 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/Operator.py
+-rw-r--r--   0        0        0      701 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/Optional.py
+-rw-r--r--   0        0        0      854 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/Union.py
+-rw-r--r--   0        0        0      714 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/ZeroOrMore.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/operator/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/predicate/Identity.py
+-rw-r--r--   0        0        0      336 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/predicate/Predicate.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/predicate/__init__.py
+-rw-r--r--   0        0        0     2032 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/gsm/utils.py
+-rw-r--r--   0        0        0     1013 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/lexer_utils.py
+-rw-r--r--   0        0        0     1583 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/report/Report.py
+-rw-r--r--   0        0        0     1343 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/report/ReportReader.py
+-rw-r--r--   0        0        0      162 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/report/ReportUnit.py
+-rw-r--r--   0        0        0     5087 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/report/ReportWriter.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/report/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/scope/Header.py
+-rw-r--r--   0        0        0     1227 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/scope/Scope.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/scope/__init__.py
+-rw-r--r--   0        0        0     5506 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/scope/scope_utils.py
+-rw-r--r--   0        0        0     2083 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/source_utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/__init__.py
+-rw-r--r--   0        0        0     1404 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/Balanced.py
+-rw-r--r--   0        0        0      875 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/Choice.py
+-rw-r--r--   0        0        0      659 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/Keyword.py
+-rw-r--r--   0        0        0      444 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/Name.py
+-rw-r--r--   0        0        0      635 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/Operator.py
+-rw-r--r--   0        0        0      629 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/Symbol.py
+-rw-r--r--   0        0        0      364 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/TokenPredicate.py
+-rw-r--r--   0        0        0      628 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/TokenValue.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_matching/predicate/__init__.py
+-rw-r--r--   0        0        0     1621 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/token_utils.py
+-rw-r--r--   0        0        0     5762 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/common/utils.py
+-rw-r--r--   0        0        0     3139 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/github_auth.py
+-rw-r--r--   0        0        0      926 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/C.py
+-rw-r--r--   0        0        0      858 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/Cpp.py
+-rw-r--r--   0        0        0      707 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/Java.py
+-rw-r--r--   0        0        0     1086 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/JavaScript.py
+-rw-r--r--   0        0        0     3018 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/Python.py
+-rw-r--r--   0        0        0     1610 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/TypeScript.py
+-rw-r--r--   0        0        0      236 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/languages/__init__.py
+-rw-r--r--   0        0        0     1911 2024-04-18 21:26:50.771452 codelimit-0.9.1/codelimit/utils.py
+-rw-r--r--   0        0        0       18 2024-04-18 21:27:18.463529 codelimit-0.9.1/codelimit/version.py
+-rw-r--r--   0        0        0     1154 2024-04-18 21:27:18.463529 codelimit-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 codelimit-0.9.1/PKG-INFO
```

### Comparing `codelimit-0.9.0/LICENSE` & `codelimit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/README.md` & `codelimit-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,9 +59,9 @@
 
 ```
 ![Checked with Code Limit](https://img.shields.io/badge/Code%20Limit-checked-green.svg)](https://github.com/getcodelimit/codelimit)
 ```
 
 ## License
 
-[ISC](LICENSE) © 2022 Rob van der Leek <robvanderleek@gmail.com>
+[GPL-3.0-or-later](LICENSE) © 2022 Rob van der Leek <robvanderleek@gmail.com>
 (https://twitter.com/robvanderleek)
```

### Comparing `codelimit-0.9.0/codelimit/__main__.py` & `codelimit-0.9.1/codelimit/__main__.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/commands/app.py` & `codelimit-0.9.1/codelimit/commands/app.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/commands/check.py` & `codelimit-0.9.1/codelimit/commands/check.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/commands/report.py` & `codelimit-0.9.1/codelimit/commands/report.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/commands/scan.py` & `codelimit-0.9.1/codelimit/commands/scan.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/commands/upload.py` & `codelimit-0.9.1/codelimit/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/CheckResult.py` & `codelimit-0.9.1/codelimit/common/CheckResult.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/Codebase.py` & `codelimit-0.9.1/codelimit/common/Codebase.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/Configuration.py` & `codelimit-0.9.1/codelimit/common/Configuration.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/Language.py` & `codelimit-0.9.1/codelimit/common/Language.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/LanguageTotals.py` & `codelimit-0.9.1/codelimit/common/LanguageTotals.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/Location.py` & `codelimit-0.9.1/codelimit/common/Location.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/ScanResultTable.py` & `codelimit-0.9.1/codelimit/common/ScanResultTable.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/ScanTotals.py` & `codelimit-0.9.1/codelimit/common/ScanTotals.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/Scanner.py` & `codelimit-0.9.1/codelimit/common/Scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pathspec import PathSpec
 from pygments.lexer import Lexer
 from pygments.lexers import get_lexer_for_filename
 from pygments.util import ClassNotFound
 from rich import print
 from rich.live import Live
 
+from codelimit import languages
 from codelimit.common.Codebase import Codebase
 from codelimit.common.Configuration import Configuration
 from codelimit.common.Language import Language
 from codelimit.common.Location import Location
 from codelimit.common.Measurement import Measurement
 from codelimit.common.ScanResultTable import ScanResultTable
 from codelimit.common.ScanTotals import ScanTotals
@@ -27,15 +28,14 @@
 from codelimit.common.scope.Scope import count_lines
 from codelimit.common.scope.scope_utils import build_scopes, unfold_scopes
 from codelimit.common.source_utils import filter_tokens
 from codelimit.common.utils import (
     calculate_checksum,
     load_language_by_name,
 )
-from codelimit.languages import LanguageName
 from codelimit.version import version
 
 locale.setlocale(locale.LC_ALL, "")
 
 
 def scan_codebase(path: Path, cached_report: Union[Report, None] = None) -> Codebase:
     codebase = Codebase(str(path.resolve().absolute()))
@@ -95,17 +95,17 @@
             rel_path = Path(os.path.join(root, file)).relative_to(folder.absolute())
             if is_excluded(rel_path) or (
                     gitignore is not None and is_excluded_by_gitignore(rel_path, gitignore)
             ):
                 continue
             try:
                 lexer = get_lexer_for_filename(rel_path)
-                language = lexer.__class__.name
+                lexer_name = lexer.__class__.name
                 file_path = os.path.join(root, file)
-                if language in LanguageName:
+                if lexer_name in languages.language_names:
                     file_entry = _scan_file(
                         codebase, lexer, folder, file_path, cached_report
                     )
                     if add_file_entry:
                         add_file_entry(file_entry)
             except ClassNotFound:
                 pass
```

### Comparing `codelimit-0.9.0/codelimit/common/SourceFileEntry.py` & `codelimit-0.9.1/codelimit/common/SourceFileEntry.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/SourceFolder.py` & `codelimit-0.9.1/codelimit/common/SourceFolder.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/Token.py` & `codelimit-0.9.1/codelimit/common/Token.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/TokenRange.py` & `codelimit-0.9.1/codelimit/common/TokenRange.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/Expression.py` & `codelimit-0.9.1/codelimit/common/gsm/Expression.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/automata/State.py` & `codelimit-0.9.1/codelimit/common/gsm/automata/State.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/matcher.py` & `codelimit-0.9.1/codelimit/common/gsm/matcher.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/operator/Atom.py` & `codelimit-0.9.1/codelimit/common/gsm/operator/Atom.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/operator/OneOrMore.py` & `codelimit-0.9.1/codelimit/common/gsm/operator/OneOrMore.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/operator/Optional.py` & `codelimit-0.9.1/codelimit/common/gsm/operator/Optional.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/operator/Union.py` & `codelimit-0.9.1/codelimit/common/gsm/operator/Union.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/operator/ZeroOrMore.py` & `codelimit-0.9.1/codelimit/common/gsm/operator/ZeroOrMore.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/predicate/Identity.py` & `codelimit-0.9.1/codelimit/common/gsm/predicate/Identity.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/gsm/utils.py` & `codelimit-0.9.1/codelimit/common/gsm/utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/lexer_utils.py` & `codelimit-0.9.1/codelimit/common/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/report/Report.py` & `codelimit-0.9.1/codelimit/common/report/Report.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/report/ReportReader.py` & `codelimit-0.9.1/codelimit/common/report/ReportReader.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/report/ReportWriter.py` & `codelimit-0.9.1/codelimit/common/report/ReportWriter.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/scope/Scope.py` & `codelimit-0.9.1/codelimit/common/scope/Scope.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/scope/scope_utils.py` & `codelimit-0.9.1/codelimit/common/scope/scope_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/source_utils.py` & `codelimit-0.9.1/codelimit/common/source_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_matching/predicate/Balanced.py` & `codelimit-0.9.1/codelimit/common/token_matching/predicate/Balanced.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_matching/predicate/Choice.py` & `codelimit-0.9.1/codelimit/common/token_matching/predicate/Choice.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_matching/predicate/Keyword.py` & `codelimit-0.9.1/codelimit/common/token_matching/predicate/Keyword.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_matching/predicate/Operator.py` & `codelimit-0.9.1/codelimit/common/token_matching/predicate/Operator.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_matching/predicate/Symbol.py` & `codelimit-0.9.1/codelimit/common/token_matching/predicate/Symbol.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_matching/predicate/TokenValue.py` & `codelimit-0.9.1/codelimit/common/token_matching/predicate/TokenValue.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/token_utils.py` & `codelimit-0.9.1/codelimit/common/token_utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/common/utils.py` & `codelimit-0.9.1/codelimit/common/utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/github_auth.py` & `codelimit-0.9.1/codelimit/github_auth.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/languages/C.py` & `codelimit-0.9.1/codelimit/languages/C.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/languages/Cpp.py` & `codelimit-0.9.1/codelimit/languages/Cpp.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/languages/Java.py` & `codelimit-0.9.1/codelimit/languages/Java.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/languages/JavaScript.py` & `codelimit-0.9.1/codelimit/languages/JavaScript.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/languages/Python.py` & `codelimit-0.9.1/codelimit/languages/Python.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/languages/TypeScript.py` & `codelimit-0.9.1/codelimit/languages/TypeScript.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/codelimit/utils.py` & `codelimit-0.9.1/codelimit/utils.py`

 * *Files identical despite different names*

### Comparing `codelimit-0.9.0/pyproject.toml` & `codelimit-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "codelimit"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Rob van der Leek <robvanderleek@gmail.com>"]
+license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 codelimit = "codelimit.__main__:cli"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.10,<3.13"
 pygments = "^2.13.0"
 requests = "^2.28.2"
 typer = "^0.9.0"
 aiohttp = "^3.9.0"
 pyyaml = "^6.0.1"
 rich = "^13.7.1"
 pathspec = "^0.12.1"
```

### Comparing `codelimit-0.9.0/PKG-INFO` & `codelimit-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: codelimit
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
+License: GPL-3.0-or-later
 Author: Rob van der Leek
 Author-email: robvanderleek@gmail.com
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.13
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
 Requires-Dist: pathspec (>=0.12.1,<0.13.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
@@ -80,10 +81,10 @@
 
 ```
 ![Checked with Code Limit](https://img.shields.io/badge/Code%20Limit-checked-green.svg)](https://github.com/getcodelimit/codelimit)
 ```
 
 ## License
 
-[ISC](LICENSE) © 2022 Rob van der Leek <robvanderleek@gmail.com>
+[GPL-3.0-or-later](LICENSE) © 2022 Rob van der Leek <robvanderleek@gmail.com>
 (https://twitter.com/robvanderleek)
```

