# Comparing `tmp/wagtail_editorjs-1.5.9.tar.gz` & `tmp/wagtail_editorjs-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_editorjs-1.5.9.tar", last modified: Sun Mar 31 07:09:38 2024, max compression
+gzip compressed data, was "wagtail_editorjs-1.6.0.tar", last modified: Fri Apr 19 16:16:26 2024, max compression
```

## Comparing `wagtail_editorjs-1.5.9.tar` & `wagtail_editorjs-1.6.0.tar`

### file list

```diff
@@ -1,120 +1,138 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.277532 wagtail_editorjs-1.5.9/
--rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.5.9/LICENSE
--rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4105 2024-03-31 07:09:38.277532 wagtail_editorjs-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     2848 2024-03-26 17:25:53.000000 wagtail_editorjs-1.5.9/README.md
--rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.5.9/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-03-31 07:09:38.287534 wagtail_editorjs-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.281660 wagtail_editorjs-1.5.9/wagtail_editorjs/
--rw-rw-rw-   0        0        0      312 2024-03-31 07:09:33.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/__init__.py
--rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/apps.py
--rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/blocks.py
--rw-rw-rw-   0        0        0     3021 2024-03-30 00:54:09.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/django_editor.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.364121 wagtail_editorjs-1.5.9/wagtail_editorjs/features/
--rw-rw-rw-   0        0        0      568 2024-03-28 18:26:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/__init__.py
--rw-rw-rw-   0        0        0     7723 2024-03-27 20:40:30.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/blocks.py
--rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/documents.py
--rw-rw-rw-   0        0        0     9758 2024-03-31 07:05:53.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/images.py
--rw-rw-rw-   0        0        0     4776 2024-03-31 07:03:23.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/inlines.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/lists.py
--rw-rw-rw-   0        0        0     4005 2024-03-29 14:43:50.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/features/tunes.py
--rw-rw-rw-   0        0        0     1733 2024-03-31 07:02:15.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/fields.py
--rw-rw-rw-   0        0        0     5444 2024-03-28 09:47:04.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/forms.py
--rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/hooks.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.365194 wagtail_editorjs-1.5.9/wagtail_editorjs/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.366789 wagtail_editorjs-1.5.9/wagtail_editorjs/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.390036 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/
--rw-rw-rw-   0        0        0      879 2024-03-29 10:32:11.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.421947 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/
--rw-rw-rw-   0        0        0      229 2024-03-29 10:32:13.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/__init__.py
--rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/attrs.py
--rw-rw-rw-   0        0        0     3494 2024-03-29 14:48:28.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/element.py
--rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/utils.py
--rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/feature_registry.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.457833 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/
--rw-rw-rw-   0        0        0      313 2024-03-27 19:22:54.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/__init__.py
--rw-rw-rw-   0        0        0     6088 2024-03-28 17:54:32.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/base.py
--rw-rw-rw-   0        0        0     2233 2024-03-27 21:16:44.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/basic.py
--rw-rw-rw-   0        0        0     8903 2024-03-31 07:03:46.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/inlines.py
--rw-rw-rw-   0        0        0      593 2024-03-27 21:31:30.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/snippets_inlines.py
--rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/view.py
--rw-rw-rw-   0        0        0     3360 2024-03-27 13:07:34.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/registry/value.py
--rw-rw-rw-   0        0        0     5214 2024-03-29 15:26:06.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/render.py
--rw-rw-rw-   0        0        0     1042 2024-03-31 07:03:01.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/settings.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.217884 wagtail_editorjs-1.5.9/wagtail_editorjs/static/
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.219895 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.473151 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/css/
--rw-rw-rw-   0        0        0     8328 2024-03-29 10:59:02.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
--rw-rw-rw-   0        0        0    11473 2024-03-30 13:38:29.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.507697 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/
--rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
--rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
--rw-rw-rw-   0        0        0     2913 2024-03-29 23:54:47.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.527824 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/init/
--rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
--rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.672189 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/
--rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
--rw-rw-rw-   0        0        0    11687 2024-03-30 13:16:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
--rw-rw-rw-   0        0        0     3617 2024-03-30 13:17:20.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
--rw-rw-rw-   0        0        0    11261 2024-03-30 13:14:32.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
--rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
--rw-rw-rw-   0        0        0     6519 2024-03-26 20:32:13.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
--rw-rw-rw-   0        0        0    16447 2024-03-30 13:17:10.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
--rw-rw-rw-   0        0        0     5742 2024-03-26 20:39:23.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.220892 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.727129 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
--rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.209229 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
--rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
--rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
--rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
--rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
--rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
--rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
--rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
--rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
--rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
--rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
--rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
--rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
--rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
--rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
--rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
--rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
--rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
--rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
--rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
--rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
--rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
--rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:37.222273 wagtail_editorjs-1.5.9/wagtail_editorjs/templates/
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.218198 wagtail_editorjs-1.5.9/wagtail_editorjs/templates/wagtail_editorjs/
--rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.225451 wagtail_editorjs-1.5.9/wagtail_editorjs/templates/wagtail_editorjs/widgets/
--rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.237452 wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.240825 wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      892 2024-03-28 09:30:53.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
--rw-rw-rw-   0        0        0      349 2024-03-26 20:17:19.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/editorjs.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.268092 wagtail_editorjs-1.5.9/wagtail_editorjs/tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/tests/__init__.py
--rw-rw-rw-   0        0        0     2555 2024-03-27 14:19:57.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/tests/test_attrs.py
--rw-rw-rw-   0        0        0     2025 2024-03-27 14:10:52.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/tests/test_inlines.py
--rw-rw-rw-   0        0        0     5784 2024-03-27 20:43:47.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/tests/test_render.py
--rw-rw-rw-   0        0        0     2269 2024-03-27 13:17:58.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.275562 wagtail_editorjs-1.5.9/wagtail_editorjs/wagtail_hooks/
--rw-rw-rw-   0        0        0       44 2024-03-31 07:08:22.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     7101 2024-03-28 18:26:01.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/wagtail_hooks/features.py
--rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.5.9/wagtail_editorjs/wagtail_hooks/urls.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:09:38.276532 wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/
--rw-rw-rw-   0        0        0     4105 2024-03-31 07:09:36.000000 wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4833 2024-03-31 07:09:37.000000 wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 07:09:36.000000 wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-31 07:09:36.000000 wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-31 07:09:36.000000 wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.104594 wagtail_editorjs-1.6.0/
+-rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4946 2024-04-19 16:16:26.104594 wagtail_editorjs-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3687 2024-04-08 19:47:07.000000 wagtail_editorjs-1.6.0/README.md
+-rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-19 16:16:26.116310 wagtail_editorjs-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.948499 wagtail_editorjs-1.6.0/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      312 2024-04-19 16:16:23.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/apps.py
+-rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/blocks.py
+-rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/django_editor.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.977420 wagtail_editorjs-1.6.0/wagtail_editorjs/features/
+-rw-rw-rw-   0        0        0      588 2024-04-18 08:53:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/__init__.py
+-rw-rw-rw-   0        0        0    10474 2024-04-18 21:16:10.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/blocks.py
+-rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/documents.py
+-rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/images.py
+-rw-rw-rw-   0        0        0     5486 2024-04-18 22:08:22.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/inlines.py
+-rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/lists.py
+-rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/features/tunes.py
+-rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/fields.py
+-rw-rw-rw-   0        0        0     6632 2024-04-16 13:02:46.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/forms.py
+-rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.978420 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.980420 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.985422 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/
+-rw-rw-rw-   0        0        0      906 2024-04-18 21:15:11.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.993563 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/
+-rw-rw-rw-   0        0        0      229 2024-03-29 10:32:13.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/__init__.py
+-rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/attrs.py
+-rw-rw-rw-   0        0        0     3494 2024-03-29 14:48:28.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/element.py
+-rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/utils.py
+-rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/feature_registry.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.005565 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/
+-rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/__init__.py
+-rw-rw-rw-   0        0        0     6980 2024-04-18 21:22:23.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/base.py
+-rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/basic.py
+-rw-rw-rw-   0        0        0     8940 2024-04-18 22:02:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/inlines.py
+-rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/snippets_inlines.py
+-rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/view.py
+-rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/registry/value.py
+-rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/render.py
+-rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.913613 wagtail_editorjs-1.6.0/wagtail_editorjs/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.916612 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.007560 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/
+-rw-rw-rw-   0        0        0     9983 2024-04-18 19:17:32.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
+-rw-rw-rw-   0        0        0    13978 2024-04-18 10:03:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.013562 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/
+-rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
+-rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
+-rw-rw-rw-   0        0        0     2913 2024-03-29 23:54:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.017094 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/init/
+-rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
+-rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.028490 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/
+-rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
+-rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+-rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
+-rw-rw-rw-   0        0        0     3695 2024-04-18 21:50:35.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
+-rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
+-rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
+-rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
+-rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+-rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.919052 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.032678 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
+-rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.061879 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
+-rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
+-rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
+-rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
+-rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
+-rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
+-rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
+-rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
+-rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
+-rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
+-rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
+-rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
+-rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
+-rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
+-rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
+-rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
+-rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
+-rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
+-rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
+-rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
+-rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
+-rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+-rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.063877 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
+-rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:25.920052 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.065009 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.067013 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/widgets/
+-rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.069585 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.072389 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      892 2024-03-28 09:30:53.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
+-rw-rw-rw-   0        0        0      349 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/editorjs.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.074398 wagtail_editorjs-1.6.0/wagtail_editorjs/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.077397 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.078396 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.086681 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_attrs.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_inlines.py
+-rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_render.py
+-rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.094849 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/settings.py
+-rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/test/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.101599 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     7231 2024-04-18 10:12:16.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/features.py
+-rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:16:26.103596 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/
+-rw-rw-rw-   0        0        0     4946 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5464 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 16:16:25.000000 wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/top_level.txt
```

### Comparing `wagtail_editorjs-1.5.9/LICENSE` & `wagtail_editorjs-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/PKG-INFO` & `wagtail_editorjs-1.6.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,18 @@
-Metadata-Version: 2.1
-Name: wagtail_editorjs
-Version: 1.5.9
-Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
-Home-page: https://github.com/Nigel2392/wagtail_editorjs
-Author: Nigel
-Author-email: nigel@goodadvice.it
-License: GPL-3.0-only
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 5
-Classifier: Framework :: Wagtail :: 6
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=5.0
-Requires-Dist: beautifulsoup4>=4.9.3
-Requires-Dist: bleach>=6.0.0
-
 wagtail_editorjs
 ================
 
 *Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
 
 A Wagtail EditorJS widget with page/image chooser support, document support and more!
 
 ## Add features:
 
-* [Add an already defined EditorJS feature](https://github.com/Nigel2392/wagtail_editorjs/blob/main/docs/editorjs_feature.md "Simple Image Feature")
+* [Add an EditorJS feature](https://github.com/Nigel2392/wagtail_editorjs/blob/main/docs/editorjs_feature.md "Simple Image Feature")
+* [Add an EditorJS tune](https://github.com/Nigel2392/wagtail_editorjs/blob/main/docs/tunes.md "text-alignment-tune") (Already exists in `wagtail_editorjs`, just an example.)
 
 Quick start
 -----------
 
 1. Add 'wagtail_editorjs' to your INSTALLED_APPS setting like this:
 
    ```
@@ -57,63 +26,65 @@
    ```django-html
    <link rel="stylesheet" href="{% static 'wagtail_editorjs/css/frontend.css' %}">
    {% load editorjs %}
    {% editorjs self.editor_field %}
    ```
 3. Add the field to your model:
 
-    ```python
-    ...
-    from wagtail_editorjs.fields import EditorJSField
-    from wagtail_editorjs.blocks import EditorJSBlock
-    
-    
-    class HomePage(Page):
-        content_panels = [
-            FieldPanel("editor_field"),
-            FieldPanel("content"),
-        ]
-        editor_field = EditorJSField(
-            # All supported features
-            features=[
-                 'attaches',
-                 'checklist',
-                 'code',
-                 'delimiter',
-                 'document',
-                 'drag-drop',
-                 'header',
-                 'image',
-                 'images',
-                 'inline-code',
-                 'link',
-                 'marker',
-                 'nested-list',
-                 'paragraph',
-                 'quote',
-                 'raw',
-                 'table',
-                 'text-alignment-tune',
-                 'text-variant-tune',
-                 'underline',
-                 'undo-redo',
-                 'warning',
-             ],
-            blank=True,
-            null=True,
-        )
-    
-        # Or as a block
-        content = fields.StreamField([
-            ('editorjs', EditorJSBlock(features=[
-                # ... same as before
-            ])),
-        ], blank=True, use_json_field=True)
-    ```
-
+   ```python
+   ...
+   from wagtail_editorjs.fields import EditorJSField
+   from wagtail_editorjs.blocks import EditorJSBlock
+
+
+   class HomePage(Page):
+       content_panels = [
+           FieldPanel("editor_field"),
+           FieldPanel("content"),
+       ]
+       editor_field = EditorJSField(
+           # All supported features
+           features=[
+                'attaches',
+                'checklist',
+                'code',
+                'delimiter',
+                'header',
+                'inline-code',
+                'marker',
+                'nested-list',
+                'paragraph',
+                'quote',
+                'raw',
+                'table',
+                'underline',
+                'warning',
+                'link-autocomplete',
+                'link',
+                'image',
+                'images',
+                'document',
+                'text-alignment-tune',
+                'text-variant-tune',
+                'background-color-tune',
+                'text-color-tune',
+                'undo-redo',
+                'drag-drop',
+            ],
+           blank=True,
+           null=True,
+       )
+
+       # Or as a block
+       content = fields.StreamField([
+           ('editorjs', EditorJSBlock(features=[
+               # ... same as before
+           ])),
+       ], blank=True, use_json_field=True)
+   ```
 
 ## List features
 
 This readme might not fully reflect which features are available.
 
 To find this out - you can:
 
@@ -126,16 +97,34 @@
 
    ```python
    from wagtail_editorjs.registry import EDITOR_JS_FEATURES
    print(EDITOR_JS_FEATURES.keys())
    dict_keys([... all registered features ...])
    ```
 
-
 ## Settings
 
 ### `EDITORJS_CLEAN_HTML`
 
 Default: `True`
 Clean the HTML output on rendering.
 This happens every time the field is rendered.
 It might be smart to set up some sort of caching mechanism.
+Optionally; cleaning can be FORCED by passing `clean=True` or `False` to the  `render_editorjs_html` function.
+
+### `EDITORJS_ADD_BLOCK_ID`
+
+Default: `true`
+Add a block ID to each editorJS block when rendering.
+This is useful for targeting the block with JavaScript,
+or possibly creating some link from frontend to admin area.
+
+### `EDITORJS_BLOCK_ID_ATTR`
+
+Default: `data-editorjs-block-id`
+The attribute name to use for the block ID.
+This is only used if  `ADD_BLOCK_ID` is True.
+
+### `EDITORJS_USE_FULL_URLS`
+
+Default: `False`
+Use full urls if the request is available in the EditorJS rendering context.
```

### Comparing `wagtail_editorjs-1.5.9/README.md` & `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_inlines.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,78 @@
-wagtail_editorjs
-================
+from django.test import TestCase
 
-*Check out [Awesome Wagtail](https://github.com/springload/awesome-wagtail) for more awesome packages and resources from the Wagtail community.*
 
-A Wagtail EditorJS widget with page/image chooser support, document support and more!
+from .base import BaseEditorJSTest
+from wagtail_editorjs.registry import (
+    InlineEditorJSFeature,
+    EDITOR_JS_FEATURES,
+)
+
+import bs4
 
-## Add features:
 
-* [Add an already defined EditorJS feature](https://github.com/Nigel2392/wagtail_editorjs/blob/main/docs/editorjs_feature.md "Simple Image Feature")
-
-Quick start
------------
-
-1. Add 'wagtail_editorjs' to your INSTALLED_APPS setting like this:
-
-   ```
-   INSTALLED_APPS = [
-   ...,
-   'wagtail_editorjs',
-   ]
-   ```
-2. Add the HTML to your template:
-
-   ```django-html
-   <link rel="stylesheet" href="{% static 'wagtail_editorjs/css/frontend.css' %}">
-   {% load editorjs %}
-   {% editorjs self.editor_field %}
-   ```
-3. Add the field to your model:
-
-    ```python
-    ...
-    from wagtail_editorjs.fields import EditorJSField
-    from wagtail_editorjs.blocks import EditorJSBlock
-    
-    
-    class HomePage(Page):
-        content_panels = [
-            FieldPanel("editor_field"),
-            FieldPanel("content"),
+
+TESTING_HTML = """
+<div class="editorjs">
+    <div class="editorjs-block" data-type="paragraph">
+        <p>Hello, World!</p>
+    </div>
+    <div class="editorjs-block" data-type="header">
+        <h1>Header</h1>
+    </div>
+    <div class="editorjs-block" data-type="list" data-testing-id="TARGET">
+
+    </div>
+    <div class="editorjs-block" data-type="table">
+        <table>
+            <tr>
+                <td>1</td>
+                <td>2</td>
+            </tr>
+            <tr>
+                <td>3</td>
+                <td>4</td>
+            </tr>
+        </table>
+    </div>
+</div>
+"""
+
+
+class TestEditorJSInline(BaseEditorJSTest):
+    def setUp(self):
+        super().setUp()
+        self.inlines = [
+            feature
+            for feature in EDITOR_JS_FEATURES.features.values()
+            if isinstance(feature, InlineEditorJSFeature)
         ]
-        editor_field = EditorJSField(
-            # All supported features
-            features=[
-                 'attaches',
-                 'checklist',
-                 'code',
-                 'delimiter',
-                 'document',
-                 'drag-drop',
-                 'header',
-                 'image',
-                 'images',
-                 'inline-code',
-                 'link',
-                 'marker',
-                 'nested-list',
-                 'paragraph',
-                 'quote',
-                 'raw',
-                 'table',
-                 'text-alignment-tune',
-                 'text-variant-tune',
-                 'underline',
-                 'undo-redo',
-                 'warning',
-             ],
-            blank=True,
-            null=True,
-        )
-    
-        # Or as a block
-        content = fields.StreamField([
-            ('editorjs', EditorJSBlock(features=[
-                # ... same as before
-            ])),
-        ], blank=True, use_json_field=True)
-    ```
-
-
-## List features
-
-This readme might not fully reflect which features are available.
-
-To find this out - you can:
-
-1. start the python shell
-
-   ```bash
-   py ./manage.py shell
-   ```
-2. Print all the available features:
-
-   ```python
-   from wagtail_editorjs.registry import EDITOR_JS_FEATURES
-   print(EDITOR_JS_FEATURES.keys())
-   dict_keys([... all registered features ...])
-   ```
-
-
-## Settings
-
-### `EDITORJS_CLEAN_HTML`
-
-Default: `True`
-Clean the HTML output on rendering.
-This happens every time the field is rendered.
-It might be smart to set up some sort of caching mechanism.
+
+    def test_inlines(self):
+
+        for feature in self.inlines:
+            feature: InlineEditorJSFeature
+            test_data = feature.get_test_data()
+
+            if not test_data:
+                continue
+
+            soup = bs4.BeautifulSoup(TESTING_HTML, "html.parser")
+            testing_block = soup.find("div", {"data-testing-id": "TARGET"})
+            testing_block.clear()
+
+            for i, (initial, _) in enumerate(test_data):
+                initial_soup = bs4.BeautifulSoup(initial, "html.parser")
+                initial_soup.attrs["data-testing-id"] = f"test_{i}"
+                testing_block.append(initial_soup)
+
+            feature.parse_inline_data(soup)
+
+            html = str(soup)
+
+            outputs = [i[1] for i in test_data]
+            for i, output in enumerate(outputs):
+                self.assertInHTML(
+                    output,
+                    html,
+                )
+
```

### Comparing `wagtail_editorjs-1.5.9/setup.cfg` & `wagtail_editorjs-1.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f65 6469 746f   = wagtail_edito
 00000020: 726a 730d 0a76 6572 7369 6f6e 203d 2031  rjs..version = 1
-00000030: 2e35 2e39 0d0a 6465 7363 7269 7074 696f  .5.9..descriptio
+00000030: 2e36 2e30 0d0a 6465 7363 7269 7074 696f  .6.0..descriptio
 00000040: 6e20 3d20 4564 6974 6f72 4a53 2061 7320  n = EditorJS as 
 00000050: 6120 7769 6467 6574 2066 6f72 2057 6167  a widget for Wag
 00000060: 7461 696c 2c20 7769 7468 2050 6167 652d  tail, with Page-
 00000070: 2061 6e64 2049 6d61 6765 2063 686f 6f73   and Image choos
 00000080: 6572 2073 7570 706f 7274 0d0a 6c6f 6e67  er support..long
 00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 000000a0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/blocks.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/django_editor.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/django_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,21 @@
 
 
 
 class EditorJSDjangoWidget(EditorJSWidget):
     """
         Taken from wagtail.
         This class is deprecated in wagtail 7.0
-        This might still be useful if we are hooking into the wagtail_fedit library.
+        This might still be useful if we have wagtail installed
+        but would like to use the editorjs widget in a non-wagtailadmin form.
     """
     def render_html(self, name, value, attrs):
         """Render the HTML (non-JS) portion of the field markup"""
         return super().render(name, value, attrs)
 
-    def get_value_data(self, value):
-        # Perform any necessary preprocessing on the value passed to render() before it is passed
-        # on to render_html / render_js_init. This is a good place to perform database lookups
-        # that are needed by both render_html and render_js_init. Return value is arbitrary
-        # (we only care that render_html / render_js_init can accept it), but will typically be
-        # a dict of data needed for rendering: id, title etc.
-        return value
-
     def render(self, name, value, attrs=None, renderer=None):
         # no point trying to come up with sensible semantics for when 'id' is missing from attrs,
         # so let's make sure it fails early in the process
         try:
             id_ = attrs["id"]
         except (KeyError, TypeError):
             raise TypeError(
```

#### html2text {}

```diff
@@ -1,29 +1,24 @@
 from django.utils.functional import cached_property from
 django.utils.safestring import mark_safe from .forms import EditorJSFormField,
 EditorJSWidget class DjangoEditorJSFormField(EditorJSFormField):
 @cached_property def widget(self): return EditorJSDjangoWidget
 ( features=self.features, tools_config=self.tools_config, ) class
 EditorJSDjangoWidget(EditorJSWidget): """ Taken from wagtail. This class is
-deprecated in wagtail 7.0 This might still be useful if we are hooking into the
-wagtail_fedit library. """ def render_html(self, name, value, attrs): """Render
-the HTML (non-JS) portion of the field markup""" return super().render(name,
-value, attrs) def get_value_data(self, value): # Perform any necessary
-preprocessing on the value passed to render() before it is passed # on to
-render_html / render_js_init. This is a good place to perform database lookups
-# that are needed by both render_html and render_js_init. Return value is
-arbitrary # (we only care that render_html / render_js_init can accept it), but
-will typically be # a dict of data needed for rendering: id, title etc. return
-value def render(self, name, value, attrs=None, renderer=None): # no point
-trying to come up with sensible semantics for when 'id' is missing from attrs,
-# so let's make sure it fails early in the process try: id_ = attrs["id"]
-except (KeyError, TypeError): raise TypeError( "WidgetWithScript cannot be
-rendered without an 'id' attribute" ) value_data = self.get_value_data(value)
-widget_html = self.render_html(name, value_data, attrs) js =
-self.render_js_init(id_, name, value_data) out = f"{widget_html}
+deprecated in wagtail 7.0 This might still be useful if we have wagtail
+installed but would like to use the editorjs widget in a non-wagtailadmin form.
+""" def render_html(self, name, value, attrs): """Render the HTML (non-JS)
+portion of the field markup""" return super().render(name, value, attrs) def
+render(self, name, value, attrs=None, renderer=None): # no point trying to come
+up with sensible semantics for when 'id' is missing from attrs, # so let's make
+sure it fails early in the process try: id_ = attrs["id"] except (KeyError,
+TypeError): raise TypeError( "WidgetWithScript cannot be rendered without an
+'id' attribute" ) value_data = self.get_value_data(value) widget_html =
+self.render_html(name, value_data, attrs) js = self.render_js_init(id_, name,
+value_data) out = f"{widget_html}
 " return mark_safe(out) def render_js_init(self, id_, name, value): # Adapted
 from editorjs-widget-controller.js return """ let editorJSWidget__wrapper =
 document.querySelector(`#${id}-wagtail-editorjs-widget-wrapper`); let
 editorJSWidget__configElem = editorJSWidget__wrapper.querySelector(`#wagtail-
 editorjs-config`); let editorJSWidget__config = JSON.parse
 (editorJSWidget__configElem.textContent); let editorJSWidget__keys =
 Object.keys(editorJSWidget__config.tools); for (let i = 0; i <
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/__init__.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     CodeFeature,
     DelimiterFeature,
     HeaderFeature,
     HTMLFeature,
     WarningFeature,
     TableFeature,
     BlockQuoteFeature,
+    ButtonFeature,
 )
 from .lists import (
     NestedListFeature,
     CheckListFeature,
 )
 from .documents import (
     AttachesFeature,
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/blocks.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/blocks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any
 from django import forms
 from django.utils.translation import gettext_lazy as _
+from django.utils.functional import cached_property
 
 import bleach
 
 from ..registry import (
+    PageChooserURLsMixin,
     EditorJSFeature,
     EditorJSBlock,
     EditorJSElement,
     wrap_tag,
 )
 
 
@@ -269,7 +271,93 @@
         return [
             {
                 "text": "This is a quote.",
                 "caption": "Anonymous",
             }
         ]
 
+from wagtail.models import Page
+from wagtail.admin.widgets import AdminPageChooser
+
+class ButtonFeature(PageChooserURLsMixin, EditorJSFeature):
+    allowed_tags:       list[str]            = ["a"]
+    allowed_attributes: dict[str, list[str]] = {
+        "a": ["href", "class"]
+    }
+    chooser_class = AdminPageChooser
+    model         = Page
+    klass         = "PageButtonTool"
+    js            = [
+        "wagtail_editorjs/js/tools/wagtail-button-tool.js",
+    ]
+
+    @cached_property
+    def widget(self):
+        if self.chooser_class is None:
+            return None
+        
+        return self.chooser_class()
+    
+    def validate(self, data: Any):
+        super().validate(data)
+
+        if "pageId" not in data["data"]:
+            raise forms.ValidationError("Invalid id value")
+        
+        if "text" not in data["data"]:
+            raise forms.ValidationError("Invalid text value")
+
+    def get_config(self, context: dict[str, Any]):
+        config = super().get_config() or {}
+        config.setdefault("config", {})
+        config["config"][
+            "chooserId"
+        ] = f"editorjs-{self.model._meta.model_name}-button-chooser-{context['widget']['attrs']['id']}"
+        return config
+    
+    def render_block_data(self, block: EditorJSBlock, context=None) -> EditorJSElement:
+        try:
+            page = self.model.objects.get(id=block["data"]["pageId"])
+        except self.model.DoesNotExist:
+            return None
+
+        request = None
+        if context:
+            request = context.get("request")
+
+        anchor = EditorJSElement(
+            "a",
+            block["data"]["text"],
+            {
+                "href": page.get_url(request),
+                "class": "editor-button",
+            }
+        )
+
+        return EditorJSElement(
+            "div", anchor, {"class": "editor-button-container"},
+        )
+
+    def render_template(self, context: dict[str, Any] = None):
+        if not self.widget:
+            return super().render_template(context)
+        
+        return self.widget.render_html(
+            f"editorjs-{self.model._meta.model_name}-button-chooser-{context['widget']['attrs']['id']}",
+            None,
+            {
+                "id": f"editorjs-{self.model._meta.model_name}-button-chooser-{context['widget']['attrs']['id']}"
+            },
+        )
+
+    @classmethod
+    def get_test_data(cls):
+        pages = cls.model.objects.all()[:5]
+
+        return [
+            {
+                "pageId": page.id,
+                "text": page.title,
+            }
+            for page in pages
+        ]
+
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/documents.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/images.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,15 @@
         # "wagtail_editorjs/js/tools/wagtail-image-row.js",
     # ]
 
     @property
     def js(self):
         return [
             *(AdminImageChooser().media._js or []),
+            "wagtail_editorjs/vendor/sortable/sortable.min.js",
             "wagtail_editorjs/js/tools/wagtail-image-row.js",
         ]
     
     @js.setter
     def js(self, value): pass
 
     def get_config(self, context: dict[str, Any]):
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/inlines.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/inlines.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,59 @@
 from wagtail.models import Page
 from wagtail.admin.widgets import AdminPageChooser
 from wagtail.documents.widgets import AdminDocumentChooser
 from wagtail.documents import get_document_model
 from wagtail import hooks
 
 from ..registry import (
+    PageChooserURLsMixin,
     ModelInlineEditorJSFeature,
     FeatureViewMixin,
 )
 from django.http import (
     HttpResponse,
     JsonResponse,
 )
 
 
 Document = get_document_model()
 
 
-class BasePageLinkMixin:
+class BasePageLinkMixin(PageChooserURLsMixin):
+    allowed_attributes = ["target", "rel"]
+    can_have_attrs = {
+        "data-target": None,
+        "data-rel": None,
+    }
+
+    def build_element(self, item, obj, context: dict[str, Any] = None, data: dict[str, Any] = None):
+        """Build the element from the object."""
+        super().build_element(item, obj, context, data)
+        if "data-target" in data and data["data-target"]:
+            item["target"] = data["data-target"]
+        if "data-rel" in data and data["data-rel"]:
+            item["rel"] = data["data-rel"]
+
     @classmethod
     def get_url(cls, instance):
         return instance.get_url()
 
     @classmethod
     def get_full_url(cls, instance, request):
         return instance.get_full_url(request)
     
     @classmethod
     def get_test_queryset(cls):
         return super().get_test_queryset().filter(depth__gt=1)
 
 class LinkFeature(BasePageLinkMixin, ModelInlineEditorJSFeature):
     allowed_tags = ["a"]
-    allowed_attributes = ["class", "href", "data-id"]
+    allowed_attributes = BasePageLinkMixin.allowed_attributes + [
+        "class", "href", "data-id"
+    ]
     must_have_attrs = {
         "data-parent-id": None,
     }
     chooser_class = AdminPageChooser
     model = Page
 
     klass="WagtailLinkTool"
@@ -64,15 +81,17 @@
 SEARCH_QUERY_PARAM = "search"
 CONSTRUCT_PAGE_QUERYSET = "construct_page_queryset"
 BUILD_PAGE_DATA = "build_page_data"
 
 
 class LinkAutoCompleteFeature(FeatureViewMixin, BasePageLinkMixin, ModelInlineEditorJSFeature):
     allowed_tags = ["a"]
-    allowed_attributes = ["class", "href", "data-id"]
+    allowed_attributes = BasePageLinkMixin.allowed_attributes + [
+        "class", "href", "data-id"
+    ]
     must_have_attrs = {
         "data-autocomplete": "page",
     }
     chooser_class = AdminPageChooser
     model = Page
     klass="LinkAutocomplete"
     js = [
```

#### html2text {}

```diff
@@ -1,33 +1,41 @@
 from typing import Any from django.urls import reverse from
 django.utils.translation import gettext_lazy as _ from wagtail.models import
 Page from wagtail.admin.widgets import AdminPageChooser from
 wagtail.documents.widgets import AdminDocumentChooser from wagtail.documents
 import get_document_model from wagtail import hooks from ..registry import
-( ModelInlineEditorJSFeature, FeatureViewMixin, ) from django.http import
-( HttpResponse, JsonResponse, ) Document = get_document_model() class
-BasePageLinkMixin: @classmethod def get_url(cls, instance): return
-instance.get_url() @classmethod def get_full_url(cls, instance, request):
-return instance.get_full_url(request) @classmethod def get_test_queryset(cls):
-return super().get_test_queryset().filter(depth__gt=1) class LinkFeature
-(BasePageLinkMixin, ModelInlineEditorJSFeature): allowed_tags = ["a"]
-allowed_attributes = ["class", "href", "data-id"] must_have_attrs = { "data-
-parent-id": None, } chooser_class = AdminPageChooser model = Page
-klass="WagtailLinkTool" js = [ "wagtail_editorjs/js/tools/wagtail-chooser-
-tool.js", "wagtail_editorjs/js/tools/wagtail-link.js", ] @classmethod def
-get_test_data(cls): models = cls.get_test_queryset()[0:5] return [ ( # Override
-to add data-autocomplete. f"", f"", ) for model in models ] SEARCH_QUERY_PARAM
-= "search" CONSTRUCT_PAGE_QUERYSET = "construct_page_queryset" BUILD_PAGE_DATA
-= "build_page_data" class LinkAutoCompleteFeature(FeatureViewMixin,
+( PageChooserURLsMixin, ModelInlineEditorJSFeature, FeatureViewMixin, ) from
+django.http import ( HttpResponse, JsonResponse, ) Document =
+get_document_model() class BasePageLinkMixin(PageChooserURLsMixin):
+allowed_attributes = ["target", "rel"] can_have_attrs = { "data-target": None,
+"data-rel": None, } def build_element(self, item, obj, context: dict[str, Any]
+= None, data: dict[str, Any] = None): """Build the element from the object."""
+super().build_element(item, obj, context, data) if "data-target" in data and
+data["data-target"]: item["target"] = data["data-target"] if "data-rel" in data
+and data["data-rel"]: item["rel"] = data["data-rel"] @classmethod def get_url
+(cls, instance): return instance.get_url() @classmethod def get_full_url(cls,
+instance, request): return instance.get_full_url(request) @classmethod def
+get_test_queryset(cls): return super().get_test_queryset().filter(depth__gt=1)
+class LinkFeature(BasePageLinkMixin, ModelInlineEditorJSFeature): allowed_tags
+= ["a"] allowed_attributes = BasePageLinkMixin.allowed_attributes + [ "class",
+"href", "data-id" ] must_have_attrs = { "data-parent-id": None, } chooser_class
+= AdminPageChooser model = Page klass="WagtailLinkTool" js =
+[ "wagtail_editorjs/js/tools/wagtail-chooser-tool.js", "wagtail_editorjs/js/
+tools/wagtail-link.js", ] @classmethod def get_test_data(cls): models =
+cls.get_test_queryset()[0:5] return [ ( # Override to add data-autocomplete.
+f"", f"", ) for model in models ] SEARCH_QUERY_PARAM = "search"
+CONSTRUCT_PAGE_QUERYSET = "construct_page_queryset" BUILD_PAGE_DATA =
+"build_page_data" class LinkAutoCompleteFeature(FeatureViewMixin,
 BasePageLinkMixin, ModelInlineEditorJSFeature): allowed_tags = ["a"]
-allowed_attributes = ["class", "href", "data-id"] must_have_attrs = { "data-
-autocomplete": "page", } chooser_class = AdminPageChooser model = Page
-klass="LinkAutocomplete" js = [ "wagtail_editorjs/vendor/editorjs/tools/link-
-autocomplete.js", ] def get_config(self, context: dict[str, Any]): config =
-super(ModelInlineEditorJSFeature, self).get_config(context) config.setdefault
+allowed_attributes = BasePageLinkMixin.allowed_attributes + [ "class", "href",
+"data-id" ] must_have_attrs = { "data-autocomplete": "page", } chooser_class =
+AdminPageChooser model = Page klass="LinkAutocomplete" js =
+[ "wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js", ] def
+get_config(self, context: dict[str, Any]): config = super
+(ModelInlineEditorJSFeature, self).get_config(context) config.setdefault
 ("config", {}) config["config"]["endpoint"] = reverse(f"wagtail_editorjs:
 {self.tool_name}") config["config"]["queryParam"] = "search" return config
 @classmethod def get_test_data(cls): models = cls.get_test_queryset()[0:5]
 return [ ( # Override to add data-autocomplete. f"", f"", ) for model in models
 ] def handle_get(self, request): """ Autocomplete for internal links """ search
 = request.GET.get(SEARCH_QUERY_PARAM) pages = Page.objects.all()\ .live()\
 .specific() for fn in hooks.get_hooks(CONSTRUCT_PAGE_QUERYSET): pages = fn
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/lists.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/lists.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/features/tunes.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/features/tunes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any
 from django import forms
 from django.utils.translation import gettext_lazy as _
 
 from ..registry import (
     EditorJSTune,
     EditorJSElement,
-    EditorJSWrapper,
     wrapper,
 )
 
 
 class AlignmentBlockTune(EditorJSTune):
     allowed_attributes = {
         "*": ["class"],
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/fields.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 from django.db import models
 from django.utils.functional import cached_property
+from django.core.exceptions import ValidationError
 
 from .forms import EditorJSFormField
 from .registry import EDITOR_JS_FEATURES, get_features
 
 
 class EditorJSField(models.JSONField):
     def __init__(self,
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/forms.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/forms.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from django import forms
 from django.forms import (
     fields as formfields,
     widgets
 )
 from wagtail import hooks
 
+from datetime import datetime
+
 from .hooks import (
     BUILD_CONFIG_HOOK,
 )
 from .registry import (
     EDITOR_JS_FEATURES,
     get_features,
     TemplateNotSpecifiedError,
@@ -156,19 +158,47 @@
             self.features, value
         )
 
         return super().prepare_value(value)
     
     def validate(self, value) -> None:
         super().validate(value)
+
         if value is None and self.required:
             raise forms.ValidationError("This field is required")
 
-        if not isinstance(value, dict):
-            raise forms.ValidationError("Invalid JSON object")
-        
+        if value:
+            if not isinstance(value, dict):
+                raise forms.ValidationError("Invalid EditorJS JSON object, expected a dictionary")
+
+            if "time" not in value:
+                raise forms.ValidationError("Invalid EditorJS JSON object, missing time")
+            
+            if "version" not in value:
+                raise forms.ValidationError("Invalid EditorJS JSON object, missing version")
+            
+            time = value["time"] # 1713272305659
+            if not isinstance(time, (int, float)):
+                raise forms.ValidationError("Invalid EditorJS JSON object, time is not an integer")
+            
+            time_invalid = "Invalid EditorJS JSON object, time is invalid"
+            try:
+                time = datetime.fromtimestamp(time / 1000)
+            except:
+                raise forms.ValidationError(time_invalid)
+
+            if time is None:
+                raise forms.ValidationError(time_invalid)
+
+        if value and self.required:
+            if "blocks" not in value:
+                raise forms.ValidationError("Invalid JSON object")
+            
+            if not value["blocks"]:
+                raise forms.ValidationError("This field is required")
+
         EDITOR_JS_FEATURES.validate_for_tools(
             self.features, value
         )
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/__init__.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .feature_registry import (
     EditorJSFeatures,
 )
 from .features import (
+    PageChooserURLsMixin,
     BaseEditorJSFeature,
     EditorJSFeature,
     EditorJSJavascriptFeature,
     EditorJSTune,
     FeatureViewMixin,
     InlineEditorJSFeature,
     ModelInlineEditorJSFeature,
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/attrs.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/element.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/element.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/element/utils.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/element/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/feature_registry.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/feature_registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/base.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 from typing import Any, Union, TYPE_CHECKING
+from django.urls import reverse_lazy
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from ..value import (
     EditorJSBlock,
 )
 
 if TYPE_CHECKING:
     from ..feature_registry import EditorJSFeatures
 
 
 class TemplateNotSpecifiedError(Exception):
     pass
 
 
+class PageChooserURLsMixin:
+    def get_config(self, context: dict[str, Any] = None) -> dict:
+        config = super().get_config(context)
+        config.setdefault("config", {})
+        config["config"]["chooserUrls"] = {
+            "pageChooser": reverse_lazy(
+                "wagtailadmin_choose_page",
+            ),
+            "externalLinkChooser": reverse_lazy(
+                "wagtailadmin_choose_page_external_link",
+            ),
+            "emailLinkChooser": reverse_lazy(
+                "wagtailadmin_choose_page_email_link",
+            ),
+            "phoneLinkChooser": reverse_lazy(
+                "wagtailadmin_choose_page_phone_link",
+            ),
+            "anchorLinkChooser": reverse_lazy(
+                "wagtailadmin_choose_page_anchor_link",
+            ),
+        },
+        return config
+
+
 class BaseEditorJSFeature:
     allowed_tags: list[str] = None
     allowed_attributes: dict[str, list[str]] = None
     klass: str = None
     js: list[str] = None
     css: list[str] = None
     # cleaner_funcs: dict[str, dict[str, Callable[[str], bool]]] = {}
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/basic.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
             Javascript only features do not get access to any configuration.
             They are not passed into the EditorJS tools.
         """
         return None
 
 
 class EditorJSFeature(BaseEditorJSFeature):
+
     def validate(self, data: Any):
         """
             Perform basic validation for an EditorJS block feature.
         """
         if not data:
             return
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/inlines.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/inlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,19 +105,19 @@
         for item in elements:
             matches[item] = {}
 
             for key in self.must_have_attrs.keys():
                 matches[item][key] = item.get(key)
 
             for key, value in self.can_have_attrs.items():
-                if value:
-                    matches[item][key] = item.get(key)
-                else:
-                    if item.has_attr(key):
-                        matches[item][key] = True
+                v = item.get(key)
+                if v:
+                    matches[item][key] = v
+                elif item.has_attr(key):
+                    matches[item][key] = True
 
         # Build all inlines.
         self.build_elements(list(matches.items()), context=context)
 
     @classmethod
     def get_test_data(cls) -> list[tuple[str, str]]:
         """
@@ -173,15 +173,15 @@
             f"editorjs-{self.model._meta.model_name}-chooser-{context['widget']['attrs']['id']}",
             None,
             {
                 "id": f"editorjs-{self.model._meta.model_name}-chooser-{context['widget']['attrs']['id']}"
             },
         )
 
-    def build_element(self, item, obj, context: dict[str, Any] = None):
+    def build_element(self, item, obj, context: dict[str, Any] = None, data: dict[str, Any] = None):
         """
         Build the element from the object.
 
         item:    bs4.element.Tag
         obj:     Model
         context: RequestContext | None
         """
@@ -222,24 +222,24 @@
 
             # # Store element and soup for later replacement of content.
             # element_soups.append((soup, element))
 
             # Item is bs4 tag, attrs are must_have_attrs
 
             id = self.get_id(item, data, context)
-            ids.append((item, id))
+            ids.append((item, id, data))
 
             # delete all attributes
             for key in list(item.attrs.keys()):
                 del item[key]
 
         # Fetch all objects
-        objects = self.model.objects.in_bulk([id for item, id in ids])
-        for item, id in ids:
-            self.build_element(item, objects[id], context)
+        objects = self.model.objects.in_bulk([id for _, id, _ in ids])
+        for item, id, data in ids:
+            self.build_element(item, objects[id], context, data)
 
     def get_css(self):
         return self.widget.media._css.get("all", []) + super().get_css()
 
     def get_js(self):
         return (self.widget.media._js or []) + super().get_js()
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/snippets_inlines.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/snippets_inlines.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,13 +11,14 @@
     def build_element(self, soup_elem, context = None): ...
 
 
 class BaseInlineSnippetChooserFeature(ModelInlineEditorJSFeature):
     model: SnippetChooserModel = None
     widget = AdminSnippetChooser
 
-    def build_element(self, soup_elem, obj: SnippetChooserModel, context: dict[str, Any] = None):
+    def build_element(self, soup_elem, obj: SnippetChooserModel, context: dict[str, Any] = None, data: dict[str, Any] = None):
+        """ Build the element from the object. """
         return obj.build_element(soup_elem, context)
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/features/view.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/features/view.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/registry/value.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/registry/value.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,18 +86,17 @@
         
         if start > end:
             start = end
         
         if start == end:
             return
         
-        for i, block in enumerate(blocks):
-            blocks[i] = self._verify_block(block)
-        
-        b[start:end] = blocks
+        b[start:end] = list(
+            map(self._verify_block, blocks),
+        )
         self["blocks"] = b
 
     def insert(self, index: int, block: "EditorJSBlock"):
         block = self._verify_block(block)        
         self.blocks.insert(index, block)
 
     def append(self, block: "EditorJSBlock"):
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/render.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
         # Optionally tools can decide to not render the block.
         if element is None:
             continue
 
         # Tune the element.
         for tune_name, tune_value in tunes.items():
+            if tune_name not in feature_mappings:
+                continue
+
             element = feature_mappings[tune_name].tune_element(element, tune_value, context)
 
         # Add the block ID to each individual block.
         if settings.ADD_BLOCK_ID:
             # This can be used to link frontend to the admin area.
             element.attrs[settings.BLOCK_ID_ATTR] = block.get("id", "")
         
@@ -127,15 +130,17 @@
     ctx = context or {}
     ctx["html"] = html
 
     if isinstance(context, Context):
         ctx = context.flatten()
 
     return render_to_string(
-        "wagtail_editorjs/rich_text.html", ctx
+        "wagtail_editorjs/rich_text.html",
+        context=ctx,
+        request=ctx.get("request", None)
     )
 
 
 
 #         def parse_allowed_attributes(tag, name, value):
 #             if (
 #                 tag not in allowed_attributes\
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/settings.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+.bi.bi path {
+    stroke: unset;
+}
+
+
 .wagtail-editorjs-widget-container {
     /* max-width: 840px; */
     border-radius: 0.25rem;
     border: 1px solid var(--w-color-grey-200);
     font-size: 1.2rem;
 }
 .wagtail-editorjs-display-none {
@@ -20,14 +25,15 @@
         margin-right: 0;
     }
     .ce-toolbar__actions {
         flex-direction: column;
         justify-content: center;
         align-items: center;
         padding-right: 0;
+        transform: translateY(-8px);
     }
     .ce-toolbar__actions > *:not(:last-child) {
         margin-left: 0;
         margin-right: 0;
         margin-bottom: 0.25rem;
     }
 }
@@ -99,30 +105,32 @@
 
 .wagtail-image-row-wrapper {
     padding: 0.25rem 0;
 }
 .wagtail-image-row-wrapper .wagtail-image-row {
     display: flex;
     flex-wrap: wrap;
+    flex-direction: row;
     gap: 0.5rem;
     align-items: center;
     justify-content: center;
     margin: 0 0.25rem;
 
     -webkit-touch-callout: none; /* iOS Safari */
     -webkit-user-select: none; /* Safari */
      -khtml-user-select: none; /* Konqueror HTML */
        -moz-user-select: none; /* Old versions of Firefox */
         -ms-user-select: none; /* Internet Explorer/Edge */
             user-select: none; /* Non-prefixed version, currently supported by Chrome, Edge, Opera and Firefox */
 }
 .wagtail-image-row-wrapper .wagtail-image-row-image-wrapper {
     display: flex;
-    flex: 1;
+    flex: 1 0 15%;
     gap: 0.5rem;
+    position: relative;
     flex-direction: column;
     border: 1px solid var(--w-color-text-context);
     overflow: hidden;
     border-radius: 0.25rem;
     min-width: 150px;
     height: 200px;
     cursor: grab;
@@ -132,14 +140,50 @@
 }
 .wagtail-image-row-wrapper .wagtail-image-row-image {
     width: 100%;
     height: 100%;
     object-fit: cover;
     object-position: center;
 }
+
+.wagtail-image-row-wrapper .wagtail-image-row-image-actions {
+    display: none;
+    position: absolute;
+    bottom: 0;
+    left: 0;
+    right: 0;
+    flex-direction: row;
+    justify-content: space-between;
+    align-items: center;
+    gap: 0.25rem;
+    padding: 0.25rem;
+}
+.wagtail-image-row-wrapper .wagtail-image-row-image-actions button {
+    background-color: var(--w-color-secondary);
+    color: var(--w-color-white-80);
+    border: 1px solid var(--w-color-grey-200);
+    border-radius: 0.25rem;
+    padding: unset;
+    display: flex;
+    justify-content: center;
+    align-items: center;
+    cursor: pointer;
+    width: 34px;
+    height: 34px;
+}
+.wagtail-image-row-wrapper .wagtail-image-row-image-actions button:hover {
+    background-color: var(--w-color-secondary-400);
+}
+.wagtail-image-row-wrapper .wagtail-image-row-image-actions button svg {
+    vertical-align: middle;
+}
+.wagtail-image-row-wrapper .wagtail-image-row-image-wrapper:hover .wagtail-image-row-image-actions {
+    display: flex;
+}
+
 .wagtail-editorjs-widget-container .ce-popover {
     --max-height: 450px;
 }
 .wagtail-editorjs-widget-container .ce-popover__custom-content {
     display: flex;
     flex-direction: row;
     flex-wrap: wrap;
@@ -264,7 +308,28 @@
 .wagtail-editorjs-widget-container [data-color] a {
     color: var(--block-color);
 }
 .wagtail-editorjs-widget-container [data-background-color] {
     background-color: var(--block-background-color);
 }
 
+.wagtail-button-wrapper {
+    gap: 0.25rem;
+    display: inline-flex;
+    flex-direction: row;
+    align-items: center;
+    justify-content: center;
+}
+.wagtail-button-wrapper .wagtail-button {
+    padding: 0 0.5rem;
+}
+.wagtail-button-wrapper svg {
+    vertical-align: middle;
+    width: 16px;
+    height: 16px;
+}
+
+.wagtail-button-wrapper .wagtail-button-icon {
+    background-color: unset;
+    color: var(--w-color-text-link-default);
+    padding: 0;
+}
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -67,15 +67,15 @@
     }
 
     getState() {
 
     }
 
     onSave() {
-        this.tool.block.dispatchChange();
+        // this.tool.block.dispatchChange();
         return this.getState();
     }
 }
 
 
 class BaseButtonSetting extends BaseToolSetting {
     setTool(api, config, tool) {
@@ -334,14 +334,39 @@
      * @param {Object} attributes
      * @param {Union<string, HTMLElement, NodeList>} children
      * @returns {_ElementType}
      */
     addElement(tag, attributes = {}, ...children) {}
 }
 
+class _ModalType {
+    openChooserModal() {
+        throw new Error('openChooserModal must be implemented by subclasses');
+    }
+}
+
+
+/**
+ * @param {_ModalType} modal
+ * @param {Object} modalArgs
+ * @param {Function} onChosen
+ * @returns {void}
+ */
+function openChooserModal(modal, onChosen) {
+    modal.openChooserModal();
+    let changeEventFunc;
+    changeEventFunc = () => {
+        modal.input.removeEventListener('change', changeEventFunc);
+        const data = modal.getState();
+        onChosen(data);
+    };
+
+    modal.input.addEventListener('change', changeEventFunc);
+}
+
 
 /**
  * @param {String} tag
  * @param {Object} attributes
  * @param {Union<string, HTMLElement, NodeList>} children
  * @returns {_ElementType}
  */
@@ -462,11 +487,15 @@
 
 window.BaseWagtailEditorJSTool = BaseWagtailEditorJSTool;
 window.BaseToggleSetting = BaseToggleSetting;
 window.BaseButtonSetting = BaseButtonSetting;
 window.BaseInputSetting = BaseInputSetting;
 window.BaseSelectInputSetting = BaseSelectInputSetting;
 window.BaseToolSetting = BaseToolSetting;
+
+window._ModalType = _ModalType;
+window.openChooserModal = openChooserModal;
+
 window.makeElement = makeElement;
 window._ElementType = _ElementType;
 window.addAttributeData = addAttributeData;
 window.makeElementType = makeElementType;
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -93,14 +93,15 @@
 
         const previousWrapperTag = this.api.selection.findParentTag(this.tag);
         if (previousWrapperTag || previousWrapperTag && previousWrapperTag.querySelector(this.tag.toLowerCase())) {
             previousWrapperTag.remove();
         }
 
         const wrapperTag = document.createElement(this.tag);
+        this.wrapperTag = wrapperTag;
 
         this.setDataOnWrapper(wrapperTag, state);
 
         wrapperTag.classList.add(this.tagClass);
         wrapperTag.appendChild(selectedText);
         range.insertNode(wrapperTag);
 
@@ -112,14 +113,15 @@
         const text = range.extractContents();
         wrapperTag.remove();
         range.insertNode(text);
     }
 
     checkState() {
         const wrapperTag = this.api.selection.findParentTag(this.tag, this.tagClass);
+        this.wrapperTag = wrapperTag;
         if (!wrapperTag) {
             return
         }
 
 
         this.state = !!wrapperTag;
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -100,15 +100,15 @@
             this.block.dispatchChange();
             this.onChange();
         });
         this.wrapper.appendChild(this.colorInput);
         this.wrapper.appendChild(this.clearButton);
 
         this.api.tooltip.onHover(this.colorInput, this.pickTooltipText, {
-            placement: 'left',
+            placement: 'right',
             hidingDelay: 200,
         });
         this.api.tooltip.onHover(this.clearButton, this.api.i18n.t('Clear Color'), {
             placement: 'top',
             hidingDelay: 200,
         });
 
@@ -174,15 +174,14 @@
         const wrapper = super.render();
         wrapper.appendChild(this.stretchBlockButton);
 
         return wrapper;
     }
 
     onChange() {
-
         if (this.stretchBlockButton && this.stretchTextElement) {
             this.stretchTextElement.innerHTML = this.stretchedTooltipText;
             if (this.data.stretched) {
                 this.stretchBlockButton.innerHTML = btnUnstretched;
             } else {
                 this.stretchBlockButton.innerHTML = btnStretched;
             }
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -7,14 +7,21 @@
 
 const wagtailImageRowToolAddIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-node-plus" viewBox="0 0 16 16">
     <!-- The MIT License (MIT) -->
     <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
     <path fill-rule="evenodd" d="M11 4a4 4 0 1 0 0 8 4 4 0 0 0 0-8M6.025 7.5a5 5 0 1 1 0 1H4A1.5 1.5 0 0 1 2.5 10h-1A1.5 1.5 0 0 1 0 8.5v-1A1.5 1.5 0 0 1 1.5 6h1A1.5 1.5 0 0 1 4 7.5zM11 5a.5.5 0 0 1 .5.5v2h2a.5.5 0 0 1 0 1h-2v2a.5.5 0 0 1-1 0v-2h-2a.5.5 0 0 1 0-1h2v-2A.5.5 0 0 1 11 5M1.5 7a.5.5 0 0 0-.5.5v1a.5.5 0 0 0 .5.5h1a.5.5 0 0 0 .5-.5v-1a.5.5 0 0 0-.5-.5z"/>
 </svg>`
 
+const wagtailImageRowTrashCanIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-trash" viewBox="0 0 16 16">
+    <!-- The MIT License (MIT) -->
+    <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
+    <path d="M5.5 5.5A.5.5 0 0 1 6 6v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5m2.5 0a.5.5 0 0 1 .5.5v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5m3 .5a.5.5 0 0 0-1 0v6a.5.5 0 0 0 1 0z"/>
+    <path d="M14.5 3a1 1 0 0 1-1 1H13v9a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V4h-.5a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1H6a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1h3.5a1 1 0 0 1 1 1zM4.118 4 4 4.059V13a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V4.059L11.882 4zM2.5 3h11V2h-11z"/>
+</svg>`;
+
 
 class ImageRowTool extends window.BaseWagtailEditorJSTool {
     constructor({
         data,
         api,
         config,
         block
@@ -72,25 +79,15 @@
         return {
             title: 'Image Row',
             icon: wagtailImageRowToolIcon,
         };
     }
 
     addImage() {
-        this.imageChooser.openChooserModal();
-
-
-        let changeEventFunc;
-        changeEventFunc = () => {
-            const data = this.imageChooser.getState();
-            this._createImage(data);
-            this.imageChooser.input.removeEventListener('change', changeEventFunc);
-        };
-
-        this.imageChooser.input.addEventListener('change', changeEventFunc);
+        window.openChooserModal(this.imageChooser, this._createImage.bind(this));
     }
 
     _createImage(imageData) {
         const imageWrapper = this.imageRow.addElement('div', {
             className: 'wagtail-image-row-image-wrapper',
         });
 
@@ -98,14 +95,41 @@
             className: 'wagtail-image-row-image',
         });
 
         image.src = `${this.config.getImageUrl}${imageData.id}/`;
         image.alt = imageData.title;
         image.dataset.imageId = imageData.id;
         image.dataset.editUrl = imageData.edit_url;
+
+        const imageActions = imageWrapper.addElement('div', {
+            className: 'wagtail-image-row-image-actions',
+        });
+
+        const imageEdit = imageActions.addElement('button', {
+            className: 'wagtail-image-row-image-edit',
+            innerHTML: wagtailImageRowToolAddIcon,
+        });
+
+        imageEdit.addEventListener('click', () => {
+            openChooserModal(this.imageChooser, (data) => {
+                image.src = `${this.config.getImageUrl}${data.id}/`;
+                image.alt = data.title;
+                image.dataset.imageId = data.id;
+                image.dataset.editUrl = data.edit_url;
+            });
+        });
+
+        const imageDelete = imageActions.addElement('button', {
+            className: 'wagtail-image-row-image-delete',
+            innerHTML: wagtailImageRowTrashCanIcon,
+        });
+
+        imageDelete.addEventListener('click', () => {
+            imageWrapper.remove();
+        });
     }
 
     render() {
         this.wrapperElement = window.makeElement('div', {
             className: 'wagtail-image-row-wrapper',
         });
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -33,56 +33,66 @@
             allow_external_link: this.config.allow_external_link || true,
             allow_email_link: this.config.allow_email_link || true,
             allow_phone_link: this.config.allow_phone_link || true,
             allow_anchor_link: this.config.allow_anchor_link || true,
         };
 
         const cfg = {
-            url: window.chooserUrls.pageChooser,
+            url: this.config.chooserUrls.pageChooser,
             urlParams: urlParams,
             onload: window.PAGE_CHOOSER_MODAL_ONLOAD_HANDLERS,
             modelNames: ['wagtailcore.page'],
         };
 
         return new window.PageChooser(this.config.chooserId, cfg);
     }
 
     showActions(wrapperTag) {
         this.pageURLInput.value = wrapperTag.href;
 
         let chooseNewPageFunc = null;
         chooseNewPageFunc = (e) => {
-            const data = this.chooser.state;
-            this.setDataOnWrapper(wrapperTag, data);
-            this.pageURLInput.value = data.url;
+            this.setDataOnWrapper(wrapperTag, this.state);
+            this.pageURLInput.value = this.state.url;
             this.chooser.input.removeEventListener('change', chooseNewPageFunc);
         };
 
         this.chooseNewPageButton.onclick = (() => {
             this.chooser.openChooserModal();
             this.chooser.input.addEventListener('change', chooseNewPageFunc);
         });
 
         this.api.tooltip.onHover(this.chooseNewPageButton, this.api.i18n.t('Choose new ' + this.constructor["chooserType"]), {
             placement: 'top',
             hidingDelay: 200,
         });
 
         this.targetSelect.onchange = (e) => {
-            this.pageURLInput.target = e.target.value;
+            if (e.target.value) {
+                this.wrapperTag.target = e.target.value;
+                this.wrapperTag.dataset.target = e.target.value;
+            } else if (this.wrapperTag.target) {
+                this.wrapperTag.removeAttribute('target');
+                delete this.wrapperTag.dataset.target;
+            }
         };
 
         this.relSelect.onchange = (e) => {
             if (!e.target.value && this.pageURLInput.rel) {
-                this.pageURLInput.removeAttribute('rel');
+                this.wrapperTag.removeAttribute('rel');
+                delete this.wrapperTag.dataset.rel;
             } else {
-                this.pageURLInput.rel = e.target.value;
+                this.wrapperTag.rel = e.target.value;
+                this.wrapperTag.dataset.rel = e.target.value;
             }
         }
 
+        this.relSelect.value = wrapperTag.rel || '';
+        this.targetSelect.value = wrapperTag.target || '';
+
         this.container.hidden = false;
 
 
     }
 
     hideActions() {
         this.container.hidden = true;
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt` & `wagtail_editorjs-1.6.0/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html` & `wagtail_editorjs-1.6.0/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc` & `wagtail_editorjs-1.6.0/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/tests/test_attrs.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_attrs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.test import TestCase
-from ..registry.element.element import EditorJSElement
-from ..registry.element.utils import (
+from wagtail_editorjs.registry.element.element import EditorJSElement
+from wagtail_editorjs.registry.element.utils import (
     wrap_tag,
     _make_attr,
     add_attributes,
     EditorJSElementAttribute,
     EditorJSStyleAttribute,
 )
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/tests/test_render.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/test_render.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from bs4 import BeautifulSoup
 
-from .utils import BaseEditorJSTest
-from ..render import render_editorjs_html
-from ..registry import (
+from .base import BaseEditorJSTest
+from wagtail_editorjs.render import render_editorjs_html
+from wagtail_editorjs.registry import (
     EditorJSTune,
     EditorJSFeature,
     EditorJSElement,
     EDITOR_JS_FEATURES,
 )
 
 
@@ -81,15 +81,15 @@
         soup2 = BeautifulSoup(rendered_2, "html.parser")
 
         d1 = soup1.decode(False)
         d2 = soup2.decode(False)
         self.assertHTMLEqual(
             d1, d2,
             msg=(
-                "The rendered HTML does not match the expected output.\n"
+                f"The rendered HTML for feature {feature} does not match the expected output.\n"
                 "This might be due to a change in the rendering process.\n\n"
                 "Expected: {expected}\n\n"
                 "Got: {got}" % {
                     "expected": d1,
                     "got": d2,
                 }
             )
@@ -127,15 +127,15 @@
             EDITOR_JS_FEATURES.keys(),
             {"blocks": test_data},
             clean=True,
         )
 
         soup = BeautifulSoup(rendered, "html.parser")
 
-        for data in test_data:
+        for i, data in enumerate(test_data):
             block = soup.find(attrs={"data-testing-id": data["tunes"]["test_tune_feature"]})
 
             if not block:
                 self.fail(
                     f"Block with id {data['tunes']['test_tune_feature']} not found.\n"
                     "The tune might not have been properly applied. Check the test data.\n\n"
                     f"Test data: {data}\n\n"
@@ -147,15 +147,15 @@
             element = self.tune.tune_element(element, data["tunes"]["test_tune_feature"])
 
             soup_element = BeautifulSoup(str(element), "html.parser")
 
             self.assertHTMLEqual(
                 str(block).replace("\n", "").strip(), str(soup_element).replace("\n", "").strip(),
                 msg=(
-                    "Block with id {feature} does not match the expected output.\n"
+                    f"Block with feature {feature} ({i}) does not match the expected output.\n"
                     "Something has gone wrong with the cleaning process.\n\n"
                     "Expected: {expected}\n\n"
                     "Got: {got}" % {
                         "feature": data['tunes']['test_tune_feature'],
                         "expected": str(soup_element).replace('\n', '').strip(),
                         "got": str(block).replace('\n', '').strip(),
                     }
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/tests/utils.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/test/core/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,22 @@
     get_test_image_file,
     get_test_image_file_jpeg,
     get_test_image_file_webp,
     get_test_image_file_avif,
 )
 from wagtail.images import get_image_model
 from wagtail.documents import get_document_model
+from wagtail_editorjs import settings
 
 
 Image = get_image_model()
 Document = get_document_model()
 
 
+
 class BaseEditorJSTest(TestCase):
     """
         Setup test data for EditorJS tests
         This is so blocks can freely be tested and query the test db
         without having to worry about setting up the data.
     """
     def setUp(self) -> None:
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/wagtail_hooks/features.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     CodeFeature,
     DelimiterFeature,
     WarningFeature,
     HeaderFeature,
     HTMLFeature,
     ImageFeature,
     ImageRowFeature,
+    ButtonFeature,
     LinkFeature,
     LinkAutoCompleteFeature,
     DocumentFeature,
     NestedListFeature,
     TableFeature,
     AlignmentBlockTune,
     TextVariantTune,
@@ -164,14 +165,20 @@
         LinkAutoCompleteFeature(
             "link-autocomplete",
         ),
     )
 
     # Wagtail specific
     registry.register(
+        "button",
+        ButtonFeature(
+            "button",
+        )
+    )
+    registry.register(
         "link",
         LinkFeature(
             "link",
             inlineToolbar = True,
         ),
     )
     registry.register(
@@ -250,14 +257,15 @@
                 "wagtail_editorjs/vendor/editorjs/tools/drag-drop.js",
                 "wagtail_editorjs/js/init/drag-drop.js",
             ],
             weight=1,
         ),
     )
 
+
     # Add tunes
     registry.register_tune("text-alignment-tune")
     registry.register_tune("text-variant-tune")
     registry.register_tune("background-color-tune")
     registry.register_tune("text-color-tune")
```

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs/wagtail_hooks/urls.py` & `wagtail_editorjs-1.6.0/wagtail_editorjs/wagtail_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.5.9/wagtail_editorjs.egg-info/SOURCES.txt` & `wagtail_editorjs-1.6.0/wagtail_editorjs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
 wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
 wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
 wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
 wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
 wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
@@ -74,21 +75,33 @@
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
 wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
 wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
 wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
 wagtail_editorjs/templatetags/__init__.py
 wagtail_editorjs/templatetags/editorjs.py
 wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
-wagtail_editorjs/tests/__init__.py
-wagtail_editorjs/tests/test_attrs.py
-wagtail_editorjs/tests/test_inlines.py
-wagtail_editorjs/tests/test_render.py
-wagtail_editorjs/tests/utils.py
+wagtail_editorjs/test/__init__.py
+wagtail_editorjs/test/manage.py
+wagtail_editorjs/test/core/__init__.py
+wagtail_editorjs/test/core/apps.py
+wagtail_editorjs/test/core/migrations/__init__.py
+wagtail_editorjs/test/core/tests/__init__.py
+wagtail_editorjs/test/core/tests/base.py
+wagtail_editorjs/test/core/tests/test_attrs.py
+wagtail_editorjs/test/core/tests/test_inlines.py
+wagtail_editorjs/test/core/tests/test_render.py
+wagtail_editorjs/test/testapp/__init__.py
+wagtail_editorjs/test/testapp/asgi.py
+wagtail_editorjs/test/testapp/settings.py
+wagtail_editorjs/test/testapp/urls.py
+wagtail_editorjs/test/testapp/wsgi.py
 wagtail_editorjs/wagtail_hooks/__init__.py
 wagtail_editorjs/wagtail_hooks/features.py
-wagtail_editorjs/wagtail_hooks/urls.py
+wagtail_editorjs/wagtail_hooks/urls.py
+wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
```

