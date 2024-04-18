# Comparing `tmp/mkdoxy-1.2.0.tar.gz` & `tmp/mkdoxy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.2.0.tar", last modified: Tue Apr  2 23:48:25 2024, max compression
+gzip compressed data, was "mkdoxy-1.2.1.tar", last modified: Thu Apr 18 23:47:09 2024, max compression
```

## Comparing `mkdoxy-1.2.0.tar` & `mkdoxy-1.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.912005 mkdoxy-1.2.0/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.0/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5999 2024-04-02 23:48:25.911688 mkdoxy-1.2.0/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.2.0/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.903595 mkdoxy-1.2.0/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2935 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.0/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      303 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     3585 2023-11-09 12:15:43.000000 mkdoxy-1.2.0/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     5619 2024-04-02 23:45:50.000000 mkdoxy-1.2.0/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     9922 2024-04-02 23:43:22.000000 mkdoxy-1.2.0/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-02 23:45:50.000000 mkdoxy-1.2.0/mkdoxy/filters.py
--rw-r--r--   0 kuba       (501) staff       (20)     2414 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-02-14 21:55:15.000000 mkdoxy-1.2.0/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    19728 2024-04-02 23:45:52.000000 mkdoxy-1.2.0/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    15034 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    26618 2024-04-02 23:45:55.000000 mkdoxy-1.2.0/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     9076 2024-04-02 23:43:22.000000 mkdoxy-1.2.0/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)    11685 2024-04-02 23:45:56.000000 mkdoxy-1.2.0/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.910061 mkdoxy-1.2.0/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.2.0/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.2.0/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.2.0/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      614 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      582 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      408 2023-12-27 13:57:12.000000 mkdoxy-1.2.0/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      499 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      438 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      791 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.2.0/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.2.0/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      414 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-02 21:46:08.000000 mkdoxy-1.2.0/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      233 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3534 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-02 23:45:59.000000 mkdoxy-1.2.0/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.910717 mkdoxy-1.2.0/mkdoxy.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     5999 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1127 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      156 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-04-02 23:48:25.000000 mkdoxy-1.2.0/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       62 2023-10-10 12:59:26.000000 mkdoxy-1.2.0/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)       38 2024-04-02 23:48:25.912063 mkdoxy-1.2.0/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1869 2024-04-02 23:43:44.000000 mkdoxy-1.2.0/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-02 23:48:25.910318 mkdoxy-1.2.0/tests/
--rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-02 23:43:22.000000 mkdoxy-1.2.0/tests/test_doxyrun.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-18 23:47:09.735925 mkdoxy-1.2.1/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.1/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-04-18 23:47:09.735682 mkdoxy-1.2.1/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4473 2024-04-18 23:45:18.000000 mkdoxy-1.2.1/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-18 23:47:09.731995 mkdoxy-1.2.1/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2935 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.1/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      303 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3585 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5619 2024-04-18 23:46:38.000000 mkdoxy-1.2.1/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9921 2024-04-18 23:45:10.000000 mkdoxy-1.2.1/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/mkdoxy/filters.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2414 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-04-18 23:45:14.000000 mkdoxy-1.2.1/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    19743 2024-04-18 23:46:40.000000 mkdoxy-1.2.1/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    15034 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    26618 2024-04-18 23:46:44.000000 mkdoxy-1.2.1/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9076 2024-04-18 23:45:10.000000 mkdoxy-1.2.1/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11689 2024-04-18 23:46:45.000000 mkdoxy-1.2.1/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-18 23:47:09.734711 mkdoxy-1.2.1/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      614 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      582 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      408 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      499 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      438 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      797 2024-04-18 23:45:18.000000 mkdoxy-1.2.1/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-18 23:45:14.000000 mkdoxy-1.2.1/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      414 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      233 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3534 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-18 23:46:47.000000 mkdoxy-1.2.1/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-18 23:47:09.734991 mkdoxy-1.2.1/mkdoxy.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-04-18 23:47:09.000000 mkdoxy-1.2.1/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1127 2024-04-18 23:47:09.000000 mkdoxy-1.2.1/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-04-18 23:47:09.000000 mkdoxy-1.2.1/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-04-18 23:47:09.000000 mkdoxy-1.2.1/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      143 2024-04-18 23:47:09.000000 mkdoxy-1.2.1/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-04-18 23:47:09.000000 mkdoxy-1.2.1/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       62 2024-04-02 23:57:40.000000 mkdoxy-1.2.1/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2024-04-18 23:47:09.735964 mkdoxy-1.2.1/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1841 2024-04-18 23:45:58.000000 mkdoxy-1.2.1/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-18 23:47:09.734830 mkdoxy-1.2.1/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-03 00:10:24.000000 mkdoxy-1.2.1/tests/test_doxyrun.py
```

### Comparing `mkdoxy-1.2.0/LICENSE` & `mkdoxy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/PKG-INFO` & `mkdoxy-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.2.0
+Version: 1.2.1
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
@@ -17,19 +17,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs
 Provides-Extra: dev
-Requires-Dist: mkdocs-material~=9.1.18; extra == "dev"
-Requires-Dist: Jinja2~=3.1.2; extra == "dev"
+Requires-Dist: mkdocs-material~=9.5.18; extra == "dev"
+Requires-Dist: Jinja2~=3.1.3; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev"
 Requires-Dist: pathlib~=1.0.1; extra == "dev"
-Requires-Dist: path~=16.7.1; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
 Requires-Dist: pytest~=6.2.5; extra == "dev"
 Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 
 # MkDoxy
 
 **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown files.
@@ -38,19 +37,19 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/blob/main/LICENSE" target="_blank"><img src="https://img.shields.io/github/license/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/releases" target="_blank"><img src="https://img.shields.io/github/v/release/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/forks" target="_blank"><img src="https://img.shields.io/github/forks/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/issues" target="_blank"><img src="https://img.shields.io/github/issues/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/discussions" target="_blank"><img src="https://img.shields.io/github/discussions/JakubAndrysek/MkDoxy?style=flat-square"></a>
-<a href="https://pypistats.org/packages/mkdoxy" target="_blank"><img src="https://static.pepy.tech/personalized-badge/mkdoxy?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads"></a>
+<a href="https://www.pepy.tech/projects/mkdoxy" target="_blank"><img src="https://static.pepy.tech/badge/mkdoxy"></a>
 </p>
 
 > **Warning**
-> **Extension is in development** and few features are not working properly.
+> **Extension is in development**, and a few features are not working properly.
 > More information in [Discussions](https://github.com/JakubAndrysek/MkDoxy/discussions) and [Issues](https://github.com/JakubAndrysek/MkDoxy/issues) pages.
 
 ---
 
 ## [:material-home-edit: Online Demo](https://jakubandrysek.github.io/MkDoxy-demo/) and [:simple-github: Demo source-code ](https://github.com/JakubAndrysek/MkDoxy-demo)
 
 ---
@@ -99,15 +98,15 @@
           full-doc: True # if you want to generate full documentation
           doxy-cfg: # standard doxygen configuration (key: value)
             FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out
             RECURSIVE: True # recursive search in source directories
 ```
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you want to change.
 
 ## Do You Enjoy MkDoxy or Does It Save You Time?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
```

#### html2text {}

```diff
@@ -1,42 +1,40 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.0 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.1 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: mkdocs Provides-Extra: dev Requires-Dist: mkdocs-
-material~=9.1.18; extra == "dev" Requires-Dist: Jinja2~=3.1.2; extra == "dev"
+material~=9.5.18; extra == "dev" Requires-Dist: Jinja2~=3.1.3; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev" Requires-Dist:
-pathlib~=1.0.1; extra == "dev" Requires-Dist: path~=16.7.1; extra == "dev"
-Requires-Dist: isort~=5.12.0; extra == "dev" Requires-Dist: pytest~=6.2.5;
-extra == "dev" Requires-Dist: pre-commit~=3.7.0; extra == "dev" # MkDoxy **
-[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://
-www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://
-www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown
-files.
+pathlib~=1.0.1; extra == "dev" Requires-Dist: isort~=5.12.0; extra == "dev"
+Requires-Dist: pytest~=6.2.5; extra == "dev" Requires-Dist: pre-commit~=3.7.0;
+extra == "dev" # MkDoxy **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin
+for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on
+**[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)**
+in your markdown files.
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_J_a_k_u_b_A_n_d_r_y_s_e_k_%_2_F_M_k_D_o_x_y_&_c_o_u_n_t___b_g_=_%_2_3_7_9_C_8_3_D_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_t_r_u_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
        _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_i_s_c_u_s_s_i_o_n_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/
-    _M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
-_m_k_d_o_x_y_?_p_e_r_i_o_d_=_m_o_n_t_h_&_u_n_i_t_s_=_i_n_t_e_r_n_a_t_i_o_n_a_l___s_y_s_t_e_m_&_l_e_f_t___c_o_l_o_r_=_b_l_a_c_k_&_r_i_g_h_t___c_o_l_o_r_=_o_r_a_n_g_e_&_l_e_f_t___t_e_x_t_=_D_o_w_n_l_o_a_d_s_]
-> **Warning** > **Extension is in development** and few features are not
+       _M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_k_d_o_x_y_]
+> **Warning** > **Extension is in development**, and a few features are not
 working properly. > More information in [Discussions](https://github.com/
 JakubAndrysek/MkDoxy/discussions) and [Issues](https://github.com/
 JakubAndrysek/MkDoxy/issues) pages. --- ## [:material-home-edit: Online Demo]
 (https://jakubandrysek.github.io/MkDoxy-demo/) and [:simple-github: Demo
 source-code ](https://github.com/JakubAndrysek/MkDoxy-demo) --- **[Feature
 List](#feature-list)** - **[Installation](#installation)** - **[Quick start]
 (#quick-start)** ## Feature List - **[Easy to use](#quick-start):**: Just add
@@ -59,14 +57,14 @@
 myProjectCpp: # name of project must be alphanumeric + numbers (without spaces)
 src-dirs: path/to/src/project1 # path to source code (support multiple paths
 separated by space) => INPUT full-doc: True # if you want to generate full
 documentation doxy-cfg: # standard doxygen configuration (key: value)
 FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out RECURSIVE:
 True # recursive search in source directories ``` ## Contributing Pull requests
 are welcome. For major changes, please open an issue first to discuss what you
-would like to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
+want to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
 definitely consider: - supporting me on GitHub Sponsors: [![](https://
 img.shields.io/static/
 v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
 github.com/sponsors/jakubandrysek) ## License This project is licensed under
 the terms of the [MIT license](https://github.com/JakubAndrysek/MkDoxy/blob/
 main/LICENSE)
```

### Comparing `mkdoxy-1.2.0/README.md` & `mkdoxy-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/blob/main/LICENSE" target="_blank"><img src="https://img.shields.io/github/license/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/releases" target="_blank"><img src="https://img.shields.io/github/v/release/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/forks" target="_blank"><img src="https://img.shields.io/github/forks/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/issues" target="_blank"><img src="https://img.shields.io/github/issues/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/discussions" target="_blank"><img src="https://img.shields.io/github/discussions/JakubAndrysek/MkDoxy?style=flat-square"></a>
-<a href="https://pypistats.org/packages/mkdoxy" target="_blank"><img src="https://static.pepy.tech/personalized-badge/mkdoxy?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads"></a>
+<a href="https://www.pepy.tech/projects/mkdoxy" target="_blank"><img src="https://static.pepy.tech/badge/mkdoxy"></a>
 </p>
 
 > **Warning**
-> **Extension is in development** and few features are not working properly.
+> **Extension is in development**, and a few features are not working properly.
 > More information in [Discussions](https://github.com/JakubAndrysek/MkDoxy/discussions) and [Issues](https://github.com/JakubAndrysek/MkDoxy/issues) pages.
 
 ---
 
 ## [:material-home-edit: Online Demo](https://jakubandrysek.github.io/MkDoxy-demo/) and [:simple-github: Demo source-code ](https://github.com/JakubAndrysek/MkDoxy-demo)
 
 ---
@@ -67,15 +67,15 @@
           full-doc: True # if you want to generate full documentation
           doxy-cfg: # standard doxygen configuration (key: value)
             FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out
             RECURSIVE: True # recursive search in source directories
 ```
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you want to change.
 
 ## Do You Enjoy MkDoxy or Does It Save You Time?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
```

#### html2text {}

```diff
@@ -6,17 +6,16 @@
 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_J_a_k_u_b_A_n_d_r_y_s_e_k_%_2_F_M_k_D_o_x_y_&_c_o_u_n_t___b_g_=_%_2_3_7_9_C_8_3_D_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_t_r_u_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
        _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_i_s_c_u_s_s_i_o_n_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/
-    _M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
-_m_k_d_o_x_y_?_p_e_r_i_o_d_=_m_o_n_t_h_&_u_n_i_t_s_=_i_n_t_e_r_n_a_t_i_o_n_a_l___s_y_s_t_e_m_&_l_e_f_t___c_o_l_o_r_=_b_l_a_c_k_&_r_i_g_h_t___c_o_l_o_r_=_o_r_a_n_g_e_&_l_e_f_t___t_e_x_t_=_D_o_w_n_l_o_a_d_s_]
-> **Warning** > **Extension is in development** and few features are not
+       _M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_k_d_o_x_y_]
+> **Warning** > **Extension is in development**, and a few features are not
 working properly. > More information in [Discussions](https://github.com/
 JakubAndrysek/MkDoxy/discussions) and [Issues](https://github.com/
 JakubAndrysek/MkDoxy/issues) pages. --- ## [:material-home-edit: Online Demo]
 (https://jakubandrysek.github.io/MkDoxy-demo/) and [:simple-github: Demo
 source-code ](https://github.com/JakubAndrysek/MkDoxy-demo) --- **[Feature
 List](#feature-list)** - **[Installation](#installation)** - **[Quick start]
 (#quick-start)** ## Feature List - **[Easy to use](#quick-start):**: Just add
@@ -39,14 +38,14 @@
 myProjectCpp: # name of project must be alphanumeric + numbers (without spaces)
 src-dirs: path/to/src/project1 # path to source code (support multiple paths
 separated by space) => INPUT full-doc: True # if you want to generate full
 documentation doxy-cfg: # standard doxygen configuration (key: value)
 FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out RECURSIVE:
 True # recursive search in source directories ``` ## Contributing Pull requests
 are welcome. For major changes, please open an issue first to discuss what you
-would like to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
+want to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
 definitely consider: - supporting me on GitHub Sponsors: [![](https://
 img.shields.io/static/
 v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
 github.com/sponsors/jakubandrysek) ## License This project is licensed under
 the terms of the [MIT license](https://github.com/JakubAndrysek/MkDoxy/blob/
 main/LICENSE)
```

### Comparing `mkdoxy-1.2.0/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.2.1/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/constants.py` & `mkdoxy-1.2.1/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/doxygen.py` & `mkdoxy-1.2.1/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/doxyrun.py` & `mkdoxy-1.2.1/mkdoxy/doxyrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class DoxygenRun:
     """! Class for running Doxygen.
-    @detailss This class is used to run Doxygen and parse the XML output.
+    @details This class is used to run Doxygen and parse the XML output.
     """
 
     def __init__(
         self,
         doxygenBinPath: str,
         doxygenSource: str,
         tempDoxyFolder: str,
@@ -33,15 +33,15 @@
         - GENERATE_XML: YES
         - RECURSIVE: YES
         - EXAMPLE_PATH: examples
         - SHOW_NAMESPACES: YES
         - GENERATE_HTML: NO
         - GENERATE_LATEX: NO
 
-        @detailss
+        @details
         @param doxygenBinPath: (str) Path to the Doxygen binary.
         @param doxygenSource: (str) Source files for Doxygen.
         @param tempDoxyFolder: (str) Temporary folder for Doxygen.
         @param doxyConfigFile: (str) Path to a Doxygen config file.
         @param doxyCfgNew: (dict) New Doxygen config options that will be added to the default config (new options will overwrite default options)
         """  # noqa: E501
 
@@ -112,30 +112,30 @@
         doxyCfg.update(doxyCfgNew)
         doxyCfg["INPUT"] = self.doxygenSource
         doxyCfg["OUTPUT_DIRECTORY"] = self.tempDoxyFolder
         return doxyCfg
 
     def is_doxygen_valid_path(self, doxygen_bin_path: str) -> bool:
         """! Check if the Doxygen binary path is valid.
-        @detailss Accepts a full path or just 'doxygen' if it exists in the system's PATH.
+        @details Accepts a full path or just 'doxygen' if it exists in the system's PATH.
         @param doxygen_bin_path: (str) The path to the Doxygen binary or just 'doxygen'.
         @return: (bool) True if the Doxygen binary path is valid, False otherwise.
         """
         # If the path is just 'doxygen', search for it in the system's PATH
         if doxygen_bin_path.lower() == "doxygen":
             return shutil.which("doxygen") is not None
 
         # Use pathlib to check if the provided full path is a file and executable
         path = Path(doxygen_bin_path)
         return path.is_file() and os.access(path, os.X_OK)
 
     # Source of dox_dict2str: https://xdress-fabio.readthedocs.io/en/latest/_modules/xdress/doxygen.html#XDressPlugin
     def dox_dict2str(self, dox_dict: dict) -> str:
         """! Convert a dictionary to a string that can be written to a doxygen config file.
-        @detailss
+        @details
         @param dox_dict: (dict) Dictionary to convert.
         @return: (str) String that can be written to a doxygen config file.
         """
         s = ""
         new_line = "{option} = {value}\n"
         for key, value in dox_dict.items():
             if value is True:
@@ -148,15 +148,15 @@
             s += new_line.format(option=key.upper(), value=_value)
 
         # Don't need an empty line at the end
         return s.strip()
 
     def str2dox_dict(self, dox_str: str) -> dict:
         """! Convert a string from a doxygen config file to a dictionary.
-        @detailss
+        @details
         @param dox_str: (str) String from a doxygen config file.
         @return: (dict) Dictionary.
         """
         dox_dict = {}
         try:
             for line in dox_str.split("\n"):
                 if line.strip() == "":
@@ -172,17 +172,17 @@
             raise DoxygenCustomConfigNotValid(
                 f"Invalid custom Doxygen config file: {self.doxyConfigFile}\n"
                 f"Make sure the file is in standard Doxygen format."
                 f"Look at https://mkdoxy.kubaandrysek.cz/usage/advanced/."
             ) from e
         return dox_dict
 
-    def hasChanged(self):
+    def hasChanged(self) -> bool:
         """! Check if the source files have changed since the last run.
-        @detailss
+        @details
         @return: (bool) True if the source files have changed since the last run.
         """
 
         def hashWrite(filename: PurePath, hash: str):
             with open(filename, "w") as file:
                 file.write(hash)
 
@@ -213,41 +213,41 @@
                 return False
 
         hashWrite(self.hashFilePath, hashNew)
         return True
 
     def run(self):
         """! Run Doxygen with the current configuration using the Popen class.
-        @detailss
+        @details
         """
         doxyBuilder = Popen(
             [self.doxygenBinPath, "-"],
             stdout=PIPE,
             stdin=PIPE,
             stderr=PIPE,
             cwd=self.runPath,
         )
         (doxyBuilder.communicate(self.dox_dict2str(self.doxyCfg).encode("utf-8"))[0].decode().strip())
         # log.info(self.destinationDir)
         # log.info(stdout_data)
 
     def checkAndRun(self):
         """! Check if the source files have changed since the last run and run Doxygen if they have.
-        @detailss
+        @details
         @return: (bool) True if Doxygen was run.
         """
         if self.hasChanged():
             self.run()
             return True
         else:
             return False
 
     def getOutputFolder(self) -> PurePath:
         """! Get the path to the XML output folder.
-        @detailss
+        @details
         @return: (PurePath) Path to the XML output folder.
         """
         return Path.joinpath(Path(self.tempDoxyFolder), Path("xml"))
 
 
 # not valid path exception
 class DoxygenBinPathNotValid(Exception):
```

### Comparing `mkdoxy-1.2.0/mkdoxy/filters.py` & `mkdoxy-1.2.1/mkdoxy/filters.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/finder.py` & `mkdoxy-1.2.1/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/generatorAuto.py` & `mkdoxy-1.2.1/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/generatorBase.py` & `mkdoxy-1.2.1/mkdoxy/generatorBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             # load custom templates and overwrite default templates - if they exist
             for fileName in os.listdir(templateDir):
                 filePath = os.path.join(templateDir, fileName)
                 if fileName.endswith(".jinja2"):
                     with open(filePath, "r") as file:
                         name = os.path.splitext(fileName)[0]
                         fileTemplate, metaData = parseTemplateFile(file.read())
-                        self.templates[name] = Template(fileTemplate)
+                        self.templates[name] = environment.from_string(fileTemplate)
                         self.metaData[name] = metaData
                         log.info(f"Overwriting template '{name}' with custom template.")
                 else:
                     log.error(f"Trying to load unsupported file '{filePath}'. Supported file ends with '.jinja2'.")
 
     @staticmethod
     def shift_each_line(value: str, shift_char: str = "\t") -> str:
```

### Comparing `mkdoxy-1.2.0/mkdoxy/generatorSnippets.py` & `mkdoxy-1.2.1/mkdoxy/generatorSnippets.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/markdown.py` & `mkdoxy-1.2.1/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/node.py` & `mkdoxy-1.2.1/mkdoxy/node.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/plugin.py` & `mkdoxy-1.2.1/mkdoxy/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/property.py` & `mkdoxy-1.2.1/mkdoxy/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         def __init__(self, xml: Element, parser: XmlParser, kind: Kind):
             self.xml = xml
             self.parser = parser
             self.kind = kind
 
         def md(self, plain: bool = False) -> str:
             briefdescription = self.xml.find("briefdescription")
-            if not briefdescription:
+            if briefdescription is None:
                 return ""
 
             paras = briefdescription.findall("para")
             if len(paras) > 0:
                 text = [self.parser.paras_as_str(para, italic=True, plain=plain) for para in paras]
                 return " ".join(text)
             else:
```

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/code.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/error.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/memDef.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -28,7 +28,9 @@
 {% if configMemDef.get('implements') -%}
 {% if node.reimplements %}
 Implements [*{{node.reimplements.name_long}}*]({{node.reimplements.url}})
 {% endif %}
 {%- endif -%}
 
 {% endfilter %}
+
+<hr>
```

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/templates/member.jinja2` & `mkdoxy-1.2.1/mkdoxy/templates/member.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/utils.py` & `mkdoxy-1.2.1/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy/xml_parser.py` & `mkdoxy-1.2.1/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.2.1/mkdoxy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.2.0
+Version: 1.2.1
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
@@ -17,19 +17,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs
 Provides-Extra: dev
-Requires-Dist: mkdocs-material~=9.1.18; extra == "dev"
-Requires-Dist: Jinja2~=3.1.2; extra == "dev"
+Requires-Dist: mkdocs-material~=9.5.18; extra == "dev"
+Requires-Dist: Jinja2~=3.1.3; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev"
 Requires-Dist: pathlib~=1.0.1; extra == "dev"
-Requires-Dist: path~=16.7.1; extra == "dev"
 Requires-Dist: isort~=5.12.0; extra == "dev"
 Requires-Dist: pytest~=6.2.5; extra == "dev"
 Requires-Dist: pre-commit~=3.7.0; extra == "dev"
 
 # MkDoxy
 
 **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown files.
@@ -38,19 +37,19 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/blob/main/LICENSE" target="_blank"><img src="https://img.shields.io/github/license/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/releases" target="_blank"><img src="https://img.shields.io/github/v/release/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/forks" target="_blank"><img src="https://img.shields.io/github/forks/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/issues" target="_blank"><img src="https://img.shields.io/github/issues/JakubAndrysek/MkDoxy?style=flat-square"></a>
 <a href="https://github.com/JakubAndrysek/MkDoxy/discussions" target="_blank"><img src="https://img.shields.io/github/discussions/JakubAndrysek/MkDoxy?style=flat-square"></a>
-<a href="https://pypistats.org/packages/mkdoxy" target="_blank"><img src="https://static.pepy.tech/personalized-badge/mkdoxy?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads"></a>
+<a href="https://www.pepy.tech/projects/mkdoxy" target="_blank"><img src="https://static.pepy.tech/badge/mkdoxy"></a>
 </p>
 
 > **Warning**
-> **Extension is in development** and few features are not working properly.
+> **Extension is in development**, and a few features are not working properly.
 > More information in [Discussions](https://github.com/JakubAndrysek/MkDoxy/discussions) and [Issues](https://github.com/JakubAndrysek/MkDoxy/issues) pages.
 
 ---
 
 ## [:material-home-edit: Online Demo](https://jakubandrysek.github.io/MkDoxy-demo/) and [:simple-github: Demo source-code ](https://github.com/JakubAndrysek/MkDoxy-demo)
 
 ---
@@ -99,15 +98,15 @@
           full-doc: True # if you want to generate full documentation
           doxy-cfg: # standard doxygen configuration (key: value)
             FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out
             RECURSIVE: True # recursive search in source directories
 ```
 
 ## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+Pull requests are welcome. For major changes, please open an issue first to discuss what you want to change.
 
 ## Do You Enjoy MkDoxy or Does It Save You Time?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
```

#### html2text {}

```diff
@@ -1,42 +1,40 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.0 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.1 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: mkdocs Provides-Extra: dev Requires-Dist: mkdocs-
-material~=9.1.18; extra == "dev" Requires-Dist: Jinja2~=3.1.2; extra == "dev"
+material~=9.5.18; extra == "dev" Requires-Dist: Jinja2~=3.1.3; extra == "dev"
 Requires-Dist: mkdocs-open-in-new-tab~=1.0.2; extra == "dev" Requires-Dist:
-pathlib~=1.0.1; extra == "dev" Requires-Dist: path~=16.7.1; extra == "dev"
-Requires-Dist: isort~=5.12.0; extra == "dev" Requires-Dist: pytest~=6.2.5;
-extra == "dev" Requires-Dist: pre-commit~=3.7.0; extra == "dev" # MkDoxy **
-[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://
-www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://
-www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown
-files.
+pathlib~=1.0.1; extra == "dev" Requires-Dist: isort~=5.12.0; extra == "dev"
+Requires-Dist: pytest~=6.2.5; extra == "dev" Requires-Dist: pre-commit~=3.7.0;
+extra == "dev" # MkDoxy **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin
+for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on
+**[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)**
+in your markdown files.
                  _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_J_a_k_u_b_A_n_d_r_y_s_e_k_%_2_F_M_k_D_o_x_y_&_c_o_u_n_t___b_g_=_%_2_3_7_9_C_8_3_D_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_h_i_t_s_&_e_d_g_e___f_l_a_t_=_t_r_u_e_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_f_o_r_k_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
  _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/_M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-
        _s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_i_s_c_u_s_s_i_o_n_s_/_J_a_k_u_b_A_n_d_r_y_s_e_k_/
-    _M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
-_m_k_d_o_x_y_?_p_e_r_i_o_d_=_m_o_n_t_h_&_u_n_i_t_s_=_i_n_t_e_r_n_a_t_i_o_n_a_l___s_y_s_t_e_m_&_l_e_f_t___c_o_l_o_r_=_b_l_a_c_k_&_r_i_g_h_t___c_o_l_o_r_=_o_r_a_n_g_e_&_l_e_f_t___t_e_x_t_=_D_o_w_n_l_o_a_d_s_]
-> **Warning** > **Extension is in development** and few features are not
+       _M_k_D_o_x_y_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_k_d_o_x_y_]
+> **Warning** > **Extension is in development**, and a few features are not
 working properly. > More information in [Discussions](https://github.com/
 JakubAndrysek/MkDoxy/discussions) and [Issues](https://github.com/
 JakubAndrysek/MkDoxy/issues) pages. --- ## [:material-home-edit: Online Demo]
 (https://jakubandrysek.github.io/MkDoxy-demo/) and [:simple-github: Demo
 source-code ](https://github.com/JakubAndrysek/MkDoxy-demo) --- **[Feature
 List](#feature-list)** - **[Installation](#installation)** - **[Quick start]
 (#quick-start)** ## Feature List - **[Easy to use](#quick-start):**: Just add
@@ -59,14 +57,14 @@
 myProjectCpp: # name of project must be alphanumeric + numbers (without spaces)
 src-dirs: path/to/src/project1 # path to source code (support multiple paths
 separated by space) => INPUT full-doc: True # if you want to generate full
 documentation doxy-cfg: # standard doxygen configuration (key: value)
 FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out RECURSIVE:
 True # recursive search in source directories ``` ## Contributing Pull requests
 are welcome. For major changes, please open an issue first to discuss what you
-would like to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
+want to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
 definitely consider: - supporting me on GitHub Sponsors: [![](https://
 img.shields.io/static/
 v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
 github.com/sponsors/jakubandrysek) ## License This project is licensed under
 the terms of the [MIT license](https://github.com/JakubAndrysek/MkDoxy/blob/
 main/LICENSE)
```

### Comparing `mkdoxy-1.2.0/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.2.1/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.0/setup.py` & `mkdoxy-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name="mkdoxy",
-    version="1.2.0",
+    version="1.2.1",
     description="MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords="mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator",  # noqa: E501
     url="https://github.com/JakubAndrysek/MkDoxy",
     author="Jakub Andrýsek",
     author_email="email@kubaandrysek.cz",
@@ -29,19 +29,18 @@
         "Documentation": "https://mkdoxy.kubaandrysek.cz/",
         "Tracker": "https://github.com/JakubAndrysek/MkDoxy/issues",
         "Funding": "https://github.com/sponsors/jakubandrysek",
     },
     install_requires=["mkdocs"],
     extras_require={
         "dev": [
-            "mkdocs-material~=9.1.18",
-            "Jinja2~=3.1.2",
+            "mkdocs-material~=9.5.18",
+            "Jinja2~=3.1.3",
             "mkdocs-open-in-new-tab~=1.0.2",
             "pathlib~=1.0.1",
-            "path~=16.7.1",
             "isort~=5.12.0",
             "pytest~=6.2.5",
             "pre-commit~=3.7.0",
         ],
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `mkdoxy-1.2.0/tests/test_doxyrun.py` & `mkdoxy-1.2.1/tests/test_doxyrun.py`

 * *Files identical despite different names*

