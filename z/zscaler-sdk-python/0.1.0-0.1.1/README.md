# Comparing `tmp/zscaler-sdk-python-0.1.0.tar.gz` & `tmp/zscaler-sdk-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler-sdk-python-0.1.0.tar", last modified: Thu Apr 18 09:09:45 2024, max compression
+gzip compressed data, was "zscaler-sdk-python-0.1.1.tar", last modified: Fri Apr 19 06:21:36 2024, max compression
```

## Comparing `zscaler-sdk-python-0.1.0.tar` & `zscaler-sdk-python-0.1.1.tar`

### file list

```diff
@@ -1,214 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/LONG_DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.084415 zscaler-sdk-python-0.1.0/docsrc/
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.084415 zscaler-sdk-python-0.1.0/docsrc/zs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.088415 zscaler-sdk-python-0.1.0/docsrc/zs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/guides/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.088415 zscaler-sdk-python-0.1.0/docsrc/zs/zia/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/admin_and_role_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/apptotal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/audit_logs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/authentication_settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/cloud_apps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/device_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/firewall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/forwarding_control.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/locations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/rule_labels.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/sandbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/ssl_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/traffic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/url_categories.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/url_filtering.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/users.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/web_dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/workload_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zia/zpa_gateway.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.092415 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/app_segments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/app_segments_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/app_segments_pra.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/cloud_connector_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/connectors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/emergency_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/idp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/lss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/machine_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/policies.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/posture_profiles.rst
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/privileged_remote_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/provisioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/saml_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/scim_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/scim_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/segment_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/server_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/servers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/service_edges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/docsrc/zs/zpa/trusted_networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1794 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.092415 zscaler-sdk-python-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.084415 zscaler-sdk-python-0.1.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.096415 zscaler-sdk-python-0.1.0/tests/integration/zia/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_icap_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_idm_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_incident_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_web_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_rule_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_vpn_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_filtering_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zia/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/tests/integration/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_timeout_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_app_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_ba_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_enrolment_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_portal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_app_connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_service_edge_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_service_edge_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/integration/zpa/test_trusted_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/no_op_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/cache/zscaler_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/errors/zscaler_api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.100415 zscaler-sdk-python-0.1.0/zscaler/ratelimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/ratelimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.104415 zscaler-sdk-python-0.1.0/zscaler/zia/
--rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/apptotal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/cloud_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    27588 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/forwarding_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/ssl_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31279 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/traffic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/url_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/web_dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/workload_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zia/zpa_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.108415 zscaler-sdk-python-0.1.0/zscaler/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/emergency_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/idp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/lss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    30654 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/provisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/service_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-18 09:09:41.000000 zscaler-sdk-python-0.1.0/zscaler/zpa/trusted_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:09:45.112415 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 09:09:45.000000 zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/docsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/docsrc/zs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/docsrc/zs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.441035 zscaler-sdk-python-0.1.1/docsrc/zs/zia/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/admin_and_role_management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/apptotal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/audit_logs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/authentication_settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/cloud_apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/device_management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/dlp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/firewall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/forwarding_control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/isolation_profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/locations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/rule_labels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/sandbox.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/security.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/ssl_inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/traffic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/url_categories.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/url_filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/users.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/web_dlp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/workload_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/zpa_gateway.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.445035 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/app_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/app_segments_inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/app_segments_pra.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/certificates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/cloud_connector_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/connectors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/emergency_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/idp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/isolation_profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/lss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/machine_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/policies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/posture_profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/privileged_remote_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/provisioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/saml_attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/scim_attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/scim_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/segment_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/server_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/servers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/service_edges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/trusted_networks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 06:21:36.469035 zscaler-sdk-python-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1750 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.445035 zscaler-sdk-python-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.449035 zscaler-sdk-python-0.1.1/tests/integration/zia/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_admin_and_role_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_authentication_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_icap_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_idm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_incident_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_web_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_rule_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_gre_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_vpn_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_filtering_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.453035 zscaler-sdk-python-0.1.1/tests/integration/zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_timeout_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_app_connector_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_ba_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_enrolment_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_machine_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_posture_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_portal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_app_connector_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_service_edge_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_saml_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_segment_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_server_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_service_edge_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_trusted_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/no_op_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/zscaler_api_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/ratelimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.461035 zscaler-sdk-python-0.1.1/zscaler/zia/
+-rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/apptotal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/authentication_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/cloud_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27588 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/dlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/forwarding_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31279 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/traffic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/url_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/url_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/web_dlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/workload_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/zpa_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/zscaler/zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/emergency_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/lss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/machine_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30654 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/segment_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/server_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/service_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/trusted_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/top_level.txt
```

### Comparing `zscaler-sdk-python-0.1.0/LICENSE.md` & `zscaler-sdk-python-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/LONG_DESCRIPTION.md` & `zscaler-sdk-python-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,128 @@
-# Official Python SDK for the Zscaler Products
+# Official Python SDK for the Zscaler Products (Beta)
 
-[![CI/CD](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml)
-[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/zscaler-sdk-python)](https://pypistats.org/packages/zscaler-sdk-python)
 [![License](https://img.shields.io/github/license/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python)
+[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
 [![Latest version released on PyPi](https://img.shields.io/pypi/v/zscaler-sdk-python.svg)](https://pypi.org/project/zscaler-sdk-python)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zscaler-sdk-python.svg)](https://pypi.python.org/pypi/zscaler-sdk-python/)
-[![GitHub Release](https://img.shields.io/github/release/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python/releases/)
 [![Zscaler Community](https://img.shields.io/badge/zscaler-community-blue)](https://community.zscaler.com/)
 
 ## Support Disclaimer
 
--> **Disclaimer:** Please refer to our [General Support Statement](docs/guides/support.md) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docs/guides/troubleshooting.md) for guidance on typical problems.
+-> **Disclaimer:** Please refer to our [General Support Statement](docsrc/zs/guides/support.rst) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docsrc/zs/guides/troubleshooting.rst) for guidance on typical problems.
 
 ## Zscaler Python SDK Overview
 
-This repository contains the Zscaler SDK for Python. This SDK can be used to interact with several Zscaler services such as:
+The Zscaler SDK for Python includes functionality to accelerate development with [Python](https://www.python.org/) several Zscaler services such as:
 
-* Zscaler Private Access (ZPA)
-* Zscaler Internet Access (ZIA)
+* [Zscaler Internet Access (ZIA)](https://help.zscaler.com/zia/getting-started-zia-api)
+* [Zscaler Private Access (ZPA)](https://help.zscaler.com/zpa/getting-started-zpa-api)
 * [Documentation](http://zscaler-sdk-python.readthedocs.io)
 
------
+Each package is supportedd by an individual and robust HTTP client designed to handle failures on different levels by performing intelligent retries.
 
-Each Zscaler product has separate developer documentation and authentication methods. This SDK aims to simplify
-software development using the Zscaler API for both customers and partners.
+**Beta:** This SDK is supported for production use cases, but we do expect future releases to have some interface changes; see [Interface stability](#interface-stability). 
+We are keen to hear feedback from you on these SDKs. Please [file issues](https://github.com/zscaler/zscaler-sdk-python/issues), and we will address them. 
+
+## Contents
 
-- [Release Status](#release-status)
-- [Need help?](#need-help)
 - [Getting Started](#getting-started)
+- [Usage](#usage)
+- [Authentication](#authentication)
 - [Pagination](#pagination)
 - [Logging](#logging)
 - [Rate Limiting](#rate-limiting)
 - [Environment variables](#environment-variables)
 - [Building the SDK](#building-the-sdk)
+- [Interface stability](#interface-stability)
+- [Need help?](#need-help)
 - [Contributing](#contributing)
 
 > Requires Python version 3.8.0 or higher.
 
-## Need help?
+## Getting started<a id="getting-started"></a>
 
-If you run into problems using the SDK, you can:
+To install the Zscaler Python SDK in your project:
+1. Please install Zscaler SDK for Python via `pip install zscaler-sdk-python` and instantiate the respective client based on your project usage:
+- `ZIAClientHelper`
+- `ZPAClientHelper`
 
-- Ask questions on the [Zenith Community][zenith]
-- Post [issues on GitHub][github-issues] (for code errors)
-- Support [customer support portal][zscaler-support]
+Zscaler SDK for Python is compatible with Python 3.7 _(until [June 2023](https://devguide.python.org/versions/))_, 3.8, 3.9, 3.10, and 3.11.
 
-## Getting started
+The upgrade to the latest version of this SDK can be done by executing the following command:
+```python
+%pip install --upgrade zscaler-sdk-python
+```
+followed by
+```python
+dbutils.library.restartPython()
+```
 
-To install the Zscaler Python SDK in your project:
+## Authentication<a id="authentication"></a>
 
-```sh
-pip install zscaler-sdk-python
-```
+Each Zscaler product has separate developer documentation and authentication methods. In this section you will find
+
+1. Credentials that are hard-coded into configuration arguments.
+
+   :warning: **Caution**: Zscaler does not recommend hard-coding credentials into arguments, as they can be exposed in plain text in version control systems. Use environment variables instead.
+
+### ZIA native authentication
+
+- For authentication via Zscaler Internet Access, you must provide `username`, `password`, `api_key` and `cloud`
 
-## Usage
+The ZIA Cloud is identified by several cloud name prefixes, which determines which API endpoint the requests should be sent to. The following cloud environments are supported:
+
+* `zscaler`
+* `zscalerone`
+* `zscalertwo`
+* `zscalerthree`
+* `zscloud`
+* `zscalerbeta`
+* `zscalergov`
+* `zscalerten`
+* `zspreview`
+
+### Environment variables
+
+You can provide credentials via the `ZIA_USERNAME`, `ZIA_PASSWORD`, `ZIA_API_KEY`, `ZIA_CLOUD` environment variables, representing your ZIA `username`, `password`, `api_key` and `cloud` respectively.
+
+| Argument     | Description | Environment variable |
+|--------------|-------------|-------------------|
+| `username`       | _(String)_ A string that contains the email ID of the API admin.| `ZIA_USERNAME` |    
+| `password`       | _(String)_ A string that contains the password for the API admin.| `ZIA_PASSWORD` |
+| `api_key`       | _(String)_ A string that contains the obfuscated API key (i.e., the return value of the obfuscateApiKey() method).| `ZIA_API_KEY` |   
+| `cloud`       | _(String)_ The host and basePath for the cloud services API is `$zsapi.<Zscaler Cloud Name>/api/v1`.| `ZIA_CLOUD` |
+
+### ZPA native authentication
+
+- For authentication via Zscaler Private Access, you must provide `client_id`, `client_secret`, `customer_id` and `cloud`
+
+The ZPA Cloud is identified by several cloud name prefixes, which determines which API endpoint the requests should be sent to. The following cloud environments are supported:
+
+* `PRODUCTION`
+* `ZPATWO`
+* `BETA`
+* `GOV`
+* `GOVUS`
+
+### Environment variables
+
+You can provide credentials via the `ZPA_CLIENT_ID`, `ZPA_CLIENT_SECRET`, `ZPA_CUSTOMER_ID`, `ZPA_CLOUD` environment variables, representing your ZPA `client_id`, `client_secret`, `customer_id` and `cloud` of your ZPA account, respectively.
+
+~> **NOTE** `ZPA_CLOUD` environment variable is required, and is used to identify the correct API gateway where the API requests should be forwarded to.
+
+| Argument     | Description | Environment variable |
+|--------------|-------------|-------------------|
+| `client_id`       | _(String)_ The ZPA API client ID generated from the ZPA console.| `ZPA_CLIENT_ID` |    
+| `client_secret`       | _(String)_ The ZPA API client secret generated from the ZPA console.| `ZPA_CLIENT_SECRET` |
+| `customer_id`       | _(String)_ The ZPA tenant ID found in the Administration > Company menu in the ZPA console.| `ZPA_CUSTOMER_ID` |   
+| `cloud`       | _(String)_ The Zscaler cloud for your tenancy.| `ZPA_CLOUD` |
+
+## Usage<a id="usage"></a>
 
 Before you can interact with any of the Zscaler APIs, you need to generate API keys or retrieve tenancy information for each product that you are interfacing with. Once you have the requirements and you have installed Zscaler SDK Python, you're ready to go.
 
 ### Quick ZIA Example
 
 ```python
 from zscaler import ZIAClientHelper
@@ -77,15 +142,15 @@
 zpa = ZPAClientHelper(client_id='ZPA_CLIENT_ID', client_secret='ZPA_CLIENT_SECRET', customer_id='ZPA_CUSTOMER_ID', cloud='ZPA_CLOUD')
 for app_segment in zpa.app_segments.list_segments():
     pprint(app_segment)
 ```
 
 ~> **NOTE** The `ZPA_CLOUD` environment variable is optional and only required if your project needs to interact with any other ZPA cloud other than production cloud. In this case, use the `ZPA_CLOUD` environment variable followed by the name of the corresponding environment: `ZPA_CLOUD=BETA`, `ZPA_CLOUD=ZPATWO`, `ZPA_CLOUD=GOV`, `ZPA_CLOUD=GOVUS`, `ZPA_CLOUD=PREVIEW`, `ZPA_CLOUD=DEV`.
 
-## Pagination
+## Pagination<a id="pagination"></a>
 
 This SDK provides methods that retrieve a list of resources from the API, which return paginated results due to the volume of data. Each method capable of returning paginated data is prefixed as `list_` and handles the pagination internally by providing an easy interface to iterate through pages. The user does not need to manually fetch each page; instead, they can process items as they iterate through them.
 
 ### Example of Iterating Over Paginated Results
 
 The following example shows how you can list ZPA items using this SDK, processing each item one at a time. This pattern is useful for operations that need to handle large datasets efficiently.
 
@@ -127,15 +192,15 @@
 
 ### Efficient Pagination Handling
 
 For more details on each pagination parameter see:
 [ZPA Pagination Parameters](zscaler/zpa/README.md)
 [ZIA Pagination Parameters](zscaler/zia/README.md)
 
-## Logging
+## Logging<a id="logging"></a>
 
 The Zscaler SDK Python, provides robust logging for debug purposes.
 Logs are disabled by default and should be enabled explicitly via custom environment variable:
 
 * `ZSCALER_SDK_LOG` - Turn on logging
 * `ZSCALER_SDK_VERBOSE` - Turn on logging in verbose mode
 
@@ -146,25 +211,25 @@
 
 **NOTE**: DO NOT SET DEBUG LEVEL IN PRODUCTION!
 
 You should now see logs in your console. Notice that API tokens are **NOT** logged to the console; however, we still advise to use caution and never use `DEBUG` level logging in production.
 
 What it being logged? `requests`, `responses`,  `http errors`, `caching responses`.
 
-### Environment variables
+## Environment variables<a id="environment-variables"></a>
 
 Each one of the configuration values above can be turned into an environment variable name with the `_` (underscore) character and UPPERCASE characters. The following are accepted:
 
 - `ZSCALER_CLIENT_CACHE_ENABLED` - Enable or disable the caching mechanism within the clien
 - `ZSCALER_CLIENT_CACHE_DEFAULT_TTL` - Duration (in seconds) that cached data remains valid. By default data is cached in memory for `3600` seconds.
 - `ZSCALER_CLIENT_CACHE_DEFAULT_TTI` - This environment variable sets the maximum amount of time (in seconds) that cached data can remain in the cache without being accessed. If the cached data is not accessed within this timeframe, it is removed from the cache, regardless of its TTL. The default TTI is `1800` seconds (`30 minutes`) 
 - `ZSCALER_SDK_LOG` - Turn on logging
 - `ZSCALER_SDK_VERBOSE` - Turn on logging in verbose mode
 
-## Rate Limiting
+## Rate Limiting<a id="rate-limiting"></a>
 
 Zscaler provides unique rate limiting numbers for each individual product. Regardless of the product, a 429 response will be returned if too many requests are made within a given time. 
 Please see:
 * [ZPA Rate Limiting][rate-limiting-zpa] for rate limiting requirements.
 * [ZIA Rate Limiting][rate-limiting-zia] for a complete list of which endpoints are rate limited.
 
 When a 429 error is received, the `Retry-After` header will tell you the time at which you can retry. This section discusses the method for handling rate limiting with this SDK.
@@ -175,34 +240,49 @@
 
 Retry Conditions: The client for both ZPA and ZIA retries a request under the following conditions:
 
 * HTTP status code 429 (Too Many Requests): This indicates that the rate limit has been exceeded. The client waits for a duration specified by the `Retry-After` header, if present, or a default of `2 ` seconds, before retrying.
 
 * Exceptions during request execution: Any requests.RequestException encountered during the request triggers a retry, except on the last attempt, where the exception is raised.
 
-## Building the SDK
+## Building the SDK<a id="building-the-sdk"></a>
 
 In most cases, you won't need to build the SDK from source. If you want to build it yourself, you'll need these prerequisites:
 
 - Clone the repo
 - Run `make build:dist` from the root of the project (assuming Python is installed)
-- Ensure tests run succesfully. 
+- Ensure tests run succesfully by executing `make test-simple`
 - Install `tox` if not installed already using: `pip install tox`. 
 - Run tests using `tox` in the root directory of the project.
 
-## Contributing
+## Interface stability<a id="interface-stability"></a>
+
+Zscaler is actively working on stabilizing the Zscaler SDK for Python's interfaces.  
+You are highly encouraged to pin the exact dependency version and read the [changelog](https://github.com/zscaler/zscaler-sdk-python/blob/master/CHANGELOG.md) 
+where Zscaler documents the changes. Zscaler may have minor [documented](https://github.com/zscaler/zscaler-sdk-python/blob/master/CHANGELOG.md)
+backward-incompatible changes, such as renaming some type names to bring more consistency.
+
+## Contributing<a id="contributing"></a>
 
 At this moment we are not accepting contributions, but we welcome suggestions on how to improve this SDK or feature requests, which can then be added in  future releases.
 
 [zenith]: https://community.zscaler.com/
 [zscaler-support]: https://help.zscaler.com/contact-support
 [github-issues]: https://github.com/zscaler/zscaler-sdk-python/issues
 [rate-limiting-zpa]: https://help.zscaler.com/zpa/understanding-rate-limiting
 [rate-limiting-zia]: https://help.zscaler.com/zia/understanding-rate-limiting
 
+## Need help?<a id="need-help"></a>
+
+If you run into problems using the SDK, you can:
+
+- Ask questions on the [Zenith Community][zenith]
+- Post [issues on GitHub][github-issues] (for code errors)
+- Support [customer support portal][zscaler-support]
+
 Contributors
 ------------
 
 - William Guilherme - [willguibr](https://github.com/willguibr)
 - Eddie Parra - [eparra](https://github.com/eparra)
 - Paul Abbot - [abbottp](https://github.com/abbottp)
```

### Comparing `zscaler-sdk-python-0.1.0/PKG-INFO` & `zscaler-sdk-python-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,149 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.0
-Summary: Official Python SDK for the Zscaler Products
-Home-page: https://github.com/zscaler/zscaler-sdk-python
-Author: Zscaler Technology Alliances
+Version: 0.1.1
+Summary: Official Python SDK for the Zscaler Products (Beta)
+Home-page: https://zscaler-sdk-python.readthedocs.io
+Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
+Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.md
 
-# Official Python SDK for the Zscaler Products
+# Official Python SDK for the Zscaler Products (Beta)
 
-[![CI/CD](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml)
-[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/zscaler-sdk-python)](https://pypistats.org/packages/zscaler-sdk-python)
 [![License](https://img.shields.io/github/license/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python)
+[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
 [![Latest version released on PyPi](https://img.shields.io/pypi/v/zscaler-sdk-python.svg)](https://pypi.org/project/zscaler-sdk-python)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zscaler-sdk-python.svg)](https://pypi.python.org/pypi/zscaler-sdk-python/)
-[![GitHub Release](https://img.shields.io/github/release/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python/releases/)
 [![Zscaler Community](https://img.shields.io/badge/zscaler-community-blue)](https://community.zscaler.com/)
 
 ## Support Disclaimer
 
--> **Disclaimer:** Please refer to our [General Support Statement](docs/guides/support.md) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docs/guides/troubleshooting.md) for guidance on typical problems.
+-> **Disclaimer:** Please refer to our [General Support Statement](docsrc/zs/guides/support.rst) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docsrc/zs/guides/troubleshooting.rst) for guidance on typical problems.
 
 ## Zscaler Python SDK Overview
 
-This repository contains the Zscaler SDK for Python. This SDK can be used to interact with several Zscaler services such as:
+The Zscaler SDK for Python includes functionality to accelerate development with [Python](https://www.python.org/) several Zscaler services such as:
 
-* Zscaler Private Access (ZPA)
-* Zscaler Internet Access (ZIA)
+* [Zscaler Internet Access (ZIA)](https://help.zscaler.com/zia/getting-started-zia-api)
+* [Zscaler Private Access (ZPA)](https://help.zscaler.com/zpa/getting-started-zpa-api)
 * [Documentation](http://zscaler-sdk-python.readthedocs.io)
 
------
+Each package is supportedd by an individual and robust HTTP client designed to handle failures on different levels by performing intelligent retries.
 
-Each Zscaler product has separate developer documentation and authentication methods. This SDK aims to simplify
-software development using the Zscaler API for both customers and partners.
+**Beta:** This SDK is supported for production use cases, but we do expect future releases to have some interface changes; see [Interface stability](#interface-stability). 
+We are keen to hear feedback from you on these SDKs. Please [file issues](https://github.com/zscaler/zscaler-sdk-python/issues), and we will address them. 
+
+## Contents
 
-- [Release Status](#release-status)
-- [Need help?](#need-help)
 - [Getting Started](#getting-started)
+- [Usage](#usage)
+- [Authentication](#authentication)
 - [Pagination](#pagination)
 - [Logging](#logging)
 - [Rate Limiting](#rate-limiting)
 - [Environment variables](#environment-variables)
 - [Building the SDK](#building-the-sdk)
+- [Interface stability](#interface-stability)
+- [Need help?](#need-help)
 - [Contributing](#contributing)
 
 > Requires Python version 3.8.0 or higher.
 
-## Need help?
+## Getting started<a id="getting-started"></a>
 
-If you run into problems using the SDK, you can:
+To install the Zscaler Python SDK in your project:
+1. Please install Zscaler SDK for Python via `pip install zscaler-sdk-python` and instantiate the respective client based on your project usage:
+- `ZIAClientHelper`
+- `ZPAClientHelper`
 
-- Ask questions on the [Zenith Community][zenith]
-- Post [issues on GitHub][github-issues] (for code errors)
-- Support [customer support portal][zscaler-support]
+Zscaler SDK for Python is compatible with Python 3.7 _(until [June 2023](https://devguide.python.org/versions/))_, 3.8, 3.9, 3.10, and 3.11.
 
-## Getting started
+The upgrade to the latest version of this SDK can be done by executing the following command:
+```python
+%pip install --upgrade zscaler-sdk-python
+```
+followed by
+```python
+dbutils.library.restartPython()
+```
 
-To install the Zscaler Python SDK in your project:
+## Authentication<a id="authentication"></a>
 
-```sh
-pip install zscaler-sdk-python
-```
+Each Zscaler product has separate developer documentation and authentication methods. In this section you will find
+
+1. Credentials that are hard-coded into configuration arguments.
+
+   :warning: **Caution**: Zscaler does not recommend hard-coding credentials into arguments, as they can be exposed in plain text in version control systems. Use environment variables instead.
+
+### ZIA native authentication
+
+- For authentication via Zscaler Internet Access, you must provide `username`, `password`, `api_key` and `cloud`
 
-## Usage
+The ZIA Cloud is identified by several cloud name prefixes, which determines which API endpoint the requests should be sent to. The following cloud environments are supported:
+
+* `zscaler`
+* `zscalerone`
+* `zscalertwo`
+* `zscalerthree`
+* `zscloud`
+* `zscalerbeta`
+* `zscalergov`
+* `zscalerten`
+* `zspreview`
+
+### Environment variables
+
+You can provide credentials via the `ZIA_USERNAME`, `ZIA_PASSWORD`, `ZIA_API_KEY`, `ZIA_CLOUD` environment variables, representing your ZIA `username`, `password`, `api_key` and `cloud` respectively.
+
+| Argument     | Description | Environment variable |
+|--------------|-------------|-------------------|
+| `username`       | _(String)_ A string that contains the email ID of the API admin.| `ZIA_USERNAME` |    
+| `password`       | _(String)_ A string that contains the password for the API admin.| `ZIA_PASSWORD` |
+| `api_key`       | _(String)_ A string that contains the obfuscated API key (i.e., the return value of the obfuscateApiKey() method).| `ZIA_API_KEY` |   
+| `cloud`       | _(String)_ The host and basePath for the cloud services API is `$zsapi.<Zscaler Cloud Name>/api/v1`.| `ZIA_CLOUD` |
+
+### ZPA native authentication
+
+- For authentication via Zscaler Private Access, you must provide `client_id`, `client_secret`, `customer_id` and `cloud`
+
+The ZPA Cloud is identified by several cloud name prefixes, which determines which API endpoint the requests should be sent to. The following cloud environments are supported:
+
+* `PRODUCTION`
+* `ZPATWO`
+* `BETA`
+* `GOV`
+* `GOVUS`
+
+### Environment variables
+
+You can provide credentials via the `ZPA_CLIENT_ID`, `ZPA_CLIENT_SECRET`, `ZPA_CUSTOMER_ID`, `ZPA_CLOUD` environment variables, representing your ZPA `client_id`, `client_secret`, `customer_id` and `cloud` of your ZPA account, respectively.
+
+~> **NOTE** `ZPA_CLOUD` environment variable is required, and is used to identify the correct API gateway where the API requests should be forwarded to.
+
+| Argument     | Description | Environment variable |
+|--------------|-------------|-------------------|
+| `client_id`       | _(String)_ The ZPA API client ID generated from the ZPA console.| `ZPA_CLIENT_ID` |    
+| `client_secret`       | _(String)_ The ZPA API client secret generated from the ZPA console.| `ZPA_CLIENT_SECRET` |
+| `customer_id`       | _(String)_ The ZPA tenant ID found in the Administration > Company menu in the ZPA console.| `ZPA_CUSTOMER_ID` |   
+| `cloud`       | _(String)_ The Zscaler cloud for your tenancy.| `ZPA_CLOUD` |
+
+## Usage<a id="usage"></a>
 
 Before you can interact with any of the Zscaler APIs, you need to generate API keys or retrieve tenancy information for each product that you are interfacing with. Once you have the requirements and you have installed Zscaler SDK Python, you're ready to go.
 
 ### Quick ZIA Example
 
 ```python
 from zscaler import ZIAClientHelper
@@ -88,15 +163,15 @@
 zpa = ZPAClientHelper(client_id='ZPA_CLIENT_ID', client_secret='ZPA_CLIENT_SECRET', customer_id='ZPA_CUSTOMER_ID', cloud='ZPA_CLOUD')
 for app_segment in zpa.app_segments.list_segments():
     pprint(app_segment)
 ```
 
 ~> **NOTE** The `ZPA_CLOUD` environment variable is optional and only required if your project needs to interact with any other ZPA cloud other than production cloud. In this case, use the `ZPA_CLOUD` environment variable followed by the name of the corresponding environment: `ZPA_CLOUD=BETA`, `ZPA_CLOUD=ZPATWO`, `ZPA_CLOUD=GOV`, `ZPA_CLOUD=GOVUS`, `ZPA_CLOUD=PREVIEW`, `ZPA_CLOUD=DEV`.
 
-## Pagination
+## Pagination<a id="pagination"></a>
 
 This SDK provides methods that retrieve a list of resources from the API, which return paginated results due to the volume of data. Each method capable of returning paginated data is prefixed as `list_` and handles the pagination internally by providing an easy interface to iterate through pages. The user does not need to manually fetch each page; instead, they can process items as they iterate through them.
 
 ### Example of Iterating Over Paginated Results
 
 The following example shows how you can list ZPA items using this SDK, processing each item one at a time. This pattern is useful for operations that need to handle large datasets efficiently.
 
@@ -138,15 +213,15 @@
 
 ### Efficient Pagination Handling
 
 For more details on each pagination parameter see:
 [ZPA Pagination Parameters](zscaler/zpa/README.md)
 [ZIA Pagination Parameters](zscaler/zia/README.md)
 
-## Logging
+## Logging<a id="logging"></a>
 
 The Zscaler SDK Python, provides robust logging for debug purposes.
 Logs are disabled by default and should be enabled explicitly via custom environment variable:
 
 * `ZSCALER_SDK_LOG` - Turn on logging
 * `ZSCALER_SDK_VERBOSE` - Turn on logging in verbose mode
 
@@ -157,25 +232,25 @@
 
 **NOTE**: DO NOT SET DEBUG LEVEL IN PRODUCTION!
 
 You should now see logs in your console. Notice that API tokens are **NOT** logged to the console; however, we still advise to use caution and never use `DEBUG` level logging in production.
 
 What it being logged? `requests`, `responses`,  `http errors`, `caching responses`.
 
-### Environment variables
+## Environment variables<a id="environment-variables"></a>
 
 Each one of the configuration values above can be turned into an environment variable name with the `_` (underscore) character and UPPERCASE characters. The following are accepted:
 
 - `ZSCALER_CLIENT_CACHE_ENABLED` - Enable or disable the caching mechanism within the clien
 - `ZSCALER_CLIENT_CACHE_DEFAULT_TTL` - Duration (in seconds) that cached data remains valid. By default data is cached in memory for `3600` seconds.
 - `ZSCALER_CLIENT_CACHE_DEFAULT_TTI` - This environment variable sets the maximum amount of time (in seconds) that cached data can remain in the cache without being accessed. If the cached data is not accessed within this timeframe, it is removed from the cache, regardless of its TTL. The default TTI is `1800` seconds (`30 minutes`) 
 - `ZSCALER_SDK_LOG` - Turn on logging
 - `ZSCALER_SDK_VERBOSE` - Turn on logging in verbose mode
 
-## Rate Limiting
+## Rate Limiting<a id="rate-limiting"></a>
 
 Zscaler provides unique rate limiting numbers for each individual product. Regardless of the product, a 429 response will be returned if too many requests are made within a given time. 
 Please see:
 * [ZPA Rate Limiting][rate-limiting-zpa] for rate limiting requirements.
 * [ZIA Rate Limiting][rate-limiting-zia] for a complete list of which endpoints are rate limited.
 
 When a 429 error is received, the `Retry-After` header will tell you the time at which you can retry. This section discusses the method for handling rate limiting with this SDK.
@@ -186,34 +261,49 @@
 
 Retry Conditions: The client for both ZPA and ZIA retries a request under the following conditions:
 
 * HTTP status code 429 (Too Many Requests): This indicates that the rate limit has been exceeded. The client waits for a duration specified by the `Retry-After` header, if present, or a default of `2 ` seconds, before retrying.
 
 * Exceptions during request execution: Any requests.RequestException encountered during the request triggers a retry, except on the last attempt, where the exception is raised.
 
-## Building the SDK
+## Building the SDK<a id="building-the-sdk"></a>
 
 In most cases, you won't need to build the SDK from source. If you want to build it yourself, you'll need these prerequisites:
 
 - Clone the repo
 - Run `make build:dist` from the root of the project (assuming Python is installed)
-- Ensure tests run succesfully. 
+- Ensure tests run succesfully by executing `make test-simple`
 - Install `tox` if not installed already using: `pip install tox`. 
 - Run tests using `tox` in the root directory of the project.
 
-## Contributing
+## Interface stability<a id="interface-stability"></a>
+
+Zscaler is actively working on stabilizing the Zscaler SDK for Python's interfaces.  
+You are highly encouraged to pin the exact dependency version and read the [changelog](https://github.com/zscaler/zscaler-sdk-python/blob/master/CHANGELOG.md) 
+where Zscaler documents the changes. Zscaler may have minor [documented](https://github.com/zscaler/zscaler-sdk-python/blob/master/CHANGELOG.md)
+backward-incompatible changes, such as renaming some type names to bring more consistency.
+
+## Contributing<a id="contributing"></a>
 
 At this moment we are not accepting contributions, but we welcome suggestions on how to improve this SDK or feature requests, which can then be added in  future releases.
 
 [zenith]: https://community.zscaler.com/
 [zscaler-support]: https://help.zscaler.com/contact-support
 [github-issues]: https://github.com/zscaler/zscaler-sdk-python/issues
 [rate-limiting-zpa]: https://help.zscaler.com/zpa/understanding-rate-limiting
 [rate-limiting-zia]: https://help.zscaler.com/zia/understanding-rate-limiting
 
+## Need help?<a id="need-help"></a>
+
+If you run into problems using the SDK, you can:
+
+- Ask questions on the [Zenith Community][zenith]
+- Post [issues on GitHub][github-issues] (for code errors)
+- Support [customer support portal][zscaler-support]
+
 Contributors
 ------------
 
 - William Guilherme - [willguibr](https://github.com/willguibr)
 - Eddie Parra - [eparra](https://github.com/eparra)
 - Paul Abbot - [abbottp](https://github.com/abbottp)
```

### Comparing `zscaler-sdk-python-0.1.0/README.md` & `zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,149 @@
-# Official Python SDK for the Zscaler Products
+Metadata-Version: 2.1
+Name: zscaler-sdk-python
+Version: 0.1.1
+Summary: Official Python SDK for the Zscaler Products (Beta)
+Home-page: https://zscaler-sdk-python.readthedocs.io
+Author: Zscaler, Inc.
+Author-email: devrel@zscaler.com
+Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8,<4.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
 
-[![CI/CD](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml/badge.svg)](https://github.com/zscaler/zscaler-sdk-python/actions/workflows/ci.yml)
-[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
+# Official Python SDK for the Zscaler Products (Beta)
+
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/zscaler-sdk-python)](https://pypistats.org/packages/zscaler-sdk-python)
 [![License](https://img.shields.io/github/license/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python)
+[![Documentation Status](https://readthedocs.org/projects/zscaler-sdk-python/badge/?version=latest)](https://zscaler-sdk-python.readthedocs.io/en/latest/?badge=latest)
 [![Latest version released on PyPi](https://img.shields.io/pypi/v/zscaler-sdk-python.svg)](https://pypi.org/project/zscaler-sdk-python)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zscaler-sdk-python.svg)](https://pypi.python.org/pypi/zscaler-sdk-python/)
-[![GitHub Release](https://img.shields.io/github/release/zscaler/zscaler-sdk-python.svg)](https://github.com/zscaler/zscaler-sdk-python/releases/)
 [![Zscaler Community](https://img.shields.io/badge/zscaler-community-blue)](https://community.zscaler.com/)
 
 ## Support Disclaimer
 
--> **Disclaimer:** Please refer to our [General Support Statement](docs/guides/support.md) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docs/guides/troubleshooting.md) for guidance on typical problems.
+-> **Disclaimer:** Please refer to our [General Support Statement](docsrc/zs/guides/support.rst) before proceeding with the use of this provider. You can also refer to our [troubleshooting guide](docsrc/zs/guides/troubleshooting.rst) for guidance on typical problems.
 
 ## Zscaler Python SDK Overview
 
-This repository contains the Zscaler SDK for Python. This SDK can be used to interact with several Zscaler services such as:
+The Zscaler SDK for Python includes functionality to accelerate development with [Python](https://www.python.org/) several Zscaler services such as:
 
-* Zscaler Private Access (ZPA)
-* Zscaler Internet Access (ZIA)
+* [Zscaler Internet Access (ZIA)](https://help.zscaler.com/zia/getting-started-zia-api)
+* [Zscaler Private Access (ZPA)](https://help.zscaler.com/zpa/getting-started-zpa-api)
 * [Documentation](http://zscaler-sdk-python.readthedocs.io)
 
------
+Each package is supportedd by an individual and robust HTTP client designed to handle failures on different levels by performing intelligent retries.
 
-Each Zscaler product has separate developer documentation and authentication methods. This SDK aims to simplify
-software development using the Zscaler API for both customers and partners.
+**Beta:** This SDK is supported for production use cases, but we do expect future releases to have some interface changes; see [Interface stability](#interface-stability). 
+We are keen to hear feedback from you on these SDKs. Please [file issues](https://github.com/zscaler/zscaler-sdk-python/issues), and we will address them. 
+
+## Contents
 
-- [Release Status](#release-status)
-- [Need help?](#need-help)
 - [Getting Started](#getting-started)
+- [Usage](#usage)
+- [Authentication](#authentication)
 - [Pagination](#pagination)
 - [Logging](#logging)
 - [Rate Limiting](#rate-limiting)
 - [Environment variables](#environment-variables)
 - [Building the SDK](#building-the-sdk)
+- [Interface stability](#interface-stability)
+- [Need help?](#need-help)
 - [Contributing](#contributing)
 
 > Requires Python version 3.8.0 or higher.
 
-## Need help?
+## Getting started<a id="getting-started"></a>
 
-If you run into problems using the SDK, you can:
+To install the Zscaler Python SDK in your project:
+1. Please install Zscaler SDK for Python via `pip install zscaler-sdk-python` and instantiate the respective client based on your project usage:
+- `ZIAClientHelper`
+- `ZPAClientHelper`
 
-- Ask questions on the [Zenith Community][zenith]
-- Post [issues on GitHub][github-issues] (for code errors)
-- Support [customer support portal][zscaler-support]
+Zscaler SDK for Python is compatible with Python 3.7 _(until [June 2023](https://devguide.python.org/versions/))_, 3.8, 3.9, 3.10, and 3.11.
 
-## Getting started
+The upgrade to the latest version of this SDK can be done by executing the following command:
+```python
+%pip install --upgrade zscaler-sdk-python
+```
+followed by
+```python
+dbutils.library.restartPython()
+```
 
-To install the Zscaler Python SDK in your project:
+## Authentication<a id="authentication"></a>
 
-```sh
-pip install zscaler-sdk-python
-```
+Each Zscaler product has separate developer documentation and authentication methods. In this section you will find
+
+1. Credentials that are hard-coded into configuration arguments.
+
+   :warning: **Caution**: Zscaler does not recommend hard-coding credentials into arguments, as they can be exposed in plain text in version control systems. Use environment variables instead.
+
+### ZIA native authentication
+
+- For authentication via Zscaler Internet Access, you must provide `username`, `password`, `api_key` and `cloud`
 
-## Usage
+The ZIA Cloud is identified by several cloud name prefixes, which determines which API endpoint the requests should be sent to. The following cloud environments are supported:
+
+* `zscaler`
+* `zscalerone`
+* `zscalertwo`
+* `zscalerthree`
+* `zscloud`
+* `zscalerbeta`
+* `zscalergov`
+* `zscalerten`
+* `zspreview`
+
+### Environment variables
+
+You can provide credentials via the `ZIA_USERNAME`, `ZIA_PASSWORD`, `ZIA_API_KEY`, `ZIA_CLOUD` environment variables, representing your ZIA `username`, `password`, `api_key` and `cloud` respectively.
+
+| Argument     | Description | Environment variable |
+|--------------|-------------|-------------------|
+| `username`       | _(String)_ A string that contains the email ID of the API admin.| `ZIA_USERNAME` |    
+| `password`       | _(String)_ A string that contains the password for the API admin.| `ZIA_PASSWORD` |
+| `api_key`       | _(String)_ A string that contains the obfuscated API key (i.e., the return value of the obfuscateApiKey() method).| `ZIA_API_KEY` |   
+| `cloud`       | _(String)_ The host and basePath for the cloud services API is `$zsapi.<Zscaler Cloud Name>/api/v1`.| `ZIA_CLOUD` |
+
+### ZPA native authentication
+
+- For authentication via Zscaler Private Access, you must provide `client_id`, `client_secret`, `customer_id` and `cloud`
+
+The ZPA Cloud is identified by several cloud name prefixes, which determines which API endpoint the requests should be sent to. The following cloud environments are supported:
+
+* `PRODUCTION`
+* `ZPATWO`
+* `BETA`
+* `GOV`
+* `GOVUS`
+
+### Environment variables
+
+You can provide credentials via the `ZPA_CLIENT_ID`, `ZPA_CLIENT_SECRET`, `ZPA_CUSTOMER_ID`, `ZPA_CLOUD` environment variables, representing your ZPA `client_id`, `client_secret`, `customer_id` and `cloud` of your ZPA account, respectively.
+
+~> **NOTE** `ZPA_CLOUD` environment variable is required, and is used to identify the correct API gateway where the API requests should be forwarded to.
+
+| Argument     | Description | Environment variable |
+|--------------|-------------|-------------------|
+| `client_id`       | _(String)_ The ZPA API client ID generated from the ZPA console.| `ZPA_CLIENT_ID` |    
+| `client_secret`       | _(String)_ The ZPA API client secret generated from the ZPA console.| `ZPA_CLIENT_SECRET` |
+| `customer_id`       | _(String)_ The ZPA tenant ID found in the Administration > Company menu in the ZPA console.| `ZPA_CUSTOMER_ID` |   
+| `cloud`       | _(String)_ The Zscaler cloud for your tenancy.| `ZPA_CLOUD` |
+
+## Usage<a id="usage"></a>
 
 Before you can interact with any of the Zscaler APIs, you need to generate API keys or retrieve tenancy information for each product that you are interfacing with. Once you have the requirements and you have installed Zscaler SDK Python, you're ready to go.
 
 ### Quick ZIA Example
 
 ```python
 from zscaler import ZIAClientHelper
@@ -77,15 +163,15 @@
 zpa = ZPAClientHelper(client_id='ZPA_CLIENT_ID', client_secret='ZPA_CLIENT_SECRET', customer_id='ZPA_CUSTOMER_ID', cloud='ZPA_CLOUD')
 for app_segment in zpa.app_segments.list_segments():
     pprint(app_segment)
 ```
 
 ~> **NOTE** The `ZPA_CLOUD` environment variable is optional and only required if your project needs to interact with any other ZPA cloud other than production cloud. In this case, use the `ZPA_CLOUD` environment variable followed by the name of the corresponding environment: `ZPA_CLOUD=BETA`, `ZPA_CLOUD=ZPATWO`, `ZPA_CLOUD=GOV`, `ZPA_CLOUD=GOVUS`, `ZPA_CLOUD=PREVIEW`, `ZPA_CLOUD=DEV`.
 
-## Pagination
+## Pagination<a id="pagination"></a>
 
 This SDK provides methods that retrieve a list of resources from the API, which return paginated results due to the volume of data. Each method capable of returning paginated data is prefixed as `list_` and handles the pagination internally by providing an easy interface to iterate through pages. The user does not need to manually fetch each page; instead, they can process items as they iterate through them.
 
 ### Example of Iterating Over Paginated Results
 
 The following example shows how you can list ZPA items using this SDK, processing each item one at a time. This pattern is useful for operations that need to handle large datasets efficiently.
 
@@ -127,15 +213,15 @@
 
 ### Efficient Pagination Handling
 
 For more details on each pagination parameter see:
 [ZPA Pagination Parameters](zscaler/zpa/README.md)
 [ZIA Pagination Parameters](zscaler/zia/README.md)
 
-## Logging
+## Logging<a id="logging"></a>
 
 The Zscaler SDK Python, provides robust logging for debug purposes.
 Logs are disabled by default and should be enabled explicitly via custom environment variable:
 
 * `ZSCALER_SDK_LOG` - Turn on logging
 * `ZSCALER_SDK_VERBOSE` - Turn on logging in verbose mode
 
@@ -146,25 +232,25 @@
 
 **NOTE**: DO NOT SET DEBUG LEVEL IN PRODUCTION!
 
 You should now see logs in your console. Notice that API tokens are **NOT** logged to the console; however, we still advise to use caution and never use `DEBUG` level logging in production.
 
 What it being logged? `requests`, `responses`,  `http errors`, `caching responses`.
 
-### Environment variables
+## Environment variables<a id="environment-variables"></a>
 
 Each one of the configuration values above can be turned into an environment variable name with the `_` (underscore) character and UPPERCASE characters. The following are accepted:
 
 - `ZSCALER_CLIENT_CACHE_ENABLED` - Enable or disable the caching mechanism within the clien
 - `ZSCALER_CLIENT_CACHE_DEFAULT_TTL` - Duration (in seconds) that cached data remains valid. By default data is cached in memory for `3600` seconds.
 - `ZSCALER_CLIENT_CACHE_DEFAULT_TTI` - This environment variable sets the maximum amount of time (in seconds) that cached data can remain in the cache without being accessed. If the cached data is not accessed within this timeframe, it is removed from the cache, regardless of its TTL. The default TTI is `1800` seconds (`30 minutes`) 
 - `ZSCALER_SDK_LOG` - Turn on logging
 - `ZSCALER_SDK_VERBOSE` - Turn on logging in verbose mode
 
-## Rate Limiting
+## Rate Limiting<a id="rate-limiting"></a>
 
 Zscaler provides unique rate limiting numbers for each individual product. Regardless of the product, a 429 response will be returned if too many requests are made within a given time. 
 Please see:
 * [ZPA Rate Limiting][rate-limiting-zpa] for rate limiting requirements.
 * [ZIA Rate Limiting][rate-limiting-zia] for a complete list of which endpoints are rate limited.
 
 When a 429 error is received, the `Retry-After` header will tell you the time at which you can retry. This section discusses the method for handling rate limiting with this SDK.
@@ -175,34 +261,49 @@
 
 Retry Conditions: The client for both ZPA and ZIA retries a request under the following conditions:
 
 * HTTP status code 429 (Too Many Requests): This indicates that the rate limit has been exceeded. The client waits for a duration specified by the `Retry-After` header, if present, or a default of `2 ` seconds, before retrying.
 
 * Exceptions during request execution: Any requests.RequestException encountered during the request triggers a retry, except on the last attempt, where the exception is raised.
 
-## Building the SDK
+## Building the SDK<a id="building-the-sdk"></a>
 
 In most cases, you won't need to build the SDK from source. If you want to build it yourself, you'll need these prerequisites:
 
 - Clone the repo
 - Run `make build:dist` from the root of the project (assuming Python is installed)
-- Ensure tests run succesfully. 
+- Ensure tests run succesfully by executing `make test-simple`
 - Install `tox` if not installed already using: `pip install tox`. 
 - Run tests using `tox` in the root directory of the project.
 
-## Contributing
+## Interface stability<a id="interface-stability"></a>
+
+Zscaler is actively working on stabilizing the Zscaler SDK for Python's interfaces.  
+You are highly encouraged to pin the exact dependency version and read the [changelog](https://github.com/zscaler/zscaler-sdk-python/blob/master/CHANGELOG.md) 
+where Zscaler documents the changes. Zscaler may have minor [documented](https://github.com/zscaler/zscaler-sdk-python/blob/master/CHANGELOG.md)
+backward-incompatible changes, such as renaming some type names to bring more consistency.
+
+## Contributing<a id="contributing"></a>
 
 At this moment we are not accepting contributions, but we welcome suggestions on how to improve this SDK or feature requests, which can then be added in  future releases.
 
 [zenith]: https://community.zscaler.com/
 [zscaler-support]: https://help.zscaler.com/contact-support
 [github-issues]: https://github.com/zscaler/zscaler-sdk-python/issues
 [rate-limiting-zpa]: https://help.zscaler.com/zpa/understanding-rate-limiting
 [rate-limiting-zia]: https://help.zscaler.com/zia/understanding-rate-limiting
 
+## Need help?<a id="need-help"></a>
+
+If you run into problems using the SDK, you can:
+
+- Ask questions on the [Zenith Community][zenith]
+- Post [issues on GitHub][github-issues] (for code errors)
+- Support [customer support portal][zscaler-support]
+
 Contributors
 ------------
 
 - William Guilherme - [willguibr](https://github.com/willguibr)
 - Eddie Parra - [eparra](https://github.com/eparra)
 - Paul Abbot - [abbottp](https://github.com/abbottp)
```

### Comparing `zscaler-sdk-python-0.1.0/docsrc/conf.py` & `zscaler-sdk-python-0.1.1/docsrc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,31 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-import zscaler
 
-sys.path.insert(0, os.path.abspath("../"))
+sys.path.insert(0, os.path.abspath('..'))
 
 # Check if building documentation on RTD
 on_rtd = os.environ.get("READTHEDOCS", None) == "True"
 
 # -- Project information -----------------------------------------------------
 
 project = "Zscaler SDK Python"
 copyright = "2023, Zscaler Inc."
 author = "Zscaler Technology Alliances"
 html_title = ""
 
 # The short X.Y version
-version = '0.1.0'
+version = '0.1.1'
 # The full version, including alpha/beta/rc tags
-release = '0.1.0'
+release = '0.1.1'
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -111,15 +110,15 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "Zscalerdoc"
+htmlhelp_basename = "zscalerdoc"
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
@@ -137,15 +136,15 @@
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     (
         master_doc,
         "Zscaler.tex",
-        "Zscaler Documentation",
+        "Zscaler SDK Python Documentation",
         "Zscaler Technology Alliances",
         "manual",
     ),
 ]
 
 # -- Options for manual page output ------------------------------------------
 
@@ -191,15 +190,14 @@
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "restfly": ("https://restfly.readthedocs.io/en/latest/", None),
-    "box": ("https://box.readthedocs.io/en/latest", None),
 }
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
```

### Comparing `zscaler-sdk-python-0.1.0/docsrc/index.rst` & `zscaler-sdk-python-0.1.1/docsrc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .. meta::
    :description lang=en:
         Official Zscaler Python  SDK that provides a simple and uniform interface for each of the Zscaler product APIs.
 .. toctree::
-   :maxdepth: 1
+   :maxdepth: 2
    :hidden:
    :caption: Contents
 
    zs/zia/index
    zs/zpa/index
    zs/guides/index
 
-Zscaler SDK Python - Library Reference
+Zscaler SDK Python (Beta) - Library Reference
 =====================================================================
 Zscaler SDK Python is an SDK that provides a uniform and easy-to-use interface for each of the Zscaler product APIs.
 
 Support Disclaimer
 ========================
 
 -> **Disclaimer:** Please refer to our `General Support Statement <docs/guides/support.rst>`_ before proceeding with the use of this provider. 
@@ -45,15 +45,15 @@
 Products
 ---------
 This repository contains the Zscaler SDK for Python. This SDK can be used to interact with several Zscaler services such as:
 
 - :doc:`Zscaler Private Access (ZPA) <zs/zpa/index>`
 - :doc:`Zscaler Internet Access (ZIA) <zs/zia/index>`
 
-* `Documentation <https://://zscaler-sdk-python.readthedocs.io>`_
+* `Documentation <https://zscaler-sdk-python.readthedocs.io>`_
 
 Installation
 ==============
 
 The most recent version can be installed from pypi as per below.
 
 .. code-block:: console
```

### Comparing `zscaler-sdk-python-0.1.0/docsrc/zs/guides/examples.rst` & `zscaler-sdk-python-0.1.1/docsrc/zs/guides/examples.rst`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/docsrc/zs/guides/support.rst` & `zscaler-sdk-python-0.1.1/docsrc/zs/guides/support.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 The Zscaler Python SDK is supported and maintained by the Zscaler Technology Alliances team in partnership with Zscaler Engineering, and we welcome questions on how to use this SDK.
 Please, refer to our `troubleshooting guide <troubleshooting.rst>`_ for guidance on typical problems.
 
 Support Ticket Severity
 -----------------------
 
 Support tickets related to the GO SDK can be opened with `Zscaler Support <https://help.zscaler.com/login-tickets>`_, however since the SDK is just a client of the underlying product API, we will **NOT** be able to treat SDK related support requests as a Severity-1 (Immediate time frame).
-
 When reporting bugs, please provide the Terraform script that demonstrates the bug and the command output. Stack traces will also be helpful.
 
 Notice that we will **NOT**, however, fix bugs upon customer demand, as we have to prioritize all pending bugs and features, as part of the product's backlog and release cycles.
 
 Urgent, production related Terraform issues can be resolved via direct interaction with the underlying API or UI. We will ask customers to resort to these methods to resolve downtime or urgent issues. If you have an urgent escalation, please contact your local Zscaler account team (RSM/SE/CSM/TAM) for assistance.
 
 Contact
 -------
 
 For questions or requests that cannot be submitted via GitHub Issues, please contact ``devrel@zscaler.com`` with "Zscaler-SDK-GO" in the subject line.
-We also provide a `private Slack channel <https://docs.google.com/forms/d/e/1FAIpQLSfkd3EMkLQdIWMNQ7QCr8TrH_xVSwSYcQshfBPDEZFOaF28qA/viewform?usp=sf_link>`_ where you can submit your questions to the SDK maintainers. Notice that this form will be reviewed and approved by Zscaler Technology Alliances team.
+We also provide a `private Slack channel <https://docs.google.com/forms/d/e/1FAIpQLSfkd3EMkLQdIWMNQ7QCr8TrH_xVSwSYcQshfBPDEZFOaF28qA/viewform?usp=sf_link>`_ 
+where you can submit your questions to the SDK maintainers. Notice that this form will be reviewed and approved by Zscaler Technology Alliances team.
```

### Comparing `zscaler-sdk-python-0.1.0/docsrc/zs/zia/url_categories.rst` & `zscaler-sdk-python-0.1.1/docsrc/zs/zia/url_categories.rst`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/conftest.py` & `zscaler-sdk-python-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/conftest.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_activation.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 #     yield
 
 # class TestActivation:
 #     """
 #     Integration Tests for the ZIA Activation
 #     """
 
-#     @pytest.mark.asyncio
-#     async def test_activation(self, fs):
+#     def test_activation(self, fs):
 #         client = MockZIAClient(fs)
 #         errors = []  # Initialize an empty list to collect errors
 
 #         # Test Config Status
 #         try:
 #             config_status = client.activate.status()
 #             # Allow for both "ACTIVE" and "PENDING" statuses
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_admin_and_role_management.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_admin_and_role_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestAdminRole:
     """
     Integration Tests for the admin roles
     """
 
-    @pytest.mark.asyncio
-    async def test_admin_role_management(self, fs):
+    def test_admin_role_management(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List all roles
             roles = client.admin_and_role_management.list_roles()
             assert isinstance(roles, list), "Expected a list of roles"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_authentication_settings.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_authentication_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,39 +34,36 @@
 
 
 class TestExemptedUrls:
     """
     Integration Tests for Authentication Settings Exempted URLs.
     """
 
-    @pytest.mark.asyncio
-    async def test_add_urls_to_exempt_list(self, fs):
+    def test_add_urls_to_exempt_list(self, fs):
         client = MockZIAClient(fs)
         urls_to_add = ["example.com", "testsite.com"]
         try:
             updated_exempt_list = (
                 client.authentication_settings.add_urls_to_exempt_list(urls_to_add)
             )
             assert (
                 updated_exempt_list is not None
             ), "The update exempt list operation returned None."
         except Exception as exc:
             pytest.fail(f"Failed to add URLs to exempt list: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_get_exempted_urls(self, fs):
+    def test_get_exempted_urls(self, fs):
         client = MockZIAClient(fs)
         try:
             exempt_list = client.authentication_settings.get_exempted_urls()
             assert isinstance(exempt_list, list), "Failed to retrieve exempt list."
         except Exception as exc:
             pytest.fail(f"Exempt list retrieval failed: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_delete_urls_from_exempt_list(self, fs):
+    def test_delete_urls_from_exempt_list(self, fs):
         client = MockZIAClient(fs)
         try:
             urls_to_clean = ["example.com", "testsite.com"]
             client.authentication_settings.delete_urls_from_exempt_list(urls_to_clean)
             print("Cleanup successful for exempt URLs list.")
         except Exception as exc:
             print(f"Cleanup failed for exempt URLs list: {exc}")
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestCloudFirewallIPDestinationGroup:
     """
     Integration Tests for the Cloud Firewall IP Destination Group.
     """
 
-    @pytest.mark.asyncio
-    async def test_cloud_firewall_ip_destination_group(self, fs):
+    def test_cloud_firewall_ip_destination_group(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         group_name = "tests-" + generate_random_string()
         group_description = "tests-" + generate_random_string()
         group_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_ip_source_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_source_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestCloudFirewallIPSourceGroup:
     """
     Integration Tests for the Cloud Firewall IP Source Group.
     """
 
-    @pytest.mark.asyncio
-    async def test_add_ip_source_group(self, fs):
+    def test_add_ip_source_group(self, fs):
         client = MockZIAClient(fs)
         errors = []
 
         group_name = "tests-" + generate_random_string()
         group_description = "tests-" + generate_random_string()
         group_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_cloud_firewall_rule.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestFirewallRules:
     """
     Integration Tests for the ZIA Firewall Rules
     """
 
-    @pytest.mark.asyncio
-    async def test_firewall_rule(self, fs):
+    def test_firewall_rule(self, fs):
         client = MockZIAClient(fs)
         errors = []
         dst_group_id = None
         src_group_id = None
         rule_id = None
 
         try:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_dictionary.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestDLPDictionary:
     """
     Integration Tests for the DLP dictionary
     """
 
-    @pytest.mark.asyncio
-    async def test_dlp_dictionary(self, fs):
+    def test_dlp_dictionary(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         dict_id = None  # Placeholder for the dictionary ID
         custom_phrase_match_type = "MATCH_ALL_CUSTOM_PHRASE_PATTERN_DICTIONARY"
         dictionary_type = "PATTERNS_AND_PHRASES"
         phrases = ([{"action": "PHRASE_COUNT_TYPE_ALL", "phrase": "test"}],)
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_engines.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_engines.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestDLPEngines:
     """
     Integration Tests for the DLP Engines
     """
 
-    @pytest.mark.asyncio
-    async def test_dlp_engines(self, fs):
+    def test_dlp_engines(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         engine_name = "tests-" + generate_random_string()
         engine_description = "tests-" + generate_random_string()
         engine_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_icap_server.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_icap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TestDLPIcapServer:
     """
     Integration Tests for the DLP Icap Server
     """
 
-    @pytest.mark.asyncio
-    async def test_dlp_icap_server(self, fs):
+    def test_dlp_icap_server(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List all icaps
             icaps = client.dlp.list_dlp_icap_servers()
             assert isinstance(icaps, list), "Expected a list of icaps"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_idm_profile.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_idm_profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TestDLPIDMProfile:
     """
     Integration Tests for the DLP IDM Profile
     """
 
-    @pytest.mark.asyncio
-    async def test_dlp_idm_profile(self, fs):
+    def test_dlp_idm_profile(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List all idm profiles
             profiles = client.dlp.list_dlp_idm_profiles()
             assert isinstance(profiles, list), "Expected a list of idm profiles"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_incident_receiver.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_incident_receiver.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestDLPIncidentReceiver:
     """
     Integration Tests for the DLP Incident Receiver
     """
 
-    @pytest.mark.asyncio
-    async def test_dlp_incident_receiver(self, fs):
+    def test_dlp_incident_receiver(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List all receivers
             receivers = client.dlp.list_dlp_incident_receiver()
             assert isinstance(receivers, list), "Expected a list of receivers"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_dlp_web_rule.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_web_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestDLPWebRule:
     """
     Integration Tests for the ZIA DLP Web Rule
     """
 
-    @pytest.mark.asyncio
-    async def test_dlp_web_rule(self, fs):
+    def test_dlp_web_rule(self, fs):
         client = MockZIAClient(fs)
         errors = []
         rule_id = None
 
         try:
             try:
                 # Create a DLP Web Rule
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_isolation_profile.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_isolation_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TestIsolationProfile:
     """
     Integration Tests for the Isolation Profile
     """
 
-    @pytest.mark.asyncio
-    async def test_isolation_profile(self, fs):
+    def test_isolation_profile(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List all profiles
             profiles = client.isolation_profile.list_isolation_profiles()
             assert isinstance(profiles, list), "Expected a list of profiles"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_group.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TestLocationGroup:
     """
     Integration Tests for the Location Group.
     """
 
-    @pytest.mark.asyncio
-    async def test_location_group(self, fs):
+    def test_location_group(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         group_id = None
 
         try:
             # List all groups
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_location_management.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestLocationManagement:
     """
     Integration Tests for the ZIA Location Management
     """
 
-    @pytest.mark.asyncio
-    async def test_location_management_vpn_ufqdn_type(self, fs):
+    def test_location_management_vpn_ufqdn_type(self, fs):
         client = MockZIAClient(fs)
         errors = []
         vpn_id = None
         location_id = None
 
         try:
             # Create VPN Credential IP Type
@@ -129,16 +128,15 @@
             errors.extend(cleanup_errors)
 
         # Assert that no errors occurred during the test
         assert (
             len(errors) == 0
         ), f"Errors occurred during the location management lifecycle test: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_sub_location(self, fs):
+    def test_sub_location(self, fs):
         client = MockZIAClient(fs)
         errors = []
         parent_location_id = None
         sub_location_id = None
 
         try:
             # Create VPN Credential IP Type
@@ -269,31 +267,29 @@
             errors.extend(cleanup_errors)
 
             # Assert that no errors occurred during the test
             assert (
                 len(errors) == 0
             ), f"Errors occurred during the sublocation management lifecycle test: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_list_cities_by_name(self, fs):
+    def test_list_cities_by_name(self, fs):
         client = MockZIAClient(fs)
         errors = []
 
         try:
             cities_list = client.locations.list_cities_by_name(prefix="San Jose")
             assert isinstance(cities_list, list), "Expected cities list not received"
         except Exception as exc:
             errors.append(f"Listing cities by name failed: {exc}")
 
         assert (
             len(errors) == 0
         ), f"Errors occurred during test_list_cities_by_name: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_get_geo_by_ip(self, fs):
+    def test_get_geo_by_ip(self, fs):
         client = MockZIAClient(fs)
         errors = []
 
         try:
             # Attempt to retrieve geographical data by IP
             geo_data = client.locations.get_geo_by_ip(ip="8.8.8.8")
             assert geo_data is not None, "Expected geographical data not received"
@@ -309,16 +305,15 @@
             ), "Country name information is missing in geographical data"
 
         except Exception as exc:
             errors.append(f"Retrieving geo data by IP failed: {exc}")
 
         assert len(errors) == 0, f"Errors occurred during test_get_geo_by_ip: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_list_region_geo_coordinates(self, fs):
+    def test_list_region_geo_coordinates(self, fs):
         client = MockZIAClient(fs)
         errors = []
 
         try:
             region_data = client.locations.list_region_geo_coordinates(
                 latitude=37.3860517, longitude=-122.0838511
             )
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_rule_labels.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_rule_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestRuleLabels:
     """
     Integration Tests for the Rule Label
     """
 
-    @pytest.mark.asyncio
-    async def test_rule_labels(self, fs):
+    def test_rule_labels(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         label_name = "tests-" + generate_random_string()
         label_description = "tests-" + generate_random_string()
         label_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_sandbox.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_sandbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,35 +42,32 @@
 
 
 class TestSandbox:
     """
     Integration Tests for the Sandbox Operations.
     """
 
-    @pytest.mark.asyncio
-    async def test_sandbox_get_quota(self, fs):
+    def test_sandbox_get_quota(self, fs):
         client = MockZIAClient(fs)
         try:
             quota = client.sandbox.get_quota()
             assert quota.allowed > 0, "Sandbox quota retrieval failed."
         except Exception as exc:
             pytest.fail(f"Sandbox quota retrieval failed: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_sandbox_get_report_summary(self, fs):
+    def test_sandbox_get_report_summary(self, fs):
         client = MockZIAClient(fs)
         test_md5_hash = "F69CA01D65E6C8F9E3540029E5F6AB92"
         try:
             report = client.sandbox.get_report(test_md5_hash)
             assert report.summary, "Sandbox report retrieval failed."
         except Exception as exc:
             pytest.fail(f"Sandbox report retrieval failed: {exc}")
 
-    # @pytest.mark.asyncio
-    # async def test_sandbox_submit_files(fs):
+    #def test_sandbox_submit_files(fs):
     #     client = MockZIAClient(fs)
     #     errors = []
 
     #     for file_name in FILE_NAMES:
     #         file_url = BASE_URL + file_name
     #         local_file_path = (
     #             file_name  # You may choose to download/locate files differently
@@ -100,16 +97,15 @@
     #         # Clean up by removing the downloaded file
     #         if os.path.exists(local_file_path):
     #             os.remove(local_file_path)
 
     # # Assert no errors occurred during the test
     # assert not errors, f"Errors occurred during sandbox file submission: {errors}"
 
-    # @pytest.mark.asyncio
-    # async def test_submit_file_for_inspection(self, fs):
+    #def test_submit_file_for_inspection(self, fs):
     #     client = MockZIAClient(fs)
     #     errors = []
 
     #     for file_name in FILE_NAMES:
     #         file_url = BASE_URL + file_name
     #         local_file_path = (
     #             file_name  # You may choose to download/locate files differently
@@ -139,25 +135,23 @@
     #             # Clean up by removing the downloaded file
     #             if os.path.exists(local_file_path):
     #                 os.remove(local_file_path)
 
     #     # Assert no errors occurred during the test
     #     assert not errors, f"Errors occurred during sandbox file submission: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_get_behavioral_analysis(self, fs):
+    def test_get_behavioral_analysis(self, fs):
         client = MockZIAClient(fs)
         try:
             behavioral_analysis = client.sandbox.get_behavioral_analysis()
             assert behavioral_analysis, "Retrieving behavioral analysis failed."
         except Exception as exc:
             pytest.fail(f"Retrieving behavioral analysis failed: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_add_hash_to_custom_list(self, fs):
+    def test_add_hash_to_custom_list(self, fs):
         client = MockZIAClient(fs)
         test_hashes = [
             "42914d6d213a20a2684064be5c80ffa9",
             "c0202cf6aeab8437c638533d14563d35",
         ]
         try:
             updated_list = client.sandbox.add_hash_to_custom_list(test_hashes)
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_security.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_security.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,96 +25,89 @@
 
 
 class TestSecurityWhitelistBlacklist:
     """
     Integration Tests for the Security Whitelist and Blacklist.
     """
 
-    @pytest.mark.asyncio
-    async def test_add_url_to_whitelist(self, fs):
+
+    def test_add_url_to_whitelist(self, fs):
         client = MockZIAClient(fs)
         url_to_add = "example.com"
         try:
             updated_whitelist = client.security.add_urls_to_whitelist([url_to_add])
             assert (
                 url_to_add in updated_whitelist
             ), f"{url_to_add} not added to whitelist."
         except Exception as exc:
             pytest.fail(f"Failed to add URL to whitelist: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_get_whitelist(self, fs):
+    def test_get_whitelist(self, fs):
         client = MockZIAClient(fs)
         try:
             whitelist = client.security.get_whitelist()
             assert isinstance(whitelist, list), "Failed to retrieve whitelist."
         except Exception as exc:
             pytest.fail(f"Whitelist retrieval failed: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_replace_url_from_whitelist(self, fs):
+    def test_replace_url_from_whitelist(self, fs):
         client = MockZIAClient(fs)
         url_to_replace = ["newsite.com"]
         try:
             updated_whitelist = client.security.replace_whitelist(url_to_replace)
             assert (
                 url_to_replace[0] in updated_whitelist
             ), "Whitelist replace operation failed."
         except Exception as exc:
             pytest.fail(f"Failed to replace whitelist: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_delete_urls_from_whitelist(self, fs):
+    def test_delete_urls_from_whitelist(self, fs):
         client = MockZIAClient(fs)
         url_to_delete = "example.com"
         try:
             updated_whitelist = client.security.delete_urls_from_whitelist(
                 [url_to_delete]
             )
             assert (
                 url_to_delete not in updated_whitelist
             ), f"{url_to_delete} was not deleted from whitelist."
         except Exception as exc:
             pytest.fail(f"Failed to delete URL from whitelist: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_add_urls_to_blacklist(self, fs):
+    def test_add_urls_to_blacklist(self, fs):
         client = MockZIAClient(fs)
         url_to_add = "badexample.com"
         try:
             updated_blacklist = client.security.add_urls_to_blacklist([url_to_add])
             assert (
                 url_to_add in updated_blacklist
             ), f"{url_to_add} not added to blacklist."
         except Exception as exc:
             pytest.fail(f"Failed to add URL to blacklist: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_get_blacklist(self, fs):
+    def test_get_blacklist(self, fs):
         client = MockZIAClient(fs)
         try:
             blacklist = client.security.get_blacklist()
             assert isinstance(blacklist, list), "Failed to retrieve blacklist."
         except Exception as exc:
             pytest.fail(f"Blacklist retrieval failed: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_replace_blacklist(self, fs):
+    def test_replace_blacklist(self, fs):
         client = MockZIAClient(fs)
         new_blacklist_urls = ["newbadexample.com"]
         try:
             updated_blacklist = client.security.replace_blacklist(new_blacklist_urls)
             assert (
                 new_blacklist_urls[0] in updated_blacklist
             ), "Blacklist replace operation failed."
         except Exception as exc:
             pytest.fail(f"Failed to replace blacklist: {exc}")
 
-    @pytest.mark.asyncio
-    async def test_erase_blacklist(self, fs):
+    def test_erase_blacklist(self, fs):
         client = MockZIAClient(fs)
         try:
             result = client.security.erase_blacklist()
             assert (
                 result == 204 or "successfully erased" in result.lower()
             ), "Failed to erase blacklist."
         except Exception as exc:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_gre_tunnel.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_gre_tunnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestTrafficGRETunnel:
     """
     Integration Tests for the ZIA Traffic GRE Tunnel.
     """
 
-    @pytest.mark.asyncio
-    async def test_traffic_gre_tunnel(self, fs):
+    def test_traffic_gre_tunnel(self, fs):
         client = MockZIAClient(fs)
         errors = []
         gre_tunnel_ids = []
         static_ip_id = None
         randomIP = generate_random_ip("104.239.237.0/24")
 
         # Create Static IP for GRE Tunnel
@@ -124,16 +123,15 @@
                     )
 
         # Assert no errors occurred during the test
         assert (
             len(errors) == 0
         ), f"Errors occurred during GRE Tunnel operations test: {'; '.join(errors)}"
 
-    @pytest.mark.asyncio
-    async def test_traffic_list_gre_ranges(self, fs):
+    def test_traffic_list_gre_ranges(self, fs):
         client = MockZIAClient(fs)
         errors = []
         randomIP = generate_random_ip("104.239.237.0/24")
         static_ip_id = None
 
         # Test Case 1: With static IP
         try:
@@ -186,16 +184,15 @@
         except Exception as exc:
             errors.append(f"Listing GRE ranges without static IP failed: {exc}")
 
         assert (
             len(errors) == 0
         ), f"Errors occurred during listing GRE ranges test: {'; '.join(errors)}"
 
-    @pytest.mark.asyncio
-    async def test_traffic_list_vips_recommended(self, fs):
+    def test_traffic_list_vips_recommended(self, fs):
         client = MockZIAClient(fs)
         errors = []
         randomIP = generate_random_ip("104.239.237.0/24")
         static_ip_id = None
 
         try:
             # Create Static IP for the test
@@ -236,16 +233,15 @@
                         f"Cleanup failed for Static IP ID {static_ip_id}: {cleanup_exc}"
                     )
 
         assert (
             len(errors) == 0
         ), f"Errors occurred during listing recommended VIPs test: {'; '.join(errors)}"
 
-    @pytest.mark.asyncio
-    async def test_traffic_list_vip_group_by_dc(self, fs):
+    def test_traffic_list_vip_group_by_dc(self, fs):
         client = MockZIAClient(fs)
         errors = []
         randomIP = generate_random_ip("104.239.237.0/24")
         static_ip_id = None
 
         try:
             # Create Static IP for the test
@@ -284,16 +280,15 @@
                         f"Cleanup failed for Static IP ID {static_ip_id}: {cleanup_exc}"
                     )
 
         assert (
             len(errors) == 0
         ), f"Errors occurred during listing VIP group by DC test: {'; '.join(errors)}"
 
-    @pytest.mark.asyncio
-    async def test_traffic_get_closest_diverse_vip_ids(self, fs):
+    def test_traffic_get_closest_diverse_vip_ids(self, fs):
         client = MockZIAClient(fs)
         errors = []
         randomIP = generate_random_ip("104.239.237.0/24")
         static_ip_id = None
 
         try:
             # Create Static IP for the test
@@ -334,16 +329,15 @@
                         f"Cleanup failed for Static IP ID {static_ip_id}: {cleanup_exc}"
                     )
 
         assert (
             len(errors) == 0
         ), f"Errors occurred during getting closest diverse VIP IDs test: {'; '.join(errors)}"
 
-    @pytest.mark.asyncio
-    async def test_traffic_list_vips(self, fs):
+    def test_traffic_list_vips(self, fs):
         client = MockZIAClient(fs)
         errors = []
 
         try:
             # Example test with max_items=10
             vips = client.traffic.list_vips(max_items=10)
             assert (
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_static_ip.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_static_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestTrafficStaticIP:
     """
     Integration Tests for the traffic static ip
     """
 
-    @pytest.mark.asyncio
-    async def test_traffic_static_ip(self, fs):
+    def test_traffic_static_ip(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         randomIP = generate_random_ip("104.239.237.0/24")
         comment = "tests-" + generate_random_string()
         static_ip_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_traffic_vpn_credential.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_vpn_credential.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestTrafficVPNCredential:
     """
     Integration Tests for the ZIA Traffic VPN Credential.
     """
 
-    @pytest.mark.asyncio
-    async def test_traffic_vpn_credential(self, fs):
+    def test_traffic_vpn_credential(self, fs):
         client = MockZIAClient(fs)
         errors = []
         created_vpn_ids = []
         static_ip_id = None
         randomIP = generate_random_ip("104.239.237.0/24")
 
         # Create Static IP for VPN Credential of type IP
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_categories.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_categories.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 
 class TestURLCategories:
     """
     Integration Tests for the URL Categories
     """
 
-    @pytest.mark.asyncio
-    async def test_url_categories(self, fs):
+    def test_url_categories(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         category_name = "tests-" + generate_random_string()
         category_description = "tests-" + generate_random_string()
         category_id = None
 
@@ -122,16 +121,15 @@
                     errors.append(f"Cleanup failed: {exc}")
 
         # Assert that no errors occurred during the test
         assert (
             len(errors) == 0
         ), f"Errors occurred during the URL category lifecycle test: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_lookup(self, fs):
+    def test_lookup(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         # Define a complete list of URLs to lookup
         urls = [
             "google.com",
             "youtube.com",
@@ -244,16 +242,15 @@
         except Exception as exc:
             errors.append(f"URL lookup failed: {exc}")
 
         assert (
             len(errors) == 0
         ), f"Errors occurred during URL lookup test: {'; '.join(errors)}"
 
-    @pytest.mark.asyncio
-    async def test_get_quota(self, fs):
+    def test_get_quota(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             quota_info = client.url_categories.get_quota()
             assert isinstance(quota_info, Box), "Quota information should be a Box."
             # Further assertions can be made here based on expected quota values or properties
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_url_filtering_rule.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_filtering_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestURLFilteringRule:
     """
     Integration Tests for the ZIA URL Filtering Rule
     """
 
-    @pytest.mark.asyncio
-    async def test_url_filtering_rule(self, fs):
+    def test_url_filtering_rule(self, fs):
         client = MockZIAClient(fs)
         errors = []
         rule_id = None
 
         try:
             # Create a url filtering Rule
             rule_name = "tests-" + generate_random_string()
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zia/test_users.py` & `zscaler-sdk-python-0.1.1/tests/integration/zia/test_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestUsers:
     """
     Integration Tests for the User Management
     """
 
-    # @pytest.mark.asyncio
-    # async def test_users(self, fs):
+    #def test_users(self, fs):
     #     client = MockZIAClient(fs)
     #     errors = []  # Initialize an empty list to collect errors
     #     user_id = None
 
     #     try:
     #         # Retrieve the first department's ID
     #         departments = client.users.list_departments(search='A000')
@@ -137,16 +136,15 @@
     #                 assert activation_response in ["ACTIVE", "PENDING"], "Activation failed or is pending after deletion"
     #             except Exception as exc:
     #                 errors.append(f"Deleting User Account or reactivation failed: {exc}")
 
     #         if errors:
     #             raise AssertionError("Errors occurred during the user management test: " + "; ".join(errors))
 
-    @pytest.mark.asyncio
-    async def test_user_departments(self, fs):
+    def test_user_departments(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List departments with optional parameters
             depts = client.users.list_departments(page_size=2, max_pages=1)
             assert (
@@ -177,16 +175,15 @@
 
         except Exception as exc:
             errors.append(f"Test failed: {exc}")
 
         # Assert that no errors occurred during the test
         assert len(errors) == 0, f"Errors occurred during departments test: {errors}"
 
-    @pytest.mark.asyncio
-    async def test_user_groups(self, fs):
+    def test_user_groups(self, fs):
         client = MockZIAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List groups with optional parameters
             groups = client.users.list_groups(
                 page_size=2, max_pages=1, sort_order="ASC"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/conftest.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_forwarding_rules.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_forwarding_rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestAccessPolicyForwardingRule:
     """
     Integration Tests for the Access Policy Forwarding Rules
     """
 
-    @pytest.mark.asyncio
-    async def test_access_policy_forwarding_rules(self, fs):
+    def test_access_policy_forwarding_rules(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         rule_id = None
 
         try:
             # Create a Forwarding Policy Rule
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_rules.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestAccessPolicyRule:
     """
     Integration Tests for the Access Policy Rules
     """
 
-    @pytest.mark.asyncio
-    async def test_access_policy_rules(self, fs):
+    def test_access_policy_rules(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         connector_group_id = None
         rule_id = None
 
         try:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_access_policy_timeout_rules.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_timeout_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestAccessPolicyTimeoutRule:
     """
     Integration Tests for the Access Policy Timeout Rules
     """
 
-    @pytest.mark.asyncio
-    async def test_access_policy_timeout_policy_rules(self, fs):
+    def test_access_policy_timeout_policy_rules(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         rule_id = None
 
         try:
             # Create a Timeout Policy Rule
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_app_connector_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_app_connector_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 
 class TestAppConnectorGroup:
     """
     Integration Tests for the App Connector Group
     """
 
-    @pytest.mark.asyncio
-    async def test_app_connector_group(self, fs):
+    def test_app_connector_group(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         group_name = "tests-" + generate_random_string()
         group_description = "tests-" + generate_random_string()
         group_enabled = True
         latitude = "37.3382082"
@@ -99,22 +98,14 @@
         except Exception as exc:
             errors.append(f"Failed to search for app connector group by name: {exc}")
 
         finally:
             # Cleanup: Delete the app connector group if it was created
             if group_id:
                 try:
-                    delete_response_code = client.connectors.delete_connector_group(
-                        group_id
-                    )
-                    assert (
-                        str(delete_response_code) == "204"
-                    ), f"Failed to delete app connector group with ID {group_id}"
+                    delete_response_code = client.connectors.delete_connector_group(group_id)
+                    assert str(delete_response_code) == "204", f"Failed to delete app connector group with ID {group_id}"
                 except Exception as cleanup_exc:
-                    errors.append(
-                        f"Cleanup failed for app connector group ID {group_id}: {cleanup_exc}"
-                    )
+                    errors.append(f"Cleanup failed for app connector group ID {group_id}: {cleanup_exc}")
 
         # Assert that no errors occurred during the test
-        assert (
-            len(errors) == 0
-        ), f"Errors occurred during the app connector group lifecycle test: {errors}"
+        assert len(errors) == 0, f"Errors occurred during the app connector group lifecycle test: {errors}"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_segment.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 
 
 class TestApplicationSegment:
     """
     Integration Tests for the Applications Segment
     """
 
-    @pytest.mark.asyncio
-    async def test_application_segment(self, fs):
+    def test_application_segment(self, fs):
         client = MockZPAClient(fs)
         errors = []
 
         # Initialize IDs for cleanup
         app_connector_group_id = None
         segment_group_id = None
         server_group_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_application_servers.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 
 
 class TestSegmentGroup:
     """
     Integration Tests for the Application Server
     """
 
-    @pytest.mark.asyncio
-    async def test_application_server(self, fs):
+    def test_application_server(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         server_name = "tests-" + generate_random_string()
         server_description = "tests-" + generate_random_string()
         server_address = "192.168.200.1"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_ba_certificates.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_ba_certificates.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestBaCertificate:
     """
     Integration Tests for the certificates.
     """
 
-    @pytest.mark.asyncio
-    async def test_ba_certificate(self, fs):
+    def test_ba_certificate(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
         certificate_id = None
 
         # List all certificates
         try:
             certs = client.certificates.list_issued_certificates()
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_enrolment_certificates.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_enrolment_certificates.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestEnrolmentCertificate:
     """
     Integration Tests for the enrolment certificates.
     """
 
-    @pytest.mark.asyncio
-    async def test_enrolment_certificate(self, fs):
+    def test_enrolment_certificate(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         # Attempt to list all enrolment certificates
         try:
             certs = client.certificates.list_enrolment()
             assert isinstance(certs, list), "Expected a list of enrolment certificates"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_idp.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_idp.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TestIdP:
     """
     Integration Tests for the identity provider.
     """
 
-    @pytest.mark.asyncio
-    async def test_idp(self, fs):
+    def test_idp(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
         idp_id = None
 
         # List all identity providers
         try:
             idps = client.idp.list_idps()
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_isolation_profile.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_isolation_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 
 class TestIsolationProfile:
     """
     Integration Tests for the Isolation Profile.
     """
 
-    @pytest.mark.asyncio
-    async def test_isolation_profile(self, fs):
+    def test_isolation_profile(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         # Attempt to list all isolation profiles
         try:
             isolation_profiles = client.isolation_profile.list_profiles()
             assert isinstance(
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_machine_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_machine_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestMachineGroups:
     """
     Integration Tests for the Machine Groups.
     """
 
-    @pytest.mark.asyncio
-    async def test_machine_groups(self, fs):
+    def test_machine_groups(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         # Attempt to list all machine groups
         try:
             machine_groups = client.machine_groups.list_groups()
             assert isinstance(machine_groups, list), "Expected a list of machine groups"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_posture_profiles.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_posture_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestPostureProfile:
     """
     Integration Tests for the Posture Profile.
     """
 
-    @pytest.mark.asyncio
-    async def test_posture_profile(self, fs):
+    def test_posture_profile(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         # Attempt to list all posture profiles
         try:
             posture_profile = client.posture_profiles.list_profiles()
             assert isinstance(
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_approval.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_approval.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestPRAApproval:
     """
     Integration Tests for the PRA Approval.
     """
 
-    @pytest.mark.asyncio
-    async def test_pra_approval(self, fs):
+    def test_pra_approval(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         approval_id = None
         app_segment_id = None
         segment_group_id = None
         app_connector_group_id = None
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_credential.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestPRACredential:
     """
     Integration Tests for the PRA Credential.
     """
 
-    @pytest.mark.asyncio
-    async def test_pra_credential(self, fs):
+    def test_pra_credential(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
         credential_id = None
 
         credential_description = "tests-" + generate_random_string()
         # Generate a random password
         password = generate_random_password()
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_pra_portal.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestPRAPortal:
     """
     Integration Tests for the PRA Portal.
     """
 
-    @pytest.mark.asyncio
-    async def test_pra_portal(self, fs):
+    def test_pra_portal(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
         portal_id = None
         certificate_id = None
 
         SDK_PREFIX = "zscaler_python_sdk"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_app_connector_group.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_app_connector_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 
 class TestAppConnectorGroupProvisioningKey:
     """
     Integration Tests for the Provisioning Key API.
     """
 
-    @pytest.mark.asyncio
-    async def test_provisioning_key_operations(self, fs):
+    def test_provisioning_key_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         connector_group_id = None
         connector_key_id = None
 
         try:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_provisioning_key_service_edge_group.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_service_edge_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 
 class TestServiceEdgeGroupProvisioningKey:
     """
     Integration Tests for the Provisioning Key API
     """
 
-    @pytest.mark.asyncio
-    async def test_provisioning_key_operations(self, fs):
+    def test_provisioning_key_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         svc_edge_group_id = None
         svc_edge_group_key_id = None
 
         try:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_saml_attributes.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_saml_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestSamlAttributes:
     """
     Integration Tests for the SAML attributes
     """
 
-    @pytest.mark.asyncio
-    async def test_saml_attributes_operations(self, fs):
+    def test_saml_attributes_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # Test listing all SAML attributes
             resp = client.saml_attributes.list_attributes()
             assert isinstance(
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_attributes.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestScimAttributes:
     """
     Integration Tests for the SCIM attributes
     """
 
-    @pytest.mark.asyncio
-    async def test_scim_attributes_operations(self, fs):
+    def test_scim_attributes_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # Test listing SCIM attributes by IDP
             idps = client.idp.list_idps()
             user_idp = next(
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_scim_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestScimGroups:
     """
     Integration Tests for the SCIM Groups
     """
 
-    @pytest.mark.asyncio
-    async def test_scim_groups_operations(self, fs):
+    def test_scim_groups_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # Test listing SCIM groups
             idps = client.idp.list_idps()
             user_idp = next(
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_segment_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_segment_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestSegmentGroup:
     """
     Integration Tests for the Segment Group
     """
 
-    @pytest.mark.asyncio
-    async def test_segment_group(self, fs):
+    def test_segment_group(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         segment_group_name = "tests-" + generate_random_string()
         segment_group_description = "tests-" + generate_random_string()
 
         try:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_server_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_server_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestServerGroup:
     """
     Integration Tests for the Server Group
     """
 
-    @pytest.mark.asyncio
-    async def test_server_group(self, fs):
+    def test_server_group(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         connector_group_id = None
         server_group_id = None
 
         try:
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_service_edge_groups.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_service_edge_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 class TestServiceEdgeGroup:
     """
     Integration Tests for the Service Edge Group
     """
 
-    @pytest.mark.asyncio
-    async def test_service_edge_group(self, fs):
+    def test_service_edge_group(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         group_name = "tests-" + generate_random_string()
         group_description = "tests-" + generate_random_string()
         group_enabled = True
         latitude = "37.3382082"
```

### Comparing `zscaler-sdk-python-0.1.0/tests/integration/zpa/test_trusted_networks.py` & `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_trusted_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 
 class TestTrustedNetworks:
     """
     Integration Tests for the Trusted Networks
     """
 
-    @pytest.mark.asyncio
-    async def test_trusted_networks(self, fs):
+    def test_trusted_networks(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
             # List all trusted networks
             try:
                 trusted_networks = client.trusted_networks.list_networks()
```

### Comparing `zscaler-sdk-python-0.1.0/tests/test_utils.py` & `zscaler-sdk-python-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/__init__.py` & `zscaler-sdk-python-0.1.1/zscaler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler-sdk-python-0.1.0/zscaler/cache/cache.py` & `zscaler-sdk-python-0.1.1/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/cache/no_op_cache.py` & `zscaler-sdk-python-0.1.1/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/cache/zscaler_cache.py` & `zscaler-sdk-python-0.1.1/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/constants.py` & `zscaler-sdk-python-0.1.1/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/errors/http_error.py` & `zscaler-sdk-python-0.1.1/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/errors/zscaler_api_error.py` & `zscaler-sdk-python-0.1.1/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/exceptions/exceptions.py` & `zscaler-sdk-python-0.1.1/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/logger.py` & `zscaler-sdk-python-0.1.1/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/ratelimiter/ratelimiter.py` & `zscaler-sdk-python-0.1.1/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/user_agent.py` & `zscaler-sdk-python-0.1.1/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/utils.py` & `zscaler-sdk-python-0.1.1/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/__init__.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/activate.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/admin_and_role_management.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/apptotal.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/audit_logs.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/authentication_settings.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/client.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/cloud_apps.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/device_management.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/dlp.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/errors.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/firewall.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/forwarding_control.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/isolation_profile.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/labels.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/locations.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/sandbox.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/security.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/ssl_inspection.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/traffic.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/url_categories.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/url_filtering.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/users.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/web_dlp.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/workload_groups.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zia/zpa_gateway.py` & `zscaler-sdk-python-0.1.1/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/README.md` & `zscaler-sdk-python-0.1.1/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/__init__.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_inspection.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/app_segments_pra.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/certificates.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/client.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/cloud_connector_groups.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/connectors.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/emergency_access.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/errors.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/idp.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/inspection.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/isolation_profile.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/lss.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/machine_groups.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/policies.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/posture_profiles.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/privileged_remote_access.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/provisioning.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/saml_attributes.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/scim_attributes.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/scim_groups.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/segment_groups.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/server_groups.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/servers.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/service_edges.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler/zpa/trusted_networks.py` & `zscaler-sdk-python-0.1.1/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.0/zscaler_sdk_python.egg-info/SOURCES.txt` & `zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 CHANGELOG.md
 LICENSE.md
-LONG_DESCRIPTION.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docsrc/Makefile
```

