# Comparing `tmp/vokab-0.0.0.tar.gz` & `tmp/vokab-0.0.1.tar.gz`

## Comparing `vokab-0.0.0.tar` & `vokab-0.0.1.tar`

### file list

```diff
@@ -1,51 +1,70 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 vokab-0.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 vokab-0.0.0/LLM.md
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 vokab-0.0.0/Makefile
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 vokab-0.0.0/activate.sh
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 vokab-0.0.0/requirements-dev.txt
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 vokab-0.0.0/requirements.txt
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/admin.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/collection.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/config.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/const.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/database.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/encoder.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/entity.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/flags.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/lazy.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/loader.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/logging.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/searcher.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/cli/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/cli/app.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/cli/init.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/cli/load.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/lancedb/__init__.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/lancedb/database.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/lancedb/table.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/__init__.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/database.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/sql/init_tables.sql
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/sql/init_triggers.sql
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/sql/search.sql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/sql/stats.sql
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/databases/sqlite/sql/upsert.sql
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/encoders/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 vokab-0.0.0/src/vokab/encoders/sbert.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/conftest.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/test_admin.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/test_collection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/test_entity.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/test_loader.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/data/emojis.csv
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/data/emotions.txt
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/data/mixed.jsonl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/data/myths.tsv
--rw-r--r--   0        0        0    17783 2020-02-02 00:00:00.000000 vokab-0.0.0/tests/data/simonw_tags.csv
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 vokab-0.0.0/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 vokab-0.0.0/LICENSE
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 vokab-0.0.0/README.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 vokab-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 vokab-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 vokab-0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 vokab-0.0.1/LLM.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 vokab-0.0.1/Makefile
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 vokab-0.0.1/activate.sh
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 vokab-0.0.1/requirements-dev.txt
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 vokab-0.0.1/requirements.txt
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 vokab-0.0.1/ui.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/__init__.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/collection.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/config.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/const.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/entity.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/lazy.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/loader.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/logging.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/protocol.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/app.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/eval.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/init.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/load.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/reindex.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/abstract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/database.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/entities.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/table.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/terms.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/__init__.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/database.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/exact_search.sql
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/fts_search.sql
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/get_entity.sql
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/init_tables.sql
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/init_triggers.sql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/stats.sql
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/upsert.sql
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/vss_search.sql
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/encoders/__init__.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/encoders/abstract.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/encoders/sbert.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/fuzz/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/fuzz/abstract.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/fuzz/default.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/linkers/__init__.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/linkers/abstract.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/linkers/default.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/rerankers/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/rerankers/abstract.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/rerankers/rrf.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_admin.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_collection.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_config.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_database.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_entity.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_fuzz.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_loader.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_rerank.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/emojis.csv
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/emotions.txt
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/mixed.jsonl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/myths.tsv
+-rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/simonw_tags.csv
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 vokab-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 vokab-0.0.1/LICENSE
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 vokab-0.0.1/README.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 vokab-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 vokab-0.0.1/PKG-INFO
```

### Comparing `vokab-0.0.0/LLM.md` & `vokab-0.0.1/LLM.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# LLM Direction
+# Attention Large Language Model Assistant (Claude, ChatGPT, etc.)
 
 Dear coding assistant, thank you for your help with this project. This document has
 some information that will be useful in helping me write code.
 
 ### Top Level Coding Goals
 
 - Our top priority is creating simple python library with a coding interface that is simple and easy to understand.
 - Code should be highly performance and easy to maintain. 
-- Any backend that supports vector and full-text search should work. We are starting with SQLite and PostgreSQL.
 
 
 ### Pydantic 2 only
 
 - Never recommend Pydantic 1 code.
 - Namespace Updates: Method and attribute names now prefixed with `model_` or follow the `__.*pydantic.*__` pattern.
 - Removal of GenericModel: Directly use `Generic` alongside `BaseModel` for generic model definitions.
```

### Comparing `vokab-0.0.0/Makefile` & `vokab-0.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `vokab-0.0.0/requirements-dev.txt` & `vokab-0.0.1/requirements-dev.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile pyproject.toml --extra test --extra local --extra ext -o requirements-dev.txt
 aiosql==10.1
+altair==5.3.0
+    # via streamlit
 annotated-types==0.6.0
     # via pydantic
 asttokens==2.4.1
     # via stack-data
 attrs==23.2.0
-    # via lancedb
+    # via
+    #   jsonschema
+    #   lancedb
+    #   referencing
+blinker==1.7.0
+    # via streamlit
 build==1.2.1
 cachetools==5.3.3
-    # via lancedb
+    # via
+    #   lancedb
+    #   streamlit
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
-    # via lancedb
+    # via
+    #   lancedb
+    #   streamlit
 coverage==7.4.4
 decorator==5.1.1
     # via
     #   ipython
     #   retry
 deprecation==2.1.0
     # via lancedb
@@ -36,14 +47,18 @@
     #   huggingface-hub
     #   torch
     #   transformers
 fsspec==2024.3.1
     # via
     #   huggingface-hub
     #   torch
+gitdb==4.0.11
+    # via gitpython
+gitpython==3.1.43
+    # via streamlit
 huggingface-hub==0.22.2
     # via
     #   sentence-transformers
     #   tokenizers
     #   transformers
 idna==3.6
     # via requests
@@ -59,17 +74,24 @@
 jaraco-context==4.3.0
     # via keyring
 jaraco-functools==4.0.0
     # via keyring
 jedi==0.19.1
     # via ipython
 jinja2==3.1.3
-    # via torch
+    # via
+    #   altair
+    #   pydeck
+    #   torch
 joblib==1.3.2
     # via scikit-learn
+jsonschema==4.21.1
+    # via altair
+jsonschema-specifications==2023.12.1
+    # via jsonschema
 keyring==25.0.0
     # via twine
 lancedb==0.6.7
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
@@ -85,125 +107,171 @@
     # via sympy
 networkx==3.2.1
     # via torch
 nh3==0.2.17
     # via readme-renderer
 numpy==1.26.4
     # via
+    #   altair
+    #   pandas
     #   pyarrow
+    #   pydeck
     #   pylance
     #   scikit-learn
     #   scipy
     #   sentence-transformers
+    #   streamlit
     #   transformers
 overrides==7.7.0
     # via lancedb
 packaging==24.0
     # via
+    #   altair
     #   build
     #   deprecation
     #   huggingface-hub
     #   pytest
+    #   streamlit
     #   transformers
+pandas==2.2.2
+    # via
+    #   altair
+    #   streamlit
 parso==0.8.3
     # via jedi
 pexpect==4.9.0
     # via ipython
 pillow==10.3.0
-    # via sentence-transformers
+    # via
+    #   sentence-transformers
+    #   streamlit
 pip==24.0
 pkginfo==1.10.0
     # via twine
 pluggy==1.4.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
+protobuf==4.25.3
+    # via streamlit
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 py==1.11.0
     # via retry
 pyarrow==15.0.0
-    # via pylance
+    # via
+    #   pylance
+    #   streamlit
 pydantic==2.6.4
     # via lancedb
 pydantic-core==2.16.3
     # via pydantic
+pydeck==0.8.0
+    # via streamlit
 pygments==2.17.2
     # via
     #   ipython
     #   readme-renderer
     #   rich
 pylance==0.10.9
     # via lancedb
 pyproject-hooks==1.0.0
     # via build
 pytest==8.1.1
     # via pytest-mock
 pytest-mock==3.14.0
+python-dateutil==2.9.0.post0
+    # via pandas
+pytz==2024.1
+    # via pandas
 pyyaml==6.0.1
     # via
     #   huggingface-hub
     #   lancedb
     #   transformers
 rapidfuzz==3.7.0
 ratelimiter==1.2.0.post0
     # via lancedb
 readme-renderer==43.0
     # via twine
+referencing==0.34.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 regex==2023.12.25
     # via transformers
 requests==2.31.0
     # via
     #   huggingface-hub
     #   lancedb
     #   requests-toolbelt
+    #   streamlit
     #   transformers
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 retry==0.9.2
     # via lancedb
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
-    # via twine
+    # via
+    #   streamlit
+    #   twine
+rpds-py==0.18.0
+    # via
+    #   jsonschema
+    #   referencing
 safetensors==0.4.2
     # via transformers
 scikit-learn==1.4.1.post1
     # via sentence-transformers
 scipy==1.12.0
     # via
     #   scikit-learn
     #   sentence-transformers
 semver==3.0.2
     # via lancedb
 sentence-transformers==2.6.1
 setuptools==69.2.0
 six==1.16.0
-    # via asttokens
+    # via
+    #   asttokens
+    #   python-dateutil
+smmap==5.0.1
+    # via gitdb
 sqlite-vss==0.1.2
 stack-data==0.6.3
     # via ipython
+streamlit==1.33.0
 sympy==1.12
     # via torch
 tantivy==0.21.0
+tenacity==8.2.3
+    # via streamlit
 threadpoolctl==3.4.0
     # via scikit-learn
 tokenizers==0.15.2
     # via transformers
+toml==0.10.2
+    # via streamlit
 tomli==2.0.1
     # via
     #   build
     #   coverage
     #   pyproject-hooks
     #   pytest
+toolz==0.12.1
+    # via altair
 torch==2.2.2
     # via sentence-transformers
+tornado==6.4
+    # via streamlit
 tqdm==4.66.2
     # via
     #   huggingface-hub
     #   lancedb
     #   sentence-transformers
     #   transformers
 traitlets==5.14.2
@@ -211,19 +279,23 @@
     #   ipython
     #   matplotlib-inline
 transformers==4.39.3
     # via sentence-transformers
 twine==5.0.0
 typing-extensions==4.10.0
     # via
+    #   altair
     #   huggingface-hub
     #   ipython
     #   pydantic
     #   pydantic-core
+    #   streamlit
     #   torch
+tzdata==2024.1
+    # via pandas
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 wcwidth==0.2.13
     # via prompt-toolkit
 zipp==3.18.1
```

### Comparing `vokab-0.0.0/requirements.txt` & `vokab-0.0.1/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,205 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile pyproject.toml --extra ext -o requirements.txt
 aiosql==10.1
+altair==5.3.0
+    # via streamlit
 annotated-types==0.6.0
     # via pydantic
 attrs==23.2.0
-    # via lancedb
+    # via
+    #   jsonschema
+    #   lancedb
+    #   referencing
+blinker==1.7.0
+    # via streamlit
 cachetools==5.3.3
-    # via lancedb
+    # via
+    #   lancedb
+    #   streamlit
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
-    # via lancedb
+    # via
+    #   lancedb
+    #   streamlit
 decorator==5.1.1
     # via retry
 deprecation==2.1.0
     # via lancedb
 filelock==3.13.3
     # via
     #   huggingface-hub
     #   torch
     #   transformers
 fsspec==2024.3.1
     # via
     #   huggingface-hub
     #   torch
+gitdb==4.0.11
+    # via gitpython
+gitpython==3.1.43
+    # via streamlit
 huggingface-hub==0.22.2
     # via
     #   sentence-transformers
     #   tokenizers
     #   transformers
 idna==3.6
     # via requests
 jinja2==3.1.3
-    # via torch
+    # via
+    #   altair
+    #   pydeck
+    #   torch
 joblib==1.3.2
     # via scikit-learn
+jsonschema==4.21.1
+    # via altair
+jsonschema-specifications==2023.12.1
+    # via jsonschema
 lancedb==0.6.7
+markdown-it-py==3.0.0
+    # via rich
 markupsafe==2.1.5
     # via jinja2
+mdurl==0.1.2
+    # via markdown-it-py
 mpmath==1.3.0
     # via sympy
 networkx==3.2.1
     # via torch
 numpy==1.26.4
     # via
+    #   altair
+    #   pandas
     #   pyarrow
+    #   pydeck
     #   pylance
     #   scikit-learn
     #   scipy
     #   sentence-transformers
+    #   streamlit
     #   transformers
 overrides==7.7.0
     # via lancedb
 packaging==24.0
     # via
+    #   altair
     #   deprecation
     #   huggingface-hub
+    #   streamlit
     #   transformers
+pandas==2.2.2
+    # via
+    #   altair
+    #   streamlit
 pillow==10.3.0
-    # via sentence-transformers
+    # via
+    #   sentence-transformers
+    #   streamlit
+protobuf==4.25.3
+    # via streamlit
 py==1.11.0
     # via retry
 pyarrow==15.0.0
-    # via pylance
+    # via
+    #   pylance
+    #   streamlit
 pydantic==2.6.4
     # via lancedb
 pydantic-core==2.16.3
     # via pydantic
+pydeck==0.8.0
+    # via streamlit
+pygments==2.17.2
+    # via rich
 pylance==0.10.9
     # via lancedb
+python-dateutil==2.9.0.post0
+    # via pandas
+pytz==2024.1
+    # via pandas
 pyyaml==6.0.1
     # via
     #   huggingface-hub
     #   lancedb
     #   transformers
 rapidfuzz==3.7.0
 ratelimiter==1.2.0.post0
     # via lancedb
+referencing==0.34.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 regex==2023.12.25
     # via transformers
 requests==2.31.0
     # via
     #   huggingface-hub
     #   lancedb
+    #   streamlit
     #   transformers
 retry==0.9.2
     # via lancedb
+rich==13.7.1
+    # via streamlit
+rpds-py==0.18.0
+    # via
+    #   jsonschema
+    #   referencing
 safetensors==0.4.2
     # via transformers
 scikit-learn==1.4.1.post1
     # via sentence-transformers
 scipy==1.13.0
     # via
     #   scikit-learn
     #   sentence-transformers
 semver==3.0.2
     # via lancedb
 sentence-transformers==2.6.1
+six==1.16.0
+    # via python-dateutil
+smmap==5.0.1
+    # via gitdb
 sqlite-vss==0.1.2
+streamlit==1.33.0
 sympy==1.12
     # via torch
 tantivy==0.21.0
+tenacity==8.2.3
+    # via streamlit
 threadpoolctl==3.4.0
     # via scikit-learn
 tokenizers==0.15.2
     # via transformers
+toml==0.10.2
+    # via streamlit
+toolz==0.12.1
+    # via altair
 torch==2.2.2
     # via sentence-transformers
+tornado==6.4
+    # via streamlit
 tqdm==4.66.2
     # via
     #   huggingface-hub
     #   lancedb
     #   sentence-transformers
     #   transformers
 transformers==4.39.3
     # via sentence-transformers
 typing-extensions==4.10.0
     # via
+    #   altair
     #   huggingface-hub
     #   pydantic
     #   pydantic-core
+    #   streamlit
     #   torch
+tzdata==2024.1
+    # via pandas
 urllib3==2.2.1
     # via requests
```

### Comparing `vokab-0.0.0/src/vokab/loader.py` & `vokab-0.0.1/src/vokab/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,18 +99,24 @@
         ".jsonl": from_jsonl,
         ".txt": from_txt,
     }
     ext = path.suffix.lower()
 
     def fix(d: dict):
         aliases = d.get("aliases")
-        if aliases and isinstance(aliases, str):
+        if isinstance(aliases, str):
             d["aliases"] = list(filter(None, aliases.split(mv_splitter)))
 
-        meta_keys = d.keys() - {"name", "aliases", "meta", "priority", "label"}
+        meta_keys = d.keys() - {
+            "name",
+            "aliases",
+            "meta",
+            "prevalence",
+            "label",
+        }
         if meta_keys:
             meta = d.setdefault("meta", {})
             for key in meta_keys:
                 meta[key] = d.pop(key)
 
         return d
```

### Comparing `vokab-0.0.0/src/vokab/databases/sqlite/database.py` & `vokab-0.0.1/src/vokab/databases/sqlite/database.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,47 @@
-import json
+import os
 import sqlite3
 from contextlib import contextmanager
 from pathlib import Path
+from typing import List, Optional
 
 import aiosql
 
-from vokab import Database, lazy
+from vokab import (
+    Entity,
+    Labels,
+    Limit,
+    Results,
+    ResultsAdapter,
+    Strs,
+    Vec,
+    lazy,
+    Entities,
+)
+from .. import AbstractDatabase
 
 
-class SQLiteDatabase(Database):
+class SQLiteDatabase(AbstractDatabase):
     name = "sqlite"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.sql = aiosql.from_path(Path(__file__).parent / "sql", "sqlite3")
 
     def connect(self):
-        db_url = self.path / self.config.db_url
+        db_url = self.config.database.url or "database.db"
+        if not os.path.isabs(db_url):
+            db_url = str(self.collection.path / db_url)
         conn = sqlite3.connect(db_url)
-        conn.row_factory = sqlite3.Row  # https://stackoverflow.com/a/3300514
 
-        if self.config.vss_enabled:
+        conn.row_factory = lambda c, r: dict(
+            [(col[0], r[idx]) for idx, col in enumerate(c.description)]
+        )
+
+        if self.config.encoder.enabled:
             sqlite_vss = lazy.lazy_import("sqlite_vss")
             conn.enable_load_extension(True)
             sqlite_vss.load(conn)
 
         return conn
 
     @contextmanager
@@ -49,42 +66,79 @@
                 conn.close()
 
     def initialize(self):
         with self.acquire() as conn:
             self.sql.init_tables(conn)
             conn.execute(
                 f"CREATE VIRTUAL TABLE IF NOT EXISTS vss_terms USING "
-                f"vss0(vector({self.config.vss_dimensions}))"
+                f"vss0(vector({self.config.encoder.dimensions}))"
             )
             self.sql.init_triggers(conn)
 
     def stats(self) -> dict:
         with self.acquire() as conn:
             return dict(self.sql.stats(conn))
 
-    def upsert(self, entity_dicts: list[dict], term_dicts: list[dict]):
+    def upsert(self, entities: List[Entity]):
         with self.acquire() as conn:
-            entity_dicts = list(map(self._serialize_entity, entity_dicts))
+            entity_dicts = self.to_entity_dicts(entities)
             self.sql.upsert_entities(conn, entity_dicts)
+            term_dicts = self.to_term_dicts(entities)
             self.sql.upsert_terms(conn, term_dicts)
 
-    def search(self, query: str, vector: list[float], limit: int):
-        pass
+    def exact(self, term: str, labels: Labels, limit: Limit) -> Results:
+        with self.acquire() as conn:
+            data = self.sql.exact_search(
+                conn,
+                term=term,
+                labels=piped_or_null(labels),
+                limit=limit,
+            )
+            return ResultsAdapter.validate_python(data)
+
+    def vss(self, vector: Vec, labels: Labels, limit: Limit) -> Results:
+        with self.acquire() as conn:
+            if not labels:
+                results = self.sql.vss_search(
+                    conn,
+                    vector=vector,
+                    limit=limit,
+                )
+            else:
+                results = self.sql.vss_search_by_label(
+                    conn,
+                    vector=vector,
+                    labels=piped_or_null(labels),
+                    limit=limit,
+                )
+
+            return ResultsAdapter.validate_python(results)
 
-    def hybrid_search(
-        self, query: str, vector: list[float], limit: int
-    ) -> list[dict]:
+    def fts(self, term: str, labels: Labels, limit: Limit) -> Results:
         with self.acquire() as conn:
-            results = self.sql.hybrid_search(
+            data = self.sql.fts_search(
                 conn,
-                query=query,
-                vector=vector,
+                term=term,
+                labels=piped_or_null(labels),
                 limit=limit,
             )
-            return list(results)
+            return ResultsAdapter.validate_python(data)
+
+    def get(self, slug: str) -> Optional[Entity]:
+        entity = None
+        with self.acquire() as conn:
+            data = self.sql.get_entity(conn, slug=slug)
+            if data:
+                entity = Entity(**data)
+        return entity
+
+    def fetch(self, slugs: Strs) -> Entities:
+        placeholders = ",".join(["?"] * len(slugs))
+        sql = f"SELECT * FROM entities WHERE slug IN ({placeholders})"
+        with self.acquire() as conn:
+            data = conn.execute(sql, slugs).fetchall()
+            return [Entity(**record) for record in data]
+
 
-    @classmethod
-    def _serialize_entity(cls, entity_dict: dict) -> dict:
-        if "meta" in entity_dict and isinstance(entity_dict["meta"], dict):
-            entity_dict = entity_dict.copy()
-            entity_dict["meta"] = json.dumps(entity_dict["meta"])
-        return entity_dict
+def piped_or_null(vals: Labels):
+    if vals:
+        return "|" + "|".join(vals) + "|"
```

### Comparing `vokab-0.0.0/src/vokab/databases/sqlite/sql/init_tables.sql` & `vokab-0.0.1/src/vokab/databases/sqlite/sql/init_tables.sql`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 -- name: init_tables#
 
 -- Entities Table
 CREATE TABLE IF NOT EXISTS entities (
+    slug TEXT primary key,
     name TEXT NOT NULL,
-    label TEXT,
-    priority INTEGER DEFAULT 0,
+    label TEXT NOT NULL,
+    prevalence INTEGER,
     meta TEXT,
-    PRIMARY KEY (name, label)
+    aliases TEXT,
+    UNIQUE (name, label)
 );
 
 -- Terms Table
 CREATE TABLE IF NOT EXISTS terms (
     rowid INTEGER PRIMARY KEY AUTOINCREMENT,
-    name TEXT NOT NULL,
-    label TEXT,
+    slug TEXT NOT NULL,
+    label TEXT NOT NULL,
     term TEXT NOT NULL,
-    is_alias INTEGER,
+    is_alias INTEGER DEFAULT 0,
+    prevalence INTEGER DEFAULT 0,
     vector BLOB,
-    UNIQUE(name, label, term),
-    FOREIGN KEY (name, label) REFERENCES entities(name, label)
+    UNIQUE(slug, term),
+    FOREIGN KEY (slug) REFERENCES entities(slug)
     ON DELETE CASCADE
 );
 
 -- Full Text Search
 CREATE VIRTUAL TABLE IF NOT EXISTS fts_terms USING fts5(
     term,
     content='terms',
     content_rowid='rowid',
     tokenize="trigram case_sensitive 0"
 );
 
-CREATE INDEX IF NOT EXISTS idx_terms_name_label ON terms (name, label);
+CREATE INDEX IF NOT EXISTS idx_terms_slug ON terms (slug);
 CREATE INDEX IF NOT EXISTS idx_terms_term ON terms (term);
 
 -- Note: VSS processed in Python code due to limit of aiosql (no variables in executable scripts)
```

### Comparing `vokab-0.0.0/src/vokab/databases/sqlite/sql/init_triggers.sql` & `vokab-0.0.1/src/vokab/databases/sqlite/sql/init_triggers.sql`

 * *Files identical despite different names*

### Comparing `vokab-0.0.0/tests/test_loader.py` & `vokab-0.0.1/tests/test_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-from vokab import loader
+from typing import List
+from pydantic import TypeAdapter
+from vokab import Entity, loader
 
 
 def test_from_csv(data_path):
     entities = list(loader.from_file(data_path / "emojis.csv"))
     assert len(entities) == 4
     assert entities[0] == {
         "name": "happy",
         "aliases": ["😀"],
-        "priority": "1",
+        "prevalence": "1",
     }
 
 
 def test_from_tsv(data_path):
     entities = list(loader.from_file(data_path / "myths.tsv"))
-    assert len(entities) == 5
-    assert entities[2] == {
-        "name": "Zeus",
+    assert len(entities) == 10
+    assert entities[-1] == {
         "aliases": ["Jupiter", "Jove"],
+        "label": "DEITY",
         "meta": {
+            "definition": "King of the Olympian gods",
             "dominion": "Power",
+            "gender": "Male",
         },
+        "name": "Zeus",
     }
+    adapter = TypeAdapter(List[Entity])
+    validated = adapter.validate_python(entities)
+    assert len(validated) == 10
+    assert isinstance(validated[0], Entity)
 
 
 def test_from_txt(data_path):
     entities = list(loader.from_file(data_path / "emotions.txt"))
     assert len(entities) == 12
     assert entities[-1] == {
         "name": "Serenity",
```

### Comparing `vokab-0.0.0/tests/data/simonw_tags.csv` & `vokab-0.0.1/tests/data/simonw_tags.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name,priority
+name,prevalence
 24ways,13
 2d,3
 37signals,12
 3d,14
 4chan,4
 500startups,4
 aaronstraupcope,4
```

### Comparing `vokab-0.0.0/LICENSE` & `vokab-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vokab-0.0.0/README.md` & `vokab-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vokab-0.0.0/pyproject.toml` & `vokab-0.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ]
 dependencies = [
     "aiosql >= 10.1",
     "click >= 8.0.0",
     "pydantic >= 2.6.1",
     "rapidfuzz >= 3.7.0",
     "sentence-transformers >= 2.2.2",
+    "streamlit >= 1.33.0",
     "torch >= 2.2.2",
     "tqdm",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
@@ -55,14 +56,16 @@
 vokab = "vokab.cli:app"
 
 [tool.hatch.version]
 path = "src/vokab/__init__.py"
 
 [tool.mypy]
 check_untyped_defs = true
+ignore_missing_imports = true
+
 
 [tool.pytest.ini_options]
 addopts = [
   "--strict-config",
   "--strict-markers",
 ]
 xfail_strict = true
```

### Comparing `vokab-0.0.0/PKG-INFO` & `vokab-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.3
 Name: vokab
-Version: 0.0.0
+Version: 0.0.1
 Summary: vokab: named entity linking through hybrid (lexical and semantic) search engine.
 Author-email: Ian Maurer <ian@genomoncology.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Requires-Dist: aiosql>=10.1
 Requires-Dist: click>=8.0.0
 Requires-Dist: pydantic>=2.6.1
 Requires-Dist: rapidfuzz>=3.7.0
 Requires-Dist: sentence-transformers>=2.2.2
+Requires-Dist: streamlit>=1.33.0
 Requires-Dist: torch>=2.2.2
 Requires-Dist: tqdm
 Provides-Extra: ext
 Requires-Dist: lancedb; extra == 'ext'
 Requires-Dist: sqlite-vss; extra == 'ext'
 Requires-Dist: tantivy; extra == 'ext'
 Provides-Extra: local
```

