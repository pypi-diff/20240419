# Comparing `tmp/nero-19.3b5.tar.gz` & `tmp/nero-19.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nero-19.3b5.tar", last modified: Tue Oct 22 21:21:07 2019, max compression
+gzip compressed data, was "dist/nero-19.3b6.tar", last modified: Sun Oct 27 18:24:13 2019, max compression
```

## Comparing `nero-19.3b5.tar` & `nero-19.3b6.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      649 2019-08-15 20:57:35.000000 nero-19.3b5/.appveyor.yml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       49 2019-08-15 20:57:35.000000 nero-19.3b5/.coveragerc
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      107 2019-08-15 20:57:35.000000 nero-19.3b5/.flake8
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/.github/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      556 2019-08-15 20:57:35.000000 nero-19.3b5/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      606 2019-08-15 20:57:35.000000 nero-19.3b5/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      146 2019-10-19 01:50:43.000000 nero-19.3b5/.gitignore
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      518 2019-08-15 20:57:35.000000 nero-19.3b5/.pre-commit-config.yaml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      210 2019-08-15 20:57:35.000000 nero-19.3b5/.pre-commit-hooks.yaml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1722 2019-10-19 01:50:43.000000 nero-19.3b5/.travis.yml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1931 2019-10-19 01:50:43.000000 nero-19.3b5/CONTRIBUTING.md
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1080 2019-08-15 20:57:35.000000 nero-19.3b5/LICENSE
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      140 2019-08-15 20:57:35.000000 nero-19.3b5/MANIFEST.in
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    69177 2019-10-22 21:21:07.000000 nero-19.3b5/PKG-INFO
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      641 2019-10-19 01:50:43.000000 nero-19.3b5/Pipfile
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    36174 2019-10-19 01:50:43.000000 nero-19.3b5/Pipfile.lock
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    55785 2019-10-22 21:11:07.000000 nero-19.3b5/README.md
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       45 2019-10-22 21:10:09.000000 nero-19.3b5/_version.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   138300 2019-10-19 01:50:43.000000 nero-19.3b5/black.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6077 2019-10-19 01:50:43.000000 nero-19.3b5/blackd.py
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/blib2to3/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     9628 2019-10-19 01:50:43.000000 nero-19.3b5/blib2to3/Grammar.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    12762 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/LICENSE
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      793 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/PatternGrammar.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      587 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/README
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        7 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/__init__.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       33 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/__init__.pyi
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/blib2to3/pgen2/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      143 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/__init__.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      184 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/__init__.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     9651 2019-10-19 01:50:43.000000 nero-19.3b5/blib2to3/pgen2/conv.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     7760 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/driver.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1053 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/driver.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     5800 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/grammar.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      811 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/grammar.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1644 2019-10-19 01:50:43.000000 nero-19.3b5/blib2to3/pgen2/literals.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      216 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/literals.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     8053 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/parse.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1162 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/parse.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    13812 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/pgen.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2186 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/pgen.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1277 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/token.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1127 2019-10-19 01:50:43.000000 nero-19.3b5/blib2to3/pgen2/token.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    21458 2019-10-19 01:50:43.000000 nero-19.3b5/blib2to3/pgen2/tokenize.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1073 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pgen2/tokenize.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2194 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pygram.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2630 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pygram.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    28543 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pytree.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3340 2019-08-15 20:57:35.000000 nero-19.3b5/blib2to3/pytree.pyi
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/docs/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      602 2019-08-15 20:57:35.000000 nero-19.3b5/docs/Makefile
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/docs/_static/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      949 2019-08-15 20:57:35.000000 nero-19.3b5/docs/_static/license.svg
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    80754 2019-08-15 20:57:35.000000 nero-19.3b5/docs/_static/logo2-readme.png
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   128768 2019-08-15 20:57:35.000000 nero-19.3b5/docs/_static/logo2.png
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      954 2019-08-15 20:57:35.000000 nero-19.3b5/docs/_static/pypi_template.svg
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     8166 2019-10-19 01:50:43.000000 nero-19.3b5/docs/conf.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1931 2019-10-19 01:50:43.000000 nero-19.3b5/docs/contributing.md
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      189 2019-10-19 01:50:43.000000 nero-19.3b5/docs/environment.yml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1880 2019-08-15 20:57:35.000000 nero-19.3b5/docs/index.rst
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      773 2019-08-15 20:57:35.000000 nero-19.3b5/docs/make.bat
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/docs/reference/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1159 2019-08-15 20:57:35.000000 nero-19.3b5/docs/reference/reference_classes.rst
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      217 2019-08-15 20:57:35.000000 nero-19.3b5/docs/reference/reference_exceptions.rst
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3536 2019-08-15 20:57:35.000000 nero-19.3b5/docs/reference/reference_functions.rst
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      174 2019-08-15 20:57:35.000000 nero-19.3b5/docs/reference/reference_summary.rst
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       34 2019-08-15 20:57:35.000000 nero-19.3b5/docs/requirements.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      819 2019-10-19 01:50:43.000000 nero-19.3b5/mypy.ini
--rwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)     3577 2019-10-22 21:11:07.000000 nero-19.3b5/nero
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    69177 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/PKG-INFO
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3548 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/SOURCES.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        1 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/dependency_links.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       79 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/entry_points.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        1 2019-10-22 21:12:51.000000 nero-19.3b5/nero.egg-info/not-zip-safe
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      107 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/requires.txt
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       31 2019-10-22 21:21:07.000000 nero-19.3b5/nero.egg-info/top_level.txt
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/plugin/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4150 2019-08-15 20:57:35.000000 nero-19.3b5/plugin/black.vim
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/profiling/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   215971 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/dict_big.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)  1118824 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/dict_huge.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   159994 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/list_big.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   897234 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/list_huge.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   184224 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/mix_big.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)  1406108 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/mix_huge.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    18306 2019-08-15 20:57:35.000000 nero-19.3b5/profiling/mix_small.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    32406 2019-08-15 20:57:35.000000 nero-19.3b5/pyproject.lock
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2238 2019-10-19 01:50:43.000000 nero-19.3b5/pyproject.toml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       84 2019-08-15 20:57:35.000000 nero-19.3b5/readthedocs.yml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      114 2019-10-22 21:21:07.000000 nero-19.3b5/setup.cfg
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2079 2019-10-22 21:20:38.000000 nero-19.3b5/setup.py
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/data/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      495 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/async_as_identifier.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       63 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/beginning_backslash.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      333 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/bracketmatch.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4057 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/cantfit.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1091 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/class_blank_parentheses.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4318 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/class_methods_new_line.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      212 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/comment_after_escaped_newline.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1858 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/comments.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     7226 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/comments2.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1570 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/comments3.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3721 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/comments4.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1194 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/comments5.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2471 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/comments6.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2533 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/comments7.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     5534 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/composition.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    15604 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/debug_visitor.out
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1193 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/debug_visitor.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4597 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/empty_lines.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       99 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/empty_pyproject.toml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    13433 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/expression.diff
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    16823 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/expression.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     9326 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/fmtonoff.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      604 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/fmtonoff2.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      598 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/force_py36.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       62 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/force_pyi.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      815 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/fstring.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6403 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/function.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1149 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/function2.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      103 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/function_trailing_comma.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2469 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/import_spacing.py
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/data/include_exclude_tests/
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/data/include_exclude_tests/b/
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/data/include_exclude_tests/b/.definitely_exclude/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/data/include_exclude_tests/b/dont_exclude/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
-drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-22 21:21:07.000000 nero-19.3b5/tests/data/include_exclude_tests/b/exclude/
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/exclude/a.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      597 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/numeric_literals.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      176 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/numeric_literals_py2.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      267 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/numeric_literals_skip_underscores.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      680 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/pep_570.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      905 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/pep_572.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      604 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/python2.py
--rwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)      250 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/python2_print_function.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      433 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/python2_unicode_literals.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1199 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/python37.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2693 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/remove_parens.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      789 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/slices.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      150 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/string_prefixes.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1922 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/string_quotes.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      315 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/stub.pyi
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       61 2019-10-19 01:50:43.000000 nero-19.3b5/tests/data/tricky_unicode_symbols.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      228 2019-08-15 20:57:35.000000 nero-19.3b5/tests/data/tupleassign.py
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       89 2019-08-15 20:57:35.000000 nero-19.3b5/tests/empty.toml
--rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    70414 2019-10-19 01:50:43.000000 nero-19.3b5/tests/test_black.py
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      649 2019-08-15 20:57:35.000000 nero-19.3b6/.appveyor.yml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       49 2019-08-15 20:57:35.000000 nero-19.3b6/.coveragerc
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      107 2019-08-15 20:57:35.000000 nero-19.3b6/.flake8
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/.github/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      556 2019-08-15 20:57:35.000000 nero-19.3b6/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      606 2019-08-15 20:57:35.000000 nero-19.3b6/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      146 2019-10-19 01:50:43.000000 nero-19.3b6/.gitignore
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      518 2019-08-15 20:57:35.000000 nero-19.3b6/.pre-commit-config.yaml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      210 2019-08-15 20:57:35.000000 nero-19.3b6/.pre-commit-hooks.yaml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1722 2019-10-19 01:50:43.000000 nero-19.3b6/.travis.yml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1931 2019-10-19 01:50:43.000000 nero-19.3b6/CONTRIBUTING.md
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1080 2019-08-15 20:57:35.000000 nero-19.3b6/LICENSE
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      140 2019-08-15 20:57:35.000000 nero-19.3b6/MANIFEST.in
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    69178 2019-10-27 18:24:13.000000 nero-19.3b6/PKG-INFO
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      641 2019-10-19 01:50:43.000000 nero-19.3b6/Pipfile
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    36174 2019-10-19 01:50:43.000000 nero-19.3b6/Pipfile.lock
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    55785 2019-10-22 21:11:07.000000 nero-19.3b6/README.md
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       45 2019-10-22 21:10:09.000000 nero-19.3b6/_version.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   138300 2019-10-19 01:50:43.000000 nero-19.3b6/black.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6077 2019-10-19 01:50:43.000000 nero-19.3b6/blackd.py
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/blib2to3/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     9628 2019-10-19 01:50:43.000000 nero-19.3b6/blib2to3/Grammar.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    12762 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/LICENSE
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      793 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/PatternGrammar.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      587 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/README
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        7 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/__init__.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       33 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/__init__.pyi
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/blib2to3/pgen2/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      143 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/__init__.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      184 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/__init__.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     9651 2019-10-19 01:50:43.000000 nero-19.3b6/blib2to3/pgen2/conv.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     7760 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/driver.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1053 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/driver.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     5800 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/grammar.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      811 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/grammar.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1644 2019-10-19 01:50:43.000000 nero-19.3b6/blib2to3/pgen2/literals.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      216 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/literals.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     8053 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/parse.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1162 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/parse.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    13812 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/pgen.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2186 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/pgen.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1277 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/token.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1127 2019-10-19 01:50:43.000000 nero-19.3b6/blib2to3/pgen2/token.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    21458 2019-10-19 01:50:43.000000 nero-19.3b6/blib2to3/pgen2/tokenize.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1073 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pgen2/tokenize.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2194 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pygram.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2630 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pygram.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    28543 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pytree.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3340 2019-08-15 20:57:35.000000 nero-19.3b6/blib2to3/pytree.pyi
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/docs/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      602 2019-08-15 20:57:35.000000 nero-19.3b6/docs/Makefile
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/docs/_static/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      949 2019-08-15 20:57:35.000000 nero-19.3b6/docs/_static/license.svg
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    80754 2019-08-15 20:57:35.000000 nero-19.3b6/docs/_static/logo2-readme.png
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   128768 2019-08-15 20:57:35.000000 nero-19.3b6/docs/_static/logo2.png
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      954 2019-08-15 20:57:35.000000 nero-19.3b6/docs/_static/pypi_template.svg
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     8166 2019-10-19 01:50:43.000000 nero-19.3b6/docs/conf.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1931 2019-10-19 01:50:43.000000 nero-19.3b6/docs/contributing.md
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      189 2019-10-19 01:50:43.000000 nero-19.3b6/docs/environment.yml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1880 2019-08-15 20:57:35.000000 nero-19.3b6/docs/index.rst
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      773 2019-08-15 20:57:35.000000 nero-19.3b6/docs/make.bat
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/docs/reference/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1159 2019-08-15 20:57:35.000000 nero-19.3b6/docs/reference/reference_classes.rst
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      217 2019-08-15 20:57:35.000000 nero-19.3b6/docs/reference/reference_exceptions.rst
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3536 2019-08-15 20:57:35.000000 nero-19.3b6/docs/reference/reference_functions.rst
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      174 2019-08-15 20:57:35.000000 nero-19.3b6/docs/reference/reference_summary.rst
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       34 2019-08-15 20:57:35.000000 nero-19.3b6/docs/requirements.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      819 2019-10-19 01:50:43.000000 nero-19.3b6/mypy.ini
+-rwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)     3577 2019-10-22 21:11:07.000000 nero-19.3b6/nero
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/nero.egg-info/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    69178 2019-10-27 18:24:12.000000 nero-19.3b6/nero.egg-info/PKG-INFO
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3548 2019-10-27 18:24:13.000000 nero-19.3b6/nero.egg-info/SOURCES.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        1 2019-10-27 18:24:12.000000 nero-19.3b6/nero.egg-info/dependency_links.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       79 2019-10-27 18:24:12.000000 nero-19.3b6/nero.egg-info/entry_points.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        1 2019-10-22 21:12:51.000000 nero-19.3b6/nero.egg-info/not-zip-safe
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      107 2019-10-27 18:24:12.000000 nero-19.3b6/nero.egg-info/requires.txt
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       31 2019-10-27 18:24:12.000000 nero-19.3b6/nero.egg-info/top_level.txt
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/plugin/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4150 2019-08-15 20:57:35.000000 nero-19.3b6/plugin/black.vim
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/profiling/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   215971 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/dict_big.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)  1118824 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/dict_huge.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   159994 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/list_big.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   897234 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/list_huge.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)   184224 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/mix_big.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)  1406108 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/mix_huge.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    18306 2019-08-15 20:57:35.000000 nero-19.3b6/profiling/mix_small.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    32406 2019-08-15 20:57:35.000000 nero-19.3b6/pyproject.lock
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2238 2019-10-19 01:50:43.000000 nero-19.3b6/pyproject.toml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       84 2019-08-15 20:57:35.000000 nero-19.3b6/readthedocs.yml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      114 2019-10-27 18:24:13.000000 nero-19.3b6/setup.cfg
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2080 2019-10-27 18:23:08.000000 nero-19.3b6/setup.py
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/data/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      495 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/async_as_identifier.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       63 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/beginning_backslash.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      333 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/bracketmatch.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4057 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/cantfit.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1091 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/class_blank_parentheses.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4318 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/class_methods_new_line.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      212 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/comment_after_escaped_newline.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1858 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/comments.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     7226 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/comments2.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1570 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/comments3.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     3721 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/comments4.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1194 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/comments5.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2471 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/comments6.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2533 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/comments7.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     5534 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/composition.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    15604 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/debug_visitor.out
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1193 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/debug_visitor.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     4597 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/empty_lines.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       99 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/empty_pyproject.toml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    13433 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/expression.diff
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    16823 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/expression.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     9326 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/fmtonoff.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      604 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/fmtonoff2.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      598 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/force_py36.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       62 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/force_pyi.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      815 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/fstring.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     6403 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/function.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1149 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/function2.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      103 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/function_trailing_comma.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2469 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/import_spacing.py
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/data/include_exclude_tests/
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/data/include_exclude_tests/b/
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/data/include_exclude_tests/b/.definitely_exclude/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/data/include_exclude_tests/b/dont_exclude/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+drwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)        0 2019-10-27 18:24:13.000000 nero-19.3b6/tests/data/include_exclude_tests/b/exclude/
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)        0 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      597 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/numeric_literals.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      176 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/numeric_literals_py2.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      267 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/numeric_literals_skip_underscores.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      680 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/pep_570.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      905 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/pep_572.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      604 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/python2.py
+-rwxrwxr-x   0 mgmiller  (1000) mgmiller  (1000)      250 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/python2_print_function.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      433 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/python2_unicode_literals.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1199 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/python37.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     2693 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/remove_parens.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      789 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/slices.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      150 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/string_prefixes.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)     1922 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/string_quotes.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      315 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/stub.pyi
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       61 2019-10-19 01:50:43.000000 nero-19.3b6/tests/data/tricky_unicode_symbols.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)      228 2019-08-15 20:57:35.000000 nero-19.3b6/tests/data/tupleassign.py
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)       89 2019-08-15 20:57:35.000000 nero-19.3b6/tests/empty.toml
+-rw-rw-r--   0 mgmiller  (1000) mgmiller  (1000)    70414 2019-10-19 01:50:43.000000 nero-19.3b6/tests/test_black.py
```

### Comparing `nero-19.3b5/.appveyor.yml` & `nero-19.3b6/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/.github/CODE_OF_CONDUCT.md` & `nero-19.3b6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/.github/ISSUE_TEMPLATE.md` & `nero-19.3b6/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/.pre-commit-config.yaml` & `nero-19.3b6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/.travis.yml` & `nero-19.3b6/.travis.yml`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/CONTRIBUTING.md` & `nero-19.3b6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/LICENSE` & `nero-19.3b6/LICENSE`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/PKG-INFO` & `nero-19.3b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nero
-Version: 19.3b5
+Version: 19.3b6
 Summary: The uncompromising code formatter.  Single quotes version.
 Home-page: https://github.com/mixmastamyk/nero
 Author: black authors
 Author-email: 
 License: MIT
 Description: 
         <h2 align="center">The Uncompromising Code Formatter</h2>
@@ -1550,15 +1550,15 @@
         * [Peter Bengtsson](mailto:mail@peterbe.com)
         * [Stavros Korokithakis](mailto:hi@stavros.io)
         * [Sunil Kapil](mailto:snlkapil@gmail.com)
         * [Utsav Shah](mailto:ukshah2@illinois.edu)
         * [Vishwas B Sharma](mailto:sharma.vishwas88@gmail.com)
         * [Chuck Wooters](mailto:chuck.wooters@microsoft.com)
         
-Keywords: automation formatter yapf autopep8 pyfmt gofmt rustfmtblack single quotes
+Keywords: automation formatter yapf autopep8 pyfmt gofmt rustfmt black single quotes
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nero Version: 19.3b5 Summary: The uncompromising
+Metadata-Version: 2.1 Name: nero Version: 19.3b6 Summary: The uncompromising
 code formatter. Single quotes version. Home-page: https://github.com/
 mixmastamyk/nero Author: black authors Author-email: License: MIT Description:
                  ********** TThhee UUnnccoommpprroommiissiinngg CCooddee FFoorrmmaatttteerr **********
    _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_P_y_P_I_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 > âAny color you like.â
 ********** PPyytthhoonn NNeerroo **********
@@ -684,15 +684,15 @@
 miggaiowski@gmail.com) * [Miroslav Shubernetskiy](mailto:miroslav@miki725.com)
 * [Neraste](mailto:neraste.herr10@gmail.com) * [Osaetin Daniel](mailto:
 osaetindaniel@gmail.com) * [Peter Bengtsson](mailto:mail@peterbe.com) *
 [Stavros Korokithakis](mailto:hi@stavros.io) * [Sunil Kapil](mailto:
 snlkapil@gmail.com) * [Utsav Shah](mailto:ukshah2@illinois.edu) * [Vishwas B
 Sharma](mailto:sharma.vishwas88@gmail.com) * [Chuck Wooters](mailto:
 chuck.wooters@microsoft.com) Keywords: automation formatter yapf autopep8 pyfmt
-gofmt rustfmtblack single quotes Platform: UNKNOWN Classifier: Development
+gofmt rustfmt black single quotes Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `nero-19.3b5/Pipfile` & `nero-19.3b6/Pipfile`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/Pipfile.lock` & `nero-19.3b6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/README.md` & `nero-19.3b6/README.md`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/black.py` & `nero-19.3b6/black.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blackd.py` & `nero-19.3b6/blackd.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/Grammar.txt` & `nero-19.3b6/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/LICENSE` & `nero-19.3b6/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/PatternGrammar.txt` & `nero-19.3b6/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/README` & `nero-19.3b6/blib2to3/README`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/conv.py` & `nero-19.3b6/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/driver.py` & `nero-19.3b6/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/driver.pyi` & `nero-19.3b6/blib2to3/pgen2/driver.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/grammar.py` & `nero-19.3b6/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/grammar.pyi` & `nero-19.3b6/blib2to3/pgen2/grammar.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/literals.py` & `nero-19.3b6/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/parse.py` & `nero-19.3b6/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/parse.pyi` & `nero-19.3b6/blib2to3/pgen2/parse.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/pgen.py` & `nero-19.3b6/blib2to3/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/pgen.pyi` & `nero-19.3b6/blib2to3/pgen2/pgen.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/token.py` & `nero-19.3b6/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/token.pyi` & `nero-19.3b6/blib2to3/pgen2/token.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/tokenize.py` & `nero-19.3b6/blib2to3/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pgen2/tokenize.pyi` & `nero-19.3b6/blib2to3/pgen2/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pygram.py` & `nero-19.3b6/blib2to3/pygram.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pygram.pyi` & `nero-19.3b6/blib2to3/pygram.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pytree.py` & `nero-19.3b6/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/blib2to3/pytree.pyi` & `nero-19.3b6/blib2to3/pytree.pyi`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/Makefile` & `nero-19.3b6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/_static/license.svg` & `nero-19.3b6/docs/_static/license.svg`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/_static/logo2-readme.png` & `nero-19.3b6/docs/_static/logo2-readme.png`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/_static/logo2.png` & `nero-19.3b6/docs/_static/logo2.png`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/_static/pypi_template.svg` & `nero-19.3b6/docs/_static/pypi_template.svg`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/conf.py` & `nero-19.3b6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/contributing.md` & `nero-19.3b6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/index.rst` & `nero-19.3b6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/make.bat` & `nero-19.3b6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/reference/reference_classes.rst` & `nero-19.3b6/docs/reference/reference_classes.rst`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/docs/reference/reference_functions.rst` & `nero-19.3b6/docs/reference/reference_functions.rst`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/mypy.ini` & `nero-19.3b6/mypy.ini`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/nero` & `nero-19.3b6/nero`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/nero.egg-info/PKG-INFO` & `nero-19.3b6/nero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nero
-Version: 19.3b5
+Version: 19.3b6
 Summary: The uncompromising code formatter.  Single quotes version.
 Home-page: https://github.com/mixmastamyk/nero
 Author: black authors
 Author-email: 
 License: MIT
 Description: 
         <h2 align="center">The Uncompromising Code Formatter</h2>
@@ -1550,15 +1550,15 @@
         * [Peter Bengtsson](mailto:mail@peterbe.com)
         * [Stavros Korokithakis](mailto:hi@stavros.io)
         * [Sunil Kapil](mailto:snlkapil@gmail.com)
         * [Utsav Shah](mailto:ukshah2@illinois.edu)
         * [Vishwas B Sharma](mailto:sharma.vishwas88@gmail.com)
         * [Chuck Wooters](mailto:chuck.wooters@microsoft.com)
         
-Keywords: automation formatter yapf autopep8 pyfmt gofmt rustfmtblack single quotes
+Keywords: automation formatter yapf autopep8 pyfmt gofmt rustfmt black single quotes
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nero Version: 19.3b5 Summary: The uncompromising
+Metadata-Version: 2.1 Name: nero Version: 19.3b6 Summary: The uncompromising
 code formatter. Single quotes version. Home-page: https://github.com/
 mixmastamyk/nero Author: black authors Author-email: License: MIT Description:
                  ********** TThhee UUnnccoommpprroommiissiinngg CCooddee FFoorrmmaatttteerr **********
    _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_P_y_P_I_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 > âAny color you like.â
 ********** PPyytthhoonn NNeerroo **********
@@ -684,15 +684,15 @@
 miggaiowski@gmail.com) * [Miroslav Shubernetskiy](mailto:miroslav@miki725.com)
 * [Neraste](mailto:neraste.herr10@gmail.com) * [Osaetin Daniel](mailto:
 osaetindaniel@gmail.com) * [Peter Bengtsson](mailto:mail@peterbe.com) *
 [Stavros Korokithakis](mailto:hi@stavros.io) * [Sunil Kapil](mailto:
 snlkapil@gmail.com) * [Utsav Shah](mailto:ukshah2@illinois.edu) * [Vishwas B
 Sharma](mailto:sharma.vishwas88@gmail.com) * [Chuck Wooters](mailto:
 chuck.wooters@microsoft.com) Keywords: automation formatter yapf autopep8 pyfmt
-gofmt rustfmtblack single quotes Platform: UNKNOWN Classifier: Development
+gofmt rustfmt black single quotes Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `nero-19.3b5/nero.egg-info/SOURCES.txt` & `nero-19.3b6/nero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/plugin/black.vim` & `nero-19.3b6/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/dict_big.py` & `nero-19.3b6/profiling/dict_big.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/dict_huge.py` & `nero-19.3b6/profiling/dict_huge.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/list_big.py` & `nero-19.3b6/profiling/list_big.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/list_huge.py` & `nero-19.3b6/profiling/list_huge.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/mix_big.py` & `nero-19.3b6/profiling/mix_big.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/mix_huge.py` & `nero-19.3b6/profiling/mix_huge.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/profiling/mix_small.py` & `nero-19.3b6/profiling/mix_small.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/pyproject.lock` & `nero-19.3b6/pyproject.lock`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/pyproject.toml` & `nero-19.3b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/setup.py` & `nero-19.3b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     readme_md = CURRENT_DIR / "README.md"
     with open(readme_md, encoding="utf8") as ld_file:
         return ld_file.read()
 
 
 setup(
     name="nero",
-    version="19.3b5",
+    version="19.3b6",
     description="The uncompromising code formatter.  Single quotes version.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
-    keywords="automation formatter yapf autopep8 pyfmt gofmt rustfmt"
+    keywords="automation formatter yapf autopep8 pyfmt gofmt rustfmt "
              "black single quotes",
     author="black authors",
     author_email="",
     url="https://github.com/mixmastamyk/nero",
     license="MIT",
     py_modules=["black", "blackd", "_version"],
     packages=["blib2to3", "blib2to3.pgen2"],
```

### Comparing `nero-19.3b5/tests/data/cantfit.py` & `nero-19.3b6/tests/data/cantfit.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/class_blank_parentheses.py` & `nero-19.3b6/tests/data/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/class_methods_new_line.py` & `nero-19.3b6/tests/data/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments.py` & `nero-19.3b6/tests/data/comments.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments2.py` & `nero-19.3b6/tests/data/comments2.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments3.py` & `nero-19.3b6/tests/data/comments3.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments4.py` & `nero-19.3b6/tests/data/comments4.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments5.py` & `nero-19.3b6/tests/data/comments5.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments6.py` & `nero-19.3b6/tests/data/comments6.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/comments7.py` & `nero-19.3b6/tests/data/comments7.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/composition.py` & `nero-19.3b6/tests/data/composition.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/debug_visitor.out` & `nero-19.3b6/tests/data/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/debug_visitor.py` & `nero-19.3b6/tests/data/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/empty_lines.py` & `nero-19.3b6/tests/data/empty_lines.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/expression.diff` & `nero-19.3b6/tests/data/expression.diff`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/expression.py` & `nero-19.3b6/tests/data/expression.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/fmtonoff.py` & `nero-19.3b6/tests/data/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/fmtonoff2.py` & `nero-19.3b6/tests/data/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/force_py36.py` & `nero-19.3b6/tests/data/force_py36.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/fstring.py` & `nero-19.3b6/tests/data/fstring.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/function.py` & `nero-19.3b6/tests/data/function.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/function2.py` & `nero-19.3b6/tests/data/function2.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/import_spacing.py` & `nero-19.3b6/tests/data/import_spacing.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/numeric_literals.py` & `nero-19.3b6/tests/data/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/pep_570.py` & `nero-19.3b6/tests/data/pep_570.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/pep_572.py` & `nero-19.3b6/tests/data/pep_572.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/python2.py` & `nero-19.3b6/tests/data/python2.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/python37.py` & `nero-19.3b6/tests/data/python37.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/remove_parens.py` & `nero-19.3b6/tests/data/remove_parens.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/slices.py` & `nero-19.3b6/tests/data/slices.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/data/string_quotes.py` & `nero-19.3b6/tests/data/string_quotes.py`

 * *Files identical despite different names*

### Comparing `nero-19.3b5/tests/test_black.py` & `nero-19.3b6/tests/test_black.py`

 * *Files identical despite different names*

