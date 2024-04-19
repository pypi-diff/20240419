# Comparing `tmp/alibabacloud_emr20210320-1.5.0.tar.gz` & `tmp/alibabacloud_emr20210320-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr20210320-1.5.0.tar", last modified: Wed Apr 17 17:15:44 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr20210320-1.6.0.tar", last modified: Thu Apr 18 12:26:11 2024, max compression
```

## Comparing `alibabacloud_emr20210320-1.5.0.tar` & `alibabacloud_emr20210320-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/
--rw-r--r--   0 root         (0) root         (0)     1317 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252698 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/client.py
--rw-r--r--   0 root         (0) root         (0)  1657374 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260572 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320/client.py
+-rw-r--r--   0 root         (0) root         (0)  1665651 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-18 12:26:11.000000 alibabacloud_emr20210320-1.6.0/setup.py
```

### Comparing `alibabacloud_emr20210320-1.5.0/ChangeLog.md` & `alibabacloud_emr20210320-1.6.0/ChangeLog.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2024-04-17 Version: 1.5.0
+- Support API DeleteApiTemplate.
+- Support API GetApiTemplate.
+- Support API ListApiTemplates.
+- Support API RunApiTemplate.
+
+
 2024-03-26 Version: 1.4.2
 - Generated python 2021-03-20 for Emr.
 
 2024-03-15 Version: 1.4.1
 - Update API GetAutoScalingPolicy: update response param.
```

### Comparing `alibabacloud_emr20210320-1.5.0/LICENSE` & `alibabacloud_emr20210320-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320-1.5.0/PKG-INFO` & `alibabacloud_emr20210320-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_emr20210320
-Version: 1.5.0
+Version: 1.6.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320-1.5.0/README-CN.md` & `alibabacloud_emr20210320-1.6.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320-1.5.0/README.md` & `alibabacloud_emr20210320-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/client.py` & `alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,100 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def create_api_template_with_options(
+        self,
+        request: emr_20210320_models.CreateApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.CreateApiTemplateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.content):
+            query['Content'] = request.content
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.CreateApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_api_template_with_options_async(
+        self,
+        request: emr_20210320_models.CreateApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.CreateApiTemplateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.content):
+            query['Content'] = request.content
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.CreateApiTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_api_template(
+        self,
+        request: emr_20210320_models.CreateApiTemplateRequest,
+    ) -> emr_20210320_models.CreateApiTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_api_template_with_options(request, runtime)
+
+    async def create_api_template_async(
+        self,
+        request: emr_20210320_models.CreateApiTemplateRequest,
+    ) -> emr_20210320_models.CreateApiTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_api_template_with_options_async(request, runtime)
+
     def create_cluster_with_options(
         self,
         request: emr_20210320_models.CreateClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> emr_20210320_models.CreateClusterResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6332,14 +6418,130 @@
         
         @param request: UntagResourcesRequest
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
 
+    def update_api_template_with_options(
+        self,
+        request: emr_20210320_models.UpdateApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.UpdateApiTemplateResponse:
+        """
+        修改集群模板
+        
+        @param request: UpdateApiTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.content):
+            query['Content'] = request.content
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.UpdateApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_api_template_with_options_async(
+        self,
+        request: emr_20210320_models.UpdateApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.UpdateApiTemplateResponse:
+        """
+        修改集群模板
+        
+        @param request: UpdateApiTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.content):
+            query['Content'] = request.content
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.UpdateApiTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_api_template(
+        self,
+        request: emr_20210320_models.UpdateApiTemplateRequest,
+    ) -> emr_20210320_models.UpdateApiTemplateResponse:
+        """
+        修改集群模板
+        
+        @param request: UpdateApiTemplateRequest
+        @return: UpdateApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.update_api_template_with_options(request, runtime)
+
+    async def update_api_template_async(
+        self,
+        request: emr_20210320_models.UpdateApiTemplateRequest,
+    ) -> emr_20210320_models.UpdateApiTemplateResponse:
+        """
+        修改集群模板
+        
+        @param request: UpdateApiTemplateRequest
+        @return: UpdateApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.update_api_template_with_options_async(request, runtime)
+
     def update_application_configs_with_options(
         self,
         request: emr_20210320_models.UpdateApplicationConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> emr_20210320_models.UpdateApplicationConfigsResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/models.py` & `alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7086,14 +7086,151 @@
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
+class CreateApiTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        api_name: str = None,
+        content: str = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        template_name: str = None,
+    ):
+        # 接口名。
+        self.api_name = api_name
+        # 接口request内容。
+        self.content = content
+        # 地域ID。
+        self.region_id = region_id
+        # 资源组ID。
+        self.resource_group_id = resource_group_id
+        # 集群模板名字。
+        self.template_name = template_name
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
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class CreateApiTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        success: str = None,
+        template_id: str = None,
+    ):
+        # 请求ID。
+        self.request_id = request_id
+        self.success = success
+        self.template_id = template_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class CreateApiTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateApiTemplateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateClusterRequest(TeaModel):
     def __init__(
         self,
         application_configs: List[ApplicationConfig] = None,
         applications: List[Application] = None,
         bootstrap_scripts: List[Script] = None,
         client_token: str = None,
@@ -46747,14 +46884,152 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateApiTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        api_name: str = None,
+        content: str = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        template_id: str = None,
+        template_name: str = None,
+    ):
+        # 接口名。
+        self.api_name = api_name
+        # 接口request内容。
+        self.content = content
+        # 区域ID。
+        self.region_id = region_id
+        # 资源组ID。
+        self.resource_group_id = resource_group_id
+        # 集群模板id。
+        self.template_id = template_id
+        # 集群模板名字。
+        self.template_name = template_name
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
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class UpdateApiTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        # 请求ID。
+        self.request_id = request_id
+        self.success = success
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UpdateApiTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateApiTemplateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateApplicationConfigsRequest(TeaModel):
     def __init__(
         self,
         application_configs: List[UpdateApplicationConfig] = None,
         application_name: str = None,
         cluster_id: str = None,
         config_action: str = None,
```

### Comparing `alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/PKG-INFO` & `alibabacloud_emr20210320-1.6.0/alibabacloud_emr20210320.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-emr20210320
-Version: 1.5.0
+Version: 1.6.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320-1.5.0/setup.py` & `alibabacloud_emr20210320-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr20210320.
 
-Created on 17/04/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr20210320"
 NAME = "alibabacloud_emr20210320" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Emr (20210320) SDK Library for Python"
```

