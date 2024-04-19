# Comparing `tmp/globlocks-1.2.1.tar.gz` & `tmp/globlocks-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globlocks-1.2.1.tar", last modified: Fri Apr 19 08:02:48 2024, max compression
+gzip compressed data, was "globlocks-1.2.2.tar", last modified: Fri Apr 19 09:38:50 2024, max compression
```

## Comparing `globlocks-1.2.1.tar` & `globlocks-1.2.2.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.408782 globlocks-1.2.1/
--rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2659 2024-04-19 08:02:48.408782 globlocks-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1576 2024-04-19 07:39:45.000000 globlocks-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.192867 globlocks-1.2.1/globlocks/
--rw-rw-rw-   0        0        0      620 2024-04-19 08:02:43.000000 globlocks-1.2.1/globlocks/__init__.py
--rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.238693 globlocks-1.2.1/globlocks/blocks/
--rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.255287 globlocks-1.2.1/globlocks/blocks/bases/
--rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/bases/__init__.py
--rw-rw-rw-   0        0        0    13076 2024-04-19 08:02:15.000000 globlocks-1.2.1/globlocks/blocks/bases/baseblock.py
--rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/bases/template.py
--rw-rw-rw-   0        0        0    10194 2024-04-19 07:59:16.000000 globlocks-1.2.1/globlocks/blocks/bases/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.258434 globlocks-1.2.1/globlocks/blocks/block_fields/
--rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.261244 globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/
--rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/__init__.py
--rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/colorblock.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.263894 globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/
--rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/__init__.py
--rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/fontpicker.py
--rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/justify.py
--rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/orderable_block.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.266008 globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/
--rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/__init__.py
--rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/rangeslider.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.275294 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/
--rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-04-02 23:32:32.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/bar.py
--rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/element.py
--rw-rw-rw-   0        0        0     3112 2024-04-02 23:34:11.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_field.py
--rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
--rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.281865 globlocks-1.2.1/globlocks/blocks/components/
--rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/__init__.py
--rw-rw-rw-   0        0        0     1653 2024-03-30 23:54:15.000000 globlocks-1.2.1/globlocks/blocks/components/heading.py
--rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/image.py
--rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/image_text.py
--rw-rw-rw-   0        0        0     9072 2024-03-31 00:20:40.000000 globlocks-1.2.1/globlocks/blocks/components/link.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.287360 globlocks-1.2.1/globlocks/blocks/components/menus/
--rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/menus/__init__.py
--rw-rw-rw-   0        0        0     2772 2024-03-29 13:30:58.000000 globlocks-1.2.1/globlocks/blocks/components/menus/flat.py
--rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/menus/layered.py
--rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/text.py
--rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/richtext.py
--rw-rw-rw-   0        0        0      756 2024-03-31 00:56:58.000000 globlocks-1.2.1/globlocks/blocks/utils.py
--rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/choices.py
--rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/colors.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.292357 globlocks-1.2.1/globlocks/fields/
--rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/__init__.py
--rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/colorfield.py
--rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/fontfield.py
--rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/orderablefield.py
--rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fonts.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.142275 globlocks-1.2.1/globlocks/locale/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.142275 globlocks-1.2.1/globlocks/locale/en/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.304451 globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      380 2024-04-10 20:48:48.000000 globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.142275 globlocks-1.2.1/globlocks/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.324015 globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1420 2024-04-11 09:05:49.000000 globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    11858 2024-04-11 09:04:54.000000 globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/panels.py
--rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/preview.py
--rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/rt_extensions.py
--rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.143282 globlocks-1.2.1/globlocks/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.146974 globlocks-1.2.1/globlocks/static/globlocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.326925 globlocks-1.2.1/globlocks/static/globlocks/admin/
--rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/block_settings.js
--rw-rw-rw-   0        0        0    24317 2024-04-02 17:24:43.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/layout.css
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.353694 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/
--rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
--rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
--rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.364819 globlocks-1.2.1/globlocks/static/globlocks/css/
--rw-rw-rw-   0        0        0     8918 2024-03-31 14:27:18.000000 globlocks-1.2.1/globlocks/static/globlocks/css/blocks.css
--rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.2.1/globlocks/static/globlocks/css/bootstrap.css
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.857289 globlocks-1.2.1/globlocks/static/globlocks/fonts/
--rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Acme-Regular.ttf
--rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
--rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
--rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
--rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
--rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
--rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
--rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
--rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
--rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Inter-Regular.ttf
--rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
--rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
--rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Lato-Regular.ttf
--rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
--rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
--rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
--rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
--rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
--rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
--rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
--rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
--rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
--rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
--rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
--rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
--rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
--rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
--rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
--rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
--rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
--rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
--rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
--rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
--rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
--rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
--rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
--rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
--rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
--rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.145975 globlocks-1.2.1/globlocks/static/globlocks/richtext/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.880300 globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/
--rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.css
--rw-rw-rw-   0        0        0     5728 2024-04-19 08:00:08.000000 globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.883252 globlocks-1.2.1/globlocks/static/globlocks/richtext/rt_extensions/
--rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.886250 globlocks-1.2.1/globlocks/static/globlocks/widgets/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.958534 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/
--rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/LICENSE
--rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
--rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:18.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
--rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.css
--rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.976913 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/
--rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
--rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
--rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker.css
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.985641 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/
--rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-controller.js
--rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.css
--rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.035884 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/
--rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
--rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.css
--rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.js
--rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.048827 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/
--rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
--rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.css
--rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.js
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.095394 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/
--rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
--rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
--rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
--rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/utils.js
--rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.2.1/globlocks/staticfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.163319 globlocks-1.2.1/globlocks/templates/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.162333 globlocks-1.2.1/globlocks/templates/globlocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.158851 globlocks-1.2.1/globlocks/templates/globlocks/blocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.158851 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.097609 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/heading/
--rw-rw-rw-   0        0        0      286 2024-03-30 23:26:30.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/heading/heading.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.118344 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/
--rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/full.html
--rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/large.html
--rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/medium.html
--rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/small.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.132573 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/
--rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image.html
--rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
--rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
--rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.135667 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/link/
--rw-rw-rw-   0        0        0     1655 2024-04-02 17:23:40.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/link/form.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.157593 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.145667 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/
--rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
--rw-rw-rw-   0        0        0      724 2024-04-03 12:55:15.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
--rw-rw-rw-   0        0        0      856 2024-03-29 20:27:49.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
--rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.149668 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/text/
--rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/text/text_block.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.187891 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/
--rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/heading.html
--rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
--rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/listblock.html
--rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/richtext.html
--rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/settings_form.html
--rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
--rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.161323 globlocks-1.2.1/globlocks/templates/globlocks/icons/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.207331 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/
--rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-center.svg
--rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-justify.svg
--rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-left.svg
--rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-right.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.249413 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/
--rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
--rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
--rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
--rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
--rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
--rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
--rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
--rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
--rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
--rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
--rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
--rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.161323 globlocks-1.2.1/globlocks/templates/globlocks/shared/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.264747 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/
--rw-rw-rw-   0        0        0      224 2024-03-29 13:43:14.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/base.html
--rw-rw-rw-   0        0        0      902 2024-03-29 23:02:43.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/heading.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.281050 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/
--rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/base.html
--rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/full.html
--rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/large.html
--rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/medium.html
--rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/small.html
--rw-rw-rw-   0        0        0      510 2024-03-29 14:23:54.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/listblock.html
--rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.309440 globlocks-1.2.1/globlocks/templates/globlocks/widgets/
--rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/color-input-widget.html
--rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/font_picker_widget.html
--rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/justify-widget-option.html
--rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/justify-widget.html
--rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/orderable_widget.html
--rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/slider_input.html
--rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/toolbar-widget.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.163319 globlocks-1.2.1/globlocks/templates/wagtailadmin/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.332813 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/
--rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block.html
--rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
--rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
--rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/field.html
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.335317 globlocks-1.2.1/globlocks/templatetags/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.337330 globlocks-1.2.1/globlocks/templatetags/__pycache__/
--rw-rw-rw-   0        0        0     4240 2024-03-28 09:30:53.000000 globlocks-1.2.1/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.356234 globlocks-1.2.1/globlocks/templatetags/globlocks/
--rw-rw-rw-   0        0        0     6660 2024-04-19 08:00:34.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.365883 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/
--rw-rw-rw-   0        0        0     9597 2024-03-29 13:53:59.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1452 2024-03-28 09:30:53.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
--rw-rw-rw-   0        0        0     3595 2024-03-28 09:30:53.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
--rw-rw-rw-   0        0        0     2569 2024-03-29 23:02:34.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/admin.py
--rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/toolbar.py
--rw-rw-rw-   0        0        0     3472 2024-03-29 23:02:32.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/utils.py
--rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templatetags/orderable_tags.py
--rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/tests.py
--rw-rw-rw-   0        0        0     1846 2024-03-30 16:43:10.000000 globlocks-1.2.1/globlocks/util.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.376194 globlocks-1.2.1/globlocks/wagtail_hooks/
--rw-rw-rw-   0        0        0       86 2024-03-26 16:56:56.000000 globlocks-1.2.1/globlocks/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/wagtail_hooks/admin_hooks.py
--rw-rw-rw-   0        0        0     4327 2024-04-15 15:46:53.000000 globlocks-1.2.1/globlocks/wagtail_hooks/alignment.py
--rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/wagtail_hooks/rt_extensions.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.388922 globlocks-1.2.1/globlocks/widgets/
--rw-rw-rw-   0        0        0      297 2024-03-26 16:31:57.000000 globlocks-1.2.1/globlocks/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/color_input_widget.py
--rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/fontpicker.py
--rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/justify_widget.py
--rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/orderable.py
--rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/range_input.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.406793 globlocks-1.2.1/globlocks.egg-info/
--rw-rw-rw-   0        0        0     2659 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11554 2024-04-19 08:02:47.000000 globlocks-1.2.1/globlocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2024-04-19 08:02:48.420998 globlocks-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.389920 globlocks-1.2.1/tests/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.392112 globlocks-1.2.1/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.394114 globlocks-1.2.1/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.395112 globlocks-1.2.1/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.403782 globlocks-1.2.1/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.979074 globlocks-1.2.2/
+-rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2659 2024-04-19 09:38:50.977073 globlocks-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1576 2024-04-19 07:39:45.000000 globlocks-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.824420 globlocks-1.2.2/globlocks/
+-rw-rw-rw-   0        0        0      620 2024-04-19 09:38:45.000000 globlocks-1.2.2/globlocks/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.895830 globlocks-1.2.2/globlocks/blocks/
+-rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.964910 globlocks-1.2.2/globlocks/blocks/bases/
+-rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/bases/__init__.py
+-rw-rw-rw-   0        0        0    13076 2024-04-19 08:02:15.000000 globlocks-1.2.2/globlocks/blocks/bases/baseblock.py
+-rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/bases/template.py
+-rw-rw-rw-   0        0        0    10194 2024-04-19 07:59:16.000000 globlocks-1.2.2/globlocks/blocks/bases/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.996477 globlocks-1.2.2/globlocks/blocks/block_fields/
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.019171 globlocks-1.2.2/globlocks/blocks/block_fields/colorblock/
+-rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/colorblock/__init__.py
+-rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/colorblock/colorblock.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.038637 globlocks-1.2.2/globlocks/blocks/block_fields/fontpicker/
+-rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/fontpicker/__init__.py
+-rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/fontpicker/fontpicker.py
+-rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/justify.py
+-rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/orderable_block.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.057492 globlocks-1.2.2/globlocks/blocks/block_fields/rangeslider/
+-rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/rangeslider/__init__.py
+-rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/rangeslider/rangeslider.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.123370 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/
+-rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-04-02 23:32:32.000000 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/bar.py
+-rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/element.py
+-rw-rw-rw-   0        0        0     3112 2024-04-02 23:34:11.000000 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/toolbar_field.py
+-rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
+-rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.183932 globlocks-1.2.2/globlocks/blocks/components/
+-rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/components/__init__.py
+-rw-rw-rw-   0        0        0     1653 2024-03-30 23:54:15.000000 globlocks-1.2.2/globlocks/blocks/components/heading.py
+-rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/components/image.py
+-rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/components/image_text.py
+-rw-rw-rw-   0        0        0     9072 2024-03-31 00:20:40.000000 globlocks-1.2.2/globlocks/blocks/components/link.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.204808 globlocks-1.2.2/globlocks/blocks/components/menus/
+-rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/components/menus/__init__.py
+-rw-rw-rw-   0        0        0     2772 2024-03-29 13:30:58.000000 globlocks-1.2.2/globlocks/blocks/components/menus/flat.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/components/menus/layered.py
+-rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/components/text.py
+-rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/blocks/richtext.py
+-rw-rw-rw-   0        0        0      756 2024-03-31 00:56:58.000000 globlocks-1.2.2/globlocks/blocks/utils.py
+-rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/choices.py
+-rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.249834 globlocks-1.2.2/globlocks/fields/
+-rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/fields/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/fields/colorfield.py
+-rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/fields/fontfield.py
+-rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/fields/orderablefield.py
+-rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/fonts.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.650373 globlocks-1.2.2/globlocks/locale/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.649393 globlocks-1.2.2/globlocks/locale/en/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.260428 globlocks-1.2.2/globlocks/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      380 2024-04-10 20:48:48.000000 globlocks-1.2.2/globlocks/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.650373 globlocks-1.2.2/globlocks/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.276634 globlocks-1.2.2/globlocks/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1420 2024-04-11 09:05:49.000000 globlocks-1.2.2/globlocks/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    11858 2024-04-11 09:04:54.000000 globlocks-1.2.2/globlocks/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/panels.py
+-rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/preview.py
+-rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/rt_extensions.py
+-rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.650373 globlocks-1.2.2/globlocks/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.653407 globlocks-1.2.2/globlocks/static/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.304672 globlocks-1.2.2/globlocks/static/globlocks/admin/
+-rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/admin/block_settings.js
+-rw-rw-rw-   0        0        0    24317 2024-04-02 17:24:43.000000 globlocks-1.2.2/globlocks/static/globlocks/admin/layout.css
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.361293 globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/
+-rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
+-rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
+-rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.384016 globlocks-1.2.2/globlocks/static/globlocks/css/
+-rw-rw-rw-   0        0        0     8918 2024-03-31 14:27:18.000000 globlocks-1.2.2/globlocks/static/globlocks/css/blocks.css
+-rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.2.2/globlocks/static/globlocks/css/bootstrap.css
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.835726 globlocks-1.2.2/globlocks/static/globlocks/fonts/
+-rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Acme-Regular.ttf
+-rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
+-rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
+-rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
+-rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
+-rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
+-rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
+-rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
+-rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
+-rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Inter-Regular.ttf
+-rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
+-rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
+-rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
+-rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
+-rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
+-rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
+-rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
+-rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
+-rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
+-rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
+-rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
+-rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
+-rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
+-rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
+-rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
+-rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
+-rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
+-rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
+-rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
+-rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
+-rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
+-rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
+-rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
+-rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
+-rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
+-rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
+-rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
+-rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.653294 globlocks-1.2.2/globlocks/static/globlocks/richtext/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.857980 globlocks-1.2.2/globlocks/static/globlocks/richtext/alignment/
+-rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/richtext/alignment/alignment.css
+-rw-rw-rw-   0        0        0     5728 2024-04-19 08:00:08.000000 globlocks-1.2.2/globlocks/static/globlocks/richtext/alignment/alignment.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.870611 globlocks-1.2.2/globlocks/static/globlocks/richtext/rt_extensions/
+-rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:49.883611 globlocks-1.2.2/globlocks/static/globlocks/widgets/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.014794 globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/
+-rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
+-rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:18.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
+-rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/pickr.css
+-rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/pickr.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.056412 globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/
+-rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
+-rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
+-rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/font-picker.css
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.091343 globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/
+-rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/justify-controller.js
+-rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/justify-widget.css
+-rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/justify-widget.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.167756 globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/
+-rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
+-rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/orderable.css
+-rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/orderable.js
+-rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.202568 globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/
+-rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
+-rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/range-slider.css
+-rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/range-slider.js
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.238806 globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/
+-rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
+-rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
+-rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
+-rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/static/globlocks/widgets/utils.js
+-rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.2.2/globlocks/staticfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.664395 globlocks-1.2.2/globlocks/templates/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.664395 globlocks-1.2.2/globlocks/templates/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.661416 globlocks-1.2.2/globlocks/templates/globlocks/blocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.660415 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.246812 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/heading/
+-rw-rw-rw-   0        0        0      286 2024-03-30 23:26:30.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/heading/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.276737 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image/
+-rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image/full.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image/large.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image/medium.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image/small.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.311401 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image_text/
+-rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image_text/image.html
+-rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
+-rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
+-rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image_text/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.324327 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/link/
+-rw-rw-rw-   0        0        0     1655 2024-04-02 17:23:40.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/link/form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.660415 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.357782 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/
+-rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
+-rw-rw-rw-   0        0        0      724 2024-04-03 12:55:15.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
+-rw-rw-rw-   0        0        0      856 2024-03-29 20:27:49.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
+-rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.366783 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/text/
+-rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/text/text_block.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.421444 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/
+-rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/heading.html
+-rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/listblock.html
+-rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/richtext.html
+-rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/settings_form.html
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
+-rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.662416 globlocks-1.2.2/globlocks/templates/globlocks/icons/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.488741 globlocks-1.2.2/globlocks/templates/globlocks/icons/text-align/
+-rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/text-align/text-center.svg
+-rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/text-align/text-justify.svg
+-rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/text-align/text-left.svg
+-rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/text-align/text-right.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.590775 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/
+-rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
+-rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
+-rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
+-rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
+-rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
+-rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
+-rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
+-rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
+-rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
+-rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
+-rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
+-rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.663389 globlocks-1.2.2/globlocks/templates/globlocks/shared/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.623361 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/
+-rw-rw-rw-   0        0        0      224 2024-03-29 13:43:14.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/base.html
+-rw-rw-rw-   0        0        0      902 2024-03-29 23:02:43.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.661895 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/images/
+-rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/images/base.html
+-rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/images/full.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/images/large.html
+-rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/images/medium.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/images/small.html
+-rw-rw-rw-   0        0        0      510 2024-03-29 14:23:54.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/listblock.html
+-rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.727338 globlocks-1.2.2/globlocks/templates/globlocks/widgets/
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/color-input-widget.html
+-rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/font_picker_widget.html
+-rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/justify-widget-option.html
+-rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/justify-widget.html
+-rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/orderable_widget.html
+-rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/slider_input.html
+-rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/globlocks/widgets/toolbar-widget.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:48.664395 globlocks-1.2.2/globlocks/templates/wagtailadmin/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.763540 globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/
+-rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/base_block.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
+-rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/field.html
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.774790 globlocks-1.2.2/globlocks/templatetags/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.776789 globlocks-1.2.2/globlocks/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0     4240 2024-03-28 09:30:53.000000 globlocks-1.2.2/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.824597 globlocks-1.2.2/globlocks/templatetags/globlocks/
+-rw-rw-rw-   0        0        0     6660 2024-04-19 08:00:34.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.836211 globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/
+-rw-rw-rw-   0        0        0     9563 2024-04-19 08:08:16.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1452 2024-03-28 09:30:53.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3595 2024-03-28 09:30:53.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2569 2024-03-29 23:02:34.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/admin.py
+-rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/toolbar.py
+-rw-rw-rw-   0        0        0     3472 2024-03-29 23:02:32.000000 globlocks-1.2.2/globlocks/templatetags/globlocks/utils.py
+-rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/templatetags/orderable_tags.py
+-rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/tests.py
+-rw-rw-rw-   0        0        0     1846 2024-03-30 16:43:10.000000 globlocks-1.2.2/globlocks/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.879782 globlocks-1.2.2/globlocks/wagtail_hooks/
+-rw-rw-rw-   0        0        0       86 2024-03-26 16:56:56.000000 globlocks-1.2.2/globlocks/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/wagtail_hooks/admin_hooks.py
+-rw-rw-rw-   0        0        0     6152 2024-04-19 09:37:40.000000 globlocks-1.2.2/globlocks/wagtail_hooks/alignment.py
+-rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/wagtail_hooks/rt_extensions.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.950088 globlocks-1.2.2/globlocks/widgets/
+-rw-rw-rw-   0        0        0      297 2024-03-26 16:31:57.000000 globlocks-1.2.2/globlocks/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/widgets/color_input_widget.py
+-rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/widgets/fontpicker.py
+-rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/widgets/justify_widget.py
+-rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/widgets/orderable.py
+-rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.2.2/globlocks/widgets/range_input.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.974076 globlocks-1.2.2/globlocks.egg-info/
+-rw-rw-rw-   0        0        0     2659 2024-04-19 09:38:48.000000 globlocks-1.2.2/globlocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11554 2024-04-19 09:38:48.000000 globlocks-1.2.2/globlocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:38:48.000000 globlocks-1.2.2/globlocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-19 09:38:48.000000 globlocks-1.2.2/globlocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 09:38:48.000000 globlocks-1.2.2/globlocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2024-04-19 09:38:50.989667 globlocks-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.951845 globlocks-1.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.954897 globlocks-1.2.2/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.958830 globlocks-1.2.2/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.960193 globlocks-1.2.2/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:38:50.970073 globlocks-1.2.2/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.2/tests/testapp/testapp/wsgi.py
```

### Comparing `globlocks-1.2.1/LICENSE` & `globlocks-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/PKG-INFO` & `globlocks-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globlocks
-Version: 1.2.1
+Version: 1.2.2
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/globlocks
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `globlocks-1.2.1/README.md` & `globlocks-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/__init__.py` & `globlocks-1.2.2/globlocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/__init__.py` & `globlocks-1.2.2/globlocks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/bases/baseblock.py` & `globlocks-1.2.2/globlocks/blocks/bases/baseblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/bases/template.py` & `globlocks-1.2.2/globlocks/blocks/bases/template.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/bases/visibility.py` & `globlocks-1.2.2/globlocks/blocks/bases/visibility.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/colorblock.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/colorblock/colorblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/fontpicker.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/fontpicker/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/justify.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/justify.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/orderable_block.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/orderable_block.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/rangeslider.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/rangeslider/rangeslider.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/__init__.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/bar.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/bar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/element.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/element.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_field.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/toolbar_field.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_widget.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/toolbar_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/tools.py` & `globlocks-1.2.2/globlocks/blocks/block_fields/toolbar/tools.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/components/heading.py` & `globlocks-1.2.2/globlocks/blocks/components/heading.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/components/image.py` & `globlocks-1.2.2/globlocks/blocks/components/image.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/components/image_text.py` & `globlocks-1.2.2/globlocks/blocks/components/image_text.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/components/link.py` & `globlocks-1.2.2/globlocks/blocks/components/link.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/components/menus/flat.py` & `globlocks-1.2.2/globlocks/blocks/components/menus/flat.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/components/text.py` & `globlocks-1.2.2/globlocks/blocks/components/text.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/richtext.py` & `globlocks-1.2.2/globlocks/blocks/richtext.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/blocks/utils.py` & `globlocks-1.2.2/globlocks/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/choices.py` & `globlocks-1.2.2/globlocks/choices.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/colors.py` & `globlocks-1.2.2/globlocks/colors.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/fields/fontfield.py` & `globlocks-1.2.2/globlocks/fields/fontfield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/fields/orderablefield.py` & `globlocks-1.2.2/globlocks/fields/orderablefield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/fonts.py` & `globlocks-1.2.2/globlocks/fonts.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/django.po` & `globlocks-1.2.2/globlocks/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/django.mo` & `globlocks-1.2.2/globlocks/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/django.po` & `globlocks-1.2.2/globlocks/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/panels.py` & `globlocks-1.2.2/globlocks/panels.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/preview.py` & `globlocks-1.2.2/globlocks/preview.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/rt_extensions.py` & `globlocks-1.2.2/globlocks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/settings.py` & `globlocks-1.2.2/globlocks/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/admin/block_settings.js` & `globlocks-1.2.2/globlocks/static/globlocks/admin/block_settings.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/admin/layout.css` & `globlocks-1.2.2/globlocks/static/globlocks/admin/layout.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js` & `globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css` & `globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js` & `globlocks-1.2.2/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/css/blocks.css` & `globlocks-1.2.2/globlocks/static/globlocks/css/blocks.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/css/bootstrap.css` & `globlocks-1.2.2/globlocks/static/globlocks/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Acme-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Acme-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Bangers-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Bangers-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Caveat-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Caveat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Creepster-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Creepster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Inter-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Inter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Kanit-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Lato-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Lobster-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Lobster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Manrope-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Monoton-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Monoton-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Oswald-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/PTMono-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/PTMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Phudu-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Phudu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Poppins-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Roboto-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Rubik-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Rubik-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Ultra-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Ultra-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf` & `globlocks-1.2.2/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.css` & `globlocks-1.2.2/globlocks/static/globlocks/richtext/alignment/alignment.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.js` & `globlocks-1.2.2/globlocks/static/globlocks/richtext/alignment/alignment.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js` & `globlocks-1.2.2/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/LICENSE` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/color-input-widget.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/color-input-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.css` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/pickr.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.min.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/color_input/pickr.min.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker.css` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/font_picker/font-picker.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-controller.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/justify-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.css` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/justify-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/justify/justify-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.css` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/orderable.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/orderable.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/sortable.min.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/orderable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.css` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/range-slider.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/range_slider/range-slider.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/static/globlocks/widgets/utils.js` & `globlocks-1.2.2/globlocks/static/globlocks/widgets/utils.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html` & `globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/link/form.html` & `globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/link/form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/item.html` & `globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/item.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html` & `globlocks-1.2.2/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-bold.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-bold.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h2.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h2.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h3.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h3.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h5.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h5.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h6.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-h6.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-palette.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg` & `globlocks-1.2.2/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/heading.html` & `globlocks-1.2.2/globlocks/templates/globlocks/shared/blocks/heading.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/widgets/font_picker_widget.html` & `globlocks-1.2.2/globlocks/templates/globlocks/widgets/font_picker_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/widgets/orderable_widget.html` & `globlocks-1.2.2/globlocks/templates/globlocks/widgets/orderable_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/widgets/slider_input.html` & `globlocks-1.2.2/globlocks/templates/globlocks/widgets/slider_input.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/globlocks/widgets/toolbar-widget.html` & `globlocks-1.2.2/globlocks/templates/globlocks/widgets/toolbar-widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block.html` & `globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/base_block.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/field.html` & `globlocks-1.2.2/globlocks/templates/wagtailadmin/block_forms/field.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc` & `globlocks-1.2.2/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/__init__.py` & `globlocks-1.2.2/globlocks/templatetags/globlocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc` & `globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,42 +1,42 @@
 magic:    0xa70d0d0a
-moddate:  0x68c70666 (Fri Mar 29 13:51:36 2024 UTC)
-files sz: 6679
+moddate:  0xa2242266 (Fri Apr 19 08:00:34 2024 UTC)
+files sz: 6660
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
       00640064036c056d065a060100640064046c076d085a080100640064056c
       096d0a5a0a0100640064066c0b6d0c5a0c0100640064076c0d6d0e5a0e01
-      00640064086c0f6d105a106d115a110100640064096c126d135a13010064
-      00640a6c146d155a156d165a1601006400640b6c176d185a186d195a1901
-      006400640c6c1a6d1b5a1b6d1c5a1c01006400640d6c1d6d1e5a1f6d205a
-      2101006400640e6c226d235a2301006400640f6c246d255a250100640064
-      106c265a260200650a6a270000000000000000a6000000ab000000000000
-      0000005a28641184005a296528a02a000000000000000000000000000000
-      000000000064126413ac14a6020000ab0200000000000000006427641684
-      01a6000000ab0000000000000000005a2b6417652c6602641884045a2d64
-      1984005a2e641a84005a2f641b5a3002006528a02a000000000000000000
-      000000000000000000000065306413ac14a6020000ab0200000000000000
-      000200652d651f6530652ea6030000ab030000000000000000a6010000ab
-      0100000000000000000100641c5a3102006528a02a000000000000000000
-      000000000000000000000065316413ac14a6020000ab0200000000000000
-      000200652d65216531652fa6030000ab030000000000000000a6010000ab
-      0100000000000000000100020065266a320000000000000000641da60100
-      00ab0100000000000000005a33650265256a340000000000000000651065
-      13653565016605190000000000000000005a366528a02a00000000000000
-      00000000000000000000000000641e6413ac14a6020000ab020000000000
-      0000006427641f65366420653764176535660664218405a6000000ab0000
-      000000000000005a380200470064228400642365046a3900000000000000
-      00a6030000ab0300000000000000005a3a6528a03b000000000000000000
-      00000000000000000000006424ac25a6010000ab01000000000000000064
-      268400a6000000ab0000000000000000005a3c64105300
+      00640064086c0f6d105a100100640064096c116d125a1201006400640a6c
+      136d145a146d155a1501006400640b6c166d175a176d185a180100640064
+      0c6c196d1a5a1a6d1b5a1b01006400640d6c1c6d1d5a1e6d1f5a20010064
+      00640e6c216d225a2201006400640f6c236d245a240100640064106c255a
+      250200650a6a260000000000000000a6000000ab0000000000000000005a
+      27641184005a286527a02900000000000000000000000000000000000000
+      0064126413ac14a6020000ab020000000000000000642764168401a60000
+      00ab0000000000000000005a2a6417652b6602641884045a2c641984005a
+      2d641a84005a2e641b5a2f02006527a02900000000000000000000000000
+      00000000000000652f6413ac14a6020000ab020000000000000000020065
+      2c651e652f652da6030000ab030000000000000000a6010000ab01000000
+      00000000000100641c5a3002006527a02900000000000000000000000000
+      0000000000000065306413ac14a6020000ab020000000000000000020065
+      2c65206530652ea6030000ab030000000000000000a6010000ab01000000
+      00000000000100020065256a310000000000000000641da6010000ab0100
+      000000000000005a32650265246a33000000000000000065106512653465
+      016605190000000000000000005a356527a0290000000000000000000000
+      000000000000000000641e6413ac14a6020000ab02000000000000000064
+      27641f65356420653664176534660664218405a6000000ab000000000000
+      0000005a370200470064228400642365046a380000000000000000a60300
+      00ab0300000000000000005a396527a03a00000000000000000000000000
+      000000000000006424ac25a6010000ab01000000000000000064268400a6
+      000000ab0000000000000000005a3b64105300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Any', 'Union'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Any)
                 10 STORE_NAME               1 (Any)
@@ -83,260 +83,258 @@
                 80 LOAD_CONST               7 (('static',))
                 82 IMPORT_NAME             13 (django.templatetags.static)
                 84 IMPORT_FROM             14 (static)
                 86 STORE_NAME              14 (static)
                 88 POP_TOP
    
      9          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               8 (('Page', 'PAGE_TEMPLATE_VAR'))
+                92 LOAD_CONST               8 (('Page',))
                 94 IMPORT_NAME             15 (wagtail.models)
                 96 IMPORT_FROM             16 (Page)
                 98 STORE_NAME              16 (Page)
-               100 IMPORT_FROM             17 (PAGE_TEMPLATE_VAR)
-               102 STORE_NAME              17 (PAGE_TEMPLATE_VAR)
-               104 POP_TOP
-   
-    10         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               9 (('AbstractDocument',))
-               110 IMPORT_NAME             18 (wagtail.documents.models)
-               112 IMPORT_FROM             19 (AbstractDocument)
-               114 STORE_NAME              19 (AbstractDocument)
-               116 POP_TOP
-   
-    11         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST              10 (('AbstractImage', 'AbstractRendition'))
-               122 IMPORT_NAME             20 (wagtail.images.models)
-               124 IMPORT_FROM             21 (AbstractImage)
-               126 STORE_NAME              21 (AbstractImage)
-               128 IMPORT_FROM             22 (AbstractRendition)
-               130 STORE_NAME              22 (AbstractRendition)
-               132 POP_TOP
-   
-    16         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST              11 (('PreviewUnavailable', 'preview_of_block'))
-               138 IMPORT_NAME             23 (globlocks.preview)
-               140 IMPORT_FROM             24 (PreviewUnavailable)
-               142 STORE_NAME              24 (PreviewUnavailable)
-               144 IMPORT_FROM             25 (preview_of_block)
-               146 STORE_NAME              25 (preview_of_block)
-               148 POP_TOP
-   
-    17         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST              12 (('GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG'))
-               154 IMPORT_NAME             26 (globlocks.settings)
-               156 IMPORT_FROM             27 (GLOBLOCKS_SCRIPT_INDENT)
-               158 STORE_NAME              27 (GLOBLOCKS_SCRIPT_INDENT)
-               160 IMPORT_FROM             28 (GLOBLOCKS_DEBUG)
-               162 STORE_NAME              28 (GLOBLOCKS_DEBUG)
-               164 POP_TOP
-   
-    18         166 LOAD_CONST               0 (0)
-               168 LOAD_CONST              13 (('globlocks_js', 'globlocks_css'))
-               170 IMPORT_NAME             29 (globlocks.staticfiles)
-               172 IMPORT_FROM             30 (globlocks_js)
-               174 STORE_NAME              31 (staticfiles_globlocks_js)
-               176 IMPORT_FROM             32 (globlocks_css)
-               178 STORE_NAME              33 (staticfiles_globlocks_css)
-               180 POP_TOP
-   
-    22         182 LOAD_CONST               0 (0)
-               184 LOAD_CONST              14 (('get_hooks',))
-               186 IMPORT_NAME             34 (globlocks.util)
-               188 IMPORT_FROM             35 (get_hooks)
-               190 STORE_NAME              35 (get_hooks)
-               192 POP_TOP
-   
-    25         194 LOAD_CONST               0 (0)
-               196 LOAD_CONST              15 (('components',))
-               198 IMPORT_NAME             36 (globlocks.blocks)
-               200 IMPORT_FROM             37 (components)
-               202 STORE_NAME              37 (components)
-               204 POP_TOP
-   
-    29         206 LOAD_CONST               0 (0)
-               208 LOAD_CONST              16 (None)
-               210 IMPORT_NAME             38 (re)
-               212 STORE_NAME              38 (re)
-   
-    32         214 PUSH_NULL
-               216 LOAD_NAME               10 (library)
-               218 LOAD_ATTR               39 (Library)
-               228 PRECALL                  0
-               232 CALL                     0
-               242 STORE_NAME              40 (register)
-   
-    35         244 LOAD_CONST              17 (<code object format_static_file, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 35>)
-               246 MAKE_FUNCTION            0
-               248 STORE_NAME              41 (format_static_file)
-   
-    44         250 LOAD_NAME               40 (register)
-               252 LOAD_METHOD             42 (simple_tag)
-               274 LOAD_CONST              18 ('render_as_preview')
-               276 LOAD_CONST              19 (True)
-               278 KW_NAMES                20
-               280 PRECALL                  2
-               284 CALL                     2
-   
-    45         294 LOAD_CONST              39 ((False,))
-               296 LOAD_CONST              22 (<code object render_as_preview, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 44>)
-               298 MAKE_FUNCTION            1 (defaults)
-   
-    44         300 PRECALL                  0
-               304 CALL                     0
-   
-    45         314 STORE_NAME              43 (render_as_preview)
-   
-    55         316 LOAD_CONST              23 ('return')
-               318 LOAD_NAME               44 (callable)
-               320 BUILD_TUPLE              2
-               322 LOAD_CONST              24 (<code object base_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 55>)
-               324 MAKE_FUNCTION            4 (annotations)
-               326 STORE_NAME              45 (base_script_tag)
-   
-    79         328 LOAD_CONST              25 (<code object format_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 79>)
-               330 MAKE_FUNCTION            0
-               332 STORE_NAME              46 (format_script_tag)
-   
-    82         334 LOAD_CONST              26 (<code object format_css_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 82>)
-               336 MAKE_FUNCTION            0
-               338 STORE_NAME              47 (format_css_tag)
-   
-    85         340 LOAD_CONST              27 ('globlocks_js')
-               342 STORE_NAME              48 (globlocks_js_hook_name)
-   
-    86         344 PUSH_NULL
-               346 LOAD_NAME               40 (register)
-               348 LOAD_METHOD             42 (simple_tag)
-               370 LOAD_NAME               48 (globlocks_js_hook_name)
-               372 LOAD_CONST              19 (True)
-               374 KW_NAMES                20
-               376 PRECALL                  2
-               380 CALL                     2
-   
-    87         390 PUSH_NULL
-               392 LOAD_NAME               45 (base_script_tag)
-               394 LOAD_NAME               31 (staticfiles_globlocks_js)
-               396 LOAD_NAME               48 (globlocks_js_hook_name)
-               398 LOAD_NAME               46 (format_script_tag)
-               400 PRECALL                  3
-               404 CALL                     3
-   
-    86         414 PRECALL                  1
-               418 CALL                     1
-               428 POP_TOP
-   
-    90         430 LOAD_CONST              28 ('globlocks_css')
-               432 STORE_NAME              49 (globlocks_css_hook_name)
-   
-    91         434 PUSH_NULL
-               436 LOAD_NAME               40 (register)
-               438 LOAD_METHOD             42 (simple_tag)
-               460 LOAD_NAME               49 (globlocks_css_hook_name)
-               462 LOAD_CONST              19 (True)
-               464 KW_NAMES                20
-               466 PRECALL                  2
-               470 CALL                     2
-   
-    92         480 PUSH_NULL
-               482 LOAD_NAME               45 (base_script_tag)
-               484 LOAD_NAME               33 (staticfiles_globlocks_css)
-               486 LOAD_NAME               49 (globlocks_css_hook_name)
-               488 LOAD_NAME               47 (format_css_tag)
-               490 PRECALL                  3
-               494 CALL                     3
-   
-    91         504 PRECALL                  1
-               508 CALL                     1
-               518 POP_TOP
-   
-    96         520 PUSH_NULL
-               522 LOAD_NAME               38 (re)
-               524 LOAD_ATTR               50 (compile)
-               534 LOAD_CONST              29 ('^[a-zA-Z0-9]+://')
-               536 PRECALL                  1
-               540 CALL                     1
-               550 STORE_NAME              51 (HAS_PROTO_RE)
-   
-    97         552 LOAD_NAME                2 (Union)
-   
-    98         554 LOAD_NAME               37 (components)
-               556 LOAD_ATTR               52 (LinkValue)
-   
-    99         566 LOAD_NAME               16 (Page)
-               568 LOAD_NAME               19 (AbstractDocument)
-   
-   100         570 LOAD_NAME               53 (str)
-               572 LOAD_NAME                1 (Any)
-   
-    98         574 BUILD_TUPLE              5
-   
-    97         576 BINARY_SUBSCR
-               586 STORE_NAME              54 (POSSIBLE_LINK_TYPES)
-   
-   104         588 LOAD_NAME               40 (register)
-               590 LOAD_METHOD             42 (simple_tag)
-               612 LOAD_CONST              30 ('link')
-               614 LOAD_CONST              19 (True)
-               616 KW_NAMES                20
-               618 PRECALL                  2
-               622 CALL                     2
-   
-   105         632 LOAD_CONST              39 ((False,))
-               634 LOAD_CONST              31 ('value')
-               636 LOAD_NAME               54 (POSSIBLE_LINK_TYPES)
-               638 LOAD_CONST              32 ('full')
-               640 LOAD_NAME               55 (bool)
-               642 LOAD_CONST              23 ('return')
-               644 LOAD_NAME               53 (str)
-               646 BUILD_TUPLE              6
-               648 LOAD_CONST              33 (<code object do_link, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 104>)
-               650 MAKE_FUNCTION            5 (defaults, annotations)
-   
-   104         652 PRECALL                  0
-               656 CALL                     0
-   
-   105         666 STORE_NAME              56 (do_link)
-   
-   147         668 PUSH_NULL
-               670 LOAD_BUILD_CLASS
-               672 LOAD_CONST              34 (<code object FragmentNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 147>)
-               674 MAKE_FUNCTION            0
-               676 LOAD_CONST              35 ('FragmentNode')
-               678 LOAD_NAME                4 (template)
-               680 LOAD_ATTR               57 (Node)
-               690 PRECALL                  3
-               694 CALL                     3
-               704 STORE_NAME              58 (FragmentNode)
-   
-   169         706 LOAD_NAME               40 (register)
-               708 LOAD_METHOD             59 (tag)
-               730 LOAD_CONST              36 ('block_fragment')
-               732 KW_NAMES                37
-               734 PRECALL                  1
-               738 CALL                     1
-   
-   170         748 LOAD_CONST              38 (<code object fragment, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 169>)
-               750 MAKE_FUNCTION            0
-   
-   169         752 PRECALL                  0
-               756 CALL                     0
-   
-   170         766 STORE_NAME              60 (fragment)
-               768 LOAD_CONST              16 (None)
-               770 RETURN_VALUE
+               100 POP_TOP
+   
+    10         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               9 (('AbstractDocument',))
+               106 IMPORT_NAME             17 (wagtail.documents.models)
+               108 IMPORT_FROM             18 (AbstractDocument)
+               110 STORE_NAME              18 (AbstractDocument)
+               112 POP_TOP
+   
+    11         114 LOAD_CONST               0 (0)
+               116 LOAD_CONST              10 (('AbstractImage', 'AbstractRendition'))
+               118 IMPORT_NAME             19 (wagtail.images.models)
+               120 IMPORT_FROM             20 (AbstractImage)
+               122 STORE_NAME              20 (AbstractImage)
+               124 IMPORT_FROM             21 (AbstractRendition)
+               126 STORE_NAME              21 (AbstractRendition)
+               128 POP_TOP
+   
+    16         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              11 (('PreviewUnavailable', 'preview_of_block'))
+               134 IMPORT_NAME             22 (globlocks.preview)
+               136 IMPORT_FROM             23 (PreviewUnavailable)
+               138 STORE_NAME              23 (PreviewUnavailable)
+               140 IMPORT_FROM             24 (preview_of_block)
+               142 STORE_NAME              24 (preview_of_block)
+               144 POP_TOP
+   
+    17         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST              12 (('GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG'))
+               150 IMPORT_NAME             25 (globlocks.settings)
+               152 IMPORT_FROM             26 (GLOBLOCKS_SCRIPT_INDENT)
+               154 STORE_NAME              26 (GLOBLOCKS_SCRIPT_INDENT)
+               156 IMPORT_FROM             27 (GLOBLOCKS_DEBUG)
+               158 STORE_NAME              27 (GLOBLOCKS_DEBUG)
+               160 POP_TOP
+   
+    18         162 LOAD_CONST               0 (0)
+               164 LOAD_CONST              13 (('globlocks_js', 'globlocks_css'))
+               166 IMPORT_NAME             28 (globlocks.staticfiles)
+               168 IMPORT_FROM             29 (globlocks_js)
+               170 STORE_NAME              30 (staticfiles_globlocks_js)
+               172 IMPORT_FROM             31 (globlocks_css)
+               174 STORE_NAME              32 (staticfiles_globlocks_css)
+               176 POP_TOP
+   
+    22         178 LOAD_CONST               0 (0)
+               180 LOAD_CONST              14 (('get_hooks',))
+               182 IMPORT_NAME             33 (globlocks.util)
+               184 IMPORT_FROM             34 (get_hooks)
+               186 STORE_NAME              34 (get_hooks)
+               188 POP_TOP
+   
+    25         190 LOAD_CONST               0 (0)
+               192 LOAD_CONST              15 (('components',))
+               194 IMPORT_NAME             35 (globlocks.blocks)
+               196 IMPORT_FROM             36 (components)
+               198 STORE_NAME              36 (components)
+               200 POP_TOP
+   
+    29         202 LOAD_CONST               0 (0)
+               204 LOAD_CONST              16 (None)
+               206 IMPORT_NAME             37 (re)
+               208 STORE_NAME              37 (re)
+   
+    32         210 PUSH_NULL
+               212 LOAD_NAME               10 (library)
+               214 LOAD_ATTR               38 (Library)
+               224 PRECALL                  0
+               228 CALL                     0
+               238 STORE_NAME              39 (register)
+   
+    35         240 LOAD_CONST              17 (<code object format_static_file, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 35>)
+               242 MAKE_FUNCTION            0
+               244 STORE_NAME              40 (format_static_file)
+   
+    44         246 LOAD_NAME               39 (register)
+               248 LOAD_METHOD             41 (simple_tag)
+               270 LOAD_CONST              18 ('render_as_preview')
+               272 LOAD_CONST              19 (True)
+               274 KW_NAMES                20
+               276 PRECALL                  2
+               280 CALL                     2
+   
+    45         290 LOAD_CONST              39 ((False,))
+               292 LOAD_CONST              22 (<code object render_as_preview, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 44>)
+               294 MAKE_FUNCTION            1 (defaults)
+   
+    44         296 PRECALL                  0
+               300 CALL                     0
+   
+    45         310 STORE_NAME              42 (render_as_preview)
+   
+    55         312 LOAD_CONST              23 ('return')
+               314 LOAD_NAME               43 (callable)
+               316 BUILD_TUPLE              2
+               318 LOAD_CONST              24 (<code object base_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 55>)
+               320 MAKE_FUNCTION            4 (annotations)
+               322 STORE_NAME              44 (base_script_tag)
+   
+    79         324 LOAD_CONST              25 (<code object format_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 79>)
+               326 MAKE_FUNCTION            0
+               328 STORE_NAME              45 (format_script_tag)
+   
+    82         330 LOAD_CONST              26 (<code object format_css_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 82>)
+               332 MAKE_FUNCTION            0
+               334 STORE_NAME              46 (format_css_tag)
+   
+    85         336 LOAD_CONST              27 ('globlocks_js')
+               338 STORE_NAME              47 (globlocks_js_hook_name)
+   
+    86         340 PUSH_NULL
+               342 LOAD_NAME               39 (register)
+               344 LOAD_METHOD             41 (simple_tag)
+               366 LOAD_NAME               47 (globlocks_js_hook_name)
+               368 LOAD_CONST              19 (True)
+               370 KW_NAMES                20
+               372 PRECALL                  2
+               376 CALL                     2
+   
+    87         386 PUSH_NULL
+               388 LOAD_NAME               44 (base_script_tag)
+               390 LOAD_NAME               30 (staticfiles_globlocks_js)
+               392 LOAD_NAME               47 (globlocks_js_hook_name)
+               394 LOAD_NAME               45 (format_script_tag)
+               396 PRECALL                  3
+               400 CALL                     3
+   
+    86         410 PRECALL                  1
+               414 CALL                     1
+               424 POP_TOP
+   
+    90         426 LOAD_CONST              28 ('globlocks_css')
+               428 STORE_NAME              48 (globlocks_css_hook_name)
+   
+    91         430 PUSH_NULL
+               432 LOAD_NAME               39 (register)
+               434 LOAD_METHOD             41 (simple_tag)
+               456 LOAD_NAME               48 (globlocks_css_hook_name)
+               458 LOAD_CONST              19 (True)
+               460 KW_NAMES                20
+               462 PRECALL                  2
+               466 CALL                     2
+   
+    92         476 PUSH_NULL
+               478 LOAD_NAME               44 (base_script_tag)
+               480 LOAD_NAME               32 (staticfiles_globlocks_css)
+               482 LOAD_NAME               48 (globlocks_css_hook_name)
+               484 LOAD_NAME               46 (format_css_tag)
+               486 PRECALL                  3
+               490 CALL                     3
+   
+    91         500 PRECALL                  1
+               504 CALL                     1
+               514 POP_TOP
+   
+    96         516 PUSH_NULL
+               518 LOAD_NAME               37 (re)
+               520 LOAD_ATTR               49 (compile)
+               530 LOAD_CONST              29 ('^[a-zA-Z0-9]+://')
+               532 PRECALL                  1
+               536 CALL                     1
+               546 STORE_NAME              50 (HAS_PROTO_RE)
+   
+    97         548 LOAD_NAME                2 (Union)
+   
+    98         550 LOAD_NAME               36 (components)
+               552 LOAD_ATTR               51 (LinkValue)
+   
+    99         562 LOAD_NAME               16 (Page)
+               564 LOAD_NAME               18 (AbstractDocument)
+   
+   100         566 LOAD_NAME               52 (str)
+               568 LOAD_NAME                1 (Any)
+   
+    98         570 BUILD_TUPLE              5
+   
+    97         572 BINARY_SUBSCR
+               582 STORE_NAME              53 (POSSIBLE_LINK_TYPES)
+   
+   104         584 LOAD_NAME               39 (register)
+               586 LOAD_METHOD             41 (simple_tag)
+               608 LOAD_CONST              30 ('link')
+               610 LOAD_CONST              19 (True)
+               612 KW_NAMES                20
+               614 PRECALL                  2
+               618 CALL                     2
+   
+   105         628 LOAD_CONST              39 ((False,))
+               630 LOAD_CONST              31 ('value')
+               632 LOAD_NAME               53 (POSSIBLE_LINK_TYPES)
+               634 LOAD_CONST              32 ('full')
+               636 LOAD_NAME               54 (bool)
+               638 LOAD_CONST              23 ('return')
+               640 LOAD_NAME               52 (str)
+               642 BUILD_TUPLE              6
+               644 LOAD_CONST              33 (<code object do_link, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 104>)
+               646 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   104         648 PRECALL                  0
+               652 CALL                     0
+   
+   105         662 STORE_NAME              55 (do_link)
+   
+   147         664 PUSH_NULL
+               666 LOAD_BUILD_CLASS
+               668 LOAD_CONST              34 (<code object FragmentNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 147>)
+               670 MAKE_FUNCTION            0
+               672 LOAD_CONST              35 ('FragmentNode')
+               674 LOAD_NAME                4 (template)
+               676 LOAD_ATTR               56 (Node)
+               686 PRECALL                  3
+               690 CALL                     3
+               700 STORE_NAME              57 (FragmentNode)
+   
+   169         702 LOAD_NAME               39 (register)
+               704 LOAD_METHOD             58 (tag)
+               726 LOAD_CONST              36 ('block_fragment')
+               728 KW_NAMES                37
+               730 PRECALL                  1
+               734 CALL                     1
+   
+   170         744 LOAD_CONST              38 (<code object fragment, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 169>)
+               746 MAKE_FUNCTION            0
+   
+   169         748 PRECALL                  0
+               752 CALL                     0
+   
+   170         762 STORE_NAME              59 (fragment)
+               764 LOAD_CONST              16 (None)
+               766 RETURN_VALUE
    consts
       0
       ('Any', 'Union')
       ('template',)
       ('reverse',)
       ('HttpRequest',)
       ('library',)
       ('mark_safe',)
       ('static',)
-      ('Page', 'PAGE_TEMPLATE_VAR')
+      ('Page',)
       ('AbstractDocument',)
       ('AbstractImage', 'AbstractRendition')
       ('PreviewUnavailable', 'preview_of_block')
       ('GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG')
       ('globlocks_js', 'globlocks_css')
       ('get_hooks',)
       ('components',)
@@ -1165,19 +1163,19 @@
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'fragment'
          firstlineno 169
          lnotab 0x021d0402020130012a012c0112010e01280106fd08050802
       (False,)
-   names      ('typing', 'Any', 'Union', 'django', 'template', 'django.urls', 'reverse', 'django.http', 'HttpRequest', 'django.template', 'library', 'django.utils.safestring', 'mark_safe', 'django.templatetags.static', 'static', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'wagtail.documents.models', 'AbstractDocument', 'wagtail.images.models', 'AbstractImage', 'AbstractRendition', 'globlocks.preview', 'PreviewUnavailable', 'preview_of_block', 'globlocks.settings', 'GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG', 'globlocks.staticfiles', 'globlocks_js', 'staticfiles_globlocks_js', 'globlocks_css', 'staticfiles_globlocks_css', 'globlocks.util', 'get_hooks', 'globlocks.blocks', 'components', 're', 'Library', 'register', 'format_static_file', 'simple_tag', 'render_as_preview', 'callable', 'base_script_tag', 'format_script_tag', 'format_css_tag', 'globlocks_js_hook_name', 'globlocks_css_hook_name', 'compile', 'HAS_PROTO_RE', 'LinkValue', 'str', 'POSSIBLE_LINK_TYPES', 'bool', 'do_link', 'Node', 'FragmentNode', 'tag', 'fragment')
+   names      ('typing', 'Any', 'Union', 'django', 'template', 'django.urls', 'reverse', 'django.http', 'HttpRequest', 'django.template', 'library', 'django.utils.safestring', 'mark_safe', 'django.templatetags.static', 'static', 'wagtail.models', 'Page', 'wagtail.documents.models', 'AbstractDocument', 'wagtail.images.models', 'AbstractImage', 'AbstractRendition', 'globlocks.preview', 'PreviewUnavailable', 'preview_of_block', 'globlocks.settings', 'GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG', 'globlocks.staticfiles', 'globlocks_js', 'staticfiles_globlocks_js', 'globlocks_css', 'staticfiles_globlocks_css', 'globlocks.util', 'get_hooks', 'globlocks.blocks', 'components', 're', 'Library', 'register', 'format_static_file', 'simple_tag', 'render_as_preview', 'callable', 'base_script_tag', 'format_script_tag', 'format_css_tag', 'globlocks_js_hook_name', 'globlocks_css_hook_name', 'compile', 'HAS_PROTO_RE', 'LinkValue', 'str', 'POSSIBLE_LINK_TYPES', 'bool', 'do_link', 'Node', 'FragmentNode', 'tag', 'fragment')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c010c010c010c010c010c0210010c0110051001100110
+      0x00ff020110010c010c010c010c010c010c020c010c0110051001100110
       040c030c0408031e0306092c0106ff0e01020a0c180603060304012e0118
       ff100404012e0118ff1005200102010c01040104fe02ff0c072c0114ff0e
       01022a26162a0104ff0e01
```

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc` & `globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc` & `globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc` & `globlocks-1.2.2/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/admin.py` & `globlocks-1.2.2/globlocks/templatetags/globlocks/admin.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/toolbar.py` & `globlocks-1.2.2/globlocks/templatetags/globlocks/toolbar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/globlocks/utils.py` & `globlocks-1.2.2/globlocks/templatetags/globlocks/utils.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/templatetags/orderable_tags.py` & `globlocks-1.2.2/globlocks/templatetags/orderable_tags.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/util.py` & `globlocks-1.2.2/globlocks/util.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/wagtail_hooks/icons.py` & `globlocks-1.2.2/globlocks/wagtail_hooks/icons.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/wagtail_hooks/rt_extensions.py` & `globlocks-1.2.2/globlocks/wagtail_hooks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/widgets/color_input_widget.py` & `globlocks-1.2.2/globlocks/widgets/color_input_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/widgets/fontpicker.py` & `globlocks-1.2.2/globlocks/widgets/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/widgets/justify_widget.py` & `globlocks-1.2.2/globlocks/widgets/justify_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/widgets/orderable.py` & `globlocks-1.2.2/globlocks/widgets/orderable.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks/widgets/range_input.py` & `globlocks-1.2.2/globlocks/widgets/range_input.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/globlocks.egg-info/PKG-INFO` & `globlocks-1.2.2/globlocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globlocks
-Version: 1.2.1
+Version: 1.2.2
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/globlocks
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `globlocks-1.2.1/globlocks.egg-info/SOURCES.txt` & `globlocks-1.2.2/globlocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/setup.cfg` & `globlocks-1.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6c6f 626c 6f63 6b73 0d0a 7665   = globlocks..ve
-00000020: 7273 696f 6e20 3d20 312e 322e 310d 0a64  rsion = 1.2.1..d
+00000020: 7273 696f 6e20 3d20 312e 322e 320d 0a64  rsion = 1.2.2..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2041 6e20  escription = An 
 00000040: 6170 706c 6963 6174 696f 6e20 6d61 6465  application made
 00000050: 2066 6f72 2074 6865 2044 6a61 6e67 6f20   for the Django 
 00000060: 5765 6220 4672 616d 6577 6f72 6b2e 0d0a  Web Framework...
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
```

### Comparing `globlocks-1.2.1/tests/testapp/manage.py` & `globlocks-1.2.2/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/tests/testapp/testapp/settings.py` & `globlocks-1.2.2/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.1/tests/testapp/testapp/urls.py` & `globlocks-1.2.2/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

