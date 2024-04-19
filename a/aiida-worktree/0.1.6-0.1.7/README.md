# Comparing `tmp/aiida_worktree-0.1.6.tar.gz` & `tmp/aiida_worktree-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_worktree-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_worktree-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_worktree-0.1.6.tar` & `aiida_worktree-0.1.7.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/LICENSE
--rw-r--r--   0        0        0     4954 2024-04-17 15:17:33.932303 aiida_worktree-0.1.6/README.md
--rw-r--r--   0        0        0      172 2024-04-18 08:27:39.451960 aiida_worktree-0.1.6/aiida_worktree/__init__.py
--rw-r--r--   0        0        0      275 2023-12-13 16:41:17.047695 aiida_worktree-0.1.6/aiida_worktree/cli/__init__.py
--rw-r--r--   0        0        0    12079 2023-12-13 16:41:17.047695 aiida_worktree-0.1.6/aiida_worktree/cli/cmd_tree.py
--rw-r--r--   0        0        0     1932 2023-12-13 16:41:17.047695 aiida_worktree-0.1.6/aiida_worktree/cli/cmd_web.py
--rw-r--r--   0        0        0      700 2023-12-13 16:41:17.047695 aiida_worktree-0.1.6/aiida_worktree/cli/cmd_worktree.py
--rw-r--r--   0        0        0     6581 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/cli/query_worktree.py
--rw-r--r--   0        0        0    11369 2024-04-17 05:39:00.099765 aiida_worktree-0.1.6/aiida_worktree/decorator.py
--rw-r--r--   0        0        0        0 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/engine/__init__.py
--rw-r--r--   0        0        0    44165 2024-04-17 05:39:00.099765 aiida_worktree-0.1.6/aiida_worktree/engine/worktree.py
--rw-r--r--   0        0        0        0 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/executors/__init__.py
--rw-r--r--   0        0        0     1098 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/executors/builtin.py
--rw-r--r--   0        0        0      634 2024-04-13 03:14:32.498807 aiida_worktree-0.1.6/aiida_worktree/executors/qe.py
--rw-r--r--   0        0        0      439 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/executors/test.py
--rw-r--r--   0        0        0     2609 2024-04-18 08:20:20.592868 aiida_worktree-0.1.6/aiida_worktree/node.py
--rw-r--r--   0        0        0      936 2024-02-12 16:38:13.895317 aiida_worktree-0.1.6/aiida_worktree/nodes/__init__.py
--rw-r--r--   0        0        0     3868 2024-02-12 16:38:13.895317 aiida_worktree-0.1.6/aiida_worktree/nodes/builtin.py
--rw-r--r--   0        0        0     4838 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/nodes/qe.py
--rw-r--r--   0        0        0     6562 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/nodes/test.py
--rw-r--r--   0        0        0     1202 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/orm/worktree.py
--rw-r--r--   0        0        0      114 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/properties/__init__.py
--rw-r--r--   0        0        0     8432 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/properties/built_in.py
--rw-r--r--   0        0        0      586 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/property.py
--rw-r--r--   0        0        0      353 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/socket.py
--rw-r--r--   0        0        0      110 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/sockets/__init__.py
--rw-r--r--   0        0        0     2852 2023-12-11 16:36:18.395013 aiida_worktree-0.1.6/aiida_worktree/sockets/built_in.py
--rw-r--r--   0        0        0     7254 2024-04-16 12:22:57.721423 aiida_worktree-0.1.6/aiida_worktree/utils/__init__.py
--rw-r--r--   0        0        0     5713 2024-04-13 03:14:32.498807 aiida_worktree-0.1.6/aiida_worktree/utils/analysis.py
--rw-r--r--   0        0        0     1677 2024-04-18 06:44:50.292276 aiida_worktree-0.1.6/aiida_worktree/utils/tree.py
--rw-r--r--   0        0        0      763 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/README.md
--rw-r--r--   0        0        0        0 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/backend/app/__init__.py
--rw-r--r--   0        0        0     2388 2024-02-12 17:45:35.080641 aiida_worktree-0.1.6/aiida_worktree/web/backend/app/api.py
--rw-r--r--   0        0        0     3638 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/backend/app/daemon.py
--rw-r--r--   0        0        0     2112 2024-02-12 17:45:35.080641 aiida_worktree-0.1.6/aiida_worktree/web/backend/app/datanode.py
--rw-r--r--   0        0        0     5938 2024-04-17 08:01:13.585776 aiida_worktree-0.1.6/aiida_worktree/web/backend/app/utils.py
--rw-r--r--   0        0        0     5087 2024-01-14 22:48:05.651634 aiida_worktree-0.1.6/aiida_worktree/web/backend/app/worktree.py
--rw-r--r--   0        0        0      115 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/backend/main.py
--rw-r--r--   0        0        0      310 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/.gitignore
--rw-r--r--   0        0        0       62 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/.rete-patch
--rw-r--r--   0        0        0     2136 2023-12-13 16:41:17.051695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/README.md
--rw-r--r--   0        0        0      517 2024-04-11 06:39:51.097296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-04-11 06:39:13.229767 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/favicon.ico
--rw-r--r--   0        0        0      653 2024-04-11 06:39:51.097296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/index.html
--rw-r--r--   0        0        0      306 2024-04-11 06:39:13.229767 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-11 06:39:13.229767 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/robots.txt
--rw-r--r--   0        0        0    18032 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css
--rw-r--r--   0        0        0    46651 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css.map
--rw-r--r--   0        0        0     4516 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js
--rw-r--r--   0        0        0    10597 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js.map
--rw-r--r--   0        0        0  3614719 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js
--rw-r--r--   0        0        0     3456 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.LICENSE.txt
--rw-r--r--   0        0        0 13933598 2024-04-11 06:39:51.125296 aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.map
--rw-r--r--   0        0        0  1408322 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/web/frontend/package-lock.json
--rw-r--r--   0        0        0     2248 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/web/frontend/package.json
--rw-r--r--   0        0        0     3870 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/public/favicon.ico
--rw-r--r--   0        0        0     1323 2023-12-28 12:44:51.918218 aiida_worktree-0.1.6/aiida_worktree/web/frontend/public/index.html
--rw-r--r--   0        0        0      306 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/public/robots.txt
--rw-r--r--   0        0        0     2442 2023-12-28 12:44:51.918218 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/App.css
--rw-r--r--   0        0        0     1135 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/App.js
--rw-r--r--   0        0        0      273 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/App.test.tsx
--rw-r--r--   0        0        0     1675 2024-04-13 03:14:32.506807 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/AtomsItem.js
--rw-r--r--   0        0        0       94 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Data.js
--rw-r--r--   0        0        0      106 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/DataNode.js
--rw-r--r--   0        0        0      505 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/DataNodeItem.css
--rw-r--r--   0        0        0     1458 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/DataNodeItem.tsx
--rw-r--r--   0        0        0     5590 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/DataNodeTable.js
--rw-r--r--   0        0        0      115 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Home.js
--rw-r--r--   0        0        0     1324 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Layout.css
--rw-r--r--   0        0        0     1065 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Layout.js
--rw-r--r--   0        0        0     5789 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/NodeDetails.js
--rw-r--r--   0        0        0     2784 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Settings.js
--rw-r--r--   0        0        0     1016 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeDetail.js
--rw-r--r--   0        0        0     2630 2023-12-28 12:44:51.918218 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeDuration.js
--rw-r--r--   0        0        0     8766 2024-04-17 06:30:26.245030 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeItem.tsx
--rw-r--r--   0        0        0     1064 2023-12-28 12:44:51.918218 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeItemStyles.ts
--rw-r--r--   0        0        0      834 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeLog.js
--rw-r--r--   0        0        0      989 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeTable.css
--rw-r--r--   0        0        0     7503 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeTable.js
--rw-r--r--   0        0        0     1120 2023-12-28 12:44:51.918218 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorktreeIndicator.js
--rw-r--r--   0        0        0     3434 2024-02-12 17:45:35.088645 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorktreeSummary.js
--rw-r--r--   0        0        0      366 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/index.css
--rw-r--r--   0        0        0      554 2023-12-14 08:55:54.387318 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/index.tsx
--rw-r--r--   0        0        0     6007 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/logo.svg
--rw-r--r--   0        0        0       40 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      425 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/reportWebVitals.ts
--rw-r--r--   0        0        0      160 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete.css
--rw-r--r--   0        0        0     2787 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization.ts
--rw-r--r--   0        0        0      813 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/CustomConnection.tsx
--rw-r--r--   0        0        0     4981 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/CustomNode.tsx
--rw-r--r--   0        0        0      566 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/CustomSocket.tsx
--rw-r--r--   0        0        0      540 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/StyledNode.tsx
--rw-r--r--   0        0        0      602 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/background.css
--rw-r--r--   0        0        0      378 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/custom-background.ts
--rw-r--r--   0        0        0       94 2023-12-13 16:41:17.055695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/vars.ts
--rw-r--r--   0        0        0     4589 2024-04-13 03:14:32.506807 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/default.ts
--rw-r--r--   0        0        0      603 2023-12-13 16:41:17.059695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/index.ts
--rw-r--r--   0        0        0      241 2023-12-13 16:41:17.059695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/setupTests.ts
--rw-r--r--   0        0        0      535 2023-12-13 16:41:17.059695 aiida_worktree-0.1.6/aiida_worktree/web/frontend/tsconfig.json
--rw-r--r--   0        0        0       94 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/widget/.gitignore
--rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_worktree-0.1.6/aiida_worktree/widget/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0      552 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/widget/README.md
--rw-r--r--   0        0        0       71 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/widget/__init__.py
--rw-r--r--   0        0        0     7051 2024-04-18 07:39:32.684824 aiida_worktree-0.1.6/aiida_worktree/widget/js/default_rete.ts
--rw-r--r--   0        0        0      556 2024-04-18 06:53:34.611232 aiida_worktree-0.1.6/aiida_worktree/widget/js/widget.css
--rw-r--r--   0        0        0     3113 2024-04-18 07:03:08.632381 aiida_worktree-0.1.6/aiida_worktree/widget/js/widget.tsx
--rw-r--r--   0        0        0    94707 2024-04-17 08:01:13.593776 aiida_worktree-0.1.6/aiida_worktree/widget/package-lock.json
--rw-r--r--   0        0        0      830 2024-04-17 08:01:13.593776 aiida_worktree-0.1.6/aiida_worktree/widget/package.json
--rw-r--r--   0        0        0      765 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/widget/pyproject.toml
--rw-r--r--   0        0        0     1241 2024-04-18 07:41:49.697224 aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/__init__.py
--rw-r--r--   0        0        0      424 2024-04-18 08:28:09.835240 aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/static/widget.css
--rw-r--r--   0        0        0  1671860 2024-04-18 08:28:09.835240 aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/static/widget.js
--rw-r--r--   0        0        0      817 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/utils.py
--rw-r--r--   0        0        0      453 2024-04-16 06:39:40.905764 aiida_worktree-0.1.6/aiida_worktree/widget/tsconfig.json
--rw-r--r--   0        0        0    12685 2024-04-17 15:17:33.932303 aiida_worktree-0.1.6/aiida_worktree/worktree.py
--rw-r--r--   0        0        0     2474 2024-04-17 15:17:33.936303 aiida_worktree-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6984 1970-01-01 00:00:00.000000 aiida_worktree-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4954 2024-04-17 15:17:33.932303 aiida_worktree-0.1.7/README.md
+-rw-r--r--   0        0        0      172 2024-04-18 15:41:26.699863 aiida_worktree-0.1.7/aiida_worktree/__init__.py
+-rw-r--r--   0        0        0      275 2023-12-13 16:41:17.047695 aiida_worktree-0.1.7/aiida_worktree/cli/__init__.py
+-rw-r--r--   0        0        0    12079 2023-12-13 16:41:17.047695 aiida_worktree-0.1.7/aiida_worktree/cli/cmd_tree.py
+-rw-r--r--   0        0        0     1932 2023-12-13 16:41:17.047695 aiida_worktree-0.1.7/aiida_worktree/cli/cmd_web.py
+-rw-r--r--   0        0        0      700 2023-12-13 16:41:17.047695 aiida_worktree-0.1.7/aiida_worktree/cli/cmd_worktree.py
+-rw-r--r--   0        0        0     6581 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/cli/query_worktree.py
+-rw-r--r--   0        0        0    12205 2024-04-18 15:41:04.600063 aiida_worktree-0.1.7/aiida_worktree/decorator.py
+-rw-r--r--   0        0        0        0 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/engine/__init__.py
+-rw-r--r--   0        0        0    44165 2024-04-17 05:39:00.099765 aiida_worktree-0.1.7/aiida_worktree/engine/worktree.py
+-rw-r--r--   0        0        0        0 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/executors/__init__.py
+-rw-r--r--   0        0        0     1098 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/executors/builtin.py
+-rw-r--r--   0        0        0      634 2024-04-13 03:14:32.498807 aiida_worktree-0.1.7/aiida_worktree/executors/qe.py
+-rw-r--r--   0        0        0      439 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/executors/test.py
+-rw-r--r--   0        0        0     2659 2024-04-18 13:02:41.705696 aiida_worktree-0.1.7/aiida_worktree/node.py
+-rw-r--r--   0        0        0      936 2024-02-12 16:38:13.895317 aiida_worktree-0.1.7/aiida_worktree/nodes/__init__.py
+-rw-r--r--   0        0        0     3868 2024-02-12 16:38:13.895317 aiida_worktree-0.1.7/aiida_worktree/nodes/builtin.py
+-rw-r--r--   0        0        0     4838 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/nodes/qe.py
+-rw-r--r--   0        0        0     6562 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/nodes/test.py
+-rw-r--r--   0        0        0     1202 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/orm/worktree.py
+-rw-r--r--   0        0        0      114 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/properties/__init__.py
+-rw-r--r--   0        0        0     8432 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/properties/built_in.py
+-rw-r--r--   0        0        0      586 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/property.py
+-rw-r--r--   0        0        0      353 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/socket.py
+-rw-r--r--   0        0        0      110 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/sockets/__init__.py
+-rw-r--r--   0        0        0     2852 2023-12-11 16:36:18.395013 aiida_worktree-0.1.7/aiida_worktree/sockets/built_in.py
+-rw-r--r--   0        0        0     7254 2024-04-16 12:22:57.721423 aiida_worktree-0.1.7/aiida_worktree/utils/__init__.py
+-rw-r--r--   0        0        0     5713 2024-04-13 03:14:32.498807 aiida_worktree-0.1.7/aiida_worktree/utils/analysis.py
+-rw-r--r--   0        0        0     1677 2024-04-18 06:44:50.292276 aiida_worktree-0.1.7/aiida_worktree/utils/tree.py
+-rw-r--r--   0        0        0      763 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/README.md
+-rw-r--r--   0        0        0        0 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/backend/app/__init__.py
+-rw-r--r--   0        0        0     2388 2024-02-12 17:45:35.080641 aiida_worktree-0.1.7/aiida_worktree/web/backend/app/api.py
+-rw-r--r--   0        0        0     3638 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/backend/app/daemon.py
+-rw-r--r--   0        0        0     2112 2024-02-12 17:45:35.080641 aiida_worktree-0.1.7/aiida_worktree/web/backend/app/datanode.py
+-rw-r--r--   0        0        0     5938 2024-04-17 08:01:13.585776 aiida_worktree-0.1.7/aiida_worktree/web/backend/app/utils.py
+-rw-r--r--   0        0        0     5087 2024-01-14 22:48:05.651634 aiida_worktree-0.1.7/aiida_worktree/web/backend/app/worktree.py
+-rw-r--r--   0        0        0      115 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/backend/main.py
+-rw-r--r--   0        0        0      310 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/.gitignore
+-rw-r--r--   0        0        0       62 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/.rete-patch
+-rw-r--r--   0        0        0     2136 2023-12-13 16:41:17.051695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/README.md
+-rw-r--r--   0        0        0      517 2024-04-11 06:39:51.097296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-04-11 06:39:13.229767 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/favicon.ico
+-rw-r--r--   0        0        0      653 2024-04-11 06:39:51.097296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/index.html
+-rw-r--r--   0        0        0      306 2024-04-11 06:39:13.229767 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-11 06:39:13.229767 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/robots.txt
+-rw-r--r--   0        0        0    18032 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css
+-rw-r--r--   0        0        0    46651 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css.map
+-rw-r--r--   0        0        0     4516 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js
+-rw-r--r--   0        0        0    10597 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js.map
+-rw-r--r--   0        0        0  3614719 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js
+-rw-r--r--   0        0        0     3456 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.LICENSE.txt
+-rw-r--r--   0        0        0 13933598 2024-04-11 06:39:51.125296 aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.map
+-rw-r--r--   0        0        0  1408322 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/web/frontend/package-lock.json
+-rw-r--r--   0        0        0     2248 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/web/frontend/package.json
+-rw-r--r--   0        0        0     3870 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/public/favicon.ico
+-rw-r--r--   0        0        0     1323 2023-12-28 12:44:51.918218 aiida_worktree-0.1.7/aiida_worktree/web/frontend/public/index.html
+-rw-r--r--   0        0        0      306 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/public/robots.txt
+-rw-r--r--   0        0        0     2442 2023-12-28 12:44:51.918218 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/App.css
+-rw-r--r--   0        0        0     1135 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/App.js
+-rw-r--r--   0        0        0      273 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/App.test.tsx
+-rw-r--r--   0        0        0     1675 2024-04-13 03:14:32.506807 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/AtomsItem.js
+-rw-r--r--   0        0        0       94 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Data.js
+-rw-r--r--   0        0        0      106 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/DataNode.js
+-rw-r--r--   0        0        0      505 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/DataNodeItem.css
+-rw-r--r--   0        0        0     1458 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/DataNodeItem.tsx
+-rw-r--r--   0        0        0     5590 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/DataNodeTable.js
+-rw-r--r--   0        0        0      115 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Home.js
+-rw-r--r--   0        0        0     1324 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Layout.css
+-rw-r--r--   0        0        0     1065 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Layout.js
+-rw-r--r--   0        0        0     5789 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/NodeDetails.js
+-rw-r--r--   0        0        0     2784 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Settings.js
+-rw-r--r--   0        0        0     1016 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeDetail.js
+-rw-r--r--   0        0        0     2630 2023-12-28 12:44:51.918218 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeDuration.js
+-rw-r--r--   0        0        0     8766 2024-04-17 06:30:26.245030 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeItem.tsx
+-rw-r--r--   0        0        0     1064 2023-12-28 12:44:51.918218 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeItemStyles.ts
+-rw-r--r--   0        0        0      834 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeLog.js
+-rw-r--r--   0        0        0      989 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeTable.css
+-rw-r--r--   0        0        0     7503 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeTable.js
+-rw-r--r--   0        0        0     1120 2023-12-28 12:44:51.918218 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorktreeIndicator.js
+-rw-r--r--   0        0        0     3434 2024-02-12 17:45:35.088645 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorktreeSummary.js
+-rw-r--r--   0        0        0      366 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/index.css
+-rw-r--r--   0        0        0      554 2023-12-14 08:55:54.387318 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/index.tsx
+-rw-r--r--   0        0        0     6007 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/logo.svg
+-rw-r--r--   0        0        0       40 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      425 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/reportWebVitals.ts
+-rw-r--r--   0        0        0      160 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete.css
+-rw-r--r--   0        0        0     2787 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization.ts
+-rw-r--r--   0        0        0      813 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/CustomConnection.tsx
+-rw-r--r--   0        0        0     4981 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/CustomNode.tsx
+-rw-r--r--   0        0        0      566 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/CustomSocket.tsx
+-rw-r--r--   0        0        0      540 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/StyledNode.tsx
+-rw-r--r--   0        0        0      602 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/background.css
+-rw-r--r--   0        0        0      378 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/custom-background.ts
+-rw-r--r--   0        0        0       94 2023-12-13 16:41:17.055695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/vars.ts
+-rw-r--r--   0        0        0     4589 2024-04-13 03:14:32.506807 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/default.ts
+-rw-r--r--   0        0        0      603 2023-12-13 16:41:17.059695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/index.ts
+-rw-r--r--   0        0        0      241 2023-12-13 16:41:17.059695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/setupTests.ts
+-rw-r--r--   0        0        0      535 2023-12-13 16:41:17.059695 aiida_worktree-0.1.7/aiida_worktree/web/frontend/tsconfig.json
+-rw-r--r--   0        0        0       94 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/widget/.gitignore
+-rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_worktree-0.1.7/aiida_worktree/widget/.ipynb_checkpoints/example-checkpoint.ipynb
+-rw-r--r--   0        0        0      552 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/widget/README.md
+-rw-r--r--   0        0        0       71 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/widget/__init__.py
+-rw-r--r--   0        0        0     7051 2024-04-18 08:31:59.832316 aiida_worktree-0.1.7/aiida_worktree/widget/js/default_rete.ts
+-rw-r--r--   0        0        0      556 2024-04-18 08:31:59.832316 aiida_worktree-0.1.7/aiida_worktree/widget/js/widget.css
+-rw-r--r--   0        0        0     3113 2024-04-18 08:31:59.832316 aiida_worktree-0.1.7/aiida_worktree/widget/js/widget.tsx
+-rw-r--r--   0        0        0    94707 2024-04-17 08:01:13.593776 aiida_worktree-0.1.7/aiida_worktree/widget/package-lock.json
+-rw-r--r--   0        0        0      830 2024-04-17 08:01:13.593776 aiida_worktree-0.1.7/aiida_worktree/widget/package.json
+-rw-r--r--   0        0        0      765 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/widget/pyproject.toml
+-rw-r--r--   0        0        0     1279 2024-04-18 10:08:49.328675 aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-18 15:41:47.939671 aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/static/widget.css
+-rw-r--r--   0        0        0  1671860 2024-04-18 15:41:47.939671 aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/static/widget.js
+-rw-r--r--   0        0        0      817 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/utils.py
+-rw-r--r--   0        0        0      453 2024-04-16 06:39:40.905764 aiida_worktree-0.1.7/aiida_worktree/widget/tsconfig.json
+-rw-r--r--   0        0        0    12685 2024-04-17 15:17:33.932303 aiida_worktree-0.1.7/aiida_worktree/worktree.py
+-rw-r--r--   0        0        0     2474 2024-04-17 15:17:33.936303 aiida_worktree-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6984 1970-01-01 00:00:00.000000 aiida_worktree-0.1.7/PKG-INFO
```

### Comparing `aiida_worktree-0.1.6/LICENSE` & `aiida_worktree-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/README.md` & `aiida_worktree-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/cli/cmd_tree.py` & `aiida_worktree-0.1.7/aiida_worktree/cli/cmd_tree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/cli/cmd_web.py` & `aiida_worktree-0.1.7/aiida_worktree/cli/cmd_web.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/cli/cmd_worktree.py` & `aiida_worktree-0.1.7/aiida_worktree/cli/cmd_worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/cli/query_worktree.py` & `aiida_worktree-0.1.7/aiida_worktree/cli/query_worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/decorator.py` & `aiida_worktree-0.1.7/aiida_worktree/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,53 +26,76 @@
         for value in port.values():
             add_input_recursive(inputs, value, prefix=port_name)
     else:
         inputs.append(["General", port_name])
     return inputs
 
 
-def build_node(ndata):
+def build_node(executor, outputs=None):
+    """Build node from executor."""
     from aiida_worktree.worktree import WorkTree
 
-    if isinstance(ndata, WorkTree):
-        return build_node_from_worktree(ndata)
-    elif "path" in ndata:
-        return build_node_from_AiiDA(ndata)
+    if isinstance(executor, WorkTree):
+        return build_node_from_worktree(executor)
+    elif isinstance(executor, str):
+        (
+            path,
+            executor_name,
+        ) = executor.rsplit(".", 1)
+        executor, _ = get_executor({"path": path, "name": executor_name})
+    if callable(executor):
+        return build_node_from_callable(executor, outputs=outputs)
 
 
-def build_node_from_AiiDA(ndata):
-    """Register a node from a AiiDA component.
-    For example: CalcJob, WorkChain, CalcFunction, WorkFunction."""
-    from aiida_worktree.node import Node
+def build_node_from_callable(executor, outputs=None):
+    """Build node from a callable object."""
     import inspect
 
-    path, executor_name, = ndata.pop(
-        "path"
-    ).rsplit(".", 1)
-    ndata["executor"] = {"path": path, "name": executor_name}
-    executor, type = get_executor(ndata["executor"])
-    # print(executor)
+    ndata = {}
     if inspect.isfunction(executor):
         # calcfunction and workfunction
         if getattr(executor, "node_class", False):
             if executor.node_class is CalcFunctionNode:
                 ndata["node_type"] = "calcfunction"
             elif executor.node_class is WorkFunctionNode:
                 ndata["node_type"] = "workfunction"
+            ndata["executor"] = executor
+            return build_node_from_AiiDA(ndata)
         else:
             ndata["node_type"] = "normal"
+            ndata["executor"] = executor
+            return build_node_from_function(executor, outputs=outputs)
     else:
         if issubclass(executor, CalcJob):
             ndata["node_type"] = "calcjob"
+            ndata["executor"] = executor
+            return build_node_from_AiiDA(ndata)
         elif issubclass(executor, WorkChain):
             ndata["node_type"] = "workchain"
+            ndata["executor"] = executor
+            return build_node_from_AiiDA(ndata)
         else:
             ndata["node_type"] = "normal"
+        ndata["executor"] = executor
+
+
+def build_node_from_function(executor, outputs=None):
+    """Build node from function."""
+    return NodeDecoratorCollection.decorator_node(outputs=outputs)(executor).node
+
+
+def build_node_from_AiiDA(ndata):
+    """Register a node from a AiiDA component.
+    For example: CalcJob, WorkChain, CalcFunction, WorkFunction."""
+    from aiida_worktree.node import Node
+
+    # print(executor)
     inputs = []
     outputs = []
+    executor = ndata["executor"]
     spec = executor.spec()
     for _key, port in spec.inputs.ports.items():
         add_input_recursive(inputs, port)
     kwargs = [input[1] for input in inputs]
     for _key, port in spec.outputs.ports.items():
         outputs.append(["General", port.name])
     if spec.inputs.dynamic:
@@ -85,15 +108,15 @@
     outputs.append(["General", "_outputs"])
     outputs.append(["General", "_wait"])
     inputs.append(["General", "_wait", {"link_limit": 1e6}])
     ndata["node_class"] = Node
     ndata["kwargs"] = kwargs
     ndata["inputs"] = inputs
     ndata["outputs"] = outputs
-    ndata["identifier"] = ndata.pop("identifier", ndata["executor"]["name"])
+    ndata["identifier"] = ndata.pop("identifier", ndata["executor"].__name__)
     # TODO In order to reload the WorkTree from process, "is_pickle" should be True
     # so I pickled the function here, but this is not necessary
     # we need to update the node_graph to support the path and name of the function
     executor = {
         "executor": pickle.dumps(executor),
         "type": ndata["node_type"],
         "is_pickle": True,
```

### Comparing `aiida_worktree-0.1.6/aiida_worktree/engine/worktree.py` & `aiida_worktree-0.1.7/aiida_worktree/engine/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/executors/builtin.py` & `aiida_worktree-0.1.7/aiida_worktree/executors/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/executors/qe.py` & `aiida_worktree-0.1.7/aiida_worktree/executors/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/node.py` & `aiida_worktree-0.1.7/aiida_worktree/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,27 @@
 
     def __init__(self, **kwargs):
         """
         Initialize a Node instance.
         """
         super().__init__(**kwargs)
         self.to_ctx = None
-        self.wait = None
+        self.wait = []
         self.process = None
         self.pk = None
         self._widget = NodeGraphWidget(
             settings={"minmap": False}, style={"width": "40%", "height": "600px"}
         )
 
     def to_dict(self):
         ndata = super().to_dict()
         ndata["to_ctx"] = [] if self.to_ctx is None else self.to_ctx
-        ndata["wait"] = [] if self.wait is None else self.wait
+        ndata["wait"] = [
+            node if isinstance(node, str) else node.name for node in self.wait
+        ]
         ndata["process"] = self.process.uuid if self.process else None
         ndata["metadata"]["pk"] = self.process.pk if self.process else None
 
         return ndata
 
     def set_from_protocol(self, *args, **kwargs):
         """For node support protocol, set the node from protocol data."""
```

### Comparing `aiida_worktree-0.1.6/aiida_worktree/nodes/__init__.py` & `aiida_worktree-0.1.7/aiida_worktree/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/nodes/builtin.py` & `aiida_worktree-0.1.7/aiida_worktree/nodes/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/nodes/qe.py` & `aiida_worktree-0.1.7/aiida_worktree/nodes/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/nodes/test.py` & `aiida_worktree-0.1.7/aiida_worktree/nodes/test.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/orm/worktree.py` & `aiida_worktree-0.1.7/aiida_worktree/orm/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/properties/built_in.py` & `aiida_worktree-0.1.7/aiida_worktree/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/property.py` & `aiida_worktree-0.1.7/aiida_worktree/property.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/sockets/built_in.py` & `aiida_worktree-0.1.7/aiida_worktree/sockets/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/utils/__init__.py` & `aiida_worktree-0.1.7/aiida_worktree/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/utils/analysis.py` & `aiida_worktree-0.1.7/aiida_worktree/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/utils/tree.py` & `aiida_worktree-0.1.7/aiida_worktree/utils/tree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/README.md` & `aiida_worktree-0.1.7/aiida_worktree/web/README.md`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/backend/app/api.py` & `aiida_worktree-0.1.7/aiida_worktree/web/backend/app/api.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/backend/app/daemon.py` & `aiida_worktree-0.1.7/aiida_worktree/web/backend/app/daemon.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/backend/app/datanode.py` & `aiida_worktree-0.1.7/aiida_worktree/web/backend/app/datanode.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/backend/app/utils.py` & `aiida_worktree-0.1.7/aiida_worktree/web/backend/app/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/backend/app/worktree.py` & `aiida_worktree-0.1.7/aiida_worktree/web/backend/app/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/README.md` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/README.md`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/asset-manifest.json` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/favicon.ico` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/index.html` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css.map` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/css/main.1cbd6711.css.map`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js.map` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/787.10122f11.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.LICENSE.txt` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.map` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/build/static/js/main.45565bc2.js.map`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/package-lock.json` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/package.json` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/package.json`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/public/favicon.ico` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/public/index.html` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/App.css` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/App.css`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/App.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/AtomsItem.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/AtomsItem.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/DataNodeItem.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/DataNodeItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/DataNodeTable.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/DataNodeTable.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Layout.css` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Layout.css`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Layout.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Layout.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/NodeDetails.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/NodeDetails.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/Settings.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/Settings.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeDetail.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeDetail.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeDuration.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeDuration.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeItem.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeItemStyles.ts` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeItemStyles.ts`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeLog.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeLog.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeTable.css` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeTable.css`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorkTreeTable.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorkTreeTable.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorktreeIndicator.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorktreeIndicator.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/components/WorktreeSummary.js` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/components/WorktreeSummary.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/index.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/logo.svg` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization.ts` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization.ts`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/CustomConnection.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/CustomConnection.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/CustomNode.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/CustomNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/CustomSocket.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/CustomSocket.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/StyledNode.tsx` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/StyledNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/customization/background.css` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/customization/background.css`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/default.ts` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/default.ts`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/src/rete/index.ts` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/src/rete/index.ts`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/web/frontend/tsconfig.json` & `aiida_worktree-0.1.7/aiida_worktree/web/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/README.md` & `aiida_worktree-0.1.7/aiida_worktree/widget/README.md`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/js/default_rete.ts` & `aiida_worktree-0.1.7/aiida_worktree/widget/js/default_rete.ts`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/js/widget.css` & `aiida_worktree-0.1.7/aiida_worktree/widget/js/widget.css`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/js/widget.tsx` & `aiida_worktree-0.1.7/aiida_worktree/widget/js/widget.tsx`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/package-lock.json` & `aiida_worktree-0.1.7/aiida_worktree/widget/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/package.json` & `aiida_worktree-0.1.7/aiida_worktree/widget/package.json`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/pyproject.toml` & `aiida_worktree-0.1.7/aiida_worktree/widget/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/__init__.py` & `aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,10 +28,11 @@
         wtdata = worktree.to_dict()
         wait_to_link(wtdata)
         wtdata = worktree_to_short_json(wtdata)
         self.value = wtdata
 
     def from_node(self, node):
         ndata = node.to_dict()
+        ndata.pop("properties", None)
         ndata["label"] = ndata["metadata"]["identifier"]
         wtdata = {"nodes": {node.name: ndata}, "links": []}
         self.value = wtdata
```

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/static/widget.js` & `aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/static/widget.js`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/widget/src/widget/utils.py` & `aiida_worktree-0.1.7/aiida_worktree/widget/src/widget/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/aiida_worktree/worktree.py` & `aiida_worktree-0.1.7/aiida_worktree/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/pyproject.toml` & `aiida_worktree-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_worktree-0.1.6/PKG-INFO` & `aiida_worktree-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-worktree
-Version: 0.1.6
+Version: 0.1.7
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Keywords: aiida,workflows
 Author-email: Xing Wang <xingwang1991@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: AiiDA
```

