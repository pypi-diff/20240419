# Comparing `tmp/fastapi_jwt_auth_md-0.5.0.tar.gz` & `tmp/fastapi_jwt_auth_md-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_jwt_auth_md-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_jwt_auth_md-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_jwt_auth_md-0.5.0.tar` & `fastapi_jwt_auth_md-1.0.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      396 2024-04-19 15:15:23.429025 fastapi_jwt_auth_md-0.5.0/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      662 2024-04-19 15:15:23.429190 fastapi_jwt_auth_md-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      321 2024-04-19 15:27:13.243688 fastapi_jwt_auth_md-0.5.0/.gitignore
--rw-r--r--   0        0        0     1458 2024-04-19 15:15:23.429458 fastapi_jwt_auth_md-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2024-04-19 15:15:23.429587 fastapi_jwt_auth_md-0.5.0/LICENSE
--rw-r--r--   0        0        0     1848 2024-04-19 15:15:23.429721 fastapi_jwt_auth_md-0.5.0/README.md
--rw-r--r--   0        0        0      866 2024-04-19 15:15:23.430183 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/additional-claims.md
--rw-r--r--   0        0        0      272 2024-04-19 15:15:23.430336 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/asymmetric.md
--rw-r--r--   0        0        0     1013 2024-04-19 15:15:23.430468 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/bigger-app.md
--rw-r--r--   0        0        0      502 2024-04-19 15:15:23.430599 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/dynamic-algorithm.md
--rw-r--r--   0        0        0      927 2024-04-19 15:15:23.430731 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/dynamic-expires.md
--rw-r--r--   0        0        0      389 2024-04-19 15:15:23.430856 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/generate-docs.md
--rw-r--r--   0        0        0     1745 2024-04-19 15:15:23.430989 fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/websocket.md
--rw-r--r--   0        0        0     8726 2024-04-19 15:15:23.431178 fastapi_jwt_auth_md-0.5.0/docs/api-doc.md
--rw-r--r--   0        0        0     1588 2024-04-19 15:15:23.431504 fastapi_jwt_auth_md-0.5.0/docs/configuration/cookies.md
--rw-r--r--   0        0        0      930 2024-04-19 15:15:23.431652 fastapi_jwt_auth_md-0.5.0/docs/configuration/csrf.md
--rw-r--r--   0        0        0      346 2024-04-19 15:15:23.431792 fastapi_jwt_auth_md-0.5.0/docs/configuration/denylist.md
--rw-r--r--   0        0        0     2163 2024-04-19 15:15:23.431930 fastapi_jwt_auth_md-0.5.0/docs/configuration/general.md
--rw-r--r--   0        0        0      375 2024-04-19 15:15:23.432062 fastapi_jwt_auth_md-0.5.0/docs/configuration/headers.md
--rw-r--r--   0        0        0     3891 2024-04-19 15:15:23.432215 fastapi_jwt_auth_md-0.5.0/docs/contributing.md
--rw-r--r--   0        0        0      309 2024-04-19 15:15:23.432405 fastapi_jwt_auth_md-0.5.0/docs/css/custom.css
--rw-r--r--   0        0        0       17 2024-04-19 15:15:23.432524 fastapi_jwt_auth_md-0.5.0/docs/index.md
--rw-r--r--   0        0        0       20 2024-04-19 15:15:23.432656 fastapi_jwt_auth_md-0.5.0/docs/release-notes.md
--rw-r--r--   0        0        0     1510 2024-04-19 15:15:23.432876 fastapi_jwt_auth_md-0.5.0/docs/usage/basic.md
--rw-r--r--   0        0        0      849 2024-04-19 15:15:23.433029 fastapi_jwt_auth_md-0.5.0/docs/usage/freshness.md
--rw-r--r--   0        0        0     3311 2024-04-19 15:15:23.433164 fastapi_jwt_auth_md-0.5.0/docs/usage/jwt-in-cookies.md
--rw-r--r--   0        0        0      387 2024-04-19 15:15:23.433297 fastapi_jwt_auth_md-0.5.0/docs/usage/optional.md
--rw-r--r--   0        0        0      975 2024-04-19 15:15:23.433435 fastapi_jwt_auth_md-0.5.0/docs/usage/refresh.md
--rw-r--r--   0        0        0     1319 2024-04-19 15:15:23.433565 fastapi_jwt_auth_md-0.5.0/docs/usage/revoking.md
--rw-r--r--   0        0        0     1447 2024-04-19 15:23:38.488480 fastapi_jwt_auth_md-0.5.0/examples/additional_claims.py
--rw-r--r--   0        0        0     2948 2024-04-19 15:15:23.434027 fastapi_jwt_auth_md-0.5.0/examples/asymmetric.py
--rw-r--r--   0        0        0     1764 2024-04-19 15:15:23.434248 fastapi_jwt_auth_md-0.5.0/examples/basic.py
--rw-r--r--   0        0        0     3176 2024-04-19 15:15:23.434395 fastapi_jwt_auth_md-0.5.0/examples/csrf_protection_cookies.py
--rw-r--r--   0        0        0     2991 2024-04-19 15:15:23.434531 fastapi_jwt_auth_md-0.5.0/examples/denylist.py
--rw-r--r--   0        0        0     3434 2024-04-19 15:15:23.434679 fastapi_jwt_auth_md-0.5.0/examples/denylist_redis.py
--rw-r--r--   0        0        0     1979 2024-04-19 15:15:23.434827 fastapi_jwt_auth_md-0.5.0/examples/dynamic_algorithm.py
--rw-r--r--   0        0        0     3144 2024-04-19 15:15:23.434965 fastapi_jwt_auth_md-0.5.0/examples/freshness.py
--rw-r--r--   0        0        0     2520 2024-04-19 15:15:23.435094 fastapi_jwt_auth_md-0.5.0/examples/generate_doc.py
--rw-r--r--   0        0        0     2793 2024-04-19 15:15:23.435225 fastapi_jwt_auth_md-0.5.0/examples/jwt_in_cookies.py
--rw-r--r--   0        0        0        0 2024-04-19 15:15:23.435367 fastapi_jwt_auth_md-0.5.0/examples/multiple_files/__init__.py
--rw-r--r--   0        0        0      704 2024-04-19 15:15:23.435518 fastapi_jwt_auth_md-0.5.0/examples/multiple_files/app.py
--rw-r--r--   0        0        0        0 2024-04-19 15:15:23.435661 fastapi_jwt_auth_md-0.5.0/examples/multiple_files/routers/__init__.py
--rw-r--r--   0        0        0      293 2024-04-19 15:23:38.488790 fastapi_jwt_auth_md-0.5.0/examples/multiple_files/routers/items.py
--rw-r--r--   0        0        0      537 2024-04-19 15:15:23.435954 fastapi_jwt_auth_md-0.5.0/examples/multiple_files/routers/users.py
--rw-r--r--   0        0        0     1278 2024-04-19 15:15:23.436082 fastapi_jwt_auth_md-0.5.0/examples/optional.py
--rw-r--r--   0        0        0     1993 2024-04-19 15:15:23.436214 fastapi_jwt_auth_md-0.5.0/examples/refresh.py
--rw-r--r--   0        0        0     2869 2024-04-19 15:15:23.436346 fastapi_jwt_auth_md-0.5.0/examples/websocket.py
--rw-r--r--   0        0        0     2787 2024-04-19 15:15:23.436478 fastapi_jwt_auth_md-0.5.0/examples/websocket_cookie.py
--rw-r--r--   0        0        0      147 2024-04-19 15:23:38.489425 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/__init__.py
--rw-r--r--   0        0        0     4949 2024-04-19 15:26:54.486107 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/auth_config.py
--rw-r--r--   0        0        0    35248 2024-04-19 15:23:38.490251 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/auth_jwt.py
--rw-r--r--   0        0        0     4083 2024-04-19 15:23:38.490755 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/config.py
--rw-r--r--   0        0        0     2218 2024-04-19 15:23:38.490950 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/exceptions.py
--rw-r--r--   0        0        0      147 2024-04-19 15:42:37.832747 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/__init__.py
--rw-r--r--   0        0        0     4949 2024-04-19 15:42:37.833577 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/auth_config.py
--rw-r--r--   0        0        0    35248 2024-04-19 15:42:37.834712 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/auth_jwt.py
--rw-r--r--   0        0        0     4083 2024-04-19 15:42:37.835380 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/config.py
--rw-r--r--   0        0        0     2218 2024-04-19 15:42:37.835925 fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/exceptions.py
--rw-r--r--   0        0        0     1914 2024-04-19 15:15:23.437577 fastapi_jwt_auth_md-0.5.0/mkdocs.yml
--rw-r--r--   0        0        0     1326 2024-04-19 15:42:53.032837 fastapi_jwt_auth_md-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0       50 2024-04-19 15:15:23.437918 fastapi_jwt_auth_md-0.5.0/scripts/docs-live.sh
--rwxr-xr-x   0        0        0       87 2024-04-19 15:15:23.438072 fastapi_jwt_auth_md-0.5.0/scripts/tests.sh
--rw-r--r--   0        0        0        0 2024-04-19 15:15:23.438213 fastapi_jwt_auth_md-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      122 2024-04-19 15:23:38.491498 fastapi_jwt_auth_md-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      883 2024-04-19 15:15:23.438481 fastapi_jwt_auth_md-0.5.0/tests/private_key.txt
--rw-r--r--   0        0        0      272 2024-04-19 15:15:23.438601 fastapi_jwt_auth_md-0.5.0/tests/public_key.txt
--rw-r--r--   0        0        0    16626 2024-04-19 15:15:23.438774 fastapi_jwt_auth_md-0.5.0/tests/test_config.py
--rw-r--r--   0        0        0    16223 2024-04-19 15:15:23.439023 fastapi_jwt_auth_md-0.5.0/tests/test_cookies.py
--rw-r--r--   0        0        0     4957 2024-04-19 15:15:23.439178 fastapi_jwt_auth_md-0.5.0/tests/test_create_token.py
--rw-r--r--   0        0        0    10475 2024-04-19 15:15:23.439452 fastapi_jwt_auth_md-0.5.0/tests/test_decode_token.py
--rw-r--r--   0        0        0     3205 2024-04-19 15:15:23.439612 fastapi_jwt_auth_md-0.5.0/tests/test_denylist.py
--rw-r--r--   0        0        0     6038 2024-04-19 15:15:23.439789 fastapi_jwt_auth_md-0.5.0/tests/test_headers.py
--rw-r--r--   0        0        0     2586 2024-04-19 15:15:23.439936 fastapi_jwt_auth_md-0.5.0/tests/test_token_multiple_locations.py
--rw-r--r--   0        0        0     3911 2024-04-19 15:15:23.440065 fastapi_jwt_auth_md-0.5.0/tests/test_url_protected.py
--rw-r--r--   0        0        0    13495 2024-04-19 15:15:23.440275 fastapi_jwt_auth_md-0.5.0/tests/test_websocket.py
--rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 fastapi_jwt_auth_md-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      396 2024-04-19 15:15:23.429025 fastapi_jwt_auth_md-1.0.0/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      662 2024-04-19 15:15:23.429190 fastapi_jwt_auth_md-1.0.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      321 2024-04-19 15:27:13.243688 fastapi_jwt_auth_md-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1458 2024-04-19 15:15:23.429458 fastapi_jwt_auth_md-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2024-04-19 15:15:23.429587 fastapi_jwt_auth_md-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1848 2024-04-19 15:15:23.429721 fastapi_jwt_auth_md-1.0.0/README.md
+-rw-r--r--   0        0        0      866 2024-04-19 15:15:23.430183 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/additional-claims.md
+-rw-r--r--   0        0        0      272 2024-04-19 15:15:23.430336 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/asymmetric.md
+-rw-r--r--   0        0        0     1013 2024-04-19 15:15:23.430468 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/bigger-app.md
+-rw-r--r--   0        0        0      502 2024-04-19 15:15:23.430599 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/dynamic-algorithm.md
+-rw-r--r--   0        0        0      927 2024-04-19 15:15:23.430731 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/dynamic-expires.md
+-rw-r--r--   0        0        0      389 2024-04-19 15:15:23.430856 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/generate-docs.md
+-rw-r--r--   0        0        0     1745 2024-04-19 15:15:23.430989 fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/websocket.md
+-rw-r--r--   0        0        0     8726 2024-04-19 15:15:23.431178 fastapi_jwt_auth_md-1.0.0/docs/api-doc.md
+-rw-r--r--   0        0        0     1588 2024-04-19 15:15:23.431504 fastapi_jwt_auth_md-1.0.0/docs/configuration/cookies.md
+-rw-r--r--   0        0        0      930 2024-04-19 15:15:23.431652 fastapi_jwt_auth_md-1.0.0/docs/configuration/csrf.md
+-rw-r--r--   0        0        0      346 2024-04-19 15:15:23.431792 fastapi_jwt_auth_md-1.0.0/docs/configuration/denylist.md
+-rw-r--r--   0        0        0     2163 2024-04-19 15:15:23.431930 fastapi_jwt_auth_md-1.0.0/docs/configuration/general.md
+-rw-r--r--   0        0        0      375 2024-04-19 15:15:23.432062 fastapi_jwt_auth_md-1.0.0/docs/configuration/headers.md
+-rw-r--r--   0        0        0     3891 2024-04-19 15:15:23.432215 fastapi_jwt_auth_md-1.0.0/docs/contributing.md
+-rw-r--r--   0        0        0      309 2024-04-19 15:15:23.432405 fastapi_jwt_auth_md-1.0.0/docs/css/custom.css
+-rw-r--r--   0        0        0       17 2024-04-19 15:15:23.432524 fastapi_jwt_auth_md-1.0.0/docs/index.md
+-rw-r--r--   0        0        0       20 2024-04-19 15:15:23.432656 fastapi_jwt_auth_md-1.0.0/docs/release-notes.md
+-rw-r--r--   0        0        0     1510 2024-04-19 15:15:23.432876 fastapi_jwt_auth_md-1.0.0/docs/usage/basic.md
+-rw-r--r--   0        0        0      849 2024-04-19 15:15:23.433029 fastapi_jwt_auth_md-1.0.0/docs/usage/freshness.md
+-rw-r--r--   0        0        0     3311 2024-04-19 15:15:23.433164 fastapi_jwt_auth_md-1.0.0/docs/usage/jwt-in-cookies.md
+-rw-r--r--   0        0        0      387 2024-04-19 15:15:23.433297 fastapi_jwt_auth_md-1.0.0/docs/usage/optional.md
+-rw-r--r--   0        0        0      975 2024-04-19 15:15:23.433435 fastapi_jwt_auth_md-1.0.0/docs/usage/refresh.md
+-rw-r--r--   0        0        0     1319 2024-04-19 15:15:23.433565 fastapi_jwt_auth_md-1.0.0/docs/usage/revoking.md
+-rw-r--r--   0        0        0     1447 2024-04-19 15:23:38.488480 fastapi_jwt_auth_md-1.0.0/examples/additional_claims.py
+-rw-r--r--   0        0        0     2948 2024-04-19 15:15:23.434027 fastapi_jwt_auth_md-1.0.0/examples/asymmetric.py
+-rw-r--r--   0        0        0     1764 2024-04-19 15:15:23.434248 fastapi_jwt_auth_md-1.0.0/examples/basic.py
+-rw-r--r--   0        0        0     3176 2024-04-19 15:15:23.434395 fastapi_jwt_auth_md-1.0.0/examples/csrf_protection_cookies.py
+-rw-r--r--   0        0        0     2991 2024-04-19 15:15:23.434531 fastapi_jwt_auth_md-1.0.0/examples/denylist.py
+-rw-r--r--   0        0        0     3434 2024-04-19 15:15:23.434679 fastapi_jwt_auth_md-1.0.0/examples/denylist_redis.py
+-rw-r--r--   0        0        0     1979 2024-04-19 15:15:23.434827 fastapi_jwt_auth_md-1.0.0/examples/dynamic_algorithm.py
+-rw-r--r--   0        0        0     3144 2024-04-19 15:15:23.434965 fastapi_jwt_auth_md-1.0.0/examples/freshness.py
+-rw-r--r--   0        0        0     2520 2024-04-19 15:15:23.435094 fastapi_jwt_auth_md-1.0.0/examples/generate_doc.py
+-rw-r--r--   0        0        0     2793 2024-04-19 15:15:23.435225 fastapi_jwt_auth_md-1.0.0/examples/jwt_in_cookies.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:15:23.435367 fastapi_jwt_auth_md-1.0.0/examples/multiple_files/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-19 15:15:23.435518 fastapi_jwt_auth_md-1.0.0/examples/multiple_files/app.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:15:23.435661 fastapi_jwt_auth_md-1.0.0/examples/multiple_files/routers/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-19 15:23:38.488790 fastapi_jwt_auth_md-1.0.0/examples/multiple_files/routers/items.py
+-rw-r--r--   0        0        0      537 2024-04-19 15:15:23.435954 fastapi_jwt_auth_md-1.0.0/examples/multiple_files/routers/users.py
+-rw-r--r--   0        0        0     1278 2024-04-19 15:15:23.436082 fastapi_jwt_auth_md-1.0.0/examples/optional.py
+-rw-r--r--   0        0        0     1993 2024-04-19 15:15:23.436214 fastapi_jwt_auth_md-1.0.0/examples/refresh.py
+-rw-r--r--   0        0        0     2869 2024-04-19 15:15:23.436346 fastapi_jwt_auth_md-1.0.0/examples/websocket.py
+-rw-r--r--   0        0        0     2787 2024-04-19 15:15:23.436478 fastapi_jwt_auth_md-1.0.0/examples/websocket_cookie.py
+-rw-r--r--   0        0        0      147 2024-04-19 15:23:38.489425 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/__init__.py
+-rw-r--r--   0        0        0     4949 2024-04-19 15:26:54.486107 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/auth_config.py
+-rw-r--r--   0        0        0    35248 2024-04-19 15:23:38.490251 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/auth_jwt.py
+-rw-r--r--   0        0        0     4083 2024-04-19 15:23:38.490755 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/config.py
+-rw-r--r--   0        0        0     2218 2024-04-19 15:23:38.490950 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/exceptions.py
+-rw-r--r--   0        0        0      147 2024-04-19 15:47:45.516278 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/__init__.py
+-rw-r--r--   0        0        0     4952 2024-04-19 15:45:25.965018 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/auth_config.py
+-rw-r--r--   0        0        0    35254 2024-04-19 15:45:37.509714 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/auth_jwt.py
+-rw-r--r--   0        0        0     4083 2024-04-19 15:42:37.835380 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/config.py
+-rw-r--r--   0        0        0     2221 2024-04-19 15:46:00.917700 fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/exceptions.py
+-rw-r--r--   0        0        0     1914 2024-04-19 15:15:23.437577 fastapi_jwt_auth_md-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0     1326 2024-04-19 15:47:29.934936 fastapi_jwt_auth_md-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0       50 2024-04-19 15:15:23.437918 fastapi_jwt_auth_md-1.0.0/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0       87 2024-04-19 15:15:23.438072 fastapi_jwt_auth_md-1.0.0/scripts/tests.sh
+-rw-r--r--   0        0        0        0 2024-04-19 15:15:23.438213 fastapi_jwt_auth_md-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-19 15:23:38.491498 fastapi_jwt_auth_md-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      883 2024-04-19 15:15:23.438481 fastapi_jwt_auth_md-1.0.0/tests/private_key.txt
+-rw-r--r--   0        0        0      272 2024-04-19 15:15:23.438601 fastapi_jwt_auth_md-1.0.0/tests/public_key.txt
+-rw-r--r--   0        0        0    16626 2024-04-19 15:15:23.438774 fastapi_jwt_auth_md-1.0.0/tests/test_config.py
+-rw-r--r--   0        0        0    16223 2024-04-19 15:15:23.439023 fastapi_jwt_auth_md-1.0.0/tests/test_cookies.py
+-rw-r--r--   0        0        0     4957 2024-04-19 15:15:23.439178 fastapi_jwt_auth_md-1.0.0/tests/test_create_token.py
+-rw-r--r--   0        0        0    10475 2024-04-19 15:15:23.439452 fastapi_jwt_auth_md-1.0.0/tests/test_decode_token.py
+-rw-r--r--   0        0        0     3205 2024-04-19 15:15:23.439612 fastapi_jwt_auth_md-1.0.0/tests/test_denylist.py
+-rw-r--r--   0        0        0     6038 2024-04-19 15:15:23.439789 fastapi_jwt_auth_md-1.0.0/tests/test_headers.py
+-rw-r--r--   0        0        0     2586 2024-04-19 15:15:23.439936 fastapi_jwt_auth_md-1.0.0/tests/test_token_multiple_locations.py
+-rw-r--r--   0        0        0     3911 2024-04-19 15:15:23.440065 fastapi_jwt_auth_md-1.0.0/tests/test_url_protected.py
+-rw-r--r--   0        0        0    13495 2024-04-19 15:15:23.440275 fastapi_jwt_auth_md-1.0.0/tests/test_websocket.py
+-rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 fastapi_jwt_auth_md-1.0.0/PKG-INFO
```

### Comparing `fastapi_jwt_auth_md-0.5.0/.github/workflows/tests.yml` & `fastapi_jwt_auth_md-1.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/CHANGELOG.md` & `fastapi_jwt_auth_md-1.0.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/LICENSE` & `fastapi_jwt_auth_md-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/README.md` & `fastapi_jwt_auth_md-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/additional-claims.md` & `fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/additional-claims.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/bigger-app.md` & `fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/bigger-app.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/dynamic-expires.md` & `fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/dynamic-expires.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/advanced-usage/websocket.md` & `fastapi_jwt_auth_md-1.0.0/docs/advanced-usage/websocket.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/api-doc.md` & `fastapi_jwt_auth_md-1.0.0/docs/api-doc.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/configuration/cookies.md` & `fastapi_jwt_auth_md-1.0.0/docs/configuration/cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/configuration/csrf.md` & `fastapi_jwt_auth_md-1.0.0/docs/configuration/csrf.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/configuration/general.md` & `fastapi_jwt_auth_md-1.0.0/docs/configuration/general.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/contributing.md` & `fastapi_jwt_auth_md-1.0.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/usage/basic.md` & `fastapi_jwt_auth_md-1.0.0/docs/usage/basic.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/usage/freshness.md` & `fastapi_jwt_auth_md-1.0.0/docs/usage/freshness.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/usage/jwt-in-cookies.md` & `fastapi_jwt_auth_md-1.0.0/docs/usage/jwt-in-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/usage/refresh.md` & `fastapi_jwt_auth_md-1.0.0/docs/usage/refresh.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/docs/usage/revoking.md` & `fastapi_jwt_auth_md-1.0.0/docs/usage/revoking.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/additional_claims.py` & `fastapi_jwt_auth_md-1.0.0/examples/additional_claims.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/asymmetric.py` & `fastapi_jwt_auth_md-1.0.0/examples/asymmetric.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/basic.py` & `fastapi_jwt_auth_md-1.0.0/examples/basic.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/csrf_protection_cookies.py` & `fastapi_jwt_auth_md-1.0.0/examples/csrf_protection_cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/denylist.py` & `fastapi_jwt_auth_md-1.0.0/examples/denylist.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/denylist_redis.py` & `fastapi_jwt_auth_md-1.0.0/examples/denylist_redis.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/dynamic_algorithm.py` & `fastapi_jwt_auth_md-1.0.0/examples/dynamic_algorithm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/freshness.py` & `fastapi_jwt_auth_md-1.0.0/examples/freshness.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/generate_doc.py` & `fastapi_jwt_auth_md-1.0.0/examples/generate_doc.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/jwt_in_cookies.py` & `fastapi_jwt_auth_md-1.0.0/examples/jwt_in_cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/multiple_files/app.py` & `fastapi_jwt_auth_md-1.0.0/examples/multiple_files/app.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/multiple_files/routers/users.py` & `fastapi_jwt_auth_md-1.0.0/examples/multiple_files/routers/users.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/optional.py` & `fastapi_jwt_auth_md-1.0.0/examples/optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/refresh.py` & `fastapi_jwt_auth_md-1.0.0/examples/refresh.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/websocket.py` & `fastapi_jwt_auth_md-1.0.0/examples/websocket.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/examples/websocket_cookie.py` & `fastapi_jwt_auth_md-1.0.0/examples/websocket_cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/auth_config.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/auth_jwt.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/config.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth/exceptions.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/auth_config.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/auth_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fastapi_jwt_auth.config import LoadConfig
+from fastapi_jwt_auth_md.config import LoadConfig
 from pydantic.v1 import ValidationError
 from typing import Callable, List
 from datetime import timedelta
 
 class AuthConfig:
     _token = None
     _token_location = {'headers'}
```

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/auth_jwt.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/auth_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jwt, re, uuid, hmac
 from jwt.algorithms import requires_cryptography, has_crypto
 from datetime import datetime, timezone, timedelta
 from typing import Optional, Dict, Union, Sequence
 from fastapi import Request, Response, WebSocket
-from fastapi_jwt_auth.auth_config import AuthConfig
-from fastapi_jwt_auth.exceptions import (
+from fastapi_jwt_auth_md.auth_config import AuthConfig
+from fastapi_jwt_auth_md.exceptions import (
     InvalidHeaderError,
     CSRFError,
     JWTDecodeError,
     RevokedTokenError,
     MissingTokenError,
     AccessTokenRequired,
     RefreshTokenRequired,
```

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/config.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/fastapi_jwt_auth_md/exceptions.py` & `fastapi_jwt_auth_md-1.0.0/fastapi_jwt_auth_md/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class AuthJWTException(Exception):
     """
-    Base except which all fastapi_jwt_auth errors extend
+    Base except which all fastapi_jwt_auth_md errors extend
     """
     pass
 
 class InvalidHeaderError(AuthJWTException):
     """
     An error getting jwt in header or jwt header information from a request
     """
```

### Comparing `fastapi_jwt_auth_md-0.5.0/mkdocs.yml` & `fastapi_jwt_auth_md-1.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/pyproject.toml` & `fastapi_jwt_auth_md-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "fastapi_jwt_auth_md"
-dist-name = "fastapi-jwt-auth_md"
+dist-name = "fastapi-jwt-auth-md"
 author = "Nyoman Pradipta Dewantara"
 author-email = "nyomanpradipta120@gmail.com"
 home-page = "https://github.com/IndominusByte/fastapi-jwt-auth"
 
 classifiers = [
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
```

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/private_key.txt` & `fastapi_jwt_auth_md-1.0.0/tests/private_key.txt`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_config.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_cookies.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_create_token.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_create_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_decode_token.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_decode_token.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_denylist.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_denylist.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_headers.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_token_multiple_locations.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_token_multiple_locations.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_url_protected.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_url_protected.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/tests/test_websocket.py` & `fastapi_jwt_auth_md-1.0.0/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_md-0.5.0/PKG-INFO` & `fastapi_jwt_auth_md-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastapi-jwt-auth_md
-Version: 0.5.0
+Name: fastapi-jwt-auth-md
+Version: 1.0.0
 Summary: FastAPI extension that provides JWT Auth support (secure, easy to use and lightweight)
 Home-page: https://github.com/IndominusByte/fastapi-jwt-auth
 Author: Nyoman Pradipta Dewantara
 Author-email: nyomanpradipta120@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-jwt-auth_md Version: 0.5.0 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-jwt-auth-md Version: 1.0.0 Summary: FastAPI
 extension that provides JWT Auth support (secure, easy to use and lightweight)
 Home-page: https://github.com/IndominusByte/fastapi-jwt-auth Author: Nyoman
 Pradipta Dewantara Author-email: nyomanpradipta120@gmail.com Requires-Python:
 >=3.6 Description-Content-Type: text/markdown Classifier: Environment :: Web
 Environment Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

