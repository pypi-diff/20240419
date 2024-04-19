# Comparing `tmp/nrtk_explorer-0.0.3.tar.gz` & `tmp/nrtk_explorer-0.0.4.tar.gz`

## Comparing `nrtk_explorer-0.0.3.tar` & `nrtk_explorer-0.0.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.codespellrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.flake8
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    19597 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/screenshot.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.github/workflows/create_release.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/desktop/README.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/desktop/create_exe.bat
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/desktop/create_linux.sh
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/desktop/create_mac.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/desktop/requirements.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/desktop/run.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/DEPLOY.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/Dockerfile
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/captain-definition
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/scripts/build_image.sh
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/scripts/build_server.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/scripts/run_image.sh
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/scripts/run_server.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/setup/apps.yml
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/setup/initialize.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/bundles/docker/setup/requirements.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/examples/jupyter/show.ipynb
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/applet.py
--rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/core.py
--rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/embeddings.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/filtering.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/jupyter.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/main.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/parameters.py
--rw-r--r--   0        0        0    16454 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/ui/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/ui/collapsible_card.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/ui/image_list.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/app/ui/result_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/dataset.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/dimension_reducers.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/embeddings_extractor.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/filtering.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/images_manager.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/ml_models.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/nrtk_transforms.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/object_detector.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/transforms.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/assets/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/library/assets/imagenet_classes.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/module/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/module/__init__.py
--rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/module/serve/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/__init__.py
--rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
--rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
--rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
--rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
--rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
--rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
--rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
--rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
--rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
--rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
--rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
--rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
--rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
--rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
--rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
--rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
--rw-r--r--   0        0        0  3685868 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/widgets/__init__.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/src/nrtk_explorer/widgets/nrtk_explorer.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/tests/requirements.txt
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/tests/test_embeddings.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/tests/test_filtering.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/tests/test_import.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/tests/test_object_detector.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/.editorconfig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/.eslintrc.cjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/.prettierrc.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/env.d.ts
--rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/package-lock.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/tsconfig.app.json
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/tsconfig.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/tsconfig.node.json
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/vite.config.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/public/styles.css
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/main.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/FilterOperatorWidget.vue
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/FilterOptionsWidget.vue
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/ImageDetection.vue
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/ParamWidget.vue
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/ParamsWidget.vue
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/ScatterPlot.vue
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/components/index.js
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/types/index.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/vue-components/src/utilities/colors.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/LICENSE
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/hatch_build.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.codespellrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.flake8
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/MANIFEST.in
+-rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/screenshot.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.github/workflows/create_release.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/desktop/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/desktop/create_exe.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/desktop/create_linux.sh
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/desktop/create_mac.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/desktop/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/desktop/run.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/DEPLOY.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/Dockerfile
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/captain-definition
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/scripts/build_image.sh
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/scripts/build_server.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/scripts/run_image.sh
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/scripts/run_server.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/setup/apps.yml
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/setup/initialize.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/bundles/docker/setup/requirements.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/examples/jupyter/show.ipynb
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/applet.py
+-rw-r--r--   0        0        0    15228 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/core.py
+-rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/embeddings.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/filtering.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/jupyter.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/main.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/parameters.py
+-rw-r--r--   0        0        0    16454 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/ui/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/ui/collapsible_card.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/ui/image_list.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/app/ui/result_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/dataset.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/dimension_reducers.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/embeddings_extractor.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/filtering.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/images_manager.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/ml_models.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/nrtk_transforms.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/object_detector.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/transforms.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/assets/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/library/assets/imagenet_classes.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/module/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/module/__init__.py
+-rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/module/serve/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/__init__.py
+-rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
+-rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
+-rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
+-rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
+-rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
+-rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
+-rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
+-rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
+-rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
+-rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
+-rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
+-rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
+-rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
+-rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
+-rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
+-rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
+-rw-r--r--   0        0        0  3685868 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/widgets/__init__.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/src/nrtk_explorer/widgets/nrtk_explorer.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/tests/requirements.txt
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/tests/test_embeddings.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/tests/test_filtering.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/tests/test_import.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/tests/test_object_detector.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/.editorconfig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/.eslintrc.cjs
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/.prettierrc.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/env.d.ts
+-rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/package-lock.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/tsconfig.app.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/tsconfig.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/tsconfig.node.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/vite.config.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/public/styles.css
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/main.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/FilterOperatorWidget.vue
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/FilterOptionsWidget.vue
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/ImageDetection.vue
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/ParamWidget.vue
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/ParamsWidget.vue
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/ScatterPlot.vue
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/components/index.js
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/types/index.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/vue-components/src/utilities/colors.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/hatch_build.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 nrtk_explorer-0.0.4/PKG-INFO
```

### Comparing `nrtk_explorer-0.0.3/CHANGELOG.md` & `nrtk_explorer-0.0.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.0.4 (2024-04-19)
+
+### Fix
+
+* fix(nrtk-explorer): fix image in readme ([`80850aa`](https://github.com/Kitware/nrtk-explorer/commit/80850aa0ad37343ca6b0a2c0961c54d92ba23a81))
+
+
 ## v0.0.3 (2024-04-18)
 
 ### Fix
 
 * fix(nrtk-explorer): removed large tests datasets ([`b219a75`](https://github.com/Kitware/nrtk-explorer/commit/b219a75402fcbd534e881fa66732a204817a534a))
```

### Comparing `nrtk_explorer-0.0.3/CONTRIBUTING.rst` & `nrtk_explorer-0.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/screenshot.png` & `nrtk_explorer-0.0.4/screenshot.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/.github/workflows/ci.yml` & `nrtk_explorer-0.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/.github/workflows/create_release.yaml` & `nrtk_explorer-0.0.4/.github/workflows/create_release.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -87,13 +87,13 @@
           github_token: ${{ secrets.GITHUB_TOKEN }}
           tag: ${{ steps.release.outputs.tag }}
 
       - name: Merge release back to main
         run: |
           git config user.email "actions@github.com"
           git config user.name "github-actions"
-
+          chown -R "${USER:-$(id -un)}" .
           git fetch
           git checkout main
           git pull
           git merge --no-ff release -m "Auto-merge release back to main"
           git push
```

### Comparing `nrtk_explorer-0.0.3/bundles/desktop/README.md` & `nrtk_explorer-0.0.4/bundles/desktop/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/bundles/docker/DEPLOY.md` & `nrtk_explorer-0.0.4/bundles/docker/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/bundles/docker/README.md` & `nrtk_explorer-0.0.4/bundles/docker/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/examples/jupyter/show.ipynb` & `nrtk_explorer-0.0.4/examples/jupyter/show.ipynb`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/core.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/core.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/embeddings.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/filtering.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/jupyter.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/parameters.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/parameters.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/transforms.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/ui/collapsible_card.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/ui/collapsible_card.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/app/ui/image_list.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/app/ui/image_list.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/dimension_reducers.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/dimension_reducers.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/embeddings_extractor.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/embeddings_extractor.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/filtering.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/images_manager.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/images_manager.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/ml_models.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/ml_models.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/nrtk_transforms.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/nrtk_transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/object_detector.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/transforms.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/library/assets/imagenet_classes.txt` & `nrtk_explorer-0.0.4/src/nrtk_explorer/library/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js` & `nrtk_explorer-0.0.4/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json` & `nrtk_explorer-0.0.4/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/src/nrtk_explorer/widgets/nrtk_explorer.py` & `nrtk_explorer-0.0.4/src/nrtk_explorer/widgets/nrtk_explorer.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/tests/conftest.py` & `nrtk_explorer-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/tests/test_embeddings.py` & `nrtk_explorer-0.0.4/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/tests/test_filtering.py` & `nrtk_explorer-0.0.4/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/tests/test_object_detector.py` & `nrtk_explorer-0.0.4/tests/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/package-lock.json` & `nrtk_explorer-0.0.4/vue-components/package-lock.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/package.json` & `nrtk_explorer-0.0.4/vue-components/package.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/vite.config.ts` & `nrtk_explorer-0.0.4/vue-components/vite.config.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/components/FilterOperatorWidget.vue` & `nrtk_explorer-0.0.4/vue-components/src/components/FilterOperatorWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/components/FilterOptionsWidget.vue` & `nrtk_explorer-0.0.4/vue-components/src/components/FilterOptionsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/components/ImageDetection.vue` & `nrtk_explorer-0.0.4/vue-components/src/components/ImageDetection.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/components/ParamWidget.vue` & `nrtk_explorer-0.0.4/vue-components/src/components/ParamWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/components/ParamsWidget.vue` & `nrtk_explorer-0.0.4/vue-components/src/components/ParamsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/components/ScatterPlot.vue` & `nrtk_explorer-0.0.4/vue-components/src/components/ScatterPlot.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/types/index.ts` & `nrtk_explorer-0.0.4/vue-components/src/types/index.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/vue-components/src/utilities/colors.ts` & `nrtk_explorer-0.0.4/vue-components/src/utilities/colors.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/LICENSE` & `nrtk_explorer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/README.md` & `nrtk_explorer-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 =============
 
 NRTK Explorer is a web application for exploring image datasets. It provides
 insights of a image dataset in [COCO][3] format and it evaluate image
 transformation and perturbation resilience of object recognition DL models. It
 is built using [trame][1] by the [kitware][2] team.
 
-![nrtk explorer](screenshot.png)
+![nrtk explorer](https://github.com/Kitware/nrtk-explorer/blob/d3df0ecf748664d806f09ad11e2bbd71a0bca1dd/screenshot.png?raw=true)
 
 Features
 --------
 
 - Explore image datasets in COCO format.
 - Apply parametrized image degradation (such as blur) to the images.
 - Benchmark dataset resilience with a differential PCA|UMAP analysis of the
```

### Comparing `nrtk_explorer-0.0.3/hatch_build.py` & `nrtk_explorer-0.0.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.0.3/pyproject.toml` & `nrtk_explorer-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nrtk-explorer"
-version="0.0.3"
+version="0.0.4"
 description="Model Visualizer"
 authors = [
   {name = "Alessandro Genova", email = "alessandro.genova@kitware.com"},
   {name = "Vicente Adolfo Bolea Sanchez", email = "vicente.bolea@kitware.com"},
 ]
 readme = "README.md"
 keywords = [
```

### Comparing `nrtk_explorer-0.0.3/PKG-INFO` & `nrtk_explorer-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nrtk-explorer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Model Visualizer
 Author-email: Alessandro Genova <alessandro.genova@kitware.com>, Vicente Adolfo Bolea Sanchez <vicente.bolea@kitware.com>
 License-File: LICENSE
 Keywords: Application,Framework,Interactive,Python,Web
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: Other/Proprietary License
@@ -53,15 +53,15 @@
 =============
 
 NRTK Explorer is a web application for exploring image datasets. It provides
 insights of a image dataset in [COCO][3] format and it evaluate image
 transformation and perturbation resilience of object recognition DL models. It
 is built using [trame][1] by the [kitware][2] team.
 
-![nrtk explorer](screenshot.png)
+![nrtk explorer](https://github.com/Kitware/nrtk-explorer/blob/d3df0ecf748664d806f09ad11e2bbd71a0bca1dd/screenshot.png?raw=true)
 
 Features
 --------
 
 - Explore image datasets in COCO format.
 - Apply parametrized image degradation (such as blur) to the images.
 - Benchmark dataset resilience with a differential PCA|UMAP analysis of the
```

