# Comparing `tmp/zettel_org-0.6.2.tar.gz` & `tmp/zettel_org-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel_org-0.6.2.tar", last modified: Mon Apr 15 13:53:40 2024, max compression
+gzip compressed data, was "zettel_org-0.6.3.tar", last modified: Fri Apr 19 15:39:39 2024, max compression
```

## Comparing `zettel_org-0.6.2.tar` & `zettel_org-0.6.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.621833 zettel_org-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.605833 zettel_org-0.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.605833 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.605833 zettel_org-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-15 13:53:31.000000 zettel_org-0.6.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-15 13:53:31.000000 zettel_org-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-15 13:53:31.000000 zettel_org-0.6.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-15 13:53:31.000000 zettel_org-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-15 13:53:31.000000 zettel_org-0.6.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 13:53:31.000000 zettel_org-0.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-15 13:53:40.621833 zettel_org-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-15 13:53:31.000000 zettel_org-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.605833 zettel_org-0.6.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2662 2024-04-15 13:53:31.000000 zettel_org-0.6.2/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-15 13:53:31.000000 zettel_org-0.6.2/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-15 13:53:31.000000 zettel_org-0.6.2/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-15 13:53:31.000000 zettel_org-0.6.2/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-15 13:53:31.000000 zettel_org-0.6.2/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.605833 zettel_org-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.605833 zettel_org-0.6.2/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.609833 zettel_org-0.6.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.609833 zettel_org-0.6.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.609833 zettel_org-0.6.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-15 13:53:31.000000 zettel_org-0.6.2/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 13:53:31.000000 zettel_org-0.6.2/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.597833 zettel_org-0.6.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.609833 zettel_org-0.6.2/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 13:53:31.000000 zettel_org-0.6.2/examples/zorg_file/tags_and_ids.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.609833 zettel_org-0.6.2/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-15 13:53:31.000000 zettel_org-0.6.2/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 13:53:31.000000 zettel_org-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-15 13:53:31.000000 zettel_org-0.6.2/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-15 13:53:31.000000 zettel_org-0.6.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 13:53:31.000000 zettel_org-0.6.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-15 13:53:31.000000 zettel_org-0.6.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.609833 zettel_org-0.6.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 13:53:31.000000 zettel_org-0.6.2/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-15 13:53:40.625833 zettel_org-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-15 13:53:31.000000 zettel_org-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.597833 zettel_org-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.621833 zettel_org-0.6.2/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-15 13:53:40.000000 zettel_org-0.6.2/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-15 13:53:40.000000 zettel_org-0.6.2/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:53:40.000000 zettel_org-0.6.2/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 13:53:40.000000 zettel_org-0.6.2/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:53:36.000000 zettel_org-0.6.2/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-15 13:53:40.000000 zettel_org-0.6.2/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 13:53:40.000000 zettel_org-0.6.2/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.613833 zettel_org-0.6.2/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.613833 zettel_org-0.6.2/src/zorg/app/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.613833 zettel_org-0.6.2/src/zorg/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/app/runners/_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.613833 zettel_org-0.6.2/src/zorg/domain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.613833 zettel_org-0.6.2/src/zorg/domain/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/domain/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/domain/messages/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/domain/messages/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/domain/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.613833 zettel_org-0.6.2/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.617833 zettel_org-0.6.2/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   118898 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/grammar/zorg_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.617833 zettel_org-0.6.2/src/zorg/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/service/zid_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.617833 zettel_org-0.6.2/src/zorg/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.617833 zettel_org-0.6.2/src/zorg/storage/file/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/file/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/file/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.617833 zettel_org-0.6.2/src/zorg/storage/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/sql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/sql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/sql/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-15 13:53:31.000000 zettel_org-0.6.2/src/zorg/storage/sql/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-15 13:53:31.000000 zettel_org-0.6.2/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.621833 zettel_org-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.621833 zettel_org-0.6.2/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    70292 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/__snapshots__/test_run_db.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:53:40.621833 zettel_org-0.6.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-15 13:53:31.000000 zettel_org-0.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.958402 zettel_org-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 15:39:31.000000 zettel_org-0.6.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-19 15:39:31.000000 zettel_org-0.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 15:39:31.000000 zettel_org-0.6.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-19 15:39:31.000000 zettel_org-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-19 15:39:31.000000 zettel_org-0.6.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-19 15:39:31.000000 zettel_org-0.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-19 15:39:39.958402 zettel_org-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-19 15:39:31.000000 zettel_org-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2662 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-19 15:39:31.000000 zettel_org-0.6.3/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.938402 zettel_org-0.6.3/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 15:39:31.000000 zettel_org-0.6.3/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 15:39:31.000000 zettel_org-0.6.3/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.930402 zettel_org-0.6.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 15:39:31.000000 zettel_org-0.6.3/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 15:39:31.000000 zettel_org-0.6.3/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 15:39:31.000000 zettel_org-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-19 15:39:31.000000 zettel_org-0.6.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.942402 zettel_org-0.6.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 15:39:31.000000 zettel_org-0.6.3/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-19 15:39:39.958402 zettel_org-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-19 15:39:31.000000 zettel_org-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.930402 zettel_org-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.958402 zettel_org-0.6.3/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:39:36.000000 zettel_org-0.6.3/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 15:39:39.000000 zettel_org-0.6.3/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.946402 zettel_org-0.6.3/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/messages/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118898 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/grammar/zorg_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.950402 zettel_org-0.6.3/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/src/zorg/storage/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/file/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/file/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-19 15:39:31.000000 zettel_org-0.6.3/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-19 15:39:31.000000 zettel_org-0.6.3/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.954402 zettel_org-0.6.3/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    70292 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:39:39.958402 zettel_org-0.6.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 15:39:31.000000 zettel_org-0.6.3/tox.ini
```

### Comparing `zettel_org-0.6.2/.cruft.json` & `zettel_org-0.6.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/.github/labels.yml` & `zettel_org-0.6.3/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/.github/workflows/ci.yml` & `zettel_org-0.6.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/.gitignore` & `zettel_org-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/.pylintrc` & `zettel_org-0.6.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/.readthedocs.yml` & `zettel_org-0.6.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/CHANGELOG.md` & `zettel_org-0.6.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,28 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.2...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.3...HEAD)
 
 No notable changes have been made.
 
 
-## [0.6.1](https://github.com/bbugyi200/zorg/compare/0.6.1...0.6.2) - 2024-04-14
+## [0.6.3](https://github.com/bbugyi200/zorg/compare/0.6.2...0.6.3) - 2024-04-19
+
+### Fixed
+
+* Fix bug where absolute filename was used to key file hash. This was causing
+  the file hash map to not be portable across different machines.
+
+
+## [0.6.2](https://github.com/bbugyi200/zorg/compare/0.6.1...0.6.2) - 2024-04-14
 
 ### Fixed
 
 * Fix crash from trying to convert deleted entity.
 
 
 ## [0.6.1](https://github.com/bbugyi200/zorg/compare/0.6.0...0.6.1) - 2024-04-10
```

### Comparing `zettel_org-0.6.2/CONTRIBUTING.md` & `zettel_org-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/Dockerfile` & `zettel_org-0.6.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/Makefile` & `zettel_org-0.6.3/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/PKG-INFO` & `zettel_org-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.2
+Version: 0.6.3
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `zettel_org-0.6.2/README.md` & `zettel_org-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/bin/build_zorg_grammars` & `zettel_org-0.6.3/bin/build_zorg_grammars`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/bin/check_cc` & `zettel_org-0.6.3/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/bin/publish_docs` & `zettel_org-0.6.3/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/bin/quick-lints` & `zettel_org-0.6.3/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/bin/render_all_cogs` & `zettel_org-0.6.3/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/docs/Makefile` & `zettel_org-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/docs/make.bat` & `zettel_org-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/docs/source/conf.py` & `zettel_org-0.6.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/examples/zorg_file/20240323.zo` & `zettel_org-0.6.3/examples/zorg_file/20240323.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/examples/zorg_file/scrambled_prj_notes.zo` & `zettel_org-0.6.3/examples/zorg_file/scrambled_prj_notes.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/lib/bugyi.sh` & `zettel_org-0.6.3/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/requirements-dev.in` & `zettel_org-0.6.3/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/requirements-dev.txt` & `zettel_org-0.6.3/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 distlib==0.3.8
     # via virtualenv
 docutils==0.20.1
     # via
     #   m2r2
     #   sphinx
     #   sphinx-rtd-theme
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 filelock==3.13.4
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0
     # via -r requirements-dev.in
@@ -237,21 +237,21 @@
     #   tox
 smmap==5.0.1
     # via gitdb
 snowballstemmer==2.2.0
     # via
     #   pydocstyle
     #   sphinx
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r requirements-dev.in
     #   sphinx-autodoc-typehints
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-autodoc-typehints==2.0.1
+sphinx-autodoc-typehints==2.1.0
     # via -r requirements-dev.in
 sphinx-rtd-theme==2.0.0
     # via -r requirements-dev.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
@@ -287,14 +287,15 @@
     #   mypy
     #   pip-tools
     #   pydocstyle
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   setuptools-scm
+    #   sphinx
     #   tox
 tomlkit==0.12.4
     # via pylint
 tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
@@ -304,15 +305,15 @@
     # via
     #   -r requirements.in
     #   zettel-org
 typer==0.12.3
     # via cruft
 types-python-dateutil==2.9.0.20240316
     # via arrow
-types-tqdm==4.66.0.20240106
+types-tqdm==4.66.0.20240417
     # via -r requirements-dev.in
 typing-extensions==4.11.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
@@ -322,15 +323,15 @@
     #   typer
 urllib3==2.2.1
     # via requests
 vimala==0.2.0
     # via
     #   -r requirements.in
     #   zettel-org
-virtualenv==20.25.1
+virtualenv==20.25.3
     # via tox
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via pip-tools
```

### Comparing `zettel_org-0.6.2/requirements.txt` & `zettel_org-0.6.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/setup.cfg` & `zettel_org-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/setup.py` & `zettel_org-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.6.2"}
+USE_SCM_VERSION = {"fallback_version": "0.6.3"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `zettel_org-0.6.2/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.6.3/src/zettel_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.2
+Version: 0.6.3
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `zettel_org-0.6.2/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.6.3/src/zettel_org.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/app/config.py` & `zettel_org-0.6.3/src/zorg/app/config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/app/runners/__init__.py` & `zettel_org-0.6.3/src/zorg/app/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/app/runners/_run_action.py` & `zettel_org-0.6.3/src/zorg/app/runners/_run_action.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/app/runners/_run_compile.py` & `zettel_org-0.6.3/src/zorg/app/runners/_run_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ..config import CompileConfig
 from ._runners import runner
 
 
 @runner
 def run_compile(cfg: CompileConfig) -> int:
     """Runner for the 'compile' command."""
-    zorg_file = walk_zorg_file(cfg.zo_path, verbose=True)
+    zorg_file = walk_zorg_file(cfg.zettel_dir, cfg.zo_path, verbose=True)
     zorg_file_dict = _convert_zorg_file_to_dict(zorg_file)
     pprint(zorg_file_dict)
     return 0
 
 
 def _convert_zorg_file_to_dict(zorg_file: ZorgFile) -> dict[str, Any]:
     zorg_file_dict = asdict(zorg_file)
```

### Comparing `zettel_org-0.6.2/src/zorg/app/runners/_run_db.py` & `zettel_org-0.6.3/src/zorg/app/runners/_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/app/runners/_run_edit.py` & `zettel_org-0.6.3/src/zorg/app/runners/_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/app/runners/_run_template.py` & `zettel_org-0.6.3/src/zorg/app/runners/_run_template.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/domain/messages/commands.py` & `zettel_org-0.6.3/src/zorg/domain/messages/commands.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/domain/messages/events.py` & `zettel_org-0.6.3/src/zorg/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/domain/models.py` & `zettel_org-0.6.3/src/zorg/domain/models.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/domain/types.py` & `zettel_org-0.6.3/src/zorg/domain/types.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFile.g4` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.g4`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFile.tokens` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFile.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.6.3/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/service/common.py` & `zettel_org-0.6.3/src/zorg/service/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/service/compiler.py` & `zettel_org-0.6.3/src/zorg/service/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,16 +406,21 @@
             self._s.h3_tags[tag_name].append(text)
         elif self._s.in_h4_header:
             self._s.h4_tags[tag_name].append(text)
         elif self._s.in_note:
             self._s.note_tags[tag_name].append(text)
 
 
-def walk_zorg_file(zo_path: Path, verbose: bool = False) -> ZorgFile:
+def walk_zorg_file(
+    zdir: Path, zo_path_part: Path, verbose: bool = False
+) -> ZorgFile:
     """Create a new _ZorgFileCompiler and walk through notes in {zorg_file}."""
+    zo_path = (
+        zo_path_part if zo_path_part.is_absolute() else zdir / zo_path_part
+    )
     zorg_file = ZorgFile(zo_path)
     stream = antlr4.FileStream(zorg_file.path, errors="ignore")
     lexer = ZorgFileLexer(stream)
     tokens = antlr4.CommonTokenStream(lexer)
     parser = ZorgFileParser(tokens)
     if not verbose:
         parser.removeErrorListeners()
```

### Comparing `zettel_org-0.6.2/src/zorg/service/file_groups.py` & `zettel_org-0.6.3/src/zorg/service/file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/service/handlers.py` & `zettel_org-0.6.3/src/zorg/service/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     total_num_todos = 0
     for zo_path in tqdm(
         sorted(cmd.zettel_dir.rglob("*.zo"), key=lambda p: p.name),
         desc="Reading notes from zorg files",
         file=sys.stdout,
     ):
         logger.info("Starting to walk zorg file", zorg_file=zo_path.name)
-        zorg_file = walk_zorg_file(zo_path)
+        zorg_file = walk_zorg_file(cmd.zettel_dir, zo_path)
         num_notes = len(zorg_file.notes)
         num_todos = len(
             [note for note in zorg_file.notes if note.todo_payload]
         )
         total_num_notes += num_notes
         total_num_todos += num_todos
         logger.info(
@@ -117,15 +117,17 @@
 def reindex_database(
     cmd: commands.ReindexDBCommand, session: SQLSession
 ) -> None:
     """Reindex an existing zorg database."""
     paths = cmd.paths if cmd.paths else sorted(cmd.zettel_dir.rglob("*.zo"))
     file_to_hash: dict[str, str] = {}
     for path in paths:
-        file_to_hash[str(path)] = _hash_file(path)
+        file_to_hash[str(path).replace(f"{cmd.zettel_dir}/", "")] = _hash_file(
+            path
+        )
 
     zorg_data_dir = cmd.zettel_dir / f".{APP_NAME}"
     zorg_data_dir.mkdir(parents=True, exist_ok=True)
     file_hash_path = zorg_data_dir / "file_hash.json"
     old_file_to_hash: dict[str, str] = (
         json.loads(file_hash_path.read_bytes())
         if file_hash_path.exists()
@@ -139,15 +141,17 @@
         ):
             logger.info("Changed file", file=file)
             old_zorg_file = session.repo.get(file).unwrap()
             if old_zorg_file is not None:
                 logger.info("Removing file from DB", file=file)
                 session.repo.remove_by_key(str(old_zorg_file.path))
 
-            zorg_file = walk_zorg_file(Path(file), verbose=cmd.verbose)
+            zorg_file = walk_zorg_file(
+                cmd.zettel_dir, Path(file), verbose=cmd.verbose
+            )
             logger.info("Adding zorg file", file=file)
             session.repo.add(zorg_file)
 
     logger.debug("Writing hash map to disk", file=str(file_hash_path))
     with file_hash_path.open("w") as f:
         json.dump(dict(sorted(file_to_hash.items())), f, indent=4)
 
@@ -186,14 +190,27 @@
         "Adding ZIDs to zorg file",
         zorg_file=event.zorg_file_path,
         new_notes=len(event.new_notes),
     )
     event.zorg_file_path.write_text("\n".join(zlines))
 
 
+def increment_zid_counters(
+    event: events.DBModifiedEvent, session: SQLSession
+) -> None:
+    """Increment the date-specific zorg ID counters.
+
+    These are stored in a directory in your zettel dir and are used when
+    generating new IDs (they are the XX in the YYMMDD#XX ID format).
+    """
+    del session
+    zid_manager = ZIDManager(event.zettel_dir)
+    zid_manager.write_to_disk()
+
+
 def _add_zid_to_line(zid: str, line: str) -> str:
     all_words = line.split(" ")
 
     num_spaces = 0
     while all_words[0] == "":
         num_spaces += 1
         all_words.pop(0)
@@ -232,27 +249,14 @@
         chunk = file.read(chunk_size)
         while chunk:
             hasher.update(chunk)
             chunk = file.read(chunk_size)
     return hasher.hexdigest()
 
 
-def increment_zid_counters(
-    event: events.DBModifiedEvent, session: SQLSession
-) -> None:
-    """Increment the date-specific zorg ID counters.
-
-    These are stored in a directory in your zettel dir and are used when
-    generating new IDs (they are the XX in the YYMMDD#XX ID format).
-    """
-    del session
-    zid_manager = ZIDManager(event.zettel_dir)
-    zid_manager.write_to_disk()
-
-
 def _process_vim_commands(
     zettel_dir: Path, vim_commands: Iterable[str]
 ) -> Iterator[str]:
     for vim_cmd in vim_commands:
         if "{zdir}" in vim_cmd:
             yield vim_cmd.format(zdir=zettel_dir)
         else:
```

### Comparing `zettel_org-0.6.2/src/zorg/service/messagebus.py` & `zettel_org-0.6.3/src/zorg/service/messagebus.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/service/templates.py` & `zettel_org-0.6.3/src/zorg/service/templates.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/service/zid_manager.py` & `zettel_org-0.6.3/src/zorg/service/zid_manager.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/storage/sql/converters.py` & `zettel_org-0.6.3/src/zorg/storage/sql/converters.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/storage/sql/engine.py` & `zettel_org-0.6.3/src/zorg/storage/sql/engine.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/storage/sql/models.py` & `zettel_org-0.6.3/src/zorg/storage/sql/models.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/storage/sql/repo.py` & `zettel_org-0.6.3/src/zorg/storage/sql/repo.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/src/zorg/storage/sql/session.py` & `zettel_org-0.6.3/src/zorg/storage/sql/session.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/targets.mk` & `zettel_org-0.6.3/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/__snapshots__/test_run_compile.ambr` & `zettel_org-0.6.3/tests/__snapshots__/test_run_compile.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/__snapshots__/test_run_db.ambr` & `zettel_org-0.6.3/tests/__snapshots__/test_run_db.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.6.3/tests/__snapshots__/test_run_edit.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.6.3/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/common.py` & `zettel_org-0.6.3/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/conftest.py` & `zettel_org-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/data/day_log.zot` & `zettel_org-0.6.3/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/data/done_log.zot` & `zettel_org-0.6.3/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/data/habit_log.zot` & `zettel_org-0.6.3/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/test_config.py` & `zettel_org-0.6.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/test_file_groups.py` & `zettel_org-0.6.3/tests/test_file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/test_run_action_open.py` & `zettel_org-0.6.3/tests/test_run_action_open.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/test_run_compile.py` & `zettel_org-0.6.3/tests/test_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/test_run_db.py` & `zettel_org-0.6.3/tests/test_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.2/tests/test_run_edit.py` & `zettel_org-0.6.3/tests/test_run_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,19 @@
             ["vim", str(zettel_dir / "foobar.zo")],
             stdout=None,
             stderr=None,
             timeout=None,
         ),
         call().unwrap(),
         call(
-            ["vim", str(zettel_dir / "baz.zo"), str(zettel_dir / "buz.zo")],
+            [
+                "vim",
+                str(zettel_dir / "baz.zo"),
+                str(zettel_dir / "buz.zo"),
+            ],
             stdout=None,
             stderr=None,
             timeout=None,
         ),
         call().unwrap(),
     ])
     assert vim_proc_mock.call_count == 2
```

### Comparing `zettel_org-0.6.2/tests/test_run_template.py` & `zettel_org-0.6.3/tests/test_run_template.py`

 * *Files identical despite different names*

