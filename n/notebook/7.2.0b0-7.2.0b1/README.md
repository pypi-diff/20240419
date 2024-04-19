# Comparing `tmp/notebook-7.2.0b0.tar.gz` & `tmp/notebook-7.2.0b1.tar.gz`

## Comparing `notebook-7.2.0b0.tar` & `notebook-7.2.0b1.tar`

### file list

```diff
@@ -1,441 +1,442 @@
--rw-r--r--   0        0        0   198708 2020-02-02 00:00:00.000000 notebook-7.2.0b0/CHANGELOG.md
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 notebook-7.2.0b0/CONTRIBUTING.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 notebook-7.2.0b0/RELEASE.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 notebook-7.2.0b0/jupyter-notebook.desktop
--rw-r--r--   0        0        0    14487 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook.svg
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 notebook-7.2.0b0/package.json
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 notebook-7.2.0b0/tsconfig.eslint.json
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 notebook-7.2.0b0/tsconfigbase.json
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 notebook-7.2.0b0/tsconfigbase.test.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 notebook-7.2.0b0/jupyter-config/jupyter_server_config.d/notebook.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 notebook-7.2.0b0/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/__main__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/_version.py
--rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/app.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/custom/custom.css
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/package.json
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/launch-tree.json
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/568.b92b1e59d9f727c2f830.js
--rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/877.847ad8d470afd79714ba.js
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/928.9eeacfc9b1fa36be5053.js
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/93.eae3497dd223d842d198.js
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/remoteEntry.5b6c0284fcb63e11cdf4.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/style.js
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/menus.json
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/pages.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/shell.json
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/title.json
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/top.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/zen.json
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/help-extension/open.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/tree-extension/widget.json
--rw-r--r--   0        0        0    40298 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1053.bundle.js
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1088.bundle.js
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1091.bundle.js
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1122.bundle.js
--rw-r--r--   0        0        0    25846 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/113.bundle.js
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/114.bundle.js
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1169.bundle.js
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1198.bundle.js
--rw-r--r--   0        0        0    45520 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1261.bundle.js
--rw-r--r--   0        0        0   120311 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/131.bundle.js
--rw-r--r--   0        0        0   751525 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1326.bundle.js
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1326.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/134.bundle.js
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1388.bundle.js
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1408.bundle.js
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1418.bundle.js
--rw-r--r--   0        0        0   456718 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1495.bundle.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1495.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    16689 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1496.bundle.js
--rw-r--r--   0        0        0   133211 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1542.bundle.js
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1542.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1558.bundle.js
--rw-r--r--   0        0        0    40776 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1584.bundle.js
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1618.bundle.js
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1647.bundle.js
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1650.bundle.js
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1684.bundle.js
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1696.bundle.js
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/170.bundle.js
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1809.bundle.js
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1827.bundle.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1828.bundle.js
--rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1833.bundle.js
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1837.bundle.js
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1846.bundle.js
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1869.bundle.js
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1941.bundle.js
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1958.bundle.js
--rw-r--r--   0        0        0    60653 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1962.bundle.js
--rw-r--r--   0        0        0    34160 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/1cb1c39ea642f26a4dfe.woff
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2007.bundle.js
--rw-r--r--   0        0        0   119944 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2065.bundle.js
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2088.bundle.js
--rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2089.bundle.js
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2122.bundle.js
--rw-r--r--   0        0        0    20897 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/214.bundle.js
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2167.bundle.js
--rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2184.bundle.js
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2188.bundle.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/221.bundle.js
--rw-r--r--   0        0        0    82023 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2241.bundle.js
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2311.bundle.js
--rw-r--r--   0        0        0    48217 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2323.bundle.js
--rw-r--r--   0        0        0  1481171 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2324.bundle.js
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2343.bundle.js
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2386.bundle.js
--rw-r--r--   0        0        0    29011 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2401.bundle.js
--rw-r--r--   0        0        0    44756 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2479.bundle.js
--rw-r--r--   0        0        0    33702 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2489.bundle.js
--rw-r--r--   0        0        0    29106 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2520.bundle.js
--rw-r--r--   0        0        0    54893 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2552.bundle.js
--rw-r--r--   0        0        0   354594 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2557.bundle.js
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2557.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2607.bundle.js
--rw-r--r--   0        0        0    37924 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/261.bundle.js
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2615.bundle.js
--rw-r--r--   0        0        0    18309 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2636.bundle.js
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2666.bundle.js
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/26683bf201fb258a2237.woff
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2682.bundle.js
--rw-r--r--   0        0        0    29991 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2692.bundle.js
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/270.bundle.js
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2702.bundle.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2756.bundle.js
--rw-r--r--   0        0        0    55533 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/28.bundle.js
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2813.bundle.js
--rw-r--r--   0        0        0    25765 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2866.bundle.js
--rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2871.bundle.js
--rw-r--r--   0        0        0   128623 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2913.bundle.js
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2913.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2924.bundle.js
--rw-r--r--   0        0        0    50041 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2944.bundle.js
--rw-r--r--   0        0        0   182907 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/2955.bundle.js
--rw-r--r--   0        0        0    35771 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3079.bundle.js
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/30e889b58cbc51adfbb0.woff
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/311.bundle.js
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3111.bundle.js
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3129.bundle.js
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3146.bundle.js
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3154.bundle.js
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3187.bundle.js
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3211.bundle.js
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3213.bundle.js
--rw-r--r--   0        0        0     6786 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3230.bundle.js
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/32792104b5ef69eded90.woff
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3301.bundle.js
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3322.bundle.js
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3325.bundle.js
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3336.bundle.js
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3340.bundle.js
--rw-r--r--   0        0        0    29122 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3360.bundle.js
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3370.bundle.js
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3420.bundle.js
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3449.bundle.js
--rw-r--r--   0        0        0    96169 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3462.bundle.js
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3466.bundle.js
--rw-r--r--   0        0        0    39408 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3488.bundle.js
--rw-r--r--   0        0        0    22195 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/35.bundle.js
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3501.bundle.js
--rw-r--r--   0        0        0   105135 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3512.bundle.js
--rw-r--r--   0        0        0    20832 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/355254db9ca10a09a3b5.woff
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3562.bundle.js
--rw-r--r--   0        0        0    94250 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3676.bundle.js
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3680.bundle.js
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/36e0d72d8a7afc696a3e.woff
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3700.bundle.js
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3733.bundle.js
--rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/373c04fd2418f5c77eea.eot
--rw-r--r--   0        0        0   125256 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/374.bundle.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3752.bundle.js
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3768.bundle.js
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/377.bundle.js
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3797.bundle.js
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3863.bundle.js
--rw-r--r--   0        0        0    21102 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3881.bundle.js
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3bc6ecaae7ecf6f8d7f8.woff
--rw-r--r--   0        0        0    40808 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3de784d07b9fa8f104c1.woff
--rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/3f6d3488cf65374f6f67.woff
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4002.bundle.js
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/403.bundle.js
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4030.bundle.js
--rw-r--r--   0        0        0    22183 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4035.bundle.js
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4038.bundle.js
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4039.bundle.js
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4042.bundle.js
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4058.bundle.js
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/409.bundle.js
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4105.bundle.js
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4148.bundle.js
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4212.bundle.js
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4271.bundle.js
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4291.bundle.js
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/431.bundle.js
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4382.bundle.js
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4387.bundle.js
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4430.bundle.js
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4498.bundle.js
--rw-r--r--   0        0        0    73759 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4499.bundle.js
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4521.bundle.js
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4526.bundle.js
--rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4588.bundle.js
--rw-r--r--   0        0        0   232362 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4630.bundle.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4630.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4645.bundle.js
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4670.bundle.js
--rw-r--r--   0        0        0   290991 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4708.bundle.js
--rw-r--r--   0        0        0    58945 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4780.bundle.js
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4810.bundle.js
--rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4811.bundle.js
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/481e39042508ae313a60.woff
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4825.bundle.js
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4837.bundle.js
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4843.bundle.js
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4965.bundle.js
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/4971.bundle.js
--rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5019.bundle.js
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5061.bundle.js
--rw-r--r--   0        0        0    39925 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5099.bundle.js
--rw-r--r--   0        0        0    55004 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5115.bundle.js
--rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5135.bundle.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5166.bundle.js
--rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5234.bundle.js
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5249.bundle.js
--rw-r--r--   0        0        0    22266 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5261.bundle.js
--rw-r--r--   0        0        0   142298 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5263.bundle.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5297.bundle.js
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5299.bundle.js
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5313.bundle.js
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5325.bundle.js
--rw-r--r--   0        0        0    25694 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5343.bundle.js
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5346.bundle.js
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5425.bundle.js
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5426.bundle.js
--rw-r--r--   0        0        0    15272 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/545.bundle.js
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5451.bundle.js
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5494.bundle.js
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5573.bundle.js
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5601.bundle.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5614.bundle.js
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/563.bundle.js
--rw-r--r--   0        0        0   154121 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5649.bundle.js
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5698.bundle.js
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5733.bundle.js
--rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5765.bundle.js
--rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5777.bundle.js
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5822.bundle.js
--rw-r--r--   0        0        0    26675 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5828.bundle.js
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5834.bundle.js
--rw-r--r--   0        0        0    79105 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5850.bundle.js
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5912.bundle.js
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5921.bundle.js
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5972.bundle.js
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5996.bundle.js
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/5cda41563a095bd70c78.woff
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6017.bundle.js
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6061.bundle.js
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6139.bundle.js
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/62.bundle.js
--rw-r--r--   0        0        0    43105 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6271.bundle.js
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6281.bundle.js
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/632.bundle.js
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6345.bundle.js
--rw-r--r--   0        0        0    10635 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6417.bundle.js
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/647.bundle.js
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6521.bundle.js
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6604.bundle.js
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/661.bundle.js
--rw-r--r--   0        0        0    69405 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6621.bundle.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6627.bundle.js
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6640.bundle.js
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6667.bundle.js
--rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/67.bundle.js
--rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6731.bundle.js
--rw-r--r--   0        0        0    25925 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6739.bundle.js
--rw-r--r--   0        0        0    14245 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6748.bundle.js
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/677.bundle.js
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6788.bundle.js
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6815.bundle.js
--rw-r--r--   0        0        0    37154 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6853.bundle.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6893.bundle.js
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/69.bundle.js
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/690.bundle.js
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6942.bundle.js
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6962.bundle.js
--rw-r--r--   0        0        0    71127 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6972.bundle.js
--rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/6999.bundle.js
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7005.bundle.js
--rw-r--r--   0        0        0    37240 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7010.bundle.js
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7022.bundle.js
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7054.bundle.js
--rw-r--r--   0        0        0    24130 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7097.bundle.js
--rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7153.bundle.js
--rw-r--r--   0        0        0    79037 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7154.bundle.js
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7170.bundle.js
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7179.bundle.js
--rw-r--r--   0        0        0    22340 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/721921bab0d001ebff02.woff
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7226.bundle.js
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7252.bundle.js
--rw-r--r--   0        0        0    50957 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7259.bundle.js
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7264.bundle.js
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/72bc573386dd1d48c5bb.woff
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7302.bundle.js
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7360.bundle.js
--rw-r--r--   0        0        0   210656 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7369.bundle.js
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7378.bundle.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7378.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7386.bundle.js
--rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7391.bundle.js
--rw-r--r--   0        0        0    67961 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7427.bundle.js
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/745.bundle.js
--rw-r--r--   0        0        0    27539 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7450.bundle.js
--rw-r--r--   0        0        0    38950 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7471.bundle.js
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7534.bundle.js
--rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7543.bundle.js
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/755.bundle.js
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7582.bundle.js
--rw-r--r--   0        0        0    27079 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7603.bundle.js
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7639.bundle.js
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7655.bundle.js
--rw-r--r--   0        0        0   101788 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7674.bundle.js
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7679.bundle.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7684.bundle.js
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7796.bundle.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7796.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7803.bundle.js
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7811.bundle.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7811.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7812.bundle.js
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7817.bundle.js
--rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7819.bundle.js
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7821.bundle.js
--rw-r--r--   0        0        0     9656 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7854.bundle.js
--rw-r--r--   0        0        0    28770 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7866.bundle.js
--rw-r--r--   0        0        0   102421 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7884.bundle.js
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7900.bundle.js
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7906.bundle.js
--rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/792.bundle.js
--rw-r--r--   0        0        0    88000 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7957.bundle.js
--rw-r--r--   0        0        0    60153 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7969.bundle.js
--rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7995.bundle.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7995.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/7997.bundle.js
--rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/79d088064beb3826054f.eot
--rw-r--r--   0        0        0    95138 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8010.bundle.js
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8032.bundle.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8060.bundle.js
--rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8285.bundle.js
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8378.bundle.js
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8381.bundle.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8433.bundle.js
--rw-r--r--   0        0        0    31497 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8443.bundle.js
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8446.bundle.js
--rw-r--r--   0        0        0    18641 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8471.bundle.js
--rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8479.bundle.js
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/85.bundle.js
--rw-r--r--   0        0        0    13993 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8579.bundle.js
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8633.bundle.js
--rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/870673df72e70f87c91a.woff
--rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8768.bundle.js
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8771.bundle.js
--rw-r--r--   0        0        0    32841 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8781.bundle.js
--rw-r--r--   0        0        0    17597 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8801.bundle.js
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/883.bundle.js
--rw-r--r--   0        0        0   197078 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8845.bundle.js
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8845.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8875.bundle.js
--rw-r--r--   0        0        0    34464 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/88b98cad3688915e50da.woff
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8907.bundle.js
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8928.bundle.js
--rw-r--r--   0        0        0   122744 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8929.bundle.js
--rw-r--r--   0        0        0    20114 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/893.bundle.js
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8937.bundle.js
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8979.bundle.js
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8983.bundle.js
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/899.bundle.js
--rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8ea8791754915a898a31.woff2
--rw-r--r--   0        0        0    19776 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/8ea8dbb1b02e6f730f55.woff
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/901.bundle.js
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9022.bundle.js
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9037.bundle.js
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/906.bundle.js
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9060.bundle.js
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9068.bundle.js
--rw-r--r--   0        0        0   145674 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/911.bundle.js
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9116.bundle.js
--rw-r--r--   0        0        0   511310 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9136.bundle.js
--rw-r--r--   0        0        0    63709 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9151.bundle.js
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9161.bundle.js
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9222.bundle.js
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9233.bundle.js
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9234.bundle.js
--rw-r--r--   0        0        0    22448 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9239.bundle.js
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9250.bundle.js
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9268.bundle.js
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9331.bundle.js
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9335.bundle.js
--rw-r--r--   0        0        0    54308 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9341.bundle.js
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9380.bundle.js
--rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9425.bundle.js
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9558.bundle.js
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9604.bundle.js
--rw-r--r--   0        0        0   278957 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9605.bundle.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9605.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9638.bundle.js
--rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9674eb1bd55047179038.svg
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9676.bundle.js
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9680.bundle.js
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9685.bundle.js
--rw-r--r--   0        0        0    87653 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9752.bundle.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9752.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    40964 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9799.bundle.js
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9821.bundle.js
--rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9834b82ad26e2a37583d.woff2
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9852.bundle.js
--rw-r--r--   0        0        0    35474 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/9866.bundle.js
--rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/a009bea404f7a500ded4.woff
--rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/a3b9817780214caf01e8.svg
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/af04542b29eaac04550a.woff
--rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/af6397503fcefbd61397.ttf
--rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/af96f67d7accf5fd2a4a.woff
--rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/b418136e3b384baaadec.woff
--rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/be0a084962d8066884f7.svg
--rw-r--r--   0        0        0    54558 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/bundle.js
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/c49810b53ecc0d87d802.woff
--rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/c56da8d69f1a0208b8e0.woff
--rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/cb9e9e693192413cde2b.woff
--rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/cda59d6efffa685830fd.ttf
--rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/e4299464e7b012968eed.eot
--rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/e42a88444448ac3d6054.woff2
--rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/e8711bbb871afd8e9dea.ttf
--rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/f9217f66874b0c01cd8c.woff
--rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/fc6ddf5df402b263cfb1.woff
--rw-r--r--   0        0        0   407657 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/static/third-party-licenses.json
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/templates/consoles.html
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/templates/edit.html
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/templates/error.html
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/templates/notebooks.html
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/templates/terminals.html
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 notebook-7.2.0b0/notebook/templates/tree.html
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 notebook-7.2.0b0/tests/conftest.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 notebook-7.2.0b0/tests/test_app.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 notebook-7.2.0b0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 notebook-7.2.0b0/LICENSE
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 notebook-7.2.0b0/README.md
--rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 notebook-7.2.0b0/pyproject.toml
--rw-r--r--   0        0        0    10213 2020-02-02 00:00:00.000000 notebook-7.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0   199919 2020-02-02 00:00:00.000000 notebook-7.2.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 notebook-7.2.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 notebook-7.2.0b1/RELEASE.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 notebook-7.2.0b1/jupyter-notebook.desktop
+-rw-r--r--   0        0        0    14487 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook.svg
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 notebook-7.2.0b1/package.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 notebook-7.2.0b1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 notebook-7.2.0b1/tsconfigbase.json
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 notebook-7.2.0b1/tsconfigbase.test.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 notebook-7.2.0b1/jupyter-config/jupyter_server_config.d/notebook.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 notebook-7.2.0b1/node_modules/@jupyterlab/ui-components/style/icons/filetype/notebook.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/__main__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/_version.py
+-rw-r--r--   0        0        0    13190 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/app.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/custom/custom.css
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/package.json
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/launch-tree.json
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig
+-rw-r--r--   0        0        0    12370 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/344.4324c02f8eb21e5108b0.js
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/568.8be37ab03fed258737af.js
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/928.874775037e1e9763baf2.js
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/93.eae3497dd223d842d198.js
+-rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/remoteEntry.4c55e11421866a455f51.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/style.js
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/menus.json
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/pages.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/shell.json
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/title.json
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/top.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/zen.json
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/help-extension/open.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/tree-extension/widget.json
+-rw-r--r--   0        0        0    40298 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1053.bundle.js
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1088.bundle.js
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1091.bundle.js
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1122.bundle.js
+-rw-r--r--   0        0        0    25846 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/113.bundle.js
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/114.bundle.js
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1169.bundle.js
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1198.bundle.js
+-rw-r--r--   0        0        0    45520 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1261.bundle.js
+-rw-r--r--   0        0        0   120311 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/131.bundle.js
+-rw-r--r--   0        0        0   751525 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1326.bundle.js
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1326.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/134.bundle.js
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1388.bundle.js
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1408.bundle.js
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1418.bundle.js
+-rw-r--r--   0        0        0   456718 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1495.bundle.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1495.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    16689 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1496.bundle.js
+-rw-r--r--   0        0        0   133211 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1542.bundle.js
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1542.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1558.bundle.js
+-rw-r--r--   0        0        0    40776 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1584.bundle.js
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1618.bundle.js
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1647.bundle.js
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1650.bundle.js
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1684.bundle.js
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1696.bundle.js
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/170.bundle.js
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1809.bundle.js
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1827.bundle.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1828.bundle.js
+-rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1833.bundle.js
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1837.bundle.js
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1846.bundle.js
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1869.bundle.js
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1941.bundle.js
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1958.bundle.js
+-rw-r--r--   0        0        0    60653 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1962.bundle.js
+-rw-r--r--   0        0        0    34160 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/1cb1c39ea642f26a4dfe.woff
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2007.bundle.js
+-rw-r--r--   0        0        0   119944 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2065.bundle.js
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2088.bundle.js
+-rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2089.bundle.js
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2122.bundle.js
+-rw-r--r--   0        0        0    20897 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/214.bundle.js
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2167.bundle.js
+-rw-r--r--   0        0        0    16586 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2184.bundle.js
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2188.bundle.js
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/221.bundle.js
+-rw-r--r--   0        0        0    82023 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2241.bundle.js
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2311.bundle.js
+-rw-r--r--   0        0        0    48217 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2323.bundle.js
+-rw-r--r--   0        0        0  1481171 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2324.bundle.js
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2343.bundle.js
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2386.bundle.js
+-rw-r--r--   0        0        0    29011 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2401.bundle.js
+-rw-r--r--   0        0        0    44756 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2479.bundle.js
+-rw-r--r--   0        0        0    33702 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2489.bundle.js
+-rw-r--r--   0        0        0    29106 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2520.bundle.js
+-rw-r--r--   0        0        0    54893 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2552.bundle.js
+-rw-r--r--   0        0        0   354594 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2557.bundle.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2557.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2607.bundle.js
+-rw-r--r--   0        0        0    37924 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/261.bundle.js
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2615.bundle.js
+-rw-r--r--   0        0        0    18309 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2636.bundle.js
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2666.bundle.js
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/26683bf201fb258a2237.woff
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2682.bundle.js
+-rw-r--r--   0        0        0    29991 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2692.bundle.js
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/270.bundle.js
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2702.bundle.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2756.bundle.js
+-rw-r--r--   0        0        0    55533 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/28.bundle.js
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2813.bundle.js
+-rw-r--r--   0        0        0    25765 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2866.bundle.js
+-rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2871.bundle.js
+-rw-r--r--   0        0        0   128623 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2913.bundle.js
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2913.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2924.bundle.js
+-rw-r--r--   0        0        0    50041 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2944.bundle.js
+-rw-r--r--   0        0        0   182907 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/2955.bundle.js
+-rw-r--r--   0        0        0    35771 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3079.bundle.js
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/30e889b58cbc51adfbb0.woff
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/311.bundle.js
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3111.bundle.js
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3129.bundle.js
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3146.bundle.js
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3154.bundle.js
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3187.bundle.js
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3211.bundle.js
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3213.bundle.js
+-rw-r--r--   0        0        0     6786 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3230.bundle.js
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/32792104b5ef69eded90.woff
+-rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3301.bundle.js
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3322.bundle.js
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3325.bundle.js
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3336.bundle.js
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3340.bundle.js
+-rw-r--r--   0        0        0    29122 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3360.bundle.js
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3370.bundle.js
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3420.bundle.js
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3449.bundle.js
+-rw-r--r--   0        0        0    96169 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3462.bundle.js
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3466.bundle.js
+-rw-r--r--   0        0        0    39408 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3488.bundle.js
+-rw-r--r--   0        0        0    22195 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/35.bundle.js
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3501.bundle.js
+-rw-r--r--   0        0        0   105135 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3512.bundle.js
+-rw-r--r--   0        0        0    20832 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/355254db9ca10a09a3b5.woff
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3562.bundle.js
+-rw-r--r--   0        0        0    94250 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3676.bundle.js
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3680.bundle.js
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/36e0d72d8a7afc696a3e.woff
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3700.bundle.js
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3733.bundle.js
+-rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0        0        0   125256 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/374.bundle.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3752.bundle.js
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3768.bundle.js
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/377.bundle.js
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3797.bundle.js
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3863.bundle.js
+-rw-r--r--   0        0        0    21102 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3881.bundle.js
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3bc6ecaae7ecf6f8d7f8.woff
+-rw-r--r--   0        0        0    40808 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3de784d07b9fa8f104c1.woff
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4002.bundle.js
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/403.bundle.js
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4030.bundle.js
+-rw-r--r--   0        0        0    22183 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4035.bundle.js
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4038.bundle.js
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4039.bundle.js
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4042.bundle.js
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4058.bundle.js
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/409.bundle.js
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4105.bundle.js
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4148.bundle.js
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4212.bundle.js
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4271.bundle.js
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4291.bundle.js
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/431.bundle.js
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4382.bundle.js
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4387.bundle.js
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4430.bundle.js
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4498.bundle.js
+-rw-r--r--   0        0        0    73759 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4499.bundle.js
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4521.bundle.js
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4526.bundle.js
+-rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4588.bundle.js
+-rw-r--r--   0        0        0   232362 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4630.bundle.js
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4630.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4645.bundle.js
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4670.bundle.js
+-rw-r--r--   0        0        0   290991 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4708.bundle.js
+-rw-r--r--   0        0        0    58945 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4780.bundle.js
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4810.bundle.js
+-rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4811.bundle.js
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/481e39042508ae313a60.woff
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4825.bundle.js
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4837.bundle.js
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4843.bundle.js
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4965.bundle.js
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/4971.bundle.js
+-rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5019.bundle.js
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5061.bundle.js
+-rw-r--r--   0        0        0    39925 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5099.bundle.js
+-rw-r--r--   0        0        0    55004 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5115.bundle.js
+-rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5135.bundle.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5166.bundle.js
+-rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5234.bundle.js
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5249.bundle.js
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5254.bundle.js
+-rw-r--r--   0        0        0    22266 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5261.bundle.js
+-rw-r--r--   0        0        0   142298 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5263.bundle.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5297.bundle.js
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5299.bundle.js
+-rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5313.bundle.js
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5325.bundle.js
+-rw-r--r--   0        0        0    25694 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5343.bundle.js
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5346.bundle.js
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5425.bundle.js
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5426.bundle.js
+-rw-r--r--   0        0        0    15272 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/545.bundle.js
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5451.bundle.js
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5494.bundle.js
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5573.bundle.js
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5601.bundle.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5614.bundle.js
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/563.bundle.js
+-rw-r--r--   0        0        0   154121 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5649.bundle.js
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5698.bundle.js
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5733.bundle.js
+-rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5765.bundle.js
+-rw-r--r--   0        0        0    16457 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5777.bundle.js
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5822.bundle.js
+-rw-r--r--   0        0        0    26675 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5828.bundle.js
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5834.bundle.js
+-rw-r--r--   0        0        0    79105 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5850.bundle.js
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5912.bundle.js
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5921.bundle.js
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5972.bundle.js
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5996.bundle.js
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/5cda41563a095bd70c78.woff
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6017.bundle.js
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6061.bundle.js
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6139.bundle.js
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/62.bundle.js
+-rw-r--r--   0        0        0    43105 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6271.bundle.js
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6281.bundle.js
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/632.bundle.js
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6345.bundle.js
+-rw-r--r--   0        0        0    10635 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6417.bundle.js
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/647.bundle.js
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6521.bundle.js
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6604.bundle.js
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/661.bundle.js
+-rw-r--r--   0        0        0    69405 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6621.bundle.js
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6627.bundle.js
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6640.bundle.js
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6667.bundle.js
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/67.bundle.js
+-rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6731.bundle.js
+-rw-r--r--   0        0        0    25925 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6739.bundle.js
+-rw-r--r--   0        0        0    14245 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6748.bundle.js
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/677.bundle.js
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6788.bundle.js
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6815.bundle.js
+-rw-r--r--   0        0        0    37154 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6853.bundle.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6893.bundle.js
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/69.bundle.js
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/690.bundle.js
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6942.bundle.js
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6962.bundle.js
+-rw-r--r--   0        0        0    71127 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6972.bundle.js
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/6999.bundle.js
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7005.bundle.js
+-rw-r--r--   0        0        0    37240 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7010.bundle.js
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7022.bundle.js
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7054.bundle.js
+-rw-r--r--   0        0        0    24130 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7097.bundle.js
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7153.bundle.js
+-rw-r--r--   0        0        0    79037 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7154.bundle.js
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7170.bundle.js
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7179.bundle.js
+-rw-r--r--   0        0        0    22340 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/721921bab0d001ebff02.woff
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7226.bundle.js
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7252.bundle.js
+-rw-r--r--   0        0        0    50957 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7259.bundle.js
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7264.bundle.js
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/72bc573386dd1d48c5bb.woff
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7302.bundle.js
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7360.bundle.js
+-rw-r--r--   0        0        0   210656 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7369.bundle.js
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7378.bundle.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7378.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7386.bundle.js
+-rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7391.bundle.js
+-rw-r--r--   0        0        0    67961 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7427.bundle.js
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/745.bundle.js
+-rw-r--r--   0        0        0    27539 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7450.bundle.js
+-rw-r--r--   0        0        0    38950 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7471.bundle.js
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7534.bundle.js
+-rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7543.bundle.js
+-rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/755.bundle.js
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7582.bundle.js
+-rw-r--r--   0        0        0    27079 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7603.bundle.js
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7639.bundle.js
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7655.bundle.js
+-rw-r--r--   0        0        0   101788 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7674.bundle.js
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7679.bundle.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7684.bundle.js
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7796.bundle.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7796.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7803.bundle.js
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7811.bundle.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7811.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7812.bundle.js
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7817.bundle.js
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7819.bundle.js
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7821.bundle.js
+-rw-r--r--   0        0        0     9656 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7854.bundle.js
+-rw-r--r--   0        0        0    28770 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7866.bundle.js
+-rw-r--r--   0        0        0   102421 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7884.bundle.js
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7900.bundle.js
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7906.bundle.js
+-rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/792.bundle.js
+-rw-r--r--   0        0        0    88000 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7957.bundle.js
+-rw-r--r--   0        0        0    60153 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7969.bundle.js
+-rw-r--r--   0        0        0    62217 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7995.bundle.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7995.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/7997.bundle.js
+-rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/79d088064beb3826054f.eot
+-rw-r--r--   0        0        0    95138 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8010.bundle.js
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8032.bundle.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8060.bundle.js
+-rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8285.bundle.js
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8378.bundle.js
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8381.bundle.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8433.bundle.js
+-rw-r--r--   0        0        0    31497 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8443.bundle.js
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8446.bundle.js
+-rw-r--r--   0        0        0    18641 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8471.bundle.js
+-rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8479.bundle.js
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/85.bundle.js
+-rw-r--r--   0        0        0    13993 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8579.bundle.js
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8633.bundle.js
+-rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/870673df72e70f87c91a.woff
+-rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8768.bundle.js
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8771.bundle.js
+-rw-r--r--   0        0        0    33098 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8781.bundle.js
+-rw-r--r--   0        0        0    17597 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8801.bundle.js
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/883.bundle.js
+-rw-r--r--   0        0        0   197078 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8845.bundle.js
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8845.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8875.bundle.js
+-rw-r--r--   0        0        0    34464 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/88b98cad3688915e50da.woff
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8907.bundle.js
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8928.bundle.js
+-rw-r--r--   0        0        0   122744 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8929.bundle.js
+-rw-r--r--   0        0        0    20114 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/893.bundle.js
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8937.bundle.js
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8979.bundle.js
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8983.bundle.js
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/899.bundle.js
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0        0        0    19776 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/8ea8dbb1b02e6f730f55.woff
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/901.bundle.js
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9022.bundle.js
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9037.bundle.js
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/906.bundle.js
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9060.bundle.js
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9068.bundle.js
+-rw-r--r--   0        0        0   145674 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/911.bundle.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9116.bundle.js
+-rw-r--r--   0        0        0   511310 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9136.bundle.js
+-rw-r--r--   0        0        0    63709 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9151.bundle.js
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9161.bundle.js
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9222.bundle.js
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9233.bundle.js
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9234.bundle.js
+-rw-r--r--   0        0        0    22448 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9239.bundle.js
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9250.bundle.js
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9268.bundle.js
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9331.bundle.js
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9335.bundle.js
+-rw-r--r--   0        0        0    54308 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9341.bundle.js
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9380.bundle.js
+-rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9425.bundle.js
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9558.bundle.js
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9604.bundle.js
+-rw-r--r--   0        0        0   278957 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9605.bundle.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9605.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9638.bundle.js
+-rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9674eb1bd55047179038.svg
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9676.bundle.js
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9680.bundle.js
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9685.bundle.js
+-rw-r--r--   0        0        0    87653 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9752.bundle.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9752.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    40964 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9799.bundle.js
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9821.bundle.js
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9852.bundle.js
+-rw-r--r--   0        0        0    35474 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/9866.bundle.js
+-rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/a009bea404f7a500ded4.woff
+-rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/af04542b29eaac04550a.woff
+-rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/af96f67d7accf5fd2a4a.woff
+-rw-r--r--   0        0        0    12660 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/b418136e3b384baaadec.woff
+-rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/be0a084962d8066884f7.svg
+-rw-r--r--   0        0        0    54871 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/bundle.js
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/c49810b53ecc0d87d802.woff
+-rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/c56da8d69f1a0208b8e0.woff
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/e4299464e7b012968eed.eot
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0        0        0    14628 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/fc6ddf5df402b263cfb1.woff
+-rw-r--r--   0        0        0   407832 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/templates/consoles.html
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/templates/edit.html
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/templates/error.html
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/templates/notebooks.html
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/templates/terminals.html
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 notebook-7.2.0b1/notebook/templates/tree.html
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 notebook-7.2.0b1/tests/conftest.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 notebook-7.2.0b1/tests/test_app.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 notebook-7.2.0b1/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 notebook-7.2.0b1/LICENSE
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 notebook-7.2.0b1/README.md
+-rw-r--r--   0        0        0     7755 2020-02-02 00:00:00.000000 notebook-7.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0    10213 2020-02-02 00:00:00.000000 notebook-7.2.0b1/PKG-INFO
```

### Comparing `notebook-7.2.0b0/CHANGELOG.md` & `notebook-7.2.0b1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,35 @@
 - The current theme (dark/light) can now be synced with the browser/system preference (Settings menu → Theme → Synchronise with System Settings)
 - A blue "read-only" status indicator is now  displayed in the toolbar of documents which cannot be saved because their model is read-only.
 - Native support for viewing jsonl/ndjson files was added
 - Collapsing of breadcrumbs in the File Browser can be disabled in File Browser settings
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.2.0b1
+
+([Full Changelog](https://github.com/jupyter/notebook/compare/@jupyter-notebook/application-extension@7.2.0-beta.0...b45d666d5ee1ee053b55ac9cb6e9aecde5d53945))
+
+### Enhancements made
+
+- Add `@jupyterlab/theme-dark-high-contrast-extension` [#7331](https://github.com/jupyter/notebook/pull/7331) ([@jtpio](https://github.com/jtpio))
+
+### Bugs fixed
+
+- Force notebook windowing mode to `defer` [#7335](https://github.com/jupyter/notebook/pull/7335) ([@jtpio](https://github.com/jtpio))
+- Fix scrollbar always showing up by default [#7327](https://github.com/jupyter/notebook/pull/7327) ([@jtpio](https://github.com/jtpio))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/notebook/graphs/contributors?from=2024-04-12&to=2024-04-19&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Agithub-actions+updated%3A2024-04-12..2024-04-19&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Ajtpio+updated%3A2024-04-12..2024-04-19&type=Issues) | [@RRosio](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3ARRosio+updated%3A2024-04-12..2024-04-19&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.2.0b0
 
 ([Full Changelog](https://github.com/jupyter/notebook/compare/@jupyter-notebook/application-extension@7.2.0-alpha.0...09bcd99e6dfffce92acc9a7f9d11a2a2122131c0))
 
 ### Maintenance and upkeep improvements
 
 - Update to JupyterLab `4.2.0b1` [#7319](https://github.com/jupyter/notebook/pull/7319) ([@jtpio](https://github.com/jtpio))
@@ -119,16 +140,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/notebook/graphs/contributors?from=2024-03-29&to=2024-04-12&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Agithub-actions+updated%3A2024-03-29..2024-04-12&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Ajtpio+updated%3A2024-03-29..2024-04-12&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter%2Fnotebook+involves%3Akrassowski+updated%3A2024-03-29..2024-04-12&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.2.0a0
 
 ([Full Changelog](https://github.com/jupyter/notebook/compare/@jupyter-notebook/application-extension@7.1.2...80b582bce69e33e36e936af2ea981bcb22a4d285))
 
 ### Enhancements made
 
 - Update to JupyterLab 4.2.0a2 [#7307](https://github.com/jupyter/notebook/pull/7307) ([@jtpio](https://github.com/jtpio))
```

### Comparing `notebook-7.2.0b0/CONTRIBUTING.md` & `notebook-7.2.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/RELEASE.md` & `notebook-7.2.0b1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook.svg` & `notebook-7.2.0b1/notebook.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/package.json` & `notebook-7.2.0b1/package.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/__init__.py` & `notebook-7.2.0b1/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/_version.py` & `notebook-7.2.0b1/notebook/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version info for notebook."""
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 import re
 from collections import namedtuple
 
 # Use "hatch version xx.yy.zz" to handle version changes
-__version__ = "7.2.0b0"
+__version__ = "7.2.0b1"
 
 # PEP440 version parser
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `notebook-7.2.0b0/notebook/app.py` & `notebook-7.2.0b1/notebook/app.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/labextension/package.json` & `notebook-7.2.0b1/notebook/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745039682539682%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-beta.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4c55e11421866a455f51.js'}}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-beta.0",
+        "@jupyter-notebook/application": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/apputils": "~4.3.0-beta.1",
         "@jupyterlab/coreutils": "~6.2.0-beta.1",
         "@jupyterlab/docregistry": "~4.2.0-beta.1",
         "@jupyterlab/notebook": "~4.2.0-beta.1",
         "@jupyterlab/translation": "~4.2.0-beta.1",
         "@jupyterlab/ui-components": "~4.2.0-beta.1",
@@ -31,15 +31,15 @@
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyter/notebook",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5b6c0284fcb63e11cdf4.js",
+            "load": "static/remoteEntry.4c55e11421866a455f51.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../notebook/labextension",
         "schemaDir": "schema"
     },
     "license": "BSD-3-Clause",
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json` & `notebook-7.2.0b1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/interface-switcher.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig` & `notebook-7.2.0b1/notebook/labextension/schemas/@jupyter-notebook/lab-extension/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9750000000000001%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-beta.1'}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-beta.0",
+        "@jupyter-notebook/application": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/apputils": "~4.3.0-beta.1",
         "@jupyterlab/coreutils": "~6.2.0-beta.1",
         "@jupyterlab/docregistry": "~4.2.0-beta.1",
         "@jupyterlab/notebook": "~4.2.0-beta.1",
         "@jupyterlab/translation": "~4.2.0-beta.1",
         "@jupyterlab/ui-components": "~4.2.0-beta.1",
@@ -96,9 +96,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/labextension/static/568.b92b1e59d9f727c2f830.js` & `notebook-7.2.0b1/notebook/labextension/static/568.8be37ab03fed258737af.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_jupyter_notebook_lab_extension = self.webpackChunk_jupyter_notebook_lab_extension || []).push([
     [568], {
         568: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => m
             });
-            var n, a = t(685),
-                r = t(311),
-                c = t(483),
-                l = t(68),
-                i = t(905),
+            var n, a = t(277),
+                r = t(98),
+                c = t(682),
+                l = t(59),
+                i = t(240),
                 s = t(882),
-                b = t(258),
-                d = t(550);
+                b = t(471),
+                d = t(813);
             ! function(e) {
                 e.launchNotebookTree = "jupyter-notebook:launch-tree", e.openNotebook = "jupyter-notebook:open-notebook", e.openLab = "jupyter-notebook:open-lab", e.openNbClassic = "jupyter-notebook:open-nbclassic"
             }(n || (n = {}));
             const u = {
                     id: "@jupyter-notebook/lab-extension:interface-switcher",
                     description: "A plugin to add custom toolbar items to the notebook page.",
                     autoStart: !0,
```

### Comparing `notebook-7.2.0b0/notebook/labextension/static/877.847ad8d470afd79714ba.js` & `notebook-7.2.0b1/notebook/labextension/static/344.4324c02f8eb21e5108b0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 "use strict";
 (self.webpackChunk_jupyter_notebook_lab_extension = self.webpackChunk_jupyter_notebook_lab_extension || []).push([
-    [877], {
+    [344], {
         30: (e, t, i) => {
             i.r(t), i.d(t, {
                 INotebookPathOpener: () => C,
                 INotebookShell: () => y,
                 NotebookApp: () => H,
                 NotebookShell: () => k,
                 PanelHandler: () => f,
                 Private: () => v,
                 SidePanelHandler: () => w,
                 SidePanelPalette: () => W,
                 defaultNotebookPathOpener: () => P
             });
-            var s, n = i(685),
-                r = i(433),
+            var s, n = i(277),
+                r = i(117),
                 a = i(950),
                 o = i(448),
-                d = i(483),
+                d = i(682),
                 l = i(797),
-                h = i(905),
+                h = i(240),
                 p = i(697),
                 g = i(930),
                 u = i(901),
                 c = i(882),
-                _ = i(550),
+                _ = i(813),
                 m = i(633);
             class f {
                 constructor() {
                     this._panelChildHook = (e, t) => {
                         if ("child-removed" === t.type) {
                             const e = t.child;
                             p.ArrayExt.removeFirstWhere(this._items, (t => t.widget === e))
```

### Comparing `notebook-7.2.0b0/notebook/labextension/static/928.9eeacfc9b1fa36be5053.js` & `notebook-7.2.0b1/notebook/labextension/static/928.874775037e1e9763baf2.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_jupyter_notebook_lab_extension = self.webpackChunk_jupyter_notebook_lab_extension || []).push([
     [928], {
         950: (t, e, r) => {
             r.d(e, {
                 as: () => p
             });
-            var n = r(311),
-                i = r(433),
-                a = r(376),
-                o = r(905),
-                s = r(550),
+            var n = r(98),
+                i = r(117),
+                a = r(107),
+                o = r(240),
+                s = r(813),
                 c = r(930),
                 d = r(4);
             const u = new c.Token("@jupyterlab/application:ILayoutRestorer", "A service providing application layout restoration functionality. Use this to have your activities restored across page loads.");
             var y;
             ! function(t) {
                 function e(r) {
                     return r && r.type ? "tab-area" === r.type ? {
```

### Comparing `notebook-7.2.0b0/notebook/labextension/static/93.eae3497dd223d842d198.js` & `notebook-7.2.0b1/notebook/labextension/static/93.eae3497dd223d842d198.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/labextension/static/remoteEntry.5b6c0284fcb63e11cdf4.js` & `notebook-7.2.0b1/notebook/labextension/static/remoteEntry.4c55e11421866a455f51.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, o, n, a, i, l, u, f, s, d, p, c, b, h, v, m, g, y, j, w, k, S = {
             215: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(451), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(451), t.e(568)]).then((() => () => t(568))),
+                        "./index": () => Promise.all([t.e(112), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(112), t.e(568)]).then((() => () => t(568))),
                         "./style": () => t.e(93).then((() => () => t(93)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -44,24 +44,24 @@
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         93: "eae3497dd223d842d198",
-        451: "c1bcf7bb2ec21116f8c2",
-        568: "b92b1e59d9f727c2f830",
-        877: "847ad8d470afd79714ba",
-        928: "9eeacfc9b1fa36be5053"
+        112: "febba3035a90163cfdef",
+        344: "4324c02f8eb21e5108b0",
+        568: "8be37ab03fed258737af",
+        928: "874775037e1e9763baf2"
     } [e] + ".js?v=" + {
         93: "eae3497dd223d842d198",
-        451: "c1bcf7bb2ec21116f8c2",
-        568: "b92b1e59d9f727c2f830",
-        877: "847ad8d470afd79714ba",
-        928: "9eeacfc9b1fa36be5053"
+        112: "febba3035a90163cfdef",
+        344: "4324c02f8eb21e5108b0",
+        568: "8be37ab03fed258737af",
+        928: "874775037e1e9763baf2"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter-notebook/application", "7.2.0-beta.0", (() => Promise.all([x.e(928), x.e(877), x.e(451)]).then((() => () => x(30))))), l("@jupyter-notebook/lab-extension", "7.2.0-beta.0", (() => Promise.all([x.e(451), x.e(568)]).then((() => () => x(568)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter-notebook/application", "7.2.0-beta.1", (() => Promise.all([x.e(928), x.e(344), x.e(112)]).then((() => () => x(30))))), l("@jupyter-notebook/lab-extension", "7.2.0-beta.1", (() => Promise.all([x.e(112), x.e(568)]).then((() => () => x(568)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -229,35 +229,35 @@
     }, h = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, o, n) {
         var a = x.I(r);
         return a && a.then ? a.then(e.bind(e, r, x.S[r], t, o, n)) : e(r, x.S[r], t, o, n)
     })(((e, r, t, o) => (i(e, t), h(d(r, t, o) || b(r, e, t, o) || l(r, t))))), g = v(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), y = v(((e, r, t, o, n) => {
         var a = r && x.o(r, t) && d(r, t, o);
         return a ? h(a) : n()
     })), j = {}, w = {
-        311: () => g("default", "@jupyterlab/apputils", [1, 4, 3, 0, , "beta", 1]),
-        483: () => g("default", "@jupyterlab/coreutils", [1, 6, 2, 0, , "beta", 1]),
-        550: () => g("default", "@jupyterlab/ui-components", [1, 4, 2, 0, , "beta", 1]),
-        685: () => g("default", "@jupyterlab/application", [1, 4, 2, 0, , "beta", 1]),
+        98: () => g("default", "@jupyterlab/apputils", [1, 4, 3, 0, , "beta", 2]),
+        240: () => g("default", "@jupyterlab/translation", [1, 4, 2, 0, , "beta", 2]),
+        277: () => g("default", "@jupyterlab/application", [1, 4, 2, 0, , "beta", 2]),
+        682: () => g("default", "@jupyterlab/coreutils", [1, 6, 2, 0, , "beta", 2]),
+        813: () => g("default", "@jupyterlab/ui-components", [1, 4, 2, 0, , "beta", 2]),
         882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        905: () => g("default", "@jupyterlab/translation", [1, 4, 2, 0, , "beta", 1]),
-        68: () => g("default", "@jupyterlab/notebook", [1, 4, 2, 0, , "beta", 1]),
-        258: () => y("default", "@jupyter-notebook/application", [1, 7, 2, 0, , "beta", 0], (() => Promise.all([x.e(928), x.e(877)]).then((() => () => x(30))))),
+        59: () => g("default", "@jupyterlab/notebook", [1, 4, 2, 0, , "beta", 2]),
+        471: () => y("default", "@jupyter-notebook/application", [1, 7, 2, 0, , "beta", 1], (() => Promise.all([x.e(928), x.e(344)]).then((() => () => x(30))))),
         4: () => g("default", "@lumino/properties", [1, 2, 0, 0]),
-        376: () => g("default", "@jupyterlab/rendermime", [1, 4, 2, 0, , "beta", 1]),
-        433: () => m("default", "@jupyterlab/docregistry", [1, 4, 2, 0, , "beta", 1]),
+        107: () => g("default", "@jupyterlab/rendermime", [1, 4, 2, 0, , "beta", 2]),
+        117: () => m("default", "@jupyterlab/docregistry", [1, 4, 2, 0, , "beta", 2]),
         633: () => g("default", "@lumino/messaging", [1, 2, 0, 0]),
         697: () => g("default", "@lumino/algorithm", [1, 2, 0, 0]),
         717: () => g("default", "@lumino/disposable", [1, 2, 0, 0]),
         797: () => g("default", "@lumino/polling", [1, 2, 0, 0]),
         901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
         930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0])
     }, k = {
-        451: [311, 483, 550, 685, 882, 905],
-        568: [68, 258],
-        877: [4, 376, 433, 633, 697, 717, 797, 901, 930]
+        112: [98, 240, 277, 682, 813, 882],
+        344: [4, 107, 117, 633, 697, 717, 797, 901, 930],
+        568: [59, 471]
     }, x.f.consumes = (e, r) => {
         x.o(k, e) && k[e].forEach((e => {
             if (x.o(j, e)) return r.push(j[e]);
             var t = r => {
                     j[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
                     }
@@ -278,15 +278,15 @@
         var e = {
             572: 0
         };
         x.f.j = (r, t) => {
             var o = x.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (451 != r) {
+                else if (112 != r) {
                 var n = new Promise(((t, n) => o = e[r] = [t, n]));
                 t.push(o[2] = n);
                 var a = x.p + x.u(r),
                     i = new Error;
                 x.l(a, (t => {
                     if (x.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
```

### Comparing `notebook-7.2.0b0/notebook/labextension/static/third-party-licenses.json` & `notebook-7.2.0b1/notebook/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '7.2.0-beta.1'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/application",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/application",
             "versionInfo": "4.2.0-beta.1"
         },
```

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/menus.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/menus.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734375%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-beta.1', "*

 * *                   "'@jupyter-notebook/ui-components': '^7.2.0-beta.1'}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-beta.0",
-        "@jupyter-notebook/ui-components": "^7.2.0-beta.0",
+        "@jupyter-notebook/application": "^7.2.0-beta.1",
+        "@jupyter-notebook/ui-components": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/apputils": "~4.3.0-beta.1",
         "@jupyterlab/codeeditor": "~4.2.0-beta.1",
         "@jupyterlab/console": "~4.2.0-beta.1",
         "@jupyterlab/coreutils": "~6.2.0-beta.1",
         "@jupyterlab/docmanager": "~4.2.0-beta.1",
         "@jupyterlab/docregistry": "~4.2.0-beta.1",
@@ -62,9 +62,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/shell.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/application-extension/top.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/application-extension/top.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/documentsearch-extension/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971875%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-beta.1'}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-beta.0",
+        "@jupyter-notebook/application": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/documentsearch": "~4.2.0-beta.1",
         "@lumino/widgets": "^2.3.2"
     },
     "description": "Jupyter Notebook - Document Search Extension",
     "devDependencies": {
         "rimraf": "^3.0.2",
@@ -50,9 +50,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/help-extension/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9732142857142858%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/ui-components': '^7.2.0-beta.1'}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/ui-components": "^7.2.0-beta.0",
+        "@jupyter-notebook/ui-components": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/apputils": "~4.3.0-beta.1",
         "@jupyterlab/mainmenu": "~4.2.0-beta.1",
         "@jupyterlab/translation": "~4.2.0-beta.1",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
@@ -53,9 +53,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9739583333333333%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-beta.1'}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-beta.0",
+        "@jupyter-notebook/application": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/apputils": "~4.3.0-beta.1",
         "@jupyterlab/cells": "~4.2.0-beta.1",
         "@jupyterlab/docmanager": "~4.2.0-beta.1",
         "@jupyterlab/notebook": "~4.2.0-beta.1",
         "@jupyterlab/settingregistry": "~4.2.0-beta.1",
         "@jupyterlab/translation": "~4.2.0-beta.1",
@@ -58,9 +58,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/notebook-extension/scroll-output.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/tree-extension/file-actions.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/tree-extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735294117647058%*

 * *Differences: {"'dependencies'": "{'@jupyter-notebook/application': '^7.2.0-beta.1', '@jupyter-notebook/tree': "*

 * *                   "'^7.2.0-beta.1'}",*

 * * "'version'": "'7.2.0-beta.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyter/notebook/issues"
     },
     "dependencies": {
-        "@jupyter-notebook/application": "^7.2.0-beta.0",
-        "@jupyter-notebook/tree": "^7.2.0-beta.0",
+        "@jupyter-notebook/application": "^7.2.0-beta.1",
+        "@jupyter-notebook/tree": "^7.2.0-beta.1",
         "@jupyterlab/application": "~4.2.0-beta.1",
         "@jupyterlab/apputils": "~4.3.0-beta.1",
         "@jupyterlab/coreutils": "~6.2.0-beta.1",
         "@jupyterlab/docmanager": "~4.2.0-beta.1",
         "@jupyterlab/filebrowser": "~4.2.0-beta.1",
         "@jupyterlab/mainmenu": "~4.2.0-beta.1",
         "@jupyterlab/services": "~7.2.0-beta.1",
@@ -63,9 +63,9 @@
     "sideEffects": [
         "style/**/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "7.2.0-beta.0"
+    "version": "7.2.0-beta.1"
 }
```

### Comparing `notebook-7.2.0b0/notebook/schemas/@jupyter-notebook/tree-extension/widget.json` & `notebook-7.2.0b1/notebook/schemas/@jupyter-notebook/tree-extension/widget.json`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1053.bundle.js` & `notebook-7.2.0b1/notebook/static/1053.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1088.bundle.js` & `notebook-7.2.0b1/notebook/static/1088.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1091.bundle.js` & `notebook-7.2.0b1/notebook/static/1091.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1122.bundle.js` & `notebook-7.2.0b1/notebook/static/1122.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/113.bundle.js` & `notebook-7.2.0b1/notebook/static/113.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/114.bundle.js` & `notebook-7.2.0b1/notebook/static/114.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1169.bundle.js` & `notebook-7.2.0b1/notebook/static/1169.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1198.bundle.js` & `notebook-7.2.0b1/notebook/static/1198.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1261.bundle.js` & `notebook-7.2.0b1/notebook/static/1261.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/131.bundle.js` & `notebook-7.2.0b1/notebook/static/131.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1326.bundle.js` & `notebook-7.2.0b1/notebook/static/1326.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/134.bundle.js` & `notebook-7.2.0b1/notebook/static/134.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1388.bundle.js` & `notebook-7.2.0b1/notebook/static/1388.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1408.bundle.js` & `notebook-7.2.0b1/notebook/static/1408.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1418.bundle.js` & `notebook-7.2.0b1/notebook/static/1418.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1495.bundle.js` & `notebook-7.2.0b1/notebook/static/1495.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1496.bundle.js` & `notebook-7.2.0b1/notebook/static/1496.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1542.bundle.js` & `notebook-7.2.0b1/notebook/static/1542.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1558.bundle.js` & `notebook-7.2.0b1/notebook/static/1558.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1584.bundle.js` & `notebook-7.2.0b1/notebook/static/1584.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1618.bundle.js` & `notebook-7.2.0b1/notebook/static/1618.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1647.bundle.js` & `notebook-7.2.0b1/notebook/static/1647.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1650.bundle.js` & `notebook-7.2.0b1/notebook/static/8875.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [1650, 8875], {
+    [8875, 1650], {
         71650: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => s
             });
             var n = o(9983),
                 a = o(70109),
-                i = o(37057),
+                i = o(28856),
                 d = o(81997);
             const s = [{
                 id: "@jupyter-notebook/docmanager-extension:opener",
                 autoStart: !0,
                 optional: [i.INotebookPathOpener, i.INotebookShell],
                 provides: a.IDocumentWidgetOpener,
                 description: "Open documents in a new browser tab",
```

### Comparing `notebook-7.2.0b0/notebook/static/1684.bundle.js` & `notebook-7.2.0b1/notebook/static/1684.bundle.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         95601: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => l
             });
             var a = n(25007),
                 o = n(9983),
                 i = n(78529),
-                r = n(37057),
+                r = n(28856),
                 s = n(33625);
             const c = {
                     id: "@jupyter-notebook/terminal-extension:opener",
                     description: "A plugin to open terminals in a new tab.",
                     requires: [a.IRouter, i.ITerminalTracker],
                     autoStart: !0,
                     activate: (e, t, n) => {
```

### Comparing `notebook-7.2.0b0/notebook/static/1696.bundle.js` & `notebook-7.2.0b1/notebook/static/1696.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/170.bundle.js` & `notebook-7.2.0b1/notebook/static/170.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1809.bundle.js` & `notebook-7.2.0b1/notebook/static/1809.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1827.bundle.js` & `notebook-7.2.0b1/notebook/static/1827.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1828.bundle.js` & `notebook-7.2.0b1/notebook/static/1828.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1833.bundle.js` & `notebook-7.2.0b1/notebook/static/1833.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1837.bundle.js` & `notebook-7.2.0b1/notebook/static/1837.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1846.bundle.js` & `notebook-7.2.0b1/notebook/static/1846.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1869.bundle.js` & `notebook-7.2.0b1/notebook/static/1869.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1941.bundle.js` & `notebook-7.2.0b1/notebook/static/1941.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1958.bundle.js` & `notebook-7.2.0b1/notebook/static/1958.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1962.bundle.js` & `notebook-7.2.0b1/notebook/static/1962.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/1cb1c39ea642f26a4dfe.woff` & `notebook-7.2.0b1/notebook/static/1cb1c39ea642f26a4dfe.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2007.bundle.js` & `notebook-7.2.0b1/notebook/static/2007.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2065.bundle.js` & `notebook-7.2.0b1/notebook/static/2065.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2088.bundle.js` & `notebook-7.2.0b1/notebook/static/2088.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2089.bundle.js` & `notebook-7.2.0b1/notebook/static/2089.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2122.bundle.js` & `notebook-7.2.0b1/notebook/static/2122.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/214.bundle.js` & `notebook-7.2.0b1/notebook/static/214.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2167.bundle.js` & `notebook-7.2.0b1/notebook/static/2167.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2184.bundle.js` & `notebook-7.2.0b1/notebook/static/2184.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2188.bundle.js` & `notebook-7.2.0b1/notebook/static/2188.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/221.bundle.js` & `notebook-7.2.0b1/notebook/static/221.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2241.bundle.js` & `notebook-7.2.0b1/notebook/static/2241.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2311.bundle.js` & `notebook-7.2.0b1/notebook/static/2311.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2323.bundle.js` & `notebook-7.2.0b1/notebook/static/2323.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2324.bundle.js` & `notebook-7.2.0b1/notebook/static/2324.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2343.bundle.js` & `notebook-7.2.0b1/notebook/static/2343.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2386.bundle.js` & `notebook-7.2.0b1/notebook/static/2386.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2401.bundle.js` & `notebook-7.2.0b1/notebook/static/2401.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2479.bundle.js` & `notebook-7.2.0b1/notebook/static/2479.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2489.bundle.js` & `notebook-7.2.0b1/notebook/static/2489.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2520.bundle.js` & `notebook-7.2.0b1/notebook/static/2520.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2552.bundle.js` & `notebook-7.2.0b1/notebook/static/2552.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2557.bundle.js` & `notebook-7.2.0b1/notebook/static/2557.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2607.bundle.js` & `notebook-7.2.0b1/notebook/static/2607.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/261.bundle.js` & `notebook-7.2.0b1/notebook/static/261.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2615.bundle.js` & `notebook-7.2.0b1/notebook/static/2615.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2636.bundle.js` & `notebook-7.2.0b1/notebook/static/2636.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2666.bundle.js` & `notebook-7.2.0b1/notebook/static/2666.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/26683bf201fb258a2237.woff` & `notebook-7.2.0b1/notebook/static/26683bf201fb258a2237.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2682.bundle.js` & `notebook-7.2.0b1/notebook/static/2682.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2692.bundle.js` & `notebook-7.2.0b1/notebook/static/2692.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/270.bundle.js` & `notebook-7.2.0b1/notebook/static/270.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2702.bundle.js` & `notebook-7.2.0b1/notebook/static/2702.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2756.bundle.js` & `notebook-7.2.0b1/notebook/static/2756.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/28.bundle.js` & `notebook-7.2.0b1/notebook/static/28.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2813.bundle.js` & `notebook-7.2.0b1/notebook/static/2813.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2866.bundle.js` & `notebook-7.2.0b1/notebook/static/2866.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2871.bundle.js` & `notebook-7.2.0b1/notebook/static/2871.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2913.bundle.js` & `notebook-7.2.0b1/notebook/static/2913.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2913.bundle.js.LICENSE.txt` & `notebook-7.2.0b1/notebook/static/2913.bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2924.bundle.js` & `notebook-7.2.0b1/notebook/static/2924.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2944.bundle.js` & `notebook-7.2.0b1/notebook/static/2944.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/2955.bundle.js` & `notebook-7.2.0b1/notebook/static/2955.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3079.bundle.js` & `notebook-7.2.0b1/notebook/static/3079.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/30e889b58cbc51adfbb0.woff` & `notebook-7.2.0b1/notebook/static/30e889b58cbc51adfbb0.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/311.bundle.js` & `notebook-7.2.0b1/notebook/static/311.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3111.bundle.js` & `notebook-7.2.0b1/notebook/static/3111.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3129.bundle.js` & `notebook-7.2.0b1/notebook/static/3129.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3154.bundle.js` & `notebook-7.2.0b1/notebook/static/3154.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3187.bundle.js` & `notebook-7.2.0b1/notebook/static/3187.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3211.bundle.js` & `notebook-7.2.0b1/notebook/static/3211.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3213.bundle.js` & `notebook-7.2.0b1/notebook/static/3213.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3230.bundle.js` & `notebook-7.2.0b1/notebook/static/3230.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/32792104b5ef69eded90.woff` & `notebook-7.2.0b1/notebook/static/32792104b5ef69eded90.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3301.bundle.js` & `notebook-7.2.0b1/notebook/static/3301.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3322.bundle.js` & `notebook-7.2.0b1/notebook/static/3322.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3325.bundle.js` & `notebook-7.2.0b1/notebook/static/3325.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3336.bundle.js` & `notebook-7.2.0b1/notebook/static/3336.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3340.bundle.js` & `notebook-7.2.0b1/notebook/static/3340.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3360.bundle.js` & `notebook-7.2.0b1/notebook/static/3360.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3370.bundle.js` & `notebook-7.2.0b1/notebook/static/3370.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3420.bundle.js` & `notebook-7.2.0b1/notebook/static/3420.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3449.bundle.js` & `notebook-7.2.0b1/notebook/static/3449.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3462.bundle.js` & `notebook-7.2.0b1/notebook/static/3462.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3466.bundle.js` & `notebook-7.2.0b1/notebook/static/3466.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3488.bundle.js` & `notebook-7.2.0b1/notebook/static/3488.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/35.bundle.js` & `notebook-7.2.0b1/notebook/static/35.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3501.bundle.js` & `notebook-7.2.0b1/notebook/static/3501.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3512.bundle.js` & `notebook-7.2.0b1/notebook/static/3512.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/355254db9ca10a09a3b5.woff` & `notebook-7.2.0b1/notebook/static/355254db9ca10a09a3b5.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3562.bundle.js` & `notebook-7.2.0b1/notebook/static/3562.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3676.bundle.js` & `notebook-7.2.0b1/notebook/static/3676.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3680.bundle.js` & `notebook-7.2.0b1/notebook/static/3680.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/36e0d72d8a7afc696a3e.woff` & `notebook-7.2.0b1/notebook/static/36e0d72d8a7afc696a3e.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3700.bundle.js` & `notebook-7.2.0b1/notebook/static/3700.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3733.bundle.js` & `notebook-7.2.0b1/notebook/static/3733.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/373c04fd2418f5c77eea.eot` & `notebook-7.2.0b1/notebook/static/373c04fd2418f5c77eea.eot`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/374.bundle.js` & `notebook-7.2.0b1/notebook/static/374.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3768.bundle.js` & `notebook-7.2.0b1/notebook/static/3768.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
                 a = o(2277),
                 s = o(91317),
                 l = o(43959),
                 d = o(60502),
                 c = o(31589),
                 g = o(81997),
                 u = o(63485),
-                w = o(69224),
+                w = o(28678),
                 h = o(78156),
                 b = o.n(h);
             class p {
                 constructor(e) {
                     this._onSelectionChanged = () => {
                         var e, t, o, n, r, i;
                         const a = Array.from(this._browser.selectedItems()),
```

### Comparing `notebook-7.2.0b0/notebook/static/377.bundle.js` & `notebook-7.2.0b1/notebook/static/377.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3797.bundle.js` & `notebook-7.2.0b1/notebook/static/3797.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3863.bundle.js` & `notebook-7.2.0b1/notebook/static/3863.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3881.bundle.js` & `notebook-7.2.0b1/notebook/static/3881.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3bc6ecaae7ecf6f8d7f8.woff` & `notebook-7.2.0b1/notebook/static/3bc6ecaae7ecf6f8d7f8.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3de784d07b9fa8f104c1.woff` & `notebook-7.2.0b1/notebook/static/3de784d07b9fa8f104c1.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/3f6d3488cf65374f6f67.woff` & `notebook-7.2.0b1/notebook/static/3f6d3488cf65374f6f67.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4002.bundle.js` & `notebook-7.2.0b1/notebook/static/4002.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/403.bundle.js` & `notebook-7.2.0b1/notebook/static/403.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4030.bundle.js` & `notebook-7.2.0b1/notebook/static/4030.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4035.bundle.js` & `notebook-7.2.0b1/notebook/static/4035.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4038.bundle.js` & `notebook-7.2.0b1/notebook/static/4038.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4039.bundle.js` & `notebook-7.2.0b1/notebook/static/4039.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4042.bundle.js` & `notebook-7.2.0b1/notebook/static/4042.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4058.bundle.js` & `notebook-7.2.0b1/notebook/static/4058.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/409.bundle.js` & `notebook-7.2.0b1/notebook/static/409.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4105.bundle.js` & `notebook-7.2.0b1/notebook/static/4105.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4148.bundle.js` & `notebook-7.2.0b1/notebook/static/4148.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4212.bundle.js` & `notebook-7.2.0b1/notebook/static/4212.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4271.bundle.js` & `notebook-7.2.0b1/notebook/static/4271.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4291.bundle.js` & `notebook-7.2.0b1/notebook/static/4291.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/431.bundle.js` & `notebook-7.2.0b1/notebook/static/431.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4382.bundle.js` & `notebook-7.2.0b1/notebook/static/4382.bundle.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [4382, 7906], {
         54382: (e, t, r) => {
             r.r(t), r.d(t, {
                 default: () => a
             });
             var n = r(43766),
-                o = r(37057);
+                o = r(28856);
             const c = "jp-mod-searchable",
                 a = [{
                     id: "@jupyter-notebook/documentsearch-extension:notebookShellWidgetListener",
                     requires: [o.INotebookShell, n.ISearchProviderRegistry],
                     autoStart: !0,
                     description: "A plugin to add document search functionalities",
                     activate: (e, t, r) => {
```

### Comparing `notebook-7.2.0b0/notebook/static/4387.bundle.js` & `notebook-7.2.0b1/notebook/static/4387.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4430.bundle.js` & `notebook-7.2.0b1/notebook/static/4430.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4498.bundle.js` & `notebook-7.2.0b1/notebook/static/4498.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4499.bundle.js` & `notebook-7.2.0b1/notebook/static/4499.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4521.bundle.js` & `notebook-7.2.0b1/notebook/static/4521.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4526.bundle.js` & `notebook-7.2.0b1/notebook/static/4526.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4588.bundle.js` & `notebook-7.2.0b1/notebook/static/4588.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4630.bundle.js` & `notebook-7.2.0b1/notebook/static/4630.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4645.bundle.js` & `notebook-7.2.0b1/notebook/static/4645.bundle.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         94645: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => p
             });
             var n = o(25007),
                 s = o(96985),
                 a = o(9983),
-                r = o(37057),
+                r = o(28856),
                 c = o(33625);
             const i = {
                     id: "@jupyter-notebook/console-extension:opener",
                     requires: [n.IRouter],
                     autoStart: !0,
                     description: "A plugin to open consoles in a new tab",
                     activate: (e, t) => {
```

### Comparing `notebook-7.2.0b0/notebook/static/4670.bundle.js` & `notebook-7.2.0b1/notebook/static/4670.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4708.bundle.js` & `notebook-7.2.0b1/notebook/static/4708.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4780.bundle.js` & `notebook-7.2.0b1/notebook/static/4780.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4810.bundle.js` & `notebook-7.2.0b1/notebook/static/4810.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4811.bundle.js` & `notebook-7.2.0b1/notebook/static/4811.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/481e39042508ae313a60.woff` & `notebook-7.2.0b1/notebook/static/481e39042508ae313a60.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4825.bundle.js` & `notebook-7.2.0b1/notebook/static/4825.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4843.bundle.js` & `notebook-7.2.0b1/notebook/static/4843.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4965.bundle.js` & `notebook-7.2.0b1/notebook/static/4965.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/4971.bundle.js` & `notebook-7.2.0b1/notebook/static/4971.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5019.bundle.js` & `notebook-7.2.0b1/notebook/static/5019.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5061.bundle.js` & `notebook-7.2.0b1/notebook/static/5061.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5099.bundle.js` & `notebook-7.2.0b1/notebook/static/5099.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5115.bundle.js` & `notebook-7.2.0b1/notebook/static/5115.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5135.bundle.js` & `notebook-7.2.0b1/notebook/static/5135.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5166.bundle.js` & `notebook-7.2.0b1/notebook/static/5166.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5234.bundle.js` & `notebook-7.2.0b1/notebook/static/5234.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5249.bundle.js` & `notebook-7.2.0b1/notebook/static/5249.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5261.bundle.js` & `notebook-7.2.0b1/notebook/static/5261.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5263.bundle.js` & `notebook-7.2.0b1/notebook/static/5263.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5299.bundle.js` & `notebook-7.2.0b1/notebook/static/5299.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5313.bundle.js` & `notebook-7.2.0b1/notebook/static/5313.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5325.bundle.js` & `notebook-7.2.0b1/notebook/static/5325.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5343.bundle.js` & `notebook-7.2.0b1/notebook/static/5343.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5346.bundle.js` & `notebook-7.2.0b1/notebook/static/5346.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5425.bundle.js` & `notebook-7.2.0b1/notebook/static/5425.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5426.bundle.js` & `notebook-7.2.0b1/notebook/static/5426.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/545.bundle.js` & `notebook-7.2.0b1/notebook/static/545.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5451.bundle.js` & `notebook-7.2.0b1/notebook/static/5451.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5494.bundle.js` & `notebook-7.2.0b1/notebook/static/5494.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5573.bundle.js` & `notebook-7.2.0b1/notebook/static/5573.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
             var n = t(95297),
                 a = t(9983),
                 s = t(70109),
                 r = t(17556),
                 i = t(44323),
                 c = t(2277),
                 d = t(60502),
-                l = t(37057),
+                l = t(28856),
                 u = t(97934),
                 k = t(63485),
                 b = t(78156),
                 p = t.n(b);
             const g = e => {
                     const o = e.model;
                     if (!o) return !1;
@@ -59,16 +59,16 @@
                 }) => n.ReactWidget.create(p().createElement(h, {
                     notebook: e,
                     translator: o
                 }))
             }(m || (m = {}));
             const C = "jp-NotebookKernelStatus-error",
                 f = "jp-NotebookKernelStatus-warn",
-                y = "jp-NotebookKernelStatus-info",
-                v = "jp-NotebookKernelStatus-fade";
+                v = "jp-NotebookKernelStatus-info",
+                y = "jp-NotebookKernelStatus-fade";
             var w;
             ! function(e) {
                 e.openEditNotebookMetadata = "notebook:edit-metadata"
             }(w || (w = {}));
             const N = {
                     id: "@jupyter-notebook/notebook-extension:checkpoints",
                     description: "A plugin for the checkpoint indicator.",
@@ -167,28 +167,28 @@
                             s = new k.Widget;
                         s.addClass("jp-NotebookKernelStatus"), e.shell.add(s, "menu", {
                             rank: 10010
                         });
                         const r = e => {
                             const o = e.kernelDisplayStatus;
                             let t = `Kernel ${a.Text.titleCase(o)}`;
-                            switch (s.removeClass(C), s.removeClass(f), s.removeClass(y), s.removeClass(v), o) {
+                            switch (s.removeClass(C), s.removeClass(f), s.removeClass(v), s.removeClass(y), o) {
                                 case "busy":
                                 case "idle":
-                                    t = "", s.addClass(v);
+                                    t = "", s.addClass(y);
                                     break;
                                 case "dead":
                                 case "terminating":
                                     s.addClass(C);
                                     break;
                                 case "unknown":
                                     s.addClass(f);
                                     break;
                                 default:
-                                    s.addClass(y), s.addClass(v)
+                                    s.addClass(v), s.addClass(y)
                             }
                             s.node.textContent = n.__(t)
                         };
                         o.currentChanged.connect((async () => {
                             const e = o.currentWidget;
                             e instanceof i.NotebookPanel && e.sessionContext.statusChanged.connect(r)
                         }))
@@ -253,15 +253,15 @@
                         o.currentChanged.connect((async () => {
                             o.currentWidget instanceof i.NotebookPanel && t && o.add(t, "right", {
                                 type: "Property Inspector"
                             })
                         }))
                     }
                 },
-                j = {
+                E = {
                     id: "@jupyter-notebook/notebook-extension:tab-icon",
                     description: "A plugin to update the tab icon based on the kernel status.",
                     autoStart: !0,
                     requires: [i.INotebookTracker],
                     activate: (e, o) => {
                         const t = a.PageConfig.getBaseUrl(),
                             n = a.URLExt.join(t, "static/favicons/favicon-notebook.ico"),
@@ -280,15 +280,15 @@
                                             o.href = n
                                     }
                                 })(t.kernelDisplayStatus)
                             }))
                         }))
                     }
                 },
-                E = {
+                j = {
                     id: "@jupyter-notebook/notebook-extension:trusted",
                     description: "A plugin that adds a Trusted indicator to the menu area.",
                     autoStart: !0,
                     requires: [l.INotebookShell, d.ITranslator],
                     activate: (e, o, t) => {
                         o.currentChanged.connect((async () => {
                             const e = o.currentWidget;
@@ -333,24 +333,21 @@
                             isVisible: () => null !== s.currentWidget && s.currentWidget instanceof i.NotebookPanel
                         }), o && o.addItem({
                             command: w.openEditNotebookMetadata,
                             category: "Notebook Operations"
                         })
                     }
                 },
-                P = {
+                M = {
                     id: "@jupyter-notebook/notebook-extension:windowing",
                     autoStart: !0,
-                    requires: [c.ISettingRegistry],
+                    requires: [i.INotebookTracker],
                     activate: (e, o) => {
-                        const t = o.load("@jupyterlab/notebook-extension:tracker");
-                        Promise.all([t, e.restored]).then((([e]) => {
-                            void 0 === e.user.windowing && e.set("windowingMode", "defer")
-                        })).catch((e => {
-                            console.error(e.message)
+                        o.widgetAdded.connect(((e, o) => {
+                            o.content._viewModel.windowingActive = !1, o.content.notebookConfig.windowingMode = "defer"
                         }))
                     }
                 },
-                W = [N, S, A, T, x, I, _, j, E, P]
+                W = [N, S, A, T, x, I, _, E, j, M]
         }
     }
 ]);
```

### Comparing `notebook-7.2.0b0/notebook/static/5601.bundle.js` & `notebook-7.2.0b1/notebook/static/5601.bundle.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         95601: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => l
             });
             var a = n(25007),
                 o = n(9983),
                 i = n(78529),
-                r = n(37057),
+                r = n(28856),
                 s = n(33625);
             const c = {
                     id: "@jupyter-notebook/terminal-extension:opener",
                     description: "A plugin to open terminals in a new tab.",
                     requires: [a.IRouter, i.ITerminalTracker],
                     autoStart: !0,
                     activate: (e, t, n) => {
```

### Comparing `notebook-7.2.0b0/notebook/static/5614.bundle.js` & `notebook-7.2.0b1/notebook/static/5614.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/563.bundle.js` & `notebook-7.2.0b1/notebook/static/563.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5649.bundle.js` & `notebook-7.2.0b1/notebook/static/5649.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5698.bundle.js` & `notebook-7.2.0b1/notebook/static/5698.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5733.bundle.js` & `notebook-7.2.0b1/notebook/static/5733.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5765.bundle.js` & `notebook-7.2.0b1/notebook/static/5765.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5777.bundle.js` & `notebook-7.2.0b1/notebook/static/5777.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5822.bundle.js` & `notebook-7.2.0b1/notebook/static/5822.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5828.bundle.js` & `notebook-7.2.0b1/notebook/static/5828.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5834.bundle.js` & `notebook-7.2.0b1/notebook/static/5834.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5850.bundle.js` & `notebook-7.2.0b1/notebook/static/5850.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5912.bundle.js` & `notebook-7.2.0b1/notebook/static/5912.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5921.bundle.js` & `notebook-7.2.0b1/notebook/static/5921.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5972.bundle.js` & `notebook-7.2.0b1/notebook/static/5972.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5996.bundle.js` & `notebook-7.2.0b1/notebook/static/5996.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/5cda41563a095bd70c78.woff` & `notebook-7.2.0b1/notebook/static/5cda41563a095bd70c78.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6017.bundle.js` & `notebook-7.2.0b1/notebook/static/6017.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6061.bundle.js` & `notebook-7.2.0b1/notebook/static/6061.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6139.bundle.js` & `notebook-7.2.0b1/notebook/static/6139.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/62.bundle.js` & `notebook-7.2.0b1/notebook/static/62.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6271.bundle.js` & `notebook-7.2.0b1/notebook/static/6271.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6281.bundle.js` & `notebook-7.2.0b1/notebook/static/6281.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/632.bundle.js` & `notebook-7.2.0b1/notebook/static/632.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6345.bundle.js` & `notebook-7.2.0b1/notebook/static/6345.bundle.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         94645: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => p
             });
             var n = o(25007),
                 s = o(96985),
                 a = o(9983),
-                r = o(37057),
+                r = o(28856),
                 c = o(33625);
             const i = {
                     id: "@jupyter-notebook/console-extension:opener",
                     requires: [n.IRouter],
                     autoStart: !0,
                     description: "A plugin to open consoles in a new tab",
                     activate: (e, t) => {
```

### Comparing `notebook-7.2.0b0/notebook/static/6417.bundle.js` & `notebook-7.2.0b1/notebook/static/6417.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/647.bundle.js` & `notebook-7.2.0b1/notebook/static/647.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6521.bundle.js` & `notebook-7.2.0b1/notebook/static/6521.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6604.bundle.js` & `notebook-7.2.0b1/notebook/static/6604.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/661.bundle.js` & `notebook-7.2.0b1/notebook/static/661.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6621.bundle.js` & `notebook-7.2.0b1/notebook/static/6621.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6627.bundle.js` & `notebook-7.2.0b1/notebook/static/6627.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6640.bundle.js` & `notebook-7.2.0b1/notebook/static/6640.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6667.bundle.js` & `notebook-7.2.0b1/notebook/static/6667.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/67.bundle.js` & `notebook-7.2.0b1/notebook/static/67.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6731.bundle.js` & `notebook-7.2.0b1/notebook/static/6731.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6739.bundle.js` & `notebook-7.2.0b1/notebook/static/6739.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6748.bundle.js` & `notebook-7.2.0b1/notebook/static/6748.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/677.bundle.js` & `notebook-7.2.0b1/notebook/static/677.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6788.bundle.js` & `notebook-7.2.0b1/notebook/static/6788.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6815.bundle.js` & `notebook-7.2.0b1/notebook/static/6815.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6853.bundle.js` & `notebook-7.2.0b1/notebook/static/6853.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6893.bundle.js` & `notebook-7.2.0b1/notebook/static/6893.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/69.bundle.js` & `notebook-7.2.0b1/notebook/static/69.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/690.bundle.js` & `notebook-7.2.0b1/notebook/static/690.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6942.bundle.js` & `notebook-7.2.0b1/notebook/static/6942.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6962.bundle.js` & `notebook-7.2.0b1/notebook/static/6962.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6972.bundle.js` & `notebook-7.2.0b1/notebook/static/6972.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/6999.bundle.js` & `notebook-7.2.0b1/notebook/static/6999.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7005.bundle.js` & `notebook-7.2.0b1/notebook/static/7005.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7010.bundle.js` & `notebook-7.2.0b1/notebook/static/7010.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7022.bundle.js` & `notebook-7.2.0b1/notebook/static/7022.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7054.bundle.js` & `notebook-7.2.0b1/notebook/static/7054.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7097.bundle.js` & `notebook-7.2.0b1/notebook/static/7097.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7153.bundle.js` & `notebook-7.2.0b1/notebook/static/7153.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7154.bundle.js` & `notebook-7.2.0b1/notebook/static/7154.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7170.bundle.js` & `notebook-7.2.0b1/notebook/static/7170.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7179.bundle.js` & `notebook-7.2.0b1/notebook/static/7179.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/721921bab0d001ebff02.woff` & `notebook-7.2.0b1/notebook/static/721921bab0d001ebff02.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7226.bundle.js` & `notebook-7.2.0b1/notebook/static/7226.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7252.bundle.js` & `notebook-7.2.0b1/notebook/static/7252.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7259.bundle.js` & `notebook-7.2.0b1/notebook/static/7259.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7264.bundle.js` & `notebook-7.2.0b1/notebook/static/7264.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/72bc573386dd1d48c5bb.woff` & `notebook-7.2.0b1/notebook/static/72bc573386dd1d48c5bb.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7302.bundle.js` & `notebook-7.2.0b1/notebook/static/7302.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
                 a = o(2277),
                 s = o(91317),
                 l = o(43959),
                 d = o(60502),
                 c = o(31589),
                 g = o(81997),
                 u = o(63485),
-                w = o(69224),
+                w = o(28678),
                 h = o(78156),
                 b = o.n(h);
             class p {
                 constructor(e) {
                     this._onSelectionChanged = () => {
                         var e, t, o, n, r, i;
                         const a = Array.from(this._browser.selectedItems()),
```

### Comparing `notebook-7.2.0b0/notebook/static/7360.bundle.js` & `notebook-7.2.0b1/notebook/static/7360.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7369.bundle.js` & `notebook-7.2.0b1/notebook/static/7369.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7378.bundle.js` & `notebook-7.2.0b1/notebook/static/7378.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7386.bundle.js` & `notebook-7.2.0b1/notebook/static/7386.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7391.bundle.js` & `notebook-7.2.0b1/notebook/static/7391.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7427.bundle.js` & `notebook-7.2.0b1/notebook/static/7427.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/745.bundle.js` & `notebook-7.2.0b1/notebook/static/745.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7450.bundle.js` & `notebook-7.2.0b1/notebook/static/7450.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7471.bundle.js` & `notebook-7.2.0b1/notebook/static/7471.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7534.bundle.js` & `notebook-7.2.0b1/notebook/static/7534.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7543.bundle.js` & `notebook-7.2.0b1/notebook/static/7543.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/755.bundle.js` & `notebook-7.2.0b1/notebook/static/755.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7582.bundle.js` & `notebook-7.2.0b1/notebook/static/7582.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7603.bundle.js` & `notebook-7.2.0b1/notebook/static/7603.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7639.bundle.js` & `notebook-7.2.0b1/notebook/static/7639.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7655.bundle.js` & `notebook-7.2.0b1/notebook/static/7655.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7674.bundle.js` & `notebook-7.2.0b1/notebook/static/7674.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7679.bundle.js` & `notebook-7.2.0b1/notebook/static/7679.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7684.bundle.js` & `notebook-7.2.0b1/notebook/static/7684.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7796.bundle.js` & `notebook-7.2.0b1/notebook/static/7796.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7803.bundle.js` & `notebook-7.2.0b1/notebook/static/7803.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7811.bundle.js` & `notebook-7.2.0b1/notebook/static/7811.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7812.bundle.js` & `notebook-7.2.0b1/notebook/static/7812.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7817.bundle.js` & `notebook-7.2.0b1/notebook/static/7817.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7819.bundle.js` & `notebook-7.2.0b1/notebook/static/7819.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7821.bundle.js` & `notebook-7.2.0b1/notebook/static/7821.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7854.bundle.js` & `notebook-7.2.0b1/notebook/static/7854.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7866.bundle.js` & `notebook-7.2.0b1/notebook/static/7866.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7884.bundle.js` & `notebook-7.2.0b1/notebook/static/7884.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7900.bundle.js` & `notebook-7.2.0b1/notebook/static/7900.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7906.bundle.js` & `notebook-7.2.0b1/notebook/static/7906.bundle.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
     [7906, 4382], {
         54382: (e, t, r) => {
             r.r(t), r.d(t, {
                 default: () => a
             });
             var n = r(43766),
-                o = r(37057);
+                o = r(28856);
             const c = "jp-mod-searchable",
                 a = [{
                     id: "@jupyter-notebook/documentsearch-extension:notebookShellWidgetListener",
                     requires: [o.INotebookShell, n.ISearchProviderRegistry],
                     autoStart: !0,
                     description: "A plugin to add document search functionalities",
                     activate: (e, t, r) => {
```

### Comparing `notebook-7.2.0b0/notebook/static/792.bundle.js` & `notebook-7.2.0b1/notebook/static/792.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7957.bundle.js` & `notebook-7.2.0b1/notebook/static/7957.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7969.bundle.js` & `notebook-7.2.0b1/notebook/static/7969.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7995.bundle.js` & `notebook-7.2.0b1/notebook/static/7995.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/7997.bundle.js` & `notebook-7.2.0b1/notebook/static/7997.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/79d088064beb3826054f.eot` & `notebook-7.2.0b1/notebook/static/79d088064beb3826054f.eot`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8010.bundle.js` & `notebook-7.2.0b1/notebook/static/8010.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8032.bundle.js` & `notebook-7.2.0b1/notebook/static/8032.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8285.bundle.js` & `notebook-7.2.0b1/notebook/static/8285.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8378.bundle.js` & `notebook-7.2.0b1/notebook/static/8378.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8381.bundle.js` & `notebook-7.2.0b1/notebook/static/8381.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8433.bundle.js` & `notebook-7.2.0b1/notebook/static/8433.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8443.bundle.js` & `notebook-7.2.0b1/notebook/static/8443.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8446.bundle.js` & `notebook-7.2.0b1/notebook/static/8446.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8471.bundle.js` & `notebook-7.2.0b1/notebook/static/8471.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8479.bundle.js` & `notebook-7.2.0b1/notebook/static/8479.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/85.bundle.js` & `notebook-7.2.0b1/notebook/static/85.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8579.bundle.js` & `notebook-7.2.0b1/notebook/static/8579.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11,16 +11,16 @@
                 r = o(9983),
                 d = o(70109),
                 l = o(42782),
                 s = o(17556),
                 c = o(61709),
                 p = o(2277),
                 u = o(60502),
-                g = o(37057),
-                m = o(21481),
+                g = o(28856),
+                m = o(75744),
                 h = o(20998),
                 b = o(2549),
                 f = o(63485);
             const v = new RegExp("/(notebooks|edit)/(.*)"),
                 y = /\.ipynb$/;
             var k;
             ! function(e) {
```

### Comparing `notebook-7.2.0b0/notebook/static/8633.bundle.js` & `notebook-7.2.0b1/notebook/static/8633.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/870673df72e70f87c91a.woff` & `notebook-7.2.0b1/notebook/static/870673df72e70f87c91a.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8768.bundle.js` & `notebook-7.2.0b1/notebook/static/8768.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8771.bundle.js` & `notebook-7.2.0b1/notebook/static/8771.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8781.bundle.js` & `notebook-7.2.0b1/notebook/static/8781.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
                 } catch (t) {
                     throw console.warn(`Failed to create module: package: ${e}; module: ${n}`), t
                 }
             }
             t(72761), t(67417), window.addEventListener("load", (async function() {
                 const e = [t(23955), t(27909), t(98947), t(65529)],
                     n = await Promise.all(e);
-                let r = [t(59123), t(72114), t(38896), t(58524), t(31663), t(64253), t(21113), t(2344).default.filter((({
+                let r = [t(81715), t(29194), t(97793), t(51267), t(73598), t(76933), t(14745), t(2344).default.filter((({
                     id: e
                 }) => ["@jupyterlab/application-extension:commands", "@jupyterlab/application-extension:context-menu", "@jupyterlab/application-extension:faviconbusy", "@jupyterlab/application-extension:router", "@jupyterlab/application-extension:top-bar", "@jupyterlab/application-extension:top-spacer"].includes(e))), t(64209).default.filter((({
                     id: e
                 }) => ["@jupyterlab/apputils-extension:palette", "@jupyterlab/apputils-extension:notification", "@jupyterlab/apputils-extension:sanitizer", "@jupyterlab/apputils-extension:sessionDialogs", "@jupyterlab/apputils-extension:settings", "@jupyterlab/apputils-extension:state", "@jupyterlab/apputils-extension:themes", "@jupyterlab/apputils-extension:themes-palette-menu", "@jupyterlab/apputils-extension:toolbar-registry", "@jupyterlab/apputils-extension:utilityCommands"].includes(e))), t(25763), t(7221).default.filter((({
                     id: e
                 }) => ["@jupyterlab/completer-extension:base-service", "@jupyterlab/completer-extension:inline-completer", "@jupyterlab/completer-extension:inline-completer-factory", "@jupyterlab/completer-extension:inline-history", "@jupyterlab/completer-extension:manager"].includes(e))), t(9135).default.filter((({
                     id: e
@@ -34,20 +34,20 @@
                     id: e
                 }) => ["@jupyterlab/fileeditor-extension:plugin"].includes(e))), t(10253).default.filter((({
                     id: e
                 }) => ["@jupyterlab/help-extension:resources"].includes(e))), t(1542), t(45317), t(24351), t(8997).default.filter((({
                     id: e
                 }) => ["@jupyterlab/mainmenu-extension:plugin"].includes(e))), t(6999), t(82985), t(94415), t(75845).default.filter((({
                     id: e
-                }) => ["@jupyterlab/notebook-extension:cell-executor", "@jupyterlab/notebook-extension:code-console", "@jupyterlab/notebook-extension:export", "@jupyterlab/notebook-extension:factory", "@jupyterlab/notebook-extension:tracker", "@jupyterlab/notebook-extension:widget-factory"].includes(e))), t(60679), t(98269), t(8998), t(79982), t(46030), t(35761), t(88765), t(19199)];
+                }) => ["@jupyterlab/notebook-extension:cell-executor", "@jupyterlab/notebook-extension:code-console", "@jupyterlab/notebook-extension:export", "@jupyterlab/notebook-extension:factory", "@jupyterlab/notebook-extension:tracker", "@jupyterlab/notebook-extension:widget-factory"].includes(e))), t(60679), t(98269), t(8998), t(79982), t(46030), t(3708), t(35761), t(88765), t(19199)];
                 switch (`/${o.PageConfig.getOption("notebookPage")}`) {
                     case "/tree":
                         r = r.concat([t(25950), t(13318).default.filter((({
                             id: e
-                        }) => ["@jupyterlab/filebrowser-extension:browser", "@jupyterlab/filebrowser-extension:download", "@jupyterlab/filebrowser-extension:file-upload-status", "@jupyterlab/filebrowser-extension:open-with", "@jupyterlab/filebrowser-extension:search", "@jupyterlab/filebrowser-extension:share-file"].includes(e))), t(40545), t(73505).default.filter((({
+                        }) => ["@jupyterlab/filebrowser-extension:browser", "@jupyterlab/filebrowser-extension:download", "@jupyterlab/filebrowser-extension:file-upload-status", "@jupyterlab/filebrowser-extension:open-with", "@jupyterlab/filebrowser-extension:search", "@jupyterlab/filebrowser-extension:share-file"].includes(e))), t(40835), t(73505).default.filter((({
                             id: e
                         }) => ["@jupyterlab/running-extension:plugin"].includes(e))), t(65097)]);
                         break;
                     case "/notebooks":
                         r = r.concat([t(51973), t(16557), t(62430).default.filter((({
                             id: e
                         }) => ["@jupyterlab/debugger-extension:config", "@jupyterlab/debugger-extension:main", "@jupyterlab/debugger-extension:notebooks", "@jupyterlab/debugger-extension:service", "@jupyterlab/debugger-extension:sidebar", "@jupyterlab/debugger-extension:sources"].includes(e))), t(51701), t(75845).default.filter((({
@@ -86,16 +86,16 @@
                             autoStart: n.autoStart,
                             enabled: !t,
                             extension: e.__scope__
                         }), t ? i.push(n.id) : yield n
                     }
                 }
                 const p = JSON.parse(o.PageConfig.getOption("federated_extensions")),
-                    b = [],
                     d = [],
+                    b = [],
                     u = [],
                     c = [];
                 (await Promise.allSettled(p.map((async e => (await async function(e, n) {
                     await
                     function(e) {
                         return new Promise(((n, t) => {
                             const o = document.createElement("script");
@@ -103,90 +103,90 @@
                         }))
                     }(e), await t.I("default");
                     const o = window._JUPYTERLAB[n];
                     await o.init(t.S.default)
                 }(`${o.URLExt.join(o.PageConfig.getOption("fullLabextensionsUrl"),e.name,e.load)}`, e.name), e))))).forEach((e => {
                     if ("rejected" === e.status) return void console.error(e.reason);
                     const n = e.value;
-                    n.extension && d.push(a(n.name, n.extension)), n.mimeExtension && u.push(a(n.name, n.mimeExtension)), n.style && !o.PageConfig.Extension.isDisabled(n.name) && c.push(a(n.name, n.style))
+                    n.extension && b.push(a(n.name, n.extension)), n.mimeExtension && u.push(a(n.name, n.mimeExtension)), n.style && !o.PageConfig.Extension.isDisabled(n.name) && c.push(a(n.name, n.style))
                 })), (await Promise.all(r)).forEach((e => {
-                    for (let n of s(e)) b.push(n)
-                })), (await Promise.allSettled(d)).forEach((e => {
+                    for (let n of s(e)) d.push(n)
+                })), (await Promise.allSettled(b)).forEach((e => {
                     if ("fulfilled" === e.status)
-                        for (let n of s(e.value)) b.push(n);
+                        for (let n of s(e.value)) d.push(n);
                     else console.error(e.reason)
                 })), (await Promise.allSettled(u)).forEach((e => {
                     if ("fulfilled" === e.status)
                         for (let t of s(e.value)) n.push(t);
                     else console.error(e.reason)
                 })), (await Promise.allSettled(c)).filter((({
                     status: e
                 }) => "rejected" === e)).forEach((({
                     reason: e
                 }) => {
                     console.error(e)
-                })), o.PageConfig.setOption("allPlugins", '{"/":{"@jupyter-notebook/application-extension":true,"@jupyter-notebook/console-extension":true,"@jupyter-notebook/docmanager-extension":true,"@jupyter-notebook/documentsearch-extension":true,"@jupyter-notebook/help-extension":true,"@jupyter-notebook/notebook-extension":true,"@jupyter-notebook/terminal-extension":true,"@jupyterlab/application-extension":["@jupyterlab/application-extension:commands","@jupyterlab/application-extension:context-menu","@jupyterlab/application-extension:faviconbusy","@jupyterlab/application-extension:router","@jupyterlab/application-extension:top-bar","@jupyterlab/application-extension:top-spacer"],"@jupyterlab/apputils-extension":["@jupyterlab/apputils-extension:palette","@jupyterlab/apputils-extension:notification","@jupyterlab/apputils-extension:sanitizer","@jupyterlab/apputils-extension:sessionDialogs","@jupyterlab/apputils-extension:settings","@jupyterlab/apputils-extension:state","@jupyterlab/apputils-extension:themes","@jupyterlab/apputils-extension:themes-palette-menu","@jupyterlab/apputils-extension:toolbar-registry","@jupyterlab/apputils-extension:utilityCommands"],"@jupyterlab/codemirror-extension":true,"@jupyterlab/completer-extension":["@jupyterlab/completer-extension:base-service","@jupyterlab/completer-extension:inline-completer","@jupyterlab/completer-extension:inline-completer-factory","@jupyterlab/completer-extension:inline-history","@jupyterlab/completer-extension:manager"],"@jupyterlab/console-extension":["@jupyterlab/console-extension:cell-executor","@jupyterlab/console-extension:completer","@jupyterlab/console-extension:factory","@jupyterlab/console-extension:foreign","@jupyterlab/console-extension:tracker"],"@jupyterlab/csvviewer-extension":true,"@jupyterlab/docmanager-extension":["@jupyterlab/docmanager-extension:plugin","@jupyterlab/docmanager-extension:download","@jupyterlab/docmanager-extension:contexts","@jupyterlab/docmanager-extension:manager"],"@jupyterlab/documentsearch-extension":["@jupyterlab/documentsearch-extension:plugin"],"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:factory","@jupyterlab/filebrowser-extension:default-file-browser"],"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:plugin"],"@jupyterlab/help-extension":["@jupyterlab/help-extension:resources"],"@jupyterlab/htmlviewer-extension":true,"@jupyterlab/imageviewer-extension":true,"@jupyterlab/lsp-extension":true,"@jupyterlab/mainmenu-extension":["@jupyterlab/mainmenu-extension:plugin"],"@jupyterlab/markedparser-extension":true,"@jupyterlab/mathjax-extension":true,"@jupyterlab/mermaid-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:cell-executor","@jupyterlab/notebook-extension:code-console","@jupyterlab/notebook-extension:export","@jupyterlab/notebook-extension:factory","@jupyterlab/notebook-extension:tracker","@jupyterlab/notebook-extension:widget-factory"],"@jupyterlab/pluginmanager-extension":true,"@jupyterlab/shortcuts-extension":true,"@jupyterlab/terminal-extension":true,"@jupyterlab/theme-light-extension":true,"@jupyterlab/theme-dark-extension":true,"@jupyterlab/translation-extension":true,"@jupyterlab/ui-components-extension":true,"@jupyterlab/hub-extension":true},"/tree":{"@jupyterlab/extensionmanager-extension":true,"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:browser","@jupyterlab/filebrowser-extension:download","@jupyterlab/filebrowser-extension:file-upload-status","@jupyterlab/filebrowser-extension:open-with","@jupyterlab/filebrowser-extension:search","@jupyterlab/filebrowser-extension:share-file"],"@jupyter-notebook/tree-extension":true,"@jupyterlab/running-extension":["@jupyterlab/running-extension:plugin"],"@jupyterlab/settingeditor-extension":true},"/notebooks":{"@jupyterlab/celltags-extension":true,"@jupyterlab/cell-toolbar-extension":true,"@jupyterlab/debugger-extension":["@jupyterlab/debugger-extension:config","@jupyterlab/debugger-extension:main","@jupyterlab/debugger-extension:notebooks","@jupyterlab/debugger-extension:service","@jupyterlab/debugger-extension:sidebar","@jupyterlab/debugger-extension:sources"],"@jupyterlab/metadataform-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:active-cell-tool","@jupyterlab/notebook-extension:completer","@jupyterlab/notebook-extension:metadata-editor","@jupyterlab/notebook-extension:search","@jupyterlab/notebook-extension:toc","@jupyterlab/notebook-extension:tools","@jupyterlab/notebook-extension:update-raw-mimetype"],"@jupyterlab/toc-extension":["@jupyterlab/toc-extension:registry","@jupyterlab/toc-extension:tracker"],"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:notebooks"]},"/consoles":{"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:consoles"]},"/edit":{"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:completer","@jupyterlab/fileeditor-extension:search"],"@jupyterlab/markdownviewer-extension":true}}');
-                const j = new(0, t(37057).NotebookApp)({
+                })), o.PageConfig.setOption("allPlugins", '{"/":{"@jupyter-notebook/application-extension":true,"@jupyter-notebook/console-extension":true,"@jupyter-notebook/docmanager-extension":true,"@jupyter-notebook/documentsearch-extension":true,"@jupyter-notebook/help-extension":true,"@jupyter-notebook/notebook-extension":true,"@jupyter-notebook/terminal-extension":true,"@jupyterlab/application-extension":["@jupyterlab/application-extension:commands","@jupyterlab/application-extension:context-menu","@jupyterlab/application-extension:faviconbusy","@jupyterlab/application-extension:router","@jupyterlab/application-extension:top-bar","@jupyterlab/application-extension:top-spacer"],"@jupyterlab/apputils-extension":["@jupyterlab/apputils-extension:palette","@jupyterlab/apputils-extension:notification","@jupyterlab/apputils-extension:sanitizer","@jupyterlab/apputils-extension:sessionDialogs","@jupyterlab/apputils-extension:settings","@jupyterlab/apputils-extension:state","@jupyterlab/apputils-extension:themes","@jupyterlab/apputils-extension:themes-palette-menu","@jupyterlab/apputils-extension:toolbar-registry","@jupyterlab/apputils-extension:utilityCommands"],"@jupyterlab/codemirror-extension":true,"@jupyterlab/completer-extension":["@jupyterlab/completer-extension:base-service","@jupyterlab/completer-extension:inline-completer","@jupyterlab/completer-extension:inline-completer-factory","@jupyterlab/completer-extension:inline-history","@jupyterlab/completer-extension:manager"],"@jupyterlab/console-extension":["@jupyterlab/console-extension:cell-executor","@jupyterlab/console-extension:completer","@jupyterlab/console-extension:factory","@jupyterlab/console-extension:foreign","@jupyterlab/console-extension:tracker"],"@jupyterlab/csvviewer-extension":true,"@jupyterlab/docmanager-extension":["@jupyterlab/docmanager-extension:plugin","@jupyterlab/docmanager-extension:download","@jupyterlab/docmanager-extension:contexts","@jupyterlab/docmanager-extension:manager"],"@jupyterlab/documentsearch-extension":["@jupyterlab/documentsearch-extension:plugin"],"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:factory","@jupyterlab/filebrowser-extension:default-file-browser"],"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:plugin"],"@jupyterlab/help-extension":["@jupyterlab/help-extension:resources"],"@jupyterlab/htmlviewer-extension":true,"@jupyterlab/imageviewer-extension":true,"@jupyterlab/lsp-extension":true,"@jupyterlab/mainmenu-extension":["@jupyterlab/mainmenu-extension:plugin"],"@jupyterlab/markedparser-extension":true,"@jupyterlab/mathjax-extension":true,"@jupyterlab/mermaid-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:cell-executor","@jupyterlab/notebook-extension:code-console","@jupyterlab/notebook-extension:export","@jupyterlab/notebook-extension:factory","@jupyterlab/notebook-extension:tracker","@jupyterlab/notebook-extension:widget-factory"],"@jupyterlab/pluginmanager-extension":true,"@jupyterlab/shortcuts-extension":true,"@jupyterlab/terminal-extension":true,"@jupyterlab/theme-light-extension":true,"@jupyterlab/theme-dark-extension":true,"@jupyterlab/theme-dark-high-contrast-extension":true,"@jupyterlab/translation-extension":true,"@jupyterlab/ui-components-extension":true,"@jupyterlab/hub-extension":true},"/tree":{"@jupyterlab/extensionmanager-extension":true,"@jupyterlab/filebrowser-extension":["@jupyterlab/filebrowser-extension:browser","@jupyterlab/filebrowser-extension:download","@jupyterlab/filebrowser-extension:file-upload-status","@jupyterlab/filebrowser-extension:open-with","@jupyterlab/filebrowser-extension:search","@jupyterlab/filebrowser-extension:share-file"],"@jupyter-notebook/tree-extension":true,"@jupyterlab/running-extension":["@jupyterlab/running-extension:plugin"],"@jupyterlab/settingeditor-extension":true},"/notebooks":{"@jupyterlab/celltags-extension":true,"@jupyterlab/cell-toolbar-extension":true,"@jupyterlab/debugger-extension":["@jupyterlab/debugger-extension:config","@jupyterlab/debugger-extension:main","@jupyterlab/debugger-extension:notebooks","@jupyterlab/debugger-extension:service","@jupyterlab/debugger-extension:sidebar","@jupyterlab/debugger-extension:sources"],"@jupyterlab/metadataform-extension":true,"@jupyterlab/notebook-extension":["@jupyterlab/notebook-extension:active-cell-tool","@jupyterlab/notebook-extension:completer","@jupyterlab/notebook-extension:metadata-editor","@jupyterlab/notebook-extension:search","@jupyterlab/notebook-extension:toc","@jupyterlab/notebook-extension:tools","@jupyterlab/notebook-extension:update-raw-mimetype"],"@jupyterlab/toc-extension":["@jupyterlab/toc-extension:registry","@jupyterlab/toc-extension:tracker"],"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:notebooks"]},"/consoles":{"@jupyterlab/tooltip-extension":["@jupyterlab/tooltip-extension:manager","@jupyterlab/tooltip-extension:consoles"]},"/edit":{"@jupyterlab/fileeditor-extension":["@jupyterlab/fileeditor-extension:completer","@jupyterlab/fileeditor-extension:search"],"@jupyterlab/markdownviewer-extension":true}}');
+                const j = new(0, t(28856).NotebookApp)({
                     mimeExtensions: n,
                     availablePlugins: l
                 });
-                j.registerPluginModules(b), "true" === (o.PageConfig.getOption("exposeAppInBrowser") || "").toLowerCase() && (window.jupyterapp = j), await j.start()
+                j.registerPluginModules(d), "true" === (o.PageConfig.getOption("exposeAppInBrowser") || "").toLowerCase() && (window.jupyterapp = j), await j.start()
             }))
         },
         72761: (e, n, t) => {
             "use strict";
             t.r(n), t(71818), t(70022), t(26238);
             var o = t(94830),
                 a = t.n(o),
                 r = t(80592),
                 i = t.n(r),
                 l = t(99763),
                 s = t.n(l),
                 p = t(28915),
-                b = t.n(p),
-                d = t(80366),
-                u = t.n(d),
+                d = t.n(p),
+                b = t(80366),
+                u = t.n(b),
                 c = t(17352),
                 j = t.n(c),
                 y = t(26633),
                 m = {};
-            m.styleTagTransform = j(), m.setAttributes = b(), m.insert = s().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = u(), a()(y.Z, m), y.Z && y.Z.locals && y.Z.locals;
+            m.styleTagTransform = j(), m.setAttributes = d(), m.insert = s().bind(null, "head"), m.domAPI = i(), m.insertStyleElement = u(), a()(y.Z, m), y.Z && y.Z.locals && y.Z.locals;
             var x = t(93862),
                 g = {};
-            g.styleTagTransform = j(), g.setAttributes = b(), g.insert = s().bind(null, "head"), g.domAPI = i(), g.insertStyleElement = u(), a()(x.Z, g), x.Z && x.Z.locals && x.Z.locals, t(20959);
+            g.styleTagTransform = j(), g.setAttributes = d(), g.insert = s().bind(null, "head"), g.domAPI = i(), g.insertStyleElement = u(), a()(x.Z, g), x.Z && x.Z.locals && x.Z.locals, t(20959);
             var h = t(58027),
                 f = {};
-            f.styleTagTransform = j(), f.setAttributes = b(), f.insert = s().bind(null, "head"), f.domAPI = i(), f.insertStyleElement = u(), a()(h.Z, f), h.Z && h.Z.locals && h.Z.locals;
+            f.styleTagTransform = j(), f.setAttributes = d(), f.insert = s().bind(null, "head"), f.domAPI = i(), f.insertStyleElement = u(), a()(h.Z, f), h.Z && h.Z.locals && h.Z.locals;
             var k = t(99776),
                 A = {};
-            A.styleTagTransform = j(), A.setAttributes = b(), A.insert = s().bind(null, "head"), A.domAPI = i(), A.insertStyleElement = u(), a()(k.Z, A), k.Z && k.Z.locals && k.Z.locals;
+            A.styleTagTransform = j(), A.setAttributes = d(), A.insert = s().bind(null, "head"), A.domAPI = i(), A.insertStyleElement = u(), a()(k.Z, A), k.Z && k.Z.locals && k.Z.locals;
             var w = t(64399),
                 v = {};
-            v.styleTagTransform = j(), v.setAttributes = b(), v.insert = s().bind(null, "head"), v.domAPI = i(), v.insertStyleElement = u(), a()(w.Z, v), w.Z && w.Z.locals && w.Z.locals;
+            v.styleTagTransform = j(), v.setAttributes = d(), v.insert = s().bind(null, "head"), v.domAPI = i(), v.insertStyleElement = u(), a()(w.Z, v), w.Z && w.Z.locals && w.Z.locals;
             var T = t(11112),
                 P = {};
-            P.styleTagTransform = j(), P.setAttributes = b(), P.insert = s().bind(null, "head"), P.domAPI = i(), P.insertStyleElement = u(), a()(T.Z, P), T.Z && T.Z.locals && T.Z.locals;
+            P.styleTagTransform = j(), P.setAttributes = d(), P.insert = s().bind(null, "head"), P.domAPI = i(), P.insertStyleElement = u(), a()(T.Z, P), T.Z && T.Z.locals && T.Z.locals;
             var Z = t(49482),
                 B = {};
-            B.styleTagTransform = j(), B.setAttributes = b(), B.insert = s().bind(null, "head"), B.domAPI = i(), B.insertStyleElement = u(), a()(Z.Z, B), Z.Z && Z.Z.locals && Z.Z.locals;
+            B.styleTagTransform = j(), B.setAttributes = d(), B.insert = s().bind(null, "head"), B.domAPI = i(), B.insertStyleElement = u(), a()(Z.Z, B), Z.Z && Z.Z.locals && Z.Z.locals;
             var S = t(71564),
                 C = {};
-            C.styleTagTransform = j(), C.setAttributes = b(), C.insert = s().bind(null, "head"), C.domAPI = i(), C.insertStyleElement = u(), a()(S.Z, C), S.Z && S.Z.locals && S.Z.locals;
+            C.styleTagTransform = j(), C.setAttributes = d(), C.insert = s().bind(null, "head"), C.domAPI = i(), C.insertStyleElement = u(), a()(S.Z, C), S.Z && S.Z.locals && S.Z.locals;
             var N = t(8173),
                 E = {};
-            E.styleTagTransform = j(), E.setAttributes = b(), E.insert = s().bind(null, "head"), E.domAPI = i(), E.insertStyleElement = u(), a()(N.Z, E), N.Z && N.Z.locals && N.Z.locals, t(40360);
+            E.styleTagTransform = j(), E.setAttributes = d(), E.insert = s().bind(null, "head"), E.domAPI = i(), E.insertStyleElement = u(), a()(N.Z, E), N.Z && N.Z.locals && N.Z.locals, t(40360);
             var D = t(30546),
                 z = {};
-            z.styleTagTransform = j(), z.setAttributes = b(), z.insert = s().bind(null, "head"), z.domAPI = i(), z.insertStyleElement = u(), a()(D.Z, z), D.Z && D.Z.locals && D.Z.locals;
+            z.styleTagTransform = j(), z.setAttributes = d(), z.insert = s().bind(null, "head"), z.domAPI = i(), z.insertStyleElement = u(), a()(D.Z, z), D.Z && D.Z.locals && D.Z.locals;
             var F = t(94623),
                 L = {};
-            L.styleTagTransform = j(), L.setAttributes = b(), L.insert = s().bind(null, "head"), L.domAPI = i(), L.insertStyleElement = u(), a()(F.Z, L), F.Z && F.Z.locals && F.Z.locals;
+            L.styleTagTransform = j(), L.setAttributes = d(), L.insert = s().bind(null, "head"), L.domAPI = i(), L.insertStyleElement = u(), a()(F.Z, L), F.Z && F.Z.locals && F.Z.locals;
             var M = t(99402),
                 O = {};
-            O.styleTagTransform = j(), O.setAttributes = b(), O.insert = s().bind(null, "head"), O.domAPI = i(), O.insertStyleElement = u(), a()(M.Z, O), M.Z && M.Z.locals && M.Z.locals, t(32723), t(82649), t(15491), t(92645), t(18934), t(24017), t(72867), t(93751), t(75617), t(91532), t(20603), t(17066), t(39380), t(9755), t(82164), t(94938), t(53555), t(86258), t(11575), t(10887), t(26449), t(3727), t(97635), t(16856), t(46165), t(8604), t(26053), t(84221), t(53927), t(67074), t(47275), t(58068), t(41346), t(74768), t(65315), t(87635), t(37609), t(49733), t(40745)
+            O.styleTagTransform = j(), O.setAttributes = d(), O.insert = s().bind(null, "head"), O.domAPI = i(), O.insertStyleElement = u(), a()(M.Z, O), M.Z && M.Z.locals && M.Z.locals, t(32723), t(82649), t(15491), t(92645), t(18934), t(24017), t(72867), t(93751), t(75617), t(91532), t(20603), t(17066), t(39380), t(9755), t(82164), t(94938), t(53555), t(86258), t(11575), t(10887), t(26449), t(3727), t(97635), t(16856), t(46165), t(8604), t(26053), t(84221), t(53927), t(67074), t(47275), t(58068), t(41346), t(74768), t(65315), t(87635), t(37609), t(49733), t(40745)
         },
         58027: (e, n, t) => {
             "use strict";
             t.d(n, {
                 Z: () => l
             });
             var o = t(66846),
@@ -275,15 +275,15 @@
             });
             var o = t(66846),
                 a = t.n(o),
                 r = t(11368),
                 i = t.n(r),
                 l = t(99686),
                 s = i()(a());
-            s.i(l.Z), s.push([e.id, "/*-----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n|\n| Distributed under the terms of the Modified BSD License.\n|----------------------------------------------------------------------------*/\n\n/**\n  Document oriented look for the notebook.\n  This includes changes to the look and feel of the JupyterLab Notebook\n  component like:\n  - scrollbar to the right of the page\n  - drop shadow on the notebook\n  - smaller empty space at the bottom of the notebook\n  - compact view on mobile\n*/\n\n/* Keep the notebook centered on the page */\n\nbody[data-notebook='notebooks'] .jp-NotebookPanel-toolbar {\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer {\n  padding-top: unset;\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(\n    calc(\n        100% - var(--jp-notebook-max-width) - var(--jp-notebook-padding-offset)\n      ) * 0.5\n  );\n  background: var(--jp-layout-color2);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-inner {\n  margin-top: var(--jp-notebook-toolbar-margin-bottom);\n}\n\nbody[data-notebook='notebooks'] .jp-Notebook-cell {\n  background: var(--jp-layout-color0);\n  padding-left: calc(2 * var(--jp-cell-padding));\n  padding-right: calc(2 * var(--jp-cell-padding));\n}\n\n/* Empty space at the bottom of the notebook (similar to classic) */\nbody[data-notebook='notebooks'] .jp-Notebook.jp-mod-scrollPastEnd::after {\n  min-height: 100px;\n}\n\n/* Fix background colors */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer > * {\n  background: var(--jp-layout-color0);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-commandMode\n  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {\n  background: var(--jp-layout-color0) !important;\n}\n\n/**\n  Extra padding to the first and and last cell of the notebook.\n  TODO: revisit when https://github.com/jupyterlab/jupyterlab/issues/13151 is fixed\n*/\n.jp-Notebook-cell[data-windowed-list-index='0'] {\n  padding-top: calc(2 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport > *:last-child {\n  padding-bottom: calc(2 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Cell toolbar adjustments */\n\nbody[data-notebook='notebooks'] .jp-cell-toolbar {\n  background: unset;\n  box-shadow: unset;\n}\n\nbody[data-notebook='notebooks']\n  .jp-RawCell[data-windowed-list-index='0']\n  .jp-cell-toolbar,\nbody[data-notebook='notebooks']\n  .jp-MarkdownCell[data-windowed-list-index='0']\n  .jp-cell-toolbar {\n  top: calc(2 * var(--jp-notebook-padding));\n}\n\n/** first code cell on mobile\n    (keep the selector above the media query)\n*/\nbody[data-notebook='notebooks']\n  .jp-CodeCell[data-windowed-list-index='0']\n  .jp-cell-toolbar {\n  top: unset;\n}\n\n@media only screen and (max-width: 760px) {\n  /* first code cell on mobile */\n  body[data-notebook='notebooks']\n    .jp-CodeCell[data-windowed-list-index='0']\n    .jp-cell-toolbar {\n    top: var(--jp-notebook-padding);\n  }\n\n  body[data-notebook='notebooks'] .jp-MarkdownCell .jp-cell-toolbar,\n  body[data-notebook='notebooks'] .jp-RawCell .jp-cell-toolbar {\n    top: calc(0.5 * var(--jp-notebook-padding));\n  }\n}\n\n/* Tweak the notebook footer (to add a new cell) */\nbody[data-notebook='notebooks'] .jp-Notebook-footer {\n  width: 100%;\n  margin-left: unset;\n  background: unset;\n}\n\n/* Mobile View */\n\nbody[data-format='mobile'] .jp-NotebookCheckpoint {\n  display: none;\n}\n\nbody[data-format='mobile'] .jp-WindowedPanel-outer > *:first-child {\n  margin-top: 0;\n}\n\nbody[data-format='mobile'] .jp-ToolbarButton .jp-DebuggerBugButton {\n  display: none;\n}\n\n/* Virtual Notebook fixes */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport {\n  background: var(--jp-layout-color0);\n  padding: unset;\n}\n\n/* Notebook box shadow */\n\nbody[data-notebook='notebooks']\n  .jp-WindowedPanel-outer\n  > *:first-child:not(:last-child) {\n  box-shadow: var(--jp-elevation-z4);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  > *:first-child:last-child::before {\n  content: '';\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n  box-shadow: 0px 0px 12px 1px var(--jp-shadow-umbra-color);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::after,\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Additional customizations of the components on the notebook page */\n\n.jp-NotebookKernelLogo {\n  flex: 0 0 auto;\n  display: flex;\n  align-items: center;\n  text-align: center;\n  margin-right: 8px;\n}\n\n.jp-NotebookKernelLogo img {\n  max-width: 28px;\n  max-height: 28px;\n  display: flex;\n}\n\n.jp-NotebookKernelStatus {\n  margin: 0;\n  font-weight: normal;\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: var(--jp-private-title-panel-height);\n  padding-left: var(--jp-kernel-status-padding);\n  padding-right: var(--jp-kernel-status-padding);\n}\n\n.jp-NotebookKernelStatus-error {\n  background-color: var(--jp-error-color0);\n}\n\n.jp-NotebookKernelStatus-warn {\n  background-color: var(--jp-warn-color0);\n}\n\n.jp-NotebookKernelStatus-info {\n  background-color: var(--jp-info-color0);\n}\n\n.jp-NotebookKernelStatus-fade {\n  animation: 0.5s fade-out forwards;\n}\n\n.jp-NotebookTrustedStatus {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  margin-top: 4px;\n  margin-bottom: 4px;\n  border: solid 1px var(--jp-border-color2);\n  cursor: help;\n}\n\n.jp-NotebookTrustedStatus-not-trusted {\n  cursor: pointer;\n}\n\n@keyframes fade-out {\n  0% {\n    opacity: 1;\n  }\n  100% {\n    opacity: 0;\n  }\n}\n\n#jp-title h1 {\n  cursor: pointer;\n  font-size: 18px;\n  margin: 0;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n#jp-title h1:hover {\n  background: var(--jp-layout-color2);\n}\n\n.jp-NotebookCheckpoint {\n  font-size: 14px;\n  margin-left: 5px;\n  margin-right: 5px;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n.jp-skiplink {\n  position: absolute;\n  top: -100em;\n}\n\n.jp-skiplink:focus-within {\n  position: absolute;\n  z-index: 10000;\n  top: 0;\n  left: 46%;\n  margin: 0 auto;\n  padding: 1em;\n  width: 15%;\n  box-shadow: var(--jp-elevation-z4);\n  border-radius: 4px;\n  background: var(--jp-layout-color0);\n  text-align: center;\n}\n\n.jp-skiplink:focus-within a {\n  text-decoration: underline;\n  color: var(--jp-content-link-color);\n}\n", ""]);
+            s.i(l.Z), s.push([e.id, "/*-----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n|\n| Distributed under the terms of the Modified BSD License.\n|----------------------------------------------------------------------------*/\n\n/**\n  Document oriented look for the notebook.\n  This includes changes to the look and feel of the JupyterLab Notebook\n  component like:\n  - scrollbar to the right of the page\n  - drop shadow on the notebook\n  - smaller empty space at the bottom of the notebook\n  - compact view on mobile\n*/\n\n/* Keep the notebook centered on the page */\n\nbody[data-notebook='notebooks'] .jp-NotebookPanel-toolbar {\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer {\n  padding-top: unset;\n  padding-left: calc(calc(100% - var(--jp-notebook-max-width)) * 0.5);\n  padding-right: calc(\n    calc(\n        100% - var(--jp-notebook-max-width) - var(--jp-notebook-padding-offset)\n      ) * 0.5\n  );\n  background: var(--jp-layout-color2);\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-inner {\n  margin-top: var(--jp-notebook-toolbar-margin-bottom);\n}\n\nbody[data-notebook='notebooks'] .jp-Notebook-cell {\n  background: var(--jp-layout-color0);\n  padding-left: calc(2 * var(--jp-cell-padding));\n  padding-right: calc(2 * var(--jp-cell-padding));\n}\n\n/* Empty space at the bottom of the notebook (similar to classic) */\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-scrollPastEnd\n  .jp-WindowedPanel-outer::after {\n  min-height: 100px;\n}\n\n/* Workaround for disabling the full windowing mode */\nbody[data-notebook='notebooks']\n  .jp-Toolbar-item[data-jp-item-name='scrollbar'] {\n  display: none;\n}\n\n/* Fix background colors */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-outer > * {\n  background: var(--jp-layout-color0);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook.jp-mod-commandMode\n  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {\n  background: var(--jp-layout-color0) !important;\n}\n\n/**\n  Extra padding to the first and and last cell of the notebook.\n  TODO: revisit when https://github.com/jupyterlab/jupyterlab/issues/13151 is fixed\n*/\n.jp-Notebook-cell[data-windowed-list-index='0'] {\n  padding-top: calc(2 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport > *:last-child {\n  padding-bottom: calc(2 * var(--jp-notebook-padding));\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Cell toolbar adjustments */\n\nbody[data-notebook='notebooks'] .jp-cell-toolbar {\n  background: unset;\n  box-shadow: unset;\n}\n\nbody[data-notebook='notebooks']\n  .jp-RawCell[data-windowed-list-index='0']\n  .jp-cell-toolbar,\nbody[data-notebook='notebooks']\n  .jp-MarkdownCell[data-windowed-list-index='0']\n  .jp-cell-toolbar {\n  top: calc(2 * var(--jp-notebook-padding));\n}\n\n/** first code cell on mobile\n    (keep the selector above the media query)\n*/\nbody[data-notebook='notebooks']\n  .jp-CodeCell[data-windowed-list-index='0']\n  .jp-cell-toolbar {\n  top: unset;\n}\n\n@media only screen and (max-width: 760px) {\n  /* first code cell on mobile */\n  body[data-notebook='notebooks']\n    .jp-CodeCell[data-windowed-list-index='0']\n    .jp-cell-toolbar {\n    top: var(--jp-notebook-padding);\n  }\n\n  body[data-notebook='notebooks'] .jp-MarkdownCell .jp-cell-toolbar,\n  body[data-notebook='notebooks'] .jp-RawCell .jp-cell-toolbar {\n    top: calc(0.5 * var(--jp-notebook-padding));\n  }\n}\n\n/* Tweak the notebook footer (to add a new cell) */\nbody[data-notebook='notebooks'] .jp-Notebook-footer {\n  width: 100%;\n  margin-left: unset;\n  background: unset;\n}\n\n/* Mobile View */\n\nbody[data-format='mobile'] .jp-NotebookCheckpoint {\n  display: none;\n}\n\nbody[data-format='mobile'] .jp-WindowedPanel-outer > *:first-child {\n  margin-top: 0;\n}\n\nbody[data-format='mobile'] .jp-ToolbarButton .jp-DebuggerBugButton {\n  display: none;\n}\n\n/* Virtual Notebook fixes */\n\nbody[data-notebook='notebooks'] .jp-WindowedPanel-viewport {\n  background: var(--jp-layout-color0);\n  padding: unset;\n}\n\n/* Notebook box shadow */\n\nbody[data-notebook='notebooks']\n  .jp-WindowedPanel-outer\n  > *:first-child:not(:last-child) {\n  box-shadow: var(--jp-elevation-z4);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  > *:first-child:last-child::before {\n  content: '';\n  position: absolute;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  right: 0;\n  box-shadow: 0px 0px 12px 1px var(--jp-shadow-umbra-color);\n}\n\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::after,\nbody[data-notebook='notebooks']\n  .jp-Notebook\n  .jp-Notebook-cell:not(:first-child)::before {\n  content: ' ';\n  height: 100%;\n  position: absolute;\n  top: 0;\n  width: 11px;\n}\n\n/* Additional customizations of the components on the notebook page */\n\n.jp-NotebookKernelLogo {\n  flex: 0 0 auto;\n  display: flex;\n  align-items: center;\n  text-align: center;\n  margin-right: 8px;\n}\n\n.jp-NotebookKernelLogo img {\n  max-width: 28px;\n  max-height: 28px;\n  display: flex;\n}\n\n.jp-NotebookKernelStatus {\n  margin: 0;\n  font-weight: normal;\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: var(--jp-private-title-panel-height);\n  padding-left: var(--jp-kernel-status-padding);\n  padding-right: var(--jp-kernel-status-padding);\n}\n\n.jp-NotebookKernelStatus-error {\n  background-color: var(--jp-error-color0);\n}\n\n.jp-NotebookKernelStatus-warn {\n  background-color: var(--jp-warn-color0);\n}\n\n.jp-NotebookKernelStatus-info {\n  background-color: var(--jp-info-color0);\n}\n\n.jp-NotebookKernelStatus-fade {\n  animation: 0.5s fade-out forwards;\n}\n\n.jp-NotebookTrustedStatus {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  margin-top: 4px;\n  margin-bottom: 4px;\n  border: solid 1px var(--jp-border-color2);\n  cursor: help;\n}\n\n.jp-NotebookTrustedStatus-not-trusted {\n  cursor: pointer;\n}\n\n@keyframes fade-out {\n  0% {\n    opacity: 1;\n  }\n  100% {\n    opacity: 0;\n  }\n}\n\n#jp-title h1 {\n  cursor: pointer;\n  font-size: 18px;\n  margin: 0;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n#jp-title h1:hover {\n  background: var(--jp-layout-color2);\n}\n\n.jp-NotebookCheckpoint {\n  font-size: 14px;\n  margin-left: 5px;\n  margin-right: 5px;\n  font-weight: normal;\n  color: var(--jp-ui-font-color0);\n  font-family: var(--jp-ui-font-family);\n  line-height: calc(1.5 * var(--jp-private-title-panel-height));\n  text-overflow: ellipsis;\n  overflow: hidden;\n  white-space: nowrap;\n}\n\n.jp-skiplink {\n  position: absolute;\n  top: -100em;\n}\n\n.jp-skiplink:focus-within {\n  position: absolute;\n  z-index: 10000;\n  top: 0;\n  left: 46%;\n  margin: 0 auto;\n  padding: 1em;\n  width: 15%;\n  box-shadow: var(--jp-elevation-z4);\n  border-radius: 4px;\n  background: var(--jp-layout-color0);\n  text-align: center;\n}\n\n.jp-skiplink:focus-within a {\n  text-decoration: underline;\n  color: var(--jp-content-link-color);\n}\n", ""]);
             const p = s
         },
         99686: (e, n, t) => {
             "use strict";
             t.d(n, {
                 Z: () => l
             });
```

### Comparing `notebook-7.2.0b0/notebook/static/8801.bundle.js` & `notebook-7.2.0b1/notebook/static/8801.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/883.bundle.js` & `notebook-7.2.0b1/notebook/static/883.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8845.bundle.js` & `notebook-7.2.0b1/notebook/static/8845.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8845.bundle.js.LICENSE.txt` & `notebook-7.2.0b1/notebook/static/8845.bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8875.bundle.js` & `notebook-7.2.0b1/notebook/static/1650.bundle.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunk_JUPYTERLAB_CORE_OUTPUT = self.webpackChunk_JUPYTERLAB_CORE_OUTPUT || []).push([
-    [8875, 1650], {
+    [1650, 8875], {
         71650: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => s
             });
             var n = o(9983),
                 a = o(70109),
-                i = o(37057),
+                i = o(28856),
                 d = o(81997);
             const s = [{
                 id: "@jupyter-notebook/docmanager-extension:opener",
                 autoStart: !0,
                 optional: [i.INotebookPathOpener, i.INotebookShell],
                 provides: a.IDocumentWidgetOpener,
                 description: "Open documents in a new browser tab",
```

### Comparing `notebook-7.2.0b0/notebook/static/88b98cad3688915e50da.woff` & `notebook-7.2.0b1/notebook/static/88b98cad3688915e50da.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8907.bundle.js` & `notebook-7.2.0b1/notebook/static/8907.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8928.bundle.js` & `notebook-7.2.0b1/notebook/static/8928.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8929.bundle.js` & `notebook-7.2.0b1/notebook/static/8929.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/893.bundle.js` & `notebook-7.2.0b1/notebook/static/893.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8937.bundle.js` & `notebook-7.2.0b1/notebook/static/8937.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8979.bundle.js` & `notebook-7.2.0b1/notebook/static/8979.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8983.bundle.js` & `notebook-7.2.0b1/notebook/static/8983.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/899.bundle.js` & `notebook-7.2.0b1/notebook/static/899.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8ea8791754915a898a31.woff2` & `notebook-7.2.0b1/notebook/static/8ea8791754915a898a31.woff2`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/8ea8dbb1b02e6f730f55.woff` & `notebook-7.2.0b1/notebook/static/8ea8dbb1b02e6f730f55.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/901.bundle.js` & `notebook-7.2.0b1/notebook/static/901.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9022.bundle.js` & `notebook-7.2.0b1/notebook/static/9022.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9037.bundle.js` & `notebook-7.2.0b1/notebook/static/9037.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/906.bundle.js` & `notebook-7.2.0b1/notebook/static/906.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9060.bundle.js` & `notebook-7.2.0b1/notebook/static/9060.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9068.bundle.js` & `notebook-7.2.0b1/notebook/static/9068.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/911.bundle.js` & `notebook-7.2.0b1/notebook/static/911.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9136.bundle.js` & `notebook-7.2.0b1/notebook/static/9136.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9151.bundle.js` & `notebook-7.2.0b1/notebook/static/9151.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9161.bundle.js` & `notebook-7.2.0b1/notebook/static/9161.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9222.bundle.js` & `notebook-7.2.0b1/notebook/static/9222.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9233.bundle.js` & `notebook-7.2.0b1/notebook/static/9233.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9234.bundle.js` & `notebook-7.2.0b1/notebook/static/9234.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9239.bundle.js` & `notebook-7.2.0b1/notebook/static/9239.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9250.bundle.js` & `notebook-7.2.0b1/notebook/static/9250.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9268.bundle.js` & `notebook-7.2.0b1/notebook/static/9268.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9331.bundle.js` & `notebook-7.2.0b1/notebook/static/9331.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9335.bundle.js` & `notebook-7.2.0b1/notebook/static/9335.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9341.bundle.js` & `notebook-7.2.0b1/notebook/static/9341.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9380.bundle.js` & `notebook-7.2.0b1/notebook/static/9380.bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
         19380: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => c
             });
             var a = o(95297),
                 n = o(17556),
                 r = o(60502),
-                u = o(21481),
+                u = o(75744),
                 l = o(78156);
             const s = [{
                 text: "About Jupyter",
                 url: "https://jupyter.org"
             }, {
                 text: "Markdown Reference",
                 url: "https://commonmark.org/help/"
```

### Comparing `notebook-7.2.0b0/notebook/static/9425.bundle.js` & `notebook-7.2.0b1/notebook/static/9425.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9558.bundle.js` & `notebook-7.2.0b1/notebook/static/9558.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9604.bundle.js` & `notebook-7.2.0b1/notebook/static/9604.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9605.bundle.js` & `notebook-7.2.0b1/notebook/static/9605.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9638.bundle.js` & `notebook-7.2.0b1/notebook/static/9638.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9674eb1bd55047179038.svg` & `notebook-7.2.0b1/notebook/static/9674eb1bd55047179038.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9676.bundle.js` & `notebook-7.2.0b1/notebook/static/9676.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9680.bundle.js` & `notebook-7.2.0b1/notebook/static/9680.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9685.bundle.js` & `notebook-7.2.0b1/notebook/static/9685.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9752.bundle.js` & `notebook-7.2.0b1/notebook/static/9752.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9799.bundle.js` & `notebook-7.2.0b1/notebook/static/9799.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9821.bundle.js` & `notebook-7.2.0b1/notebook/static/9821.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9834b82ad26e2a37583d.woff2` & `notebook-7.2.0b1/notebook/static/9834b82ad26e2a37583d.woff2`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9852.bundle.js` & `notebook-7.2.0b1/notebook/static/9852.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/9866.bundle.js` & `notebook-7.2.0b1/notebook/static/9866.bundle.js`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/a009bea404f7a500ded4.woff` & `notebook-7.2.0b1/notebook/static/a009bea404f7a500ded4.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/a3b9817780214caf01e8.svg` & `notebook-7.2.0b1/notebook/static/a3b9817780214caf01e8.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/af04542b29eaac04550a.woff` & `notebook-7.2.0b1/notebook/static/af04542b29eaac04550a.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/af6397503fcefbd61397.ttf` & `notebook-7.2.0b1/notebook/static/af6397503fcefbd61397.ttf`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/af96f67d7accf5fd2a4a.woff` & `notebook-7.2.0b1/notebook/static/af96f67d7accf5fd2a4a.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/b418136e3b384baaadec.woff` & `notebook-7.2.0b1/notebook/static/b418136e3b384baaadec.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/be0a084962d8066884f7.svg` & `notebook-7.2.0b1/notebook/static/be0a084962d8066884f7.svg`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/bundle.js` & `notebook-7.2.0b1/notebook/static/bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     var e, t, a, l, r, n, o, i, s, u, b, m, h, p, d, f, P, y, j, c, g = {
             37559: (e, t, a) => {
-                Promise.all([a.e(9136), a.e(9983), a.e(7057), a.e(2123), a.e(8781)]).then(a.bind(a, 60880))
+                Promise.all([a.e(9136), a.e(9983), a.e(8856), a.e(2123), a.e(8781)]).then(a.bind(a, 60880))
             },
             68444: (e, t, a) => {
                 a.p = function(e) {
                     let t = Object.create(null);
                     if ("undefined" != typeof document && document) {
                         const e = document.getElementById("jupyter-config-data");
                         e && (t = JSON.parse(e.textContent || "{}"))
@@ -110,15 +110,15 @@
                         (!i || !i.loaded && (!l != !i.eager ? l : o > i.from)) && (r[t] = {
                             get: a,
                             from: o,
                             eager: !!l
                         })
                     },
                     s = [];
-                return "default" === a && (i("@codemirror/commands", "6.3.3", (() => Promise.all([v.e(7450), v.e(3546), v.e(9843), v.e(9352), v.e(7592)]).then((() => () => v(67450))))), i("@codemirror/lang-markdown", "6.2.4", (() => Promise.all([v.e(5850), v.e(9239), v.e(9799), v.e(7866), v.e(6271), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(7592)]).then((() => () => v(76271))))), i("@codemirror/language", "6.10.1", (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))), i("@codemirror/search", "6.5.6", (() => Promise.all([v.e(5261), v.e(3546), v.e(9843)]).then((() => () => v(25261))))), i("@codemirror/state", "6.4.1", (() => v.e(2323).then((() => () => v(92323))))), i("@codemirror/view", "6.26.1", (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))), i("@jupyter-notebook/application-extension", "7.2.0-beta.0", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(2782), v.e(7556), v.e(109), v.e(6985), v.e(7057), v.e(1481), v.e(8579)]).then((() => () => v(88579))))), i("@jupyter-notebook/application", "7.2.0-beta.0", (() => Promise.all([v.e(901), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(5007), v.e(1709), v.e(2549), v.e(7934), v.e(2782), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))), i("@jupyter-notebook/console-extension", "7.2.0-beta.0", (() => Promise.all([v.e(3625), v.e(9983), v.e(5007), v.e(6985), v.e(7057), v.e(4645)]).then((() => () => v(94645))))), i("@jupyter-notebook/docmanager-extension", "7.2.0-beta.0", (() => Promise.all([v.e(1997), v.e(9983), v.e(109), v.e(7057), v.e(1650)]).then((() => () => v(71650))))), i("@jupyter-notebook/documentsearch-extension", "7.2.0-beta.0", (() => Promise.all([v.e(3766), v.e(7057), v.e(4382)]).then((() => () => v(54382))))), i("@jupyter-notebook/help-extension", "7.2.0-beta.0", (() => Promise.all([v.e(502), v.e(8713), v.e(8156), v.e(7556), v.e(1481), v.e(9380)]).then((() => () => v(19380))))), i("@jupyter-notebook/notebook-extension", "7.2.0-beta.0", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(9983), v.e(2277), v.e(7934), v.e(7556), v.e(109), v.e(4323), v.e(7057), v.e(5573)]).then((() => () => v(5573))))), i("@jupyter-notebook/terminal-extension", "7.2.0-beta.0", (() => Promise.all([v.e(3625), v.e(9983), v.e(5007), v.e(7057), v.e(8529), v.e(5601)]).then((() => () => v(95601))))), i("@jupyter-notebook/tree-extension", "7.2.0-beta.0", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(2277), v.e(8802), v.e(1317), v.e(3959), v.e(9224), v.e(3768)]).then((() => () => v(83768))))), i("@jupyter-notebook/tree", "7.2.0-beta.0", (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(3146)]).then((() => () => v(73146))))), i("@jupyter-notebook/ui-components", "7.2.0-beta.0", (() => Promise.all([v.e(1589), v.e(9068)]).then((() => () => v(59068))))), i("@jupyter/ydoc", "2.0.1", (() => Promise.all([v.e(35), v.e(998), v.e(1997), v.e(7843)]).then((() => () => v(50035))))), i("@jupyterlab/application-extension", "4.2.0-beta.1", (() => Promise.all([v.e(3881), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(2549), v.e(7568), v.e(2287), v.e(6934), v.e(2964)]).then((() => () => v(92871))))), i("@jupyterlab/application", "4.2.0-beta.1", (() => Promise.all([v.e(901), v.e(6853), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(1709), v.e(2549), v.e(7934), v.e(2782), v.e(9113), v.e(9503), v.e(4421), v.e(4771)]).then((() => () => v(76853))))), i("@jupyterlab/apputils-extension", "4.2.0-beta.1", (() => Promise.all([v.e(5099), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(2549), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(7556), v.e(8395), v.e(2287), v.e(6934), v.e(8005), v.e(4343)]).then((() => () => v(25099))))), i("@jupyterlab/apputils", "4.3.0-beta.1", (() => Promise.all([v.e(9605), v.e(998), v.e(502), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2277), v.e(2549), v.e(7568), v.e(9113), v.e(9503), v.e(8395), v.e(2287), v.e(5012), v.e(3752)]).then((() => () => v(89605))))), i("@jupyterlab/attachments", "4.2.0-beta.1", (() => Promise.all([v.e(1997), v.e(1709), v.e(5012), v.e(4042)]).then((() => () => v(44042))))), i("@jupyterlab/cell-toolbar-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(2277), v.e(2122)]).then((() => () => v(92122))))), i("@jupyterlab/cell-toolbar", "4.2.0-beta.1", (() => Promise.all([v.e(8713), v.e(1589), v.e(1997), v.e(3625), v.e(5012), v.e(7386)]).then((() => () => v(37386))))), i("@jupyterlab/cells", "4.2.0-beta.1", (() => Promise.all([v.e(2479), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(9503), v.e(7231), v.e(8395), v.e(3072), v.e(3766), v.e(3546), v.e(7253), v.e(4475), v.e(7508), v.e(3565), v.e(7925)]).then((() => () => v(72479))))), i("@jupyterlab/celltags-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(1589), v.e(8156), v.e(3625), v.e(4323), v.e(5346)]).then((() => () => v(15346))))), i("@jupyterlab/codeeditor", "4.2.0-beta.1", (() => Promise.all([v.e(7391), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(7568), v.e(5012), v.e(7508)]).then((() => () => v(77391))))), i("@jupyterlab/codemirror-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(8156), v.e(5007), v.e(2277), v.e(7568), v.e(7231), v.e(7253), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))), i("@jupyterlab/codemirror", "4.2.0-beta.1", (() => Promise.all([v.e(9799), v.e(5263), v.e(998), v.e(502), v.e(1997), v.e(9983), v.e(7231), v.e(3766), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(3831), v.e(7592), v.e(7843)]).then((() => () => v(95263))))), i("@jupyterlab/completer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(1589), v.e(8156), v.e(2277), v.e(6934), v.e(9469), v.e(3340)]).then((() => () => v(33340))))), i("@jupyterlab/completer", "4.2.0-beta.1", (() => Promise.all([v.e(2944), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(1709), v.e(9503), v.e(7231), v.e(8395), v.e(3546), v.e(9843)]).then((() => () => v(62944))))), i("@jupyterlab/console-extension", "4.2.0-beta.1", (() => Promise.all([v.e(6748), v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(7231), v.e(7556), v.e(4421), v.e(8802), v.e(6985), v.e(4778), v.e(9469)]).then((() => () => v(86748))))), i("@jupyterlab/console", "4.2.0-beta.1", (() => Promise.all([v.e(2636), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(1709), v.e(5012), v.e(3546), v.e(9843), v.e(9615), v.e(2867), v.e(7508)]).then((() => () => v(72636))))), i("@jupyterlab/coreutils", "6.2.0-beta.1", (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))), i("@jupyterlab/csvviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1827), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(5007), v.e(2277), v.e(2782), v.e(7556), v.e(3766)]).then((() => () => v(41827))))), i("@jupyterlab/csvviewer", "4.2.0-beta.1", (() => Promise.all([v.e(8032), v.e(998), v.e(502), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(2782), v.e(9072), v.e(5313)]).then((() => () => v(65313))))), i("@jupyterlab/debugger-extension", "4.2.0-beta.1", (() => Promise.all([v.e(2184), v.e(502), v.e(8713), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(2782), v.e(7231), v.e(4323), v.e(6985), v.e(2867), v.e(2069), v.e(8126), v.e(4877)]).then((() => () => v(42184))))), i("@jupyterlab/debugger", "4.2.0-beta.1", (() => Promise.all([v.e(6621), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(7231), v.e(5012), v.e(3546), v.e(9843), v.e(2867)]).then((() => () => v(36621))))), i("@jupyterlab/docmanager-extension", "4.2.0-beta.1", (() => Promise.all([v.e(8471), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(7568), v.e(2287), v.e(109)]).then((() => () => v(8471))))), i("@jupyterlab/docmanager", "4.2.0-beta.1", (() => Promise.all([v.e(7543), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2549), v.e(7934), v.e(2782), v.e(7568), v.e(9503), v.e(4421)]).then((() => () => v(37543))))), i("@jupyterlab/docregistry", "4.2.0-beta.1", (() => Promise.all([v.e(2489), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(2549), v.e(9503), v.e(7231)]).then((() => () => v(72489))))), i("@jupyterlab/documentsearch-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(5007), v.e(2277), v.e(3766), v.e(4212)]).then((() => () => v(24212))))), i("@jupyterlab/documentsearch", "4.2.0-beta.1", (() => Promise.all([v.e(6999), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))), i("@jupyterlab/extensionmanager-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(2311)]).then((() => () => v(22311))))), i("@jupyterlab/extensionmanager", "4.2.0-beta.1", (() => Promise.all([v.e(9151), v.e(502), v.e(8713), v.e(1589), v.e(8156), v.e(9983), v.e(7934), v.e(9113)]).then((() => () => v(59151))))), i("@jupyterlab/filebrowser-extension", "4.2.0-beta.1", (() => Promise.all([v.e(893), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(7568), v.e(2287), v.e(109), v.e(6934), v.e(8802)]).then((() => () => v(30893))))), i("@jupyterlab/filebrowser", "4.2.0-beta.1", (() => Promise.all([v.e(9341), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(9503), v.e(8395), v.e(109), v.e(4475), v.e(9615)]).then((() => () => v(39341))))), i("@jupyterlab/fileeditor-extension", "4.2.0-beta.1", (() => Promise.all([v.e(7603), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(7568), v.e(7231), v.e(7556), v.e(3072), v.e(3766), v.e(7253), v.e(8802), v.e(6985), v.e(5964), v.e(4778), v.e(2069), v.e(9469), v.e(3831)]).then((() => () => v(97603))))), i("@jupyterlab/fileeditor", "4.2.0-beta.1", (() => Promise.all([v.e(1833), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(2782), v.e(7568), v.e(7231), v.e(3072), v.e(7253), v.e(5964)]).then((() => () => v(31833))))), i("@jupyterlab/help-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1496), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(5007), v.e(9113), v.e(7556), v.e(4475)]).then((() => () => v(91496))))), i("@jupyterlab/htmlviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(6962)]).then((() => () => v(56962))))), i("@jupyterlab/htmlviewer", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(2782), v.e(5325)]).then((() => () => v(35325))))), i("@jupyterlab/hub-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(9983), v.e(5007), v.e(6893)]).then((() => () => v(56893))))), i("@jupyterlab/imageviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(6139)]).then((() => () => v(56139))))), i("@jupyterlab/imageviewer", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(8713), v.e(3485), v.e(9983), v.e(2782), v.e(7900)]).then((() => () => v(67900))))), i("@jupyterlab/javascript-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1709), v.e(5733)]).then((() => () => v(65733))))), i("@jupyterlab/json-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))), i("@jupyterlab/launcher", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(2549), v.e(4421), v.e(8771)]).then((() => () => v(68771))))), i("@jupyterlab/logconsole", "4.2.0-beta.1", (() => Promise.all([v.e(2089), v.e(998), v.e(502), v.e(3485), v.e(1997), v.e(1709), v.e(3565)]).then((() => () => v(2089))))), i("@jupyterlab/lsp-extension", "4.2.0-beta.1", (() => Promise.all([v.e(3466), v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(1997), v.e(8156), v.e(2277), v.e(7934), v.e(5964), v.e(1317)]).then((() => () => v(83466))))), i("@jupyterlab/lsp", "4.2.0-beta.1", (() => Promise.all([v.e(3512), v.e(998), v.e(502), v.e(8713), v.e(1997), v.e(9983), v.e(2782), v.e(9113)]).then((() => () => v(13512))))), i("@jupyterlab/mainmenu-extension", "4.2.0-beta.1", (() => Promise.all([v.e(545), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(9113), v.e(7556), v.e(109), v.e(8802)]).then((() => () => v(60545))))), i("@jupyterlab/mainmenu", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(8713), v.e(3485), v.e(1589), v.e(3625), v.e(2007)]).then((() => () => v(12007))))), i("@jupyterlab/markdownviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(3072), v.e(3785), v.e(9685)]).then((() => () => v(79685))))), i("@jupyterlab/markdownviewer", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(9983), v.e(1709), v.e(2782), v.e(3072), v.e(9680)]).then((() => () => v(99680))))), i("@jupyterlab/markedparser-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(9983), v.e(1709), v.e(7253), v.e(6561), v.e(9268)]).then((() => () => v(79268))))), i("@jupyterlab/mathjax-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(1709), v.e(1408)]).then((() => () => v(11408))))), i("@jupyterlab/mermaid-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(6561), v.e(9161)]).then((() => () => v(79161))))), i("@jupyterlab/mermaid", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(9983), v.e(2615)]).then((() => () => v(92615))))), i("@jupyterlab/metadataform-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(2277), v.e(4323), v.e(2621), v.e(9335)]).then((() => () => v(89335))))), i("@jupyterlab/metadataform", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(2277), v.e(4323), v.e(7478), v.e(2924)]).then((() => () => v(22924))))), i("@jupyterlab/nbformat", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3325)]).then((() => () => v(23325))))), i("@jupyterlab/notebook-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1962), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(7934), v.e(7568), v.e(9113), v.e(9503), v.e(7231), v.e(7556), v.e(2287), v.e(109), v.e(5012), v.e(3072), v.e(3766), v.e(7253), v.e(4323), v.e(8802), v.e(5964), v.e(2867), v.e(4778), v.e(9469), v.e(2964), v.e(8126), v.e(2621), v.e(2123)]).then((() => () => v(51962))))), i("@jupyterlab/notebook", "4.2.0-beta.1", (() => Promise.all([v.e(374), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(9503), v.e(7231), v.e(8395), v.e(5012), v.e(4421), v.e(3072), v.e(3766), v.e(4475), v.e(5964), v.e(9615), v.e(2867), v.e(7508), v.e(6642)]).then((() => () => v(90374))))), i("@jupyterlab/observables", "5.2.0-beta.1", (() => Promise.all([v.e(170), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503)]).then((() => () => v(10170))))), i("@jupyterlab/outputarea", "4.2.0-beta.1", (() => Promise.all([v.e(7226), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(3625), v.e(1709), v.e(9113), v.e(5012), v.e(4421), v.e(6642)]).then((() => () => v(47226))))), i("@jupyterlab/pdf-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))), i("@jupyterlab/pluginmanager-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(7401), v.e(3187)]).then((() => () => v(53187))))), i("@jupyterlab/pluginmanager", "4.2.0-beta.1", (() => Promise.all([v.e(9821), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(9113)]).then((() => () => v(69821))))), i("@jupyterlab/property-inspector", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(3485), v.e(1589), v.e(1997), v.e(1198)]).then((() => () => v(41198))))), i("@jupyterlab/rendermime-interfaces", "3.10.0-beta.1", (() => v.e(5297).then((() => () => v(75297))))), i("@jupyterlab/rendermime", "4.2.0-beta.1", (() => Promise.all([v.e(2401), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(9983), v.e(5012), v.e(6642), v.e(6982)]).then((() => () => v(72401))))), i("@jupyterlab/running-extension", "4.2.0-beta.1", (() => Promise.all([v.e(7854), v.e(502), v.e(8713), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(5007), v.e(7934), v.e(2782), v.e(2287), v.e(109), v.e(1317)]).then((() => () => v(97854))))), i("@jupyterlab/running", "4.2.0-beta.1", (() => Promise.all([v.e(1809), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))), i("@jupyterlab/services", "7.2.0-beta.1", (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(9983), v.e(2549), v.e(7934), v.e(2287)]).then((() => () => v(83676))))), i("@jupyterlab/settingeditor-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(1709), v.e(7231), v.e(2287), v.e(7401), v.e(8633)]).then((() => () => v(98633))))), i("@jupyterlab/settingeditor", "4.2.0-beta.1", (() => Promise.all([v.e(3360), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(7231), v.e(2287), v.e(7478)]).then((() => () => v(63360))))), i("@jupyterlab/settingregistry", "4.2.0-beta.1", (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))), i("@jupyterlab/shortcuts-extension", "5.0.0-beta.1", (() => Promise.all([v.e(113), v.e(998), v.e(502), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(2277), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))), i("@jupyterlab/statedb", "4.2.0-beta.1", (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))), i("@jupyterlab/statusbar", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(2549), v.e(3680)]).then((() => () => v(53680))))), i("@jupyterlab/terminal-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(5007), v.e(2277), v.e(9113), v.e(7556), v.e(1317), v.e(4778), v.e(8529), v.e(5912)]).then((() => () => v(15912))))), i("@jupyterlab/terminal", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))), i("@jupyterlab/theme-dark-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(6627)]).then((() => () => v(6627))))), i("@jupyterlab/theme-light-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5426)]).then((() => () => v(45426))))), i("@jupyterlab/toc-extension", "6.2.0-beta.1", (() => Promise.all([v.e(502), v.e(1589), v.e(5007), v.e(2277), v.e(3072), v.e(62)]).then((() => () => v(40062))))), i("@jupyterlab/toc", "6.2.0-beta.1", (() => Promise.all([v.e(5921), v.e(998), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(1709), v.e(2549)]).then((() => () => v(75921))))), i("@jupyterlab/tooltip-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(3485), v.e(3625), v.e(9983), v.e(1709), v.e(4323), v.e(6985), v.e(2069), v.e(3715), v.e(6604)]).then((() => () => v(6604))))), i("@jupyterlab/tooltip", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(1709), v.e(1647)]).then((() => () => v(51647))))), i("@jupyterlab/translation-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(2277), v.e(7556), v.e(6815)]).then((() => () => v(56815))))), i("@jupyterlab/translation", "4.2.0-beta.1", (() => Promise.all([v.e(7819), v.e(998), v.e(9983), v.e(9113), v.e(2287)]).then((() => () => v(57819))))), i("@jupyterlab/ui-components-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1589), v.e(3863)]).then((() => () => v(73863))))), i("@jupyterlab/ui-components", "4.2.0-beta.1", (() => Promise.all([v.e(755), v.e(7811), v.e(2557), v.e(998), v.e(502), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(2557))))), i("@jupyterlab/vega5-extension", "4.2.0-beta.1", (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))), i("@jupyterlab/workspaces", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(1997), v.e(7934), v.e(1828)]).then((() => () => v(11828))))), i("@lezer/common", "1.2.1", (() => v.e(7997).then((() => () => v(97997))))), i("@lezer/highlight", "1.2.0", (() => Promise.all([v.e(3797), v.e(9352)]).then((() => () => v(23797))))), i("@lumino/algorithm", "2.0.1", (() => v.e(5614).then((() => () => v(15614))))), i("@lumino/application", "2.3.1", (() => Promise.all([v.e(6731), v.e(998), v.e(3485), v.e(6934)]).then((() => () => v(16731))))), i("@lumino/commands", "2.3.0", (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))), i("@lumino/coreutils", "2.1.2", (() => v.e(2756).then((() => () => v(12756))))), i("@lumino/datagrid", "2.3.1", (() => Promise.all([v.e(8929), v.e(998), v.e(3485), v.e(1997), v.e(3625), v.e(9503), v.e(8395), v.e(9615), v.e(554)]).then((() => () => v(98929))))), i("@lumino/disposable", "2.1.2", (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))), i("@lumino/domutils", "2.0.1", (() => v.e(1696).then((() => () => v(1696))))), i("@lumino/dragdrop", "2.1.4", (() => Promise.all([v.e(4291), v.e(2549)]).then((() => () => v(54291))))), i("@lumino/keyboard", "2.0.1", (() => v.e(9222).then((() => () => v(19222))))), i("@lumino/messaging", "2.0.1", (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))), i("@lumino/polling", "2.1.2", (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))), i("@lumino/properties", "2.0.1", (() => v.e(3733).then((() => () => v(13733))))), i("@lumino/signaling", "2.1.2", (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))), i("@lumino/virtualdom", "2.0.1", (() => Promise.all([v.e(5234), v.e(3625)]).then((() => () => v(85234))))), i("@lumino/widgets", "2.3.2", (() => Promise.all([v.e(911), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503), v.e(8395), v.e(4421), v.e(6934), v.e(4475), v.e(9615), v.e(554)]).then((() => () => v(30911))))), i("@rjsf/utils", "5.16.1", (() => Promise.all([v.e(755), v.e(7811), v.e(7995), v.e(8156)]).then((() => () => v(57995))))), i("@rjsf/validator-ajv8", "5.15.1", (() => Promise.all([v.e(755), v.e(7796), v.e(131), v.e(4885)]).then((() => () => v(70131))))), i("marked-gfm-heading-id", "3.1.1", (() => v.e(7179).then((() => () => v(67179))))), i("marked-mangle", "1.1.5", (() => v.e(1869).then((() => () => v(81869))))), i("marked", "9.1.6", (() => v.e(3079).then((() => () => v(33079))))), i("react-dom", "18.2.0", (() => Promise.all([v.e(1542), v.e(8156)]).then((() => () => v(31542))))), i("react-toastify", "9.1.3", (() => Promise.all([v.e(8156), v.e(5777)]).then((() => () => v(25777))))), i("react", "18.2.0", (() => v.e(7378).then((() => () => v(27378))))), i("yjs", "13.6.8", (() => v.e(7957).then((() => () => v(67957)))))), e[a] = s.length ? Promise.all(s).then((() => e[a] = 1)) : 1
+                return "default" === a && (i("@codemirror/commands", "6.3.3", (() => Promise.all([v.e(7450), v.e(3546), v.e(9843), v.e(9352), v.e(7592)]).then((() => () => v(67450))))), i("@codemirror/lang-markdown", "6.2.4", (() => Promise.all([v.e(5850), v.e(9239), v.e(9799), v.e(7866), v.e(6271), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(7592)]).then((() => () => v(76271))))), i("@codemirror/language", "6.10.1", (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))), i("@codemirror/search", "6.5.6", (() => Promise.all([v.e(5261), v.e(3546), v.e(9843)]).then((() => () => v(25261))))), i("@codemirror/state", "6.4.1", (() => v.e(2323).then((() => () => v(92323))))), i("@codemirror/view", "6.26.1", (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))), i("@jupyter-notebook/application-extension", "7.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(2782), v.e(7556), v.e(109), v.e(6985), v.e(8856), v.e(5744), v.e(8579)]).then((() => () => v(88579))))), i("@jupyter-notebook/application", "7.2.0-beta.1", (() => Promise.all([v.e(901), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(5007), v.e(1709), v.e(2549), v.e(7934), v.e(2782), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))), i("@jupyter-notebook/console-extension", "7.2.0-beta.1", (() => Promise.all([v.e(3625), v.e(9983), v.e(5007), v.e(6985), v.e(8856), v.e(4645)]).then((() => () => v(94645))))), i("@jupyter-notebook/docmanager-extension", "7.2.0-beta.1", (() => Promise.all([v.e(1997), v.e(9983), v.e(109), v.e(8856), v.e(1650)]).then((() => () => v(71650))))), i("@jupyter-notebook/documentsearch-extension", "7.2.0-beta.1", (() => Promise.all([v.e(3766), v.e(8856), v.e(4382)]).then((() => () => v(54382))))), i("@jupyter-notebook/help-extension", "7.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(8156), v.e(7556), v.e(5744), v.e(9380)]).then((() => () => v(19380))))), i("@jupyter-notebook/notebook-extension", "7.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(9983), v.e(2277), v.e(7934), v.e(7556), v.e(109), v.e(4323), v.e(8856), v.e(5573)]).then((() => () => v(5573))))), i("@jupyter-notebook/terminal-extension", "7.2.0-beta.1", (() => Promise.all([v.e(3625), v.e(9983), v.e(5007), v.e(8856), v.e(8529), v.e(5601)]).then((() => () => v(95601))))), i("@jupyter-notebook/tree-extension", "7.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(2277), v.e(8802), v.e(1317), v.e(3959), v.e(8678), v.e(3768)]).then((() => () => v(83768))))), i("@jupyter-notebook/tree", "7.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(3146)]).then((() => () => v(73146))))), i("@jupyter-notebook/ui-components", "7.2.0-beta.1", (() => Promise.all([v.e(1589), v.e(9068)]).then((() => () => v(59068))))), i("@jupyter/ydoc", "2.0.1", (() => Promise.all([v.e(35), v.e(998), v.e(1997), v.e(7843)]).then((() => () => v(50035))))), i("@jupyterlab/application-extension", "4.2.0-beta.1", (() => Promise.all([v.e(3881), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(2549), v.e(7568), v.e(2287), v.e(6934), v.e(2964)]).then((() => () => v(92871))))), i("@jupyterlab/application", "4.2.0-beta.1", (() => Promise.all([v.e(901), v.e(6853), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(1709), v.e(2549), v.e(7934), v.e(2782), v.e(9113), v.e(9503), v.e(4421), v.e(4771)]).then((() => () => v(76853))))), i("@jupyterlab/apputils-extension", "4.2.0-beta.1", (() => Promise.all([v.e(5099), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(2549), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(7556), v.e(8395), v.e(2287), v.e(6934), v.e(8005), v.e(4343)]).then((() => () => v(25099))))), i("@jupyterlab/apputils", "4.3.0-beta.1", (() => Promise.all([v.e(9605), v.e(998), v.e(502), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2277), v.e(2549), v.e(7568), v.e(9113), v.e(9503), v.e(8395), v.e(2287), v.e(5012), v.e(3752)]).then((() => () => v(89605))))), i("@jupyterlab/attachments", "4.2.0-beta.1", (() => Promise.all([v.e(1997), v.e(1709), v.e(5012), v.e(4042)]).then((() => () => v(44042))))), i("@jupyterlab/cell-toolbar-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(2277), v.e(2122)]).then((() => () => v(92122))))), i("@jupyterlab/cell-toolbar", "4.2.0-beta.1", (() => Promise.all([v.e(8713), v.e(1589), v.e(1997), v.e(3625), v.e(5012), v.e(7386)]).then((() => () => v(37386))))), i("@jupyterlab/cells", "4.2.0-beta.1", (() => Promise.all([v.e(2479), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(9503), v.e(7231), v.e(8395), v.e(3072), v.e(3766), v.e(3546), v.e(7253), v.e(4475), v.e(7508), v.e(3565), v.e(7925)]).then((() => () => v(72479))))), i("@jupyterlab/celltags-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(1589), v.e(8156), v.e(3625), v.e(4323), v.e(5346)]).then((() => () => v(15346))))), i("@jupyterlab/codeeditor", "4.2.0-beta.1", (() => Promise.all([v.e(7391), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(7568), v.e(5012), v.e(7508)]).then((() => () => v(77391))))), i("@jupyterlab/codemirror-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(8156), v.e(5007), v.e(2277), v.e(7568), v.e(7231), v.e(7253), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))), i("@jupyterlab/codemirror", "4.2.0-beta.1", (() => Promise.all([v.e(9799), v.e(5263), v.e(998), v.e(502), v.e(1997), v.e(9983), v.e(7231), v.e(3766), v.e(3546), v.e(9843), v.e(9352), v.e(2209), v.e(3831), v.e(7592), v.e(7843)]).then((() => () => v(95263))))), i("@jupyterlab/completer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(1589), v.e(8156), v.e(2277), v.e(6934), v.e(9469), v.e(3340)]).then((() => () => v(33340))))), i("@jupyterlab/completer", "4.2.0-beta.1", (() => Promise.all([v.e(2944), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(1709), v.e(9503), v.e(7231), v.e(8395), v.e(3546), v.e(9843)]).then((() => () => v(62944))))), i("@jupyterlab/console-extension", "4.2.0-beta.1", (() => Promise.all([v.e(6748), v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(7231), v.e(7556), v.e(4421), v.e(8802), v.e(6985), v.e(4778), v.e(9469)]).then((() => () => v(86748))))), i("@jupyterlab/console", "4.2.0-beta.1", (() => Promise.all([v.e(2636), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(1709), v.e(5012), v.e(3546), v.e(9843), v.e(9615), v.e(2867), v.e(7508)]).then((() => () => v(72636))))), i("@jupyterlab/coreutils", "6.2.0-beta.1", (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))), i("@jupyterlab/csvviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1827), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(5007), v.e(2277), v.e(2782), v.e(7556), v.e(3766)]).then((() => () => v(41827))))), i("@jupyterlab/csvviewer", "4.2.0-beta.1", (() => Promise.all([v.e(8032), v.e(998), v.e(502), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(2782), v.e(9072), v.e(5313)]).then((() => () => v(65313))))), i("@jupyterlab/debugger-extension", "4.2.0-beta.1", (() => Promise.all([v.e(2184), v.e(502), v.e(8713), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(2782), v.e(7231), v.e(4323), v.e(6985), v.e(2867), v.e(2069), v.e(8126), v.e(4877)]).then((() => () => v(42184))))), i("@jupyterlab/debugger", "4.2.0-beta.1", (() => Promise.all([v.e(6621), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(7231), v.e(5012), v.e(3546), v.e(9843), v.e(2867)]).then((() => () => v(36621))))), i("@jupyterlab/docmanager-extension", "4.2.0-beta.1", (() => Promise.all([v.e(8471), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(7568), v.e(2287), v.e(109)]).then((() => () => v(8471))))), i("@jupyterlab/docmanager", "4.2.0-beta.1", (() => Promise.all([v.e(7543), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2549), v.e(7934), v.e(2782), v.e(7568), v.e(9503), v.e(4421)]).then((() => () => v(37543))))), i("@jupyterlab/docregistry", "4.2.0-beta.1", (() => Promise.all([v.e(2489), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(2549), v.e(9503), v.e(7231)]).then((() => () => v(72489))))), i("@jupyterlab/documentsearch-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(5007), v.e(2277), v.e(3766), v.e(4212)]).then((() => () => v(24212))))), i("@jupyterlab/documentsearch", "4.2.0-beta.1", (() => Promise.all([v.e(6999), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))), i("@jupyterlab/extensionmanager-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(2311)]).then((() => () => v(22311))))), i("@jupyterlab/extensionmanager", "4.2.0-beta.1", (() => Promise.all([v.e(9151), v.e(502), v.e(8713), v.e(1589), v.e(8156), v.e(9983), v.e(7934), v.e(9113)]).then((() => () => v(59151))))), i("@jupyterlab/filebrowser-extension", "4.2.0-beta.1", (() => Promise.all([v.e(893), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(7568), v.e(2287), v.e(109), v.e(6934), v.e(8802)]).then((() => () => v(30893))))), i("@jupyterlab/filebrowser", "4.2.0-beta.1", (() => Promise.all([v.e(9341), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(9503), v.e(8395), v.e(109), v.e(4475), v.e(9615)]).then((() => () => v(39341))))), i("@jupyterlab/fileeditor-extension", "4.2.0-beta.1", (() => Promise.all([v.e(7603), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(7568), v.e(7231), v.e(7556), v.e(3072), v.e(3766), v.e(7253), v.e(8802), v.e(6985), v.e(5964), v.e(4778), v.e(2069), v.e(9469), v.e(3831)]).then((() => () => v(97603))))), i("@jupyterlab/fileeditor", "4.2.0-beta.1", (() => Promise.all([v.e(1833), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(2782), v.e(7568), v.e(7231), v.e(3072), v.e(7253), v.e(5964)]).then((() => () => v(31833))))), i("@jupyterlab/help-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1496), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(5007), v.e(9113), v.e(7556), v.e(4475)]).then((() => () => v(91496))))), i("@jupyterlab/htmlviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(6962)]).then((() => () => v(56962))))), i("@jupyterlab/htmlviewer", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(2782), v.e(5325)]).then((() => () => v(35325))))), i("@jupyterlab/hub-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(9983), v.e(5007), v.e(6893)]).then((() => () => v(56893))))), i("@jupyterlab/imageviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(6139)]).then((() => () => v(56139))))), i("@jupyterlab/imageviewer", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(8713), v.e(3485), v.e(9983), v.e(2782), v.e(7900)]).then((() => () => v(67900))))), i("@jupyterlab/javascript-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1709), v.e(5733)]).then((() => () => v(65733))))), i("@jupyterlab/json-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))), i("@jupyterlab/launcher", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(2549), v.e(4421), v.e(8771)]).then((() => () => v(68771))))), i("@jupyterlab/logconsole", "4.2.0-beta.1", (() => Promise.all([v.e(2089), v.e(998), v.e(502), v.e(3485), v.e(1997), v.e(1709), v.e(3565)]).then((() => () => v(2089))))), i("@jupyterlab/lsp-extension", "4.2.0-beta.1", (() => Promise.all([v.e(3466), v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(1997), v.e(8156), v.e(2277), v.e(7934), v.e(5964), v.e(1317)]).then((() => () => v(83466))))), i("@jupyterlab/lsp", "4.2.0-beta.1", (() => Promise.all([v.e(3512), v.e(998), v.e(502), v.e(8713), v.e(1997), v.e(9983), v.e(2782), v.e(9113)]).then((() => () => v(13512))))), i("@jupyterlab/mainmenu-extension", "4.2.0-beta.1", (() => Promise.all([v.e(545), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(9113), v.e(7556), v.e(109), v.e(8802)]).then((() => () => v(60545))))), i("@jupyterlab/mainmenu", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(8713), v.e(3485), v.e(1589), v.e(3625), v.e(2007)]).then((() => () => v(12007))))), i("@jupyterlab/markdownviewer-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(3072), v.e(3785), v.e(9685)]).then((() => () => v(79685))))), i("@jupyterlab/markdownviewer", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(9983), v.e(1709), v.e(2782), v.e(3072), v.e(9680)]).then((() => () => v(99680))))), i("@jupyterlab/markedparser-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(9983), v.e(1709), v.e(7253), v.e(6561), v.e(9268)]).then((() => () => v(79268))))), i("@jupyterlab/mathjax-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(1709), v.e(1408)]).then((() => () => v(11408))))), i("@jupyterlab/mermaid-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(6561), v.e(9161)]).then((() => () => v(79161))))), i("@jupyterlab/mermaid", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(9983), v.e(2615)]).then((() => () => v(92615))))), i("@jupyterlab/metadataform-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(2277), v.e(4323), v.e(2621), v.e(9335)]).then((() => () => v(89335))))), i("@jupyterlab/metadataform", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(2277), v.e(4323), v.e(7478), v.e(2924)]).then((() => () => v(22924))))), i("@jupyterlab/nbformat", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3325)]).then((() => () => v(23325))))), i("@jupyterlab/notebook-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1962), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(9983), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(7934), v.e(7568), v.e(9113), v.e(9503), v.e(7231), v.e(7556), v.e(2287), v.e(109), v.e(5012), v.e(3072), v.e(3766), v.e(7253), v.e(4323), v.e(8802), v.e(5964), v.e(2867), v.e(4778), v.e(9469), v.e(2964), v.e(8126), v.e(2621), v.e(2123)]).then((() => () => v(51962))))), i("@jupyterlab/notebook", "4.2.0-beta.1", (() => Promise.all([v.e(374), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(9503), v.e(7231), v.e(8395), v.e(5012), v.e(4421), v.e(3072), v.e(3766), v.e(4475), v.e(5964), v.e(9615), v.e(2867), v.e(7508), v.e(6642)]).then((() => () => v(90374))))), i("@jupyterlab/observables", "5.2.0-beta.1", (() => Promise.all([v.e(170), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503)]).then((() => () => v(10170))))), i("@jupyterlab/outputarea", "4.2.0-beta.1", (() => Promise.all([v.e(7226), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(3625), v.e(1709), v.e(9113), v.e(5012), v.e(4421), v.e(6642)]).then((() => () => v(47226))))), i("@jupyterlab/pdf-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))), i("@jupyterlab/pluginmanager-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(7401), v.e(3187)]).then((() => () => v(53187))))), i("@jupyterlab/pluginmanager", "4.2.0-beta.1", (() => Promise.all([v.e(9821), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(9113)]).then((() => () => v(69821))))), i("@jupyterlab/property-inspector", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(3485), v.e(1589), v.e(1997), v.e(1198)]).then((() => () => v(41198))))), i("@jupyterlab/rendermime-interfaces", "3.10.0-beta.1", (() => v.e(5297).then((() => () => v(75297))))), i("@jupyterlab/rendermime", "4.2.0-beta.1", (() => Promise.all([v.e(2401), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(9983), v.e(5012), v.e(6642), v.e(6982)]).then((() => () => v(72401))))), i("@jupyterlab/running-extension", "4.2.0-beta.1", (() => Promise.all([v.e(7854), v.e(502), v.e(8713), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(5007), v.e(7934), v.e(2782), v.e(2287), v.e(109), v.e(1317)]).then((() => () => v(97854))))), i("@jupyterlab/running", "4.2.0-beta.1", (() => Promise.all([v.e(1809), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))), i("@jupyterlab/services", "7.2.0-beta.1", (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(9983), v.e(2549), v.e(7934), v.e(2287)]).then((() => () => v(83676))))), i("@jupyterlab/settingeditor-extension", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(1709), v.e(7231), v.e(2287), v.e(7401), v.e(8633)]).then((() => () => v(98633))))), i("@jupyterlab/settingeditor", "4.2.0-beta.1", (() => Promise.all([v.e(3360), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(7231), v.e(2287), v.e(7478)]).then((() => () => v(63360))))), i("@jupyterlab/settingregistry", "4.2.0-beta.1", (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))), i("@jupyterlab/shortcuts-extension", "5.0.0-beta.1", (() => Promise.all([v.e(113), v.e(998), v.e(502), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(2277), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))), i("@jupyterlab/statedb", "4.2.0-beta.1", (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))), i("@jupyterlab/statusbar", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(2549), v.e(3680)]).then((() => () => v(53680))))), i("@jupyterlab/terminal-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(5007), v.e(2277), v.e(9113), v.e(7556), v.e(1317), v.e(4778), v.e(8529), v.e(5912)]).then((() => () => v(15912))))), i("@jupyterlab/terminal", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(502), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))), i("@jupyterlab/theme-dark-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(6627)]).then((() => () => v(6627))))), i("@jupyterlab/theme-dark-high-contrast-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5254)]).then((() => () => v(95254))))), i("@jupyterlab/theme-light-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5426)]).then((() => () => v(45426))))), i("@jupyterlab/toc-extension", "6.2.0-beta.1", (() => Promise.all([v.e(502), v.e(1589), v.e(5007), v.e(2277), v.e(3072), v.e(62)]).then((() => () => v(40062))))), i("@jupyterlab/toc", "6.2.0-beta.1", (() => Promise.all([v.e(5921), v.e(998), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(9983), v.e(1709), v.e(2549)]).then((() => () => v(75921))))), i("@jupyterlab/tooltip-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(3485), v.e(3625), v.e(9983), v.e(1709), v.e(4323), v.e(6985), v.e(2069), v.e(3715), v.e(6604)]).then((() => () => v(6604))))), i("@jupyterlab/tooltip", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(1709), v.e(1647)]).then((() => () => v(51647))))), i("@jupyterlab/translation-extension", "4.2.0-beta.1", (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(2277), v.e(7556), v.e(6815)]).then((() => () => v(56815))))), i("@jupyterlab/translation", "4.2.0-beta.1", (() => Promise.all([v.e(7819), v.e(998), v.e(9983), v.e(9113), v.e(2287)]).then((() => () => v(57819))))), i("@jupyterlab/ui-components-extension", "4.2.0-beta.1", (() => Promise.all([v.e(1589), v.e(3863)]).then((() => () => v(73863))))), i("@jupyterlab/ui-components", "4.2.0-beta.1", (() => Promise.all([v.e(755), v.e(7811), v.e(2557), v.e(998), v.e(502), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(2557))))), i("@jupyterlab/vega5-extension", "4.2.0-beta.1", (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))), i("@jupyterlab/workspaces", "4.2.0-beta.1", (() => Promise.all([v.e(998), v.e(1997), v.e(7934), v.e(1828)]).then((() => () => v(11828))))), i("@lezer/common", "1.2.1", (() => v.e(7997).then((() => () => v(97997))))), i("@lezer/highlight", "1.2.0", (() => Promise.all([v.e(3797), v.e(9352)]).then((() => () => v(23797))))), i("@lumino/algorithm", "2.0.1", (() => v.e(5614).then((() => () => v(15614))))), i("@lumino/application", "2.3.1", (() => Promise.all([v.e(6731), v.e(998), v.e(3485), v.e(6934)]).then((() => () => v(16731))))), i("@lumino/commands", "2.3.0", (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))), i("@lumino/coreutils", "2.1.2", (() => v.e(2756).then((() => () => v(12756))))), i("@lumino/datagrid", "2.3.1", (() => Promise.all([v.e(8929), v.e(998), v.e(3485), v.e(1997), v.e(3625), v.e(9503), v.e(8395), v.e(9615), v.e(554)]).then((() => () => v(98929))))), i("@lumino/disposable", "2.1.2", (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))), i("@lumino/domutils", "2.0.1", (() => v.e(1696).then((() => () => v(1696))))), i("@lumino/dragdrop", "2.1.4", (() => Promise.all([v.e(4291), v.e(2549)]).then((() => () => v(54291))))), i("@lumino/keyboard", "2.0.1", (() => v.e(9222).then((() => () => v(19222))))), i("@lumino/messaging", "2.0.1", (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))), i("@lumino/polling", "2.1.2", (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))), i("@lumino/properties", "2.0.1", (() => v.e(3733).then((() => () => v(13733))))), i("@lumino/signaling", "2.1.2", (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))), i("@lumino/virtualdom", "2.0.1", (() => Promise.all([v.e(5234), v.e(3625)]).then((() => () => v(85234))))), i("@lumino/widgets", "2.3.2", (() => Promise.all([v.e(911), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(9503), v.e(8395), v.e(4421), v.e(6934), v.e(4475), v.e(9615), v.e(554)]).then((() => () => v(30911))))), i("@rjsf/utils", "5.16.1", (() => Promise.all([v.e(755), v.e(7811), v.e(7995), v.e(8156)]).then((() => () => v(57995))))), i("@rjsf/validator-ajv8", "5.15.1", (() => Promise.all([v.e(755), v.e(7796), v.e(131), v.e(4885)]).then((() => () => v(70131))))), i("marked-gfm-heading-id", "3.1.1", (() => v.e(7179).then((() => () => v(67179))))), i("marked-mangle", "1.1.5", (() => v.e(1869).then((() => () => v(81869))))), i("marked", "9.1.6", (() => v.e(3079).then((() => () => v(33079))))), i("react-dom", "18.2.0", (() => Promise.all([v.e(1542), v.e(8156)]).then((() => () => v(31542))))), i("react-toastify", "9.1.3", (() => Promise.all([v.e(8156), v.e(5777)]).then((() => () => v(25777))))), i("react", "18.2.0", (() => v.e(7378).then((() => () => v(27378))))), i("yjs", "13.6.8", (() => v.e(7957).then((() => () => v(67957)))))), e[a] = s.length ? Promise.all(s).then((() => e[a] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         v.g.importScripts && (e = v.g.location + "");
         var t = v.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
@@ -215,61 +215,62 @@
         var n = v.I(t);
         return n && n.then ? n.then(e.bind(e, t, v.S[t], a, l, r)) : e(t, v.S[t], a, l, r)
     })(((e, t, a, l, r) => t && v.o(t, a) ? b(t, 0, a, l) : r())), P = d(((e, t, a, l, r) => {
         var n = t && v.o(t, a) && m(t, a, l);
         return n ? p(n) : r()
     })), y = {}, j = {
         9983: () => f("default", "@jupyterlab/coreutils", [2, 6, 2, 0, , "beta", 1], (() => Promise.all([v.e(2866), v.e(998), v.e(1997)]).then((() => () => v(2866))))),
-        37057: () => P("default", "@jupyter-notebook/application", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(901), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(5007), v.e(1709), v.e(2549), v.e(7934), v.e(2782), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))),
+        28856: () => P("default", "@jupyter-notebook/application", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(901), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(3625), v.e(9983), v.e(5007), v.e(1709), v.e(2549), v.e(7934), v.e(2782), v.e(9503), v.e(4421), v.e(5135)]).then((() => () => v(45135))))),
         32123: () => P("default", "@jupyterlab/docmanager-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(8471), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(5007), v.e(2277), v.e(7568), v.e(2287), v.e(109)]).then((() => () => v(8471))))),
         1542: () => P("default", "@jupyterlab/htmlviewer-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(6962)]).then((() => () => v(56962))))),
         2344: () => P("default", "@jupyterlab/application-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(3881), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(5007), v.e(2277), v.e(2549), v.e(7568), v.e(2287), v.e(6934), v.e(2964)]).then((() => () => v(92871))))),
         2438: () => P("default", "@jupyterlab/toc-extension", [2, 6, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(1589), v.e(5007), v.e(2277), v.e(3072), v.e(62)]).then((() => () => v(40062))))),
+        3708: () => P("default", "@jupyterlab/theme-dark-high-contrast-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(5254)]).then((() => () => v(95254))))),
         6999: () => P("default", "@jupyterlab/markedparser-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(1709), v.e(7253), v.e(6561), v.e(3129)]).then((() => () => v(79268))))),
         7221: () => P("default", "@jupyterlab/completer-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(1589), v.e(8156), v.e(2277), v.e(6934), v.e(9469), v.e(3340)]).then((() => () => v(33340))))),
         8997: () => P("default", "@jupyterlab/mainmenu-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(545), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(3625), v.e(5007), v.e(2277), v.e(9113), v.e(7556), v.e(109), v.e(8802)]).then((() => () => v(60545))))),
         8998: () => P("default", "@jupyterlab/terminal-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(5007), v.e(2277), v.e(9113), v.e(7556), v.e(1317), v.e(4778), v.e(8529), v.e(5912)]).then((() => () => v(15912))))),
         9135: () => P("default", "@jupyterlab/console-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(6748), v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(7231), v.e(7556), v.e(4421), v.e(8802), v.e(6985), v.e(4778), v.e(9469)]).then((() => () => v(86748))))),
         10253: () => P("default", "@jupyterlab/help-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1496), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(5007), v.e(9113), v.e(7556), v.e(4475)]).then((() => () => v(91496))))),
         12427: () => P("default", "@jupyterlab/tooltip-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(3485), v.e(3625), v.e(1709), v.e(4323), v.e(6985), v.e(2069), v.e(3715), v.e(2088)]).then((() => () => v(6604))))),
         13318: () => P("default", "@jupyterlab/filebrowser-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(893), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(5007), v.e(2277), v.e(7568), v.e(2287), v.e(109), v.e(6934), v.e(8802)]).then((() => () => v(30893))))),
+        14745: () => P("default", "@jupyter-notebook/terminal-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(3625), v.e(5007), v.e(8529), v.e(1684)]).then((() => () => v(95601))))),
         16557: () => P("default", "@jupyterlab/cell-toolbar-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(2277), v.e(2122)]).then((() => () => v(92122))))),
         19199: () => P("default", "@jupyterlab/hub-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(7684)]).then((() => () => v(56893))))),
-        21113: () => P("default", "@jupyter-notebook/terminal-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(3625), v.e(5007), v.e(8529), v.e(1684)]).then((() => () => v(95601))))),
         23955: () => P("default", "@jupyterlab/javascript-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1709), v.e(5733)]).then((() => () => v(65733))))),
         24351: () => P("default", "@jupyterlab/lsp-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(3466), v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(1997), v.e(8156), v.e(2277), v.e(7934), v.e(5964), v.e(1317)]).then((() => () => v(83466))))),
         25763: () => P("default", "@jupyterlab/codemirror-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(8156), v.e(5007), v.e(2277), v.e(7568), v.e(7231), v.e(7253), v.e(7478), v.e(3831), v.e(7592), v.e(7655)]).then((() => () => v(97655))))),
         25950: () => P("default", "@jupyterlab/extensionmanager-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(2311)]).then((() => () => v(22311))))),
         27909: () => P("default", "@jupyterlab/json-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(8005), v.e(690)]).then((() => () => v(60690))))),
-        31663: () => P("default", "@jupyter-notebook/help-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(502), v.e(8713), v.e(8156), v.e(7556), v.e(1481), v.e(9380)]).then((() => () => v(19380))))),
+        29194: () => P("default", "@jupyter-notebook/console-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(3625), v.e(5007), v.e(6985), v.e(6345)]).then((() => () => v(94645))))),
         35761: () => P("default", "@jupyterlab/translation-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(2277), v.e(7556), v.e(6815)]).then((() => () => v(56815))))),
-        38896: () => P("default", "@jupyter-notebook/docmanager-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(1997), v.e(109), v.e(8875)]).then((() => () => v(71650))))),
-        40545: () => P("default", "@jupyter-notebook/tree-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2277), v.e(8802), v.e(1317), v.e(3959), v.e(9224), v.e(7302)]).then((() => () => v(83768))))),
+        40835: () => P("default", "@jupyter-notebook/tree-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2277), v.e(8802), v.e(1317), v.e(3959), v.e(8678), v.e(7302)]).then((() => () => v(83768))))),
         45317: () => P("default", "@jupyterlab/imageviewer-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(6139)]).then((() => () => v(56139))))),
         46030: () => P("default", "@jupyterlab/theme-dark-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(6627)]).then((() => () => v(6627))))),
         49938: () => P("default", "@jupyterlab/fileeditor-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(7603), v.e(502), v.e(8713), v.e(1589), v.e(3625), v.e(5007), v.e(2277), v.e(7568), v.e(7231), v.e(7556), v.e(3072), v.e(3766), v.e(7253), v.e(8802), v.e(6985), v.e(5964), v.e(4778), v.e(2069), v.e(9469), v.e(3831)]).then((() => () => v(97603))))),
+        51267: () => P("default", "@jupyter-notebook/documentsearch-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(3766), v.e(7906)]).then((() => () => v(54382))))),
         51701: () => P("default", "@jupyterlab/metadataform-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(502), v.e(1589), v.e(2277), v.e(4323), v.e(2621), v.e(9335)]).then((() => () => v(89335))))),
         51973: () => P("default", "@jupyterlab/celltags-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(1589), v.e(8156), v.e(3625), v.e(4323), v.e(5346)]).then((() => () => v(15346))))),
-        58524: () => P("default", "@jupyter-notebook/documentsearch-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(3766), v.e(7906)]).then((() => () => v(54382))))),
-        59123: () => P("default", "@jupyter-notebook/application-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(2782), v.e(7556), v.e(109), v.e(6985), v.e(1481), v.e(8579)]).then((() => () => v(88579))))),
         60679: () => P("default", "@jupyterlab/pluginmanager-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(7401), v.e(3187)]).then((() => () => v(53187))))),
         62430: () => P("default", "@jupyterlab/debugger-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(2184), v.e(502), v.e(8713), v.e(5007), v.e(2277), v.e(1709), v.e(2782), v.e(7231), v.e(4323), v.e(6985), v.e(2867), v.e(2069), v.e(8126), v.e(4877)]).then((() => () => v(42184))))),
         64209: () => P("default", "@jupyterlab/apputils-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(5099), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(5007), v.e(2277), v.e(2549), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(7556), v.e(8395), v.e(2287), v.e(6934), v.e(8005), v.e(4343)]).then((() => () => v(25099))))),
-        64253: () => P("default", "@jupyter-notebook/notebook-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(2277), v.e(7934), v.e(7556), v.e(109), v.e(4323), v.e(5573)]).then((() => () => v(5573))))),
         65097: () => P("default", "@jupyterlab/settingeditor-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(1589), v.e(5007), v.e(2277), v.e(1709), v.e(7231), v.e(2287), v.e(7401), v.e(8633)]).then((() => () => v(98633))))),
         65529: () => P("default", "@jupyterlab/vega5-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(3485), v.e(6061)]).then((() => () => v(16061))))),
         68433: () => P("default", "@jupyterlab/csvviewer-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1827), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(5007), v.e(2277), v.e(2782), v.e(7556), v.e(3766)]).then((() => () => v(41827))))),
-        72114: () => P("default", "@jupyter-notebook/console-extension", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(3625), v.e(5007), v.e(6985), v.e(6345)]).then((() => () => v(94645))))),
         73505: () => P("default", "@jupyterlab/running-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(7854), v.e(502), v.e(8713), v.e(1589), v.e(1997), v.e(8156), v.e(5007), v.e(7934), v.e(2782), v.e(2287), v.e(109), v.e(1317)]).then((() => () => v(97854))))),
+        73598: () => P("default", "@jupyter-notebook/help-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(8156), v.e(7556), v.e(5744), v.e(9380)]).then((() => () => v(19380))))),
         75845: () => P("default", "@jupyterlab/notebook-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1962), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(8156), v.e(3625), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(7934), v.e(7568), v.e(9113), v.e(9503), v.e(7231), v.e(7556), v.e(2287), v.e(109), v.e(5012), v.e(3072), v.e(3766), v.e(7253), v.e(4323), v.e(8802), v.e(5964), v.e(2867), v.e(4778), v.e(9469), v.e(2964), v.e(8126), v.e(2621)]).then((() => () => v(51962))))),
+        76933: () => P("default", "@jupyter-notebook/notebook-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(8156), v.e(2277), v.e(7934), v.e(7556), v.e(109), v.e(4323), v.e(5573)]).then((() => () => v(5573))))),
         77306: () => P("default", "@jupyterlab/markdownviewer-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(5007), v.e(2277), v.e(1709), v.e(3072), v.e(3785), v.e(7252)]).then((() => () => v(79685))))),
         79982: () => P("default", "@jupyterlab/theme-light-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(5426)]).then((() => () => v(45426))))),
+        81715: () => P("default", "@jupyter-notebook/application-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(5007), v.e(2277), v.e(1709), v.e(2549), v.e(2782), v.e(7556), v.e(109), v.e(6985), v.e(5744), v.e(8579)]).then((() => () => v(88579))))),
         82985: () => P("default", "@jupyterlab/mathjax-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(1709), v.e(1408)]).then((() => () => v(11408))))),
         88765: () => P("default", "@jupyterlab/ui-components-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1589), v.e(3863)]).then((() => () => v(73863))))),
         94415: () => P("default", "@jupyterlab/mermaid-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(6561), v.e(9161)]).then((() => () => v(79161))))),
+        97793: () => P("default", "@jupyter-notebook/docmanager-extension", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(1997), v.e(109), v.e(8875)]).then((() => () => v(71650))))),
         98269: () => P("default", "@jupyterlab/shortcuts-extension", [2, 5, 0, 0, , "beta", 1], (() => Promise.all([v.e(113), v.e(998), v.e(502), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(2277), v.e(2549), v.e(8395), v.e(6934), v.e(554)]).then((() => () => v(113))))),
         98947: () => P("default", "@jupyterlab/pdf-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(3485), v.e(2549), v.e(4058)]).then((() => () => v(84058))))),
         99932: () => P("default", "@jupyterlab/documentsearch-extension", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(502), v.e(8713), v.e(3485), v.e(5007), v.e(2277), v.e(3766), v.e(4212)]).then((() => () => v(24212))))),
         3546: () => f("default", "@codemirror/view", [2, 6, 26, 1], (() => Promise.all([v.e(2955), v.e(9843)]).then((() => () => v(22955))))),
         89843: () => f("default", "@codemirror/state", [2, 6, 4, 1], (() => v.e(2323).then((() => () => v(92323))))),
         79352: () => f("default", "@lezer/common", [2, 1, 2, 1], (() => v.e(7997).then((() => () => v(97997))))),
         17592: () => P("default", "@codemirror/language", [1, 6, 10, 1], (() => Promise.all([v.e(1584), v.e(3546), v.e(9843), v.e(9352), v.e(2209)]).then((() => () => v(31584))))),
@@ -282,29 +283,29 @@
         2277: () => f("default", "@jupyterlab/settingregistry", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(7796), v.e(5649), v.e(998), v.e(1997), v.e(2549), v.e(6934)]).then((() => () => v(5649))))),
         61709: () => f("default", "@jupyterlab/rendermime", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(2401), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1997), v.e(9983), v.e(5012), v.e(6642), v.e(6982)]).then((() => () => v(72401))))),
         2549: () => f("default", "@lumino/disposable", [2, 2, 1, 2], (() => Promise.all([v.e(1997), v.e(5451)]).then((() => () => v(65451))))),
         42782: () => P("default", "@jupyterlab/docregistry", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(2489), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(2549), v.e(9503), v.e(7231)]).then((() => () => v(72489))))),
         17556: () => f("default", "@jupyterlab/mainmenu", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(3485), v.e(1589), v.e(3625), v.e(2607)]).then((() => () => v(12007))))),
         70109: () => f("default", "@jupyterlab/docmanager", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(7543), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(2549), v.e(7934), v.e(2782), v.e(7568), v.e(9503), v.e(4421)]).then((() => () => v(37543))))),
         96985: () => f("default", "@jupyterlab/console", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(2636), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(9983), v.e(1709), v.e(5012), v.e(3546), v.e(9843), v.e(9615), v.e(2867), v.e(7508)]).then((() => () => v(72636))))),
-        21481: () => P("default", "@jupyter-notebook/ui-components", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(1589), v.e(9068)]).then((() => () => v(59068))))),
+        75744: () => P("default", "@jupyter-notebook/ui-components", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(1589), v.e(9068)]).then((() => () => v(59068))))),
         31589: () => f("default", "@jupyterlab/ui-components", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(755), v.e(7811), v.e(2557), v.e(998), v.e(502), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(2549), v.e(7934), v.e(9503), v.e(4421), v.e(6934), v.e(4475), v.e(8005), v.e(4885)]).then((() => () => v(2557))))),
         81997: () => f("default", "@lumino/signaling", [2, 2, 1, 2], (() => Promise.all([v.e(998), v.e(3625), v.e(409)]).then((() => () => v(40409))))),
         33625: () => f("default", "@lumino/algorithm", [2, 2, 0, 1], (() => v.e(5614).then((() => () => v(15614))))),
         97934: () => P("default", "@lumino/polling", [1, 2, 1, 2], (() => Promise.all([v.e(998), v.e(1997), v.e(4271)]).then((() => () => v(64271))))),
         49503: () => f("default", "@lumino/messaging", [2, 2, 0, 1], (() => Promise.all([v.e(7821), v.e(3625)]).then((() => () => v(77821))))),
         14421: () => f("default", "@lumino/properties", [2, 2, 0, 1], (() => v.e(3733).then((() => () => v(13733))))),
         43766: () => f("default", "@jupyterlab/documentsearch", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(6999), v.e(998), v.e(502), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(2549), v.e(7934), v.e(6934)]).then((() => () => v(36999))))),
         78156: () => f("default", "react", [2, 18, 2, 0], (() => v.e(7378).then((() => () => v(27378))))),
         44323: () => f("default", "@jupyterlab/notebook", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(374), v.e(998), v.e(8713), v.e(3485), v.e(1589), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(9503), v.e(7231), v.e(8395), v.e(5012), v.e(4421), v.e(3072), v.e(3766), v.e(4475), v.e(5964), v.e(9615), v.e(2867), v.e(7508), v.e(6642)]).then((() => () => v(90374))))),
         78529: () => f("default", "@jupyterlab/terminal", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(502), v.e(3485), v.e(9503), v.e(8395), v.e(3213)]).then((() => () => v(53213))))),
         58802: () => f("default", "@jupyterlab/filebrowser", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(9341), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(7934), v.e(2782), v.e(7568), v.e(9113), v.e(9503), v.e(8395), v.e(109), v.e(4475), v.e(9615)]).then((() => () => v(39341))))),
         91317: () => P("default", "@jupyterlab/running", [1, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1809), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(2549), v.e(8395)]).then((() => () => v(1809))))),
         43959: () => f("default", "@jupyterlab/settingeditor", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(3360), v.e(998), v.e(3485), v.e(1997), v.e(8156), v.e(3625), v.e(9983), v.e(1709), v.e(7934), v.e(7231), v.e(2287), v.e(7478)]).then((() => () => v(63360))))),
-        69224: () => f("default", "@jupyter-notebook/tree", [2, 7, 2, 0, , "beta", 0], (() => Promise.all([v.e(998), v.e(4837)]).then((() => () => v(73146))))),
+        28678: () => f("default", "@jupyter-notebook/tree", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(4837)]).then((() => () => v(73146))))),
         17843: () => f("default", "yjs", [2, 13, 6, 8], (() => v.e(7957).then((() => () => v(67957))))),
         47568: () => f("default", "@jupyterlab/statusbar", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(998), v.e(3485), v.e(8156), v.e(3625), v.e(2549), v.e(7639)]).then((() => () => v(53680))))),
         12287: () => f("default", "@jupyterlab/statedb", [2, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(4526), v.e(998), v.e(1997), v.e(4421)]).then((() => () => v(34526))))),
         16934: () => f("default", "@lumino/commands", [2, 2, 3, 0], (() => Promise.all([v.e(3301), v.e(998), v.e(1997), v.e(3625), v.e(2549), v.e(8395), v.e(554)]).then((() => () => v(43301))))),
         22964: () => P("default", "@jupyterlab/property-inspector", [1, 4, 2, 0, , "beta", 1], (() => Promise.all([v.e(1997), v.e(8907)]).then((() => () => v(41198))))),
         59341: () => f("default", "@jupyterlab/services", [2, 7, 2, 0, , "beta", 1], (() => Promise.all([v.e(3676), v.e(998), v.e(1997), v.e(9983), v.e(2549), v.e(7934), v.e(2287)]).then((() => () => v(83676))))),
         34771: () => f("default", "@lumino/application", [2, 2, 3, 1], (() => Promise.all([v.e(6731), v.e(6934)]).then((() => () => v(16731))))),
@@ -354,15 +355,14 @@
         53: [60053],
         109: [70109],
         502: [60502],
         554: [80554],
         998: [20998],
         1120: [51120],
         1317: [91317],
-        1481: [21481],
         1589: [31589],
         1709: [61709],
         1997: [81997],
         2069: [94152],
         2122: [31560],
         2123: [32123],
         2209: [92209],
@@ -392,24 +392,24 @@
         4475: [24475],
         4771: [34771],
         4778: [24778],
         4877: [84877],
         4885: [24885],
         5007: [25007],
         5012: [95012],
+        5744: [75744],
         5964: [35964],
         6017: [94571],
         6139: [92736],
         6561: [6561],
         6642: [76642],
         6934: [16934],
         6962: [47980],
         6982: [96982],
         6985: [96985],
-        7057: [37057],
         7231: [97231],
         7253: [57253],
         7401: [27401],
         7478: [27478],
         7508: [57508],
         7556: [17556],
         7568: [47568],
@@ -418,20 +418,21 @@
         7925: [67925],
         7934: [97934],
         8005: [38005],
         8126: [98126],
         8156: [78156],
         8395: [18395],
         8529: [78529],
+        8678: [28678],
         8713: [95297],
-        8781: [1542, 2344, 2438, 6999, 7221, 8997, 8998, 9135, 10253, 12427, 13318, 16557, 19199, 21113, 23955, 24351, 25763, 25950, 27909, 31663, 35761, 38896, 40545, 45317, 46030, 49938, 51701, 51973, 58524, 59123, 60679, 62430, 64209, 64253, 65097, 65529, 68433, 72114, 73505, 75845, 77306, 79982, 82985, 88765, 94415, 98269, 98947, 99932],
+        8781: [1542, 2344, 2438, 3708, 6999, 7221, 8997, 8998, 9135, 10253, 12427, 13318, 14745, 16557, 19199, 23955, 24351, 25763, 25950, 27909, 29194, 35761, 40835, 45317, 46030, 49938, 51267, 51701, 51973, 60679, 62430, 64209, 65097, 65529, 68433, 73505, 73598, 75845, 76933, 77306, 79982, 81715, 82985, 88765, 94415, 97793, 98269, 98947, 99932],
         8802: [58802],
+        8856: [28856],
         9072: [59072],
         9113: [59341],
-        9224: [69224],
         9352: [79352],
         9469: [69469],
         9503: [49503],
         9615: [99615],
         9843: [89843],
         9853: [29853],
         9983: [9983]
@@ -460,15 +461,15 @@
         var e = {
             179: 0
         };
         v.f.j = (t, a) => {
             var l = v.o(e, t) ? e[t] : void 0;
             if (0 !== l)
                 if (l) a.push(l[2]);
-                else if (/^(1((0|58|70)9|120|317|481|997)|2(2(09|77|87)|069|123|549|621|782|867|964)|3(7(15|66|85)|(48|56|62)5|072|546|831|959)|4(3(23|29|43)|77[18]|152|421|475|877|885)|5(0(07|12|2)|3|54|964)|6(9(34|82|85)|561|642)|7(5(08|56|68|92)|057|231|253|401|478|843|925|934)|8(005|126|156|395|529|713|802)|9(98(|3)|(11|50|84|85)3|072|224|352|469|615))$/.test(t)) e[t] = 0;
+                else if (/^(1((0|58|70)9|120|317|997)|2(2(09|77|87)|069|123|549|621|782|867|964)|3(7(15|66|85)|(48|56|62)5|072|546|831|959)|4(3(23|29|43)|77[18]|152|421|475|877|885)|5(0(07|12|2)|(5|74|96)4|3)|6(9(34|82|85)|561|642)|7(5(08|56|68|92)|231|253|401|478|843|925|934)|8((12|15|85)6|005|395|529|678|713|802)|9(98(|3)|(11|50|84|85)3|072|352|469|615))$/.test(t)) e[t] = 0;
             else {
                 var r = new Promise(((a, r) => l = e[t] = [a, r]));
                 a.push(l[2] = r);
                 var n = v.p + v.u(t),
                     o = new Error;
                 v.l(n, (a => {
                     if (v.o(e, t) && (0 !== (l = e[t]) && (e[t] = void 0), l)) {
```

### Comparing `notebook-7.2.0b0/notebook/static/c49810b53ecc0d87d802.woff` & `notebook-7.2.0b1/notebook/static/c49810b53ecc0d87d802.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/c56da8d69f1a0208b8e0.woff` & `notebook-7.2.0b1/notebook/static/c56da8d69f1a0208b8e0.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/cb9e9e693192413cde2b.woff` & `notebook-7.2.0b1/notebook/static/cb9e9e693192413cde2b.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/cda59d6efffa685830fd.ttf` & `notebook-7.2.0b1/notebook/static/cda59d6efffa685830fd.ttf`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/e4299464e7b012968eed.eot` & `notebook-7.2.0b1/notebook/static/e4299464e7b012968eed.eot`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/e42a88444448ac3d6054.woff2` & `notebook-7.2.0b1/notebook/static/e42a88444448ac3d6054.woff2`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/e8711bbb871afd8e9dea.ttf` & `notebook-7.2.0b1/notebook/static/e8711bbb871afd8e9dea.ttf`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/f9217f66874b0c01cd8c.woff` & `notebook-7.2.0b1/notebook/static/f9217f66874b0c01cd8c.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/fc6ddf5df402b263cfb1.woff` & `notebook-7.2.0b1/notebook/static/fc6ddf5df402b263cfb1.woff`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/static/third-party-licenses.json` & `notebook-7.2.0b1/notebook/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966922005571031%*

 * *Differences: {"'packages'": "{23: {'versionInfo': '7.2.0-beta.1'}, 24: {'versionInfo': '7.2.0-beta.1'}, 25: "*

 * *               "{'versionInfo': '7.2.0-beta.1'}, 26: {'versionInfo': '7.2.0-beta.1'}, 27: "*

 * *               "{'versionInfo': '7.2.0-beta.1'}, 28: {'versionInfo': '7.2.0-beta.1'}, 29: "*

 * *               "{'versionInfo': '7.2.0-beta.1'}, 30: {'versionInfo': '7.2.0-beta.1'}, 31: "*

 * *               "{'versionInfo': '7.2.0-beta.1'}, 32: {'versionInfo': '7.2.0-beta.1'}, 33: "*

 * *               "{'versionInfo': '7.2.0-beta.1'} […]*

```diff
@@ -138,75 +138,75 @@
             "name": "@fortawesome/fontawesome-free",
             "versionInfo": "5.15.4"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/application",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/application-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/console-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/docmanager-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/documentsearch-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/help-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/notebook-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/terminal-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/tree",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/tree-extension",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-notebook/ui-components",
-            "versionInfo": "7.2.0-beta.0"
+            "versionInfo": "7.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/react-components",
             "versionInfo": "0.15.2"
         },
@@ -689,14 +689,20 @@
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/theme-dark-extension",
             "versionInfo": "4.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
+            "name": "@jupyterlab/theme-dark-high-contrast-extension",
+            "versionInfo": "4.2.0-beta.1"
+        },
+        {
+            "extractedText": "",
+            "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/theme-light-extension",
             "versionInfo": "4.2.0-beta.1"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/toc",
```

### Comparing `notebook-7.2.0b0/notebook/templates/consoles.html` & `notebook-7.2.0b1/notebook/templates/consoles.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/templates/edit.html` & `notebook-7.2.0b1/notebook/templates/edit.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/templates/error.html` & `notebook-7.2.0b1/notebook/templates/error.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/templates/notebooks.html` & `notebook-7.2.0b1/notebook/templates/notebooks.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/templates/terminals.html` & `notebook-7.2.0b1/notebook/templates/terminals.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/notebook/templates/tree.html` & `notebook-7.2.0b1/notebook/templates/tree.html`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/tests/conftest.py` & `notebook-7.2.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/tests/test_app.py` & `notebook-7.2.0b1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/.gitignore` & `notebook-7.2.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/LICENSE` & `notebook-7.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/README.md` & `notebook-7.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/pyproject.toml` & `notebook-7.2.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `notebook-7.2.0b0/PKG-INFO` & `notebook-7.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: notebook
-Version: 7.2.0b0
+Version: 7.2.0b1
 Summary: Jupyter Notebook - A web-based notebook environment for interactive computing
 Project-URL: Documentation, https://jupyter-notebook.readthedocs.io/
 Project-URL: Homepage, https://github.com/jupyter/notebook
 Project-URL: Source, https://github.com/jupyter/notebook
 Project-URL: Tracker, https://github.com/jupyter/notebook/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

