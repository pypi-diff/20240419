# Comparing `tmp/globlocks-1.1.8.tar.gz` & `tmp/globlocks-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globlocks-1.1.8.tar", last modified: Sat Mar 16 17:17:00 2024, max compression
+gzip compressed data, was "globlocks-1.1.9.tar", last modified: Fri Apr 19 07:11:30 2024, max compression
```

## Comparing `globlocks-1.1.8.tar` & `globlocks-1.1.9.tar`

### file list

```diff
@@ -1,283 +1,294 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.487710 globlocks-1.1.8/
--rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1253 2024-03-16 17:17:00.487710 globlocks-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-03-01 12:36:04.000000 globlocks-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.103211 globlocks-1.1.8/globlocks/
--rw-rw-rw-   0        0        0      620 2024-03-16 17:16:55.000000 globlocks-1.1.8/globlocks/__init__.py
--rw-rw-rw-   0        0        0      156 2024-03-01 09:12:55.000000 globlocks-1.1.8/globlocks/apps.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.157992 globlocks-1.1.8/globlocks/blocks/
--rw-rw-rw-   0        0        0      447 2024-03-11 15:58:03.000000 globlocks-1.1.8/globlocks/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.178640 globlocks-1.1.8/globlocks/blocks/bases/
--rw-rw-rw-   0        0        0      251 2024-03-11 15:57:48.000000 globlocks-1.1.8/globlocks/blocks/bases/__init__.py
--rw-rw-rw-   0        0        0    12943 2024-03-12 19:11:57.000000 globlocks-1.1.8/globlocks/blocks/bases/baseblock.py
--rw-rw-rw-   0        0        0     9540 2024-03-16 12:44:06.000000 globlocks-1.1.8/globlocks/blocks/bases/visibility.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.190475 globlocks-1.1.8/globlocks/blocks/block_fields/
--rw-rw-rw-   0        0        0      292 2024-03-15 20:11:04.000000 globlocks-1.1.8/globlocks/blocks/block_fields/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.209653 globlocks-1.1.8/globlocks/blocks/block_fields/colorblock/
--rw-rw-rw-   0        0        0       34 2023-09-19 19:43:14.000000 globlocks-1.1.8/globlocks/blocks/block_fields/colorblock/__init__.py
--rw-rw-rw-   0        0        0      778 2024-03-01 09:20:41.000000 globlocks-1.1.8/globlocks/blocks/block_fields/colorblock/colorblock.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.225180 globlocks-1.1.8/globlocks/blocks/block_fields/fontpicker/
--rw-rw-rw-   0        0        0       39 2023-09-19 19:26:48.000000 globlocks-1.1.8/globlocks/blocks/block_fields/fontpicker/__init__.py
--rw-rw-rw-   0        0        0     1228 2024-03-01 09:20:36.000000 globlocks-1.1.8/globlocks/blocks/block_fields/fontpicker/fontpicker.py
--rw-rw-rw-   0        0        0      553 2024-03-11 13:34:53.000000 globlocks-1.1.8/globlocks/blocks/block_fields/justify.py
--rw-rw-rw-   0        0        0     2058 2024-03-12 18:10:54.000000 globlocks-1.1.8/globlocks/blocks/block_fields/orderable_block.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.240384 globlocks-1.1.8/globlocks/blocks/block_fields/rangeslider/
--rw-rw-rw-   0        0        0       41 2023-09-19 19:26:58.000000 globlocks-1.1.8/globlocks/blocks/block_fields/rangeslider/__init__.py
--rw-rw-rw-   0        0        0     1510 2024-03-01 09:20:29.000000 globlocks-1.1.8/globlocks/blocks/block_fields/rangeslider/rangeslider.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.297757 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/
--rw-rw-rw-   0        0        0      644 2024-03-11 13:43:25.000000 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/__init__.py
--rw-rw-rw-   0        0        0     4956 2024-03-15 21:07:59.000000 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/bar.py
--rw-rw-rw-   0        0        0     4372 2024-03-12 09:33:22.000000 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/element.py
--rw-rw-rw-   0        0        0      774 2024-03-11 14:19:30.000000 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/toolbar_field.py
--rw-rw-rw-   0        0        0     2651 2024-03-11 14:40:08.000000 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
--rw-rw-rw-   0        0        0     5108 2024-03-12 09:34:47.000000 globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.315938 globlocks-1.1.8/globlocks/blocks/components/
--rw-rw-rw-   0        0        0      191 2024-03-12 17:14:03.000000 globlocks-1.1.8/globlocks/blocks/components/__init__.py
--rw-rw-rw-   0        0        0     1633 2024-03-12 17:35:42.000000 globlocks-1.1.8/globlocks/blocks/components/heading.py
--rw-rw-rw-   0        0        0     2105 2024-03-16 11:36:53.000000 globlocks-1.1.8/globlocks/blocks/components/image_text.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.325308 globlocks-1.1.8/globlocks/blocks/components/menus/
--rw-rw-rw-   0        0        0        0 2024-03-15 19:52:15.000000 globlocks-1.1.8/globlocks/blocks/components/menus/__init__.py
--rw-rw-rw-   0        0        0      669 2024-03-15 20:17:25.000000 globlocks-1.1.8/globlocks/blocks/components/menus/flat.py
--rw-rw-rw-   0        0        0        0 2024-03-15 19:52:51.000000 globlocks-1.1.8/globlocks/blocks/components/menus/layered.py
--rw-rw-rw-   0        0        0     1242 2024-03-12 19:40:38.000000 globlocks-1.1.8/globlocks/blocks/components/text.py
--rw-rw-rw-   0        0        0     5408 2024-03-12 17:36:16.000000 globlocks-1.1.8/globlocks/blocks/richtext.py
--rw-rw-rw-   0        0        0     3386 2024-03-05 11:02:40.000000 globlocks-1.1.8/globlocks/blocks/template.py
--rw-rw-rw-   0        0        0     3134 2024-03-10 19:13:29.000000 globlocks-1.1.8/globlocks/colors.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.360116 globlocks-1.1.8/globlocks/fields/
--rw-rw-rw-   0        0        0      154 2024-03-10 17:09:09.000000 globlocks-1.1.8/globlocks/fields/__init__.py
--rw-rw-rw-   0        0        0      292 2023-09-20 14:22:36.000000 globlocks-1.1.8/globlocks/fields/colorfield.py
--rw-rw-rw-   0        0        0     3568 2024-03-01 09:16:42.000000 globlocks-1.1.8/globlocks/fields/fontfield.py
--rw-rw-rw-   0        0        0     5396 2024-03-15 21:07:34.000000 globlocks-1.1.8/globlocks/fields/orderablefield.py
--rw-rw-rw-   0        0        0     4533 2024-03-10 19:00:38.000000 globlocks-1.1.8/globlocks/fonts.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.013460 globlocks-1.1.8/globlocks/locale/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.012460 globlocks-1.1.8/globlocks/locale/en/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.372490 globlocks-1.1.8/globlocks/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      380 2024-03-08 23:37:35.000000 globlocks-1.1.8/globlocks/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3183 2024-03-08 23:35:00.000000 globlocks-1.1.8/globlocks/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.013460 globlocks-1.1.8/globlocks/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.383533 globlocks-1.1.8/globlocks/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1711 2024-03-08 23:28:33.000000 globlocks-1.1.8/globlocks/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3549 2024-03-08 23:28:23.000000 globlocks-1.1.8/globlocks/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      552 2024-02-29 14:32:14.000000 globlocks-1.1.8/globlocks/panels.py
--rw-rw-rw-   0        0        0     1682 2024-03-01 09:19:16.000000 globlocks-1.1.8/globlocks/preview.py
--rw-rw-rw-   0        0        0    10553 2024-03-12 17:41:54.000000 globlocks-1.1.8/globlocks/rt_extensions.py
--rw-rw-rw-   0        0        0     3121 2024-03-16 11:44:43.000000 globlocks-1.1.8/globlocks/settings.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.013460 globlocks-1.1.8/globlocks/static/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.016620 globlocks-1.1.8/globlocks/static/globlocks/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.386533 globlocks-1.1.8/globlocks/static/globlocks/admin/
--rw-rw-rw-   0        0        0     1133 2024-03-09 19:16:02.000000 globlocks-1.1.8/globlocks/static/globlocks/admin/block_settings.js
--rw-rw-rw-   0        0        0    20720 2024-03-15 22:39:46.000000 globlocks-1.1.8/globlocks/static/globlocks/admin/layout.css
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.390117 globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/
--rw-rw-rw-   0        0        0     9564 2024-03-16 17:15:12.000000 globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
--rw-rw-rw-   0        0        0     3295 2024-03-16 16:54:05.000000 globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
--rw-rw-rw-   0        0        0     6365 2024-03-16 15:45:59.000000 globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.391086 globlocks-1.1.8/globlocks/static/globlocks/css/
--rw-rw-rw-   0        0        0     1722 2024-03-16 13:01:30.000000 globlocks-1.1.8/globlocks/static/globlocks/css/blocks.css
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.779350 globlocks-1.1.8/globlocks/static/globlocks/fonts/
--rw-rw-rw-   0        0        0    21948 2023-09-05 20:43:14.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Acme-Regular.ttf
--rw-rw-rw-   0        0        0    92956 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
--rw-rw-rw-   0        0        0   142696 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
--rw-rw-rw-   0        0        0    92468 2023-07-24 18:16:58.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
--rw-rw-rw-   0        0        0    57676 2023-09-05 20:40:40.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
--rw-rw-rw-   0        0        0   256900 2023-09-05 20:42:58.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
--rw-rw-rw-   0        0        0    61368 2022-09-22 05:27:10.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
--rw-rw-rw-   0        0        0    26000 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
--rw-rw-rw-   0        0        0    97864 2023-09-05 20:41:08.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
--rw-rw-rw-   0        0        0   309828 2023-09-05 11:41:12.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Inter-Regular.ttf
--rw-rw-rw-   0        0        0    41676 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
--rw-rw-rw-   0        0        0   169744 2023-09-05 11:40:48.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
--rw-rw-rw-   0        0        0    75152 2023-09-05 11:41:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Lato-Regular.ttf
--rw-rw-rw-   0        0        0   396740 2023-09-05 20:40:54.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
--rw-rw-rw-   0        0        0   234956 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
--rw-rw-rw-   0        0        0    96832 2023-09-05 20:40:12.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
--rw-rw-rw-   0        0        0    49908 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
--rw-rw-rw-   0        0        0   197976 2023-09-05 11:41:32.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
--rw-rw-rw-   0        0        0   556216 2023-09-05 11:41:36.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
--rw-rw-rw-   0        0        0    87252 2023-09-05 11:41:56.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0        0        0   169480 2022-09-22 05:27:10.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
--rw-rw-rw-   0        0        0   315408 2023-09-05 20:40:46.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
--rw-rw-rw-   0        0        0    33876 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
--rw-rw-rw-   0        0        0    73620 2023-09-05 20:43:28.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
--rw-rw-rw-   0        0        0   109192 2022-09-22 05:27:10.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
--rw-rw-rw-   0        0        0    65396 2023-09-05 11:42:00.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
--rw-rw-rw-   0        0        0   158240 2023-09-05 11:42:04.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
--rw-rw-rw-   0        0        0   168260 2023-09-05 11:42:14.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   166836 2023-09-05 11:42:26.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
--rw-rw-rw-   0        0        0    86908 2023-09-05 11:42:30.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0   119328 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
--rw-rw-rw-   0        0        0   207632 2023-09-05 11:42:38.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
--rw-rw-rw-   0        0        0   132092 2023-09-05 11:42:42.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
--rw-rw-rw-   0        0        0   117132 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
--rw-rw-rw-   0        0        0    64808 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
--rw-rw-rw-   0        0        0    48468 2023-09-05 20:42:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
--rw-rw-rw-   0        0        0    42756 2022-09-22 05:27:10.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
--rw-rw-rw-   0        0        0    90904 2023-06-22 20:54:32.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
--rw-rw-rw-   0        0        0    40160 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
--rw-rw-rw-   0        0        0   299684 2023-09-05 11:42:46.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
--rw-rw-rw-   0        0        0    51084 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
--rw-rw-rw-   0        0        0   244332 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0   192904 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0    57468 2023-08-25 17:51:24.000000 globlocks-1.1.8/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.016620 globlocks-1.1.8/globlocks/static/globlocks/richtext/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.781360 globlocks-1.1.8/globlocks/static/globlocks/richtext/alignment/
--rw-rw-rw-   0        0        0      558 2024-03-11 21:42:52.000000 globlocks-1.1.8/globlocks/static/globlocks/richtext/alignment/alignment.css
--rw-rw-rw-   0        0        0     5653 2024-03-15 21:06:55.000000 globlocks-1.1.8/globlocks/static/globlocks/richtext/alignment/alignment.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.782362 globlocks-1.1.8/globlocks/static/globlocks/richtext/rt_extensions/
--rw-rw-rw-   0        0        0     1920 2024-03-11 20:56:47.000000 globlocks-1.1.8/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.783362 globlocks-1.1.8/globlocks/static/globlocks/widgets/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.796894 globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/
--rw-rw-rw-   0        0        0     1097 2024-03-10 13:15:59.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/LICENSE
--rw-rw-rw-   0        0        0      488 2024-03-01 09:28:55.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
--rw-rw-rw-   0        0        0     3755 2023-11-05 19:34:36.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
--rw-rw-rw-   0        0        0     9002 2023-09-07 08:18:46.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/pickr.css
--rw-rw-rw-   0        0        0    23556 2023-09-07 08:09:12.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/pickr.min.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.834329 globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/
--rw-rw-rw-   0        0        0      581 2024-03-01 09:28:55.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
--rw-rw-rw-   0        0        0     3307 2024-03-01 12:55:55.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
--rw-rw-rw-   0        0        0     1070 2023-09-11 10:30:02.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/font-picker.css
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.838837 globlocks-1.1.8/globlocks/static/globlocks/widgets/justify/
--rw-rw-rw-   0        0        0      577 2024-03-09 15:01:52.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/justify/justify-controller.js
--rw-rw-rw-   0        0        0     1656 2024-03-10 22:06:01.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/justify/justify-widget.css
--rw-rw-rw-   0        0        0     3894 2024-03-10 23:34:39.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/justify/justify-widget.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.843003 globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/
--rw-rw-rw-   0        0        0      516 2024-03-01 09:28:55.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
--rw-rw-rw-   0        0        0      800 2023-09-05 09:10:26.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/orderable.css
--rw-rw-rw-   0        0        0     2222 2023-09-10 21:13:12.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/orderable.js
--rw-rw-rw-   0        0        0    44136 2023-09-05 08:17:10.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.845419 globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/
--rw-rw-rw-   0        0        0      578 2024-03-01 09:28:55.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
--rw-rw-rw-   0        0        0     1152 2023-09-10 16:39:38.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/range-slider.css
--rw-rw-rw-   0        0        0     2164 2023-12-11 20:53:33.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/range-slider.js
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.848918 globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/
--rw-rw-rw-   0        0        0      970 2024-03-11 17:49:05.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
--rw-rw-rw-   0        0        0      810 2024-03-10 14:09:52.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
--rw-rw-rw-   0        0        0    16889 2024-03-15 20:38:00.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
--rw-rw-rw-   0        0        0      796 2024-03-10 21:47:01.000000 globlocks-1.1.8/globlocks/static/globlocks/widgets/utils.js
--rw-rw-rw-   0        0        0      344 2024-03-10 19:06:51.000000 globlocks-1.1.8/globlocks/staticfiles.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.024467 globlocks-1.1.8/globlocks/templates/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.023019 globlocks-1.1.8/globlocks/templates/globlocks/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.022019 globlocks-1.1.8/globlocks/templates/globlocks/blocks/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.022019 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.856611 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/heading/
--rw-rw-rw-   0        0        0      231 2024-03-12 09:46:10.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/heading/heading.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.865103 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image/
--rw-rw-rw-   0        0        0       78 2024-03-12 15:31:18.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image/image.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.901276 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image_text/
--rw-rw-rw-   0        0        0      350 2024-03-12 15:45:29.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image_text/image.html
--rw-rw-rw-   0        0        0      376 2024-03-12 15:44:55.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
--rw-rw-rw-   0        0        0      588 2024-03-12 17:44:34.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
--rw-rw-rw-   0        0        0      387 2024-03-15 21:06:29.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image_text/text.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.905280 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/text/
--rw-rw-rw-   0        0        0      118 2024-03-12 14:59:13.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/text/text.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.969472 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/
--rw-rw-rw-   0        0        0      221 2024-03-12 08:53:51.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/heading.html
--rw-rw-rw-   0        0        0      355 2024-03-10 17:19:07.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
--rw-rw-rw-   0        0        0      114 2024-03-09 09:56:15.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/listblock.html
--rw-rw-rw-   0        0        0      241 2024-03-09 10:08:00.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/richtext.html
--rw-rw-rw-   0        0        0      238 2024-03-10 16:23:21.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/settings_form.html
--rw-rw-rw-   0        0        0      363 2024-03-09 09:47:59.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
--rw-rw-rw-   0        0        0      361 2024-03-10 16:23:49.000000 globlocks-1.1.8/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.023019 globlocks-1.1.8/globlocks/templates/globlocks/icons/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.003324 globlocks-1.1.8/globlocks/templates/globlocks/icons/text-align/
--rw-rw-rw-   0        0        0      465 2024-03-08 23:15:34.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/text-align/text-center.svg
--rw-rw-rw-   0        0        0      468 2024-03-15 20:17:13.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/text-align/text-justify.svg
--rw-rw-rw-   0        0        0      461 2024-03-15 20:15:50.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/text-align/text-left.svg
--rw-rw-rw-   0        0        0      464 2024-03-08 23:15:13.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/text-align/text-right.svg
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.118239 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/
--rw-rw-rw-   0        0        0      549 2024-03-10 14:29:53.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
--rw-rw-rw-   0        0        0      338 2024-03-10 14:29:50.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
--rw-rw-rw-   0        0        0      546 2024-03-10 14:29:47.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
--rw-rw-rw-   0        0        0      711 2024-03-10 14:29:43.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
--rw-rw-rw-   0        0        0      430 2024-03-10 14:29:39.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
--rw-rw-rw-   0        0        0      596 2024-03-10 14:29:34.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
--rw-rw-rw-   0        0        0      712 2024-03-10 14:29:31.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
--rw-rw-rw-   0        0        0      426 2024-03-10 14:29:28.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
--rw-rw-rw-   0        0        0      542 2024-03-10 14:33:24.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
--rw-rw-rw-   0        0        0      872 2024-03-10 14:32:47.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
--rw-rw-rw-   0        0        0      654 2024-03-10 14:29:23.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
--rw-rw-rw-   0        0        0      409 2024-03-10 14:29:19.000000 globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.023019 globlocks-1.1.8/globlocks/templates/globlocks/shared/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.156892 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/
--rw-rw-rw-   0        0        0      167 2024-03-12 09:45:07.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/base.html
--rw-rw-rw-   0        0        0      850 2024-03-12 09:43:48.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/heading.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.159918 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/images/
--rw-rw-rw-   0        0        0        0 2024-03-12 15:31:58.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/images/base.html
--rw-rw-rw-   0        0        0        0 2024-03-12 15:31:32.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/images/full.html
--rw-rw-rw-   0        0        0        0 2024-03-12 15:31:42.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/images/large.html
--rw-rw-rw-   0        0        0        0 2024-03-12 15:32:09.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/images/medium.html
--rw-rw-rw-   0        0        0        0 2024-03-12 15:32:05.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/images/small.html
--rw-rw-rw-   0        0        0      309 2024-03-15 21:08:51.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/listblock.html
--rw-rw-rw-   0        0        0      317 2024-03-12 09:45:57.000000 globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/text.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.221239 globlocks-1.1.8/globlocks/templates/globlocks/widgets/
--rw-rw-rw-   0        0        0      360 2023-11-19 18:46:26.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/color-input-widget.html
--rw-rw-rw-   0        0        0     1999 2023-10-04 17:59:30.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/font_picker_widget.html
--rw-rw-rw-   0        0        0      487 2024-03-15 20:20:46.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/justify-widget-option.html
--rw-rw-rw-   0        0        0      421 2024-03-09 15:17:42.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/justify-widget.html
--rw-rw-rw-   0        0        0      624 2023-09-05 12:05:32.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/orderable_widget.html
--rw-rw-rw-   0        0        0      873 2023-11-19 19:04:24.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/slider_input.html
--rw-rw-rw-   0        0        0     1052 2024-03-09 21:15:59.000000 globlocks-1.1.8/globlocks/templates/globlocks/widgets/toolbar-widget.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:16:59.024467 globlocks-1.1.8/globlocks/templates/wagtailadmin/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.256559 globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/
--rw-rw-rw-   0        0        0      678 2024-03-12 17:48:47.000000 globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block.html
--rw-rw-rw-   0        0        0      399 2024-03-09 09:11:06.000000 globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
--rw-rw-rw-   0        0        0      542 2024-03-12 08:53:41.000000 globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
--rw-rw-rw-   0        0        0     1081 2024-03-11 16:16:11.000000 globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.268864 globlocks-1.1.8/globlocks/templatetags/
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.274511 globlocks-1.1.8/globlocks/templatetags/__pycache__/
--rw-rw-rw-   0        0        0     6328 2024-03-12 08:18:16.000000 globlocks-1.1.8/globlocks/templatetags/__pycache__/globlocks.cpython-311.pyc
--rw-rw-rw-   0        0        0      951 2024-03-04 15:09:25.000000 globlocks-1.1.8/globlocks/templatetags/__pycache__/globlocks_admin.cpython-311.pyc
--rw-rw-rw-   0        0        0     3844 2024-03-11 14:35:58.000000 globlocks-1.1.8/globlocks/templatetags/__pycache__/globlocks_toolbar.cpython-311.pyc
--rw-rw-rw-   0        0        0     4248 2024-03-12 17:29:51.000000 globlocks-1.1.8/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.311062 globlocks-1.1.8/globlocks/templatetags/globlocks/
--rw-rw-rw-   0        0        0     4246 2024-03-12 08:55:59.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.318657 globlocks-1.1.8/globlocks/templatetags/globlocks/__pycache__/
--rw-rw-rw-   0        0        0     6337 2024-03-12 08:56:05.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      951 2024-03-12 08:53:56.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
--rw-rw-rw-   0        0        0     6333 2024-03-12 08:55:10.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/__pycache__/main.cpython-311.pyc
--rw-rw-rw-   0        0        0     3603 2024-03-12 09:37:09.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
--rw-rw-rw-   0        0        0     1503 2024-03-12 09:02:39.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0      613 2024-03-12 08:53:09.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/admin.py
--rw-rw-rw-   0        0        0     2273 2024-03-12 09:37:03.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/toolbar.py
--rw-rw-rw-   0        0        0      803 2024-03-12 09:02:36.000000 globlocks-1.1.8/globlocks/templatetags/globlocks/utils.py
--rw-rw-rw-   0        0        0     2463 2024-02-01 09:34:50.000000 globlocks-1.1.8/globlocks/templatetags/orderable_tags.py
--rw-rw-rw-   0        0        0       63 2024-03-01 09:12:55.000000 globlocks-1.1.8/globlocks/tests.py
--rw-rw-rw-   0        0        0     1832 2024-03-12 17:29:10.000000 globlocks-1.1.8/globlocks/util.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.369886 globlocks-1.1.8/globlocks/wagtail_hooks/
--rw-rw-rw-   0        0        0       84 2024-03-12 07:52:13.000000 globlocks-1.1.8/globlocks/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      495 2024-03-08 21:45:48.000000 globlocks-1.1.8/globlocks/wagtail_hooks/admin_hooks.py
--rw-rw-rw-   0        0        0     4327 2024-03-12 19:05:52.000000 globlocks-1.1.8/globlocks/wagtail_hooks/alignment.py
--rw-rw-rw-   0        0        0      955 2024-03-10 14:33:44.000000 globlocks-1.1.8/globlocks/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     1511 2024-03-12 19:01:04.000000 globlocks-1.1.8/globlocks/wagtail_hooks/rt_extensions.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.422794 globlocks-1.1.8/globlocks/widgets/
--rw-rw-rw-   0        0        0      295 2024-03-10 17:09:14.000000 globlocks-1.1.8/globlocks/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-03-01 09:28:55.000000 globlocks-1.1.8/globlocks/widgets/color_input_widget.py
--rw-rw-rw-   0        0        0     3341 2024-03-01 09:22:26.000000 globlocks-1.1.8/globlocks/widgets/fontpicker.py
--rw-rw-rw-   0        0        0     1660 2024-03-15 20:20:49.000000 globlocks-1.1.8/globlocks/widgets/justify_widget.py
--rw-rw-rw-   0        0        0     1898 2024-03-01 09:21:22.000000 globlocks-1.1.8/globlocks/widgets/orderable.py
--rw-rw-rw-   0        0        0     1692 2024-03-01 09:21:30.000000 globlocks-1.1.8/globlocks/widgets/range_input.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.486700 globlocks-1.1.8/globlocks.egg-info/
--rw-rw-rw-   0        0        0     1253 2024-03-16 17:16:58.000000 globlocks-1.1.8/globlocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11040 2024-03-16 17:16:58.000000 globlocks-1.1.8/globlocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 17:16:58.000000 globlocks-1.1.8/globlocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-03-16 17:16:58.000000 globlocks-1.1.8/globlocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-16 17:16:58.000000 globlocks-1.1.8/globlocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0     1028 2024-03-16 17:17:00.495290 globlocks-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.423798 globlocks-1.1.8/tests/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.433334 globlocks-1.1.8/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.444880 globlocks-1.1.8/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.446167 globlocks-1.1.8/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:17:00.485186 globlocks-1.1.8/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.1.8/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.214935 globlocks-1.1.9/
+-rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1984 2024-04-19 07:11:30.214935 globlocks-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2024-03-19 08:19:55.000000 globlocks-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.429346 globlocks-1.1.9/globlocks/
+-rw-rw-rw-   0        0        0      620 2024-04-19 07:11:25.000000 globlocks-1.1.9/globlocks/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.461919 globlocks-1.1.9/globlocks/blocks/
+-rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.471404 globlocks-1.1.9/globlocks/blocks/bases/
+-rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/__init__.py
+-rw-rw-rw-   0        0        0    13076 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/baseblock.py
+-rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/template.py
+-rw-rw-rw-   0        0        0    10194 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.477592 globlocks-1.1.9/globlocks/blocks/block_fields/
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.480871 globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/
+-rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/__init__.py
+-rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/colorblock.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.481524 globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/
+-rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/__init__.py
+-rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/fontpicker.py
+-rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/justify.py
+-rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/orderable_block.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.488776 globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/
+-rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/__init__.py
+-rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/rangeslider.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.500032 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/
+-rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/__init__.py
+-rw-rw-rw-   0        0        0     4956 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/bar.py
+-rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/element.py
+-rw-rw-rw-   0        0        0      774 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_field.py
+-rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
+-rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.508710 globlocks-1.1.9/globlocks/blocks/components/
+-rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/__init__.py
+-rw-rw-rw-   0        0        0     1603 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/heading.py
+-rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/image.py
+-rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/image_text.py
+-rw-rw-rw-   0        0        0     9047 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/link.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.513187 globlocks-1.1.9/globlocks/blocks/components/menus/
+-rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/menus/__init__.py
+-rw-rw-rw-   0        0        0     2567 2024-03-19 09:11:52.000000 globlocks-1.1.9/globlocks/blocks/components/menus/flat.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/menus/layered.py
+-rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/text.py
+-rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/richtext.py
+-rw-rw-rw-   0        0        0      425 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/utils.py
+-rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/choices.py
+-rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.520328 globlocks-1.1.9/globlocks/fields/
+-rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/colorfield.py
+-rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/fontfield.py
+-rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/orderablefield.py
+-rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fonts.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.341140 globlocks-1.1.9/globlocks/locale/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.340140 globlocks-1.1.9/globlocks/locale/en/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.532263 globlocks-1.1.9/globlocks/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.342137 globlocks-1.1.9/globlocks/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.546064 globlocks-1.1.9/globlocks/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3549 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/panels.py
+-rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/preview.py
+-rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/rt_extensions.py
+-rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.343141 globlocks-1.1.9/globlocks/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.351616 globlocks-1.1.9/globlocks/static/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.583064 globlocks-1.1.9/globlocks/static/globlocks/admin/
+-rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/block_settings.js
+-rw-rw-rw-   0        0        0    24293 2024-03-26 09:23:48.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/layout.css
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.622376 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/
+-rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
+-rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
+-rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.645282 globlocks-1.1.9/globlocks/static/globlocks/css/
+-rw-rw-rw-   0        0        0     8847 2024-03-19 12:00:45.000000 globlocks-1.1.9/globlocks/static/globlocks/css/blocks.css
+-rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.1.9/globlocks/static/globlocks/css/bootstrap.css
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.113700 globlocks-1.1.9/globlocks/static/globlocks/fonts/
+-rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Acme-Regular.ttf
+-rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
+-rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
+-rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
+-rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
+-rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
+-rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
+-rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
+-rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
+-rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Inter-Regular.ttf
+-rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
+-rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
+-rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
+-rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
+-rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
+-rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
+-rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
+-rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
+-rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
+-rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
+-rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
+-rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
+-rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
+-rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
+-rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
+-rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
+-rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
+-rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
+-rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
+-rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
+-rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
+-rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
+-rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
+-rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
+-rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
+-rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
+-rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
+-rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.349109 globlocks-1.1.9/globlocks/static/globlocks/richtext/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.132649 globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/
+-rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.css
+-rw-rw-rw-   0        0        0     5728 2024-04-19 07:10:50.000000 globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.143434 globlocks-1.1.9/globlocks/static/globlocks/richtext/rt_extensions/
+-rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.163953 globlocks-1.1.9/globlocks/static/globlocks/widgets/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.289623 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/
+-rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
+-rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:49.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
+-rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.css
+-rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.341792 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/
+-rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
+-rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
+-rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker.css
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.381066 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/
+-rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-controller.js
+-rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.css
+-rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.473830 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/
+-rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
+-rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.css
+-rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.js
+-rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.515906 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/
+-rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
+-rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.css
+-rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.574915 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/
+-rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
+-rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
+-rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
+-rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/utils.js
+-rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.1.9/globlocks/staticfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.375470 globlocks-1.1.9/globlocks/templates/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.373466 globlocks-1.1.9/globlocks/templates/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.368673 globlocks-1.1.9/globlocks/templates/globlocks/blocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.367662 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.576258 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/heading/
+-rw-rw-rw-   0        0        0      257 2024-03-19 10:10:04.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/heading/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.625806 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/
+-rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/full.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/large.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/medium.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/small.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.664260 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/
+-rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image.html
+-rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
+-rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
+-rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.677406 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/link/
+-rw-rw-rw-   0        0        0     1655 2024-03-19 08:35:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/link/form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.366211 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.722663 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/
+-rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
+-rw-rw-rw-   0        0        0      555 2024-03-19 10:14:53.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
+-rw-rw-rw-   0        0        0      908 2024-03-19 10:29:01.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
+-rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.732600 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/text/
+-rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/text/text_block.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.808965 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/
+-rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/heading.html
+-rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/listblock.html
+-rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/richtext.html
+-rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/settings_form.html
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
+-rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.369648 globlocks-1.1.9/globlocks/templates/globlocks/icons/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.848629 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/
+-rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-center.svg
+-rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-justify.svg
+-rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-left.svg
+-rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-right.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.971562 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/
+-rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
+-rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
+-rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
+-rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
+-rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
+-rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
+-rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
+-rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
+-rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
+-rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
+-rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
+-rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.372471 globlocks-1.1.9/globlocks/templates/globlocks/shared/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.010432 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/
+-rw-rw-rw-   0        0        0      226 2024-03-19 09:32:33.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/base.html
+-rw-rw-rw-   0        0        0      902 2024-03-19 09:26:20.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.056198 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/
+-rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/base.html
+-rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/full.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/large.html
+-rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/medium.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/small.html
+-rw-rw-rw-   0        0        0      309 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/listblock.html
+-rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.127220 globlocks-1.1.9/globlocks/templates/globlocks/widgets/
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/color-input-widget.html
+-rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/font_picker_widget.html
+-rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/justify-widget-option.html
+-rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/justify-widget.html
+-rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/orderable_widget.html
+-rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/slider_input.html
+-rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/toolbar-widget.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.375470 globlocks-1.1.9/globlocks/templates/wagtailadmin/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.164543 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/
+-rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
+-rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/field.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.164543 globlocks-1.1.9/globlocks/templatetags/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.171058 globlocks-1.1.9/globlocks/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0     4257 2024-03-19 07:31:29.000000 globlocks-1.1.9/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.175860 globlocks-1.1.9/globlocks/templatetags/globlocks/
+-rw-rw-rw-   0        0        0     6627 2024-03-19 09:43:06.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.186254 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/
+-rw-rw-rw-   0        0        0     9504 2024-03-19 09:43:08.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1469 2024-03-19 07:31:29.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3595 2024-03-19 11:12:51.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2281 2024-03-19 09:18:19.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/admin.py
+-rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/toolbar.py
+-rw-rw-rw-   0        0        0     1242 2024-03-19 09:18:17.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/utils.py
+-rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templatetags/orderable_tags.py
+-rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/tests.py
+-rw-rw-rw-   0        0        0     1832 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.192918 globlocks-1.1.9/globlocks/wagtail_hooks/
+-rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/admin_hooks.py
+-rw-rw-rw-   0        0        0     4327 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/alignment.py
+-rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/rt_extensions.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.198837 globlocks-1.1.9/globlocks/widgets/
+-rw-rw-rw-   0        0        0      295 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/color_input_widget.py
+-rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/fontpicker.py
+-rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/justify_widget.py
+-rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/orderable.py
+-rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/range_input.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.214935 globlocks-1.1.9/globlocks.egg-info/
+-rw-rw-rw-   0        0        0     1984 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11470 2024-04-19 07:11:28.000000 globlocks-1.1.9/globlocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2024-04-19 07:11:30.229616 globlocks-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.198837 globlocks-1.1.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.205706 globlocks-1.1.9/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.208708 globlocks-1.1.9/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.210371 globlocks-1.1.9/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.214935 globlocks-1.1.9/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/wsgi.py
```

### Comparing `globlocks-1.1.8/LICENSE` & `globlocks-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/__init__.py` & `globlocks-1.1.9/globlocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/bases/baseblock.py` & `globlocks-1.1.9/globlocks/blocks/bases/baseblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     MUTABLE_META_ATTRIBUTES = [
         "label",
         "position",
         "button_label",
         "hide_labels",
         "absolute_position",
+        "hide_block_button",
         "icon",
     ]
 
     def __init__(self, *args, base_block=None, **kwargs):
         self.base_block: BaseBlock = base_block
         super().__init__(*args, **kwargs)
 
@@ -43,24 +44,26 @@
         context["verbose_name"] = self.meta.label or self.name or self.__class__.__name__
         context["button_label"] = self.meta.button_label
         context["hide_labels"] = self.meta.hide_labels
         context["button_icon"] = self.meta.icon
         context["full_size"] = self.meta.full
         context["absolute_position"] = self.meta.absolute_position
         context["compact_view"] = self.meta.compact_view
+        context["hide_block_button"] = self.meta.hide_block_button
         return context
 
     class Meta:
         form_template = (
             "wagtailadmin/block_forms/base_block_settings_struct.html"
         )
         label = _("Configure")
         button_label = _("Open Settings")
         hide_labels = False
         absolute_position = False
+        hide_block_button = False
         compact_view = False
         full=False
 
 
 class BaseBlock(blocks.StructBlock):
     """
         Let the user easily configure blocks by adding custom settings.
```

### Comparing `globlocks-1.1.8/globlocks/blocks/bases/visibility.py` & `globlocks-1.1.9/globlocks/blocks/bases/visibility.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import OrderedDict
+import random
 
 from django import forms
 from django.http import HttpRequest
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
@@ -20,14 +21,23 @@
 
 from .baseblock import BaseBlock, BaseBlockConfiguration
 from globlocks.settings import (
     GLOBLOCKS_EDITORS_SEE_HIDDEN,
 )
 
 
+_alphabet = "abcdefghijklmnopqrstuvwxyz"
+
+def rand_id():
+    return "".join(
+        random.choice(_alphabet)
+        for _ in range(8)
+    )
+
+
 class ToggleShowableButton:
     name:  str          = None
     block: blocks.Block = None
 
     def get_translations(self):
         return {}
     
@@ -54,15 +64,15 @@
         help_text=_("Whether to show the content."),
         classname="col-12",
 
     )
 
     def get_translations(self):
         return super().get_translations() | {
-            "showText": _("Show ({label})"),
+            "showText": _("Show"),
             "hideText": _("Hide"),
         }
     
     def get_js(self):
         return super().get_js() + [
             "globlocks/admin/toggleable-block/toggleable-block-buttons.js",
         ]
@@ -108,46 +118,52 @@
         classname="col-12 col-md-6",
     )
 
     def op(self, value):
         return value > self.get_cmp()
     
 
-class ToggleShowableBlockConfigurationValue(blocks.StructValue):
+class ToggleableConfigValue(blocks.StructValue):
     def __init__(self, block, *args):
         super().__init__(block, *args)
         settings = self.get("settings", {})
         for button in block.buttons:
             settings[button.name] = button.value_for_value_class(
                 settings.get(button.name),
             )
 
-class ToggleShowableConfiguration(BaseBlockConfiguration):
+class ToggleableConfig(BaseBlockConfiguration):
     def __init__(self, local_blocks=None, buttons=None, *args, **kwargs):
         super().__init__(local_blocks, *args, **kwargs)
 
         self.buttons = buttons or []
         child_blocks = OrderedDict()
         for button in self.buttons:
 
             button.block.set_name(button.name)
             child_blocks[button.name] = button.block
 
         self.child_blocks = child_blocks | self.child_blocks
+        self.hide_block_button = len(self.child_blocks) == len(self.buttons)
+
+    def get_form_context(self, value, prefix="", errors=None):
+        return super().get_form_context(value, prefix, errors) | {
+            "hide_block_button": self.hide_block_button,
+        }
 
     class Meta:
         label = _("Configuration")
         icon = "cog"
         button_label = _("Open Settings")
 
 
-class ToggleShowableAdapter(StructBlockAdapter):
-    js_constructor = "globlocks.blocks.ToggleShowableBlock"
+class ToggleableAdapter(StructBlockAdapter):
+    js_constructor = "globlocks.blocks.ToggleableBlock"
 
-    def __init__(self, block: "ToggleShowableBlock") -> None:
+    def __init__(self, block: "ToggleableBlock") -> None:
         super().__init__()
         self.block = block
 
     @cached_property
     def media(self):
         structblock_media = super().media
         js = set()
@@ -184,27 +200,26 @@
             }
 
         meta["buttons"] = buttons
 
         return block_name, child_blocks, meta
 
 
-class ToggleShowableBlock(BaseBlock):
-    advanced_settings_class = ToggleShowableConfiguration
-    adapter_class = ToggleShowableAdapter
+class ToggleableBlock(BaseBlock):
+    advanced_settings_class = ToggleableConfig
+    adapter_class = ToggleableAdapter
     buttons: list[ToggleShowableButton] = [
         DateTimeFromButton(),
         DateTimeToButton(),
         ToggleShowableButtonIsShown(),
     ]
 
     class Meta:
         icon = "arrow-up"
-        label = _("Toggle Showable")
-        show_text = _("Show ({label})")
+        show_text = _("Show")
         hide_text = _("Hide")
 
     def __init__(self, local_blocks=None, buttons=None, **kwargs):
         self.buttons = buttons or self.buttons
         super().__init__(local_blocks, **kwargs)
 
     def advanced_settings_kwargs(self, **kwargs):
@@ -247,18 +262,20 @@
                         )
                     ):
                     return ""
                 
                 title = self.hidden_editor_title(value, context)
                 label = self.hidden_editor_label(value, context)
                 preview = self.hidden_editor_preview(value, context)
+                id = rand_id()
+                _js = f"javascript:(() => {{{id}.remove(); return void(0)}})()"
 
                 # Default values, always shown
                 s = [
-                    "<div class='globlocks-toggleable-block'>\n",
+                    f"<div class='globlocks-toggleable-block' id=\"{id}\">\n",
                     f"    <h2 class=\"mb-1\">{title}</h2>\n",
                     f"    <h3 class=\"mb-1\">({label})</h3>\n",
                 ]
 
                 # add preview when available
                 if preview:
                     s.append("   <p>")
@@ -268,15 +285,21 @@
                 # Add optional edit link
                 edit_url = reverse(
                     "wagtailadmin_pages:edit",
                     args=(page.id,),
                 )
                 if "block_id" in context:
                     edit_url += f"#block-{context['block_id']}-section"
-                s.append(f"    <a href=\"{edit_url}\" class=\"globlocks-toggleable-block-btn\">{str(_('Edit'))}</a>\n")
+
+                s.append(
+                    f"    <a href=\"{edit_url}\" class=\"globlocks-toggleable-block-btn\">{str(_('Edit'))}</a>\n"
+                )
+                s.append(
+                    f"    <a href=\"{_js}\" class=\"globlocks-toggleable-block-btn\">{str(_('Close'))}</a>\n"
+                )
 
                 # Close container
                 s.append("</div>")
 
                 return mark_safe("".join(s))
 
         
@@ -312,9 +335,9 @@
             adapter = adapter(**kwargs)
 
         register(adapter, cls)
         return adapter
     
 
 
-ToggleShowableBlock.register_adapter()
+ToggleableBlock.register_adapter()
```

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/colorblock/colorblock.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/colorblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/fontpicker/fontpicker.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/orderable_block.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/orderable_block.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/rangeslider/rangeslider.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/rangeslider.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/__init__.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/bar.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/bar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/element.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/element.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/toolbar_field.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_field.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/toolbar_widget.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/block_fields/toolbar/tools.py` & `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/tools.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/components/heading.py` & `globlocks-1.1.9/globlocks/blocks/components/heading.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from wagtail import blocks
 from django.utils.translation import gettext_lazy as _
 from ..block_fields import (
     toolbar,
 )
 from ..bases import (
-    ToggleShowableConfiguration,
-    ToggleShowableBlock,
+    ToggleableConfig,
+    ToggleableBlock,
 )
 
 
-class HeadingConfiguration(ToggleShowableConfiguration):
+class HeadingConfiguration(ToggleableConfig):
     toolbar = toolbar.ToolbarBlock(
         targets=[
             "heading",
             "subheading"
         ],
         tag_name="h2",
         tools = [
@@ -37,15 +37,15 @@
     class Meta:
         label = _("Configuration")
         icon = "cog"
         button_label = _("Open Settings")
         label_format = _("Heading Configuration")
         absolute_position = True
 
-class Heading(ToggleShowableBlock):
+class Heading(ToggleableBlock):
     advanced_settings_class = HeadingConfiguration
 
     heading = blocks.CharBlock(
         required=True,
         help_text=_("The heading of the block."),
         form_classname="title",
     )
```

### Comparing `globlocks-1.1.8/globlocks/blocks/components/image_text.py` & `globlocks-1.1.9/globlocks/blocks/components/image_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     TextBlock,
 )
 from ..block_fields import (
     OrderableBlock,
     Orderable,
 )
 
+
+
 class ImageTextBlockConfiguration(TextBlock.advanced_settings_class):
 
     ordering = OrderableBlock(
         required=True,
         help_text=_("The order of the image and text."),
         orderables=[
             Orderable(
@@ -33,15 +35,15 @@
         ],
     )
 
     class Meta:
         label = _("Layout Settings")
         button_label = _("Open Layout Settings")
         label_format = _("Image Text Layout Settings")
-        hide_labels = True
+        hide_labels = False
         absolute_position = True
         icon = "resubmit"
 
 
 class ImageTextBlock(TextBlock):
     default_features = GLOBLOCKS_RICHTEXT_FEATURES
     advanced_settings_class = ImageTextBlockConfiguration
@@ -52,18 +54,19 @@
     )
 
     heading = blocks.CharBlock(
         required=True,
         help_text=_("The heading above the text."),
     )
 
+
     class Meta:
         label = _("Image and Text")
         label_format = _("Image / Text: {heading} {image}")
-        group = _("Image")
+        group = _("Images")
         template = "globlocks/blocks/components/image_text/image_text.html"
         form_template = "globlocks/blocks/components/image_text/image_text_form.html"
         compact_view = True
 
     def render_as_preview(self, value, context=None):
         return mark_safe(f"<strong>{value['heading']}:</strong> {strip_tags(value['text'])}\n")
```

### Comparing `globlocks-1.1.8/globlocks/blocks/components/text.py` & `globlocks-1.1.9/globlocks/blocks/components/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from ...settings import (
     GLOBLOCKS_RICHTEXT_FEATURES_HEADINGS,
 )
 from ...util import (
     make_block_tuple,
 )
 from ..bases import (
-    ToggleShowableBlock,
+    ToggleableBlock,
 )
 
 
 
-class TextBlock(ToggleShowableBlock):
+class TextBlock(ToggleableBlock):
     """
         A block for text.
     """
     default_features = GLOBLOCKS_RICHTEXT_FEATURES_HEADINGS
     text = blocks.Block()
 
     def init_local_blocks(self, local_blocks=None, **kwargs):
```

### Comparing `globlocks-1.1.8/globlocks/blocks/richtext.py` & `globlocks-1.1.9/globlocks/blocks/richtext.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/blocks/template.py` & `globlocks-1.1.9/globlocks/blocks/bases/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from wagtail import blocks
 from django.utils.translation import gettext_lazy as _
 from django.forms import ValidationError
 
-from .bases import BaseBlockConfiguration, BaseBlock
+from .baseblock import BaseBlockConfiguration, BaseBlock
+
+from conditional_field import (
+    classname as make_classname,
+    handler,
+)
 
 
 class TemplateBlockConfiguration(BaseBlockConfiguration):
     # placeholder, real value get set in __init__()
     custom_template = blocks.Block()
 
     def __init__(self, local_blocks=None, template_choices=None, classname=None, **kwargs):
@@ -22,15 +27,18 @@
                 "custom_template",
                 blocks.ChoiceBlock(
                     choices=template_choices,
                     default=template_choices[0][0],
                     required=True,
                     label=_("Template"),
                     help_text=_("The template to use for rendering."),
-                    classname=classname,
+                    classname=make_classname(
+                        classname,
+                        handler("custom_template"),
+                    ),
                     translatable=False,
                 ),
             ),
         )
 
         super().__init__(local_blocks, **kwargs)
```

### Comparing `globlocks-1.1.8/globlocks/colors.py` & `globlocks-1.1.9/globlocks/colors.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/fields/fontfield.py` & `globlocks-1.1.9/globlocks/fields/fontfield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/fields/orderablefield.py` & `globlocks-1.1.9/globlocks/fields/orderablefield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/fonts.py` & `globlocks-1.1.9/globlocks/fonts.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/locale/en/LC_MESSAGES/django.po` & `globlocks-1.1.9/globlocks/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/locale/nl/LC_MESSAGES/django.po` & `globlocks-1.1.9/globlocks/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/panels.py` & `globlocks-1.1.9/globlocks/panels.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/preview.py` & `globlocks-1.1.9/globlocks/preview.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/rt_extensions.py` & `globlocks-1.1.9/globlocks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/settings.py` & `globlocks-1.1.9/globlocks/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 """
     Basic richtext features used throughout the application.
     Only contains inline elements.
 """
 GLOBLOCKS_RICHTEXT_FEATURES = getattr(settings, "GLOBLOCKS_RICHTEXT_FEATURES", [
-    "bold", "italic", "ol", "ul", 
+    "bold", "italic",
     "link", "document-link", "image", 
     'text-alignment', 'word-counter',
 ])
 
 
 """
     More advanced richtext features used throughout the application.
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/admin/block_settings.js` & `globlocks-1.1.9/globlocks/static/globlocks/admin/block_settings.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/admin/layout.css` & `globlocks-1.1.9/globlocks/static/globlocks/admin/layout.css`

 * *Files 27% similar despite different names*

```diff
@@ -13,30 +13,37 @@
 }
 /* This messes with the outline when focused for some reason */
 /* .Draftail-Editor.Draftail-Editor .public-DraftEditor-content, */
 /* .Draftail-Editor.Draftail-Editor .public-DraftEditorPlaceholder-root { */
   /* padding: 0 0.625rem; */
 /* } */
 
+.goodadvice-collapsible [data-comment-add],
+.globlocks-link-form [data-comment-add],
+[data-comment-add].hide-comments,
+.hide-comments [data-comment-add] {
+  display: none;
+}
+
 .Draftail-Editor.Draftail-Editor :focus {
   outline: none !important;
 }
 .Draftail-Editor.Draftail-Editor:has(*:focus) {
   outline: 3px solid var(--w-color-focus) !important;
 }
 .Draftail-Editor.Draftail-Editor .public-DraftEditor-content,
 .Draftail-Editor.Draftail-Editor .public-DraftEditorPlaceholder-root {
-  padding: 0 0.325rem;
+  padding: 0.2rem 0.325rem;
 }
 .Draftail-Editor.Draftail-Editor .Draftail-Toolbar {
   padding: 0.1rem;
   border-bottom: 1px solid var(--w-color-border-field-default);
 }
 .Draftail-Editor.Draftail-Editor div[data-contents] > *[data-block] {
-  margin: 0.125rem 0;
+  margin: 0.525rem 0;
 }
 
 div[data-contentpath="settings"]:has(.goodadvice-collapsible) {
   position: relative;
 }
 div[data-contentpath="settings"]:has(.goodadvice-collapsible) > label {
   display: none;
@@ -184,26 +191,144 @@
   border-radius: 5px;
   padding: 0.5em;
 }
 /* .goodadvice-collapsible:not(.full) .goodadvice-collapsible-target > *:not(:has(.goodadvice-collapsible)) { */
   /*  */
 /* } */
 
-.row .w-field__comment-button {
-    inset-inline-end: -1.5rem;
-}
+/* .row .w-field__comment-button { */
+    /* inset-inline-end: -1.5rem; */
+/* } */
 
 .row .w-field__wrapper {
   padding: 0;
   margin-bottom: 5px;
 }
 .w-combobox__menu {
   scrollbar-gutter: stable;
 }
 
+.w-field--radio_select .w-field__input > * > * {
+  display: inline-block;
+  margin-right: 0.5em;
+  font-size: 0.9em;
+}
+.w-field__input:has(> input[type="url"]) {
+  position: relative;
+}
+.w-field__input:has(> input[type="url"])::after {
+  content: "URL";
+  position: absolute;
+  inset-inline-end: 0.5em;
+  inset-block-start: 0.5em;
+  color: var(--w-color-grey-200);
+  font-size: 0.8em;
+  pointer-events: none;
+  top: 50%;
+  transform: translateY(-50%);
+}
+.w-field__input:has(> input[type="url"]:focus)::after {
+  content: "";
+}
+
+/* HIDDEN SETTINGS `hide_block_button` */
+.goodadvice-collapsible.hidden,
+.goodadvice-collapsible .hidden,
+.goodadvice-collapsible-parent.hidden,
+.goodadvice-collapsible-parent .hidden {
+  display: none;
+}
+
+/* HELP TEXT */
+.c-sf-help .help {
+  margin-bottom: 0.325rem;
+}
+
+
+/* LINK FORM */
+
+.link-form-radios {
+  display: flex;
+  flex-direction: column;
+  justify-content: flex-start;
+  align-items: flex-end;
+}
+/* :not(.goodadvice-collapsible) .link-form-radios.link-form-radios { */
+  /* justify-content: space-between; */
+/* } */
+:not(.goodadvice-collapsible) .link-form-radios.link-form-radios .w-field__input {
+  margin-top: 0;
+}
+/* :not(.goodadvice-collapsible) .link-form-radios.link-form-radios .w-field__wrapper { */
+  /* margin-bottom: 0; */
+/* } */
+[data-contentpath="link"]:has(.globlocks-link-form):not(:has(.help)) .w-field__label {
+  margin-bottom: 0.5rem;
+}
+[data-contentpath="link"]:has(.globlocks-link-form):has(.help) .w-field__label {
+  margin-bottom: 0.325rem;
+}
+[data-contentpath="link"]:has(.globlocks-link-form) .help {
+  margin-bottom: 0.5rem;
+}
+[data-contentpath="link"]:has(.globlocks-link-form) .link-form-fields {
+  margin-top: 2px; /* I hate magic values. This makes the inputs align properly next to eachother. */
+}
+[data-contentpath="link"]:has(.globlocks-link-form) .link-form-fields .w-field {
+  display: flex;
+  flex-direction: column-reverse;
+}
+[data-contentpath="link"]:has(.globlocks-link-form) .link-form-fields [data-contentpath]:not(:has(input)) {
+
+}
+.globlocks-link-form ::placeholder {
+  font-size: 0.8em;
+  vertical-align: middle;
+}
+.globlocks-link-form.stacked input[type="text"],
+.globlocks-link-form.stacked input[type="email"],
+.globlocks-link-form.stacked input[type="url"] {
+  max-width: 400px;
+}
+.globlocks-link-form.stacked .w-field__input:has(> input[type="url"]) {
+  max-width: 400px;
+}
+
+.globlocks-link-form.unstacked .link-form-radios {
+  height: 100%;
+}
+.w-field__input .link-form-radios .w-field:has(.w-field__wrapper .w-field--model_choice_field button) {
+  align-self: center;
+}
+.w-field__input .link-form-radios label:has(input[type="radio"]) {
+  font-size: 0.8em;
+  margin-bottom: 0.1rem;
+}
+.w-field__input .link-form-radios input[type="radio"] {
+  width: 1rem;
+  height: 1rem;
+  margin-inline-end: 0.2rem;
+}
+.w-field__input .link-form-radios input[type="radio"]::before {
+  width: 0.5rem;
+  height: 0.5rem;
+}
+.w-field__input .link-form-radios label:has(input[type="radio"]:checked) {
+  font-weight: bold;
+}
+.w-field__input .link-form-radios .unchosen [data-chooser-action-choose] {
+  padding: 0.275em;
+}
+
+/* END LINK FORM */
+
+.row.nopad.nopad {
+  --bs-gutter-x: 0;
+}
+
 .noselect {
   -webkit-touch-callout: none; /* iOS Safari */
     -webkit-user-select: none; /* Safari */
      -khtml-user-select: none; /* Konqueror HTML */
        -moz-user-select: none; /* Old versions of Firefox */
         -ms-user-select: none; /* Internet Explorer/Edge */
             user-select: none; /* Non-prefixed version, currently
@@ -1089,8 +1214,13 @@
   padding-right: 1.5rem;
 }
 .pr-4 {
   padding-right: 2rem;
 }
 .pr-5 {
   padding-right: 2.5rem;
+}
+.color-input-widget {
+  display: flex;
+  flex-direction: column;
+  min-width: 150px;
 }
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js` & `globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -100,16 +100,18 @@
                 this.shownInput.checked,
                 this.block,
                 this.settings,
                 this,
             )
         });
 
-        if (this.settings.childBlocks.length > 1) {
-            this.shownObj.element.style.display = 'none';
+        const childBlockKeys = Object.keys(settings.childBlocks);
+        if (childBlockKeys.length > 1) {
+            let container = $(this.shownObj.element).closest('[data-contentpath]');
+            container.css('display', 'none');
         }
     }
 
     getState() {
         return this.shownInput.checked;
     }
 
@@ -129,26 +131,24 @@
             'globlocks-showable-block-button',
         )
 
         return btn;
     }
 
     show() {
-        this.element.innerText = this.def
-            .replaceText(this.block, this.opts.translations.hideText);
+        this.element.innerText = this.opts.translations.hideText;
 
         this.element.classList.remove('warning');
         this.element.classList.remove('danger');
         this.element.classList.add('success');
         // this.shownInput.checked = true;
     }
 
     hide() {
-        this.element.innerText = this.def
-            .replaceText(this.block, this.opts.translations.showText);
+        this.element.innerText = this.opts.translations.showText;
 
         this.element.classList.remove('success');
         this.element.classList.remove('warning');
         this.element.classList.remove('danger');
         if (this.block.hiddenBy.length > 1 || !this.block.hiddenBy.includes(this)) {
             this.element.classList.add('danger');
         } else {
@@ -293,15 +293,17 @@
     }
 
     getDateInput() {
         if (this.dateInput) {
             return this.dateInput;
         }
         const inputDef = this.settings.childBlocks.hide_before_date;
-        inputDef.element.style.display = 'none';
+        let container = $(inputDef.element).closest('[data-contentpath]');
+        container.css('display', 'none');
+
         const inputId = inputDef.idForLabel;
         const input = document.getElementById(inputId);
         return input;
     }
 }
 
 class DateToButton extends DateFromToBaseButton {
@@ -314,15 +316,17 @@
     }
 
     getDateInput() {
         if (this.dateInput) {
             return this.dateInput;
         }
         const inputDef = this.settings.childBlocks.hide_after_date;
-        inputDef.element.style.display = 'none';
+        let container = $(inputDef.element).closest('[data-contentpath]');
+        container.css('display', 'none');
+
         const inputId = inputDef.idForLabel;
         const input = document.getElementById(inputId);
         return input;
     }
 }
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css` & `globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css`

 * *Files 20% similar despite different names*

```diff
@@ -20,34 +20,66 @@
     border: var(--globlocks-showable-border-width) solid var(--globlocks-showable-border-color);
     padding: calc(var(--globlocks-showable-padding-y) - var(--globlocks-showable-border-width)) 
              calc(var(--globlocks-showable-padding-x) - var(--globlocks-showable-border-width));
     border-radius: var(--globlocks-showable-border-radius);
     max-height: 300px;
     overflow: hidden;
 }
+.globlocks-showable-block-hidden::before {
+    content: "";
+    position: absolute;
+    top: 0;
+    left: 0;
+    right: 0;
+    bottom: 0;
+    background-color: var(--w-color-grey-50);
+    opacity: 0.4;
+    z-index: 1;
+}
+.w-theme-dark .globlocks-showable-block-hidden::before {
+    background-color: var(--w-color-grey-400);
+}
 .globlocks-showable-block-hidden::after {
     content: '......';
     position: absolute;
     bottom: 5px;
     left: 50%;
     transform: translateX(-50%);
     font-size: 1.8em;
     font-weight: bold;
+    z-index: 2;
 }
-.globlocks-showable-block.globlocks-showable-block-hidden > :not(.globlocks-showable-block-buttons) {
+.globlocks-showable-block.globlocks-showable-block-hidden > :not(.overlaying) {
     filter: blur(5px);
     pointer-events: none;
 }
+.globlocks-showable-block > .globlocks-showable-block-text-overlay {
+    display: block;
+    position: absolute;
+    top: 0;
+    left: 0;
+    right: 0;
+    bottom: 0;
+    display: none;
+    color: var(--w-color-text-context);
+    justify-content: center;
+    align-items: center;
+    z-index: 3;
+}
+.globlocks-showable-block.globlocks-showable-block-hidden > .globlocks-showable-block-text-overlay {
+    display: flex;
+}
 .globlocks-showable-block-buttons {
     position: absolute;
     top: 3px;
     right: 3px;
     display: flex;
     flex-direction: row;
     gap: 2px;
+    z-index: 4;
 }
 .globlocks-showable-block-button {
     display: block;
     padding: 0.1em 0.5em;
     font-size: 14px;
     border-radius: 0.5em;
     cursor: pointer;
@@ -87,15 +119,15 @@
     top: calc(100% + 0.25em);
     background-color: var(--w-color-warning-100);
     /* padding: 0.25em; */
     right: 0;
     display: none;
     flex-direction: column;
     border-radius: 5px;
-    z-index: 100;
+    z-index: 1;
 }
 .globlocks-showable-block-buttons-menu-content,
 .globlocks-showable-block-buttons-menu-content:focus-within,
 .globlocks-showable-block-buttons-menu-content input,
 .globlocks-showable-block-buttons-menu-content input:focus{
     outline: none !important;
-}
+}
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js` & `globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -87,17 +87,21 @@
         const block = super.render(
             placeholder,
             prefix,
             initialState,
             initialError,
         );
 
+        this.textOverlay = document.createElement('div');
+        this.textOverlay.classList.add('overlaying', 'globlocks-showable-block-text-overlay');
+        block.container[0].appendChild(this.textOverlay);
+
         const settings = block.childBlocks.settings;
         const buttonWrapper = document.createElement('div');
-        buttonWrapper.classList.add('globlocks-showable-block-buttons');
+        buttonWrapper.classList.add('overlaying', 'globlocks-showable-block-buttons');
         block.container[0].appendChild(buttonWrapper);
         block.showableButtons = {};
 
         const keys = Object.keys(this.meta.buttons);
         for (let i = 0; i < keys.length; i++) {
             const key = keys[i];
             const btnOpts = this.meta.buttons[key];
@@ -178,22 +182,24 @@
         container.classList.add('globlocks-showable-block-hidden');
         const keys = Object.keys(block.showableButtons);
         for (let i = 0; i < keys.length; i++) {
             let buttonKey = keys[i];
             let button = block.showableButtons[buttonKey];
             button.hide();
         }
+
+        this.textOverlay.innerText = block.getTextLabel();
     }
 
     replaceText(block, text) {
         return text.replace('{label}', block.getTextLabel());
     }
 }
 
-window.telepath.register('globlocks.blocks.ToggleShowableBlock', ToggleableBlockDefinition);
+window.telepath.register('globlocks.blocks.ToggleableBlock', ToggleableBlockDefinition);
 
 
 if (!window.globlocks) {
     window.globlocks = {};
 }
 
 if (!window.globlocks.showableBlockButtons) {
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Acme-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Acme-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Bangers-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Bangers-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Caveat-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Caveat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Creepster-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Creepster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Inter-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Inter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Kanit-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Lato-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Lobster-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Lobster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Manrope-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Monoton-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Monoton-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Oswald-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/PTMono-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/PTMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Phudu-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Phudu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Poppins-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Roboto-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Rubik-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Rubik-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Ultra-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Ultra-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf` & `globlocks-1.1.9/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/richtext/alignment/alignment.css` & `globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/richtext/alignment/alignment.js` & `globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -91,49 +91,56 @@
         let modifiedContent = window.DraftJS.Modifier.applyInlineStyle(finalContent, finalSelection, alignment);
         const nextEditorState = window.DraftJS.EditorState.push(editorState, modifiedContent, 'change-inline-style');
 
         this.props.onComplete(nextEditorState);
     }
 }
 
+
 function TextAlignControl({
     getEditorState,
     onChange
 }) {
     // For script definition see
     // wagtail_hooks/rt_extensions.py
-    const alignments_i18n = JSON.parse(
-        document.getElementById('globlocks-text-alignment-i18n').textContent,
-    );
+    const translationData = document.getElementById('globlocks-text-alignment-i18n')
+    let alignments_i18n;
+    if (translationData) {
+        alignments_i18n = JSON.parse(
+            translationData.textContent,
+        );
+    } else {
+        alignments_i18n = {
+            left: "Left",
+            center: "Center",
+            right: "Right",
+        }
+    }
     const editorState = getEditorState();
 
-    console.log('TextAlignControl', editorState);
-
     return React.createElement(TextAlignment, {
         editorState: editorState,
         onComplete: onChange,
         alignmentTextLeft: alignments_i18n['left'],
         alignmentTextCenter: alignments_i18n['center'],
         alignmentTextRight: alignments_i18n['right'],
     });
 }
 
+
 // text-left, text-center, text-right (controls)
-console.log('Registering text-alignment');
 window.draftail.registerPlugin({
     type: 'text-alignment',
     inline: TextAlignControl,
 }, 'controls');
 
 
 const blockStyleFn = (block) => {
     let alignment = 'left';
 
-    console.log('blockStyleFn', block);
-
     let data = block.getData();
     if (data.get('alignment')) {
         alignment = data.get('alignment');
     }
 
     block.findStyleRanges((e) => {
         if (e.hasStyle('center')) {
@@ -145,15 +152,14 @@
     });
 
 
     return `editor-alignment-${alignment}`;
 };
 
 
-console.log('Registering blockStyleFn');
 const initEditorProxyTextAlign = new Proxy(window.draftail.initEditor, {
     apply: (target, thisArg, argumentsList) => {
         // Get the target editor in the same way initEditor does and
         // create a partially-applied AIControl component with the
         // element passed as the `field` prop so we can access
         // it later.
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js` & `globlocks-1.1.9/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/LICENSE` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/color-input-widget.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/color-input-widget.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,116 +1,111 @@
-function invertColor(hex) {
-    return (Number(`0x1${hex}`) ^ 0xFFFFFF).toString(16).substr(1).toUpperCase()
-}
-
-class ColorInputWidget {
-    constructor(id) {
-        /*
-        id = the ID of the HTML element where color input behaviour should be attached
-        */
-        this.textInput = document.getElementById(id);
-        this.colorInput = document.getElementById(id + "-color-btn");
-
-        this.textInput.addEventListener('change', this.handleUpdate.bind(this));
-
-        this.pickr = Pickr.create({
-            el: this.colorInput,
-            theme: 'classic', // or 'monolith', or 'nano'
-            useAsButton: true,
-            default: this.textInput.value,
-            defaultRepresentation: 'RGBA',
-            swatches: [
-                'rgba(244, 67, 54, 1)',
-                'rgba(233, 30, 99, 1)',
-                'rgba(156, 39, 176, 1)',
-                'rgba(103, 58, 183, 1)',
-                'rgba(63, 81, 181, 1)',
-                'rgba(33, 150, 243, 1)',
-                'rgba(3, 169, 244, 1)',
-            ],
-            components: {
-
-                // Main components
-                preview: true,
-                opacity: true,
-                hue: true,
-
-                // Input / output Options
-                interaction: {
-                    //hex: true,
-                    rgba: true,
-                    //hsla: true,
-                    //hsva: true,
-                    cancel: true,
-                    clear: true,
-                    save: true
-                }
-            }
-        })
-
-        function savePickrColor(color, instance) {
-            const rep = this.pickr.getColorRepresentation();
-            let formattedColor;
-            if (rep == "RGBA") {
-                formattedColor = color.toRGBA().toString(1);
-            } else if (rep == "HSLA") {
-                formattedColor = color.toHSLA().toString();
-            } else if (rep == "HSVA") {
-                formattedColor = color.toHSVA().toString();
-            } else if (rep == "HEXA") {
-                formattedColor = color.toHEXA().toString();
-            }
-            this.textInput.value = formattedColor;
-            this.textInput.dispatchEvent(new Event('change', {
-                was_manually_triggered: true
-            }));
-        }
-
-        this.pickr.on('change', savePickrColor.bind(this));
-        this.pickr.on('save', savePickrColor.bind(this));
-        this.pickr.on('clear', (color, instance) => {
-            this.textInput.value = "";
-        });
-        this.pickr.on('init', instance => {
-            let hexColor = this.pickr.getColor().toHEXA().toString()
-            hexColor = hexColor.substring(0, hexColor.length - 2)
-            this.textInput.style.backgroundColor = hexColor;
-
-            hexColor = hexColor.replace("#", "")
-            hexColor = invertColor(hexColor)
-            this.textInput.style.color = "#" + hexColor;
-        })
-    }
-    handleUpdate(evt) {
-        if (evt.was_manually_triggered) {
-            return;
-        }
-        this.setState(evt.target.value);
-    }
-
-    setState(newState) {
-        this.textInput.value = newState;
-        this.pickr.setColor(newState, true);
-
-        let hexColor = this.pickr.getColor().toHEXA().toString()
-        if (hexColor.length > 7) {
-            hexColor = hexColor.substring(0, hexColor.length - 2)
-        }
-        this.textInput.style.backgroundColor = hexColor;
-
-        hexColor = hexColor.replace("#", "")
-        hexColor = invertColor(hexColor)
-        this.textInput.style.color = "#" + hexColor;
-    }
-
-    getState() {
-        return this.textInput.value;
-    }
-
-    getValue() {
-        return this.textInput.value;
-    }
-
-    focus() {
-        this.textInput.focus();
-    }
+function invertColor(hex) {
+    return (Number(`0x1${hex}`) ^ 0xFFFFFF).toString(16).substr(1).toUpperCase()
+}
+
+class ColorInputWidget {
+    constructor(id) {
+        /*
+        id = the ID of the HTML element where color input behaviour should be attached
+        */
+        this.textInput = document.getElementById(id);
+        this.colorInput = document.getElementById(id + "-color-btn");
+
+        this.textInput.addEventListener('change', this.handleUpdate.bind(this));
+
+        this.pickr = Pickr.create({
+            el: this.colorInput,
+            theme: 'classic', // or 'monolith', or 'nano'
+            useAsButton: true,
+            default: this.textInput.value,
+            defaultRepresentation: 'RGBA',
+            swatches: [
+                'rgba(244, 67, 54, 1)',
+                'rgba(233, 30, 99, 1)',
+                'rgba(156, 39, 176, 1)',
+                'rgba(103, 58, 183, 1)',
+                'rgba(63, 81, 181, 1)',
+                'rgba(33, 150, 243, 1)',
+                'rgba(3, 169, 244, 1)',
+            ],
+            components: {
+
+                // Main components
+                preview: true,
+                opacity: true,
+                hue: true,
+
+                // Input / output Options
+                interaction: {
+                    //hex: true,
+                    rgba: true,
+                    //hsla: true,
+                    //hsva: true,
+                    cancel: true,
+                    clear: true,
+                    save: true
+                }
+            }
+        })
+
+        function savePickrColor(color, instance) {
+            const rep = this.pickr.getColorRepresentation();
+            let formattedColor;
+            if (rep == "RGBA") {
+                formattedColor = color.toRGBA().toString(1);
+            } else if (rep == "HSLA") {
+                formattedColor = color.toHSLA().toString();
+            } else if (rep == "HSVA") {
+                formattedColor = color.toHSVA().toString();
+            } else if (rep == "HEXA") {
+                formattedColor = color.toHEXA().toString();
+            }
+            this.textInput.value = formattedColor;
+            this.textInput.dispatchEvent(new Event('change', {
+                was_manually_triggered: true
+            }));
+        }
+
+        this.pickr.on('change', savePickrColor.bind(this));
+        this.pickr.on('save', savePickrColor.bind(this));
+        this.pickr.on('clear', (color, instance) => {
+            this.textInput.value = "";
+        });
+        this.pickr.on('init', instance => {
+            let hexColor = this.pickr.getColor().toHEXA().toString()
+            this.setState(hexColor);
+        })
+    }
+    handleUpdate(evt) {
+        if (evt.was_manually_triggered) {
+            return;
+        }
+        this.setState(evt.target.value);
+    }
+
+    setState(newState) {
+        this.textInput.value = newState;
+        this.pickr.setColor(newState, true);
+
+        let hexColor = this.pickr.getColor().toHEXA().toString()
+        if (hexColor.length > 7) {
+            hexColor = hexColor.substring(0, hexColor.length - 2)
+        }
+        this.textInput.style.backgroundColor = hexColor;
+
+        hexColor = hexColor.replace("#", "")
+        hexColor = invertColor(hexColor)
+        this.textInput.style.color = "#" + hexColor;
+    }
+
+    getState() {
+        return this.textInput.value;
+    }
+
+    getValue() {
+        return this.textInput.value;
+    }
+
+    focus() {
+        this.textInput.focus();
+    }
 }
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/pickr.css` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-/*! Pickr 1.8.2 MIT | https://github.com/Simonwep/pickr */
+/*! Pickr 1.8.2 MIT | https://github.com/Simonwep/pickr */
 .pickr{position:relative;overflow:visible;transform:translateY(0)}.pickr *{box-sizing:border-box;outline:none;border:none;-webkit-appearance:none}.pickr .pcr-button{position:relative;height:2em;width:2em;padding:0.5em;cursor:pointer;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Roboto","Helvetica Neue",Arial,sans-serif;border-radius:.15em;background:url('data:image/svg+xml;utf8, <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 50 50" stroke="%2342445A" stroke-width="5px" stroke-linecap="round"><path d="M45,45L5,5"></path><path d="M45,5L5,45"></path></svg>') no-repeat center;background-size:0;transition:all 0.3s}.pickr .pcr-button::before{position:absolute;content:'';top:0;left:0;width:100%;height:100%;background:url('data:image/svg+xml;utf8, <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2 2"><path fill="white" d="M1,0H2V1H1V0ZM0,1H1V2H0V1Z"/><path fill="gray" d="M0,0H1V1H0V0ZM1,1H2V2H1V1Z"/></svg>');background-size:.5em;border-radius:.15em;z-index:-1}.pickr .pcr-button::before{z-index:initial}.pickr .pcr-button::after{position:absolute;content:'';top:0;left:0;height:100%;width:100%;transition:background 0.3s;background:var(--pcr-color);border-radius:.15em}.pickr .pcr-button.clear{background-size:70%}.pickr .pcr-button.clear::before{opacity:0}.pickr .pcr-button.clear:focus{box-shadow:0 0 0 1px rgba(255,255,255,0.85),0 0 0 3px var(--pcr-color)}.pickr .pcr-button.disabled{cursor:not-allowed}.pickr *,.pcr-app *{box-sizing:border-box;outline:none;border:none;-webkit-appearance:none}.pickr input:focus,.pickr input.pcr-active,.pickr button:focus,.pickr button.pcr-active,.pcr-app input:focus,.pcr-app input.pcr-active,.pcr-app button:focus,.pcr-app button.pcr-active{box-shadow:0 0 0 1px rgba(255,255,255,0.85),0 0 0 3px var(--pcr-color)}.pickr .pcr-palette,.pickr .pcr-slider,.pcr-app .pcr-palette,.pcr-app .pcr-slider{transition:box-shadow 0.3s}.pickr .pcr-palette:focus,.pickr .pcr-slider:focus,.pcr-app .pcr-palette:focus,.pcr-app .pcr-slider:focus{box-shadow:0 0 0 1px rgba(255,255,255,0.85),0 0 0 3px rgba(0,0,0,0.25)}.pcr-app{position:fixed;display:flex;flex-direction:column;z-index:10000;border-radius:0.1em;background:#fff;opacity:0;visibility:hidden;transition:opacity 0.3s, visibility 0s 0.3s;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Roboto","Helvetica Neue",Arial,sans-serif;box-shadow:0 0.15em 1.5em 0 rgba(0,0,0,0.1),0 0 1em 0 rgba(0,0,0,0.03);left:0;top:0}.pcr-app.visible{transition:opacity 0.3s;visibility:visible;opacity:1}.pcr-app .pcr-swatches{display:flex;flex-wrap:wrap;margin-top:0.75em}.pcr-app .pcr-swatches.pcr-last{margin:0}@supports (display: grid){.pcr-app .pcr-swatches{display:grid;align-items:center;grid-template-columns:repeat(auto-fit, 1.75em)}}.pcr-app .pcr-swatches>button{font-size:1em;position:relative;width:calc(1.75em - 5px);height:calc(1.75em - 5px);border-radius:0.15em;cursor:pointer;margin:2.5px;flex-shrink:0;justify-self:center;transition:all 0.15s;overflow:hidden;background:transparent;z-index:1}.pcr-app .pcr-swatches>button::before{position:absolute;content:'';top:0;left:0;width:100%;height:100%;background:url('data:image/svg+xml;utf8, <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2 2"><path fill="white" d="M1,0H2V1H1V0ZM0,1H1V2H0V1Z"/><path fill="gray" d="M0,0H1V1H0V0ZM1,1H2V2H1V1Z"/></svg>');background-size:6px;border-radius:.15em;z-index:-1}.pcr-app .pcr-swatches>button::after{content:'';position:absolute;top:0;left:0;width:100%;height:100%;background:var(--pcr-color);border:1px solid rgba(0,0,0,0.05);border-radius:0.15em;box-sizing:border-box}.pcr-app .pcr-swatches>button:hover{filter:brightness(1.05)}.pcr-app .pcr-swatches>button:not(.pcr-active){box-shadow:none}.pcr-app .pcr-interaction{display:flex;flex-wrap:wrap;align-items:center;margin:0 -0.2em 0 -0.2em}.pcr-app .pcr-interaction>*{margin:0 0.2em}.pcr-app .pcr-interaction input{letter-spacing:0.07em;font-size:0.75em;text-align:center;cursor:pointer;color:#75797e;background:#f1f3f4;border-radius:.15em;transition:all 0.15s;padding:0.45em 0.5em;margin-top:0.75em}.pcr-app .pcr-interaction input:hover{filter:brightness(0.975)}.pcr-app .pcr-interaction input:focus{box-shadow:0 0 0 1px rgba(255,255,255,0.85),0 0 0 3px rgba(66,133,244,0.75)}.pcr-app .pcr-interaction .pcr-result{color:#75797e;text-align:left;flex:1 1 8em;min-width:8em;transition:all 0.2s;border-radius:.15em;background:#f1f3f4;cursor:text}.pcr-app .pcr-interaction .pcr-result::-moz-selection{background:#4285f4;color:#fff}.pcr-app .pcr-interaction .pcr-result::selection{background:#4285f4;color:#fff}.pcr-app .pcr-interaction .pcr-type.active{color:#fff;background:#4285f4}.pcr-app .pcr-interaction .pcr-save,.pcr-app .pcr-interaction .pcr-cancel,.pcr-app .pcr-interaction .pcr-clear{color:#fff;width:auto}.pcr-app .pcr-interaction .pcr-save,.pcr-app .pcr-interaction .pcr-cancel,.pcr-app .pcr-interaction .pcr-clear{color:#fff}.pcr-app .pcr-interaction .pcr-save:hover,.pcr-app .pcr-interaction .pcr-cancel:hover,.pcr-app .pcr-interaction .pcr-clear:hover{filter:brightness(0.925)}.pcr-app .pcr-interaction .pcr-save{background:#4285f4}.pcr-app .pcr-interaction .pcr-clear,.pcr-app .pcr-interaction .pcr-cancel{background:#f44250}.pcr-app .pcr-interaction .pcr-clear:focus,.pcr-app .pcr-interaction .pcr-cancel:focus{box-shadow:0 0 0 1px rgba(255,255,255,0.85),0 0 0 3px rgba(244,66,80,0.75)}.pcr-app .pcr-selection .pcr-picker{position:absolute;height:18px;width:18px;border:2px solid #fff;border-radius:100%;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.pcr-app .pcr-selection .pcr-color-palette,.pcr-app .pcr-selection .pcr-color-chooser,.pcr-app .pcr-selection .pcr-color-opacity{position:relative;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;display:flex;flex-direction:column;cursor:grab;cursor:-webkit-grab}.pcr-app .pcr-selection .pcr-color-palette:active,.pcr-app .pcr-selection .pcr-color-chooser:active,.pcr-app .pcr-selection .pcr-color-opacity:active{cursor:grabbing;cursor:-webkit-grabbing}.pcr-app[data-theme='classic']{width:28.5em;max-width:95vw;padding:0.8em}.pcr-app[data-theme='classic'] .pcr-selection{display:flex;justify-content:space-between;flex-grow:1}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-preview{position:relative;z-index:1;width:2em;display:flex;flex-direction:column;justify-content:space-between;margin-right:0.75em}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-preview::before{position:absolute;content:'';top:0;left:0;width:100%;height:100%;background:url('data:image/svg+xml;utf8, <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2 2"><path fill="white" d="M1,0H2V1H1V0ZM0,1H1V2H0V1Z"/><path fill="gray" d="M0,0H1V1H0V0ZM1,1H2V2H1V1Z"/></svg>');background-size:.5em;border-radius:.15em;z-index:-1}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-preview .pcr-last-color{cursor:pointer;border-radius:0.15em 0.15em 0 0;z-index:2}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-preview .pcr-current-color{border-radius:0 0 0.15em 0.15em}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-preview .pcr-last-color,.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-preview .pcr-current-color{background:var(--pcr-color);width:100%;height:50%}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-palette{width:100%;height:8em;z-index:1}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-palette .pcr-palette{flex-grow:1;border-radius:.15em}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-palette .pcr-palette::before{position:absolute;content:'';top:0;left:0;width:100%;height:100%;background:url('data:image/svg+xml;utf8, <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2 2"><path fill="white" d="M1,0H2V1H1V0ZM0,1H1V2H0V1Z"/><path fill="gray" d="M0,0H1V1H0V0ZM1,1H2V2H1V1Z"/></svg>');background-size:.5em;border-radius:.15em;z-index:-1}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-chooser,.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-opacity{margin-left:0.75em}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-chooser .pcr-picker,.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-opacity .pcr-picker{left:50%;transform:translateX(-50%)}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-chooser .pcr-slider,.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-opacity .pcr-slider{width:8px;flex-grow:1;border-radius:50em}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-chooser .pcr-slider{background:linear-gradient(to bottom, red, #ff0, lime, cyan, blue, #f0f, red)}.pcr-app[data-theme='classic'] .pcr-selection .pcr-color-opacity .pcr-slider{background:linear-gradient(to bottom, transparent, black),url('data:image/svg+xml;utf8, <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2 2"><path fill="white" d="M1,0H2V1H1V0ZM0,1H1V2H0V1Z"/><path fill="gray" d="M0,0H1V1H0V0ZM1,1H2V2H1V1Z"/></svg>');background-size:100%, 50%}
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/color_input/pickr.min.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,872 +1,872 @@
-/*! Pickr 1.8.2 MIT | https://github.com/Simonwep/pickr */ ! function(t, e) {
-    "object" == typeof exports && "object" == typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define([], e) : "object" == typeof exports ? exports.Pickr = e() : t.Pickr = e()
-}(self, (function() {
-    return (() => {
-        "use strict";
-        var t = {
-                d: (e, o) => {
-                    for (var n in o) t.o(o, n) && !t.o(e, n) && Object.defineProperty(e, n, {
-                        enumerable: !0,
-                        get: o[n]
-                    })
-                },
-                o: (t, e) => Object.prototype.hasOwnProperty.call(t, e),
-                r: t => {
-                    "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
-                        value: "Module"
-                    }), Object.defineProperty(t, "__esModule", {
-                        value: !0
-                    })
-                }
-            },
-            e = {};
-        t.d(e, {
-            default: () => L
-        });
-        var o = {};
-
-        function n(t, e, o, n, i = {}) {
-            e instanceof HTMLCollection || e instanceof NodeList ? e = Array.from(e) : Array.isArray(e) || (e = [e]), Array.isArray(o) || (o = [o]);
-            for (const s of e)
-                for (const e of o) s[t](e, n, {
-                    capture: !1,
-                    ...i
-                });
-            return Array.prototype.slice.call(arguments, 1)
-        }
-        t.r(o), t.d(o, {
-            adjustableInputNumbers: () => p,
-            createElementFromString: () => r,
-            createFromTemplate: () => a,
-            eventPath: () => l,
-            off: () => s,
-            on: () => i,
-            resolveElement: () => c
-        });
-        const i = n.bind(null, "addEventListener"),
-            s = n.bind(null, "removeEventListener");
-
-        function r(t) {
-            const e = document.createElement("div");
-            return e.innerHTML = t.trim(), e.firstElementChild
-        }
-
-        function a(t) {
-            const e = (t, e) => {
-                    const o = t.getAttribute(e);
-                    return t.removeAttribute(e), o
-                },
-                o = (t, n = {}) => {
-                    const i = e(t, ":obj"),
-                        s = e(t, ":ref"),
-                        r = i ? n[i] = {} : n;
-                    s && (n[s] = t);
-                    for (const n of Array.from(t.children)) {
-                        const t = e(n, ":arr"),
-                            i = o(n, t ? {} : r);
-                        t && (r[t] || (r[t] = [])).push(Object.keys(i).length ? i : n)
-                    }
-                    return n
-                };
-            return o(r(t))
-        }
-
-        function l(t) {
-            let e = t.path || t.composedPath && t.composedPath();
-            if (e) return e;
-            let o = t.target.parentElement;
-            for (e = [t.target, o]; o = o.parentElement;) e.push(o);
-            return e.push(document, window), e
-        }
-
-        function c(t) {
-            return t instanceof Element ? t : "string" == typeof t ? t.split(/>>/g).reduce(((t, e, o, n) => (t = t.querySelector(e), o < n.length - 1 ? t.shadowRoot : t)), document) : null
-        }
-
-        function p(t, e = (t => t)) {
-            function o(o) {
-                const n = [.001, .01, .1][Number(o.shiftKey || 2 * o.ctrlKey)] * (o.deltaY < 0 ? 1 : -1);
-                let i = 0,
-                    s = t.selectionStart;
-                t.value = t.value.replace(/[\d.]+/g, ((t, o) => o <= s && o + t.length >= s ? (s = o, e(Number(t), n, i)) : (i++, t))), t.focus(), t.setSelectionRange(s, s), o.preventDefault(), t.dispatchEvent(new Event("input"))
-            }
-            i(t, "focus", (() => i(window, "wheel", o, {
-                passive: !1
-            }))), i(t, "blur", (() => s(window, "wheel", o)))
-        }
-        const {
-            min: u,
-            max: h,
-            floor: d,
-            round: m
-        } = Math;
-
-        function f(t, e, o) {
-            e /= 100, o /= 100;
-            const n = d(t = t / 360 * 6),
-                i = t - n,
-                s = o * (1 - e),
-                r = o * (1 - i * e),
-                a = o * (1 - (1 - i) * e),
-                l = n % 6;
-            return [255 * [o, r, s, s, a, o][l], 255 * [a, o, o, r, s, s][l], 255 * [s, s, a, o, o, r][l]]
-        }
-
-        function v(t, e, o) {
-            const n = (2 - (e /= 100)) * (o /= 100) / 2;
-            return 0 !== n && (e = 1 === n ? 0 : n < .5 ? e * o / (2 * n) : e * o / (2 - 2 * n)), [t, 100 * e, 100 * n]
-        }
-
-        function b(t, e, o) {
-            const n = u(t /= 255, e /= 255, o /= 255),
-                i = h(t, e, o),
-                s = i - n;
-            let r, a;
-            if (0 === s) r = a = 0;
-            else {
-                a = s / i;
-                const n = ((i - t) / 6 + s / 2) / s,
-                    l = ((i - e) / 6 + s / 2) / s,
-                    c = ((i - o) / 6 + s / 2) / s;
-                t === i ? r = c - l : e === i ? r = 1 / 3 + n - c : o === i && (r = 2 / 3 + l - n), r < 0 ? r += 1 : r > 1 && (r -= 1)
-            }
-            return [360 * r, 100 * a, 100 * i]
-        }
-
-        function y(t, e, o, n) {
-            e /= 100, o /= 100;
-            return [...b(255 * (1 - u(1, (t /= 100) * (1 - (n /= 100)) + n)), 255 * (1 - u(1, e * (1 - n) + n)), 255 * (1 - u(1, o * (1 - n) + n)))]
-        }
-
-        function g(t, e, o) {
-            e /= 100;
-            const n = 2 * (e *= (o /= 100) < .5 ? o : 1 - o) / (o + e) * 100,
-                i = 100 * (o + e);
-            return [t, isNaN(n) ? 0 : n, i]
-        }
-
-        function _(t) {
-            return b(...t.match(/.{2}/g).map((t => parseInt(t, 16))))
-        }
-
-        function w(t) {
-            t = t.match(/^[a-zA-Z]+$/) ? function(t) {
-                if ("black" === t.toLowerCase()) return "#000";
-                const e = document.createElement("canvas").getContext("2d");
-                return e.fillStyle = t, "#000" === e.fillStyle ? null : e.fillStyle
-            }(t) : t;
-            const e = {
-                    cmyk: /^cmyk[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)/i,
-                    rgba: /^((rgba)|rgb)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]*?([\d.]+|$)/i,
-                    hsla: /^((hsla)|hsl)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]*?([\d.]+|$)/i,
-                    hsva: /^((hsva)|hsv)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]*?([\d.]+|$)/i,
-                    hexa: /^#?(([\dA-Fa-f]{3,4})|([\dA-Fa-f]{6})|([\dA-Fa-f]{8}))$/i
-                },
-                o = t => t.map((t => /^(|\d+)\.\d+|\d+$/.test(t) ? Number(t) : void 0));
-            let n;
-            t: for (const i in e) {
-                if (!(n = e[i].exec(t))) continue;
-                const s = t => !!n[2] == ("number" == typeof t);
-                switch (i) {
-                    case "cmyk": {
-                        const [, t, e, s, r] = o(n);
-                        if (t > 100 || e > 100 || s > 100 || r > 100) break t;
-                        return {
-                            values: y(t, e, s, r),
-                            type: i
-                        }
-                    }
-                    case "rgba": {
-                        const [, , , t, e, r, a] = o(n);
-                        if (t > 255 || e > 255 || r > 255 || a < 0 || a > 1 || !s(a)) break t;
-                        return {
-                            values: [...b(t, e, r), a],
-                            a,
-                            type: i
-                        }
-                    }
-                    case "hexa": {
-                        let [, t] = n;
-                        4 !== t.length && 3 !== t.length || (t = t.split("").map((t => t + t)).join(""));
-                        const e = t.substring(0, 6);
-                        let o = t.substring(6);
-                        return o = o ? parseInt(o, 16) / 255 : void 0, {
-                            values: [..._(e), o],
-                            a: o,
-                            type: i
-                        }
-                    }
-                    case "hsla": {
-                        const [, , , t, e, r, a] = o(n);
-                        if (t > 360 || e > 100 || r > 100 || a < 0 || a > 1 || !s(a)) break t;
-                        return {
-                            values: [...g(t, e, r), a],
-                            a,
-                            type: i
-                        }
-                    }
-                    case "hsva": {
-                        const [, , , t, e, r, a] = o(n);
-                        if (t > 360 || e > 100 || r > 100 || a < 0 || a > 1 || !s(a)) break t;
-                        return {
-                            values: [t, e, r, a],
-                            a,
-                            type: i
-                        }
-                    }
-                }
-            }
-            return {
-                values: null,
-                type: null
-            }
-        }
-
-        function A(t = 0, e = 0, o = 0, n = 1) {
-            const i = (t, e) => (o = -1) => e(~o ? t.map((t => Number(t.toFixed(o)))) : t),
-                s = {
-                    h: t,
-                    s: e,
-                    v: o,
-                    a: n,
-                    toHSVA() {
-                        const t = [s.h, s.s, s.v, s.a];
-                        return t.toString = i(t, (t => `hsva(${t[0]}, ${t[1]}%, ${t[2]}%, ${s.a})`)), t
-                    },
-                    toHSLA() {
-                        const t = [...v(s.h, s.s, s.v), s.a];
-                        return t.toString = i(t, (t => `hsla(${t[0]}, ${t[1]}%, ${t[2]}%, ${s.a})`)), t
-                    },
-                    toRGBA() {
-                        const t = [...f(s.h, s.s, s.v), s.a];
-                        return t.toString = i(t, (t => `rgba(${t[0]}, ${t[1]}, ${t[2]}, ${s.a})`)), t
-                    },
-                    toCMYK() {
-                        const t = function(t, e, o) {
-                            const n = f(t, e, o),
-                                i = n[0] / 255,
-                                s = n[1] / 255,
-                                r = n[2] / 255,
-                                a = u(1 - i, 1 - s, 1 - r);
-                            return [100 * (1 === a ? 0 : (1 - i - a) / (1 - a)), 100 * (1 === a ? 0 : (1 - s - a) / (1 - a)), 100 * (1 === a ? 0 : (1 - r - a) / (1 - a)), 100 * a]
-                        }(s.h, s.s, s.v);
-                        return t.toString = i(t, (t => `cmyk(${t[0]}%, ${t[1]}%, ${t[2]}%, ${t[3]}%)`)), t
-                    },
-                    toHEXA() {
-                        const t = function(t, e, o) {
-                                return f(t, e, o).map((t => m(t).toString(16).padStart(2, "0")))
-                            }(s.h, s.s, s.v),
-                            e = s.a >= 1 ? "" : Number((255 * s.a).toFixed(0)).toString(16).toUpperCase().padStart(2, "0");
-                        return e && t.push(e), t.toString = () => `#${t.join("").toUpperCase()}`, t
-                    },
-                    clone: () => A(s.h, s.s, s.v, s.a)
-                };
-            return s
-        }
-        const C = t => Math.max(Math.min(t, 1), 0);
-
-        function $(t) {
-            const e = {
-                    options: Object.assign({
-                        lock: null,
-                        onchange: () => 0,
-                        onstop: () => 0
-                    }, t),
-                    _keyboard(t) {
-                        const {
-                            options: o
-                        } = e, {
-                            type: n,
-                            key: i
-                        } = t;
-                        if (document.activeElement === o.wrapper) {
-                            const {
-                                lock: o
-                            } = e.options, s = "ArrowUp" === i, r = "ArrowRight" === i, a = "ArrowDown" === i, l = "ArrowLeft" === i;
-                            if ("keydown" === n && (s || r || a || l)) {
-                                let n = 0,
-                                    i = 0;
-                                "v" === o ? n = s || r ? 1 : -1 : "h" === o ? n = s || r ? -1 : 1 : (i = s ? -1 : a ? 1 : 0, n = l ? -1 : r ? 1 : 0), e.update(C(e.cache.x + .01 * n), C(e.cache.y + .01 * i)), t.preventDefault()
-                            } else i.startsWith("Arrow") && (e.options.onstop(), t.preventDefault())
-                        }
-                    },
-                    _tapstart(t) {
-                        i(document, ["mouseup", "touchend", "touchcancel"], e._tapstop), i(document, ["mousemove", "touchmove"], e._tapmove), t.cancelable && t.preventDefault(), e._tapmove(t)
-                    },
-                    _tapmove(t) {
-                        const {
-                            options: o,
-                            cache: n
-                        } = e, {
-                            lock: i,
-                            element: s,
-                            wrapper: r
-                        } = o, a = r.getBoundingClientRect();
-                        let l = 0,
-                            c = 0;
-                        if (t) {
-                            const e = t && t.touches && t.touches[0];
-                            l = t ? (e || t).clientX : 0, c = t ? (e || t).clientY : 0, l < a.left ? l = a.left : l > a.left + a.width && (l = a.left + a.width), c < a.top ? c = a.top : c > a.top + a.height && (c = a.top + a.height), l -= a.left, c -= a.top
-                        } else n && (l = n.x * a.width, c = n.y * a.height);
-                        "h" !== i && (s.style.left = `calc(${l/a.width*100}% - ${s.offsetWidth/2}px)`), "v" !== i && (s.style.top = `calc(${c/a.height*100}% - ${s.offsetHeight/2}px)`), e.cache = {
-                            x: l / a.width,
-                            y: c / a.height
-                        };
-                        const p = C(l / a.width),
-                            u = C(c / a.height);
-                        switch (i) {
-                            case "v":
-                                return o.onchange(p);
-                            case "h":
-                                return o.onchange(u);
-                            default:
-                                return o.onchange(p, u)
-                        }
-                    },
-                    _tapstop() {
-                        e.options.onstop(), s(document, ["mouseup", "touchend", "touchcancel"], e._tapstop), s(document, ["mousemove", "touchmove"], e._tapmove)
-                    },
-                    trigger() {
-                        e._tapmove()
-                    },
-                    update(t = 0, o = 0) {
-                        const {
-                            left: n,
-                            top: i,
-                            width: s,
-                            height: r
-                        } = e.options.wrapper.getBoundingClientRect();
-                        "h" === e.options.lock && (o = t), e._tapmove({
-                            clientX: n + s * t,
-                            clientY: i + r * o
-                        })
-                    },
-                    destroy() {
-                        const {
-                            options: t,
-                            _tapstart: o,
-                            _keyboard: n
-                        } = e;
-                        s(document, ["keydown", "keyup"], n), s([t.wrapper, t.element], "mousedown", o), s([t.wrapper, t.element], "touchstart", o, {
-                            passive: !1
-                        })
-                    }
-                },
-                {
-                    options: o,
-                    _tapstart: n,
-                    _keyboard: r
-                } = e;
-            return i([o.wrapper, o.element], "mousedown", n), i([o.wrapper, o.element], "touchstart", n, {
-                passive: !1
-            }), i(document, ["keydown", "keyup"], r), e
-        }
-
-        function k(t = {}) {
-            t = Object.assign({
-                onchange: () => 0,
-                className: "",
-                elements: []
-            }, t);
-            const e = i(t.elements, "click", (e => {
-                t.elements.forEach((o => o.classList[e.target === o ? "add" : "remove"](t.className))), t.onchange(e), e.stopPropagation()
-            }));
-            return {
-                destroy: () => s(...e)
-            }
-        }
-        const S = {
-                variantFlipOrder: {
-                    start: "sme",
-                    middle: "mse",
-                    end: "ems"
-                },
-                positionFlipOrder: {
-                    top: "tbrl",
-                    right: "rltb",
-                    bottom: "btrl",
-                    left: "lrbt"
-                },
-                position: "bottom",
-                margin: 8
-            },
-            O = (t, e, o) => {
-                const {
-                    container: n,
-                    margin: i,
-                    position: s,
-                    variantFlipOrder: r,
-                    positionFlipOrder: a
-                } = {
-                    container: document.documentElement.getBoundingClientRect(),
-                    ...S,
-                    ...o
-                }, {
-                    left: l,
-                    top: c
-                } = e.style;
-                e.style.left = "0", e.style.top = "0";
-                const p = t.getBoundingClientRect(),
-                    u = e.getBoundingClientRect(),
-                    h = {
-                        t: p.top - u.height - i,
-                        b: p.bottom + i,
-                        r: p.right + i,
-                        l: p.left - u.width - i
-                    },
-                    d = {
-                        vs: p.left,
-                        vm: p.left + p.width / 2 + -u.width / 2,
-                        ve: p.left + p.width - u.width,
-                        hs: p.top,
-                        hm: p.bottom - p.height / 2 - u.height / 2,
-                        he: p.bottom - u.height
-                    },
-                    [m, f = "middle"] = s.split("-"),
-                    v = a[m],
-                    b = r[f],
-                    {
-                        top: y,
-                        left: g,
-                        bottom: _,
-                        right: w
-                    } = n;
-                for (const t of v) {
-                    const o = "t" === t || "b" === t,
-                        n = h[t],
-                        [i, s] = o ? ["top", "left"] : ["left", "top"],
-                        [r, a] = o ? [u.height, u.width] : [u.width, u.height],
-                        [l, c] = o ? [_, w] : [w, _],
-                        [p, m] = o ? [y, g] : [g, y];
-                    if (!(n < p || n + r > l))
-                        for (const r of b) {
-                            const l = d[(o ? "v" : "h") + r];
-                            if (!(l < m || l + a > c)) return e.style[s] = l - u[s] + "px", e.style[i] = n - u[i] + "px", t + r
-                        }
-                }
-                return e.style.left = l, e.style.top = c, null
-            };
-
-        function E(t, e, o) {
-            return e in t ? Object.defineProperty(t, e, {
-                value: o,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : t[e] = o, t
-        }
-        class L {
-            constructor(t) {
-                E(this, "_initializingActive", !0), E(this, "_recalc", !0), E(this, "_nanopop", null), E(this, "_root", null), E(this, "_color", A()), E(this, "_lastColor", A()), E(this, "_swatchColors", []), E(this, "_setupAnimationFrame", null), E(this, "_eventListener", {
-                    init: [],
-                    save: [],
-                    hide: [],
-                    show: [],
-                    clear: [],
-                    change: [],
-                    changestop: [],
-                    cancel: [],
-                    swatchselect: []
-                }), this.options = t = Object.assign({
-                    ...L.DEFAULT_OPTIONS
-                }, t);
-                const {
-                    swatches: e,
-                    components: o,
-                    theme: n,
-                    sliders: i,
-                    lockOpacity: s,
-                    padding: r
-                } = t;
-                ["nano", "monolith"].includes(n) && !i && (t.sliders = "h"), o.interaction || (o.interaction = {});
-                const {
-                    preview: a,
-                    opacity: l,
-                    hue: c,
-                    palette: p
-                } = o;
-                o.opacity = !s && l, o.palette = p || a || l || c, this._preBuild(), this._buildComponents(), this._bindEvents(), this._finalBuild(), e && e.length && e.forEach((t => this.addSwatch(t)));
-                const {
-                    button: u,
-                    app: h
-                } = this._root;
-                this._nanopop = ((t, e, o) => {
-                    const n = "object" != typeof t || t instanceof HTMLElement ? {
-                        reference: t,
-                        popper: e,
-                        ...o
-                    } : t;
-                    return {
-                        update(t = n) {
-                            const {
-                                reference: e,
-                                popper: o
-                            } = Object.assign(n, t);
-                            if (!o || !e) throw new Error("Popper- or reference-element missing.");
-                            return O(e, o, n)
-                        }
-                    }
-                })(u, h, {
-                    margin: r
-                }), u.setAttribute("role", "button"), u.setAttribute("aria-label", this._t("btn:toggle"));
-                const d = this;
-                this._setupAnimationFrame = requestAnimationFrame((function e() {
-                    if (!h.offsetWidth) return requestAnimationFrame(e);
-                    d.setColor(t.default), d._rePositioningPicker(), t.defaultRepresentation && (d._representation = t.defaultRepresentation, d.setColorRepresentation(d._representation)), t.showAlways && d.show(), d._initializingActive = !1, d._emit("init")
-                }))
-            }
-            _preBuild() {
-                const {
-                    options: t
-                } = this;
-                for (const e of ["el", "container"]) t[e] = c(t[e]);
-                this._root = (t => {
-                    const {
-                        components: e,
-                        useAsButton: o,
-                        inline: n,
-                        appClass: i,
-                        theme: s,
-                        lockOpacity: r
-                    } = t.options, l = t => t ? "" : 'style="display:none" hidden', c = e => t._t(e), p = a(`\n      <div :ref="root" class="pickr">\n\n        ${o?"":'<button type="button" :ref="button" class="pcr-button"></button>'}\n\n        <div :ref="app" class="pcr-app ${i||""}" data-theme="${s}" ${n?'style="position: unset"':""} aria-label="${c("ui:dialog")}" role="window">\n          <div class="pcr-selection" ${l(e.palette)}>\n            <div :obj="preview" class="pcr-color-preview" ${l(e.preview)}>\n              <button type="button" :ref="lastColor" class="pcr-last-color" aria-label="${c("btn:last-color")}"></button>\n              <div :ref="currentColor" class="pcr-current-color"></div>\n            </div>\n\n            <div :obj="palette" class="pcr-color-palette">\n              <div :ref="picker" class="pcr-picker"></div>\n              <div :ref="palette" class="pcr-palette" tabindex="0" aria-label="${c("aria:palette")}" role="listbox"></div>\n            </div>\n\n            <div :obj="hue" class="pcr-color-chooser" ${l(e.hue)}>\n              <div :ref="picker" class="pcr-picker"></div>\n              <div :ref="slider" class="pcr-hue pcr-slider" tabindex="0" aria-label="${c("aria:hue")}" role="slider"></div>\n            </div>\n\n            <div :obj="opacity" class="pcr-color-opacity" ${l(e.opacity)}>\n              <div :ref="picker" class="pcr-picker"></div>\n              <div :ref="slider" class="pcr-opacity pcr-slider" tabindex="0" aria-label="${c("aria:opacity")}" role="slider"></div>\n            </div>\n          </div>\n\n          <div class="pcr-swatches ${e.palette?"":"pcr-last"}" :ref="swatches"></div>\n\n          <div :obj="interaction" class="pcr-interaction" ${l(Object.keys(e.interaction).length)}>\n            <input :ref="result" class="pcr-result" type="text" spellcheck="false" ${l(e.interaction.input)} aria-label="${c("aria:input")}">\n\n            <input :arr="options" class="pcr-type" data-type="HEXA" value="${r?"HEX":"HEXA"}" type="button" ${l(e.interaction.hex)}>\n            <input :arr="options" class="pcr-type" data-type="RGBA" value="${r?"RGB":"RGBA"}" type="button" ${l(e.interaction.rgba)}>\n            <input :arr="options" class="pcr-type" data-type="HSLA" value="${r?"HSL":"HSLA"}" type="button" ${l(e.interaction.hsla)}>\n            <input :arr="options" class="pcr-type" data-type="HSVA" value="${r?"HSV":"HSVA"}" type="button" ${l(e.interaction.hsva)}>\n            <input :arr="options" class="pcr-type" data-type="CMYK" value="CMYK" type="button" ${l(e.interaction.cmyk)}>\n\n            <input :ref="save" class="pcr-save" value="${c("btn:save")}" type="button" ${l(e.interaction.save)} aria-label="${c("aria:btn:save")}">\n            <input :ref="cancel" class="pcr-cancel" value="${c("btn:cancel")}" type="button" ${l(e.interaction.cancel)} aria-label="${c("aria:btn:cancel")}">\n            <input :ref="clear" class="pcr-clear" value="${c("btn:clear")}" type="button" ${l(e.interaction.clear)} aria-label="${c("aria:btn:clear")}">\n          </div>\n        </div>\n      </div>\n    `), u = p.interaction;
-                    return u.options.find((t => !t.hidden && !t.classList.add("active"))), u.type = () => u.options.find((t => t.classList.contains("active"))), p
-                })(this), t.useAsButton && (this._root.button = t.el), t.container.appendChild(this._root.root)
-            }
-            _finalBuild() {
-                const t = this.options,
-                    e = this._root;
-                if (t.container.removeChild(e.root), t.inline) {
-                    const o = t.el.parentElement;
-                    t.el.nextSibling ? o.insertBefore(e.app, t.el.nextSibling) : o.appendChild(e.app)
-                } else t.container.appendChild(e.app);
-                t.useAsButton ? t.inline && t.el.remove() : t.el.parentNode.replaceChild(e.root, t.el), t.disabled && this.disable(), t.comparison || (e.button.style.transition = "none", t.useAsButton || (e.preview.lastColor.style.transition = "none")), this.hide()
-            }
-            _buildComponents() {
-                const t = this,
-                    e = this.options.components,
-                    o = (t.options.sliders || "v").repeat(2),
-                    [n, i] = o.match(/^[vh]+$/g) ? o : [],
-                    s = () => this._color || (this._color = this._lastColor.clone()),
-                    r = {
-                        palette: $({
-                            element: t._root.palette.picker,
-                            wrapper: t._root.palette.palette,
-                            onstop: () => t._emit("changestop", "slider", t),
-                            onchange(o, n) {
-                                if (!e.palette) return;
-                                const i = s(),
-                                    {
-                                        _root: r,
-                                        options: a
-                                    } = t,
-                                    {
-                                        lastColor: l,
-                                        currentColor: c
-                                    } = r.preview;
-                                t._recalc && (i.s = 100 * o, i.v = 100 - 100 * n, i.v < 0 && (i.v = 0), t._updateOutput("slider"));
-                                const p = i.toRGBA().toString(0);
-                                this.element.style.background = p, this.wrapper.style.background = `\n                        linear-gradient(to top, rgba(0, 0, 0, ${i.a}), transparent),\n                        linear-gradient(to left, hsla(${i.h}, 100%, 50%, ${i.a}), rgba(255, 255, 255, ${i.a}))\n                    `, a.comparison ? a.useAsButton || t._lastColor || l.style.setProperty("--pcr-color", p) : (r.button.style.setProperty("--pcr-color", p), r.button.classList.remove("clear"));
-                                const u = i.toHEXA().toString();
-                                for (const {
-                                        el: e,
-                                        color: o
-                                    }
-                                    of t._swatchColors) e.classList[u === o.toHEXA().toString() ? "add" : "remove"]("pcr-active");
-                                c.style.setProperty("--pcr-color", p)
-                            }
-                        }),
-                        hue: $({
-                            lock: "v" === i ? "h" : "v",
-                            element: t._root.hue.picker,
-                            wrapper: t._root.hue.slider,
-                            onstop: () => t._emit("changestop", "slider", t),
-                            onchange(o) {
-                                if (!e.hue || !e.palette) return;
-                                const n = s();
-                                t._recalc && (n.h = 360 * o), this.element.style.backgroundColor = `hsl(${n.h}, 100%, 50%)`, r.palette.trigger()
-                            }
-                        }),
-                        opacity: $({
-                            lock: "v" === n ? "h" : "v",
-                            element: t._root.opacity.picker,
-                            wrapper: t._root.opacity.slider,
-                            onstop: () => t._emit("changestop", "slider", t),
-                            onchange(o) {
-                                if (!e.opacity || !e.palette) return;
-                                const n = s();
-                                t._recalc && (n.a = Math.round(100 * o) / 100), this.element.style.background = `rgba(0, 0, 0, ${n.a})`, r.palette.trigger()
-                            }
-                        }),
-                        selectable: k({
-                            elements: t._root.interaction.options,
-                            className: "active",
-                            onchange(e) {
-                                t._representation = e.target.getAttribute("data-type").toUpperCase(), t._recalc && t._updateOutput("swatch")
-                            }
-                        })
-                    };
-                this._components = r
-            }
-            _bindEvents() {
-                const {
-                    _root: t,
-                    options: e
-                } = this, o = [i(t.interaction.clear, "click", (() => this._clearColor())), i([t.interaction.cancel, t.preview.lastColor], "click", (() => {
-                    this.setHSVA(...(this._lastColor || this._color).toHSVA(), !0), this._emit("cancel")
-                })), i(t.interaction.save, "click", (() => {
-                    !this.applyColor() && !e.showAlways && this.hide()
-                })), i(t.interaction.result, ["keyup", "input"], (t => {
-                    this.setColor(t.target.value, !0) && !this._initializingActive && (this._emit("change", this._color, "input", this), this._emit("changestop", "input", this)), t.stopImmediatePropagation()
-                })), i(t.interaction.result, ["focus", "blur"], (t => {
-                    this._recalc = "blur" === t.type, this._recalc && this._updateOutput(null)
-                })), i([t.palette.palette, t.palette.picker, t.hue.slider, t.hue.picker, t.opacity.slider, t.opacity.picker], ["mousedown", "touchstart"], (() => this._recalc = !0), {
-                    passive: !0
-                })];
-                if (!e.showAlways) {
-                    const n = e.closeWithKey;
-                    o.push(i(t.button, "click", (() => this.isOpen() ? this.hide() : this.show())), i(document, "keyup", (t => this.isOpen() && (t.key === n || t.code === n) && this.hide())), i(document, ["touchstart", "mousedown"], (e => {
-                        this.isOpen() && !l(e).some((e => e === t.app || e === t.button)) && this.hide()
-                    }), {
-                        capture: !0
-                    }))
-                }
-                if (e.adjustableNumbers) {
-                    const e = {
-                        rgba: [255, 255, 255, 1],
-                        hsva: [360, 100, 100, 1],
-                        hsla: [360, 100, 100, 1],
-                        cmyk: [100, 100, 100, 100]
-                    };
-                    p(t.interaction.result, ((t, o, n) => {
-                        const i = e[this.getColorRepresentation().toLowerCase()];
-                        if (i) {
-                            const e = i[n],
-                                s = t + (e >= 100 ? 1e3 * o : o);
-                            return s <= 0 ? 0 : Number((s < e ? s : e).toPrecision(3))
-                        }
-                        return t
-                    }))
-                }
-                if (e.autoReposition && !e.inline) {
-                    let t = null;
-                    const n = this;
-                    o.push(i(window, ["scroll", "resize"], (() => {
-                        n.isOpen() && (e.closeOnScroll && n.hide(), null === t ? (t = setTimeout((() => t = null), 100), requestAnimationFrame((function e() {
-                            n._rePositioningPicker(), null !== t && requestAnimationFrame(e)
-                        }))) : (clearTimeout(t), t = setTimeout((() => t = null), 100)))
-                    }), {
-                        capture: !0
-                    }))
-                }
-                this._eventBindings = o
-            }
-            _rePositioningPicker() {
-                const {
-                    options: t
-                } = this;
-                if (!t.inline) {
-                    if (!this._nanopop.update({
-                            container: document.body.getBoundingClientRect(),
-                            position: t.position
-                        })) {
-                        const t = this._root.app,
-                            e = t.getBoundingClientRect();
-                        t.style.top = (window.innerHeight - e.height) / 2 + "px", t.style.left = (window.innerWidth - e.width) / 2 + "px"
-                    }
-                }
-            }
-            _updateOutput(t) {
-                const {
-                    _root: e,
-                    _color: o,
-                    options: n
-                } = this;
-                if (e.interaction.type()) {
-                    const t = `to${e.interaction.type().getAttribute("data-type")}`;
-                    e.interaction.result.value = "function" == typeof o[t] ? o[t]().toString(n.outputPrecision) : ""
-                }!this._initializingActive && this._recalc && this._emit("change", o, t, this)
-            }
-            _clearColor(t = !1) {
-                const {
-                    _root: e,
-                    options: o
-                } = this;
-                o.useAsButton || e.button.style.setProperty("--pcr-color", "rgba(0, 0, 0, 0.15)"), e.button.classList.add("clear"), o.showAlways || this.hide(), this._lastColor = null, this._initializingActive || t || (this._emit("save", null), this._emit("clear"))
-            }
-            _parseLocalColor(t) {
-                const {
-                    values: e,
-                    type: o,
-                    a: n
-                } = w(t), {
-                    lockOpacity: i
-                } = this.options, s = void 0 !== n && 1 !== n;
-                return e && 3 === e.length && (e[3] = void 0), {
-                    values: !e || i && s ? null : e,
-                    type: o
-                }
-            }
-            _t(t) {
-                return this.options.i18n[t] || L.I18N_DEFAULTS[t]
-            }
-            _emit(t, ...e) {
-                this._eventListener[t].forEach((t => t(...e, this)))
-            }
-            on(t, e) {
-                return this._eventListener[t].push(e), this
-            }
-            off(t, e) {
-                const o = this._eventListener[t] || [],
-                    n = o.indexOf(e);
-                return ~n && o.splice(n, 1), this
-            }
-            addSwatch(t) {
-                const {
-                    values: e
-                } = this._parseLocalColor(t);
-                if (e) {
-                    const {
-                        _swatchColors: t,
-                        _root: o
-                    } = this, n = A(...e), s = r(`<button type="button" style="--pcr-color: ${n.toRGBA().toString(0)}" aria-label="${this._t("btn:swatch")}"/>`);
-                    return o.swatches.appendChild(s), t.push({
-                        el: s,
-                        color: n
-                    }), this._eventBindings.push(i(s, "click", (() => {
-                        this.setHSVA(...n.toHSVA(), !0), this._emit("swatchselect", n), this._emit("change", n, "swatch", this)
-                    }))), !0
-                }
-                return !1
-            }
-            removeSwatch(t) {
-                const e = this._swatchColors[t];
-                if (e) {
-                    const {
-                        el: o
-                    } = e;
-                    return this._root.swatches.removeChild(o), this._swatchColors.splice(t, 1), !0
-                }
-                return !1
-            }
-            applyColor(t = !1) {
-                const {
-                    preview: e,
-                    button: o
-                } = this._root, n = this._color.toRGBA().toString(0);
-                return e.lastColor.style.setProperty("--pcr-color", n), this.options.useAsButton || o.style.setProperty("--pcr-color", n), o.classList.remove("clear"), this._lastColor = this._color.clone(), this._initializingActive || t || this._emit("save", this._color), this
-            }
-            destroy() {
-                cancelAnimationFrame(this._setupAnimationFrame), this._eventBindings.forEach((t => s(...t))), Object.keys(this._components).forEach((t => this._components[t].destroy()))
-            }
-            destroyAndRemove() {
-                this.destroy();
-                const {
-                    root: t,
-                    app: e
-                } = this._root;
-                t.parentElement && t.parentElement.removeChild(t), e.parentElement.removeChild(e), Object.keys(this).forEach((t => this[t] = null))
-            }
-            hide() {
-                return !!this.isOpen() && (this._root.app.classList.remove("visible"), this._emit("hide"), !0)
-            }
-            show() {
-                return !this.options.disabled && !this.isOpen() && (this._root.app.classList.add("visible"), this._rePositioningPicker(), this._emit("show", this._color), this)
-            }
-            isOpen() {
-                return this._root.app.classList.contains("visible")
-            }
-            setHSVA(t = 360, e = 0, o = 0, n = 1, i = !1) {
-                const s = this._recalc;
-                if (this._recalc = !1, t < 0 || t > 360 || e < 0 || e > 100 || o < 0 || o > 100 || n < 0 || n > 1) return !1;
-                this._color = A(t, e, o, n);
-                const {
-                    hue: r,
-                    opacity: a,
-                    palette: l
-                } = this._components;
-                return r.update(t / 360), a.update(n), l.update(e / 100, 1 - o / 100), i || this.applyColor(), s && this._updateOutput(), this._recalc = s, !0
-            }
-            setColor(t, e = !1) {
-                if (null === t) return this._clearColor(e), !0;
-                const {
-                    values: o,
-                    type: n
-                } = this._parseLocalColor(t);
-                if (o) {
-                    const t = n.toUpperCase(),
-                        {
-                            options: i
-                        } = this._root.interaction,
-                        s = i.find((e => e.getAttribute("data-type") === t));
-                    if (s && !s.hidden)
-                        for (const t of i) t.classList[t === s ? "add" : "remove"]("active");
-                    return !!this.setHSVA(...o, e) && this.setColorRepresentation(t)
-                }
-                return !1
-            }
-            setColorRepresentation(t) {
-                return t = t.toUpperCase(), !!this._root.interaction.options.find((e => e.getAttribute("data-type").startsWith(t) && !e.click()))
-            }
-            getColorRepresentation() {
-                return this._representation
-            }
-            getColor() {
-                return this._color
-            }
-            getSelectedColor() {
-                return this._lastColor
-            }
-            getRoot() {
-                return this._root
-            }
-            disable() {
-                return this.hide(), this.options.disabled = !0, this._root.button.classList.add("disabled"), this
-            }
-            enable() {
-                return this.options.disabled = !1, this._root.button.classList.remove("disabled"), this
-            }
-        }
-        return E(L, "utils", o), E(L, "version", "1.8.2"), E(L, "I18N_DEFAULTS", {
-            "ui:dialog": "color picker dialog",
-            "btn:toggle": "toggle color picker dialog",
-            "btn:swatch": "color swatch",
-            "btn:last-color": "use previous color",
-            "btn:save": "Save",
-            "btn:cancel": "Cancel",
-            "btn:clear": "Clear",
-            "aria:btn:save": "save and close",
-            "aria:btn:cancel": "cancel and close",
-            "aria:btn:clear": "clear and close",
-            "aria:input": "color input field",
-            "aria:palette": "color selection area",
-            "aria:hue": "hue selection slider",
-            "aria:opacity": "selection slider"
-        }), E(L, "DEFAULT_OPTIONS", {
-            appClass: null,
-            theme: "classic",
-            useAsButton: !1,
-            padding: 8,
-            disabled: !1,
-            comparison: !0,
-            closeOnScroll: !1,
-            outputPrecision: 0,
-            lockOpacity: !1,
-            autoReposition: !0,
-            container: "body",
-            components: {
-                interaction: {}
-            },
-            i18n: {},
-            swatches: null,
-            inline: !1,
-            sliders: null,
-            default: "#42445a",
-            defaultRepresentation: null,
-            position: "bottom-middle",
-            adjustableNumbers: !0,
-            showAlways: !1,
-            closeWithKey: "Escape"
-        }), E(L, "create", (t => new L(t))), e = e.default
-    })()
-}));
+/*! Pickr 1.8.2 MIT | https://github.com/Simonwep/pickr */ ! function(t, e) {
+    "object" == typeof exports && "object" == typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define([], e) : "object" == typeof exports ? exports.Pickr = e() : t.Pickr = e()
+}(self, (function() {
+    return (() => {
+        "use strict";
+        var t = {
+                d: (e, o) => {
+                    for (var n in o) t.o(o, n) && !t.o(e, n) && Object.defineProperty(e, n, {
+                        enumerable: !0,
+                        get: o[n]
+                    })
+                },
+                o: (t, e) => Object.prototype.hasOwnProperty.call(t, e),
+                r: t => {
+                    "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
+                        value: "Module"
+                    }), Object.defineProperty(t, "__esModule", {
+                        value: !0
+                    })
+                }
+            },
+            e = {};
+        t.d(e, {
+            default: () => L
+        });
+        var o = {};
+
+        function n(t, e, o, n, i = {}) {
+            e instanceof HTMLCollection || e instanceof NodeList ? e = Array.from(e) : Array.isArray(e) || (e = [e]), Array.isArray(o) || (o = [o]);
+            for (const s of e)
+                for (const e of o) s[t](e, n, {
+                    capture: !1,
+                    ...i
+                });
+            return Array.prototype.slice.call(arguments, 1)
+        }
+        t.r(o), t.d(o, {
+            adjustableInputNumbers: () => p,
+            createElementFromString: () => r,
+            createFromTemplate: () => a,
+            eventPath: () => l,
+            off: () => s,
+            on: () => i,
+            resolveElement: () => c
+        });
+        const i = n.bind(null, "addEventListener"),
+            s = n.bind(null, "removeEventListener");
+
+        function r(t) {
+            const e = document.createElement("div");
+            return e.innerHTML = t.trim(), e.firstElementChild
+        }
+
+        function a(t) {
+            const e = (t, e) => {
+                    const o = t.getAttribute(e);
+                    return t.removeAttribute(e), o
+                },
+                o = (t, n = {}) => {
+                    const i = e(t, ":obj"),
+                        s = e(t, ":ref"),
+                        r = i ? n[i] = {} : n;
+                    s && (n[s] = t);
+                    for (const n of Array.from(t.children)) {
+                        const t = e(n, ":arr"),
+                            i = o(n, t ? {} : r);
+                        t && (r[t] || (r[t] = [])).push(Object.keys(i).length ? i : n)
+                    }
+                    return n
+                };
+            return o(r(t))
+        }
+
+        function l(t) {
+            let e = t.path || t.composedPath && t.composedPath();
+            if (e) return e;
+            let o = t.target.parentElement;
+            for (e = [t.target, o]; o = o.parentElement;) e.push(o);
+            return e.push(document, window), e
+        }
+
+        function c(t) {
+            return t instanceof Element ? t : "string" == typeof t ? t.split(/>>/g).reduce(((t, e, o, n) => (t = t.querySelector(e), o < n.length - 1 ? t.shadowRoot : t)), document) : null
+        }
+
+        function p(t, e = (t => t)) {
+            function o(o) {
+                const n = [.001, .01, .1][Number(o.shiftKey || 2 * o.ctrlKey)] * (o.deltaY < 0 ? 1 : -1);
+                let i = 0,
+                    s = t.selectionStart;
+                t.value = t.value.replace(/[\d.]+/g, ((t, o) => o <= s && o + t.length >= s ? (s = o, e(Number(t), n, i)) : (i++, t))), t.focus(), t.setSelectionRange(s, s), o.preventDefault(), t.dispatchEvent(new Event("input"))
+            }
+            i(t, "focus", (() => i(window, "wheel", o, {
+                passive: !1
+            }))), i(t, "blur", (() => s(window, "wheel", o)))
+        }
+        const {
+            min: u,
+            max: h,
+            floor: d,
+            round: m
+        } = Math;
+
+        function f(t, e, o) {
+            e /= 100, o /= 100;
+            const n = d(t = t / 360 * 6),
+                i = t - n,
+                s = o * (1 - e),
+                r = o * (1 - i * e),
+                a = o * (1 - (1 - i) * e),
+                l = n % 6;
+            return [255 * [o, r, s, s, a, o][l], 255 * [a, o, o, r, s, s][l], 255 * [s, s, a, o, o, r][l]]
+        }
+
+        function v(t, e, o) {
+            const n = (2 - (e /= 100)) * (o /= 100) / 2;
+            return 0 !== n && (e = 1 === n ? 0 : n < .5 ? e * o / (2 * n) : e * o / (2 - 2 * n)), [t, 100 * e, 100 * n]
+        }
+
+        function b(t, e, o) {
+            const n = u(t /= 255, e /= 255, o /= 255),
+                i = h(t, e, o),
+                s = i - n;
+            let r, a;
+            if (0 === s) r = a = 0;
+            else {
+                a = s / i;
+                const n = ((i - t) / 6 + s / 2) / s,
+                    l = ((i - e) / 6 + s / 2) / s,
+                    c = ((i - o) / 6 + s / 2) / s;
+                t === i ? r = c - l : e === i ? r = 1 / 3 + n - c : o === i && (r = 2 / 3 + l - n), r < 0 ? r += 1 : r > 1 && (r -= 1)
+            }
+            return [360 * r, 100 * a, 100 * i]
+        }
+
+        function y(t, e, o, n) {
+            e /= 100, o /= 100;
+            return [...b(255 * (1 - u(1, (t /= 100) * (1 - (n /= 100)) + n)), 255 * (1 - u(1, e * (1 - n) + n)), 255 * (1 - u(1, o * (1 - n) + n)))]
+        }
+
+        function g(t, e, o) {
+            e /= 100;
+            const n = 2 * (e *= (o /= 100) < .5 ? o : 1 - o) / (o + e) * 100,
+                i = 100 * (o + e);
+            return [t, isNaN(n) ? 0 : n, i]
+        }
+
+        function _(t) {
+            return b(...t.match(/.{2}/g).map((t => parseInt(t, 16))))
+        }
+
+        function w(t) {
+            t = t.match(/^[a-zA-Z]+$/) ? function(t) {
+                if ("black" === t.toLowerCase()) return "#000";
+                const e = document.createElement("canvas").getContext("2d");
+                return e.fillStyle = t, "#000" === e.fillStyle ? null : e.fillStyle
+            }(t) : t;
+            const e = {
+                    cmyk: /^cmyk[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)/i,
+                    rgba: /^((rgba)|rgb)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]*?([\d.]+|$)/i,
+                    hsla: /^((hsla)|hsl)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]*?([\d.]+|$)/i,
+                    hsva: /^((hsva)|hsv)[\D]+([\d.]+)[\D]+([\d.]+)[\D]+([\d.]+)[\D]*?([\d.]+|$)/i,
+                    hexa: /^#?(([\dA-Fa-f]{3,4})|([\dA-Fa-f]{6})|([\dA-Fa-f]{8}))$/i
+                },
+                o = t => t.map((t => /^(|\d+)\.\d+|\d+$/.test(t) ? Number(t) : void 0));
+            let n;
+            t: for (const i in e) {
+                if (!(n = e[i].exec(t))) continue;
+                const s = t => !!n[2] == ("number" == typeof t);
+                switch (i) {
+                    case "cmyk": {
+                        const [, t, e, s, r] = o(n);
+                        if (t > 100 || e > 100 || s > 100 || r > 100) break t;
+                        return {
+                            values: y(t, e, s, r),
+                            type: i
+                        }
+                    }
+                    case "rgba": {
+                        const [, , , t, e, r, a] = o(n);
+                        if (t > 255 || e > 255 || r > 255 || a < 0 || a > 1 || !s(a)) break t;
+                        return {
+                            values: [...b(t, e, r), a],
+                            a,
+                            type: i
+                        }
+                    }
+                    case "hexa": {
+                        let [, t] = n;
+                        4 !== t.length && 3 !== t.length || (t = t.split("").map((t => t + t)).join(""));
+                        const e = t.substring(0, 6);
+                        let o = t.substring(6);
+                        return o = o ? parseInt(o, 16) / 255 : void 0, {
+                            values: [..._(e), o],
+                            a: o,
+                            type: i
+                        }
+                    }
+                    case "hsla": {
+                        const [, , , t, e, r, a] = o(n);
+                        if (t > 360 || e > 100 || r > 100 || a < 0 || a > 1 || !s(a)) break t;
+                        return {
+                            values: [...g(t, e, r), a],
+                            a,
+                            type: i
+                        }
+                    }
+                    case "hsva": {
+                        const [, , , t, e, r, a] = o(n);
+                        if (t > 360 || e > 100 || r > 100 || a < 0 || a > 1 || !s(a)) break t;
+                        return {
+                            values: [t, e, r, a],
+                            a,
+                            type: i
+                        }
+                    }
+                }
+            }
+            return {
+                values: null,
+                type: null
+            }
+        }
+
+        function A(t = 0, e = 0, o = 0, n = 1) {
+            const i = (t, e) => (o = -1) => e(~o ? t.map((t => Number(t.toFixed(o)))) : t),
+                s = {
+                    h: t,
+                    s: e,
+                    v: o,
+                    a: n,
+                    toHSVA() {
+                        const t = [s.h, s.s, s.v, s.a];
+                        return t.toString = i(t, (t => `hsva(${t[0]}, ${t[1]}%, ${t[2]}%, ${s.a})`)), t
+                    },
+                    toHSLA() {
+                        const t = [...v(s.h, s.s, s.v), s.a];
+                        return t.toString = i(t, (t => `hsla(${t[0]}, ${t[1]}%, ${t[2]}%, ${s.a})`)), t
+                    },
+                    toRGBA() {
+                        const t = [...f(s.h, s.s, s.v), s.a];
+                        return t.toString = i(t, (t => `rgba(${t[0]}, ${t[1]}, ${t[2]}, ${s.a})`)), t
+                    },
+                    toCMYK() {
+                        const t = function(t, e, o) {
+                            const n = f(t, e, o),
+                                i = n[0] / 255,
+                                s = n[1] / 255,
+                                r = n[2] / 255,
+                                a = u(1 - i, 1 - s, 1 - r);
+                            return [100 * (1 === a ? 0 : (1 - i - a) / (1 - a)), 100 * (1 === a ? 0 : (1 - s - a) / (1 - a)), 100 * (1 === a ? 0 : (1 - r - a) / (1 - a)), 100 * a]
+                        }(s.h, s.s, s.v);
+                        return t.toString = i(t, (t => `cmyk(${t[0]}%, ${t[1]}%, ${t[2]}%, ${t[3]}%)`)), t
+                    },
+                    toHEXA() {
+                        const t = function(t, e, o) {
+                                return f(t, e, o).map((t => m(t).toString(16).padStart(2, "0")))
+                            }(s.h, s.s, s.v),
+                            e = s.a >= 1 ? "" : Number((255 * s.a).toFixed(0)).toString(16).toUpperCase().padStart(2, "0");
+                        return e && t.push(e), t.toString = () => `#${t.join("").toUpperCase()}`, t
+                    },
+                    clone: () => A(s.h, s.s, s.v, s.a)
+                };
+            return s
+        }
+        const C = t => Math.max(Math.min(t, 1), 0);
+
+        function $(t) {
+            const e = {
+                    options: Object.assign({
+                        lock: null,
+                        onchange: () => 0,
+                        onstop: () => 0
+                    }, t),
+                    _keyboard(t) {
+                        const {
+                            options: o
+                        } = e, {
+                            type: n,
+                            key: i
+                        } = t;
+                        if (document.activeElement === o.wrapper) {
+                            const {
+                                lock: o
+                            } = e.options, s = "ArrowUp" === i, r = "ArrowRight" === i, a = "ArrowDown" === i, l = "ArrowLeft" === i;
+                            if ("keydown" === n && (s || r || a || l)) {
+                                let n = 0,
+                                    i = 0;
+                                "v" === o ? n = s || r ? 1 : -1 : "h" === o ? n = s || r ? -1 : 1 : (i = s ? -1 : a ? 1 : 0, n = l ? -1 : r ? 1 : 0), e.update(C(e.cache.x + .01 * n), C(e.cache.y + .01 * i)), t.preventDefault()
+                            } else i.startsWith("Arrow") && (e.options.onstop(), t.preventDefault())
+                        }
+                    },
+                    _tapstart(t) {
+                        i(document, ["mouseup", "touchend", "touchcancel"], e._tapstop), i(document, ["mousemove", "touchmove"], e._tapmove), t.cancelable && t.preventDefault(), e._tapmove(t)
+                    },
+                    _tapmove(t) {
+                        const {
+                            options: o,
+                            cache: n
+                        } = e, {
+                            lock: i,
+                            element: s,
+                            wrapper: r
+                        } = o, a = r.getBoundingClientRect();
+                        let l = 0,
+                            c = 0;
+                        if (t) {
+                            const e = t && t.touches && t.touches[0];
+                            l = t ? (e || t).clientX : 0, c = t ? (e || t).clientY : 0, l < a.left ? l = a.left : l > a.left + a.width && (l = a.left + a.width), c < a.top ? c = a.top : c > a.top + a.height && (c = a.top + a.height), l -= a.left, c -= a.top
+                        } else n && (l = n.x * a.width, c = n.y * a.height);
+                        "h" !== i && (s.style.left = `calc(${l/a.width*100}% - ${s.offsetWidth/2}px)`), "v" !== i && (s.style.top = `calc(${c/a.height*100}% - ${s.offsetHeight/2}px)`), e.cache = {
+                            x: l / a.width,
+                            y: c / a.height
+                        };
+                        const p = C(l / a.width),
+                            u = C(c / a.height);
+                        switch (i) {
+                            case "v":
+                                return o.onchange(p);
+                            case "h":
+                                return o.onchange(u);
+                            default:
+                                return o.onchange(p, u)
+                        }
+                    },
+                    _tapstop() {
+                        e.options.onstop(), s(document, ["mouseup", "touchend", "touchcancel"], e._tapstop), s(document, ["mousemove", "touchmove"], e._tapmove)
+                    },
+                    trigger() {
+                        e._tapmove()
+                    },
+                    update(t = 0, o = 0) {
+                        const {
+                            left: n,
+                            top: i,
+                            width: s,
+                            height: r
+                        } = e.options.wrapper.getBoundingClientRect();
+                        "h" === e.options.lock && (o = t), e._tapmove({
+                            clientX: n + s * t,
+                            clientY: i + r * o
+                        })
+                    },
+                    destroy() {
+                        const {
+                            options: t,
+                            _tapstart: o,
+                            _keyboard: n
+                        } = e;
+                        s(document, ["keydown", "keyup"], n), s([t.wrapper, t.element], "mousedown", o), s([t.wrapper, t.element], "touchstart", o, {
+                            passive: !1
+                        })
+                    }
+                },
+                {
+                    options: o,
+                    _tapstart: n,
+                    _keyboard: r
+                } = e;
+            return i([o.wrapper, o.element], "mousedown", n), i([o.wrapper, o.element], "touchstart", n, {
+                passive: !1
+            }), i(document, ["keydown", "keyup"], r), e
+        }
+
+        function k(t = {}) {
+            t = Object.assign({
+                onchange: () => 0,
+                className: "",
+                elements: []
+            }, t);
+            const e = i(t.elements, "click", (e => {
+                t.elements.forEach((o => o.classList[e.target === o ? "add" : "remove"](t.className))), t.onchange(e), e.stopPropagation()
+            }));
+            return {
+                destroy: () => s(...e)
+            }
+        }
+        const S = {
+                variantFlipOrder: {
+                    start: "sme",
+                    middle: "mse",
+                    end: "ems"
+                },
+                positionFlipOrder: {
+                    top: "tbrl",
+                    right: "rltb",
+                    bottom: "btrl",
+                    left: "lrbt"
+                },
+                position: "bottom",
+                margin: 8
+            },
+            O = (t, e, o) => {
+                const {
+                    container: n,
+                    margin: i,
+                    position: s,
+                    variantFlipOrder: r,
+                    positionFlipOrder: a
+                } = {
+                    container: document.documentElement.getBoundingClientRect(),
+                    ...S,
+                    ...o
+                }, {
+                    left: l,
+                    top: c
+                } = e.style;
+                e.style.left = "0", e.style.top = "0";
+                const p = t.getBoundingClientRect(),
+                    u = e.getBoundingClientRect(),
+                    h = {
+                        t: p.top - u.height - i,
+                        b: p.bottom + i,
+                        r: p.right + i,
+                        l: p.left - u.width - i
+                    },
+                    d = {
+                        vs: p.left,
+                        vm: p.left + p.width / 2 + -u.width / 2,
+                        ve: p.left + p.width - u.width,
+                        hs: p.top,
+                        hm: p.bottom - p.height / 2 - u.height / 2,
+                        he: p.bottom - u.height
+                    },
+                    [m, f = "middle"] = s.split("-"),
+                    v = a[m],
+                    b = r[f],
+                    {
+                        top: y,
+                        left: g,
+                        bottom: _,
+                        right: w
+                    } = n;
+                for (const t of v) {
+                    const o = "t" === t || "b" === t,
+                        n = h[t],
+                        [i, s] = o ? ["top", "left"] : ["left", "top"],
+                        [r, a] = o ? [u.height, u.width] : [u.width, u.height],
+                        [l, c] = o ? [_, w] : [w, _],
+                        [p, m] = o ? [y, g] : [g, y];
+                    if (!(n < p || n + r > l))
+                        for (const r of b) {
+                            const l = d[(o ? "v" : "h") + r];
+                            if (!(l < m || l + a > c)) return e.style[s] = l - u[s] + "px", e.style[i] = n - u[i] + "px", t + r
+                        }
+                }
+                return e.style.left = l, e.style.top = c, null
+            };
+
+        function E(t, e, o) {
+            return e in t ? Object.defineProperty(t, e, {
+                value: o,
+                enumerable: !0,
+                configurable: !0,
+                writable: !0
+            }) : t[e] = o, t
+        }
+        class L {
+            constructor(t) {
+                E(this, "_initializingActive", !0), E(this, "_recalc", !0), E(this, "_nanopop", null), E(this, "_root", null), E(this, "_color", A()), E(this, "_lastColor", A()), E(this, "_swatchColors", []), E(this, "_setupAnimationFrame", null), E(this, "_eventListener", {
+                    init: [],
+                    save: [],
+                    hide: [],
+                    show: [],
+                    clear: [],
+                    change: [],
+                    changestop: [],
+                    cancel: [],
+                    swatchselect: []
+                }), this.options = t = Object.assign({
+                    ...L.DEFAULT_OPTIONS
+                }, t);
+                const {
+                    swatches: e,
+                    components: o,
+                    theme: n,
+                    sliders: i,
+                    lockOpacity: s,
+                    padding: r
+                } = t;
+                ["nano", "monolith"].includes(n) && !i && (t.sliders = "h"), o.interaction || (o.interaction = {});
+                const {
+                    preview: a,
+                    opacity: l,
+                    hue: c,
+                    palette: p
+                } = o;
+                o.opacity = !s && l, o.palette = p || a || l || c, this._preBuild(), this._buildComponents(), this._bindEvents(), this._finalBuild(), e && e.length && e.forEach((t => this.addSwatch(t)));
+                const {
+                    button: u,
+                    app: h
+                } = this._root;
+                this._nanopop = ((t, e, o) => {
+                    const n = "object" != typeof t || t instanceof HTMLElement ? {
+                        reference: t,
+                        popper: e,
+                        ...o
+                    } : t;
+                    return {
+                        update(t = n) {
+                            const {
+                                reference: e,
+                                popper: o
+                            } = Object.assign(n, t);
+                            if (!o || !e) throw new Error("Popper- or reference-element missing.");
+                            return O(e, o, n)
+                        }
+                    }
+                })(u, h, {
+                    margin: r
+                }), u.setAttribute("role", "button"), u.setAttribute("aria-label", this._t("btn:toggle"));
+                const d = this;
+                this._setupAnimationFrame = requestAnimationFrame((function e() {
+                    if (!h.offsetWidth) return requestAnimationFrame(e);
+                    d.setColor(t.default), d._rePositioningPicker(), t.defaultRepresentation && (d._representation = t.defaultRepresentation, d.setColorRepresentation(d._representation)), t.showAlways && d.show(), d._initializingActive = !1, d._emit("init")
+                }))
+            }
+            _preBuild() {
+                const {
+                    options: t
+                } = this;
+                for (const e of ["el", "container"]) t[e] = c(t[e]);
+                this._root = (t => {
+                    const {
+                        components: e,
+                        useAsButton: o,
+                        inline: n,
+                        appClass: i,
+                        theme: s,
+                        lockOpacity: r
+                    } = t.options, l = t => t ? "" : 'style="display:none" hidden', c = e => t._t(e), p = a(`\n      <div :ref="root" class="pickr">\n\n        ${o?"":'<button type="button" :ref="button" class="pcr-button"></button>'}\n\n        <div :ref="app" class="pcr-app ${i||""}" data-theme="${s}" ${n?'style="position: unset"':""} aria-label="${c("ui:dialog")}" role="window">\n          <div class="pcr-selection" ${l(e.palette)}>\n            <div :obj="preview" class="pcr-color-preview" ${l(e.preview)}>\n              <button type="button" :ref="lastColor" class="pcr-last-color" aria-label="${c("btn:last-color")}"></button>\n              <div :ref="currentColor" class="pcr-current-color"></div>\n            </div>\n\n            <div :obj="palette" class="pcr-color-palette">\n              <div :ref="picker" class="pcr-picker"></div>\n              <div :ref="palette" class="pcr-palette" tabindex="0" aria-label="${c("aria:palette")}" role="listbox"></div>\n            </div>\n\n            <div :obj="hue" class="pcr-color-chooser" ${l(e.hue)}>\n              <div :ref="picker" class="pcr-picker"></div>\n              <div :ref="slider" class="pcr-hue pcr-slider" tabindex="0" aria-label="${c("aria:hue")}" role="slider"></div>\n            </div>\n\n            <div :obj="opacity" class="pcr-color-opacity" ${l(e.opacity)}>\n              <div :ref="picker" class="pcr-picker"></div>\n              <div :ref="slider" class="pcr-opacity pcr-slider" tabindex="0" aria-label="${c("aria:opacity")}" role="slider"></div>\n            </div>\n          </div>\n\n          <div class="pcr-swatches ${e.palette?"":"pcr-last"}" :ref="swatches"></div>\n\n          <div :obj="interaction" class="pcr-interaction" ${l(Object.keys(e.interaction).length)}>\n            <input :ref="result" class="pcr-result" type="text" spellcheck="false" ${l(e.interaction.input)} aria-label="${c("aria:input")}">\n\n            <input :arr="options" class="pcr-type" data-type="HEXA" value="${r?"HEX":"HEXA"}" type="button" ${l(e.interaction.hex)}>\n            <input :arr="options" class="pcr-type" data-type="RGBA" value="${r?"RGB":"RGBA"}" type="button" ${l(e.interaction.rgba)}>\n            <input :arr="options" class="pcr-type" data-type="HSLA" value="${r?"HSL":"HSLA"}" type="button" ${l(e.interaction.hsla)}>\n            <input :arr="options" class="pcr-type" data-type="HSVA" value="${r?"HSV":"HSVA"}" type="button" ${l(e.interaction.hsva)}>\n            <input :arr="options" class="pcr-type" data-type="CMYK" value="CMYK" type="button" ${l(e.interaction.cmyk)}>\n\n            <input :ref="save" class="pcr-save" value="${c("btn:save")}" type="button" ${l(e.interaction.save)} aria-label="${c("aria:btn:save")}">\n            <input :ref="cancel" class="pcr-cancel" value="${c("btn:cancel")}" type="button" ${l(e.interaction.cancel)} aria-label="${c("aria:btn:cancel")}">\n            <input :ref="clear" class="pcr-clear" value="${c("btn:clear")}" type="button" ${l(e.interaction.clear)} aria-label="${c("aria:btn:clear")}">\n          </div>\n        </div>\n      </div>\n    `), u = p.interaction;
+                    return u.options.find((t => !t.hidden && !t.classList.add("active"))), u.type = () => u.options.find((t => t.classList.contains("active"))), p
+                })(this), t.useAsButton && (this._root.button = t.el), t.container.appendChild(this._root.root)
+            }
+            _finalBuild() {
+                const t = this.options,
+                    e = this._root;
+                if (t.container.removeChild(e.root), t.inline) {
+                    const o = t.el.parentElement;
+                    t.el.nextSibling ? o.insertBefore(e.app, t.el.nextSibling) : o.appendChild(e.app)
+                } else t.container.appendChild(e.app);
+                t.useAsButton ? t.inline && t.el.remove() : t.el.parentNode.replaceChild(e.root, t.el), t.disabled && this.disable(), t.comparison || (e.button.style.transition = "none", t.useAsButton || (e.preview.lastColor.style.transition = "none")), this.hide()
+            }
+            _buildComponents() {
+                const t = this,
+                    e = this.options.components,
+                    o = (t.options.sliders || "v").repeat(2),
+                    [n, i] = o.match(/^[vh]+$/g) ? o : [],
+                    s = () => this._color || (this._color = this._lastColor.clone()),
+                    r = {
+                        palette: $({
+                            element: t._root.palette.picker,
+                            wrapper: t._root.palette.palette,
+                            onstop: () => t._emit("changestop", "slider", t),
+                            onchange(o, n) {
+                                if (!e.palette) return;
+                                const i = s(),
+                                    {
+                                        _root: r,
+                                        options: a
+                                    } = t,
+                                    {
+                                        lastColor: l,
+                                        currentColor: c
+                                    } = r.preview;
+                                t._recalc && (i.s = 100 * o, i.v = 100 - 100 * n, i.v < 0 && (i.v = 0), t._updateOutput("slider"));
+                                const p = i.toRGBA().toString(0);
+                                this.element.style.background = p, this.wrapper.style.background = `\n                        linear-gradient(to top, rgba(0, 0, 0, ${i.a}), transparent),\n                        linear-gradient(to left, hsla(${i.h}, 100%, 50%, ${i.a}), rgba(255, 255, 255, ${i.a}))\n                    `, a.comparison ? a.useAsButton || t._lastColor || l.style.setProperty("--pcr-color", p) : (r.button.style.setProperty("--pcr-color", p), r.button.classList.remove("clear"));
+                                const u = i.toHEXA().toString();
+                                for (const {
+                                        el: e,
+                                        color: o
+                                    }
+                                    of t._swatchColors) e.classList[u === o.toHEXA().toString() ? "add" : "remove"]("pcr-active");
+                                c.style.setProperty("--pcr-color", p)
+                            }
+                        }),
+                        hue: $({
+                            lock: "v" === i ? "h" : "v",
+                            element: t._root.hue.picker,
+                            wrapper: t._root.hue.slider,
+                            onstop: () => t._emit("changestop", "slider", t),
+                            onchange(o) {
+                                if (!e.hue || !e.palette) return;
+                                const n = s();
+                                t._recalc && (n.h = 360 * o), this.element.style.backgroundColor = `hsl(${n.h}, 100%, 50%)`, r.palette.trigger()
+                            }
+                        }),
+                        opacity: $({
+                            lock: "v" === n ? "h" : "v",
+                            element: t._root.opacity.picker,
+                            wrapper: t._root.opacity.slider,
+                            onstop: () => t._emit("changestop", "slider", t),
+                            onchange(o) {
+                                if (!e.opacity || !e.palette) return;
+                                const n = s();
+                                t._recalc && (n.a = Math.round(100 * o) / 100), this.element.style.background = `rgba(0, 0, 0, ${n.a})`, r.palette.trigger()
+                            }
+                        }),
+                        selectable: k({
+                            elements: t._root.interaction.options,
+                            className: "active",
+                            onchange(e) {
+                                t._representation = e.target.getAttribute("data-type").toUpperCase(), t._recalc && t._updateOutput("swatch")
+                            }
+                        })
+                    };
+                this._components = r
+            }
+            _bindEvents() {
+                const {
+                    _root: t,
+                    options: e
+                } = this, o = [i(t.interaction.clear, "click", (() => this._clearColor())), i([t.interaction.cancel, t.preview.lastColor], "click", (() => {
+                    this.setHSVA(...(this._lastColor || this._color).toHSVA(), !0), this._emit("cancel")
+                })), i(t.interaction.save, "click", (() => {
+                    !this.applyColor() && !e.showAlways && this.hide()
+                })), i(t.interaction.result, ["keyup", "input"], (t => {
+                    this.setColor(t.target.value, !0) && !this._initializingActive && (this._emit("change", this._color, "input", this), this._emit("changestop", "input", this)), t.stopImmediatePropagation()
+                })), i(t.interaction.result, ["focus", "blur"], (t => {
+                    this._recalc = "blur" === t.type, this._recalc && this._updateOutput(null)
+                })), i([t.palette.palette, t.palette.picker, t.hue.slider, t.hue.picker, t.opacity.slider, t.opacity.picker], ["mousedown", "touchstart"], (() => this._recalc = !0), {
+                    passive: !0
+                })];
+                if (!e.showAlways) {
+                    const n = e.closeWithKey;
+                    o.push(i(t.button, "click", (() => this.isOpen() ? this.hide() : this.show())), i(document, "keyup", (t => this.isOpen() && (t.key === n || t.code === n) && this.hide())), i(document, ["touchstart", "mousedown"], (e => {
+                        this.isOpen() && !l(e).some((e => e === t.app || e === t.button)) && this.hide()
+                    }), {
+                        capture: !0
+                    }))
+                }
+                if (e.adjustableNumbers) {
+                    const e = {
+                        rgba: [255, 255, 255, 1],
+                        hsva: [360, 100, 100, 1],
+                        hsla: [360, 100, 100, 1],
+                        cmyk: [100, 100, 100, 100]
+                    };
+                    p(t.interaction.result, ((t, o, n) => {
+                        const i = e[this.getColorRepresentation().toLowerCase()];
+                        if (i) {
+                            const e = i[n],
+                                s = t + (e >= 100 ? 1e3 * o : o);
+                            return s <= 0 ? 0 : Number((s < e ? s : e).toPrecision(3))
+                        }
+                        return t
+                    }))
+                }
+                if (e.autoReposition && !e.inline) {
+                    let t = null;
+                    const n = this;
+                    o.push(i(window, ["scroll", "resize"], (() => {
+                        n.isOpen() && (e.closeOnScroll && n.hide(), null === t ? (t = setTimeout((() => t = null), 100), requestAnimationFrame((function e() {
+                            n._rePositioningPicker(), null !== t && requestAnimationFrame(e)
+                        }))) : (clearTimeout(t), t = setTimeout((() => t = null), 100)))
+                    }), {
+                        capture: !0
+                    }))
+                }
+                this._eventBindings = o
+            }
+            _rePositioningPicker() {
+                const {
+                    options: t
+                } = this;
+                if (!t.inline) {
+                    if (!this._nanopop.update({
+                            container: document.body.getBoundingClientRect(),
+                            position: t.position
+                        })) {
+                        const t = this._root.app,
+                            e = t.getBoundingClientRect();
+                        t.style.top = (window.innerHeight - e.height) / 2 + "px", t.style.left = (window.innerWidth - e.width) / 2 + "px"
+                    }
+                }
+            }
+            _updateOutput(t) {
+                const {
+                    _root: e,
+                    _color: o,
+                    options: n
+                } = this;
+                if (e.interaction.type()) {
+                    const t = `to${e.interaction.type().getAttribute("data-type")}`;
+                    e.interaction.result.value = "function" == typeof o[t] ? o[t]().toString(n.outputPrecision) : ""
+                }!this._initializingActive && this._recalc && this._emit("change", o, t, this)
+            }
+            _clearColor(t = !1) {
+                const {
+                    _root: e,
+                    options: o
+                } = this;
+                o.useAsButton || e.button.style.setProperty("--pcr-color", "rgba(0, 0, 0, 0.15)"), e.button.classList.add("clear"), o.showAlways || this.hide(), this._lastColor = null, this._initializingActive || t || (this._emit("save", null), this._emit("clear"))
+            }
+            _parseLocalColor(t) {
+                const {
+                    values: e,
+                    type: o,
+                    a: n
+                } = w(t), {
+                    lockOpacity: i
+                } = this.options, s = void 0 !== n && 1 !== n;
+                return e && 3 === e.length && (e[3] = void 0), {
+                    values: !e || i && s ? null : e,
+                    type: o
+                }
+            }
+            _t(t) {
+                return this.options.i18n[t] || L.I18N_DEFAULTS[t]
+            }
+            _emit(t, ...e) {
+                this._eventListener[t].forEach((t => t(...e, this)))
+            }
+            on(t, e) {
+                return this._eventListener[t].push(e), this
+            }
+            off(t, e) {
+                const o = this._eventListener[t] || [],
+                    n = o.indexOf(e);
+                return ~n && o.splice(n, 1), this
+            }
+            addSwatch(t) {
+                const {
+                    values: e
+                } = this._parseLocalColor(t);
+                if (e) {
+                    const {
+                        _swatchColors: t,
+                        _root: o
+                    } = this, n = A(...e), s = r(`<button type="button" style="--pcr-color: ${n.toRGBA().toString(0)}" aria-label="${this._t("btn:swatch")}"/>`);
+                    return o.swatches.appendChild(s), t.push({
+                        el: s,
+                        color: n
+                    }), this._eventBindings.push(i(s, "click", (() => {
+                        this.setHSVA(...n.toHSVA(), !0), this._emit("swatchselect", n), this._emit("change", n, "swatch", this)
+                    }))), !0
+                }
+                return !1
+            }
+            removeSwatch(t) {
+                const e = this._swatchColors[t];
+                if (e) {
+                    const {
+                        el: o
+                    } = e;
+                    return this._root.swatches.removeChild(o), this._swatchColors.splice(t, 1), !0
+                }
+                return !1
+            }
+            applyColor(t = !1) {
+                const {
+                    preview: e,
+                    button: o
+                } = this._root, n = this._color.toRGBA().toString(0);
+                return e.lastColor.style.setProperty("--pcr-color", n), this.options.useAsButton || o.style.setProperty("--pcr-color", n), o.classList.remove("clear"), this._lastColor = this._color.clone(), this._initializingActive || t || this._emit("save", this._color), this
+            }
+            destroy() {
+                cancelAnimationFrame(this._setupAnimationFrame), this._eventBindings.forEach((t => s(...t))), Object.keys(this._components).forEach((t => this._components[t].destroy()))
+            }
+            destroyAndRemove() {
+                this.destroy();
+                const {
+                    root: t,
+                    app: e
+                } = this._root;
+                t.parentElement && t.parentElement.removeChild(t), e.parentElement.removeChild(e), Object.keys(this).forEach((t => this[t] = null))
+            }
+            hide() {
+                return !!this.isOpen() && (this._root.app.classList.remove("visible"), this._emit("hide"), !0)
+            }
+            show() {
+                return !this.options.disabled && !this.isOpen() && (this._root.app.classList.add("visible"), this._rePositioningPicker(), this._emit("show", this._color), this)
+            }
+            isOpen() {
+                return this._root.app.classList.contains("visible")
+            }
+            setHSVA(t = 360, e = 0, o = 0, n = 1, i = !1) {
+                const s = this._recalc;
+                if (this._recalc = !1, t < 0 || t > 360 || e < 0 || e > 100 || o < 0 || o > 100 || n < 0 || n > 1) return !1;
+                this._color = A(t, e, o, n);
+                const {
+                    hue: r,
+                    opacity: a,
+                    palette: l
+                } = this._components;
+                return r.update(t / 360), a.update(n), l.update(e / 100, 1 - o / 100), i || this.applyColor(), s && this._updateOutput(), this._recalc = s, !0
+            }
+            setColor(t, e = !1) {
+                if (null === t) return this._clearColor(e), !0;
+                const {
+                    values: o,
+                    type: n
+                } = this._parseLocalColor(t);
+                if (o) {
+                    const t = n.toUpperCase(),
+                        {
+                            options: i
+                        } = this._root.interaction,
+                        s = i.find((e => e.getAttribute("data-type") === t));
+                    if (s && !s.hidden)
+                        for (const t of i) t.classList[t === s ? "add" : "remove"]("active");
+                    return !!this.setHSVA(...o, e) && this.setColorRepresentation(t)
+                }
+                return !1
+            }
+            setColorRepresentation(t) {
+                return t = t.toUpperCase(), !!this._root.interaction.options.find((e => e.getAttribute("data-type").startsWith(t) && !e.click()))
+            }
+            getColorRepresentation() {
+                return this._representation
+            }
+            getColor() {
+                return this._color
+            }
+            getSelectedColor() {
+                return this._lastColor
+            }
+            getRoot() {
+                return this._root
+            }
+            disable() {
+                return this.hide(), this.options.disabled = !0, this._root.button.classList.add("disabled"), this
+            }
+            enable() {
+                return this.options.disabled = !1, this._root.button.classList.remove("disabled"), this
+            }
+        }
+        return E(L, "utils", o), E(L, "version", "1.8.2"), E(L, "I18N_DEFAULTS", {
+            "ui:dialog": "color picker dialog",
+            "btn:toggle": "toggle color picker dialog",
+            "btn:swatch": "color swatch",
+            "btn:last-color": "use previous color",
+            "btn:save": "Save",
+            "btn:cancel": "Cancel",
+            "btn:clear": "Clear",
+            "aria:btn:save": "save and close",
+            "aria:btn:cancel": "cancel and close",
+            "aria:btn:clear": "clear and close",
+            "aria:input": "color input field",
+            "aria:palette": "color selection area",
+            "aria:hue": "hue selection slider",
+            "aria:opacity": "selection slider"
+        }), E(L, "DEFAULT_OPTIONS", {
+            appClass: null,
+            theme: "classic",
+            useAsButton: !1,
+            padding: 8,
+            disabled: !1,
+            comparison: !0,
+            closeOnScroll: !1,
+            outputPrecision: 0,
+            lockOpacity: !1,
+            autoReposition: !0,
+            container: "body",
+            components: {
+                interaction: {}
+            },
+            i18n: {},
+            swatches: null,
+            inline: !1,
+            sliders: null,
+            default: "#42445a",
+            defaultRepresentation: null,
+            position: "bottom-middle",
+            adjustableNumbers: !0,
+            showAlways: !1,
+            closeWithKey: "Escape"
+        }), E(L, "create", (t => new L(t))), e = e.default
+    })()
+}));
 //# sourceMappingURL=pickr.min.js.map
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/font_picker/font-picker.css` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/justify/justify-controller.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/justify/justify-widget.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,16 @@
 class JustifyWidget {
     constructor(querySelector, value = null, targets = []) {
         this.targets = targets;
         this.radioSelect = document.querySelector(`#${querySelector}`);
         this.radioSelectInputs = {};
         let inputs = this.radioSelect.querySelectorAll('input[type="radio"]');
 
+        console.log('JustifyWidget', this.radioSelect, inputs);
+
         for (let i = 0; i < inputs.length; i++) {
             let input = inputs[i];
             this.radioSelectInputs[input.value] = input;
             input.addEventListener('change', (e) => {
                 this.setState(e.target.value);
             });
         }
@@ -33,36 +35,46 @@
             if (!targetWrapper) {
                 console.error(`Target wrapper not found for target: ${target}`, this.targetPanel);
                 continue
             }
             let inputs = [
                 ...targetWrapper.find('input'),
                 ...targetWrapper.find('textarea'),
+                ...targetWrapper.find('.Draftail-Editor'),
             ];
 
             let $targetWrapper = $(targetWrapper);
             const value = this.getValue();
             for (let j = 0; j < keys.length; j++) {
                 let key = keys[j];
                 $targetWrapper.removeClass(key);
             }
 
             $targetWrapper.addClass(value);
 
             for (let j = 0; j < inputs.length; j++) {
                 let input = inputs[j];
+                let $input = $(input);
                 let inputId = input.id;
                 if (inputId && inputId.length >= target.length && inputId.substring(inputId.length - target.length) === target) {
                     for (let k = 0; k < keys.length; k++) {
                         let key = keys[k];
-                        if ($(input).hasClass(key)) {
-                            $(input).removeClass(key);
+                        if ($input.hasClass(key)) {
+                            $input.removeClass(key);
                         }
                     }
-                    $(input).addClass(value);
+                    $input.addClass(value);
+                } else if ($input.hasClass('Draftail-Editor')) {
+                    for (let k = 0; k < keys.length; k++) {
+                        let key = keys[k];
+                        if ($input.hasClass(key)) {
+                            $input.removeClass(key);
+                        }
+                    }
+                    $input.addClass(value);
                 }
             }
             if (inputs.length === 0) {
                 console.error(`No inputs found for target: ${target}`, targetWrapper);
             }
         }
     }
@@ -70,25 +82,28 @@
     setDefault() {
         if (!this.radioSelectInputs) {
             return;
         }
         const keys = Object.keys(this.radioSelectInputs)
         for (let i = 0; i < keys.length; i++) {
             let key = keys[i];
+            if (!key) {
+                continue;
+            }
             if (this.radioSelectInputs[key].checked) {
-                this.setState(key);
+                this.setState(key, true);
                 return;
             }
         }
         const key = keys[0]
-        this.setState(this.radioSelectInputs[key].value);
+        this.setState(this.radioSelectInputs[key].value, true);
     }
 
-    setState(value) {
-        if (!value) {
+    setState(value, isFromDefault = false) {
+        if (!value && !isFromDefault) {
             this.setDefault();
             return;
         }
         this.value = value;
         this.radioSelectInputs[value].checked = true;
         this.updateTargetElements();
     }
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/orderable.css` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/orderable.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/orderable/sortable.min.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/sortable.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1524 +1,1524 @@
-/*! Sortable 1.15.0 - MIT | git://github.com/SortableJS/Sortable.git */ ! function(t, e) {
-    "object" == typeof exports && "undefined" != typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define(e) : (t = t || self).Sortable = e()
-}(this, function() {
-    "use strict";
-
-    function e(e, t) {
-        var n, o = Object.keys(e);
-        return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
-            return Object.getOwnPropertyDescriptor(e, t).enumerable
-        })), o.push.apply(o, n)), o
-    }
-
-    function M(o) {
-        for (var t = 1; t < arguments.length; t++) {
-            var i = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? e(Object(i), !0).forEach(function(t) {
-                var e, n;
-                e = o, t = i[n = t], n in e ? Object.defineProperty(e, n, {
-                    value: t,
-                    enumerable: !0,
-                    configurable: !0,
-                    writable: !0
-                }) : e[n] = t
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(o, Object.getOwnPropertyDescriptors(i)) : e(Object(i)).forEach(function(t) {
-                Object.defineProperty(o, t, Object.getOwnPropertyDescriptor(i, t))
-            })
-        }
-        return o
-    }
-
-    function o(t) {
-        return (o = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
-            return typeof t
-        } : function(t) {
-            return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-        })(t)
-    }
-
-    function a() {
-        return (a = Object.assign || function(t) {
-            for (var e = 1; e < arguments.length; e++) {
-                var n, o = arguments[e];
-                for (n in o) Object.prototype.hasOwnProperty.call(o, n) && (t[n] = o[n])
-            }
-            return t
-        }).apply(this, arguments)
-    }
-
-    function i(t, e) {
-        if (null == t) return {};
-        var n, o = function(t, e) {
-            if (null == t) return {};
-            for (var n, o = {}, i = Object.keys(t), r = 0; r < i.length; r++) n = i[r], 0 <= e.indexOf(n) || (o[n] = t[n]);
-            return o
-        }(t, e);
-        if (Object.getOwnPropertySymbols)
-            for (var i = Object.getOwnPropertySymbols(t), r = 0; r < i.length; r++) n = i[r], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (o[n] = t[n]);
-        return o
-    }
-
-    function r(t) {
-        return function(t) {
-            if (Array.isArray(t)) return l(t)
-        }(t) || function(t) {
-            if ("undefined" != typeof Symbol && null != t[Symbol.iterator] || null != t["@@iterator"]) return Array.from(t)
-        }(t) || function(t, e) {
-            if (t) {
-                if ("string" == typeof t) return l(t, e);
-                var n = Object.prototype.toString.call(t).slice(8, -1);
-                return "Map" === (n = "Object" === n && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? l(t, e) : void 0
-            }
-        }(t) || function() {
-            throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-        }()
-    }
-
-    function l(t, e) {
-        (null == e || e > t.length) && (e = t.length);
-        for (var n = 0, o = new Array(e); n < e; n++) o[n] = t[n];
-        return o
-    }
-
-    function t(t) {
-        if ("undefined" != typeof window && window.navigator) return !!navigator.userAgent.match(t)
-    }
-    var y = t(/(?:Trident.*rv[ :]?11\.|msie|iemobile|Windows Phone)/i),
-        w = t(/Edge/i),
-        s = t(/firefox/i),
-        u = t(/safari/i) && !t(/chrome/i) && !t(/android/i),
-        n = t(/iP(ad|od|hone)/i),
-        c = t(/chrome/i) && t(/android/i),
-        d = {
-            capture: !1,
-            passive: !1
-        };
-
-    function h(t, e, n) {
-        t.addEventListener(e, n, !y && d)
-    }
-
-    function f(t, e, n) {
-        t.removeEventListener(e, n, !y && d)
-    }
-
-    function p(t, e) {
-        if (e && (">" === e[0] && (e = e.substring(1)), t)) try {
-            if (t.matches) return t.matches(e);
-            if (t.msMatchesSelector) return t.msMatchesSelector(e);
-            if (t.webkitMatchesSelector) return t.webkitMatchesSelector(e)
-        } catch (t) {
-            return
-        }
-    }
-
-    function N(t, e, n, o) {
-        if (t) {
-            n = n || document;
-            do {
-                if (null != e && (">" !== e[0] || t.parentNode === n) && p(t, e) || o && t === n) return t
-            } while (t !== n && (t = (i = t).host && i !== document && i.host.nodeType ? i.host : i.parentNode))
-        }
-        var i;
-        return null
-    }
-    var g, m = /\s+/g;
-
-    function I(t, e, n) {
-        var o;
-        t && e && (t.classList ? t.classList[n ? "add" : "remove"](e) : (o = (" " + t.className + " ").replace(m, " ").replace(" " + e + " ", " "), t.className = (o + (n ? " " + e : "")).replace(m, " ")))
-    }
-
-    function P(t, e, n) {
-        var o = t && t.style;
-        if (o) {
-            if (void 0 === n) return document.defaultView && document.defaultView.getComputedStyle ? n = document.defaultView.getComputedStyle(t, "") : t.currentStyle && (n = t.currentStyle), void 0 === e ? n : n[e];
-            o[e = !(e in o || -1 !== e.indexOf("webkit")) ? "-webkit-" + e : e] = n + ("string" == typeof n ? "" : "px")
-        }
-    }
-
-    function v(t, e) {
-        var n = "";
-        if ("string" == typeof t) n = t;
-        else
-            do {
-                var o = P(t, "transform")
-            } while (o && "none" !== o && (n = o + " " + n), !e && (t = t.parentNode));
-        var i = window.DOMMatrix || window.WebKitCSSMatrix || window.CSSMatrix || window.MSCSSMatrix;
-        return i && new i(n)
-    }
-
-    function b(t, e, n) {
-        if (t) {
-            var o = t.getElementsByTagName(e),
-                i = 0,
-                r = o.length;
-            if (n)
-                for (; i < r; i++) n(o[i], i);
-            return o
-        }
-        return []
-    }
-
-    function O() {
-        var t = document.scrollingElement;
-        return t || document.documentElement
-    }
-
-    function k(t, e, n, o, i) {
-        if (t.getBoundingClientRect || t === window) {
-            var r, a, l, s, c, u, d = t !== window && t.parentNode && t !== O() ? (a = (r = t.getBoundingClientRect()).top, l = r.left, s = r.bottom, c = r.right, u = r.height, r.width) : (l = a = 0, s = window.innerHeight, c = window.innerWidth, u = window.innerHeight, window.innerWidth);
-            if ((e || n) && t !== window && (i = i || t.parentNode, !y))
-                do {
-                    if (i && i.getBoundingClientRect && ("none" !== P(i, "transform") || n && "static" !== P(i, "position"))) {
-                        var h = i.getBoundingClientRect();
-                        a -= h.top + parseInt(P(i, "border-top-width")), l -= h.left + parseInt(P(i, "border-left-width")), s = a + r.height, c = l + r.width;
-                        break
-                    }
-                } while (i = i.parentNode);
-            return o && t !== window && (o = (e = v(i || t)) && e.a, t = e && e.d, e && (s = (a /= t) + (u /= t), c = (l /= o) + (d /= o))), {
-                top: a,
-                left: l,
-                bottom: s,
-                right: c,
-                width: d,
-                height: u
-            }
-        }
-    }
-
-    function R(t, e, n) {
-        for (var o = A(t, !0), i = k(t)[e]; o;) {
-            var r = k(o)[n];
-            if (!("top" === n || "left" === n ? r <= i : i <= r)) return o;
-            if (o === O()) break;
-            o = A(o, !1)
-        }
-        return !1
-    }
-
-    function X(t, e, n, o) {
-        for (var i = 0, r = 0, a = t.children; r < a.length;) {
-            if ("none" !== a[r].style.display && a[r] !== Bt.ghost && (o || a[r] !== Bt.dragged) && N(a[r], n.draggable, t, !1)) {
-                if (i === e) return a[r];
-                i++
-            }
-            r++
-        }
-        return null
-    }
-
-    function Y(t, e) {
-        for (var n = t.lastElementChild; n && (n === Bt.ghost || "none" === P(n, "display") || e && !p(n, e));) n = n.previousElementSibling;
-        return n || null
-    }
-
-    function B(t, e) {
-        var n = 0;
-        if (!t || !t.parentNode) return -1;
-        for (; t = t.previousElementSibling;) "TEMPLATE" === t.nodeName.toUpperCase() || t === Bt.clone || e && !p(t, e) || n++;
-        return n
-    }
-
-    function E(t) {
-        var e = 0,
-            n = 0,
-            o = O();
-        if (t)
-            do {
-                var i = v(t),
-                    r = i.a,
-                    i = i.d
-            } while (e += t.scrollLeft * r, n += t.scrollTop * i, t !== o && (t = t.parentNode));
-        return [e, n]
-    }
-
-    function A(t, e) {
-        if (!t || !t.getBoundingClientRect) return O();
-        var n = t,
-            o = !1;
-        do {
-            if (n.clientWidth < n.scrollWidth || n.clientHeight < n.scrollHeight) {
-                var i = P(n);
-                if (n.clientWidth < n.scrollWidth && ("auto" == i.overflowX || "scroll" == i.overflowX) || n.clientHeight < n.scrollHeight && ("auto" == i.overflowY || "scroll" == i.overflowY)) {
-                    if (!n.getBoundingClientRect || n === document.body) return O();
-                    if (o || e) return n;
-                    o = !0
-                }
-            }
-        } while (n = n.parentNode);
-        return O()
-    }
-
-    function D(t, e) {
-        return Math.round(t.top) === Math.round(e.top) && Math.round(t.left) === Math.round(e.left) && Math.round(t.height) === Math.round(e.height) && Math.round(t.width) === Math.round(e.width)
-    }
-
-    function S(e, n) {
-        return function() {
-            var t;
-            g || (1 === (t = arguments).length ? e.call(this, t[0]) : e.apply(this, t), g = setTimeout(function() {
-                g = void 0
-            }, n))
-        }
-    }
-
-    function F(t, e, n) {
-        t.scrollLeft += e, t.scrollTop += n
-    }
-
-    function _(t) {
-        var e = window.Polymer,
-            n = window.jQuery || window.Zepto;
-        return e && e.dom ? e.dom(t).cloneNode(!0) : n ? n(t).clone(!0)[0] : t.cloneNode(!0)
-    }
-
-    function C(t, e) {
-        P(t, "position", "absolute"), P(t, "top", e.top), P(t, "left", e.left), P(t, "width", e.width), P(t, "height", e.height)
-    }
-
-    function T(t) {
-        P(t, "position", ""), P(t, "top", ""), P(t, "left", ""), P(t, "width", ""), P(t, "height", "")
-    }
-    var j = "Sortable" + (new Date).getTime();
-
-    function x() {
-        var e, o = [];
-        return {
-            captureAnimationState: function() {
-                o = [], this.options.animation && [].slice.call(this.el.children).forEach(function(t) {
-                    var e, n;
-                    "none" !== P(t, "display") && t !== Bt.ghost && (o.push({
-                        target: t,
-                        rect: k(t)
-                    }), e = M({}, o[o.length - 1].rect), !t.thisAnimationDuration || (n = v(t, !0)) && (e.top -= n.f, e.left -= n.e), t.fromRect = e)
-                })
-            },
-            addAnimationState: function(t) {
-                o.push(t)
-            },
-            removeAnimationState: function(t) {
-                o.splice(function(t, e) {
-                    for (var n in t)
-                        if (t.hasOwnProperty(n))
-                            for (var o in e)
-                                if (e.hasOwnProperty(o) && e[o] === t[n][o]) return Number(n);
-                    return -1
-                }(o, {
-                    target: t
-                }), 1)
-            },
-            animateAll: function(t) {
-                var c = this;
-                if (!this.options.animation) return clearTimeout(e), void("function" == typeof t && t());
-                var u = !1,
-                    d = 0;
-                o.forEach(function(t) {
-                    var e = 0,
-                        n = t.target,
-                        o = n.fromRect,
-                        i = k(n),
-                        r = n.prevFromRect,
-                        a = n.prevToRect,
-                        l = t.rect,
-                        s = v(n, !0);
-                    s && (i.top -= s.f, i.left -= s.e), n.toRect = i, n.thisAnimationDuration && D(r, i) && !D(o, i) && (l.top - i.top) / (l.left - i.left) == (o.top - i.top) / (o.left - i.left) && (t = l, s = r, r = a, a = c.options, e = Math.sqrt(Math.pow(s.top - t.top, 2) + Math.pow(s.left - t.left, 2)) / Math.sqrt(Math.pow(s.top - r.top, 2) + Math.pow(s.left - r.left, 2)) * a.animation), D(i, o) || (n.prevFromRect = o, n.prevToRect = i, e = e || c.options.animation, c.animate(n, l, i, e)), e && (u = !0, d = Math.max(d, e), clearTimeout(n.animationResetTimer), n.animationResetTimer = setTimeout(function() {
-                        n.animationTime = 0, n.prevFromRect = null, n.fromRect = null, n.prevToRect = null, n.thisAnimationDuration = null
-                    }, e), n.thisAnimationDuration = e)
-                }), clearTimeout(e), u ? e = setTimeout(function() {
-                    "function" == typeof t && t()
-                }, d) : "function" == typeof t && t(), o = []
-            },
-            animate: function(t, e, n, o) {
-                var i, r;
-                o && (P(t, "transition", ""), P(t, "transform", ""), i = (r = v(this.el)) && r.a, r = r && r.d, i = (e.left - n.left) / (i || 1), r = (e.top - n.top) / (r || 1), t.animatingX = !!i, t.animatingY = !!r, P(t, "transform", "translate3d(" + i + "px," + r + "px,0)"), this.forRepaintDummy = t.offsetWidth, P(t, "transition", "transform " + o + "ms" + (this.options.easing ? " " + this.options.easing : "")), P(t, "transform", "translate3d(0,0,0)"), "number" == typeof t.animated && clearTimeout(t.animated), t.animated = setTimeout(function() {
-                    P(t, "transition", ""), P(t, "transform", ""), t.animated = !1, t.animatingX = !1, t.animatingY = !1
-                }, o))
-            }
-        }
-    }
-    var H = [],
-        L = {
-            initializeByDefault: !0
-        },
-        K = {
-            mount: function(e) {
-                for (var t in L) !L.hasOwnProperty(t) || t in e || (e[t] = L[t]);
-                H.forEach(function(t) {
-                    if (t.pluginName === e.pluginName) throw "Sortable: Cannot mount plugin ".concat(e.pluginName, " more than once")
-                }), H.push(e)
-            },
-            pluginEvent: function(e, n, o) {
-                var t = this;
-                this.eventCanceled = !1, o.cancel = function() {
-                    t.eventCanceled = !0
-                };
-                var i = e + "Global";
-                H.forEach(function(t) {
-                    n[t.pluginName] && (n[t.pluginName][i] && n[t.pluginName][i](M({
-                        sortable: n
-                    }, o)), n.options[t.pluginName] && n[t.pluginName][e] && n[t.pluginName][e](M({
-                        sortable: n
-                    }, o)))
-                })
-            },
-            initializePlugins: function(n, o, i, t) {
-                for (var e in H.forEach(function(t) {
-                        var e = t.pluginName;
-                        (n.options[e] || t.initializeByDefault) && ((t = new t(n, o, n.options)).sortable = n, t.options = n.options, n[e] = t, a(i, t.defaults))
-                    }), n.options) {
-                    var r;
-                    n.options.hasOwnProperty(e) && (void 0 !== (r = this.modifyOption(n, e, n.options[e])) && (n.options[e] = r))
-                }
-            },
-            getEventProperties: function(e, n) {
-                var o = {};
-                return H.forEach(function(t) {
-                    "function" == typeof t.eventProperties && a(o, t.eventProperties.call(n[t.pluginName], e))
-                }), o
-            },
-            modifyOption: function(e, n, o) {
-                var i;
-                return H.forEach(function(t) {
-                    e[t.pluginName] && t.optionListeners && "function" == typeof t.optionListeners[n] && (i = t.optionListeners[n].call(e[t.pluginName], o))
-                }), i
-            }
-        };
-
-    function W(t) {
-        var e = t.sortable,
-            n = t.rootEl,
-            o = t.name,
-            i = t.targetEl,
-            r = t.cloneEl,
-            a = t.toEl,
-            l = t.fromEl,
-            s = t.oldIndex,
-            c = t.newIndex,
-            u = t.oldDraggableIndex,
-            d = t.newDraggableIndex,
-            h = t.originalEvent,
-            f = t.putSortable,
-            p = t.extraEventProperties;
-        if (e = e || n && n[j]) {
-            var g, m = e.options,
-                t = "on" + o.charAt(0).toUpperCase() + o.substr(1);
-            !window.CustomEvent || y || w ? (g = document.createEvent("Event")).initEvent(o, !0, !0) : g = new CustomEvent(o, {
-                bubbles: !0,
-                cancelable: !0
-            }), g.to = a || n, g.from = l || n, g.item = i || n, g.clone = r, g.oldIndex = s, g.newIndex = c, g.oldDraggableIndex = u, g.newDraggableIndex = d, g.originalEvent = h, g.pullMode = f ? f.lastPutMode : void 0;
-            var v, b = M(M({}, p), K.getEventProperties(o, e));
-            for (v in b) g[v] = b[v];
-            n && n.dispatchEvent(g), m[t] && m[t].call(e, g)
-        }
-    }
-
-    function z(t, e) {
-        var n = (o = 2 < arguments.length && void 0 !== arguments[2] ? arguments[2] : {}).evt,
-            o = i(o, G);
-        K.pluginEvent.bind(Bt)(t, e, M({
-            dragEl: q,
-            parentEl: V,
-            ghostEl: Z,
-            rootEl: $,
-            nextEl: Q,
-            lastDownEl: J,
-            cloneEl: tt,
-            cloneHidden: et,
-            dragStarted: pt,
-            putSortable: lt,
-            activeSortable: Bt.active,
-            originalEvent: n,
-            oldIndex: nt,
-            oldDraggableIndex: it,
-            newIndex: ot,
-            newDraggableIndex: rt,
-            hideGhostForTarget: kt,
-            unhideGhostForTarget: Rt,
-            cloneNowHidden: function() {
-                et = !0
-            },
-            cloneNowShown: function() {
-                et = !1
-            },
-            dispatchSortableEvent: function(t) {
-                U({
-                    sortable: e,
-                    name: t,
-                    originalEvent: n
-                })
-            }
-        }, o))
-    }
-    var G = ["evt"];
-
-    function U(t) {
-        W(M({
-            putSortable: lt,
-            cloneEl: tt,
-            targetEl: q,
-            rootEl: $,
-            oldIndex: nt,
-            oldDraggableIndex: it,
-            newIndex: ot,
-            newDraggableIndex: rt
-        }, t))
-    }
-    var q, V, Z, $, Q, J, tt, et, nt, ot, it, rt, at, lt, st, ct, ut, dt, ht, ft, pt, gt, mt, vt, bt, yt = !1,
-        wt = !1,
-        Et = [],
-        Dt = !1,
-        St = !1,
-        _t = [],
-        Ct = !1,
-        Tt = [],
-        xt = "undefined" != typeof document,
-        Ot = n,
-        At = w || y ? "cssFloat" : "float",
-        Mt = xt && !c && !n && "draggable" in document.createElement("div"),
-        Nt = function() {
-            if (xt) {
-                if (y) return !1;
-                var t = document.createElement("x");
-                return t.style.cssText = "pointer-events:auto", "auto" === t.style.pointerEvents
-            }
-        }(),
-        It = function(t, e) {
-            var n = P(t),
-                o = parseInt(n.width) - parseInt(n.paddingLeft) - parseInt(n.paddingRight) - parseInt(n.borderLeftWidth) - parseInt(n.borderRightWidth),
-                i = X(t, 0, e),
-                r = X(t, 1, e),
-                a = i && P(i),
-                l = r && P(r),
-                s = a && parseInt(a.marginLeft) + parseInt(a.marginRight) + k(i).width,
-                t = l && parseInt(l.marginLeft) + parseInt(l.marginRight) + k(r).width;
-            if ("flex" === n.display) return "column" === n.flexDirection || "column-reverse" === n.flexDirection ? "vertical" : "horizontal";
-            if ("grid" === n.display) return n.gridTemplateColumns.split(" ").length <= 1 ? "vertical" : "horizontal";
-            if (i && a.float && "none" !== a.float) {
-                e = "left" === a.float ? "left" : "right";
-                return !r || "both" !== l.clear && l.clear !== e ? "horizontal" : "vertical"
-            }
-            return i && ("block" === a.display || "flex" === a.display || "table" === a.display || "grid" === a.display || o <= s && "none" === n[At] || r && "none" === n[At] && o < s + t) ? "vertical" : "horizontal"
-        },
-        Pt = function(t) {
-            function l(r, a) {
-                return function(t, e, n, o) {
-                    var i = t.options.group.name && e.options.group.name && t.options.group.name === e.options.group.name;
-                    if (null == r && (a || i)) return !0;
-                    if (null == r || !1 === r) return !1;
-                    if (a && "clone" === r) return r;
-                    if ("function" == typeof r) return l(r(t, e, n, o), a)(t, e, n, o);
-                    e = (a ? t : e).options.group.name;
-                    return !0 === r || "string" == typeof r && r === e || r.join && -1 < r.indexOf(e)
-                }
-            }
-            var e = {},
-                n = t.group;
-            n && "object" == o(n) || (n = {
-                name: n
-            }), e.name = n.name, e.checkPull = l(n.pull, !0), e.checkPut = l(n.put), e.revertClone = n.revertClone, t.group = e
-        },
-        kt = function() {
-            !Nt && Z && P(Z, "display", "none")
-        },
-        Rt = function() {
-            !Nt && Z && P(Z, "display", "")
-        };
-    xt && !c && document.addEventListener("click", function(t) {
-        if (wt) return t.preventDefault(), t.stopPropagation && t.stopPropagation(), t.stopImmediatePropagation && t.stopImmediatePropagation(), wt = !1
-    }, !0);
-
-    function Xt(t) {
-        if (q) {
-            t = t.touches ? t.touches[0] : t;
-            var e = (i = t.clientX, r = t.clientY, Et.some(function(t) {
-                var e = t[j].options.emptyInsertThreshold;
-                if (e && !Y(t)) {
-                    var n = k(t),
-                        o = i >= n.left - e && i <= n.right + e,
-                        e = r >= n.top - e && r <= n.bottom + e;
-                    return o && e ? a = t : void 0
-                }
-            }), a);
-            if (e) {
-                var n, o = {};
-                for (n in t) t.hasOwnProperty(n) && (o[n] = t[n]);
-                o.target = o.rootEl = e, o.preventDefault = void 0, o.stopPropagation = void 0, e[j]._onDragOver(o)
-            }
-        }
-        var i, r, a
-    }
-
-    function Yt(t) {
-        q && q.parentNode[j]._isOutsideThisEl(t.target)
-    }
-
-    function Bt(t, e) {
-        if (!t || !t.nodeType || 1 !== t.nodeType) throw "Sortable: `el` must be an HTMLElement, not ".concat({}.toString.call(t));
-        this.el = t, this.options = e = a({}, e), t[j] = this;
-        var n, o, i = {
-            group: null,
-            sort: !0,
-            disabled: !1,
-            store: null,
-            handle: null,
-            draggable: /^[uo]l$/i.test(t.nodeName) ? ">li" : ">*",
-            swapThreshold: 1,
-            invertSwap: !1,
-            invertedSwapThreshold: null,
-            removeCloneOnHide: !0,
-            direction: function() {
-                return It(t, this.options)
-            },
-            ghostClass: "sortable-ghost",
-            chosenClass: "sortable-chosen",
-            dragClass: "sortable-drag",
-            ignore: "a, img",
-            filter: null,
-            preventOnFilter: !0,
-            animation: 0,
-            easing: null,
-            setData: function(t, e) {
-                t.setData("Text", e.textContent)
-            },
-            dropBubble: !1,
-            dragoverBubble: !1,
-            dataIdAttr: "data-id",
-            delay: 0,
-            delayOnTouchOnly: !1,
-            touchStartThreshold: (Number.parseInt ? Number : window).parseInt(window.devicePixelRatio, 10) || 1,
-            forceFallback: !1,
-            fallbackClass: "sortable-fallback",
-            fallbackOnBody: !1,
-            fallbackTolerance: 0,
-            fallbackOffset: {
-                x: 0,
-                y: 0
-            },
-            supportPointer: !1 !== Bt.supportPointer && "PointerEvent" in window && !u,
-            emptyInsertThreshold: 5
-        };
-        for (n in K.initializePlugins(this, t, i), i) n in e || (e[n] = i[n]);
-        for (o in Pt(e), this) "_" === o.charAt(0) && "function" == typeof this[o] && (this[o] = this[o].bind(this));
-        this.nativeDraggable = !e.forceFallback && Mt, this.nativeDraggable && (this.options.touchStartThreshold = 1), e.supportPointer ? h(t, "pointerdown", this._onTapStart) : (h(t, "mousedown", this._onTapStart), h(t, "touchstart", this._onTapStart)), this.nativeDraggable && (h(t, "dragover", this), h(t, "dragenter", this)), Et.push(this.el), e.store && e.store.get && this.sort(e.store.get(this) || []), a(this, x())
-    }
-
-    function Ft(t, e, n, o, i, r, a, l) {
-        var s, c, u = t[j],
-            d = u.options.onMove;
-        return !window.CustomEvent || y || w ? (s = document.createEvent("Event")).initEvent("move", !0, !0) : s = new CustomEvent("move", {
-            bubbles: !0,
-            cancelable: !0
-        }), s.to = e, s.from = t, s.dragged = n, s.draggedRect = o, s.related = i || e, s.relatedRect = r || k(e), s.willInsertAfter = l, s.originalEvent = a, t.dispatchEvent(s), c = d ? d.call(u, s, a) : c
-    }
-
-    function jt(t) {
-        t.draggable = !1
-    }
-
-    function Ht() {
-        Ct = !1
-    }
-
-    function Lt(t) {
-        return setTimeout(t, 0)
-    }
-
-    function Kt(t) {
-        return clearTimeout(t)
-    }
-    Bt.prototype = {
-        constructor: Bt,
-        _isOutsideThisEl: function(t) {
-            this.el.contains(t) || t === this.el || (gt = null)
-        },
-        _getDirection: function(t, e) {
-            return "function" == typeof this.options.direction ? this.options.direction.call(this, t, e, q) : this.options.direction
-        },
-        _onTapStart: function(e) {
-            if (e.cancelable) {
-                var n = this,
-                    o = this.el,
-                    t = this.options,
-                    i = t.preventOnFilter,
-                    r = e.type,
-                    a = e.touches && e.touches[0] || e.pointerType && "touch" === e.pointerType && e,
-                    l = (a || e).target,
-                    s = e.target.shadowRoot && (e.path && e.path[0] || e.composedPath && e.composedPath()[0]) || l,
-                    c = t.filter;
-                if (! function(t) {
-                        Tt.length = 0;
-                        var e = t.getElementsByTagName("input"),
-                            n = e.length;
-                        for (; n--;) {
-                            var o = e[n];
-                            o.checked && Tt.push(o)
-                        }
-                    }(o), !q && !(/mousedown|pointerdown/.test(r) && 0 !== e.button || t.disabled) && !s.isContentEditable && (this.nativeDraggable || !u || !l || "SELECT" !== l.tagName.toUpperCase()) && !((l = N(l, t.draggable, o, !1)) && l.animated || J === l)) {
-                    if (nt = B(l), it = B(l, t.draggable), "function" == typeof c) {
-                        if (c.call(this, e, l, this)) return U({
-                            sortable: n,
-                            rootEl: s,
-                            name: "filter",
-                            targetEl: l,
-                            toEl: o,
-                            fromEl: o
-                        }), z("filter", n, {
-                            evt: e
-                        }), void(i && e.cancelable && e.preventDefault())
-                    } else if (c = c && c.split(",").some(function(t) {
-                            if (t = N(s, t.trim(), o, !1)) return U({
-                                sortable: n,
-                                rootEl: t,
-                                name: "filter",
-                                targetEl: l,
-                                fromEl: o,
-                                toEl: o
-                            }), z("filter", n, {
-                                evt: e
-                            }), !0
-                        })) return void(i && e.cancelable && e.preventDefault());
-                    t.handle && !N(s, t.handle, o, !1) || this._prepareDragStart(e, a, l)
-                }
-            }
-        },
-        _prepareDragStart: function(t, e, n) {
-            var o, i = this,
-                r = i.el,
-                a = i.options,
-                l = r.ownerDocument;
-            n && !q && n.parentNode === r && (o = k(n), $ = r, V = (q = n).parentNode, Q = q.nextSibling, J = n, at = a.group, st = {
-                target: Bt.dragged = q,
-                clientX: (e || t).clientX,
-                clientY: (e || t).clientY
-            }, ht = st.clientX - o.left, ft = st.clientY - o.top, this._lastX = (e || t).clientX, this._lastY = (e || t).clientY, q.style["will-change"] = "all", o = function() {
-                z("delayEnded", i, {
-                    evt: t
-                }), Bt.eventCanceled ? i._onDrop() : (i._disableDelayedDragEvents(), !s && i.nativeDraggable && (q.draggable = !0), i._triggerDragStart(t, e), U({
-                    sortable: i,
-                    name: "choose",
-                    originalEvent: t
-                }), I(q, a.chosenClass, !0))
-            }, a.ignore.split(",").forEach(function(t) {
-                b(q, t.trim(), jt)
-            }), h(l, "dragover", Xt), h(l, "mousemove", Xt), h(l, "touchmove", Xt), h(l, "mouseup", i._onDrop), h(l, "touchend", i._onDrop), h(l, "touchcancel", i._onDrop), s && this.nativeDraggable && (this.options.touchStartThreshold = 4, q.draggable = !0), z("delayStart", this, {
-                evt: t
-            }), !a.delay || a.delayOnTouchOnly && !e || this.nativeDraggable && (w || y) ? o() : Bt.eventCanceled ? this._onDrop() : (h(l, "mouseup", i._disableDelayedDrag), h(l, "touchend", i._disableDelayedDrag), h(l, "touchcancel", i._disableDelayedDrag), h(l, "mousemove", i._delayedDragTouchMoveHandler), h(l, "touchmove", i._delayedDragTouchMoveHandler), a.supportPointer && h(l, "pointermove", i._delayedDragTouchMoveHandler), i._dragStartTimer = setTimeout(o, a.delay)))
-        },
-        _delayedDragTouchMoveHandler: function(t) {
-            t = t.touches ? t.touches[0] : t;
-            Math.max(Math.abs(t.clientX - this._lastX), Math.abs(t.clientY - this._lastY)) >= Math.floor(this.options.touchStartThreshold / (this.nativeDraggable && window.devicePixelRatio || 1)) && this._disableDelayedDrag()
-        },
-        _disableDelayedDrag: function() {
-            q && jt(q), clearTimeout(this._dragStartTimer), this._disableDelayedDragEvents()
-        },
-        _disableDelayedDragEvents: function() {
-            var t = this.el.ownerDocument;
-            f(t, "mouseup", this._disableDelayedDrag), f(t, "touchend", this._disableDelayedDrag), f(t, "touchcancel", this._disableDelayedDrag), f(t, "mousemove", this._delayedDragTouchMoveHandler), f(t, "touchmove", this._delayedDragTouchMoveHandler), f(t, "pointermove", this._delayedDragTouchMoveHandler)
-        },
-        _triggerDragStart: function(t, e) {
-            e = e || "touch" == t.pointerType && t, !this.nativeDraggable || e ? this.options.supportPointer ? h(document, "pointermove", this._onTouchMove) : h(document, e ? "touchmove" : "mousemove", this._onTouchMove) : (h(q, "dragend", this), h($, "dragstart", this._onDragStart));
-            try {
-                document.selection ? Lt(function() {
-                    document.selection.empty()
-                }) : window.getSelection().removeAllRanges()
-            } catch (t) {}
-        },
-        _dragStarted: function(t, e) {
-            var n;
-            yt = !1, $ && q ? (z("dragStarted", this, {
-                evt: e
-            }), this.nativeDraggable && h(document, "dragover", Yt), n = this.options, t || I(q, n.dragClass, !1), I(q, n.ghostClass, !0), Bt.active = this, t && this._appendGhost(), U({
-                sortable: this,
-                name: "start",
-                originalEvent: e
-            })) : this._nulling()
-        },
-        _emulateDragOver: function() {
-            if (ct) {
-                this._lastX = ct.clientX, this._lastY = ct.clientY, kt();
-                for (var t = document.elementFromPoint(ct.clientX, ct.clientY), e = t; t && t.shadowRoot && (t = t.shadowRoot.elementFromPoint(ct.clientX, ct.clientY)) !== e;) e = t;
-                if (q.parentNode[j]._isOutsideThisEl(t), e)
-                    do {
-                        if (e[j])
-                            if (e[j]._onDragOver({
-                                    clientX: ct.clientX,
-                                    clientY: ct.clientY,
-                                    target: t,
-                                    rootEl: e
-                                }) && !this.options.dragoverBubble) break
-                    } while (e = (t = e).parentNode);
-                Rt()
-            }
-        },
-        _onTouchMove: function(t) {
-            if (st) {
-                var e = this.options,
-                    n = e.fallbackTolerance,
-                    o = e.fallbackOffset,
-                    i = t.touches ? t.touches[0] : t,
-                    r = Z && v(Z, !0),
-                    a = Z && r && r.a,
-                    l = Z && r && r.d,
-                    e = Ot && bt && E(bt),
-                    a = (i.clientX - st.clientX + o.x) / (a || 1) + (e ? e[0] - _t[0] : 0) / (a || 1),
-                    l = (i.clientY - st.clientY + o.y) / (l || 1) + (e ? e[1] - _t[1] : 0) / (l || 1);
-                if (!Bt.active && !yt) {
-                    if (n && Math.max(Math.abs(i.clientX - this._lastX), Math.abs(i.clientY - this._lastY)) < n) return;
-                    this._onDragStart(t, !0)
-                }
-                Z && (r ? (r.e += a - (ut || 0), r.f += l - (dt || 0)) : r = {
-                    a: 1,
-                    b: 0,
-                    c: 0,
-                    d: 1,
-                    e: a,
-                    f: l
-                }, r = "matrix(".concat(r.a, ",").concat(r.b, ",").concat(r.c, ",").concat(r.d, ",").concat(r.e, ",").concat(r.f, ")"), P(Z, "webkitTransform", r), P(Z, "mozTransform", r), P(Z, "msTransform", r), P(Z, "transform", r), ut = a, dt = l, ct = i), t.cancelable && t.preventDefault()
-            }
-        },
-        _appendGhost: function() {
-            if (!Z) {
-                var t = this.options.fallbackOnBody ? document.body : $,
-                    e = k(q, !0, Ot, !0, t),
-                    n = this.options;
-                if (Ot) {
-                    for (bt = t;
-                        "static" === P(bt, "position") && "none" === P(bt, "transform") && bt !== document;) bt = bt.parentNode;
-                    bt !== document.body && bt !== document.documentElement ? (bt === document && (bt = O()), e.top += bt.scrollTop, e.left += bt.scrollLeft) : bt = O(), _t = E(bt)
-                }
-                I(Z = q.cloneNode(!0), n.ghostClass, !1), I(Z, n.fallbackClass, !0), I(Z, n.dragClass, !0), P(Z, "transition", ""), P(Z, "transform", ""), P(Z, "box-sizing", "border-box"), P(Z, "margin", 0), P(Z, "top", e.top), P(Z, "left", e.left), P(Z, "width", e.width), P(Z, "height", e.height), P(Z, "opacity", "0.8"), P(Z, "position", Ot ? "absolute" : "fixed"), P(Z, "zIndex", "100000"), P(Z, "pointerEvents", "none"), Bt.ghost = Z, t.appendChild(Z), P(Z, "transform-origin", ht / parseInt(Z.style.width) * 100 + "% " + ft / parseInt(Z.style.height) * 100 + "%")
-            }
-        },
-        _onDragStart: function(t, e) {
-            var n = this,
-                o = t.dataTransfer,
-                i = n.options;
-            z("dragStart", this, {
-                evt: t
-            }), Bt.eventCanceled ? this._onDrop() : (z("setupClone", this), Bt.eventCanceled || ((tt = _(q)).removeAttribute("id"), tt.draggable = !1, tt.style["will-change"] = "", this._hideClone(), I(tt, this.options.chosenClass, !1), Bt.clone = tt), n.cloneId = Lt(function() {
-                z("clone", n), Bt.eventCanceled || (n.options.removeCloneOnHide || $.insertBefore(tt, q), n._hideClone(), U({
-                    sortable: n,
-                    name: "clone"
-                }))
-            }), e || I(q, i.dragClass, !0), e ? (wt = !0, n._loopId = setInterval(n._emulateDragOver, 50)) : (f(document, "mouseup", n._onDrop), f(document, "touchend", n._onDrop), f(document, "touchcancel", n._onDrop), o && (o.effectAllowed = "move", i.setData && i.setData.call(n, o, q)), h(document, "drop", n), P(q, "transform", "translateZ(0)")), yt = !0, n._dragStartId = Lt(n._dragStarted.bind(n, e, t)), h(document, "selectstart", n), pt = !0, u && P(document.body, "user-select", "none"))
-        },
-        _onDragOver: function(n) {
-            var o, i, r, t, a = this.el,
-                l = n.target,
-                e = this.options,
-                s = e.group,
-                c = Bt.active,
-                u = at === s,
-                d = e.sort,
-                h = lt || c,
-                f = this,
-                p = !1;
-            if (!Ct) {
-                if (void 0 !== n.preventDefault && n.cancelable && n.preventDefault(), l = N(l, e.draggable, a, !0), T("dragOver"), Bt.eventCanceled) return p;
-                if (q.contains(n.target) || l.animated && l.animatingX && l.animatingY || f._ignoreWhileAnimating === l) return O(!1);
-                if (wt = !1, c && !e.disabled && (u ? d || (i = V !== $) : lt === this || (this.lastPutMode = at.checkPull(this, c, q, n)) && s.checkPut(this, c, q, n))) {
-                    if (r = "vertical" === this._getDirection(n, l), o = k(q), T("dragOverValid"), Bt.eventCanceled) return p;
-                    if (i) return V = $, x(), this._hideClone(), T("revert"), Bt.eventCanceled || (Q ? $.insertBefore(q, Q) : $.appendChild(q)), O(!0);
-                    var g = Y(a, e.draggable);
-                    if (!g || function(t, e, n) {
-                            n = k(Y(n.el, n.options.draggable));
-                            return e ? t.clientX > n.right + 10 || t.clientX <= n.right && t.clientY > n.bottom && t.clientX >= n.left : t.clientX > n.right && t.clientY > n.top || t.clientX <= n.right && t.clientY > n.bottom + 10
-                        }(n, r, this) && !g.animated) {
-                        if (g === q) return O(!1);
-                        if ((l = g && a === n.target ? g : l) && (w = k(l)), !1 !== Ft($, a, q, o, l, w, n, !!l)) return x(), g && g.nextSibling ? a.insertBefore(q, g.nextSibling) : a.appendChild(q), V = a, A(), O(!0)
-                    } else if (g && function(t, e, n) {
-                            n = k(X(n.el, 0, n.options, !0));
-                            return e ? t.clientX < n.left - 10 || t.clientY < n.top && t.clientX < n.right : t.clientY < n.top - 10 || t.clientY < n.bottom && t.clientX < n.left
-                        }(n, r, this)) {
-                        var m = X(a, 0, e, !0);
-                        if (m === q) return O(!1);
-                        if (w = k(l = m), !1 !== Ft($, a, q, o, l, w, n, !1)) return x(), a.insertBefore(q, m), V = a, A(), O(!0)
-                    } else if (l.parentNode === a) {
-                        var v, b, y, w = k(l),
-                            E = q.parentNode !== a,
-                            D = (D = q.animated && q.toRect || o, C = l.animated && l.toRect || w, S = (t = r) ? D.left : D.top, s = t ? D.right : D.bottom, g = t ? D.width : D.height, m = t ? C.left : C.top, D = t ? C.right : C.bottom, C = t ? C.width : C.height, !(S === m || s === D || S + g / 2 === m + C / 2)),
-                            S = r ? "top" : "left",
-                            g = R(l, "top", "top") || R(q, "top", "top"),
-                            m = g ? g.scrollTop : void 0;
-                        if (gt !== l && (b = w[S], Dt = !1, St = !D && e.invertSwap || E), 0 !== (v = function(t, e, n, o, i, r, a, l) {
-                                var s = o ? t.clientY : t.clientX,
-                                    c = o ? n.height : n.width,
-                                    t = o ? n.top : n.left,
-                                    o = o ? n.bottom : n.right,
-                                    n = !1;
-                                if (!a)
-                                    if (l && vt < c * i) {
-                                        if (Dt = !Dt && (1 === mt ? t + c * r / 2 < s : s < o - c * r / 2) ? !0 : Dt) n = !0;
-                                        else if (1 === mt ? s < t + vt : o - vt < s) return -mt
-                                    } else if (t + c * (1 - i) / 2 < s && s < o - c * (1 - i) / 2) return function(t) {
-                                    return B(q) < B(t) ? 1 : -1
-                                }(e);
-                                if ((n = n || a) && (s < t + c * r / 2 || o - c * r / 2 < s)) return t + c / 2 < s ? 1 : -1;
-                                return 0
-                            }(n, l, w, r, D ? 1 : e.swapThreshold, null == e.invertedSwapThreshold ? e.swapThreshold : e.invertedSwapThreshold, St, gt === l)))
-                            for (var _ = B(q);
-                                (y = V.children[_ -= v]) && ("none" === P(y, "display") || y === Z););
-                        if (0 === v || y === l) return O(!1);
-                        mt = v;
-                        var C = (gt = l).nextElementSibling,
-                            E = !1,
-                            D = Ft($, a, q, o, l, w, n, E = 1 === v);
-                        if (!1 !== D) return 1 !== D && -1 !== D || (E = 1 === D), Ct = !0, setTimeout(Ht, 30), x(), E && !C ? a.appendChild(q) : l.parentNode.insertBefore(q, E ? C : l), g && F(g, 0, m - g.scrollTop), V = q.parentNode, void 0 === b || St || (vt = Math.abs(b - k(l)[S])), A(), O(!0)
-                    }
-                    if (a.contains(q)) return O(!1)
-                }
-                return !1
-            }
-
-            function T(t, e) {
-                z(t, f, M({
-                    evt: n,
-                    isOwner: u,
-                    axis: r ? "vertical" : "horizontal",
-                    revert: i,
-                    dragRect: o,
-                    targetRect: w,
-                    canSort: d,
-                    fromSortable: h,
-                    target: l,
-                    completed: O,
-                    onMove: function(t, e) {
-                        return Ft($, a, q, o, t, k(t), n, e)
-                    },
-                    changed: A
-                }, e))
-            }
-
-            function x() {
-                T("dragOverAnimationCapture"), f.captureAnimationState(), f !== h && h.captureAnimationState()
-            }
-
-            function O(t) {
-                return T("dragOverCompleted", {
-                    insertion: t
-                }), t && (u ? c._hideClone() : c._showClone(f), f !== h && (I(q, (lt || c).options.ghostClass, !1), I(q, e.ghostClass, !0)), lt !== f && f !== Bt.active ? lt = f : f === Bt.active && lt && (lt = null), h === f && (f._ignoreWhileAnimating = l), f.animateAll(function() {
-                    T("dragOverAnimationComplete"), f._ignoreWhileAnimating = null
-                }), f !== h && (h.animateAll(), h._ignoreWhileAnimating = null)), (l === q && !q.animated || l === a && !l.animated) && (gt = null), e.dragoverBubble || n.rootEl || l === document || (q.parentNode[j]._isOutsideThisEl(n.target), t || Xt(n)), !e.dragoverBubble && n.stopPropagation && n.stopPropagation(), p = !0
-            }
-
-            function A() {
-                ot = B(q), rt = B(q, e.draggable), U({
-                    sortable: f,
-                    name: "change",
-                    toEl: a,
-                    newIndex: ot,
-                    newDraggableIndex: rt,
-                    originalEvent: n
-                })
-            }
-        },
-        _ignoreWhileAnimating: null,
-        _offMoveEvents: function() {
-            f(document, "mousemove", this._onTouchMove), f(document, "touchmove", this._onTouchMove), f(document, "pointermove", this._onTouchMove), f(document, "dragover", Xt), f(document, "mousemove", Xt), f(document, "touchmove", Xt)
-        },
-        _offUpEvents: function() {
-            var t = this.el.ownerDocument;
-            f(t, "mouseup", this._onDrop), f(t, "touchend", this._onDrop), f(t, "pointerup", this._onDrop), f(t, "touchcancel", this._onDrop), f(document, "selectstart", this)
-        },
-        _onDrop: function(t) {
-            var e = this.el,
-                n = this.options;
-            ot = B(q), rt = B(q, n.draggable), z("drop", this, {
-                evt: t
-            }), V = q && q.parentNode, ot = B(q), rt = B(q, n.draggable), Bt.eventCanceled || (Dt = St = yt = !1, clearInterval(this._loopId), clearTimeout(this._dragStartTimer), Kt(this.cloneId), Kt(this._dragStartId), this.nativeDraggable && (f(document, "drop", this), f(e, "dragstart", this._onDragStart)), this._offMoveEvents(), this._offUpEvents(), u && P(document.body, "user-select", ""), P(q, "transform", ""), t && (pt && (t.cancelable && t.preventDefault(), n.dropBubble || t.stopPropagation()), Z && Z.parentNode && Z.parentNode.removeChild(Z), ($ === V || lt && "clone" !== lt.lastPutMode) && tt && tt.parentNode && tt.parentNode.removeChild(tt), q && (this.nativeDraggable && f(q, "dragend", this), jt(q), q.style["will-change"] = "", pt && !yt && I(q, (lt || this).options.ghostClass, !1), I(q, this.options.chosenClass, !1), U({
-                sortable: this,
-                name: "unchoose",
-                toEl: V,
-                newIndex: null,
-                newDraggableIndex: null,
-                originalEvent: t
-            }), $ !== V ? (0 <= ot && (U({
-                rootEl: V,
-                name: "add",
-                toEl: V,
-                fromEl: $,
-                originalEvent: t
-            }), U({
-                sortable: this,
-                name: "remove",
-                toEl: V,
-                originalEvent: t
-            }), U({
-                rootEl: V,
-                name: "sort",
-                toEl: V,
-                fromEl: $,
-                originalEvent: t
-            }), U({
-                sortable: this,
-                name: "sort",
-                toEl: V,
-                originalEvent: t
-            })), lt && lt.save()) : ot !== nt && 0 <= ot && (U({
-                sortable: this,
-                name: "update",
-                toEl: V,
-                originalEvent: t
-            }), U({
-                sortable: this,
-                name: "sort",
-                toEl: V,
-                originalEvent: t
-            })), Bt.active && (null != ot && -1 !== ot || (ot = nt, rt = it), U({
-                sortable: this,
-                name: "end",
-                toEl: V,
-                originalEvent: t
-            }), this.save())))), this._nulling()
-        },
-        _nulling: function() {
-            z("nulling", this), $ = q = V = Z = Q = tt = J = et = st = ct = pt = ot = rt = nt = it = gt = mt = lt = at = Bt.dragged = Bt.ghost = Bt.clone = Bt.active = null, Tt.forEach(function(t) {
-                t.checked = !0
-            }), Tt.length = ut = dt = 0
-        },
-        handleEvent: function(t) {
-            switch (t.type) {
-                case "drop":
-                case "dragend":
-                    this._onDrop(t);
-                    break;
-                case "dragenter":
-                case "dragover":
-                    q && (this._onDragOver(t), function(t) {
-                        t.dataTransfer && (t.dataTransfer.dropEffect = "move");
-                        t.cancelable && t.preventDefault()
-                    }(t));
-                    break;
-                case "selectstart":
-                    t.preventDefault()
-            }
-        },
-        toArray: function() {
-            for (var t, e = [], n = this.el.children, o = 0, i = n.length, r = this.options; o < i; o++) N(t = n[o], r.draggable, this.el, !1) && e.push(t.getAttribute(r.dataIdAttr) || function(t) {
-                var e = t.tagName + t.className + t.src + t.href + t.textContent,
-                    n = e.length,
-                    o = 0;
-                for (; n--;) o += e.charCodeAt(n);
-                return o.toString(36)
-            }(t));
-            return e
-        },
-        sort: function(t, e) {
-            var n = {},
-                o = this.el;
-            this.toArray().forEach(function(t, e) {
-                e = o.children[e];
-                N(e, this.options.draggable, o, !1) && (n[t] = e)
-            }, this), e && this.captureAnimationState(), t.forEach(function(t) {
-                n[t] && (o.removeChild(n[t]), o.appendChild(n[t]))
-            }), e && this.animateAll()
-        },
-        save: function() {
-            var t = this.options.store;
-            t && t.set && t.set(this)
-        },
-        closest: function(t, e) {
-            return N(t, e || this.options.draggable, this.el, !1)
-        },
-        option: function(t, e) {
-            var n = this.options;
-            if (void 0 === e) return n[t];
-            var o = K.modifyOption(this, t, e);
-            n[t] = void 0 !== o ? o : e, "group" === t && Pt(n)
-        },
-        destroy: function() {
-            z("destroy", this);
-            var t = this.el;
-            t[j] = null, f(t, "mousedown", this._onTapStart), f(t, "touchstart", this._onTapStart), f(t, "pointerdown", this._onTapStart), this.nativeDraggable && (f(t, "dragover", this), f(t, "dragenter", this)), Array.prototype.forEach.call(t.querySelectorAll("[draggable]"), function(t) {
-                t.removeAttribute("draggable")
-            }), this._onDrop(), this._disableDelayedDragEvents(), Et.splice(Et.indexOf(this.el), 1), this.el = t = null
-        },
-        _hideClone: function() {
-            et || (z("hideClone", this), Bt.eventCanceled || (P(tt, "display", "none"), this.options.removeCloneOnHide && tt.parentNode && tt.parentNode.removeChild(tt), et = !0))
-        },
-        _showClone: function(t) {
-            "clone" === t.lastPutMode ? et && (z("showClone", this), Bt.eventCanceled || (q.parentNode != $ || this.options.group.revertClone ? Q ? $.insertBefore(tt, Q) : $.appendChild(tt) : $.insertBefore(tt, q), this.options.group.revertClone && this.animate(q, tt), P(tt, "display", ""), et = !1)) : this._hideClone()
-        }
-    }, xt && h(document, "touchmove", function(t) {
-        (Bt.active || yt) && t.cancelable && t.preventDefault()
-    }), Bt.utils = {
-        on: h,
-        off: f,
-        css: P,
-        find: b,
-        is: function(t, e) {
-            return !!N(t, e, t, !1)
-        },
-        extend: function(t, e) {
-            if (t && e)
-                for (var n in e) e.hasOwnProperty(n) && (t[n] = e[n]);
-            return t
-        },
-        throttle: S,
-        closest: N,
-        toggleClass: I,
-        clone: _,
-        index: B,
-        nextTick: Lt,
-        cancelNextTick: Kt,
-        detectDirection: It,
-        getChild: X
-    }, Bt.get = function(t) {
-        return t[j]
-    }, Bt.mount = function() {
-        for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-        (e = e[0].constructor === Array ? e[0] : e).forEach(function(t) {
-            if (!t.prototype || !t.prototype.constructor) throw "Sortable: Mounted plugin must be a constructor function, not ".concat({}.toString.call(t));
-            t.utils && (Bt.utils = M(M({}, Bt.utils), t.utils)), K.mount(t)
-        })
-    }, Bt.create = function(t, e) {
-        return new Bt(t, e)
-    };
-    var Wt, zt, Gt, Ut, qt, Vt, Zt = [],
-        $t = !(Bt.version = "1.15.0");
-
-    function Qt() {
-        Zt.forEach(function(t) {
-            clearInterval(t.pid)
-        }), Zt = []
-    }
-
-    function Jt() {
-        clearInterval(Vt)
-    }
-    var te, ee = S(function(n, t, e, o) {
-            if (t.scroll) {
-                var i, r = (n.touches ? n.touches[0] : n).clientX,
-                    a = (n.touches ? n.touches[0] : n).clientY,
-                    l = t.scrollSensitivity,
-                    s = t.scrollSpeed,
-                    c = O(),
-                    u = !1;
-                zt !== e && (zt = e, Qt(), Wt = t.scroll, i = t.scrollFn, !0 === Wt && (Wt = A(e, !0)));
-                var d = 0,
-                    h = Wt;
-                do {
-                    var f = h,
-                        p = k(f),
-                        g = p.top,
-                        m = p.bottom,
-                        v = p.left,
-                        b = p.right,
-                        y = p.width,
-                        w = p.height,
-                        E = void 0,
-                        D = void 0,
-                        S = f.scrollWidth,
-                        _ = f.scrollHeight,
-                        C = P(f),
-                        T = f.scrollLeft,
-                        p = f.scrollTop,
-                        D = f === c ? (E = y < S && ("auto" === C.overflowX || "scroll" === C.overflowX || "visible" === C.overflowX), w < _ && ("auto" === C.overflowY || "scroll" === C.overflowY || "visible" === C.overflowY)) : (E = y < S && ("auto" === C.overflowX || "scroll" === C.overflowX), w < _ && ("auto" === C.overflowY || "scroll" === C.overflowY)),
-                        T = E && (Math.abs(b - r) <= l && T + y < S) - (Math.abs(v - r) <= l && !!T),
-                        p = D && (Math.abs(m - a) <= l && p + w < _) - (Math.abs(g - a) <= l && !!p);
-                    if (!Zt[d])
-                        for (var x = 0; x <= d; x++) Zt[x] || (Zt[x] = {});
-                    Zt[d].vx == T && Zt[d].vy == p && Zt[d].el === f || (Zt[d].el = f, Zt[d].vx = T, Zt[d].vy = p, clearInterval(Zt[d].pid), 0 == T && 0 == p || (u = !0, Zt[d].pid = setInterval(function() {
-                        o && 0 === this.layer && Bt.active._onTouchMove(qt);
-                        var t = Zt[this.layer].vy ? Zt[this.layer].vy * s : 0,
-                            e = Zt[this.layer].vx ? Zt[this.layer].vx * s : 0;
-                        "function" == typeof i && "continue" !== i.call(Bt.dragged.parentNode[j], e, t, n, qt, Zt[this.layer].el) || F(Zt[this.layer].el, e, t)
-                    }.bind({
-                        layer: d
-                    }), 24))), d++
-                } while (t.bubbleScroll && h !== c && (h = A(h, !1)));
-                $t = u
-            }
-        }, 30),
-        c = function(t) {
-            var e = t.originalEvent,
-                n = t.putSortable,
-                o = t.dragEl,
-                i = t.activeSortable,
-                r = t.dispatchSortableEvent,
-                a = t.hideGhostForTarget,
-                t = t.unhideGhostForTarget;
-            e && (i = n || i, a(), e = e.changedTouches && e.changedTouches.length ? e.changedTouches[0] : e, e = document.elementFromPoint(e.clientX, e.clientY), t(), i && !i.el.contains(e) && (r("spill"), this.onSpill({
-                dragEl: o,
-                putSortable: n
-            })))
-        };
-
-    function ne() {}
-
-    function oe() {}
-    ne.prototype = {
-        startIndex: null,
-        dragStart: function(t) {
-            t = t.oldDraggableIndex;
-            this.startIndex = t
-        },
-        onSpill: function(t) {
-            var e = t.dragEl,
-                n = t.putSortable;
-            this.sortable.captureAnimationState(), n && n.captureAnimationState();
-            t = X(this.sortable.el, this.startIndex, this.options);
-            t ? this.sortable.el.insertBefore(e, t) : this.sortable.el.appendChild(e), this.sortable.animateAll(), n && n.animateAll()
-        },
-        drop: c
-    }, a(ne, {
-        pluginName: "revertOnSpill"
-    }), oe.prototype = {
-        onSpill: function(t) {
-            var e = t.dragEl,
-                t = t.putSortable || this.sortable;
-            t.captureAnimationState(), e.parentNode && e.parentNode.removeChild(e), t.animateAll()
-        },
-        drop: c
-    }, a(oe, {
-        pluginName: "removeOnSpill"
-    });
-    var ie, re, ae, le, se, ce = [],
-        ue = [],
-        de = !1,
-        he = !1,
-        fe = !1;
-
-    function pe(n, o) {
-        ue.forEach(function(t, e) {
-            e = o.children[t.sortableIndex + (n ? Number(e) : 0)];
-            e ? o.insertBefore(t, e) : o.appendChild(t)
-        })
-    }
-
-    function ge() {
-        ce.forEach(function(t) {
-            t !== ae && t.parentNode && t.parentNode.removeChild(t)
-        })
-    }
-    return Bt.mount(new function() {
-        function t() {
-            for (var t in this.defaults = {
-                    scroll: !0,
-                    forceAutoScrollFallback: !1,
-                    scrollSensitivity: 30,
-                    scrollSpeed: 10,
-                    bubbleScroll: !0
-                }, this) "_" === t.charAt(0) && "function" == typeof this[t] && (this[t] = this[t].bind(this))
-        }
-        return t.prototype = {
-            dragStarted: function(t) {
-                t = t.originalEvent;
-                this.sortable.nativeDraggable ? h(document, "dragover", this._handleAutoScroll) : this.options.supportPointer ? h(document, "pointermove", this._handleFallbackAutoScroll) : t.touches ? h(document, "touchmove", this._handleFallbackAutoScroll) : h(document, "mousemove", this._handleFallbackAutoScroll)
-            },
-            dragOverCompleted: function(t) {
-                t = t.originalEvent;
-                this.options.dragOverBubble || t.rootEl || this._handleAutoScroll(t)
-            },
-            drop: function() {
-                this.sortable.nativeDraggable ? f(document, "dragover", this._handleAutoScroll) : (f(document, "pointermove", this._handleFallbackAutoScroll), f(document, "touchmove", this._handleFallbackAutoScroll), f(document, "mousemove", this._handleFallbackAutoScroll)), Jt(), Qt(), clearTimeout(g), g = void 0
-            },
-            nulling: function() {
-                qt = zt = Wt = $t = Vt = Gt = Ut = null, Zt.length = 0
-            },
-            _handleFallbackAutoScroll: function(t) {
-                this._handleAutoScroll(t, !0)
-            },
-            _handleAutoScroll: function(e, n) {
-                var o, i = this,
-                    r = (e.touches ? e.touches[0] : e).clientX,
-                    a = (e.touches ? e.touches[0] : e).clientY,
-                    t = document.elementFromPoint(r, a);
-                qt = e, n || this.options.forceAutoScrollFallback || w || y || u ? (ee(e, this.options, t, n), o = A(t, !0), !$t || Vt && r === Gt && a === Ut || (Vt && Jt(), Vt = setInterval(function() {
-                    var t = A(document.elementFromPoint(r, a), !0);
-                    t !== o && (o = t, Qt()), ee(e, i.options, t, n)
-                }, 10), Gt = r, Ut = a)) : this.options.bubbleScroll && A(t, !0) !== O() ? ee(e, this.options, A(t, !1), !1) : Qt()
-            }
-        }, a(t, {
-            pluginName: "scroll",
-            initializeByDefault: !0
-        })
-    }), Bt.mount(oe, ne), Bt.mount(new function() {
-        function t() {
-            this.defaults = {
-                swapClass: "sortable-swap-highlight"
-            }
-        }
-        return t.prototype = {
-            dragStart: function(t) {
-                t = t.dragEl;
-                te = t
-            },
-            dragOverValid: function(t) {
-                var e = t.completed,
-                    n = t.target,
-                    o = t.onMove,
-                    i = t.activeSortable,
-                    r = t.changed,
-                    a = t.cancel;
-                i.options.swap && (t = this.sortable.el, i = this.options, n && n !== t && (t = te, te = !1 !== o(n) ? (I(n, i.swapClass, !0), n) : null, t && t !== te && I(t, i.swapClass, !1)), r(), e(!0), a())
-            },
-            drop: function(t) {
-                var e, n, o = t.activeSortable,
-                    i = t.putSortable,
-                    r = t.dragEl,
-                    a = i || this.sortable,
-                    l = this.options;
-                te && I(te, l.swapClass, !1), te && (l.swap || i && i.options.swap) && r !== te && (a.captureAnimationState(), a !== o && o.captureAnimationState(), n = te, t = (e = r).parentNode, l = n.parentNode, t && l && !t.isEqualNode(n) && !l.isEqualNode(e) && (i = B(e), r = B(n), t.isEqualNode(l) && i < r && r++, t.insertBefore(n, t.children[i]), l.insertBefore(e, l.children[r])), a.animateAll(), a !== o && o.animateAll())
-            },
-            nulling: function() {
-                te = null
-            }
-        }, a(t, {
-            pluginName: "swap",
-            eventProperties: function() {
-                return {
-                    swapItem: te
-                }
-            }
-        })
-    }), Bt.mount(new function() {
-        function t(o) {
-            for (var t in this) "_" === t.charAt(0) && "function" == typeof this[t] && (this[t] = this[t].bind(this));
-            o.options.avoidImplicitDeselect || (o.options.supportPointer ? h(document, "pointerup", this._deselectMultiDrag) : (h(document, "mouseup", this._deselectMultiDrag), h(document, "touchend", this._deselectMultiDrag))), h(document, "keydown", this._checkKeyDown), h(document, "keyup", this._checkKeyUp), this.defaults = {
-                selectedClass: "sortable-selected",
-                multiDragKey: null,
-                avoidImplicitDeselect: !1,
-                setData: function(t, e) {
-                    var n = "";
-                    ce.length && re === o ? ce.forEach(function(t, e) {
-                        n += (e ? ", " : "") + t.textContent
-                    }) : n = e.textContent, t.setData("Text", n)
-                }
-            }
-        }
-        return t.prototype = {
-            multiDragKeyDown: !1,
-            isMultiDrag: !1,
-            delayStartGlobal: function(t) {
-                t = t.dragEl;
-                ae = t
-            },
-            delayEnded: function() {
-                this.isMultiDrag = ~ce.indexOf(ae)
-            },
-            setupClone: function(t) {
-                var e = t.sortable,
-                    t = t.cancel;
-                if (this.isMultiDrag) {
-                    for (var n = 0; n < ce.length; n++) ue.push(_(ce[n])), ue[n].sortableIndex = ce[n].sortableIndex, ue[n].draggable = !1, ue[n].style["will-change"] = "", I(ue[n], this.options.selectedClass, !1), ce[n] === ae && I(ue[n], this.options.chosenClass, !1);
-                    e._hideClone(), t()
-                }
-            },
-            clone: function(t) {
-                var e = t.sortable,
-                    n = t.rootEl,
-                    o = t.dispatchSortableEvent,
-                    t = t.cancel;
-                this.isMultiDrag && (this.options.removeCloneOnHide || ce.length && re === e && (pe(!0, n), o("clone"), t()))
-            },
-            showClone: function(t) {
-                var e = t.cloneNowShown,
-                    n = t.rootEl,
-                    t = t.cancel;
-                this.isMultiDrag && (pe(!1, n), ue.forEach(function(t) {
-                    P(t, "display", "")
-                }), e(), se = !1, t())
-            },
-            hideClone: function(t) {
-                var e = this,
-                    n = (t.sortable, t.cloneNowHidden),
-                    t = t.cancel;
-                this.isMultiDrag && (ue.forEach(function(t) {
-                    P(t, "display", "none"), e.options.removeCloneOnHide && t.parentNode && t.parentNode.removeChild(t)
-                }), n(), se = !0, t())
-            },
-            dragStartGlobal: function(t) {
-                t.sortable;
-                !this.isMultiDrag && re && re.multiDrag._deselectMultiDrag(), ce.forEach(function(t) {
-                    t.sortableIndex = B(t)
-                }), ce = ce.sort(function(t, e) {
-                    return t.sortableIndex - e.sortableIndex
-                }), fe = !0
-            },
-            dragStarted: function(t) {
-                var e, n = this,
-                    t = t.sortable;
-                this.isMultiDrag && (this.options.sort && (t.captureAnimationState(), this.options.animation && (ce.forEach(function(t) {
-                    t !== ae && P(t, "position", "absolute")
-                }), e = k(ae, !1, !0, !0), ce.forEach(function(t) {
-                    t !== ae && C(t, e)
-                }), de = he = !0)), t.animateAll(function() {
-                    de = he = !1, n.options.animation && ce.forEach(function(t) {
-                        T(t)
-                    }), n.options.sort && ge()
-                }))
-            },
-            dragOver: function(t) {
-                var e = t.target,
-                    n = t.completed,
-                    t = t.cancel;
-                he && ~ce.indexOf(e) && (n(!1), t())
-            },
-            revert: function(t) {
-                var n, o, e = t.fromSortable,
-                    i = t.rootEl,
-                    r = t.sortable,
-                    a = t.dragRect;
-                1 < ce.length && (ce.forEach(function(t) {
-                    r.addAnimationState({
-                        target: t,
-                        rect: he ? k(t) : a
-                    }), T(t), t.fromRect = a, e.removeAnimationState(t)
-                }), he = !1, n = !this.options.removeCloneOnHide, o = i, ce.forEach(function(t, e) {
-                    e = o.children[t.sortableIndex + (n ? Number(e) : 0)];
-                    e ? o.insertBefore(t, e) : o.appendChild(t)
-                }))
-            },
-            dragOverCompleted: function(t) {
-                var e, n = t.sortable,
-                    o = t.isOwner,
-                    i = t.insertion,
-                    r = t.activeSortable,
-                    a = t.parentEl,
-                    l = t.putSortable,
-                    t = this.options;
-                i && (o && r._hideClone(), de = !1, t.animation && 1 < ce.length && (he || !o && !r.options.sort && !l) && (e = k(ae, !1, !0, !0), ce.forEach(function(t) {
-                    t !== ae && (C(t, e), a.appendChild(t))
-                }), he = !0), o || (he || ge(), 1 < ce.length ? (o = se, r._showClone(n), r.options.animation && !se && o && ue.forEach(function(t) {
-                    r.addAnimationState({
-                        target: t,
-                        rect: le
-                    }), t.fromRect = le, t.thisAnimationDuration = null
-                })) : r._showClone(n)))
-            },
-            dragOverAnimationCapture: function(t) {
-                var e = t.dragRect,
-                    n = t.isOwner,
-                    t = t.activeSortable;
-                ce.forEach(function(t) {
-                    t.thisAnimationDuration = null
-                }), t.options.animation && !n && t.multiDrag.isMultiDrag && (le = a({}, e), e = v(ae, !0), le.top -= e.f, le.left -= e.e)
-            },
-            dragOverAnimationComplete: function() {
-                he && (he = !1, ge())
-            },
-            drop: function(t) {
-                var e = t.originalEvent,
-                    n = t.rootEl,
-                    o = t.parentEl,
-                    i = t.sortable,
-                    r = t.dispatchSortableEvent,
-                    a = t.oldIndex,
-                    l = t.putSortable,
-                    s = l || this.sortable;
-                if (e) {
-                    var c, u, d, h = this.options,
-                        f = o.children;
-                    if (!fe)
-                        if (h.multiDragKey && !this.multiDragKeyDown && this._deselectMultiDrag(), I(ae, h.selectedClass, !~ce.indexOf(ae)), ~ce.indexOf(ae)) ce.splice(ce.indexOf(ae), 1), ie = null, W({
-                            sortable: i,
-                            rootEl: n,
-                            name: "deselect",
-                            targetEl: ae,
-                            originalEvent: e
-                        });
-                        else {
-                            if (ce.push(ae), W({
-                                    sortable: i,
-                                    rootEl: n,
-                                    name: "select",
-                                    targetEl: ae,
-                                    originalEvent: e
-                                }), e.shiftKey && ie && i.el.contains(ie)) {
-                                var p = B(ie),
-                                    t = B(ae);
-                                if (~p && ~t && p !== t)
-                                    for (var g, m = p < t ? (g = p, t) : (g = t, p + 1); g < m; g++) ~ce.indexOf(f[g]) || (I(f[g], h.selectedClass, !0), ce.push(f[g]), W({
-                                        sortable: i,
-                                        rootEl: n,
-                                        name: "select",
-                                        targetEl: f[g],
-                                        originalEvent: e
-                                    }))
-                            } else ie = ae;
-                            re = s
-                        } fe && this.isMultiDrag && (he = !1, (o[j].options.sort || o !== n) && 1 < ce.length && (c = k(ae), u = B(ae, ":not(." + this.options.selectedClass + ")"), !de && h.animation && (ae.thisAnimationDuration = null), s.captureAnimationState(), de || (h.animation && (ae.fromRect = c, ce.forEach(function(t) {
-                        var e;
-                        t.thisAnimationDuration = null, t !== ae && (e = he ? k(t) : c, t.fromRect = e, s.addAnimationState({
-                            target: t,
-                            rect: e
-                        }))
-                    })), ge(), ce.forEach(function(t) {
-                        f[u] ? o.insertBefore(t, f[u]) : o.appendChild(t), u++
-                    }), a === B(ae) && (d = !1, ce.forEach(function(t) {
-                        t.sortableIndex !== B(t) && (d = !0)
-                    }), d && r("update"))), ce.forEach(function(t) {
-                        T(t)
-                    }), s.animateAll()), re = s), (n === o || l && "clone" !== l.lastPutMode) && ue.forEach(function(t) {
-                        t.parentNode && t.parentNode.removeChild(t)
-                    })
-                }
-            },
-            nullingGlobal: function() {
-                this.isMultiDrag = fe = !1, ue.length = 0
-            },
-            destroyGlobal: function() {
-                this._deselectMultiDrag(), f(document, "pointerup", this._deselectMultiDrag), f(document, "mouseup", this._deselectMultiDrag), f(document, "touchend", this._deselectMultiDrag), f(document, "keydown", this._checkKeyDown), f(document, "keyup", this._checkKeyUp)
-            },
-            _deselectMultiDrag: function(t) {
-                if (!(void 0 !== fe && fe || re !== this.sortable || t && N(t.target, this.options.draggable, this.sortable.el, !1) || t && 0 !== t.button))
-                    for (; ce.length;) {
-                        var e = ce[0];
-                        I(e, this.options.selectedClass, !1), ce.shift(), W({
-                            sortable: this.sortable,
-                            rootEl: this.sortable.el,
-                            name: "deselect",
-                            targetEl: e,
-                            originalEvent: t
-                        })
-                    }
-            },
-            _checkKeyDown: function(t) {
-                t.key === this.options.multiDragKey && (this.multiDragKeyDown = !0)
-            },
-            _checkKeyUp: function(t) {
-                t.key === this.options.multiDragKey && (this.multiDragKeyDown = !1)
-            }
-        }, a(t, {
-            pluginName: "multiDrag",
-            utils: {
-                select: function(t) {
-                    var e = t.parentNode[j];
-                    e && e.options.multiDrag && !~ce.indexOf(t) && (re && re !== e && (re.multiDrag._deselectMultiDrag(), re = e), I(t, e.options.selectedClass, !0), ce.push(t))
-                },
-                deselect: function(t) {
-                    var e = t.parentNode[j],
-                        n = ce.indexOf(t);
-                    e && e.options.multiDrag && ~n && (I(t, e.options.selectedClass, !1), ce.splice(n, 1))
-                }
-            },
-            eventProperties: function() {
-                var n = this,
-                    o = [],
-                    i = [];
-                return ce.forEach(function(t) {
-                    var e;
-                    o.push({
-                        multiDragElement: t,
-                        index: t.sortableIndex
-                    }), e = he && t !== ae ? -1 : he ? B(t, ":not(." + n.options.selectedClass + ")") : B(t), i.push({
-                        multiDragElement: t,
-                        index: e
-                    })
-                }), {
-                    items: r(ce),
-                    clones: [].concat(ue),
-                    oldIndicies: o,
-                    newIndicies: i
-                }
-            },
-            optionListeners: {
-                multiDragKey: function(t) {
-                    return "ctrl" === (t = t.toLowerCase()) ? t = "Control" : 1 < t.length && (t = t.charAt(0).toUpperCase() + t.substr(1)), t
-                }
-            }
-        })
-    }), Bt
+/*! Sortable 1.15.0 - MIT | git://github.com/SortableJS/Sortable.git */ ! function(t, e) {
+    "object" == typeof exports && "undefined" != typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define(e) : (t = t || self).Sortable = e()
+}(this, function() {
+    "use strict";
+
+    function e(e, t) {
+        var n, o = Object.keys(e);
+        return Object.getOwnPropertySymbols && (n = Object.getOwnPropertySymbols(e), t && (n = n.filter(function(t) {
+            return Object.getOwnPropertyDescriptor(e, t).enumerable
+        })), o.push.apply(o, n)), o
+    }
+
+    function M(o) {
+        for (var t = 1; t < arguments.length; t++) {
+            var i = null != arguments[t] ? arguments[t] : {};
+            t % 2 ? e(Object(i), !0).forEach(function(t) {
+                var e, n;
+                e = o, t = i[n = t], n in e ? Object.defineProperty(e, n, {
+                    value: t,
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0
+                }) : e[n] = t
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(o, Object.getOwnPropertyDescriptors(i)) : e(Object(i)).forEach(function(t) {
+                Object.defineProperty(o, t, Object.getOwnPropertyDescriptor(i, t))
+            })
+        }
+        return o
+    }
+
+    function o(t) {
+        return (o = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            return typeof t
+        } : function(t) {
+            return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+        })(t)
+    }
+
+    function a() {
+        return (a = Object.assign || function(t) {
+            for (var e = 1; e < arguments.length; e++) {
+                var n, o = arguments[e];
+                for (n in o) Object.prototype.hasOwnProperty.call(o, n) && (t[n] = o[n])
+            }
+            return t
+        }).apply(this, arguments)
+    }
+
+    function i(t, e) {
+        if (null == t) return {};
+        var n, o = function(t, e) {
+            if (null == t) return {};
+            for (var n, o = {}, i = Object.keys(t), r = 0; r < i.length; r++) n = i[r], 0 <= e.indexOf(n) || (o[n] = t[n]);
+            return o
+        }(t, e);
+        if (Object.getOwnPropertySymbols)
+            for (var i = Object.getOwnPropertySymbols(t), r = 0; r < i.length; r++) n = i[r], 0 <= e.indexOf(n) || Object.prototype.propertyIsEnumerable.call(t, n) && (o[n] = t[n]);
+        return o
+    }
+
+    function r(t) {
+        return function(t) {
+            if (Array.isArray(t)) return l(t)
+        }(t) || function(t) {
+            if ("undefined" != typeof Symbol && null != t[Symbol.iterator] || null != t["@@iterator"]) return Array.from(t)
+        }(t) || function(t, e) {
+            if (t) {
+                if ("string" == typeof t) return l(t, e);
+                var n = Object.prototype.toString.call(t).slice(8, -1);
+                return "Map" === (n = "Object" === n && t.constructor ? t.constructor.name : n) || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? l(t, e) : void 0
+            }
+        }(t) || function() {
+            throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+        }()
+    }
+
+    function l(t, e) {
+        (null == e || e > t.length) && (e = t.length);
+        for (var n = 0, o = new Array(e); n < e; n++) o[n] = t[n];
+        return o
+    }
+
+    function t(t) {
+        if ("undefined" != typeof window && window.navigator) return !!navigator.userAgent.match(t)
+    }
+    var y = t(/(?:Trident.*rv[ :]?11\.|msie|iemobile|Windows Phone)/i),
+        w = t(/Edge/i),
+        s = t(/firefox/i),
+        u = t(/safari/i) && !t(/chrome/i) && !t(/android/i),
+        n = t(/iP(ad|od|hone)/i),
+        c = t(/chrome/i) && t(/android/i),
+        d = {
+            capture: !1,
+            passive: !1
+        };
+
+    function h(t, e, n) {
+        t.addEventListener(e, n, !y && d)
+    }
+
+    function f(t, e, n) {
+        t.removeEventListener(e, n, !y && d)
+    }
+
+    function p(t, e) {
+        if (e && (">" === e[0] && (e = e.substring(1)), t)) try {
+            if (t.matches) return t.matches(e);
+            if (t.msMatchesSelector) return t.msMatchesSelector(e);
+            if (t.webkitMatchesSelector) return t.webkitMatchesSelector(e)
+        } catch (t) {
+            return
+        }
+    }
+
+    function N(t, e, n, o) {
+        if (t) {
+            n = n || document;
+            do {
+                if (null != e && (">" !== e[0] || t.parentNode === n) && p(t, e) || o && t === n) return t
+            } while (t !== n && (t = (i = t).host && i !== document && i.host.nodeType ? i.host : i.parentNode))
+        }
+        var i;
+        return null
+    }
+    var g, m = /\s+/g;
+
+    function I(t, e, n) {
+        var o;
+        t && e && (t.classList ? t.classList[n ? "add" : "remove"](e) : (o = (" " + t.className + " ").replace(m, " ").replace(" " + e + " ", " "), t.className = (o + (n ? " " + e : "")).replace(m, " ")))
+    }
+
+    function P(t, e, n) {
+        var o = t && t.style;
+        if (o) {
+            if (void 0 === n) return document.defaultView && document.defaultView.getComputedStyle ? n = document.defaultView.getComputedStyle(t, "") : t.currentStyle && (n = t.currentStyle), void 0 === e ? n : n[e];
+            o[e = !(e in o || -1 !== e.indexOf("webkit")) ? "-webkit-" + e : e] = n + ("string" == typeof n ? "" : "px")
+        }
+    }
+
+    function v(t, e) {
+        var n = "";
+        if ("string" == typeof t) n = t;
+        else
+            do {
+                var o = P(t, "transform")
+            } while (o && "none" !== o && (n = o + " " + n), !e && (t = t.parentNode));
+        var i = window.DOMMatrix || window.WebKitCSSMatrix || window.CSSMatrix || window.MSCSSMatrix;
+        return i && new i(n)
+    }
+
+    function b(t, e, n) {
+        if (t) {
+            var o = t.getElementsByTagName(e),
+                i = 0,
+                r = o.length;
+            if (n)
+                for (; i < r; i++) n(o[i], i);
+            return o
+        }
+        return []
+    }
+
+    function O() {
+        var t = document.scrollingElement;
+        return t || document.documentElement
+    }
+
+    function k(t, e, n, o, i) {
+        if (t.getBoundingClientRect || t === window) {
+            var r, a, l, s, c, u, d = t !== window && t.parentNode && t !== O() ? (a = (r = t.getBoundingClientRect()).top, l = r.left, s = r.bottom, c = r.right, u = r.height, r.width) : (l = a = 0, s = window.innerHeight, c = window.innerWidth, u = window.innerHeight, window.innerWidth);
+            if ((e || n) && t !== window && (i = i || t.parentNode, !y))
+                do {
+                    if (i && i.getBoundingClientRect && ("none" !== P(i, "transform") || n && "static" !== P(i, "position"))) {
+                        var h = i.getBoundingClientRect();
+                        a -= h.top + parseInt(P(i, "border-top-width")), l -= h.left + parseInt(P(i, "border-left-width")), s = a + r.height, c = l + r.width;
+                        break
+                    }
+                } while (i = i.parentNode);
+            return o && t !== window && (o = (e = v(i || t)) && e.a, t = e && e.d, e && (s = (a /= t) + (u /= t), c = (l /= o) + (d /= o))), {
+                top: a,
+                left: l,
+                bottom: s,
+                right: c,
+                width: d,
+                height: u
+            }
+        }
+    }
+
+    function R(t, e, n) {
+        for (var o = A(t, !0), i = k(t)[e]; o;) {
+            var r = k(o)[n];
+            if (!("top" === n || "left" === n ? r <= i : i <= r)) return o;
+            if (o === O()) break;
+            o = A(o, !1)
+        }
+        return !1
+    }
+
+    function X(t, e, n, o) {
+        for (var i = 0, r = 0, a = t.children; r < a.length;) {
+            if ("none" !== a[r].style.display && a[r] !== Bt.ghost && (o || a[r] !== Bt.dragged) && N(a[r], n.draggable, t, !1)) {
+                if (i === e) return a[r];
+                i++
+            }
+            r++
+        }
+        return null
+    }
+
+    function Y(t, e) {
+        for (var n = t.lastElementChild; n && (n === Bt.ghost || "none" === P(n, "display") || e && !p(n, e));) n = n.previousElementSibling;
+        return n || null
+    }
+
+    function B(t, e) {
+        var n = 0;
+        if (!t || !t.parentNode) return -1;
+        for (; t = t.previousElementSibling;) "TEMPLATE" === t.nodeName.toUpperCase() || t === Bt.clone || e && !p(t, e) || n++;
+        return n
+    }
+
+    function E(t) {
+        var e = 0,
+            n = 0,
+            o = O();
+        if (t)
+            do {
+                var i = v(t),
+                    r = i.a,
+                    i = i.d
+            } while (e += t.scrollLeft * r, n += t.scrollTop * i, t !== o && (t = t.parentNode));
+        return [e, n]
+    }
+
+    function A(t, e) {
+        if (!t || !t.getBoundingClientRect) return O();
+        var n = t,
+            o = !1;
+        do {
+            if (n.clientWidth < n.scrollWidth || n.clientHeight < n.scrollHeight) {
+                var i = P(n);
+                if (n.clientWidth < n.scrollWidth && ("auto" == i.overflowX || "scroll" == i.overflowX) || n.clientHeight < n.scrollHeight && ("auto" == i.overflowY || "scroll" == i.overflowY)) {
+                    if (!n.getBoundingClientRect || n === document.body) return O();
+                    if (o || e) return n;
+                    o = !0
+                }
+            }
+        } while (n = n.parentNode);
+        return O()
+    }
+
+    function D(t, e) {
+        return Math.round(t.top) === Math.round(e.top) && Math.round(t.left) === Math.round(e.left) && Math.round(t.height) === Math.round(e.height) && Math.round(t.width) === Math.round(e.width)
+    }
+
+    function S(e, n) {
+        return function() {
+            var t;
+            g || (1 === (t = arguments).length ? e.call(this, t[0]) : e.apply(this, t), g = setTimeout(function() {
+                g = void 0
+            }, n))
+        }
+    }
+
+    function F(t, e, n) {
+        t.scrollLeft += e, t.scrollTop += n
+    }
+
+    function _(t) {
+        var e = window.Polymer,
+            n = window.jQuery || window.Zepto;
+        return e && e.dom ? e.dom(t).cloneNode(!0) : n ? n(t).clone(!0)[0] : t.cloneNode(!0)
+    }
+
+    function C(t, e) {
+        P(t, "position", "absolute"), P(t, "top", e.top), P(t, "left", e.left), P(t, "width", e.width), P(t, "height", e.height)
+    }
+
+    function T(t) {
+        P(t, "position", ""), P(t, "top", ""), P(t, "left", ""), P(t, "width", ""), P(t, "height", "")
+    }
+    var j = "Sortable" + (new Date).getTime();
+
+    function x() {
+        var e, o = [];
+        return {
+            captureAnimationState: function() {
+                o = [], this.options.animation && [].slice.call(this.el.children).forEach(function(t) {
+                    var e, n;
+                    "none" !== P(t, "display") && t !== Bt.ghost && (o.push({
+                        target: t,
+                        rect: k(t)
+                    }), e = M({}, o[o.length - 1].rect), !t.thisAnimationDuration || (n = v(t, !0)) && (e.top -= n.f, e.left -= n.e), t.fromRect = e)
+                })
+            },
+            addAnimationState: function(t) {
+                o.push(t)
+            },
+            removeAnimationState: function(t) {
+                o.splice(function(t, e) {
+                    for (var n in t)
+                        if (t.hasOwnProperty(n))
+                            for (var o in e)
+                                if (e.hasOwnProperty(o) && e[o] === t[n][o]) return Number(n);
+                    return -1
+                }(o, {
+                    target: t
+                }), 1)
+            },
+            animateAll: function(t) {
+                var c = this;
+                if (!this.options.animation) return clearTimeout(e), void("function" == typeof t && t());
+                var u = !1,
+                    d = 0;
+                o.forEach(function(t) {
+                    var e = 0,
+                        n = t.target,
+                        o = n.fromRect,
+                        i = k(n),
+                        r = n.prevFromRect,
+                        a = n.prevToRect,
+                        l = t.rect,
+                        s = v(n, !0);
+                    s && (i.top -= s.f, i.left -= s.e), n.toRect = i, n.thisAnimationDuration && D(r, i) && !D(o, i) && (l.top - i.top) / (l.left - i.left) == (o.top - i.top) / (o.left - i.left) && (t = l, s = r, r = a, a = c.options, e = Math.sqrt(Math.pow(s.top - t.top, 2) + Math.pow(s.left - t.left, 2)) / Math.sqrt(Math.pow(s.top - r.top, 2) + Math.pow(s.left - r.left, 2)) * a.animation), D(i, o) || (n.prevFromRect = o, n.prevToRect = i, e = e || c.options.animation, c.animate(n, l, i, e)), e && (u = !0, d = Math.max(d, e), clearTimeout(n.animationResetTimer), n.animationResetTimer = setTimeout(function() {
+                        n.animationTime = 0, n.prevFromRect = null, n.fromRect = null, n.prevToRect = null, n.thisAnimationDuration = null
+                    }, e), n.thisAnimationDuration = e)
+                }), clearTimeout(e), u ? e = setTimeout(function() {
+                    "function" == typeof t && t()
+                }, d) : "function" == typeof t && t(), o = []
+            },
+            animate: function(t, e, n, o) {
+                var i, r;
+                o && (P(t, "transition", ""), P(t, "transform", ""), i = (r = v(this.el)) && r.a, r = r && r.d, i = (e.left - n.left) / (i || 1), r = (e.top - n.top) / (r || 1), t.animatingX = !!i, t.animatingY = !!r, P(t, "transform", "translate3d(" + i + "px," + r + "px,0)"), this.forRepaintDummy = t.offsetWidth, P(t, "transition", "transform " + o + "ms" + (this.options.easing ? " " + this.options.easing : "")), P(t, "transform", "translate3d(0,0,0)"), "number" == typeof t.animated && clearTimeout(t.animated), t.animated = setTimeout(function() {
+                    P(t, "transition", ""), P(t, "transform", ""), t.animated = !1, t.animatingX = !1, t.animatingY = !1
+                }, o))
+            }
+        }
+    }
+    var H = [],
+        L = {
+            initializeByDefault: !0
+        },
+        K = {
+            mount: function(e) {
+                for (var t in L) !L.hasOwnProperty(t) || t in e || (e[t] = L[t]);
+                H.forEach(function(t) {
+                    if (t.pluginName === e.pluginName) throw "Sortable: Cannot mount plugin ".concat(e.pluginName, " more than once")
+                }), H.push(e)
+            },
+            pluginEvent: function(e, n, o) {
+                var t = this;
+                this.eventCanceled = !1, o.cancel = function() {
+                    t.eventCanceled = !0
+                };
+                var i = e + "Global";
+                H.forEach(function(t) {
+                    n[t.pluginName] && (n[t.pluginName][i] && n[t.pluginName][i](M({
+                        sortable: n
+                    }, o)), n.options[t.pluginName] && n[t.pluginName][e] && n[t.pluginName][e](M({
+                        sortable: n
+                    }, o)))
+                })
+            },
+            initializePlugins: function(n, o, i, t) {
+                for (var e in H.forEach(function(t) {
+                        var e = t.pluginName;
+                        (n.options[e] || t.initializeByDefault) && ((t = new t(n, o, n.options)).sortable = n, t.options = n.options, n[e] = t, a(i, t.defaults))
+                    }), n.options) {
+                    var r;
+                    n.options.hasOwnProperty(e) && (void 0 !== (r = this.modifyOption(n, e, n.options[e])) && (n.options[e] = r))
+                }
+            },
+            getEventProperties: function(e, n) {
+                var o = {};
+                return H.forEach(function(t) {
+                    "function" == typeof t.eventProperties && a(o, t.eventProperties.call(n[t.pluginName], e))
+                }), o
+            },
+            modifyOption: function(e, n, o) {
+                var i;
+                return H.forEach(function(t) {
+                    e[t.pluginName] && t.optionListeners && "function" == typeof t.optionListeners[n] && (i = t.optionListeners[n].call(e[t.pluginName], o))
+                }), i
+            }
+        };
+
+    function W(t) {
+        var e = t.sortable,
+            n = t.rootEl,
+            o = t.name,
+            i = t.targetEl,
+            r = t.cloneEl,
+            a = t.toEl,
+            l = t.fromEl,
+            s = t.oldIndex,
+            c = t.newIndex,
+            u = t.oldDraggableIndex,
+            d = t.newDraggableIndex,
+            h = t.originalEvent,
+            f = t.putSortable,
+            p = t.extraEventProperties;
+        if (e = e || n && n[j]) {
+            var g, m = e.options,
+                t = "on" + o.charAt(0).toUpperCase() + o.substr(1);
+            !window.CustomEvent || y || w ? (g = document.createEvent("Event")).initEvent(o, !0, !0) : g = new CustomEvent(o, {
+                bubbles: !0,
+                cancelable: !0
+            }), g.to = a || n, g.from = l || n, g.item = i || n, g.clone = r, g.oldIndex = s, g.newIndex = c, g.oldDraggableIndex = u, g.newDraggableIndex = d, g.originalEvent = h, g.pullMode = f ? f.lastPutMode : void 0;
+            var v, b = M(M({}, p), K.getEventProperties(o, e));
+            for (v in b) g[v] = b[v];
+            n && n.dispatchEvent(g), m[t] && m[t].call(e, g)
+        }
+    }
+
+    function z(t, e) {
+        var n = (o = 2 < arguments.length && void 0 !== arguments[2] ? arguments[2] : {}).evt,
+            o = i(o, G);
+        K.pluginEvent.bind(Bt)(t, e, M({
+            dragEl: q,
+            parentEl: V,
+            ghostEl: Z,
+            rootEl: $,
+            nextEl: Q,
+            lastDownEl: J,
+            cloneEl: tt,
+            cloneHidden: et,
+            dragStarted: pt,
+            putSortable: lt,
+            activeSortable: Bt.active,
+            originalEvent: n,
+            oldIndex: nt,
+            oldDraggableIndex: it,
+            newIndex: ot,
+            newDraggableIndex: rt,
+            hideGhostForTarget: kt,
+            unhideGhostForTarget: Rt,
+            cloneNowHidden: function() {
+                et = !0
+            },
+            cloneNowShown: function() {
+                et = !1
+            },
+            dispatchSortableEvent: function(t) {
+                U({
+                    sortable: e,
+                    name: t,
+                    originalEvent: n
+                })
+            }
+        }, o))
+    }
+    var G = ["evt"];
+
+    function U(t) {
+        W(M({
+            putSortable: lt,
+            cloneEl: tt,
+            targetEl: q,
+            rootEl: $,
+            oldIndex: nt,
+            oldDraggableIndex: it,
+            newIndex: ot,
+            newDraggableIndex: rt
+        }, t))
+    }
+    var q, V, Z, $, Q, J, tt, et, nt, ot, it, rt, at, lt, st, ct, ut, dt, ht, ft, pt, gt, mt, vt, bt, yt = !1,
+        wt = !1,
+        Et = [],
+        Dt = !1,
+        St = !1,
+        _t = [],
+        Ct = !1,
+        Tt = [],
+        xt = "undefined" != typeof document,
+        Ot = n,
+        At = w || y ? "cssFloat" : "float",
+        Mt = xt && !c && !n && "draggable" in document.createElement("div"),
+        Nt = function() {
+            if (xt) {
+                if (y) return !1;
+                var t = document.createElement("x");
+                return t.style.cssText = "pointer-events:auto", "auto" === t.style.pointerEvents
+            }
+        }(),
+        It = function(t, e) {
+            var n = P(t),
+                o = parseInt(n.width) - parseInt(n.paddingLeft) - parseInt(n.paddingRight) - parseInt(n.borderLeftWidth) - parseInt(n.borderRightWidth),
+                i = X(t, 0, e),
+                r = X(t, 1, e),
+                a = i && P(i),
+                l = r && P(r),
+                s = a && parseInt(a.marginLeft) + parseInt(a.marginRight) + k(i).width,
+                t = l && parseInt(l.marginLeft) + parseInt(l.marginRight) + k(r).width;
+            if ("flex" === n.display) return "column" === n.flexDirection || "column-reverse" === n.flexDirection ? "vertical" : "horizontal";
+            if ("grid" === n.display) return n.gridTemplateColumns.split(" ").length <= 1 ? "vertical" : "horizontal";
+            if (i && a.float && "none" !== a.float) {
+                e = "left" === a.float ? "left" : "right";
+                return !r || "both" !== l.clear && l.clear !== e ? "horizontal" : "vertical"
+            }
+            return i && ("block" === a.display || "flex" === a.display || "table" === a.display || "grid" === a.display || o <= s && "none" === n[At] || r && "none" === n[At] && o < s + t) ? "vertical" : "horizontal"
+        },
+        Pt = function(t) {
+            function l(r, a) {
+                return function(t, e, n, o) {
+                    var i = t.options.group.name && e.options.group.name && t.options.group.name === e.options.group.name;
+                    if (null == r && (a || i)) return !0;
+                    if (null == r || !1 === r) return !1;
+                    if (a && "clone" === r) return r;
+                    if ("function" == typeof r) return l(r(t, e, n, o), a)(t, e, n, o);
+                    e = (a ? t : e).options.group.name;
+                    return !0 === r || "string" == typeof r && r === e || r.join && -1 < r.indexOf(e)
+                }
+            }
+            var e = {},
+                n = t.group;
+            n && "object" == o(n) || (n = {
+                name: n
+            }), e.name = n.name, e.checkPull = l(n.pull, !0), e.checkPut = l(n.put), e.revertClone = n.revertClone, t.group = e
+        },
+        kt = function() {
+            !Nt && Z && P(Z, "display", "none")
+        },
+        Rt = function() {
+            !Nt && Z && P(Z, "display", "")
+        };
+    xt && !c && document.addEventListener("click", function(t) {
+        if (wt) return t.preventDefault(), t.stopPropagation && t.stopPropagation(), t.stopImmediatePropagation && t.stopImmediatePropagation(), wt = !1
+    }, !0);
+
+    function Xt(t) {
+        if (q) {
+            t = t.touches ? t.touches[0] : t;
+            var e = (i = t.clientX, r = t.clientY, Et.some(function(t) {
+                var e = t[j].options.emptyInsertThreshold;
+                if (e && !Y(t)) {
+                    var n = k(t),
+                        o = i >= n.left - e && i <= n.right + e,
+                        e = r >= n.top - e && r <= n.bottom + e;
+                    return o && e ? a = t : void 0
+                }
+            }), a);
+            if (e) {
+                var n, o = {};
+                for (n in t) t.hasOwnProperty(n) && (o[n] = t[n]);
+                o.target = o.rootEl = e, o.preventDefault = void 0, o.stopPropagation = void 0, e[j]._onDragOver(o)
+            }
+        }
+        var i, r, a
+    }
+
+    function Yt(t) {
+        q && q.parentNode[j]._isOutsideThisEl(t.target)
+    }
+
+    function Bt(t, e) {
+        if (!t || !t.nodeType || 1 !== t.nodeType) throw "Sortable: `el` must be an HTMLElement, not ".concat({}.toString.call(t));
+        this.el = t, this.options = e = a({}, e), t[j] = this;
+        var n, o, i = {
+            group: null,
+            sort: !0,
+            disabled: !1,
+            store: null,
+            handle: null,
+            draggable: /^[uo]l$/i.test(t.nodeName) ? ">li" : ">*",
+            swapThreshold: 1,
+            invertSwap: !1,
+            invertedSwapThreshold: null,
+            removeCloneOnHide: !0,
+            direction: function() {
+                return It(t, this.options)
+            },
+            ghostClass: "sortable-ghost",
+            chosenClass: "sortable-chosen",
+            dragClass: "sortable-drag",
+            ignore: "a, img",
+            filter: null,
+            preventOnFilter: !0,
+            animation: 0,
+            easing: null,
+            setData: function(t, e) {
+                t.setData("Text", e.textContent)
+            },
+            dropBubble: !1,
+            dragoverBubble: !1,
+            dataIdAttr: "data-id",
+            delay: 0,
+            delayOnTouchOnly: !1,
+            touchStartThreshold: (Number.parseInt ? Number : window).parseInt(window.devicePixelRatio, 10) || 1,
+            forceFallback: !1,
+            fallbackClass: "sortable-fallback",
+            fallbackOnBody: !1,
+            fallbackTolerance: 0,
+            fallbackOffset: {
+                x: 0,
+                y: 0
+            },
+            supportPointer: !1 !== Bt.supportPointer && "PointerEvent" in window && !u,
+            emptyInsertThreshold: 5
+        };
+        for (n in K.initializePlugins(this, t, i), i) n in e || (e[n] = i[n]);
+        for (o in Pt(e), this) "_" === o.charAt(0) && "function" == typeof this[o] && (this[o] = this[o].bind(this));
+        this.nativeDraggable = !e.forceFallback && Mt, this.nativeDraggable && (this.options.touchStartThreshold = 1), e.supportPointer ? h(t, "pointerdown", this._onTapStart) : (h(t, "mousedown", this._onTapStart), h(t, "touchstart", this._onTapStart)), this.nativeDraggable && (h(t, "dragover", this), h(t, "dragenter", this)), Et.push(this.el), e.store && e.store.get && this.sort(e.store.get(this) || []), a(this, x())
+    }
+
+    function Ft(t, e, n, o, i, r, a, l) {
+        var s, c, u = t[j],
+            d = u.options.onMove;
+        return !window.CustomEvent || y || w ? (s = document.createEvent("Event")).initEvent("move", !0, !0) : s = new CustomEvent("move", {
+            bubbles: !0,
+            cancelable: !0
+        }), s.to = e, s.from = t, s.dragged = n, s.draggedRect = o, s.related = i || e, s.relatedRect = r || k(e), s.willInsertAfter = l, s.originalEvent = a, t.dispatchEvent(s), c = d ? d.call(u, s, a) : c
+    }
+
+    function jt(t) {
+        t.draggable = !1
+    }
+
+    function Ht() {
+        Ct = !1
+    }
+
+    function Lt(t) {
+        return setTimeout(t, 0)
+    }
+
+    function Kt(t) {
+        return clearTimeout(t)
+    }
+    Bt.prototype = {
+        constructor: Bt,
+        _isOutsideThisEl: function(t) {
+            this.el.contains(t) || t === this.el || (gt = null)
+        },
+        _getDirection: function(t, e) {
+            return "function" == typeof this.options.direction ? this.options.direction.call(this, t, e, q) : this.options.direction
+        },
+        _onTapStart: function(e) {
+            if (e.cancelable) {
+                var n = this,
+                    o = this.el,
+                    t = this.options,
+                    i = t.preventOnFilter,
+                    r = e.type,
+                    a = e.touches && e.touches[0] || e.pointerType && "touch" === e.pointerType && e,
+                    l = (a || e).target,
+                    s = e.target.shadowRoot && (e.path && e.path[0] || e.composedPath && e.composedPath()[0]) || l,
+                    c = t.filter;
+                if (! function(t) {
+                        Tt.length = 0;
+                        var e = t.getElementsByTagName("input"),
+                            n = e.length;
+                        for (; n--;) {
+                            var o = e[n];
+                            o.checked && Tt.push(o)
+                        }
+                    }(o), !q && !(/mousedown|pointerdown/.test(r) && 0 !== e.button || t.disabled) && !s.isContentEditable && (this.nativeDraggable || !u || !l || "SELECT" !== l.tagName.toUpperCase()) && !((l = N(l, t.draggable, o, !1)) && l.animated || J === l)) {
+                    if (nt = B(l), it = B(l, t.draggable), "function" == typeof c) {
+                        if (c.call(this, e, l, this)) return U({
+                            sortable: n,
+                            rootEl: s,
+                            name: "filter",
+                            targetEl: l,
+                            toEl: o,
+                            fromEl: o
+                        }), z("filter", n, {
+                            evt: e
+                        }), void(i && e.cancelable && e.preventDefault())
+                    } else if (c = c && c.split(",").some(function(t) {
+                            if (t = N(s, t.trim(), o, !1)) return U({
+                                sortable: n,
+                                rootEl: t,
+                                name: "filter",
+                                targetEl: l,
+                                fromEl: o,
+                                toEl: o
+                            }), z("filter", n, {
+                                evt: e
+                            }), !0
+                        })) return void(i && e.cancelable && e.preventDefault());
+                    t.handle && !N(s, t.handle, o, !1) || this._prepareDragStart(e, a, l)
+                }
+            }
+        },
+        _prepareDragStart: function(t, e, n) {
+            var o, i = this,
+                r = i.el,
+                a = i.options,
+                l = r.ownerDocument;
+            n && !q && n.parentNode === r && (o = k(n), $ = r, V = (q = n).parentNode, Q = q.nextSibling, J = n, at = a.group, st = {
+                target: Bt.dragged = q,
+                clientX: (e || t).clientX,
+                clientY: (e || t).clientY
+            }, ht = st.clientX - o.left, ft = st.clientY - o.top, this._lastX = (e || t).clientX, this._lastY = (e || t).clientY, q.style["will-change"] = "all", o = function() {
+                z("delayEnded", i, {
+                    evt: t
+                }), Bt.eventCanceled ? i._onDrop() : (i._disableDelayedDragEvents(), !s && i.nativeDraggable && (q.draggable = !0), i._triggerDragStart(t, e), U({
+                    sortable: i,
+                    name: "choose",
+                    originalEvent: t
+                }), I(q, a.chosenClass, !0))
+            }, a.ignore.split(",").forEach(function(t) {
+                b(q, t.trim(), jt)
+            }), h(l, "dragover", Xt), h(l, "mousemove", Xt), h(l, "touchmove", Xt), h(l, "mouseup", i._onDrop), h(l, "touchend", i._onDrop), h(l, "touchcancel", i._onDrop), s && this.nativeDraggable && (this.options.touchStartThreshold = 4, q.draggable = !0), z("delayStart", this, {
+                evt: t
+            }), !a.delay || a.delayOnTouchOnly && !e || this.nativeDraggable && (w || y) ? o() : Bt.eventCanceled ? this._onDrop() : (h(l, "mouseup", i._disableDelayedDrag), h(l, "touchend", i._disableDelayedDrag), h(l, "touchcancel", i._disableDelayedDrag), h(l, "mousemove", i._delayedDragTouchMoveHandler), h(l, "touchmove", i._delayedDragTouchMoveHandler), a.supportPointer && h(l, "pointermove", i._delayedDragTouchMoveHandler), i._dragStartTimer = setTimeout(o, a.delay)))
+        },
+        _delayedDragTouchMoveHandler: function(t) {
+            t = t.touches ? t.touches[0] : t;
+            Math.max(Math.abs(t.clientX - this._lastX), Math.abs(t.clientY - this._lastY)) >= Math.floor(this.options.touchStartThreshold / (this.nativeDraggable && window.devicePixelRatio || 1)) && this._disableDelayedDrag()
+        },
+        _disableDelayedDrag: function() {
+            q && jt(q), clearTimeout(this._dragStartTimer), this._disableDelayedDragEvents()
+        },
+        _disableDelayedDragEvents: function() {
+            var t = this.el.ownerDocument;
+            f(t, "mouseup", this._disableDelayedDrag), f(t, "touchend", this._disableDelayedDrag), f(t, "touchcancel", this._disableDelayedDrag), f(t, "mousemove", this._delayedDragTouchMoveHandler), f(t, "touchmove", this._delayedDragTouchMoveHandler), f(t, "pointermove", this._delayedDragTouchMoveHandler)
+        },
+        _triggerDragStart: function(t, e) {
+            e = e || "touch" == t.pointerType && t, !this.nativeDraggable || e ? this.options.supportPointer ? h(document, "pointermove", this._onTouchMove) : h(document, e ? "touchmove" : "mousemove", this._onTouchMove) : (h(q, "dragend", this), h($, "dragstart", this._onDragStart));
+            try {
+                document.selection ? Lt(function() {
+                    document.selection.empty()
+                }) : window.getSelection().removeAllRanges()
+            } catch (t) {}
+        },
+        _dragStarted: function(t, e) {
+            var n;
+            yt = !1, $ && q ? (z("dragStarted", this, {
+                evt: e
+            }), this.nativeDraggable && h(document, "dragover", Yt), n = this.options, t || I(q, n.dragClass, !1), I(q, n.ghostClass, !0), Bt.active = this, t && this._appendGhost(), U({
+                sortable: this,
+                name: "start",
+                originalEvent: e
+            })) : this._nulling()
+        },
+        _emulateDragOver: function() {
+            if (ct) {
+                this._lastX = ct.clientX, this._lastY = ct.clientY, kt();
+                for (var t = document.elementFromPoint(ct.clientX, ct.clientY), e = t; t && t.shadowRoot && (t = t.shadowRoot.elementFromPoint(ct.clientX, ct.clientY)) !== e;) e = t;
+                if (q.parentNode[j]._isOutsideThisEl(t), e)
+                    do {
+                        if (e[j])
+                            if (e[j]._onDragOver({
+                                    clientX: ct.clientX,
+                                    clientY: ct.clientY,
+                                    target: t,
+                                    rootEl: e
+                                }) && !this.options.dragoverBubble) break
+                    } while (e = (t = e).parentNode);
+                Rt()
+            }
+        },
+        _onTouchMove: function(t) {
+            if (st) {
+                var e = this.options,
+                    n = e.fallbackTolerance,
+                    o = e.fallbackOffset,
+                    i = t.touches ? t.touches[0] : t,
+                    r = Z && v(Z, !0),
+                    a = Z && r && r.a,
+                    l = Z && r && r.d,
+                    e = Ot && bt && E(bt),
+                    a = (i.clientX - st.clientX + o.x) / (a || 1) + (e ? e[0] - _t[0] : 0) / (a || 1),
+                    l = (i.clientY - st.clientY + o.y) / (l || 1) + (e ? e[1] - _t[1] : 0) / (l || 1);
+                if (!Bt.active && !yt) {
+                    if (n && Math.max(Math.abs(i.clientX - this._lastX), Math.abs(i.clientY - this._lastY)) < n) return;
+                    this._onDragStart(t, !0)
+                }
+                Z && (r ? (r.e += a - (ut || 0), r.f += l - (dt || 0)) : r = {
+                    a: 1,
+                    b: 0,
+                    c: 0,
+                    d: 1,
+                    e: a,
+                    f: l
+                }, r = "matrix(".concat(r.a, ",").concat(r.b, ",").concat(r.c, ",").concat(r.d, ",").concat(r.e, ",").concat(r.f, ")"), P(Z, "webkitTransform", r), P(Z, "mozTransform", r), P(Z, "msTransform", r), P(Z, "transform", r), ut = a, dt = l, ct = i), t.cancelable && t.preventDefault()
+            }
+        },
+        _appendGhost: function() {
+            if (!Z) {
+                var t = this.options.fallbackOnBody ? document.body : $,
+                    e = k(q, !0, Ot, !0, t),
+                    n = this.options;
+                if (Ot) {
+                    for (bt = t;
+                        "static" === P(bt, "position") && "none" === P(bt, "transform") && bt !== document;) bt = bt.parentNode;
+                    bt !== document.body && bt !== document.documentElement ? (bt === document && (bt = O()), e.top += bt.scrollTop, e.left += bt.scrollLeft) : bt = O(), _t = E(bt)
+                }
+                I(Z = q.cloneNode(!0), n.ghostClass, !1), I(Z, n.fallbackClass, !0), I(Z, n.dragClass, !0), P(Z, "transition", ""), P(Z, "transform", ""), P(Z, "box-sizing", "border-box"), P(Z, "margin", 0), P(Z, "top", e.top), P(Z, "left", e.left), P(Z, "width", e.width), P(Z, "height", e.height), P(Z, "opacity", "0.8"), P(Z, "position", Ot ? "absolute" : "fixed"), P(Z, "zIndex", "100000"), P(Z, "pointerEvents", "none"), Bt.ghost = Z, t.appendChild(Z), P(Z, "transform-origin", ht / parseInt(Z.style.width) * 100 + "% " + ft / parseInt(Z.style.height) * 100 + "%")
+            }
+        },
+        _onDragStart: function(t, e) {
+            var n = this,
+                o = t.dataTransfer,
+                i = n.options;
+            z("dragStart", this, {
+                evt: t
+            }), Bt.eventCanceled ? this._onDrop() : (z("setupClone", this), Bt.eventCanceled || ((tt = _(q)).removeAttribute("id"), tt.draggable = !1, tt.style["will-change"] = "", this._hideClone(), I(tt, this.options.chosenClass, !1), Bt.clone = tt), n.cloneId = Lt(function() {
+                z("clone", n), Bt.eventCanceled || (n.options.removeCloneOnHide || $.insertBefore(tt, q), n._hideClone(), U({
+                    sortable: n,
+                    name: "clone"
+                }))
+            }), e || I(q, i.dragClass, !0), e ? (wt = !0, n._loopId = setInterval(n._emulateDragOver, 50)) : (f(document, "mouseup", n._onDrop), f(document, "touchend", n._onDrop), f(document, "touchcancel", n._onDrop), o && (o.effectAllowed = "move", i.setData && i.setData.call(n, o, q)), h(document, "drop", n), P(q, "transform", "translateZ(0)")), yt = !0, n._dragStartId = Lt(n._dragStarted.bind(n, e, t)), h(document, "selectstart", n), pt = !0, u && P(document.body, "user-select", "none"))
+        },
+        _onDragOver: function(n) {
+            var o, i, r, t, a = this.el,
+                l = n.target,
+                e = this.options,
+                s = e.group,
+                c = Bt.active,
+                u = at === s,
+                d = e.sort,
+                h = lt || c,
+                f = this,
+                p = !1;
+            if (!Ct) {
+                if (void 0 !== n.preventDefault && n.cancelable && n.preventDefault(), l = N(l, e.draggable, a, !0), T("dragOver"), Bt.eventCanceled) return p;
+                if (q.contains(n.target) || l.animated && l.animatingX && l.animatingY || f._ignoreWhileAnimating === l) return O(!1);
+                if (wt = !1, c && !e.disabled && (u ? d || (i = V !== $) : lt === this || (this.lastPutMode = at.checkPull(this, c, q, n)) && s.checkPut(this, c, q, n))) {
+                    if (r = "vertical" === this._getDirection(n, l), o = k(q), T("dragOverValid"), Bt.eventCanceled) return p;
+                    if (i) return V = $, x(), this._hideClone(), T("revert"), Bt.eventCanceled || (Q ? $.insertBefore(q, Q) : $.appendChild(q)), O(!0);
+                    var g = Y(a, e.draggable);
+                    if (!g || function(t, e, n) {
+                            n = k(Y(n.el, n.options.draggable));
+                            return e ? t.clientX > n.right + 10 || t.clientX <= n.right && t.clientY > n.bottom && t.clientX >= n.left : t.clientX > n.right && t.clientY > n.top || t.clientX <= n.right && t.clientY > n.bottom + 10
+                        }(n, r, this) && !g.animated) {
+                        if (g === q) return O(!1);
+                        if ((l = g && a === n.target ? g : l) && (w = k(l)), !1 !== Ft($, a, q, o, l, w, n, !!l)) return x(), g && g.nextSibling ? a.insertBefore(q, g.nextSibling) : a.appendChild(q), V = a, A(), O(!0)
+                    } else if (g && function(t, e, n) {
+                            n = k(X(n.el, 0, n.options, !0));
+                            return e ? t.clientX < n.left - 10 || t.clientY < n.top && t.clientX < n.right : t.clientY < n.top - 10 || t.clientY < n.bottom && t.clientX < n.left
+                        }(n, r, this)) {
+                        var m = X(a, 0, e, !0);
+                        if (m === q) return O(!1);
+                        if (w = k(l = m), !1 !== Ft($, a, q, o, l, w, n, !1)) return x(), a.insertBefore(q, m), V = a, A(), O(!0)
+                    } else if (l.parentNode === a) {
+                        var v, b, y, w = k(l),
+                            E = q.parentNode !== a,
+                            D = (D = q.animated && q.toRect || o, C = l.animated && l.toRect || w, S = (t = r) ? D.left : D.top, s = t ? D.right : D.bottom, g = t ? D.width : D.height, m = t ? C.left : C.top, D = t ? C.right : C.bottom, C = t ? C.width : C.height, !(S === m || s === D || S + g / 2 === m + C / 2)),
+                            S = r ? "top" : "left",
+                            g = R(l, "top", "top") || R(q, "top", "top"),
+                            m = g ? g.scrollTop : void 0;
+                        if (gt !== l && (b = w[S], Dt = !1, St = !D && e.invertSwap || E), 0 !== (v = function(t, e, n, o, i, r, a, l) {
+                                var s = o ? t.clientY : t.clientX,
+                                    c = o ? n.height : n.width,
+                                    t = o ? n.top : n.left,
+                                    o = o ? n.bottom : n.right,
+                                    n = !1;
+                                if (!a)
+                                    if (l && vt < c * i) {
+                                        if (Dt = !Dt && (1 === mt ? t + c * r / 2 < s : s < o - c * r / 2) ? !0 : Dt) n = !0;
+                                        else if (1 === mt ? s < t + vt : o - vt < s) return -mt
+                                    } else if (t + c * (1 - i) / 2 < s && s < o - c * (1 - i) / 2) return function(t) {
+                                    return B(q) < B(t) ? 1 : -1
+                                }(e);
+                                if ((n = n || a) && (s < t + c * r / 2 || o - c * r / 2 < s)) return t + c / 2 < s ? 1 : -1;
+                                return 0
+                            }(n, l, w, r, D ? 1 : e.swapThreshold, null == e.invertedSwapThreshold ? e.swapThreshold : e.invertedSwapThreshold, St, gt === l)))
+                            for (var _ = B(q);
+                                (y = V.children[_ -= v]) && ("none" === P(y, "display") || y === Z););
+                        if (0 === v || y === l) return O(!1);
+                        mt = v;
+                        var C = (gt = l).nextElementSibling,
+                            E = !1,
+                            D = Ft($, a, q, o, l, w, n, E = 1 === v);
+                        if (!1 !== D) return 1 !== D && -1 !== D || (E = 1 === D), Ct = !0, setTimeout(Ht, 30), x(), E && !C ? a.appendChild(q) : l.parentNode.insertBefore(q, E ? C : l), g && F(g, 0, m - g.scrollTop), V = q.parentNode, void 0 === b || St || (vt = Math.abs(b - k(l)[S])), A(), O(!0)
+                    }
+                    if (a.contains(q)) return O(!1)
+                }
+                return !1
+            }
+
+            function T(t, e) {
+                z(t, f, M({
+                    evt: n,
+                    isOwner: u,
+                    axis: r ? "vertical" : "horizontal",
+                    revert: i,
+                    dragRect: o,
+                    targetRect: w,
+                    canSort: d,
+                    fromSortable: h,
+                    target: l,
+                    completed: O,
+                    onMove: function(t, e) {
+                        return Ft($, a, q, o, t, k(t), n, e)
+                    },
+                    changed: A
+                }, e))
+            }
+
+            function x() {
+                T("dragOverAnimationCapture"), f.captureAnimationState(), f !== h && h.captureAnimationState()
+            }
+
+            function O(t) {
+                return T("dragOverCompleted", {
+                    insertion: t
+                }), t && (u ? c._hideClone() : c._showClone(f), f !== h && (I(q, (lt || c).options.ghostClass, !1), I(q, e.ghostClass, !0)), lt !== f && f !== Bt.active ? lt = f : f === Bt.active && lt && (lt = null), h === f && (f._ignoreWhileAnimating = l), f.animateAll(function() {
+                    T("dragOverAnimationComplete"), f._ignoreWhileAnimating = null
+                }), f !== h && (h.animateAll(), h._ignoreWhileAnimating = null)), (l === q && !q.animated || l === a && !l.animated) && (gt = null), e.dragoverBubble || n.rootEl || l === document || (q.parentNode[j]._isOutsideThisEl(n.target), t || Xt(n)), !e.dragoverBubble && n.stopPropagation && n.stopPropagation(), p = !0
+            }
+
+            function A() {
+                ot = B(q), rt = B(q, e.draggable), U({
+                    sortable: f,
+                    name: "change",
+                    toEl: a,
+                    newIndex: ot,
+                    newDraggableIndex: rt,
+                    originalEvent: n
+                })
+            }
+        },
+        _ignoreWhileAnimating: null,
+        _offMoveEvents: function() {
+            f(document, "mousemove", this._onTouchMove), f(document, "touchmove", this._onTouchMove), f(document, "pointermove", this._onTouchMove), f(document, "dragover", Xt), f(document, "mousemove", Xt), f(document, "touchmove", Xt)
+        },
+        _offUpEvents: function() {
+            var t = this.el.ownerDocument;
+            f(t, "mouseup", this._onDrop), f(t, "touchend", this._onDrop), f(t, "pointerup", this._onDrop), f(t, "touchcancel", this._onDrop), f(document, "selectstart", this)
+        },
+        _onDrop: function(t) {
+            var e = this.el,
+                n = this.options;
+            ot = B(q), rt = B(q, n.draggable), z("drop", this, {
+                evt: t
+            }), V = q && q.parentNode, ot = B(q), rt = B(q, n.draggable), Bt.eventCanceled || (Dt = St = yt = !1, clearInterval(this._loopId), clearTimeout(this._dragStartTimer), Kt(this.cloneId), Kt(this._dragStartId), this.nativeDraggable && (f(document, "drop", this), f(e, "dragstart", this._onDragStart)), this._offMoveEvents(), this._offUpEvents(), u && P(document.body, "user-select", ""), P(q, "transform", ""), t && (pt && (t.cancelable && t.preventDefault(), n.dropBubble || t.stopPropagation()), Z && Z.parentNode && Z.parentNode.removeChild(Z), ($ === V || lt && "clone" !== lt.lastPutMode) && tt && tt.parentNode && tt.parentNode.removeChild(tt), q && (this.nativeDraggable && f(q, "dragend", this), jt(q), q.style["will-change"] = "", pt && !yt && I(q, (lt || this).options.ghostClass, !1), I(q, this.options.chosenClass, !1), U({
+                sortable: this,
+                name: "unchoose",
+                toEl: V,
+                newIndex: null,
+                newDraggableIndex: null,
+                originalEvent: t
+            }), $ !== V ? (0 <= ot && (U({
+                rootEl: V,
+                name: "add",
+                toEl: V,
+                fromEl: $,
+                originalEvent: t
+            }), U({
+                sortable: this,
+                name: "remove",
+                toEl: V,
+                originalEvent: t
+            }), U({
+                rootEl: V,
+                name: "sort",
+                toEl: V,
+                fromEl: $,
+                originalEvent: t
+            }), U({
+                sortable: this,
+                name: "sort",
+                toEl: V,
+                originalEvent: t
+            })), lt && lt.save()) : ot !== nt && 0 <= ot && (U({
+                sortable: this,
+                name: "update",
+                toEl: V,
+                originalEvent: t
+            }), U({
+                sortable: this,
+                name: "sort",
+                toEl: V,
+                originalEvent: t
+            })), Bt.active && (null != ot && -1 !== ot || (ot = nt, rt = it), U({
+                sortable: this,
+                name: "end",
+                toEl: V,
+                originalEvent: t
+            }), this.save())))), this._nulling()
+        },
+        _nulling: function() {
+            z("nulling", this), $ = q = V = Z = Q = tt = J = et = st = ct = pt = ot = rt = nt = it = gt = mt = lt = at = Bt.dragged = Bt.ghost = Bt.clone = Bt.active = null, Tt.forEach(function(t) {
+                t.checked = !0
+            }), Tt.length = ut = dt = 0
+        },
+        handleEvent: function(t) {
+            switch (t.type) {
+                case "drop":
+                case "dragend":
+                    this._onDrop(t);
+                    break;
+                case "dragenter":
+                case "dragover":
+                    q && (this._onDragOver(t), function(t) {
+                        t.dataTransfer && (t.dataTransfer.dropEffect = "move");
+                        t.cancelable && t.preventDefault()
+                    }(t));
+                    break;
+                case "selectstart":
+                    t.preventDefault()
+            }
+        },
+        toArray: function() {
+            for (var t, e = [], n = this.el.children, o = 0, i = n.length, r = this.options; o < i; o++) N(t = n[o], r.draggable, this.el, !1) && e.push(t.getAttribute(r.dataIdAttr) || function(t) {
+                var e = t.tagName + t.className + t.src + t.href + t.textContent,
+                    n = e.length,
+                    o = 0;
+                for (; n--;) o += e.charCodeAt(n);
+                return o.toString(36)
+            }(t));
+            return e
+        },
+        sort: function(t, e) {
+            var n = {},
+                o = this.el;
+            this.toArray().forEach(function(t, e) {
+                e = o.children[e];
+                N(e, this.options.draggable, o, !1) && (n[t] = e)
+            }, this), e && this.captureAnimationState(), t.forEach(function(t) {
+                n[t] && (o.removeChild(n[t]), o.appendChild(n[t]))
+            }), e && this.animateAll()
+        },
+        save: function() {
+            var t = this.options.store;
+            t && t.set && t.set(this)
+        },
+        closest: function(t, e) {
+            return N(t, e || this.options.draggable, this.el, !1)
+        },
+        option: function(t, e) {
+            var n = this.options;
+            if (void 0 === e) return n[t];
+            var o = K.modifyOption(this, t, e);
+            n[t] = void 0 !== o ? o : e, "group" === t && Pt(n)
+        },
+        destroy: function() {
+            z("destroy", this);
+            var t = this.el;
+            t[j] = null, f(t, "mousedown", this._onTapStart), f(t, "touchstart", this._onTapStart), f(t, "pointerdown", this._onTapStart), this.nativeDraggable && (f(t, "dragover", this), f(t, "dragenter", this)), Array.prototype.forEach.call(t.querySelectorAll("[draggable]"), function(t) {
+                t.removeAttribute("draggable")
+            }), this._onDrop(), this._disableDelayedDragEvents(), Et.splice(Et.indexOf(this.el), 1), this.el = t = null
+        },
+        _hideClone: function() {
+            et || (z("hideClone", this), Bt.eventCanceled || (P(tt, "display", "none"), this.options.removeCloneOnHide && tt.parentNode && tt.parentNode.removeChild(tt), et = !0))
+        },
+        _showClone: function(t) {
+            "clone" === t.lastPutMode ? et && (z("showClone", this), Bt.eventCanceled || (q.parentNode != $ || this.options.group.revertClone ? Q ? $.insertBefore(tt, Q) : $.appendChild(tt) : $.insertBefore(tt, q), this.options.group.revertClone && this.animate(q, tt), P(tt, "display", ""), et = !1)) : this._hideClone()
+        }
+    }, xt && h(document, "touchmove", function(t) {
+        (Bt.active || yt) && t.cancelable && t.preventDefault()
+    }), Bt.utils = {
+        on: h,
+        off: f,
+        css: P,
+        find: b,
+        is: function(t, e) {
+            return !!N(t, e, t, !1)
+        },
+        extend: function(t, e) {
+            if (t && e)
+                for (var n in e) e.hasOwnProperty(n) && (t[n] = e[n]);
+            return t
+        },
+        throttle: S,
+        closest: N,
+        toggleClass: I,
+        clone: _,
+        index: B,
+        nextTick: Lt,
+        cancelNextTick: Kt,
+        detectDirection: It,
+        getChild: X
+    }, Bt.get = function(t) {
+        return t[j]
+    }, Bt.mount = function() {
+        for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
+        (e = e[0].constructor === Array ? e[0] : e).forEach(function(t) {
+            if (!t.prototype || !t.prototype.constructor) throw "Sortable: Mounted plugin must be a constructor function, not ".concat({}.toString.call(t));
+            t.utils && (Bt.utils = M(M({}, Bt.utils), t.utils)), K.mount(t)
+        })
+    }, Bt.create = function(t, e) {
+        return new Bt(t, e)
+    };
+    var Wt, zt, Gt, Ut, qt, Vt, Zt = [],
+        $t = !(Bt.version = "1.15.0");
+
+    function Qt() {
+        Zt.forEach(function(t) {
+            clearInterval(t.pid)
+        }), Zt = []
+    }
+
+    function Jt() {
+        clearInterval(Vt)
+    }
+    var te, ee = S(function(n, t, e, o) {
+            if (t.scroll) {
+                var i, r = (n.touches ? n.touches[0] : n).clientX,
+                    a = (n.touches ? n.touches[0] : n).clientY,
+                    l = t.scrollSensitivity,
+                    s = t.scrollSpeed,
+                    c = O(),
+                    u = !1;
+                zt !== e && (zt = e, Qt(), Wt = t.scroll, i = t.scrollFn, !0 === Wt && (Wt = A(e, !0)));
+                var d = 0,
+                    h = Wt;
+                do {
+                    var f = h,
+                        p = k(f),
+                        g = p.top,
+                        m = p.bottom,
+                        v = p.left,
+                        b = p.right,
+                        y = p.width,
+                        w = p.height,
+                        E = void 0,
+                        D = void 0,
+                        S = f.scrollWidth,
+                        _ = f.scrollHeight,
+                        C = P(f),
+                        T = f.scrollLeft,
+                        p = f.scrollTop,
+                        D = f === c ? (E = y < S && ("auto" === C.overflowX || "scroll" === C.overflowX || "visible" === C.overflowX), w < _ && ("auto" === C.overflowY || "scroll" === C.overflowY || "visible" === C.overflowY)) : (E = y < S && ("auto" === C.overflowX || "scroll" === C.overflowX), w < _ && ("auto" === C.overflowY || "scroll" === C.overflowY)),
+                        T = E && (Math.abs(b - r) <= l && T + y < S) - (Math.abs(v - r) <= l && !!T),
+                        p = D && (Math.abs(m - a) <= l && p + w < _) - (Math.abs(g - a) <= l && !!p);
+                    if (!Zt[d])
+                        for (var x = 0; x <= d; x++) Zt[x] || (Zt[x] = {});
+                    Zt[d].vx == T && Zt[d].vy == p && Zt[d].el === f || (Zt[d].el = f, Zt[d].vx = T, Zt[d].vy = p, clearInterval(Zt[d].pid), 0 == T && 0 == p || (u = !0, Zt[d].pid = setInterval(function() {
+                        o && 0 === this.layer && Bt.active._onTouchMove(qt);
+                        var t = Zt[this.layer].vy ? Zt[this.layer].vy * s : 0,
+                            e = Zt[this.layer].vx ? Zt[this.layer].vx * s : 0;
+                        "function" == typeof i && "continue" !== i.call(Bt.dragged.parentNode[j], e, t, n, qt, Zt[this.layer].el) || F(Zt[this.layer].el, e, t)
+                    }.bind({
+                        layer: d
+                    }), 24))), d++
+                } while (t.bubbleScroll && h !== c && (h = A(h, !1)));
+                $t = u
+            }
+        }, 30),
+        c = function(t) {
+            var e = t.originalEvent,
+                n = t.putSortable,
+                o = t.dragEl,
+                i = t.activeSortable,
+                r = t.dispatchSortableEvent,
+                a = t.hideGhostForTarget,
+                t = t.unhideGhostForTarget;
+            e && (i = n || i, a(), e = e.changedTouches && e.changedTouches.length ? e.changedTouches[0] : e, e = document.elementFromPoint(e.clientX, e.clientY), t(), i && !i.el.contains(e) && (r("spill"), this.onSpill({
+                dragEl: o,
+                putSortable: n
+            })))
+        };
+
+    function ne() {}
+
+    function oe() {}
+    ne.prototype = {
+        startIndex: null,
+        dragStart: function(t) {
+            t = t.oldDraggableIndex;
+            this.startIndex = t
+        },
+        onSpill: function(t) {
+            var e = t.dragEl,
+                n = t.putSortable;
+            this.sortable.captureAnimationState(), n && n.captureAnimationState();
+            t = X(this.sortable.el, this.startIndex, this.options);
+            t ? this.sortable.el.insertBefore(e, t) : this.sortable.el.appendChild(e), this.sortable.animateAll(), n && n.animateAll()
+        },
+        drop: c
+    }, a(ne, {
+        pluginName: "revertOnSpill"
+    }), oe.prototype = {
+        onSpill: function(t) {
+            var e = t.dragEl,
+                t = t.putSortable || this.sortable;
+            t.captureAnimationState(), e.parentNode && e.parentNode.removeChild(e), t.animateAll()
+        },
+        drop: c
+    }, a(oe, {
+        pluginName: "removeOnSpill"
+    });
+    var ie, re, ae, le, se, ce = [],
+        ue = [],
+        de = !1,
+        he = !1,
+        fe = !1;
+
+    function pe(n, o) {
+        ue.forEach(function(t, e) {
+            e = o.children[t.sortableIndex + (n ? Number(e) : 0)];
+            e ? o.insertBefore(t, e) : o.appendChild(t)
+        })
+    }
+
+    function ge() {
+        ce.forEach(function(t) {
+            t !== ae && t.parentNode && t.parentNode.removeChild(t)
+        })
+    }
+    return Bt.mount(new function() {
+        function t() {
+            for (var t in this.defaults = {
+                    scroll: !0,
+                    forceAutoScrollFallback: !1,
+                    scrollSensitivity: 30,
+                    scrollSpeed: 10,
+                    bubbleScroll: !0
+                }, this) "_" === t.charAt(0) && "function" == typeof this[t] && (this[t] = this[t].bind(this))
+        }
+        return t.prototype = {
+            dragStarted: function(t) {
+                t = t.originalEvent;
+                this.sortable.nativeDraggable ? h(document, "dragover", this._handleAutoScroll) : this.options.supportPointer ? h(document, "pointermove", this._handleFallbackAutoScroll) : t.touches ? h(document, "touchmove", this._handleFallbackAutoScroll) : h(document, "mousemove", this._handleFallbackAutoScroll)
+            },
+            dragOverCompleted: function(t) {
+                t = t.originalEvent;
+                this.options.dragOverBubble || t.rootEl || this._handleAutoScroll(t)
+            },
+            drop: function() {
+                this.sortable.nativeDraggable ? f(document, "dragover", this._handleAutoScroll) : (f(document, "pointermove", this._handleFallbackAutoScroll), f(document, "touchmove", this._handleFallbackAutoScroll), f(document, "mousemove", this._handleFallbackAutoScroll)), Jt(), Qt(), clearTimeout(g), g = void 0
+            },
+            nulling: function() {
+                qt = zt = Wt = $t = Vt = Gt = Ut = null, Zt.length = 0
+            },
+            _handleFallbackAutoScroll: function(t) {
+                this._handleAutoScroll(t, !0)
+            },
+            _handleAutoScroll: function(e, n) {
+                var o, i = this,
+                    r = (e.touches ? e.touches[0] : e).clientX,
+                    a = (e.touches ? e.touches[0] : e).clientY,
+                    t = document.elementFromPoint(r, a);
+                qt = e, n || this.options.forceAutoScrollFallback || w || y || u ? (ee(e, this.options, t, n), o = A(t, !0), !$t || Vt && r === Gt && a === Ut || (Vt && Jt(), Vt = setInterval(function() {
+                    var t = A(document.elementFromPoint(r, a), !0);
+                    t !== o && (o = t, Qt()), ee(e, i.options, t, n)
+                }, 10), Gt = r, Ut = a)) : this.options.bubbleScroll && A(t, !0) !== O() ? ee(e, this.options, A(t, !1), !1) : Qt()
+            }
+        }, a(t, {
+            pluginName: "scroll",
+            initializeByDefault: !0
+        })
+    }), Bt.mount(oe, ne), Bt.mount(new function() {
+        function t() {
+            this.defaults = {
+                swapClass: "sortable-swap-highlight"
+            }
+        }
+        return t.prototype = {
+            dragStart: function(t) {
+                t = t.dragEl;
+                te = t
+            },
+            dragOverValid: function(t) {
+                var e = t.completed,
+                    n = t.target,
+                    o = t.onMove,
+                    i = t.activeSortable,
+                    r = t.changed,
+                    a = t.cancel;
+                i.options.swap && (t = this.sortable.el, i = this.options, n && n !== t && (t = te, te = !1 !== o(n) ? (I(n, i.swapClass, !0), n) : null, t && t !== te && I(t, i.swapClass, !1)), r(), e(!0), a())
+            },
+            drop: function(t) {
+                var e, n, o = t.activeSortable,
+                    i = t.putSortable,
+                    r = t.dragEl,
+                    a = i || this.sortable,
+                    l = this.options;
+                te && I(te, l.swapClass, !1), te && (l.swap || i && i.options.swap) && r !== te && (a.captureAnimationState(), a !== o && o.captureAnimationState(), n = te, t = (e = r).parentNode, l = n.parentNode, t && l && !t.isEqualNode(n) && !l.isEqualNode(e) && (i = B(e), r = B(n), t.isEqualNode(l) && i < r && r++, t.insertBefore(n, t.children[i]), l.insertBefore(e, l.children[r])), a.animateAll(), a !== o && o.animateAll())
+            },
+            nulling: function() {
+                te = null
+            }
+        }, a(t, {
+            pluginName: "swap",
+            eventProperties: function() {
+                return {
+                    swapItem: te
+                }
+            }
+        })
+    }), Bt.mount(new function() {
+        function t(o) {
+            for (var t in this) "_" === t.charAt(0) && "function" == typeof this[t] && (this[t] = this[t].bind(this));
+            o.options.avoidImplicitDeselect || (o.options.supportPointer ? h(document, "pointerup", this._deselectMultiDrag) : (h(document, "mouseup", this._deselectMultiDrag), h(document, "touchend", this._deselectMultiDrag))), h(document, "keydown", this._checkKeyDown), h(document, "keyup", this._checkKeyUp), this.defaults = {
+                selectedClass: "sortable-selected",
+                multiDragKey: null,
+                avoidImplicitDeselect: !1,
+                setData: function(t, e) {
+                    var n = "";
+                    ce.length && re === o ? ce.forEach(function(t, e) {
+                        n += (e ? ", " : "") + t.textContent
+                    }) : n = e.textContent, t.setData("Text", n)
+                }
+            }
+        }
+        return t.prototype = {
+            multiDragKeyDown: !1,
+            isMultiDrag: !1,
+            delayStartGlobal: function(t) {
+                t = t.dragEl;
+                ae = t
+            },
+            delayEnded: function() {
+                this.isMultiDrag = ~ce.indexOf(ae)
+            },
+            setupClone: function(t) {
+                var e = t.sortable,
+                    t = t.cancel;
+                if (this.isMultiDrag) {
+                    for (var n = 0; n < ce.length; n++) ue.push(_(ce[n])), ue[n].sortableIndex = ce[n].sortableIndex, ue[n].draggable = !1, ue[n].style["will-change"] = "", I(ue[n], this.options.selectedClass, !1), ce[n] === ae && I(ue[n], this.options.chosenClass, !1);
+                    e._hideClone(), t()
+                }
+            },
+            clone: function(t) {
+                var e = t.sortable,
+                    n = t.rootEl,
+                    o = t.dispatchSortableEvent,
+                    t = t.cancel;
+                this.isMultiDrag && (this.options.removeCloneOnHide || ce.length && re === e && (pe(!0, n), o("clone"), t()))
+            },
+            showClone: function(t) {
+                var e = t.cloneNowShown,
+                    n = t.rootEl,
+                    t = t.cancel;
+                this.isMultiDrag && (pe(!1, n), ue.forEach(function(t) {
+                    P(t, "display", "")
+                }), e(), se = !1, t())
+            },
+            hideClone: function(t) {
+                var e = this,
+                    n = (t.sortable, t.cloneNowHidden),
+                    t = t.cancel;
+                this.isMultiDrag && (ue.forEach(function(t) {
+                    P(t, "display", "none"), e.options.removeCloneOnHide && t.parentNode && t.parentNode.removeChild(t)
+                }), n(), se = !0, t())
+            },
+            dragStartGlobal: function(t) {
+                t.sortable;
+                !this.isMultiDrag && re && re.multiDrag._deselectMultiDrag(), ce.forEach(function(t) {
+                    t.sortableIndex = B(t)
+                }), ce = ce.sort(function(t, e) {
+                    return t.sortableIndex - e.sortableIndex
+                }), fe = !0
+            },
+            dragStarted: function(t) {
+                var e, n = this,
+                    t = t.sortable;
+                this.isMultiDrag && (this.options.sort && (t.captureAnimationState(), this.options.animation && (ce.forEach(function(t) {
+                    t !== ae && P(t, "position", "absolute")
+                }), e = k(ae, !1, !0, !0), ce.forEach(function(t) {
+                    t !== ae && C(t, e)
+                }), de = he = !0)), t.animateAll(function() {
+                    de = he = !1, n.options.animation && ce.forEach(function(t) {
+                        T(t)
+                    }), n.options.sort && ge()
+                }))
+            },
+            dragOver: function(t) {
+                var e = t.target,
+                    n = t.completed,
+                    t = t.cancel;
+                he && ~ce.indexOf(e) && (n(!1), t())
+            },
+            revert: function(t) {
+                var n, o, e = t.fromSortable,
+                    i = t.rootEl,
+                    r = t.sortable,
+                    a = t.dragRect;
+                1 < ce.length && (ce.forEach(function(t) {
+                    r.addAnimationState({
+                        target: t,
+                        rect: he ? k(t) : a
+                    }), T(t), t.fromRect = a, e.removeAnimationState(t)
+                }), he = !1, n = !this.options.removeCloneOnHide, o = i, ce.forEach(function(t, e) {
+                    e = o.children[t.sortableIndex + (n ? Number(e) : 0)];
+                    e ? o.insertBefore(t, e) : o.appendChild(t)
+                }))
+            },
+            dragOverCompleted: function(t) {
+                var e, n = t.sortable,
+                    o = t.isOwner,
+                    i = t.insertion,
+                    r = t.activeSortable,
+                    a = t.parentEl,
+                    l = t.putSortable,
+                    t = this.options;
+                i && (o && r._hideClone(), de = !1, t.animation && 1 < ce.length && (he || !o && !r.options.sort && !l) && (e = k(ae, !1, !0, !0), ce.forEach(function(t) {
+                    t !== ae && (C(t, e), a.appendChild(t))
+                }), he = !0), o || (he || ge(), 1 < ce.length ? (o = se, r._showClone(n), r.options.animation && !se && o && ue.forEach(function(t) {
+                    r.addAnimationState({
+                        target: t,
+                        rect: le
+                    }), t.fromRect = le, t.thisAnimationDuration = null
+                })) : r._showClone(n)))
+            },
+            dragOverAnimationCapture: function(t) {
+                var e = t.dragRect,
+                    n = t.isOwner,
+                    t = t.activeSortable;
+                ce.forEach(function(t) {
+                    t.thisAnimationDuration = null
+                }), t.options.animation && !n && t.multiDrag.isMultiDrag && (le = a({}, e), e = v(ae, !0), le.top -= e.f, le.left -= e.e)
+            },
+            dragOverAnimationComplete: function() {
+                he && (he = !1, ge())
+            },
+            drop: function(t) {
+                var e = t.originalEvent,
+                    n = t.rootEl,
+                    o = t.parentEl,
+                    i = t.sortable,
+                    r = t.dispatchSortableEvent,
+                    a = t.oldIndex,
+                    l = t.putSortable,
+                    s = l || this.sortable;
+                if (e) {
+                    var c, u, d, h = this.options,
+                        f = o.children;
+                    if (!fe)
+                        if (h.multiDragKey && !this.multiDragKeyDown && this._deselectMultiDrag(), I(ae, h.selectedClass, !~ce.indexOf(ae)), ~ce.indexOf(ae)) ce.splice(ce.indexOf(ae), 1), ie = null, W({
+                            sortable: i,
+                            rootEl: n,
+                            name: "deselect",
+                            targetEl: ae,
+                            originalEvent: e
+                        });
+                        else {
+                            if (ce.push(ae), W({
+                                    sortable: i,
+                                    rootEl: n,
+                                    name: "select",
+                                    targetEl: ae,
+                                    originalEvent: e
+                                }), e.shiftKey && ie && i.el.contains(ie)) {
+                                var p = B(ie),
+                                    t = B(ae);
+                                if (~p && ~t && p !== t)
+                                    for (var g, m = p < t ? (g = p, t) : (g = t, p + 1); g < m; g++) ~ce.indexOf(f[g]) || (I(f[g], h.selectedClass, !0), ce.push(f[g]), W({
+                                        sortable: i,
+                                        rootEl: n,
+                                        name: "select",
+                                        targetEl: f[g],
+                                        originalEvent: e
+                                    }))
+                            } else ie = ae;
+                            re = s
+                        } fe && this.isMultiDrag && (he = !1, (o[j].options.sort || o !== n) && 1 < ce.length && (c = k(ae), u = B(ae, ":not(." + this.options.selectedClass + ")"), !de && h.animation && (ae.thisAnimationDuration = null), s.captureAnimationState(), de || (h.animation && (ae.fromRect = c, ce.forEach(function(t) {
+                        var e;
+                        t.thisAnimationDuration = null, t !== ae && (e = he ? k(t) : c, t.fromRect = e, s.addAnimationState({
+                            target: t,
+                            rect: e
+                        }))
+                    })), ge(), ce.forEach(function(t) {
+                        f[u] ? o.insertBefore(t, f[u]) : o.appendChild(t), u++
+                    }), a === B(ae) && (d = !1, ce.forEach(function(t) {
+                        t.sortableIndex !== B(t) && (d = !0)
+                    }), d && r("update"))), ce.forEach(function(t) {
+                        T(t)
+                    }), s.animateAll()), re = s), (n === o || l && "clone" !== l.lastPutMode) && ue.forEach(function(t) {
+                        t.parentNode && t.parentNode.removeChild(t)
+                    })
+                }
+            },
+            nullingGlobal: function() {
+                this.isMultiDrag = fe = !1, ue.length = 0
+            },
+            destroyGlobal: function() {
+                this._deselectMultiDrag(), f(document, "pointerup", this._deselectMultiDrag), f(document, "mouseup", this._deselectMultiDrag), f(document, "touchend", this._deselectMultiDrag), f(document, "keydown", this._checkKeyDown), f(document, "keyup", this._checkKeyUp)
+            },
+            _deselectMultiDrag: function(t) {
+                if (!(void 0 !== fe && fe || re !== this.sortable || t && N(t.target, this.options.draggable, this.sortable.el, !1) || t && 0 !== t.button))
+                    for (; ce.length;) {
+                        var e = ce[0];
+                        I(e, this.options.selectedClass, !1), ce.shift(), W({
+                            sortable: this.sortable,
+                            rootEl: this.sortable.el,
+                            name: "deselect",
+                            targetEl: e,
+                            originalEvent: t
+                        })
+                    }
+            },
+            _checkKeyDown: function(t) {
+                t.key === this.options.multiDragKey && (this.multiDragKeyDown = !0)
+            },
+            _checkKeyUp: function(t) {
+                t.key === this.options.multiDragKey && (this.multiDragKeyDown = !1)
+            }
+        }, a(t, {
+            pluginName: "multiDrag",
+            utils: {
+                select: function(t) {
+                    var e = t.parentNode[j];
+                    e && e.options.multiDrag && !~ce.indexOf(t) && (re && re !== e && (re.multiDrag._deselectMultiDrag(), re = e), I(t, e.options.selectedClass, !0), ce.push(t))
+                },
+                deselect: function(t) {
+                    var e = t.parentNode[j],
+                        n = ce.indexOf(t);
+                    e && e.options.multiDrag && ~n && (I(t, e.options.selectedClass, !1), ce.splice(n, 1))
+                }
+            },
+            eventProperties: function() {
+                var n = this,
+                    o = [],
+                    i = [];
+                return ce.forEach(function(t) {
+                    var e;
+                    o.push({
+                        multiDragElement: t,
+                        index: t.sortableIndex
+                    }), e = he && t !== ae ? -1 : he ? B(t, ":not(." + n.options.selectedClass + ")") : B(t), i.push({
+                        multiDragElement: t,
+                        index: e
+                    })
+                }), {
+                    items: r(ce),
+                    clones: [].concat(ue),
+                    oldIndicies: o,
+                    newIndicies: i
+                }
+            },
+            optionListeners: {
+                multiDragKey: function(t) {
+                    return "ctrl" === (t = t.toLowerCase()) ? t = "Control" : 1 < t.length && (t = t.charAt(0).toUpperCase() + t.substr(1)), t
+                }
+            }
+        })
+    }), Bt
 });
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/range-slider.css` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/range_slider/range-slider.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -443,18 +443,22 @@
                 this.updateGroup(toolObject);
             }.bind(this));
 
             while (typeof value === 'string' && value.length > 0) {
                 try {
                     value = JSON.parse(value);
                 } catch (e) {
-                    value = null;
+                    value = {};
                 }
             }
 
+            if (value === null) {
+                value = {};
+            }
+
             if (tool in value) {
                 toolObject.initialize(this, button, this.targets, value[tool]);
             } else {
                 toolObject.initialize(this, button, this.targets, {});
             }
 
             if (toolObject.isActive(value[tool])) {
```

### Comparing `globlocks-1.1.8/globlocks/static/globlocks/widgets/utils.js` & `globlocks-1.1.9/globlocks/static/globlocks/widgets/utils.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html` & `globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-bold.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-bold.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h2.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h2.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h3.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h3.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h5.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h5.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-h6.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h6.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-palette.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg` & `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/shared/blocks/heading.html` & `globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/heading.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends "./base.html" %}
 {% load wagtailcore_tags globlocks.utils %}
+{% block classname %}{{ classname }}{% endblock %}
 {% block content %}
     {% if title %}
         {% block title %}
             <div class="globlocks-title">
                 {% block tag %}
                     <{{ tagname }} {{ attributes|safe }}>
                         {{ title|safe }}
```

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/widgets/font_picker_widget.html` & `globlocks-1.1.9/globlocks/templates/globlocks/widgets/font_picker_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/widgets/orderable_widget.html` & `globlocks-1.1.9/globlocks/templates/globlocks/widgets/orderable_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/widgets/slider_input.html` & `globlocks-1.1.9/globlocks/templates/globlocks/widgets/slider_input.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/globlocks/widgets/toolbar-widget.html` & `globlocks-1.1.9/globlocks/templates/globlocks/widgets/toolbar-widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block.html` & `globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 {% load wagtailadmin_tags  %}
-
 <div class="goodadvice-collapsible-parent{% if compact_view %} goodadvice-compact{% endif %} {{ classname }}">
     {% block help_text %}
         {% if help_text and not hide_help_text %}
             <span>
                 <div class="help">
                     {% icon name="help" classname="default" %}
                     {{ help_text }}
                 </div>
             </span>
         {% endif %}
     {% endblock help_text %}
         
-    {% block inner_children %}
-        {% for child in children.values %}
-            {% include "./base_block_field.html" %}
-        {% endfor %}
-    {% endblock inner_children %}
+     <div class="row {% if block_definition.meta.no_row_padding %}nopad{% endif %}">
+        {% block inner_children %}
+            {% for child in children.values %}
+                {% include "./base_block_field.html" %}
+            {% endfor %}
+        {% endblock inner_children %}
+    </div>
 </div>
```

### Comparing `globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html` & `globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/field.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
 {% load globlocks.admin %}
-<div class="{% columns col_size|default:12 col_xs col_sm col_md col_lg col_xl %}">
-    <div class="w-field" data-field data-contentpath="{{ child.block.name }}">
-        {% if child.block.label and not hide_labels %}
-            <label class="w-field__label" {% if child.id_for_label %}for="{{ child.id_for_label }}"{% endif %}>{{ child.block.label }}{% if child.block.required %}<span class="w-required-mark">*</span>{% endif %}</label>
-        {% endif %}
-        {{ child.render_form }}
-    </div>
+<div class="{% columns col_size|default:12 col_xs col_sm col_md col_lg col_xl %} w-field" data-field data-contentpath="{{ child.block.name }}" aria-label="{{ child.block.label }}">
+    {% if child.block.label and not hide_label %}
+        <label class="w-field__label" {% if child.id_for_label %}for="{{ child.id_for_label }}"{% endif %}>{{ child.block.label }}{% if child.block.required %}<span class="w-required-mark">*</span>{% endif %}</label>
+    {% endif %}
+    {{ child.render_form }}
 </div>
```

### Comparing `globlocks-1.1.8/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% load wagtailadmin_tags i18n %}
 
-<div class="{{ classname }} goodadvice-collapsible{% if full_size %} full{%endif%} collapsed">
+<div class="{{ classname }} goodadvice-collapsible{% if full_size %} full{%endif%} collapsed{% if hide_block_button %} hidden{%endif%}">
     <button type="button" class="goodadvice-collapsible-button button button-small bicolor button--icon">
         <span class="icon-wrapper">
             {% icon name=button_icon|default:"cog" classname="icon icon-plus icon" %} 
         </span>
         {{ button_label|default:verbose_name }}
     </button>
     {% if help_text %}
         <div class="help-text">
             <small>{{help_text}}</small>
         </div>
     {% endif %}
     <div class="goodadvice-collapsible-target{% if absolute_position %} goodadvice-collapsible-absolute{%endif%}" style="display:none;">
         <span class="goodadvice-collapsible-close">&times;</span>
-        <div class="row">
+        <div class="row {% if block_definition.meta.no_row_padding %}nopad{% endif %}">
             {% block inner_children %}
                 {% for child in children.values %}
-                    {% include "./base_block_settings_field.html" with col_size=12 %}
+                    {% include "./base_block_settings_field.html" with col_size=12 hide_label=hide_labels %}
                 {% endfor %}
             {% endblock %}
         </div>
     </div>
 </div>
```

### Comparing `globlocks-1.1.8/globlocks/templatetags/__pycache__/globlocks_admin.cpython-311.pyc` & `globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x1fe4e565 (Mon Mar  4 15:09:19 2024 UTC)
-files sz: 613
+moddate:  0x503ff965 (Tue Mar 19 07:31:28 2024 UTC)
+files sz: 886
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c006d015a010100020065016a020000000000000000a6
       000000ab0000000000000000005a036503a0040000000000000000000000
-      0000000000000000006402ac03a6010000ab010000000000000000640664
-      058401a6000000ab0000000000000000005a0564045300
+      0000000000000000006402ac03a6010000ab010000000000000000640484
+      00a6000000ab0000000000000000005a056503a004000000000000000000
+      00000000000000000000006405ac03a6010000ab01000000000000000064
+      0864078401a6000000ab0000000000000000005a0664065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('library',))
                  6 IMPORT_NAME              0 (django.template)
                  8 IMPORT_FROM              1 (library)
                 10 STORE_NAME               1 (library)
@@ -25,86 +27,160 @@
                 18 LOAD_ATTR                2 (Library)
                 28 PRECALL                  0
                 32 CALL                     0
                 42 STORE_NAME               3 (register)
    
     13          44 LOAD_NAME                3 (register)
                 46 LOAD_METHOD              4 (simple_tag)
-                68 LOAD_CONST               2 ('columns')
+                68 LOAD_CONST               2 ('get_from_mapping')
                 70 KW_NAMES                 3
                 72 PRECALL                  1
                 76 CALL                     1
    
-    14          86 LOAD_CONST               6 ((None, None, None, None, None))
-                88 LOAD_CONST               5 (<code object do_columns, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_admin.py", line 13>)
-                90 MAKE_FUNCTION            1 (defaults)
-   
-    13          92 PRECALL                  0
-                96 CALL                     0
-   
-    14         106 STORE_NAME               5 (do_columns)
-               108 LOAD_CONST               4 (None)
-               110 RETURN_VALUE
+    14          86 LOAD_CONST               4 (<code object do_get_from_mapping, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/globlocks/admin.py", line 13>)
+                88 MAKE_FUNCTION            0
+   
+    13          90 PRECALL                  0
+                94 CALL                     0
+   
+    14         104 STORE_NAME               5 (do_get_from_mapping)
+   
+    24         106 LOAD_NAME                3 (register)
+               108 LOAD_METHOD              4 (simple_tag)
+               130 LOAD_CONST               5 ('columns')
+               132 KW_NAMES                 3
+               134 PRECALL                  1
+               138 CALL                     1
+   
+    25         148 LOAD_CONST               8 ((None, None, None, None, None))
+               150 LOAD_CONST               7 (<code object do_columns, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/globlocks/admin.py", line 24>)
+               152 MAKE_FUNCTION            1 (defaults)
+   
+    24         154 PRECALL                  0
+               158 CALL                     0
+   
+    25         168 STORE_NAME               6 (do_columns)
+               170 LOAD_CONST               6 (None)
+               172 RETURN_VALUE
    consts
       0
       ('library',)
-      'columns'
+      'get_from_mapping'
       ('name',)
+      code
+         argcount  : 2
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007c006401a6020000ab020000000000
+            00000072157c00a00100000000000000000000000000000000000000007c
+            01a6010000ab01000000000000000053007401000000000000000000007c
+            006402a6020000ab02000000000000000072087c007c0119000000000000
+            00000053007405000000000000000000007c007c01a6020000ab02000000
+            00000000005300
+          13           0 RESUME                   0
+         
+          15           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                      14 LOAD_FAST                0 (mapping)
+                      16 LOAD_CONST               1 ('get')
+                      18 PRECALL                  2
+                      22 CALL                     2
+                      32 POP_JUMP_FORWARD_IF_FALSE    21 (to 76)
+         
+          16          34 LOAD_FAST                0 (mapping)
+                      36 LOAD_METHOD              1 (get)
+                      58 LOAD_FAST                1 (key)
+                      60 PRECALL                  1
+                      64 CALL                     1
+                      74 RETURN_VALUE
+         
+          18     >>   76 LOAD_GLOBAL              1 (NULL + hasattr)
+                      88 LOAD_FAST                0 (mapping)
+                      90 LOAD_CONST               2 ('__getitem__')
+                      92 PRECALL                  2
+                      96 CALL                     2
+                     106 POP_JUMP_FORWARD_IF_FALSE     8 (to 124)
+         
+          19         108 LOAD_FAST                0 (mapping)
+                     110 LOAD_FAST                1 (key)
+                     112 BINARY_SUBSCR
+                     122 RETURN_VALUE
+         
+          21     >>  124 LOAD_GLOBAL              5 (NULL + getattr)
+                     136 LOAD_FAST                0 (mapping)
+                     138 LOAD_FAST                1 (key)
+                     140 PRECALL                  2
+                     144 CALL                     2
+                     154 RETURN_VALUE
+         consts
+            None
+            'get'
+            '__getitem__'
+         names      ('hasattr', 'get', 'getattr')
+         varnames   ('mapping', 'key')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/globlocks/admin.py'
+         name       'do_get_from_mapping'
+         firstlineno 13
+         lnotab 0x020220012a0220011002
+      'columns'
       None
       code
          argcount  : 6
          nlocals   : 6
          stacksize : 12
          flags     : 3
          code
             0x97007c0070097c0170077c0270057c0370037c0470017c057d007c0170
             017c007d017c0270017c017d027c0370017c027d037c0470017c037d047c
             0570017c047d0564017c009b0064027c019b0064037c029b0064047c039b
             0064057c049b0064067c059b009d0c5300
-          13           0 RESUME                   0
+          24           0 RESUME                   0
          
-          15           2 LOAD_FAST                0 (col_size)
+          26           2 LOAD_FAST                0 (col_size)
                        4 JUMP_IF_TRUE_OR_POP      9 (to 24)
                        6 LOAD_FAST                1 (col_xs)
                        8 JUMP_IF_TRUE_OR_POP      7 (to 24)
                       10 LOAD_FAST                2 (col_sm)
                       12 JUMP_IF_TRUE_OR_POP      5 (to 24)
                       14 LOAD_FAST                3 (col_md)
                       16 JUMP_IF_TRUE_OR_POP      3 (to 24)
                       18 LOAD_FAST                4 (col_lg)
                       20 JUMP_IF_TRUE_OR_POP      1 (to 24)
                       22 LOAD_FAST                5 (col_xl)
                  >>   24 STORE_FAST               0 (col_size)
          
-          16          26 LOAD_FAST                1 (col_xs)
+          27          26 LOAD_FAST                1 (col_xs)
                       28 JUMP_IF_TRUE_OR_POP      1 (to 32)
                       30 LOAD_FAST                0 (col_size)
                  >>   32 STORE_FAST               1 (col_xs)
          
-          17          34 LOAD_FAST                2 (col_sm)
+          28          34 LOAD_FAST                2 (col_sm)
                       36 JUMP_IF_TRUE_OR_POP      1 (to 40)
                       38 LOAD_FAST                1 (col_xs)
                  >>   40 STORE_FAST               2 (col_sm)
          
-          18          42 LOAD_FAST                3 (col_md)
+          29          42 LOAD_FAST                3 (col_md)
                       44 JUMP_IF_TRUE_OR_POP      1 (to 48)
                       46 LOAD_FAST                2 (col_sm)
                  >>   48 STORE_FAST               3 (col_md)
          
-          19          50 LOAD_FAST                4 (col_lg)
+          30          50 LOAD_FAST                4 (col_lg)
                       52 JUMP_IF_TRUE_OR_POP      1 (to 56)
                       54 LOAD_FAST                3 (col_md)
                  >>   56 STORE_FAST               4 (col_lg)
          
-          20          58 LOAD_FAST                5 (col_xl)
+          31          58 LOAD_FAST                5 (col_xl)
                       60 JUMP_IF_TRUE_OR_POP      1 (to 64)
                       62 LOAD_FAST                4 (col_lg)
                  >>   64 STORE_FAST               5 (col_xl)
          
-          21          66 LOAD_CONST               1 ('col-')
+          32          66 LOAD_CONST               1 ('col-')
                       68 LOAD_FAST                0 (col_size)
                       70 FORMAT_VALUE             0
                       72 LOAD_CONST               2 (' col-xs-')
                       74 LOAD_FAST                1 (col_xs)
                       76 FORMAT_VALUE             0
                       78 LOAD_CONST               3 (' col-sm-')
                       80 LOAD_FAST                2 (col_sm)
@@ -128,20 +204,20 @@
             ' col-md-'
             ' col-lg-'
             ' col-xl-'
          names      ()
          varnames   ('col_size', 'col_xs', 'col_sm', 'col_md', 'col_lg', 'col_xl')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_admin.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/globlocks/admin.py'
          name       'do_columns'
-         firstlineno 13
+         firstlineno 24
          lnotab 0x0202180108010801080108010801
       (None, None, None, None, None)
-   names      ('django.template', 'library', 'Library', 'register', 'simple_tag', 'do_columns')
+   names      ('django.template', 'library', 'Library', 'register', 'simple_tag', 'do_get_from_mapping', 'do_columns')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_admin.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/globlocks/admin.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021e0a2a0106ff0e01
+   lnotab 0x00ff02010c021e0a2a0104ff0e01020a2a0106ff0e01
```

### Comparing `globlocks-1.1.8/globlocks/templatetags/__pycache__/globlocks_toolbar.cpython-311.pyc` & `globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,28 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0xcd0cef65 (Mon Mar 11 13:53:17 2024 UTC)
-files sz: 2275
+moddate:  0xce71f965 (Tue Mar 19 11:06:54 2024 UTC)
+files sz: 2273
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c026d045a040100640464056c056d065a060100020065036a07000000
-      0000000000a6000000ab0000000000000000005a08640684005a096508a0
-      0a00000000000000000000000000000000000000006407ac08a6010000ab
-      0100000000000000006409650b640a650b640b650b6606640c8404a60000
-      00ab0000000000000000005a0c6508a00d00000000000000000000000000
-      00000000000000640dac08a6010000ab010000000000000000640e650b64
-      0f65066a0e0000000000000000660464108404a6000000ab000000000000
-      0000005a0f6508a00d000000000000000000000000000000000000000064
-      11ac08a6010000ab010000000000000000640f65066a0e00000000000000
-      00640b6501650b65066a1000000000000000006602190000000000000000
-      00660464128404a6000000ab0000000000000000005a1164135300
+      036c046d055a050100640064046c026d065a060100640064056c076d085a
+      080100020065036a090000000000000000a6000000ab0000000000000000
+      005a0a640684005a0b650aa00c0000000000000000000000000000000000
+      0000006407ac08a6010000ab0100000000000000006409650d640a650d64
+      0b650d6606640c8404a6000000ab0000000000000000005a0e650aa00f00
+      00000000000000000000000000000000000000640dac08a6010000ab0100
+      00000000000000640e650d640f65086a1000000000000000006604641084
+      04a6000000ab0000000000000000005a11650aa00f000000000000000000
+      00000000000000000000006411ac08a6010000ab01000000000000000064
+      0f65086a100000000000000000640b6501650d65086a1200000000000000
+      00660219000000000000000000660464128404a6000000ab000000000000
+      0000005a1364135300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Tuple',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Tuple)
                 10 STORE_NAME               1 (Tuple)
@@ -32,191 +33,198 @@
                 16 LOAD_CONST               2 (('library',))
                 18 IMPORT_NAME              2 (django.template)
                 20 IMPORT_FROM              3 (library)
                 22 STORE_NAME               3 (library)
                 24 POP_TOP
    
      3          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('TemplateSyntaxError',))
-                30 IMPORT_NAME              2 (django.template)
-                32 IMPORT_FROM              4 (TemplateSyntaxError)
-                34 STORE_NAME               4 (TemplateSyntaxError)
+                28 LOAD_CONST               3 (('mark_safe',))
+                30 IMPORT_NAME              4 (django.utils.safestring)
+                32 IMPORT_FROM              5 (mark_safe)
+                34 STORE_NAME               5 (mark_safe)
                 36 POP_TOP
    
-     7          38 LOAD_CONST               4 (2)
-                40 LOAD_CONST               5 (('toolbar',))
-                42 IMPORT_NAME              5 (blocks)
-                44 IMPORT_FROM              6 (toolbar)
-                46 STORE_NAME               6 (toolbar)
+     4          38 LOAD_CONST               0 (0)
+                40 LOAD_CONST               4 (('TemplateSyntaxError',))
+                42 IMPORT_NAME              2 (django.template)
+                44 IMPORT_FROM              6 (TemplateSyntaxError)
+                46 STORE_NAME               6 (TemplateSyntaxError)
                 48 POP_TOP
    
-    10          50 PUSH_NULL
-                52 LOAD_NAME                3 (library)
-                54 LOAD_ATTR                7 (Library)
-                64 PRECALL                  0
-                68 CALL                     0
-                78 STORE_NAME               8 (register)
-   
-    12          80 LOAD_CONST               6 (<code object _valid_toolbar_value, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_toolbar.py", line 12>)
-                82 MAKE_FUNCTION            0
-                84 STORE_NAME               9 (_valid_toolbar_value)
-   
-    17          86 LOAD_NAME                8 (register)
-                88 LOAD_METHOD             10 (filter)
-               110 LOAD_CONST               7 ('t_style')
-               112 KW_NAMES                 8
-               114 PRECALL                  1
-               118 CALL                     1
-   
-    18         128 LOAD_CONST               9 ('styleAttr')
-               130 LOAD_NAME               11 (str)
-               132 LOAD_CONST              10 ('styleValue')
-               134 LOAD_NAME               11 (str)
-               136 LOAD_CONST              11 ('return')
-               138 LOAD_NAME               11 (str)
-               140 BUILD_TUPLE              6
-               142 LOAD_CONST              12 (<code object t_style, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_toolbar.py", line 17>)
-               144 MAKE_FUNCTION            4 (annotations)
-   
-    17         146 PRECALL                  0
-               150 CALL                     0
-   
-    18         160 STORE_NAME              12 (t_style)
-   
-    35         162 LOAD_NAME                8 (register)
-               164 LOAD_METHOD             13 (simple_tag)
-               186 LOAD_CONST              13 ('apply_toolbar')
-               188 KW_NAMES                 8
-               190 PRECALL                  1
-               194 CALL                     1
-   
-    36         204 LOAD_CONST              14 ('target_value')
-               206 LOAD_NAME               11 (str)
-               208 LOAD_CONST              15 ('toolbar_value')
-               210 LOAD_NAME                6 (toolbar)
-               212 LOAD_ATTR               14 (ToolbarValue)
-               222 BUILD_TUPLE              4
-               224 LOAD_CONST              16 (<code object apply_toolbar, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_toolbar.py", line 35>)
-               226 MAKE_FUNCTION            4 (annotations)
-   
-    35         228 PRECALL                  0
-               232 CALL                     0
-   
-    36         242 STORE_NAME              15 (apply_toolbar)
-   
-    58         244 LOAD_NAME                8 (register)
-               246 LOAD_METHOD             13 (simple_tag)
-               268 LOAD_CONST              17 ('toolbar_attributes')
-               270 KW_NAMES                 8
-               272 PRECALL                  1
-               276 CALL                     1
-   
-    59         286 LOAD_CONST              15 ('toolbar_value')
-               288 LOAD_NAME                6 (toolbar)
-               290 LOAD_ATTR               14 (ToolbarValue)
-               300 LOAD_CONST              11 ('return')
-               302 LOAD_NAME                1 (Tuple)
-               304 LOAD_NAME               11 (str)
-               306 LOAD_NAME                6 (toolbar)
-               308 LOAD_ATTR               16 (Attributes)
-               318 BUILD_TUPLE              2
-               320 BINARY_SUBSCR
-               330 BUILD_TUPLE              4
-               332 LOAD_CONST              18 (<code object toolbar_attributes, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_toolbar.py", line 58>)
-               334 MAKE_FUNCTION            4 (annotations)
-   
-    58         336 PRECALL                  0
-               340 CALL                     0
-   
-    59         350 STORE_NAME              17 (toolbar_attributes)
-               352 LOAD_CONST              19 (None)
-               354 RETURN_VALUE
+     8          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               5 (('toolbar',))
+                54 IMPORT_NAME              7 (globlocks.blocks)
+                56 IMPORT_FROM              8 (toolbar)
+                58 STORE_NAME               8 (toolbar)
+                60 POP_TOP
+   
+    11          62 PUSH_NULL
+                64 LOAD_NAME                3 (library)
+                66 LOAD_ATTR                9 (Library)
+                76 PRECALL                  0
+                80 CALL                     0
+                90 STORE_NAME              10 (register)
+   
+    13          92 LOAD_CONST               6 (<code object _valid_toolbar_value, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\toolbar.py", line 13>)
+                94 MAKE_FUNCTION            0
+                96 STORE_NAME              11 (_valid_toolbar_value)
+   
+    18          98 LOAD_NAME               10 (register)
+               100 LOAD_METHOD             12 (filter)
+               122 LOAD_CONST               7 ('t_style')
+               124 KW_NAMES                 8
+               126 PRECALL                  1
+               130 CALL                     1
+   
+    19         140 LOAD_CONST               9 ('styleAttr')
+               142 LOAD_NAME               13 (str)
+               144 LOAD_CONST              10 ('styleValue')
+               146 LOAD_NAME               13 (str)
+               148 LOAD_CONST              11 ('return')
+               150 LOAD_NAME               13 (str)
+               152 BUILD_TUPLE              6
+               154 LOAD_CONST              12 (<code object t_style, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\toolbar.py", line 18>)
+               156 MAKE_FUNCTION            4 (annotations)
+   
+    18         158 PRECALL                  0
+               162 CALL                     0
+   
+    19         172 STORE_NAME              14 (t_style)
+   
+    36         174 LOAD_NAME               10 (register)
+               176 LOAD_METHOD             15 (simple_tag)
+               198 LOAD_CONST              13 ('apply_toolbar')
+               200 KW_NAMES                 8
+               202 PRECALL                  1
+               206 CALL                     1
+   
+    37         216 LOAD_CONST              14 ('target_value')
+               218 LOAD_NAME               13 (str)
+               220 LOAD_CONST              15 ('toolbar_value')
+               222 LOAD_NAME                8 (toolbar)
+               224 LOAD_ATTR               16 (ToolbarValue)
+               234 BUILD_TUPLE              4
+               236 LOAD_CONST              16 (<code object apply_toolbar, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\toolbar.py", line 36>)
+               238 MAKE_FUNCTION            4 (annotations)
+   
+    36         240 PRECALL                  0
+               244 CALL                     0
+   
+    37         254 STORE_NAME              17 (apply_toolbar)
+   
+    59         256 LOAD_NAME               10 (register)
+               258 LOAD_METHOD             15 (simple_tag)
+               280 LOAD_CONST              17 ('toolbar_attributes')
+               282 KW_NAMES                 8
+               284 PRECALL                  1
+               288 CALL                     1
+   
+    60         298 LOAD_CONST              15 ('toolbar_value')
+               300 LOAD_NAME                8 (toolbar)
+               302 LOAD_ATTR               16 (ToolbarValue)
+               312 LOAD_CONST              11 ('return')
+               314 LOAD_NAME                1 (Tuple)
+               316 LOAD_NAME               13 (str)
+               318 LOAD_NAME                8 (toolbar)
+               320 LOAD_ATTR               18 (Attributes)
+               330 BUILD_TUPLE              2
+               332 BINARY_SUBSCR
+               342 BUILD_TUPLE              4
+               344 LOAD_CONST              18 (<code object toolbar_attributes, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\toolbar.py", line 59>)
+               346 MAKE_FUNCTION            4 (annotations)
+   
+    59         348 PRECALL                  0
+               352 CALL                     0
+   
+    60         362 STORE_NAME              19 (toolbar_attributes)
+               364 LOAD_CONST              19 (None)
+               366 RETURN_VALUE
    consts
       0
       ('Tuple',)
       ('library',)
+      ('mark_safe',)
       ('TemplateSyntaxError',)
-      2
       ('toolbar',)
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x97007c00721a7401000000000000000000007c00740200000000000000
             0000006a020000000000000000a6020000ab020000000000000000730f74
             07000000000000000000006401a6010000ab010000000000000000820164
             005300
-          12           0 RESUME                   0
+          13           0 RESUME                   0
          
-          13           2 LOAD_FAST                0 (value)
+          14           2 LOAD_FAST                0 (value)
                        4 POP_JUMP_FORWARD_IF_FALSE    26 (to 58)
                        6 LOAD_GLOBAL              1 (NULL + isinstance)
                       18 LOAD_FAST                0 (value)
                       20 LOAD_GLOBAL              2 (toolbar)
                       32 LOAD_ATTR                2 (ToolbarValue)
                       42 PRECALL                  2
                       46 CALL                     2
                       56 POP_JUMP_FORWARD_IF_TRUE    15 (to 88)
          
-          14     >>   58 LOAD_GLOBAL              7 (NULL + TemplateSyntaxError)
+          15     >>   58 LOAD_GLOBAL              7 (NULL + TemplateSyntaxError)
                       70 LOAD_CONST               1 ('apply_toolbar tag requires a toolbar value')
                       72 PRECALL                  1
                       76 CALL                     1
                       86 RAISE_VARARGS            1
          
-          13     >>   88 LOAD_CONST               0 (None)
+          14     >>   88 LOAD_CONST               0 (None)
                       90 RETURN_VALUE
          consts
             None
             'apply_toolbar tag requires a toolbar value'
          names      ('isinstance', 'toolbar', 'ToolbarValue', 'TemplateSyntaxError')
          varnames   ('value',)
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\toolbar.py'
          name       '_valid_toolbar_value'
-         firstlineno 12
+         firstlineno 13
          lnotab 0x020138011eff
       't_style'
       ('name',)
       'styleAttr'
       'styleValue'
       'return'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 2
          flags     : 3
          code 0x97007c0072027c017302640153007c007c0166025300
-          17           0 RESUME                   0
+          18           0 RESUME                   0
          
-          29           2 LOAD_FAST                0 (styleAttr)
+          30           2 LOAD_FAST                0 (styleAttr)
                        4 POP_JUMP_FORWARD_IF_FALSE     2 (to 10)
                        6 LOAD_FAST                1 (styleValue)
                        8 POP_JUMP_FORWARD_IF_TRUE     2 (to 14)
          
-          30     >>   10 LOAD_CONST               1 (None)
+          31     >>   10 LOAD_CONST               1 (None)
                       12 RETURN_VALUE
          
-          32     >>   14 LOAD_FAST                0 (styleAttr)
+          33     >>   14 LOAD_FAST                0 (styleAttr)
                       16 LOAD_FAST                1 (styleValue)
                       18 BUILD_TUPLE              2
                       20 RETURN_VALUE
          consts
             '\n        Helper tag for adding styles inside of your templates to the toolbar.\n\n        (returns a tuple of styleAttr, styleValue)\n\n        Example:\n        ```django-template\n        {% apply_toolbar ... style="color"|t_style:"red" %}\n        ```\n    '
             None
          names      ()
          varnames   ('styleAttr', 'styleValue')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\toolbar.py'
          name       't_style'
-         firstlineno 17
+         firstlineno 18
          lnotab 0x020c08010402
       'apply_toolbar'
       'target_value'
       'toolbar_value'
       code
          argcount  : 2
          nlocals   : 6
@@ -228,69 +236,69 @@
             0000000000a6000000ab0000000000000000007d037c02a0020000000000
             000000000000000000000000000000a6000000ab00000000000000000044
             005d305e017d047d05740700000000000000000000640284007c054400a6
             000000ab000000000000000000a6010000ab010000000000000000721302
             007c036a0400000000000000006a0500000000000000007c0467017c05a2
             0152008e0001008c317c01a0060000000000000000000000000000000000
             0000007c037c00a6020000ab0200000000000000005300
-          35           0 RESUME                   0
+          36           0 RESUME                   0
          
-          46           2 LOAD_FAST                0 (target_value)
+          47           2 LOAD_FAST                0 (target_value)
                        4 POP_JUMP_FORWARD_IF_TRUE     2 (to 10)
          
-          47           6 LOAD_CONST               1 ('')
+          48           6 LOAD_CONST               1 ('')
                        8 RETURN_VALUE
          
-          49     >>   10 LOAD_GLOBAL              1 (NULL + _valid_toolbar_value)
+          50     >>   10 LOAD_GLOBAL              1 (NULL + _valid_toolbar_value)
                       22 LOAD_FAST                1 (toolbar_value)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 POP_TOP
          
-          51          40 LOAD_FAST                1 (toolbar_value)
+          52          40 LOAD_FAST                1 (toolbar_value)
                       42 LOAD_METHOD              1 (create_element)
                       64 PRECALL                  0
                       68 CALL                     0
                       78 STORE_FAST               3 (element)
          
-          52          80 LOAD_FAST                2 (kwargs)
+          53          80 LOAD_FAST                2 (kwargs)
                       82 LOAD_METHOD              2 (items)
                      104 PRECALL                  0
                      108 CALL                     0
                      118 GET_ITER
                  >>  120 FOR_ITER                48 (to 218)
                      122 UNPACK_EX                1
                      124 STORE_FAST               4 (k)
                      126 STORE_FAST               5 (v)
          
-          53         128 LOAD_GLOBAL              7 (NULL + all)
-                     140 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_toolbar.py", line 53>)
+          54         128 LOAD_GLOBAL              7 (NULL + all)
+                     140 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\toolbar.py", line 54>)
                      142 MAKE_FUNCTION            0
                      144 LOAD_FAST                5 (v)
                      146 GET_ITER
                      148 PRECALL                  0
                      152 CALL                     0
                      162 PRECALL                  1
                      166 CALL                     1
                      176 POP_JUMP_FORWARD_IF_FALSE    19 (to 216)
          
-          54         178 PUSH_NULL
+          55         178 PUSH_NULL
                      180 LOAD_FAST                3 (element)
                      182 LOAD_ATTR                4 (attrs)
                      192 LOAD_ATTR                5 (add)
                      202 LOAD_FAST                4 (k)
                      204 BUILD_LIST               1
                      206 LOAD_FAST                5 (v)
                      208 LIST_EXTEND              1
                      210 LIST_TO_TUPLE
                      212 CALL_FUNCTION_EX         0
                      214 POP_TOP
                  >>  216 JUMP_BACKWARD           49 (to 120)
          
-          55     >>  218 LOAD_FAST                1 (toolbar_value)
+          56     >>  218 LOAD_FAST                1 (toolbar_value)
                      220 LOAD_METHOD              6 (render_element)
                      242 LOAD_FAST                3 (element)
                      244 LOAD_FAST                0 (target_value)
                      246 PRECALL                  2
                      250 CALL                     2
                      260 RETURN_VALUE
          consts
@@ -298,15 +306,15 @@
             ''
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code 0x970067007c005d067d017c016400750191028c075300
-                53           0 RESUME                   0
+                54           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 6 (to 20)
                              8 STORE_FAST               1 (val)
                             10 LOAD_FAST                1 (val)
                             12 LOAD_CONST               0 (None)
                             14 IS_OP                    1
@@ -315,136 +323,82 @@
                        >>   20 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('.0', 'val')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\toolbar.py'
                name       '<listcomp>'
-               firstlineno 53
+               firstlineno 54
                lnotab 0x
          names      ('_valid_toolbar_value', 'create_element', 'items', 'all', 'attrs', 'add', 'render_element')
          varnames   ('target_value', 'toolbar_value', 'kwargs', 'element', 'k', 'v')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\toolbar.py'
          name       'apply_toolbar'
-         firstlineno 35
+         firstlineno 36
          lnotab 0x020b040104021e022801300132012801
       'toolbar_attributes'
       code
          argcount  : 1
-         nlocals   : 5
+         nlocals   : 3
          stacksize : 5
          flags     : 11
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             0001007c00a0010000000000000000000000000000000000000000a60000
-            00ab0000000000000000007d027c01a00200000000000000000000000000
-            00000000000000a6000000ab00000000000000000044005d305e017d037d
-            04740700000000000000000000640184007c044400a6000000ab00000000
-            0000000000a6010000ab010000000000000000721302007c026a04000000
-            00000000006a0500000000000000007c0367017c04a20152008e0001008c
-            317c02a0060000000000000000000000000000000000000000a6000000ab
-            0000000000000000005300
-          58           0 RESUME                   0
+            00ab0000000000000000007d0202007c006a0200000000000000007c0266
+            0169007c01a4018e017d027c02a003000000000000000000000000000000
+            0000000000a6000000ab0000000000000000005300
+          59           0 RESUME                   0
          
-          74           2 LOAD_GLOBAL              1 (NULL + _valid_toolbar_value)
+          75           2 LOAD_GLOBAL              1 (NULL + _valid_toolbar_value)
                       14 LOAD_FAST                0 (toolbar_value)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          76          32 LOAD_FAST                0 (toolbar_value)
+          77          32 LOAD_FAST                0 (toolbar_value)
                       34 LOAD_METHOD              1 (create_element)
                       56 PRECALL                  0
                       60 CALL                     0
                       70 STORE_FAST               2 (element)
          
-          77          72 LOAD_FAST                1 (kwargs)
-                      74 LOAD_METHOD              2 (items)
-                      96 PRECALL                  0
-                     100 CALL                     0
-                     110 GET_ITER
-                 >>  112 FOR_ITER                48 (to 210)
-                     114 UNPACK_EX                1
-                     116 STORE_FAST               3 (k)
-                     118 STORE_FAST               4 (v)
-         
-          78         120 LOAD_GLOBAL              7 (NULL + all)
-                     132 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\globlocks_toolbar.py", line 78>)
-                     134 MAKE_FUNCTION            0
-                     136 LOAD_FAST                4 (v)
-                     138 GET_ITER
-                     140 PRECALL                  0
-                     144 CALL                     0
-                     154 PRECALL                  1
-                     158 CALL                     1
-                     168 POP_JUMP_FORWARD_IF_FALSE    19 (to 208)
-         
-          79         170 PUSH_NULL
-                     172 LOAD_FAST                2 (element)
-                     174 LOAD_ATTR                4 (attrs)
-                     184 LOAD_ATTR                5 (add)
-                     194 LOAD_FAST                3 (k)
-                     196 BUILD_LIST               1
-                     198 LOAD_FAST                4 (v)
-                     200 LIST_EXTEND              1
-                     202 LIST_TO_TUPLE
-                     204 CALL_FUNCTION_EX         0
-                     206 POP_TOP
-                 >>  208 JUMP_BACKWARD           49 (to 112)
-         
-          81     >>  210 LOAD_FAST                2 (element)
-                     212 LOAD_METHOD              6 (generate)
-                     234 PRECALL                  0
-                     238 CALL                     0
-                     248 RETURN_VALUE
+          78          72 PUSH_NULL
+                      74 LOAD_FAST                0 (toolbar_value)
+                      76 LOAD_ATTR                2 (_generate_element)
+                      86 LOAD_FAST                2 (element)
+                      88 BUILD_TUPLE              1
+                      90 BUILD_MAP                0
+                      92 LOAD_FAST                1 (kwargs)
+                      94 DICT_MERGE               1
+                      96 CALL_FUNCTION_EX         1
+                      98 STORE_FAST               2 (element)
+         
+          79         100 LOAD_FAST                2 (element)
+                     102 LOAD_METHOD              3 (generate)
+                     124 PRECALL                  0
+                     128 CALL                     0
+                     138 RETURN_VALUE
          consts
             '\n        Get attributes from the toolbar to generate your own target value.\n\n        Example:\n\n        ```django-template\n        {% toolbar_attributes ... as tagname, attributes %}\n\n        <{{ tagname }} {{ attributes|safe }}>\n            ...\n        </{{ tagname }}>\n        ```\n    '
-            code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 4
-               flags     : 19
-               code 0x970067007c005d067d017c016400750191028c075300
-                78           0 RESUME                   0
-                             2 BUILD_LIST               0
-                             4 LOAD_FAST                0 (.0)
-                       >>    6 FOR_ITER                 6 (to 20)
-                             8 STORE_FAST               1 (val)
-                            10 LOAD_FAST                1 (val)
-                            12 LOAD_CONST               0 (None)
-                            14 IS_OP                    1
-                            16 LIST_APPEND              2
-                            18 JUMP_BACKWARD            7 (to 6)
-                       >>   20 RETURN_VALUE
-               consts
-                  None
-               names      ()
-               varnames   ('.0', 'val')
-               freevars   ()
-               cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
-               name       '<listcomp>'
-               firstlineno 78
-               lnotab 0x
-         names      ('_valid_toolbar_value', 'create_element', 'items', 'all', 'attrs', 'add', 'generate')
-         varnames   ('toolbar_value', 'kwargs', 'element', 'k', 'v')
+         names      ('_valid_toolbar_value', 'create_element', '_generate_element', 'generate')
+         varnames   ('toolbar_value', 'kwargs', 'element')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\toolbar.py'
          name       'toolbar_attributes'
-         firstlineno 58
-         lnotab 0x02101e022801300132012802
+         firstlineno 59
+         lnotab 0x02101e0228011c01
       None
-   names      ('typing', 'Tuple', 'django.template', 'library', 'TemplateSyntaxError', 'blocks', 'toolbar', 'Library', 'register', '_valid_toolbar_value', 'filter', 'str', 't_style', 'simple_tag', 'ToolbarValue', 'apply_toolbar', 'Attributes', 'toolbar_attributes')
+   names      ('typing', 'Tuple', 'django.template', 'library', 'django.utils.safestring', 'mark_safe', 'TemplateSyntaxError', 'globlocks.blocks', 'toolbar', 'Library', 'register', '_valid_toolbar_value', 'filter', 'str', 't_style', 'simple_tag', 'ToolbarValue', 'apply_toolbar', 'Attributes', 'toolbar_attributes')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\globlocks_toolbar.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\toolbar.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c010c040c031e0206052a0112ff0e0102112a0118ff0e
-      0102162a0132ff0e01
+      0x00ff02010c010c010c010c040c031e0206052a0112ff0e0102112a0118
+      ff0e0102162a0132ff0e01
```

### Comparing `globlocks-1.1.8/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc` & `globlocks-1.1.9/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xba65bb65 (Thu Feb  1 09:34:50 2024 UTC)
+moddate:  0x503ff965 (Tue Mar 19 07:31:28 2024 UTC)
 files sz: 2463
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -39,15 +39,15 @@
                 40 STORE_NAME               4 (_CENTER)
    
      8          42 LOAD_CONST               3 (1)
                 44 STORE_NAME               5 (_RIGHT)
    
     10          46 PUSH_NULL
                 48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               4 (<code object _Position, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 10>)
+                50 LOAD_CONST               4 (<code object _Position, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 10>)
                 52 MAKE_FUNCTION            0
                 54 LOAD_CONST               5 ('_Position')
                 56 PRECALL                  2
                 60 CALL                     2
                 70 STORE_NAME               6 (_Position)
    
     63          72 PUSH_NULL
@@ -77,15 +77,15 @@
                164 KW_NAMES                 7
                166 PRECALL                  1
                170 CALL                     1
    
     68         180 LOAD_CONST               8 ('return')
                182 LOAD_NAME                6 (_Position)
                184 BUILD_TUPLE              2
-               186 LOAD_CONST               9 (<code object position_is, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 67>)
+               186 LOAD_CONST               9 (<code object position_is, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 67>)
                188 MAKE_FUNCTION            4 (annotations)
    
     67         190 PRECALL                  0
                194 CALL                     0
    
     68         204 STORE_NAME              11 (position_is)
    
@@ -96,15 +96,15 @@
                234 KW_NAMES                12
                236 PRECALL                  2
                240 CALL                     2
    
     84         250 LOAD_CONST               8 ('return')
                252 LOAD_NAME                6 (_Position)
                254 BUILD_TUPLE              2
-               256 LOAD_CONST              13 (<code object position_of, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 83>)
+               256 LOAD_CONST              13 (<code object position_of, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 83>)
                258 MAKE_FUNCTION            4 (annotations)
    
     83         260 PRECALL                  0
                264 CALL                     0
    
     84         274 STORE_NAME              13 (position_of)
                276 LOAD_CONST              14 (None)
@@ -130,43 +130,43 @@
                        8 STORE_NAME               2 (__qualname__)
          
           11          10 LOAD_NAME                3 (_CENTER)
                       12 BUILD_TUPLE              1
                       14 LOAD_CONST               1 ('position')
                       16 LOAD_NAME                4 (int)
                       18 BUILD_TUPLE              2
-                      20 LOAD_CONST               2 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 11>)
+                      20 LOAD_CONST               2 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 11>)
                       22 MAKE_FUNCTION            5 (defaults, annotations)
                       24 STORE_NAME               5 (__init__)
          
-          14          26 LOAD_CONST               3 (<code object __str__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 14>)
+          14          26 LOAD_CONST               3 (<code object __str__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 14>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               6 (__str__)
          
-          23          32 LOAD_CONST               4 (<code object __int__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 23>)
+          23          32 LOAD_CONST               4 (<code object __int__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 23>)
                       34 MAKE_FUNCTION            0
                       36 STORE_NAME               7 (__int__)
          
-          26          38 LOAD_CONST               5 (<code object __eq__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 26>)
+          26          38 LOAD_CONST               5 (<code object __eq__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 26>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME               8 (__eq__)
          
-          35          44 LOAD_CONST               6 (<code object __gt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 35>)
+          35          44 LOAD_CONST               6 (<code object __gt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 35>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               9 (__gt__)
          
-          42          50 LOAD_CONST               7 (<code object __lt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 42>)
+          42          50 LOAD_CONST               7 (<code object __lt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 42>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME              10 (__lt__)
          
-          49          56 LOAD_CONST               8 (<code object __ge__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 49>)
+          49          56 LOAD_CONST               8 (<code object __ge__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 49>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME              11 (__ge__)
          
-          56          62 LOAD_CONST               9 (<code object __le__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\go-dev\application\globlocks\templatetags\orderable_tags.py", line 56>)
+          56          62 LOAD_CONST               9 (<code object __le__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 56>)
                       64 MAKE_FUNCTION            0
                       66 STORE_NAME              12 (__le__)
                       68 LOAD_CONST              10 (None)
                       70 RETURN_VALUE
          consts
             '_Position'
             'position'
@@ -185,15 +185,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('position',)
                varnames   ('self', 'position')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__init__'
                firstlineno 11
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -239,15 +239,15 @@
                   'left'
                   'center'
                   'right'
                names      ('position', '_LEFT', '_CENTER', '_RIGHT')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__str__'
                firstlineno 14
                lnotab 0x0201200104012001040120010401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -260,15 +260,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('position',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__int__'
                firstlineno 23
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -331,15 +331,15 @@
                consts
                   None
                   False
                names      ('isinstance', 'int', 'position', '_Position', 'str')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__eq__'
                firstlineno 26
                lnotab 0x02012a0116012a0120012a012601
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -384,15 +384,15 @@
                consts
                   None
                   False
                names      ('isinstance', 'int', 'position', '_Position')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__gt__'
                firstlineno 35
                lnotab 0x02012a0116012a012001
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -437,15 +437,15 @@
                consts
                   None
                   False
                names      ('isinstance', 'int', 'position', '_Position')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__lt__'
                firstlineno 42
                lnotab 0x02012a0116012a012001
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -490,15 +490,15 @@
                consts
                   None
                   False
                names      ('isinstance', 'int', 'position', '_Position')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__ge__'
                firstlineno 49
                lnotab 0x02012a0116012a012001
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -543,24 +543,24 @@
                consts
                   None
                   False
                names      ('isinstance', 'int', 'position', '_Position')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
                name       '__le__'
                firstlineno 56
                lnotab 0x02012a0116012a012001
             None
          names      ('__name__', '__module__', '__qualname__', '_CENTER', 'int', '__init__', '__str__', '__int__', '__eq__', '__gt__', '__lt__', '__ge__', '__le__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
          name       '_Position'
          firstlineno 10
          lnotab 0x0a011003060906030609060706070607
       '_Position'
       'position_is'
       ('name',)
       'return'
@@ -641,15 +641,15 @@
             1
             2
             0
          names      ('Center', 'len', 'Left', 'Right')
          varnames   ('blocks', 'counter', 'length', 'half')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
          name       'position_is'
          firstlineno 67
          lnotab 0x020204010e011e010c010e010c0128010a010c010e010c010e01
       'position_of'
       True
       ('name', 'takes_context')
       code
@@ -692,22 +692,22 @@
             'forloop'
             'counter0'
             0
          names      ('get', 'position_is')
          varnames   ('context', 'blocks', 'fl', 'counter0')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
          name       'position_of'
          firstlineno 83
          lnotab 0x02022c012c01
       None
    names      ('django.template', 'Library', 'register', '_LEFT', '_CENTER', '_RIGHT', '_Position', 'Left', 'Center', 'Right', 'filter', 'position_is', 'simple_tag', 'position_of')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\go-dev\\application\\globlocks\\templatetags\\orderable_tags.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0314020401040104021a351601160116022a010aff0e0102
       0f2c010aff0e01
```

### Comparing `globlocks-1.1.8/globlocks/templatetags/globlocks/toolbar.py` & `globlocks-1.1.9/globlocks/templatetags/globlocks/toolbar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/templatetags/globlocks/utils.py` & `globlocks-1.1.9/globlocks/templatetags/globlocks/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,30 @@
 
 register = library.Library()
 
 
 MIN_SIZE = 1
 MAX_SIZE = 6
 
+@register.simple_tag(name="class")
+def class_tag(*args) -> str:
+    """
+        Helper tag for joining classes together.
+    """
+    return " ".join(args)
+
+@register.filter(name="add_class")
+def add_class(value: str, adder: str) -> str:
+    """
+        Helper tag for adding a class to an element.
+    """
+    if not value:
+        raise TemplateSyntaxError("add_class tag requires a value")
+
+    return f"{value} {adder}"
 
 @register.filter(name="heading")
 def heading(value: str, adder: int) -> str:
     """
         Helper tag for altering heading sizes, taking into account the min and max heading sizes.
     """
     if not value:
```

### Comparing `globlocks-1.1.8/globlocks/templatetags/orderable_tags.py` & `globlocks-1.1.9/globlocks/templatetags/orderable_tags.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/util.py` & `globlocks-1.1.9/globlocks/util.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/wagtail_hooks/alignment.py` & `globlocks-1.1.9/globlocks/wagtail_hooks/alignment.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/wagtail_hooks/icons.py` & `globlocks-1.1.9/globlocks/wagtail_hooks/icons.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/wagtail_hooks/rt_extensions.py` & `globlocks-1.1.9/globlocks/wagtail_hooks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/widgets/color_input_widget.py` & `globlocks-1.1.9/globlocks/widgets/color_input_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/widgets/fontpicker.py` & `globlocks-1.1.9/globlocks/widgets/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/widgets/justify_widget.py` & `globlocks-1.1.9/globlocks/widgets/justify_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from django.forms import widgets
 from django.utils.translation import gettext_lazy as _
+from ..choices import (
+    text_alignment_choices,
+)
 
 import json
 
 
 class JustifyWidget(widgets.RadioSelect):
     template_name = "globlocks/widgets/justify-widget.html"
     option_template_name = "globlocks/widgets/justify-widget-option.html"
     option_inherits_attrs = False
-    default_choices = (
-        ("text-left", _("Left")),
-        ("text-center", _("Center")),
-        ("text-right", _("Right")),
-    )
+    default_choices = text_alignment_choices
 
     def __init__(self, attrs=None, choices=None, targets: list[str] = None):
         choices = choices or self.default_choices
         self.targets = targets or []
         super().__init__(attrs=attrs, choices=choices)
```

### Comparing `globlocks-1.1.8/globlocks/widgets/orderable.py` & `globlocks-1.1.9/globlocks/widgets/orderable.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks/widgets/range_input.py` & `globlocks-1.1.9/globlocks/widgets/range_input.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/globlocks.egg-info/SOURCES.txt` & `globlocks-1.1.9/globlocks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 globlocks/__init__.py
 globlocks/apps.py
+globlocks/choices.py
 globlocks/colors.py
 globlocks/fonts.py
 globlocks/panels.py
 globlocks/preview.py
 globlocks/rt_extensions.py
 globlocks/settings.py
 globlocks/staticfiles.py
@@ -18,17 +19,18 @@
 globlocks.egg-info/PKG-INFO
 globlocks.egg-info/SOURCES.txt
 globlocks.egg-info/dependency_links.txt
 globlocks.egg-info/requires.txt
 globlocks.egg-info/top_level.txt
 globlocks/blocks/__init__.py
 globlocks/blocks/richtext.py
-globlocks/blocks/template.py
+globlocks/blocks/utils.py
 globlocks/blocks/bases/__init__.py
 globlocks/blocks/bases/baseblock.py
+globlocks/blocks/bases/template.py
 globlocks/blocks/bases/visibility.py
 globlocks/blocks/block_fields/__init__.py
 globlocks/blocks/block_fields/justify.py
 globlocks/blocks/block_fields/orderable_block.py
 globlocks/blocks/block_fields/colorblock/__init__.py
 globlocks/blocks/block_fields/colorblock/colorblock.py
 globlocks/blocks/block_fields/fontpicker/__init__.py
@@ -39,33 +41,34 @@
 globlocks/blocks/block_fields/toolbar/bar.py
 globlocks/blocks/block_fields/toolbar/element.py
 globlocks/blocks/block_fields/toolbar/toolbar_field.py
 globlocks/blocks/block_fields/toolbar/toolbar_widget.py
 globlocks/blocks/block_fields/toolbar/tools.py
 globlocks/blocks/components/__init__.py
 globlocks/blocks/components/heading.py
+globlocks/blocks/components/image.py
 globlocks/blocks/components/image_text.py
+globlocks/blocks/components/link.py
 globlocks/blocks/components/text.py
 globlocks/blocks/components/menus/__init__.py
 globlocks/blocks/components/menus/flat.py
 globlocks/blocks/components/menus/layered.py
 globlocks/fields/__init__.py
 globlocks/fields/colorfield.py
 globlocks/fields/fontfield.py
 globlocks/fields/orderablefield.py
-globlocks/locale/en/LC_MESSAGES/django.mo
 globlocks/locale/en/LC_MESSAGES/django.po
-globlocks/locale/nl/LC_MESSAGES/django.mo
 globlocks/locale/nl/LC_MESSAGES/django.po
 globlocks/static/globlocks/admin/block_settings.js
 globlocks/static/globlocks/admin/layout.css
 globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
 globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
 globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
 globlocks/static/globlocks/css/blocks.css
+globlocks/static/globlocks/css/bootstrap.css
 globlocks/static/globlocks/fonts/Acme-Regular.ttf
 globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
 globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
 globlocks/static/globlocks/fonts/Bangers-Regular.ttf
 globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
 globlocks/static/globlocks/fonts/Caveat-Regular.ttf
 globlocks/static/globlocks/fonts/Creepster-Regular.ttf
@@ -128,20 +131,28 @@
 globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
 globlocks/static/globlocks/widgets/range_slider/range-slider.css
 globlocks/static/globlocks/widgets/range_slider/range-slider.js
 globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
 globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
 globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
 globlocks/templates/globlocks/blocks/components/heading/heading.html
-globlocks/templates/globlocks/blocks/components/image/image.html
+globlocks/templates/globlocks/blocks/components/image/full.html
+globlocks/templates/globlocks/blocks/components/image/large.html
+globlocks/templates/globlocks/blocks/components/image/medium.html
+globlocks/templates/globlocks/blocks/components/image/small.html
 globlocks/templates/globlocks/blocks/components/image_text/image.html
 globlocks/templates/globlocks/blocks/components/image_text/image_text.html
 globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
 globlocks/templates/globlocks/blocks/components/image_text/text.html
-globlocks/templates/globlocks/blocks/components/text/text.html
+globlocks/templates/globlocks/blocks/components/link/form.html
+globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
+globlocks/templates/globlocks/blocks/components/menus/flat/item.html
+globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
+globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
+globlocks/templates/globlocks/blocks/components/text/text_block.html
 globlocks/templates/globlocks/blocks/richtext/heading.html
 globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
 globlocks/templates/globlocks/blocks/richtext/listblock.html
 globlocks/templates/globlocks/blocks/richtext/richtext.html
 globlocks/templates/globlocks/blocks/richtext/settings_form.html
 globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
 globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
@@ -177,26 +188,23 @@
 globlocks/templates/globlocks/widgets/orderable_widget.html
 globlocks/templates/globlocks/widgets/slider_input.html
 globlocks/templates/globlocks/widgets/toolbar-widget.html
 globlocks/templates/wagtailadmin/block_forms/base_block.html
 globlocks/templates/wagtailadmin/block_forms/base_block_field.html
 globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
 globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+globlocks/templates/wagtailadmin/block_forms/field.html
 globlocks/templatetags/orderable_tags.py
-globlocks/templatetags/__pycache__/globlocks.cpython-311.pyc
-globlocks/templatetags/__pycache__/globlocks_admin.cpython-311.pyc
-globlocks/templatetags/__pycache__/globlocks_toolbar.cpython-311.pyc
 globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
 globlocks/templatetags/globlocks/__init__.py
 globlocks/templatetags/globlocks/admin.py
 globlocks/templatetags/globlocks/toolbar.py
 globlocks/templatetags/globlocks/utils.py
 globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
 globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
-globlocks/templatetags/globlocks/__pycache__/main.cpython-311.pyc
 globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
 globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
 globlocks/wagtail_hooks/__init__.py
 globlocks/wagtail_hooks/admin_hooks.py
 globlocks/wagtail_hooks/alignment.py
 globlocks/wagtail_hooks/icons.py
 globlocks/wagtail_hooks/rt_extensions.py
```

### Comparing `globlocks-1.1.8/setup.cfg` & `globlocks-1.1.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6c6f 626c 6f63 6b73 0d0a 7665   = globlocks..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 380d 0a64  rsion = 1.1.8..d
+00000020: 7273 696f 6e20 3d20 312e 312e 390d 0a64  rsion = 1.1.9..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2041 6e20  escription = An 
 00000040: 6170 706c 6963 6174 696f 6e20 6d61 6465  application made
 00000050: 2066 6f72 2074 6865 2044 6a61 6e67 6f20   for the Django 
 00000060: 5765 6220 4672 616d 6577 6f72 6b2e 0d0a  Web Framework...
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
@@ -55,11 +55,13 @@
 00000360: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
 00000370: 2074 7275 650d 0a70 6163 6b61 6765 7320   true..packages 
 00000380: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
 00000390: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
 000003a0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
 000003b0: 6573 203d 200d 0a09 446a 616e 676f 203e  es = ...Django >
 000003c0: 3d20 342e 320d 0a09 5761 6774 6169 6c20  = 4.2...Wagtail 
-000003d0: 3e3d 2034 2e32 0d0a 0d0a 5b65 6767 5f69  >= 4.2....[egg_i
-000003e0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000003f0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000400: 0d0a 0d0a                                ....
+000003d0: 3e3d 2034 2e32 0d0a 0963 6f6e 6469 7469  >= 4.2...conditi
+000003e0: 6f6e 616c 5f66 6965 6c64 203e 3d20 312e  onal_field >= 1.
+000003f0: 302e 300d 0a0d 0a5b 6567 675f 696e 666f  0.0....[egg_info
+00000400: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000410: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000420: 0a                                       .
```

### Comparing `globlocks-1.1.8/tests/testapp/manage.py` & `globlocks-1.1.9/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/tests/testapp/testapp/settings.py` & `globlocks-1.1.9/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.8/tests/testapp/testapp/urls.py` & `globlocks-1.1.9/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

