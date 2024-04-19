# Comparing `tmp/antchain_stlr-2.6.0.tar.gz` & `tmp/antchain_stlr-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.6.0.tar", last modified: Wed Jun 21 09:35:35 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.7.4.tar", last modified: Fri Apr 19 06:58:10 2024, max compression
```

## Comparing `antchain_stlr-2.6.0.tar` & `antchain_stlr-2.7.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)   113763 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   266168 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-21 09:35:35.000000 antchain_stlr-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127505 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   307516 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/setup.py
```

### Comparing `antchain_stlr-2.6.0/LICENSE` & `antchain_stlr-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.6.0/PKG-INFO` & `antchain_stlr-2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.6.0
+Version: 2.7.4
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.6.0/README-CN.md` & `antchain_stlr-2.7.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.6.0/README.md` & `antchain_stlr-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.6.0/antchain_sdk_stlr/client.py` & `antchain_stlr-2.7.4/antchain_sdk_stlr/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.6.0',
+                    'sdk_version': '2.7.4',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.6.0',
+                    'sdk_version': '2.7.4',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -2601,14 +2601,328 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.SubmitEcarLcaassementResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.lcaassement.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def upload_ecar_plaformfile(
+        self,
+        request: stlr_models.UploadEcarPlaformfileRequest,
+    ) -> stlr_models.UploadEcarPlaformfileResponse:
+        """
+        Description: 三方平台文件上传
+        Summary: 三方平台文件上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_ecar_plaformfile_ex(request, headers, runtime)
+
+    async def upload_ecar_plaformfile_async(
+        self,
+        request: stlr_models.UploadEcarPlaformfileRequest,
+    ) -> stlr_models.UploadEcarPlaformfileResponse:
+        """
+        Description: 三方平台文件上传
+        Summary: 三方平台文件上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_ecar_plaformfile_ex_async(request, headers, runtime)
+
+    def upload_ecar_plaformfile_ex(
+        self,
+        request: stlr_models.UploadEcarPlaformfileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.UploadEcarPlaformfileResponse:
+        """
+        Description: 三方平台文件上传
+        Summary: 三方平台文件上传
+        """
+        if not UtilClient.is_unset(request.file_object):
+            upload_req = stlr_models.CreateAntcloudGatewayxFileUploadRequest(
+                auth_token=request.auth_token,
+                api_code='antchain.carbon.ecar.plaformfile.upload',
+                file_name=request.file_object_name
+            )
+            upload_resp = self.create_antcloud_gatewayx_file_upload_ex(upload_req, headers, runtime)
+            if not AntchainUtils.is_success(upload_resp.result_code, 'ok'):
+                upload_ecar_plaformfile_response = stlr_models.UploadEcarPlaformfileResponse(
+                    req_msg_id=upload_resp.req_msg_id,
+                    result_code=upload_resp.result_code,
+                    result_msg=upload_resp.result_msg
+                )
+                return upload_ecar_plaformfile_response
+            upload_headers = AntchainUtils.parse_upload_headers(upload_resp.upload_headers)
+            AntchainUtils.put_object(request.file_object, upload_headers, upload_resp.upload_url)
+            request.file_id = upload_resp.file_id
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.UploadEcarPlaformfileResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.plaformfile.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_ecar_plaformfile_ex_async(
+        self,
+        request: stlr_models.UploadEcarPlaformfileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.UploadEcarPlaformfileResponse:
+        """
+        Description: 三方平台文件上传
+        Summary: 三方平台文件上传
+        """
+        if not UtilClient.is_unset(request.file_object):
+            upload_req = stlr_models.CreateAntcloudGatewayxFileUploadRequest(
+                auth_token=request.auth_token,
+                api_code='antchain.carbon.ecar.plaformfile.upload',
+                file_name=request.file_object_name
+            )
+            upload_resp = await self.create_antcloud_gatewayx_file_upload_ex_async(upload_req, headers, runtime)
+            if not AntchainUtils.is_success(upload_resp.result_code, 'ok'):
+                upload_ecar_plaformfile_response = stlr_models.UploadEcarPlaformfileResponse(
+                    req_msg_id=upload_resp.req_msg_id,
+                    result_code=upload_resp.result_code,
+                    result_msg=upload_resp.result_msg
+                )
+                return upload_ecar_plaformfile_response
+            upload_headers = AntchainUtils.parse_upload_headers(upload_resp.upload_headers)
+            await AntchainUtils.put_object_async(request.file_object, upload_headers, upload_resp.upload_url)
+            request.file_id = upload_resp.file_id
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.UploadEcarPlaformfileResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.plaformfile.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_ecar_lcaorderwithcustomer(
+        self,
+        request: stlr_models.SubmitEcarLcaorderwithcustomerRequest,
+    ) -> stlr_models.SubmitEcarLcaorderwithcustomerResponse:
+        """
+        Description: 三方平台提交LCA订单，同时包括客户入驻信息
+        Summary: LCA订单提交(含客户入驻信息)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_ecar_lcaorderwithcustomer_ex(request, headers, runtime)
+
+    async def submit_ecar_lcaorderwithcustomer_async(
+        self,
+        request: stlr_models.SubmitEcarLcaorderwithcustomerRequest,
+    ) -> stlr_models.SubmitEcarLcaorderwithcustomerResponse:
+        """
+        Description: 三方平台提交LCA订单，同时包括客户入驻信息
+        Summary: LCA订单提交(含客户入驻信息)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_ecar_lcaorderwithcustomer_ex_async(request, headers, runtime)
+
+    def submit_ecar_lcaorderwithcustomer_ex(
+        self,
+        request: stlr_models.SubmitEcarLcaorderwithcustomerRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.SubmitEcarLcaorderwithcustomerResponse:
+        """
+        Description: 三方平台提交LCA订单，同时包括客户入驻信息
+        Summary: LCA订单提交(含客户入驻信息)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.SubmitEcarLcaorderwithcustomerResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.lcaorderwithcustomer.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_ecar_lcaorderwithcustomer_ex_async(
+        self,
+        request: stlr_models.SubmitEcarLcaorderwithcustomerRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.SubmitEcarLcaorderwithcustomerResponse:
+        """
+        Description: 三方平台提交LCA订单，同时包括客户入驻信息
+        Summary: LCA订单提交(含客户入驻信息)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.SubmitEcarLcaorderwithcustomerResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.lcaorderwithcustomer.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_ecar_plaformauthtoken(
+        self,
+        request: stlr_models.GetEcarPlaformauthtokenRequest,
+    ) -> stlr_models.GetEcarPlaformauthtokenResponse:
+        """
+        Description: 三方平台信登token获取
+        Summary: 三方平台获取信登token
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_ecar_plaformauthtoken_ex(request, headers, runtime)
+
+    async def get_ecar_plaformauthtoken_async(
+        self,
+        request: stlr_models.GetEcarPlaformauthtokenRequest,
+    ) -> stlr_models.GetEcarPlaformauthtokenResponse:
+        """
+        Description: 三方平台信登token获取
+        Summary: 三方平台获取信登token
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_ecar_plaformauthtoken_ex_async(request, headers, runtime)
+
+    def get_ecar_plaformauthtoken_ex(
+        self,
+        request: stlr_models.GetEcarPlaformauthtokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.GetEcarPlaformauthtokenResponse:
+        """
+        Description: 三方平台信登token获取
+        Summary: 三方平台获取信登token
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.GetEcarPlaformauthtokenResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.plaformauthtoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_ecar_plaformauthtoken_ex_async(
+        self,
+        request: stlr_models.GetEcarPlaformauthtokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.GetEcarPlaformauthtokenResponse:
+        """
+        Description: 三方平台信登token获取
+        Summary: 三方平台获取信登token
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.GetEcarPlaformauthtokenResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.plaformauthtoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_ecar_lcaorder(
+        self,
+        request: stlr_models.QueryEcarLcaorderRequest,
+    ) -> stlr_models.QueryEcarLcaorderResponse:
+        """
+        Description: LCA订单查询
+        Summary: LCA订单查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_ecar_lcaorder_ex(request, headers, runtime)
+
+    async def query_ecar_lcaorder_async(
+        self,
+        request: stlr_models.QueryEcarLcaorderRequest,
+    ) -> stlr_models.QueryEcarLcaorderResponse:
+        """
+        Description: LCA订单查询
+        Summary: LCA订单查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_ecar_lcaorder_ex_async(request, headers, runtime)
+
+    def query_ecar_lcaorder_ex(
+        self,
+        request: stlr_models.QueryEcarLcaorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryEcarLcaorderResponse:
+        """
+        Description: LCA订单查询
+        Summary: LCA订单查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryEcarLcaorderResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.lcaorder.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_ecar_lcaorder_ex_async(
+        self,
+        request: stlr_models.QueryEcarLcaorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryEcarLcaorderResponse:
+        """
+        Description: LCA订单查询
+        Summary: LCA订单查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryEcarLcaorderResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.lcaorder.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def batchcreate_ecar_greencertificategeneration(
+        self,
+        request: stlr_models.BatchcreateEcarGreencertificategenerationRequest,
+    ) -> stlr_models.BatchcreateEcarGreencertificategenerationResponse:
+        """
+        Description: 绿证发电量数据上报接口
+        Summary: 绿证发电量数据上报接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.batchcreate_ecar_greencertificategeneration_ex(request, headers, runtime)
+
+    async def batchcreate_ecar_greencertificategeneration_async(
+        self,
+        request: stlr_models.BatchcreateEcarGreencertificategenerationRequest,
+    ) -> stlr_models.BatchcreateEcarGreencertificategenerationResponse:
+        """
+        Description: 绿证发电量数据上报接口
+        Summary: 绿证发电量数据上报接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.batchcreate_ecar_greencertificategeneration_ex_async(request, headers, runtime)
+
+    def batchcreate_ecar_greencertificategeneration_ex(
+        self,
+        request: stlr_models.BatchcreateEcarGreencertificategenerationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.BatchcreateEcarGreencertificategenerationResponse:
+        """
+        Description: 绿证发电量数据上报接口
+        Summary: 绿证发电量数据上报接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.BatchcreateEcarGreencertificategenerationResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.greencertificategeneration.batchcreate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def batchcreate_ecar_greencertificategeneration_ex_async(
+        self,
+        request: stlr_models.BatchcreateEcarGreencertificategenerationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.BatchcreateEcarGreencertificategenerationResponse:
+        """
+        Description: 绿证发电量数据上报接口
+        Summary: 绿证发电量数据上报接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.BatchcreateEcarGreencertificategenerationResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.greencertificategeneration.batchcreate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.6.0/antchain_sdk_stlr/models.py` & `antchain_stlr-2.7.4/antchain_sdk_stlr/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,14 +186,139 @@
         if m.get('item_code') is not None:
             self.item_code = m.get('item_code')
         if m.get('item_amount') is not None:
             self.item_amount = m.get('item_amount')
         return self
 
 
+class InverterGeneration(TeaModel):
+    def __init__(
+        self,
+        inv_sn: str = None,
+        manufacturer: str = None,
+        daily: str = None,
+        total: str = None,
+    ):
+        # 逆变器SN
+        self.inv_sn = inv_sn
+        # 生产商名称
+        self.manufacturer = manufacturer
+        # 当日发电量，最多3位小数
+        self.daily = daily
+        # 累计发电量，最多3位小数
+        self.total = total
+
+    def validate(self):
+        self.validate_required(self.inv_sn, 'inv_sn')
+        self.validate_required(self.manufacturer, 'manufacturer')
+        self.validate_required(self.daily, 'daily')
+        self.validate_required(self.total, 'total')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.inv_sn is not None:
+            result['inv_sn'] = self.inv_sn
+        if self.manufacturer is not None:
+            result['manufacturer'] = self.manufacturer
+        if self.daily is not None:
+            result['daily'] = self.daily
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('inv_sn') is not None:
+            self.inv_sn = m.get('inv_sn')
+        if m.get('manufacturer') is not None:
+            self.manufacturer = m.get('manufacturer')
+        if m.get('daily') is not None:
+            self.daily = m.get('daily')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
+class LcaStageCarbonItem(TeaModel):
+    def __init__(
+        self,
+        lca_stage_code: str = None,
+        lca_stage_carbon_amount: str = None,
+    ):
+        # 生命周期阶段：
+        # [MaterialPurchase]-原材料，[ProductManufacture]-生产制造，[ProductSale]-分销，[ProductUsage]-产品使用，[ProductWithdraw]-处置/再生利用
+        self.lca_stage_code = lca_stage_code
+        # 阶段碳排放量
+        self.lca_stage_carbon_amount = lca_stage_carbon_amount
+
+    def validate(self):
+        self.validate_required(self.lca_stage_code, 'lca_stage_code')
+        self.validate_required(self.lca_stage_carbon_amount, 'lca_stage_carbon_amount')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.lca_stage_code is not None:
+            result['lca_stage_code'] = self.lca_stage_code
+        if self.lca_stage_carbon_amount is not None:
+            result['lca_stage_carbon_amount'] = self.lca_stage_carbon_amount
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('lca_stage_code') is not None:
+            self.lca_stage_code = m.get('lca_stage_code')
+        if m.get('lca_stage_carbon_amount') is not None:
+            self.lca_stage_carbon_amount = m.get('lca_stage_carbon_amount')
+        return self
+
+
+class EnterpriseDocumentFile(TeaModel):
+    def __init__(
+        self,
+        document_name: str = None,
+        document_address: str = None,
+    ):
+        # 文档名称
+        self.document_name = document_name
+        # 文件地址
+        self.document_address = document_address
+
+    def validate(self):
+        self.validate_required(self.document_name, 'document_name')
+        self.validate_required(self.document_address, 'document_address')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.document_name is not None:
+            result['document_name'] = self.document_name
+        if self.document_address is not None:
+            result['document_address'] = self.document_address
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('document_name') is not None:
+            self.document_name = m.get('document_name')
+        if m.get('document_address') is not None:
+            self.document_address = m.get('document_address')
+        return self
+
+
 class CertProductAuthDO(TeaModel):
     def __init__(
         self,
         product_id: str = None,
         product_name: str = None,
     ):
         # 三方平台产品ID
@@ -661,170 +786,56 @@
         if m.get('counteraction_amount') is not None:
             self.counteraction_amount = m.get('counteraction_amount')
         if m.get('data_unit') is not None:
             self.data_unit = m.get('data_unit')
         return self
 
 
-class CarbonOffsetActiveDataDetail(TeaModel):
+class DeviceGeneration(TeaModel):
     def __init__(
         self,
-        active_data_no: str = None,
-        active_data_name: str = None,
-        active_data_unit: str = None,
-        description: str = None,
-        active_data_value: str = None,
+        device_no: str = None,
+        inverter_generations: List[InverterGeneration] = None,
     ):
-        # 活动数据编号
-        self.active_data_no = active_data_no
-        # 活动数据名称
-        self.active_data_name = active_data_name
-        # 活动数据单位
-        self.active_data_unit = active_data_unit
-        # 活动数据描述文案
-        self.description = description
-        # 活动数据值
-        self.active_data_value = active_data_value
+        # 设备内部编号，注册设备后获取
+        self.device_no = device_no
+        # 逆变器发电量列表
+        self.inverter_generations = inverter_generations
 
     def validate(self):
-        self.validate_required(self.active_data_no, 'active_data_no')
-        self.validate_required(self.active_data_value, 'active_data_value')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.active_data_no is not None:
-            result['active_data_no'] = self.active_data_no
-        if self.active_data_name is not None:
-            result['active_data_name'] = self.active_data_name
-        if self.active_data_unit is not None:
-            result['active_data_unit'] = self.active_data_unit
-        if self.description is not None:
-            result['description'] = self.description
-        if self.active_data_value is not None:
-            result['active_data_value'] = self.active_data_value
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('active_data_no') is not None:
-            self.active_data_no = m.get('active_data_no')
-        if m.get('active_data_name') is not None:
-            self.active_data_name = m.get('active_data_name')
-        if m.get('active_data_unit') is not None:
-            self.active_data_unit = m.get('active_data_unit')
-        if m.get('description') is not None:
-            self.description = m.get('description')
-        if m.get('active_data_value') is not None:
-            self.active_data_value = m.get('active_data_value')
-        return self
-
-
-class EnterpriseMemberSummary(TeaModel):
-    def __init__(
-        self,
-        account_did: str = None,
-        name: str = None,
-        mobile: str = None,
-        register_time: str = None,
-    ):
-        # 机构会员DID
-        self.account_did = account_did
-        # 会员姓名，数据脱敏处理返回
-        self.name = name
-        # 会员手机号码，数据脱敏处理返回
-        self.mobile = mobile
-        # 会员注册时间
-        self.register_time = register_time
-
-    def validate(self):
-        self.validate_required(self.account_did, 'account_did')
-        self.validate_required(self.register_time, 'register_time')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.account_did is not None:
-            result['account_did'] = self.account_did
-        if self.name is not None:
-            result['name'] = self.name
-        if self.mobile is not None:
-            result['mobile'] = self.mobile
-        if self.register_time is not None:
-            result['register_time'] = self.register_time
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('account_did') is not None:
-            self.account_did = m.get('account_did')
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('mobile') is not None:
-            self.mobile = m.get('mobile')
-        if m.get('register_time') is not None:
-            self.register_time = m.get('register_time')
-        return self
-
-
-class AnyStatisticalItem(TeaModel):
-    def __init__(
-        self,
-        item_code: str = None,
-        amount: str = None,
-        unit: str = None,
-        unit_label: str = None,
-    ):
-        # 统计项目编码
-        self.item_code = item_code
-        # 数据值，按字符串输出，最多保留6位小数
-        self.amount = amount
-        # 单位编码
-        self.unit = unit
-        # 单位标签
-        self.unit_label = unit_label
-
-    def validate(self):
-        self.validate_required(self.item_code, 'item_code')
-        self.validate_required(self.amount, 'amount')
-        self.validate_required(self.unit, 'unit')
-        self.validate_required(self.unit_label, 'unit_label')
+        self.validate_required(self.device_no, 'device_no')
+        self.validate_required(self.inverter_generations, 'inverter_generations')
+        if self.inverter_generations:
+            for k in self.inverter_generations:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.item_code is not None:
-            result['item_code'] = self.item_code
-        if self.amount is not None:
-            result['amount'] = self.amount
-        if self.unit is not None:
-            result['unit'] = self.unit
-        if self.unit_label is not None:
-            result['unit_label'] = self.unit_label
+        if self.device_no is not None:
+            result['device_no'] = self.device_no
+        result['inverter_generations'] = []
+        if self.inverter_generations is not None:
+            for k in self.inverter_generations:
+                result['inverter_generations'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('item_code') is not None:
-            self.item_code = m.get('item_code')
-        if m.get('amount') is not None:
-            self.amount = m.get('amount')
-        if m.get('unit') is not None:
-            self.unit = m.get('unit')
-        if m.get('unit_label') is not None:
-            self.unit_label = m.get('unit_label')
+        if m.get('device_no') is not None:
+            self.device_no = m.get('device_no')
+        self.inverter_generations = []
+        if m.get('inverter_generations') is not None:
+            for k in m.get('inverter_generations'):
+                temp_model = InverterGeneration()
+                self.inverter_generations.append(temp_model.from_map(k))
         return self
 
 
 class CarbonAccountInfo(TeaModel):
     def __init__(
         self,
         user_did: str = None,
@@ -884,86 +895,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('user_did') is not None:
             self.user_did = m.get('user_did')
         return self
 
 
-class EnterpriseDocumentFile(TeaModel):
-    def __init__(
-        self,
-        document_name: str = None,
-        document_address: str = None,
-    ):
-        # 文档名称
-        self.document_name = document_name
-        # 文件地址
-        self.document_address = document_address
-
-    def validate(self):
-        self.validate_required(self.document_name, 'document_name')
-        self.validate_required(self.document_address, 'document_address')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.document_name is not None:
-            result['document_name'] = self.document_name
-        if self.document_address is not None:
-            result['document_address'] = self.document_address
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('document_name') is not None:
-            self.document_name = m.get('document_name')
-        if m.get('document_address') is not None:
-            self.document_address = m.get('document_address')
-        return self
-
-
-class BlockchainDTO(TeaModel):
-    def __init__(
-        self,
-        tx_hash: str = None,
-        block_number: int = None,
-    ):
-        # 交易hash
-        self.tx_hash = tx_hash
-        # 当前块高
-        self.block_number = block_number
-
-    def validate(self):
-        self.validate_required(self.tx_hash, 'tx_hash')
-        self.validate_required(self.block_number, 'block_number')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.tx_hash is not None:
-            result['tx_hash'] = self.tx_hash
-        if self.block_number is not None:
-            result['block_number'] = self.block_number
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('tx_hash') is not None:
-            self.tx_hash = m.get('tx_hash')
-        if m.get('block_number') is not None:
-            self.block_number = m.get('block_number')
-        return self
-
-
 class CarbonOffsetAcquisitionItem(TeaModel):
     def __init__(
         self,
         acquisition_item_no: str = None,
         project_no: str = None,
         account_did: str = None,
         occurrent_time: str = None,
@@ -1238,80 +1177,78 @@
         if m.get('authentication_deetail') is not None:
             self.authentication_deetail = m.get('authentication_deetail')
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
-class EmissionsScopeStatistics(TeaModel):
+class PlatformCustomerSummary(TeaModel):
     def __init__(
         self,
-        inventory_scope_no: str = None,
-        inventory_scope_name: str = None,
-        emissions: int = None,
-        percentage: int = None,
-        category_emissions_list: List[EmissionsCategoryStatistics] = None,
-    ):
-        # 盘查范围编码
-        self.inventory_scope_no = inventory_scope_no
-        # 盘查范围名称
-        self.inventory_scope_name = inventory_scope_name
-        # 碳排放量
-        self.emissions = emissions
-        # 排放占比
-        self.percentage = percentage
-        # 范围下各分类排放数据
-        self.category_emissions_list = category_emissions_list
-
-    def validate(self):
-        self.validate_required(self.inventory_scope_no, 'inventory_scope_no')
-        self.validate_required(self.inventory_scope_name, 'inventory_scope_name')
-        self.validate_required(self.emissions, 'emissions')
-        self.validate_required(self.percentage, 'percentage')
-        self.validate_required(self.category_emissions_list, 'category_emissions_list')
-        if self.category_emissions_list:
-            for k in self.category_emissions_list:
-                if k:
-                    k.validate()
+        customer_id: str = None,
+        customer_name: str = None,
+        contact_person: str = None,
+        contact_telephone: str = None,
+        contact_email: str = None,
+        social_credit_code: str = None,
+    ):
+        # 三方平台的客户ID
+        self.customer_id = customer_id
+        # 三方平台客户名称
+        self.customer_name = customer_name
+        # 联系人
+        self.contact_person = contact_person
+        # 联系电话
+        self.contact_telephone = contact_telephone
+        # 联系邮箱
+        self.contact_email = contact_email
+        # 统一社会信用代码
+        self.social_credit_code = social_credit_code
+
+    def validate(self):
+        self.validate_required(self.customer_id, 'customer_id')
+        self.validate_required(self.customer_name, 'customer_name')
+        self.validate_required(self.contact_person, 'contact_person')
+        self.validate_required(self.contact_telephone, 'contact_telephone')
+        self.validate_required(self.social_credit_code, 'social_credit_code')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.inventory_scope_no is not None:
-            result['inventory_scope_no'] = self.inventory_scope_no
-        if self.inventory_scope_name is not None:
-            result['inventory_scope_name'] = self.inventory_scope_name
-        if self.emissions is not None:
-            result['emissions'] = self.emissions
-        if self.percentage is not None:
-            result['percentage'] = self.percentage
-        result['category_emissions_list'] = []
-        if self.category_emissions_list is not None:
-            for k in self.category_emissions_list:
-                result['category_emissions_list'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('inventory_scope_no') is not None:
-            self.inventory_scope_no = m.get('inventory_scope_no')
-        if m.get('inventory_scope_name') is not None:
-            self.inventory_scope_name = m.get('inventory_scope_name')
-        if m.get('emissions') is not None:
-            self.emissions = m.get('emissions')
-        if m.get('percentage') is not None:
-            self.percentage = m.get('percentage')
-        self.category_emissions_list = []
-        if m.get('category_emissions_list') is not None:
-            for k in m.get('category_emissions_list'):
-                temp_model = EmissionsCategoryStatistics()
-                self.category_emissions_list.append(temp_model.from_map(k))
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
+        if self.customer_name is not None:
+            result['customer_name'] = self.customer_name
+        if self.contact_person is not None:
+            result['contact_person'] = self.contact_person
+        if self.contact_telephone is not None:
+            result['contact_telephone'] = self.contact_telephone
+        if self.contact_email is not None:
+            result['contact_email'] = self.contact_email
+        if self.social_credit_code is not None:
+            result['social_credit_code'] = self.social_credit_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
+        if m.get('customer_name') is not None:
+            self.customer_name = m.get('customer_name')
+        if m.get('contact_person') is not None:
+            self.contact_person = m.get('contact_person')
+        if m.get('contact_telephone') is not None:
+            self.contact_telephone = m.get('contact_telephone')
+        if m.get('contact_email') is not None:
+            self.contact_email = m.get('contact_email')
+        if m.get('social_credit_code') is not None:
+            self.social_credit_code = m.get('social_credit_code')
         return self
 
 
 class EmissionsLocationStatistics(TeaModel):
     def __init__(
         self,
         location_no: str = None,
@@ -1395,14 +1332,529 @@
         if m.get('item_code') is not None:
             self.item_code = m.get('item_code')
         if m.get('item_value') is not None:
             self.item_value = m.get('item_value')
         return self
 
 
+class LcaCarbonDatum(TeaModel):
+    def __init__(
+        self,
+        lca_carbon_amount: str = None,
+        lca_report_file_url: str = None,
+        lca_detail_file_url: str = None,
+        life_cycle_boundary: str = None,
+        lca_start_date: str = None,
+        lca_end_date: str = None,
+        lca_stage_carbon_datum: List[LcaStageCarbonItem] = None,
+    ):
+        # LCA碳排放总量
+        self.lca_carbon_amount = lca_carbon_amount
+        # 足迹报告pdf文件下载地址（30分钟内下载有效）
+        self.lca_report_file_url = lca_report_file_url
+        # 足迹分析结果详情文件地址（30分钟内下载有效）
+        self.lca_detail_file_url = lca_detail_file_url
+        # B2B-从摇篮到大门，B2C-从摇篮到坟墓
+        self.life_cycle_boundary = life_cycle_boundary
+        # 足迹开始时间，格式：yyyyMMdd
+        self.lca_start_date = lca_start_date
+        # 足迹结束时间 格式：yyyyMMdd
+        self.lca_end_date = lca_end_date
+        # 分阶段碳排放量列表
+        self.lca_stage_carbon_datum = lca_stage_carbon_datum
+
+    def validate(self):
+        self.validate_required(self.lca_carbon_amount, 'lca_carbon_amount')
+        self.validate_required(self.lca_report_file_url, 'lca_report_file_url')
+        self.validate_required(self.lca_detail_file_url, 'lca_detail_file_url')
+        self.validate_required(self.life_cycle_boundary, 'life_cycle_boundary')
+        self.validate_required(self.lca_start_date, 'lca_start_date')
+        self.validate_required(self.lca_end_date, 'lca_end_date')
+        self.validate_required(self.lca_stage_carbon_datum, 'lca_stage_carbon_datum')
+        if self.lca_stage_carbon_datum:
+            for k in self.lca_stage_carbon_datum:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.lca_carbon_amount is not None:
+            result['lca_carbon_amount'] = self.lca_carbon_amount
+        if self.lca_report_file_url is not None:
+            result['lca_report_file_url'] = self.lca_report_file_url
+        if self.lca_detail_file_url is not None:
+            result['lca_detail_file_url'] = self.lca_detail_file_url
+        if self.life_cycle_boundary is not None:
+            result['life_cycle_boundary'] = self.life_cycle_boundary
+        if self.lca_start_date is not None:
+            result['lca_start_date'] = self.lca_start_date
+        if self.lca_end_date is not None:
+            result['lca_end_date'] = self.lca_end_date
+        result['lca_stage_carbon_datum'] = []
+        if self.lca_stage_carbon_datum is not None:
+            for k in self.lca_stage_carbon_datum:
+                result['lca_stage_carbon_datum'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('lca_carbon_amount') is not None:
+            self.lca_carbon_amount = m.get('lca_carbon_amount')
+        if m.get('lca_report_file_url') is not None:
+            self.lca_report_file_url = m.get('lca_report_file_url')
+        if m.get('lca_detail_file_url') is not None:
+            self.lca_detail_file_url = m.get('lca_detail_file_url')
+        if m.get('life_cycle_boundary') is not None:
+            self.life_cycle_boundary = m.get('life_cycle_boundary')
+        if m.get('lca_start_date') is not None:
+            self.lca_start_date = m.get('lca_start_date')
+        if m.get('lca_end_date') is not None:
+            self.lca_end_date = m.get('lca_end_date')
+        self.lca_stage_carbon_datum = []
+        if m.get('lca_stage_carbon_datum') is not None:
+            for k in m.get('lca_stage_carbon_datum'):
+                temp_model = LcaStageCarbonItem()
+                self.lca_stage_carbon_datum.append(temp_model.from_map(k))
+        return self
+
+
+class EnterpriseProductOutline(TeaModel):
+    def __init__(
+        self,
+        enterprise_custom_code: str = None,
+        product_name: str = None,
+        specification: str = None,
+        product_description: str = None,
+        product_category_name: str = None,
+        brand_information: str = None,
+    ):
+        # 产品自定义编码
+        # 
+        self.enterprise_custom_code = enterprise_custom_code
+        # 产品名称
+        # 
+        self.product_name = product_name
+        # 规格型号
+        self.specification = specification
+        # 产品描述
+        self.product_description = product_description
+        # 产品分类名称
+        self.product_category_name = product_category_name
+        # 品牌信息
+        self.brand_information = brand_information
+
+    def validate(self):
+        self.validate_required(self.enterprise_custom_code, 'enterprise_custom_code')
+        self.validate_required(self.product_name, 'product_name')
+        self.validate_required(self.specification, 'specification')
+        self.validate_required(self.product_category_name, 'product_category_name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enterprise_custom_code is not None:
+            result['enterprise_custom_code'] = self.enterprise_custom_code
+        if self.product_name is not None:
+            result['product_name'] = self.product_name
+        if self.specification is not None:
+            result['specification'] = self.specification
+        if self.product_description is not None:
+            result['product_description'] = self.product_description
+        if self.product_category_name is not None:
+            result['product_category_name'] = self.product_category_name
+        if self.brand_information is not None:
+            result['brand_information'] = self.brand_information
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enterprise_custom_code') is not None:
+            self.enterprise_custom_code = m.get('enterprise_custom_code')
+        if m.get('product_name') is not None:
+            self.product_name = m.get('product_name')
+        if m.get('specification') is not None:
+            self.specification = m.get('specification')
+        if m.get('product_description') is not None:
+            self.product_description = m.get('product_description')
+        if m.get('product_category_name') is not None:
+            self.product_category_name = m.get('product_category_name')
+        if m.get('brand_information') is not None:
+            self.brand_information = m.get('brand_information')
+        return self
+
+
+class CarbonOffsetActiveDataDetail(TeaModel):
+    def __init__(
+        self,
+        active_data_no: str = None,
+        active_data_name: str = None,
+        active_data_unit: str = None,
+        description: str = None,
+        active_data_value: str = None,
+    ):
+        # 活动数据编号
+        self.active_data_no = active_data_no
+        # 活动数据名称
+        self.active_data_name = active_data_name
+        # 活动数据单位
+        self.active_data_unit = active_data_unit
+        # 活动数据描述文案
+        self.description = description
+        # 活动数据值
+        self.active_data_value = active_data_value
+
+    def validate(self):
+        self.validate_required(self.active_data_no, 'active_data_no')
+        self.validate_required(self.active_data_value, 'active_data_value')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_data_no is not None:
+            result['active_data_no'] = self.active_data_no
+        if self.active_data_name is not None:
+            result['active_data_name'] = self.active_data_name
+        if self.active_data_unit is not None:
+            result['active_data_unit'] = self.active_data_unit
+        if self.description is not None:
+            result['description'] = self.description
+        if self.active_data_value is not None:
+            result['active_data_value'] = self.active_data_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('active_data_no') is not None:
+            self.active_data_no = m.get('active_data_no')
+        if m.get('active_data_name') is not None:
+            self.active_data_name = m.get('active_data_name')
+        if m.get('active_data_unit') is not None:
+            self.active_data_unit = m.get('active_data_unit')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('active_data_value') is not None:
+            self.active_data_value = m.get('active_data_value')
+        return self
+
+
+class EnterpriseMemberSummary(TeaModel):
+    def __init__(
+        self,
+        account_did: str = None,
+        name: str = None,
+        mobile: str = None,
+        register_time: str = None,
+    ):
+        # 机构会员DID
+        self.account_did = account_did
+        # 会员姓名，数据脱敏处理返回
+        self.name = name
+        # 会员手机号码，数据脱敏处理返回
+        self.mobile = mobile
+        # 会员注册时间
+        self.register_time = register_time
+
+    def validate(self):
+        self.validate_required(self.account_did, 'account_did')
+        self.validate_required(self.register_time, 'register_time')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.name is not None:
+            result['name'] = self.name
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
+        if self.register_time is not None:
+            result['register_time'] = self.register_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
+        if m.get('register_time') is not None:
+            self.register_time = m.get('register_time')
+        return self
+
+
+class AnyStatisticalItem(TeaModel):
+    def __init__(
+        self,
+        item_code: str = None,
+        amount: str = None,
+        unit: str = None,
+        unit_label: str = None,
+    ):
+        # 统计项目编码
+        self.item_code = item_code
+        # 数据值，按字符串输出，最多保留6位小数
+        self.amount = amount
+        # 单位编码
+        self.unit = unit
+        # 单位标签
+        self.unit_label = unit_label
+
+    def validate(self):
+        self.validate_required(self.item_code, 'item_code')
+        self.validate_required(self.amount, 'amount')
+        self.validate_required(self.unit, 'unit')
+        self.validate_required(self.unit_label, 'unit_label')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_code is not None:
+            result['item_code'] = self.item_code
+        if self.amount is not None:
+            result['amount'] = self.amount
+        if self.unit is not None:
+            result['unit'] = self.unit
+        if self.unit_label is not None:
+            result['unit_label'] = self.unit_label
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('item_code') is not None:
+            self.item_code = m.get('item_code')
+        if m.get('amount') is not None:
+            self.amount = m.get('amount')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
+        if m.get('unit_label') is not None:
+            self.unit_label = m.get('unit_label')
+        return self
+
+
+class EnterpriseProductSummary(TeaModel):
+    def __init__(
+        self,
+        enterprise_custom_code: str = None,
+        product_name: str = None,
+        specification: str = None,
+        product_description: str = None,
+        product_category_name: str = None,
+        brand_information: str = None,
+        process_flow_file_list: List[EnterpriseDocumentFile] = None,
+        product_picture_file_list: List[EnterpriseDocumentFile] = None,
+    ):
+        # 产品自定义编码
+        self.enterprise_custom_code = enterprise_custom_code
+        # 产品名称
+        self.product_name = product_name
+        # 规格型号
+        self.specification = specification
+        # 产品描述
+        self.product_description = product_description
+        # 产品分类名称
+        self.product_category_name = product_category_name
+        # 品牌信息
+        self.brand_information = brand_information
+        # 工艺流程文件路径，上传文件后由上传文件接口提供，最多支持上传3个工艺流程文件
+        self.process_flow_file_list = process_flow_file_list
+        # 产品图片文件路径，上传文件后由上传文件接口提供，最多支持上传8个产品图片文件
+        self.product_picture_file_list = product_picture_file_list
+
+    def validate(self):
+        self.validate_required(self.enterprise_custom_code, 'enterprise_custom_code')
+        self.validate_required(self.product_name, 'product_name')
+        self.validate_required(self.specification, 'specification')
+        self.validate_required(self.product_category_name, 'product_category_name')
+        if self.process_flow_file_list:
+            for k in self.process_flow_file_list:
+                if k:
+                    k.validate()
+        if self.product_picture_file_list:
+            for k in self.product_picture_file_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enterprise_custom_code is not None:
+            result['enterprise_custom_code'] = self.enterprise_custom_code
+        if self.product_name is not None:
+            result['product_name'] = self.product_name
+        if self.specification is not None:
+            result['specification'] = self.specification
+        if self.product_description is not None:
+            result['product_description'] = self.product_description
+        if self.product_category_name is not None:
+            result['product_category_name'] = self.product_category_name
+        if self.brand_information is not None:
+            result['brand_information'] = self.brand_information
+        result['process_flow_file_list'] = []
+        if self.process_flow_file_list is not None:
+            for k in self.process_flow_file_list:
+                result['process_flow_file_list'].append(k.to_map() if k else None)
+        result['product_picture_file_list'] = []
+        if self.product_picture_file_list is not None:
+            for k in self.product_picture_file_list:
+                result['product_picture_file_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enterprise_custom_code') is not None:
+            self.enterprise_custom_code = m.get('enterprise_custom_code')
+        if m.get('product_name') is not None:
+            self.product_name = m.get('product_name')
+        if m.get('specification') is not None:
+            self.specification = m.get('specification')
+        if m.get('product_description') is not None:
+            self.product_description = m.get('product_description')
+        if m.get('product_category_name') is not None:
+            self.product_category_name = m.get('product_category_name')
+        if m.get('brand_information') is not None:
+            self.brand_information = m.get('brand_information')
+        self.process_flow_file_list = []
+        if m.get('process_flow_file_list') is not None:
+            for k in m.get('process_flow_file_list'):
+                temp_model = EnterpriseDocumentFile()
+                self.process_flow_file_list.append(temp_model.from_map(k))
+        self.product_picture_file_list = []
+        if m.get('product_picture_file_list') is not None:
+            for k in m.get('product_picture_file_list'):
+                temp_model = EnterpriseDocumentFile()
+                self.product_picture_file_list.append(temp_model.from_map(k))
+        return self
+
+
+class BlockchainDTO(TeaModel):
+    def __init__(
+        self,
+        tx_hash: str = None,
+        block_number: int = None,
+    ):
+        # 交易hash
+        self.tx_hash = tx_hash
+        # 当前块高
+        self.block_number = block_number
+
+    def validate(self):
+        self.validate_required(self.tx_hash, 'tx_hash')
+        self.validate_required(self.block_number, 'block_number')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tx_hash is not None:
+            result['tx_hash'] = self.tx_hash
+        if self.block_number is not None:
+            result['block_number'] = self.block_number
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('tx_hash') is not None:
+            self.tx_hash = m.get('tx_hash')
+        if m.get('block_number') is not None:
+            self.block_number = m.get('block_number')
+        return self
+
+
+class EmissionsScopeStatistics(TeaModel):
+    def __init__(
+        self,
+        inventory_scope_no: str = None,
+        inventory_scope_name: str = None,
+        emissions: int = None,
+        percentage: int = None,
+        category_emissions_list: List[EmissionsCategoryStatistics] = None,
+    ):
+        # 盘查范围编码
+        self.inventory_scope_no = inventory_scope_no
+        # 盘查范围名称
+        self.inventory_scope_name = inventory_scope_name
+        # 碳排放量
+        self.emissions = emissions
+        # 排放占比
+        self.percentage = percentage
+        # 范围下各分类排放数据
+        self.category_emissions_list = category_emissions_list
+
+    def validate(self):
+        self.validate_required(self.inventory_scope_no, 'inventory_scope_no')
+        self.validate_required(self.inventory_scope_name, 'inventory_scope_name')
+        self.validate_required(self.emissions, 'emissions')
+        self.validate_required(self.percentage, 'percentage')
+        self.validate_required(self.category_emissions_list, 'category_emissions_list')
+        if self.category_emissions_list:
+            for k in self.category_emissions_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.inventory_scope_no is not None:
+            result['inventory_scope_no'] = self.inventory_scope_no
+        if self.inventory_scope_name is not None:
+            result['inventory_scope_name'] = self.inventory_scope_name
+        if self.emissions is not None:
+            result['emissions'] = self.emissions
+        if self.percentage is not None:
+            result['percentage'] = self.percentage
+        result['category_emissions_list'] = []
+        if self.category_emissions_list is not None:
+            for k in self.category_emissions_list:
+                result['category_emissions_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('inventory_scope_no') is not None:
+            self.inventory_scope_no = m.get('inventory_scope_no')
+        if m.get('inventory_scope_name') is not None:
+            self.inventory_scope_name = m.get('inventory_scope_name')
+        if m.get('emissions') is not None:
+            self.emissions = m.get('emissions')
+        if m.get('percentage') is not None:
+            self.percentage = m.get('percentage')
+        self.category_emissions_list = []
+        if m.get('category_emissions_list') is not None:
+            for k in m.get('category_emissions_list'):
+                temp_model = EmissionsCategoryStatistics()
+                self.category_emissions_list.append(temp_model.from_map(k))
+        return self
+
+
 class GreenOperationStatisticsByFrequence(TeaModel):
     def __init__(
         self,
         occurrence_period: str = None,
         green_energy_amount: int = None,
         green_operation_records: int = None,
     ):
@@ -6762,14 +7214,636 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class UploadEcarPlaformfileRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        file_name: str = None,
+        file_object: BinaryIO = None,
+        file_object_name: str = None,
+        file_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 上传的文件名
+        self.file_name = file_name
+        # 待上传文件
+        # 待上传文件
+        self.file_object = file_object
+        # 待上传文件名
+        self.file_object_name = file_object_name
+        self.file_id = file_id
+
+    def validate(self):
+        self.validate_required(self.file_id, 'file_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.file_object is not None:
+            result['fileObject'] = self.file_object
+        if self.file_object_name is not None:
+            result['fileObjectName'] = self.file_object_name
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('fileObject') is not None:
+            self.file_object = m.get('fileObject')
+        if m.get('fileObjectName') is not None:
+            self.file_object_name = m.get('fileObjectName')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        return self
+
+
+class UploadEcarPlaformfileResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        document_name: str = None,
+        document_address: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 文档名称
+        self.document_name = document_name
+        # 文档地址信息
+        self.document_address = document_address
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.document_name is not None:
+            result['document_name'] = self.document_name
+        if self.document_address is not None:
+            result['document_address'] = self.document_address
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('document_name') is not None:
+            self.document_name = m.get('document_name')
+        if m.get('document_address') is not None:
+            self.document_address = m.get('document_address')
+        return self
+
+
+class SubmitEcarLcaorderwithcustomerRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        customer: PlatformCustomerSummary = None,
+        product: EnterpriseProductSummary = None,
+        order_time: str = None,
+        order_amount: str = None,
+        source_order_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 客户信息
+        self.customer = customer
+        # 产品信息
+        self.product = product
+        # 订单时间，格式：yyyy-MM-dd HH:mm:ss
+        self.order_time = order_time
+        # 订单金额，订单金额只能为有效数字（整数不得大于10位，小数不得大于6位）
+        self.order_amount = order_amount
+        # 来源于三方平台的订单编号
+        self.source_order_no = source_order_no
+
+    def validate(self):
+        self.validate_required(self.customer, 'customer')
+        if self.customer:
+            self.customer.validate()
+        self.validate_required(self.product, 'product')
+        if self.product:
+            self.product.validate()
+        self.validate_required(self.order_time, 'order_time')
+        self.validate_required(self.order_amount, 'order_amount')
+        self.validate_required(self.source_order_no, 'source_order_no')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.customer is not None:
+            result['customer'] = self.customer.to_map()
+        if self.product is not None:
+            result['product'] = self.product.to_map()
+        if self.order_time is not None:
+            result['order_time'] = self.order_time
+        if self.order_amount is not None:
+            result['order_amount'] = self.order_amount
+        if self.source_order_no is not None:
+            result['source_order_no'] = self.source_order_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('customer') is not None:
+            temp_model = PlatformCustomerSummary()
+            self.customer = temp_model.from_map(m['customer'])
+        if m.get('product') is not None:
+            temp_model = EnterpriseProductSummary()
+            self.product = temp_model.from_map(m['product'])
+        if m.get('order_time') is not None:
+            self.order_time = m.get('order_time')
+        if m.get('order_amount') is not None:
+            self.order_amount = m.get('order_amount')
+        if m.get('source_order_no') is not None:
+            self.source_order_no = m.get('source_order_no')
+        return self
+
+
+class SubmitEcarLcaorderwithcustomerResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_no: str = None,
+        source_order_no: str = None,
+        carbon_account_no: str = None,
+        order_status: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 订单编号
+        self.order_no = order_no
+        # 来源于三方平台的订单编号
+        self.source_order_no = source_order_no
+        # 碳账户编号，碳矩阵为客户分配的碳账户编号
+        self.carbon_account_no = carbon_account_no
+        # 订单状态，Pending——处理中，Closed——已关闭，Finished——已完成
+        self.order_status = order_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_no is not None:
+            result['order_no'] = self.order_no
+        if self.source_order_no is not None:
+            result['source_order_no'] = self.source_order_no
+        if self.carbon_account_no is not None:
+            result['carbon_account_no'] = self.carbon_account_no
+        if self.order_status is not None:
+            result['order_status'] = self.order_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_no') is not None:
+            self.order_no = m.get('order_no')
+        if m.get('source_order_no') is not None:
+            self.source_order_no = m.get('source_order_no')
+        if m.get('carbon_account_no') is not None:
+            self.carbon_account_no = m.get('carbon_account_no')
+        if m.get('order_status') is not None:
+            self.order_status = m.get('order_status')
+        return self
+
+
+class GetEcarPlaformauthtokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        customer_id: str = None,
+        carbon_account_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 三方平台的客户ID
+        self.customer_id = customer_id
+        # 碳账户编号，碳矩阵为客户分配的碳账户编号，跟前面三方平台的客户customer_id必须任意传一个参数，优先使用customer_id查询客户
+        self.carbon_account_no = carbon_account_no
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
+        if self.carbon_account_no is not None:
+            result['carbon_account_no'] = self.carbon_account_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
+        if m.get('carbon_account_no') is not None:
+            self.carbon_account_no = m.get('carbon_account_no')
+        return self
+
+
+class GetEcarPlaformauthtokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        customer_id: str = None,
+        carbon_account_no: str = None,
+        access_token: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 三方平台客户ID
+        self.customer_id = customer_id
+        # 碳账户编号，碳矩阵为客户分配的碳账户编号
+        self.carbon_account_no = carbon_account_no
+        # 授权三方平台客户信登的TOKEN
+        self.access_token = access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
+        if self.carbon_account_no is not None:
+            result['carbon_account_no'] = self.carbon_account_no
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
+        if m.get('carbon_account_no') is not None:
+            self.carbon_account_no = m.get('carbon_account_no')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        return self
+
+
+class QueryEcarLcaorderRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_no: str = None,
+        source_order_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单号码
+        self.order_no = order_no
+        # 来源于三方平台的订单编号，跟前面的订单编号order_no必须任传一个进行订单查询。优先使用碳矩阵平台生成的订单编号查询
+        self.source_order_no = source_order_no
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.order_no is not None:
+            result['order_no'] = self.order_no
+        if self.source_order_no is not None:
+            result['source_order_no'] = self.source_order_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_no') is not None:
+            self.order_no = m.get('order_no')
+        if m.get('source_order_no') is not None:
+            self.source_order_no = m.get('source_order_no')
+        return self
+
+
+class QueryEcarLcaorderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_no: str = None,
+        source_order_no: str = None,
+        customer_id: str = None,
+        carbon_account_no: str = None,
+        order_status: str = None,
+        product: EnterpriseProductOutline = None,
+        lca_carbon_datum: LcaCarbonDatum = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # LCA订单单号
+        self.order_no = order_no
+        # 来源于三方平台的订单编号
+        self.source_order_no = source_order_no
+        # 三方平台客户ID，在三方平台唯一
+        self.customer_id = customer_id
+        # 碳账户编号，碳矩阵为客户分配的碳账户编号
+        self.carbon_account_no = carbon_account_no
+        # Pending——待分配，Closed——已关闭，Allocated——已分配，Finished——已完成
+        self.order_status = order_status
+        # 产品概要信息
+        self.product = product
+        # 足迹计算信息
+        self.lca_carbon_datum = lca_carbon_datum
+
+    def validate(self):
+        if self.product:
+            self.product.validate()
+        if self.lca_carbon_datum:
+            self.lca_carbon_datum.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_no is not None:
+            result['order_no'] = self.order_no
+        if self.source_order_no is not None:
+            result['source_order_no'] = self.source_order_no
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
+        if self.carbon_account_no is not None:
+            result['carbon_account_no'] = self.carbon_account_no
+        if self.order_status is not None:
+            result['order_status'] = self.order_status
+        if self.product is not None:
+            result['product'] = self.product.to_map()
+        if self.lca_carbon_datum is not None:
+            result['lca_carbon_datum'] = self.lca_carbon_datum.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_no') is not None:
+            self.order_no = m.get('order_no')
+        if m.get('source_order_no') is not None:
+            self.source_order_no = m.get('source_order_no')
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
+        if m.get('carbon_account_no') is not None:
+            self.carbon_account_no = m.get('carbon_account_no')
+        if m.get('order_status') is not None:
+            self.order_status = m.get('order_status')
+        if m.get('product') is not None:
+            temp_model = EnterpriseProductOutline()
+            self.product = temp_model.from_map(m['product'])
+        if m.get('lca_carbon_datum') is not None:
+            temp_model = LcaCarbonDatum()
+            self.lca_carbon_datum = temp_model.from_map(m['lca_carbon_datum'])
+        return self
+
+
+class BatchcreateEcarGreencertificategenerationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        date: str = None,
+        generation: List[DeviceGeneration] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 数据发生时间
+        self.date = date
+        # 设备发电量列表
+        self.generation = generation
+
+    def validate(self):
+        self.validate_required(self.date, 'date')
+        self.validate_required(self.generation, 'generation')
+        if self.generation:
+            for k in self.generation:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.date is not None:
+            result['date'] = self.date
+        result['generation'] = []
+        if self.generation is not None:
+            for k in self.generation:
+                result['generation'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('date') is not None:
+            self.date = m.get('date')
+        self.generation = []
+        if m.get('generation') is not None:
+            for k in m.get('generation'):
+                temp_model = DeviceGeneration()
+                self.generation.append(temp_model.from_map(k))
+        return self
+
+
+class BatchcreateEcarGreencertificategenerationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
```

### Comparing `antchain_stlr-2.6.0/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.7.4/antchain_stlr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.6.0
+Version: 2.7.4
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.6.0/setup.py` & `antchain_stlr-2.7.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 21/06/2023
+Created on 19/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

