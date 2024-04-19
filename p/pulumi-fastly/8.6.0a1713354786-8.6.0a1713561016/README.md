# Comparing `tmp/pulumi_fastly-8.6.0a1713354786.tar.gz` & `tmp/pulumi_fastly-8.6.0a1713561016.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.6.0a1713354786.tar", last modified: Wed Apr 17 11:59:07 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.6.0a1713561016.tar", last modified: Fri Apr 19 21:12:58 2024, max compression
```

## Comparing `pulumi_fastly-8.6.0a1713354786.tar` & `pulumi_fastly-8.6.0a1713561016.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:59:07.637405 pulumi_fastly-8.6.0a1713354786/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-17 11:59:07.637405 pulumi_fastly-8.6.0a1713354786/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:59:07.633405 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   521999 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:59:07.633405 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   470310 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    92270 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23295 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:59:07.633405 pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-17 11:59:07.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-17 11:59:07.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:59:07.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 11:59:07.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 11:59:07.000000 pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-17 11:59:01.000000 pulumi_fastly-8.6.0a1713354786/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:59:07.637405 pulumi_fastly-8.6.0a1713354786/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:58.166438 pulumi_fastly-8.6.0a1713561016/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-19 21:12:58.166438 pulumi_fastly-8.6.0a1713561016/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:58.166438 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   521999 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:58.166438 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470310 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92456 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23105 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26020 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:58.166438 pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-19 21:12:58.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-19 21:12:58.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:12:58.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:12:58.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 21:12:58.000000 pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 21:12:51.000000 pulumi_fastly-8.6.0a1713561016/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:12:58.166438 pulumi_fastly-8.6.0a1713561016/setup.cfg
```

### Comparing `pulumi_fastly-8.6.0a1713354786/PKG-INFO` & `pulumi_fastly-8.6.0a1713561016/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1713354786
+Version: 8.6.0a1713561016
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1713354786/README.md` & `pulumi_fastly-8.6.0a1713561016/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/__init__.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/alert.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,18 +301,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
-        example_service_vcl = fastly.ServiceVcl("exampleServiceVcl")
-        # ...
-        example_alert = fastly.Alert("exampleAlert",
-            service_id=example_service_vcl.id,
+        example = fastly.ServiceVcl("example", name="my_vcl_service")
+        example_alert = fastly.Alert("example",
+            name="my_vcl_service errors",
+            service_id=example.id,
             source="stats",
             metric="status_5xx",
             evaluation_strategy=fastly.AlertEvaluationStrategyArgs(
                 type="above_threshold",
                 period="5m",
                 threshold=10,
             ))
@@ -350,18 +350,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
-        example_service_vcl = fastly.ServiceVcl("exampleServiceVcl")
-        # ...
-        example_alert = fastly.Alert("exampleAlert",
-            service_id=example_service_vcl.id,
+        example = fastly.ServiceVcl("example", name="my_vcl_service")
+        example_alert = fastly.Alert("example",
+            name="my_vcl_service errors",
+            service_id=example.id,
             source="stats",
             metric="status_5xx",
             evaluation_strategy=fastly.AlertEvaluationStrategyArgs(
                 type="above_threshold",
                 period="5m",
                 threshold=10,
             ))
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/configstore.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/configstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,23 +112,24 @@
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Config Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
-        example_configstore = fastly.Configstore("exampleConfigstore")
-        example_package_hash = fastly.get_package_hash(filename="package.tar.gz")
-        example_service_compute = fastly.ServiceCompute("exampleServiceCompute",
+        example_configstore = fastly.Configstore("example", name="my_config_store")
+        example = fastly.get_package_hash(filename="package.tar.gz")
+        example_service_compute = fastly.ServiceCompute("example",
+            name="my_compute_service",
             domains=[fastly.ServiceComputeDomainArgs(
                 name="demo.example.com",
             )],
             package=fastly.ServiceComputePackageArgs(
                 filename="package.tar.gz",
-                source_code_hash=example_package_hash.hash,
+                source_code_hash=example.hash,
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_configstore.id,
             )],
             force_destroy=True)
         ```
@@ -166,23 +167,24 @@
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Config Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
-        example_configstore = fastly.Configstore("exampleConfigstore")
-        example_package_hash = fastly.get_package_hash(filename="package.tar.gz")
-        example_service_compute = fastly.ServiceCompute("exampleServiceCompute",
+        example_configstore = fastly.Configstore("example", name="my_config_store")
+        example = fastly.get_package_hash(filename="package.tar.gz")
+        example_service_compute = fastly.ServiceCompute("example",
+            name="my_compute_service",
             domains=[fastly.ServiceComputeDomainArgs(
                 name="demo.example.com",
             )],
             package=fastly.ServiceComputePackageArgs(
                 filename="package.tar.gz",
-                source_code_hash=example_package_hash.hash,
+                source_code_hash=example.hash,
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_configstore.id,
             )],
             force_destroy=True)
         ```
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_service_vcl = fastly.ServiceVcl("exampleServiceVcl",
+    example_service_vcl = fastly.ServiceVcl("example",
+        name="Example Service",
         domains=[fastly.ServiceVclDomainArgs(
             name="example.com",
         )],
         dictionaries=[
             fastly.ServiceVclDictionaryArgs(
                 name="example_1",
             ),
@@ -106,17 +107,17 @@
                 name="example_2",
             ),
             fastly.ServiceVclDictionaryArgs(
                 name="example_3",
             ),
         ],
         force_destroy=True)
-    example_dictionaries = fastly.get_dictionaries_output(service_id=example_service_vcl.id,
+    example = fastly.get_dictionaries_output(service_id=example_service_vcl.id,
         service_version=example_service_vcl.active_version)
-    pulumi.export("serviceDictionaries", example_dictionaries)
+    pulumi.export("serviceDictionaries", example)
     ```
     <!--End PulumiCodeChooser -->
 
     [1]: https://developer.fastly.com/reference/api/dictionaries/
 
 
     :param str service_id: Alphanumeric string identifying the service.
@@ -145,15 +146,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_service_vcl = fastly.ServiceVcl("exampleServiceVcl",
+    example_service_vcl = fastly.ServiceVcl("example",
+        name="Example Service",
         domains=[fastly.ServiceVclDomainArgs(
             name="example.com",
         )],
         dictionaries=[
             fastly.ServiceVclDictionaryArgs(
                 name="example_1",
             ),
@@ -161,17 +163,17 @@
                 name="example_2",
             ),
             fastly.ServiceVclDictionaryArgs(
                 name="example_3",
             ),
         ],
         force_destroy=True)
-    example_dictionaries = fastly.get_dictionaries_output(service_id=example_service_vcl.id,
+    example = fastly.get_dictionaries_output(service_id=example_service_vcl.id,
         service_version=example_service_vcl.active_version)
-    pulumi.export("serviceDictionaries", example_dictionaries)
+    pulumi.export("serviceDictionaries", example)
     ```
     <!--End PulumiCodeChooser -->
 
     [1]: https://developer.fastly.com/reference/api/dictionaries/
 
 
     :param str service_id: Alphanumeric string identifying the service.
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,21 +77,23 @@
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_aws as aws
     import pulumi_fastly as fastly
 
     fastly = fastly.get_fastly_ip_ranges()
-    from_fastly = aws.ec2.SecurityGroup("fromFastly", ingress=[aws.ec2.SecurityGroupIngressArgs(
-        from_port=443,
-        to_port=443,
-        protocol="tcp",
-        cidr_blocks=fastly.cidr_blocks,
-        ipv6_cidr_blocks=fastly.ipv6_cidr_blocks,
-    )])
+    from_fastly = aws.index.SecurityGroup("from_fastly",
+        name=from_fastly,
+        ingress=[{
+            fromPort: 443,
+            toPort: 443,
+            protocol: tcp,
+            cidrBlocks: fastly.cidr_blocks,
+            ipv6CidrBlocks: fastly.ipv6_cidr_blocks,
+        }])
     ```
     <!--End PulumiCodeChooser -->
 
     [1]: https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -113,20 +115,22 @@
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_aws as aws
     import pulumi_fastly as fastly
 
     fastly = fastly.get_fastly_ip_ranges()
-    from_fastly = aws.ec2.SecurityGroup("fromFastly", ingress=[aws.ec2.SecurityGroupIngressArgs(
-        from_port=443,
-        to_port=443,
-        protocol="tcp",
-        cidr_blocks=fastly.cidr_blocks,
-        ipv6_cidr_blocks=fastly.ipv6_cidr_blocks,
-    )])
+    from_fastly = aws.index.SecurityGroup("from_fastly",
+        name=from_fastly,
+        ingress=[{
+            fromPort: 443,
+            toPort: 443,
+            protocol: tcp,
+            cidrBlocks: fastly.cidr_blocks,
+            ipv6CidrBlocks: fastly.ipv6_cidr_blocks,
+        }])
     ```
     <!--End PulumiCodeChooser -->
 
     [1]: https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_package_hash.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,19 +89,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_package_hash = fastly.get_package_hash(filename="./path/to/package.tar.gz")
-    # ...
-    example_service_compute = fastly.ServiceCompute("exampleServiceCompute", package=fastly.ServiceComputePackageArgs(
+    example = fastly.get_package_hash(filename="./path/to/package.tar.gz")
+    example_service_compute = fastly.ServiceCompute("example", package=fastly.ServiceComputePackageArgs(
         filename="./path/to/package.tar.gz",
-        source_code_hash=example_package_hash.hash,
+        source_code_hash=example.hash,
     ))
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str content: The contents of the Wasm deployment package as a base64 encoded string (e.g. could be provided using an input variable or via external data source output variable). Conflicts with `filename`. Exactly one of these two arguments must be specified
     :param str filename: The path to the Wasm deployment package within your local filesystem. Conflicts with `content`. Exactly one of these two arguments must be specified
@@ -129,19 +128,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_package_hash = fastly.get_package_hash(filename="./path/to/package.tar.gz")
-    # ...
-    example_service_compute = fastly.ServiceCompute("exampleServiceCompute", package=fastly.ServiceComputePackageArgs(
+    example = fastly.get_package_hash(filename="./path/to/package.tar.gz")
+    example_service_compute = fastly.ServiceCompute("example", package=fastly.ServiceComputePackageArgs(
         filename="./path/to/package.tar.gz",
-        source_code_hash=example_package_hash.hash,
+        source_code_hash=example.hash,
     ))
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str content: The contents of the Wasm deployment package as a base64 encoded string (e.g. could be provided using an input variable or via external data source output variable). Conflicts with `filename`. Exactly one of these two arguments must be specified
     :param str filename: The path to the Wasm deployment package within your local filesystem. Conflicts with `content`. Exactly one of these two arguments must be specified
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_services.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_activation_ids.py`

 * *Files 24% similar despite different names*

```diff
@@ -76,17 +76,17 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=fastly_tls_certificate["example"]["id"])
-    example_tls_activation = [fastly.get_tls_activation(id=__value) for __key, __value in example_tls_activation_ids.ids]
-    pulumi.export("activationDomains", [a.domain for a in example_tls_activation])
+    example = fastly.get_tls_activation_ids(certificate_id=example_fastly_tls_certificate["id"])
+    example_get_tls_activation = {__key: fastly.get_tls_activation(id=__value) for __key, __value in example.ids}
+    pulumi.export("activationDomains", [a.domain for a in example_get_tls_activation])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
     __args__ = dict()
@@ -109,17 +109,17 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=fastly_tls_certificate["example"]["id"])
-    example_tls_activation = [fastly.get_tls_activation(id=__value) for __key, __value in example_tls_activation_ids.ids]
-    pulumi.export("activationDomains", [a.domain for a in example_tls_activation])
+    example = fastly.get_tls_activation_ids(certificate_id=example_fastly_tls_certificate["id"])
+    example_get_tls_activation = {__key: fastly.get_tls_activation(id=__value) for __key, __value in example.ids}
+    pulumi.export("activationDomains", [a.domain for a in example_get_tls_activation])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,17 +63,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_certificate_ids = fastly.get_tls_certificate_ids()
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", certificate_id=example_tls_certificate_ids.ids[0])
-    # ...
+    example = fastly.get_tls_certificate_ids()
+    example_tls_activation = fastly.TlsActivation("example", certificate_id=example.ids[0])
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsCertificateIds:getTlsCertificateIds', __args__, opts=opts, typ=GetTlsCertificateIdsResult).value
 
@@ -90,14 +89,13 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_certificate_ids = fastly.get_tls_certificate_ids()
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", certificate_id=example_tls_certificate_ids.ids[0])
-    # ...
+    example = fastly.get_tls_certificate_ids()
+    example_tls_activation = fastly.TlsActivation("example", certificate_id=example.ids[0])
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,17 +160,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_configuration = fastly.get_tls_configuration(default=True)
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", configuration_id=example_tls_configuration.id)
-    # ...
+    example = fastly.get_tls_configuration(default=True)
+    example_tls_activation = fastly.TlsActivation("example", configuration_id=example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param bool default: Signifies whether Fastly will use this configuration as a default when creating a new TLS activation.
     :param Sequence[str] http_protocols: HTTP protocols available on the TLS configuration.
     :param str id: ID of the TLS configuration obtained from the Fastly API or another data source. Conflicts with all the other filters.
@@ -220,17 +219,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_configuration = fastly.get_tls_configuration(default=True)
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", configuration_id=example_tls_configuration.id)
-    # ...
+    example = fastly.get_tls_configuration(default=True)
+    example_tls_activation = fastly.TlsActivation("example", configuration_id=example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param bool default: Signifies whether Fastly will use this configuration as a default when creating a new TLS activation.
     :param Sequence[str] http_protocols: HTTP protocols available on the TLS configuration.
     :param str id: ID of the TLS configuration obtained from the Fastly API or another data source. Conflicts with all the other filters.
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,17 +63,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_configuration_ids = fastly.get_tls_configuration_ids()
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", configuration_id=example_tls_configuration_ids.ids[0])
-    # ...
+    example = fastly.get_tls_configuration_ids()
+    example_tls_activation = fastly.TlsActivation("example", configuration_id=example.ids[0])
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsConfigurationIds:getTlsConfigurationIds', __args__, opts=opts, typ=GetTlsConfigurationIdsResult).value
 
@@ -90,14 +89,13 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_configuration_ids = fastly.get_tls_configuration_ids()
-    example_tls_activation = fastly.TlsActivation("exampleTlsActivation", configuration_id=example_tls_configuration_ids.ids[0])
-    # ...
+    example = fastly.get_tls_configuration_ids()
+    example_tls_activation = fastly.TlsActivation("example", configuration_id=example.ids[0])
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_platform_certificate_ids = fastly.get_tls_platform_certificate_ids()
-    example_tls_platform_certificate = fastly.get_tls_platform_certificate(id=example_tls_platform_certificate_ids.ids[0])
+    example = fastly.get_tls_platform_certificate_ids()
+    example_get_tls_platform_certificate = fastly.get_tls_platform_certificate(id=example.ids[0])
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPlatformCertificateIds:getTlsPlatformCertificateIds', __args__, opts=opts, typ=GetTlsPlatformCertificateIdsResult).value
 
@@ -89,13 +89,13 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_platform_certificate_ids = fastly.get_tls_platform_certificate_ids()
-    example_tls_platform_certificate = fastly.get_tls_platform_certificate(id=example_tls_platform_certificate_ids.ids[0])
+    example = fastly.get_tls_platform_certificate_ids()
+    example_get_tls_platform_certificate = fastly.get_tls_platform_certificate(id=example.ids[0])
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key_ids()
-    example = fastly.get_tls_private_key(id=fastly_tls_private_key_ids["demo"]["ids"])
+    example = fastly.get_tls_private_key(id=demo_fastly_tls_private_key_ids["ids"])
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPrivateKeyIds:getTlsPrivateKeyIds', __args__, opts=opts, typ=GetTlsPrivateKeyIdsResult).value
 
@@ -90,12 +90,12 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key_ids()
-    example = fastly.get_tls_private_key(id=fastly_tls_private_key_ids["demo"]["ids"])
+    example = fastly.get_tls_private_key(id=demo_fastly_tls_private_key_ids["ids"])
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,17 +63,17 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_subscription_ids = fastly.get_tls_subscription_ids()
-    example_tls_subscription = [fastly.get_tls_subscription(id=__value) for __key, __value in example_tls_subscription_ids.ids]
-    pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_tls_subscription])
+    example = fastly.get_tls_subscription_ids()
+    example_get_tls_subscription = {__key: fastly.get_tls_subscription(id=__value) for __key, __value in example.ids}
+    pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_get_tls_subscription])
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsSubscriptionIds:getTlsSubscriptionIds', __args__, opts=opts, typ=GetTlsSubscriptionIdsResult).value
 
@@ -90,14 +90,14 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
-    example_tls_subscription_ids = fastly.get_tls_subscription_ids()
-    example_tls_subscription = [fastly.get_tls_subscription(id=__value) for __key, __value in example_tls_subscription_ids.ids]
-    pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_tls_subscription])
+    example = fastly.get_tls_subscription_ids()
+    example_get_tls_subscription = {__key: fastly.get_tls_subscription(id=__value) for __key, __value in example.ids}
+    pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_get_tls_subscription])
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/kvstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,23 +108,24 @@
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a KV Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
-        example_kvstore = fastly.Kvstore("exampleKvstore")
-        example_package_hash = fastly.get_package_hash(filename="package.tar.gz")
-        example_service_compute = fastly.ServiceCompute("exampleServiceCompute",
+        example_kvstore = fastly.Kvstore("example", name="my_kv_store")
+        example = fastly.get_package_hash(filename="package.tar.gz")
+        example_service_compute = fastly.ServiceCompute("example",
+            name="my_compute_service",
             domains=[fastly.ServiceComputeDomainArgs(
                 name="demo.example.com",
             )],
             package=fastly.ServiceComputePackageArgs(
                 filename="package.tar.gz",
-                source_code_hash=example_package_hash.hash,
+                source_code_hash=example.hash,
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_kvstore.id,
             )],
             force_destroy=True)
         ```
@@ -158,23 +159,24 @@
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a KV Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
-        example_kvstore = fastly.Kvstore("exampleKvstore")
-        example_package_hash = fastly.get_package_hash(filename="package.tar.gz")
-        example_service_compute = fastly.ServiceCompute("exampleServiceCompute",
+        example_kvstore = fastly.Kvstore("example", name="my_kv_store")
+        example = fastly.get_package_hash(filename="package.tar.gz")
+        example_service_compute = fastly.ServiceCompute("example",
+            name="my_compute_service",
             domains=[fastly.ServiceComputeDomainArgs(
                 name="demo.example.com",
             )],
             package=fastly.ServiceComputePackageArgs(
                 filename="package.tar.gz",
-                source_code_hash=example_package_hash.hash,
+                source_code_hash=example.hash,
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_kvstore.id,
             )],
             force_destroy=True)
         ```
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/outputs.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/provider.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/secretstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,23 +75,24 @@
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Secret Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
-        example_secretstore = fastly.Secretstore("exampleSecretstore")
-        example_package_hash = fastly.get_package_hash(filename="package.tar.gz")
-        example_service_compute = fastly.ServiceCompute("exampleServiceCompute",
+        example_secretstore = fastly.Secretstore("example", name="my_secret_store")
+        example = fastly.get_package_hash(filename="package.tar.gz")
+        example_service_compute = fastly.ServiceCompute("example",
+            name="my_compute_service",
             domains=[fastly.ServiceComputeDomainArgs(
                 name="demo.example.com",
             )],
             package=fastly.ServiceComputePackageArgs(
                 filename="package.tar.gz",
-                source_code_hash=example_package_hash.hash,
+                source_code_hash=example.hash,
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_secretstore.id,
             )],
             force_destroy=True)
         ```
@@ -124,23 +125,24 @@
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         # IMPORTANT: Deleting a Secret Store requires first deleting its resource_link.
         # This requires a two-step `pulumi up` as we can't guarantee deletion order.
         # e.g. resource_link deletion within fastly_service_compute might not finish first.
-        example_secretstore = fastly.Secretstore("exampleSecretstore")
-        example_package_hash = fastly.get_package_hash(filename="package.tar.gz")
-        example_service_compute = fastly.ServiceCompute("exampleServiceCompute",
+        example_secretstore = fastly.Secretstore("example", name="my_secret_store")
+        example = fastly.get_package_hash(filename="package.tar.gz")
+        example_service_compute = fastly.ServiceCompute("example",
+            name="my_compute_service",
             domains=[fastly.ServiceComputeDomainArgs(
                 name="demo.example.com",
             )],
             package=fastly.ServiceComputePackageArgs(
                 filename="package.tar.gz",
-                source_code_hash=example_package_hash.hash,
+                source_code_hash=example.hash,
             ),
             resource_links=[fastly.ServiceComputeResourceLinkArgs(
                 name="my_resource_link",
                 resource_id=example_secretstore.id,
             )],
             force_destroy=True)
         ```
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo")
-        #...
         user = fastly.User("user")
-        # ...
         auth = fastly.ServiceAuthorization("auth",
             service_id=demo.id,
             user_id=user.id,
             permission="purge_all")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -185,17 +183,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo")
-        #...
         user = fastly.User("user")
-        # ...
         auth = fastly.ServiceAuthorization("auth",
             service_id=demo.id,
             user_id=user.id,
             permission="purge_all")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/service_waf_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1133,14 +1133,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
+            name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
                 comment="demo",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="origin1",
@@ -1181,14 +1182,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
+            name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
                 comment="demo",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="origin1",
@@ -1236,14 +1238,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
+            name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
                 comment="demo",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="origin1",
@@ -1353,14 +1356,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
+            name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
                 comment="demo",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="origin1",
@@ -1401,14 +1405,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
+            name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
                 comment="demo",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="origin1",
@@ -1456,14 +1461,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
         demo = fastly.ServiceVcl("demo",
+            name="demofastly",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
                 comment="demo",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="origin1",
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_activation.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,30 +189,35 @@
         Basic usage:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
-        demo_service_vcl = fastly.ServiceVcl("demoServiceVcl",
+        demo = fastly.ServiceVcl("demo",
+            name="my-service",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="localhost",
             )],
             force_destroy=True)
-        demo_tls_private_key = fastly.TlsPrivateKey("demoTlsPrivateKey", key_pem="...")
-        demo_tls_certificate = fastly.TlsCertificate("demoTlsCertificate", certificate_body="...",
-        opts=pulumi.ResourceOptions(depends_on=[demo_tls_private_key]))
+        demo_tls_private_key = fastly.TlsPrivateKey("demo",
+            key_pem="...",
+            name="demo-key")
+        demo_tls_certificate = fastly.TlsCertificate("demo",
+            certificate_body="...",
+            name="demo-cert",
+            opts=pulumi.ResourceOptions(depends_on=[demo_tls_private_key]))
         test = fastly.TlsActivation("test",
             certificate_id=demo_tls_certificate.id,
             domain="example.com",
-            opts=pulumi.ResourceOptions(depends_on=[demo_service_vcl]))
+            opts=pulumi.ResourceOptions(depends_on=[demo]))
         ```
         <!--End PulumiCodeChooser -->
 
         > **Warning:** Updating the `TlsPrivateKey`/`TlsCertificate` resources should be done in multiple plan/apply steps to avoid potential downtime. The new certificate and associated private key must first be created so they exist alongside the currently active resources. Once the new resources have been created, then the `TlsActivation` can be updated to point to the new certificate. Finally, the original key/certificate resources can be deleted.
 
         ## Import
 
@@ -245,30 +250,35 @@
         Basic usage:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
-        demo_service_vcl = fastly.ServiceVcl("demoServiceVcl",
+        demo = fastly.ServiceVcl("demo",
+            name="my-service",
             domains=[fastly.ServiceVclDomainArgs(
                 name="example.com",
             )],
             backends=[fastly.ServiceVclBackendArgs(
                 address="127.0.0.1",
                 name="localhost",
             )],
             force_destroy=True)
-        demo_tls_private_key = fastly.TlsPrivateKey("demoTlsPrivateKey", key_pem="...")
-        demo_tls_certificate = fastly.TlsCertificate("demoTlsCertificate", certificate_body="...",
-        opts=pulumi.ResourceOptions(depends_on=[demo_tls_private_key]))
+        demo_tls_private_key = fastly.TlsPrivateKey("demo",
+            key_pem="...",
+            name="demo-key")
+        demo_tls_certificate = fastly.TlsCertificate("demo",
+            certificate_body="...",
+            name="demo-cert",
+            opts=pulumi.ResourceOptions(depends_on=[demo_tls_private_key]))
         test = fastly.TlsActivation("test",
             certificate_id=demo_tls_certificate.id,
             domain="example.com",
-            opts=pulumi.ResourceOptions(depends_on=[demo_service_vcl]))
+            opts=pulumi.ResourceOptions(depends_on=[demo]))
         ```
         <!--End PulumiCodeChooser -->
 
         > **Warning:** Updating the `TlsPrivateKey`/`TlsCertificate` resources should be done in multiple plan/apply steps to avoid potential downtime. The new certificate and associated private key must first be created so they exist alongside the currently active resources. Once the new resources have been created, then the `TlsActivation` can be updated to point to the new certificate. Finally, the original key/certificate resources can be deleted.
 
         ## Import
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,32 +238,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
-        key_private_key = tls.PrivateKey("keyPrivateKey", algorithm="RSA")
-        cert = tls.SelfSignedCert("cert",
-            key_algorithm=key_private_key.algorithm,
-            private_key_pem=key_private_key.private_key_pem,
-            subjects=[tls.SelfSignedCertSubjectArgs(
-                common_name="example.com",
-            )],
+        key = tls.index.PrivateKey("key", algorithm=RSA)
+        cert = tls.index.SelfSignedCert("cert",
+            key_algorithm=key.algorithm,
+            private_key_pem=key.private_key_pem,
+            subject=[{
+                commonName: example.com,
+            }],
             is_ca_certificate=True,
             validity_period_hours=360,
             allowed_uses=[
-                "cert_signing",
-                "server_auth",
+                cert_signing,
+                server_auth,
             ],
-            dns_names=["example.com"])
-        key_tls_private_key = fastly.TlsPrivateKey("keyTlsPrivateKey", key_pem=key_private_key.private_key_pem)
-        example = fastly.TlsCertificate("example", certificate_body=cert.cert_pem,
-        opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
-        # The private key has to be present before the certificate can be uploaded
+            dns_names=[example.com])
+        key_tls_private_key = fastly.TlsPrivateKey("key",
+            key_pem=key["privateKeyPem"],
+            name="tf-demo")
+        example = fastly.TlsCertificate("example",
+            name="tf-demo",
+            certificate_body=cert["certPem"],
+            opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Updating certificates
 
         There are three scenarios for updating a certificate:
 
@@ -306,32 +309,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
-        key_private_key = tls.PrivateKey("keyPrivateKey", algorithm="RSA")
-        cert = tls.SelfSignedCert("cert",
-            key_algorithm=key_private_key.algorithm,
-            private_key_pem=key_private_key.private_key_pem,
-            subjects=[tls.SelfSignedCertSubjectArgs(
-                common_name="example.com",
-            )],
+        key = tls.index.PrivateKey("key", algorithm=RSA)
+        cert = tls.index.SelfSignedCert("cert",
+            key_algorithm=key.algorithm,
+            private_key_pem=key.private_key_pem,
+            subject=[{
+                commonName: example.com,
+            }],
             is_ca_certificate=True,
             validity_period_hours=360,
             allowed_uses=[
-                "cert_signing",
-                "server_auth",
+                cert_signing,
+                server_auth,
             ],
-            dns_names=["example.com"])
-        key_tls_private_key = fastly.TlsPrivateKey("keyTlsPrivateKey", key_pem=key_private_key.private_key_pem)
-        example = fastly.TlsCertificate("example", certificate_body=cert.cert_pem,
-        opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
-        # The private key has to be present before the certificate can be uploaded
+            dns_names=[example.com])
+        key_tls_private_key = fastly.TlsPrivateKey("key",
+            key_pem=key["privateKeyPem"],
+            name="tf-demo")
+        example = fastly.TlsCertificate("example",
+            name="tf-demo",
+            certificate_body=cert["certPem"],
+            opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Updating certificates
 
         There are three scenarios for updating a certificate:
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_platform_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,53 +270,55 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
-        ca_key = tls.PrivateKey("caKey", algorithm="RSA")
-        key_private_key = tls.PrivateKey("keyPrivateKey", algorithm="RSA")
-        ca = tls.SelfSignedCert("ca",
+        ca_key = tls.index.PrivateKey("ca_key", algorithm=RSA)
+        key = tls.index.PrivateKey("key", algorithm=RSA)
+        ca = tls.index.SelfSignedCert("ca",
             key_algorithm=ca_key.algorithm,
             private_key_pem=ca_key.private_key_pem,
-            subjects=[tls.SelfSignedCertSubjectArgs(
-                common_name="Example CA",
-            )],
+            subject=[{
+                commonName: Example CA,
+            }],
             is_ca_certificate=True,
             validity_period_hours=360,
             allowed_uses=[
-                "cert_signing",
-                "server_auth",
+                cert_signing,
+                server_auth,
             ])
-        example = tls.CertRequest("example",
-            key_algorithm=key_private_key.algorithm,
-            private_key_pem=key_private_key.private_key_pem,
-            subjects=[tls.CertRequestSubjectArgs(
-                common_name="example.com",
-            )],
+        example = tls.index.CertRequest("example",
+            key_algorithm=key.algorithm,
+            private_key_pem=key.private_key_pem,
+            subject=[{
+                commonName: example.com,
+            }],
             dns_names=[
-                "example.com",
-                "www.example.com",
+                example.com,
+                www.example.com,
             ])
-        cert_locally_signed_cert = tls.LocallySignedCert("certLocallySignedCert",
+        cert = tls.index.LocallySignedCert("cert",
             cert_request_pem=example.cert_request_pem,
             ca_key_algorithm=ca_key.algorithm,
             ca_private_key_pem=ca_key.private_key_pem,
             ca_cert_pem=ca.cert_pem,
             validity_period_hours=360,
             allowed_uses=[
-                "cert_signing",
-                "server_auth",
+                cert_signing,
+                server_auth,
             ])
         config = fastly.get_tls_configuration(tls_service="PLATFORM")
-        key_tls_private_key = fastly.TlsPrivateKey("keyTlsPrivateKey", key_pem=key_private_key.private_key_pem)
-        cert_tls_platform_certificate = fastly.TlsPlatformCertificate("certTlsPlatformCertificate",
-            certificate_body=cert_locally_signed_cert.cert_pem,
-            intermediates_blob=ca.cert_pem,
+        key_tls_private_key = fastly.TlsPrivateKey("key",
+            key_pem=key["privateKeyPem"],
+            name="tf-demo")
+        cert_tls_platform_certificate = fastly.TlsPlatformCertificate("cert",
+            certificate_body=cert["certPem"],
+            intermediates_blob=ca["certPem"],
             configuration_id=config.id,
             allow_untrusted_root=True,
             opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -352,53 +354,55 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
-        ca_key = tls.PrivateKey("caKey", algorithm="RSA")
-        key_private_key = tls.PrivateKey("keyPrivateKey", algorithm="RSA")
-        ca = tls.SelfSignedCert("ca",
+        ca_key = tls.index.PrivateKey("ca_key", algorithm=RSA)
+        key = tls.index.PrivateKey("key", algorithm=RSA)
+        ca = tls.index.SelfSignedCert("ca",
             key_algorithm=ca_key.algorithm,
             private_key_pem=ca_key.private_key_pem,
-            subjects=[tls.SelfSignedCertSubjectArgs(
-                common_name="Example CA",
-            )],
+            subject=[{
+                commonName: Example CA,
+            }],
             is_ca_certificate=True,
             validity_period_hours=360,
             allowed_uses=[
-                "cert_signing",
-                "server_auth",
+                cert_signing,
+                server_auth,
             ])
-        example = tls.CertRequest("example",
-            key_algorithm=key_private_key.algorithm,
-            private_key_pem=key_private_key.private_key_pem,
-            subjects=[tls.CertRequestSubjectArgs(
-                common_name="example.com",
-            )],
+        example = tls.index.CertRequest("example",
+            key_algorithm=key.algorithm,
+            private_key_pem=key.private_key_pem,
+            subject=[{
+                commonName: example.com,
+            }],
             dns_names=[
-                "example.com",
-                "www.example.com",
+                example.com,
+                www.example.com,
             ])
-        cert_locally_signed_cert = tls.LocallySignedCert("certLocallySignedCert",
+        cert = tls.index.LocallySignedCert("cert",
             cert_request_pem=example.cert_request_pem,
             ca_key_algorithm=ca_key.algorithm,
             ca_private_key_pem=ca_key.private_key_pem,
             ca_cert_pem=ca.cert_pem,
             validity_period_hours=360,
             allowed_uses=[
-                "cert_signing",
-                "server_auth",
+                cert_signing,
+                server_auth,
             ])
         config = fastly.get_tls_configuration(tls_service="PLATFORM")
-        key_tls_private_key = fastly.TlsPrivateKey("keyTlsPrivateKey", key_pem=key_private_key.private_key_pem)
-        cert_tls_platform_certificate = fastly.TlsPlatformCertificate("certTlsPlatformCertificate",
-            certificate_body=cert_locally_signed_cert.cert_pem,
-            intermediates_blob=ca.cert_pem,
+        key_tls_private_key = fastly.TlsPrivateKey("key",
+            key_pem=key["privateKeyPem"],
+            name="tf-demo")
+        cert_tls_platform_certificate = fastly.TlsPlatformCertificate("cert",
+            certificate_body=cert["certPem"],
+            intermediates_blob=ca["certPem"],
             configuration_id=config.id,
             allow_untrusted_root=True,
             opts=pulumi.ResourceOptions(depends_on=[key_tls_private_key]))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_private_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,16 +189,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
-        demo_private_key = tls.PrivateKey("demoPrivateKey", algorithm="RSA")
-        demo_tls_private_key = fastly.TlsPrivateKey("demoTlsPrivateKey", key_pem=demo_private_key.private_key_pem)
+        demo = tls.index.PrivateKey("demo", algorithm=RSA)
+        demo_tls_private_key = fastly.TlsPrivateKey("demo",
+            key_pem=demo["privateKeyPem"],
+            name="tf-demo")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Private Key can be imported using its ID, e.g.
 
@@ -228,16 +230,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
         import pulumi_tls as tls
 
-        demo_private_key = tls.PrivateKey("demoPrivateKey", algorithm="RSA")
-        demo_tls_private_key = fastly.TlsPrivateKey("demoTlsPrivateKey", key_pem=demo_private_key.private_key_pem)
+        demo = tls.index.PrivateKey("demo", algorithm=RSA)
+        demo_tls_private_key = fastly.TlsPrivateKey("demo",
+            key_pem=demo["privateKeyPem"],
+            name="tf-demo")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Private Key can be imported using its ID, e.g.
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly/user.py` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,17 @@
         Basic usage:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
-        demo = fastly.User("demo", login="demo@example.com")
+        demo = fastly.User("demo",
+            login="demo@example.com",
+            name="Demo User")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Fastly User can be imported using their user ID, e.g.
 
@@ -179,15 +181,17 @@
         Basic usage:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_fastly as fastly
 
-        demo = fastly.User("demo", login="demo@example.com")
+        demo = fastly.User("demo",
+            login="demo@example.com",
+            name="Demo User")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Fastly User can be imported using their user ID, e.g.
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1713354786
+Version: 8.6.0a1713561016
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1713354786/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.6.0a1713561016/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1713354786/pyproject.toml` & `pulumi_fastly-8.6.0a1713561016/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.6.0a1713354786"
+  version = "8.6.0a1713561016"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

