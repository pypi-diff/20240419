# Comparing `tmp/sagemaker-jupyterlab-extension-0.3.1.tar.gz` & `tmp/sagemaker_jupyterlab_extension-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-jupyterlab-extension-0.3.1.tar", last modified: Thu Apr  4 00:01:35 2024, max compression
+gzip compressed data, was "sagemaker_jupyterlab_extension-0.3.2.tar", last modified: Thu Apr 18 20:08:37 2024, max compression
```

## Comparing `sagemaker-jupyterlab-extension-0.3.1.tar` & `sagemaker_jupyterlab_extension-0.3.2.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/LICENSE
--rw-r--r--   0 p4admin  (12569) amazon     (100)      612 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1322 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8139 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/THIRD-PARTY-LICENSES
--rw-r--r--   0 p4admin  (12569) amazon     (100)      221 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/install.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.652631 sagemaker-jupyterlab-extension-0.3.1/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.656631 sagemaker-jupyterlab-extension-0.3.1/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      105 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3949 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.656631 sagemaker-jupyterlab-extension-0.3.1/public_dist/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  2341809 2024-04-03 23:59:53.000000 sagemaker-jupyterlab-extension-0.3.1/public_dist/sagemaker_jupyterlab_extension-0.3.1-py3-none-any.whl
--rw-r--r--   0 p4admin  (12569) amazon     (100)      156 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/pyproject.toml
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.660631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1133 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/_version.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    11587 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/handlers.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.660631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4091 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3280 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    92715 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1874 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)  4112866 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8620 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2309 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    28123 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   205663 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    36761 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      249 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4283 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12933 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   292756 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       50 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)   103503 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      487 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4474 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   237708 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   266482 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    58332 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7725 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   139405 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12105 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      185 2024-04-04 00:00:40.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    91011 2024-04-04 00:01:24.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       60 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/helper.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1647 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5332 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5041 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7701 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_request_logger.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       64 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      555 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2552 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/git_clone_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      507 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/metric_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7250 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/request_logger.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5749 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-03 23:58:45.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       31 2024-04-04 00:01:35.000000 sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2953 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.672631 sagemaker-jupyterlab-extension-0.3.1/src/components/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3246 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/GitCloneComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6489 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/ResourceUsageComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1019 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/SpaceMenu.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1797 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/AutoComplete.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      799 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/CheckboxComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1917 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/GitCloneComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      881 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/InputField.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1068 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/LinearProgressWithLabel.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3156 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/ResourceUsageComponent.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2389 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/SpaceMenu.spec.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/components/common/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1394 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/AutoComplete.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      988 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/CheckboxComponent.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/InputField.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      980 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/common/LinearProgressWithLabel.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      575 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/InputFieldStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      469 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/SpaceMenuStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      475 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/components/styles/autoCompleteStyles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.676631 sagemaker-jupyterlab-extension-0.3.1/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1201 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/errorMessages.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/gitCloneConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3263 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/il18Strings.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      174 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      632 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/resourceUsageConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1480 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/sessionManagementConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/constants/spaceMenuConstants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      425 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6451 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/GitClonePlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      767 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/HideShutDownPlugin.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      785 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       45 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4320 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/utils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/ResourceUsagePlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6247 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/SessionManagementPlugin.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1167 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/SpaceMenuPlugin.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3662 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/GitClonePlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      787 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/HideShutDownPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      741 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/ResourceUsagePlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4826 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SessionManagementPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1365 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SpaceMenuPlugin.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      226 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/plugins/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/service/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2425 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/index.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1193 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/mock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      526 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/constants.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/service/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/style/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/style/common.css
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/style/index.css
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.680631 sagemaker-jupyterlab-extension-0.3.1/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      531 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/ReactWidgetWrapper.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8036 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/gitCloneUtils.spec.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    16809 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/sessionManagerUtils.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5331 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/gitCloneUtils.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      547 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/logger.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    10835 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/utils/sessionManagerUtils.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1971 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/GitCloneWidget.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2161 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/ResourceUsageWidget.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      809 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/SpaceMenuWidget.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1597 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/GitCloneWidget.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1638 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/ResourceUsageWidget.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/SpaceMenuWidget.spec.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-04 00:01:35.684630 sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/gitCloneStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2092 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/resourceUsageStyle.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9490 2024-04-03 23:50:02.000000 sagemaker-jupyterlab-extension-0.3.1/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4755 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/LICENSE
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      612 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1322 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8139 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/THIRD-PARTY-LICENSES
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      221 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/install.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.280175 sagemaker_jupyterlab_extension-0.3.2/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.284175 sagemaker_jupyterlab_extension-0.3.2/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      105 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3949 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.284175 sagemaker_jupyterlab_extension-0.3.2/public_dist/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  2341836 2024-04-18 20:06:59.000000 sagemaker_jupyterlab_extension-0.3.2/public_dist/sagemaker_jupyterlab_extension-0.3.2-py3-none-any.whl
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      156 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/pyproject.toml
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.288175 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1133 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      683 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/_version.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    11587 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/handlers.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.292175 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4091 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.300174 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3280 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    92715 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1874 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  4112866 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8620 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2309 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    28122 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   205663 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    36761 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      249 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4283 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12933 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   292756 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       50 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   103503 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      487 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4474 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   237708 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   266482 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    58332 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7725 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   139404 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12103 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      185 2024-04-18 20:07:46.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    91011 2024-04-18 20:08:26.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.304174 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       60 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/helper.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1647 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5332 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5041 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7701 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_request_logger.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.304174 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       64 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      555 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2552 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/git_clone_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      507 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/metric_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7250 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/request_logger.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2274 2024-04-18 20:08:37.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5749 2024-04-18 20:08:37.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-18 20:08:37.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-04-18 20:05:53.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-18 20:08:37.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       31 2024-04-18 20:08:37.000000 sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2953 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.304174 sagemaker_jupyterlab_extension-0.3.2/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.304174 sagemaker_jupyterlab_extension-0.3.2/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.304174 sagemaker_jupyterlab_extension-0.3.2/src/components/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3246 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/GitCloneComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6489 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/ResourceUsageComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1019 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/SpaceMenu.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.304174 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1797 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/AutoComplete.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      799 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/CheckboxComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1917 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/GitCloneComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      881 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/InputField.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1068 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/LinearProgressWithLabel.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3156 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/ResourceUsageComponent.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2389 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/SpaceMenu.spec.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.308174 sagemaker_jupyterlab_extension-0.3.2/src/components/common/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1394 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/common/AutoComplete.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      988 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/common/CheckboxComponent.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/common/InputField.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      980 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/common/LinearProgressWithLabel.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.308174 sagemaker_jupyterlab_extension-0.3.2/src/components/styles/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      575 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/styles/InputFieldStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      469 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/styles/SpaceMenuStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      475 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/components/styles/autoCompleteStyles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.308174 sagemaker_jupyterlab_extension-0.3.2/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1201 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      154 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/errorMessages.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      191 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/gitCloneConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3263 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/il18Strings.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      174 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      632 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/resourceUsageConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1480 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/sessionManagementConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/constants/spaceMenuConstants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      425 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.308174 sagemaker_jupyterlab_extension-0.3.2/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6451 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/GitClonePlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      767 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/HideShutDownPlugin.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/plugins/PerformancePlugin/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      785 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       45 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/PerformancePlugin/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4320 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/PerformancePlugin/utils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      814 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/ResourceUsagePlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6247 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/SessionManagementPlugin.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1167 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/SpaceMenuPlugin.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3662 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/GitClonePlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      787 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/HideShutDownPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      741 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/ResourceUsagePlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4826 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/SessionManagementPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1365 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/SpaceMenuPlugin.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      226 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/plugins/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/service/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/service/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2425 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/service/__tests__/index.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1193 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/service/__tests__/mock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      526 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/service/constants.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1142 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/service/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/style/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/style/common.css
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/style/index.css
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      531 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/utils/ReactWidgetWrapper.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.312174 sagemaker_jupyterlab_extension-0.3.2/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8036 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/utils/__tests__/gitCloneUtils.spec.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    16809 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/utils/__tests__/sessionManagerUtils.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5331 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/utils/gitCloneUtils.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      547 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/utils/logger.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    10835 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/utils/sessionManagerUtils.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1971 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/GitCloneWidget.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2161 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/ResourceUsageWidget.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      809 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/SpaceMenuWidget.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/src/widgets/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1597 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/__tests__/GitCloneWidget.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1638 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/__tests__/ResourceUsageWidget.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      405 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/__tests__/SpaceMenuWidget.spec.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-04-18 20:08:37.316174 sagemaker_jupyterlab_extension-0.3.2/src/widgets/styles/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      350 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/styles/gitCloneStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2092 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/src/widgets/styles/resourceUsageStyle.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9490 2024-04-18 19:56:48.000000 sagemaker_jupyterlab_extension-0.3.2/tsconfig.json
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/LICENSE` & `sagemaker_jupyterlab_extension-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/MANIFEST.in` & `sagemaker_jupyterlab_extension-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/PKG-INFO` & `sagemaker_jupyterlab_extension-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.3.1
+Version: 0.3.2
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/README.md` & `sagemaker_jupyterlab_extension-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/THIRD-PARTY-LICENSES` & `sagemaker_jupyterlab_extension-0.3.2/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/package.json` & `sagemaker_jupyterlab_extension-0.3.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.3.2'"}*

```diff
@@ -100,9 +100,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/public_dist/sagemaker_jupyterlab_extension-0.3.1-py3-none-any.whl` & `sagemaker_jupyterlab_extension-0.3.2/public_dist/sagemaker_jupyterlab_extension-0.3.2-py3-none-any.whl`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,78 +1,78 @@
-Zip file size: 2341809 bytes, number of entries: 76
+Zip file size: 2341836 bytes, number of entries: 76
 -rw-r--r--  2.0 unx     1133 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/__init__.py
 -rw-r--r--  2.0 unx      683 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/_version.py
 -rw-r--r--  2.0 unx    11587 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/handlers.py
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/package.json
 -rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
 -rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
 -rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 -rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 -rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 -rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
--rw-r--r--  2.0 unx    28123 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
+-rw-r--r--  2.0 unx    28122 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js
 -rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 -rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 -rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
 -rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
 -rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
 -rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 -rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 -rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 -rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
 -rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
--rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
+-rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js
 -rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 -rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
--rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
--rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
+-rw-r--r--  2.0 unx   139404 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js.LICENSE.txt
+-rw-r--r--  2.0 unx    12103 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js
 -rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/style.js
 -rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/__init__.py
 -rw-r--r--  2.0 unx      405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/helper.py
 -rw-r--r--  2.0 unx     1647 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_error_util.py
 -rw-r--r--  2.0 unx     5332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
 -rw-r--r--  2.0 unx     5041 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_handlers.py
 -rw-r--r--  2.0 unx     7701 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/tests/test_request_logger.py
 -rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/__init__.py
 -rw-r--r--  2.0 unx      555 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/error_util.py
 -rw-r--r--  2.0 unx     2552 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/git_clone_util.py
 -rw-r--r--  2.0 unx      507 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/metric_util.py
 -rw-r--r--  2.0 unx     7250 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension/utils/request_logger.py
--rw-r--r--  2.0 unx     8139 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES
--rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
--rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
--rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
--rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
--rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
--rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
--rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
--rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
--rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
--rw-r--r--  2.0 unx    28123 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js
--rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
--rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
--rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
--rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
--rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
--rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
--rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
--rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
--rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
--rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
--rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js
--rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
--rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
--rw-r--r--  2.0 unx   139405 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
--rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
--rw-r--r--  2.0 unx    12105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js
--rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
--rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
--rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    11677 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD
-76 files, 11528062 bytes uncompressed, 2321251 bytes compressed:  79.9%
+-rw-r--r--  2.0 unx     8139 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/THIRD-PARTY-LICENSES
+-rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+-rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
+-rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
+-rw-r--r--  2.0 unx     3280 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
+-rw-r--r--  2.0 unx    92715 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
+-rw-r--r--  2.0 unx     1874 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
+-rw-r--r--  2.0 unx  4112866 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
+-rw-r--r--  2.0 unx     8620 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
+-rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
+-rw-r--r--  2.0 unx    28122 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.f4872310b34e6c6b2839.js
+-rw-r--r--  2.0 unx   205663 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
+-rw-r--r--  2.0 unx    36761 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
+-rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
+-rw-r--r--  2.0 unx     4283 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
+-rw-r--r--  2.0 unx    12933 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
+-rw-r--r--  2.0 unx   292756 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+-rw-r--r--  2.0 unx   103503 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
+-rw-r--r--  2.0 unx      487 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+-rw-r--r--  2.0 unx     4474 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
+-rw-r--r--  2.0 unx   237708 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
+-rw-r--r--  2.0 unx   266482 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.87642002230f9f1eed39.js
+-rw-r--r--  2.0 unx    58332 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
+-rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
+-rw-r--r--  2.0 unx   139404 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js.LICENSE.txt
+-rw-r--r--  2.0 unx    12103 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.473afc439684735f2efc.js
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
+-rw-r--r--  2.0 unx    91011 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
+-rw-r--r--  2.0 unx     4755 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2281 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11677 b- defN 80-Jan-01 00:00 sagemaker_jupyterlab_extension-0.3.2.dist-info/RECORD
+76 files, 11528054 bytes uncompressed, 2321278 bytes compressed:  79.9%
```

#### zipnote «TEMP»/diffoscope__qss16bu_/tmpwra5zf0o_.zip

```diff
@@ -24,15 +24,15 @@
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 Comment: 
@@ -60,30 +60,30 @@
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
+Filename: sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/style.js
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 Comment: 
@@ -117,113 +117,113 @@
 
 Filename: sagemaker_jupyterlab_extension/utils/metric_util.py
 Comment: 
 
 Filename: sagemaker_jupyterlab_extension/utils/request_logger.py
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/THIRD-PARTY-LICENSES
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.f4872310b34e6c6b2839.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.87642002230f9f1eed39.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js.LICENSE.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.473afc439684735f2efc.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
+Filename: sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE
+Filename: sagemaker_jupyterlab_extension-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA
+Filename: sagemaker_jupyterlab_extension-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/WHEEL
+Filename: sagemaker_jupyterlab_extension-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/top_level.txt
+Filename: sagemaker_jupyterlab_extension-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD
+Filename: sagemaker_jupyterlab_extension-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

#### sagemaker_jupyterlab_extension/labextension/package.json

##### Pretty-printed

 * *Similarity: 0.9661111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.473afc439684735f2efc.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -60,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7282f69f1fc0d8e37b1c.js",
+            "load": "static/remoteEntry.473afc439684735f2efc.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -105,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

#### sagemaker_jupyterlab_extension/tests/test_request_logger.py

```diff
@@ -211,15 +211,15 @@
     assert (
         data["UriPath"] == "/jupyterlab/default/aws/sagemaker/api/git/list-repositories"
     )
     assert data["ResponseLatencyMS"] == 0.1
     assert (
         data["Context"]["ExtensionName"] == "SagemakerStudioJuypterLabExtensionCommon"
     )
-    assert data["Context"]["ExtensionVersion"] == "0.3.1"
+    assert data["Context"]["ExtensionVersion"] == "0.3.2"
     assert data["Context"]["AccountId"] == "1234567890"
     assert data["Context"]["DomainId"] == "d-jk12345678"
     assert data["Context"]["SpaceName"] == "default-space"
     data["_aws"]["Timestamp"] = 123456
 
     assert data["_aws"] == {
         "CloudWatchMetrics": [
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js` & `sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [548], {
         4548: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => Xe
             });
-            var a = n(9557);
+            var a = n(797);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
                 i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
                 o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
                 r = {
                     shutdown: "filemenu:shutdown"
                 },
                 l = "Sso",
@@ -94,16 +94,16 @@
                         e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
             var w = n(9801),
                 b = n.n(w),
                 E = n(6029),
                 f = n.n(E),
-                x = n(8368),
-                S = n(9510);
+                x = n(4072),
+                S = n(1464);
             class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
@@ -170,17 +170,17 @@
                     return {
                         sigInDialogResult: await i.launch(),
                         confirmDialog: i
                     }
                 };
             var N = n(6797),
                 B = n(6697),
-                I = n(1638),
-                z = n(7217),
-                A = n(5326);
+                I = n(2294),
+                z = n(2818),
+                A = n(2232);
             const U = (e, t, n, a, s, i, o) => {
                     const r = T(),
                         l = o(),
                         d = l && l + c;
                     if (null === r) j(e, !1);
                     else {
                         const o = b().unix(r / 1e3).diff(b()()),
@@ -290,17 +290,17 @@
                                 s.stop()
                             }), a, (e => {
                                 t = e
                             }), (() => t));
                         a()
                     }
                 };
-            var P = n(4613);
+            var P = n(7180);
             const G = [200, 201];
-            var $, O = n(6311);
+            var $, O = n(8671);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
             }($ || ($ = {}));
             const F = async (e, t) => {
                 const n = z.ServerConnection.makeSettings(),
                     a = O.URLExt.join(n.baseUrl, e);
                 try {
@@ -518,15 +518,15 @@
                         item: n,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ue = n(8031),
+            var ue = n(9380),
                 pe = n(2715);
             const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
@@ -725,15 +725,15 @@
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Re = n(5962),
+            var Re = n(8937),
                 Te = n(2190);
             const {
                 name: je,
                 version: ke
             } = n(4147), De = (e, t, n) => e.child({
                 ExtensionName: je,
                 ExtensionVersion: ke,
@@ -777,15 +777,15 @@
                         return !1
                     }
                     return "directory" === n.type
                 };
             var ze = n(1775),
                 Ae = n(248),
                 Ue = n(4337),
-                Le = n(8625);
+                Le = n(9510);
             const {
                 dialogTitle: Pe,
                 cancelButton: Ge,
                 cloneButton: $e,
                 errors: Oe
             } = m.GitClone, Fe = {
                 id: s,
@@ -1010,15 +1010,15 @@
                     }), f().createElement("p", null, `${n&&n[1]||Ye} / ${t?e:Je}`))
                 };
             class Ke extends S.ReactWidget {
                 constructor() {
                     super(), this.getSpaceName = async () => {
                         await F("aws/sagemaker/api/context", $.GET).then((e => {
                             e && e.json().then((e => {
-                                this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
+                                this.spaceName = e ? null == e ? void 0 : e.spaceName : null, this.update()
                             }))
                         }))
                     }, this.spaceName = "", this.getSpaceName()
                 }
                 render() {
                     return f().createElement(Qe, {
                         spaceName: this.spaceName
@@ -1063,11 +1063,11 @@
                 i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
                 }), "Language");
             t.Z = o
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.1","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.2","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js` & `sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -14,18 +14,18 @@
                 nA: () => G,
                 ZM: () => Q,
                 cU: () => J,
                 ky: () => K,
                 fS: () => V,
                 no: () => Z
             });
-            var n = i(9510),
-                s = i(3471),
-                r = i(6311),
-                o = i(3452),
+            var n = i(1464),
+                s = i(7594),
+                r = i(8671),
+                o = i(6805),
                 a = i(6697),
                 l = i(7930),
                 c = i(4882),
                 h = i(6029),
                 d = i.n(h);
             class u extends Error {
                 constructor(...e) {
@@ -34,15 +34,15 @@
             }
             var f = i(4666),
                 p = i(1894),
                 g = i(9861),
                 m = i(3343),
                 _ = i(9405),
                 y = i(9946),
-                v = i(8625),
+                v = i(9510),
                 b = i(1618);
             const w = 27.5,
                 x = 200;
 
             function C(e) {
                 const [t, i] = d().useState(""), [n, s] = d().useState(null), r = e.branches.filter((e => !t || e.name.includes(t))), {
                     action: o,
@@ -1854,15 +1854,15 @@
         },
         4148: (e, t, i) => {
             "use strict";
             i.d(t, {
                 x: () => I,
                 m: () => O
             });
-            var n = i(9510),
+            var n = i(1464),
                 s = i(4882),
                 r = i(4901),
                 o = i(6029);
             let a;
             a = "undefined" != typeof window ? window : "undefined" != typeof self ? self : i.g;
             let l = null,
                 c = null;
@@ -2046,19 +2046,19 @@
                 _ = i(1083);
             const y = (0, i(9946).oB)({
                 flex: "1 1 auto",
                 minHeight: "150px",
                 overflow: "hidden",
                 overflowY: "auto"
             });
-            var v = i(8625),
+            var v = i(9510),
                 b = i(4337),
                 w = i(427),
                 x = i(1552),
-                C = i(3452),
+                C = i(6805),
                 k = i(9405),
                 E = i(2322);
             const S = e => {
                 const [t, i] = o.useState(!0), n = e.files.length;
                 return o.createElement("div", {
                     className: E.ny
                 }, o.createElement("div", {
@@ -2703,15 +2703,15 @@
             }
         },
         7320: (e, t, i) => {
             "use strict";
             i.d(t, {
                 y: () => a
             });
-            var n = i(3452),
+            var n = i(6805),
                 s = i(6029),
                 r = i(4387),
                 o = i(8211);
             const a = e => {
                 var t;
                 const i = (0, o.Qz)(e.filepath),
                     a = e.filepath.slice(0, e.filepath.length - i.length).replace(/^\/|\/$/g, ""),
@@ -2925,15 +2925,15 @@
             }
         },
         429: (e, t, i) => {
             "use strict";
             i.d(t, {
                 zx: () => C
             });
-            var n = i(9510),
+            var n = i(1464),
                 s = i(3343),
                 r = i(4666),
                 o = i(1894),
                 a = i(6029),
                 l = i(9946),
                 c = i(1618);
             const h = (0, l.oB)({
@@ -3180,17 +3180,17 @@
         },
         1709: (e, t, i) => {
             "use strict";
             i.d(t, {
                 W: () => f,
                 w: () => u
             });
-            var n = i(3471),
-                s = i(7777),
-                r = i(5962),
+            var n = i(7594),
+                s = i(8873),
+                r = i(8937),
                 o = i(7930),
                 a = i(4882),
                 l = i(2027),
                 c = i(1770),
                 h = i(3781),
                 d = i(8799);
             const u = async ({
@@ -3389,16 +3389,16 @@
         },
         1218: (e, t, i) => {
             "use strict";
             i.d(t, {
                 f: () => o,
                 q: () => a
             });
-            var n = i(6311),
-                s = i(7217),
+            var n = i(8671),
+                s = i(2818),
                 r = i(4337);
             const o = ["Invalid username or password", "could not read Username", "could not read Password", "Authentication error"];
             async function a(e = "", t = "GET", i = null, o = "git") {
                 const a = s.ServerConnection.makeSettings(),
                     l = n.URLExt.join(a.baseUrl, o, e),
                     c = {
                         method: t,
@@ -3433,16 +3433,16 @@
         },
         568: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Bj: () => m,
                 bI: () => g
             });
-            var n, s = i(6311),
-                r = i(1638),
+            var n, s = i(8671),
+                r = i(2294),
                 o = i(7930),
                 a = i(6797),
                 l = i(4901),
                 c = i(1218);
             class h {
                 constructor() {
                     this._first = null, this._last = null, this._size = 0
@@ -4420,15 +4420,15 @@
         },
         5350: (e, t, i) => {
             "use strict";
             i.d(t, {
                 d: () => r,
                 x: () => s
             });
-            var n = i(9510);
+            var n = i(1464);
 
             function s(e, t) {
                 return {
                     autoClose: !1,
                     actions: [{
                         label: t.__("Show"),
                         callback: () => {
@@ -4845,15 +4845,15 @@
                         },
                         "&:disabled:active": {
                             backgroundColor: "var(--jp-layout-color3)"
                         }
                     }
                 })
         },
-        8625: (e, t, i) => {
+        9510: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Ug: () => r,
                 B3: () => o,
                 W6: () => a,
                 j0: () => l,
                 $N: () => c,
@@ -4870,15 +4870,15 @@
                 O4: () => v,
                 Ir: () => b,
                 W8: () => w,
                 V2: () => x,
                 yi: () => C,
                 Ds: () => k
             });
-            var n = i(3452);
+            var n = i(6805);
             const s = new n.LabIcon({
                     name: "git",
                     svgstr: '<svg\n  xmlns="http://www.w3.org/2000/svg"\n  viewBox="0 0 20 20"\n  width="16"\n>\n  <path\n    class="jp-icon3 jp-icon-selectable"\n    d="M19.6 9.1 10.9 0.4c-0.5-0.5-1.3-0.5-1.8 0l-1.8 1.8 2.3 2.3c0.5-0.2 1.1-0.1 1.6 0.4 0.4 0.4 0.5 1 0.4 1.6l2.2 2.2c0.5-0.2 1.2-0.1 1.6 0.4 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0C12.7 10.7 12.6 10.1 12.8 9.5l-2.1-2.1v5.4c0.1 0.1 0.3 0.2 0.4 0.3 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0-0.6-0.6-0.6-1.6 0-2.2 0.1-0.1 0.3-0.3 0.5-0.3V7.4C9.3 7.3 9.1 7.2 9 7 8.5 6.6 8.4 5.9 8.6 5.3L6.4 3.1 0.4 9.1c-0.5 0.5-0.5 1.3 0 1.8l8.7 8.7c0.5 0.5 1.3 0.5 1.8 0l8.7-8.7c0.5-0.5 0.5-1.3 0-1.8"\n    fill="#616161"\n  />\n</svg>\n'
                 }),
                 r = new n.LabIcon({
                     name: "git:add",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg"\n   width="16"\n   viewBox="0 0 24 24"\n   version="1.1">\n  <g\n     class="jp-icon3 jp-icon-selectable"\n     fill="#4F4F4F">\n    <path\n       d="m 22,13 h -9 v 9 H 11 V 13 H 2 v -2 h 9 V 2 h 2 v 9 h 9 z"/>\n  </g>\n</svg>\n'
@@ -4964,15 +4964,15 @@
             "use strict";
             i.d(t, {
                 $R: () => o,
                 H_: () => r,
                 LC: () => s,
                 TQ: () => a
             });
-            var n = i(7217);
+            var n = i(2818);
             const s = new(i(7930).Token)("jupyter.extensions.git_plugin");
             var r, o, a;
             ! function(e) {
                 let t, i;
                 ! function(e) {
                     let t;
                     ! function(e) {
@@ -5016,15 +5016,15 @@
             i.d(t, {
                 LJ: () => a,
                 Qz: () => r,
                 XO: () => c,
                 _v: () => l,
                 hp: () => o
             });
-            var n = i(6311),
+            var n = i(8671),
                 s = i(4337);
 
             function r(e) {
                 return "/" === e[e.length - 1] ? e : n.PathExt.basename(e)
             }
 
             function o(e) {
@@ -5065,15 +5065,15 @@
             }
         },
         8858: (e, t, i) => {
             "use strict";
             i.d(t, {
                 t: () => s
             });
-            var n = i(9510);
+            var n = i(1464);
             async function s(e, t, i) {
                 if ((await (0, n.showDialog)({
                         title: t.__("Discard all changes"),
                         body: i ? t.__("Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone.") : t.__("Are you sure you want to permanently discard changes to all files? This action cannot be undone."),
                         buttons: [n.Dialog.cancelButton({
                             label: t.__("Cancel")
                         }), n.Dialog.warnButton({
@@ -5740,15 +5740,15 @@
                             return l(arguments, "callee").get
                         } catch (e) {
                             return c
                         }
                     }
                 }() : c,
                 d = i(1405)(),
-                u = i(3276)(),
+                u = i(8185)(),
                 f = Object.getPrototypeOf || (u ? function(e) {
                     return e.__proto__
                 } : null),
                 p = {},
                 g = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
                 m = {
                     "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
@@ -5985,15 +5985,15 @@
                         value: 1
                     }).length
                 } catch (e) {
                     return !0
                 }
             }, e.exports = s
         },
-        3276: e => {
+        8185: e => {
             "use strict";
             var t = {
                     foo: {}
                 },
                 i = Object;
             e.exports = function() {
                 return {
@@ -6484,23 +6484,23 @@
             "use strict";
             i.d(t, {
                 QK: () => ne,
                 LI: () => Y
             });
             var n = i(8204),
                 s = i(6211),
-                r = i(5962),
+                r = i(8937),
                 o = i(4882),
                 a = i(9073),
                 l = i(8799),
                 c = i(4850),
                 h = i(1373),
                 d = i(8093),
-                u = i(3471),
-                f = i(7777);
+                u = i(7594),
+                f = i(8873);
             class p extends u.CodeEditorWrapper {
                 constructor(e) {
                     const {
                         factory: t,
                         value: i,
                         ...n
                     } = e, s = new d.YFile;
@@ -7761,15 +7761,15 @@
                 fy: () => b,
                 zr: () => d,
                 Jj: () => x,
                 Z: () => C,
                 tM: () => y,
                 CL: () => f
             });
-            var n = i(6963),
+            var n = i(3991),
                 s = i(1156),
                 r = i(4526),
                 o = i(7930),
                 a = i(8799),
                 l = i(4850),
                 c = i(1386);
             class h {
@@ -8590,15 +8590,15 @@
         },
         9073: (e, t, i) => {
             "use strict";
             i.d(t, {
                 M8: () => u,
                 AH: () => y
             });
-            var n = i(6963),
+            var n = i(3991),
                 s = i(4901),
                 r = i(4526),
                 o = i(3781),
                 a = i(1604),
                 l = i(1386),
                 c = i(8439),
                 h = i(4850),
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js` & `sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -1,34 +1,34 @@
-/*! For license information please see 891.4794a088a65e99550778.js.LICENSE.txt */
+/*! For license information please see 891.dba4cf1876582ab44697.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [891], {
         4891: (e, t, s) => {
             s.r(t), s.d(t, {
                 DiffModel: () => Wr.j,
                 Git: () => _.H_,
                 IGitExtension: () => _.LC,
                 NotebookDiff: () => $t,
                 PlainTextDiff: () => Or.W,
                 default: () => Pr
             });
-            var i = s(8368),
-                r = s(9510),
-                a = s(3471),
-                o = s(5326),
-                n = s(8031),
-                l = s(9557),
-                d = s(8048),
-                c = s(4008),
-                h = s(4613),
-                p = s(5962),
+            var i = s(4072),
+                r = s(1464),
+                a = s(7594),
+                o = s(2232),
+                n = s(9380),
+                l = s(797),
+                d = s(3413),
+                c = s(5099),
+                h = s(7180),
+                p = s(8937),
                 m = s(6029),
                 u = s.n(m),
                 g = s(1775),
-                f = s(8625),
+                f = s(9510),
                 _ = s(4337),
                 b = s(4882);
             class v extends b.Widget {
                 constructor(e) {
                     super({
                         node: v.createFormNode(e)
                     })
@@ -1432,15 +1432,15 @@
                     return s
                 }
                 get model() {
                     return this._model
                 }
             }
             var st = s(9073),
-                it = s(6963),
+                it = s(3991),
                 rt = s(5359);
             const at = "jp-DropPanel",
                 ot = "jp-DragPanel",
                 nt = "jp-mod-dragHandle",
                 lt = "jp-mod-dropTarget",
                 dt = "application/vnd.jupyter.dragindex";
 
@@ -1698,15 +1698,15 @@
                     return null
                 }
                 validateSource(e) {
                     return this.acceptDropsFromExternalSource ? -1 !== this.friends.indexOf(e.source) : super.validateSource(e)
                 }
             }
             ft._counter = 0, ft._groups = {};
-            var _t = s(1778);
+            var _t = s(3195);
             class bt extends _t.OutputAreaModel {
                 insert(e, t) {
                     this.list.insert(e, t)
                 }
                 move(e, t) {
                     this.list.move(e, t)
                 }
@@ -2674,16 +2674,16 @@
                         return null === (t = null == e ? void 0 : e.composite.displayStatus) || void 0 === t || t
                     } : function() {
                         return !1
                     }
                 }
             }(ls || (ls = {}));
             var ps = s(568),
-                ms = s(6311),
-                us = s(7217);
+                ms = s(8671),
+                us = s(2818);
             var gs = s(7858),
                 fs = s(1083);
             const _s = (0, F.oB)({
                     display: "flex",
                     flexDirection: "column",
                     height: "100%",
                     overflowY: "auto"
@@ -2758,15 +2758,15 @@
                 getValue() {
                     return {
                         name: this._name.value,
                         email: this._email.value
                     }
                 }
             }
-            var Ss = s(3452),
+            var Ss = s(6805),
                 ks = s(7350),
                 js = s(9397),
                 Ds = s(9522),
                 Bs = s(3926),
                 Ns = s(6514),
                 Ts = s(3931),
                 Fs = s(2964),
@@ -5480,15 +5480,15 @@
                         filebrowser: this._fileBrowserModel,
                         model: this._model,
                         settings: this._settings,
                         trans: this._trans
                     })
                 }
             }
-            var Rr = s(7777),
+            var Rr = s(8873),
                 Wr = s(5658),
                 Or = s(1709);
             const Ir = {
                     id: "@jupyterlab/git:plugin",
                     requires: [i.ILayoutRestorer, Rr.IEditorLanguageRegistry, a.IEditorServices, n.IDefaultFileBrowser, d.IRenderMimeRegistry, c.ISettingRegistry, o.IDocumentManager],
                     optional: [l.IMainMenu, h.IStatusBar, r.ICommandPalette, p.ITranslator],
                     provides: _.LC,
```

#### Comparing `sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js` & `sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js`

 * *Files 6% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
-            3570: (e, r, t) => {
+            3173: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
-                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
+                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(337), t.e(548)]).then((() => () => t(4548))),
+                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(337), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -51,58 +51,58 @@
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
         181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
+        337: "da58975bf5e0af92782f",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "a6ac1d0d39311897c48d",
-        571: "8dccdf5de15d462291c1",
+        548: "f4872310b34e6c6b2839",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
+        730: "9f65e223c4a041d10b21",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
         799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "26c15aab8d5d7301c11a",
-        853: "ced0d3671ec7406522f7",
+        823: "87642002230f9f1eed39",
         860: "d9b9c7e6da98c3818e92",
-        891: "4794a088a65e99550778"
+        891: "dba4cf1876582ab44697"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
         181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
+        337: "da58975bf5e0af92782f",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "a6ac1d0d39311897c48d",
-        571: "8dccdf5de15d462291c1",
+        548: "f4872310b34e6c6b2839",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
+        730: "9f65e223c4a041d10b21",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
         799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "26c15aab8d5d7301c11a",
-        853: "ced0d3671ec7406522f7",
+        823: "87642002230f9f1eed39",
         860: "d9b9c7e6da98c3818e92",
-        891: "4794a088a65e99550778"
+        891: "dba4cf1876582ab44697"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.1", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.2", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(337), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(337), S.e(730)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -273,59 +273,59 @@
     })(((e, r, t, a) => (l(e, t), m(c(r, t, a) || p(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && c(r, t, a);
         return o ? m(o) : n()
     })), j = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
         8800: () => y("default", "@emotion/styled", [1, 11, 3, 0], (() => S.e(860).then((() => () => S(4378))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
+        797: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
         1373: () => g("default", "@codemirror/language", [1, 6, 0, 0]),
-        1638: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
-        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
-        4613: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
+        1464: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        2232: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 6]),
+        2294: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
+        2818: () => g("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        3991: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 6]),
+        4072: () => g("default", "@jupyterlab/application", [1, 4, 1, 6]),
         4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
-        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
         6211: () => g("default", "@codemirror/view", [1, 6, 9, 6]),
-        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         6697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         6797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
-        6963: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 5]),
-        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
-        7777: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
+        6805: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        7180: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 6]),
+        7594: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 6]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        8031: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8204: () => g("default", "@codemirror/state", [1, 6, 2, 0]),
-        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
-        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
+        8671: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        8873: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 6]),
+        8937: () => g("default", "@jupyterlab/translation", [1, 4, 1, 6]),
+        9380: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
         248: () => g("default", "@amzn/sagemaker-jupyterlab-extension-common", [2, 0, 1, 2]),
-        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(571)]).then((() => () => S(4891))))),
+        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(730)]).then((() => () => S(4891))))),
         5933: () => y("default", "@emotion/css", [1, 11, 1, 3], (() => S.e(222).then((() => () => S(3505))))),
         9801: () => y("default", "moment", [1, 2, 29, 4], (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381))))),
-        1778: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
-        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
+        3195: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 6]),
+        3413: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        5099: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
         5359: () => g("default", "@lumino/dragdrop", [1, 2, 0, 0]),
         5633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         7350: () => g("default", "@lumino/commands", [1, 2, 0, 1]),
         7489: () => y("default", "@mui/material", [1, 5, 12, 1], (() => Promise.all([S.e(181), S.e(799)]).then((() => () => S(7799))))),
         7858: () => y("default", "@mui/icons-material", [1, 5, 11, 16], (() => S.e(242).then((() => () => S(4242))))),
-        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         851: () => g("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => g("default", "@lezer/highlight", [1, 1, 0, 0])
     }, P = {
         29: [6029],
+        337: [797, 1373, 1464, 2232, 2294, 2818, 3991, 4072, 4882, 4901, 6211, 6697, 6797, 6805, 7180, 7594, 7930, 8093, 8204, 8671, 8873, 8937, 9380],
         548: [248, 2190, 5933, 9801],
-        571: [1778, 4008, 5359, 5633, 7350, 7489, 7858, 8048],
         704: [7704],
+        730: [3195, 3413, 5099, 5359, 5633, 7350, 7489, 7858],
         798: [851, 7138],
-        800: [8800],
-        853: [1373, 1638, 3452, 3471, 4613, 4882, 4901, 5326, 5962, 6211, 6311, 6697, 6797, 6963, 7217, 7777, 7930, 8031, 8093, 8204, 8368, 9510, 9557]
+        800: [8800]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -346,15 +346,15 @@
         var e = {
             584: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(29|571|704|798|800|853)$/.test(r)) e[r] = 0;
+                else if (/^(7(04|30|98)|29|337|800)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = S.p + S.u(r),
                     l = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(3570);
+    var E = S(3173);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES` & `sagemaker_jupyterlab_extension-0.3.2.data/data/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json`

 * *Files 1% similar despite different names*

##### Pretty-printed

 * *Similarity: 0.9661111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.473afc439684735f2efc.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -60,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7282f69f1fc0d8e37b1c.js",
+            "load": "static/remoteEntry.473afc439684735f2efc.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -105,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.f4872310b34e6c6b2839.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [548], {
         4548: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => Xe
             });
-            var a = n(9557);
+            var a = n(797);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
                 i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
                 o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
                 r = {
                     shutdown: "filemenu:shutdown"
                 },
                 l = "Sso",
@@ -94,16 +94,16 @@
                         e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
             var w = n(9801),
                 b = n.n(w),
                 E = n(6029),
                 f = n.n(E),
-                x = n(8368),
-                S = n(9510);
+                x = n(4072),
+                S = n(1464);
             class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
@@ -170,17 +170,17 @@
                     return {
                         sigInDialogResult: await i.launch(),
                         confirmDialog: i
                     }
                 };
             var N = n(6797),
                 B = n(6697),
-                I = n(1638),
-                z = n(7217),
-                A = n(5326);
+                I = n(2294),
+                z = n(2818),
+                A = n(2232);
             const U = (e, t, n, a, s, i, o) => {
                     const r = T(),
                         l = o(),
                         d = l && l + c;
                     if (null === r) j(e, !1);
                     else {
                         const o = b().unix(r / 1e3).diff(b()()),
@@ -290,17 +290,17 @@
                                 s.stop()
                             }), a, (e => {
                                 t = e
                             }), (() => t));
                         a()
                     }
                 };
-            var P = n(4613);
+            var P = n(7180);
             const G = [200, 201];
-            var $, O = n(6311);
+            var $, O = n(8671);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
             }($ || ($ = {}));
             const F = async (e, t) => {
                 const n = z.ServerConnection.makeSettings(),
                     a = O.URLExt.join(n.baseUrl, e);
                 try {
@@ -518,15 +518,15 @@
                         item: n,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ue = n(8031),
+            var ue = n(9380),
                 pe = n(2715);
             const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
@@ -725,15 +725,15 @@
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Re = n(5962),
+            var Re = n(8937),
                 Te = n(2190);
             const {
                 name: je,
                 version: ke
             } = n(4147), De = (e, t, n) => e.child({
                 ExtensionName: je,
                 ExtensionVersion: ke,
@@ -777,15 +777,15 @@
                         return !1
                     }
                     return "directory" === n.type
                 };
             var ze = n(1775),
                 Ae = n(248),
                 Ue = n(4337),
-                Le = n(8625);
+                Le = n(9510);
             const {
                 dialogTitle: Pe,
                 cancelButton: Ge,
                 cloneButton: $e,
                 errors: Oe
             } = m.GitClone, Fe = {
                 id: s,
@@ -1010,15 +1010,15 @@
                     }), f().createElement("p", null, `${n&&n[1]||Ye} / ${t?e:Je}`))
                 };
             class Ke extends S.ReactWidget {
                 constructor() {
                     super(), this.getSpaceName = async () => {
                         await F("aws/sagemaker/api/context", $.GET).then((e => {
                             e && e.json().then((e => {
-                                this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
+                                this.spaceName = e ? null == e ? void 0 : e.spaceName : null, this.update()
                             }))
                         }))
                     }, this.spaceName = "", this.getSpaceName()
                 }
                 render() {
                     return f().createElement(Qe, {
                         spaceName: this.spaceName
@@ -1063,11 +1063,11 @@
                 i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
                 }), "Language");
             t.Z = o
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.1","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.2","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.87642002230f9f1eed39.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -14,18 +14,18 @@
                 nA: () => G,
                 ZM: () => Q,
                 cU: () => J,
                 ky: () => K,
                 fS: () => V,
                 no: () => Z
             });
-            var n = i(9510),
-                s = i(3471),
-                r = i(6311),
-                o = i(3452),
+            var n = i(1464),
+                s = i(7594),
+                r = i(8671),
+                o = i(6805),
                 a = i(6697),
                 l = i(7930),
                 c = i(4882),
                 h = i(6029),
                 d = i.n(h);
             class u extends Error {
                 constructor(...e) {
@@ -34,15 +34,15 @@
             }
             var f = i(4666),
                 p = i(1894),
                 g = i(9861),
                 m = i(3343),
                 _ = i(9405),
                 y = i(9946),
-                v = i(8625),
+                v = i(9510),
                 b = i(1618);
             const w = 27.5,
                 x = 200;
 
             function C(e) {
                 const [t, i] = d().useState(""), [n, s] = d().useState(null), r = e.branches.filter((e => !t || e.name.includes(t))), {
                     action: o,
@@ -1854,15 +1854,15 @@
         },
         4148: (e, t, i) => {
             "use strict";
             i.d(t, {
                 x: () => I,
                 m: () => O
             });
-            var n = i(9510),
+            var n = i(1464),
                 s = i(4882),
                 r = i(4901),
                 o = i(6029);
             let a;
             a = "undefined" != typeof window ? window : "undefined" != typeof self ? self : i.g;
             let l = null,
                 c = null;
@@ -2046,19 +2046,19 @@
                 _ = i(1083);
             const y = (0, i(9946).oB)({
                 flex: "1 1 auto",
                 minHeight: "150px",
                 overflow: "hidden",
                 overflowY: "auto"
             });
-            var v = i(8625),
+            var v = i(9510),
                 b = i(4337),
                 w = i(427),
                 x = i(1552),
-                C = i(3452),
+                C = i(6805),
                 k = i(9405),
                 E = i(2322);
             const S = e => {
                 const [t, i] = o.useState(!0), n = e.files.length;
                 return o.createElement("div", {
                     className: E.ny
                 }, o.createElement("div", {
@@ -2703,15 +2703,15 @@
             }
         },
         7320: (e, t, i) => {
             "use strict";
             i.d(t, {
                 y: () => a
             });
-            var n = i(3452),
+            var n = i(6805),
                 s = i(6029),
                 r = i(4387),
                 o = i(8211);
             const a = e => {
                 var t;
                 const i = (0, o.Qz)(e.filepath),
                     a = e.filepath.slice(0, e.filepath.length - i.length).replace(/^\/|\/$/g, ""),
@@ -2925,15 +2925,15 @@
             }
         },
         429: (e, t, i) => {
             "use strict";
             i.d(t, {
                 zx: () => C
             });
-            var n = i(9510),
+            var n = i(1464),
                 s = i(3343),
                 r = i(4666),
                 o = i(1894),
                 a = i(6029),
                 l = i(9946),
                 c = i(1618);
             const h = (0, l.oB)({
@@ -3180,17 +3180,17 @@
         },
         1709: (e, t, i) => {
             "use strict";
             i.d(t, {
                 W: () => f,
                 w: () => u
             });
-            var n = i(3471),
-                s = i(7777),
-                r = i(5962),
+            var n = i(7594),
+                s = i(8873),
+                r = i(8937),
                 o = i(7930),
                 a = i(4882),
                 l = i(2027),
                 c = i(1770),
                 h = i(3781),
                 d = i(8799);
             const u = async ({
@@ -3389,16 +3389,16 @@
         },
         1218: (e, t, i) => {
             "use strict";
             i.d(t, {
                 f: () => o,
                 q: () => a
             });
-            var n = i(6311),
-                s = i(7217),
+            var n = i(8671),
+                s = i(2818),
                 r = i(4337);
             const o = ["Invalid username or password", "could not read Username", "could not read Password", "Authentication error"];
             async function a(e = "", t = "GET", i = null, o = "git") {
                 const a = s.ServerConnection.makeSettings(),
                     l = n.URLExt.join(a.baseUrl, o, e),
                     c = {
                         method: t,
@@ -3433,16 +3433,16 @@
         },
         568: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Bj: () => m,
                 bI: () => g
             });
-            var n, s = i(6311),
-                r = i(1638),
+            var n, s = i(8671),
+                r = i(2294),
                 o = i(7930),
                 a = i(6797),
                 l = i(4901),
                 c = i(1218);
             class h {
                 constructor() {
                     this._first = null, this._last = null, this._size = 0
@@ -4420,15 +4420,15 @@
         },
         5350: (e, t, i) => {
             "use strict";
             i.d(t, {
                 d: () => r,
                 x: () => s
             });
-            var n = i(9510);
+            var n = i(1464);
 
             function s(e, t) {
                 return {
                     autoClose: !1,
                     actions: [{
                         label: t.__("Show"),
                         callback: () => {
@@ -4845,15 +4845,15 @@
                         },
                         "&:disabled:active": {
                             backgroundColor: "var(--jp-layout-color3)"
                         }
                     }
                 })
         },
-        8625: (e, t, i) => {
+        9510: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Ug: () => r,
                 B3: () => o,
                 W6: () => a,
                 j0: () => l,
                 $N: () => c,
@@ -4870,15 +4870,15 @@
                 O4: () => v,
                 Ir: () => b,
                 W8: () => w,
                 V2: () => x,
                 yi: () => C,
                 Ds: () => k
             });
-            var n = i(3452);
+            var n = i(6805);
             const s = new n.LabIcon({
                     name: "git",
                     svgstr: '<svg\n  xmlns="http://www.w3.org/2000/svg"\n  viewBox="0 0 20 20"\n  width="16"\n>\n  <path\n    class="jp-icon3 jp-icon-selectable"\n    d="M19.6 9.1 10.9 0.4c-0.5-0.5-1.3-0.5-1.8 0l-1.8 1.8 2.3 2.3c0.5-0.2 1.1-0.1 1.6 0.4 0.4 0.4 0.5 1 0.4 1.6l2.2 2.2c0.5-0.2 1.2-0.1 1.6 0.4 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0C12.7 10.7 12.6 10.1 12.8 9.5l-2.1-2.1v5.4c0.1 0.1 0.3 0.2 0.4 0.3 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0-0.6-0.6-0.6-1.6 0-2.2 0.1-0.1 0.3-0.3 0.5-0.3V7.4C9.3 7.3 9.1 7.2 9 7 8.5 6.6 8.4 5.9 8.6 5.3L6.4 3.1 0.4 9.1c-0.5 0.5-0.5 1.3 0 1.8l8.7 8.7c0.5 0.5 1.3 0.5 1.8 0l8.7-8.7c0.5-0.5 0.5-1.3 0-1.8"\n    fill="#616161"\n  />\n</svg>\n'
                 }),
                 r = new n.LabIcon({
                     name: "git:add",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg"\n   width="16"\n   viewBox="0 0 24 24"\n   version="1.1">\n  <g\n     class="jp-icon3 jp-icon-selectable"\n     fill="#4F4F4F">\n    <path\n       d="m 22,13 h -9 v 9 H 11 V 13 H 2 v -2 h 9 V 2 h 2 v 9 h 9 z"/>\n  </g>\n</svg>\n'
@@ -4964,15 +4964,15 @@
             "use strict";
             i.d(t, {
                 $R: () => o,
                 H_: () => r,
                 LC: () => s,
                 TQ: () => a
             });
-            var n = i(7217);
+            var n = i(2818);
             const s = new(i(7930).Token)("jupyter.extensions.git_plugin");
             var r, o, a;
             ! function(e) {
                 let t, i;
                 ! function(e) {
                     let t;
                     ! function(e) {
@@ -5016,15 +5016,15 @@
             i.d(t, {
                 LJ: () => a,
                 Qz: () => r,
                 XO: () => c,
                 _v: () => l,
                 hp: () => o
             });
-            var n = i(6311),
+            var n = i(8671),
                 s = i(4337);
 
             function r(e) {
                 return "/" === e[e.length - 1] ? e : n.PathExt.basename(e)
             }
 
             function o(e) {
@@ -5065,15 +5065,15 @@
             }
         },
         8858: (e, t, i) => {
             "use strict";
             i.d(t, {
                 t: () => s
             });
-            var n = i(9510);
+            var n = i(1464);
             async function s(e, t, i) {
                 if ((await (0, n.showDialog)({
                         title: t.__("Discard all changes"),
                         body: i ? t.__("Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone.") : t.__("Are you sure you want to permanently discard changes to all files? This action cannot be undone."),
                         buttons: [n.Dialog.cancelButton({
                             label: t.__("Cancel")
                         }), n.Dialog.warnButton({
@@ -5740,15 +5740,15 @@
                             return l(arguments, "callee").get
                         } catch (e) {
                             return c
                         }
                     }
                 }() : c,
                 d = i(1405)(),
-                u = i(3276)(),
+                u = i(8185)(),
                 f = Object.getPrototypeOf || (u ? function(e) {
                     return e.__proto__
                 } : null),
                 p = {},
                 g = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
                 m = {
                     "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
@@ -5985,15 +5985,15 @@
                         value: 1
                     }).length
                 } catch (e) {
                     return !0
                 }
             }, e.exports = s
         },
-        3276: e => {
+        8185: e => {
             "use strict";
             var t = {
                     foo: {}
                 },
                 i = Object;
             e.exports = function() {
                 return {
@@ -6484,23 +6484,23 @@
             "use strict";
             i.d(t, {
                 QK: () => ne,
                 LI: () => Y
             });
             var n = i(8204),
                 s = i(6211),
-                r = i(5962),
+                r = i(8937),
                 o = i(4882),
                 a = i(9073),
                 l = i(8799),
                 c = i(4850),
                 h = i(1373),
                 d = i(8093),
-                u = i(3471),
-                f = i(7777);
+                u = i(7594),
+                f = i(8873);
             class p extends u.CodeEditorWrapper {
                 constructor(e) {
                     const {
                         factory: t,
                         value: i,
                         ...n
                     } = e, s = new d.YFile;
@@ -7761,15 +7761,15 @@
                 fy: () => b,
                 zr: () => d,
                 Jj: () => x,
                 Z: () => C,
                 tM: () => y,
                 CL: () => f
             });
-            var n = i(6963),
+            var n = i(3991),
                 s = i(1156),
                 r = i(4526),
                 o = i(7930),
                 a = i(8799),
                 l = i(4850),
                 c = i(1386);
             class h {
@@ -8590,15 +8590,15 @@
         },
         9073: (e, t, i) => {
             "use strict";
             i.d(t, {
                 M8: () => u,
                 AH: () => y
             });
-            var n = i(6963),
+            var n = i(3991),
                 s = i(4901),
                 r = i(4526),
                 o = i(3781),
                 a = i(1604),
                 l = i(1386),
                 c = i(8439),
                 h = i(4850),
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js`

 * *Files 0% similar despite different names*

##### js-beautify {}

```diff
@@ -1,34 +1,34 @@
-/*! For license information please see 891.4794a088a65e99550778.js.LICENSE.txt */
+/*! For license information please see 891.dba4cf1876582ab44697.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [891], {
         4891: (e, t, s) => {
             s.r(t), s.d(t, {
                 DiffModel: () => Wr.j,
                 Git: () => _.H_,
                 IGitExtension: () => _.LC,
                 NotebookDiff: () => $t,
                 PlainTextDiff: () => Or.W,
                 default: () => Pr
             });
-            var i = s(8368),
-                r = s(9510),
-                a = s(3471),
-                o = s(5326),
-                n = s(8031),
-                l = s(9557),
-                d = s(8048),
-                c = s(4008),
-                h = s(4613),
-                p = s(5962),
+            var i = s(4072),
+                r = s(1464),
+                a = s(7594),
+                o = s(2232),
+                n = s(9380),
+                l = s(797),
+                d = s(3413),
+                c = s(5099),
+                h = s(7180),
+                p = s(8937),
                 m = s(6029),
                 u = s.n(m),
                 g = s(1775),
-                f = s(8625),
+                f = s(9510),
                 _ = s(4337),
                 b = s(4882);
             class v extends b.Widget {
                 constructor(e) {
                     super({
                         node: v.createFormNode(e)
                     })
@@ -1432,15 +1432,15 @@
                     return s
                 }
                 get model() {
                     return this._model
                 }
             }
             var st = s(9073),
-                it = s(6963),
+                it = s(3991),
                 rt = s(5359);
             const at = "jp-DropPanel",
                 ot = "jp-DragPanel",
                 nt = "jp-mod-dragHandle",
                 lt = "jp-mod-dropTarget",
                 dt = "application/vnd.jupyter.dragindex";
 
@@ -1698,15 +1698,15 @@
                     return null
                 }
                 validateSource(e) {
                     return this.acceptDropsFromExternalSource ? -1 !== this.friends.indexOf(e.source) : super.validateSource(e)
                 }
             }
             ft._counter = 0, ft._groups = {};
-            var _t = s(1778);
+            var _t = s(3195);
             class bt extends _t.OutputAreaModel {
                 insert(e, t) {
                     this.list.insert(e, t)
                 }
                 move(e, t) {
                     this.list.move(e, t)
                 }
@@ -2674,16 +2674,16 @@
                         return null === (t = null == e ? void 0 : e.composite.displayStatus) || void 0 === t || t
                     } : function() {
                         return !1
                     }
                 }
             }(ls || (ls = {}));
             var ps = s(568),
-                ms = s(6311),
-                us = s(7217);
+                ms = s(8671),
+                us = s(2818);
             var gs = s(7858),
                 fs = s(1083);
             const _s = (0, F.oB)({
                     display: "flex",
                     flexDirection: "column",
                     height: "100%",
                     overflowY: "auto"
@@ -2758,15 +2758,15 @@
                 getValue() {
                     return {
                         name: this._name.value,
                         email: this._email.value
                     }
                 }
             }
-            var Ss = s(3452),
+            var Ss = s(6805),
                 ks = s(7350),
                 js = s(9397),
                 Ds = s(9522),
                 Bs = s(3926),
                 Ns = s(6514),
                 Ts = s(3931),
                 Fs = s(2964),
@@ -5480,15 +5480,15 @@
                         filebrowser: this._fileBrowserModel,
                         model: this._model,
                         settings: this._settings,
                         trans: this._trans
                     })
                 }
             }
-            var Rr = s(7777),
+            var Rr = s(8873),
                 Wr = s(5658),
                 Or = s(1709);
             const Ir = {
                     id: "@jupyterlab/git:plugin",
                     requires: [i.ILayoutRestorer, Rr.IEditorLanguageRegistry, a.IEditorServices, n.IDefaultFileBrowser, d.IRenderMimeRegistry, c.ISettingRegistry, o.IDocumentManager],
                     optional: [l.IMainMenu, h.IStatusBar, r.ICommandPalette, p.ITranslator],
                     provides: _.LC,
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.473afc439684735f2efc.js`

 * *Files 6% similar despite different names*

##### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
-            3570: (e, r, t) => {
+            3173: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
-                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
+                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(337), t.e(548)]).then((() => () => t(4548))),
+                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(337), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -51,58 +51,58 @@
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
         181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
+        337: "da58975bf5e0af92782f",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "a6ac1d0d39311897c48d",
-        571: "8dccdf5de15d462291c1",
+        548: "f4872310b34e6c6b2839",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
+        730: "9f65e223c4a041d10b21",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
         799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "26c15aab8d5d7301c11a",
-        853: "ced0d3671ec7406522f7",
+        823: "87642002230f9f1eed39",
         860: "d9b9c7e6da98c3818e92",
-        891: "4794a088a65e99550778"
+        891: "dba4cf1876582ab44697"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
         181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
+        337: "da58975bf5e0af92782f",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "a6ac1d0d39311897c48d",
-        571: "8dccdf5de15d462291c1",
+        548: "f4872310b34e6c6b2839",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
+        730: "9f65e223c4a041d10b21",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
         799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "26c15aab8d5d7301c11a",
-        853: "ced0d3671ec7406522f7",
+        823: "87642002230f9f1eed39",
         860: "d9b9c7e6da98c3818e92",
-        891: "4794a088a65e99550778"
+        891: "dba4cf1876582ab44697"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.1", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.2", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(337), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(337), S.e(730)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -273,59 +273,59 @@
     })(((e, r, t, a) => (l(e, t), m(c(r, t, a) || p(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && c(r, t, a);
         return o ? m(o) : n()
     })), j = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
         8800: () => y("default", "@emotion/styled", [1, 11, 3, 0], (() => S.e(860).then((() => () => S(4378))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
+        797: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
         1373: () => g("default", "@codemirror/language", [1, 6, 0, 0]),
-        1638: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
-        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
-        4613: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
+        1464: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        2232: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 6]),
+        2294: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
+        2818: () => g("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        3991: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 6]),
+        4072: () => g("default", "@jupyterlab/application", [1, 4, 1, 6]),
         4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
-        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
         6211: () => g("default", "@codemirror/view", [1, 6, 9, 6]),
-        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         6697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         6797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
-        6963: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 5]),
-        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
-        7777: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
+        6805: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        7180: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 6]),
+        7594: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 6]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        8031: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8204: () => g("default", "@codemirror/state", [1, 6, 2, 0]),
-        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
-        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
+        8671: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        8873: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 6]),
+        8937: () => g("default", "@jupyterlab/translation", [1, 4, 1, 6]),
+        9380: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
         248: () => g("default", "@amzn/sagemaker-jupyterlab-extension-common", [2, 0, 1, 2]),
-        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(571)]).then((() => () => S(4891))))),
+        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(730)]).then((() => () => S(4891))))),
         5933: () => y("default", "@emotion/css", [1, 11, 1, 3], (() => S.e(222).then((() => () => S(3505))))),
         9801: () => y("default", "moment", [1, 2, 29, 4], (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381))))),
-        1778: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
-        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
+        3195: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 6]),
+        3413: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        5099: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
         5359: () => g("default", "@lumino/dragdrop", [1, 2, 0, 0]),
         5633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         7350: () => g("default", "@lumino/commands", [1, 2, 0, 1]),
         7489: () => y("default", "@mui/material", [1, 5, 12, 1], (() => Promise.all([S.e(181), S.e(799)]).then((() => () => S(7799))))),
         7858: () => y("default", "@mui/icons-material", [1, 5, 11, 16], (() => S.e(242).then((() => () => S(4242))))),
-        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         851: () => g("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => g("default", "@lezer/highlight", [1, 1, 0, 0])
     }, P = {
         29: [6029],
+        337: [797, 1373, 1464, 2232, 2294, 2818, 3991, 4072, 4882, 4901, 6211, 6697, 6797, 6805, 7180, 7594, 7930, 8093, 8204, 8671, 8873, 8937, 9380],
         548: [248, 2190, 5933, 9801],
-        571: [1778, 4008, 5359, 5633, 7350, 7489, 7858, 8048],
         704: [7704],
+        730: [3195, 3413, 5099, 5359, 5633, 7350, 7489, 7858],
         798: [851, 7138],
-        800: [8800],
-        853: [1373, 1638, 3452, 3471, 4613, 4882, 4901, 5326, 5962, 6211, 6311, 6697, 6797, 6963, 7217, 7777, 7930, 8031, 8093, 8204, 8368, 9510, 9557]
+        800: [8800]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -346,15 +346,15 @@
         var e = {
             584: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(29|571|704|798|800|853)$/.test(r)) e[r] = 0;
+                else if (/^(7(04|30|98)|29|337|800)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = S.p + S.u(r),
                     l = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(3570);
+    var E = S(3173);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json` & `sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE` & `sagemaker_jupyterlab_extension-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA` & `sagemaker_jupyterlab_extension-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.3.1
+Version: 0.3.2
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

#### Comparing `sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD` & `sagemaker_jupyterlab_extension-0.3.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 sagemaker_jupyterlab_extension/__init__.py,sha256=hxDcPQ4HLDyOST0TL-Lu5fvzhEwrIgSkZLybVPPEkgk,1133
 sagemaker_jupyterlab_extension/_version.py,sha256=H8LOQyA3X6Xj3pixozSSsatne-Jd9sIhfgCIwlM6AGg,683
 sagemaker_jupyterlab_extension/handlers.py,sha256=j2uNNvU6Vu2guPRev4OEuyKtc_YkOJfAql3exvdn1nw,11587
-sagemaker_jupyterlab_extension/labextension/package.json,sha256=MJlCTqCdvftbBuXD6FnQG7gwbiFt7MxiShrRbgGUhl8,4091
+sagemaker_jupyterlab_extension/labextension/package.json,sha256=fkUI0wDVT63nMLtvJMQxYxKMO5CC_lsvMwbRBhI3svA,4091
 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
 sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
-sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js,sha256=pqwdDTkxGJfEjX8rz1Mva5X-RXr5FGeFs98FHE2UxHg,28123
+sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js,sha256=9IcjELNObGsoOZ05j97gelAa7eMRnRQH_C6fiziV-i0,28122
 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
 sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
-sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js,sha256=JsFaq41dcwHBGlJbsMA6G_eWnb33uUncDPP8e8qUf5I,266482
+sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js,sha256=h2QgAiMPnx7tOa0WITReViwRLp6IEfA4fH5KHrnK0xo,266482
 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
-sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
-sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
-sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js,sha256=coL2nx_A2ON7HHT_xMFMCti2yk2w5G6rylX5P6EipG4,12105
+sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js,sha256=reDepbAyimKis4NMUqqriTsHuEaJ4lOm3DDtU4pkXrs,139404
+sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
+sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js,sha256=Rzr8Q5aEc18u_NNlRg_YnKiLZEt_LmDVQhVGYz0kv2E,12103
 sagemaker_jupyterlab_extension/labextension/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
 sagemaker_jupyterlab_extension/tests/__init__.py,sha256=LJe9lg48SCXTjTOe_oc0_Zj9blApYphXi-12E_3fh2s,60
 sagemaker_jupyterlab_extension/tests/helper.py,sha256=bH3LEHznHOzkfOfBmRn-S8hh5sUuRHj_EmjvjUdQ4uc,405
 sagemaker_jupyterlab_extension/tests/test_error_util.py,sha256=QBhspnhVQzw_a8yUVlfhxalT8ywS3sntb_diFK4nvDw,1647
 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py,sha256=O-QWKCetqSPCpzhBlFqS4zO1dp9_nJdGGpE_mqor2BU,5332
 sagemaker_jupyterlab_extension/tests/test_handlers.py,sha256=6BOEKL3v87psZtcqVbqlHjfRzyiBFZfFcUbig-ELCB8,5041
-sagemaker_jupyterlab_extension/tests/test_request_logger.py,sha256=MLvH7Ncrj34HdS9wkNZNAd_UDBDWKpBzpnNRPxNQqzc,7701
+sagemaker_jupyterlab_extension/tests/test_request_logger.py,sha256=cDkWqvbHpGSQJ9DqBL087D86VqpNAyHdUdezw-BUgz0,7701
 sagemaker_jupyterlab_extension/utils/__init__.py,sha256=r4W_GQMVXe3D90bLPU9hZUehj0U1AhbN1qDE9M5vI6Y,64
 sagemaker_jupyterlab_extension/utils/error_util.py,sha256=fT6BDMGeHK9J70A8vyGkl_ygL662XQ5incmoq8X_R1Y,555
 sagemaker_jupyterlab_extension/utils/git_clone_util.py,sha256=pHExYjlSniCLZ-Q78OjrfIvsPPz2Cd13jB7F9Jiiu-s,2552
 sagemaker_jupyterlab_extension/utils/metric_util.py,sha256=h2w-vEFVpJkSSOA97gr5hpG6ROe6xgfYbK_VaaBItvg,507
 sagemaker_jupyterlab_extension/utils/request_logger.py,sha256=SNq6_gng-ElaUDl_akXmcFRYy9gFlydcRwWRZphNFs4,7250
-sagemaker_jupyterlab_extension-0.3.1.data/data/THIRD-PARTY-LICENSES,sha256=lL9OuaJ1ullVxluRJKKFT6xqWiCV3COZsSBBQHmFD6U,8139
-sagemaker_jupyterlab_extension-0.3.1.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json,sha256=U-i2pBYj1meFIyYC2auwNjK24HQIzgGCAcZZPtqjJZQ,105
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json,sha256=Y5TsP4lidrq-9l8YzVJvdwPbOXcVvHbehOFJov8eM_A,221
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json,sha256=MJlCTqCdvftbBuXD6FnQG7gwbiFt7MxiShrRbgGUhl8,4091
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.a6ac1d0d39311897c48d.js,sha256=pqwdDTkxGJfEjX8rz1Mva5X-RXr5FGeFs98FHE2UxHg,28123
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.26c15aab8d5d7301c11a.js,sha256=JsFaq41dcwHBGlJbsMA6G_eWnb33uUncDPP8e8qUf5I,266482
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js,sha256=5iQSQgHaR-F5tI50GUTo-KOV1q9-eYprmtQw962uIOg,139405
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.4794a088a65e99550778.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.7282f69f1fc0d8e37b1c.js,sha256=coL2nx_A2ON7HHT_xMFMCti2yk2w5G6rylX5P6EipG4,12105
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
-sagemaker_jupyterlab_extension-0.3.1.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
-sagemaker_jupyterlab_extension-0.3.1.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
-sagemaker_jupyterlab_extension-0.3.1.dist-info/METADATA,sha256=wMFygsrQaYHwrrG8vq2NB_IUVAieHGuS0NV7gqQ4oBc,2281
-sagemaker_jupyterlab_extension-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-sagemaker_jupyterlab_extension-0.3.1.dist-info/top_level.txt,sha256=96mz5zVRnlKUFu46rV4QFpibtf4h9CD5HVkLxPBcah8,31
-sagemaker_jupyterlab_extension-0.3.1.dist-info/RECORD,,
+sagemaker_jupyterlab_extension-0.3.2.data/data/THIRD-PARTY-LICENSES,sha256=lL9OuaJ1ullVxluRJKKFT6xqWiCV3COZsSBBQHmFD6U,8139
+sagemaker_jupyterlab_extension-0.3.2.data/data/etc/jupyter/jupyter_server_config.d/sagemaker_jupyterlab_extension.json,sha256=U-i2pBYj1meFIyYC2auwNjK24HQIzgGCAcZZPtqjJZQ,105
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/install.json,sha256=Y5TsP4lidrq-9l8YzVJvdwPbOXcVvHbehOFJov8eM_A,221
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/package.json,sha256=fkUI0wDVT63nMLtvJMQxYxKMO5CC_lsvMwbRBhI3svA,4091
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/10.c2420c83a55ee1ffecfe.js,sha256=wkIMg6Ve4f_s_ptN3vtQkhMPVH3mMP72Z6oG6PFw-zM,3280
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/181.9a0cdfa414e5cba3947c.js,sha256=mgzfpBTly6OUfBmlVxrxcB1y7VZM780VsUDayhCRzJU,92715
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/222.587a32e1b3cb7433cc73.js,sha256=WHoy4bPLdDPMcySsIDRCa7-D_OuoFcsqMpurM7cdcds,1874
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/242.13e5d4563ddb8069ebd5.js,sha256=E-XUVj3bgGnr1SJ29J8TSKFR4SQ_BKWeNKpLC8ke_K8,4112866
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/378.ddf9e5d607ffbd26d01d.js,sha256=3fnl1gf_vSbQHZc0h1SRxsp1mOf1FirZVXjASR021ao,8620
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/505.36ee543eaffaebaab59c.js,sha256=Nu5UPq_666q1nPVEKc-id0TMsWFDfqp3w7xojYWWCHw,2309
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/548.f4872310b34e6c6b2839.js,sha256=9IcjELNObGsoOZ05j97gelAa7eMRnRQH_C6fiziV-i0,28122
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/638.15eb86f53ace37ec5976.js,sha256=FeuG9TrON-xZdnI5cbcn_iJgmEi-XMCeKR1IJpMn5G8,205663
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js,sha256=dIVo2_yRcWKYw8-GwmNY-jsw90lpR6srl6bJHbMgFkE,36761
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/66.595d680d94ba923d3910.js.LICENSE.txt,sha256=eNJ8gc9n9IF8nW1d9sI9niuHstYzjNz5vqXx9UgWSPc,249
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/700.e7c4fbade0a06566f249.js,sha256=58T7reCgZWbySbyV_MHlvKi1DtR-n_c7pq_t-X8rK2c,4283
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/729.bc14cebf36af6ebe7071.js,sha256=vBTOvzavbr5wcWeHdxPLchR6hAbTEe_f0B5fIsxuPl8,12933
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js,sha256=lrRMCutxArB8O82gNTpG5SUjUhCMJGlZgUabupjaxU8,292756
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt,sha256=A-v1lwmuIX1DpNJ1MDzKDMWv7f_d6cjHlGOCEvthhdY,50
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js,sha256=JPBf2rR0jhZtMTJAKKDEtFx2dUjg4UkjS9K6QjyZK50,103503
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt,sha256=weTFhhgz7AMPWCChyr5kCa2PQKaGQbpqgkfcn-WNw7E,487
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/792.0955427b3d825d758aea.js,sha256=CVVCez2CXXWK6pDUnafBD01BfMgmZrLyE3eMbf0n5Gg,4474
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/799.e93d309a2347b726b4c9.js,sha256=6T0wmiNHtya0yRj7fFMvBT3z5B7M8kUQoFSgnIyQAJc,237708
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/823.87642002230f9f1eed39.js,sha256=h2QgAiMPnx7tOa0WITReViwRLp6IEfA4fH5KHrnK0xo,266482
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/85.4514c686223ec8054093.js,sha256=RRTGhiI-yAVAk2vziqnxwLO64p6X1RQpV4g4hXLj_Y0,58332
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/860.d9b9c7e6da98c3818e92.js,sha256=2bnH5tqYw4GOkmgVOREuJu7zut_l54oGstHwNJdGI8g,7725
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js,sha256=reDepbAyimKis4NMUqqriTsHuEaJ4lOm3DDtU4pkXrs,139404
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/891.dba4cf1876582ab44697.js.LICENSE.txt,sha256=0uKAUrni3KBhrQ_pfdSGdNaDuXB9yhSLQ73wG8hcXK4,132
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/remoteEntry.473afc439684735f2efc.js,sha256=Rzr8Q5aEc18u_NNlRg_YnKiLZEt_LmDVQhVGYz0kv2E,12103
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/style.js,sha256=NCOXHxa4RN4j6TNqwL1Tho42dFaFEng3VScxQRoDST4,185
+sagemaker_jupyterlab_extension-0.3.2.data/data/share/jupyter/labextensions/@amzn/sagemaker-jupyterlab-extensions/static/third-party-licenses.json,sha256=lPLAXxBmYR2EMC9_pN6eC-lJ9W7t2nEDslDxX-FZAIs,91011
+sagemaker_jupyterlab_extension-0.3.2.dist-info/LICENSE,sha256=ZWQ-fVLy0k5hdDLaputxwZyEfnfpvEx3ZImaRiZyuTA,4755
+sagemaker_jupyterlab_extension-0.3.2.dist-info/METADATA,sha256=byHosAyEBt-PJtLOBlL78LQuVzyK1HJ5AGLAJWcNuVw,2281
+sagemaker_jupyterlab_extension-0.3.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sagemaker_jupyterlab_extension-0.3.2.dist-info/top_level.txt,sha256=96mz5zVRnlKUFu46rV4QFpibtf4h9CD5HVkLxPBcah8,31
+sagemaker_jupyterlab_extension-0.3.2.dist-info/RECORD,,
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/__init__.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/_version.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/_version.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/handlers.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/package.json` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9661111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.473afc439684735f2efc.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -60,15 +60,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7282f69f1fc0d8e37b1c.js",
+            "load": "static/remoteEntry.473afc439684735f2efc.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/git:clone"
         ],
         "extension": true,
         "outputDir": "sagemaker_jupyterlab_extension/labextension",
@@ -105,9 +105,9 @@
         "test": "jest",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "style": "src/style/index.css",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [548], {
         4548: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => Xe
             });
-            var a = n(9557);
+            var a = n(797);
             const s = "@amzn/sagemaker-jupyterlab-extensions:gitclone",
                 i = "@amzn/sagemaker-jupyterlab-extensions:performance-metering",
                 o = "@amzn/sagemaker-jupyterlab-extensions:spacemenu",
                 r = {
                     shutdown: "filemenu:shutdown"
                 },
                 l = "Sso",
@@ -94,16 +94,16 @@
                         e.commands._commands.get(r.shutdown).isVisible = () => !1
                     }
                 };
             var w = n(9801),
                 b = n.n(w),
                 E = n(6029),
                 f = n.n(E),
-                x = n(8368),
-                S = n(9510);
+                x = n(4072),
+                S = n(1464);
             class C {
                 constructor() {
                     this._dismissTime = 0, this._count = 0
                 }
                 setDismissTime(e) {
                     e && (this._dismissTime = e, this._count = 1)
                 }
@@ -170,17 +170,17 @@
                     return {
                         sigInDialogResult: await i.launch(),
                         confirmDialog: i
                     }
                 };
             var N = n(6797),
                 B = n(6697),
-                I = n(1638),
-                z = n(7217),
-                A = n(5326);
+                I = n(2294),
+                z = n(2818),
+                A = n(2232);
             const U = (e, t, n, a, s, i, o) => {
                     const r = T(),
                         l = o(),
                         d = l && l + c;
                     if (null === r) j(e, !1);
                     else {
                         const o = b().unix(r / 1e3).diff(b()()),
@@ -290,17 +290,17 @@
                                 s.stop()
                             }), a, (e => {
                                 t = e
                             }), (() => t));
                         a()
                     }
                 };
-            var P = n(4613);
+            var P = n(7180);
             const G = [200, 201];
-            var $, O = n(6311);
+            var $, O = n(8671);
             ! function(e) {
                 e.POST = "POST", e.GET = "GET"
             }($ || ($ = {}));
             const F = async (e, t) => {
                 const n = z.ServerConnection.makeSettings(),
                     a = O.URLExt.join(n.baseUrl, e);
                 try {
@@ -518,15 +518,15 @@
                         item: n,
                         align: "left",
                         isActive: () => !0,
                         rank: 100
                     })
                 }
             };
-            var ue = n(8031),
+            var ue = n(9380),
                 pe = n(2715);
             const me = V.css`
   .MuiInputBase-input MuiInput-input {
     width: 400px;
     margin-bottom: 20px;
   }
 `,
@@ -725,15 +725,15 @@
                         gitRepositories: this._gitCloneRepositories,
                         setGitURL: this.setGitURL,
                         setPath: this.setPath,
                         setOpenREADME: this.setOpenREADME
                     })
                 }
             }
-            var Re = n(5962),
+            var Re = n(8937),
                 Te = n(2190);
             const {
                 name: je,
                 version: ke
             } = n(4147), De = (e, t, n) => e.child({
                 ExtensionName: je,
                 ExtensionVersion: ke,
@@ -777,15 +777,15 @@
                         return !1
                     }
                     return "directory" === n.type
                 };
             var ze = n(1775),
                 Ae = n(248),
                 Ue = n(4337),
-                Le = n(8625);
+                Le = n(9510);
             const {
                 dialogTitle: Pe,
                 cancelButton: Ge,
                 cloneButton: $e,
                 errors: Oe
             } = m.GitClone, Fe = {
                 id: s,
@@ -1010,15 +1010,15 @@
                     }), f().createElement("p", null, `${n&&n[1]||Ye} / ${t?e:Je}`))
                 };
             class Ke extends S.ReactWidget {
                 constructor() {
                     super(), this.getSpaceName = async () => {
                         await F("aws/sagemaker/api/context", $.GET).then((e => {
                             e && e.json().then((e => {
-                                this.spaceName = e ? null == e ? void 0 : e.SpaceName : null, this.update()
+                                this.spaceName = e ? null == e ? void 0 : e.spaceName : null, this.update()
                             }))
                         }))
                     }, this.spaceName = "", this.getSpaceName()
                 }
                 render() {
                     return f().createElement(Qe, {
                         spaceName: this.spaceName
@@ -1063,11 +1063,11 @@
                 i = n(5893),
                 o = (0, s.default)((0, i.jsx)("path", {
                     d: "M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zm6.93 6h-2.95c-.32-1.25-.78-2.45-1.38-3.56 1.84.63 3.37 1.91 4.33 3.56zM12 4.04c.83 1.2 1.48 2.53 1.91 3.96h-3.82c.43-1.43 1.08-2.76 1.91-3.96zM4.26 14C4.1 13.36 4 12.69 4 12s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H4.26zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56-1.84-.63-3.37-1.9-4.33-3.56zm2.95-8H5.08c.96-1.66 2.49-2.93 4.33-3.56C8.81 5.55 8.35 6.75 8.03 8zM12 19.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96zM14.34 14H9.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95c-.96 1.65-2.49 2.93-4.33 3.56zM16.36 14c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38z"
                 }), "Language");
             t.Z = o
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.1","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
+            e.exports = JSON.parse('{"name":"@amzn/sagemaker-jupyterlab-extensions","description":"SageMaker JupyterLab workspace primary extension module","version":"0.3.2","author":"Amazon","homepage":"https://aws.amazon.com/sagemaker/","license":"Amazon Software License","licenses":[{"type":"Amazon Software License","url":"http://aws.amazon.com/asl"}],"directories":{"test":"__tests__"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"scripts":{"build":"tsc","build:labextension":"tsc && jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True --source-map True .","lint:check":"eslint . --ext .js,.ts,.tsx","lint:fix":"eslint --fix . --ext .js,.ts,.tsx","release":"run-s build","install:extension":"jlpm run build","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch .","watch":"run-p watch:src watch:labextension","dev:setup":"run-s -n dev:docker:build dev:docker:reset dev:docker:create","dev:docker:build":"(cd devSetup ; sh pull-jupyterlab-base-image.sh && docker build . --tag jupyterlab_ext_dev_image --build-arg CONTAINER_USER_ID=$(id -u) --build-arg CONTAINER_GROUP_ID=$(id -g))","dev:docker:reset":"docker stop jupyterlab_ext_dev_container || true && docker rm jupyterlab_ext_dev_container || true","dev:docker:create":"docker create --name jupyterlab_ext_dev_container --publish 8888:8888 --volume $(pwd):/sagemaker-studio-extension jupyterlab_ext_dev_image","dev:start":"docker start jupyterlab_ext_dev_container --attach","test":"jest","test:watch":"jest --watch"},"main":"lib/index.js","dependencies":{"@amzn/sagemaker-jupyterlab-extension-common":"^0.1.2","@emotion/css":"^11.1.3","@emotion/styled":"^11.11.0","@jupyterlab/application":"^4.0.5","@jupyterlab/apputils":"^4.0.5","@jupyterlab/coreutils":"^6.0.5","@jupyterlab/docmanager":"^4.0.5","@jupyterlab/docregistry":"^4.0.5","@jupyterlab/filebrowser":"^4.0.5","@jupyterlab/git":"^0.50.0","@jupyterlab/mainmenu":"^4.0.5","@jupyterlab/services":"^7.0.0","@jupyterlab/statusbar":"^4.0.5","@jupyterlab/terminal":"^4.0.5","@jupyterlab/translation":"^4.0.5","@lumino/algorithm":"^2.0.0","@lumino/commands":"^2.0.0","@lumino/polling":"^2.1.2","@lumino/signaling":"^2.1.2","@lumino/widgets":"^2.0.0","@mui/icons-material":"5.14","@mui/material":"^5.14.4","@testing-library/react":"^13.0.0","isomorphic-fetch":"^3.0.0","moment":"^2.29.4","p-retry":"^5.1.2","react":"^18.2.0","react-dom":"^18.2.0","cookie":"0.6.0"},"jupyterlab":{"extension":true,"outputDir":"sagemaker_jupyterlab_extension/labextension","disabledExtensions":["@jupyterlab/git:clone"],"sharedPackages":{"@amzn/sagemaker-jupyterlab-extension-common":{"bundled":false,"singleton":true,"strictVersion":false}}},"style":"src/style/index.css","devDependencies":{"@babel/preset-env":"^7.22.7","@babel/preset-react":"^7.22.5","@jupyterlab/builder":"^4.0.5","@types/lodash":"^4.14.172","@types/react":"^18.2.21","@types/react-dom":"^18.2.7","@typescript-eslint/eslint-plugin":"^5.61.0","eslint-config-prettier":"^8.8.0","eslint-plugin-import":"^2.27.5","eslint-plugin-json":"^3.1.0","eslint-plugin-prettier":"^4.2.1","eslint-plugin-react":"^7.32.2","eslint-plugin-react-hooks":"^4.6.0","jest":"^27.2.4","npm-run-all":"^4.1.5","prettier":"^2.4.1","ts-jest":"^27.0.5","typescript":"^4.3.5"}}')
         }
     }
 ]);
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -14,18 +14,18 @@
                 nA: () => G,
                 ZM: () => Q,
                 cU: () => J,
                 ky: () => K,
                 fS: () => V,
                 no: () => Z
             });
-            var n = i(9510),
-                s = i(3471),
-                r = i(6311),
-                o = i(3452),
+            var n = i(1464),
+                s = i(7594),
+                r = i(8671),
+                o = i(6805),
                 a = i(6697),
                 l = i(7930),
                 c = i(4882),
                 h = i(6029),
                 d = i.n(h);
             class u extends Error {
                 constructor(...e) {
@@ -34,15 +34,15 @@
             }
             var f = i(4666),
                 p = i(1894),
                 g = i(9861),
                 m = i(3343),
                 _ = i(9405),
                 y = i(9946),
-                v = i(8625),
+                v = i(9510),
                 b = i(1618);
             const w = 27.5,
                 x = 200;
 
             function C(e) {
                 const [t, i] = d().useState(""), [n, s] = d().useState(null), r = e.branches.filter((e => !t || e.name.includes(t))), {
                     action: o,
@@ -1854,15 +1854,15 @@
         },
         4148: (e, t, i) => {
             "use strict";
             i.d(t, {
                 x: () => I,
                 m: () => O
             });
-            var n = i(9510),
+            var n = i(1464),
                 s = i(4882),
                 r = i(4901),
                 o = i(6029);
             let a;
             a = "undefined" != typeof window ? window : "undefined" != typeof self ? self : i.g;
             let l = null,
                 c = null;
@@ -2046,19 +2046,19 @@
                 _ = i(1083);
             const y = (0, i(9946).oB)({
                 flex: "1 1 auto",
                 minHeight: "150px",
                 overflow: "hidden",
                 overflowY: "auto"
             });
-            var v = i(8625),
+            var v = i(9510),
                 b = i(4337),
                 w = i(427),
                 x = i(1552),
-                C = i(3452),
+                C = i(6805),
                 k = i(9405),
                 E = i(2322);
             const S = e => {
                 const [t, i] = o.useState(!0), n = e.files.length;
                 return o.createElement("div", {
                     className: E.ny
                 }, o.createElement("div", {
@@ -2703,15 +2703,15 @@
             }
         },
         7320: (e, t, i) => {
             "use strict";
             i.d(t, {
                 y: () => a
             });
-            var n = i(3452),
+            var n = i(6805),
                 s = i(6029),
                 r = i(4387),
                 o = i(8211);
             const a = e => {
                 var t;
                 const i = (0, o.Qz)(e.filepath),
                     a = e.filepath.slice(0, e.filepath.length - i.length).replace(/^\/|\/$/g, ""),
@@ -2925,15 +2925,15 @@
             }
         },
         429: (e, t, i) => {
             "use strict";
             i.d(t, {
                 zx: () => C
             });
-            var n = i(9510),
+            var n = i(1464),
                 s = i(3343),
                 r = i(4666),
                 o = i(1894),
                 a = i(6029),
                 l = i(9946),
                 c = i(1618);
             const h = (0, l.oB)({
@@ -3180,17 +3180,17 @@
         },
         1709: (e, t, i) => {
             "use strict";
             i.d(t, {
                 W: () => f,
                 w: () => u
             });
-            var n = i(3471),
-                s = i(7777),
-                r = i(5962),
+            var n = i(7594),
+                s = i(8873),
+                r = i(8937),
                 o = i(7930),
                 a = i(4882),
                 l = i(2027),
                 c = i(1770),
                 h = i(3781),
                 d = i(8799);
             const u = async ({
@@ -3389,16 +3389,16 @@
         },
         1218: (e, t, i) => {
             "use strict";
             i.d(t, {
                 f: () => o,
                 q: () => a
             });
-            var n = i(6311),
-                s = i(7217),
+            var n = i(8671),
+                s = i(2818),
                 r = i(4337);
             const o = ["Invalid username or password", "could not read Username", "could not read Password", "Authentication error"];
             async function a(e = "", t = "GET", i = null, o = "git") {
                 const a = s.ServerConnection.makeSettings(),
                     l = n.URLExt.join(a.baseUrl, o, e),
                     c = {
                         method: t,
@@ -3433,16 +3433,16 @@
         },
         568: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Bj: () => m,
                 bI: () => g
             });
-            var n, s = i(6311),
-                r = i(1638),
+            var n, s = i(8671),
+                r = i(2294),
                 o = i(7930),
                 a = i(6797),
                 l = i(4901),
                 c = i(1218);
             class h {
                 constructor() {
                     this._first = null, this._last = null, this._size = 0
@@ -4420,15 +4420,15 @@
         },
         5350: (e, t, i) => {
             "use strict";
             i.d(t, {
                 d: () => r,
                 x: () => s
             });
-            var n = i(9510);
+            var n = i(1464);
 
             function s(e, t) {
                 return {
                     autoClose: !1,
                     actions: [{
                         label: t.__("Show"),
                         callback: () => {
@@ -4845,15 +4845,15 @@
                         },
                         "&:disabled:active": {
                             backgroundColor: "var(--jp-layout-color3)"
                         }
                     }
                 })
         },
-        8625: (e, t, i) => {
+        9510: (e, t, i) => {
             "use strict";
             i.d(t, {
                 Ug: () => r,
                 B3: () => o,
                 W6: () => a,
                 j0: () => l,
                 $N: () => c,
@@ -4870,15 +4870,15 @@
                 O4: () => v,
                 Ir: () => b,
                 W8: () => w,
                 V2: () => x,
                 yi: () => C,
                 Ds: () => k
             });
-            var n = i(3452);
+            var n = i(6805);
             const s = new n.LabIcon({
                     name: "git",
                     svgstr: '<svg\n  xmlns="http://www.w3.org/2000/svg"\n  viewBox="0 0 20 20"\n  width="16"\n>\n  <path\n    class="jp-icon3 jp-icon-selectable"\n    d="M19.6 9.1 10.9 0.4c-0.5-0.5-1.3-0.5-1.8 0l-1.8 1.8 2.3 2.3c0.5-0.2 1.1-0.1 1.6 0.4 0.4 0.4 0.5 1 0.4 1.6l2.2 2.2c0.5-0.2 1.2-0.1 1.6 0.4 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0C12.7 10.7 12.6 10.1 12.8 9.5l-2.1-2.1v5.4c0.1 0.1 0.3 0.2 0.4 0.3 0.6 0.6 0.6 1.6 0 2.2-0.6 0.6-1.6 0.6-2.2 0-0.6-0.6-0.6-1.6 0-2.2 0.1-0.1 0.3-0.3 0.5-0.3V7.4C9.3 7.3 9.1 7.2 9 7 8.5 6.6 8.4 5.9 8.6 5.3L6.4 3.1 0.4 9.1c-0.5 0.5-0.5 1.3 0 1.8l8.7 8.7c0.5 0.5 1.3 0.5 1.8 0l8.7-8.7c0.5-0.5 0.5-1.3 0-1.8"\n    fill="#616161"\n  />\n</svg>\n'
                 }),
                 r = new n.LabIcon({
                     name: "git:add",
                     svgstr: '<svg\n   xmlns="http://www.w3.org/2000/svg"\n   width="16"\n   viewBox="0 0 24 24"\n   version="1.1">\n  <g\n     class="jp-icon3 jp-icon-selectable"\n     fill="#4F4F4F">\n    <path\n       d="m 22,13 h -9 v 9 H 11 V 13 H 2 v -2 h 9 V 2 h 2 v 9 h 9 z"/>\n  </g>\n</svg>\n'
@@ -4964,15 +4964,15 @@
             "use strict";
             i.d(t, {
                 $R: () => o,
                 H_: () => r,
                 LC: () => s,
                 TQ: () => a
             });
-            var n = i(7217);
+            var n = i(2818);
             const s = new(i(7930).Token)("jupyter.extensions.git_plugin");
             var r, o, a;
             ! function(e) {
                 let t, i;
                 ! function(e) {
                     let t;
                     ! function(e) {
@@ -5016,15 +5016,15 @@
             i.d(t, {
                 LJ: () => a,
                 Qz: () => r,
                 XO: () => c,
                 _v: () => l,
                 hp: () => o
             });
-            var n = i(6311),
+            var n = i(8671),
                 s = i(4337);
 
             function r(e) {
                 return "/" === e[e.length - 1] ? e : n.PathExt.basename(e)
             }
 
             function o(e) {
@@ -5065,15 +5065,15 @@
             }
         },
         8858: (e, t, i) => {
             "use strict";
             i.d(t, {
                 t: () => s
             });
-            var n = i(9510);
+            var n = i(1464);
             async function s(e, t, i) {
                 if ((await (0, n.showDialog)({
                         title: t.__("Discard all changes"),
                         body: i ? t.__("Your current changes forbid pulling the latest changes. Do you want to permanently discard those changes? This action cannot be undone.") : t.__("Are you sure you want to permanently discard changes to all files? This action cannot be undone."),
                         buttons: [n.Dialog.cancelButton({
                             label: t.__("Cancel")
                         }), n.Dialog.warnButton({
@@ -5740,15 +5740,15 @@
                             return l(arguments, "callee").get
                         } catch (e) {
                             return c
                         }
                     }
                 }() : c,
                 d = i(1405)(),
-                u = i(3276)(),
+                u = i(8185)(),
                 f = Object.getPrototypeOf || (u ? function(e) {
                     return e.__proto__
                 } : null),
                 p = {},
                 g = "undefined" != typeof Uint8Array && f ? f(Uint8Array) : n,
                 m = {
                     "%AggregateError%": "undefined" == typeof AggregateError ? n : AggregateError,
@@ -5985,15 +5985,15 @@
                         value: 1
                     }).length
                 } catch (e) {
                     return !0
                 }
             }, e.exports = s
         },
-        3276: e => {
+        8185: e => {
             "use strict";
             var t = {
                     foo: {}
                 },
                 i = Object;
             e.exports = function() {
                 return {
@@ -6484,23 +6484,23 @@
             "use strict";
             i.d(t, {
                 QK: () => ne,
                 LI: () => Y
             });
             var n = i(8204),
                 s = i(6211),
-                r = i(5962),
+                r = i(8937),
                 o = i(4882),
                 a = i(9073),
                 l = i(8799),
                 c = i(4850),
                 h = i(1373),
                 d = i(8093),
-                u = i(3471),
-                f = i(7777);
+                u = i(7594),
+                f = i(8873);
             class p extends u.CodeEditorWrapper {
                 constructor(e) {
                     const {
                         factory: t,
                         value: i,
                         ...n
                     } = e, s = new d.YFile;
@@ -7761,15 +7761,15 @@
                 fy: () => b,
                 zr: () => d,
                 Jj: () => x,
                 Z: () => C,
                 tM: () => y,
                 CL: () => f
             });
-            var n = i(6963),
+            var n = i(3991),
                 s = i(1156),
                 r = i(4526),
                 o = i(7930),
                 a = i(8799),
                 l = i(4850),
                 c = i(1386);
             class h {
@@ -8590,15 +8590,15 @@
         },
         9073: (e, t, i) => {
             "use strict";
             i.d(t, {
                 M8: () => u,
                 AH: () => y
             });
-            var n = i(6963),
+            var n = i(3991),
                 s = i(4901),
                 r = i(4526),
                 o = i(3781),
                 a = i(1604),
                 l = i(1386),
                 c = i(8439),
                 h = i(4850),
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
-/*! For license information please see 891.4794a088a65e99550778.js.LICENSE.txt */
+/*! For license information please see 891.dba4cf1876582ab44697.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || []).push([
     [891], {
         4891: (e, t, s) => {
             s.r(t), s.d(t, {
                 DiffModel: () => Wr.j,
                 Git: () => _.H_,
                 IGitExtension: () => _.LC,
                 NotebookDiff: () => $t,
                 PlainTextDiff: () => Or.W,
                 default: () => Pr
             });
-            var i = s(8368),
-                r = s(9510),
-                a = s(3471),
-                o = s(5326),
-                n = s(8031),
-                l = s(9557),
-                d = s(8048),
-                c = s(4008),
-                h = s(4613),
-                p = s(5962),
+            var i = s(4072),
+                r = s(1464),
+                a = s(7594),
+                o = s(2232),
+                n = s(9380),
+                l = s(797),
+                d = s(3413),
+                c = s(5099),
+                h = s(7180),
+                p = s(8937),
                 m = s(6029),
                 u = s.n(m),
                 g = s(1775),
-                f = s(8625),
+                f = s(9510),
                 _ = s(4337),
                 b = s(4882);
             class v extends b.Widget {
                 constructor(e) {
                     super({
                         node: v.createFormNode(e)
                     })
@@ -1432,15 +1432,15 @@
                     return s
                 }
                 get model() {
                     return this._model
                 }
             }
             var st = s(9073),
-                it = s(6963),
+                it = s(3991),
                 rt = s(5359);
             const at = "jp-DropPanel",
                 ot = "jp-DragPanel",
                 nt = "jp-mod-dragHandle",
                 lt = "jp-mod-dropTarget",
                 dt = "application/vnd.jupyter.dragindex";
 
@@ -1698,15 +1698,15 @@
                     return null
                 }
                 validateSource(e) {
                     return this.acceptDropsFromExternalSource ? -1 !== this.friends.indexOf(e.source) : super.validateSource(e)
                 }
             }
             ft._counter = 0, ft._groups = {};
-            var _t = s(1778);
+            var _t = s(3195);
             class bt extends _t.OutputAreaModel {
                 insert(e, t) {
                     this.list.insert(e, t)
                 }
                 move(e, t) {
                     this.list.move(e, t)
                 }
@@ -2674,16 +2674,16 @@
                         return null === (t = null == e ? void 0 : e.composite.displayStatus) || void 0 === t || t
                     } : function() {
                         return !1
                     }
                 }
             }(ls || (ls = {}));
             var ps = s(568),
-                ms = s(6311),
-                us = s(7217);
+                ms = s(8671),
+                us = s(2818);
             var gs = s(7858),
                 fs = s(1083);
             const _s = (0, F.oB)({
                     display: "flex",
                     flexDirection: "column",
                     height: "100%",
                     overflowY: "auto"
@@ -2758,15 +2758,15 @@
                 getValue() {
                     return {
                         name: this._name.value,
                         email: this._email.value
                     }
                 }
             }
-            var Ss = s(3452),
+            var Ss = s(6805),
                 ks = s(7350),
                 js = s(9397),
                 Ds = s(9522),
                 Bs = s(3926),
                 Ns = s(6514),
                 Ts = s(3931),
                 Fs = s(2964),
@@ -5480,15 +5480,15 @@
                         filebrowser: this._fileBrowserModel,
                         model: this._model,
                         settings: this._settings,
                         trans: this._trans
                     })
                 }
             }
-            var Rr = s(7777),
+            var Rr = s(8873),
                 Wr = s(5658),
                 Or = s(1709);
             const Ir = {
                     id: "@jupyterlab/git:plugin",
                     requires: [i.ILayoutRestorer, Rr.IEditorLanguageRegistry, a.IEditorServices, n.IDefaultFileBrowser, d.IRenderMimeRegistry, c.ISettingRegistry, o.IDocumentManager],
                     optional: [l.IMainMenu, h.IStatusBar, r.ICommandPalette, p.ITranslator],
                     provides: _.LC,
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, l, i, d, u, f, c, s, b, p, m, h, v, g, y, j, w, P, k = {
-            3570: (e, r, t) => {
+            3173: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
-                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(853), t.e(548)]).then((() => () => t(4548))),
+                        "./index": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(337), t.e(548)]).then((() => () => t(4548))),
+                        "./extension": () => Promise.all([t.e(729), t.e(66), t.e(766), t.e(181), t.e(823), t.e(29), t.e(800), t.e(704), t.e(337), t.e(548)]).then((() => () => t(4548))),
                         "./style": () => t.e(792).then((() => () => t(4792)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -51,58 +51,58 @@
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
         181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
+        337: "da58975bf5e0af92782f",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "a6ac1d0d39311897c48d",
-        571: "8dccdf5de15d462291c1",
+        548: "f4872310b34e6c6b2839",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
+        730: "9f65e223c4a041d10b21",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
         799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "26c15aab8d5d7301c11a",
-        853: "ced0d3671ec7406522f7",
+        823: "87642002230f9f1eed39",
         860: "d9b9c7e6da98c3818e92",
-        891: "4794a088a65e99550778"
+        891: "dba4cf1876582ab44697"
     } [e] + ".js?v=" + {
         10: "c2420c83a55ee1ffecfe",
         29: "f2e584ec0be118d7b54c",
         66: "595d680d94ba923d3910",
         85: "4514c686223ec8054093",
         181: "9a0cdfa414e5cba3947c",
         222: "587a32e1b3cb7433cc73",
         242: "13e5d4563ddb8069ebd5",
+        337: "da58975bf5e0af92782f",
         378: "ddf9e5d607ffbd26d01d",
         505: "36ee543eaffaebaab59c",
-        548: "a6ac1d0d39311897c48d",
-        571: "8dccdf5de15d462291c1",
+        548: "f4872310b34e6c6b2839",
         638: "15eb86f53ace37ec5976",
         700: "e7c4fbade0a06566f249",
         704: "5cfc0421a535f6454049",
         729: "bc14cebf36af6ebe7071",
+        730: "9f65e223c4a041d10b21",
         762: "04ff1166c1cadfd1dda1",
         766: "ae47c4f1494b6a6ea83c",
         792: "0955427b3d825d758aea",
         798: "e5ba8c34b3ad08f57ff2",
         799: "e93d309a2347b726b4c9",
         800: "61e818e75a1cec06f3f1",
-        823: "26c15aab8d5d7301c11a",
-        853: "ced0d3671ec7406522f7",
+        823: "87642002230f9f1eed39",
         860: "d9b9c7e6da98c3818e92",
-        891: "4794a088a65e99550778"
+        891: "dba4cf1876582ab44697"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -154,15 +154,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.1", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(853), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(853), S.e(571)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@amzn/sagemaker-jupyterlab-extensions", "0.3.2", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(823), S.e(29), S.e(800), S.e(704), S.e(337), S.e(548)]).then((() => () => S(4548))))), i("@emotion/css", "11.11.2", (() => Promise.all([S.e(729), S.e(505)]).then((() => () => S(3505))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(729), S.e(29), S.e(378)]).then((() => () => S(4378))))), i("@jupyterlab/git", "0.50.0", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(85), S.e(823), S.e(891), S.e(29), S.e(800), S.e(704), S.e(337), S.e(730)]).then((() => () => S(4891))))), i("@mui/icons-material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(242), S.e(29), S.e(800)]).then((() => () => S(4242))))), i("@mui/material", "5.14.7", (() => Promise.all([S.e(729), S.e(66), S.e(766), S.e(181), S.e(85), S.e(799), S.e(29), S.e(800), S.e(704)]).then((() => () => S(7799))))), i("moment", "2.29.4", (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -273,59 +273,59 @@
     })(((e, r, t, a) => (l(e, t), m(c(r, t, a) || p(r, e, t, a) || i(r, t))))), g = h(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), y = h(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && c(r, t, a);
         return o ? m(o) : n()
     })), j = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
         8800: () => y("default", "@emotion/styled", [1, 11, 3, 0], (() => S.e(860).then((() => () => S(4378))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
+        797: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
         1373: () => g("default", "@codemirror/language", [1, 6, 0, 0]),
-        1638: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
-        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
-        4613: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
+        1464: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        2232: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 6]),
+        2294: () => v("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
+        2818: () => g("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        3991: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 6]),
+        4072: () => g("default", "@jupyterlab/application", [1, 4, 1, 6]),
         4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
-        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
         6211: () => g("default", "@codemirror/view", [1, 6, 9, 6]),
-        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         6697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         6797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
-        6963: () => v("default", "@jupyterlab/nbformat", [1, 4, 1, 5]),
-        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
-        7777: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 5]),
+        6805: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        7180: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 6]),
+        7594: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 6]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        8031: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8204: () => g("default", "@codemirror/state", [1, 6, 2, 0]),
-        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
-        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
+        8671: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        8873: () => g("default", "@jupyterlab/codemirror", [1, 4, 1, 6]),
+        8937: () => g("default", "@jupyterlab/translation", [1, 4, 1, 6]),
+        9380: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
         248: () => g("default", "@amzn/sagemaker-jupyterlab-extension-common", [2, 0, 1, 2]),
-        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(571)]).then((() => () => S(4891))))),
+        2190: () => y("default", "@jupyterlab/git", [2, 0, 50, 0], (() => Promise.all([S.e(85), S.e(891), S.e(730)]).then((() => () => S(4891))))),
         5933: () => y("default", "@emotion/css", [1, 11, 1, 3], (() => S.e(222).then((() => () => S(3505))))),
         9801: () => y("default", "moment", [1, 2, 29, 4], (() => Promise.all([S.e(762), S.e(700)]).then((() => () => S(381))))),
-        1778: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
-        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
+        3195: () => v("default", "@jupyterlab/outputarea", [1, 4, 1, 6]),
+        3413: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        5099: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
         5359: () => g("default", "@lumino/dragdrop", [1, 2, 0, 0]),
         5633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         7350: () => g("default", "@lumino/commands", [1, 2, 0, 1]),
         7489: () => y("default", "@mui/material", [1, 5, 12, 1], (() => Promise.all([S.e(181), S.e(799)]).then((() => () => S(7799))))),
         7858: () => y("default", "@mui/icons-material", [1, 5, 11, 16], (() => S.e(242).then((() => () => S(4242))))),
-        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         851: () => g("default", "@lezer/common", [1, 1, 0, 0]),
         7138: () => g("default", "@lezer/highlight", [1, 1, 0, 0])
     }, P = {
         29: [6029],
+        337: [797, 1373, 1464, 2232, 2294, 2818, 3991, 4072, 4882, 4901, 6211, 6697, 6797, 6805, 7180, 7594, 7930, 8093, 8204, 8671, 8873, 8937, 9380],
         548: [248, 2190, 5933, 9801],
-        571: [1778, 4008, 5359, 5633, 7350, 7489, 7858, 8048],
         704: [7704],
+        730: [3195, 3413, 5099, 5359, 5633, 7350, 7489, 7858],
         798: [851, 7138],
-        800: [8800],
-        853: [1373, 1638, 3452, 3471, 4613, 4882, 4901, 5326, 5962, 6211, 6311, 6697, 6797, 6963, 7217, 7777, 7930, 8031, 8093, 8204, 8368, 9510, 9557]
+        800: [8800]
     }, S.f.consumes = (e, r) => {
         S.o(P, e) && P[e].forEach((e => {
             if (S.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -346,15 +346,15 @@
         var e = {
             584: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(29|571|704|798|800|853)$/.test(r)) e[r] = 0;
+                else if (/^(7(04|30|98)|29|337|800)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = S.p + S.u(r),
                     l = new Error;
                 S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -373,10 +373,10 @@
                     i && i(S)
                 }
                 for (r && r(t); d < o.length; d++) n = o[d], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions = self.webpackChunk_amzn_sagemaker_jupyterlab_extensions || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(3570);
+    var E = S(3173);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyterlab-extensions"] = E
 })();
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_error_util.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_git_clone_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_handlers.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/tests/test_request_logger.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/tests/test_request_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     assert (
         data["UriPath"] == "/jupyterlab/default/aws/sagemaker/api/git/list-repositories"
     )
     assert data["ResponseLatencyMS"] == 0.1
     assert (
         data["Context"]["ExtensionName"] == "SagemakerStudioJuypterLabExtensionCommon"
     )
-    assert data["Context"]["ExtensionVersion"] == "0.3.1"
+    assert data["Context"]["ExtensionVersion"] == "0.3.2"
     assert data["Context"]["AccountId"] == "1234567890"
     assert data["Context"]["DomainId"] == "d-jk12345678"
     assert data["Context"]["SpaceName"] == "default-space"
     data["_aws"]["Timestamp"] = 123456
 
     assert data["_aws"] == {
         "CloudWatchMetrics": [
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/error_util.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/error_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/git_clone_util.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/git_clone_util.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension/utils/request_logger.py` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension/utils/request_logger.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/PKG-INFO` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-jupyterlab-extension
-Version: 0.3.1
+Version: 0.3.2
 Summary: SageMaker JupyterLab workspace primary extension module
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Amazon Software License
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt` & `sagemaker_jupyterlab_extension-0.3.2/sagemaker_jupyterlab_extension.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 THIRD-PARTY-LICENSES
 install.json
 package.json
 pyproject.toml
 setup.py
 tsconfig.json
 jupyter-config/jupyter_server_config.d/sagemaker_jupyterlab_extension.json
-public_dist/sagemaker_jupyterlab_extension-0.3.1-py3-none-any.whl
+public_dist/sagemaker_jupyterlab_extension-0.3.2-py3-none-any.whl
 sagemaker_jupyterlab_extension/__init__.py
 sagemaker_jupyterlab_extension/_version.py
 sagemaker_jupyterlab_extension/handlers.py
 sagemaker_jupyterlab_extension.egg-info/PKG-INFO
 sagemaker_jupyterlab_extension.egg-info/SOURCES.txt
 sagemaker_jupyterlab_extension.egg-info/dependency_links.txt
 sagemaker_jupyterlab_extension.egg-info/not-zip-safe
@@ -21,32 +21,32 @@
 sagemaker_jupyterlab_extension/labextension/package.json
 sagemaker_jupyterlab_extension/labextension/static/10.c2420c83a55ee1ffecfe.js
 sagemaker_jupyterlab_extension/labextension/static/181.9a0cdfa414e5cba3947c.js
 sagemaker_jupyterlab_extension/labextension/static/222.587a32e1b3cb7433cc73.js
 sagemaker_jupyterlab_extension/labextension/static/242.13e5d4563ddb8069ebd5.js
 sagemaker_jupyterlab_extension/labextension/static/378.ddf9e5d607ffbd26d01d.js
 sagemaker_jupyterlab_extension/labextension/static/505.36ee543eaffaebaab59c.js
-sagemaker_jupyterlab_extension/labextension/static/548.a6ac1d0d39311897c48d.js
+sagemaker_jupyterlab_extension/labextension/static/548.f4872310b34e6c6b2839.js
 sagemaker_jupyterlab_extension/labextension/static/638.15eb86f53ace37ec5976.js
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js
 sagemaker_jupyterlab_extension/labextension/static/66.595d680d94ba923d3910.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/700.e7c4fbade0a06566f249.js
 sagemaker_jupyterlab_extension/labextension/static/729.bc14cebf36af6ebe7071.js
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js
 sagemaker_jupyterlab_extension/labextension/static/762.04ff1166c1cadfd1dda1.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js
 sagemaker_jupyterlab_extension/labextension/static/766.ae47c4f1494b6a6ea83c.js.LICENSE.txt
 sagemaker_jupyterlab_extension/labextension/static/792.0955427b3d825d758aea.js
 sagemaker_jupyterlab_extension/labextension/static/799.e93d309a2347b726b4c9.js
-sagemaker_jupyterlab_extension/labextension/static/823.26c15aab8d5d7301c11a.js
+sagemaker_jupyterlab_extension/labextension/static/823.87642002230f9f1eed39.js
 sagemaker_jupyterlab_extension/labextension/static/85.4514c686223ec8054093.js
 sagemaker_jupyterlab_extension/labextension/static/860.d9b9c7e6da98c3818e92.js
-sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js
-sagemaker_jupyterlab_extension/labextension/static/891.4794a088a65e99550778.js.LICENSE.txt
-sagemaker_jupyterlab_extension/labextension/static/remoteEntry.7282f69f1fc0d8e37b1c.js
+sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js
+sagemaker_jupyterlab_extension/labextension/static/891.dba4cf1876582ab44697.js.LICENSE.txt
+sagemaker_jupyterlab_extension/labextension/static/remoteEntry.473afc439684735f2efc.js
 sagemaker_jupyterlab_extension/labextension/static/style.js
 sagemaker_jupyterlab_extension/labextension/static/third-party-licenses.json
 sagemaker_jupyterlab_extension/tests/__init__.py
 sagemaker_jupyterlab_extension/tests/helper.py
 sagemaker_jupyterlab_extension/tests/test_error_util.py
 sagemaker_jupyterlab_extension/tests/test_git_clone_util.py
 sagemaker_jupyterlab_extension/tests/test_handlers.py
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/setup.py` & `sagemaker_jupyterlab_extension-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/GitCloneComponent.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/GitCloneComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/ResourceUsageComponent.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/ResourceUsageComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/SpaceMenu.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/SpaceMenu.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/AutoComplete.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/AutoComplete.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/CheckboxComponent.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/CheckboxComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/GitCloneComponent.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/GitCloneComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/InputField.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/InputField.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/LinearProgressWithLabel.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/LinearProgressWithLabel.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/ResourceUsageComponent.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/ResourceUsageComponent.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/__tests__/SpaceMenu.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/__tests__/SpaceMenu.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/common/AutoComplete.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/common/AutoComplete.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/common/CheckboxComponent.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/common/CheckboxComponent.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/common/InputField.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/common/InputField.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/common/LinearProgressWithLabel.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/components/common/LinearProgressWithLabel.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/components/styles/InputFieldStyles.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/components/styles/InputFieldStyles.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/constants/common.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/constants/common.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/constants/il18Strings.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/constants/il18Strings.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/constants/resourceUsageConstants.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/constants/resourceUsageConstants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/constants/sessionManagementConstants.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/constants/sessionManagementConstants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/GitClonePlugin.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/GitClonePlugin.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/HideShutDownPlugin.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/HideShutDownPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/PerformancePlugin/PerformanceMeteringPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/PerformancePlugin/utils.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/PerformancePlugin/utils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/ResourceUsagePlugin.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/ResourceUsagePlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/SessionManagementPlugin.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/SessionManagementPlugin.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/SpaceMenuPlugin.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/SpaceMenuPlugin.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/GitClonePlugin.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/GitClonePlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/HideShutDownPlugin.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/HideShutDownPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/ResourceUsagePlugin.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/ResourceUsagePlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SessionManagementPlugin.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/SessionManagementPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/plugins/__tests__/SpaceMenuPlugin.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/plugins/__tests__/SpaceMenuPlugin.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/index.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/service/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/service/__tests__/mock.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/service/__tests__/mock.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/service/constants.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/service/constants.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/service/index.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/service/index.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/utils/ReactWidgetWrapper.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/utils/ReactWidgetWrapper.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/gitCloneUtils.spec.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/utils/__tests__/gitCloneUtils.spec.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/utils/__tests__/sessionManagerUtils.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/utils/__tests__/sessionManagerUtils.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/utils/gitCloneUtils.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/utils/gitCloneUtils.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/utils/logger.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/utils/logger.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/utils/sessionManagerUtils.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/utils/sessionManagerUtils.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/widgets/GitCloneWidget.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/widgets/GitCloneWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/widgets/ResourceUsageWidget.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/widgets/ResourceUsageWidget.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/widgets/SpaceMenuWidget.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/widgets/SpaceMenuWidget.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     this.getSpaceName();
   }
 
   getSpaceName = async () => {
     await fetchApiResponse(SAGEMAKER_CONTEXT_URL, OPTIONS_TYPE.GET).then((result: any) => {
       result &&
         result.json().then((data: any) => {
-          this.spaceName = data ? data?.SpaceName : null;
+          this.spaceName = data ? data?.spaceName : null;
           this.update();
         });
     });
   };
 
   render() {
     return <SpaceMenu spaceName={this.spaceName} />;
```

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/GitCloneWidget.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/widgets/__tests__/GitCloneWidget.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/widgets/__tests__/ResourceUsageWidget.spec.tsx` & `sagemaker_jupyterlab_extension-0.3.2/src/widgets/__tests__/ResourceUsageWidget.spec.tsx`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/src/widgets/styles/resourceUsageStyle.ts` & `sagemaker_jupyterlab_extension-0.3.2/src/widgets/styles/resourceUsageStyle.ts`

 * *Files identical despite different names*

### Comparing `sagemaker-jupyterlab-extension-0.3.1/tsconfig.json` & `sagemaker_jupyterlab_extension-0.3.2/tsconfig.json`

 * *Files identical despite different names*

