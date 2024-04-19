# Comparing `tmp/ecjtu-0.1.0.tar.gz` & `tmp/ecjtu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecjtu-0.1.0.tar", max compression
+gzip compressed data, was "ecjtu-0.1.1.tar", max compression
```

## Comparing `ecjtu-0.1.0.tar` & `ecjtu-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-19 21:08:49.256355 ecjtu-0.1.0/LICENSE
--rw-r--r--   0        0        0    16998 2024-04-19 21:08:49.256355 ecjtu-0.1.0/README.md
--rw-r--r--   0        0        0      611 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/__init__.py
--rw-r--r--   0        0        0      179 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/__main__.py
--rw-r--r--   0        0        0    11897 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/client.py
--rw-r--r--   0        0        0     1060 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/constants.py
--rw-r--r--   0        0        0    13901 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/crud.py
--rw-r--r--   0        0        0     2148 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/models.py
--rw-r--r--   0        0        0        0 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/server.py
--rw-r--r--   0        0        0     1640 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/utils/__init__.py
--rw-r--r--   0        0        0     2156 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/utils/logger.py
--rw-r--r--   0        0        0     1311 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/utils/singleton.py
--rw-r--r--   0        0        0     2889 2024-04-19 21:08:49.260355 ecjtu-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    18075 1970-01-01 00:00:00.000000 ecjtu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-19 21:14:13.233436 ecjtu-0.1.1/LICENSE
+-rw-r--r--   0        0        0    16992 2024-04-19 21:14:13.237436 ecjtu-0.1.1/README.md
+-rw-r--r--   0        0        0      611 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/__main__.py
+-rw-r--r--   0        0        0    11897 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/client.py
+-rw-r--r--   0        0        0     1060 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/constants.py
+-rw-r--r--   0        0        0    13901 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/crud.py
+-rw-r--r--   0        0        0     2148 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/models.py
+-rw-r--r--   0        0        0        0 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/server.py
+-rw-r--r--   0        0        0     1640 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/utils/__init__.py
+-rw-r--r--   0        0        0     2156 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/utils/logger.py
+-rw-r--r--   0        0        0     1311 2024-04-19 21:14:13.237436 ecjtu-0.1.1/ecjtu/utils/singleton.py
+-rw-r--r--   0        0        0     2869 2024-04-19 21:14:13.237436 ecjtu-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18028 1970-01-01 00:00:00.000000 ecjtu-0.1.1/PKG-INFO
```

### Comparing `ecjtu-0.1.0/LICENSE` & `ecjtu-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/README.md` & `ecjtu-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 </div>
 
 ## 📚 Introduction
 
 ecjtu 是一个用 Pythonic 的 ECJTU API SDK，旨在为开发者提供一个简洁、高效的方式来访问和管理其学籍资料、成绩、课表等信息，构建自己的应用程序 🌟。
 
-欢迎校友加入 EFC（ECJTU For Code），我们致力于构建一个充满活力的平台，集结校园内外对技术充满热情的开发者、技术爱好者以及创新思维者。在这里，您可以自由地分享您的编程知识，展示您的创新项目，以及与志同道合的人一起推动开源文化的发展。
+欢迎校友加入 EFC（ECJTU For Code），我们致力于构建一个充满活力的平台，集结校园内外对技术充满热情的开发者、技术爱好者。在这里，您可以自由地分享您的编程知识，展示您的创新项目，以及与志同道合的人一起推动开源文化的发展，make sth happen
 
 
 <div style="width: 250px;margin: 0 auto;">
     <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/ecjtu_group.png"/>
 </div>
```

### Comparing `ecjtu-0.1.0/ecjtu/__init__.py` & `ecjtu-0.1.1/ecjtu/__init__.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/client.py` & `ecjtu-0.1.1/ecjtu/client.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/constants.py` & `ecjtu-0.1.1/ecjtu/constants.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/crud.py` & `ecjtu-0.1.1/ecjtu/crud.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/models.py` & `ecjtu-0.1.1/ecjtu/models.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/utils/__init__.py` & `ecjtu-0.1.1/ecjtu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/utils/logger.py` & `ecjtu-0.1.1/ecjtu/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/ecjtu/utils/singleton.py` & `ecjtu-0.1.1/ecjtu/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.1.0/pyproject.toml` & `ecjtu-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ecjtu"
-version = "0.1.0"
+version = "0.1.1"
 description = "ECJTU API SDK service"
 readme = "README.md"
 authors = ["ecjtu <zeeland4work@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/Undertone0809/ecjtu"
 homepage = "https://github.com/Undertone0809/ecjtu"
 keywords = []
@@ -29,15 +29,14 @@
 "ecjtu" = "ecjtu.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 urllib3 = "1.26.18"
 pyopenssl = "24.1.0"
 beautifulsoup4 = "4.12.3"
-notebook = "^7.1.2"
 pydantic = "^2.6.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.3"
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
 ruff = "^0.1.6"
```

### Comparing `ecjtu-0.1.0/PKG-INFO` & `ecjtu-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecjtu
-Version: 0.1.0
+Version: 0.1.1
 Summary: ECJTU API SDK service
 Home-page: https://github.com/Undertone0809/ecjtu
 License: MIT
 Author: ecjtu
 Author-email: zeeland4work@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (==4.12.3)
-Requires-Dist: notebook (>=7.1.2,<8.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyopenssl (==24.1.0)
 Requires-Dist: urllib3 (==1.26.18)
 Project-URL: Repository, https://github.com/Undertone0809/ecjtu
 Description-Content-Type: text/markdown
 
 # ecjtu
@@ -44,15 +43,15 @@
 
 </div>
 
 ## 📚 Introduction
 
 ecjtu 是一个用 Pythonic 的 ECJTU API SDK，旨在为开发者提供一个简洁、高效的方式来访问和管理其学籍资料、成绩、课表等信息，构建自己的应用程序 🌟。
 
-欢迎校友加入 EFC（ECJTU For Code），我们致力于构建一个充满活力的平台，集结校园内外对技术充满热情的开发者、技术爱好者以及创新思维者。在这里，您可以自由地分享您的编程知识，展示您的创新项目，以及与志同道合的人一起推动开源文化的发展。
+欢迎校友加入 EFC（ECJTU For Code），我们致力于构建一个充满活力的平台，集结校园内外对技术充满热情的开发者、技术爱好者。在这里，您可以自由地分享您的编程知识，展示您的创新项目，以及与志同道合的人一起推动开源文化的发展，make sth happen
 
 
 <div style="width: 250px;margin: 0 auto;">
     <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/ecjtu_group.png"/>
 </div>
```

