# Comparing `tmp/ormdantic-1.6.1.tar.gz` & `tmp/ormdantic-1.7.0.tar.gz`

## Comparing `ormdantic-1.6.1.tar` & `ormdantic-1.7.0.tar`

### file list

```diff
@@ -1,52 +1,79 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 ormdantic-1.6.1/mkdocs.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0    18349 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.github/logo.png
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/code_of_conduct.md
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/contributing.md
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/faq.md
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/favicon.png
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/index.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/installation.md
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/license.md
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 ormdantic-1.6.1/docs/usage.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/__init__.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/py.typed
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/__init__.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/_crud.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/_field.py
--rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/_lazy.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/_query.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/_serializer.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/generator/_table.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/handler/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/handler/errors.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/handler/helper.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/handler/random.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/handler/snake.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/models/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/models/models.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/types/__init__.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ormdantic-1.6.1/ormdantic/types/base.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ormdantic-1.6.1/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ormdantic-1.6.1/scripts/format.sh
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ormdantic-1.6.1/scripts/integration.sh
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ormdantic-1.6.1/scripts/lint.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ormdantic-1.6.1/scripts/test.sh
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ormdantic-1.6.1/scripts/test_html.sh
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/test_errors.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/test_generator.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/test_orm.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/test_otm_relations.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/test_snake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 ormdantic-1.6.1/tests/integration/demo.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 ormdantic-1.6.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ormdantic-1.6.1/LICENSE
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 ormdantic-1.6.1/README.md
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ormdantic-1.6.1/pyproject.toml
--rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 ormdantic-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 ormdantic-1.7.0/mkdocs.yml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0    18349 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.github/logo.png
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/favicon.png
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/index.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/installation.md
+-rw-r--r--   0        0        0    21732 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/release.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/crud.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/errors.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/field.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/ormdantic.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/query.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/reference.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/serializer.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/api/table.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/css/custom.css
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/css/termynal.css
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/development/contributing.md
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/faq/code_of_conduct.md
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/faq/faq.md
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/faq/license.md
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/js/custom.js
+-rw-r--r--   0        0        0     8901 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/js/termynal.js
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/usage/generator.md
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 ormdantic-1.7.0/docs/usage/usage.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/__init__.py
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/py.typed
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/__init__.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/_crud.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/_field.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/_lazy.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/_query.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/_serializer.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/generator/_table.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/handler/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/handler/errors.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/handler/helper.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/handler/random.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/handler/snake.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/models/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/models/models.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/types/__init__.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ormdantic-1.7.0/ormdantic/types/base.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/all.txt
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/docs.in
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/docs.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/extra.in
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/extra.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/linting.in
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/linting.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/testing.in
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 ormdantic-1.7.0/requirements/testing.txt
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/clean.sh
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/docs_build.sh
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/docs_serve.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/format.sh
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/integration.sh
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/lint.sh
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/requirements.sh
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ormdantic-1.7.0/scripts/test.sh
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/test_errors.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/test_generator.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/test_orm.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/test_otm_relations.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/test_snake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 ormdantic-1.7.0/tests/integration/demo.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 ormdantic-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ormdantic-1.7.0/LICENSE
+-rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 ormdantic-1.7.0/README.md
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 ormdantic-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 ormdantic-1.7.0/PKG-INFO
```

### Comparing `ormdantic-1.6.1/.github/logo.png` & `ormdantic-1.7.0/.github/logo.png`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/.github/workflows/ci.yml` & `ormdantic-1.7.0/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -16,19 +16,23 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install Dependencies
-        run: pip install -e .[lint]
-      - uses: pre-commit/action@v3.0.0
+      - name: setup uv
+        uses: yezz123/setup-uv@v4
         with:
-          extra_args: --all-files --verbose
+          uv-version: "0.1.22"
+          uv-venv: ".venv"
+      - name: Install Dependencies
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/linting.txt
+      - name: Run Pre-commit
+        run: bash scripts/format.sh
       - name: check Static Analysis
         run: bash scripts/lint.sh
 
   tests:
 
     name: test py${{ matrix.python-version }} on ${{ matrix.os }}
 
@@ -46,38 +50,38 @@
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-
-      - name: Install SQLAlchemy version 1.4.42
-        run: |
-          python -m pip install --upgrade pip
-          pip install SQLAlchemy==1.4.42
+      - name: setup uv
+        uses: yezz123/setup-uv@v4
+        with:
+          uv-version: "0.1.22"
+          uv-venv: ".venv"
 
       - name: Install Dependencies
-        run: pip install -e .[sqlite,test]
+        run:  uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/testing.txt && uv pip install -r requirements/extra.txt
 
       - name: Freeze Dependencies
-        run: pip freeze
+        run: uv pip freeze
 
       - name: Test with pytest
         run: bash scripts/test.sh
         env:
           DATABASE_URL: sqlite+aiosqlite:///db.sqlite3
 
       - name: Upload coverage
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
 
-  postgres:
-    name: test on python ${{ matrix.python-version }} with postgres ${{ matrix.postgres-version }}
+  Integration:
+    name: test on python ${{ matrix.python-version }} with Integration tests
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
         postgres-version: [14]
 
@@ -103,49 +107,34 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install Dependencies
-        run: pip install -e .[postgresql,test]
-      - name: Integration Tests, Postgres
-        run: bash scripts/integration.sh
-        env:
-          DATABASE_URL: postgresql+asyncpg://postgres:postgres@localhost:5432/postgres
-
-  sqlite:
-    name: test on python ${{ matrix.python-version }} with sqlite
-    runs-on: ubuntu-latest
-    timeout-minutes: 30
-    strategy:
-      matrix:
-        python-version: ["3.10", "3.11", "3.12"]
-
-    steps:
-
-      - uses: actions/checkout@v4
-
-      - name: Set up Python
-        uses: actions/setup-python@v5
+      - name: setup uv
+        uses: yezz123/setup-uv@v4
         with:
-          python-version: ${{ matrix.python-version }}
-
+          uv-version: "0.1.22"
+          uv-venv: ".venv"
       - name: Install Dependencies
-        run: pip install -e .[sqlite,test]
-
-      - name: Integration Tests, SQLite
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/testing.txt && uv pip install -r requirements/extra.txt
+      - name: Integration Tests - SQLite
         run: bash scripts/integration.sh
         env:
           DATABASE_URL: sqlite+aiosqlite:///db.sqlite3
+      - name: Integration Tests - Postgres
+        run: bash scripts/integration.sh
+        env:
+          DATABASE_URL: postgresql+asyncpg://postgres:postgres@localhost:5432/postgres
+
 
   # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
   check:
     if: always()
-    needs: [lint, tests, postgres, sqlite]
+    needs: [lint, tests, Integration]
     runs-on: ubuntu-latest
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
```

### Comparing `ormdantic-1.6.1/.github/workflows/release.yml` & `ormdantic-1.7.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: "3.10"
       - name: Install build dependencies
         run: pip install build
       - name: check GITHUB_REF matches package version
-        uses: samuelcolvin/check-python-version@v3.1
+        uses: samuelcolvin/check-python-version@v4.1
         with:
           version_file_path: ormdantic/__init__.py
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `ormdantic-1.6.1/docs/code_of_conduct.md` & `ormdantic-1.7.0/docs/faq/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/docs/faq.md` & `ormdantic-1.7.0/docs/faq/faq.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/docs/favicon.png` & `ormdantic-1.7.0/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/docs/index.md` & `ormdantic-1.7.0/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+---
+hide:
+  - navigation
+---
+
 ![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/logo.png)
 
 <p align="center">
     <em>Asynchronous ORM that uses pydantic models to represent database tables ✨</em>
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/
-logo.png)
+--- hide: - navigation --- ![Logo](https://raw.githubusercontent.com/yezz123/
+ormdantic/main/.github/logo.png)
   AAssyynncchhrroonnoouuss OORRMM tthhaatt uusseess ppyyddaannttiicc mmooddeellss ttoo rreepprreesseenntt ddaattaabbaassee ttaabblleess ?â??¨
   _[_T_e_s_t_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_y_e_z_z_1_2_3_/_o_r_m_d_a_n_t_i_c_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]
                           _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_p_o_n_s_o_r_]
 Ormdantic is a library for interacting with Asynchronous SQL databases from
 Python code, with Python objects. It is designed to be intuitive, easy to use,
 compatible, and robust. **Ormdantic** is based on [Pypika](https://github.com/
 kayak/pypika), and powered by _P_y_d_a_n_t_i_c and _S_Q_L_A_l_c_h_e_m_y, and Highly inspired by
```

### Comparing `ormdantic-1.6.1/docs/license.md` & `ormdantic-1.7.0/docs/faq/license.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/docs/usage.md` & `ormdantic-1.7.0/docs/usage/usage.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Ormdantic Usage
+
 ## Create SQLAlchemy engine
 
 Ormdantic uses SQLAlchemy under hood to run different queries, which is why we need to initialize by creating an asynchronous engine.
 
 > **Note**: You will use the `connection` parameter to pass the connection to the engine directly.
 
 ```python
@@ -166,54 +168,7 @@
 
 ```python
      count_advanced = await database[Coffee].count(
           where={"sweetener": 2}, depth=1
      )
      print(count_advanced)
 ```
-
-## Generator
-
-We introduce a new feature called `Generator`, which is a way to generate a Model instance with random data.
-
-So, Given a Pydantic model type can generate instances of that model with randomly generated values.
-
-using `ormdantic.generator.Generator` to generate a Model instance.
-
-```python
-from enum import auto, Enum
-from uuid import UUID
-
-from ormdantic.generator import Generator
-from pydantic import BaseModel
-
-
-class Flavor(Enum):
-    MOCHA = auto()
-    VANILLA = auto()
-
-
-class Brand(BaseModel):
-    brand_name: str
-
-
-class Coffee(BaseModel):
-    id: UUID
-    description: str
-    cream: bool
-    sweetener: int
-    flavor: Flavor
-    brand: Brand
-
-
-print(Generator(Coffee))
-```
-
-so the results will be:
-
-```shell
-id=UUID('93b517c2-083b-457d-a0e5-6e1bd2a927e4')
-description='ctWOb' cream=True sweetener=234
-flavor=<Flavor.VANILLA: 2> brand=Brand(brand_name='LMrIf')
-```
-
-We can integrate this with our database while testing our application (Live Tests).
```

### Comparing `ormdantic-1.6.1/ormdantic/orm.py` & `ormdantic-1.7.0/ormdantic/orm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module providing a way to create ORM models and schemas"""
+
 from types import UnionType
 from typing import Callable, ForwardRef, Type, get_args, get_origin
 
 from pydantic.fields import ModelField
 from sqlalchemy import MetaData
 from sqlalchemy.ext.asyncio import create_async_engine
 
@@ -15,55 +16,42 @@
 )
 from ormdantic.models import Map, OrmTable, Relationship
 from ormdantic.types import ModelType
 
 
 class Ormdantic:
     """
-    It combines SQLAlchemy, Pydantic and Pypika tries to simplify the code you write as much as possible, allowing you to reduce the code duplication to a minimum,
-    but while getting the best developer experience possible.
+    Ormdantic provides a way to create ORM models and schemas.
     """
 
     def __init__(self, connection: str) -> None:
         """Register models as ORM models and create schemas"""
         self._metadata: MetaData | None = None
         self._crud_generators: dict[Type, CRUD] = {}  # type: ignore
         self._engine = create_async_engine(connection)
         self._table_map: Map = Map()
 
     def __getitem__(self, item: Type[ModelType]) -> CRUD[ModelType]:
-        """Get a `Table` for the given pydantic model.
-
-        :param item: Pydantic model.
-        :return: A `Table` for the given pydantic model.
-        """
+        """Get a `Table` for the given pydantic model."""
         return self._crud_generators[item]
 
     def table(
         self,
         tablename: str | None = None,
         *,
         pk: str,
         indexed: list[str] | None = None,
         unique: list[str] | None = None,
         unique_constraints: list[list[str]] | None = None,
         back_references: dict[str, str] | None = None,
     ) -> Callable[[Type[ModelType]], Type[ModelType]]:
-        """Register a model as a database table.
-
-        :param tablename: The database table name.
-        :param pk: Field name of table primary key.
-        :param indexed: Names of fields to index.
-        :param unique: Names of fields that must be unique.
-        :param unique_constraints: Fields that must be unique together.
-        :param back_references: Dict of field names to back-referenced field names.
-        :return: The decorated model.
-        """
+        """Register a model as a database table."""
 
         def _wrapper(cls: Type[ModelType]) -> Type[ModelType]:
+            """Decorator function."""
             tablename_ = tablename or snake_case(cls.__name__)
             cls_back_references = back_references or {}
             table_metadata = OrmTable[ModelType](
                 model=cls,
                 tablename=tablename_,
                 pk=pk,
                 indexed=indexed or [],
@@ -80,32 +68,33 @@
             self._table_map.model_to_data[cls] = table_metadata
             self._table_map.name_to_data[tablename_] = table_metadata
             return cls
 
         return _wrapper
 
     async def init(self) -> None:
+        """Initialize ORM models."""
         # Populate relation information.
         for table_data in self._table_map.name_to_data.values():
             rels = self.get(table_data)
             table_data.relationships = rels
         # Now that relation information is populated generate tables.
         self._metadata = MetaData()
         for table_data in self._table_map.name_to_data.values():
-            # noinspection PyTypeChecker
             self._crud_generators[table_data.model] = CRUD(
                 table_data,
                 self._table_map,
                 self._engine,
             )
         await Table(self._engine, self._metadata, self._table_map).init()
         async with self._engine.begin() as conn:
             await conn.run_sync(self._metadata.create_all)
 
     def get(self, table_data: OrmTable[ModelType]) -> dict[str, Relationship]:
+        """Get relationships for a given table."""
         relationships = {}
         for field_name, field in table_data.model.__fields__.items():
             related_table = self._get_related_table(field)
             if related_table is None:
                 continue
             if back_reference := table_data.back_references.get(field_name):
                 relationships[field_name] = self._get_many_relationship(
@@ -137,14 +126,15 @@
             relationships[field_name] = Relationship(
                 foreign_table=related_table.tablename
             )
 
         return relationships
 
     def _get_related_table(self, field: ModelField) -> OrmTable | None:  # type: ignore
+        """Get related table for a given field."""
         related_table: OrmTable | None = None  # type: ignore
         # Try to get foreign model from union.
         if args := get_args(field.type_):
             for arg in args:
                 try:
                     related_table = self._table_map.model_to_data.get(arg)
                 except TypeError:
@@ -157,14 +147,15 @@
     @staticmethod
     def _get_many_relationship(
         field_name: str,
         back_reference: str,
         table_data: OrmTable,  # type: ignore
         related_table: OrmTable,  # type: ignore
     ) -> Relationship:
+        """Get many-to-many relationship."""
         back_referenced_field = related_table.model.__fields__.get(back_reference)
         # TODO: Check if back-reference is present but mismatched in type.
         if (
             table_data.model not in get_args(back_referenced_field.type_)
             and table_data.model != back_referenced_field.type_
         ):
             raise MismatchingBackReferenceError(
```

### Comparing `ormdantic-1.6.1/ormdantic/generator/_crud.py` & `ormdantic-1.7.0/ormdantic/generator/_crud.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 """Handle table interactions for a model."""
 
-
 from typing import Any, Generic
 
 from pypika import Order
 from pypika.queries import QueryBuilder
 from sqlalchemy import text
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, async_sessionmaker
 
 from ormdantic.generator._field import OrmField
 from ormdantic.generator._query import OrmQuery
 from ormdantic.generator._serializer import OrmSerializer
 from ormdantic.models import Map, OrmTable, Result
 from ormdantic.types import ModelType
 
 
-class PydanticSQLCRUDGenerator(Generic[ModelType]):
+class OrmCrud(Generic[ModelType]):
     """Provides DB CRUD methods and table information for a model."""
 
     def __init__(
         self,
         table_data: OrmTable,  # type: ignore
         table_map: Map,
         engine: AsyncEngine,
     ) -> None:
+        """Initialize OrmCrud."""
         self._engine = engine
         self._table_map = table_map
         self._table_data = table_data
         self.tablename = table_data.tablename
         self.columns = table_data.columns
 
     async def find_one(self, pk: Any, depth: int = 0) -> ModelType | None:
-        """Find a model instance by primary key.
-
-        :param pk: Primary key of the record to get.
-        :param depth: ORM fetch depth.
-        :return: A model representing the record if it exists else None.
-        """
+        """Find a model instance by primary key."""
         result = await self._execute_query(
             OrmField(self._table_data, self._table_map).get_find_one_query(pk, depth)
         )
         return OrmSerializer[ModelType | None](
             table_data=self._table_data,
             table_map=self._table_map,
             result_set=result,
@@ -81,60 +75,45 @@
         """Insert a model instance."""
         await self._execute_query(
             OrmQuery(model_instance, self._table_map).get_insert_query()
         )
         return model_instance
 
     async def update(self, model_instance: ModelType) -> ModelType:
-        """Update a record.
-
-        :param `model_instance``: Model representing record to update.
-        :return: The updated model.
-        """
+        """Update a record."""
         await self._execute_query(
             OrmQuery(model_instance, self._table_map).get_update_queries()
         )
         return model_instance
 
     async def upsert(self, model_instance: ModelType) -> ModelType:
-        """Insert a record if it does not exist, else update it.
-
-        :param `model_instance``: Model representing record to insert or update.
-        :return: The inserted or updated model.
-        """
+        """Insert a record if it does not exist, else update it."""
 
         await self._execute_query(
             OrmQuery(model_instance, self._table_map).get_upsert_query()
         )
         return model_instance
 
     async def delete(self, pk: Any) -> bool:
-        """Delete a model instance by primary key.
-
-        :param pk: Primary key of the record to delete.
-        """
+        """Delete a model instance by primary key."""
         await self._execute_query(
             OrmField(self._table_data, self._table_map).get_delete_query(pk)
         )
         return True
 
     async def count(self, where: dict[str, Any] | None = None, depth: int = 0) -> int:
-        """Count records.
-
-        :param where: Where clause to filter records.
-        :param depth: ORM fetch depth.
-        :return: Number of records.
-        """
+        """Count records."""
         result = await self._execute_query(
             OrmField(self._table_data, self._table_map).get_count_query(where, depth)
         )
         return result.scalar()
 
     async def _execute_query(self, query: QueryBuilder) -> Any:
-        async_session = sessionmaker(
+        """Execute a query."""
+        async_session = async_sessionmaker(
             self._engine, expire_on_commit=False, class_=AsyncSession
         )
         async with async_session() as session:
             async with session.begin():
                 result = await session.execute(text(str(query)))
             await session.commit()
         await self._engine.dispose()
```

### Comparing `ormdantic-1.6.1/ormdantic/generator/_field.py` & `ormdantic-1.7.0/ormdantic/generator/_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for building queries from field data."""
+
 from typing import Any
 
 from pypika import Field, Order
 from pypika.functions import Count
 from pypika.queries import Query, QueryBuilder, Table
 
 from ormdantic.handler import py_type_to_sql
```

### Comparing `ormdantic-1.6.1/ormdantic/generator/_lazy.py` & `ormdantic-1.7.0/ormdantic/generator/_lazy.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     - `type_ is` an enum, the function returns a random value from the enum.
     - `type_ is` a UUID, the function returns a randomly generated UUID.
     - `type_ is` a date, time, timedelta, or datetime, the function returns a random value using the corresponding Random*Value class.
 
     If none of these conditions are met, the function returns a default value for the given type.
     """
     if isinstance(type_, typing.ForwardRef):
-        # noinspection PyUnresolvedReferences
         type_ = pydantic.typing.evaluate_forwardref(type_, None, None)
     origin = typing.get_origin(type_)
     if origin is dict:
         k_type, v_type = typing.get_args(type_)
         return {
             _get_value(
                 k_type, model_field, use_default_values, optionals_use_none
```

### Comparing `ormdantic-1.6.1/ormdantic/generator/_query.py` & `ormdantic-1.7.0/ormdantic/generator/_query.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/ormdantic/generator/_serializer.py` & `ormdantic-1.7.0/ormdantic/generator/_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """Generate Python models from a table map and result set."""
 
     def __init__(
         self,
         table_data: OrmTable,  # type: ignore
         table_map: Map,
         # TODO: Missing type parameters for generic type "CursorResult".
-        result_set: CursorResult,
+        result_set: CursorResult[Any],
         is_array: bool,
         depth: int,
     ) -> None:
         """Generate Python models from a table map and result set.
 
         :param table_data: Table data for the returned model type.
         :param table_map: Map of tablenames and models.
```

### Comparing `ormdantic-1.6.1/ormdantic/generator/_table.py` & `ormdantic-1.7.0/ormdantic/generator/_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Module providing PydanticSQLTableGenerator."""
+"""Module providing OrmTableGenerator."""
+
 import uuid
 from datetime import date, datetime
 from types import UnionType
 from typing import Any, get_args, get_origin
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
@@ -23,22 +24,22 @@
 from sqlalchemy.dialects import postgresql
 from sqlalchemy.ext.asyncio import AsyncEngine
 
 from ormdantic.handler import TableName_From_Model, TypeConversionError
 from ormdantic.models import Map, OrmTable
 
 
-class PydanticSQLTableGenerator:
+class OrmTableGenerator:
     def __init__(
         self,
         engine: AsyncEngine,
         metadata: MetaData,
         table_map: Map,
     ) -> None:
-        """Initialize PydanticSQLTableGenerator."""
+        """Initialize OrmTableGenerator."""
         self._engine = engine
         self._metadata = metadata
         self._table_map = table_map
         self._tables: list[str] = []
 
     async def init(self) -> None:
         """Generate SQL Alchemy tables."""
@@ -56,15 +57,15 @@
             )
         async with self._engine.begin() as conn:
             await conn.run_sync(self._metadata.create_all)
 
     def _get_columns(
         self,
         table_data: OrmTable,  # type: ignore
-    ) -> tuple[Column[Any] | Column, ...]:
+    ) -> tuple[Column[Any] | Column[Any], ...]:
         columns = []
         for field_name, field in table_data.model.__fields__.items():
             kwargs = {
                 "primary_key": field_name == table_data.pk,
                 "index": field_name in table_data.indexed,
                 "unique": field_name in table_data.unique,
                 "nullable": not field.required,
@@ -74,15 +75,15 @@
             column = self._get_column(field_name, field, **kwargs)
             if column is not None:
                 columns.append(column)
         return tuple(columns)
 
     def _get_column(
         self, field_name: str, field: ModelField, **kwargs: Any
-    ) -> Column | None:
+    ) -> Column[Any] | None:
         outer_origin = get_origin(field.outer_type_)
         origin = get_origin(field.type_)
         if outer_origin and outer_origin == list:
             return self._get_column_from_type_args(
                 field_name, field, **kwargs
             )  # pragma: no cover
         if origin:
@@ -92,15 +93,15 @@
                 raise TypeConversionError(field.type_)  # pragma: no cover
         if get_origin(field.outer_type_) == dict:
             return Column(field_name, JSON, **kwargs)
         if field.type_ is uuid.UUID:
             col_type = (
                 postgresql.UUID if self._engine.name == "postgres" else String(36)
             )
-            return Column(field_name, col_type, **kwargs)
+            return Column(field_name, col_type, **kwargs)  # type: ignore
         if issubclass(field.type_, BaseModel):
             return Column(field_name, JSON, **kwargs)
         if issubclass(field.type_, str):
             return Column(field_name, String(field.field_info.max_length), **kwargs)
         if issubclass(field.type_, float):
             return Column(field_name, Float, **kwargs)
         if issubclass(field.type_, int):
@@ -115,15 +116,15 @@
             return Column(field_name, Date, **kwargs)
 
         # Catchall for dict/list or any other.
         return Column(field_name, JSON, **kwargs)
 
     def _get_column_from_type_args(
         self, field_name: str, field: ModelField, **kwargs: Any
-    ) -> Column | None:
+    ) -> Column[Any] | None:
         for arg in get_args(field.type_):
             if arg in [it.model for it in self._table_map.name_to_data.values()]:
                 foreign_table = TableName_From_Model(arg, self._table_map)
                 foreign_data = self._table_map.name_to_data[foreign_table]
                 return Column(
                     field_name,
                     ForeignKey(f"{foreign_table}.{foreign_data.pk}"),
```

### Comparing `ormdantic-1.6.1/ormdantic/handler/__init__.py` & `ormdantic-1.7.0/ormdantic/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/ormdantic/handler/errors.py` & `ormdantic-1.7.0/ormdantic/handler/errors.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/ormdantic/handler/helper.py` & `ormdantic-1.7.0/ormdantic/handler/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions used throughout the project."""
+
 import json
 from typing import Any, Type
 from uuid import UUID
 
 from pydantic import BaseModel
 
 from ormdantic.models.models import Map
```

### Comparing `ormdantic-1.6.1/ormdantic/handler/random.py` & `ormdantic-1.7.0/ormdantic/handler/random.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/ormdantic/handler/snake.py` & `ormdantic-1.7.0/ormdantic/handler/snake.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/ormdantic/models/models.py` & `ormdantic-1.7.0/ormdantic/models/models.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/ormdantic/types/base.py` & `ormdantic-1.7.0/ormdantic/types/base.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/scripts/clean.sh` & `ormdantic-1.7.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/tests/test_errors.py` & `ormdantic-1.7.0/tests/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import unittest
 from typing import Callable
 from uuid import UUID, uuid4
 
 import pytest
+import sqlalchemy
 from decouple import config
 from pydantic import BaseModel, Field
 from sqlalchemy import MetaData
 
 from ormdantic import Ormdantic
 from ormdantic.handler import (
     MismatchingBackReferenceError,
@@ -151,9 +152,9 @@
 
     @staticmethod
     async def test_conversion_type_error() -> None:
         with pytest.raises(TypeConversionError) as e:
             await db_5.init()
         assert (
             e.value.args[0]
-            == "Type typing.Callable[[], int] is not supported by SQLAlchemy 1.4.42."
+            == f"Type typing.Callable[[], int] is not supported by SQLAlchemy {sqlalchemy.__version__}."
         )
```

### Comparing `ormdantic-1.6.1/tests/test_generator.py` & `ormdantic-1.7.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/tests/test_orm.py` & `ormdantic-1.7.0/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/tests/test_otm_relations.py` & `ormdantic-1.7.0/tests/test_otm_relations.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/tests/test_snake.py` & `ormdantic-1.7.0/tests/test_snake.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/tests/integration/demo.py` & `ormdantic-1.7.0/tests/integration/demo.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/.gitignore` & `ormdantic-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/LICENSE` & `ormdantic-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ormdantic-1.6.1/README.md` & `ormdantic-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -300,31 +300,25 @@
 source venv/bin/activate
 ```
 
 And then install the development dependencies:
 
 ```bash
 # Install dependencies
-pip install -e .[sqlite,postgresql,test,lint,docs]
+pip install -r requirements/all.txt
 ```
 
 ### Run tests 🌝
 
 You can run all the tests with:
 
 ```bash
 bash scripts/test.sh
 ```
 
-> Note: You can also generate a coverage report with:
-
-```bash
-bash scripts/test_html.sh
-```
-
 ### Format the code 🍂
 
 Execute the following command to apply `pre-commit` formatting:
 
 ```bash
 bash scripts/format.sh
 ```
```

### Comparing `ormdantic-1.6.1/pyproject.toml` & `ormdantic-1.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -34,18 +34,17 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Database",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "typing-extensions >=3.7.4,<4.10.0",
     "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0",
-    "sqlalchemy[asyncio]>=1.3.18,<2.0.0",
-    "PyPika ==0.48.9"
+    "sqlalchemy[asyncio]>=2.0.0",
+    "PyPika==0.48.9"
 ]
 
 dynamic = ["version"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
@@ -58,75 +57,57 @@
 sqlite = [
     "aiosqlite",
 ]
 postgresql = [
     "psycopg2-binary",
     "asyncpg"
 ]
-lint = [
-    "pre-commit==3.6.0",
-    "mypy==1.7.1",
-]
-test = [
-    "pytest==7.4.3",
-    "pytest-asyncio == 0.23.2",
-    "pytest-cov==4.1.0",
-    "python-decouple",
-    "pytest-pretty==1.2.0"
-]
-docs = [
-    "mkdocs >=1.1.2,<2.0.0",
-    "mkdocs-material >=8.1.4,<10.0.0",
-    "mdx-include >=1.4.1,<2.0.0",
-    "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
-    "mkdocs-mermaid2-plugin==1.1.1",
-    "markdown-include==0.8.1",
-    "pymdown-extensions==10.5",
-    "jinja2==3.1.2"
-]
 
 [tool.hatch.version]
 path = "ormdantic/__init__.py"
 
 [tool.isort]
 profile = "black"
 known_third_party = ["pydantic", "sqlalchemy", "typing_extensions"]
 
-[tool.ruff]
+[tool.ruff.lint]
+mccabe = { max-complexity = 14 }
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 
-[tool.ruff.isort]
-known-third-party = ["pydantic", "sqlalchemy", "typing_extensions"]
+[tool.ruff.lint.isort]
+known-third-party = ["pydantic", "typing_extensions", "sqlalchemy"]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [tool.coverage.run]
 source = ["ormdantic"]
 branch = true
 context = '${CONTEXT}'
 
 [tool.coverage.paths]
 source = [
-    "ormdantic",
+    'ormdantic/',
+    '/Users/runner/work/ormdantic/ormdantic/ormdantic/',
+    'D:\a\ormdantic\ormdantic\ormdantic',
 ]
 
 [tool.mypy]
 plugins = "pydantic.mypy"
 follow_imports = "silent"
 strict_optional = true
 warn_redundant_casts = true
```

### Comparing `ormdantic-1.6.1/PKG-INFO` & `ormdantic-1.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ormdantic
-Version: 1.6.1
+Version: 1.7.0
 Summary: asynchronous ORM that uses pydantic models to represent database tables
 Project-URL: Homepage, https://github.com/yezz123/ormdantic
 Project-URL: Documentation, https://ormdantic.yezz.me/
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,39 +24,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
 Requires-Dist: pypika==0.48.9
-Requires-Dist: sqlalchemy[asyncio]<2.0.0,>=1.3.18
-Requires-Dist: typing-extensions<4.10.0,>=3.7.4
-Provides-Extra: docs
-Requires-Dist: jinja2==3.1.2; extra == 'docs'
-Requires-Dist: markdown-include==0.8.1; extra == 'docs'
-Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'docs'
-Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'docs'
-Requires-Dist: mkdocs-material<10.0.0,>=8.1.4; extra == 'docs'
-Requires-Dist: mkdocs-mermaid2-plugin==1.1.1; extra == 'docs'
-Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'docs'
-Requires-Dist: pymdown-extensions==10.5; extra == 'docs'
-Provides-Extra: lint
-Requires-Dist: mypy==1.7.1; extra == 'lint'
-Requires-Dist: pre-commit==3.6.0; extra == 'lint'
+Requires-Dist: sqlalchemy[asyncio]>=2.0.0
 Provides-Extra: postgresql
 Requires-Dist: asyncpg; extra == 'postgresql'
 Requires-Dist: psycopg2-binary; extra == 'postgresql'
 Provides-Extra: sqlite
 Requires-Dist: aiosqlite; extra == 'sqlite'
-Provides-Extra: test
-Requires-Dist: pytest-asyncio==0.23.2; extra == 'test'
-Requires-Dist: pytest-cov==4.1.0; extra == 'test'
-Requires-Dist: pytest-pretty==1.2.0; extra == 'test'
-Requires-Dist: pytest==7.4.3; extra == 'test'
-Requires-Dist: python-decouple; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/logo.png)
 
 <p align="center">
     <em>Asynchronous ORM that uses pydantic models to represent database tables ✨</em>
 </p>
@@ -357,31 +338,25 @@
 source venv/bin/activate
 ```
 
 And then install the development dependencies:
 
 ```bash
 # Install dependencies
-pip install -e .[sqlite,postgresql,test,lint,docs]
+pip install -r requirements/all.txt
 ```
 
 ### Run tests 🌝
 
 You can run all the tests with:
 
 ```bash
 bash scripts/test.sh
 ```
 
-> Note: You can also generate a coverage report with:
-
-```bash
-bash scripts/test_html.sh
-```
-
 ### Format the code 🍂
 
 Execute the following command to apply `pre-commit` formatting:
 
 ```bash
 bash scripts/format.sh
 ```
```

