# Comparing `tmp/ft_jwt-0.0.9.tar.gz` & `tmp/ft_jwt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.9.tar", last modified: Thu Apr  4 15:40:23 2024, max compression
+gzip compressed data, was "dist/ft_jwt-0.1.0.tar", last modified: Fri Apr 19 11:40:25 2024, max compression
```

## Comparing `ft_jwt-0.0.9.tar` & `ft_jwt-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 14:17:44.000000 ft_jwt-0.0.9/LICENSE
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1853 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1286 2024-04-04 15:37:53.000000 ft_jwt-0.0.9/README.md
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:17:44.000000 ft_jwt-0.0.9/ft_jwt/__init__.py
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 14:17:44.000000 ft_jwt-0.0.9/ft_jwt/ft_jwt.py
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1853 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 15:40:22.000000 ft_jwt-0.0.9/setup.cfg
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      724 2024-04-04 15:40:17.000000 ft_jwt-0.0.9/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-15 07:40:53.000000 ft_jwt-0.1.0/ft_jwt/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3963 2024-04-18 16:42:29.000000 ft_jwt-0.1.0/ft_jwt/ft_jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/ft_jwt.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2697 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      174 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-19 11:40:24.000000 ft_jwt-0.1.0/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2697 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1585 2024-04-19 11:40:18.000000 ft_jwt-0.1.0/README.md
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-19 11:40:25.000000 ft_jwt-0.1.0/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      724 2024-04-19 11:38:14.000000 ft_jwt-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ft_jwt-0.0.9/setup.py` & `ft_jwt-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.9",
+	version="0.1.0",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/minthe/ft_transcendence/blob/main/auth/ft_jwt/ft_jwt/ft_jwt.py",
 	packages=setuptools.find_packages(),
```

