# Comparing `tmp/ecjtu-0.0.1.tar.gz` & `tmp/ecjtu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecjtu-0.0.1.tar", max compression
+gzip compressed data, was "ecjtu-0.1.0.tar", max compression
```

## Comparing `ecjtu-0.0.1.tar` & `ecjtu-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      611 2024-04-19 18:46:35.601564 ecjtu-0.0.1/ecjtu/__init__.py
--rw-r--r--   0        0        0      179 2024-04-19 13:42:34.833786 ecjtu-0.0.1/ecjtu/__main__.py
--rw-r--r--   0        0        0    12280 2024-04-19 20:21:49.395771 ecjtu-0.0.1/ecjtu/client.py
--rw-r--r--   0        0        0     1076 2024-04-19 14:14:46.479676 ecjtu-0.0.1/ecjtu/constants.py
--rw-r--r--   0        0        0    14372 2024-04-19 15:01:08.596851 ecjtu-0.0.1/ecjtu/crud.py
--rw-r--r--   0        0        0     2190 2024-04-19 14:39:01.414272 ecjtu-0.0.1/ecjtu/models.py
--rw-r--r--   0        0        0        0 2024-04-19 20:25:34.278665 ecjtu-0.0.1/ecjtu/server.py
--rw-r--r--   0        0        0     1704 2024-04-15 14:48:31.176061 ecjtu-0.0.1/ecjtu/utils/__init__.py
--rw-r--r--   0        0        0     2156 2024-04-15 15:01:40.857941 ecjtu-0.0.1/ecjtu/utils/logger.py
--rw-r--r--   0        0        0     1311 2024-04-15 10:47:24.495846 ecjtu-0.0.1/ecjtu/utils/singleton.py
--rw-r--r--   0        0        0     1070 2024-04-03 09:05:03.563865 ecjtu-0.0.1/LICENSE
--rw-r--r--   0        0        0     2889 2024-04-19 20:58:33.758206 ecjtu-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    17434 2024-04-19 20:49:21.518139 ecjtu-0.0.1/README.md
--rw-r--r--   0        0        0    18075 1970-01-01 00:00:00.000000 ecjtu-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-19 21:08:49.256355 ecjtu-0.1.0/LICENSE
+-rw-r--r--   0        0        0    16998 2024-04-19 21:08:49.256355 ecjtu-0.1.0/README.md
+-rw-r--r--   0        0        0      611 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/__main__.py
+-rw-r--r--   0        0        0    11897 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/client.py
+-rw-r--r--   0        0        0     1060 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/constants.py
+-rw-r--r--   0        0        0    13901 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/crud.py
+-rw-r--r--   0        0        0     2148 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/models.py
+-rw-r--r--   0        0        0        0 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/server.py
+-rw-r--r--   0        0        0     1640 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/utils/__init__.py
+-rw-r--r--   0        0        0     2156 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/utils/logger.py
+-rw-r--r--   0        0        0     1311 2024-04-19 21:08:49.256355 ecjtu-0.1.0/ecjtu/utils/singleton.py
+-rw-r--r--   0        0        0     2889 2024-04-19 21:08:49.260355 ecjtu-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    18075 1970-01-01 00:00:00.000000 ecjtu-0.1.0/PKG-INFO
```

### Comparing `ecjtu-0.0.1/ecjtu/__init__.py` & `ecjtu-0.1.0/ecjtu/__init__.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.0.1/ecjtu/client.py` & `ecjtu-0.1.0/ecjtu/client.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,383 +1,383 @@
-import json
-import os
-import typing
-from typing import Generic, Optional, TypeVar, Union
-
-import httpx
-from bs4 import BeautifulSoup
-from httpx import USE_CLIENT_DEFAULT, Response, Timeout
-from httpx._client import UseClientDefault  # noqa
-from httpx._types import (  # noqa
-    AuthTypes,
-    CookieTypes,
-    HeaderTypes,
-    QueryParamTypes,
-    RequestContent,
-    RequestData,
-    RequestExtensions,
-    RequestFiles,
-    TimeoutTypes,
-    URLTypes,
-)
-
-from ecjtu import crud
-from ecjtu.constants import (
-    CAS_ECJTU_DOMAIN,
-    ECJTU2JWXT_URL,
-    ECJTU_LOGIN_URL,
-    JWXT_LOGIN_URL,
-    PORTAL_ECJTU_DOMAIN,
-    PWD_ENC_URL,
-)
-from ecjtu.utils.logger import logger
-
-_HttpxClientT = TypeVar("_HttpxClientT", bound=Union[httpx.Client, httpx.AsyncClient])
-
-
-def _get_enc_password(original_pwd: str) -> str:
-    """Get encrypted password
-
-    Args:
-        original_pwd(str): Original password
-
-    Returns:
-        str: Encrypted password
-    """
-    enc_response = httpx.post(PWD_ENC_URL, data={"pwd": original_pwd})
-
-    _ = enc_response.content.decode("utf8").replace("'", '"')
-    return json.loads(_)["passwordEnc"]
-
-
-class BaseClient(Generic[_HttpxClientT]):
-    _version: str
-    max_retries: int = 5
-    timeout: Union[float, Timeout, None]
-    _limits: httpx.Limits
-    cookies: httpx.Cookies
-
-    @property
-    def has_login(self) -> bool:
-        return "CASTGC" in self.cookies
-
-
-class ECJTU(BaseClient[httpx.Client], httpx.Client):
-    def __init__(
-        self, stud_id: Optional[str] = None, password: Optional[str] = None, **kwargs
-    ) -> None:
-        """Initialize ECJTU client.
-
-        Args:
-            stud_id(str): Student ID
-            password(str): Password
-        """
-        super().__init__(verify=False, **kwargs)
-
-        self.stud_id: str = stud_id or os.environ.get("ECJTU_STUDENT_ID")
-        self.password: str = password or os.environ.get("ECJTU_PASSWORD")
-        self.enc_password: str = _get_enc_password(self.password)
-
-        self.scheduled_courses = crud.ScheduledCourseCRUD(self)
-        self.scores = crud.ScoreCRUD(self)
-        self.gpa = crud.GPACRUD(self)
-        self.elective_courses = crud.ElectiveCourseCRUD(self)
-
-    def post(
-        self,
-        url: URLTypes,
-        *,
-        content: RequestContent | None = None,
-        data: RequestData | None = None,
-        files: RequestFiles | None = None,
-        json: typing.Any | None = None,
-        params: QueryParamTypes | None = None,
-        headers: HeaderTypes | None = None,
-        cookies: CookieTypes | None = None,
-        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
-        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        extensions: RequestExtensions | None = None,
-        current_retries: int = 0,
-    ) -> Response:
-        """Wrap the httpx post method to handle retries and check login status.
-
-        Addition Args:
-            current_retries(int): Current retries count
-        """
-        if not self.has_login:
-            self.login()
-
-        params = dict(
-            content=content,
-            data=data,
-            files=files,
-            json=json,
-            params=params,
-            headers=headers,
-            cookies=cookies,
-            auth=auth,
-            follow_redirects=follow_redirects,
-            timeout=timeout,
-            extensions=extensions,
-        )
-
-        try:
-            return super().post(url, **params)
-
-        except httpx.HTTPStatusError as e:
-            if current_retries >= self.max_retries:
-                raise e
-
-            return self.post(url, **params, current_retries=current_retries + 1)
-
-    def get(
-        self,
-        url: URLTypes,
-        *,
-        params: QueryParamTypes | None = None,
-        headers: HeaderTypes | None = None,
-        cookies: CookieTypes | None = None,
-        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
-        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        extensions: RequestExtensions | None = None,
-        current_retries: int = 0,
-    ) -> Response:
-        """Wrap the httpx get method to handle retries and check login status.
-
-        Addition Args:
-            current_retries(int): Current retries count
-        """
-        if not self.has_login:
-            self.login()
-
-        _params = dict(
-            params=params,
-            headers=headers,
-            cookies=cookies,
-            auth=auth,
-            follow_redirects=follow_redirects,
-            timeout=timeout,
-            extensions=extensions,
-        )
-
-        try:
-            return super().get(url, **_params)
-
-        except httpx.HTTPStatusError as e:
-            if current_retries >= self.max_retries:
-                raise e
-
-            return self.get(url, **_params, current_retries=current_retries + 1)
-
-    def login(self) -> None:
-        """Login to ECJTU system and update the client session."""
-        logger.info("Logging in")
-
-        login_payload = {
-            "username": self.stud_id,
-            "password": self.enc_password,
-            "service": PORTAL_ECJTU_DOMAIN,
-        }
-
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36\
-                  (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
-            "Host": CAS_ECJTU_DOMAIN,
-        }
-        response = super().get(ECJTU_LOGIN_URL, headers=headers)
-        soup = BeautifulSoup(response.content, "html.parser")
-
-        login_payload["lt"] = soup.find("input", {"name": "lt"})["value"]
-
-        headers_append = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Referer": ECJTU_LOGIN_URL,
-        }
-        headers.update(headers_append)
-        response = super().post(
-            ECJTU_LOGIN_URL,
-            data=login_payload,
-            headers=headers,
-        )
-
-        if "CASTGC" not in response.cookies:
-            raise ValueError("Error in account or password")
-
-        super().get(JWXT_LOGIN_URL, headers=headers)
-
-        response_url = super().get(ECJTU2JWXT_URL)
-
-        result = super().get(response_url.headers["location"], follow_redirects=True)
-
-        if result.status_code != 200:
-            raise ValueError(
-                f"Error in JWXT system, login failed: {result.status_code}"
-            )
-
-        logger.info("Login successful")
-
-    def start_api_server(self, port: int = 8000):
-        # TODO: Start a FastAPI server
-        pass
-
-
-class AsyncECJTU(BaseClient[httpx.AsyncClient], httpx.AsyncClient):
-    def __init__(self, stud_id: str, password: str, **kwargs) -> None:
-        """Initialize ECJTU client.
-
-        Args:
-            stud_id(str): Student ID
-            password(str): Password
-        """
-        super().__init__(verify=False, **kwargs)
-
-        self.stud_id: str = stud_id or os.environ.get("ECJTU_STUDENT_ID")
-        self.password: str = password or os.environ.get("ECJTU_PASSWORD")
-        self.enc_password: str = _get_enc_password(self.password)
-
-        self.scheduled_courses = crud.AsyncScheduledCourseCRUD(self)
-        self.scores = crud.AsyncScoreCRUD(self)
-        self.gpa = crud.AsyncGPACRUD(self)
-        self.elective_courses = crud.AsyncElectiveCourseCRUD(self)
-
-    async def post(
-        self,
-        url: URLTypes,
-        *,
-        content: RequestContent | None = None,
-        data: RequestData | None = None,
-        files: RequestFiles | None = None,
-        json: typing.Any | None = None,
-        params: QueryParamTypes | None = None,
-        headers: HeaderTypes | None = None,
-        cookies: CookieTypes | None = None,
-        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
-        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        extensions: RequestExtensions | None = None,
-        current_retries: int = 0,
-    ) -> Response:
-        """Wrap the httpx post method to handle retries and check login status.
-
-        Addition Args:
-            current_retries(int): Current retries count
-        """
-        if not self.has_login:
-            await self.login()
-
-        params = dict(
-            content=content,
-            data=data,
-            files=files,
-            json=json,
-            params=params,
-            headers=headers,
-            cookies=cookies,
-            auth=auth,
-            follow_redirects=follow_redirects,
-            timeout=timeout,
-            extensions=extensions,
-        )
-
-        try:
-            return await super().post(url, **params)
-
-        except httpx.HTTPStatusError as e:
-            if current_retries >= self.max_retries:
-                raise e
-
-            return await self.post(url, **params, current_retries=current_retries + 1)
-
-    async def get(
-        self,
-        url: URLTypes,
-        *,
-        params: QueryParamTypes | None = None,
-        headers: HeaderTypes | None = None,
-        cookies: CookieTypes | None = None,
-        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
-        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
-        extensions: RequestExtensions | None = None,
-        current_retries: int = 0,
-    ) -> Response:
-        """Wrap the httpx get method to handle retries and check login status.
-
-        Addition Args:
-            current_retries(int): Current retries count
-        """
-        if not self.has_login:
-            await self.login()
-
-        _params = dict(
-            params=params,
-            headers=headers,
-            cookies=cookies,
-            auth=auth,
-            follow_redirects=follow_redirects,
-            timeout=timeout,
-            extensions=extensions,
-        )
-
-        try:
-            return await super().get(url, **_params)
-
-        except httpx.HTTPStatusError as e:
-            if current_retries >= self.max_retries:
-                raise e
-
-            return await self.get(url, **_params, current_retries=current_retries + 1)
-
-    async def login(self) -> None:
-        """Login to ECJTU system and update the client session."""
-        logger.info("Logging in")
-
-        login_payload = {
-            "username": self.stud_id,
-            "password": self.enc_password,
-            "service": PORTAL_ECJTU_DOMAIN,
-        }
-
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36\
-                  (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
-            "Host": CAS_ECJTU_DOMAIN,
-        }
-        response = await super().get(ECJTU_LOGIN_URL, headers=headers)
-        soup = BeautifulSoup(response.content, "html.parser")
-
-        login_payload["lt"] = soup.find("input", {"name": "lt"})["value"]
-
-        headers_append = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Referer": ECJTU_LOGIN_URL,
-        }
-        headers.update(headers_append)
-        response = await super().post(
-            ECJTU_LOGIN_URL,
-            data=login_payload,
-            headers=headers,
-        )
-
-        if "CASTGC" not in response.cookies:
-            raise ValueError("Error in account or password")
-
-        await super().get(JWXT_LOGIN_URL, headers=headers)
-
-        response_url = await super().get(ECJTU2JWXT_URL)
-
-        result = await super().get(
-            response_url.headers["location"], follow_redirects=True
-        )
-
-        if result.status_code != 200:
-            raise ValueError(
-                f"Error in JWXT system, login failed: {result.status_code}"
-            )
-
-        logger.info("Login successful")
-
-    async def start_api_server(self):
-        # TODO: Start a FastAPI server
-        pass
+import json
+import os
+import typing
+from typing import Generic, Optional, TypeVar, Union
+
+import httpx
+from bs4 import BeautifulSoup
+from httpx import USE_CLIENT_DEFAULT, Response, Timeout
+from httpx._client import UseClientDefault  # noqa
+from httpx._types import (  # noqa
+    AuthTypes,
+    CookieTypes,
+    HeaderTypes,
+    QueryParamTypes,
+    RequestContent,
+    RequestData,
+    RequestExtensions,
+    RequestFiles,
+    TimeoutTypes,
+    URLTypes,
+)
+
+from ecjtu import crud
+from ecjtu.constants import (
+    CAS_ECJTU_DOMAIN,
+    ECJTU2JWXT_URL,
+    ECJTU_LOGIN_URL,
+    JWXT_LOGIN_URL,
+    PORTAL_ECJTU_DOMAIN,
+    PWD_ENC_URL,
+)
+from ecjtu.utils.logger import logger
+
+_HttpxClientT = TypeVar("_HttpxClientT", bound=Union[httpx.Client, httpx.AsyncClient])
+
+
+def _get_enc_password(original_pwd: str) -> str:
+    """Get encrypted password
+
+    Args:
+        original_pwd(str): Original password
+
+    Returns:
+        str: Encrypted password
+    """
+    enc_response = httpx.post(PWD_ENC_URL, data={"pwd": original_pwd})
+
+    _ = enc_response.content.decode("utf8").replace("'", '"')
+    return json.loads(_)["passwordEnc"]
+
+
+class BaseClient(Generic[_HttpxClientT]):
+    _version: str
+    max_retries: int = 5
+    timeout: Union[float, Timeout, None]
+    _limits: httpx.Limits
+    cookies: httpx.Cookies
+
+    @property
+    def has_login(self) -> bool:
+        return "CASTGC" in self.cookies
+
+
+class ECJTU(BaseClient[httpx.Client], httpx.Client):
+    def __init__(
+        self, stud_id: Optional[str] = None, password: Optional[str] = None, **kwargs
+    ) -> None:
+        """Initialize ECJTU client.
+
+        Args:
+            stud_id(str): Student ID
+            password(str): Password
+        """
+        super().__init__(verify=False, **kwargs)
+
+        self.stud_id: str = stud_id or os.environ.get("ECJTU_STUDENT_ID")
+        self.password: str = password or os.environ.get("ECJTU_PASSWORD")
+        self.enc_password: str = _get_enc_password(self.password)
+
+        self.scheduled_courses = crud.ScheduledCourseCRUD(self)
+        self.scores = crud.ScoreCRUD(self)
+        self.gpa = crud.GPACRUD(self)
+        self.elective_courses = crud.ElectiveCourseCRUD(self)
+
+    def post(
+        self,
+        url: URLTypes,
+        *,
+        content: RequestContent | None = None,
+        data: RequestData | None = None,
+        files: RequestFiles | None = None,
+        json: typing.Any | None = None,
+        params: QueryParamTypes | None = None,
+        headers: HeaderTypes | None = None,
+        cookies: CookieTypes | None = None,
+        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
+        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        extensions: RequestExtensions | None = None,
+        current_retries: int = 0,
+    ) -> Response:
+        """Wrap the httpx post method to handle retries and check login status.
+
+        Addition Args:
+            current_retries(int): Current retries count
+        """
+        if not self.has_login:
+            self.login()
+
+        params = dict(
+            content=content,
+            data=data,
+            files=files,
+            json=json,
+            params=params,
+            headers=headers,
+            cookies=cookies,
+            auth=auth,
+            follow_redirects=follow_redirects,
+            timeout=timeout,
+            extensions=extensions,
+        )
+
+        try:
+            return super().post(url, **params)
+
+        except httpx.HTTPStatusError as e:
+            if current_retries >= self.max_retries:
+                raise e
+
+            return self.post(url, **params, current_retries=current_retries + 1)
+
+    def get(
+        self,
+        url: URLTypes,
+        *,
+        params: QueryParamTypes | None = None,
+        headers: HeaderTypes | None = None,
+        cookies: CookieTypes | None = None,
+        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
+        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        extensions: RequestExtensions | None = None,
+        current_retries: int = 0,
+    ) -> Response:
+        """Wrap the httpx get method to handle retries and check login status.
+
+        Addition Args:
+            current_retries(int): Current retries count
+        """
+        if not self.has_login:
+            self.login()
+
+        _params = dict(
+            params=params,
+            headers=headers,
+            cookies=cookies,
+            auth=auth,
+            follow_redirects=follow_redirects,
+            timeout=timeout,
+            extensions=extensions,
+        )
+
+        try:
+            return super().get(url, **_params)
+
+        except httpx.HTTPStatusError as e:
+            if current_retries >= self.max_retries:
+                raise e
+
+            return self.get(url, **_params, current_retries=current_retries + 1)
+
+    def login(self) -> None:
+        """Login to ECJTU system and update the client session."""
+        logger.info("Logging in")
+
+        login_payload = {
+            "username": self.stud_id,
+            "password": self.enc_password,
+            "service": PORTAL_ECJTU_DOMAIN,
+        }
+
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36\
+                  (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
+            "Host": CAS_ECJTU_DOMAIN,
+        }
+        response = super().get(ECJTU_LOGIN_URL, headers=headers)
+        soup = BeautifulSoup(response.content, "html.parser")
+
+        login_payload["lt"] = soup.find("input", {"name": "lt"})["value"]
+
+        headers_append = {
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Referer": ECJTU_LOGIN_URL,
+        }
+        headers.update(headers_append)
+        response = super().post(
+            ECJTU_LOGIN_URL,
+            data=login_payload,
+            headers=headers,
+        )
+
+        if "CASTGC" not in response.cookies:
+            raise ValueError("Error in account or password")
+
+        super().get(JWXT_LOGIN_URL, headers=headers)
+
+        response_url = super().get(ECJTU2JWXT_URL)
+
+        result = super().get(response_url.headers["location"], follow_redirects=True)
+
+        if result.status_code != 200:
+            raise ValueError(
+                f"Error in JWXT system, login failed: {result.status_code}"
+            )
+
+        logger.info("Login successful")
+
+    def start_api_server(self, port: int = 8000):
+        # TODO: Start a FastAPI server
+        pass
+
+
+class AsyncECJTU(BaseClient[httpx.AsyncClient], httpx.AsyncClient):
+    def __init__(self, stud_id: str, password: str, **kwargs) -> None:
+        """Initialize ECJTU client.
+
+        Args:
+            stud_id(str): Student ID
+            password(str): Password
+        """
+        super().__init__(verify=False, **kwargs)
+
+        self.stud_id: str = stud_id or os.environ.get("ECJTU_STUDENT_ID")
+        self.password: str = password or os.environ.get("ECJTU_PASSWORD")
+        self.enc_password: str = _get_enc_password(self.password)
+
+        self.scheduled_courses = crud.AsyncScheduledCourseCRUD(self)
+        self.scores = crud.AsyncScoreCRUD(self)
+        self.gpa = crud.AsyncGPACRUD(self)
+        self.elective_courses = crud.AsyncElectiveCourseCRUD(self)
+
+    async def post(
+        self,
+        url: URLTypes,
+        *,
+        content: RequestContent | None = None,
+        data: RequestData | None = None,
+        files: RequestFiles | None = None,
+        json: typing.Any | None = None,
+        params: QueryParamTypes | None = None,
+        headers: HeaderTypes | None = None,
+        cookies: CookieTypes | None = None,
+        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
+        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        extensions: RequestExtensions | None = None,
+        current_retries: int = 0,
+    ) -> Response:
+        """Wrap the httpx post method to handle retries and check login status.
+
+        Addition Args:
+            current_retries(int): Current retries count
+        """
+        if not self.has_login:
+            await self.login()
+
+        params = dict(
+            content=content,
+            data=data,
+            files=files,
+            json=json,
+            params=params,
+            headers=headers,
+            cookies=cookies,
+            auth=auth,
+            follow_redirects=follow_redirects,
+            timeout=timeout,
+            extensions=extensions,
+        )
+
+        try:
+            return await super().post(url, **params)
+
+        except httpx.HTTPStatusError as e:
+            if current_retries >= self.max_retries:
+                raise e
+
+            return await self.post(url, **params, current_retries=current_retries + 1)
+
+    async def get(
+        self,
+        url: URLTypes,
+        *,
+        params: QueryParamTypes | None = None,
+        headers: HeaderTypes | None = None,
+        cookies: CookieTypes | None = None,
+        auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
+        timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
+        extensions: RequestExtensions | None = None,
+        current_retries: int = 0,
+    ) -> Response:
+        """Wrap the httpx get method to handle retries and check login status.
+
+        Addition Args:
+            current_retries(int): Current retries count
+        """
+        if not self.has_login:
+            await self.login()
+
+        _params = dict(
+            params=params,
+            headers=headers,
+            cookies=cookies,
+            auth=auth,
+            follow_redirects=follow_redirects,
+            timeout=timeout,
+            extensions=extensions,
+        )
+
+        try:
+            return await super().get(url, **_params)
+
+        except httpx.HTTPStatusError as e:
+            if current_retries >= self.max_retries:
+                raise e
+
+            return await self.get(url, **_params, current_retries=current_retries + 1)
+
+    async def login(self) -> None:
+        """Login to ECJTU system and update the client session."""
+        logger.info("Logging in")
+
+        login_payload = {
+            "username": self.stud_id,
+            "password": self.enc_password,
+            "service": PORTAL_ECJTU_DOMAIN,
+        }
+
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36\
+                  (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
+            "Host": CAS_ECJTU_DOMAIN,
+        }
+        response = await super().get(ECJTU_LOGIN_URL, headers=headers)
+        soup = BeautifulSoup(response.content, "html.parser")
+
+        login_payload["lt"] = soup.find("input", {"name": "lt"})["value"]
+
+        headers_append = {
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Referer": ECJTU_LOGIN_URL,
+        }
+        headers.update(headers_append)
+        response = await super().post(
+            ECJTU_LOGIN_URL,
+            data=login_payload,
+            headers=headers,
+        )
+
+        if "CASTGC" not in response.cookies:
+            raise ValueError("Error in account or password")
+
+        await super().get(JWXT_LOGIN_URL, headers=headers)
+
+        response_url = await super().get(ECJTU2JWXT_URL)
+
+        result = await super().get(
+            response_url.headers["location"], follow_redirects=True
+        )
+
+        if result.status_code != 200:
+            raise ValueError(
+                f"Error in JWXT system, login failed: {result.status_code}"
+            )
+
+        logger.info("Login successful")
+
+    async def start_api_server(self):
+        # TODO: Start a FastAPI server
+        pass
```

### Comparing `ecjtu-0.0.1/ecjtu/constants.py` & `ecjtu-0.1.0/ecjtu/constants.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-RAW_RESPONSE_HEADER = "X-Stainless-Raw-Response"
-
-ECJTU_DOMAIN = "ecjtu.edu.cn"
-PORTAL_ECJTU_DOMAIN = f"http://portal.{ECJTU_DOMAIN}/dcp/index.jsp"
-CAS_ECJTU_DOMAIN = f"cas.{ECJTU_DOMAIN}"
-JWXT_ECJTU_DOMAIN = f"jwxt.{ECJTU_DOMAIN}"
-PWD_ENC_URL = f"http://{CAS_ECJTU_DOMAIN}/cas/loginPasswdEnc"
-ECJTU_LOGIN_URL = f"http://{CAS_ECJTU_DOMAIN}/cas/login"  # 智慧交大登录页
-JWXT_LOGIN_URL = (
-    f"https://{JWXT_ECJTU_DOMAIN}/stuMag/Login_dcpLogin.action"  # 教务系统登录页
-)
-ECJTU2JWXT_URL = f"http://{CAS_ECJTU_DOMAIN}/cas/login?service=https%3A%2F%2Fjwxt.ecjtu.edu.cn%2FstuMag%2FLogin_dcpLogin.action"  # 智慧交大登录教务系统 # noqa
-GET_CLASSES_URL = f"https://{JWXT_ECJTU_DOMAIN}/Schedule/Weekcalendar_getTodayWeekcalendar.action"  # 获取课程信息(post) # noqa
-GET_GPA_URL = f"https://{JWXT_ECJTU_DOMAIN}/scoreQuery/stuScoreQue_getStuScore.action?item=0401"  # 获取成绩信息(get) # noqa
-
-GET_ELERTIVE_COURSE_URL_TEMPLATE = f"https://{JWXT_ECJTU_DOMAIN}/infoQuery/XKStu_findTerm.action"  # 获取选修课程信息(get) # noqa
+RAW_RESPONSE_HEADER = "X-Stainless-Raw-Response"
+
+ECJTU_DOMAIN = "ecjtu.edu.cn"
+PORTAL_ECJTU_DOMAIN = f"http://portal.{ECJTU_DOMAIN}/dcp/index.jsp"
+CAS_ECJTU_DOMAIN = f"cas.{ECJTU_DOMAIN}"
+JWXT_ECJTU_DOMAIN = f"jwxt.{ECJTU_DOMAIN}"
+PWD_ENC_URL = f"http://{CAS_ECJTU_DOMAIN}/cas/loginPasswdEnc"
+ECJTU_LOGIN_URL = f"http://{CAS_ECJTU_DOMAIN}/cas/login"  # 智慧交大登录页
+JWXT_LOGIN_URL = (
+    f"https://{JWXT_ECJTU_DOMAIN}/stuMag/Login_dcpLogin.action"  # 教务系统登录页
+)
+ECJTU2JWXT_URL = f"http://{CAS_ECJTU_DOMAIN}/cas/login?service=https%3A%2F%2Fjwxt.ecjtu.edu.cn%2FstuMag%2FLogin_dcpLogin.action"  # 智慧交大登录教务系统 # noqa
+GET_CLASSES_URL = f"https://{JWXT_ECJTU_DOMAIN}/Schedule/Weekcalendar_getTodayWeekcalendar.action"  # 获取课程信息(post) # noqa
+GET_GPA_URL = f"https://{JWXT_ECJTU_DOMAIN}/scoreQuery/stuScoreQue_getStuScore.action?item=0401"  # 获取成绩信息(get) # noqa
+
+GET_ELERTIVE_COURSE_URL_TEMPLATE = f"https://{JWXT_ECJTU_DOMAIN}/infoQuery/XKStu_findTerm.action"  # 获取选修课程信息(get) # noqa
```

### Comparing `ecjtu-0.0.1/ecjtu/crud.py` & `ecjtu-0.1.0/ecjtu/crud.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,471 +1,471 @@
-import re
-from abc import abstractmethod
-from datetime import datetime, timedelta
-from typing import TYPE_CHECKING, List, Optional
-
-from bs4 import BeautifulSoup
-
-from ecjtu.constants import (
-    GET_CLASSES_URL,
-    GET_ELERTIVE_COURSE_URL_TEMPLATE,
-    GET_GPA_URL,
-)
-from ecjtu.models import GPA, ElectiveCourse, ScheduledCourse, Score
-from ecjtu.utils import (
-    get_cur_semester,
-    get_cur_week_datetime,
-    get_last_semester,
-    get_today_date,
-)
-from ecjtu.utils.logger import logger
-
-if TYPE_CHECKING:
-    from ecjtu.client import ECJTU, AsyncECJTU
-
-
-class CRUDClient:
-    """
-    CRUD mixin for resources. This class provides basic CRUD operations for resources.
-    """
-
-    def __init__(self, client: "ECJTU"):
-        self.client: "ECJTU" = client
-        self.cache: dict = {}
-
-    @abstractmethod
-    def today(self, *args, **kwargs):
-        raise NotImplementedError
-
-    @abstractmethod
-    def filter(self, *args, **kwargs):
-        raise NotImplementedError
-
-
-class AsyncCRUDClient:
-    """
-    CRUD mixin for resources. This class provides basic CRUD operations for resources.
-    """
-
-    def __init__(self, client: "AsyncECJTU"):
-        self.client: AsyncECJTU = client
-        self.cache: dict = {}
-
-    @abstractmethod
-    async def today(self, *args, **kwargs):
-        raise NotImplementedError
-
-    @abstractmethod
-    async def filter(self, *args, **kwargs):
-        raise NotImplementedError
-
-
-class ScheduledCourseCRUD(CRUDClient):
-    def _fetch_courses(self, date: str) -> List[ScheduledCourse]:
-        """Fetch courses by date
-
-        Args:
-            date(str): The date to fetch, eg: 2023-01-01
-
-        Returns:
-            List[ScheduledCourse]: List of courses
-        """
-        classes: List[ScheduledCourse] = []
-
-        resp = self.client.post(GET_CLASSES_URL, data={"date": date})
-        for k, v in resp.json().items():
-            if k == "weekcalendarpojoList":
-                for item in v:
-                    cls = ScheduledCourse.model_validate(item)
-                    logger.info(cls)
-                    classes.append(cls)
-
-        return classes
-
-    def filter(self, *, date: str) -> List[ScheduledCourse]:
-        """Filter courses by date
-
-        Args:
-            date(str): The date to filter, eg: 2023-01-01
-
-        Returns:
-            List[ElectiveCourse]: List of courses
-        """
-        return self._fetch_courses(date)
-
-    def today(self) -> List[ScheduledCourse]:
-        """Get today's classes
-
-        Returns:
-            List[ElectiveCourse]: List of courses
-        """
-        date: str = get_today_date()
-        return self._fetch_courses(date)
-
-    def this_week(self) -> List[List[ScheduledCourse]]:
-        """Get this week's classes
-
-        Returns:
-            List[List[ElectiveCourse]]: List of courses
-        """
-        start_datetime: datetime = get_cur_week_datetime()
-        week_classes: List[List[ScheduledCourse]] = []
-
-        for i in range(7):
-            date: str = (start_datetime + timedelta(days=i)).strftime("%Y-%m-%d")
-            week_classes.append(self._fetch_courses(date))
-
-        return week_classes
-
-
-class AsyncScheduledCourseCRUD(AsyncCRUDClient):
-    async def _fetch_courses(self, date: str) -> List[ScheduledCourse]:
-        """Fetch courses by date
-
-        Args:
-            date(str): The date to fetch, eg: 2023-01-01
-
-        Returns:
-            List[ScheduledCourse]: List of courses
-        """
-        classes: List[ScheduledCourse] = []
-
-        resp = await self.client.post(GET_CLASSES_URL, data={"date": date})
-        for k, v in resp.json().items():
-            if k == "weekcalendarpojoList":
-                for item in v:
-                    cls = ScheduledCourse.model_validate(item)
-                    logger.info(cls)
-                    classes.append(cls)
-
-        return classes
-
-    async def filter(self, *, date: str) -> List[ScheduledCourse]:
-        """Filter courses by date
-
-        Args:
-            date(str): The date to filter, eg: 2023-01-01
-
-        Returns:
-            List[ElectiveCourse]: List of courses
-        """
-        return await self._fetch_courses(date)
-
-    async def today(self) -> List[ScheduledCourse]:
-        """Get today's classes
-
-        Returns:
-            List[ElectiveCourse]: List of courses
-        """
-        date: str = get_today_date()
-        return await self._fetch_courses(date)
-
-    async def this_week(self) -> List[List[ScheduledCourse]]:
-        """Get this week's classes
-
-        Returns:
-            List[List[ElectiveCourse]]: List of courses
-        """
-        start_datetime: datetime = get_cur_week_datetime()
-        week_classes: List[List[ScheduledCourse]] = []
-
-        for i in range(7):
-            date: str = (start_datetime + timedelta(days=i)).strftime("%Y-%m-%d")
-            week_classes.append(await self._fetch_courses(date))
-
-        return week_classes
-
-
-class GPACRUD(CRUDClient):
-    def today(self) -> GPA:
-        """Get current GPA
-
-        Returns:
-            GPA: GPA model
-        """
-        resp_html = self.client.get(GET_GPA_URL)
-
-        if resp_html.status_code != 200:
-            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
-
-        soup = BeautifulSoup(resp_html.text, "html.parser")
-        data = [td.text for td in soup.find_all("tr")[3].find_all("td")]
-        return GPA.model_validate(
-            {"student_name": data[1], "gpa": data[6], "status": data[2]}
-        )
-
-    def filter(self, **kwargs) -> List[GPA]:
-        raise Exception("GAP can't be filtered")
-
-
-class AsyncGPACRUD(AsyncCRUDClient):
-    async def today(self) -> GPA:
-        """Get current GPA
-
-        Returns:
-            GPA: GPA model
-        """
-        resp_html = await self.client.get(GET_GPA_URL)
-
-        if resp_html.status_code != 200:
-            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
-
-        soup = BeautifulSoup(resp_html.text, "html.parser")
-        data = [td.text for td in soup.find_all("tr")[3].find_all("td")]
-        return GPA.model_validate(
-            {"student_name": data[1], "gpa": data[6], "status": data[2]}
-        )
-
-    async def filter(self, **kwargs) -> List[GPA]:
-        raise Exception("GAP can't be filtered")
-
-
-class ScoreCRUD(CRUDClient):
-    def _fetch_scores(self, semester: str) -> List[Score]:
-        """Fetch scores by semester
-
-        Args:
-            semester(str): The semester to fetch, eg: 2023.1
-
-        Returns:
-            List[Score]: List of scores
-        """
-        resp_html = self.client.get(GET_GPA_URL)
-
-        if resp_html.status_code != 200:
-            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
-
-        scores: List[Score] = []
-        soup = BeautifulSoup(resp_html.text, "html.parser")
-
-        pattern = re.compile(r"\b{}\b".format(semester.replace(".", "_")))
-        ul_tags = soup.find_all("ul", class_=pattern)
-        for ul_tag in ul_tags:
-            li_list = ul_tag.find_all("li")
-            li_values = [li.text for li in li_list]
-
-            score = Score(
-                semester=semester,
-                course_name=li_values[1],
-                course_nature=li_values[2],
-                credit=float(li_values[4]),
-                grade=li_values[5],
-            )
-            scores.append(score)
-
-        return scores
-
-    def today(self) -> List[Score]:
-        """Get last semester's scores.
-
-        The scores of this semester are not available until the semester ends.
-
-        Returns:
-            List[Score]: List of scores
-        """
-        semester = get_last_semester()
-        return self._fetch_scores(semester)
-
-    def filter(self, *, semester: Optional[str] = None, **kwargs) -> List[Score]:
-        """Filter scores by specified conditions.
-
-        Args:
-            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
-
-        Returns:
-            List[Score]: List of scores
-        """
-        return self._fetch_scores(semester)
-
-
-class AsyncScoreCRUD(AsyncCRUDClient):
-    async def _fetch_scores(self, semester: str) -> List[Score]:
-        """Fetch scores by semester
-
-        Args:
-            semester(str): The semester to fetch, eg: 2023.1
-
-        Returns:
-            List[Score]: List of scores
-        """
-        resp_html = await self.client.get(GET_GPA_URL)
-
-        if resp_html.status_code != 200:
-            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
-
-        scores: List[Score] = []
-        soup = BeautifulSoup(resp_html.text, "html.parser")
-
-        pattern = re.compile(r"\b{}\b".format(semester.replace(".", "_")))
-        ul_tags = soup.find_all("ul", class_=pattern)
-        for ul_tag in ul_tags:
-            li_list = ul_tag.find_all("li")
-            li_values = [li.text for li in li_list]
-
-            score = Score(
-                semester=semester,
-                course_name=li_values[1],
-                course_nature=li_values[2],
-                credit=float(li_values[4]),
-                grade=li_values[5],
-            )
-            scores.append(score)
-
-        return scores
-
-    async def today(self) -> List[Score]:
-        """Get last semester's scores.
-
-        The scores of this semester are not available until the semester ends.
-
-        Returns:
-            List[Score]: List of scores
-        """
-        semester = get_last_semester()
-        return await self._fetch_scores(semester)
-
-    async def filter(self, *, semester: Optional[str] = None, **kwargs) -> List[Score]:
-        """Filter scores by specified conditions.
-
-        Args:
-            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
-
-        Returns:
-            List[Score]: List of scores
-        """
-        return await self._fetch_scores(semester)
-
-
-class ElectiveCourseCRUD(CRUDClient):
-    def _fetch_elecourses(self, semester: str) -> List[ElectiveCourse]:
-        """Fetch elecourses by date
-
-        Args:
-            semester(str): The semester to fetch, eg: 2023.1
-
-        Returns:
-            List[ElectiveCourse]: List of courses
-        """
-
-        get_elertive_course_url = GET_ELERTIVE_COURSE_URL_TEMPLATE + "?term=" + semester
-
-        resp_html = self.client.get(get_elertive_course_url)
-
-        if resp_html.status_code != 200:
-            raise Exception(
-                f"Failed to get elective courses, status code: {resp_html.status_code}"
-            )
-
-        ele_courses: List[ElectiveCourse] = []
-        soup = BeautifulSoup(resp_html.text, "html.parser")
-
-        tbody_tag = soup.find("tbody")
-        tr_list = tbody_tag.find_all("tr")
-
-        for tr_tag in tr_list:
-            td_tags = tr_tag.find_all("td")
-            td = [td.text for td in td_tags]
-            ele_course = ElectiveCourse(
-                semester=td[0],
-                class_name=td[11],
-                class_type=td[4],
-                class_assessment_method=td[5],
-                class_info=td[8],
-                class_number=td[12],
-                credit=float(td[7]),
-                teacher=td[9],
-            )
-            ele_courses.append(ele_course)
-
-        return ele_courses
-
-    def today(self, *args, **kwargs):
-        """
-        Get today's elective courses
-
-        Returns:
-            List[ElectiveCourse]: List of elective courses
-        """
-        semester = get_cur_semester()
-        return self._fetch_elecourses(semester)
-
-    def filter(
-        self, *, semester: Optional[str] = None, **kwargs
-    ) -> List[ElectiveCourse]:
-        """
-        Filter elective courses by specified conditions.
-
-        Args:
-            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
-
-        Returns:
-            List[ElectiveCourse]: List of elective courses
-        """
-        return self._fetch_elecourses(semester)
-
-
-class AsyncElectiveCourseCRUD(AsyncCRUDClient):
-    async def _fetch_elecourses(self, semester: str) -> List[ElectiveCourse]:
-        """Fetch elecourses by date
-
-        Args:
-            semester(str): The semester to fetch, eg: 2023.1
-
-        Returns:
-            List[ElectiveCourse]: List of courses
-        """
-
-        get_elertive_course_url = GET_ELERTIVE_COURSE_URL_TEMPLATE + "?term=" + semester
-
-        resp_html = await self.client.get(get_elertive_course_url)
-
-        if resp_html.status_code != 200:
-            raise Exception(
-                f"Failed to get elective courses, status code: {resp_html.status_code}"
-            )
-
-        ele_courses: List[ElectiveCourse] = []
-        soup = BeautifulSoup(resp_html.text, "html.parser")
-
-        tbody_tag = soup.find("tbody")
-        tr_list = tbody_tag.find_all("tr")
-
-        for tr_tag in tr_list:
-            td_tags = tr_tag.find_all("td")
-            td = [td.text for td in td_tags]
-            ele_course = ElectiveCourse(
-                semester=td[0],
-                class_name=td[11],
-                class_type=td[4],
-                class_assessment_method=td[5],
-                class_info=td[8],
-                class_number=td[12],
-                credit=float(td[7]),
-                teacher=td[9],
-            )
-            ele_courses.append(ele_course)
-
-        return ele_courses
-
-    async def today(self, *args, **kwargs):
-        """
-        Get today's elective courses
-
-        Returns:
-            List[ElectiveCourse]: List of elective courses
-        """
-        semester = get_cur_semester()
-        return await self._fetch_elecourses(semester)
-
-    async def filter(
-        self, *, semester: Optional[str] = None, **kwargs
-    ) -> List[ElectiveCourse]:
-        """
-        Filter elective courses by specified conditions.
-
-        Args:
-            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
-
-        Returns:
-            List[ElectiveCourse]: List of elective courses
-        """
-        return await self._fetch_elecourses(semester)
+import re
+from abc import abstractmethod
+from datetime import datetime, timedelta
+from typing import TYPE_CHECKING, List, Optional
+
+from bs4 import BeautifulSoup
+
+from ecjtu.constants import (
+    GET_CLASSES_URL,
+    GET_ELERTIVE_COURSE_URL_TEMPLATE,
+    GET_GPA_URL,
+)
+from ecjtu.models import GPA, ElectiveCourse, ScheduledCourse, Score
+from ecjtu.utils import (
+    get_cur_semester,
+    get_cur_week_datetime,
+    get_last_semester,
+    get_today_date,
+)
+from ecjtu.utils.logger import logger
+
+if TYPE_CHECKING:
+    from ecjtu.client import ECJTU, AsyncECJTU
+
+
+class CRUDClient:
+    """
+    CRUD mixin for resources. This class provides basic CRUD operations for resources.
+    """
+
+    def __init__(self, client: "ECJTU"):
+        self.client: "ECJTU" = client
+        self.cache: dict = {}
+
+    @abstractmethod
+    def today(self, *args, **kwargs):
+        raise NotImplementedError
+
+    @abstractmethod
+    def filter(self, *args, **kwargs):
+        raise NotImplementedError
+
+
+class AsyncCRUDClient:
+    """
+    CRUD mixin for resources. This class provides basic CRUD operations for resources.
+    """
+
+    def __init__(self, client: "AsyncECJTU"):
+        self.client: AsyncECJTU = client
+        self.cache: dict = {}
+
+    @abstractmethod
+    async def today(self, *args, **kwargs):
+        raise NotImplementedError
+
+    @abstractmethod
+    async def filter(self, *args, **kwargs):
+        raise NotImplementedError
+
+
+class ScheduledCourseCRUD(CRUDClient):
+    def _fetch_courses(self, date: str) -> List[ScheduledCourse]:
+        """Fetch courses by date
+
+        Args:
+            date(str): The date to fetch, eg: 2023-01-01
+
+        Returns:
+            List[ScheduledCourse]: List of courses
+        """
+        classes: List[ScheduledCourse] = []
+
+        resp = self.client.post(GET_CLASSES_URL, data={"date": date})
+        for k, v in resp.json().items():
+            if k == "weekcalendarpojoList":
+                for item in v:
+                    cls = ScheduledCourse.model_validate(item)
+                    logger.info(cls)
+                    classes.append(cls)
+
+        return classes
+
+    def filter(self, *, date: str) -> List[ScheduledCourse]:
+        """Filter courses by date
+
+        Args:
+            date(str): The date to filter, eg: 2023-01-01
+
+        Returns:
+            List[ElectiveCourse]: List of courses
+        """
+        return self._fetch_courses(date)
+
+    def today(self) -> List[ScheduledCourse]:
+        """Get today's classes
+
+        Returns:
+            List[ElectiveCourse]: List of courses
+        """
+        date: str = get_today_date()
+        return self._fetch_courses(date)
+
+    def this_week(self) -> List[List[ScheduledCourse]]:
+        """Get this week's classes
+
+        Returns:
+            List[List[ElectiveCourse]]: List of courses
+        """
+        start_datetime: datetime = get_cur_week_datetime()
+        week_classes: List[List[ScheduledCourse]] = []
+
+        for i in range(7):
+            date: str = (start_datetime + timedelta(days=i)).strftime("%Y-%m-%d")
+            week_classes.append(self._fetch_courses(date))
+
+        return week_classes
+
+
+class AsyncScheduledCourseCRUD(AsyncCRUDClient):
+    async def _fetch_courses(self, date: str) -> List[ScheduledCourse]:
+        """Fetch courses by date
+
+        Args:
+            date(str): The date to fetch, eg: 2023-01-01
+
+        Returns:
+            List[ScheduledCourse]: List of courses
+        """
+        classes: List[ScheduledCourse] = []
+
+        resp = await self.client.post(GET_CLASSES_URL, data={"date": date})
+        for k, v in resp.json().items():
+            if k == "weekcalendarpojoList":
+                for item in v:
+                    cls = ScheduledCourse.model_validate(item)
+                    logger.info(cls)
+                    classes.append(cls)
+
+        return classes
+
+    async def filter(self, *, date: str) -> List[ScheduledCourse]:
+        """Filter courses by date
+
+        Args:
+            date(str): The date to filter, eg: 2023-01-01
+
+        Returns:
+            List[ElectiveCourse]: List of courses
+        """
+        return await self._fetch_courses(date)
+
+    async def today(self) -> List[ScheduledCourse]:
+        """Get today's classes
+
+        Returns:
+            List[ElectiveCourse]: List of courses
+        """
+        date: str = get_today_date()
+        return await self._fetch_courses(date)
+
+    async def this_week(self) -> List[List[ScheduledCourse]]:
+        """Get this week's classes
+
+        Returns:
+            List[List[ElectiveCourse]]: List of courses
+        """
+        start_datetime: datetime = get_cur_week_datetime()
+        week_classes: List[List[ScheduledCourse]] = []
+
+        for i in range(7):
+            date: str = (start_datetime + timedelta(days=i)).strftime("%Y-%m-%d")
+            week_classes.append(await self._fetch_courses(date))
+
+        return week_classes
+
+
+class GPACRUD(CRUDClient):
+    def today(self) -> GPA:
+        """Get current GPA
+
+        Returns:
+            GPA: GPA model
+        """
+        resp_html = self.client.get(GET_GPA_URL)
+
+        if resp_html.status_code != 200:
+            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
+
+        soup = BeautifulSoup(resp_html.text, "html.parser")
+        data = [td.text for td in soup.find_all("tr")[3].find_all("td")]
+        return GPA.model_validate(
+            {"student_name": data[1], "gpa": data[6], "status": data[2]}
+        )
+
+    def filter(self, **kwargs) -> List[GPA]:
+        raise Exception("GAP can't be filtered")
+
+
+class AsyncGPACRUD(AsyncCRUDClient):
+    async def today(self) -> GPA:
+        """Get current GPA
+
+        Returns:
+            GPA: GPA model
+        """
+        resp_html = await self.client.get(GET_GPA_URL)
+
+        if resp_html.status_code != 200:
+            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
+
+        soup = BeautifulSoup(resp_html.text, "html.parser")
+        data = [td.text for td in soup.find_all("tr")[3].find_all("td")]
+        return GPA.model_validate(
+            {"student_name": data[1], "gpa": data[6], "status": data[2]}
+        )
+
+    async def filter(self, **kwargs) -> List[GPA]:
+        raise Exception("GAP can't be filtered")
+
+
+class ScoreCRUD(CRUDClient):
+    def _fetch_scores(self, semester: str) -> List[Score]:
+        """Fetch scores by semester
+
+        Args:
+            semester(str): The semester to fetch, eg: 2023.1
+
+        Returns:
+            List[Score]: List of scores
+        """
+        resp_html = self.client.get(GET_GPA_URL)
+
+        if resp_html.status_code != 200:
+            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
+
+        scores: List[Score] = []
+        soup = BeautifulSoup(resp_html.text, "html.parser")
+
+        pattern = re.compile(r"\b{}\b".format(semester.replace(".", "_")))
+        ul_tags = soup.find_all("ul", class_=pattern)
+        for ul_tag in ul_tags:
+            li_list = ul_tag.find_all("li")
+            li_values = [li.text for li in li_list]
+
+            score = Score(
+                semester=semester,
+                course_name=li_values[1],
+                course_nature=li_values[2],
+                credit=float(li_values[4]),
+                grade=li_values[5],
+            )
+            scores.append(score)
+
+        return scores
+
+    def today(self) -> List[Score]:
+        """Get last semester's scores.
+
+        The scores of this semester are not available until the semester ends.
+
+        Returns:
+            List[Score]: List of scores
+        """
+        semester = get_last_semester()
+        return self._fetch_scores(semester)
+
+    def filter(self, *, semester: Optional[str] = None, **kwargs) -> List[Score]:
+        """Filter scores by specified conditions.
+
+        Args:
+            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
+
+        Returns:
+            List[Score]: List of scores
+        """
+        return self._fetch_scores(semester)
+
+
+class AsyncScoreCRUD(AsyncCRUDClient):
+    async def _fetch_scores(self, semester: str) -> List[Score]:
+        """Fetch scores by semester
+
+        Args:
+            semester(str): The semester to fetch, eg: 2023.1
+
+        Returns:
+            List[Score]: List of scores
+        """
+        resp_html = await self.client.get(GET_GPA_URL)
+
+        if resp_html.status_code != 200:
+            raise Exception(f"Failed to get GPA, status code: {resp_html.status_code}")
+
+        scores: List[Score] = []
+        soup = BeautifulSoup(resp_html.text, "html.parser")
+
+        pattern = re.compile(r"\b{}\b".format(semester.replace(".", "_")))
+        ul_tags = soup.find_all("ul", class_=pattern)
+        for ul_tag in ul_tags:
+            li_list = ul_tag.find_all("li")
+            li_values = [li.text for li in li_list]
+
+            score = Score(
+                semester=semester,
+                course_name=li_values[1],
+                course_nature=li_values[2],
+                credit=float(li_values[4]),
+                grade=li_values[5],
+            )
+            scores.append(score)
+
+        return scores
+
+    async def today(self) -> List[Score]:
+        """Get last semester's scores.
+
+        The scores of this semester are not available until the semester ends.
+
+        Returns:
+            List[Score]: List of scores
+        """
+        semester = get_last_semester()
+        return await self._fetch_scores(semester)
+
+    async def filter(self, *, semester: Optional[str] = None, **kwargs) -> List[Score]:
+        """Filter scores by specified conditions.
+
+        Args:
+            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
+
+        Returns:
+            List[Score]: List of scores
+        """
+        return await self._fetch_scores(semester)
+
+
+class ElectiveCourseCRUD(CRUDClient):
+    def _fetch_elecourses(self, semester: str) -> List[ElectiveCourse]:
+        """Fetch elecourses by date
+
+        Args:
+            semester(str): The semester to fetch, eg: 2023.1
+
+        Returns:
+            List[ElectiveCourse]: List of courses
+        """
+
+        get_elertive_course_url = GET_ELERTIVE_COURSE_URL_TEMPLATE + "?term=" + semester
+
+        resp_html = self.client.get(get_elertive_course_url)
+
+        if resp_html.status_code != 200:
+            raise Exception(
+                f"Failed to get elective courses, status code: {resp_html.status_code}"
+            )
+
+        ele_courses: List[ElectiveCourse] = []
+        soup = BeautifulSoup(resp_html.text, "html.parser")
+
+        tbody_tag = soup.find("tbody")
+        tr_list = tbody_tag.find_all("tr")
+
+        for tr_tag in tr_list:
+            td_tags = tr_tag.find_all("td")
+            td = [td.text for td in td_tags]
+            ele_course = ElectiveCourse(
+                semester=td[0],
+                class_name=td[11],
+                class_type=td[4],
+                class_assessment_method=td[5],
+                class_info=td[8],
+                class_number=td[12],
+                credit=float(td[7]),
+                teacher=td[9],
+            )
+            ele_courses.append(ele_course)
+
+        return ele_courses
+
+    def today(self, *args, **kwargs):
+        """
+        Get today's elective courses
+
+        Returns:
+            List[ElectiveCourse]: List of elective courses
+        """
+        semester = get_cur_semester()
+        return self._fetch_elecourses(semester)
+
+    def filter(
+        self, *, semester: Optional[str] = None, **kwargs
+    ) -> List[ElectiveCourse]:
+        """
+        Filter elective courses by specified conditions.
+
+        Args:
+            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
+
+        Returns:
+            List[ElectiveCourse]: List of elective courses
+        """
+        return self._fetch_elecourses(semester)
+
+
+class AsyncElectiveCourseCRUD(AsyncCRUDClient):
+    async def _fetch_elecourses(self, semester: str) -> List[ElectiveCourse]:
+        """Fetch elecourses by date
+
+        Args:
+            semester(str): The semester to fetch, eg: 2023.1
+
+        Returns:
+            List[ElectiveCourse]: List of courses
+        """
+
+        get_elertive_course_url = GET_ELERTIVE_COURSE_URL_TEMPLATE + "?term=" + semester
+
+        resp_html = await self.client.get(get_elertive_course_url)
+
+        if resp_html.status_code != 200:
+            raise Exception(
+                f"Failed to get elective courses, status code: {resp_html.status_code}"
+            )
+
+        ele_courses: List[ElectiveCourse] = []
+        soup = BeautifulSoup(resp_html.text, "html.parser")
+
+        tbody_tag = soup.find("tbody")
+        tr_list = tbody_tag.find_all("tr")
+
+        for tr_tag in tr_list:
+            td_tags = tr_tag.find_all("td")
+            td = [td.text for td in td_tags]
+            ele_course = ElectiveCourse(
+                semester=td[0],
+                class_name=td[11],
+                class_type=td[4],
+                class_assessment_method=td[5],
+                class_info=td[8],
+                class_number=td[12],
+                credit=float(td[7]),
+                teacher=td[9],
+            )
+            ele_courses.append(ele_course)
+
+        return ele_courses
+
+    async def today(self, *args, **kwargs):
+        """
+        Get today's elective courses
+
+        Returns:
+            List[ElectiveCourse]: List of elective courses
+        """
+        semester = get_cur_semester()
+        return await self._fetch_elecourses(semester)
+
+    async def filter(
+        self, *, semester: Optional[str] = None, **kwargs
+    ) -> List[ElectiveCourse]:
+        """
+        Filter elective courses by specified conditions.
+
+        Args:
+            semester(Optional[str]): The semester to filter, eg: 2023.1, 2023.2
+
+        Returns:
+            List[ElectiveCourse]: List of elective courses
+        """
+        return await self._fetch_elecourses(semester)
```

### Comparing `ecjtu-0.0.1/ecjtu/models.py` & `ecjtu-0.1.0/ecjtu/models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from pydantic import BaseModel, Field
-
-
-class ElectiveCourse(BaseModel):
-    semester: str = Field(..., description="学期", examples=["2023.1"])
-    class_name: str = Field(
-        ..., description="教学班名称", examples=["高等数学(20232-23)[小2班]"]
-    )
-    class_type: str = Field(..., description="课程类型", examples=["必修课"])
-    class_assessment_method: str = Field(..., description="考核方式", examples=["考试"])
-    class_info: str = Field(
-        ..., description="上课信息", examples=["第1-4周 星期一 第7,8节[31-313]"]
-    )
-    class_number: str = Field(..., description="课程编号", examples=["19"])
-    credit: float = Field(..., description="学分", examples=[3.0])
-    teacher: str = Field(..., description="教师", examples=["张三"])
-
-
-class ScheduledCourse(BaseModel):
-    class_span: str = Field(..., description="上课时间", alias="classSpan")
-    course: str = Field(..., description="课程名称", alias="course")
-    course_name: str = Field(..., description="详细课程名称", alias="className")
-    week_span: str = Field(..., description="周数", alias="weekSpan")
-    course_type: str = Field(..., description="是否为必修课", alias="courseRequire")
-    teacher: str = Field(..., description="教师姓名", alias="teacherName")
-    week_day: int = Field(..., description="星期几", alias="weekDay")
-    class_room: str = Field(..., description="教室", alias="classRoom")
-    pk_type: str = Field(..., description="课程类型", alias="pkType")
-
-
-class GPA(BaseModel):
-    student_name: str = Field(..., description="学生名称")
-    gpa: str = Field(..., description="绩点")
-    status: str = Field(..., description="状态")
-
-
-class Score(BaseModel):
-    semester: str = Field(..., description="课程学期", examples=["2023.1"])
-    course_name: str = Field(..., description="课程名", examples=["高等数学"])
-    course_nature: str = Field(..., description="课程性质", examples=["必修"])
-    credit: float = Field(..., description="学分", examples=[3.0])
-    grade: str = Field(..., description="成绩", examples=["合格", "94"])
+from pydantic import BaseModel, Field
+
+
+class ElectiveCourse(BaseModel):
+    semester: str = Field(..., description="学期", examples=["2023.1"])
+    class_name: str = Field(
+        ..., description="教学班名称", examples=["高等数学(20232-23)[小2班]"]
+    )
+    class_type: str = Field(..., description="课程类型", examples=["必修课"])
+    class_assessment_method: str = Field(..., description="考核方式", examples=["考试"])
+    class_info: str = Field(
+        ..., description="上课信息", examples=["第1-4周 星期一 第7,8节[31-313]"]
+    )
+    class_number: str = Field(..., description="课程编号", examples=["19"])
+    credit: float = Field(..., description="学分", examples=[3.0])
+    teacher: str = Field(..., description="教师", examples=["张三"])
+
+
+class ScheduledCourse(BaseModel):
+    class_span: str = Field(..., description="上课时间", alias="classSpan")
+    course: str = Field(..., description="课程名称", alias="course")
+    course_name: str = Field(..., description="详细课程名称", alias="className")
+    week_span: str = Field(..., description="周数", alias="weekSpan")
+    course_type: str = Field(..., description="是否为必修课", alias="courseRequire")
+    teacher: str = Field(..., description="教师姓名", alias="teacherName")
+    week_day: int = Field(..., description="星期几", alias="weekDay")
+    class_room: str = Field(..., description="教室", alias="classRoom")
+    pk_type: str = Field(..., description="课程类型", alias="pkType")
+
+
+class GPA(BaseModel):
+    student_name: str = Field(..., description="学生名称")
+    gpa: str = Field(..., description="绩点")
+    status: str = Field(..., description="状态")
+
+
+class Score(BaseModel):
+    semester: str = Field(..., description="课程学期", examples=["2023.1"])
+    course_name: str = Field(..., description="课程名", examples=["高等数学"])
+    course_nature: str = Field(..., description="课程性质", examples=["必修"])
+    credit: float = Field(..., description="学分", examples=[3.0])
+    grade: str = Field(..., description="成绩", examples=["合格", "94"])
```

### Comparing `ecjtu-0.0.1/ecjtu/utils/__init__.py` & `ecjtu-0.1.0/ecjtu/utils/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import os
-import tempfile
-from datetime import datetime, timedelta
-
-
-def convert_backslashes(path: str):
-    """Convert all \\ to / of file path."""
-    return path.replace("\\", "/")
-
-
-def get_default_storage_path(module_name: str = "") -> str:
-    storage_path = os.path.expanduser("~/.ecjtu")
-
-    if module_name:
-        storage_path = os.path.join(storage_path, module_name)
-
-    # Try to create the storage path (with module subdirectory if specified)
-    # Use a temporary directory instead if permission is denied,
-    try:
-        os.makedirs(storage_path, exist_ok=True)
-    except PermissionError:
-        storage_path = os.path.join(tempfile.gettempdir(), "ecjtu", module_name)
-        os.makedirs(storage_path, exist_ok=True)
-
-    return convert_backslashes(storage_path)
-
-
-def get_today_date() -> str:
-    """Get today's date in the format of "YYYY-MM-DD".
-
-    Returns:
-        str: Today's date
-    """
-    return datetime.now().strftime("%Y-%m-%d")
-
-
-def get_cur_week_datetime() -> datetime:
-    """Get the start datetime of the current week."""
-    today = datetime.now()
-    return today - timedelta(days=today.weekday())
-
-
-def get_cur_semester() -> str:
-    """Get the current semester, eg: 2023.1 or 2022.2
-
-    Returns:
-        str: The current semester
-    """
-    now = datetime.now()
-    if now.month < 9:
-        return f"{now.year - 1}.2"
-    return f"{now.year}.1"
-
-
-def get_last_semester() -> str:
-    """Get the last semester, eg: 2023.1 or 2022.2
-
-    Returns:
-        str: The last semester
-    """
-    now = datetime.now()
-    if now.month < 9:
-        return f"{now.year - 1}.1"
-    return f"{now.year}.2"
+import os
+import tempfile
+from datetime import datetime, timedelta
+
+
+def convert_backslashes(path: str):
+    """Convert all \\ to / of file path."""
+    return path.replace("\\", "/")
+
+
+def get_default_storage_path(module_name: str = "") -> str:
+    storage_path = os.path.expanduser("~/.ecjtu")
+
+    if module_name:
+        storage_path = os.path.join(storage_path, module_name)
+
+    # Try to create the storage path (with module subdirectory if specified)
+    # Use a temporary directory instead if permission is denied,
+    try:
+        os.makedirs(storage_path, exist_ok=True)
+    except PermissionError:
+        storage_path = os.path.join(tempfile.gettempdir(), "ecjtu", module_name)
+        os.makedirs(storage_path, exist_ok=True)
+
+    return convert_backslashes(storage_path)
+
+
+def get_today_date() -> str:
+    """Get today's date in the format of "YYYY-MM-DD".
+
+    Returns:
+        str: Today's date
+    """
+    return datetime.now().strftime("%Y-%m-%d")
+
+
+def get_cur_week_datetime() -> datetime:
+    """Get the start datetime of the current week."""
+    today = datetime.now()
+    return today - timedelta(days=today.weekday())
+
+
+def get_cur_semester() -> str:
+    """Get the current semester, eg: 2023.1 or 2022.2
+
+    Returns:
+        str: The current semester
+    """
+    now = datetime.now()
+    if now.month < 9:
+        return f"{now.year - 1}.2"
+    return f"{now.year}.1"
+
+
+def get_last_semester() -> str:
+    """Get the last semester, eg: 2023.1 or 2022.2
+
+    Returns:
+        str: The last semester
+    """
+    now = datetime.now()
+    if now.month < 9:
+        return f"{now.year - 1}.1"
+    return f"{now.year}.2"
```

### Comparing `ecjtu-0.0.1/ecjtu/utils/logger.py` & `ecjtu-0.1.0/ecjtu/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.0.1/ecjtu/utils/singleton.py` & `ecjtu-0.1.0/ecjtu/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `ecjtu-0.0.1/LICENSE` & `ecjtu-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecjtu-0.0.1/pyproject.toml` & `ecjtu-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ecjtu"
-version = "0.0.1"
+version = "0.1.0"
 description = "ECJTU API SDK service"
 readme = "README.md"
 authors = ["ecjtu <zeeland4work@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/Undertone0809/ecjtu"
 homepage = "https://github.com/Undertone0809/ecjtu"
 keywords = []
```

### Comparing `ecjtu-0.0.1/README.md` & `ecjtu-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,437 +1,437 @@
-# ecjtu
-
-<div align="center">
-
-[![Python Version](https://img.shields.io/pypi/pyversions/ecjtu.svg)](https://pypi.org/project/ecjtu/)
-[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Undertone0809/ecjtu/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
-
-[![Code style: ruff](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/astral-sh/ruff)
-[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Undertone0809/ecjtu/blob/main/.pre-commit-config.yaml)
-[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Undertone0809/ecjtu/releases)
-[![License](https://img.shields.io/github/license/Undertone0809/ecjtu)](https://github.com/Undertone0809/ecjtu/blob/main/LICENSE)
-![Coverage Report](assets/images/coverage.svg)
-
-All your need is ECJTU API SDK service
-
-</div>
-
-## 📚 Introduction
-
-ecjtu 是一个用 Pythonic 的 ECJTU API SDK，旨在为开发者提供一个简洁、高效的方式来访问和管理其学籍资料、成绩、课表等信息，构建自己的应用程序 🌟。
-
-欢迎校友加入 EFC（ECJTU For Code），我们致力于构建一个充满活力的平台，集结校园内外对技术充满热情的开发者、技术爱好者以及创新思维者。在这里，您可以自由地分享您的编程知识，展示您的创新项目，以及与志同道合的人一起推动开源文化的发展。
-
-
-<div style="width: 250px;margin: 0 auto;">
-    <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/ecjtu_group.png"/>
-</div>
-
-
-
-## 💡 Features
-
-- 获取课程表信息
-- 获取成绩信息
-- 获取绩点信息
-- 获取选修课程信息
-- 提供对应的异步版本
-
-## 📗 Usage
-
-打开终端命令行，输入以下命令：
-
-```shell
-pip install ecjtu
-```
-
-下面将介绍 ECJTU 的基本使用方式，接下来，我们导入 `ECJTU` 类，并构造一个 client 进行登录。
-
-```python
-from ecjtu import ECJTU
-
-client = ECJTU(stud_id="your student id", password="pwd")
-```
-
-如果你的代码会存储在远程仓库中，我们推荐将学号和密码保存在环境变量中，ECJTU 支持以环境变量的方式初始化，下面是两种使用环境变量初始化的方式。
-
-### 方法一
-
-```python
-import os
-from ecjtu import ECJTU
-
-os.environ["ECJTU_STUDENT_ID"] = "xxx"
-os.environ["ECJTU_PASSWORD"] = "xxx"
-
-client = ECJTU()
-```
-
-### 方法二
-使用 [dotenv](https://pypi.org/project/python-dotenv/) 库，将学号和密码保存在 `.env` 文件中，在项目根目录下创建 `.env` 文件，内容如下：
-
-```text
-ECJTU_STUDENT_ID=xxx
-ECJTU_PASSWORD=xxx
-```
-
-然后在代码中使用如下方式初始化 client：
-
-```python
-from dotenv import load_dotenv
-from ecjtu import ECJTU
-
-load_dotenv()
-client = ECJTU()
-```
-
-通过这种方式，你可以避免将学号和密码明文保存在代码中，提高安全性。需要注意的是，不要将 `.env` 文件上传到公共仓库中，应在 `.gitignore` 中声明忽略该文件。
-
-### 查询课程表
-
-使用 client，你可以获取选修的课程、课程表、绩点、成绩等信息。下面的示例展示了如何使用 client 获取今日课表。
-
-
-```python
-from typing import List
-from ecjtu import ScheduledCourse
-
-courses: List[ScheduledCourse] = client.scheduled_courses.today()
-print(courses)
-```
-
-Output Example:
-
-```text
-[ScheduledCourse(class_span='1,2', course='材料力学(B)', course_name='材料力学(B)(20232-1)', week_span='1-15', course_type='必修课', teacher='程俊峰', week_day=5, class_room='31-504', pk_type='上课'), ScheduledCourse(class_span='3,4', course='Java程序设计(B)', course_name='Java程序设计(B)(20232-2)', week_span='1-16', course_type='限选课', teacher='王珏', week_day=5, class_room='31-311D', pk_type='上课'), ScheduledCourse(class_span='5,6', course='数据库系统原理', course_name='数据库系统原理(20232-2)', week_span='1-16', course_type='必修课', teacher='魏永丰', week_day=5, class_room='31-505', pk_type='上课')]
-```
-
-获取本周课表
-
-```python
-courses: List[List[ScheduledCourse]] = client.scheduled_courses.this_week()
-
-for day, courses in enumerate(courses):
-    print(f"星期{day + 1}")
-    for course in courses:
-        print(course)
-```
-
-Output Example:
-
-```text
-星期1
-class_span='3,4' course='工程地质学' course_name='工程地质学(20232-1)' week_span='1-12' course_type='限选课' teacher='黄龙华' week_day=1 class_room='31-510' pk_type='上课'
-星期2
-class_span='5,6' course='软件工程（B）' course_name='软件工程（B）(20232-2)' week_span='1-16' course_type='必修课' teacher='刘冲' week_day=2 class_room='31-313' pk_type='上课'
-星期3
-class_span='3,4' course='材料力学(B)' course_name='材料力学(B)(20232-1)' week_span='1-15' course_type='必修课' teacher='程俊峰' week_day=3 class_room='31-504' pk_type='上课'
-class_span='5,6' course='计算方法(B)' course_name='计算方法(B)(20232-2)' week_span='1-16' course_type='限选课' teacher='邓志刚' week_day=3 class_room='31-503' pk_type='上课'
-class_span='7,8' course='体育IⅤ' course_name='定向越野Ⅳ(20232-1)' week_span='1-16' course_type='必修课' teacher='余振东' week_day=3 class_room='北区田径场3' pk_type='上课'
-星期4
-class_span='3,4' course='材料力学(B)' course_name='材料力学(B)(20232-1)' week_span='8' course_type='必修课' teacher='程俊峰' week_day=4 class_room='材料力学实验室(教9-202、113、114、结108)' pk_type='实验'
-class_span='9,10' course='大学日语Ⅳ' course_name='日语(2022-1)' week_span='1-16' course_type='必修课' teacher='谢幸荣' week_day=4 class_room='25-121' pk_type='上课'
-星期5
-class_span='1,2' course='材料力学(B)' course_name='材料力学(B)(20232-1)' week_span='1-15' course_type='必修课' teacher='程俊峰' week_day=5 class_room='31-504' pk_type='上课'
-class_span='3,4' course='Java程序设计(B)' course_name='Java程序设计(B)(20232-2)' week_span='1-16' course_type='限选课' teacher='王珏' week_day=5 class_room='31-311D' pk_type='上课'
-class_span='5,6' course='数据库系统原理' course_name='数据库系统原理(20232-2)' week_span='1-16' course_type='必修课' teacher='魏永丰' week_day=5 class_room='31-505' pk_type='上课'
-星期6
-星期7
-```
-
-获取指定日期的课程表，日期格式为 `yyyy-mm-dd`
-
-```python
-courses: List[ScheduledCourse] = client.scheduled_courses.filter(date="2023-04-15")
-```
-
-### Score
-
-**获取本学期成绩**
-
-> 事实上，获取的是上个学期的成绩，因为本学期的成绩通常要等到期末才出来。
-
-```python
-from typing import List
-from ecjtu import Score
-
-scores: List[Score] = client.scores.today()
-print(scores)
-```
-
-Output Example:
-
-```text
-[Score(semester='2023.1', course_name='【1500100250】网页动画制作', course_nature='公共任选课【科学技术类】', credit=2.0, grade='优秀'), Score(semester='2023.1', course_name='【1501100020】理论力学（A）', course_nature='必修课', credit=3.5, grade='92'), Score(semester='2023.1', course_name='【1505100033】体育Ⅲ', course_nature='必修课', credit=1.0, grade='93'), Score(semester='2023.1', course_name='【1508100090】概率论与数理统计', course_nature='必修课', credit=3.0, grade='88'), Score(semester='2023.1', course_name='【1509103673】大学日语Ⅲ', course_nature='必修课', credit=2.0, grade='97'), Score(semester='2023.1', course_name='【1514100153】形势与政策Ⅲ', course_nature='必修课', credit=0.5, grade='优秀'), Score(semester='2023.1', course_name='【1521101440】数据结构', course_nature='必修课', credit=3.0, grade='97'), Score(semester='2023.1', course_name='【1521101450】离散数学', course_nature='必修课', credit=3.0, grade='96'), Score(semester='2023.1', course_name='【1521190081】综合课程设计Ⅰ', course_nature='必修课', credit=2.0, grade='优秀')]
-```
-
-**获取指定学期的成绩**，这里的 `2022.1` 代表 2022 年第一学期：
-
-```python
-scores: List[Score] = client.scores.filter(semester="2022.1")
-
-print(scores)
-```
-
-```text
-[Score(semester='2022.1', course_name='【1500100101】职业生涯与发展规划', course_nature='必修课', credit=0.5, grade='优秀'), Score(semester='2022.1', course_name='【1500190090】专业导论', course_nature='必修课', credit=0.0, grade='优秀'), Score(semester='2022.1', course_name='【1500190200】军事技能', course_nature='必修课', credit=1.0, grade='合格'), Score(semester='2022.1', course_name='【1505100031】体育Ⅰ', course_nature='必修课', credit=1.0, grade='99'), Score(semester='2022.1', course_name='【1505101460】国家安全与军事理论', course_nature='必修课', credit=2.0, grade='优秀'), Score(semester='2022.1', course_name='【1508100011】高等数学(A)Ⅰ', course_nature='必修课', credit=6.0, grade='90'), Score(semester='2022.1', course_name='【1508100201】土建工程制图Ⅰ', course_nature='必修课', credit=3.0, grade='85'), Score(semester='2022.1', course_name='【1509103671】大学日语Ⅰ', course_nature='必修课', credit=3.0, grade='90'), Score(semester='2022.1', course_name='【1514100151】形势与政策Ⅰ', course_nature='必修课', credit=0.5, grade='良好'), Score(semester='2022.1', course_name='【1514100170】思想道德与法治', course_nature='必修课', credit=3.0, grade='90'), Score(semester='2022.1', course_name='【1521101220】软件开发基础', course_nature='必修课', credit=4.0, grade='94')]
-```
-
-### GPA
-
-获取当前 GPA
-
-```python
-gpa: GPA = client.gpa.today()
-
-print(gpa)
-```
-
-```text
-student_name='Zeeland' gpa='4.44' status='正常|有学籍'
-```
-
-### 查询选修的课程
-
-```python
-courses = client.elective_courses.today()
-
-for course in courses:
-    print(course)
-```
-
-```text
-semester='2023.2' class_name='创新创业过程与方法(20232-23)【小2班】' class_type='必修课' class_assessment_method='考查' class_info='第1-4周 星期一 第7,8节[31-313]' class_number='19' credit=0.5 teacher='游永忠'
-semester='2023.2' class_name='材料力学(B)(20232-1)【小1班】' class_type='必修课' class_assessment_method='考试' class_info='第1-15周 星期三 第3,4节[31-504]|第1-15周 星期四 第3,4节(双)[31-509]|第1-15周 星期五 第1,2节[31-504]' class_number='11' credit=4.5 teacher='程俊峰'
-semester='2023.2' class_name='工程地质学(20232-1)【小1班】' class_type='限选课' class_assessment_method='考查' class_info='第1-12周 星期一 第3,4节[31-510]' class_number='7' credit=1.5 teacher='黄龙华'
-semester='2023.2' class_name='测量学（A）(20232-2)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='第1-16周 星期二 第3,4节[31-411A]|第1-16周 星期四 第3,4节(单)[31-411A]' class_number='7' credit=3.0 teacher='陈云锅'
-semester='2023.2' class_name='测量实习(A)(20232-8)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='' class_number='7' credit=2.0 teacher='陈云锅'
-semester='2023.2' class_name='形势与政策Ⅳ(20232-53)【小2班】' class_type='必修课' class_assessment_method='考查' class_info='第3-6周 星期四 第5,6节[31-304]' class_number='22' credit=0.5 teacher='周可颐'
-semester='2023.2' class_name='计算方法(B)(20232-2)【小1班】' class_type='限选课' class_assessment_method='考查' class_info='第1-16周 星期三 第5,6节[31-503]' class_number='7' credit=2.0 teacher='邓志刚'
-semester='2023.2' class_name='软件工程（B）(20232-2)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='第1-16周 星期二 第5,6节[31-313]' class_number='7' credit=2.0 teacher='刘冲'
-semester='2023.2' class_name='数据库系统原理(20232-2)【小1班】' class_type='必修课' class_assessment_method='考试' class_info='第1-16周 星期二 第1,2节(单)[31-505]|第1-16周 星期五 第5,6节[31-505]' class_number='12' credit=3.0 teacher='魏永丰'
-semester='2023.2' class_name='Java程序设计(B)(20232-2)【小1班】' class_type='限选课' class_assessment_method='考查' class_info='第1-16周 星期四 第7,8节(单)[31-311E]|第1-16周 星期五 第3,4节[31-311D]' class_number='7' credit=3.0 teacher='王珏'
-semester='2023.2' class_name='综合课程设计Ⅱ(20232-10)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='' class_number='7' credit=2.0 teacher='王珏'
-semester='2023.2' class_name='日语(2022-1)【小3班】' class_type='必修课' class_assessment_method='考试' class_info='第1-16周 星期四 第9,10节[25-121]' class_number='21' credit=2.0 teacher='谢幸荣(1-16)'
-semester='2023.2' class_name='定向越野Ⅳ(20232-1)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='第1-16周 星期三 第7,8节[北区田径场3]' class_number='14' credit=1.0 teacher='余振东'
-```
-
-### 异步版本
-
-异步版本与同步版本的使用方式基本一致，可以使用相同的规范调用，下面是一个简单的示例。
-
-```python
-import asyncio
-
-from ecjtu import AsyncECJTU
-
-client = AsyncECJTU(stud_id="xxx", password="xxx")
-
-
-async def main():
-    courses = await client.scheduled_courses.today()
-    print(courses)
-
-
-asyncio.run(main())
-```
-
-## 🧰 本地开发
-
-欢迎贡献代码与二次开发，你可以通过以下方式安装依赖，推荐使用 Conda 作为环境管理工具，首先创建一个新的环境并激活：
-
-```bash
-conda create -n ecjtu python==3.10
-conda activate ecjtu
-```
-
-激活环境后，你可以安装依赖：
-
-```bash
-pip install poetry
-poetry install
-```
-
-## 🏴󠁧󠁢󠁷󠁬󠁳󠁿 TODO
-
-下面列举了一些未来可能添加的功能，欢迎贡献代码，提出建议。
-
-- [ ] 添加 web 服务器，提供 API 服务
-- [ ] 提供 docker 快速服务部署
-- [ ] 增加考试查询
-
-## 📖 Makefile usage
-
-[`Makefile`](https://github.com/Undertone0809/ecjtu/blob/main/Makefile) contains a lot of functions for faster development.
-
-<details>
-<summary>Install all dependencies and pre-commit hooks</summary>
-<p>
-
-Install requirements:
-
-```bash
-make install
-```
-
-Pre-commit hooks coulb be installed after `git init` via
-
-```bash
-make pre-commit-install
-```
-
-</p>
-</details>
-
-<details>
-<summary>Codestyle and type checks</summary>
-<p>
-
-Automatic format uses `ruff`.
-
-```bash
-make polish-codestyle
-
-# or use synonym
-make format
-```
-
-Codestyle checks only, without rewriting files:
-
-```bash
-make check-codestyle
-```
-
-> Note: `check-codestyle` uses `ruff` and `darglint` library
-
-</p>
-</details>
-
-<details>
-<summary>Code security</summary>
-<p>
-
-> If this command is not selected during installation, it cannnot be used.
-
-```bash
-make check-safety
-```
-
-This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
-
-```bash
-make check-safety
-```
-
-</p>
-</details>
-
-<details>
-<summary>Tests with coverage badges</summary>
-<p>
-
-Run `pytest`
-
-```bash
-make test
-```
-
-</p>
-</details>
-
-<details>
-<summary>All linters</summary>
-<p>
-
-Of course there is a command to run all linters in one:
-
-```bash
-make lint
-```
-
-the same as:
-
-```bash
-make check-codestyle && make test && make check-safety
-```
-
-</p>
-</details>
-
-<details>
-<summary>Docker</summary>
-<p>
-
-```bash
-make docker-build
-```
-
-which is equivalent to:
-
-```bash
-make docker-build VERSION=latest
-```
-
-Remove docker image with
-
-```bash
-make docker-remove
-```
-
-More information [about docker](https://github.com/Undertone0809/python-package-template/tree/main/%7B%7B%20cookiecutter.project_name%20%7D%7D/docker).
-
-</p>
-</details>
-
-<details>
-<summary>Cleanup</summary>
-<p>
-Delete pycache files
-
-```bash
-make pycache-remove
-```
-
-Remove package build
-
-```bash
-make build-remove
-```
-
-Delete .DS_STORE files
-
-```bash
-make dsstore-remove
-```
-
-Remove .mypycache
-
-```bash
-make mypycache-remove
-```
-
-Or to remove all above run:
-
-```bash
-make cleanup
-```
-
-</p>
-</details>
-
-## 📝 Log system
-
-When you run ECJTU, all the logs are stored in a log folder. Promptulate divides the logs by date, which means that each day will have a separate log file.
-
-You can find the logs in the following path:
-
-- windows: `/Users/username/.ecjtu/logs`
-- linux: `/home/username/.ecjtu/logs`
-
-## 🚀 Contributing
-
-Hi there! Thank you for even being interested in contributing to ecjtu. As an open-source project in a rapidly developing field, we are extremely open to contributions, whether they involve new features, improved infrastructure, better documentation, or bug fixes.
-
-See the detail in [CONTRIBUTING.md](./CONTRIBUTING.md)
-
+# ecjtu
+
+<div align="center">
+
+[![Python Version](https://img.shields.io/pypi/pyversions/ecjtu.svg)](https://pypi.org/project/ecjtu/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Undertone0809/ecjtu/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: ruff](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/astral-sh/ruff)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Undertone0809/ecjtu/blob/main/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Undertone0809/ecjtu/releases)
+[![License](https://img.shields.io/github/license/Undertone0809/ecjtu)](https://github.com/Undertone0809/ecjtu/blob/main/LICENSE)
+![Coverage Report](assets/images/coverage.svg)
+
+All your need is ECJTU API SDK service
+
+</div>
+
+## 📚 Introduction
+
+ecjtu 是一个用 Pythonic 的 ECJTU API SDK，旨在为开发者提供一个简洁、高效的方式来访问和管理其学籍资料、成绩、课表等信息，构建自己的应用程序 🌟。
+
+欢迎校友加入 EFC（ECJTU For Code），我们致力于构建一个充满活力的平台，集结校园内外对技术充满热情的开发者、技术爱好者以及创新思维者。在这里，您可以自由地分享您的编程知识，展示您的创新项目，以及与志同道合的人一起推动开源文化的发展。
+
+
+<div style="width: 250px;margin: 0 auto;">
+    <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/ecjtu_group.png"/>
+</div>
+
+
+
+## 💡 Features
+
+- 获取课程表信息
+- 获取成绩信息
+- 获取绩点信息
+- 获取选修课程信息
+- 提供对应的异步版本
+
+## 📗 Usage
+
+打开终端命令行，输入以下命令：
+
+```shell
+pip install ecjtu
+```
+
+下面将介绍 ECJTU 的基本使用方式，接下来，我们导入 `ECJTU` 类，并构造一个 client 进行登录。
+
+```python
+from ecjtu import ECJTU
+
+client = ECJTU(stud_id="your student id", password="pwd")
+```
+
+如果你的代码会存储在远程仓库中，我们推荐将学号和密码保存在环境变量中，ECJTU 支持以环境变量的方式初始化，下面是两种使用环境变量初始化的方式。
+
+### 方法一
+
+```python
+import os
+from ecjtu import ECJTU
+
+os.environ["ECJTU_STUDENT_ID"] = "xxx"
+os.environ["ECJTU_PASSWORD"] = "xxx"
+
+client = ECJTU()
+```
+
+### 方法二
+使用 [dotenv](https://pypi.org/project/python-dotenv/) 库，将学号和密码保存在 `.env` 文件中，在项目根目录下创建 `.env` 文件，内容如下：
+
+```text
+ECJTU_STUDENT_ID=xxx
+ECJTU_PASSWORD=xxx
+```
+
+然后在代码中使用如下方式初始化 client：
+
+```python
+from dotenv import load_dotenv
+from ecjtu import ECJTU
+
+load_dotenv()
+client = ECJTU()
+```
+
+通过这种方式，你可以避免将学号和密码明文保存在代码中，提高安全性。需要注意的是，不要将 `.env` 文件上传到公共仓库中，应在 `.gitignore` 中声明忽略该文件。
+
+### 查询课程表
+
+使用 client，你可以获取选修的课程、课程表、绩点、成绩等信息。下面的示例展示了如何使用 client 获取今日课表。
+
+
+```python
+from typing import List
+from ecjtu import ScheduledCourse
+
+courses: List[ScheduledCourse] = client.scheduled_courses.today()
+print(courses)
+```
+
+Output Example:
+
+```text
+[ScheduledCourse(class_span='1,2', course='材料力学(B)', course_name='材料力学(B)(20232-1)', week_span='1-15', course_type='必修课', teacher='程俊峰', week_day=5, class_room='31-504', pk_type='上课'), ScheduledCourse(class_span='3,4', course='Java程序设计(B)', course_name='Java程序设计(B)(20232-2)', week_span='1-16', course_type='限选课', teacher='王珏', week_day=5, class_room='31-311D', pk_type='上课'), ScheduledCourse(class_span='5,6', course='数据库系统原理', course_name='数据库系统原理(20232-2)', week_span='1-16', course_type='必修课', teacher='魏永丰', week_day=5, class_room='31-505', pk_type='上课')]
+```
+
+获取本周课表
+
+```python
+courses: List[List[ScheduledCourse]] = client.scheduled_courses.this_week()
+
+for day, courses in enumerate(courses):
+    print(f"星期{day + 1}")
+    for course in courses:
+        print(course)
+```
+
+Output Example:
+
+```text
+星期1
+class_span='3,4' course='工程地质学' course_name='工程地质学(20232-1)' week_span='1-12' course_type='限选课' teacher='黄龙华' week_day=1 class_room='31-510' pk_type='上课'
+星期2
+class_span='5,6' course='软件工程（B）' course_name='软件工程（B）(20232-2)' week_span='1-16' course_type='必修课' teacher='刘冲' week_day=2 class_room='31-313' pk_type='上课'
+星期3
+class_span='3,4' course='材料力学(B)' course_name='材料力学(B)(20232-1)' week_span='1-15' course_type='必修课' teacher='程俊峰' week_day=3 class_room='31-504' pk_type='上课'
+class_span='5,6' course='计算方法(B)' course_name='计算方法(B)(20232-2)' week_span='1-16' course_type='限选课' teacher='邓志刚' week_day=3 class_room='31-503' pk_type='上课'
+class_span='7,8' course='体育IⅤ' course_name='定向越野Ⅳ(20232-1)' week_span='1-16' course_type='必修课' teacher='余振东' week_day=3 class_room='北区田径场3' pk_type='上课'
+星期4
+class_span='3,4' course='材料力学(B)' course_name='材料力学(B)(20232-1)' week_span='8' course_type='必修课' teacher='程俊峰' week_day=4 class_room='材料力学实验室(教9-202、113、114、结108)' pk_type='实验'
+class_span='9,10' course='大学日语Ⅳ' course_name='日语(2022-1)' week_span='1-16' course_type='必修课' teacher='谢幸荣' week_day=4 class_room='25-121' pk_type='上课'
+星期5
+class_span='1,2' course='材料力学(B)' course_name='材料力学(B)(20232-1)' week_span='1-15' course_type='必修课' teacher='程俊峰' week_day=5 class_room='31-504' pk_type='上课'
+class_span='3,4' course='Java程序设计(B)' course_name='Java程序设计(B)(20232-2)' week_span='1-16' course_type='限选课' teacher='王珏' week_day=5 class_room='31-311D' pk_type='上课'
+class_span='5,6' course='数据库系统原理' course_name='数据库系统原理(20232-2)' week_span='1-16' course_type='必修课' teacher='魏永丰' week_day=5 class_room='31-505' pk_type='上课'
+星期6
+星期7
+```
+
+获取指定日期的课程表，日期格式为 `yyyy-mm-dd`
+
+```python
+courses: List[ScheduledCourse] = client.scheduled_courses.filter(date="2023-04-15")
+```
+
+### Score
+
+**获取本学期成绩**
+
+> 事实上，获取的是上个学期的成绩，因为本学期的成绩通常要等到期末才出来。
+
+```python
+from typing import List
+from ecjtu import Score
+
+scores: List[Score] = client.scores.today()
+print(scores)
+```
+
+Output Example:
+
+```text
+[Score(semester='2023.1', course_name='【1500100250】网页动画制作', course_nature='公共任选课【科学技术类】', credit=2.0, grade='优秀'), Score(semester='2023.1', course_name='【1501100020】理论力学（A）', course_nature='必修课', credit=3.5, grade='92'), Score(semester='2023.1', course_name='【1505100033】体育Ⅲ', course_nature='必修课', credit=1.0, grade='93'), Score(semester='2023.1', course_name='【1508100090】概率论与数理统计', course_nature='必修课', credit=3.0, grade='88'), Score(semester='2023.1', course_name='【1509103673】大学日语Ⅲ', course_nature='必修课', credit=2.0, grade='97'), Score(semester='2023.1', course_name='【1514100153】形势与政策Ⅲ', course_nature='必修课', credit=0.5, grade='优秀'), Score(semester='2023.1', course_name='【1521101440】数据结构', course_nature='必修课', credit=3.0, grade='97'), Score(semester='2023.1', course_name='【1521101450】离散数学', course_nature='必修课', credit=3.0, grade='96'), Score(semester='2023.1', course_name='【1521190081】综合课程设计Ⅰ', course_nature='必修课', credit=2.0, grade='优秀')]
+```
+
+**获取指定学期的成绩**，这里的 `2022.1` 代表 2022 年第一学期：
+
+```python
+scores: List[Score] = client.scores.filter(semester="2022.1")
+
+print(scores)
+```
+
+```text
+[Score(semester='2022.1', course_name='【1500100101】职业生涯与发展规划', course_nature='必修课', credit=0.5, grade='优秀'), Score(semester='2022.1', course_name='【1500190090】专业导论', course_nature='必修课', credit=0.0, grade='优秀'), Score(semester='2022.1', course_name='【1500190200】军事技能', course_nature='必修课', credit=1.0, grade='合格'), Score(semester='2022.1', course_name='【1505100031】体育Ⅰ', course_nature='必修课', credit=1.0, grade='99'), Score(semester='2022.1', course_name='【1505101460】国家安全与军事理论', course_nature='必修课', credit=2.0, grade='优秀'), Score(semester='2022.1', course_name='【1508100011】高等数学(A)Ⅰ', course_nature='必修课', credit=6.0, grade='90'), Score(semester='2022.1', course_name='【1508100201】土建工程制图Ⅰ', course_nature='必修课', credit=3.0, grade='85'), Score(semester='2022.1', course_name='【1509103671】大学日语Ⅰ', course_nature='必修课', credit=3.0, grade='90'), Score(semester='2022.1', course_name='【1514100151】形势与政策Ⅰ', course_nature='必修课', credit=0.5, grade='良好'), Score(semester='2022.1', course_name='【1514100170】思想道德与法治', course_nature='必修课', credit=3.0, grade='90'), Score(semester='2022.1', course_name='【1521101220】软件开发基础', course_nature='必修课', credit=4.0, grade='94')]
+```
+
+### GPA
+
+获取当前 GPA
+
+```python
+gpa: GPA = client.gpa.today()
+
+print(gpa)
+```
+
+```text
+student_name='Zeeland' gpa='4.44' status='正常|有学籍'
+```
+
+### 查询选修的课程
+
+```python
+courses = client.elective_courses.today()
+
+for course in courses:
+    print(course)
+```
+
+```text
+semester='2023.2' class_name='创新创业过程与方法(20232-23)【小2班】' class_type='必修课' class_assessment_method='考查' class_info='第1-4周 星期一 第7,8节[31-313]' class_number='19' credit=0.5 teacher='游永忠'
+semester='2023.2' class_name='材料力学(B)(20232-1)【小1班】' class_type='必修课' class_assessment_method='考试' class_info='第1-15周 星期三 第3,4节[31-504]|第1-15周 星期四 第3,4节(双)[31-509]|第1-15周 星期五 第1,2节[31-504]' class_number='11' credit=4.5 teacher='程俊峰'
+semester='2023.2' class_name='工程地质学(20232-1)【小1班】' class_type='限选课' class_assessment_method='考查' class_info='第1-12周 星期一 第3,4节[31-510]' class_number='7' credit=1.5 teacher='黄龙华'
+semester='2023.2' class_name='测量学（A）(20232-2)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='第1-16周 星期二 第3,4节[31-411A]|第1-16周 星期四 第3,4节(单)[31-411A]' class_number='7' credit=3.0 teacher='陈云锅'
+semester='2023.2' class_name='测量实习(A)(20232-8)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='' class_number='7' credit=2.0 teacher='陈云锅'
+semester='2023.2' class_name='形势与政策Ⅳ(20232-53)【小2班】' class_type='必修课' class_assessment_method='考查' class_info='第3-6周 星期四 第5,6节[31-304]' class_number='22' credit=0.5 teacher='周可颐'
+semester='2023.2' class_name='计算方法(B)(20232-2)【小1班】' class_type='限选课' class_assessment_method='考查' class_info='第1-16周 星期三 第5,6节[31-503]' class_number='7' credit=2.0 teacher='邓志刚'
+semester='2023.2' class_name='软件工程（B）(20232-2)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='第1-16周 星期二 第5,6节[31-313]' class_number='7' credit=2.0 teacher='刘冲'
+semester='2023.2' class_name='数据库系统原理(20232-2)【小1班】' class_type='必修课' class_assessment_method='考试' class_info='第1-16周 星期二 第1,2节(单)[31-505]|第1-16周 星期五 第5,6节[31-505]' class_number='12' credit=3.0 teacher='魏永丰'
+semester='2023.2' class_name='Java程序设计(B)(20232-2)【小1班】' class_type='限选课' class_assessment_method='考查' class_info='第1-16周 星期四 第7,8节(单)[31-311E]|第1-16周 星期五 第3,4节[31-311D]' class_number='7' credit=3.0 teacher='王珏'
+semester='2023.2' class_name='综合课程设计Ⅱ(20232-10)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='' class_number='7' credit=2.0 teacher='王珏'
+semester='2023.2' class_name='日语(2022-1)【小3班】' class_type='必修课' class_assessment_method='考试' class_info='第1-16周 星期四 第9,10节[25-121]' class_number='21' credit=2.0 teacher='谢幸荣(1-16)'
+semester='2023.2' class_name='定向越野Ⅳ(20232-1)【小1班】' class_type='必修课' class_assessment_method='考查' class_info='第1-16周 星期三 第7,8节[北区田径场3]' class_number='14' credit=1.0 teacher='余振东'
+```
+
+### 异步版本
+
+异步版本与同步版本的使用方式基本一致，可以使用相同的规范调用，下面是一个简单的示例。
+
+```python
+import asyncio
+
+from ecjtu import AsyncECJTU
+
+client = AsyncECJTU(stud_id="xxx", password="xxx")
+
+
+async def main():
+    courses = await client.scheduled_courses.today()
+    print(courses)
+
+
+asyncio.run(main())
+```
+
+## 🧰 本地开发
+
+欢迎贡献代码与二次开发，你可以通过以下方式安装依赖，推荐使用 Conda 作为环境管理工具，首先创建一个新的环境并激活：
+
+```bash
+conda create -n ecjtu python==3.10
+conda activate ecjtu
+```
+
+激活环境后，你可以安装依赖：
+
+```bash
+pip install poetry
+poetry install
+```
+
+## 🏴󠁧󠁢󠁷󠁬󠁳󠁿 TODO
+
+下面列举了一些未来可能添加的功能，欢迎贡献代码，提出建议。
+
+- [ ] 添加 web 服务器，提供 API 服务
+- [ ] 提供 docker 快速服务部署
+- [ ] 增加考试查询
+
+## 📖 Makefile usage
+
+[`Makefile`](https://github.com/Undertone0809/ecjtu/blob/main/Makefile) contains a lot of functions for faster development.
+
+<details>
+<summary>Install all dependencies and pre-commit hooks</summary>
+<p>
+
+Install requirements:
+
+```bash
+make install
+```
+
+Pre-commit hooks coulb be installed after `git init` via
+
+```bash
+make pre-commit-install
+```
+
+</p>
+</details>
+
+<details>
+<summary>Codestyle and type checks</summary>
+<p>
+
+Automatic format uses `ruff`.
+
+```bash
+make polish-codestyle
+
+# or use synonym
+make format
+```
+
+Codestyle checks only, without rewriting files:
+
+```bash
+make check-codestyle
+```
+
+> Note: `check-codestyle` uses `ruff` and `darglint` library
+
+</p>
+</details>
+
+<details>
+<summary>Code security</summary>
+<p>
+
+> If this command is not selected during installation, it cannnot be used.
+
+```bash
+make check-safety
+```
+
+This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
+
+```bash
+make check-safety
+```
+
+</p>
+</details>
+
+<details>
+<summary>Tests with coverage badges</summary>
+<p>
+
+Run `pytest`
+
+```bash
+make test
+```
+
+</p>
+</details>
+
+<details>
+<summary>All linters</summary>
+<p>
+
+Of course there is a command to run all linters in one:
+
+```bash
+make lint
+```
+
+the same as:
+
+```bash
+make check-codestyle && make test && make check-safety
+```
+
+</p>
+</details>
+
+<details>
+<summary>Docker</summary>
+<p>
+
+```bash
+make docker-build
+```
+
+which is equivalent to:
+
+```bash
+make docker-build VERSION=latest
+```
+
+Remove docker image with
+
+```bash
+make docker-remove
+```
+
+More information [about docker](https://github.com/Undertone0809/python-package-template/tree/main/%7B%7B%20cookiecutter.project_name%20%7D%7D/docker).
+
+</p>
+</details>
+
+<details>
+<summary>Cleanup</summary>
+<p>
+Delete pycache files
+
+```bash
+make pycache-remove
+```
+
+Remove package build
+
+```bash
+make build-remove
+```
+
+Delete .DS_STORE files
+
+```bash
+make dsstore-remove
+```
+
+Remove .mypycache
+
+```bash
+make mypycache-remove
+```
+
+Or to remove all above run:
+
+```bash
+make cleanup
+```
+
+</p>
+</details>
+
+## 📝 Log system
+
+When you run ECJTU, all the logs are stored in a log folder. Promptulate divides the logs by date, which means that each day will have a separate log file.
+
+You can find the logs in the following path:
+
+- windows: `/Users/username/.ecjtu/logs`
+- linux: `/home/username/.ecjtu/logs`
+
+## 🚀 Contributing
+
+Hi there! Thank you for even being interested in contributing to ecjtu. As an open-source project in a rapidly developing field, we are extremely open to contributions, whether they involve new features, improved infrastructure, better documentation, or bug fixes.
+
+See the detail in [CONTRIBUTING.md](./CONTRIBUTING.md)
+
 For more information, please contact: [zeeland4work@gmail.com](mailto:zeeland4work@gmail.com)
```

### Comparing `ecjtu-0.0.1/PKG-INFO` & `ecjtu-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecjtu
-Version: 0.0.1
+Version: 0.1.0
 Summary: ECJTU API SDK service
 Home-page: https://github.com/Undertone0809/ecjtu
 License: MIT
 Author: ecjtu
 Author-email: zeeland4work@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
```

