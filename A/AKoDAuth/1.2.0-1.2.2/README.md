# Comparing `tmp/AKoDAuth-1.2.0.tar.gz` & `tmp/AKoDAuth-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AKoDAuth-1.2.0.tar", last modified: Sun Apr 14 04:25:44 2024, max compression
+gzip compressed data, was "AKoDAuth-1.2.2.tar", last modified: Fri Apr 19 13:38:02 2024, max compression
```

## Comparing `AKoDAuth-1.2.0.tar` & `AKoDAuth-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 04:25:44.237631 AKoDAuth-1.2.0/
-drwxrwxrwx   0        0        0        0 2024-04-14 04:25:44.228035 AKoDAuth-1.2.0/AKoDAuth/
--rw-rw-rw-   0        0        0     2353 2024-04-14 04:24:59.000000 AKoDAuth-1.2.0/AKoDAuth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:25:44.235636 AKoDAuth-1.2.0/AKoDAuth.egg-info/
--rw-rw-rw-   0        0        0      227 2024-04-14 04:25:44.000000 AKoDAuth-1.2.0/AKoDAuth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-04-14 04:25:44.000000 AKoDAuth-1.2.0/AKoDAuth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 04:25:44.000000 AKoDAuth-1.2.0/AKoDAuth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-14 04:25:44.000000 AKoDAuth-1.2.0/AKoDAuth.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 04:25:44.000000 AKoDAuth-1.2.0/AKoDAuth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2024-03-23 17:29:31.000000 AKoDAuth-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-03-20 01:03:08.000000 AKoDAuth-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      227 2024-04-14 04:25:44.236634 AKoDAuth-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2024-03-25 04:45:00.000000 AKoDAuth-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 04:25:44.237631 AKoDAuth-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-04-14 04:25:26.000000 AKoDAuth-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:38:02.638342 AKoDAuth-1.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-19 13:38:02.628789 AKoDAuth-1.2.2/AKoDAuth/
+-rw-rw-rw-   0        0        0     3011 2024-04-19 13:36:44.000000 AKoDAuth-1.2.2/AKoDAuth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:38:02.635760 AKoDAuth-1.2.2/AKoDAuth.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-04-19 13:38:02.000000 AKoDAuth-1.2.2/AKoDAuth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-19 13:38:02.000000 AKoDAuth-1.2.2/AKoDAuth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:38:02.000000 AKoDAuth-1.2.2/AKoDAuth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-19 13:38:02.000000 AKoDAuth-1.2.2/AKoDAuth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 13:38:02.000000 AKoDAuth-1.2.2/AKoDAuth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2024-03-23 17:29:31.000000 AKoDAuth-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-03-20 01:03:08.000000 AKoDAuth-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      227 2024-04-19 13:38:02.637847 AKoDAuth-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-04-17 01:36:57.000000 AKoDAuth-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:38:02.638846 AKoDAuth-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      336 2024-04-19 13:33:06.000000 AKoDAuth-1.2.2/setup.py
```

### Comparing `AKoDAuth-1.2.0/AKoDAuth/__init__.py` & `AKoDAuth-1.2.2/AKoDAuth/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,32 +4,56 @@
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from cryptography.hazmat.primitives import hashes
 from cryptography.fernet import Fernet
 
 key = b''
 publickey = ''
 activationkey = ''
+
+
+customloco = 'none'
+svtype = 'default'
 def setActivationKey(string):
     global activationKey
     activationKey = string
-
 def privatekey(encrypted_key):
     global privkey
     privkey = bytes(encrypted_key, 'utf-8')
 def publicserverkey(link):
     global publickey
     identifier = b'3iDdjV4wARLuGZaPN9_E-hqHT0O8Ibiju293QLmCsgo='
     fernet = Fernet(identifier)
     link = fernet.decrypt(link.encode()).decode()
     if not bytes([array for array in [51, 105, 68, 100, 106, 86, 52, 119, 65, 82, 76, 117, 71, 90, 97, 80, 78, 57, 95, 69, 45, 104, 113, 72, 84, 48, 79, 56, 73, 98, 105, 106, 117, 50, 57, 51, 81, 76, 109, 67, 115, 103, 111, 61]]) == identifier: exit()
     publickey = link
+def service(value):
+    global svtype
+    if value == 'default':
+        svtype = 'default'
+    elif value == 'webdav':
+        svtype = 'webdav'
+    else:
+        svtype = 'default'
+def customWebDAVLocation(value):
+    if svtype == 'webdav':
+        global customloco
+        customloco = value
+    else:
+        return
 def isValid(login, password):
     global publickey, activationkey, privkey
-    url = publickey + login + '/check'
-    response = requests.get(url)
+    if svtype == 'default':
+        url = publickey + login + '/check'
+        response = requests.get(url)
+    elif svtype == 'webdav':
+        if customloco == 'none':
+            url = publickey + 'accs/' + login + '/check'
+        else:
+            url = publickey + customloco + '/' + login + '/check'
+        response = requests.post(url)
     if response.status_code == 404:
         return False
     try:
         encrypted_data = response.content
         iv = b'JMWUGHTG78TH78G1'
         final_encrypted_data = encrypted_data[len(iv):]
         password = password.encode()
```

### Comparing `AKoDAuth-1.2.0/LICENSE.txt` & `AKoDAuth-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

