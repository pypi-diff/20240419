# Comparing `tmp/alibabacloud_emr20210320_py2-1.5.0.tar.gz` & `tmp/alibabacloud_emr20210320_py2-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr20210320_py2-1.5.0.tar", last modified: Wed Apr 17 17:11:57 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr20210320_py2-1.6.0.tar", last modified: Fri Apr 19 06:24:27 2024, max compression
```

## Comparing `alibabacloud_emr20210320_py2-1.5.0.tar` & `alibabacloud_emr20210320_py2-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/
--rw-r--r--   0 root         (0) root         (0)     2667 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109730 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/client.py
--rw-r--r--   0 root         (0) root         (0)  1678468 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:11:57.000000 alibabacloud_emr20210320_py2-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2024-04-17 17:11:56.000000 alibabacloud_emr20210320_py2-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/
+-rw-r--r--   0 root         (0) root         (0)     2820 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   113080 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320/client.py
+-rw-r--r--   0 root         (0) root         (0)  1686772 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-19 06:24:27.000000 alibabacloud_emr20210320_py2-1.6.0/setup.py
```

### Comparing `alibabacloud_emr20210320_py2-1.5.0/ChangeLog.md` & `alibabacloud_emr20210320_py2-1.6.0/ChangeLog.md`

 * *Files 8% similar despite different names*

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
 - Generated python2 2021-03-20 for Emr.
 
 2024-03-15 Version: 1.4.1
 - Update API GetAutoScalingPolicy: update response param.
```

### Comparing `alibabacloud_emr20210320_py2-1.5.0/LICENSE` & `alibabacloud_emr20210320_py2-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320_py2-1.5.0/PKG-INFO` & `alibabacloud_emr20210320_py2-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_emr20210320_py2
-Version: 1.5.0
+Version: 1.6.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320_py2-1.5.0/README-CN.md` & `alibabacloud_emr20210320_py2-1.6.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320_py2-1.5.0/README.md` & `alibabacloud_emr20210320_py2-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/client.py` & `alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,50 @@
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def create_api_template_with_options(self, request, runtime):
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
+    def create_api_template(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_api_template_with_options(request, runtime)
+
     def create_cluster_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.application_configs):
             query['ApplicationConfigs'] = request.application_configs
         if not UtilClient.is_unset(request.applications):
             query['Applications'] = request.applications
@@ -2983,14 +3019,70 @@
         @param request: UntagResourcesRequest
 
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
+    def update_api_template_with_options(self, request, runtime):
+        """
+        修改集群模板
+        
+
+        @param request: UpdateApiTemplateRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
+    def update_api_template(self, request):
+        """
+        修改集群模板
+        
+
+        @param request: UpdateApiTemplateRequest
+
+        @return: UpdateApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.update_api_template_with_options(request, runtime)
+
     def update_application_configs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.application_configs):
             query['ApplicationConfigs'] = request.application_configs
         if not UtilClient.is_unset(request.application_name):
             query['ApplicationName'] = request.application_name
```

### Comparing `alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320/models.py` & `alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6301,14 +6301,134 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Values') is not None:
             self.values = m.get('Values')
         return self
 
 
+class CreateApiTemplateRequest(TeaModel):
+    def __init__(self, api_name=None, content=None, region_id=None, resource_group_id=None, template_name=None):
+        # 接口名。
+        self.api_name = api_name  # type: str
+        # 接口request内容。
+        self.content = content  # type: str
+        # 地域ID。
+        self.region_id = region_id  # type: str
+        # 资源组ID。
+        self.resource_group_id = resource_group_id  # type: str
+        # 集群模板名字。
+        self.template_name = template_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateApiTemplateRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, success=None, template_id=None):
+        # 请求ID。
+        self.request_id = request_id  # type: str
+        self.success = success  # type: str
+        self.template_id = template_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateApiTemplateResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateApiTemplateResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateApiTemplateResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, application_configs=None, applications=None, bootstrap_scripts=None, client_token=None,
                  cluster_name=None, cluster_type=None, deploy_mode=None, node_attributes=None, node_groups=None,
                  payment_type=None, region_id=None, release_version=None, resource_group_id=None, security_mode=None,
                  subscription_config=None, tags=None):
         # The configurations of the applications. Valid values of N: 1 to 1000.
         self.application_configs = application_configs  # type: list[ApplicationConfig]
@@ -41441,14 +41561,136 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateApiTemplateRequest(TeaModel):
+    def __init__(self, api_name=None, content=None, region_id=None, resource_group_id=None, template_id=None,
+                 template_name=None):
+        # 接口名。
+        self.api_name = api_name  # type: str
+        # 接口request内容。
+        self.content = content  # type: str
+        # 区域ID。
+        self.region_id = region_id  # type: str
+        # 资源组ID。
+        self.resource_group_id = resource_group_id  # type: str
+        # 集群模板id。
+        self.template_id = template_id  # type: str
+        # 集群模板名字。
+        self.template_name = template_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateApiTemplateRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, success=None):
+        # 请求ID。
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateApiTemplateResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UpdateApiTemplateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UpdateApiTemplateResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UpdateApiTemplateResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, application_configs=None, application_name=None, cluster_id=None, config_action=None,
                  config_scope=None, description=None, node_group_id=None, node_id=None, region_id=None):
         # The application configurations.
         self.application_configs = application_configs  # type: list[UpdateApplicationConfig]
         # The application name.
         self.application_name = application_name  # type: str
```

### Comparing `alibabacloud_emr20210320_py2-1.5.0/alibabacloud_emr20210320_py2.egg-info/PKG-INFO` & `alibabacloud_emr20210320_py2-1.6.0/alibabacloud_emr20210320_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-emr20210320-py2
-Version: 1.5.0
+Version: 1.6.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320_py2-1.5.0/setup.py` & `alibabacloud_emr20210320_py2-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr20210320_py2.
 
-Created on 17/04/2024
+Created on 19/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr20210320"
 NAME = "alibabacloud_emr20210320_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Emr (20210320) SDK Library for Python2"
```

