# Comparing `tmp/django-ipware-6.0.5.tar.gz` & `tmp/django-ipware-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipware-6.0.5.tar", last modified: Thu Apr 11 23:38:35 2024, max compression
+gzip compressed data, was "django-ipware-7.0.0.tar", last modified: Fri Apr 19 19:52:02 2024, max compression
```

## Comparing `django-ipware-6.0.5.tar` & `django-ipware-7.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-11 23:38:35.411474 django-ipware-6.0.5/
--rw-r--r--   0 val        (501) staff       (20)     1103 2023-10-02 23:45:14.000000 django-ipware-6.0.5/LICENSE
--rw-r--r--   0 val        (501) staff       (20)     9013 2024-04-11 23:38:35.411549 django-ipware-6.0.5/PKG-INFO
--rw-r--r--   0 val        (501) staff       (20)     8160 2024-04-11 23:36:17.000000 django-ipware-6.0.5/README.md
-drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-11 23:38:35.410925 django-ipware-6.0.5/django_ipware.egg-info/
--rw-r--r--   0 val        (501) staff       (20)     9013 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/PKG-INFO
--rw-r--r--   0 val        (501) staff       (20)      340 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/SOURCES.txt
--rw-r--r--   0 val        (501) staff       (20)        1 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/dependency_links.txt
--rw-r--r--   0 val        (501) staff       (20)        1 2023-11-23 00:20:32.000000 django-ipware-6.0.5/django_ipware.egg-info/not-zip-safe
--rw-r--r--   0 val        (501) staff       (20)       21 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/requires.txt
--rw-r--r--   0 val        (501) staff       (20)        7 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/top_level.txt
-drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-11 23:38:35.411375 django-ipware-6.0.5/ipware/
--rw-r--r--   0 val        (501) staff       (20)       87 2023-10-02 23:45:14.000000 django-ipware-6.0.5/ipware/__init__.py
--rw-r--r--   0 val        (501) staff       (20)      319 2024-04-11 23:36:17.000000 django-ipware-6.0.5/ipware/__version__.py
--rw-r--r--   0 val        (501) staff       (20)      250 2023-10-02 23:45:14.000000 django-ipware-6.0.5/ipware/apps.py
--rw-r--r--   0 val        (501) staff       (20)     1205 2024-02-04 19:26:02.000000 django-ipware-6.0.5/ipware/ip.py
--rw-r--r--   0 val        (501) staff       (20)      502 2023-11-23 00:20:01.000000 django-ipware-6.0.5/pyproject.toml
--rw-r--r--   0 val        (501) staff       (20)       73 2024-04-11 23:38:35.411854 django-ipware-6.0.5/setup.cfg
--rw-r--r--   0 val        (501) staff       (20)     2344 2024-04-11 23:36:17.000000 django-ipware-6.0.5/setup.py
+drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-19 19:52:02.211833 django-ipware-7.0.0/
+-rw-r--r--   0 val        (501) staff       (20)     1103 2023-10-02 23:45:14.000000 django-ipware-7.0.0/LICENSE
+-rw-r--r--   0 val        (501) staff       (20)     9013 2024-04-19 19:52:02.211922 django-ipware-7.0.0/PKG-INFO
+-rw-r--r--   0 val        (501) staff       (20)     8160 2024-04-11 23:36:17.000000 django-ipware-7.0.0/README.md
+drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-19 19:52:02.211059 django-ipware-7.0.0/django_ipware.egg-info/
+-rw-r--r--   0 val        (501) staff       (20)     9013 2024-04-19 19:52:02.000000 django-ipware-7.0.0/django_ipware.egg-info/PKG-INFO
+-rw-r--r--   0 val        (501) staff       (20)      340 2024-04-19 19:52:02.000000 django-ipware-7.0.0/django_ipware.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (501) staff       (20)        1 2024-04-19 19:52:02.000000 django-ipware-7.0.0/django_ipware.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (501) staff       (20)        1 2023-11-23 00:20:32.000000 django-ipware-7.0.0/django_ipware.egg-info/not-zip-safe
+-rw-r--r--   0 val        (501) staff       (20)       21 2024-04-19 19:52:02.000000 django-ipware-7.0.0/django_ipware.egg-info/requires.txt
+-rw-r--r--   0 val        (501) staff       (20)        7 2024-04-19 19:52:02.000000 django-ipware-7.0.0/django_ipware.egg-info/top_level.txt
+drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-19 19:52:02.211666 django-ipware-7.0.0/ipware/
+-rw-r--r--   0 val        (501) staff       (20)       87 2023-10-02 23:45:14.000000 django-ipware-7.0.0/ipware/__init__.py
+-rw-r--r--   0 val        (501) staff       (20)      319 2024-04-19 19:44:45.000000 django-ipware-7.0.0/ipware/__version__.py
+-rw-r--r--   0 val        (501) staff       (20)      250 2023-10-02 23:45:14.000000 django-ipware-7.0.0/ipware/apps.py
+-rw-r--r--   0 val        (501) staff       (20)     1026 2024-04-19 19:50:35.000000 django-ipware-7.0.0/ipware/ip.py
+-rw-r--r--   0 val        (501) staff       (20)      502 2023-11-23 00:20:01.000000 django-ipware-7.0.0/pyproject.toml
+-rw-r--r--   0 val        (501) staff       (20)       73 2024-04-19 19:52:02.212208 django-ipware-7.0.0/setup.cfg
+-rw-r--r--   0 val        (501) staff       (20)     2344 2024-04-11 23:36:17.000000 django-ipware-7.0.0/setup.py
```

### Comparing `django-ipware-6.0.5/LICENSE` & `django-ipware-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipware-6.0.5/PKG-INFO` & `django-ipware-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipware
-Version: 6.0.5
+Version: 7.0.0
 Summary: A Django application to retrieve user's IP address
 Home-page: https://github.com/un33k/django-ipware
 Author: Val Neekman
 Author-email: info@neekware.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `django-ipware-6.0.5/README.md` & `django-ipware-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-ipware-6.0.5/django_ipware.egg-info/PKG-INFO` & `django-ipware-7.0.0/django_ipware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipware
-Version: 6.0.5
+Version: 7.0.0
 Summary: A Django application to retrieve user's IP address
 Home-page: https://github.com/un33k/django-ipware
 Author: Val Neekman
 Author-email: info@neekware.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `django-ipware-6.0.5/ipware/ip.py` & `django-ipware-7.0.0/ipware/ip.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,23 +9,21 @@
     request: HttpRequest,
     proxy_order: Literal['left-most', 'right-most'] = 'left-most',
     proxy_count: Optional[int] = None,
     proxy_trusted_ips: Optional[Iterable[str]] = None,
     request_header_order: Optional[Iterable[str]] = None,
 ) -> Tuple[str, bool]:
     leftmost = proxy_order == 'left-most'
-    proxy_count = proxy_count if proxy_count is not None else getattr(settings, 'IPWARE_META_PROXY_COUNT', 0)
-    proxy_list = proxy_trusted_ips if proxy_trusted_ips is not None else []
     request_header_order = getattr(settings, 'IPWARE_META_PRECEDENCE_ORDER', request_header_order)
 
     # Instantiate IpWare with values from the function arguments
     ipw = IpWare(precedence=request_header_order,
                  leftmost=leftmost,
                  proxy_count=proxy_count,
-                 proxy_list=proxy_list)
+                 proxy_list=proxy_trusted_ips)
 
     ip, _ = ipw.get_client_ip(request.META, True)
 
     client_ip = None
     routable = False
 
     if ip:
```

### Comparing `django-ipware-6.0.5/setup.py` & `django-ipware-7.0.0/setup.py`

 * *Files identical despite different names*

