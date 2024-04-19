# Comparing `tmp/mms_client-1.3.1.tar.gz` & `tmp/mms_client-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.3.1.tar", max compression
+gzip compressed data, was "mms_client-1.4.0.tar", max compression
```

## Comparing `mms_client-1.3.1.tar` & `mms_client-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1211 2024-04-16 05:21:13.995898 mms_client-1.3.1/LICENSE
--rw-r--r--   0        0        0    13490 2024-04-16 05:21:13.995898 mms_client-1.3.1/README.md
--rw-r--r--   0        0        0     2913 2024-04-16 05:21:13.999898 mms_client-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/__init__.py
--rw-r--r--   0        0        0      571 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    25839 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/base.py
--rw-r--r--   0        0        0     7574 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/market.py
--rw-r--r--   0        0        0      521 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3651 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      537 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0    14139 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/award.py
--rw-r--r--   0        0        0     9710 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/base.py
--rw-r--r--   0        0        0     1629 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    14785 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2706 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6791 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/registration.py
--rw-r--r--   0        0        0    65974 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4399 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-16 05:21:14.003898 mms_client-1.3.1/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    29534 2024-04-16 05:21:14.003898 mms_client-1.3.1/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0     9653 2024-04-16 05:21:14.003898 mms_client-1.3.1/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    14774 1970-01-01 00:00:00.000000 mms_client-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-19 03:46:14.952465 mms_client-1.4.0/LICENSE
+-rw-r--r--   0        0        0    14870 2024-04-19 03:46:14.952465 mms_client-1.4.0/README.md
+-rw-r--r--   0        0        0     2913 2024-04-19 03:46:14.956465 mms_client-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    26245 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     7574 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      521 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3651 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      537 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9710 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0    65974 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4399 2024-04-19 03:46:14.956465 mms_client-1.4.0/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:14.960465 mms_client-1.4.0/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     1693 2024-04-19 03:46:14.960465 mms_client-1.4.0/src/mms_client/utils/auditing.py
+-rw-r--r--   0        0        0     2306 2024-04-19 03:46:14.960465 mms_client-1.4.0/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    29534 2024-04-19 03:46:14.960465 mms_client-1.4.0/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0    10020 2024-04-19 03:46:14.960465 mms_client-1.4.0/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    16154 1970-01-01 00:00:00.000000 mms_client-1.4.0/PKG-INFO
```

### Comparing `mms_client-1.3.1/LICENSE` & `mms_client-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/README.md` & `mms_client-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -157,14 +157,35 @@
 
 ```python
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, logger=my_logger)
 ```
 
 The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
 
+## Auditing XML Requests & Responses
+A common requirement for this sort of library is recording or saving the raw XML requests and responses for audit/logging purposes. This library supports this workflow through the `mms_client.utils.auditing.AuditPlugin` object. This object intercepts the XML request at the Zeep client level right before it is sent to the MMS and, similarly, intercepts the XML response immediately after it is received from the MMS. Before passing these objects on, without modifying them, it records the XML data as a byte string and passes it to two methods: `audit_request` and `audit_response`. These can be overridden by any object that inherits from this class, allowing the user to direct this data to whatever store they prefer to use for auditing or logging.
+
+```python
+class TestAuditPlugin(AuditPlugin):
+
+    def __init__(self):
+        self.request = None
+        self.response = None
+
+    def audit_request(self, mms_request: bytes) -> None:
+        self.request = mms_request
+
+    def audit_response(self, mms_response: bytes) -> None:
+        self.response = mms_response
+
+client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
+```
+
+This same input allows for the user to create their own plugins and add them to the Zeep client, allowing for a certain amount of extensibility.
+
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
 - MarketQuery_AwardResultsQuery
 - RegistrationSubmit_Resource
```

### Comparing `mms_client-1.3.1/pyproject.toml` & `mms_client-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.3.1"
+version = "v1.4.0"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mms_client-1.3.1/src/mms_client/client.py` & `mms_client-1.4.0/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.4.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.4.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.4.0/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.4.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.4.0/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.4.0/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.4.0/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/security/certs.py` & `mms_client-1.4.0/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/security/crypto.py` & `mms_client-1.4.0/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/services/base.py` & `mms_client-1.4.0/src/mms_client/services/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from mms_client.types.transport import ResponseDataType
 from mms_client.utils.errors import AudienceError
 from mms_client.utils.errors import MMSClientError
 from mms_client.utils.errors import MMSValidationError
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import ClientType
 from mms_client.utils.web import Interface
+from mms_client.utils.web import Plugin
 from mms_client.utils.web import ZWrapper
 
 # Set the default logger for the MMS client
 default_logger = getLogger("MMS Client")
 
 
 @dataclass
@@ -249,26 +250,29 @@
     def __init__(
         self,
         participant: str,
         user: str,
         client_type: ClientType,
         cert: Certificate,
         logger: Optional[Logger] = None,
+        plugins: Optional[List[Plugin]] = None,
         is_admin: bool = False,
         test: bool = False,
     ):
         """Create a new MMS client with the given participant, user, client type, and authentication.
 
         Arguments:
         participant (str):          The MMS code of the business entity to which the requesting user belongs.
         user (str):                 The user name of the person making the request.
         client_type (ClientType):   The type of client to use for making requests to the MMS server.
         cert (Certificate):         The certificate to use for signing requests.
         logger (Logger):            The logger to use for instrumentation. If this is not provided, then the default
                                     logger will be used.
+        plugins (List[Plugin]):     A list of plugins to add to the Zeep client. This can be useful for auditing or
+                                    other purposes.
         is_admin (bool):            Whether the user is an admin (i.e. is a market operator).
         test (bool):                Whether to use the test server.
         """
         # First, save the base field associated with the client
         self._participant = participant
         self._user = user
         self._client_type = client_type
@@ -277,14 +281,15 @@
 
         # Next, save the security-related fields associated with the client
         self._cert = cert
         self._signer = CryptoWrapper(cert)
 
         # Now, set our logger to either the provided logger or the default logger
         self._logger = logger or default_logger
+        self._plugins = plugins or []
 
         # Finally, create a list of wrappers for the different interfaces
         self._wrappers: Dict[Interface, ZWrapper] = {}
 
     @property
     def participant(self) -> str:
         """Return the MMS code of the business entity to which the requesting user belongs."""
@@ -594,10 +599,16 @@
 
         Arguments:
         service (ServiceConfiguration):  The service for which to get the wrapper.
         """
         if service.interface not in self._wrappers:
             self._logger.debug(f"Creating wrapper for {service.interface.name} interface.")
             self._wrappers[service.interface] = ZWrapper(
-                self._client_type, service.interface, self._cert.to_adapter(), self._logger, True, self._test
+                self._client_type,
+                service.interface,
+                self._cert.to_adapter(),
+                self._logger,
+                self._plugins,
+                True,
+                self._test,
             )
         return self._wrappers[service.interface]
```

### Comparing `mms_client-1.3.1/src/mms_client/services/market.py` & `mms_client-1.4.0/src/mms_client/services/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/services/omi.py` & `mms_client-1.4.0/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/services/registration.py` & `mms_client-1.4.0/src/mms_client/services/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/services/report.py` & `mms_client-1.4.0/src/mms_client/services/report.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/award.py` & `mms_client-1.4.0/src/mms_client/types/award.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/base.py` & `mms_client-1.4.0/src/mms_client/types/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/enums.py` & `mms_client-1.4.0/src/mms_client/types/enums.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/fields.py` & `mms_client-1.4.0/src/mms_client/types/fields.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/market.py` & `mms_client-1.4.0/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/offer.py` & `mms_client-1.4.0/src/mms_client/types/offer.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/registration.py` & `mms_client-1.4.0/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/resource.py` & `mms_client-1.4.0/src/mms_client/types/resource.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/types/transport.py` & `mms_client-1.4.0/src/mms_client/types/transport.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/utils/errors.py` & `mms_client-1.4.0/src/mms_client/utils/errors.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/utils/serialization.py` & `mms_client-1.4.0/src/mms_client/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.1/src/mms_client/utils/web.py` & `mms_client-1.4.0/src/mms_client/utils/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Contains the HTTP/web layer for communicating with the MMS server."""
 
 from enum import Enum
 from logging import Logger
 from pathlib import Path
+from typing import List
+from typing import Optional
 
 from backoff import expo
 from backoff import on_exception
 from requests import Session
 from requests_pkcs12 import Pkcs12Adapter
 from zeep import Client
+from zeep import Plugin
 from zeep import Transport
 from zeep.cache import SqliteCache
 from zeep.exceptions import TransportError
 from zeep.xsd.valueobjects import CompoundValue
 
 from mms_client.types.transport import MmsRequest
 from mms_client.types.transport import MmsResponse
@@ -128,14 +131,15 @@
 
     def __init__(
         self,
         client: ClientType,
         interface: Interface,
         adapter: Pkcs12Adapter,
         logger: Logger,
+        plugins: Optional[List[Plugin]] = None,
         cache: bool = True,
         test: bool = False,
     ):
         """Create a new Zeep wrapper object for a specific MMS service endpoint.
 
         Arguments:
         client (ClientType):        The type of client to use. This can be either "bsp" (Balancing Service Provider) or
@@ -143,14 +147,16 @@
                                     use.
         interface (Interface):      The type of interface to use. This can be either "omi" (Other Market Initiator) or
                                     "mi" (Market Initiator). This will determine which service endpoint to use as well
                                     as the service and port to use.
         adapter (Pkcs12Adapter):    The PKCS12 adapter containing the certificate and private key to use for
                                     authenticating with the MMS server.
         logger (Logger):            The logger to use for instrumentation.
+        plugins (List[Plugin]):     A list of Zeep plugins to use with the client. This is useful for adding additional
+                                    functionality to the client, such as auditing or logging.
         cache (bool):               If True, use a cache for the Zeep client. This is useful for avoiding repeated
                                     lookups of the WSDL file, which should result in lower latency.
         test (bool):                If True, use the test service endpoint. This is useful for testing the client.
         """
         # First, we'll check that the client is valid. If it's not, we'll raise a ValueError.
         if client not in URLS:
             raise ValueError(f"Invalid client, '{client}'. Only 'bsp' and 'tso' are supported.")
@@ -180,14 +186,15 @@
 
         # Finally, we create the Zeep client with the given WSDL file location, session, and cache settings and then,
         # from that client, we create the SOAP service with the given service binding and selected endpoint.
         self._logger = logger
         self._client = Client(
             wsdl=str(location.resolve()),
             transport=Transport(cache=SqliteCache() if cache else None, session=sess),
+            plugins=plugins,
         )
         self._create_service()
 
     @on_exception(expo, TransportError, max_tries=3, giveup=fatal_code)  # type: ignore[arg-type]
     def submit(self, req: MmsRequest) -> MmsResponse:
         """Submit the given request to the MMS server and return the response."""
         try:
```

### Comparing `mms_client-1.3.1/PKG-INFO` & `mms_client-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.3.1
+Version: 1.4.0
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -189,14 +189,35 @@
 
 ```python
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, logger=my_logger)
 ```
 
 The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
 
+## Auditing XML Requests & Responses
+A common requirement for this sort of library is recording or saving the raw XML requests and responses for audit/logging purposes. This library supports this workflow through the `mms_client.utils.auditing.AuditPlugin` object. This object intercepts the XML request at the Zeep client level right before it is sent to the MMS and, similarly, intercepts the XML response immediately after it is received from the MMS. Before passing these objects on, without modifying them, it records the XML data as a byte string and passes it to two methods: `audit_request` and `audit_response`. These can be overridden by any object that inherits from this class, allowing the user to direct this data to whatever store they prefer to use for auditing or logging.
+
+```python
+class TestAuditPlugin(AuditPlugin):
+
+    def __init__(self):
+        self.request = None
+        self.response = None
+
+    def audit_request(self, mms_request: bytes) -> None:
+        self.request = mms_request
+
+    def audit_response(self, mms_response: bytes) -> None:
+        self.response = mms_response
+
+client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
+```
+
+This same input allows for the user to create their own plugins and add them to the Zeep client, allowing for a certain amount of extensibility.
+
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
 - MarketQuery_AwardResultsQuery
 - RegistrationSubmit_Resource
```

