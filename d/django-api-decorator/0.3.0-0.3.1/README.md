# Comparing `tmp/django_api_decorator-0.3.0.tar.gz` & `tmp/django_api_decorator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_api_decorator-0.3.0.tar", max compression
+gzip compressed data, was "django_api_decorator-0.3.1.tar", max compression
```

## Comparing `django_api_decorator-0.3.0.tar` & `django_api_decorator-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-11-21 11:37:07.144324 django_api_decorator-0.3.0/LICENSE
--rw-r--r--   0        0        0     2697 2023-11-21 11:37:07.144324 django_api_decorator-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-11-21 11:37:07.144324 django_api_decorator-0.3.0/django_api_decorator/__init__.py
--rw-r--r--   0        0        0      390 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/apps.py
--rw-r--r--   0        0        0    12466 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/decorators.py
--rw-r--r--   0        0        0        0 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/management/commands/generate_api_schemas.py
--rw-r--r--   0        0        0     9675 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/openapi.py
--rw-r--r--   0        0        0        0 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/py.typed
--rw-r--r--   0        0        0     1552 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/schema_file.py
--rw-r--r--   0        0        0     1037 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/types.py
--rw-r--r--   0        0        0     1993 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/django_api_decorator/utils.py
--rw-r--r--   0        0        0     1072 2023-11-21 11:37:07.148324 django_api_decorator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 django_api_decorator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2697 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/__init__.py
+-rw-r--r--   0        0        0      390 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/apps.py
+-rw-r--r--   0        0        0    12735 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/decorators.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/management/commands/generate_api_schemas.py
+-rw-r--r--   0        0        0     9675 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/openapi.py
+-rw-r--r--   0        0        0        0 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/py.typed
+-rw-r--r--   0        0        0     1552 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/schema_file.py
+-rw-r--r--   0        0        0     1037 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/types.py
+-rw-r--r--   0        0        0     1993 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/django_api_decorator/utils.py
+-rw-r--r--   0        0        0     1077 2024-04-19 09:33:50.529211 django_api_decorator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 django_api_decorator-0.3.1/PKG-INFO
```

### Comparing `django_api_decorator-0.3.0/LICENSE` & `django_api_decorator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/README.md` & `django_api_decorator-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/django_api_decorator/decorators.py` & `django_api_decorator-0.3.1/django_api_decorator/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 
 from .types import ApiMeta, FieldError, PublicAPIError
 
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 Annotation = Any
+ExceptionHandler = Callable[
+    [HttpRequest, ValidationError | pydantic.ValidationError], HttpResponse
+]
 
 
 def api(
     *,
     method: str,
     query_params: list[str] | None = None,
     login_required: bool | None = None,
     response_status: int = 200,
     atomic: bool | None = None,
     auth_check: Callable[[HttpRequest], bool] | None = None,
     serialize_by_alias: bool = False,
+    validation_error_handler: ExceptionHandler | None = None,
 ) -> Callable[[Callable[P, T]], Callable[P, HttpResponse]]:
     """
     Defines an API view. This handles validation of query parameters, parsing of
     the request body, access control, and serialization of the response payload.
 
     * query_params:
         This is a list of the function parameters that should be
@@ -71,14 +75,15 @@
         else getattr(settings, "API_DECORATOR_DEFAULT_LOGIN_REQUIRED", True)
     )
     atomic = (
         atomic
         if atomic is not None
         else getattr(settings, "API_DECORATOR_DEFAULT_ATOMIC", True)
     )
+    validation_error_handler = validation_error_handler or handle_validation_error
 
     def default_auth_check(request: HttpRequest) -> bool:
         return hasattr(request, "user") and request.user.is_authenticated
 
     _auth_check = (
         auth_check
         if auth_check is not None
@@ -134,15 +139,15 @@
                 query_params = query_params_model.model_validate(raw_query_params)
                 extra_kwargs.update(query_params.model_dump(exclude_defaults=True))
             except (
                 ValidationError,
                 pydantic.ValidationError,
             ) as e:
                 # Normalize and return a unified error message payload
-                return handle_validation_error(exception=e)
+                return validation_error_handler(request, e)
 
             try:
                 if atomic:
                     with transaction.atomic():
                         response = func(request, *args, **kwargs, **extra_kwargs)
                 else:
                     response = func(request, *args, **kwargs, **extra_kwargs)
@@ -151,15 +156,15 @@
                 return JsonResponse(
                     {"errors": ["The resource you tried to access does not exist"]},
                     status=404,
                 )
             except ValidationError as e:
                 # Normalize and return a unified error message payload, but only
                 # for Django's ValidationError error, not DRF or Pydantic
-                return handle_validation_error(exception=e)
+                return validation_error_handler(request, e)
 
             except PublicAPIError as exc:
                 # Raised custom errors to frontend
                 return JsonResponse(
                     {"errors": exc.message},
                     status=exc.status_code,
                 )
@@ -286,16 +291,16 @@
 
 class PydanticErrorDict(TypedDict):
     loc: tuple[int | str, ...]
     msg: str
 
 
 def handle_validation_error(
-    *,
-    exception: (ValidationError | pydantic.ValidationError),
+    request: HttpRequest,
+    exception: ValidationError | pydantic.ValidationError,
 ) -> HttpResponse:
     errors: list[str]
     field_errors: Mapping[str, FieldError]
 
     if isinstance(exception, pydantic.ValidationError):
 
         def error_loc(loc: tuple[int | str, ...]) -> str:
```

### Comparing `django_api_decorator-0.3.0/django_api_decorator/management/commands/generate_api_schemas.py` & `django_api_decorator-0.3.1/django_api_decorator/management/commands/generate_api_schemas.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/django_api_decorator/openapi.py` & `django_api_decorator-0.3.1/django_api_decorator/openapi.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/django_api_decorator/schema_file.py` & `django_api_decorator-0.3.1/django_api_decorator/schema_file.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/django_api_decorator/types.py` & `django_api_decorator-0.3.1/django_api_decorator/types.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/django_api_decorator/utils.py` & `django_api_decorator-0.3.1/django_api_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.3.0/pyproject.toml` & `django_api_decorator-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-api-decorator"
-version = "0.3.0"
+version = "0.3.1"
 description = "A collection of tools to build function based Django APIs"
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/django-api-decorator"
 repository = "https://github.com/kolonialno/django-api-decorator"
 packages = [{include = "django_api_decorator"}]
@@ -13,15 +13,15 @@
 python = "^3.10"
 Django = ">=3"
 pydantic = "^2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 pytest-django = "^4.5.2"
 flake8-black = "^0.3.6"
 mypy = "^1.4.1"
 django-stubs = "^4.2.3"
 pytest-mock = "^3.11.1"
```

### Comparing `django_api_decorator-0.3.0/PKG-INFO` & `django_api_decorator-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-decorator
-Version: 0.3.0
+Version: 0.3.1
 Summary: A collection of tools to build function based Django APIs
 Home-page: https://github.com/kolonialno/django-api-decorator
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

