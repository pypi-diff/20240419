# Comparing `tmp/logto-0.2.0.tar.gz` & `tmp/logto-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logto-0.2.0.tar", max compression
+gzip compressed data, was "logto-0.2.1.tar", last modified: Fri Apr 19 14:31:53 2024, max compression
```

## Comparing `logto-0.2.0.tar` & `logto-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1349 2023-11-26 10:16:31.443833 logto-0.2.0/README.md
--rw-r--r--   0        0        0    16879 2023-11-29 14:32:45.197255 logto-0.2.0/logto/LogtoClient.py
--rw-r--r--   0        0        0    15489 2023-11-29 14:32:45.197647 logto-0.2.0/logto/LogtoClient_test.py
--rw-r--r--   0        0        0      133 2023-08-09 15:40:18.595464 logto-0.2.0/logto/LogtoException.py
--rw-r--r--   0        0        0     6610 2023-11-29 14:32:45.198031 logto-0.2.0/logto/OidcCore.py
--rw-r--r--   0        0        0     7162 2023-11-26 10:16:31.445856 logto-0.2.0/logto/OidcCore_test.py
--rw-r--r--   0        0        0     2099 2023-08-09 15:40:18.596017 logto-0.2.0/logto/Storage.py
--rw-r--r--   0        0        0      618 2023-08-09 15:40:18.596218 logto-0.2.0/logto/__init__.py
--rw-r--r--   0        0        0     6794 2023-11-29 14:57:59.793116 logto-0.2.0/logto/models/oidc.py
--rw-r--r--   0        0        0     2307 2023-11-29 14:32:45.198547 logto-0.2.0/logto/models/response.py
--rw-r--r--   0        0        0      791 2023-11-29 14:32:45.198798 logto-0.2.0/logto/utilities/__init__.py
--rw-r--r--   0        0        0     1062 2023-08-08 09:45:36.572898 logto-0.2.0/logto/utilities/__init__test.py
--rw-r--r--   0        0        0     1279 2023-08-09 15:40:18.597013 logto-0.2.0/logto/utilities/test.py
--rw-r--r--   0        0        0     1633 2023-11-29 14:57:59.793418 logto-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 logto-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3987 2024-04-19 14:22:22.525121 logto-0.2.1/README.md
+-rw-r--r--   0        0        0    16879 2023-11-29 14:32:45.197255 logto-0.2.1/logto/LogtoClient.py
+-rw-r--r--   0        0        0    15489 2023-11-29 14:32:45.197647 logto-0.2.1/logto/LogtoClient_test.py
+-rw-r--r--   0        0        0      133 2023-08-09 15:40:18.595464 logto-0.2.1/logto/LogtoException.py
+-rw-r--r--   0        0        0     6738 2024-04-19 14:22:22.525533 logto-0.2.1/logto/OidcCore.py
+-rw-r--r--   0        0        0     7162 2023-11-26 10:16:31.445856 logto-0.2.1/logto/OidcCore_test.py
+-rw-r--r--   0        0        0     2099 2023-08-09 15:40:18.596017 logto-0.2.1/logto/Storage.py
+-rw-r--r--   0        0        0      618 2023-08-09 15:40:18.596218 logto-0.2.1/logto/__init__.py
+-rw-r--r--   0        0        0     8061 2024-04-19 06:44:33.694773 logto-0.2.1/logto/models/oidc.py
+-rw-r--r--   0        0        0     2307 2023-11-29 14:32:45.198547 logto-0.2.1/logto/models/response.py
+-rw-r--r--   0        0        0      791 2023-11-29 14:32:45.198798 logto-0.2.1/logto/utilities/__init__.py
+-rw-r--r--   0        0        0     1062 2023-08-08 09:45:36.572898 logto-0.2.1/logto/utilities/__init__test.py
+-rw-r--r--   0        0        0     1279 2023-08-09 15:40:18.597013 logto-0.2.1/logto/utilities/test.py
+-rw-r--r--   0        0        0     1691 2024-04-19 14:31:53.547433 logto-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4584 1970-01-01 00:00:00.000000 logto-0.2.1/PKG-INFO
```

### Comparing `logto-0.2.0/logto/LogtoClient.py` & `logto-0.2.1/logto/LogtoClient.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/LogtoClient_test.py` & `logto-0.2.1/logto/LogtoClient_test.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/OidcCore.py` & `logto-0.2.1/logto/OidcCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,24 @@
                 tokenEndpoint,
                 data=removeFalsyKeys(
                     {
                         "grant_type": "refresh_token",
                         "client_id": clientId,
                         "client_secret": clientSecret,
                         "refresh_token": refreshToken,
-                        "resource": resource
-                        if not resource.startswith(OrganizationUrnPrefix)
-                        else None,
-                        "organization_id": resource[len(OrganizationUrnPrefix) :]
-                        if resource.startswith(OrganizationUrnPrefix)
-                        else None,
+                        "resource": (
+                            resource
+                            if not resource.startswith(OrganizationUrnPrefix)
+                            else None
+                        ),
+                        "organization_id": (
+                            resource[len(OrganizationUrnPrefix) :]
+                            if resource.startswith(OrganizationUrnPrefix)
+                            else None
+                        ),
                     }
                 ),
             ) as resp:
                 if resp.status != 200:
                     raise LogtoException(await resp.text())
 
                 json = await resp.json()
```

### Comparing `logto-0.2.0/logto/OidcCore_test.py` & `logto-0.2.1/logto/OidcCore_test.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/Storage.py` & `logto-0.2.1/logto/Storage.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/__init__.py` & `logto-0.2.1/logto/__init__.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/models/oidc.py` & `logto-0.2.1/logto/models/oidc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import Enum
-from typing import List, Optional
+from typing import List, Optional, Any
 from pydantic import BaseModel, ConfigDict
+import warnings
 
 
 class OidcProviderMetadata(BaseModel):
     """
     The OpenID Connect Discovery response object.
 
     See https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderMetadata
@@ -48,15 +49,24 @@
     end_session_endpoint: Optional[str] = None
     code_challenge_methods_supported: List[str] = []
 
 
 class Scope(Enum):
     """The scope base class for determining the scope type."""
 
-    pass
+    def __new__(cls, value: Any):
+        member = object.__new__(cls)
+        member._value_ = value
+        return member
+
+    @classmethod
+    def _get_deprecated_member(cls, member):
+        # _get_deprecated_member is a protect util method to get the deprecated member with warning.
+        warnings.warn(f"{member.name} is deprecated.", DeprecationWarning, stacklevel=2)
+        return member
 
 
 class OAuthScope(Scope):
     offlineAccess = "offline_access"
 
 
 class UserInfoScope(Scope):
@@ -70,14 +80,23 @@
     """The scope for the basic profile. It maps to the `name`, `username`, `picture` claims."""
     email = "email"
     """The scope for the email address. It maps to the `email`, `email_verified` claims."""
     phone = "phone"
     """The scope for the phone number. It maps to the `phone_number`, `phone_number_verified` claims."""
     customData = "custom_data"
     """
+    DEPRECATED: use `custom_data` instead.
+
+    The scope for the custom data. It maps to the `custom_data` claim.
+
+    Note that the custom data is not included in the ID token by default. You need to
+    use `fetchUserInfo()` to get the custom data.
+    """
+    custom_data = "custom_data"
+    """
     The scope for the custom data. It maps to the `custom_data` claim.
 
     Note that the custom data is not included in the ID token by default. You need to
     use `fetchUserInfo()` to get the custom data.
     """
     identities = "identities"
     """
@@ -95,14 +114,26 @@
     organization_roles = "urn:logto:scope:organization_roles"
     """
     Scope for user's organization roles per [RFC 0001](https://github.com/logto-io/rfcs).
 
     To learn more about Logto Organizations, see https://docs.logto.io/docs/recipes/organizations/.
     """
 
+    @classmethod
+    def _missing_(cls, value):
+        """
+        `_missing_` is a [built-in method](https://docs.python.org/3/library/enum.html#supported-sunder-names) to handle
+        missing members, we overwrite it and throws a warning for deprecated members.
+
+        In this way, we can both warn the users, keep the type checking working and make the deprecated value backward compatible.
+        """
+        if value == cls.customData.value:
+            return cls._get_deprecated_member(cls.customData)
+        return super()._missing_(value)
+
 
 class IdTokenClaims(BaseModel):
     """
     The ID token claims object.
 
     To access the extra claims, use `__pydantic_extra__`. See
     https://docs.pydantic.dev/latest/usage/models/#extra-fields for more information.
```

### Comparing `logto-0.2.0/logto/models/response.py` & `logto-0.2.1/logto/models/response.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/utilities/__init__.py` & `logto-0.2.1/logto/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/utilities/__init__test.py` & `logto-0.2.1/logto/utilities/__init__test.py`

 * *Files identical despite different names*

### Comparing `logto-0.2.0/logto/utilities/test.py` & `logto-0.2.1/logto/utilities/test.py`

 * *Files identical despite different names*

