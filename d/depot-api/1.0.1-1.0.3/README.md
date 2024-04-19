# Comparing `tmp/depot_api-1.0.1.tar.gz` & `tmp/depot_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depot_api-1.0.1.tar", last modified: Thu Apr 18 11:33:21 2024, max compression
+gzip compressed data, was "depot_api-1.0.3.tar", last modified: Fri Apr 19 07:14:04 2024, max compression
```

## Comparing `depot_api-1.0.1.tar` & `depot_api-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,43 @@
--rw-r--r--   0        0        0     5827 2024-04-18 08:54:32.210134 depot_api-1.0.1/README.md
--rw-r--r--   0        0        0     1483 2024-04-18 08:54:32.220430 depot_api-1.0.1/depot_api/__init__.py
--rw-r--r--   0        0        0       97 2024-04-18 08:54:32.221882 depot_api-1.0.1/depot_api/api/__init__.py
--rw-r--r--   0        0        0   176880 2024-04-18 08:54:32.202505 depot_api-1.0.1/depot_api/api/default_api.py
--rw-r--r--   0        0        0    25761 2024-04-18 08:54:32.224958 depot_api-1.0.1/depot_api/api_client.py
--rw-r--r--   0        0        0      652 2024-04-18 08:54:32.225447 depot_api-1.0.1/depot_api/api_response.py
--rw-r--r--   0        0        0    14459 2024-04-18 08:54:32.219724 depot_api-1.0.1/depot_api/configuration.py
--rw-r--r--   0        0        0     5972 2024-04-18 08:54:32.222702 depot_api-1.0.1/depot_api/exceptions.py
--rw-r--r--   0        0        0      935 2024-04-18 08:54:32.221477 depot_api-1.0.1/depot_api/models/__init__.py
--rw-r--r--   0        0        0     3049 2024-04-15 14:00:46.761397 depot_api-1.0.1/depot_api/models/cluster.py
--rw-r--r--   0        0        0     2716 2024-04-18 08:54:32.030479 depot_api-1.0.1/depot_api/models/cluster_in.py
--rw-r--r--   0        0        0     2978 2024-04-18 08:54:32.043662 depot_api-1.0.1/depot_api/models/http_validation_error.py
--rw-r--r--   0        0        0     4801 2024-04-18 08:54:32.093363 depot_api-1.0.1/depot_api/models/id.py
--rw-r--r--   0        0        0     3427 2024-04-18 08:54:32.098926 depot_api-1.0.1/depot_api/models/job_instance.py
--rw-r--r--   0        0        0     2948 2024-04-18 08:54:32.108502 depot_api-1.0.1/depot_api/models/job_instance_in.py
--rw-r--r--   0        0        0     3056 2024-04-18 08:54:32.116591 depot_api-1.0.1/depot_api/models/provider.py
--rw-r--r--   0        0        0     2988 2024-04-18 08:54:32.122496 depot_api-1.0.1/depot_api/models/repository.py
--rw-r--r--   0        0        0     3199 2024-04-18 08:54:32.125437 depot_api-1.0.1/depot_api/models/repository_out.py
--rw-r--r--   0        0        0     3079 2024-04-18 08:54:32.128734 depot_api-1.0.1/depot_api/models/validation_error.py
--rw-r--r--   0        0        0     4901 2024-04-18 08:54:32.132441 depot_api-1.0.1/depot_api/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0        0 2024-04-18 08:54:32.218006 depot_api-1.0.1/depot_api/py.typed
--rw-r--r--   0        0        0     9227 2024-04-18 08:54:32.226776 depot_api-1.0.1/depot_api/rest.py
--rw-r--r--   0        0        0     1947 2024-04-18 11:33:21.163305 depot_api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 08:54:32.223236 depot_api-1.0.1/test/__init__.py
--rw-r--r--   0        0        0     1509 2024-04-15 14:00:46.763230 depot_api-1.0.1/test/test_cluster.py
--rw-r--r--   0        0        0     1685 2024-04-16 05:26:03.952432 depot_api-1.0.1/test/test_cluster_in.py
--rw-r--r--   0        0        0     3543 2024-04-15 14:00:46.839817 depot_api-1.0.1/test/test_default_api.py
--rw-r--r--   0        0        0     1698 2024-04-15 14:00:46.769812 depot_api-1.0.1/test/test_http_validation_error.py
--rw-r--r--   0        0        0     1203 2024-04-15 14:00:46.780645 depot_api-1.0.1/test/test_id.py
--rw-r--r--   0        0        0     1663 2024-04-15 14:00:46.785728 depot_api-1.0.1/test/test_job_instance.py
--rw-r--r--   0        0        0     1732 2024-04-18 06:49:32.731307 depot_api-1.0.1/test/test_job_instance_in.py
--rw-r--r--   0        0        0     1526 2024-04-15 14:00:46.790366 depot_api-1.0.1/test/test_provider.py
--rw-r--r--   0        0        0     1569 2024-04-15 14:00:46.793463 depot_api-1.0.1/test/test_repository.py
--rw-r--r--   0        0        0     2371 2024-04-15 14:00:46.796985 depot_api-1.0.1/test/test_repository_out.py
--rw-r--r--   0        0        0     1609 2024-04-15 14:00:46.800103 depot_api-1.0.1/test/test_validation_error.py
--rw-r--r--   0        0        0     1458 2024-04-15 14:00:46.802999 depot_api-1.0.1/test/test_validation_error_loc_inner.py
--rw-r--r--   0        0        0     6596 1970-01-01 00:00:00.000000 depot_api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5878 2024-04-18 20:09:02.598312 depot_api-1.0.3/README.md
+-rw-r--r--   0        0        0     1474 2024-04-18 20:09:02.613539 depot_api-1.0.3/depot_api/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-18 20:09:02.616145 depot_api-1.0.3/depot_api/api/__init__.py
+-rw-r--r--   0        0        0   159078 2024-04-18 20:09:02.589955 depot_api-1.0.3/depot_api/api/default_api.py
+-rw-r--r--   0        0        0    25761 2024-04-18 20:09:02.620663 depot_api-1.0.3/depot_api/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-18 20:09:02.621487 depot_api-1.0.3/depot_api/api_response.py
+-rw-r--r--   0        0        0    14735 2024-04-18 20:09:02.612579 depot_api-1.0.3/depot_api/configuration.py
+-rw-r--r--   0        0        0     5972 2024-04-18 20:09:02.616813 depot_api-1.0.3/depot_api/exceptions.py
+-rw-r--r--   0        0        0      926 2024-04-18 20:09:02.615375 depot_api-1.0.3/depot_api/models/__init__.py
+-rw-r--r--   0        0        0     4826 2024-04-18 20:09:02.452513 depot_api-1.0.3/depot_api/models/client_id.py
+-rw-r--r--   0        0        0     4850 2024-04-18 20:09:02.465267 depot_api-1.0.3/depot_api/models/client_secret.py
+-rw-r--r--   0        0        0     3049 2024-04-15 14:00:46.761397 depot_api-1.0.3/depot_api/models/cluster.py
+-rw-r--r--   0        0        0     2716 2024-04-18 20:09:02.472913 depot_api-1.0.3/depot_api/models/cluster_in.py
+-rw-r--r--   0        0        0     4897 2024-04-18 20:09:02.477071 depot_api-1.0.3/depot_api/models/grant_type.py
+-rw-r--r--   0        0        0     2978 2024-04-18 20:09:02.482914 depot_api-1.0.3/depot_api/models/http_validation_error.py
+-rw-r--r--   0        0        0     4801 2024-04-18 20:09:02.487509 depot_api-1.0.3/depot_api/models/id.py
+-rw-r--r--   0        0        0     3427 2024-04-18 08:54:32.098926 depot_api-1.0.3/depot_api/models/job_instance.py
+-rw-r--r--   0        0        0     2948 2024-04-18 20:09:02.492062 depot_api-1.0.3/depot_api/models/job_instance_in.py
+-rw-r--r--   0        0        0     3056 2024-04-18 20:09:02.496032 depot_api-1.0.3/depot_api/models/provider.py
+-rw-r--r--   0        0        0     2988 2024-04-18 08:54:32.122496 depot_api-1.0.3/depot_api/models/repository.py
+-rw-r--r--   0        0        0     3199 2024-04-18 08:54:32.125437 depot_api-1.0.3/depot_api/models/repository_out.py
+-rw-r--r--   0        0        0     3079 2024-04-18 20:09:02.500051 depot_api-1.0.3/depot_api/models/validation_error.py
+-rw-r--r--   0        0        0     4901 2024-04-18 20:09:02.503214 depot_api-1.0.3/depot_api/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:09:02.610764 depot_api-1.0.3/depot_api/py.typed
+-rw-r--r--   0        0        0     9227 2024-04-18 20:09:02.623931 depot_api-1.0.3/depot_api/rest.py
+-rw-r--r--   0        0        0     1868 2024-04-19 07:14:04.643959 depot_api-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 20:09:02.617148 depot_api-1.0.3/test/__init__.py
+-rw-r--r--   0        0        0     1276 2024-04-18 20:09:02.454188 depot_api-1.0.3/test/test_client_id.py
+-rw-r--r--   0        0        0     1324 2024-04-18 20:09:02.466568 depot_api-1.0.3/test/test_client_secret.py
+-rw-r--r--   0        0        0     1509 2024-04-15 14:00:46.763230 depot_api-1.0.3/test/test_cluster.py
+-rw-r--r--   0        0        0     1685 2024-04-16 05:26:03.952432 depot_api-1.0.3/test/test_cluster_in.py
+-rw-r--r--   0        0        0     3543 2024-04-15 14:00:46.839817 depot_api-1.0.3/test/test_default_api.py
+-rw-r--r--   0        0        0     1288 2024-04-18 20:09:02.478374 depot_api-1.0.3/test/test_grant_type.py
+-rw-r--r--   0        0        0     1698 2024-04-15 14:00:46.769812 depot_api-1.0.3/test/test_http_validation_error.py
+-rw-r--r--   0        0        0     1203 2024-04-15 14:00:46.780645 depot_api-1.0.3/test/test_id.py
+-rw-r--r--   0        0        0     1663 2024-04-15 14:00:46.785728 depot_api-1.0.3/test/test_job_instance.py
+-rw-r--r--   0        0        0     1732 2024-04-18 06:49:32.731307 depot_api-1.0.3/test/test_job_instance_in.py
+-rw-r--r--   0        0        0     1526 2024-04-15 14:00:46.790366 depot_api-1.0.3/test/test_provider.py
+-rw-r--r--   0        0        0     1569 2024-04-15 14:00:46.793463 depot_api-1.0.3/test/test_repository.py
+-rw-r--r--   0        0        0     2371 2024-04-15 14:00:46.796985 depot_api-1.0.3/test/test_repository_out.py
+-rw-r--r--   0        0        0     1609 2024-04-15 14:00:46.800103 depot_api-1.0.3/test/test_validation_error.py
+-rw-r--r--   0        0        0     1458 2024-04-15 14:00:46.802999 depot_api-1.0.3/test/test_validation_error_loc_inner.py
+-rw-r--r--   0        0        0     6594 1970-01-01 00:00:00.000000 depot_api-1.0.3/PKG-INFO
```

### Comparing `depot_api-1.0.1/README.md` & `depot_api-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,20 @@
 
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = depot_api.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+configuration.access_token = os.environ["ACCESS_TOKEN"]
 
 
 # Enter a context with an instance of the API client
 with depot_api.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = depot_api.DefaultApi(api_client)
     cluster_in = depot_api.ClusterIn() # ClusterIn | 
@@ -84,49 +90,55 @@
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**create_cluster_clusters_post**](docs/DefaultApi.md#create_cluster_clusters_post) | **POST** /clusters/ | Create Cluster
 *DefaultApi* | [**create_job_instance_job_instances_post**](docs/DefaultApi.md#create_job_instance_job_instances_post) | **POST** /job_instances/ | Create Job Instance
 *DefaultApi* | [**create_provider_providers_post**](docs/DefaultApi.md#create_provider_providers_post) | **POST** /providers/ | Create Provider
-*DefaultApi* | [**create_repository_repositories_post**](docs/DefaultApi.md#create_repository_repositories_post) | **POST** /repositories/ | Create Repository
 *DefaultApi* | [**delete_cluster_clusters_cluster_id_delete**](docs/DefaultApi.md#delete_cluster_clusters_cluster_id_delete) | **DELETE** /clusters/{cluster_id} | Delete Cluster
 *DefaultApi* | [**delete_job_instance_job_instances_job_instance_id_delete**](docs/DefaultApi.md#delete_job_instance_job_instances_job_instance_id_delete) | **DELETE** /job_instances/{job_instance_id} | Delete Job Instance
 *DefaultApi* | [**delete_provider_providers_provider_id_delete**](docs/DefaultApi.md#delete_provider_providers_provider_id_delete) | **DELETE** /providers/{provider_id} | Delete Provider
 *DefaultApi* | [**list_clusters_clusters_get**](docs/DefaultApi.md#list_clusters_clusters_get) | **GET** /clusters/ | List Clusters
 *DefaultApi* | [**list_job_instances_job_instances_get**](docs/DefaultApi.md#list_job_instances_job_instances_get) | **GET** /job_instances/ | List Job Instances
 *DefaultApi* | [**list_providers_providers_get**](docs/DefaultApi.md#list_providers_providers_get) | **GET** /providers/ | List Providers
 *DefaultApi* | [**list_providers_types_provider_types_get**](docs/DefaultApi.md#list_providers_types_provider_types_get) | **GET** /provider_types/ | List Providers Types
-*DefaultApi* | [**list_repositories_repositories_get**](docs/DefaultApi.md#list_repositories_repositories_get) | **GET** /repositories/ | List Repositories
-*DefaultApi* | [**login_login_post**](docs/DefaultApi.md#login_login_post) | **POST** /login/ | Login
+*DefaultApi* | [**login_token_post**](docs/DefaultApi.md#login_token_post) | **POST** /token | Login
 *DefaultApi* | [**read_cluster_clusters_cluster_id_get**](docs/DefaultApi.md#read_cluster_clusters_cluster_id_get) | **GET** /clusters/{cluster_id} | Read Cluster
 *DefaultApi* | [**read_job_instance_job_instances_job_instance_id_get**](docs/DefaultApi.md#read_job_instance_job_instances_job_instance_id_get) | **GET** /job_instances/{job_instance_id} | Read Job Instance
 *DefaultApi* | [**read_log_logs_job_instance_id_get**](docs/DefaultApi.md#read_log_logs_job_instance_id_get) | **GET** /logs/{job_instance_id} | Read Log
 *DefaultApi* | [**read_provider_providers_provider_id_get**](docs/DefaultApi.md#read_provider_providers_provider_id_get) | **GET** /providers/{provider_id} | Read Provider
-*DefaultApi* | [**read_repository_repositories_repository_id_get**](docs/DefaultApi.md#read_repository_repositories_repository_id_get) | **GET** /repositories/{repository_id} | Read Repository
+*DefaultApi* | [**read_users_me_users_me_get**](docs/DefaultApi.md#read_users_me_users_me_get) | **GET** /users/me | Read Users Me
 
 
 ## Documentation For Models
 
+ - [ClientId](docs/ClientId.md)
+ - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
+ - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [Id](docs/Id.md)
- - [JobInstance](docs/JobInstance.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
  - [Provider](docs/Provider.md)
- - [Repository](docs/Repository.md)
- - [RepositoryOut](docs/RepositoryOut.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
-Endpoints do not require authorization.
+
+Authentication schemes defined for the API:
+<a id="OAuth2PasswordBearer"></a>
+### OAuth2PasswordBearer
+
+- **Type**: OAuth
+- **Flow**: password
+- **Authorization URL**: 
+- **Scopes**: N/A
 
 
 ## Author
```

### Comparing `depot_api-1.0.1/depot_api/__init__.py` & `depot_api-1.0.3/depot_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from depot_api.exceptions import ApiTypeError
 from depot_api.exceptions import ApiValueError
 from depot_api.exceptions import ApiKeyError
 from depot_api.exceptions import ApiAttributeError
 from depot_api.exceptions import ApiException
 
 # import models into sdk package
+from depot_api.models.client_id import ClientId
+from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
+from depot_api.models.grant_type import GrantType
 from depot_api.models.http_validation_error import HTTPValidationError
 from depot_api.models.id import Id
-from depot_api.models.job_instance import JobInstance
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.provider import Provider
-from depot_api.models.repository import Repository
-from depot_api.models.repository_out import RepositoryOut
 from depot_api.models.validation_error import ValidationError
 from depot_api.models.validation_error_loc_inner import ValidationErrorLocInner
```

### Comparing `depot_api-1.0.1/depot_api/api/default_api.py` & `depot_api-1.0.3/depot_api/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictInt, StrictStr
-from typing import Any, Optional
+from typing import Optional
+from depot_api.models.client_id import ClientId
+from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
+from depot_api.models.grant_type import GrantType
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.provider import Provider
-from depot_api.models.repository import Repository
-from depot_api.models.repository_out import RepositoryOut
 
 from depot_api.api_client import ApiClient, RequestSerialized
 from depot_api.api_response import ApiResponse
 from depot_api.rest import RESTResponseType
 
 
 class DefaultApi:
@@ -288,14 +289,15 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/clusters/',
             path_params=_path_params,
             query_params=_query_params,
@@ -558,14 +560,15 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/job_instances/',
             path_params=_path_params,
             query_params=_query_params,
@@ -828,14 +831,15 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/providers/',
             path_params=_path_params,
             query_params=_query_params,
@@ -849,284 +853,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_repository_repositories_post(
-        self,
-        repository: Repository,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RepositoryOut:
-        """Create Repository
-
-
-        :param repository: (required)
-        :type repository: Repository
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._create_repository_repositories_post_serialize(
-            repository=repository,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RepositoryOut",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def create_repository_repositories_post_with_http_info(
-        self,
-        repository: Repository,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[RepositoryOut]:
-        """Create Repository
-
-
-        :param repository: (required)
-        :type repository: Repository
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._create_repository_repositories_post_serialize(
-            repository=repository,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RepositoryOut",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def create_repository_repositories_post_without_preload_content(
-        self,
-        repository: Repository,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Create Repository
-
-
-        :param repository: (required)
-        :type repository: Repository
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._create_repository_repositories_post_serialize(
-            repository=repository,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RepositoryOut",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _create_repository_repositories_post_serialize(
-        self,
-        repository,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-        if repository is not None:
-            _body_params = repository
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
-
-        # authentication setting
-        _auth_settings: List[str] = [
-        ]
-
-        return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/repositories/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def delete_cluster_clusters_cluster_id_delete(
         self,
         cluster_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -1355,14 +1089,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/clusters/{cluster_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -1612,14 +1347,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/job_instances/{job_instance_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -1869,14 +1605,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/providers/{provider_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -2108,14 +1845,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/clusters/',
             path_params=_path_params,
             query_params=_query_params,
@@ -2347,14 +2085,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/job_instances/',
             path_params=_path_params,
             query_params=_query_params,
@@ -2586,14 +2325,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/providers/',
             path_params=_path_params,
             query_params=_query_params,
@@ -2825,14 +2565,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/provider_types/',
             path_params=_path_params,
             query_params=_query_params,
@@ -2846,277 +2587,22 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_repositories_repositories_get(
-        self,
-        response_model: Optional[Any] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """List Repositories
-
-
-        :param response_model:
-        :type response_model: object
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._list_repositories_repositories_get_serialize(
-            response_model=response_model,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def list_repositories_repositories_get_with_http_info(
-        self,
-        response_model: Optional[Any] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """List Repositories
-
-
-        :param response_model:
-        :type response_model: object
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._list_repositories_repositories_get_serialize(
-            response_model=response_model,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def list_repositories_repositories_get_without_preload_content(
-        self,
-        response_model: Optional[Any] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """List Repositories
-
-
-        :param response_model:
-        :type response_model: object
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._list_repositories_repositories_get_serialize(
-            response_model=response_model,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _list_repositories_repositories_get_serialize(
-        self,
-        response_model,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if response_model is not None:
-            
-            _query_params.append(('response_model', response_model))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/repositories/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def login_login_post(
+    def login_token_post(
         self,
         username: StrictStr,
         password: StrictStr,
+        grant_type: Optional[GrantType] = None,
+        scope: Optional[StrictStr] = None,
+        client_id: Optional[ClientId] = None,
+        client_secret: Optional[ClientSecret] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3129,14 +2615,22 @@
         """Login
 
 
         :param username: (required)
         :type username: str
         :param password: (required)
         :type password: str
+        :param grant_type:
+        :type grant_type: GrantType
+        :param scope:
+        :type scope: str
+        :param client_id:
+        :type client_id: ClientId
+        :param client_secret:
+        :type client_secret: ClientSecret
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3151,17 +2645,21 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._login_login_post_serialize(
+        _param = self._login_token_post_serialize(
             username=username,
             password=password,
+            grant_type=grant_type,
+            scope=scope,
+            client_id=client_id,
+            client_secret=client_secret,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3176,18 +2674,22 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def login_login_post_with_http_info(
+    def login_token_post_with_http_info(
         self,
         username: StrictStr,
         password: StrictStr,
+        grant_type: Optional[GrantType] = None,
+        scope: Optional[StrictStr] = None,
+        client_id: Optional[ClientId] = None,
+        client_secret: Optional[ClientSecret] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3200,14 +2702,22 @@
         """Login
 
 
         :param username: (required)
         :type username: str
         :param password: (required)
         :type password: str
+        :param grant_type:
+        :type grant_type: GrantType
+        :param scope:
+        :type scope: str
+        :param client_id:
+        :type client_id: ClientId
+        :param client_secret:
+        :type client_secret: ClientSecret
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3222,17 +2732,21 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._login_login_post_serialize(
+        _param = self._login_token_post_serialize(
             username=username,
             password=password,
+            grant_type=grant_type,
+            scope=scope,
+            client_id=client_id,
+            client_secret=client_secret,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3247,18 +2761,22 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def login_login_post_without_preload_content(
+    def login_token_post_without_preload_content(
         self,
         username: StrictStr,
         password: StrictStr,
+        grant_type: Optional[GrantType] = None,
+        scope: Optional[StrictStr] = None,
+        client_id: Optional[ClientId] = None,
+        client_secret: Optional[ClientSecret] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3271,14 +2789,22 @@
         """Login
 
 
         :param username: (required)
         :type username: str
         :param password: (required)
         :type password: str
+        :param grant_type:
+        :type grant_type: GrantType
+        :param scope:
+        :type scope: str
+        :param client_id:
+        :type client_id: ClientId
+        :param client_secret:
+        :type client_secret: ClientSecret
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3293,17 +2819,21 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._login_login_post_serialize(
+        _param = self._login_token_post_serialize(
             username=username,
             password=password,
+            grant_type=grant_type,
+            scope=scope,
+            client_id=client_id,
+            client_secret=client_secret,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3313,18 +2843,22 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _login_login_post_serialize(
+    def _login_token_post_serialize(
         self,
         username,
         password,
+        grant_type,
+        scope,
+        client_id,
+        client_secret,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3337,42 +2871,59 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if username is not None:
-            
-            _query_params.append(('username', username))
-            
-        if password is not None:
-            
-            _query_params.append(('password', password))
-            
         # process the header parameters
         # process the form parameters
+        if grant_type is not None:
+            _form_params.append(('grant_type', grant_type))
+        if username is not None:
+            _form_params.append(('username', username))
+        if password is not None:
+            _form_params.append(('password', password))
+        if scope is not None:
+            _form_params.append(('scope', scope))
+        if client_id is not None:
+            _form_params.append(('client_id', client_id))
+        if client_secret is not None:
+            _form_params.append(('client_secret', client_secret))
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/x-www-form-urlencoded'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/login/',
+            resource_path='/token',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3617,14 +3168,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/clusters/{cluster_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -3874,14 +3426,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/job_instances/{job_instance_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -4131,14 +3684,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/logs/{job_instance_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -4388,14 +3942,15 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/providers/{provider_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -4409,35 +3964,32 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def read_repository_repositories_repository_id_get(
+    def read_users_me_users_me_get(
         self,
-        repository_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RepositoryOut:
-        """Read Repository
+    ) -> object:
+        """Read Users Me
 
 
-        :param repository_id: (required)
-        :type repository_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4452,59 +4004,54 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._read_repository_repositories_repository_id_get_serialize(
-            repository_id=repository_id,
+        _param = self._read_users_me_users_me_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RepositoryOut",
-            '422': "HTTPValidationError",
+            '200': "object",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def read_repository_repositories_repository_id_get_with_http_info(
+    def read_users_me_users_me_get_with_http_info(
         self,
-        repository_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[RepositoryOut]:
-        """Read Repository
+    ) -> ApiResponse[object]:
+        """Read Users Me
 
 
-        :param repository_id: (required)
-        :type repository_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4519,59 +4066,54 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._read_repository_repositories_repository_id_get_serialize(
-            repository_id=repository_id,
+        _param = self._read_users_me_users_me_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RepositoryOut",
-            '422': "HTTPValidationError",
+            '200': "object",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def read_repository_repositories_repository_id_get_without_preload_content(
+    def read_users_me_users_me_get_without_preload_content(
         self,
-        repository_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Read Repository
+        """Read Users Me
 
 
-        :param repository_id: (required)
-        :type repository_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4586,36 +4128,33 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._read_repository_repositories_repository_id_get_serialize(
-            repository_id=repository_id,
+        _param = self._read_users_me_users_me_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RepositoryOut",
-            '422': "HTTPValidationError",
+            '200': "object",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _read_repository_repositories_repository_id_get_serialize(
+    def _read_users_me_users_me_get_serialize(
         self,
-        repository_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -4627,16 +4166,14 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if repository_id is not None:
-            _path_params['repository_id'] = repository_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -4645,19 +4182,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'OAuth2PasswordBearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/repositories/{repository_id}',
+            resource_path='/users/me',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `depot_api-1.0.1/depot_api/api_client.py` & `depot_api-1.0.3/depot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/api_response.py` & `depot_api-1.0.3/depot_api/api_response.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/configuration.py` & `depot_api-1.0.3/depot_api/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum
       values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
+    :Example:
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -355,14 +356,21 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if self.access_token is not None:
+            auth['OAuth2PasswordBearer'] = {
+                'type': 'oauth2',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
+            }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
```

### Comparing `depot_api-1.0.1/depot_api/exceptions.py` & `depot_api-1.0.3/depot_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/__init__.py` & `depot_api-1.0.3/depot_api/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
+from depot_api.models.client_id import ClientId
+from depot_api.models.client_secret import ClientSecret
 from depot_api.models.cluster_in import ClusterIn
+from depot_api.models.grant_type import GrantType
 from depot_api.models.http_validation_error import HTTPValidationError
 from depot_api.models.id import Id
-from depot_api.models.job_instance import JobInstance
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.provider import Provider
-from depot_api.models.repository import Repository
-from depot_api.models.repository_out import RepositoryOut
 from depot_api.models.validation_error import ValidationError
 from depot_api.models.validation_error_loc_inner import ValidationErrorLocInner
```

### Comparing `depot_api-1.0.1/depot_api/models/cluster.py` & `depot_api-1.0.3/depot_api/models/cluster.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/cluster_in.py` & `depot_api-1.0.3/depot_api/models/cluster_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/http_validation_error.py` & `depot_api-1.0.3/depot_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/id.py` & `depot_api-1.0.3/depot_api/models/id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/job_instance.py` & `depot_api-1.0.3/depot_api/models/job_instance.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/job_instance_in.py` & `depot_api-1.0.3/depot_api/models/job_instance_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/provider.py` & `depot_api-1.0.3/depot_api/models/provider.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/repository.py` & `depot_api-1.0.3/depot_api/models/repository.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/repository_out.py` & `depot_api-1.0.3/depot_api/models/repository_out.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/validation_error.py` & `depot_api-1.0.3/depot_api/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/models/validation_error_loc_inner.py` & `depot_api-1.0.3/depot_api/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/depot_api/rest.py` & `depot_api-1.0.3/depot_api/rest.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/pyproject.toml` & `depot_api-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -56,30 +56,29 @@
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 authors = [
     { name = "OpenAPI Generator Community", email = "team@openapitools.org" },
-    { name = "OpenAPI Generator community", email = "team@openapitools.org" },
     { name = "CodeDepot Team", email = "contact@codedepot.ai" },
 ]
 requires-python = "<4.0,>=3.7"
 dependencies = [
     "urllib3>=1.25.3",
     "python-dateutil>=2.8.2",
     "pydantic>=2",
     "typing-extensions>=4.7.1",
     "pydantic >= 2",
     "python-dateutil",
     "typing-extensions >= 4.7.1",
     "urllib3 >= 1.25.3, < 2.1.0",
 ]
 name = "depot-api"
-version = "1.0.1"
+version = "1.0.3"
 description = "FastAPI client for the Depot API"
 readme = "README.md"
 keywords = [
     "OpenAPI",
     "OpenAPI-Generator",
     "FastAPI",
 ]
```

### Comparing `depot_api-1.0.1/test/test_cluster.py` & `depot_api-1.0.3/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_cluster_in.py` & `depot_api-1.0.3/test/test_cluster_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_default_api.py` & `depot_api-1.0.3/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_http_validation_error.py` & `depot_api-1.0.3/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_id.py` & `depot_api-1.0.3/test/test_id.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_job_instance.py` & `depot_api-1.0.3/test/test_job_instance.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_job_instance_in.py` & `depot_api-1.0.3/test/test_job_instance_in.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_provider.py` & `depot_api-1.0.3/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_repository.py` & `depot_api-1.0.3/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_repository_out.py` & `depot_api-1.0.3/test/test_repository_out.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_validation_error.py` & `depot_api-1.0.3/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/test/test_validation_error_loc_inner.py` & `depot_api-1.0.3/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `depot_api-1.0.1/PKG-INFO` & `depot_api-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depot-api
-Version: 1.0.1
+Version: 1.0.3
 Summary: FastAPI client for the Depot API
 Keywords: OpenAPI,OpenAPI-Generator,FastAPI
-Author-Email: OpenAPI Generator Community <team@openapitools.org>, OpenAPI Generator community <team@openapitools.org>, CodeDepot Team <contact@codedepot.ai>
+Author-Email: OpenAPI Generator Community <team@openapitools.org>, CodeDepot Team <contact@codedepot.ai>
 License: NoLicense
 Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
 Project-URL: Homepage, https://codedepot.ai
 Requires-Python: <4.0,>=3.7
 Requires-Dist: urllib3>=1.25.3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pydantic>=2
@@ -77,14 +77,20 @@
 
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = depot_api.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+configuration.access_token = os.environ["ACCESS_TOKEN"]
 
 
 # Enter a context with an instance of the API client
 with depot_api.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = depot_api.DefaultApi(api_client)
     cluster_in = depot_api.ClusterIn() # ClusterIn | 
@@ -104,49 +110,55 @@
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**create_cluster_clusters_post**](docs/DefaultApi.md#create_cluster_clusters_post) | **POST** /clusters/ | Create Cluster
 *DefaultApi* | [**create_job_instance_job_instances_post**](docs/DefaultApi.md#create_job_instance_job_instances_post) | **POST** /job_instances/ | Create Job Instance
 *DefaultApi* | [**create_provider_providers_post**](docs/DefaultApi.md#create_provider_providers_post) | **POST** /providers/ | Create Provider
-*DefaultApi* | [**create_repository_repositories_post**](docs/DefaultApi.md#create_repository_repositories_post) | **POST** /repositories/ | Create Repository
 *DefaultApi* | [**delete_cluster_clusters_cluster_id_delete**](docs/DefaultApi.md#delete_cluster_clusters_cluster_id_delete) | **DELETE** /clusters/{cluster_id} | Delete Cluster
 *DefaultApi* | [**delete_job_instance_job_instances_job_instance_id_delete**](docs/DefaultApi.md#delete_job_instance_job_instances_job_instance_id_delete) | **DELETE** /job_instances/{job_instance_id} | Delete Job Instance
 *DefaultApi* | [**delete_provider_providers_provider_id_delete**](docs/DefaultApi.md#delete_provider_providers_provider_id_delete) | **DELETE** /providers/{provider_id} | Delete Provider
 *DefaultApi* | [**list_clusters_clusters_get**](docs/DefaultApi.md#list_clusters_clusters_get) | **GET** /clusters/ | List Clusters
 *DefaultApi* | [**list_job_instances_job_instances_get**](docs/DefaultApi.md#list_job_instances_job_instances_get) | **GET** /job_instances/ | List Job Instances
 *DefaultApi* | [**list_providers_providers_get**](docs/DefaultApi.md#list_providers_providers_get) | **GET** /providers/ | List Providers
 *DefaultApi* | [**list_providers_types_provider_types_get**](docs/DefaultApi.md#list_providers_types_provider_types_get) | **GET** /provider_types/ | List Providers Types
-*DefaultApi* | [**list_repositories_repositories_get**](docs/DefaultApi.md#list_repositories_repositories_get) | **GET** /repositories/ | List Repositories
-*DefaultApi* | [**login_login_post**](docs/DefaultApi.md#login_login_post) | **POST** /login/ | Login
+*DefaultApi* | [**login_token_post**](docs/DefaultApi.md#login_token_post) | **POST** /token | Login
 *DefaultApi* | [**read_cluster_clusters_cluster_id_get**](docs/DefaultApi.md#read_cluster_clusters_cluster_id_get) | **GET** /clusters/{cluster_id} | Read Cluster
 *DefaultApi* | [**read_job_instance_job_instances_job_instance_id_get**](docs/DefaultApi.md#read_job_instance_job_instances_job_instance_id_get) | **GET** /job_instances/{job_instance_id} | Read Job Instance
 *DefaultApi* | [**read_log_logs_job_instance_id_get**](docs/DefaultApi.md#read_log_logs_job_instance_id_get) | **GET** /logs/{job_instance_id} | Read Log
 *DefaultApi* | [**read_provider_providers_provider_id_get**](docs/DefaultApi.md#read_provider_providers_provider_id_get) | **GET** /providers/{provider_id} | Read Provider
-*DefaultApi* | [**read_repository_repositories_repository_id_get**](docs/DefaultApi.md#read_repository_repositories_repository_id_get) | **GET** /repositories/{repository_id} | Read Repository
+*DefaultApi* | [**read_users_me_users_me_get**](docs/DefaultApi.md#read_users_me_users_me_get) | **GET** /users/me | Read Users Me
 
 
 ## Documentation For Models
 
+ - [ClientId](docs/ClientId.md)
+ - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
+ - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [Id](docs/Id.md)
- - [JobInstance](docs/JobInstance.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
  - [Provider](docs/Provider.md)
- - [Repository](docs/Repository.md)
- - [RepositoryOut](docs/RepositoryOut.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
-Endpoints do not require authorization.
+
+Authentication schemes defined for the API:
+<a id="OAuth2PasswordBearer"></a>
+### OAuth2PasswordBearer
+
+- **Type**: OAuth
+- **Flow**: password
+- **Authorization URL**: 
+- **Scopes**: N/A
 
 
 ## Author
```

