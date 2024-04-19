# Comparing `tmp/selenium_driverless-1.9.tar.gz` & `tmp/selenium_driverless-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.9.tar", last modified: Wed Apr 17 11:26:49 2024, max compression
+gzip compressed data, was "selenium_driverless-1.9.1.tar", last modified: Fri Apr 19 12:43:46 2024, max compression
```

## Comparing `selenium_driverless-1.9.tar` & `selenium_driverless-1.9.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.804611 selenium_driverless-1.9/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.734253 selenium_driverless-1.9/.github/
--rw-rw-rw-   0        0        0      512 2023-10-29 12:51:12.000000 selenium_driverless-1.9/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.738253 selenium_driverless-1.9/.github/workflows/
--rw-rw-rw-   0        0        0      905 2023-10-29 12:51:12.000000 selenium_driverless-1.9/.github/workflows/dependency-review.yml
--rw-rw-rw-   0        0        0      738 2023-09-19 13:08:57.000000 selenium_driverless-1.9/LICENSE.md
--rw-rw-rw-   0        0        0      185 2023-11-30 15:16:31.000000 selenium_driverless-1.9/MANIFEST.in
--rw-rw-rw-   0        0        0    13633 2024-04-17 11:26:49.802610 selenium_driverless-1.9/PKG-INFO
--rw-rw-rw-   0        0        0    12052 2024-04-17 11:26:14.000000 selenium_driverless-1.9/README.md
--rw-rw-rw-   0        0        0      696 2024-01-29 19:33:57.000000 selenium_driverless-1.9/build_upload.md
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.745241 selenium_driverless-1.9/dev/
--rw-rw-rw-   0        0        0     1112 2024-03-28 13:55:11.000000 selenium_driverless-1.9/dev/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.863731 selenium_driverless-1.9/dev/assets/
--rw-rw-rw-   0        0        0   429242 2023-08-27 15:04:01.000000 selenium_driverless-1.9/dev/assets/bypass_turnstile.mp4
--rw-rw-rw-   0        0        0    12478 2023-08-19 09:44:36.000000 selenium_driverless-1.9/dev/assets/events_mouse.png
--rw-rw-rw-   0        0        0     6691 2023-08-19 09:42:33.000000 selenium_driverless-1.9/dev/assets/events_mousepad.png
--rw-rw-rw-   0        0        0   166789 2024-03-28 13:50:09.000000 selenium_driverless-1.9/dev/assets/heatmap.png
--rw-rw-rw-   0        0        0    98170 2023-08-26 16:55:56.000000 selenium_driverless-1.9/dev/assets/mouse_path_gen.png
--rw-rw-rw-   0        0        0    40709 2023-08-26 16:54:15.000000 selenium_driverless-1.9/dev/assets/mousemove_events_gen.png
--rw-rw-rw-   0        0        0    38402 2023-08-26 17:36:05.000000 selenium_driverless-1.9/dev/assets/mousemove_events_test_sample_based.png
--rw-rw-rw-   0        0        0    88273 2023-08-26 19:31:36.000000 selenium_driverless-1.9/dev/assets/mousemove_events_test_samples_based.png
--rw-rw-rw-   0        0        0    10468 2023-08-19 09:33:39.000000 selenium_driverless-1.9/dev/assets/real_mouse_path.png
--rw-rw-rw-   0        0        0     2109 2024-01-24 23:45:42.000000 selenium_driverless-1.9/dev/human_like_path.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.881453 selenium_driverless-1.9/docs/
--rw-rw-rw-   0        0        0      234 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/.buildinfo
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.077910 selenium_driverless-1.9/docs/.doctrees/
--rw-rw-rw-   0        0        0  2696582 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/.doctrees/environment.pickle
--rw-rw-rw-   0        0        0     7192 2024-04-17 10:22:19.000000 selenium_driverless-1.9/docs/.doctrees/index.doctree
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.082918 selenium_driverless-1.9/docs/_modules/
--rw-rw-rw-   0        0        0     5232 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/_modules/index.html
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.672089 selenium_driverless-1.9/docs/_modules/selenium_driverless/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.671089 selenium_driverless-1.9/docs/_modules/selenium_driverless/types/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.087907 selenium_driverless-1.9/docs/_modules/selenium_driverless/types/options/
--rw-rw-rw-   0        0        0    50445 2024-04-17 11:22:39.000000 selenium_driverless-1.9/docs/_modules/selenium_driverless/types/options/index.html
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.096926 selenium_driverless-1.9/docs/_modules/selenium_driverless/webdriver/
--rw-rw-rw-   0        0        0   241680 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/_modules/selenium_driverless/webdriver/index.html
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.119706 selenium_driverless-1.9/docs/_sources/
--rw-rw-rw-   0        0        0     1425 2024-04-16 23:06:25.000000 selenium_driverless-1.9/docs/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.186585 selenium_driverless-1.9/docs/_static/
--rw-rw-rw-   0        0        0     4289 2024-04-17 11:22:37.000000 selenium_driverless-1.9/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    16018 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/basic.css
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.193718 selenium_driverless-1.9/docs/_static/css/
--rw-rw-rw-   0        0        0     3229 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.524370 selenium_driverless-1.9/docs/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   444379 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   135314 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/css/theme.css
--rw-rw-rw-   0        0        0     4472 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/doctools.js
--rw-rw-rw-   0        0        0      345 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/file.png
--rw-rw-rw-   0        0        0    89501 2024-04-17 11:22:37.000000 selenium_driverless-1.9/docs/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.561036 selenium_driverless-1.9/docs/_static/js/
--rw-rw-rw-   0        0        0      934 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4370 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2734 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2024-01-23 15:14:55.000000 selenium_driverless-1.9/docs/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/minus.png
--rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/plus.png
--rw-rw-rw-   0        0        0     4976 2024-04-17 11:22:38.000000 selenium_driverless-1.9/docs/_static/pygments.css
--rw-rw-rw-   0        0        0    18732 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/searchtools.js
--rw-rw-rw-   0        0        0     5123 2024-01-23 09:09:05.000000 selenium_driverless-1.9/docs/_static/sphinx_highlight.js
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.564684 selenium_driverless-1.9/docs/genindex/
--rw-rw-rw-   0        0        0    83639 2024-04-17 11:22:39.000000 selenium_driverless-1.9/docs/genindex/index.html
--rw-rw-rw-   0        0        0    14429 2024-04-17 11:22:39.000000 selenium_driverless-1.9/docs/index.html
--rw-rw-rw-   0        0        0     3220 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/objects.inv
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.576692 selenium_driverless-1.9/docs/search/
--rw-rw-rw-   0        0        0     4666 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/search/index.html
--rw-rw-rw-   0        0        0    44475 2024-04-17 11:22:40.000000 selenium_driverless-1.9/docs/searchindex.js
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.585683 selenium_driverless-1.9/docs_source/
--rw-rw-rw-   0        0        0     1394 2024-03-28 15:03:07.000000 selenium_driverless-1.9/docs_source/conf.py
--rw-rw-rw-   0        0        0     1425 2024-04-16 23:06:25.000000 selenium_driverless-1.9/docs_source/index.rst
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.591689 selenium_driverless-1.9/examples/
--rw-rw-rw-   0        0        0      661 2024-01-13 02:29:22.000000 selenium_driverless-1.9/examples/proxy_with_auth.py
--rw-rw-rw-   0        0        0      330 2023-09-19 13:08:57.000000 selenium_driverless-1.9/main.py
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.9/pyproject.toml
--rw-rw-rw-   0        0        0      288 2024-04-16 12:32:39.000000 selenium_driverless-1.9/requirements.txt
--rw-rw-rw-   0        0        0      133 2024-04-17 11:26:49.809702 selenium_driverless-1.9/setup.cfg
--rw-rw-rw-   0        0        0     1997 2024-03-28 14:43:45.000000 selenium_driverless-1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:48.684090 selenium_driverless-1.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.602702 selenium_driverless-1.9/src/selenium_driverless/
--rw-rw-rw-   0        0        0       90 2024-04-17 11:24:02.000000 selenium_driverless-1.9/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.628866 selenium_driverless-1.9/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.9/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.629863 selenium_driverless-1.9/src/selenium_driverless/files/js/
--rw-rw-rw-   0        0        0     7941 2023-09-27 20:37:25.000000 selenium_driverless-1.9/src/selenium_driverless/files/js/show_mousemove.js
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.635890 selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/
--rw-rw-rw-   0        0        0      866 2023-07-06 16:49:03.000000 selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js
--rw-rw-rw-   0        0        0     1895 2024-01-25 12:59:36.000000 selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.639862 selenium_driverless-1.9/src/selenium_driverless/input/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.9/src/selenium_driverless/input/__init__.py
--rw-rw-rw-   0        0        0    11698 2024-04-17 10:38:30.000000 selenium_driverless-1.9/src/selenium_driverless/input/pointer.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.661876 selenium_driverless-1.9/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     4079 2024-02-03 16:33:48.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/driver_utils.py
--rw-rw-rw-   0        0        0     5933 2024-04-17 10:04:35.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/geometry.py
--rw-rw-rw-   0        0        0    30549 2024-04-17 10:35:33.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/network_interceptor.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/prefs.py
--rw-rw-rw-   0        0        0     6830 2024-03-28 15:00:20.000000 selenium_driverless-1.9/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.701167 selenium_driverless-1.9/src/selenium_driverless/sync/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.9/src/selenium_driverless/sync/__init__.py
--rw-rw-rw-   0        0        0     1102 2023-09-19 13:27:55.000000 selenium_driverless-1.9/src/selenium_driverless/sync/alert.py
--rw-rw-rw-   0        0        0     1300 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/base_target.py
--rw-rw-rw-   0        0        0     1377 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/context.py
--rw-rw-rw-   0        0        0     1244 2023-09-19 13:06:07.000000 selenium_driverless-1.9/src/selenium_driverless/sync/executor.py
--rw-rw-rw-   0        0        0     1124 2023-09-19 13:27:55.000000 selenium_driverless-1.9/src/selenium_driverless/sync/pointer.py
--rw-rw-rw-   0        0        0     1111 2023-09-19 13:27:55.000000 selenium_driverless-1.9/src/selenium_driverless/sync/switch_to.py
--rw-rw-rw-   0        0        0     1446 2024-02-03 16:33:48.000000 selenium_driverless-1.9/src/selenium_driverless/sync/target.py
--rw-rw-rw-   0        0        0     1420 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/webdriver.py
--rw-rw-rw-   0        0        0     1615 2023-12-16 21:52:11.000000 selenium_driverless-1.9/src/selenium_driverless/sync/webelement.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.743602 selenium_driverless-1.9/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0      631 2023-09-25 19:30:05.000000 selenium_driverless-1.9/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     4151 2024-01-24 23:45:42.000000 selenium_driverless-1.9/src/selenium_driverless/types/alert.py
--rw-rw-rw-   0        0        0     5749 2024-04-16 21:43:55.000000 selenium_driverless-1.9/src/selenium_driverless/types/base_target.py
--rw-rw-rw-   0        0        0     1184 2024-03-28 15:03:07.000000 selenium_driverless-1.9/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    41099 2024-04-17 11:07:13.000000 selenium_driverless-1.9/src/selenium_driverless/types/context.py
--rw-rw-rw-   0        0        0    29930 2024-02-03 11:02:55.000000 selenium_driverless-1.9/src/selenium_driverless/types/deserialize.py
--rw-rw-rw-   0        0        0    13951 2024-03-10 10:13:26.000000 selenium_driverless-1.9/src/selenium_driverless/types/options.py
--rw-rw-rw-   0        0        0    57931 2024-04-17 11:08:17.000000 selenium_driverless-1.9/src/selenium_driverless/types/target.py
--rw-rw-rw-   0        0        0    38016 2024-04-17 11:22:35.000000 selenium_driverless-1.9/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.753615 selenium_driverless-1.9/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.9/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     5340 2024-03-28 18:41:47.000000 selenium_driverless-1.9/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    66796 2024-04-17 11:07:13.000000 selenium_driverless-1.9/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.797663 selenium_driverless-1.9/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0    13633 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-17 11:26:48.000000 selenium_driverless-1.9/src/selenium_driverless.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      223 2023-09-19 13:08:57.000000 selenium_driverless-1.9/sync_main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.780683 selenium_driverless-1.9/tests/
--rw-rw-rw-   0        0        0     1884 2024-04-17 10:45:25.000000 selenium_driverless-1.9/tests/bypass_turnstile.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:26:49.792611 selenium_driverless-1.9/tests/selenium_detector/
--rw-rw-rw-   0        0        0     1054 2024-04-17 11:18:06.000000 selenium_driverless-1.9/tests/selenium_detector/selenium_detector.py
--rw-rw-rw-   0        0        0     1036 2024-04-17 11:19:31.000000 selenium_driverless-1.9/tests/selenium_detector/sync_selenium_detector.py
--rw-rw-rw-   0        0        0     1102 2024-04-17 10:22:08.000000 selenium_driverless-1.9/tests/show_mousemove.py
--rw-rw-rw-   0        0        0     1637 2024-03-28 18:46:42.000000 selenium_driverless-1.9/tests/target_interception.py
--rw-rw-rw-   0        0        0     4539 2024-04-17 11:19:31.000000 selenium_driverless-1.9/tests/test_driverless.py
--rw-rw-rw-   0        0        0    23694 2024-04-17 10:45:41.000000 selenium_driverless-1.9/tests/turnstile_captcha.png
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:46.092455 selenium_driverless-1.9.1/
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:44.980949 selenium_driverless-1.9.1/.github/
+-rw-rw-rw-   0        0        0      512 2023-10-29 12:51:12.000000 selenium_driverless-1.9.1/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:44.984244 selenium_driverless-1.9.1/.github/workflows/
+-rw-rw-rw-   0        0        0      905 2023-10-29 12:51:12.000000 selenium_driverless-1.9.1/.github/workflows/dependency-review.yml
+-rw-rw-rw-   0        0        0      738 2023-09-19 13:08:57.000000 selenium_driverless-1.9.1/LICENSE.md
+-rw-rw-rw-   0        0        0      185 2023-11-30 15:16:31.000000 selenium_driverless-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12553 2024-04-19 12:43:46.089922 selenium_driverless-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10970 2024-04-19 12:20:22.000000 selenium_driverless-1.9.1/README.md
+-rw-rw-rw-   0        0        0      696 2024-01-29 19:33:57.000000 selenium_driverless-1.9.1/build_upload.md
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:44.991496 selenium_driverless-1.9.1/dev/
+-rw-rw-rw-   0        0        0     1112 2024-03-28 13:55:11.000000 selenium_driverless-1.9.1/dev/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.088077 selenium_driverless-1.9.1/dev/assets/
+-rw-rw-rw-   0        0        0   429242 2023-08-27 15:04:01.000000 selenium_driverless-1.9.1/dev/assets/bypass_turnstile.mp4
+-rw-rw-rw-   0        0        0    12478 2023-08-19 09:44:36.000000 selenium_driverless-1.9.1/dev/assets/events_mouse.png
+-rw-rw-rw-   0        0        0     6691 2023-08-19 09:42:33.000000 selenium_driverless-1.9.1/dev/assets/events_mousepad.png
+-rw-rw-rw-   0        0        0   166789 2024-03-28 13:50:09.000000 selenium_driverless-1.9.1/dev/assets/heatmap.png
+-rw-rw-rw-   0        0        0    98170 2023-08-26 16:55:56.000000 selenium_driverless-1.9.1/dev/assets/mouse_path_gen.png
+-rw-rw-rw-   0        0        0    40709 2023-08-26 16:54:15.000000 selenium_driverless-1.9.1/dev/assets/mousemove_events_gen.png
+-rw-rw-rw-   0        0        0    38402 2023-08-26 17:36:05.000000 selenium_driverless-1.9.1/dev/assets/mousemove_events_test_sample_based.png
+-rw-rw-rw-   0        0        0    88273 2023-08-26 19:31:36.000000 selenium_driverless-1.9.1/dev/assets/mousemove_events_test_samples_based.png
+-rw-rw-rw-   0        0        0    10468 2023-08-19 09:33:39.000000 selenium_driverless-1.9.1/dev/assets/real_mouse_path.png
+-rw-rw-rw-   0        0        0     2109 2024-01-24 23:45:42.000000 selenium_driverless-1.9.1/dev/human_like_path.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.113711 selenium_driverless-1.9.1/docs/
+-rw-rw-rw-   0        0        0      234 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/.buildinfo
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.306033 selenium_driverless-1.9.1/docs/.doctrees/
+-rw-rw-rw-   0        0        0  2762868 2024-04-19 12:42:30.000000 selenium_driverless-1.9.1/docs/.doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     7192 2024-04-19 12:42:02.000000 selenium_driverless-1.9.1/docs/.doctrees/index.doctree
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.337898 selenium_driverless-1.9.1/docs/_modules/
+-rw-rw-rw-   0        0        0     5230 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/_modules/index.html
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:44.885668 selenium_driverless-1.9.1/docs/_modules/selenium_driverless/
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:44.884666 selenium_driverless-1.9.1/docs/_modules/selenium_driverless/types/
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.366613 selenium_driverless-1.9.1/docs/_modules/selenium_driverless/types/options/
+-rw-rw-rw-   0        0        0    50737 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/_modules/selenium_driverless/types/options/index.html
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.380029 selenium_driverless-1.9.1/docs/_modules/selenium_driverless/webdriver/
+-rw-rw-rw-   0        0        0   241396 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/_modules/selenium_driverless/webdriver/index.html
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.411072 selenium_driverless-1.9.1/docs/_sources/
+-rw-rw-rw-   0        0        0     1425 2024-04-16 23:06:25.000000 selenium_driverless-1.9.1/docs/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.480548 selenium_driverless-1.9.1/docs/_static/
+-rw-rw-rw-   0        0        0     4289 2024-04-19 12:42:25.000000 selenium_driverless-1.9.1/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-rw-   0        0        0    16018 2024-04-19 12:42:30.000000 selenium_driverless-1.9.1/docs/_static/basic.css
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.489841 selenium_driverless-1.9.1/docs/_static/css/
+-rw-rw-rw-   0        0        0     3229 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.775897 selenium_driverless-1.9.1/docs/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   135314 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/css/theme.css
+-rw-rw-rw-   0        0        0     4472 2024-01-23 09:09:05.000000 selenium_driverless-1.9.1/docs/_static/doctools.js
+-rw-rw-rw-   0        0        0      343 2024-04-19 12:42:30.000000 selenium_driverless-1.9.1/docs/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2024-01-23 09:09:05.000000 selenium_driverless-1.9.1/docs/_static/file.png
+-rw-rw-rw-   0        0        0    89501 2024-04-19 12:42:25.000000 selenium_driverless-1.9.1/docs/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.806055 selenium_driverless-1.9.1/docs/_static/js/
+-rw-rw-rw-   0        0        0      934 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4370 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2734 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2024-01-23 15:14:55.000000 selenium_driverless-1.9.1/docs/_static/js/theme.js
+-rw-rw-rw-   0        0        0     4957 2024-04-19 12:42:30.000000 selenium_driverless-1.9.1/docs/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.9.1/docs/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2024-01-23 09:09:05.000000 selenium_driverless-1.9.1/docs/_static/plus.png
+-rw-rw-rw-   0        0        0     4976 2024-04-19 12:42:30.000000 selenium_driverless-1.9.1/docs/_static/pygments.css
+-rw-rw-rw-   0        0        0    18732 2024-01-23 09:09:05.000000 selenium_driverless-1.9.1/docs/_static/searchtools.js
+-rw-rw-rw-   0        0        0     5123 2024-01-23 09:09:05.000000 selenium_driverless-1.9.1/docs/_static/sphinx_highlight.js
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.811046 selenium_driverless-1.9.1/docs/genindex/
+-rw-rw-rw-   0        0        0    85650 2024-04-19 12:42:31.000000 selenium_driverless-1.9.1/docs/genindex/index.html
+-rw-rw-rw-   0        0        0    14427 2024-04-19 12:42:31.000000 selenium_driverless-1.9.1/docs/index.html
+-rw-rw-rw-   0        0        0     3281 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/objects.inv
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.820533 selenium_driverless-1.9.1/docs/search/
+-rw-rw-rw-   0        0        0     4664 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/search/index.html
+-rw-rw-rw-   0        0        0    47896 2024-04-19 12:42:32.000000 selenium_driverless-1.9.1/docs/searchindex.js
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.829534 selenium_driverless-1.9.1/docs_source/
+-rw-rw-rw-   0        0        0     1394 2024-03-28 15:03:07.000000 selenium_driverless-1.9.1/docs_source/conf.py
+-rw-rw-rw-   0        0        0     1425 2024-04-16 23:06:25.000000 selenium_driverless-1.9.1/docs_source/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.833132 selenium_driverless-1.9.1/examples/
+-rw-rw-rw-   0        0        0      661 2024-01-13 02:29:22.000000 selenium_driverless-1.9.1/examples/proxy_with_auth.py
+-rw-rw-rw-   0        0        0      330 2023-09-19 13:08:57.000000 selenium_driverless-1.9.1/main.py
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0      288 2024-04-16 12:32:39.000000 selenium_driverless-1.9.1/requirements.txt
+-rw-rw-rw-   0        0        0      133 2024-04-19 12:43:46.095448 selenium_driverless-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1997 2024-03-28 14:43:45.000000 selenium_driverless-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:44.906997 selenium_driverless-1.9.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.844138 selenium_driverless-1.9.1/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       92 2024-04-19 12:17:01.000000 selenium_driverless-1.9.1/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.869153 selenium_driverless-1.9.1/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.9.1/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.871151 selenium_driverless-1.9.1/src/selenium_driverless/files/js/
+-rw-rw-rw-   0        0        0     7941 2023-09-27 20:37:25.000000 selenium_driverless-1.9.1/src/selenium_driverless/files/js/show_mousemove.js
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.878476 selenium_driverless-1.9.1/src/selenium_driverless/files/mv3_extension/
+-rw-rw-rw-   0        0        0      866 2023-07-06 16:49:03.000000 selenium_driverless-1.9.1/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js
+-rw-rw-rw-   0        0        0     1895 2024-01-25 12:59:36.000000 selenium_driverless-1.9.1/src/selenium_driverless/files/mv3_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.891424 selenium_driverless-1.9.1/src/selenium_driverless/input/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.9.1/src/selenium_driverless/input/__init__.py
+-rw-rw-rw-   0        0        0    11698 2024-04-17 10:38:30.000000 selenium_driverless-1.9.1/src/selenium_driverless/input/pointer.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.919160 selenium_driverless-1.9.1/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.9.1/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4071 2024-04-19 12:24:35.000000 selenium_driverless-1.9.1/src/selenium_driverless/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0     5933 2024-04-17 10:04:35.000000 selenium_driverless-1.9.1/src/selenium_driverless/scripts/geometry.py
+-rw-rw-rw-   0        0        0    30549 2024-04-17 10:35:33.000000 selenium_driverless-1.9.1/src/selenium_driverless/scripts/network_interceptor.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 21:52:11.000000 selenium_driverless-1.9.1/src/selenium_driverless/scripts/prefs.py
+-rw-rw-rw-   0        0        0     6770 2024-04-19 12:15:34.000000 selenium_driverless-1.9.1/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:45.963843 selenium_driverless-1.9.1/src/selenium_driverless/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/__init__.py
+-rw-rw-rw-   0        0        0     1102 2023-09-19 13:27:55.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/alert.py
+-rw-rw-rw-   0        0        0     1300 2023-12-16 21:52:11.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/base_target.py
+-rw-rw-rw-   0        0        0     1377 2023-12-16 21:52:11.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/context.py
+-rw-rw-rw-   0        0        0     1244 2023-09-19 13:06:07.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/executor.py
+-rw-rw-rw-   0        0        0     1124 2023-09-19 13:27:55.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/pointer.py
+-rw-rw-rw-   0        0        0     1111 2023-09-19 13:27:55.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/switch_to.py
+-rw-rw-rw-   0        0        0     1446 2024-02-03 16:33:48.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/target.py
+-rw-rw-rw-   0        0        0     1420 2023-12-16 21:52:11.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/webdriver.py
+-rw-rw-rw-   0        0        0     1615 2023-12-16 21:52:11.000000 selenium_driverless-1.9.1/src/selenium_driverless/sync/webelement.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:46.029968 selenium_driverless-1.9.1/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0      631 2023-09-25 19:30:05.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     4124 2024-04-19 12:29:18.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/alert.py
+-rw-rw-rw-   0        0        0     5749 2024-04-16 21:43:55.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/base_target.py
+-rw-rw-rw-   0        0        0     1184 2024-03-28 15:03:07.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    40521 2024-04-19 12:29:18.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/context.py
+-rw-rw-rw-   0        0        0    29930 2024-02-03 11:02:55.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/deserialize.py
+-rw-rw-rw-   0        0        0    14072 2024-04-19 12:23:31.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/options.py
+-rw-rw-rw-   0        0        0    59407 2024-04-19 12:42:21.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/target.py
+-rw-rw-rw-   0        0        0    39176 2024-04-19 12:41:54.000000 selenium_driverless-1.9.1/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:46.041446 selenium_driverless-1.9.1/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.9.1/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     5340 2024-03-28 18:41:47.000000 selenium_driverless-1.9.1/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    66858 2024-04-19 12:24:35.000000 selenium_driverless-1.9.1/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:46.085693 selenium_driverless-1.9.1/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0    12553 2024-04-19 12:43:44.000000 selenium_driverless-1.9.1/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2024-04-19 12:43:44.000000 selenium_driverless-1.9.1/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:43:44.000000 selenium_driverless-1.9.1/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-04-19 12:43:44.000000 selenium_driverless-1.9.1/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-19 12:43:44.000000 selenium_driverless-1.9.1/src/selenium_driverless.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      223 2023-09-19 13:08:57.000000 selenium_driverless-1.9.1/sync_main.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:46.067555 selenium_driverless-1.9.1/tests/
+-rw-rw-rw-   0        0        0     1884 2024-04-17 10:45:25.000000 selenium_driverless-1.9.1/tests/bypass_turnstile.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:43:46.079479 selenium_driverless-1.9.1/tests/selenium_detector/
+-rw-rw-rw-   0        0        0     1054 2024-04-19 11:56:32.000000 selenium_driverless-1.9.1/tests/selenium_detector/selenium_detector.py
+-rw-rw-rw-   0        0        0     1036 2024-04-17 11:19:31.000000 selenium_driverless-1.9.1/tests/selenium_detector/sync_selenium_detector.py
+-rw-rw-rw-   0        0        0     1055 2024-04-19 10:56:56.000000 selenium_driverless-1.9.1/tests/show_mousemove.py
+-rw-rw-rw-   0        0        0     1637 2024-03-28 18:46:42.000000 selenium_driverless-1.9.1/tests/target_interception.py
+-rw-rw-rw-   0        0        0     4539 2024-04-19 11:58:51.000000 selenium_driverless-1.9.1/tests/test_driverless.py
+-rw-rw-rw-   0        0        0    23694 2024-04-17 10:45:41.000000 selenium_driverless-1.9.1/tests/turnstile_captcha.png
```

### Comparing `selenium_driverless-1.9/.github/dependabot.yml` & `selenium_driverless-1.9.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/.github/workflows/dependency-review.yml` & `selenium_driverless-1.9.1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/LICENSE.md` & `selenium_driverless-1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/PKG-INFO` & `selenium_driverless-1.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.9
+Version: 1.9.1
 Summary: Undetected selenium without chromedriver usage (Non-commercial use only!)
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 License: CC BY-NC-SA 4.0
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
@@ -43,15 +43,15 @@
 
 
 - Use Selenium __without chromedriver__
 - Currently passes __Cloudflare__, __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-turnstile), and others
 - Multiple tabs simultaneously
 - Multiple Incognito-contexts with isolated cookies & local storage
 - Proxy-auth support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
-- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/))
+- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/RequestInterception/))
 - Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch))
 
 ### Questions? 
 Feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord**:)
 
 Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 <details>
@@ -128,14 +128,18 @@
 asyncio.run(main())
 
 ```
 
 ### synchronous
 asyncified, might be buggy
 
+<details>
+
+<summary>example code</summary>
+
 ```python
 from selenium_driverless.sync import webdriver
 
 options = webdriver.ChromeOptions()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.sleep(0.5)
@@ -143,14 +147,16 @@
 
     title = driver.title
     url = driver.current_url
     source = driver.page_source
     print(title)
 ```
 
+</details>
+
 ### custom debugger address
 ```python
 from selenium_driverless import webdriver
 
 options = webdriver.ChromeOptions()
 options.debugger_address = "127.0.0.1:2005"
 
@@ -199,16 +205,16 @@
 
 
 asyncio.run(main())
 ```
 
 </details>
 
-### Unique execution contexts
-- execute `javascript` without getting detected
+### Isolated execution contexts
+- execute `javascript` without getting detected ( in a **isolated world**)
 <details>
 <summary>Example Code (Click to expand)</summary>
 
 ```python
 from selenium_driverless.sync import webdriver
 from selenium_driverless import webdriver
 import asyncio
@@ -250,15 +256,14 @@
 pointer = driver.current_pointer
 move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
 
 await pointer.move_to(100, 500)
 await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
 ```
 ### Iframes
-- switch and interact with iframes
 
 ```python
 iframes = await driver.find_elements(By.TAG_NAME, "iframe")
 await asyncio.sleep(0.5)
 iframe_document = await iframes[0].content_document
 # iframe_document.find_elements(...)
 ```
@@ -320,48 +325,14 @@
 sys.modules["cdp_socket"].EXC_HANDLER = handler
 ```
 
 ## Help
 
 You found a bug? Feel free to open an issue:)
 You've got other questions or proposials? feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord** or open a discusion\
-Note: **please check the todo's below at first!**
-
-## Todo's
-<details>
-<summary>Click to expand</summary>
-
-- implementations
-  - [x] `WebElement`s
-    - [ ] improve `mid_location` calculation
-    - [ ] add `WebElement.screenshot`
-  - [x] `Input`
-      - [x] `Mouse`
-        - [x] `mousemove`
-        - [x] `click`
-        - [ ] `scroll`
-        - [ ] `drag&drop`
-      - [x] `write`
-      - [ ] `Touch`
-        - [ ] `touchmove`
-        - [ ] `TouchTap`
-        - [ ] `scoll`
-        - [ ] `pinch//zoom`
-      - [ ] `KeyBoard`
-        - [ ] `SendKeys`
-          - [ ] `send files`
-  - [ ] [support `options.add_extension()`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/37)
-  - [ ] [support prefs](https://github.com/kaliiiiiiiiii/Selenium-Driverless/discussions/92#discussioncomment-7462309)
-- [x] sync
-  - [ ] move sync to threaded for allowing event_handlers
-  - [ ] support multithreading with sync version
-    - [x] on independent driver instances
-    - [ ] on same driver instance
-- [ ] check [Python 3.12.0](https://www.python.org/downloads/release/python-3120/)
-</details>
 
 ## Authors
 
 Copyright and Author: \
 [Aurin Aegerter](mailto:aurinliun@gmx.ch) (aka **Steve**)
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selenium_driverless Version: 1.9 Summary:
+Metadata-Version: 2.1 Name: selenium_driverless Version: 1.9.1 Summary:
 Undetected selenium without chromedriver usage (Non-commercial use only!) Home-
 page: https://github.com/kaliiiiiiiiii/Selenium-Driverless Author: Aurin
 Aegerter Author-email: aurinliun@gmx.ch License: CC BY-NC-SA 4.0 Project-URL:
 Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless Project-
 URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Keywords: Selenium,webautomation Classifier: Development Status :: 2 - Pre-
@@ -25,120 +25,106 @@
 [Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use
 Selenium __without chromedriver__ - Currently passes __Cloudflare__,
 __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
 tree/master/dev#bypass-turnstile), and others - Multiple tabs simultaneously -
 Multiple Incognito-contexts with isolated cookies & local storage - Proxy-auth
 support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
 blob/dev/examples/proxy_with_auth.py)) - Network-interception ([documentation]
-(https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/
-RequestInterception/)) - Single requests ([documentation](https://
-kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/
-#selenium_driverless.types.target.Target.fetch)) ### Questions? Feel free to
-join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on
-**Discord**:) Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-
-Driverless/tree/dev) for the latest implementations. dev-installation (click to
-expand) ```shell pip uninstall -y selenium-driverless pip install https://
-github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip ```
-#### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7]
-(https://www.python.org/downloads/) * [Google-Chrome](https://www.google.de/
-chrome/) installed (Chromium not tested) ### Installing * Install [Google-
-Chrome](https://www.google.de/chrome/) * ```pip install selenium-driverless```
-### Usage ### with asyncio ```python from selenium_driverless import webdriver
-from selenium_driverless.types.by import By import asyncio async def main():
-options = webdriver.ChromeOptions() async with webdriver.Chrome
-(options=options) as driver: await driver.get('http://nowsecure.nl#relax',
-wait_load=True) await driver.sleep(0.5) await driver.wait_for_cdp
-("Page.domContentEventFired", timeout=15) # wait 10s for elem to exist elem =
-await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a',
-timeout=10) await elem.click(move_to=True) alert = await driver.switch_to.alert
-print(alert.text) await alert.accept() print(await driver.title) asyncio.run
-(main()) ``` ### synchronous asyncified, might be buggy ```python from
-selenium_driverless.sync import webdriver options = webdriver.ChromeOptions()
-with webdriver.Chrome(options=options) as driver: driver.get('http://
-nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
-("Page.domContentEventFired", timeout=15) title = driver.title url =
-driver.current_url source = driver.page_source print(title) ``` ### custom
-debugger address ```python from selenium_driverless import webdriver options =
-webdriver.ChromeOptions() options.debugger_address = "127.0.0.1:2005" # specify
-if you don't want to run remote # options.add_argument("--remote-debugging-
-port=2005") async with webdriver.Chrome(options=options) as driver: await
-driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs
-simultaneously Note: asyncio is recommended, threading only works on
-independent webdriver.Chrome instances. Example Code (Click to expand)
-```python from selenium_driverless.sync import webdriver from
-selenium_driverless.utils.utils import read from selenium_driverless import
-webdriver import asyncio async def target_1_handler(target): await target.get
-('https://abrahamjuliot.github.io/creepjs/') print(await target.title) async
-def target_2_handler(target): await target.get("about:blank") await
-target.execute_script(script=read("/files/js/show_mousemove.js")) await
-target.pointer.move_to(500, 500, total_time=2) async def main(): options =
-webdriver.ChromeOptions() async with webdriver.Chrome(options=options) as
-driver: target_1 = await driver.current_target target_2 = await
-driver.new_window("tab", activate=False) await asyncio.gather( target_1_handler
-(target_1), target_2_handler(target_2) ) await target_1.focus() input("press
-ENTER to exit") asyncio.run(main()) ``` ### Unique execution contexts - execute
-`javascript` without getting detected Example Code (Click to expand) ```python
-from selenium_driverless.sync import webdriver from selenium_driverless import
-webdriver import asyncio async def main(): options = webdriver.ChromeOptions()
-async with webdriver.Chrome(options=options) as driver: await driver.get
-('chrome://version') script = """ const proxy = new Proxy
-(document.documentElement, { get(target, prop, receiver) { if(prop ===
-"outerHTML"){ console.log('detected access on "'+prop+'"', receiver) return
-"mocked value:)" } else{return Reflect.get(...arguments)} }, });
-Object.defineProperty(document, "documentElement", { value: proxy }) """ await
-driver.execute_script(script) src = await driver.execute_script("return
+(https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/RequestInterception/))
+- Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-
+Driverless/api/Target/#selenium_driverless.types.target.Target.fetch)) ###
+Questions? Feel free to join the [Driverless-Community](https://discord.com/
+invite/MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
+kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
+dev-installation (click to expand) ```shell pip uninstall -y selenium-
+driverless pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/
+archive/refs/heads/dev.zip ``` #### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]###
+Dependencies * [Python >= 3.7](https://www.python.org/downloads/) * [Google-
+Chrome](https://www.google.de/chrome/) installed (Chromium not tested) ###
+Installing * Install [Google-Chrome](https://www.google.de/chrome/) * ```pip
+install selenium-driverless``` ### Usage ### with asyncio ```python from
+selenium_driverless import webdriver from selenium_driverless.types.by import
+By import asyncio async def main(): options = webdriver.ChromeOptions() async
+with webdriver.Chrome(options=options) as driver: await driver.get('http://
+nowsecure.nl#relax', wait_load=True) await driver.sleep(0.5) await
+driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s for
+elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div[2]/
+div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
+driver.switch_to.alert print(alert.text) await alert.accept() print(await
+driver.title) asyncio.run(main()) ``` ### synchronous asyncified, might be
+buggy example code ```python from selenium_driverless.sync import webdriver
+options = webdriver.ChromeOptions() with webdriver.Chrome(options=options) as
+driver: driver.get('http://nowsecure.nl#relax') driver.sleep(0.5)
+driver.wait_for_cdp("Page.domContentEventFired", timeout=15) title =
+driver.title url = driver.current_url source = driver.page_source print(title)
+``` ### custom debugger address ```python from selenium_driverless import
+webdriver options = webdriver.ChromeOptions() options.debugger_address =
+"127.0.0.1:2005" # specify if you don't want to run remote #
+options.add_argument("--remote-debugging-port=2005") async with
+webdriver.Chrome(options=options) as driver: await driver.get('http://
+nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs simultaneously Note:
+asyncio is recommended, threading only works on independent webdriver.Chrome
+instances. Example Code (Click to expand) ```python from
+selenium_driverless.sync import webdriver from selenium_driverless.utils.utils
+import read from selenium_driverless import webdriver import asyncio async def
+target_1_handler(target): await target.get('https://abrahamjuliot.github.io/
+creepjs/') print(await target.title) async def target_2_handler(target): await
+target.get("about:blank") await target.execute_script(script=read("/files/js/
+show_mousemove.js")) await target.pointer.move_to(500, 500, total_time=2) async
+def main(): options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: target_1 = await driver.current_target target_2 =
+await driver.new_window("tab", activate=False) await asyncio.gather
+( target_1_handler(target_1), target_2_handler(target_2) ) await target_1.focus
+() input("press ENTER to exit") asyncio.run(main()) ``` ### Isolated execution
+contexts - execute `javascript` without getting detected ( in a **isolated
+world**) Example Code (Click to expand) ```python from selenium_driverless.sync
+import webdriver from selenium_driverless import webdriver import asyncio async
+def main(): options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: await driver.get('chrome://version') script = """
+const proxy = new Proxy(document.documentElement, { get(target, prop, receiver)
+{ if(prop === "outerHTML"){ console.log('detected access on "'+prop+'"',
+receiver) return "mocked value:)" } else{return Reflect.get(...arguments)} },
+}); Object.defineProperty(document, "documentElement", { value: proxy }) """
+await driver.execute_script(script) src = await driver.execute_script("return
 document.documentElement.outerHTML", unique_context=True) mocked = await
 driver.execute_script("return document.documentElement.outerHTML",
 unique_context=False) print(src, mocked) asyncio.run(main()) ``` ### Pointer
 Interaction see [@master/dev/show_mousemove.py](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for
 visualization ```python pointer = driver.current_pointer move_kwargs =
 {"total_time": 0.7, "accel": 2, "smooth_soft": 20} await pointer.move_to(100,
 500) await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True) ```
-### Iframes - switch and interact with iframes ```python iframes = await
-driver.find_elements(By.TAG_NAME, "iframe") await asyncio.sleep(0.5)
-iframe_document = await iframes[0].content_document #
-iframe_document.find_elements(...) ``` ### use preferences ```python from
-selenium_driverless import webdriver options = webdriver.ChromeOptions() #
-recommended usage options.update_pref("download.prompt_for_download", False) #
-or options.prefs.update({"download": {"prompt_for_download": False}}) #
-supported options.add_experimental_option("prefs",
-{"download.prompt_for_download": False}) ``` ### Multiple Contexts - different
-cookies for each context - A context can have multiple windows and tabs within
-- different proxy for each context - opens as a window as incognito Example
-Code (Click to expand) ```python from selenium_driverless import webdriver
-import asyncio async def main(): options = webdriver.ChromeOptions() async with
-webdriver.Chrome(options=options) as driver: context_1 = driver.current_context
-await driver.set_auth("username", "password", "localhost:5000") # proxy not
-supported on windows due to https://bugs.chromium.org/p/chromium/issues/
-detail?id=1310057 context_2 = await driver.new_context(proxy_bypass_list=
-["localhost"], proxy_server="http://localhost:5000") await
-context_1.current_target.get("https://examle.com") await context_2.get("https:/
-/examle.com") input("press ENTER to exit:)") asyncio.run(main()) ``` ####
-Custom exception handling You can implement custom exception handling as
-following ```python import selenium_driverless import sys handler = (lambda e:
-print(f'Exception in event-handler:\n{e.__class__.__module__}.
+### Iframes ```python iframes = await driver.find_elements(By.TAG_NAME,
+"iframe") await asyncio.sleep(0.5) iframe_document = await iframes
+[0].content_document # iframe_document.find_elements(...) ``` ### use
+preferences ```python from selenium_driverless import webdriver options =
+webdriver.ChromeOptions() # recommended usage options.update_pref
+("download.prompt_for_download", False) # or options.prefs.update({"download":
+{"prompt_for_download": False}}) # supported options.add_experimental_option
+("prefs", {"download.prompt_for_download": False}) ``` ### Multiple Contexts -
+different cookies for each context - A context can have multiple windows and
+tabs within - different proxy for each context - opens as a window as incognito
+Example Code (Click to expand) ```python from selenium_driverless import
+webdriver import asyncio async def main(): options = webdriver.ChromeOptions()
+async with webdriver.Chrome(options=options) as driver: context_1 =
+driver.current_context await driver.set_auth("username", "password",
+"localhost:5000") # proxy not supported on windows due to https://
+bugs.chromium.org/p/chromium/issues/detail?id=1310057 context_2 = await
+driver.new_context(proxy_bypass_list=["localhost"], proxy_server="http://
+localhost:5000") await context_1.current_target.get("https://examle.com") await
+context_2.get("https://examle.com") input("press ENTER to exit:)") asyncio.run
+(main()) ``` #### Custom exception handling You can implement custom exception
+handling as following ```python import selenium_driverless import sys handler =
+(lambda e: print(f'Exception in event-handler:\n{e.__class__.__module__}.
 {e.__class__.__name__}: {e}', file=sys.stderr)) sys.modules
 ["selenium_driverless"].EXC_HANDLER = handler sys.modules
 ["cdp_socket"].EXC_HANDLER = handler ``` ## Help You found a bug? Feel free to
 open an issue:) You've got other questions or proposials? feel free to join the
 [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord** or
-open a discusion\ Note: **please check the todo's below at first!** ## Todo's
-Click to expand - implementations - [x] `WebElement`s - [ ] improve
-`mid_location` calculation - [ ] add `WebElement.screenshot` - [x] `Input` -
-[x] `Mouse` - [x] `mousemove` - [x] `click` - [ ] `scroll` - [ ] `drag&drop` -
-[x] `write` - [ ] `Touch` - [ ] `touchmove` - [ ] `TouchTap` - [ ] `scoll` -
-[ ] `pinch//zoom` - [ ] `KeyBoard` - [ ] `SendKeys` - [ ] `send files` - [ ]
-[support `options.add_extension()`](https://github.com/kaliiiiiiiiii/Selenium-
-Driverless/issues/37) - [ ] [support prefs](https://github.com/kaliiiiiiiiii/
-Selenium-Driverless/discussions/92#discussioncomment-7462309) - [x] sync - [ ]
-move sync to threaded for allowing event_handlers - [ ] support multithreading
-with sync version - [x] on independent driver instances - [ ] on same driver
-instance - [ ] check [Python 3.12.0](https://www.python.org/downloads/release/
-python-3120/) ## Authors Copyright and Author: \ [Aurin Aegerter](mailto:
+open a discusion\ ## Authors Copyright and Author: \ [Aurin Aegerter](mailto:
 aurinliun@gmx.ch) (aka **Steve**) ## License Shield: [![CC BY-NC-SA 4.0][cc-by-
 nc-sa-shield]][cc-by-nc-sa] Unless specified differently in a single file, this
 work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike
 4.0 International License][cc-by-nc-sa]. [![CC BY-NC-SA 4.0][cc-by-nc-sa-
 image]][cc-by-nc-sa] [cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-
 sa/4.0/ [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/
 88x31.png [cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--
```

### Comparing `selenium_driverless-1.9/README.md` & `selenium_driverless-1.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 - Use Selenium __without chromedriver__
 - Currently passes __Cloudflare__, __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-turnstile), and others
 - Multiple tabs simultaneously
 - Multiple Incognito-contexts with isolated cookies & local storage
 - Proxy-auth support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
-- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/))
+- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/RequestInterception/))
 - Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch))
 
 ### Questions? 
 Feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord**:)
 
 Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 <details>
@@ -90,14 +90,18 @@
 asyncio.run(main())
 
 ```
 
 ### synchronous
 asyncified, might be buggy
 
+<details>
+
+<summary>example code</summary>
+
 ```python
 from selenium_driverless.sync import webdriver
 
 options = webdriver.ChromeOptions()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.sleep(0.5)
@@ -105,14 +109,16 @@
 
     title = driver.title
     url = driver.current_url
     source = driver.page_source
     print(title)
 ```
 
+</details>
+
 ### custom debugger address
 ```python
 from selenium_driverless import webdriver
 
 options = webdriver.ChromeOptions()
 options.debugger_address = "127.0.0.1:2005"
 
@@ -161,16 +167,16 @@
 
 
 asyncio.run(main())
 ```
 
 </details>
 
-### Unique execution contexts
-- execute `javascript` without getting detected
+### Isolated execution contexts
+- execute `javascript` without getting detected ( in a **isolated world**)
 <details>
 <summary>Example Code (Click to expand)</summary>
 
 ```python
 from selenium_driverless.sync import webdriver
 from selenium_driverless import webdriver
 import asyncio
@@ -212,15 +218,14 @@
 pointer = driver.current_pointer
 move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
 
 await pointer.move_to(100, 500)
 await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
 ```
 ### Iframes
-- switch and interact with iframes
 
 ```python
 iframes = await driver.find_elements(By.TAG_NAME, "iframe")
 await asyncio.sleep(0.5)
 iframe_document = await iframes[0].content_document
 # iframe_document.find_elements(...)
 ```
@@ -282,48 +287,14 @@
 sys.modules["cdp_socket"].EXC_HANDLER = handler
 ```
 
 ## Help
 
 You found a bug? Feel free to open an issue:)
 You've got other questions or proposials? feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord** or open a discusion\
-Note: **please check the todo's below at first!**
-
-## Todo's
-<details>
-<summary>Click to expand</summary>
-
-- implementations
-  - [x] `WebElement`s
-    - [ ] improve `mid_location` calculation
-    - [ ] add `WebElement.screenshot`
-  - [x] `Input`
-      - [x] `Mouse`
-        - [x] `mousemove`
-        - [x] `click`
-        - [ ] `scroll`
-        - [ ] `drag&drop`
-      - [x] `write`
-      - [ ] `Touch`
-        - [ ] `touchmove`
-        - [ ] `TouchTap`
-        - [ ] `scoll`
-        - [ ] `pinch//zoom`
-      - [ ] `KeyBoard`
-        - [ ] `SendKeys`
-          - [ ] `send files`
-  - [ ] [support `options.add_extension()`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/37)
-  - [ ] [support prefs](https://github.com/kaliiiiiiiiii/Selenium-Driverless/discussions/92#discussioncomment-7462309)
-- [x] sync
-  - [ ] move sync to threaded for allowing event_handlers
-  - [ ] support multithreading with sync version
-    - [x] on independent driver instances
-    - [ ] on same driver instance
-- [ ] check [Python 3.12.0](https://www.python.org/downloads/release/python-3120/)
-</details>
 
 ## Authors
 
 Copyright and Author: \
 [Aurin Aegerter](mailto:aurinliun@gmx.ch) (aka **Steve**)
 
 ## License
```

#### html2text {}

```diff
@@ -5,119 +5,106 @@
 kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use Selenium __without
 chromedriver__ - Currently passes __Cloudflare__, __Bet365__, [Turnstile]
 (https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-
 turnstile), and others - Multiple tabs simultaneously - Multiple Incognito-
 contexts with isolated cookies & local storage - Proxy-auth support ([example
 code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/
 proxy_with_auth.py)) - Network-interception ([documentation](https://
-kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/)) -
-Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-
-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch)) ###
-Questions? Feel free to join the [Driverless-Community](https://discord.com/
-invite/MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
-kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
-dev-installation (click to expand) ```shell pip uninstall -y selenium-
-driverless pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/
-archive/refs/heads/dev.zip ``` #### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]###
-Dependencies * [Python >= 3.7](https://www.python.org/downloads/) * [Google-
-Chrome](https://www.google.de/chrome/) installed (Chromium not tested) ###
-Installing * Install [Google-Chrome](https://www.google.de/chrome/) * ```pip
-install selenium-driverless``` ### Usage ### with asyncio ```python from
-selenium_driverless import webdriver from selenium_driverless.types.by import
-By import asyncio async def main(): options = webdriver.ChromeOptions() async
-with webdriver.Chrome(options=options) as driver: await driver.get('http://
+kaliiiiiiiiii.github.io/Selenium-Driverless/api/RequestInterception/)) - Single
+requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/
+api/Target/#selenium_driverless.types.target.Target.fetch)) ### Questions? Feel
+free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3)
+on **Discord**:) Also, see [dev-branch](https://github.com/kaliiiiiiiiii/
+Selenium-Driverless/tree/dev) for the latest implementations. dev-installation
+(click to expand) ```shell pip uninstall -y selenium-driverless pip install
+https://github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip
+``` #### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >=
+3.7](https://www.python.org/downloads/) * [Google-Chrome](https://
+www.google.de/chrome/) installed (Chromium not tested) ### Installing * Install
+[Google-Chrome](https://www.google.de/chrome/) * ```pip install selenium-
+driverless``` ### Usage ### with asyncio ```python from selenium_driverless
+import webdriver from selenium_driverless.types.by import By import asyncio
+async def main(): options = webdriver.ChromeOptions() async with
+webdriver.Chrome(options=options) as driver: await driver.get('http://
 nowsecure.nl#relax', wait_load=True) await driver.sleep(0.5) await
 driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s for
 elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div[2]/
 div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
 driver.switch_to.alert print(alert.text) await alert.accept() print(await
 driver.title) asyncio.run(main()) ``` ### synchronous asyncified, might be
-buggy ```python from selenium_driverless.sync import webdriver options =
-webdriver.ChromeOptions() with webdriver.Chrome(options=options) as driver:
-driver.get('http://nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
-("Page.domContentEventFired", timeout=15) title = driver.title url =
-driver.current_url source = driver.page_source print(title) ``` ### custom
-debugger address ```python from selenium_driverless import webdriver options =
-webdriver.ChromeOptions() options.debugger_address = "127.0.0.1:2005" # specify
-if you don't want to run remote # options.add_argument("--remote-debugging-
-port=2005") async with webdriver.Chrome(options=options) as driver: await
-driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs
-simultaneously Note: asyncio is recommended, threading only works on
-independent webdriver.Chrome instances. Example Code (Click to expand)
-```python from selenium_driverless.sync import webdriver from
-selenium_driverless.utils.utils import read from selenium_driverless import
-webdriver import asyncio async def target_1_handler(target): await target.get
-('https://abrahamjuliot.github.io/creepjs/') print(await target.title) async
-def target_2_handler(target): await target.get("about:blank") await
-target.execute_script(script=read("/files/js/show_mousemove.js")) await
-target.pointer.move_to(500, 500, total_time=2) async def main(): options =
-webdriver.ChromeOptions() async with webdriver.Chrome(options=options) as
-driver: target_1 = await driver.current_target target_2 = await
-driver.new_window("tab", activate=False) await asyncio.gather( target_1_handler
-(target_1), target_2_handler(target_2) ) await target_1.focus() input("press
-ENTER to exit") asyncio.run(main()) ``` ### Unique execution contexts - execute
-`javascript` without getting detected Example Code (Click to expand) ```python
-from selenium_driverless.sync import webdriver from selenium_driverless import
-webdriver import asyncio async def main(): options = webdriver.ChromeOptions()
-async with webdriver.Chrome(options=options) as driver: await driver.get
-('chrome://version') script = """ const proxy = new Proxy
-(document.documentElement, { get(target, prop, receiver) { if(prop ===
-"outerHTML"){ console.log('detected access on "'+prop+'"', receiver) return
-"mocked value:)" } else{return Reflect.get(...arguments)} }, });
-Object.defineProperty(document, "documentElement", { value: proxy }) """ await
-driver.execute_script(script) src = await driver.execute_script("return
+buggy example code ```python from selenium_driverless.sync import webdriver
+options = webdriver.ChromeOptions() with webdriver.Chrome(options=options) as
+driver: driver.get('http://nowsecure.nl#relax') driver.sleep(0.5)
+driver.wait_for_cdp("Page.domContentEventFired", timeout=15) title =
+driver.title url = driver.current_url source = driver.page_source print(title)
+``` ### custom debugger address ```python from selenium_driverless import
+webdriver options = webdriver.ChromeOptions() options.debugger_address =
+"127.0.0.1:2005" # specify if you don't want to run remote #
+options.add_argument("--remote-debugging-port=2005") async with
+webdriver.Chrome(options=options) as driver: await driver.get('http://
+nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs simultaneously Note:
+asyncio is recommended, threading only works on independent webdriver.Chrome
+instances. Example Code (Click to expand) ```python from
+selenium_driverless.sync import webdriver from selenium_driverless.utils.utils
+import read from selenium_driverless import webdriver import asyncio async def
+target_1_handler(target): await target.get('https://abrahamjuliot.github.io/
+creepjs/') print(await target.title) async def target_2_handler(target): await
+target.get("about:blank") await target.execute_script(script=read("/files/js/
+show_mousemove.js")) await target.pointer.move_to(500, 500, total_time=2) async
+def main(): options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: target_1 = await driver.current_target target_2 =
+await driver.new_window("tab", activate=False) await asyncio.gather
+( target_1_handler(target_1), target_2_handler(target_2) ) await target_1.focus
+() input("press ENTER to exit") asyncio.run(main()) ``` ### Isolated execution
+contexts - execute `javascript` without getting detected ( in a **isolated
+world**) Example Code (Click to expand) ```python from selenium_driverless.sync
+import webdriver from selenium_driverless import webdriver import asyncio async
+def main(): options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: await driver.get('chrome://version') script = """
+const proxy = new Proxy(document.documentElement, { get(target, prop, receiver)
+{ if(prop === "outerHTML"){ console.log('detected access on "'+prop+'"',
+receiver) return "mocked value:)" } else{return Reflect.get(...arguments)} },
+}); Object.defineProperty(document, "documentElement", { value: proxy }) """
+await driver.execute_script(script) src = await driver.execute_script("return
 document.documentElement.outerHTML", unique_context=True) mocked = await
 driver.execute_script("return document.documentElement.outerHTML",
 unique_context=False) print(src, mocked) asyncio.run(main()) ``` ### Pointer
 Interaction see [@master/dev/show_mousemove.py](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for
 visualization ```python pointer = driver.current_pointer move_kwargs =
 {"total_time": 0.7, "accel": 2, "smooth_soft": 20} await pointer.move_to(100,
 500) await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True) ```
-### Iframes - switch and interact with iframes ```python iframes = await
-driver.find_elements(By.TAG_NAME, "iframe") await asyncio.sleep(0.5)
-iframe_document = await iframes[0].content_document #
-iframe_document.find_elements(...) ``` ### use preferences ```python from
-selenium_driverless import webdriver options = webdriver.ChromeOptions() #
-recommended usage options.update_pref("download.prompt_for_download", False) #
-or options.prefs.update({"download": {"prompt_for_download": False}}) #
-supported options.add_experimental_option("prefs",
-{"download.prompt_for_download": False}) ``` ### Multiple Contexts - different
-cookies for each context - A context can have multiple windows and tabs within
-- different proxy for each context - opens as a window as incognito Example
-Code (Click to expand) ```python from selenium_driverless import webdriver
-import asyncio async def main(): options = webdriver.ChromeOptions() async with
-webdriver.Chrome(options=options) as driver: context_1 = driver.current_context
-await driver.set_auth("username", "password", "localhost:5000") # proxy not
-supported on windows due to https://bugs.chromium.org/p/chromium/issues/
-detail?id=1310057 context_2 = await driver.new_context(proxy_bypass_list=
-["localhost"], proxy_server="http://localhost:5000") await
-context_1.current_target.get("https://examle.com") await context_2.get("https:/
-/examle.com") input("press ENTER to exit:)") asyncio.run(main()) ``` ####
-Custom exception handling You can implement custom exception handling as
-following ```python import selenium_driverless import sys handler = (lambda e:
-print(f'Exception in event-handler:\n{e.__class__.__module__}.
+### Iframes ```python iframes = await driver.find_elements(By.TAG_NAME,
+"iframe") await asyncio.sleep(0.5) iframe_document = await iframes
+[0].content_document # iframe_document.find_elements(...) ``` ### use
+preferences ```python from selenium_driverless import webdriver options =
+webdriver.ChromeOptions() # recommended usage options.update_pref
+("download.prompt_for_download", False) # or options.prefs.update({"download":
+{"prompt_for_download": False}}) # supported options.add_experimental_option
+("prefs", {"download.prompt_for_download": False}) ``` ### Multiple Contexts -
+different cookies for each context - A context can have multiple windows and
+tabs within - different proxy for each context - opens as a window as incognito
+Example Code (Click to expand) ```python from selenium_driverless import
+webdriver import asyncio async def main(): options = webdriver.ChromeOptions()
+async with webdriver.Chrome(options=options) as driver: context_1 =
+driver.current_context await driver.set_auth("username", "password",
+"localhost:5000") # proxy not supported on windows due to https://
+bugs.chromium.org/p/chromium/issues/detail?id=1310057 context_2 = await
+driver.new_context(proxy_bypass_list=["localhost"], proxy_server="http://
+localhost:5000") await context_1.current_target.get("https://examle.com") await
+context_2.get("https://examle.com") input("press ENTER to exit:)") asyncio.run
+(main()) ``` #### Custom exception handling You can implement custom exception
+handling as following ```python import selenium_driverless import sys handler =
+(lambda e: print(f'Exception in event-handler:\n{e.__class__.__module__}.
 {e.__class__.__name__}: {e}', file=sys.stderr)) sys.modules
 ["selenium_driverless"].EXC_HANDLER = handler sys.modules
 ["cdp_socket"].EXC_HANDLER = handler ``` ## Help You found a bug? Feel free to
 open an issue:) You've got other questions or proposials? feel free to join the
 [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord** or
-open a discusion\ Note: **please check the todo's below at first!** ## Todo's
-Click to expand - implementations - [x] `WebElement`s - [ ] improve
-`mid_location` calculation - [ ] add `WebElement.screenshot` - [x] `Input` -
-[x] `Mouse` - [x] `mousemove` - [x] `click` - [ ] `scroll` - [ ] `drag&drop` -
-[x] `write` - [ ] `Touch` - [ ] `touchmove` - [ ] `TouchTap` - [ ] `scoll` -
-[ ] `pinch//zoom` - [ ] `KeyBoard` - [ ] `SendKeys` - [ ] `send files` - [ ]
-[support `options.add_extension()`](https://github.com/kaliiiiiiiiii/Selenium-
-Driverless/issues/37) - [ ] [support prefs](https://github.com/kaliiiiiiiiii/
-Selenium-Driverless/discussions/92#discussioncomment-7462309) - [x] sync - [ ]
-move sync to threaded for allowing event_handlers - [ ] support multithreading
-with sync version - [x] on independent driver instances - [ ] on same driver
-instance - [ ] check [Python 3.12.0](https://www.python.org/downloads/release/
-python-3120/) ## Authors Copyright and Author: \ [Aurin Aegerter](mailto:
+open a discusion\ ## Authors Copyright and Author: \ [Aurin Aegerter](mailto:
 aurinliun@gmx.ch) (aka **Steve**) ## License Shield: [![CC BY-NC-SA 4.0][cc-by-
 nc-sa-shield]][cc-by-nc-sa] Unless specified differently in a single file, this
 work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike
 4.0 International License][cc-by-nc-sa]. [![CC BY-NC-SA 4.0][cc-by-nc-sa-
 image]][cc-by-nc-sa] [cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-
 sa/4.0/ [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/
 88x31.png [cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--
```

### Comparing `selenium_driverless-1.9/build_upload.md` & `selenium_driverless-1.9.1/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/README.md` & `selenium_driverless-1.9.1/dev/README.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/bypass_turnstile.mp4` & `selenium_driverless-1.9.1/dev/assets/bypass_turnstile.mp4`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/events_mouse.png` & `selenium_driverless-1.9.1/dev/assets/events_mouse.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/events_mousepad.png` & `selenium_driverless-1.9.1/dev/assets/events_mousepad.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/heatmap.png` & `selenium_driverless-1.9.1/dev/assets/heatmap.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/mouse_path_gen.png` & `selenium_driverless-1.9.1/dev/assets/mouse_path_gen.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/mousemove_events_gen.png` & `selenium_driverless-1.9.1/dev/assets/mousemove_events_gen.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/mousemove_events_test_sample_based.png` & `selenium_driverless-1.9.1/dev/assets/mousemove_events_test_sample_based.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/mousemove_events_test_samples_based.png` & `selenium_driverless-1.9.1/dev/assets/mousemove_events_test_samples_based.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/assets/real_mouse_path.png` & `selenium_driverless-1.9.1/dev/assets/real_mouse_path.png`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/dev/human_like_path.py` & `selenium_driverless-1.9.1/dev/human_like_path.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/.doctrees/index.doctree` & `selenium_driverless-1.9.1/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_modules/index.html` & `selenium_driverless-1.9.1/docs/_modules/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" data-content_root="../">
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Overview: module code &mdash; Selenium-Driverless 1.8.0.2 documentation</title>
+  <title>Overview: module code &mdash; Selenium-Driverless 1.9.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=80d5e7a1" />
       <link rel="stylesheet" type="text/css" href="../_static/css/theme.css?v=19f00094" />
 
   
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="../_static/documentation_options.js?v=696515ce"></script>
+        <script src="../_static/documentation_options.js?v=fd4b3c67"></script>
         <script src="../_static/doctools.js?v=888ff710"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex/" />
     <link rel="search" title="Search" href="../search/" /> 
 </head>
```

### Comparing `selenium_driverless-1.9/docs/_modules/selenium_driverless/types/options/index.html` & `selenium_driverless-1.9.1/docs/_modules/selenium_driverless/types/options/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" data-content_root="../../../../">
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>selenium_driverless.types.options &mdash; Selenium-Driverless 1.8.0.2 documentation</title>
+  <title>selenium_driverless.types.options &mdash; Selenium-Driverless 1.9.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../../_static/pygments.css?v=80d5e7a1" />
       <link rel="stylesheet" type="text/css" href="../../../../_static/css/theme.css?v=19f00094" />
 
   
   <!--[if lt IE 9]>
     <script src="../../../../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../../../../_static/jquery.js?v=5d32c60e"></script>
         <script src="../../../../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="../../../../_static/documentation_options.js?v=696515ce"></script>
+        <script src="../../../../_static/documentation_options.js?v=fd4b3c67"></script>
         <script src="../../../../_static/doctools.js?v=888ff710"></script>
         <script src="../../../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../../../../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../../../../genindex/" />
     <link rel="search" title="Search" href="../../../../search/" /> 
 </head>
 
@@ -107,14 +107,22 @@
 <span class="kn">from</span> <span class="nn">selenium_driverless.scripts.prefs</span> <span class="kn">import</span> <span class="n">prefs_to_json</span>
 
 
 <span class="c1"># noinspection PyUnreachableCode,PyUnusedLocal</span>
 <div class="viewcode-block" id="Options">
 <a class="viewcode-back" href="../../../../api/ChromeOptions/#selenium_driverless.types.options.Options">[docs]</a>
 <span class="k">class</span> <span class="nc">Options</span><span class="p">(</span><span class="n">metaclass</span><span class="o">=</span><span class="n">ABCMeta</span><span class="p">):</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
+<span class="sd">    the `webdriver.ChromeOptions` class</span>
+
+<span class="sd">    .. warning::</span>
+
+<span class="sd">        options should not be reused</span>
+
+<span class="sd">    &quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_single_proxy</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="kn">from</span> <span class="nn">selenium_driverless.utils.utils</span> <span class="kn">import</span> <span class="n">find_chrome_executable</span><span class="p">,</span> <span class="n">IS_POSIX</span>
         <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="fm">__init__</span><span class="p">()</span>
```

#### html2text {}

```diff
@@ -43,14 +43,22 @@
 from selenium_driverless.scripts.prefs import prefs_to_json
 
 
 # noinspection PyUnreachableCode,PyUnusedLocal
 
 _[_d_o_c_s_]
 class Options(metaclass=ABCMeta):
+    """
+    the `webdriver.ChromeOptions` class
+
+    .. warning::
+
+        options should not be reused
+
+    """
 
     def __init__(self) -> None:
 
         self._single_proxy = None
         from selenium_driverless.utils.utils import find_chrome_executable,
 IS_POSIX
         super().__init__()
```

### Comparing `selenium_driverless-1.9/docs/_modules/selenium_driverless/webdriver/index.html` & `selenium_driverless-1.9.1/docs/_modules/selenium_driverless/webdriver/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" data-content_root="../../../">
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>selenium_driverless.webdriver &mdash; Selenium-Driverless 1.8.0.2 documentation</title>
+  <title>selenium_driverless.webdriver &mdash; Selenium-Driverless 1.9.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css?v=80d5e7a1" />
       <link rel="stylesheet" type="text/css" href="../../../_static/css/theme.css?v=19f00094" />
 
   
   <!--[if lt IE 9]>
     <script src="../../../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../../../_static/jquery.js?v=5d32c60e"></script>
         <script src="../../../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="../../../_static/documentation_options.js?v=696515ce"></script>
+        <script src="../../../_static/documentation_options.js?v=fd4b3c67"></script>
         <script src="../../../_static/doctools.js?v=888ff710"></script>
         <script src="../../../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../../../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../../../genindex/" />
     <link rel="search" title="Search" href="../../../search/" /> 
 </head>
 
@@ -1296,21 +1296,35 @@
 <a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_png">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">get_screenshot_as_png</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bytes</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the screenshot of the current tab as a binary data.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_screenshot_as_png</span><span class="p">()</span></div>
 
 
-<div class="viewcode-block" id="Chrome.get_screenshot_as_base64">
-<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_base64">[docs]</a>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">get_screenshot_as_base64</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-<span class="w">        </span><span class="sd">&quot;&quot;&quot;Gets the screenshot of the current tab as a base64 encoded string</span>
-<span class="sd">        which is useful in embedded images in HTML.</span>
+<div class="viewcode-block" id="Chrome.snapshot">
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.snapshot">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">snapshot</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;gets the current snapshot as mhtml&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">snapshot</span><span class="p">()</span></div>
+
+
+<div class="viewcode-block" id="Chrome.save_snapshot">
+<a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.save_snapshot">[docs]</a>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">save_snapshot</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">filename</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;Saves a snapshot of the current window to a MHTML file.</span>
+
+<span class="sd">        :param filename: The full path you wish to save your snapshot to. This</span>
+<span class="sd">                   should end with a ``.mhtml`` extension.</span>
+
+<span class="sd">        .. code-block:: Python</span>
+
+<span class="sd">            await driver.get_snapshot(&#39;snapshot.mhtml&#39;)</span>
+
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">get_screenshot_as_base64</span><span class="p">()</span></div>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">save_snapshot</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span></div>
 
 
     <span class="c1"># noinspection PyPep8Naming</span>
 <div class="viewcode-block" id="Chrome.set_window_size">
 <a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_window_size">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">set_window_size</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">width</span><span class="p">:</span> <span class="nb">int</span><span class="p">,</span> <span class="n">height</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets the width and height of the window, the current tab is within (unless ``windowHandle`` specified)</span>
@@ -1779,47 +1793,41 @@
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
         <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">get_issue_message</span><span class="p">()</span></div>
 
 
 <div class="viewcode-block" id="Chrome.set_sink_to_use">
 <a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.set_sink_to_use">[docs]</a>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">set_sink_to_use</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">set_sink_to_use</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Sets a specific sink, using its name, as a Cast session receiver</span>
 <span class="sd">        target.</span>
 
-<span class="sd">        :Args:</span>
-<span class="sd">         - sink_name: Name of the sink to use as the target.</span>
+<span class="sd">        :param sink_name: Name of the sink to use as the target.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
-        <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">set_sink_to_use</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">set_sink_to_use</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.start_desktop_mirroring">
 <a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.start_desktop_mirroring">[docs]</a>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">start_desktop_mirroring</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">start_desktop_mirroring</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Starts a desktop mirroring session on a specific receiver target.</span>
 
-<span class="sd">        :Args:</span>
-<span class="sd">         - sink_name: Name of the sink to use as the target.</span>
+<span class="sd">        :param sink_name: Name of the sink to use as the target.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
-        <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">start_desktop_mirroring</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">start_desktop_mirroring</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.start_tab_mirroring">
 <a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.start_tab_mirroring">[docs]</a>
-    <span class="k">async</span> <span class="k">def</span> <span class="nf">start_tab_mirroring</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+    <span class="k">async</span> <span class="k">def</span> <span class="nf">start_tab_mirroring</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Starts a tab mirroring session on a specific receiver target.</span>
 
-<span class="sd">        :Args:</span>
-<span class="sd">         - sink_name: Name of the sink to use as the target.</span>
+<span class="sd">        :param sink_name: Name of the sink to use as the target.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">target</span> <span class="o">=</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_target</span><span class="p">(</span><span class="n">target_id</span><span class="o">=</span><span class="n">target_id</span><span class="p">)</span>
-        <span class="k">return</span> <span class="k">await</span> <span class="n">target</span><span class="o">.</span><span class="n">start_tab_mirroring</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
+        <span class="k">return</span> <span class="k">await</span> <span class="bp">self</span><span class="o">.</span><span class="n">current_target</span><span class="o">.</span><span class="n">start_tab_mirroring</span><span class="p">(</span><span class="n">sink_name</span><span class="o">=</span><span class="n">sink_name</span><span class="p">)</span></div>
 
 
 <div class="viewcode-block" id="Chrome.stop_casting">
 <a class="viewcode-back" href="../../../api/Chrome/#selenium_driverless.webdriver.Chrome.stop_casting">[docs]</a>
     <span class="k">async</span> <span class="k">def</span> <span class="nf">stop_casting</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">sink_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">target_id</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
 <span class="w">        </span><span class="sd">&quot;&quot;&quot;Stops the existing Cast session on a specific receiver target.</span>
```

#### html2text {}

```diff
@@ -1425,19 +1425,34 @@
         """
         return await self.current_target.get_screenshot_as_png()
 
 
 
 
 _[_d_o_c_s_]
-    async def get_screenshot_as_base64(self) -> str:
-        """Gets the screenshot of the current tab as a base64 encoded string
-        which is useful in embedded images in HTML.
+    async def snapshot(self) -> str:
+        """gets the current snapshot as mhtml"""
+        return await self.current_target.snapshot()
+
+
+
+
+_[_d_o_c_s_]
+    async def save_snapshot(self, filename: str):
+        """Saves a snapshot of the current window to a MHTML file.
+
+        :param filename: The full path you wish to save your snapshot to. This
+                   should end with a ``.mhtml`` extension.
+
+        .. code-block:: Python
+
+            await driver.get_snapshot('snapshot.mhtml')
+
         """
-        return await self.current_target.get_screenshot_as_base64()
+        return await self.current_target.save_snapshot(filename)
 
 
 
     # noinspection PyPep8Naming
 
 _[_d_o_c_s_]
     async def set_window_size(self, width: int, height: int) -> None:
@@ -1981,52 +1996,45 @@
         target = await self.get_target(target_id=target_id)
         return await target.get_issue_message()
 
 
 
 
 _[_d_o_c_s_]
-    async def set_sink_to_use(self, sink_name: str, target_id: str = None) -
-> dict:
+    async def set_sink_to_use(self, sink_name: str) -> dict:
         """Sets a specific sink, using its name, as a Cast session receiver
         target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.set_sink_to_use(sink_name=sink_name)
+        return await self.current_target.set_sink_to_use(sink_name=sink_name)
 
 
 
 
 _[_d_o_c_s_]
-    async def start_desktop_mirroring(self, sink_name: str, target_id: str =
-None) -> dict:
+    async def start_desktop_mirroring(self, sink_name: str) -> dict:
         """Starts a desktop mirroring session on a specific receiver target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.start_desktop_mirroring(sink_name=sink_name)
+        return await self.current_target.start_desktop_mirroring
+(sink_name=sink_name)
 
 
 
 
 _[_d_o_c_s_]
-    async def start_tab_mirroring(self, sink_name: str, target_id: str = None)
--> dict:
+    async def start_tab_mirroring(self, sink_name: str) -> dict:
         """Starts a tab mirroring session on a specific receiver target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.start_tab_mirroring(sink_name=sink_name)
+        return await self.current_target.start_tab_mirroring
+(sink_name=sink_name)
 
 
 
 
 _[_d_o_c_s_]
     async def stop_casting(self, sink_name: str, target_id: str = None) -
 > dict:
```

### Comparing `selenium_driverless-1.9/docs/_sources/index.rst.txt` & `selenium_driverless-1.9.1/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/_sphinx_javascript_frameworks_compat.js` & `selenium_driverless-1.9.1/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/basic.css` & `selenium_driverless-1.9.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/badge_only.css` & `selenium_driverless-1.9.1/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.eot` & `selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.svg` & `selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.ttf` & `selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/fontawesome-webfont.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold-italic.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-bold.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal-italic.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/fonts/lato-normal.woff2` & `selenium_driverless-1.9.1/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/css/theme.css` & `selenium_driverless-1.9.1/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/doctools.js` & `selenium_driverless-1.9.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/jquery.js` & `selenium_driverless-1.9.1/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/js/badge_only.js` & `selenium_driverless-1.9.1/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/js/html5shiv-printshiv.min.js` & `selenium_driverless-1.9.1/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/js/html5shiv.min.js` & `selenium_driverless-1.9.1/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/js/theme.js` & `selenium_driverless-1.9.1/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/language_data.js` & `selenium_driverless-1.9.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/pygments.css` & `selenium_driverless-1.9.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/searchtools.js` & `selenium_driverless-1.9.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/_static/sphinx_highlight.js` & `selenium_driverless-1.9.1/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs/genindex/index.html` & `selenium_driverless-1.9.1/docs/genindex/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" data-content_root="../">
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; Selenium-Driverless 1.8.0.2 documentation</title>
+  <title>Index &mdash; Selenium-Driverless 1.9.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=80d5e7a1" />
       <link rel="stylesheet" type="text/css" href="../_static/css/theme.css?v=19f00094" />
 
   
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="../_static/documentation_options.js?v=696515ce"></script>
+        <script src="../_static/documentation_options.js?v=fd4b3c67"></script>
         <script src="../_static/doctools.js?v=888ff710"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="../search/" /> 
 </head>
 
@@ -119,14 +119,16 @@
 <h2 id="A">A</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.accept_insecure_certs">accept_insecure_certs (selenium_driverless.types.options.Options property)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.accessible_name">accessible_name (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
+      <li><a href="../api/Target/#selenium_driverless.types.target.Target.activate">activate() (selenium_driverless.types.target.Target method)</a>
+</li>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.add_argument">add_argument() (selenium_driverless.types.options.Options method)</a>
 </li>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.add_arguments">add_arguments() (selenium_driverless.types.options.Options method)</a>
 </li>
       <li><a href="../api/Target/#selenium_driverless.types.base_target.BaseTarget.add_cdp_listener">add_cdp_listener() (selenium_driverless.types.base_target.BaseTarget method)</a>
 
       <ul>
@@ -141,18 +143,18 @@
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.add_cookie">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.add_cookie">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
-      <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.add_experimental_option">add_experimental_option() (selenium_driverless.types.options.Options method)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.add_experimental_option">add_experimental_option() (selenium_driverless.types.options.Options method)</a>
+</li>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.add_extension">add_extension() (selenium_driverless.types.options.Options method)</a>
 </li>
       <li><a href="../api/Chrome/#selenium_driverless.scripts.switch_to.SwitchTo.alert">alert (selenium_driverless.scripts.switch_to.SwitchTo property)</a>
 </li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.Modifiers.ALT">ALT (selenium_driverless.input.pointer.Modifiers attribute)</a>
 </li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.RequestPattern.AnyRequest">AnyRequest (selenium_driverless.scripts.network_interceptor.RequestPattern attribute)</a>
@@ -189,22 +191,24 @@
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.back">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.back">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
+      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.backend_node_id">backend_node_id (selenium_driverless.types.webelement.WebElement property)</a>
+</li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.base_context">base_context (selenium_driverless.webdriver.Chrome property)</a>
 </li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.base_target">base_target (selenium_driverless.webdriver.Chrome property)</a>
 </li>
-      <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer">BasePointer (class in selenium_driverless.input.pointer)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer">BasePointer (class in selenium_driverless.input.pointer)</a>
+</li>
       <li><a href="../api/Target/#selenium_driverless.types.base_target.BaseTarget">BaseTarget (class in selenium_driverless.types.base_target)</a>
 </li>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.binary_location">binary_location (selenium_driverless.types.options.Options property)</a>
 </li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.InterceptedRequest.body">body (selenium_driverless.scripts.network_interceptor.InterceptedRequest property)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.box_model">box_model (selenium_driverless.types.webelement.WebElement property)</a>
@@ -227,14 +231,16 @@
 </li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.InterceptedAuth.cancel">cancel() (selenium_driverless.scripts.network_interceptor.InterceptedAuth method)</a>
 </li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome">Chrome (class in selenium_driverless.webdriver)</a>
 </li>
       <li><a href="../api/By/#selenium_driverless.types.by.By.CLASS_NAME">CLASS_NAME (selenium_driverless.types.by.By attribute)</a>
 </li>
+      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.class_name">class_name (selenium_driverless.types.webelement.WebElement property)</a>
+</li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.clear">clear() (selenium_driverless.types.webelement.WebElement method)</a>
 </li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.clear_auth">clear_auth() (selenium_driverless.webdriver.Chrome method)</a>
 </li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.clear_proxy">clear_proxy() (selenium_driverless.webdriver.Chrome method)</a>
 </li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer.click">click() (selenium_driverless.input.pointer.BasePointer method)</a>
@@ -255,18 +261,20 @@
       </ul></li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.Modifiers.COMMAND">COMMAND (selenium_driverless.input.pointer.Modifiers attribute)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.content_document">content_document (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
       <li><a href="../api/Context/#selenium_driverless.types.context.Context">Context (class in selenium_driverless.types.context)</a>
 </li>
-      <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.contexts">contexts (selenium_driverless.webdriver.Chrome property)</a>
+      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.context_id">context_id (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.contexts">contexts (selenium_driverless.webdriver.Chrome property)</a>
+</li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.InterceptedAuth.continue_auth">continue_auth() (selenium_driverless.scripts.network_interceptor.InterceptedAuth method)</a>
 </li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.InterceptedRequest.continue_request">continue_request() (selenium_driverless.scripts.network_interceptor.InterceptedRequest method)</a>
 </li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.InterceptedRequest.continue_response">continue_response() (selenium_driverless.scripts.network_interceptor.InterceptedRequest method)</a>
 </li>
       <li><a href="../api/By/#selenium_driverless.types.by.By.CSS">CSS (selenium_driverless.types.by.By attribute)</a>
@@ -341,14 +349,16 @@
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer.dispatch">dispatch() (selenium_driverless.input.pointer.BasePointer method)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.document_url">document_url (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
+      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.dom_attributes">dom_attributes (selenium_driverless.types.webelement.WebElement property)</a>
+</li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer.double_click">double_click() (selenium_driverless.input.pointer.BasePointer method)</a>
 </li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer.down">down() (selenium_driverless.input.pointer.BasePointer method)</a>
 
       <ul>
         <li><a href="../api/Input/#selenium_driverless.input.pointer.Pointer.down">(selenium_driverless.input.pointer.Pointer method)</a>
 </li>
@@ -459,17 +469,19 @@
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.find_elements">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.find_elements">(selenium_driverless.types.webelement.WebElement method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.find_elements">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
-      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.focus">focus() (selenium_driverless.types.webelement.WebElement method)</a>
+      <li><a href="../api/Target/#selenium_driverless.types.target.Target.focus">focus() (selenium_driverless.types.target.Target method)</a>
 
       <ul>
+        <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.focus">(selenium_driverless.types.webelement.WebElement method)</a>
+</li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.focus">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.Buttons.FORWARD">FORWARD (selenium_driverless.input.pointer.Buttons attribute)</a>
 
@@ -569,22 +581,14 @@
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_network_conditions">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.get_property">get_property() (selenium_driverless.types.webelement.WebElement method)</a>
 </li>
-      <li><a href="../api/Context/#selenium_driverless.types.context.Context.get_screenshot_as_base64">get_screenshot_as_base64() (selenium_driverless.types.context.Context method)</a>
-
-      <ul>
-        <li><a href="../api/Target/#selenium_driverless.types.target.Target.get_screenshot_as_base64">(selenium_driverless.types.target.Target method)</a>
-</li>
-        <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_base64">(selenium_driverless.webdriver.Chrome method)</a>
-</li>
-      </ul></li>
       <li><a href="../api/Context/#selenium_driverless.types.context.Context.get_screenshot_as_file">get_screenshot_as_file() (selenium_driverless.types.context.Context method)</a>
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.get_screenshot_as_file">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_screenshot_as_file">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
@@ -603,20 +607,28 @@
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.get_sinks">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_sinks">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_target">get_target() (selenium_driverless.webdriver.Chrome method)</a>
 </li>
-      <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_target_for_iframe">get_target_for_iframe() (selenium_driverless.webdriver.Chrome method)</a>
+      <li><a href="../api/Target/#selenium_driverless.types.target.Target.get_target_for_iframe">get_target_for_iframe() (selenium_driverless.types.target.Target method)</a>
+
+      <ul>
+        <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_target_for_iframe">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
+      </ul></li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_targets">get_targets() (selenium_driverless.webdriver.Chrome method)</a>
 </li>
-      <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_targets_for_iframes">get_targets_for_iframes() (selenium_driverless.webdriver.Chrome method)</a>
+      <li><a href="../api/Target/#selenium_driverless.types.target.Target.get_targets_for_iframes">get_targets_for_iframes() (selenium_driverless.types.target.Target method)</a>
+
+      <ul>
+        <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_targets_for_iframes">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
+      </ul></li>
       <li><a href="../api/Context/#selenium_driverless.types.context.Context.get_window_position">get_window_position() (selenium_driverless.types.context.Context method)</a>
 
       <ul>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.get_window_position">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
       <li><a href="../api/Context/#selenium_driverless.types.context.Context.get_window_rect">get_window_rect() (selenium_driverless.types.context.Context method)</a>
@@ -777,14 +789,16 @@
         <li><a href="../api/Context/#selenium_driverless.types.context.Context.new_window">(selenium_driverless.types.context.Context method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.new_window">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.node_id">node_id (selenium_driverless.types.webelement.WebElement property)</a>
+</li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.Buttons.NONE">NONE (selenium_driverless.input.pointer.Buttons attribute)</a>
 
       <ul>
         <li><a href="../api/Input/#selenium_driverless.input.pointer.Modifiers.NONE">(selenium_driverless.input.pointer.Modifiers attribute)</a>
 </li>
         <li><a href="../api/Input/#selenium_driverless.input.pointer.MouseButton.NONE">(selenium_driverless.input.pointer.MouseButton attribute)</a>
 </li>
@@ -831,16 +845,14 @@
         <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.InterceptedRequest.params">(selenium_driverless.scripts.network_interceptor.InterceptedRequest property)</a>
 </li>
         <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.Request.params">(selenium_driverless.scripts.network_interceptor.Request property)</a>
 </li>
       </ul></li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.parent">parent (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
-      <li><a href="../api/Chrome/#selenium_driverless.scripts.switch_to.SwitchTo.parent_frame">parent_frame() (selenium_driverless.scripts.switch_to.SwitchTo method)</a>
-</li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.NetworkInterceptor.patterns">patterns (selenium_driverless.scripts.network_interceptor.NetworkInterceptor property)</a>
 </li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.PointerType.PEN">PEN (selenium_driverless.input.pointer.PointerType attribute)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.Pointer">Pointer (class in selenium_driverless.input.pointer)</a>
@@ -975,14 +987,22 @@
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.save_screenshot">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.save_screenshot">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
+      <li><a href="../api/Context/#selenium_driverless.types.context.Context.save_snapshot">save_snapshot() (selenium_driverless.types.context.Context method)</a>
+
+      <ul>
+        <li><a href="../api/Target/#selenium_driverless.types.target.Target.save_snapshot">(selenium_driverless.types.target.Target method)</a>
+</li>
+        <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.save_snapshot">(selenium_driverless.webdriver.Chrome method)</a>
+</li>
+      </ul></li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.AuthChallenge.scheme">scheme (selenium_driverless.scripts.network_interceptor.AuthChallenge property)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.screenshot">screenshot() (selenium_driverless.types.webelement.WebElement method)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.screenshot_as_base64">screenshot_as_base64 (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.screenshot_as_png">screenshot_as_png (selenium_driverless.types.webelement.WebElement property)</a>
@@ -1005,14 +1025,16 @@
         <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.send_keys">(selenium_driverless.types.webelement.WebElement method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.send_keys">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.set_auth">set_auth() (selenium_driverless.webdriver.Chrome method)</a>
 </li>
+      <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.set_dom_attribute">set_dom_attribute() (selenium_driverless.types.webelement.WebElement method)</a>
+</li>
       <li><a href="../api/Context/#selenium_driverless.types.context.Context.set_download_behaviour">set_download_behaviour() (selenium_driverless.types.context.Context method)</a>
 
       <ul>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.set_download_behaviour">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.set_file">set_file() (selenium_driverless.types.webelement.WebElement method)</a>
@@ -1079,14 +1101,22 @@
 </li>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.single_proxy">single_proxy (selenium_driverless.types.options.Options property)</a>
 </li>
       <li><a href="../api/WebELement/#selenium_driverless.types.webelement.WebElement.size">size (selenium_driverless.types.webelement.WebElement property)</a>
 </li>
       <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.sleep">sleep() (selenium_driverless.webdriver.Chrome static method)</a>
 </li>
+      <li><a href="../api/Context/#selenium_driverless.types.context.Context.snapshot">snapshot() (selenium_driverless.types.context.Context method)</a>
+
+      <ul>
+        <li><a href="../api/Target/#selenium_driverless.types.target.Target.snapshot">(selenium_driverless.types.target.Target method)</a>
+</li>
+        <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.snapshot">(selenium_driverless.webdriver.Chrome method)</a>
+</li>
+      </ul></li>
       <li><a href="../api/Target/#selenium_driverless.types.base_target.BaseTarget.socket">socket (selenium_driverless.types.base_target.BaseTarget property)</a>
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.socket">(selenium_driverless.types.target.Target property)</a>
 </li>
       </ul></li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.AuthChallenge.source">source (selenium_driverless.scripts.network_interceptor.AuthChallenge property)</a>
@@ -1101,16 +1131,14 @@
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.start_desktop_mirroring">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.start_desktop_mirroring">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
       </ul></li>
-      <li><a href="../api/Context/#selenium_driverless.types.context.Context.start_session">start_session() (selenium_driverless.types.context.Context method)</a>
-</li>
       <li><a href="../api/Context/#selenium_driverless.types.context.Context.start_tab_mirroring">start_tab_mirroring() (selenium_driverless.types.context.Context method)</a>
 
       <ul>
         <li><a href="../api/Target/#selenium_driverless.types.target.Target.start_tab_mirroring">(selenium_driverless.types.target.Target method)</a>
 </li>
         <li><a href="../api/Chrome/#selenium_driverless.webdriver.Chrome.start_tab_mirroring">(selenium_driverless.webdriver.Chrome method)</a>
 </li>
@@ -1187,24 +1215,26 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="U">U</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="../api/Target/#selenium_driverless.types.target.Target.unfocus">unfocus() (selenium_driverless.types.target.Target method)</a>
+</li>
       <li><a href="../api/Input/#selenium_driverless.input.pointer.BasePointer.up">up() (selenium_driverless.input.pointer.BasePointer method)</a>
 
       <ul>
         <li><a href="../api/Input/#selenium_driverless.input.pointer.Pointer.up">(selenium_driverless.input.pointer.Pointer method)</a>
 </li>
       </ul></li>
-      <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.update_pref">update_pref() (selenium_driverless.types.options.Options method)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.update_pref">update_pref() (selenium_driverless.types.options.Options method)</a>
+</li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.Request.url">url (selenium_driverless.scripts.network_interceptor.Request property)</a>
 </li>
       <li><a href="../api/RequestInterception/#selenium_driverless.scripts.network_interceptor.Request.url_fragment">url_fragment (selenium_driverless.scripts.network_interceptor.Request property)</a>
 </li>
       <li><a href="../api/ChromeOptions/#selenium_driverless.types.options.Options.user_data_dir">user_data_dir (selenium_driverless.types.options.Options property)</a>
 </li>
   </ul></td>
```

#### html2text {}

```diff
@@ -15,20 +15,22 @@
 ___ | _AA | _BB | _CC | _DD | _EE | _FF | _GG | _HH | _II | _LL | _MM | _NN | _OO | _PP | _QQ | _RR | _SS | _TT | _UU |
 _VV | _WW | _XX
 ********** __ **********
     * _____a_i_t_e_r_____(_)_                                                             * _____i_n_i_t_____(_)_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r
       _m_e_t_h_o_d_)                                                                   _m_e_t_h_o_d_)
 ********** AA **********
-    * _a_c_c_e_p_t___i_n_s_e_c_u_r_e___c_e_r_t_s_                                 * _a_d_d___e_x_t_e_n_s_i_o_n_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s              _m_e_t_h_o_d_)
-      _p_r_o_p_e_r_t_y_)                                             * _a_l_e_r_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o_ _p_r_o_p_e_r_t_y_)
-    * _a_c_c_e_s_s_i_b_l_e___n_a_m_e_                                       * _A_L_T_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t      * _A_n_y_R_e_q_u_e_s_t_ 
-      _p_r_o_p_e_r_t_y_)                                               _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_P_a_t_t_e_r_n
+    * _a_c_c_e_p_t___i_n_s_e_c_u_r_e___c_e_r_t_s_                                 * _a_d_d___e_x_p_e_r_i_m_e_n_t_a_l___o_p_t_i_o_n_(_)_ 
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s              _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _m_e_t_h_o_d_)
+      _p_r_o_p_e_r_t_y_)                                             * _a_d_d___e_x_t_e_n_s_i_o_n_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
+    * _a_c_c_e_s_s_i_b_l_e___n_a_m_e_                                         _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t      * _a_l_e_r_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o_ _p_r_o_p_e_r_t_y_)
+      _p_r_o_p_e_r_t_y_)                                             * _A_L_T_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)
+    * _a_c_t_i_v_a_t_e_(_)_                                            * _A_n_y_R_e_q_u_e_s_t_ 
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)        _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_P_a_t_t_e_r_n
     * _a_d_d___a_r_g_u_m_e_n_t_(_)_                                          _a_t_t_r_i_b_u_t_e_)
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s            * _A_n_y_R_e_s_p_o_n_s_e_ 
       _m_e_t_h_o_d_)                                                 _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_P_a_t_t_e_r_n
     * _a_d_d___a_r_g_u_m_e_n_t_s_(_)_                                         _a_t_t_r_i_b_u_t_e_)
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s            * _a_r_g_u_m_e_n_t_s_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _p_r_o_p_e_r_t_y_)
       _m_e_t_h_o_d_)                                               * _a_r_i_a___r_o_l_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
     * _a_d_d___c_d_p___l_i_s_t_e_n_e_r_(_)_                                      _p_r_o_p_e_r_t_y_)
@@ -43,87 +45,86 @@
     * _a_d_d___c_o_o_k_i_e_(_)_                                          * _a_u_t_o___c_l_e_a_n___d_i_r_s_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t              _p_r_o_p_e_r_t_y_)
       _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
             _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
             _m_e_t_h_o_d_)
-    * _a_d_d___e_x_p_e_r_i_m_e_n_t_a_l___o_p_t_i_o_n_(_)_ 
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
-      _m_e_t_h_o_d_)
 ********** BB **********
-    * _B_A_C_K_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_u_t_t_o_n_s          * _B_a_s_e_T_a_r_g_e_t_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_)
-      _a_t_t_r_i_b_u_t_e_)                                               * _b_i_n_a_r_y___l_o_c_a_t_i_o_n_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_u_s_e_B_u_t_t_o_n       _p_r_o_p_e_r_t_y_)
-            _a_t_t_r_i_b_u_t_e_)                                         * _b_o_d_y_ 
-    * _b_a_c_k_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t          _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
-      _m_e_t_h_o_d_)                                                    _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t           * _b_o_x___m_o_d_e_l_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
-            _m_e_t_h_o_d_)                                              _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)      * _b_r_o_w_s_e_r___c_o_n_t_e_x_t___i_d_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o
-    * _b_a_s_e___c_o_n_t_e_x_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e         _p_r_o_p_e_r_t_y_)
+    * _B_A_C_K_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_u_t_t_o_n_s          * _B_a_s_e_P_o_i_n_t_e_r_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_)
+      _a_t_t_r_i_b_u_t_e_)                                               * _B_a_s_e_T_a_r_g_e_t_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_u_s_e_B_u_t_t_o_n     * _b_i_n_a_r_y___l_o_c_a_t_i_o_n_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
+            _a_t_t_r_i_b_u_t_e_)                                           _p_r_o_p_e_r_t_y_)
+    * _b_a_c_k_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t        * _b_o_d_y_ 
+      _m_e_t_h_o_d_)                                                    _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t             _p_r_o_p_e_r_t_y_)
+            _m_e_t_h_o_d_)                                            * _b_o_x___m_o_d_e_l_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)        _p_r_o_p_e_r_t_y_)
+    * _b_a_c_k_e_n_d___n_o_d_e___i_d_                                          * _b_r_o_w_s_e_r___c_o_n_t_e_x_t___i_d_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t           _p_r_o_p_e_r_t_y_)
       _p_r_o_p_e_r_t_y_)                                                * _B_u_t_t_o_n_s_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_)
-    * _b_a_s_e___t_a_r_g_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e        * _B_y_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_)
+    * _b_a_s_e___c_o_n_t_e_x_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e       * _B_y_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_)
       _p_r_o_p_e_r_t_y_)                                                * _b_y_p_a_s_s___b_r_o_w_s_e_r_(_)_ 
-    * _B_a_s_e_P_o_i_n_t_e_r_ _(_c_l_a_s_s_ _i_n                                      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
-      _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_)                         _m_e_t_h_o_d_)
+    * _b_a_s_e___t_a_r_g_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e          _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
+      _p_r_o_p_e_r_t_y_)                                                  _m_e_t_h_o_d_)
 ********** CC **********
-    * _c_a_n___a_c_c_e_s_s___o_p_e_n_e_r_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o       * _c_o_n_t_i_n_u_e___a_u_t_h_(_)_ 
-      _p_r_o_p_e_r_t_y_)                                                              _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_A_u_t_h
-    * _c_a_n_c_e_l_(_)_                                                               _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_A_u_t_h     * _c_o_n_t_i_n_u_e___r_e_q_u_e_s_t_(_)_ 
-      _m_e_t_h_o_d_)                                                                _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
-    * _C_h_r_o_m_e_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_)                        _m_e_t_h_o_d_)
-    * _C_L_A_S_S___N_A_M_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)               * _c_o_n_t_i_n_u_e___r_e_s_p_o_n_s_e_(_)_ 
-    * _c_l_e_a_r_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
-    * _c_l_e_a_r___a_u_t_h_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)             _m_e_t_h_o_d_)
-    * _c_l_e_a_r___p_r_o_x_y_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)          * _C_S_S_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)
-    * _c_l_i_c_k_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r_ _m_e_t_h_o_d_)       * _C_S_S___S_E_L_E_C_T_O_R_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r_ _m_e_t_h_o_d_)             * _C_T_R_L_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)       * _c_u_r_r_e_n_t___c_o_n_t_e_x_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
-    * _c_l_o_s_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)           * _c_u_r_r_e_n_t___p_o_i_n_t_e_r_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                 _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                        o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
-    * _C_O_M_M_A_N_D_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)      * _c_u_r_r_e_n_t___t_a_r_g_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
-    * _c_o_n_t_e_n_t___d_o_c_u_m_e_n_t_                                                     * _c_u_r_r_e_n_t___t_a_r_g_e_t___i_n_f_o_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)           * _c_u_r_r_e_n_t___u_r_l_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _p_r_o_p_e_r_t_y_)
-    * _C_o_n_t_e_x_t_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_)                       o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _p_r_o_p_e_r_t_y_)
-    * _c_o_n_t_e_x_t_s_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)                   o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
-                                                                           * _c_u_r_r_e_n_t___w_i_n_d_o_w___h_a_n_d_l_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-                                                                             _p_r_o_p_e_r_t_y_)
+    * _c_a_n___a_c_c_e_s_s___o_p_e_n_e_r_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o       * _c_o_n_t_e_x_t_s_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+      _p_r_o_p_e_r_t_y_)                                                            * _c_o_n_t_i_n_u_e___a_u_t_h_(_)_ 
+    * _c_a_n_c_e_l_(_)_                                                               _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_A_u_t_h
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_A_u_t_h       _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                                              * _c_o_n_t_i_n_u_e___r_e_q_u_e_s_t_(_)_ 
+    * _C_h_r_o_m_e_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_)                        _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
+    * _C_L_A_S_S___N_A_M_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)                 _m_e_t_h_o_d_)
+    * _c_l_a_s_s___n_a_m_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t          * _c_o_n_t_i_n_u_e___r_e_s_p_o_n_s_e_(_)_ 
+      _p_r_o_p_e_r_t_y_)                                                              _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
+    * _c_l_e_a_r_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)       _m_e_t_h_o_d_)
+    * _c_l_e_a_r___a_u_t_h_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)           * _C_S_S_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)
+    * _c_l_e_a_r___p_r_o_x_y_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)          * _C_S_S___S_E_L_E_C_T_O_R_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)
+    * _c_l_i_c_k_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r_ _m_e_t_h_o_d_)       * _C_T_R_L_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r_ _m_e_t_h_o_d_)             * _c_u_r_r_e_n_t___c_o_n_t_e_x_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)       * _c_u_r_r_e_n_t___p_o_i_n_t_e_r_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+    * _c_l_o_s_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)             _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                     o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                  * _c_u_r_r_e_n_t___t_a_r_g_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+    * _C_O_M_M_A_N_D_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)      * _c_u_r_r_e_n_t___t_a_r_g_e_t___i_n_f_o_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+    * _c_o_n_t_e_n_t___d_o_c_u_m_e_n_t_                                                     * _c_u_r_r_e_n_t___u_r_l_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _p_r_o_p_e_r_t_y_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)                 o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _p_r_o_p_e_r_t_y_)
+    * _C_o_n_t_e_x_t_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_)                       o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+    * _c_o_n_t_e_x_t___i_d_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t          * _c_u_r_r_e_n_t___w_i_n_d_o_w___h_a_n_d_l_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+      _p_r_o_p_e_r_t_y_)                                                              _p_r_o_p_e_r_t_y_)
                                                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
                                                                            * _c_u_r_r_e_n_t___w_i_n_d_o_w___i_d_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
 ********** DD **********
     * _d_e_b_u_g_g_e_r___a_d_d_r_e_s_s_                                    * _d_i_s_p_a_t_c_h_(_)_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s            _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r
       _p_r_o_p_e_r_t_y_)                                             _m_e_t_h_o_d_)
     * _D_E_F_A_U_L_T_                                             * _d_o_c_u_m_e_n_t___u_r_l_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_u_t_t_o_n_s            _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
       _a_t_t_r_i_b_u_t_e_)                                            _p_r_o_p_e_r_t_y_)
-    * _d_e_f_a_u_l_t___c_o_n_t_e_n_t_(_)_                                   * _d_o_u_b_l_e___c_l_i_c_k_(_)_ 
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r
-      _m_e_t_h_o_d_)                                               _m_e_t_h_o_d_)
-    * _d_e_l_e_t_e___a_l_l___c_o_o_k_i_e_s_(_)_                                * _d_o_w_n_(_)_ 
+    * _d_e_f_a_u_l_t___c_o_n_t_e_n_t_(_)_                                   * _d_o_m___a_t_t_r_i_b_u_t_e_s_ 
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
+      _m_e_t_h_o_d_)                                               _p_r_o_p_e_r_t_y_)
+    * _d_e_l_e_t_e___a_l_l___c_o_o_k_i_e_s_(_)_                                * _d_o_u_b_l_e___c_l_i_c_k_(_)_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t            _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r
       _m_e_t_h_o_d_)                                               _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t            o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r
-            _m_e_t_h_o_d_)                                               _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e         * _d_o_w_n_l_o_a_d_s___d_i_r_ 
-            _m_e_t_h_o_d_)                                         _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-    * _d_e_l_e_t_e___c_o_o_k_i_e_(_)_                                       _p_r_o_p_e_r_t_y_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t                o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
-      _m_e_t_h_o_d_)                                                     _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t            o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
-            _m_e_t_h_o_d_)                                               _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e         * _d_o_w_n_l_o_a_d_s___d_i_r___f_o_r___c_o_n_t_e_x_t_(_)_ 
-            _m_e_t_h_o_d_)                                         _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_._B_a_s_e_T_a_r_g_e_t
-    * _d_e_l_e_t_e___n_e_t_w_o_r_k___c_o_n_d_i_t_i_o_n_s_(_)_                           _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-      _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t      * _d_o_w_n_(_)_ 
+            _m_e_t_h_o_d_)                                         _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e           _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                                             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r
+    * _d_e_l_e_t_e___c_o_o_k_i_e_(_)_                                             _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t          * _d_o_w_n_l_o_a_d_s___d_i_r_ 
+      _m_e_t_h_o_d_)                                               _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t        _p_r_o_p_e_r_t_y_)
+            _m_e_t_h_o_d_)                                             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e                 _p_r_o_p_e_r_t_y_)
+            _m_e_t_h_o_d_)                                             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
+    * _d_e_l_e_t_e___n_e_t_w_o_r_k___c_o_n_d_i_t_i_o_n_s_(_)_                                 _p_r_o_p_e_r_t_y_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t          * _d_o_w_n_l_o_a_d_s___d_i_r___f_o_r___c_o_n_t_e_x_t_(_)_ 
+      _m_e_t_h_o_d_)                                               _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_._B_a_s_e_T_a_r_g_e_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t        _m_e_t_h_o_d_)
             _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
             _m_e_t_h_o_d_)
 ********** EE **********
     * _e_n_a_b_l_e___m_o_b_i_l_e_(_)_                                            * _e_x_e_c_u_t_e___c_d_p___c_m_d_(_)_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _m_e_t_h_o_d_)           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_._B_a_s_e_T_a_r_g_e_t
     * _e_n_s_u_r_e___e_x_t_e_n_s_i_o_n_s___i_n_c_o_g_n_i_t_o___a_l_l_o_w_e_d_(_)_                        _m_e_t_h_o_d_)
@@ -154,71 +155,72 @@
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                    _p_r_o_p_e_r_t_y_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)                o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                             _p_r_o_p_e_r_t_y_)
     * _f_i_n_d___e_l_e_m_e_n_t_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)      * _f_r_a_m_e___t_r_e_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                  * _f_u_l_f_i_l_l_(_)_ 
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)            _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                       _m_e_t_h_o_d_)
-    * _f_o_c_u_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)        * _f_u_l_l_s_c_r_e_e_n___w_i_n_d_o_w_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+    * _f_o_c_u_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                * _f_u_l_l_s_c_r_e_e_n___w_i_n_d_o_w_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)                o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
 ********** GG **********
     * _g_e_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t      * _g_e_t___p_r_o_p_e_r_t_y_(_)_ 
       _m_e_t_h_o_d_)                                                 _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t          _m_e_t_h_o_d_)
-            _m_e_t_h_o_d_)                                         * _g_e_t___s_c_r_e_e_n_s_h_o_t___a_s___b_a_s_e_6_4_(_)_ 
+            _m_e_t_h_o_d_)                                         * _g_e_t___s_c_r_e_e_n_s_h_o_t___a_s___f_i_l_e_(_)_ 
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e             _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
             _m_e_t_h_o_d_)                                           _m_e_t_h_o_d_)
     * _g_e_t___a_l_e_r_t_(_)_                                                 o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o               _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)                                                     o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
     * _g_e_t___a_t_t_r_i_b_u_t_e_(_)_                                               _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t      * _g_e_t___s_c_r_e_e_n_s_h_o_t___a_s___f_i_l_e_(_)_ 
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t      * _g_e_t___s_c_r_e_e_n_s_h_o_t___a_s___p_n_g_(_)_ 
       _m_e_t_h_o_d_)                                                 _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
     * _g_e_t___c_d_p___e_v_e_n_t___i_t_e_r_(_)_                                    _m_e_t_h_o_d_)
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_._B_a_s_e_T_a_r_g_e_t           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
       _m_e_t_h_o_d_)                                                       _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t            o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
             _m_e_t_h_o_d_)                                                 _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t        * _g_e_t___s_c_r_e_e_n_s_h_o_t___a_s___p_n_g_(_)_ 
-            _m_e_t_h_o_d_)                                           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e             _m_e_t_h_o_d_)
-            _m_e_t_h_o_d_)                                               o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
-    * _g_e_t___c_o_o_k_i_e_(_)_                                                  _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
-      _m_e_t_h_o_d_)                                                       _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t        * _g_e_t___s_i_n_k_s_(_)_ 
             _m_e_t_h_o_d_)                                           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e             _m_e_t_h_o_d_)
             _m_e_t_h_o_d_)                                               o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
-    * _g_e_t___c_o_o_k_i_e_s_(_)_                                                 _m_e_t_h_o_d_)
+    * _g_e_t___c_o_o_k_i_e_(_)_                                                  _m_e_t_h_o_d_)
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
       _m_e_t_h_o_d_)                                                       _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t        * _g_e_t___t_a_r_g_e_t_(_)_ 
             _m_e_t_h_o_d_)                                           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e           * _g_e_t___t_a_r_g_e_t___f_o_r___i_f_r_a_m_e_(_)_ 
-            _m_e_t_h_o_d_)                                           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-    * _g_e_t___d_o_m___a_t_t_r_i_b_u_t_e_(_)_                                   * _g_e_t___t_a_r_g_e_t_s_(_)_ 
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t        _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                               * _g_e_t___t_a_r_g_e_t_s___f_o_r___i_f_r_a_m_e_s_(_)_ 
-    * _g_e_t___h_i_s_t_o_r_y_(_)_                                           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)      * _g_e_t___w_i_n_d_o_w___p_o_s_i_t_i_o_n_(_)_ 
-    * _g_e_t___i_s_s_u_e___m_e_s_s_a_g_e_(_)_                                     _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t              _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                                     o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t                _m_e_t_h_o_d_)
-            _m_e_t_h_o_d_)                                         * _g_e_t___w_i_n_d_o_w___r_e_c_t_(_)_ 
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e             _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-            _m_e_t_h_o_d_)                                           _m_e_t_h_o_d_)
-    * _g_e_t___l_i_s_t_e_n_e_r_s_(_)_                                             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t              _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                               * _g_e_t___w_i_n_d_o_w___s_i_z_e_(_)_ 
-    * _g_e_t___n_e_t_w_o_r_k___c_o_n_d_i_t_i_o_n_s_(_)_                                _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t              _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                                           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
+    * _g_e_t___c_o_o_k_i_e_s_(_)_                                               o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t                    _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                               * _g_e_t___t_a_r_g_e_t_s_(_)_ 
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t          _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                                         * _g_e_t___t_a_r_g_e_t_s___f_o_r___i_f_r_a_m_e_s_(_)_ 
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e             _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                                               o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
+    * _g_e_t___d_o_m___a_t_t_r_i_b_u_t_e_(_)_                                           _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t      * _g_e_t___w_i_n_d_o_w___p_o_s_i_t_i_o_n_(_)_ 
+      _m_e_t_h_o_d_)                                                 _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+    * _g_e_t___h_i_s_t_o_r_y_(_)_                                           _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)            o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
+    * _g_e_t___i_s_s_u_e___m_e_s_s_a_g_e_(_)_                                           _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t            * _g_e_t___w_i_n_d_o_w___r_e_c_t_(_)_ 
+      _m_e_t_h_o_d_)                                                 _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t          _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                                               o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e                   _m_e_t_h_o_d_)
+            _m_e_t_h_o_d_)                                         * _g_e_t___w_i_n_d_o_w___s_i_z_e_(_)_ 
+    * _g_e_t___l_i_s_t_e_n_e_r_s_(_)_                                         _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t        _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)                                                     o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t                _m_e_t_h_o_d_)
+    * _g_e_t___n_e_t_w_o_r_k___c_o_n_d_i_t_i_o_n_s_(_)_                                      _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+      _m_e_t_h_o_d_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t
             _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
             _m_e_t_h_o_d_)
 ********** HH **********
     * _h_a_s___p_o_s_t___d_a_t_a_                                                * _h_e_a_d_l_e_s_s_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
       _p_r_o_p_e_r_t_y_)                                                      _p_r_o_p_e_r_t_y_)
@@ -264,25 +266,25 @@
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_u_s_e_B_u_t_t_o_n           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r_ _m_e_t_h_o_d_)
             _a_t_t_r_i_b_u_t_e_)                                             * _m_o_v_e___t_o_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r
     * _m_i_n_i_m_i_z_e___w_i_n_d_o_w_(_)_                                              _m_e_t_h_o_d_)
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)                 o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)          * _m_v_3___e_x_t_e_n_s_i_o_n_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
                                                                      _p_r_o_p_e_r_t_y_)
 ********** NN **********
-    * _N_A_M_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)                        * _N_O_N_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_u_t_t_o_n_s
-    * _n_e_t_w_o_r_k___i_d_                                                                _a_t_t_r_i_b_u_t_e_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s
-      _p_r_o_p_e_r_t_y_)                                                                       _a_t_t_r_i_b_u_t_e_)
-    * _N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r_ _(_c_l_a_s_s_ _i_n                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_u_s_e_B_u_t_t_o_n
-      _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_)                                _a_t_t_r_i_b_u_t_e_)
-    * _n_e_w_(_)_                                                                   * _n_o_r_m_a_l_i_z_e___w_i_n_d_o_w_(_)_ 
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_P_a_t_t_e_r_n           _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-      _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-    * _n_e_w___c_o_n_t_e_x_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-    * _n_e_w___w_i_n_d_o_w_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o
+    * _N_A_M_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)                        * _n_o_d_e___i_d_ 
+    * _n_e_t_w_o_r_k___i_d_                                                                _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t       _p_r_o_p_e_r_t_y_)
+      _p_r_o_p_e_r_t_y_)                                                               * _N_O_N_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_u_t_t_o_n_s
+    * _N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r_ _(_c_l_a_s_s_ _i_n                                              _a_t_t_r_i_b_u_t_e_)
+      _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_)                              o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s
+    * _n_e_w_(_)_                                                                           _a_t_t_r_i_b_u_t_e_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_P_a_t_t_e_r_n               o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_u_s_e_B_u_t_t_o_n
+      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                                                  _a_t_t_r_i_b_u_t_e_)
+    * _n_e_w___c_o_n_t_e_x_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)             * _n_o_r_m_a_l_i_z_e___w_i_n_d_o_w_(_)_ 
+    * _n_e_w___w_i_n_d_o_w_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o              _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
 ********** OO **********
     * _o_b_j___i_d_                                               * _o_p_e_n_e_r___i_d_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t       _p_r_o_p_e_r_t_y_)
       _p_r_o_p_e_r_t_y_)                                            * _O_p_t_i_o_n_s_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_)
@@ -297,19 +299,19 @@
       _p_r_o_p_e_r_t_y_)                                                                       _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_A_u_t_h        * _P_o_i_n_t_e_r_T_y_p_e_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_)
             _p_r_o_p_e_r_t_y_)                                                               * _p_o_s_t___d_a_t_a_ 
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t
             _p_r_o_p_e_r_t_y_)                                                                 _p_r_o_p_e_r_t_y_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_ _p_r_o_p_e_r_t_y_)      * _p_o_s_t___d_a_t_a___e_n_t_r_i_e_s_ 
     * _p_a_r_e_n_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)               _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t
-    * _p_a_r_e_n_t___f_r_a_m_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o_ _m_e_t_h_o_d_)          _p_r_o_p_e_r_t_y_)
-    * _p_a_t_t_e_r_n_s_                                                                      * _p_r_e_f_s_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r             _p_r_o_p_e_r_t_y_)
-      _p_r_o_p_e_r_t_y_)                                                                     * _P_R_E_S_S_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._E_v_e_n_t_T_y_p_e
-    * _P_E_N_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r_T_y_p_e_ _a_t_t_r_i_b_u_t_e_)                   _a_t_t_r_i_b_u_t_e_)
+    * _p_a_t_t_e_r_n_s_                                                                        _p_r_o_p_e_r_t_y_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r           * _p_r_e_f_s_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
+      _p_r_o_p_e_r_t_y_)                                                                       _p_r_o_p_e_r_t_y_)
+    * _P_E_N_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r_T_y_p_e_ _a_t_t_r_i_b_u_t_e_)                 * _P_R_E_S_S_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._E_v_e_n_t_T_y_p_e
+                                                                                      _a_t_t_r_i_b_u_t_e_)
                                                                                     * _p_r_i_n_t___p_a_g_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
                                                                                       _m_e_t_h_o_d_)
                                                                                           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
                                                                                           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
 ********** QQ **********
     * _q_u_i_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
@@ -346,53 +348,59 @@
                                                                                        * _R_I_G_H_T_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_u_t_t_o_n_s_ _a_t_t_r_i_b_u_t_e_)
                                                                                              o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_u_s_e_B_u_t_t_o_n_ _a_t_t_r_i_b_u_t_e_)
 ********** SS **********
     * _s_a_v_e___s_c_r_e_e_n_s_h_o_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t       * _s_e_t___w_i_n_d_o_w___p_o_s_i_t_i_o_n_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
       _m_e_t_h_o_d_)                                                              _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                   o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                * _s_e_t___w_i_n_d_o_w___r_e_c_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-    * _s_c_h_e_m_e_                                                               _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._A_u_t_h_C_h_a_l_l_e_n_g_e           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-      _p_r_o_p_e_r_t_y_)                                                          * _s_e_t___w_i_n_d_o_w___s_i_z_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-    * _s_c_r_e_e_n_s_h_o_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t        _m_e_t_h_o_d_)
+    * _s_a_v_e___s_n_a_p_s_h_o_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t           _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)                                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-    * _s_c_r_e_e_n_s_h_o_t___a_s___b_a_s_e_6_4_                                               * _s_e_t___w_i_n_d_o_w___s_t_a_t_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)         * _s_h_a_d_o_w___r_o_o_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
-    * _s_c_r_e_e_n_s_h_o_t___a_s___p_n_g_                                                    _p_r_o_p_e_r_t_y_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)         * _S_H_I_F_T_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)
-    * _s_c_r_o_l_l___t_o_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t       * _s_i_n_g_l_e___p_r_o_x_y_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _p_r_o_p_e_r_t_y_)
-      _m_e_t_h_o_d_)                                                            * _s_i_z_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)
-    * _s_e_a_r_c_h___e_l_e_m_e_n_t_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t       * _s_l_e_e_p_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                                            * _s_o_c_k_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_._B_a_s_e_T_a_r_g_e_t_ _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                   o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                * _s_o_u_r_c_e_ 
-    * _s_e_n_d___k_e_y_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._A_u_t_h_C_h_a_l_l_e_n_g_e
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)               _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                * _s_t_a_g_e_ 
-    * _s_e_t___a_u_t_h_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)             _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
-    * _s_e_t___d_o_w_n_l_o_a_d___b_e_h_a_v_i_o_u_r_(_)_                                             _p_r_o_p_e_r_t_y_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)                 * _s_t_a_r_t___d_e_s_k_t_o_p___m_i_r_r_o_r_i_n_g_(_)_ 
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                  _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
-    * _s_e_t___f_i_l_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t              o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)             * _s_e_t___w_i_n_d_o_w___s_i_z_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                  _m_e_t_h_o_d_)
+    * _s_c_h_e_m_e_                                                                   o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._A_u_t_h_C_h_a_l_l_e_n_g_e     * _s_e_t___w_i_n_d_o_w___s_t_a_t_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+      _p_r_o_p_e_r_t_y_)                                                          * _s_h_a_d_o_w___r_o_o_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
+    * _s_c_r_e_e_n_s_h_o_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t        _p_r_o_p_e_r_t_y_)
+      _m_e_t_h_o_d_)                                                            * _S_H_I_F_T_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._M_o_d_i_f_i_e_r_s_ _a_t_t_r_i_b_u_t_e_)
+    * _s_c_r_e_e_n_s_h_o_t___a_s___b_a_s_e_6_4_                                               * _s_i_n_g_l_e___p_r_o_x_y_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _p_r_o_p_e_r_t_y_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)         * _s_i_z_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)
+    * _s_c_r_e_e_n_s_h_o_t___a_s___p_n_g_                                                  * _s_l_e_e_p_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)         * _s_n_a_p_s_h_o_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
+    * _s_c_r_o_l_l___t_o_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)                                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-    * _s_e_t___f_i_l_e_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t       * _s_t_a_r_t___s_e_s_s_i_o_n_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                                            * _s_t_a_r_t___t_a_b___m_i_r_r_o_r_i_n_g_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
-    * _s_e_t___n_e_t_w_o_r_k___c_o_n_d_i_t_i_o_n_s_(_)_                                             _m_e_t_h_o_d_)
+    * _s_e_a_r_c_h___e_l_e_m_e_n_t_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t       * _s_o_c_k_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_a_s_e___t_a_r_g_e_t_._B_a_s_e_T_a_r_g_e_t_ _p_r_o_p_e_r_t_y_)
+      _m_e_t_h_o_d_)                                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)             * _s_o_u_r_c_e_ 
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                  _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._A_u_t_h_C_h_a_l_l_e_n_g_e
+    * _s_e_n_d___k_e_y_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)       _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                   o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)     * _s_t_a_g_e_ 
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                  _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._I_n_t_e_r_c_e_p_t_e_d_R_e_q_u_e_s_t
+    * _s_e_t___a_u_t_h_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)             _p_r_o_p_e_r_t_y_)
+    * _s_e_t___d_o_m___a_t_t_r_i_b_u_t_e_(_)_                                                * _s_t_a_r_t___d_e_s_k_t_o_p___m_i_r_r_o_r_i_n_g_(_)_ 
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)             _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
+    * _s_e_t___d_o_w_n_l_o_a_d___b_e_h_a_v_i_o_u_r_(_)_                                                 o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)                       o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                * _s_t_a_r_t___t_a_b___m_i_r_r_o_r_i_n_g_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+    * _s_e_t___f_i_l_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t          _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
+    * _s_e_t___f_i_l_e_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
+      _m_e_t_h_o_d_)                                                            * _s_t_a_r_t_u_p___u_r_l_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _p_r_o_p_e_r_t_y_)
+    * _s_e_t___n_e_t_w_o_r_k___c_o_n_d_i_t_i_o_n_s_(_)_                                           * _s_t_o_p___c_a_s_t_i_n_g_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)                       o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)                   o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                * _s_t_a_r_t_u_p___u_r_l_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s_ _p_r_o_p_e_r_t_y_)
-    * _s_e_t___p_e_r_m_i_s_s_i_o_n_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t       * _s_t_o_p___c_a_s_t_i_n_g_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                                                  o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
-          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                      o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
-    * _s_e_t___p_r_o_x_y_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)          * _s_u_b_m_i_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)
-    * _s_e_t___s_i_n_g_l_e___p_r_o_x_y_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e           * _s_u_b_t_y_p_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o_ _p_r_o_p_e_r_t_y_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                * _s_u_b_m_i_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)
+    * _s_e_t___p_e_r_m_i_s_s_i_o_n_s_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t       * _s_u_b_t_y_p_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o_ _p_r_o_p_e_r_t_y_)
       _m_e_t_h_o_d_)                                                            * _s_w_i_t_c_h___t_o_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t_ _p_r_o_p_e_r_t_y_)
-    * _s_e_t___s_i_n_k___t_o___u_s_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t             o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
-      _m_e_t_h_o_d_)                                                            * _S_w_i_t_c_h_T_o_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_)
+          o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)                      o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
+    * _s_e_t___p_r_o_x_y_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)          * _S_w_i_t_c_h_T_o_ _(_c_l_a_s_s_ _i_n_ _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_)
+    * _s_e_t___s_i_n_g_l_e___p_r_o_x_y_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e
+      _m_e_t_h_o_d_)
+    * _s_e_t___s_i_n_k___t_o___u_s_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t
+      _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _m_e_t_h_o_d_)
     * _s_e_t___s_o_u_r_c_e_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _m_e_t_h_o_d_)
 ********** TT **********
     * _T_A_G___N_A_M_E_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._b_y_._B_y_ _a_t_t_r_i_b_u_t_e_)                          * _t_a_r_g_e_t_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._s_w_i_t_c_h___t_o_._S_w_i_t_c_h_T_o
     * _t_a_g___n_a_m_e_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t_ _p_r_o_p_e_r_t_y_)             _m_e_t_h_o_d_)
@@ -406,22 +414,24 @@
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._N_e_t_w_o_r_k_I_n_t_e_r_c_e_p_t_o_r           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._w_e_b_d_r_i_v_e_r_._C_h_r_o_m_e_ _p_r_o_p_e_r_t_y_)
             _p_r_o_p_e_r_t_y_)                                                               * _t_o___j_s_o_n_(_)_ 
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t_ _p_r_o_p_e_r_t_y_)        _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r_E_v_e_n_t_ _m_e_t_h_o_d_)
     * _T_a_r_g_e_t_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_I_n_f_o_ _p_r_o_p_e_r_t_y_)                 * _t_r_u_s_t___t_o_k_e_n___p_a_r_a_m_s_ 
                                                                                       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t
                                                                                       _p_r_o_p_e_r_t_y_)
 ********** UU **********
+    * _u_n_f_o_c_u_s_(_)_                                            * _u_p_d_a_t_e___p_r_e_f_(_)_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
+      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._t_a_r_g_e_t_._T_a_r_g_e_t_ _m_e_t_h_o_d_)       _m_e_t_h_o_d_)
     * _u_p_(_)_                                                 * _u_r_l_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._B_a_s_e_P_o_i_n_t_e_r         _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t
       _m_e_t_h_o_d_)                                                _p_r_o_p_e_r_t_y_)
           o _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._i_n_p_u_t_._p_o_i_n_t_e_r_._P_o_i_n_t_e_r     * _u_r_l___f_r_a_g_m_e_n_t_ 
             _m_e_t_h_o_d_)                                          _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._s_c_r_i_p_t_s_._n_e_t_w_o_r_k___i_n_t_e_r_c_e_p_t_o_r_._R_e_q_u_e_s_t
-    * _u_p_d_a_t_e___p_r_e_f_(_)_                                          _p_r_o_p_e_r_t_y_)
-      _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s           * _u_s_e_r___d_a_t_a___d_i_r_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
-      _m_e_t_h_o_d_)                                                _p_r_o_p_e_r_t_y_)
+                                                             _p_r_o_p_e_r_t_y_)
+                                                           * _u_s_e_r___d_a_t_a___d_i_r_ _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._o_p_t_i_o_n_s_._O_p_t_i_o_n_s
+                                                             _p_r_o_p_e_r_t_y_)
 ********** VV **********
     * _v_a_l_u_e_                                                * _v_a_l_u_e___o_f___c_s_s___p_r_o_p_e_r_t_y_(_)_ 
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_._W_e_b_E_l_e_m_e_n_t
       _p_r_o_p_e_r_t_y_)                                              _m_e_t_h_o_d_)
 ********** WW **********
     * _w_a_i_t___d_o_w_n_l_o_a_d_(_)_                                       * _W_e_b_E_l_e_m_e_n_t_ _(_c_l_a_s_s_ _i_n
       _(_s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._c_o_n_t_e_x_t_._C_o_n_t_e_x_t              _s_e_l_e_n_i_u_m___d_r_i_v_e_r_l_e_s_s_._t_y_p_e_s_._w_e_b_e_l_e_m_e_n_t_)
```

### Comparing `selenium_driverless-1.9/docs/index.html` & `selenium_driverless-1.9.1/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" data-content_root="./">
 <head>
   <meta charset="utf-8" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Documentation of Driverless &mdash; Selenium-Driverless 1.8.0.2 documentation</title>
+  <title>Documentation of Driverless &mdash; Selenium-Driverless 1.9.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=80d5e7a1" />
       <link rel="stylesheet" type="text/css" href="_static/css/theme.css?v=19f00094" />
 
   
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="_static/jquery.js?v=5d32c60e"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="_static/documentation_options.js?v=696515ce"></script>
+        <script src="_static/documentation_options.js?v=fd4b3c67"></script>
         <script src="_static/doctools.js?v=888ff710"></script>
         <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex/" />
     <link rel="search" title="Search" href="search/" />
     <link rel="next" title="By Element Locator" href="api/By/" /> 
 </head>
```

### Comparing `selenium_driverless-1.9/docs/search/index.html` & `selenium_driverless-1.9.1/docs/search/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" data-content_root="../">
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; Selenium-Driverless 1.8.0.2 documentation</title>
+  <title>Search &mdash; Selenium-Driverless 1.9.1 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css?v=80d5e7a1" />
       <link rel="stylesheet" type="text/css" href="../_static/css/theme.css?v=19f00094" />
 
   
     
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script src="../_static/jquery.js?v=5d32c60e"></script>
         <script src="../_static/_sphinx_javascript_frameworks_compat.js?v=2cd50e6c"></script>
-        <script src="../_static/documentation_options.js?v=696515ce"></script>
+        <script src="../_static/documentation_options.js?v=fd4b3c67"></script>
         <script src="../_static/doctools.js?v=888ff710"></script>
         <script src="../_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="../_static/js/theme.js"></script>
     <script src="../_static/searchtools.js"></script>
     <script src="../_static/language_data.js"></script>
     <link rel="index" title="Index" href="../genindex/" />
     <link rel="search" title="Search" href="#" />
```

### Comparing `selenium_driverless-1.9/docs/searchindex.js` & `selenium_driverless-1.9.1/docs/searchindex.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
         "sourc": [0, 1, 2, 3, 4, 5, 6, 7],
         "set": [0, 1, 2, 3, 5, 6, 7],
         "support": [0, 1, 2, 3, 6, 7],
         "strategi": 0,
         "id": [0, 1, 5, 6, 7],
         "name": [0, 1, 2, 3, 5, 6, 7],
         "xpath": [0, 3, 6, 8],
-        "tag_nam": [0, 1, 3, 7],
+        "tag_nam": [0, 3, 7],
         "tag": 0,
         "class_nam": [0, 7],
         "css_selector": 0,
         "css": 0,
         "selector": [0, 3, 6],
         "alia": [0, 1, 7],
         "option": [1, 2, 3, 4, 5, 6, 7, 8],
@@ -28,15 +28,15 @@
         "fals": [1, 2, 3, 5, 6, 7],
         "max_ws_siz": [1, 3, 5, 6],
         "134217728": 1,
         "control": 1,
         "chromium": [1, 2, 3, 6],
         "base": [1, 3, 6],
         "browser": [1, 2, 3, 5, 6],
-        "without": [1, 3, 5, 6],
+        "without": [1, 3, 5],
         "ani": [1, 3, 5, 6, 7],
         "driver": [1, 2, 3, 4, 5, 6, 8],
         "properti": [1, 2, 3, 5, 6, 7],
         "frame_tre": 1,
         "dict": [1, 2, 3, 4, 5, 6, 7],
         "async": [1, 2, 3, 4, 5, 6, 7, 8],
         "all": [1, 2, 3, 6, 7, 8],
@@ -78,15 +78,15 @@
         "constitut": 1,
         "ar": [1, 6],
         "ignor": [1, 2],
         "return": [1, 2, 3, 4, 5, 6, 7],
         "The": [1, 2, 3, 5, 6, 7],
         "proxi": [1, 2, 5],
         "doesn": [1, 2, 3, 5, 7],
-        "t": [1, 2, 3, 5, 7, 8],
+        "t": [1, 2, 3, 5, 6, 7, 8],
         "work": 1,
         "window": [1, 3, 6, 7],
         "due": [1, 2, 4],
         "crbug": [1, 2],
         "1310057": 1,
         "server": [1, 5],
         "us": [1, 2, 3, 5, 6, 7],
@@ -110,15 +110,15 @@
         "handl": [1, 3, 5, 7],
         "global": [1, 6],
         "onli": [1, 2, 3, 6, 7],
         "bind": 1,
         "cdp": [1, 3, 6],
         "protocol": [1, 3, 6],
         "mv3_extens": [1, 2],
-        "background": 1,
+        "background": [1, 3],
         "script": [1, 3, 6, 7, 8],
         "load": [1, 2, 3, 5, 6],
         "extens": [1, 2, 3, 5, 6],
         "manifest": 1,
         "version": 1,
         "3": [1, 7],
         "ensure_extensions_incognito_allow": 1,
@@ -133,62 +133,62 @@
         "not_allow": 1,
         "configur": 1,
         "For": [1, 3, 6],
         "chang": [1, 5, 7],
         "behaviour": [1, 3],
         "you": [1, 2, 3, 5, 6, 7],
         "ll": 1,
-        "have": 1,
+        "have": [1, 6],
         "modifi": [1, 4, 8],
         "json": [1, 2, 3, 4, 5, 6, 7],
         "file": [1, 2, 3, 6, 7],
         "compress": [1, 2, 5],
         "directori": [1, 2, 3, 6],
         "see": [1, 3, 5, 6, 7, 8],
         "develop": [1, 6],
         "com": [1, 2, 8],
         "doc": [1, 6],
         "refer": [1, 3, 5, 6, 7],
         "base_context": 1,
-        "which": [1, 2, 3, 4, 5, 6],
+        "which": [1, 2, 4, 5, 6],
         "isn": [1, 7],
         "downloads_dir": [1, 2, 3, 6],
         "download": [1, 2, 3, 6],
         "set_download_behaviour": [1, 3],
         "path": [1, 2, 3, 4, 6, 7],
         "deni": [1, 3],
         "allowandnam": [1, 3],
-        "instead": [1, 2, 3, 7],
+        "instead": [1, 2, 3, 6, 7],
         "can": [1, 2, 3, 6, 7],
         "caus": [1, 3, 5],
         "some": [1, 3, 5, 8],
         "bug": [1, 3],
         "current_context": 1,
         "switch": [1, 3],
         "target_id": [1, 3, 6],
         "2": [1, 3, 4, 5, 6, 7, 8],
         "targetid": [1, 6],
         "advanc": 1,
-        "usag": [1, 3, 6, 7],
+        "usag": [1, 3, 6],
         "float": [1, 3, 4, 6, 7],
         "second": [1, 3, 6, 7],
         "": [1, 7],
         "track": 1,
         "alreadi": [1, 5],
-        "get_target_for_ifram": 1,
+        "get_target_for_ifram": [1, 6],
         "ifram": [1, 3, 6, 7],
         "specif": [1, 3, 4, 6],
         "oopif": 1,
         "site": [1, 5],
         "isol": [1, 6],
         "solut": 1,
         "look": 1,
         "webel": [1, 3, 4, 6, 8],
-        "content_docu": [1, 7],
-        "get_targets_for_ifram": 1,
+        "content_docu": [1, 6, 7],
+        "get_targets_for_ifram": [1, 6],
         "more": 1,
         "inform": 1,
         "wait_download": [1, 3, 6],
         "wait": [1, 3, 6, 7, 8],
         "someth": [1, 3, 6],
         "like": [1, 3, 6, 7],
         "frameid": [1, 3, 5, 6],
@@ -244,15 +244,15 @@
         "execut": [1, 2, 3, 6, 7],
         "javascript": [1, 3, 6, 7],
         "globalthi": [1, 3, 6, 7],
         "argument": [1, 2, 3, 6, 7],
         "document": [1, 3, 6, 7],
         "obj": [1, 3, 6, 7],
         "here": [1, 3, 6, 7],
-        "string": [1, 3, 5, 6],
+        "string": [1, 5, 6],
         "pass": [1, 2, 5, 6, 7],
         "either": [1, 2, 4, 6],
         "serializ": [1, 6],
         "remoteobject": [1, 6],
         "await": [1, 2, 3, 4, 5, 6, 7, 8],
         "valu": [1, 2, 3, 5, 6, 7],
         "idonli": [1, 6],
@@ -281,17 +281,17 @@
         "re": [1, 3, 6, 7],
         "fetch": [1, 3, 5, 6, 7],
         "httpbin": [1, 3, 5, 6, 7],
         "mind": [1, 3, 5, 6, 7],
         "cor": [1, 3, 6, 7],
         "current_url": [1, 3, 6],
         "page_sourc": [1, 3, 6],
-        "html": [1, 3, 6, 7, 8],
+        "html": [1, 6, 7, 8],
         "close": [1, 3, 6, 7],
-        "focu": [1, 3, 7],
+        "focu": [1, 3, 6, 7],
         "focus": [1, 7],
         "quit": [1, 3],
         "clean_dir": 1,
         "clean": [1, 2],
         "out": 1,
         "user": [1, 2, 5, 6, 7],
         "data": [1, 2, 3, 5, 6, 7],
@@ -300,25 +300,25 @@
         "current_window_handl": [1, 3],
         "deprec": [1, 2],
         "remov": [1, 2, 3, 6, 7],
         "current_window_id": 1,
         "windowid": 1,
         "belong": 1,
         "window_handl": [1, 3],
-        "aren": [1, 8],
+        "aren": [1, 6, 8],
         "order": [1, 5],
         "posit": [1, 3, 4],
         "do": [1, 7],
         "reli": 1,
         "index": 1,
         "iter": [1, 3, 5, 6],
         "them": 1,
         "new_window": [1, 3],
         "type_hint": [1, 3],
-        "activ": [1, 3],
+        "activ": [1, 3, 6],
         "should": [1, 2, 3, 4, 5, 6],
         "explicitli": 1,
         "new_target": 1,
         "set_window_st": 1,
         "state": 1,
         "normal": [1, 4],
         "minim": [1, 3],
@@ -391,18 +391,18 @@
         "your": [1, 3, 5, 6],
         "end": [1, 3, 6],
         "save_screenshot": [1, 3, 6],
         "func": 1,
         "get_screenshot_as_png": [1, 3, 6],
         "binari": [1, 2, 3, 5, 6, 7],
         "byte": [1, 3, 5, 6, 7],
-        "get_screenshot_as_base64": [1, 3, 6],
-        "base64": [1, 3, 5, 6, 7],
-        "encod": [1, 3, 5, 6],
-        "embed": [1, 3, 6],
+        "get_screenshot_as_base64": [],
+        "base64": [5, 6, 7],
+        "encod": [5, 6],
+        "embed": [],
         "set_window_s": [1, 3],
         "width": [1, 3],
         "height": [1, 3],
         "unless": [1, 2],
         "windowhandl": [1, 3],
         "pixel": [1, 3],
         "get_window_s": [1, 3],
@@ -514,15 +514,15 @@
         "getresponsebodi": 6,
         "requestid": [5, 6],
         "base64encod": 6,
         "bodi": [5, 6, 8],
         "respons": [5, 6],
         "get_sink": [1, 3, 6],
         "sink": [1, 3, 6],
-        "avail": [1, 3, 6],
+        "avail": [1, 3, 6, 7],
         "cast": [1, 3, 6],
         "get_issue_messag": [1, 3, 6],
         "error": [1, 3, 5, 6],
         "messag": [1, 3, 6],
         "issu": [1, 3, 6],
         "session": [1, 2, 3, 6],
         "set_sink_to_us": [1, 3, 6],
@@ -537,31 +537,31 @@
         "stop": [1, 3, 6],
         "loop": [1, 3, 6, 7],
         "alert": [1, 3, 8],
         "get_alert": 1,
         "5": [1, 2, 3, 4, 6, 7, 8],
         "default_cont": [1, 3],
         "frame_refer": 1,
-        "integ": 1,
-        "repres": [1, 6, 7],
-        "frame_nam": [1, 3],
+        "integ": [],
+        "repres": [6, 7],
+        "frame_nam": 3,
         "union": [1, 2, 4, 5, 7],
-        "what": 1,
-        "kind": 1,
-        "parent_fram": [1, 3],
-        "parent": [1, 7],
-        "If": [1, 3, 7],
-        "top": [1, 3],
-        "level": [1, 3, 7],
-        "brows": [1, 3],
-        "remain": 1,
-        "unchang": 1,
+        "what": [1, 3],
+        "kind": [1, 3],
+        "parent_fram": 3,
+        "parent": 7,
+        "If": 7,
+        "top": [],
+        "level": 7,
+        "brows": [],
+        "remain": [],
+        "unchang": [],
         "window_id": 1,
-        "window_nam": 1,
-        "main": [1, 3, 4, 5, 8],
+        "window_nam": [],
+        "main": [3, 4, 5, 8],
         "chrome": [2, 3, 5, 6, 7, 8],
         "add_argu": 2,
         "launch": 2,
         "pref": 2,
         "prefer": 2,
         "update_pref": 2,
         "updat": 2,
@@ -585,25 +585,25 @@
         "env": 2,
         "subprocess": 2,
         "popen": 2,
         "environ": 2,
         "add_extens": 2,
         "zip": 2,
         "crx": 2,
-        "etc": 2,
+        "etc": [2, 6],
         "extract": 2,
         "debugger_address": 2,
         "address": 2,
         "remot": 2,
         "instanc": [2, 6, 7],
         "make": [2, 3, 5, 6],
         "well": [2, 3],
         "single_proxi": 2,
         "auto_clean_dir": 2,
-        "automat": [2, 3, 5, 7],
+        "automat": [2, 5, 7],
         "enable_mobil": 2,
         "android_packag": 2,
         "android": 2,
         "android_act": 2,
         "device_seri": 2,
         "enabl": [2, 7],
         "mobil": 2,
@@ -622,33 +622,33 @@
         "pick": 2,
         "up": [2, 4],
         "add_experimental_opt": 2,
         "experiment": 2,
         "method": [2, 3, 5, 6, 7, 8],
         "is_incognito": 3,
         "1048576": [3, 6],
-        "drive": [3, 6],
-        "chromedriv": [3, 6],
-        "start_sess": 3,
-        "desir": 3,
-        "capabl": 3,
+        "drive": 3,
+        "chromedriv": 3,
+        "start_sess": [],
+        "desir": [],
+        "capabl": [],
         "behavior": [3, 5],
         "click": [3, 4, 7, 8],
         "const": 3,
         "accord": 3,
         "obj_id": [3, 7],
         "docs_sourc": 3,
         "start_monoton": 3,
         "everi": [3, 7],
         "associ": 3,
-        "hint": 3,
-        "select": [3, 7],
+        "hint": [],
+        "select": 7,
         "invok": 3,
         "manag": 3,
-        "full": [3, 6],
+        "full": [1, 3, 6],
         "screen": 3,
         "oper": [3, 7],
         "take": [3, 4, 5, 6, 7],
         "best": [3, 6],
         "effort": [3, 6],
         "provid": [3, 5, 6],
         "contain": 3,
@@ -743,23 +743,23 @@
         "geteventlisten": 7,
         "get_properti": 7,
         "elem": [7, 8],
         "tagnam": 7,
         "textcont": 7,
         "entri": 7,
         "highlight": 7,
-        "disabl": 7,
+        "disabl": [6, 7],
         "fade": 7,
         "is_click": 7,
         "listener_depth": 7,
         "button": [4, 7, 8],
         "input": [7, 8],
         "textarea": 7,
         "video": 7,
-        "map": 7,
+        "map": [6, 7],
         "wise": 7,
         "mousedown": [4, 7],
         "mouseup": [4, 7],
         "visible_timeout": 7,
         "spread_a": 7,
         "spread_b": 7,
         "bias_a": 7,
@@ -805,21 +805,21 @@
         "submit": 7,
         "form": 7,
         "detect": [5, 7],
         "It": 7,
         "possibl": [5, 7],
         "get_dom_attribut": 7,
         "attribut": 7,
-        "unlik": 7,
+        "unlik": [],
         "get_attribut": 7,
         "declar": 7,
         "markup": 7,
         "retriev": 7,
-        "text_length": 7,
-        "target_el": 7,
+        "text_length": [],
+        "target_el": [],
         "is_select": 7,
         "checkbox": 7,
         "radio": 7,
         "is_en": 7,
         "shadow_root": 7,
         "shadowroot": 7,
         "doe": [5, 7],
@@ -1107,15 +1107,34 @@
         "mousepress": 4,
         "mousereleas": 4,
         "wheel": 4,
         "mousewheel": 4,
         "pinter": 4,
         "want": [],
         "befor": 7,
-        "click_on": 7
+        "click_on": 7,
+        "snapshot": [1, 3, 6],
+        "mhtml": [1, 3, 6],
+        "save_snapshot": [1, 3, 6],
+        "get_snapshot": [1, 3, 6],
+        "bring": [1, 3, 6],
+        "front": [1, 3, 6],
+        "own": 6,
+        "allow_not_on_map": 6,
+        "keyboard": 6,
+        "unfocu": 6,
+        "reus": 2,
+        "webwork": 6,
+        "executioncontextid": 7,
+        "nodeid": 7,
+        "backendnodeid": 7,
+        "classnam": 7,
+        "dom_attribut": 7,
+        "welel": 7,
+        "set_dom_attribut": 7
     },
     "objects": {
         "selenium_driverless.input.pointer": [
             [4, 0, 1, "", "BasePointer"],
             [4, 0, 1, "", "Buttons"],
             [4, 0, 1, "", "EventType"],
             [4, 0, 1, "", "Modifiers"],
@@ -1273,15 +1292,14 @@
         ],
         "selenium_driverless.scripts.switch_to.SwitchTo": [
             [1, 3, 1, "", "alert"],
             [1, 1, 1, "", "default_content"],
             [1, 1, 1, "", "frame"],
             [1, 1, 1, "", "get_alert"],
             [1, 1, 1, "", "new_window"],
-            [1, 1, 1, "", "parent_frame"],
             [1, 1, 1, "", "target"],
             [1, 1, 1, "", "window"]
         ],
         "selenium_driverless.types.base_target": [
             [6, 0, 1, "", "BaseTarget"]
         ],
         "selenium_driverless.types.base_target.BaseTarget": [
@@ -1332,15 +1350,14 @@
             [3, 1, 1, "", "fullscreen_window"],
             [3, 1, 1, "", "get"],
             [3, 1, 1, "", "get_cdp_event_iter"],
             [3, 1, 1, "", "get_cookie"],
             [3, 1, 1, "", "get_cookies"],
             [3, 1, 1, "", "get_issue_message"],
             [3, 1, 1, "", "get_network_conditions"],
-            [3, 1, 1, "", "get_screenshot_as_base64"],
             [3, 1, 1, "", "get_screenshot_as_file"],
             [3, 1, 1, "", "get_screenshot_as_png"],
             [3, 1, 1, "", "get_sinks"],
             [3, 1, 1, "", "get_window_position"],
             [3, 1, 1, "", "get_window_rect"],
             [3, 1, 1, "", "get_window_size"],
             [3, 1, 1, "", "maximize_window"],
@@ -1348,25 +1365,26 @@
             [3, 1, 1, "", "new_window"],
             [3, 3, 1, "", "page_source"],
             [3, 1, 1, "", "print_page"],
             [3, 1, 1, "", "quit"],
             [3, 1, 1, "", "refresh"],
             [3, 1, 1, "", "remove_cdp_listener"],
             [3, 1, 1, "", "save_screenshot"],
+            [3, 1, 1, "", "save_snapshot"],
             [3, 1, 1, "", "search_elements"],
             [3, 1, 1, "", "send_keys"],
             [3, 1, 1, "", "set_download_behaviour"],
             [3, 1, 1, "", "set_network_conditions"],
             [3, 1, 1, "", "set_permissions"],
             [3, 1, 1, "", "set_sink_to_use"],
             [3, 1, 1, "", "set_window_position"],
             [3, 1, 1, "", "set_window_rect"],
             [3, 1, 1, "", "set_window_size"],
+            [3, 1, 1, "", "snapshot"],
             [3, 1, 1, "", "start_desktop_mirroring"],
-            [3, 1, 1, "", "start_session"],
             [3, 1, 1, "", "start_tab_mirroring"],
             [3, 1, 1, "", "stop_casting"],
             [3, 3, 1, "", "switch_to"],
             [3, 3, 1, "", "title"],
             [3, 1, 1, "", "wait_download"],
             [3, 1, 1, "", "wait_for_cdp"],
             [3, 3, 1, "", "window_handles"],
@@ -1397,14 +1415,15 @@
             [2, 3, 1, "", "user_data_dir"]
         ],
         "selenium_driverless.types.target": [
             [6, 0, 1, "", "Target"],
             [6, 0, 1, "", "TargetInfo"]
         ],
         "selenium_driverless.types.target.Target": [
+            [6, 1, 1, "", "activate"],
             [6, 1, 1, "", "add_cdp_listener"],
             [6, 1, 1, "", "add_cookie"],
             [6, 1, 1, "", "back"],
             [6, 1, 1, "", "close"],
             [6, 3, 1, "", "current_url"],
             [6, 1, 1, "", "delete_all_cookies"],
             [6, 1, 1, "", "delete_cookie"],
@@ -1413,42 +1432,47 @@
             [6, 1, 1, "", "execute_async_script"],
             [6, 1, 1, "", "execute_cdp_cmd"],
             [6, 1, 1, "", "execute_raw_script"],
             [6, 1, 1, "", "execute_script"],
             [6, 1, 1, "", "fetch"],
             [6, 1, 1, "", "find_element"],
             [6, 1, 1, "", "find_elements"],
+            [6, 1, 1, "", "focus"],
             [6, 1, 1, "", "forward"],
             [6, 1, 1, "", "get"],
             [6, 1, 1, "", "get_cdp_event_iter"],
             [6, 1, 1, "", "get_cookie"],
             [6, 1, 1, "", "get_cookies"],
             [6, 1, 1, "", "get_history"],
             [6, 1, 1, "", "get_issue_message"],
             [6, 1, 1, "", "get_network_conditions"],
-            [6, 1, 1, "", "get_screenshot_as_base64"],
             [6, 1, 1, "", "get_screenshot_as_file"],
             [6, 1, 1, "", "get_screenshot_as_png"],
             [6, 1, 1, "", "get_sinks"],
+            [6, 1, 1, "", "get_target_for_iframe"],
+            [6, 1, 1, "", "get_targets_for_iframes"],
             [6, 3, 1, "", "page_source"],
             [6, 3, 1, "", "pointer"],
             [6, 1, 1, "", "print_page"],
             [6, 1, 1, "", "refresh"],
             [6, 1, 1, "", "remove_cdp_listener"],
             [6, 1, 1, "", "save_screenshot"],
+            [6, 1, 1, "", "save_snapshot"],
             [6, 1, 1, "", "search_elements"],
             [6, 1, 1, "", "send_keys"],
             [6, 1, 1, "", "set_network_conditions"],
             [6, 1, 1, "", "set_sink_to_use"],
             [6, 1, 1, "", "set_source"],
+            [6, 1, 1, "", "snapshot"],
             [6, 3, 1, "", "socket"],
             [6, 1, 1, "", "start_desktop_mirroring"],
             [6, 1, 1, "", "start_tab_mirroring"],
             [6, 1, 1, "", "stop_casting"],
             [6, 3, 1, "", "title"],
+            [6, 1, 1, "", "unfocus"],
             [6, 1, 1, "", "wait_download"],
             [6, 1, 1, "", "wait_for_cdp"],
             [6, 1, 1, "", "xhr"]
         ],
         "selenium_driverless.types.target.TargetInfo": [
             [6, 3, 1, "", "Target"],
             [6, 3, 1, "", "attached"],
@@ -1461,19 +1485,23 @@
         ],
         "selenium_driverless.types.webelement": [
             [7, 0, 1, "", "WebElement"]
         ],
         "selenium_driverless.types.webelement.WebElement": [
             [7, 3, 1, "", "accessible_name"],
             [7, 3, 1, "", "aria_role"],
+            [7, 3, 1, "", "backend_node_id"],
             [7, 3, 1, "", "box_model"],
+            [7, 3, 1, "", "class_name"],
             [7, 1, 1, "", "clear"],
             [7, 1, 1, "", "click"],
             [7, 3, 1, "", "content_document"],
+            [7, 3, 1, "", "context_id"],
             [7, 3, 1, "", "document_url"],
+            [7, 3, 1, "", "dom_attributes"],
             [7, 1, 1, "", "eval_async"],
             [7, 1, 1, "", "execute_async_script"],
             [7, 1, 1, "", "execute_script"],
             [7, 1, 1, "", "find_element"],
             [7, 1, 1, "", "find_elements"],
             [7, 1, 1, "", "focus"],
             [7, 1, 1, "", "get_attribute"],
@@ -1484,23 +1512,25 @@
             [7, 1, 1, "", "is_clickable"],
             [7, 1, 1, "", "is_displayed"],
             [7, 1, 1, "", "is_enabled"],
             [7, 1, 1, "", "is_selected"],
             [7, 3, 1, "", "location"],
             [7, 3, 1, "", "location_once_scrolled_into_view"],
             [7, 1, 1, "", "mid_location"],
+            [7, 3, 1, "", "node_id"],
             [7, 3, 1, "", "obj_id"],
             [7, 3, 1, "", "parent"],
             [7, 3, 1, "", "rect"],
             [7, 1, 1, "", "remove"],
             [7, 1, 1, "", "screenshot"],
             [7, 3, 1, "", "screenshot_as_base64"],
             [7, 3, 1, "", "screenshot_as_png"],
             [7, 1, 1, "", "scroll_to"],
             [7, 1, 1, "", "send_keys"],
+            [7, 1, 1, "", "set_dom_attribute"],
             [7, 1, 1, "", "set_file"],
             [7, 1, 1, "", "set_files"],
             [7, 1, 1, "", "set_source"],
             [7, 3, 1, "", "shadow_root"],
             [7, 3, 1, "", "size"],
             [7, 3, 1, "", "source"],
             [7, 1, 1, "", "submit"],
@@ -1549,15 +1579,14 @@
             [1, 1, 1, "", "fullscreen_window"],
             [1, 1, 1, "", "get"],
             [1, 1, 1, "", "get_cdp_event_iter"],
             [1, 1, 1, "", "get_cookie"],
             [1, 1, 1, "", "get_cookies"],
             [1, 1, 1, "", "get_issue_message"],
             [1, 1, 1, "", "get_network_conditions"],
-            [1, 1, 1, "", "get_screenshot_as_base64"],
             [1, 1, 1, "", "get_screenshot_as_file"],
             [1, 1, 1, "", "get_screenshot_as_png"],
             [1, 1, 1, "", "get_sinks"],
             [1, 1, 1, "", "get_target"],
             [1, 1, 1, "", "get_target_for_iframe"],
             [1, 1, 1, "", "get_targets"],
             [1, 1, 1, "", "get_targets_for_iframes"],
@@ -1572,28 +1601,30 @@
             [1, 1, 1, "", "normalize_window"],
             [1, 3, 1, "", "page_source"],
             [1, 1, 1, "", "print_page"],
             [1, 1, 1, "", "quit"],
             [1, 1, 1, "", "refresh"],
             [1, 1, 1, "", "remove_cdp_listener"],
             [1, 1, 1, "", "save_screenshot"],
+            [1, 1, 1, "", "save_snapshot"],
             [1, 1, 1, "", "search_elements"],
             [1, 1, 1, "", "send_keys"],
             [1, 1, 1, "", "set_auth"],
             [1, 1, 1, "", "set_download_behaviour"],
             [1, 1, 1, "", "set_network_conditions"],
             [1, 1, 1, "", "set_permissions"],
             [1, 1, 1, "", "set_proxy"],
             [1, 1, 1, "", "set_single_proxy"],
             [1, 1, 1, "", "set_sink_to_use"],
             [1, 1, 1, "", "set_window_position"],
             [1, 1, 1, "", "set_window_rect"],
             [1, 1, 1, "", "set_window_size"],
             [1, 1, 1, "", "set_window_state"],
             [1, 1, 1, "", "sleep"],
+            [1, 1, 1, "", "snapshot"],
             [1, 1, 1, "", "start_desktop_mirroring"],
             [1, 1, 1, "", "start_tab_mirroring"],
             [1, 1, 1, "", "stop_casting"],
             [1, 3, 1, "", "switch_to"],
             [1, 3, 1, "", "targets"],
             [1, 3, 1, "", "title"],
             [1, 1, 1, "", "wait_download"],
@@ -1653,192 +1684,264 @@
         "sphinx.ext.viewcode": 1,
         "sphinx": 60
     },
     "alltitles": {
         "By Element Locator": [
             [0, "by-element-locator"]
         ],
+        "webdriver.Chrome": [
+            [1, "webdriver-chrome"]
+        ],
         "ChromeOptions": [
             [2, "chromeoptions"]
         ],
+        "Context": [
+            [3, "context"]
+        ],
+        "Input": [
+            [4, "input"]
+        ],
+        "Request-Interception": [
+            [5, "request-interception"]
+        ],
+        "Example Script": [
+            [5, "example-script"]
+        ],
+        "API": [
+            [5, "api"],
+            [8, "api"]
+        ],
+        "WebElement": [
+            [7, "webelement"]
+        ],
         "Documentation of Driverless": [
             [8, "documentation-of-driverless"]
         ],
         "Installation": [
             [8, "installation"]
         ],
         "Usage": [
             [8, "usage"]
         ],
-        "API": [
-            [8, "api"],
-            [5, "api"]
-        ],
         "Source": [
             [8, "source"]
         ],
-        "Request-Interception": [
-            [5, "request-interception"]
+        "Target": [
+            [6, "target"]
+        ]
+    },
+    "indexentries": {
+        "basetarget (class in selenium_driverless.types.base_target)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget"]
         ],
-        "Example Script": [
-            [5, "example-script"]
+        "target (class in selenium_driverless.types.target)": [
+            [6, "selenium_driverless.types.target.Target"]
         ],
-        "Input": [
-            [4, "input"]
+        "target (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.Target"]
         ],
-        "webdriver.Chrome": [
-            [1, "webdriver-chrome"]
+        "targetinfo (class in selenium_driverless.types.target)": [
+            [6, "selenium_driverless.types.target.TargetInfo"]
         ],
-        "Context": [
-            [3, "context"]
+        "activate() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.activate"]
         ],
-        "Target": [
-            [6, "target"]
+        "add_cdp_listener() (selenium_driverless.types.base_target.basetarget method)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.add_cdp_listener"]
         ],
-        "WebElement": [
-            [7, "webelement"]
-        ]
-    },
-    "indexentries": {
-        "webelement (class in selenium_driverless.types.webelement)": [
-            [7, "selenium_driverless.types.webelement.WebElement"]
+        "add_cdp_listener() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.add_cdp_listener"]
+        ],
+        "add_cookie() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.add_cookie"]
+        ],
+        "attached (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.attached"]
+        ],
+        "back() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.back"]
+        ],
+        "browser_context_id (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.browser_context_id"]
+        ],
+        "can_access_opener (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.can_access_opener"]
+        ],
+        "close() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.close"]
+        ],
+        "current_url (selenium_driverless.types.target.target property)": [
+            [6, "selenium_driverless.types.target.Target.current_url"]
+        ],
+        "delete_all_cookies() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.delete_all_cookies"]
+        ],
+        "delete_cookie() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.delete_cookie"]
+        ],
+        "delete_network_conditions() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.delete_network_conditions"]
+        ],
+        "downloads_dir_for_context() (selenium_driverless.types.base_target.basetarget method)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.downloads_dir_for_context"]
+        ],
+        "eval_async() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.eval_async"]
+        ],
+        "execute_async_script() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.execute_async_script"]
+        ],
+        "execute_cdp_cmd() (selenium_driverless.types.base_target.basetarget method)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.execute_cdp_cmd"]
+        ],
+        "execute_cdp_cmd() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.execute_cdp_cmd"]
+        ],
+        "execute_raw_script() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.execute_raw_script"]
+        ],
+        "execute_script() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.execute_script"]
+        ],
+        "fetch() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.fetch"]
         ],
-        "accessible_name (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.accessible_name"]
+        "find_element() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.find_element"]
         ],
-        "aria_role (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.aria_role"]
+        "find_elements() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.find_elements"]
         ],
-        "box_model (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.box_model"]
+        "focus() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.focus"]
         ],
-        "clear() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.clear"]
+        "forward() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.forward"]
         ],
-        "click() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.click"]
+        "get() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get"]
         ],
-        "content_document (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.content_document"]
+        "get_cdp_event_iter() (selenium_driverless.types.base_target.basetarget method)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.get_cdp_event_iter"]
         ],
-        "document_url (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.document_url"]
+        "get_cdp_event_iter() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_cdp_event_iter"]
         ],
-        "eval_async() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.eval_async"]
+        "get_cookie() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_cookie"]
         ],
-        "execute_async_script() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.execute_async_script"]
+        "get_cookies() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_cookies"]
         ],
-        "execute_script() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.execute_script"]
+        "get_history() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_history"]
         ],
-        "find_element() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.find_element"]
+        "get_issue_message() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_issue_message"]
         ],
-        "find_elements() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.find_elements"]
+        "get_network_conditions() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_network_conditions"]
         ],
-        "focus() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.focus"]
+        "get_screenshot_as_file() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_screenshot_as_file"]
         ],
-        "get_attribute() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.get_attribute"]
+        "get_screenshot_as_png() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_screenshot_as_png"]
         ],
-        "get_dom_attribute() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.get_dom_attribute"]
+        "get_sinks() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_sinks"]
         ],
-        "get_listeners() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.get_listeners"]
+        "get_target_for_iframe() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_target_for_iframe"]
         ],
-        "get_property() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.get_property"]
+        "get_targets_for_iframes() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.get_targets_for_iframes"]
         ],
-        "highlight() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.highlight"]
+        "id (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.id"]
         ],
-        "is_clickable() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.is_clickable"]
+        "opener_frame_id (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.opener_frame_id"]
         ],
-        "is_displayed() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.is_displayed"]
+        "opener_id (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.opener_id"]
         ],
-        "is_enabled() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.is_enabled"]
+        "page_source (selenium_driverless.types.target.target property)": [
+            [6, "selenium_driverless.types.target.Target.page_source"]
         ],
-        "is_selected() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.is_selected"]
+        "pointer (selenium_driverless.types.target.target property)": [
+            [6, "selenium_driverless.types.target.Target.pointer"]
         ],
-        "location (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.location"]
+        "print_page() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.print_page"]
         ],
-        "location_once_scrolled_into_view (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.location_once_scrolled_into_view"]
+        "refresh() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.refresh"]
         ],
-        "mid_location() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.mid_location"]
+        "remove_cdp_listener() (selenium_driverless.types.base_target.basetarget method)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.remove_cdp_listener"]
         ],
-        "obj_id (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.obj_id"]
+        "remove_cdp_listener() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.remove_cdp_listener"]
         ],
-        "parent (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.parent"]
+        "save_screenshot() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.save_screenshot"]
         ],
-        "rect (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.rect"]
+        "save_snapshot() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.save_snapshot"]
         ],
-        "remove() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.remove"]
+        "search_elements() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.search_elements"]
         ],
-        "screenshot() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.screenshot"]
+        "send_keys() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.send_keys"]
         ],
-        "screenshot_as_base64 (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.screenshot_as_base64"]
+        "set_network_conditions() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.set_network_conditions"]
         ],
-        "screenshot_as_png (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.screenshot_as_png"]
+        "set_sink_to_use() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.set_sink_to_use"]
         ],
-        "scroll_to() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.scroll_to"]
+        "set_source() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.set_source"]
         ],
-        "send_keys() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.send_keys"]
+        "snapshot() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.snapshot"]
         ],
-        "set_file() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.set_file"]
+        "socket (selenium_driverless.types.base_target.basetarget property)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.socket"]
         ],
-        "set_files() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.set_files"]
+        "socket (selenium_driverless.types.target.target property)": [
+            [6, "selenium_driverless.types.target.Target.socket"]
         ],
-        "set_source() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.set_source"]
+        "start_desktop_mirroring() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.start_desktop_mirroring"]
         ],
-        "shadow_root (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.shadow_root"]
+        "start_tab_mirroring() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.start_tab_mirroring"]
         ],
-        "size (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.size"]
+        "stop_casting() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.stop_casting"]
         ],
-        "source (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.source"]
+        "subtype (selenium_driverless.types.target.targetinfo property)": [
+            [6, "selenium_driverless.types.target.TargetInfo.subtype"]
         ],
-        "submit() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.submit"]
+        "title (selenium_driverless.types.target.target property)": [
+            [6, "selenium_driverless.types.target.Target.title"]
         ],
-        "tag_name (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.tag_name"]
+        "unfocus() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.unfocus"]
         ],
-        "text (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.text"]
+        "wait_download() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.wait_download"]
         ],
-        "value (selenium_driverless.types.webelement.webelement property)": [
-            [7, "selenium_driverless.types.webelement.WebElement.value"]
+        "wait_for_cdp() (selenium_driverless.types.base_target.basetarget method)": [
+            [6, "selenium_driverless.types.base_target.BaseTarget.wait_for_cdp"]
         ],
-        "value_of_css_property() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.value_of_css_property"]
+        "wait_for_cdp() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.wait_for_cdp"]
         ],
-        "write() (selenium_driverless.types.webelement.webelement method)": [
-            [7, "selenium_driverless.types.webelement.WebElement.write"]
+        "xhr() (selenium_driverless.types.target.target method)": [
+            [6, "selenium_driverless.types.target.Target.xhr"]
         ]
     }
 })
```

### Comparing `selenium_driverless-1.9/docs_source/conf.py` & `selenium_driverless-1.9.1/docs_source/conf.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/docs_source/index.rst` & `selenium_driverless-1.9.1/docs_source/index.rst`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/examples/proxy_with_auth.py` & `selenium_driverless-1.9.1/examples/proxy_with_auth.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/setup.py` & `selenium_driverless-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/files/js/show_mousemove.js` & `selenium_driverless-1.9.1/src/selenium_driverless/files/js/show_mousemove.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js` & `selenium_driverless-1.9.1/src/selenium_driverless/files/mv3_extension/driverless_background_mv3_243ffdd55e32a012b4f253b2879af978.js`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/files/mv3_extension/manifest.json` & `selenium_driverless-1.9.1/src/selenium_driverless/files/mv3_extension/manifest.json`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/input/pointer.py` & `selenium_driverless-1.9.1/src/selenium_driverless/input/pointer.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/scripts/driver_utils.py` & `selenium_driverless-1.9.1/src/selenium_driverless/scripts/driver_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,15 @@
     await target.execute_cdp_cmd("Network.clearBrowserCookies")
 
 
 # noinspection GrazieInspection
 async def add_cookie(target, cookie_dict, context_id: str = None) -> None:
     """Adds a cookie to your current session.
 
-    :Args:
-     - cookie_dict: A dictionary object, with required keys - "name" and "value";
+    :param cookie_dict: A dictionary object, with required keys - "name" and "value";
         optional keys - "path", "domain", "secure", "httpOnly", "expiry", "sameSite"
 
     :Usage:
         ::
 
             target.add_cookie({'name' : 'foo', 'value' : 'bar'})
             target.add_cookie({'name' : 'foo', 'value' : 'bar', 'path' : '/'})
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/scripts/geometry.py` & `selenium_driverless-1.9.1/src/selenium_driverless/scripts/geometry.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/scripts/network_interceptor.py` & `selenium_driverless-1.9.1/src/selenium_driverless/scripts/network_interceptor.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/scripts/prefs.py` & `selenium_driverless-1.9.1/src/selenium_driverless/scripts/prefs.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.9.1/src/selenium_driverless/scripts/switch_to.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,99 +86,87 @@
 
                 target.switch_to.default_content()
         """
         base_target = self._context.current_target.base_target
         if base_target:
             return await self.target(target_id=base_target, activate=activate)
 
-    async def frame(self, frame_reference: Union[str, int, WebElement], activate: bool = False) -> None:
-        """Switches focus to the specified frame, by index, name, or
-        webelement.
+    async def frame(self, frame_reference: Union[str, int, WebElement], focus:bool=True) -> None:
+        """Switches to the specified frame
 
-        .. warning::
-
-            this is deprecated and should not be used
-
-        :Args:
-         - frame_reference: The name of the window to switch to, an integer representing the index,
-                            or a webelement that is an (i)frame to switch to.
-
-        :Usage:
-            ::
-
-                target.switch_to.frame('frame_name')
-                target.switch_to.frame(1)
-                target.switch_to.frame(target.find_elements(By.TAG_NAME, "iframe")[0])
+        :param frame_reference: the reference by ID, name, index, or WebElement
+        :param focus: whether to emulate focus on the frame
+        :param focus: whether to emulate focus on the iframe
         """
         warnings.warn(
             "driver.switch_to.iframe deprecated and not reliable use Webelement.content_document instead",
             DeprecationWarning)
         if isinstance(frame_reference, str):
             try:
                 frame_reference = await self._context.find_element(By.ID, frame_reference)
             except NoSuchElementException:
                 try:
                     frame_reference = await self._context.find_element(By.NAME, frame_reference)
                 except NoSuchElementException:
-                    raise NoSuchIframe(frame_reference, f"couldn't get element by: {frame_reference}")
+                    pass
+        if isinstance(frame_reference, int):
+            try:
+                frames = await self._context.find_elements(By.TAG_NAME, "iframe")
+                frame_reference = frames[frame_reference]
+            except KeyError:
+                pass
+
+        if not isinstance(frame_reference, WebElement):
+            raise NoSuchIframe(frame_reference, f"couldn't get element by: {frame_reference}")
         target = await self._context.current_target.get_target_for_iframe(frame_reference)
-        if activate:
+        if focus:
             await target.focus()
+        await self.target(target)
         return target
 
-    async def target(self, target_id: typing.Union[str, TargetInfo, Target], activate: bool = True) -> Target:
+    async def target(self, target_id: typing.Union[str, TargetInfo, Target], activate: bool = False, focus:bool=True) -> Target:
         """
         switches to a target
 
         :param target_id: the target to switch to
-        :param activate: whether to activate the target
+        :param activate: whether to bring the target to the front
+        :param focus: whether to emulate focus on the target
         """
         if isinstance(target_id, TargetInfo):
             self._context._current_target = target_id.Target
         elif isinstance(target_id, Target):
             self._context._current_target = target_id
         elif isinstance(target_id, WebElement):
             # noinspection PyDeprecation
-            self._context._current_target = self.frame(target_id, activate=False)
+            self._context._current_target = self.frame(target_id)
         else:
             self._context._current_target = await self._context.get_target(target_id)
 
         if activate:
+            await self._context.current_target.activate()
+        if focus:
             await self._context.current_target.focus()
         return self._context.current_target
 
-    async def new_window(self, type_hint: typing.Literal["tab", "window"] = "tab", url="", activate: bool = True) -> Target:
-        """Switches to a new window
-
-        :param type_hint: what kind of window to switch to
-        :param url: url to load in the new target
-        :param activate: whether to activate the new target
+    async def window(self, window_id: str or TargetInfo, activate: bool = False, focus:bool=True) -> Target:
         """
-        target = await self._context.new_window(type_hint=type_hint, url=url, activate=activate)
-        return await self.target(target, activate=activate)
-
-    async def parent_frame(self, activate: bool = False) -> None:
-        """Switches focus to the parent context. If the current context is the
-        top level browsing context, the context remains unchanged.
-
-        :Usage:
-            ::
+        switches to a window
 
-                target.switch_to.parent_frame()
+        alias to :func:`SwitchTo.target <selenium_driverless.scripts.switch_to.SwitchTo.target`
         """
-        # noinspection PyProtectedMember
-        parent = self._context.current_target._parent_target
-        if parent:
-            await self.target(target_id=parent, activate=activate)
+        return await self.target(window_id, activate=activate, focus=focus)
 
-    async def window(self, window_id: str or TargetInfo, activate: bool = True) -> None:
-        """Switches focus to the specified window.
+    async def new_window(self, type_hint: typing.Literal["tab", "window"] = "tab", url="", activate: bool = False,
+                         focus: bool = True, background: bool = True) -> Target:
+        """creates a new tab or window
 
-        :Args:
-         - window_name: The name or window handle of the window to switch to.
-
-        :Usage:
-            ::
-
-                target.switch_to.window('main')
+        :param type_hint: what kind of target to create
+        :param url: url to start the target at
+        :param activate: whether to bring the target to the front
+        :param focus: whether to emulate focus on the target
+        :param background: whether to start the target in the background
         """
-        await self.target(window_id, activate=activate)
+        target = await self._context.new_window(type_hint=type_hint, url=url, activate=activate, focus=focus, background=background)
+        return await self.target(target)
+
+    async def parent_frame(self, activate: bool = False) -> Target:
+        raise NotImplemented()
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/alert.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/base_target.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/base_target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/context.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/context.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/executor.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/executor.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/pointer.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/pointer.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/switch_to.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/target.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/webdriver.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/sync/webelement.py` & `selenium_driverless-1.9.1/src/selenium_driverless/sync/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/alert.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         alert_text = Alert(target).text
         self.assertEqual("Do you wish to quit?", alert_text)
     """
 
     def __init__(self, target, timeout: float = 5) -> None:
         """Creates a new Alert.
 
-        :Args:
-         - target: The WebDriver instance which performs user actions.
+        :param target: The Target instance which performs user actions.
         """
         from selenium_driverless.types.target import Target
         self.target: Target = target
         self._timeout = timeout
         self._started = False
 
     def __await__(self):
@@ -114,11 +113,10 @@
         """Accepts the alert available."""
         await self.target.execute_cdp_cmd("Page.handleJavaScriptDialog", {"accept": True})
 
     # noinspection PyPep8Naming
     async def send_keys(self, keysToSend: str) -> None:
         """Send Keys to the Alert.
 
-        :Args:
-         - keysToSend: The text to be sent to Alert.
+        :param keysToSend: The text to be sent to Alert.
         """
         await self.target.execute_cdp_cmd("Page.handleJavaScriptDialog", {"accept": True, "promptText": keysToSend})
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/base_target.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/base_target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/by.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/by.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/context.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,19 +90,14 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
     def __await__(self):
         return self.start_session().__await__()
 
     async def start_session(self):
-        """Creates a new session with the desired capabilities.
-
-        :Args:
-         - capabilities - a capabilities dict to start the session with.
-        """
         from selenium_driverless.webdriver import Chrome
         self._driver: Chrome
 
         if not self._started:
             if not self.context_id:
                 self._context_id = await self._current_target.browser_context_id
             _type = await self.current_target.type
@@ -116,15 +111,15 @@
                     else:
                         del targets[_id]
             if self._loop:
                 self._switch_to = await SyncSwitchTo(context=self, loop=self._loop, context_id=self._context_id)
             else:
                 self._switch_to = await SwitchTo(context=self, loop=self._loop, context_id=self._context_id)
             if targets:
-                await self.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": True})
+                await self.current_target.focus(activate=False)
             self._started = True
         return self
 
     @property
     async def frame_tree(self):
         return await self.current_target.frame_tree
 
@@ -461,42 +456,45 @@
         tabs = []
         targets = await self.targets
         for info in list(targets.values()):
             if info.type == "page":
                 tabs.append(info)
         return tabs
 
-    async def new_window(self, type_hint: Optional[str] = "tab", url="", activate: bool = True) -> Target:
-        """Switches to a new top-level browsing context.
-
-        The type hint can be one of "tab" or "window". If not specified the
-        browser will automatically select it.
-
-        :Usage:
-            ::
+    async def new_window(self, type_hint: typing.Literal["tab", "window"] = "tab", url="", activate: bool = False, focus:bool=True, background:bool=True) -> Target:
+        """creates a new tab or window
 
-                target.switch_to.new_window('tab')
+        :param type_hint: what kind of target to create
+        :param url: url to start the target at
+        :param activate: whether to bring the target to the front
+        :param focus: whether to emulate focus on the target
+        :param background: whether to start the target in the background
         """
         if self._is_incognito and url in ["chrome://extensions"]:
             raise ValueError(f"{url} only supported in non-incognito contexts")
-        new_tab = False
+
+        args = {"url": url}
         if type_hint == "window":
-            new_tab = True
+            args["newWindow"] = True
         elif type_hint == "tab":
             pass
         else:
             raise ValueError("type hint needs to be 'window' or 'tab'")
-        args = {"url": url, "newWindow": new_tab, "forTab": new_tab}
+        if not (background is None):
+            args["background"] = background
+
         # noinspection PyProtectedMember
         if self._context_id and self._is_incognito:
             args["browserContextId"] = self._context_id
         target = await self.base_target.execute_cdp_cmd("Target.createTarget", args)
         target_id = target["targetId"]
         target = await self.get_target(target_id)
         if activate:
+            await target.activate()
+        if focus:
             await target.focus()
         return target
 
     async def set_window_state(self, state):
         states = ["normal", "minimized", "maximized", "fullscreen"]
         if state not in states:
             raise ValueError(f"expected one of {states}, but got: {state}")
@@ -618,31 +616,29 @@
 
                 target.delete_all_cookies()
         """
         target = await self.get_target(target_id=target_id)
         await target.delete_all_cookies()
 
     # noinspection GrazieInspection
-    async def add_cookie(self, cookie_dict: dict, target_id: str = None) -> None:
+    async def add_cookie(self, cookie_dict: dict) -> None:
         """Adds a cookie to your current session.
 
-        :Args:
-         - cookie_dict: A dictionary object, with required keys - "name" and "value";
+        :param cookie_dict: A dictionary object, with required keys - "name" and "value";
             optional keys - "path", "domain", "secure", "httpOnly", "expiry", "sameSite"
 
         :Usage:
             ::
 
                 target.add_cookie({'name' : 'foo', 'value' : 'bar'})
                 target.add_cookie({'name' : 'foo', 'value' : 'bar', 'path' : '/'})
                 target.add_cookie({'name' : 'foo', 'value' : 'bar', 'path' : '/', 'secure' : True})
                 target.add_cookie({'name' : 'foo', 'value' : 'bar', 'sameSite' : 'Strict'})
         """
-        target = await self.get_target(target_id=target_id)
-        await target.add_cookie(cookie_dict=cookie_dict)
+        await self.current_target.add_cookie(cookie_dict=cookie_dict)
 
     # Timeouts
     @staticmethod
     async def sleep(time_to_wait: float) -> None:
         await asyncio.sleep(time_to_wait)
 
     # noinspection PyUnusedLocal
@@ -668,31 +664,21 @@
     async def search_elements(self, query: str, target_id: str = None) -> typing.List[WebElement]:
         """
         query:str | Plain text or query selector or XPath search query.
         """
         target = await self.get_target(target_id=target_id)
         return await target.search_elements(query=query)
 
-    async def get_screenshot_as_file(self, filename: str, target_id: str = None) -> bool:
-        # noinspection GrazieInspection
+    async def get_screenshot_as_file(self, filename: str) -> bool:
         """Saves a screenshot of the current window to a PNG image file.
-                Returns False if there is any IOError, else returns True. Use full
-                paths in your filename.
 
-                :Args:
-                 - filename: The full path you wish to save your screenshot to. This
+        :param filename: The full path you wish to save your screenshot to. This
                    should end with a `.png` extension.
-
-                :Usage:
-                    ::
-
-                        target.get_screenshot_as_file('/Screenshots/foo.png')
-                """
-        target = await self.get_target(target_id=target_id)
-        return await target.get_screenshot_as_file(filename=filename)
+        """
+        return await self.current_target.get_screenshot_as_file(filename=filename)
 
     async def save_screenshot(self, filename, target_id: str = None) -> bool:
         # noinspection GrazieInspection
         """Saves a screenshot of the current window to a PNG image file.
                 Returns False if there is any IOError, else returns True. Use full
                 paths in your filename.
 
@@ -715,25 +701,30 @@
             ::
 
                 target.get_screenshot_as_png()
         """
         target = await self.get_target(target_id=target_id)
         return await target.get_screenshot_as_png()
 
-    async def get_screenshot_as_base64(self, target_id: str = None) -> str:
-        """Gets the screenshot of the current window as a base64 encoded string
-        which is useful in embedded images in HTML.
+    async def snapshot(self) -> str:
+        """gets the current snapshot as mhtml"""
+        return await self.current_target.snapshot()
 
-        :Usage:
-            ::
+    async def save_snapshot(self, filename: str):
+        """Saves a snapshot of the current window to a MHTML file.
+
+        :param filename: The full path you wish to save your snapshot to. This
+                   should end with a ``.mhtml`` extension.
+
+        .. code-block:: Python
+
+            await driver.get_snapshot('snapshot.mhtml')
 
-                target.get_screenshot_as_base64()
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.get_screenshot_as_base64()
+        return await self.current_target.save_snapshot(filename)
 
     # noinspection PyPep8Naming
     async def set_window_size(self, width, height, windowHandle: str = "current") -> None:
         """Sets the width and height of the current window. (window.resizeTo)
 
         :Args:
          - width: the width in pixels to set the window to
@@ -745,25 +736,16 @@
                 target.set_window_size(800,600)
         """
         if windowHandle != "current":
             warnings.warn("Only 'current' window is supported for W3C compatible browsers.")
         await self.set_window_rect(width=int(width), height=int(height))
 
     # noinspection PyPep8Naming
-    async def get_window_size(self, windowHandle: str = "current") -> dict:
-        """Gets the width and height of the current window.
-
-        :Usage:
-            ::
-
-                target.get_window_size()
-        """
-
-        if windowHandle != "current":
-            warnings.warn("Only 'current' window is supported for W3C compatible browsers.")
+    async def get_window_size(self) -> dict:
+        """Gets the width and height of the current window."""
         size = await self.get_window_rect()
 
         if size.get("value", None):
             size = size["value"]
 
         return {k: size[k] for k in ("width", "height")}
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/deserialize.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/deserialize.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/options.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 
 from selenium_driverless.utils.utils import sel_driverless_path
 from selenium_driverless.scripts.prefs import prefs_to_json
 
 
 # noinspection PyUnreachableCode,PyUnusedLocal
 class Options(metaclass=ABCMeta):
+    """
+    the `webdriver.ChromeOptions` class
+
+    .. warning::
+
+        options should not be reused
+
+    """
 
     def __init__(self) -> None:
 
         self._single_proxy = None
         from selenium_driverless.utils.utils import find_chrome_executable, IS_POSIX
         super().__init__()
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/target.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,36 +56,31 @@
     ' ': ('Space', 32)
 }
 
 SHIFT_KEY_NEEDED = '~!@#$%^&*()_+{}|:"<>?'
 
 
 class NoSuchIframe(Exception):
-    def __init__(self, elem: WebElement, message: str):
-        self._elem = elem
-        super().__init__(message)
+    reference: typing.Union[WebElement, int, str]
 
-    @property
-    def elem(self):
-        return self._elem
+    def __init__(self, reference: typing.Union[WebElement, int, str], message: str):
+        self.reference = reference
+        super().__init__(message)
 
 
 class Target:
-    """Allows you to drive the browser without chromedriver."""
+    """the Target class
+
+    Usually a tab, (cors-)iframe, WebWorker etc.
+    """
 
     # noinspection PyShadowingBuiltins
     def __init__(self, host: str, target_id: str, driver, context, is_remote: bool = False,
                  loop: asyncio.AbstractEventLoop or None = None, timeout: float = 30,
                  type: str = None, start_socket: bool = False, max_ws_size: int = 2 ** 20) -> None:
-        """Creates a new instance of the chrome target. Starts the service and
-        then creates new instance of chrome target.
-
-        :Args:
-         - options - this takes an instance of ChromeOptions.rst
-        """
         from selenium_driverless.types.context import Context
         self._parent_target = None
         self._context: Context = context
         self._window_id = None
         self._pointer = None
         self._page_enabled = None
         self._dom_enabled = None
@@ -206,14 +201,26 @@
         if self._loop:
             alert = SyncAlert(self, loop=self._loop, timeout=timeout)
         else:
             alert = await Alert(self, timeout=timeout)
         return alert
 
     async def get_targets_for_iframes(self, iframes: typing.List[WebElement]):
+        """
+        find targets for a list of iframes
+
+        :param iframes: iframes to find targets for
+
+        .. warning::
+
+            only CORS iframes have its own target,
+            you might use :func:`WebElement.content_document <selenium_driverless.types.webelement.WebElement.content_document>`
+            instead
+
+        """
         if not iframes:
             raise ValueError(f"Expected WebElements, but got{iframes}")
 
         async def target_getter(target_id: str, timeout: float = 2, max_ws_size: int = 2 ** 20):
             return await get_target(target_id=target_id, host=self._host, loop=self._loop, is_remote=self._is_remote,
                                     timeout=timeout, max_ws_size=max_ws_size, driver=self._driver,
                                     context=self._context)
@@ -239,14 +246,26 @@
                         target._parent_target = self
                     else:
                         target._base_target = self
                     targets[target.id] = target
         return list(targets.values())
 
     async def get_target_for_iframe(self, iframe: WebElement):
+        """
+        find a target for an iframe
+
+        :param iframe: iframe to find target for
+
+        .. warning::
+
+            only CORS iframes have its own target,
+            you might use :func:`WebElement.content_document <selenium_driverless.types.webelement.WebElement.content_document>`
+            instead
+
+        """
         targets = await self.get_targets_for_iframes([iframe])
         if not targets:
             raise NoSuchIframe(iframe, "no target for iframe found")
         return targets[0]
 
     async def wait_download(self, timeout: float or None = 30) -> dict:
         """
@@ -399,71 +418,77 @@
         return await doc.__isolated_exec_id__
 
     @property
     def pointer(self) -> Pointer:
         """the :class:`Pointer <selenium_driverless.input.pointer.Pointer>` for this target"""
         return self._pointer
 
-    async def send_keys(self, text: str):
+    async def send_keys(self, text: str, allow_not_on_mapping: bool = True):
         """
         send text & keys to the target
 
         :param text: the text to send to the target
+        :param allow_not_on_mapping: allow keys which aren't int the keyboard mapping
         """
         async with self._send_key_lock:
             for letter in text:
                 if letter in KEY_MAPPING:
                     key_code, virtual_key_code = KEY_MAPPING[letter]
-                    # Determine if a shift key is needed
-                    shift_pressed = False
-                    if letter.isupper() or letter in SHIFT_KEY_NEEDED:
-                        shift_pressed = True
-                        await self.execute_cdp_cmd("Input.dispatchKeyEvent", {
-                                "type": "keyDown",
-                                "code": "ShiftLeft",
-                                "windowsVirtualKeyCode": 16,
-                                "key": "Shift",
-                                "modifiers": 8 if shift_pressed else 0
-                        })
-                        await asyncio.sleep(random.uniform(0.05, 0.1))  # Simulate human typing speed
-
-                    key_event = {
-                            "type": "keyDown",
-                            "code": key_code,
-                            "windowsVirtualKeyCode": virtual_key_code,
-                            "key": letter,
-                            "modifiers": 8 if shift_pressed else 0
-                        }
-
-                    # Send keydown event
-                    await self.execute_cdp_cmd("Input.dispatchKeyEvent", key_event)
-                    await asyncio.sleep(random.uniform(0.05, 0.1))
-
-                    # Simulate key press for the actual character
-                    key_event["type"] = "char"
-                    key_event["text"] = letter
-                    await self.execute_cdp_cmd("Input.dispatchKeyEvent", key_event)
-                    await asyncio.sleep(random.uniform(0.05, 0.1))
-                    del key_event['text']
-
-                    # Simulate key release
-                    key_event["type"] = "keyUp"
-                    await self.execute_cdp_cmd("Input.dispatchKeyEvent", key_event)
-                    await asyncio.sleep(random.uniform(0.05, 0.1))
-
-                    # Release the shift key if it was pressed
-                    if shift_pressed:
-                        await self.execute_cdp_cmd("Input.dispatchKeyEvent", {
-                            "type": "keyUp",
-                            "code": "ShiftLeft",
-                            "windowsVirtualKeyCode": 16,
-                            "key": "Shift",
-                            "modifiers": 0
-                        })
-                        await asyncio.sleep(random.uniform(0.05, 0.1))  # Simulate human typing speed
+                elif allow_not_on_mapping:
+                    key_code, virtual_key_code = 0, 0
+                else:
+                    raise ValueError(f"letter:{letter} not in keyboard mapping")
+
+                # Determine if a shift key is needed
+                shift_pressed = False
+                if letter.isupper() or letter in SHIFT_KEY_NEEDED:
+                    shift_pressed = True
+                    await self.execute_cdp_cmd("Input.dispatchKeyEvent", {
+                        "type": "keyDown",
+                        "code": "ShiftLeft",
+                        "windowsVirtualKeyCode": 16,
+                        "key": "Shift",
+                        "modifiers": 8 if shift_pressed else 0
+                    })
+                await asyncio.sleep(random.uniform(0.01, 0.05))  # Simulate human typing speed
+
+                key_event = {
+                    "type": "keyDown",
+                    "code": key_code,
+                    "windowsVirtualKeyCode": virtual_key_code,
+                    "key": letter,
+                    "modifiers": 8 if shift_pressed else 0
+                }
+
+                # Send keydown event
+                await self.execute_cdp_cmd("Input.dispatchKeyEvent", key_event)
+                await asyncio.sleep(random.uniform(0.01, 0.05))
+
+                # Simulate key press for the actual character
+                key_event["type"] = "char"
+                key_event["text"] = letter
+                await self.execute_cdp_cmd("Input.dispatchKeyEvent", key_event)
+                await asyncio.sleep(random.uniform(0.01, 0.05))
+                del key_event['text']
+
+                # Simulate key release
+                key_event["type"] = "keyUp"
+                await self.execute_cdp_cmd("Input.dispatchKeyEvent", key_event)
+                await asyncio.sleep(random.uniform(0.01, 0.05))
+
+                # Release the shift key if it was pressed
+                if shift_pressed:
+                    await self.execute_cdp_cmd("Input.dispatchKeyEvent", {
+                        "type": "keyUp",
+                        "code": "ShiftLeft",
+                        "windowsVirtualKeyCode": 16,
+                        "key": "Shift",
+                        "modifiers": 0
+                    })
+                    await asyncio.sleep(random.uniform(0.01, 0.05))  # Simulate human typing speed
 
     async def execute_raw_script(self, script: str, *args, await_res: bool = False, serialization: str = None,
                                  max_depth: int = None, timeout: float = 2, execution_context_id: str = None,
                                  unique_context: bool = False):
         """executes a JavaScript on ``GlobalThis`` such as
 
         .. code-block:: js
@@ -653,23 +678,50 @@
             if e.code == -32000 and e.message == 'Command can only be executed on top-level targets':
                 pass
             else:
                 raise e
         except (asyncio.TimeoutError, TimeoutError):
             pass
 
-    async def focus(self):
-        await self.execute_cdp_cmd("Target.activateTarget",
-                                   {"targetId": self.id})
+    async def focus(self, activate=False):
+        """
+        emulates Focus of the target
+
+        :param activate: whether to bring the window to the front
+        """
+        if activate:
+            await self.activate()
         try:
             await self.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": True})
         except CDPError as e:
             if not (e.code == -32601 and e.message == "'Emulation.setFocusEmulationEnabled' wasn't found"):
                 raise e
 
+    async def unfocus(self):
+        """
+        disables focus emulation for the target
+        """
+        try:
+            await self.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": False})
+        except CDPError as e:
+            if e.code == -32601 and e.message == "'Target.activateTarget' wasn't found":
+                return False
+            raise e
+
+    async def activate(self):
+        """
+        brings the window to the front
+        """
+        try:
+            await self.execute_cdp_cmd("Target.activateTarget", {"targetId": self.id})
+        except CDPError as e:
+            if e.code == -32601 and e.message == "'Target.activateTarget' wasn't found":
+                return False
+            raise e
+
     @property
     async def info(self):
         res = await self.execute_cdp_cmd("Target.getTargetInfo", {"targetId": self.id})
         return await TargetInfo(res["targetInfo"], self)
 
     @property
     async def frame_tree(self):
@@ -878,43 +930,29 @@
                                             frame_id=None)
             else:
                 elem = await WebElement(target=self, node_id=node_id, loop=self._loop, isolated_exec_id=None,
                                         frame_id=None)
             elems.append(elem)
         return elems
 
-    async def get_screenshot_as_file(self, filename) -> bool:
+    async def get_screenshot_as_file(self, filename:str) -> None:
         # noinspection GrazieInspection
         """Saves a screenshot of the current window to a PNG image file.
-                Returns False if there is any IOError, else returns True. Use full
-                paths in your filename.
-
-                :Args:
-                 - filename: The full path you wish to save your screenshot to. This
-                   should end with a `.png` extension.
 
-                :Usage:
-                    ::
-
-                        target.get_screenshot_as_file('/Screenshots/foo.png')
-                """
+        :param filename: The full path.
+            This should end with a `.png` extension.
+        """
         if not str(filename).lower().endswith(".png"):
             warnings.warn(
                 "name used for saved screenshot does not match file " "type. It should end with a `.png` extension",
                 UserWarning,
             )
         png = await self.get_screenshot_as_png()
-        try:
-            async with aiofiles.open(filename, "wb") as f:
-                await f.write(png)
-        except OSError:
-            return False
-        finally:
-            del png
-        return True
+        async with aiofiles.open(filename, "wb") as f:
+            await f.write(png)
 
     async def save_screenshot(self, filename) -> bool:
         # noinspection GrazieInspection
         """Saves a screenshot of the current window to a PNG image file.
                 Returns False if there is any IOError, else returns True. Use full
                 paths in your filename.
 
@@ -927,34 +965,43 @@
 
                         target.save_screenshot('/Screenshots/foo.png')
                 """
         return await self.get_screenshot_as_file(filename)
 
     async def get_screenshot_as_png(self) -> bytes:
         """Gets the screenshot of the current window as a binary data.
+        """
+        res = await self.execute_cdp_cmd("Page.captureScreenshot", {"format": "png"}, timeout=30)
+        return b64decode(res["data"].encode("ascii"))
 
-        :Usage:
-            ::
+    async def snapshot(self) -> str:
+        """gets the current snapshot as mhtml"""
+        res = await self.execute_cdp_cmd("Page.captureSnapshot")
+        return res["data"]
 
-                target.get_screenshot_as_png()
-        """
-        base_64 = await self.get_screenshot_as_base64()
-        return b64decode(base_64.encode("ascii"))
+    async def save_snapshot(self, filename:str):
+        """Saves a snapshot of the current window to a MHTML file.
 
-    async def get_screenshot_as_base64(self) -> str:
-        """Gets the screenshot of the current window as a base64 encoded string
-        which is useful in embedded images in HTML.
+        :param filename: The full path you wish to save your snapshot to. This
+                   should end with a ``.mhtml`` extension.
 
-        :Usage:
-            ::
+        .. code-block:: Python
+
+            await driver.get_snapshot('snapshot.mhtml')
 
-                target.get_screenshot_as_base64()
         """
-        res = await self.execute_cdp_cmd("Page.captureScreenshot", {"format": "png"}, timeout=30)
-        return res["data"]
+
+        if len(filename) <= 6 or filename[-6:] != ".mhtml":
+            warnings.warn(
+                "name used for saved snapshot does not match file " "type. It should end with a `.mhtml` extension",
+                UserWarning,
+            )
+        mhtml = await self.snapshot()
+        async with aiofiles.open(filename, "w") as f:
+            await f.write(mhtml)
 
     async def get_network_conditions(self):
         """Gets Chromium network emulation settings.
 
         :Returns:
             A dict. For example:
             {'latency': 4, 'download_throughput': 2, 'upload_throughput': 2,
@@ -1312,24 +1359,22 @@
          - sink_name: Name of the sink to use as the target.
         """
         return await self.execute_cdp_cmd("Cast.startDesktopMirrorin", {"sinkName": sink_name})
 
     async def start_tab_mirroring(self, sink_name: str) -> dict:
         """Starts a tab mirroring session on a specific receiver target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
         return await self.execute_cdp_cmd("Cast.startTabMirroring", {"sinkName": sink_name})
 
     async def stop_casting(self, sink_name: str) -> dict:
         """Stops the existing Cast session on a specific receiver target.
 
-        :Args:
-         - sink_name: Name of the sink to stop the Cast session.
+        :param sink_name: Name of the sink to stop the Cast session.
         """
         return await self.execute_cdp_cmd("Cast.stopCasting", {"sinkName": sink_name})
 
 
 class TargetInfo:
     """
     Info for a Target
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/types/webelement.py` & `selenium_driverless-1.9.1/src/selenium_driverless/types/webelement.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,17 @@
     async def obj_id(self) -> str:
         """**async** returns the `Runtime.RemoteObjectId <https://vanilla.aslushnikov.com/?Runtime.RemoteObjectId>`_ for the element
         """
         return await self.__obj_id_for_context__()
 
     @property
     async def context_id(self):
+        """
+        **async** the ``Runtime.ExecutionContextId``
+        """
         self._check_stale()
         if not self.___context_id__:
             await self.obj_id
         return self.__context_id__
 
     def _check_stale(self):
         if self._stale:
@@ -168,14 +171,18 @@
         if self.__obj_id__:
             return int(self.__obj_id__.split(".")[1])
         else:
             return self.___context_id__
 
     @property
     async def node_id(self):
+        """
+        **async**
+        the ``DOM.NodeId``
+        """
         self._check_stale()
         if not self._node_id:
             node = await self.__target__.execute_cdp_cmd("DOM.requestNode", {"objectId": await self.obj_id})
             self._node_id = node["nodeId"]
         return self._node_id
 
     @property
@@ -183,15 +190,15 @@
         if not self.___frame_id__:
             await self._describe()
         return self.___frame_id__
 
     @property
     async def content_document(self):
         """
-        gets the document of the iframe
+        **async** gets the document of the iframe
         """
         _desc = await self._describe()
         if _desc.get("localName") == "iframe":
             node = _desc.get("contentDocument")
             if node:
                 frame_id = _desc.get("frameId")
                 if node['documentURL'] == 'about:blank':
@@ -220,26 +227,32 @@
             # different target for cross-site
             targets = await self.__target__.get_targets_for_iframes([self])
             if targets:
                 return await targets[0]._document_elem
 
     @property
     async def document_url(self):
-        """gets the url if the element is an iframe, else returns ``None``"""
+        """**async** gets the url if the element is an iframe, else returns ``None``"""
         res = await self._describe()
         return res.get('documentURL')
 
     @property
     async def backend_node_id(self):
+        """
+        **async** the ``DOM.BackendNodeId``
+        """
         if not self._backend_node_id:
             await self._describe()
         return self._backend_node_id
 
     @property
     def class_name(self):
+        """
+        the ClassName of the element (if available)
+        """
         return self._class_name
 
     async def find_element(self, by: str, value: str, idx: int = 0, timeout: int or None = None):
         """find an element in the current target
 
         :param by: one of the locators at :func:`By <selenium_driverless.types.by.By>`
         :param value: the actual query to find the element by
@@ -252,15 +265,17 @@
             elems = await self.find_elements(by=by, value=value)
             if (not timeout) or (time.perf_counter() - start) > timeout:
                 break
         if elems:
             if isinstance(elems, list):
                 return elems[idx]
             else:
-                raise Exception("find_elements returned not a list. This possibly is related to https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/84\n", elems)
+                raise Exception(
+                    "find_elements returned not a list. This possibly is related to https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/84\n",
+                    elems)
         raise NoSuchElementException()
 
     async def find_elements(self, by: str = By.ID, value: str or None = None):
         """find multiple elements in the current target
 
         :param by: one of the locators at :func:`By <selenium_driverless.types.by.By>`
         :param value: the actual query to find the elements by
@@ -329,14 +344,16 @@
             else:
                 raise e
         return res["outerHTML"]
 
     async def set_source(self, value: str):
         """
         sets the OuterHTML of the element
+
+        :param value: the str to set the outerHtml to
         """
         try:
             await self.__target__.execute_cdp_cmd("DOM.setOuterHTML",
                                                   {"nodeId": await self.node_id, "outerHTML": value})
         except CDPError as e:
             if e.code == -32000 and 'Could not find node with given id' in e.message:
                 raise StaleElementReferenceException(self)
@@ -344,15 +361,15 @@
                 raise e
 
     async def get_property(self, name: str) -> str or None:
         """Gets the given property of the element.
 
         :param name: the name of the property to get
 
-        .. warning::
+        .. note::
             this gets the JavaScript property (``elem[name]``), and not HTML property
         """
         return await self.execute_script(f"return obj[arguments[0]]", name)
 
     @property
     async def tag_name(self) -> str:
         """This element's ``tagName`` property."""
@@ -435,15 +452,17 @@
             for listener in listeners:
                 _type = listener["type"]
                 if _type in ["click", "mousedown", "mouseup"]:
                     is_clickable = True
                     break
         return is_clickable
 
-    async def click(self, timeout: float = None, visible_timeout: float = 30,spread_a: float = 1, spread_b: float = 1, bias_a: float = 0.5, bias_b: float = 0.5, border:float=0.05, scroll_to=True, move_to: bool = True,
+    async def click(self, timeout: float = None, visible_timeout: float = 30, spread_a: float = 1, spread_b: float = 1,
+                    bias_a: float = 0.5, bias_b: float = 0.5, border: float = 0.05, scroll_to=True,
+                    move_to: bool = True,
                     ensure_clickable: typing.Union[bool, int] = False) -> None:
         """Clicks the element.
 
         :param timeout: the time in seconds to take for clicking on the element
         :param visible_timeout: the time in seconds to wait for being able to compute the elements box model
         :param spread_a: spread over a
         :param spread_b: spread over b
@@ -478,15 +497,15 @@
         if ensure_clickable:
             is_clickable = await self.is_clickable()
             if not is_clickable:
                 raise ElementNotClickable(x, y)
 
         await self.__target__.pointer.click(x, y=y, click_kwargs={"timeout": timeout}, move_to=move_to)
 
-    async def write(self, text: str,click_kwargs=None, click_on:bool=True):
+    async def write(self, text: str, click_kwargs=None, click_on: bool = True):
         """
         inserts literal text to the element
 
         .. warning::
 
             This method is generally detectable.
             You might consider using :func:`Elem.send_keys <selenium_driverless.types.webelement.WebElement.send_keys>` instead.
@@ -517,15 +536,15 @@
 
         :param paths: the absolute paths to the files
         """
         args = {"files": paths}
         args.update(self._args_builder)
         await self.__target__.execute_cdp_cmd("DOM.setFileInputFiles", args)
 
-    async def send_keys(self, text: str, click_kwargs:dict=None, click_on:bool=True) -> None:
+    async def send_keys(self, text: str, click_kwargs: dict = None, click_on: bool = True) -> None:
         """
         send text & keys to the target
 
         :param text: the text to send to the target
         :param click_kwargs: arguments to pass for :func:`Elem.send_keys <selenium_driverless.types.webelement.WebElement.send_keys>`
         :param click_on: whether to click on the element before sending the keys
         """
@@ -533,15 +552,16 @@
             click_kwargs = {}
         if click_on:
             await self.click(**click_kwargs)
         else:
             await self.focus()
         await self.__target__.send_keys(text)
 
-    async def mid_location(self, spread_a: float = 1, spread_b: float = 1, bias_a: float = 0.5, bias_b: float = 0.5, border:float=0.05) -> typing.List[int]:
+    async def mid_location(self, spread_a: float = 1, spread_b: float = 1, bias_a: float = 0.5, bias_b: float = 0.5,
+                           border: float = 0.05) -> typing.List[int]:
         """
         returns random location in the element with probability close to the middle
 
         :param spread_a: spread over a
         :param spread_b: spread over b
         :param bias_a: bias over a (0-1)
         :param bias_b: bias over b (0-1)
@@ -580,14 +600,23 @@
             "e.initEvent('submit', true, true);\n"
             "if (form.dispatchEvent(e)) { HTMLFormElement.prototype.submit.call(form) }\n"
         )
         return await self.execute_script(script, unique_context=True)
 
     @property
     async def dom_attributes(self) -> dict:
+        """returns the dom attributes as a dict
+
+        .. warning::
+
+            this isn't implemented properly yet and might change,
+            use :func:`WebElement.execute_script <selenium_driverless.types.webelement.WelElement.execute_script`
+            instead
+
+        """
         try:
             res = await self.__target__.execute_cdp_cmd("DOM.getAttributes", {"nodeId": await self.node_id})
             attr_list = res["attributes"]
             attributes_dict = defaultdict(lambda: None)
 
             for i in range(0, len(attr_list), 2):
                 key = attr_list[i]
@@ -595,38 +624,47 @@
                 attributes_dict[key] = value
             return attributes_dict
         except CDPError as e:
             if not (e.code == -32000 and 'Node is not an Element' in e.message):
                 raise e
 
     async def get_dom_attribute(self, name: str) -> str or None:
-        """Gets the given attribute of the element. Unlike
-        :func:`~selenium.webdriver.remote.BaseWebElement.get_attribute`, this
-        method only returns attributes declared in the element's HTML markup.
+        """Gets the given attribute of the element.
+        Only returns attributes declared in the element's HTML markup.
+
+        :param name: Name of the attribute to retrieve.
 
-        :Args:
-            - name - Name of the attribute to retrieve.
+        .. warning::
 
-        :Usage:
-            ::
+            this isn't implemented properly yet and might change,
+            use :func:`WebElement.execute_script <selenium_driverless.types.webelement.WelElement.execute_script`
+            instead
 
-                text_length = target_element.get_dom_attribute("class")
         """
         attrs = await self.dom_attributes
         return attrs[name]
 
     async def set_dom_attribute(self, name: str, value: str):
+        """set a dom_attribute
+
+        :param name: the name of the DOM (=>html) attribute
+        :param value: the value to set the attribute to
+        """
         await self.__target__.execute_cdp_cmd("DOM.setAttributeValue", {"nodeId": await self.node_id,
                                                                         "name": name, "value": value})
 
     async def get_attribute(self, name):
         """Alias to WebElement.get_property.
 
         .. warning::
-            do not use! This method might change in future
+
+            this isn't implemented properly yet and might change,
+            use :func:`WebElement.execute_script <selenium_driverless.types.webelement.WelElement.execute_script`
+            instead
+
         """
         return await self.get_property(name)
 
     async def is_selected(self) -> bool:
         """Returns whether the element is selected.
 
         Can be used to check if a checkbox or radio button is selected.
@@ -661,15 +699,14 @@
             return not (size["height"] == 0 or size["width"] == 0)
         except CDPError as e:
             if e.code == -32000 and 'Could not compute box model.' in e.message:
                 return False
             else:
                 raise e
 
-
     @property
     async def location_once_scrolled_into_view(self) -> dict:
         """
         scrolls to the element and returns the coordinates of it
         """
         await self.scroll_to()
         result = await self.rect
@@ -717,15 +754,15 @@
         """A dictionary with the size and location of the element."""
         # todo: calculate form DOM.getBoxModel
         result = await self.execute_script("return obj.getClientRects()[0].toJSON()", serialization="json",
                                            unique_context=True)
         return result
 
     @property
-    async def css_metrics(self):
+    async def css_metrics(self) -> typing.List[dict, float]:
         script = """
             function getRotationAngle(target) 
                 {
                   const _obj = window.getComputedStyle(target, null);
                   const matrix = _obj.getPropertyValue('transform');
                   let angle = 0; 
                   if (matrix !== 'none') 
@@ -827,15 +864,15 @@
             return False
         finally:
             del png
         return True
 
     @property
     async def parent(self) -> WebElement:
-        """The parent element this element"""
+        """**async** The parent element this element"""
         args = {}
         if self._node_id:
             args["nodeId"] = self._node_id
         else:
             args["objectId"] = await self.obj_id
         node: dict = await self._describe()
         node_id = node.get("parentId")
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.9.1/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.9.1/src/selenium_driverless/webdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1098,19 +1098,30 @@
         return await self.get_screenshot_as_file(filename)
 
     async def get_screenshot_as_png(self) -> bytes:
         """Gets the screenshot of the current tab as a binary data.
         """
         return await self.current_target.get_screenshot_as_png()
 
-    async def get_screenshot_as_base64(self) -> str:
-        """Gets the screenshot of the current tab as a base64 encoded string
-        which is useful in embedded images in HTML.
+    async def snapshot(self) -> str:
+        """gets the current snapshot as mhtml"""
+        return await self.current_target.snapshot()
+
+    async def save_snapshot(self, filename: str):
+        """Saves a snapshot of the current window to a MHTML file.
+
+        :param filename: The full path you wish to save your snapshot to. This
+                   should end with a ``.mhtml`` extension.
+
+        .. code-block:: Python
+
+            await driver.get_snapshot('snapshot.mhtml')
+
         """
-        return await self.current_target.get_screenshot_as_base64()
+        return await self.current_target.save_snapshot(filename)
 
     # noinspection PyPep8Naming
     async def set_window_size(self, width: int, height: int) -> None:
         """Sets the width and height of the window, the current tab is within (unless ``windowHandle`` specified)
 
         :param width: the width in pixels to set the window to
         :param height: the height in pixels to set the window to
@@ -1504,41 +1515,35 @@
     async def get_issue_message(self, target_id: str = None):
         """
         :Returns: An error message when there is any issue in a Cast session.
         """
         target = await self.get_target(target_id=target_id)
         return await target.get_issue_message()
 
-    async def set_sink_to_use(self, sink_name: str, target_id: str = None) -> dict:
+    async def set_sink_to_use(self, sink_name: str) -> dict:
         """Sets a specific sink, using its name, as a Cast session receiver
         target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.set_sink_to_use(sink_name=sink_name)
+        return await self.current_target.set_sink_to_use(sink_name=sink_name)
 
-    async def start_desktop_mirroring(self, sink_name: str, target_id: str = None) -> dict:
+    async def start_desktop_mirroring(self, sink_name: str) -> dict:
         """Starts a desktop mirroring session on a specific receiver target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.start_desktop_mirroring(sink_name=sink_name)
+        return await self.current_target.start_desktop_mirroring(sink_name=sink_name)
 
-    async def start_tab_mirroring(self, sink_name: str, target_id: str = None) -> dict:
+    async def start_tab_mirroring(self, sink_name: str) -> dict:
         """Starts a tab mirroring session on a specific receiver target.
 
-        :Args:
-         - sink_name: Name of the sink to use as the target.
+        :param sink_name: Name of the sink to use as the target.
         """
-        target = await self.get_target(target_id=target_id)
-        return await target.start_tab_mirroring(sink_name=sink_name)
+        return await self.current_target.start_tab_mirroring(sink_name=sink_name)
 
     async def stop_casting(self, sink_name: str, target_id: str = None) -> dict:
         """Stops the existing Cast session on a specific receiver target.
 
         :Args:
          - sink_name: Name of the sink to stop the Cast session.
         """
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.9.1/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.9
+Version: 1.9.1
 Summary: Undetected selenium without chromedriver usage (Non-commercial use only!)
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 License: CC BY-NC-SA 4.0
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
@@ -43,15 +43,15 @@
 
 
 - Use Selenium __without chromedriver__
 - Currently passes __Cloudflare__, __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/master/dev#bypass-turnstile), and others
 - Multiple tabs simultaneously
 - Multiple Incognito-contexts with isolated cookies & local storage
 - Proxy-auth support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/blob/dev/examples/proxy_with_auth.py))
-- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/RequestInterception/))
+- Network-interception ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/RequestInterception/))
 - Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/#selenium_driverless.types.target.Target.fetch))
 
 ### Questions? 
 Feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord**:)
 
 Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
 <details>
@@ -128,14 +128,18 @@
 asyncio.run(main())
 
 ```
 
 ### synchronous
 asyncified, might be buggy
 
+<details>
+
+<summary>example code</summary>
+
 ```python
 from selenium_driverless.sync import webdriver
 
 options = webdriver.ChromeOptions()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.sleep(0.5)
@@ -143,14 +147,16 @@
 
     title = driver.title
     url = driver.current_url
     source = driver.page_source
     print(title)
 ```
 
+</details>
+
 ### custom debugger address
 ```python
 from selenium_driverless import webdriver
 
 options = webdriver.ChromeOptions()
 options.debugger_address = "127.0.0.1:2005"
 
@@ -199,16 +205,16 @@
 
 
 asyncio.run(main())
 ```
 
 </details>
 
-### Unique execution contexts
-- execute `javascript` without getting detected
+### Isolated execution contexts
+- execute `javascript` without getting detected ( in a **isolated world**)
 <details>
 <summary>Example Code (Click to expand)</summary>
 
 ```python
 from selenium_driverless.sync import webdriver
 from selenium_driverless import webdriver
 import asyncio
@@ -250,15 +256,14 @@
 pointer = driver.current_pointer
 move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
 
 await pointer.move_to(100, 500)
 await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
 ```
 ### Iframes
-- switch and interact with iframes
 
 ```python
 iframes = await driver.find_elements(By.TAG_NAME, "iframe")
 await asyncio.sleep(0.5)
 iframe_document = await iframes[0].content_document
 # iframe_document.find_elements(...)
 ```
@@ -320,48 +325,14 @@
 sys.modules["cdp_socket"].EXC_HANDLER = handler
 ```
 
 ## Help
 
 You found a bug? Feel free to open an issue:)
 You've got other questions or proposials? feel free to join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord** or open a discusion\
-Note: **please check the todo's below at first!**
-
-## Todo's
-<details>
-<summary>Click to expand</summary>
-
-- implementations
-  - [x] `WebElement`s
-    - [ ] improve `mid_location` calculation
-    - [ ] add `WebElement.screenshot`
-  - [x] `Input`
-      - [x] `Mouse`
-        - [x] `mousemove`
-        - [x] `click`
-        - [ ] `scroll`
-        - [ ] `drag&drop`
-      - [x] `write`
-      - [ ] `Touch`
-        - [ ] `touchmove`
-        - [ ] `TouchTap`
-        - [ ] `scoll`
-        - [ ] `pinch//zoom`
-      - [ ] `KeyBoard`
-        - [ ] `SendKeys`
-          - [ ] `send files`
-  - [ ] [support `options.add_extension()`](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues/37)
-  - [ ] [support prefs](https://github.com/kaliiiiiiiiii/Selenium-Driverless/discussions/92#discussioncomment-7462309)
-- [x] sync
-  - [ ] move sync to threaded for allowing event_handlers
-  - [ ] support multithreading with sync version
-    - [x] on independent driver instances
-    - [ ] on same driver instance
-- [ ] check [Python 3.12.0](https://www.python.org/downloads/release/python-3120/)
-</details>
 
 ## Authors
 
 Copyright and Author: \
 [Aurin Aegerter](mailto:aurinliun@gmx.ch) (aka **Steve**)
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selenium_driverless Version: 1.9 Summary:
+Metadata-Version: 2.1 Name: selenium_driverless Version: 1.9.1 Summary:
 Undetected selenium without chromedriver usage (Non-commercial use only!) Home-
 page: https://github.com/kaliiiiiiiiii/Selenium-Driverless Author: Aurin
 Aegerter Author-email: aurinliun@gmx.ch License: CC BY-NC-SA 4.0 Project-URL:
 Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless Project-
 URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Keywords: Selenium,webautomation Classifier: Development Status :: 2 - Pre-
@@ -25,120 +25,106 @@
 [Documentation](https://kaliiiiiiiiii.github.io/Selenium-Driverless/#) - Use
 Selenium __without chromedriver__ - Currently passes __Cloudflare__,
 __Bet365__, [Turnstile](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
 tree/master/dev#bypass-turnstile), and others - Multiple tabs simultaneously -
 Multiple Incognito-contexts with isolated cookies & local storage - Proxy-auth
 support ([example code](https://github.com/kaliiiiiiiiii/Selenium-Driverless/
 blob/dev/examples/proxy_with_auth.py)) - Network-interception ([documentation]
-(https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/Chrome/
-RequestInterception/)) - Single requests ([documentation](https://
-kaliiiiiiiiii.github.io/Selenium-Driverless/api/Target/
-#selenium_driverless.types.target.Target.fetch)) ### Questions? Feel free to
-join the [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on
-**Discord**:) Also, see [dev-branch](https://github.com/kaliiiiiiiiii/Selenium-
-Driverless/tree/dev) for the latest implementations. dev-installation (click to
-expand) ```shell pip uninstall -y selenium-driverless pip install https://
-github.com/kaliiiiiiiiii/Selenium-Driverless/archive/refs/heads/dev.zip ```
-#### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]### Dependencies * [Python >= 3.7]
-(https://www.python.org/downloads/) * [Google-Chrome](https://www.google.de/
-chrome/) installed (Chromium not tested) ### Installing * Install [Google-
-Chrome](https://www.google.de/chrome/) * ```pip install selenium-driverless```
-### Usage ### with asyncio ```python from selenium_driverless import webdriver
-from selenium_driverless.types.by import By import asyncio async def main():
-options = webdriver.ChromeOptions() async with webdriver.Chrome
-(options=options) as driver: await driver.get('http://nowsecure.nl#relax',
-wait_load=True) await driver.sleep(0.5) await driver.wait_for_cdp
-("Page.domContentEventFired", timeout=15) # wait 10s for elem to exist elem =
-await driver.find_element(By.XPATH, '/html/body/div[2]/div/main/p[2]/a',
-timeout=10) await elem.click(move_to=True) alert = await driver.switch_to.alert
-print(alert.text) await alert.accept() print(await driver.title) asyncio.run
-(main()) ``` ### synchronous asyncified, might be buggy ```python from
-selenium_driverless.sync import webdriver options = webdriver.ChromeOptions()
-with webdriver.Chrome(options=options) as driver: driver.get('http://
-nowsecure.nl#relax') driver.sleep(0.5) driver.wait_for_cdp
-("Page.domContentEventFired", timeout=15) title = driver.title url =
-driver.current_url source = driver.page_source print(title) ``` ### custom
-debugger address ```python from selenium_driverless import webdriver options =
-webdriver.ChromeOptions() options.debugger_address = "127.0.0.1:2005" # specify
-if you don't want to run remote # options.add_argument("--remote-debugging-
-port=2005") async with webdriver.Chrome(options=options) as driver: await
-driver.get('http://nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs
-simultaneously Note: asyncio is recommended, threading only works on
-independent webdriver.Chrome instances. Example Code (Click to expand)
-```python from selenium_driverless.sync import webdriver from
-selenium_driverless.utils.utils import read from selenium_driverless import
-webdriver import asyncio async def target_1_handler(target): await target.get
-('https://abrahamjuliot.github.io/creepjs/') print(await target.title) async
-def target_2_handler(target): await target.get("about:blank") await
-target.execute_script(script=read("/files/js/show_mousemove.js")) await
-target.pointer.move_to(500, 500, total_time=2) async def main(): options =
-webdriver.ChromeOptions() async with webdriver.Chrome(options=options) as
-driver: target_1 = await driver.current_target target_2 = await
-driver.new_window("tab", activate=False) await asyncio.gather( target_1_handler
-(target_1), target_2_handler(target_2) ) await target_1.focus() input("press
-ENTER to exit") asyncio.run(main()) ``` ### Unique execution contexts - execute
-`javascript` without getting detected Example Code (Click to expand) ```python
-from selenium_driverless.sync import webdriver from selenium_driverless import
-webdriver import asyncio async def main(): options = webdriver.ChromeOptions()
-async with webdriver.Chrome(options=options) as driver: await driver.get
-('chrome://version') script = """ const proxy = new Proxy
-(document.documentElement, { get(target, prop, receiver) { if(prop ===
-"outerHTML"){ console.log('detected access on "'+prop+'"', receiver) return
-"mocked value:)" } else{return Reflect.get(...arguments)} }, });
-Object.defineProperty(document, "documentElement", { value: proxy }) """ await
-driver.execute_script(script) src = await driver.execute_script("return
+(https://kaliiiiiiiiii.github.io/Selenium-Driverless/api/RequestInterception/))
+- Single requests ([documentation](https://kaliiiiiiiiii.github.io/Selenium-
+Driverless/api/Target/#selenium_driverless.types.target.Target.fetch)) ###
+Questions? Feel free to join the [Driverless-Community](https://discord.com/
+invite/MzZZjr2ZM3) on **Discord**:) Also, see [dev-branch](https://github.com/
+kaliiiiiiiiii/Selenium-Driverless/tree/dev) for the latest implementations.
+dev-installation (click to expand) ```shell pip uninstall -y selenium-
+driverless pip install https://github.com/kaliiiiiiiiii/Selenium-Driverless/
+archive/refs/heads/dev.zip ``` #### Also, feel free to _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]###
+Dependencies * [Python >= 3.7](https://www.python.org/downloads/) * [Google-
+Chrome](https://www.google.de/chrome/) installed (Chromium not tested) ###
+Installing * Install [Google-Chrome](https://www.google.de/chrome/) * ```pip
+install selenium-driverless``` ### Usage ### with asyncio ```python from
+selenium_driverless import webdriver from selenium_driverless.types.by import
+By import asyncio async def main(): options = webdriver.ChromeOptions() async
+with webdriver.Chrome(options=options) as driver: await driver.get('http://
+nowsecure.nl#relax', wait_load=True) await driver.sleep(0.5) await
+driver.wait_for_cdp("Page.domContentEventFired", timeout=15) # wait 10s for
+elem to exist elem = await driver.find_element(By.XPATH, '/html/body/div[2]/
+div/main/p[2]/a', timeout=10) await elem.click(move_to=True) alert = await
+driver.switch_to.alert print(alert.text) await alert.accept() print(await
+driver.title) asyncio.run(main()) ``` ### synchronous asyncified, might be
+buggy example code ```python from selenium_driverless.sync import webdriver
+options = webdriver.ChromeOptions() with webdriver.Chrome(options=options) as
+driver: driver.get('http://nowsecure.nl#relax') driver.sleep(0.5)
+driver.wait_for_cdp("Page.domContentEventFired", timeout=15) title =
+driver.title url = driver.current_url source = driver.page_source print(title)
+``` ### custom debugger address ```python from selenium_driverless import
+webdriver options = webdriver.ChromeOptions() options.debugger_address =
+"127.0.0.1:2005" # specify if you don't want to run remote #
+options.add_argument("--remote-debugging-port=2005") async with
+webdriver.Chrome(options=options) as driver: await driver.get('http://
+nowsecure.nl#relax', wait_load=True) ``` ## Multiple tabs simultaneously Note:
+asyncio is recommended, threading only works on independent webdriver.Chrome
+instances. Example Code (Click to expand) ```python from
+selenium_driverless.sync import webdriver from selenium_driverless.utils.utils
+import read from selenium_driverless import webdriver import asyncio async def
+target_1_handler(target): await target.get('https://abrahamjuliot.github.io/
+creepjs/') print(await target.title) async def target_2_handler(target): await
+target.get("about:blank") await target.execute_script(script=read("/files/js/
+show_mousemove.js")) await target.pointer.move_to(500, 500, total_time=2) async
+def main(): options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: target_1 = await driver.current_target target_2 =
+await driver.new_window("tab", activate=False) await asyncio.gather
+( target_1_handler(target_1), target_2_handler(target_2) ) await target_1.focus
+() input("press ENTER to exit") asyncio.run(main()) ``` ### Isolated execution
+contexts - execute `javascript` without getting detected ( in a **isolated
+world**) Example Code (Click to expand) ```python from selenium_driverless.sync
+import webdriver from selenium_driverless import webdriver import asyncio async
+def main(): options = webdriver.ChromeOptions() async with webdriver.Chrome
+(options=options) as driver: await driver.get('chrome://version') script = """
+const proxy = new Proxy(document.documentElement, { get(target, prop, receiver)
+{ if(prop === "outerHTML"){ console.log('detected access on "'+prop+'"',
+receiver) return "mocked value:)" } else{return Reflect.get(...arguments)} },
+}); Object.defineProperty(document, "documentElement", { value: proxy }) """
+await driver.execute_script(script) src = await driver.execute_script("return
 document.documentElement.outerHTML", unique_context=True) mocked = await
 driver.execute_script("return document.documentElement.outerHTML",
 unique_context=False) print(src, mocked) asyncio.run(main()) ``` ### Pointer
 Interaction see [@master/dev/show_mousemove.py](https://github.com/
 kaliiiiiiiiii/Selenium-Driverless/blob/master/dev/show_mousemove.py) for
 visualization ```python pointer = driver.current_pointer move_kwargs =
 {"total_time": 0.7, "accel": 2, "smooth_soft": 20} await pointer.move_to(100,
 500) await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True) ```
-### Iframes - switch and interact with iframes ```python iframes = await
-driver.find_elements(By.TAG_NAME, "iframe") await asyncio.sleep(0.5)
-iframe_document = await iframes[0].content_document #
-iframe_document.find_elements(...) ``` ### use preferences ```python from
-selenium_driverless import webdriver options = webdriver.ChromeOptions() #
-recommended usage options.update_pref("download.prompt_for_download", False) #
-or options.prefs.update({"download": {"prompt_for_download": False}}) #
-supported options.add_experimental_option("prefs",
-{"download.prompt_for_download": False}) ``` ### Multiple Contexts - different
-cookies for each context - A context can have multiple windows and tabs within
-- different proxy for each context - opens as a window as incognito Example
-Code (Click to expand) ```python from selenium_driverless import webdriver
-import asyncio async def main(): options = webdriver.ChromeOptions() async with
-webdriver.Chrome(options=options) as driver: context_1 = driver.current_context
-await driver.set_auth("username", "password", "localhost:5000") # proxy not
-supported on windows due to https://bugs.chromium.org/p/chromium/issues/
-detail?id=1310057 context_2 = await driver.new_context(proxy_bypass_list=
-["localhost"], proxy_server="http://localhost:5000") await
-context_1.current_target.get("https://examle.com") await context_2.get("https:/
-/examle.com") input("press ENTER to exit:)") asyncio.run(main()) ``` ####
-Custom exception handling You can implement custom exception handling as
-following ```python import selenium_driverless import sys handler = (lambda e:
-print(f'Exception in event-handler:\n{e.__class__.__module__}.
+### Iframes ```python iframes = await driver.find_elements(By.TAG_NAME,
+"iframe") await asyncio.sleep(0.5) iframe_document = await iframes
+[0].content_document # iframe_document.find_elements(...) ``` ### use
+preferences ```python from selenium_driverless import webdriver options =
+webdriver.ChromeOptions() # recommended usage options.update_pref
+("download.prompt_for_download", False) # or options.prefs.update({"download":
+{"prompt_for_download": False}}) # supported options.add_experimental_option
+("prefs", {"download.prompt_for_download": False}) ``` ### Multiple Contexts -
+different cookies for each context - A context can have multiple windows and
+tabs within - different proxy for each context - opens as a window as incognito
+Example Code (Click to expand) ```python from selenium_driverless import
+webdriver import asyncio async def main(): options = webdriver.ChromeOptions()
+async with webdriver.Chrome(options=options) as driver: context_1 =
+driver.current_context await driver.set_auth("username", "password",
+"localhost:5000") # proxy not supported on windows due to https://
+bugs.chromium.org/p/chromium/issues/detail?id=1310057 context_2 = await
+driver.new_context(proxy_bypass_list=["localhost"], proxy_server="http://
+localhost:5000") await context_1.current_target.get("https://examle.com") await
+context_2.get("https://examle.com") input("press ENTER to exit:)") asyncio.run
+(main()) ``` #### Custom exception handling You can implement custom exception
+handling as following ```python import selenium_driverless import sys handler =
+(lambda e: print(f'Exception in event-handler:\n{e.__class__.__module__}.
 {e.__class__.__name__}: {e}', file=sys.stderr)) sys.modules
 ["selenium_driverless"].EXC_HANDLER = handler sys.modules
 ["cdp_socket"].EXC_HANDLER = handler ``` ## Help You found a bug? Feel free to
 open an issue:) You've got other questions or proposials? feel free to join the
 [Driverless-Community](https://discord.com/invite/MzZZjr2ZM3) on **Discord** or
-open a discusion\ Note: **please check the todo's below at first!** ## Todo's
-Click to expand - implementations - [x] `WebElement`s - [ ] improve
-`mid_location` calculation - [ ] add `WebElement.screenshot` - [x] `Input` -
-[x] `Mouse` - [x] `mousemove` - [x] `click` - [ ] `scroll` - [ ] `drag&drop` -
-[x] `write` - [ ] `Touch` - [ ] `touchmove` - [ ] `TouchTap` - [ ] `scoll` -
-[ ] `pinch//zoom` - [ ] `KeyBoard` - [ ] `SendKeys` - [ ] `send files` - [ ]
-[support `options.add_extension()`](https://github.com/kaliiiiiiiiii/Selenium-
-Driverless/issues/37) - [ ] [support prefs](https://github.com/kaliiiiiiiiii/
-Selenium-Driverless/discussions/92#discussioncomment-7462309) - [x] sync - [ ]
-move sync to threaded for allowing event_handlers - [ ] support multithreading
-with sync version - [x] on independent driver instances - [ ] on same driver
-instance - [ ] check [Python 3.12.0](https://www.python.org/downloads/release/
-python-3120/) ## Authors Copyright and Author: \ [Aurin Aegerter](mailto:
+open a discusion\ ## Authors Copyright and Author: \ [Aurin Aegerter](mailto:
 aurinliun@gmx.ch) (aka **Steve**) ## License Shield: [![CC BY-NC-SA 4.0][cc-by-
 nc-sa-shield]][cc-by-nc-sa] Unless specified differently in a single file, this
 work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike
 4.0 International License][cc-by-nc-sa]. [![CC BY-NC-SA 4.0][cc-by-nc-sa-
 image]][cc-by-nc-sa] [cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-
 sa/4.0/ [cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/
 88x31.png [cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--
```

### Comparing `selenium_driverless-1.9/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.9.1/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/tests/bypass_turnstile.py` & `selenium_driverless-1.9.1/tests/bypass_turnstile.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/tests/selenium_detector/selenium_detector.py` & `selenium_driverless-1.9.1/tests/selenium_detector/selenium_detector.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/tests/selenium_detector/sync_selenium_detector.py` & `selenium_driverless-1.9.1/tests/selenium_detector/sync_selenium_detector.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/tests/show_mousemove.py` & `selenium_driverless-1.9.1/tests/show_mousemove.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     async with webdriver.Chrome(options=options) as driver:
         await driver.get("about:blank")
         await driver.execute_script(script=await read("/files/js/show_mousemove.js", sel_root=True))
         elem = await driver.find_element(By.ID, "clear")
         pointer = driver.current_pointer
 
         move_kwargs = {"total_time": 0.7, "accel": 2, "smooth_soft": 20}
-        await driver.execute_cdp_cmd("Emulation.setFocusEmulationEnabled", {"enabled": True})
+        await driver.current_target.activate()
 
         for _ in range(50):
             await pointer.click(100, 500, move_kwargs=move_kwargs, move_to=True)
             await asyncio.sleep(0)
             await pointer.click(500, 50, move_kwargs=move_kwargs, move_to=True)
             await asyncio.sleep(0)
         input("Press ENTER to exit")
```

### Comparing `selenium_driverless-1.9/tests/target_interception.py` & `selenium_driverless-1.9.1/tests/target_interception.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/tests/test_driverless.py` & `selenium_driverless-1.9.1/tests/test_driverless.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.9/tests/turnstile_captcha.png` & `selenium_driverless-1.9.1/tests/turnstile_captcha.png`

 * *Files identical despite different names*

