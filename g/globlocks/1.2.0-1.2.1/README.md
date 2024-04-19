# Comparing `tmp/globlocks-1.2.0.tar.gz` & `tmp/globlocks-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globlocks-1.2.0.tar", last modified: Fri Apr 19 07:16:01 2024, max compression
+gzip compressed data, was "globlocks-1.2.1.tar", last modified: Fri Apr 19 08:02:48 2024, max compression
```

## Comparing `globlocks-1.2.0.tar` & `globlocks-1.2.1.tar`

### file list

```diff
@@ -1,294 +1,296 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.752883 globlocks-1.2.0/
--rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1984 2024-04-19 07:16:01.752883 globlocks-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      901 2024-03-19 08:19:55.000000 globlocks-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.134495 globlocks-1.2.0/globlocks/
--rw-rw-rw-   0        0        0      620 2024-04-19 07:15:55.000000 globlocks-1.2.0/globlocks/__init__.py
--rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.217225 globlocks-1.2.0/globlocks/blocks/
--rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.282814 globlocks-1.2.0/globlocks/blocks/bases/
--rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/__init__.py
--rw-rw-rw-   0        0        0    13076 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/baseblock.py
--rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/template.py
--rw-rw-rw-   0        0        0    10194 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.310955 globlocks-1.2.0/globlocks/blocks/block_fields/
--rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.337348 globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/
--rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/__init__.py
--rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/colorblock.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.361510 globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/
--rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/__init__.py
--rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/fontpicker.py
--rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/justify.py
--rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/orderable_block.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.386291 globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/
--rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/__init__.py
--rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/rangeslider.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.459339 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/
--rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/__init__.py
--rw-rw-rw-   0        0        0     4956 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/bar.py
--rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/element.py
--rw-rw-rw-   0        0        0      774 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_field.py
--rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
--rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.529148 globlocks-1.2.0/globlocks/blocks/components/
--rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/__init__.py
--rw-rw-rw-   0        0        0     1603 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/heading.py
--rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/image.py
--rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/image_text.py
--rw-rw-rw-   0        0        0     9047 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/link.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.554771 globlocks-1.2.0/globlocks/blocks/components/menus/
--rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/menus/__init__.py
--rw-rw-rw-   0        0        0     2567 2024-03-19 09:11:52.000000 globlocks-1.2.0/globlocks/blocks/components/menus/flat.py
--rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/menus/layered.py
--rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/text.py
--rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/richtext.py
--rw-rw-rw-   0        0        0      425 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/utils.py
--rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/choices.py
--rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/colors.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.594099 globlocks-1.2.0/globlocks/fields/
--rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/__init__.py
--rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/colorfield.py
--rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/fontfield.py
--rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/orderablefield.py
--rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fonts.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.935293 globlocks-1.2.0/globlocks/locale/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.933577 globlocks-1.2.0/globlocks/locale/en/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.605504 globlocks-1.2.0/globlocks/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.935293 globlocks-1.2.0/globlocks/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.610601 globlocks-1.2.0/globlocks/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3549 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/panels.py
--rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/preview.py
--rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/rt_extensions.py
--rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.937305 globlocks-1.2.0/globlocks/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.940609 globlocks-1.2.0/globlocks/static/globlocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.639915 globlocks-1.2.0/globlocks/static/globlocks/admin/
--rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/block_settings.js
--rw-rw-rw-   0        0        0    24293 2024-03-26 09:23:48.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/layout.css
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.688688 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/
--rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
--rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
--rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.706876 globlocks-1.2.0/globlocks/static/globlocks/css/
--rw-rw-rw-   0        0        0     8847 2024-03-19 12:00:45.000000 globlocks-1.2.0/globlocks/static/globlocks/css/blocks.css
--rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.2.0/globlocks/static/globlocks/css/bootstrap.css
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.200251 globlocks-1.2.0/globlocks/static/globlocks/fonts/
--rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Acme-Regular.ttf
--rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
--rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
--rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
--rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
--rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
--rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
--rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
--rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
--rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Inter-Regular.ttf
--rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
--rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
--rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Lato-Regular.ttf
--rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
--rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
--rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
--rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
--rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
--rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
--rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
--rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
--rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
--rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
--rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
--rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
--rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
--rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
--rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
--rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
--rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
--rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
--rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
--rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
--rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
--rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
--rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
--rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
--rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
--rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.940609 globlocks-1.2.0/globlocks/static/globlocks/richtext/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.239068 globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/
--rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.css
--rw-rw-rw-   0        0        0     5728 2024-04-19 07:10:50.000000 globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.257279 globlocks-1.2.0/globlocks/static/globlocks/richtext/rt_extensions/
--rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.275789 globlocks-1.2.0/globlocks/static/globlocks/widgets/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.433244 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/
--rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/LICENSE
--rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
--rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:49.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
--rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.css
--rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.483286 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/
--rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
--rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
--rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker.css
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.533371 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/
--rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-controller.js
--rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.css
--rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.633022 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/
--rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
--rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.css
--rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.js
--rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.704619 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/
--rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
--rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.css
--rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.758651 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/
--rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
--rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
--rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
--rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/utils.js
--rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.2.0/globlocks/staticfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.955478 globlocks-1.2.0/globlocks/templates/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.955478 globlocks-1.2.0/globlocks/templates/globlocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.950029 globlocks-1.2.0/globlocks/templates/globlocks/blocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.949054 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.770710 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/heading/
--rw-rw-rw-   0        0        0      257 2024-03-19 10:10:04.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/heading/heading.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.809821 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/
--rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/full.html
--rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/large.html
--rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/medium.html
--rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/small.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.860553 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/
--rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image.html
--rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
--rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
--rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.870458 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/link/
--rw-rw-rw-   0        0        0     1655 2024-03-19 08:35:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/link/form.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.943691 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.923598 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/
--rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
--rw-rw-rw-   0        0        0      555 2024-03-19 10:14:53.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
--rw-rw-rw-   0        0        0      908 2024-03-19 10:29:01.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
--rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.938210 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/text/
--rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/text/text_block.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.015092 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/
--rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/heading.html
--rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
--rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/listblock.html
--rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/richtext.html
--rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/settings_form.html
--rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
--rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.953021 globlocks-1.2.0/globlocks/templates/globlocks/icons/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.064990 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/
--rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-center.svg
--rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-justify.svg
--rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-left.svg
--rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-right.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.191760 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/
--rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
--rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
--rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
--rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
--rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
--rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
--rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
--rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
--rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
--rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
--rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
--rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.954018 globlocks-1.2.0/globlocks/templates/globlocks/shared/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.238160 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/
--rw-rw-rw-   0        0        0      226 2024-03-19 09:32:33.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/base.html
--rw-rw-rw-   0        0        0      902 2024-03-19 09:26:20.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/heading.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.292489 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/
--rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/base.html
--rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/full.html
--rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/large.html
--rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/medium.html
--rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/small.html
--rw-rw-rw-   0        0        0      309 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/listblock.html
--rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.374821 globlocks-1.2.0/globlocks/templates/globlocks/widgets/
--rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/color-input-widget.html
--rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/font_picker_widget.html
--rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/justify-widget-option.html
--rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/justify-widget.html
--rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/orderable_widget.html
--rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/slider_input.html
--rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/toolbar-widget.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.955478 globlocks-1.2.0/globlocks/templates/wagtailadmin/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.418912 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/
--rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block.html
--rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
--rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
--rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/field.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.433614 globlocks-1.2.0/globlocks/templatetags/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.435567 globlocks-1.2.0/globlocks/templatetags/__pycache__/
--rw-rw-rw-   0        0        0     4257 2024-03-19 07:31:29.000000 globlocks-1.2.0/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.492902 globlocks-1.2.0/globlocks/templatetags/globlocks/
--rw-rw-rw-   0        0        0     6627 2024-03-19 09:43:06.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.506522 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/
--rw-rw-rw-   0        0        0     9504 2024-03-19 09:43:08.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1469 2024-03-19 07:31:29.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
--rw-rw-rw-   0        0        0     3595 2024-03-19 11:12:51.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
--rw-rw-rw-   0        0        0     2281 2024-03-19 09:18:19.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/admin.py
--rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/toolbar.py
--rw-rw-rw-   0        0        0     1242 2024-03-19 09:18:17.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/utils.py
--rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templatetags/orderable_tags.py
--rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/tests.py
--rw-rw-rw-   0        0        0     1832 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/util.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.576413 globlocks-1.2.0/globlocks/wagtail_hooks/
--rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/admin_hooks.py
--rw-rw-rw-   0        0        0     4327 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/alignment.py
--rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/rt_extensions.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.667055 globlocks-1.2.0/globlocks/widgets/
--rw-rw-rw-   0        0        0      295 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/color_input_widget.py
--rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/fontpicker.py
--rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/justify_widget.py
--rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/orderable.py
--rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/range_input.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.748890 globlocks-1.2.0/globlocks.egg-info/
--rw-rw-rw-   0        0        0     1984 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11470 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2024-04-19 07:16:01.764573 globlocks-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.667989 globlocks-1.2.0/tests/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.682543 globlocks-1.2.0/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.692248 globlocks-1.2.0/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.692248 globlocks-1.2.0/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.742891 globlocks-1.2.0/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.408782 globlocks-1.2.1/
+-rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2659 2024-04-19 08:02:48.408782 globlocks-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1576 2024-04-19 07:39:45.000000 globlocks-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.192867 globlocks-1.2.1/globlocks/
+-rw-rw-rw-   0        0        0      620 2024-04-19 08:02:43.000000 globlocks-1.2.1/globlocks/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.238693 globlocks-1.2.1/globlocks/blocks/
+-rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.255287 globlocks-1.2.1/globlocks/blocks/bases/
+-rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/bases/__init__.py
+-rw-rw-rw-   0        0        0    13076 2024-04-19 08:02:15.000000 globlocks-1.2.1/globlocks/blocks/bases/baseblock.py
+-rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/bases/template.py
+-rw-rw-rw-   0        0        0    10194 2024-04-19 07:59:16.000000 globlocks-1.2.1/globlocks/blocks/bases/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.258434 globlocks-1.2.1/globlocks/blocks/block_fields/
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.261244 globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/
+-rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/__init__.py
+-rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/colorblock.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.263894 globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/
+-rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/__init__.py
+-rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/fontpicker.py
+-rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/justify.py
+-rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/orderable_block.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.266008 globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/
+-rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/__init__.py
+-rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/rangeslider.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.275294 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/
+-rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-04-02 23:32:32.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/bar.py
+-rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/element.py
+-rw-rw-rw-   0        0        0     3112 2024-04-02 23:34:11.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_field.py
+-rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
+-rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.281865 globlocks-1.2.1/globlocks/blocks/components/
+-rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/__init__.py
+-rw-rw-rw-   0        0        0     1653 2024-03-30 23:54:15.000000 globlocks-1.2.1/globlocks/blocks/components/heading.py
+-rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/image.py
+-rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/image_text.py
+-rw-rw-rw-   0        0        0     9072 2024-03-31 00:20:40.000000 globlocks-1.2.1/globlocks/blocks/components/link.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.287360 globlocks-1.2.1/globlocks/blocks/components/menus/
+-rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/menus/__init__.py
+-rw-rw-rw-   0        0        0     2772 2024-03-29 13:30:58.000000 globlocks-1.2.1/globlocks/blocks/components/menus/flat.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/menus/layered.py
+-rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/components/text.py
+-rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/blocks/richtext.py
+-rw-rw-rw-   0        0        0      756 2024-03-31 00:56:58.000000 globlocks-1.2.1/globlocks/blocks/utils.py
+-rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/choices.py
+-rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.292357 globlocks-1.2.1/globlocks/fields/
+-rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/colorfield.py
+-rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/fontfield.py
+-rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fields/orderablefield.py
+-rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/fonts.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.142275 globlocks-1.2.1/globlocks/locale/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.142275 globlocks-1.2.1/globlocks/locale/en/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.304451 globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      380 2024-04-10 20:48:48.000000 globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.142275 globlocks-1.2.1/globlocks/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.324015 globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1420 2024-04-11 09:05:49.000000 globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    11858 2024-04-11 09:04:54.000000 globlocks-1.2.1/globlocks/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/panels.py
+-rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/preview.py
+-rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/rt_extensions.py
+-rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.143282 globlocks-1.2.1/globlocks/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.146974 globlocks-1.2.1/globlocks/static/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.326925 globlocks-1.2.1/globlocks/static/globlocks/admin/
+-rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/block_settings.js
+-rw-rw-rw-   0        0        0    24317 2024-04-02 17:24:43.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/layout.css
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.353694 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/
+-rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
+-rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
+-rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.364819 globlocks-1.2.1/globlocks/static/globlocks/css/
+-rw-rw-rw-   0        0        0     8918 2024-03-31 14:27:18.000000 globlocks-1.2.1/globlocks/static/globlocks/css/blocks.css
+-rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.2.1/globlocks/static/globlocks/css/bootstrap.css
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.857289 globlocks-1.2.1/globlocks/static/globlocks/fonts/
+-rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Acme-Regular.ttf
+-rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
+-rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
+-rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
+-rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
+-rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
+-rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
+-rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
+-rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
+-rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Inter-Regular.ttf
+-rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
+-rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
+-rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
+-rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
+-rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
+-rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
+-rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
+-rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
+-rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
+-rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
+-rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
+-rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
+-rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
+-rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
+-rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
+-rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
+-rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
+-rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
+-rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
+-rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
+-rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
+-rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
+-rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
+-rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
+-rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
+-rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
+-rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
+-rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.145975 globlocks-1.2.1/globlocks/static/globlocks/richtext/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.880300 globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/
+-rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.css
+-rw-rw-rw-   0        0        0     5728 2024-04-19 08:00:08.000000 globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.883252 globlocks-1.2.1/globlocks/static/globlocks/richtext/rt_extensions/
+-rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.886250 globlocks-1.2.1/globlocks/static/globlocks/widgets/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.958534 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/
+-rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
+-rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:18.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
+-rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.css
+-rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.976913 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/
+-rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
+-rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
+-rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker.css
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.985641 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/
+-rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-controller.js
+-rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.css
+-rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.035884 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/
+-rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
+-rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.css
+-rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.js
+-rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.048827 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/
+-rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
+-rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.css
+-rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.js
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.095394 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/
+-rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
+-rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
+-rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
+-rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/static/globlocks/widgets/utils.js
+-rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.2.1/globlocks/staticfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.163319 globlocks-1.2.1/globlocks/templates/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.162333 globlocks-1.2.1/globlocks/templates/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.158851 globlocks-1.2.1/globlocks/templates/globlocks/blocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.158851 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.097609 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/heading/
+-rw-rw-rw-   0        0        0      286 2024-03-30 23:26:30.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/heading/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.118344 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/
+-rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/full.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/large.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/medium.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image/small.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.132573 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/
+-rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image.html
+-rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
+-rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
+-rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.135667 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/link/
+-rw-rw-rw-   0        0        0     1655 2024-04-02 17:23:40.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/link/form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.157593 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.145667 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/
+-rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
+-rw-rw-rw-   0        0        0      724 2024-04-03 12:55:15.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
+-rw-rw-rw-   0        0        0      856 2024-03-29 20:27:49.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
+-rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.149668 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/text/
+-rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/text/text_block.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.187891 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/
+-rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/heading.html
+-rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/listblock.html
+-rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/richtext.html
+-rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/settings_form.html
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
+-rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.161323 globlocks-1.2.1/globlocks/templates/globlocks/icons/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.207331 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/
+-rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-center.svg
+-rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-justify.svg
+-rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-left.svg
+-rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/text-align/text-right.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.249413 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/
+-rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
+-rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
+-rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
+-rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
+-rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
+-rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
+-rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
+-rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
+-rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
+-rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
+-rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
+-rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.161323 globlocks-1.2.1/globlocks/templates/globlocks/shared/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.264747 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/
+-rw-rw-rw-   0        0        0      224 2024-03-29 13:43:14.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/base.html
+-rw-rw-rw-   0        0        0      902 2024-03-29 23:02:43.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.281050 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/
+-rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/base.html
+-rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/full.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/large.html
+-rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/medium.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/images/small.html
+-rw-rw-rw-   0        0        0      510 2024-03-29 14:23:54.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/listblock.html
+-rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.309440 globlocks-1.2.1/globlocks/templates/globlocks/widgets/
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/color-input-widget.html
+-rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/font_picker_widget.html
+-rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/justify-widget-option.html
+-rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/justify-widget.html
+-rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/orderable_widget.html
+-rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/slider_input.html
+-rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/globlocks/widgets/toolbar-widget.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:47.163319 globlocks-1.2.1/globlocks/templates/wagtailadmin/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.332813 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/
+-rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
+-rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/field.html
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.335317 globlocks-1.2.1/globlocks/templatetags/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.337330 globlocks-1.2.1/globlocks/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0     4240 2024-03-28 09:30:53.000000 globlocks-1.2.1/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.356234 globlocks-1.2.1/globlocks/templatetags/globlocks/
+-rw-rw-rw-   0        0        0     6660 2024-04-19 08:00:34.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.365883 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/
+-rw-rw-rw-   0        0        0     9597 2024-03-29 13:53:59.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1452 2024-03-28 09:30:53.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3595 2024-03-28 09:30:53.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2569 2024-03-29 23:02:34.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/admin.py
+-rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/toolbar.py
+-rw-rw-rw-   0        0        0     3472 2024-03-29 23:02:32.000000 globlocks-1.2.1/globlocks/templatetags/globlocks/utils.py
+-rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/templatetags/orderable_tags.py
+-rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/tests.py
+-rw-rw-rw-   0        0        0     1846 2024-03-30 16:43:10.000000 globlocks-1.2.1/globlocks/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.376194 globlocks-1.2.1/globlocks/wagtail_hooks/
+-rw-rw-rw-   0        0        0       86 2024-03-26 16:56:56.000000 globlocks-1.2.1/globlocks/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/wagtail_hooks/admin_hooks.py
+-rw-rw-rw-   0        0        0     4327 2024-04-15 15:46:53.000000 globlocks-1.2.1/globlocks/wagtail_hooks/alignment.py
+-rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/wagtail_hooks/rt_extensions.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.388922 globlocks-1.2.1/globlocks/widgets/
+-rw-rw-rw-   0        0        0      297 2024-03-26 16:31:57.000000 globlocks-1.2.1/globlocks/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/color_input_widget.py
+-rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/fontpicker.py
+-rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/justify_widget.py
+-rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/orderable.py
+-rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.2.1/globlocks/widgets/range_input.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.406793 globlocks-1.2.1/globlocks.egg-info/
+-rw-rw-rw-   0        0        0     2659 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11554 2024-04-19 08:02:47.000000 globlocks-1.2.1/globlocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 08:02:46.000000 globlocks-1.2.1/globlocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2024-04-19 08:02:48.420998 globlocks-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.389920 globlocks-1.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.392112 globlocks-1.2.1/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.394114 globlocks-1.2.1/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.395112 globlocks-1.2.1/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:02:48.403782 globlocks-1.2.1/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.1/tests/testapp/testapp/wsgi.py
```

### Comparing `globlocks-1.2.0/LICENSE` & `globlocks-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/PKG-INFO` & `globlocks-1.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globlocks
-Version: 1.2.0
+Version: 1.2.1
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/globlocks
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -65,7 +65,34 @@
    INSTALLED_APPS = [
        ...,
        'globlocks',
        'conditional_field',
    ]
    ```
 2. ...
+
+## Richtext Alignment
+
+`globlocks` has a richtext feature for text alignment; without the limits that feature would normally impose.
+
+*Normally* - headings would not be able to get aligned. **This is a problem.**
+
+Luckily, we have the solution! *And you can use it too!*
+
+**To add the alignment features to your richtext**
+
+1. Follow the installation steps for `globlocks`.
+2. Add `text-alignment` to your richtext features. (it is included in default features)
+
+To align it on the frontend too; add the following CSS:
+
+```css
+.text-left {
+    text-align: left;
+}
+.text-center{
+    text-align: center;
+}
+.text-right {
+    text-align: right;
+}
+```
```

### Comparing `globlocks-1.2.0/globlocks/__init__.py` & `globlocks-1.2.1/globlocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/__init__.py` & `globlocks-1.2.1/globlocks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/bases/baseblock.py` & `globlocks-1.2.1/globlocks/blocks/bases/baseblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/bases/template.py` & `globlocks-1.2.1/globlocks/blocks/bases/template.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/bases/visibility.py` & `globlocks-1.2.1/globlocks/blocks/bases/visibility.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/colorblock.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/colorblock/colorblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/fontpicker.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/fontpicker/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/justify.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/justify.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/orderable_block.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/orderable_block.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/rangeslider.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/rangeslider/rangeslider.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/__init__.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/element.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/element.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_widget.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/toolbar_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/tools.py` & `globlocks-1.2.1/globlocks/blocks/block_fields/toolbar/tools.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/components/heading.py` & `globlocks-1.2.1/globlocks/blocks/components/heading.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,21 @@
 class Heading(ToggleableBlock):
     advanced_settings_class = HeadingConfiguration
 
     heading = blocks.CharBlock(
         required=True,
         help_text=_("The heading of the block."),
         form_classname="title",
+        max_length=100,
     )
 
     subheading = blocks.CharBlock(
         required=False,
         help_text=_("The subheading of the block."),
+        max_length=100,
     )
 
     class Meta:
         group=_("Text")
         icon = "title"
         label = _("Heading")
         label_format = _("Heading: {heading}")
```

### Comparing `globlocks-1.2.0/globlocks/blocks/components/image.py` & `globlocks-1.2.1/globlocks/blocks/components/image.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/components/image_text.py` & `globlocks-1.2.1/globlocks/blocks/components/image_text.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/components/link.py` & `globlocks-1.2.1/globlocks/blocks/components/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
         "no_row_padding",
     ]
 
     # (Optional) text for the link.
     text = CharBlockWithAttrs(
         required=False,
         label=_("Text"),
+        max_length=255,
         attrs={
             "placeholder": _("A short description of the link (optional)"),
             "autocomplete": "off",
         },
     )
 
     # Placeholder for the choice block
```

### Comparing `globlocks-1.2.0/globlocks/blocks/components/menus/flat.py` & `globlocks-1.2.1/globlocks/blocks/components/menus/flat.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     ]
 
     image = ImageChooserBlock(
         required=False,
         help_text=_("An image to display with the menu item."),
         classname=make_classname(
             SHOW(1, "custom_template"),
+
+            # Which parent element do we want to search for our handler?
+            # This is useful for traveling up the DOM tree to find the
+            # parent element that contains the handler.
             parent_queryselector("class", "globlocks-showable-block")
         )
     )
 
     link = Link(
         help_text=_("Where do you want to link to?"),
         features=ALLOWED_FEATURES,
```

### Comparing `globlocks-1.2.0/globlocks/blocks/components/text.py` & `globlocks-1.2.1/globlocks/blocks/components/text.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/blocks/richtext.py` & `globlocks-1.2.1/globlocks/blocks/richtext.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/choices.py` & `globlocks-1.2.1/globlocks/choices.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/colors.py` & `globlocks-1.2.1/globlocks/colors.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/fields/fontfield.py` & `globlocks-1.2.1/globlocks/fields/fontfield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/fields/orderablefield.py` & `globlocks-1.2.1/globlocks/fields/orderablefield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/fonts.py` & `globlocks-1.2.1/globlocks/fonts.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/locale/en/LC_MESSAGES/django.po` & `globlocks-1.2.1/globlocks/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/panels.py` & `globlocks-1.2.1/globlocks/panels.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/preview.py` & `globlocks-1.2.1/globlocks/preview.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/rt_extensions.py` & `globlocks-1.2.1/globlocks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/settings.py` & `globlocks-1.2.1/globlocks/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/admin/block_settings.js` & `globlocks-1.2.1/globlocks/static/globlocks/admin/block_settings.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/admin/layout.css` & `globlocks-1.2.1/globlocks/static/globlocks/admin/layout.css`

 * *Files 0% similar despite different names*

```diff
@@ -376,25 +376,25 @@
   }
 }
 @media (min-width: 1400px) {
   .container-xxl, .container-xl, .container-lg, .container-md, .container-sm, .container {
     max-width: 1320px;
   }
 }
-.row {
+#wagtail .row {
   --bs-gutter-x: 1.5rem;
   --bs-gutter-y: 0;
   display: flex;
   flex-wrap: wrap;
   margin-top: calc(-1 * var(--bs-gutter-y));
   margin-bottom: calc(var(--bs-gutter-y));
 }
-.row > * {
+#wagtail .row > * {
   flex-shrink: 0;
-  width: 100%;
+  /* width: 100%; */
   max-width: 100%;
   padding-right: calc(var(--bs-gutter-x) * 0.5);
   padding-left: calc(var(--bs-gutter-x) * 0.5);
   margin-top: var(--bs-gutter-y);
 }
 
 .col {
```

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js` & `globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css` & `globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js` & `globlocks-1.2.1/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/css/blocks.css` & `globlocks-1.2.1/globlocks/static/globlocks/css/blocks.css`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     --globlocks-danger-saturation: 100%;
     --globlocks-danger-lightness: 50%;
     --globlocks-danger-button: #ffffff;
     --globlocks-danger-button-bg: hsl(var(--globlocks-danger-hue), calc(var(--globlocks-danger-saturation) - 10%), calc(var(--globlocks-danger-lightness) + 10%));
     
 }
 
+.globlocks-edit-icon {
+    margin-right: 0.25em;
+    display: inline-block;
+}
+
 
 .globlocks-styles {
     color: var(--globlocks-text-color);
     font-family: 'Arial', sans-serif;
     font-size: 1em;
     line-height: 1.3;
     background-color: #f5f5f5;
@@ -269,15 +274,14 @@
     --globlocks-items: var(--globlocks-item-count);
 }
 .globlocks-menu-horizontal {
 
 }
 .globlocks-menu-horizontal .globlocks-menu__items {
     display: flex;
-    gap: 1em;
 }
 .globlocks-menu-vertical {
 
 }
 .globlocks-menu-vertical .globlocks-menu__items {
     display: flex;
     flex-direction: column;
@@ -287,14 +291,14 @@
 
 }
 .globlocks-menu-item__link__image {
 
 }
 .globlocks-menu-item__link__image img {
     width: 100%;
-    height: auto;
-    max-width: 20rem;
+    height: 10rem;
+    object-fit: cover;
 }
 .globlocks-menu-item__link__title {
     text-decoration: none;
 }
```

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/css/bootstrap.css` & `globlocks-1.2.1/globlocks/static/globlocks/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Acme-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Acme-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Bangers-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Bangers-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Caveat-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Caveat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Creepster-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Creepster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Inter-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Inter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Kanit-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Lato-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Lobster-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Lobster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Manrope-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Monoton-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Monoton-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Oswald-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/PTMono-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/PTMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Phudu-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Phudu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Poppins-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Roboto-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Rubik-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Rubik-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Ultra-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Ultra-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf` & `globlocks-1.2.1/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.css` & `globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.js` & `globlocks-1.2.1/globlocks/static/globlocks/richtext/alignment/alignment.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js` & `globlocks-1.2.1/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/LICENSE` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/color-input-widget.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/color-input-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.css` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.min.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/color_input/pickr.min.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker.css` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/font_picker/font-picker.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-controller.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.css` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/justify/justify-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.css` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/orderable.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/sortable.min.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/orderable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.css` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/range_slider/range-slider.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/static/globlocks/widgets/utils.js` & `globlocks-1.2.1/globlocks/static/globlocks/widgets/utils.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html` & `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/link/form.html` & `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/link/form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/item.html` & `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/item.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-{% load wagtailimages_tags globlocks %}
-<div class="globlocks-menu-item">
-    <a href="{% link self.link %}" class="globlocks-menu-item__link">
-        {% if show_image and self.image %}
-            <div class="globlocks-menu-item__link__image">
-                {% image self.image original as self_image %}
-                <img src="{{ self_image.url }}" alt="{{ self.title }}">
+{% load wagtailimages_tags globlocks fedit %}
+{% fedit_block block_id=block.id show_image=show_image %}
+    <div data-block-id="{{ block_id }}" class="globlocks-menu-item">
+        <a href="{% link self.link %}" class="globlocks-menu-item__link">
+            {% if show_image and self.image %}
+                <div class="globlocks-menu-item__link__image">
+                    {% image self.image original as self_image %}
+                    <img src="{{ self_image.url }}" alt="{{ self.title }}">
+                </div>
+            {% endif %}
+            <div class="globlocks-menu-item__link__title">
+                {{ self.link.link_text }}
             </div>
-        {% endif %}
-        <div class="globlocks-menu-item__link__title">
-            {{ self.link.link_text }}
-        </div>
-    </a>
-</div>
+        </a>
+    </div>
+{% unfedit_block %}
```

#### html2text {}

```diff
@@ -1,5 +1,7 @@
-{% load wagtailimages_tags globlocks %}
+{% load wagtailimages_tags globlocks fedit %} {% fedit_block block_id=block.id
+show_image=show_image %}
 _{_%_ _i_f_ _s_h_o_w___i_m_a_g_e_ _a_n_d_ _s_e_l_f_._i_m_a_g_e_ _%_}
 _{_%_ _i_m_a_g_e_ _s_e_l_f_._i_m_a_g_e_ _o_r_i_g_i_n_a_l_ _a_s_ _s_e_l_f___i_m_a_g_e_ _%_}_[_{_{_ _s_e_l_f_._t_i_t_l_e_ _}_}_]
 _{_%_ _e_n_d_i_f_ _%_}
 _{_{_ _s_e_l_f_._l_i_n_k_._l_i_n_k___t_e_x_t_ _}_}
+{% unfedit_block %}
```

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html` & `globlocks-1.2.1/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 {% extends "globlocks/shared/blocks/base.html" %}
 
-{% load globlocks wagtailcore_tags %}
+{% load wagtailcore_tags %}
 
 {% block classname %}globlocks-listblock globlocks-menu globlocks-menu-{% block direction %}{% endblock %} text-{{ self.settings.alignment }}{% endblock %}
 
 {% block block_attributes %}style="--item-count:{{ self.items|length }};"{% endblock %}
 
 {% block content %}
-    {% block_fragment as menu_items %}
-        
-    {% endblock_fragment %}
     <div class="globlocks-menu__header__wrapper">
-        {% include "globlocks/shared/blocks/heading.html" with tagname="h2" classname="globlocks-menu__header" title=self.title subtitle=self.subtitle|richtext %}
+        {% include "globlocks/shared/blocks/heading.html" with block_id=block_id tagname="h2" classname="globlocks-menu__header" title=self.title subtitle=self.subtitle|richtext %}
     </div>
     <div class="globlocks-menu__items {% block items_class %}{% endblock %}">
-        {% for item in self.items %}{% block menu_items %}{% include_block item with block_id=item.id %}{% endblock %}{% endfor %}
+        {% for item in self.items.bound_blocks %}{% block menu_items %}{% include_block item.value with block_id=item.id %}{% endblock %}{% endfor %}
     </div>
 {% endblock %}
```

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-bold.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-bold.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h2.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h2.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h3.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h3.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h5.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h5.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h6.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-h6.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-palette.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg` & `globlocks-1.2.1/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/heading.html` & `globlocks-1.2.1/globlocks/templates/globlocks/shared/blocks/heading.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/widgets/font_picker_widget.html` & `globlocks-1.2.1/globlocks/templates/globlocks/widgets/font_picker_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/widgets/orderable_widget.html` & `globlocks-1.2.1/globlocks/templates/globlocks/widgets/orderable_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/widgets/slider_input.html` & `globlocks-1.2.1/globlocks/templates/globlocks/widgets/slider_input.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/globlocks/widgets/toolbar-widget.html` & `globlocks-1.2.1/globlocks/templates/globlocks/widgets/toolbar-widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block.html` & `globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/field.html` & `globlocks-1.2.1/globlocks/templates/wagtailadmin/block_forms/field.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc` & `globlocks-1.2.1/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -39,15 +39,15 @@
                 40 STORE_NAME               4 (_CENTER)
    
      8          42 LOAD_CONST               3 (1)
                 44 STORE_NAME               5 (_RIGHT)
    
     10          46 PUSH_NULL
                 48 LOAD_BUILD_CLASS
-                50 LOAD_CONST               4 (<code object _Position, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 10>)
+                50 LOAD_CONST               4 (<code object _Position, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 10>)
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
-               186 LOAD_CONST               9 (<code object position_is, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 67>)
+               186 LOAD_CONST               9 (<code object position_is, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 67>)
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
-               256 LOAD_CONST              13 (<code object position_of, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 83>)
+               256 LOAD_CONST              13 (<code object position_of, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 83>)
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
-                      20 LOAD_CONST               2 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 11>)
+                      20 LOAD_CONST               2 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 11>)
                       22 MAKE_FUNCTION            5 (defaults, annotations)
                       24 STORE_NAME               5 (__init__)
          
-          14          26 LOAD_CONST               3 (<code object __str__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 14>)
+          14          26 LOAD_CONST               3 (<code object __str__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 14>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               6 (__str__)
          
-          23          32 LOAD_CONST               4 (<code object __int__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 23>)
+          23          32 LOAD_CONST               4 (<code object __int__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 23>)
                       34 MAKE_FUNCTION            0
                       36 STORE_NAME               7 (__int__)
          
-          26          38 LOAD_CONST               5 (<code object __eq__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 26>)
+          26          38 LOAD_CONST               5 (<code object __eq__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 26>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME               8 (__eq__)
          
-          35          44 LOAD_CONST               6 (<code object __gt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 35>)
+          35          44 LOAD_CONST               6 (<code object __gt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 35>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               9 (__gt__)
          
-          42          50 LOAD_CONST               7 (<code object __lt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 42>)
+          42          50 LOAD_CONST               7 (<code object __lt__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 42>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME              10 (__lt__)
          
-          49          56 LOAD_CONST               8 (<code object __ge__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 49>)
+          49          56 LOAD_CONST               8 (<code object __ge__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 49>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME              11 (__ge__)
          
-          56          62 LOAD_CONST               9 (<code object __le__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/orderable_tags.py", line 56>)
+          56          62 LOAD_CONST               9 (<code object __le__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\orderable_tags.py", line 56>)
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
                name       '__le__'
                firstlineno 56
                lnotab 0x02012a0116012a012001
             None
          names      ('__name__', '__module__', '__qualname__', '_CENTER', 'int', '__init__', '__str__', '__int__', '__eq__', '__gt__', '__lt__', '__ge__', '__le__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
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
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
          name       'position_of'
          firstlineno 83
          lnotab 0x02022c012c01
       None
    names      ('django.template', 'Library', 'register', '_LEFT', '_CENTER', '_RIGHT', '_Position', 'Left', 'Center', 'Right', 'filter', 'position_is', 'simple_tag', 'position_of')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/orderable_tags.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\orderable_tags.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0314020401040104021a351601160116022a010aff0e0102
       0f2c010aff0e01
```

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/__init__.py` & `globlocks-1.2.1/globlocks/templatetags/globlocks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Union
 from django import template
+from django.urls import reverse
 from django.http import HttpRequest
 from django.template import library
 from django.utils.safestring import mark_safe
 from django.templatetags.static import static
 
 from wagtail.models import Page
 from wagtail.documents.models import AbstractDocument
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-from typing import Any, Union from django import template from django.http
-import HttpRequest from django.template import library from
-django.utils.safestring import mark_safe from django.templatetags.static import
-static from wagtail.models import Page from wagtail.documents.models import
-AbstractDocument from wagtail.images.models import ( AbstractImage,
-AbstractRendition, ) from globlocks.preview import PreviewUnavailable,
-preview_of_block from globlocks.settings import GLOBLOCKS_SCRIPT_INDENT,
-GLOBLOCKS_DEBUG from globlocks.staticfiles import ( globlocks_js as
-staticfiles_globlocks_js, globlocks_css as staticfiles_globlocks_css, ) from
-globlocks.util import ( get_hooks, ) from globlocks.blocks import ( components,
-) import re register = library.Library() def format_static_file(file): for
-prefix in ["/", "http://", "https://"]: if file.startswith(prefix): return file
-return static(file) @register.simple_tag(name="render_as_preview",
-takes_context=True) def render_as_preview(context, block, fail_silently=False,
-**kwargs): try: v = preview_of_block(block, context,
-fail_silently=fail_silently, **kwargs) if v is None: return "" return v except
-PreviewUnavailable: return block def base_script_tag(files_or_hook, hook_name,
-format_fn) -> callable: def _tag(context): request = context.get("request",
-None) s = [] files = files_or_hook files = ( *files, *get_hooks(hook_name), )
-for file in files: if callable(file): file = file(request, context) if hasattr
-(file, "__html__"): s.append(file.__html__()) else: s.append(format_fn(file))
-return mark_safe(f"\n{GLOBLOCKS_SCRIPT_INDENT}".join(s)) return _tag def
-format_script_tag(file): return f'
+from typing import Any, Union from django import template from django.urls
+import reverse from django.http import HttpRequest from django.template import
+library from django.utils.safestring import mark_safe from
+django.templatetags.static import static from wagtail.models import Page from
+wagtail.documents.models import AbstractDocument from wagtail.images.models
+import ( AbstractImage, AbstractRendition, ) from globlocks.preview import
+PreviewUnavailable, preview_of_block from globlocks.settings import
+GLOBLOCKS_SCRIPT_INDENT, GLOBLOCKS_DEBUG from globlocks.staticfiles import
+( globlocks_js as staticfiles_globlocks_js, globlocks_css as
+staticfiles_globlocks_css, ) from globlocks.util import ( get_hooks, ) from
+globlocks.blocks import ( components, ) import re register = library.Library()
+def format_static_file(file): for prefix in ["/", "http://", "https://"]: if
+file.startswith(prefix): return file return static(file) @register.simple_tag
+(name="render_as_preview", takes_context=True) def render_as_preview(context,
+block, fail_silently=False, **kwargs): try: v = preview_of_block(block,
+context, fail_silently=fail_silently, **kwargs) if v is None: return "" return
+v except PreviewUnavailable: return block def base_script_tag(files_or_hook,
+hook_name, format_fn) -> callable: def _tag(context): request = context.get
+("request", None) s = [] files = files_or_hook files = ( *files, *get_hooks
+(hook_name), ) for file in files: if callable(file): file = file(request,
+context) if hasattr(file, "__html__"): s.append(file.__html__()) else: s.append
+(format_fn(file)) return mark_safe(f"\n{GLOBLOCKS_SCRIPT_INDENT}".join(s))
+return _tag def format_script_tag(file): return f'
 ' def format_css_tag(file): return f'
 ' globlocks_js_hook_name = "globlocks_js" register.simple_tag
 (name=globlocks_js_hook_name, takes_context=True)( base_script_tag
 (staticfiles_globlocks_js, globlocks_js_hook_name, format_script_tag) )
 globlocks_css_hook_name = "globlocks_css" register.simple_tag
 (name=globlocks_css_hook_name, takes_context=True)( base_script_tag
 (staticfiles_globlocks_css, globlocks_css_hook_name, format_css_tag) )
```

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc` & `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,42 +1,42 @@
 magic:    0xa70d0d0a
-moddate:  0x2a5ef965 (Tue Mar 19 09:43:06 2024 UTC)
-files sz: 6627
+moddate:  0x68c70666 (Fri Mar 29 13:51:36 2024 UTC)
+files sz: 6679
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
       00640064036c056d065a060100640064046c076d085a080100640064056c
       096d0a5a0a0100640064066c0b6d0c5a0c0100640064076c0d6d0e5a0e01
-      00640064086c0f6d105a100100640064096c116d125a126d135a13010064
+      00640064086c0f6d105a106d115a110100640064096c126d135a13010064
       00640a6c146d155a156d165a1601006400640b6c176d185a186d195a1901
-      006400640c6c1a6d1b5a1c6d1d5a1e01006400640d6c1f6d205a20010064
-      00640e6c216d225a2201006400640f6c235a23020065086a240000000000
-      000000a6000000ab0000000000000000005a25641084005a266525a02700
-      0000000000000000000000000000000000000064116412ac13a6020000ab
-      020000000000000000642664158401a6000000ab0000000000000000005a
-      28641665296602641784045a2a641884005a2b641984005a2c641a5a2d02
-      006525a0270000000000000000000000000000000000000000652d6412ac
-      13a6020000ab0200000000000000000200652a651c652d652ba6030000ab
-      030000000000000000a6010000ab0100000000000000000100641b5a2e02
-      006525a0270000000000000000000000000000000000000000652e6412ac
-      13a6020000ab0200000000000000000200652a651e652e652ca6030000ab
-      030000000000000000a6010000ab0100000000000000000100020065236a
-      2f0000000000000000641ca6010000ab0100000000000000005a30650265
-      226a310000000000000000650e6510653265016605190000000000000000
-      005a336525a0270000000000000000000000000000000000000000641d64
-      12ac13a6020000ab0200000000000000006426641e6533641f6534641665
-      32660664208405a6000000ab0000000000000000005a3502004700642184
-      00642265046a360000000000000000a6030000ab0300000000000000005a
-      376525a03800000000000000000000000000000000000000006423ac24a6
-      010000ab01000000000000000064258400a6000000ab0000000000000000
-      005a39640f5300
+      006400640c6c1a6d1b5a1b6d1c5a1c01006400640d6c1d6d1e5a1f6d205a
+      2101006400640e6c226d235a2301006400640f6c246d255a250100640064
+      106c265a260200650a6a270000000000000000a6000000ab000000000000
+      0000005a28641184005a296528a02a000000000000000000000000000000
+      000000000064126413ac14a6020000ab0200000000000000006427641684
+      01a6000000ab0000000000000000005a2b6417652c6602641884045a2d64
+      1984005a2e641a84005a2f641b5a3002006528a02a000000000000000000
+      000000000000000000000065306413ac14a6020000ab0200000000000000
+      000200652d651f6530652ea6030000ab030000000000000000a6010000ab
+      0100000000000000000100641c5a3102006528a02a000000000000000000
+      000000000000000000000065316413ac14a6020000ab0200000000000000
+      000200652d65216531652fa6030000ab030000000000000000a6010000ab
+      0100000000000000000100020065266a320000000000000000641da60100
+      00ab0100000000000000005a33650265256a340000000000000000651065
+      13653565016605190000000000000000005a366528a02a00000000000000
+      00000000000000000000000000641e6413ac14a6020000ab020000000000
+      0000006427641f65366420653764176535660664218405a6000000ab0000
+      000000000000005a380200470064228400642365046a3900000000000000
+      00a6030000ab0300000000000000005a3a6528a03b000000000000000000
+      00000000000000000000006424ac25a6010000ab01000000000000000064
+      268400a6000000ab0000000000000000005a3c64105300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Any', 'Union'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Any)
                 10 STORE_NAME               1 (Any)
@@ -48,285 +48,295 @@
                 20 LOAD_CONST               2 (('template',))
                 22 IMPORT_NAME              3 (django)
                 24 IMPORT_FROM              4 (template)
                 26 STORE_NAME               4 (template)
                 28 POP_TOP
    
      3          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('HttpRequest',))
-                34 IMPORT_NAME              5 (django.http)
-                36 IMPORT_FROM              6 (HttpRequest)
-                38 STORE_NAME               6 (HttpRequest)
+                32 LOAD_CONST               3 (('reverse',))
+                34 IMPORT_NAME              5 (django.urls)
+                36 IMPORT_FROM              6 (reverse)
+                38 STORE_NAME               6 (reverse)
                 40 POP_TOP
    
      4          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('library',))
-                46 IMPORT_NAME              7 (django.template)
-                48 IMPORT_FROM              8 (library)
-                50 STORE_NAME               8 (library)
+                44 LOAD_CONST               4 (('HttpRequest',))
+                46 IMPORT_NAME              7 (django.http)
+                48 IMPORT_FROM              8 (HttpRequest)
+                50 STORE_NAME               8 (HttpRequest)
                 52 POP_TOP
    
      5          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               5 (('mark_safe',))
-                58 IMPORT_NAME              9 (django.utils.safestring)
-                60 IMPORT_FROM             10 (mark_safe)
-                62 STORE_NAME              10 (mark_safe)
+                56 LOAD_CONST               5 (('library',))
+                58 IMPORT_NAME              9 (django.template)
+                60 IMPORT_FROM             10 (library)
+                62 STORE_NAME              10 (library)
                 64 POP_TOP
    
      6          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               6 (('static',))
-                70 IMPORT_NAME             11 (django.templatetags.static)
-                72 IMPORT_FROM             12 (static)
-                74 STORE_NAME              12 (static)
+                68 LOAD_CONST               6 (('mark_safe',))
+                70 IMPORT_NAME             11 (django.utils.safestring)
+                72 IMPORT_FROM             12 (mark_safe)
+                74 STORE_NAME              12 (mark_safe)
                 76 POP_TOP
    
-     8          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               7 (('Page',))
-                82 IMPORT_NAME             13 (wagtail.models)
-                84 IMPORT_FROM             14 (Page)
-                86 STORE_NAME              14 (Page)
+     7          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               7 (('static',))
+                82 IMPORT_NAME             13 (django.templatetags.static)
+                84 IMPORT_FROM             14 (static)
+                86 STORE_NAME              14 (static)
                 88 POP_TOP
    
      9          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               8 (('AbstractDocument',))
-                94 IMPORT_NAME             15 (wagtail.documents.models)
-                96 IMPORT_FROM             16 (AbstractDocument)
-                98 STORE_NAME              16 (AbstractDocument)
-               100 POP_TOP
-   
-    10         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               9 (('AbstractImage', 'AbstractRendition'))
-               106 IMPORT_NAME             17 (wagtail.images.models)
-               108 IMPORT_FROM             18 (AbstractImage)
-               110 STORE_NAME              18 (AbstractImage)
-               112 IMPORT_FROM             19 (AbstractRendition)
-               114 STORE_NAME              19 (AbstractRendition)
+                92 LOAD_CONST               8 (('Page', 'PAGE_TEMPLATE_VAR'))
+                94 IMPORT_NAME             15 (wagtail.models)
+                96 IMPORT_FROM             16 (Page)
+                98 STORE_NAME              16 (Page)
+               100 IMPORT_FROM             17 (PAGE_TEMPLATE_VAR)
+               102 STORE_NAME              17 (PAGE_TEMPLATE_VAR)
+               104 POP_TOP
+   
+    10         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               9 (('AbstractDocument',))
+               110 IMPORT_NAME             18 (wagtail.documents.models)
+               112 IMPORT_FROM             19 (AbstractDocument)
+               114 STORE_NAME              19 (AbstractDocument)
                116 POP_TOP
    
-    15         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST              10 (('PreviewUnavailable', 'preview_of_block'))
-               122 IMPORT_NAME             20 (globlocks.preview)
-               124 IMPORT_FROM             21 (PreviewUnavailable)
-               126 STORE_NAME              21 (PreviewUnavailable)
-               128 IMPORT_FROM             22 (preview_of_block)
-               130 STORE_NAME              22 (preview_of_block)
+    11         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST              10 (('AbstractImage', 'AbstractRendition'))
+               122 IMPORT_NAME             20 (wagtail.images.models)
+               124 IMPORT_FROM             21 (AbstractImage)
+               126 STORE_NAME              21 (AbstractImage)
+               128 IMPORT_FROM             22 (AbstractRendition)
+               130 STORE_NAME              22 (AbstractRendition)
                132 POP_TOP
    
     16         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST              11 (('GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG'))
-               138 IMPORT_NAME             23 (globlocks.settings)
-               140 IMPORT_FROM             24 (GLOBLOCKS_SCRIPT_INDENT)
-               142 STORE_NAME              24 (GLOBLOCKS_SCRIPT_INDENT)
-               144 IMPORT_FROM             25 (GLOBLOCKS_DEBUG)
-               146 STORE_NAME              25 (GLOBLOCKS_DEBUG)
+               136 LOAD_CONST              11 (('PreviewUnavailable', 'preview_of_block'))
+               138 IMPORT_NAME             23 (globlocks.preview)
+               140 IMPORT_FROM             24 (PreviewUnavailable)
+               142 STORE_NAME              24 (PreviewUnavailable)
+               144 IMPORT_FROM             25 (preview_of_block)
+               146 STORE_NAME              25 (preview_of_block)
                148 POP_TOP
    
     17         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST              12 (('globlocks_js', 'globlocks_css'))
-               154 IMPORT_NAME             26 (globlocks.staticfiles)
-               156 IMPORT_FROM             27 (globlocks_js)
-               158 STORE_NAME              28 (staticfiles_globlocks_js)
-               160 IMPORT_FROM             29 (globlocks_css)
-               162 STORE_NAME              30 (staticfiles_globlocks_css)
+               152 LOAD_CONST              12 (('GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG'))
+               154 IMPORT_NAME             26 (globlocks.settings)
+               156 IMPORT_FROM             27 (GLOBLOCKS_SCRIPT_INDENT)
+               158 STORE_NAME              27 (GLOBLOCKS_SCRIPT_INDENT)
+               160 IMPORT_FROM             28 (GLOBLOCKS_DEBUG)
+               162 STORE_NAME              28 (GLOBLOCKS_DEBUG)
                164 POP_TOP
    
-    21         166 LOAD_CONST               0 (0)
-               168 LOAD_CONST              13 (('get_hooks',))
-               170 IMPORT_NAME             31 (globlocks.util)
-               172 IMPORT_FROM             32 (get_hooks)
-               174 STORE_NAME              32 (get_hooks)
-               176 POP_TOP
-   
-    24         178 LOAD_CONST               0 (0)
-               180 LOAD_CONST              14 (('components',))
-               182 IMPORT_NAME             33 (globlocks.blocks)
-               184 IMPORT_FROM             34 (components)
-               186 STORE_NAME              34 (components)
-               188 POP_TOP
-   
-    28         190 LOAD_CONST               0 (0)
-               192 LOAD_CONST              15 (None)
-               194 IMPORT_NAME             35 (re)
-               196 STORE_NAME              35 (re)
-   
-    31         198 PUSH_NULL
-               200 LOAD_NAME                8 (library)
-               202 LOAD_ATTR               36 (Library)
-               212 PRECALL                  0
-               216 CALL                     0
-               226 STORE_NAME              37 (register)
-   
-    34         228 LOAD_CONST              16 (<code object format_static_file, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 34>)
-               230 MAKE_FUNCTION            0
-               232 STORE_NAME              38 (format_static_file)
-   
-    43         234 LOAD_NAME               37 (register)
-               236 LOAD_METHOD             39 (simple_tag)
-               258 LOAD_CONST              17 ('render_as_preview')
-               260 LOAD_CONST              18 (True)
-               262 KW_NAMES                19
-               264 PRECALL                  2
-               268 CALL                     2
-   
-    44         278 LOAD_CONST              38 ((False,))
-               280 LOAD_CONST              21 (<code object render_as_preview, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 43>)
-               282 MAKE_FUNCTION            1 (defaults)
-   
-    43         284 PRECALL                  0
-               288 CALL                     0
-   
-    44         298 STORE_NAME              40 (render_as_preview)
-   
-    54         300 LOAD_CONST              22 ('return')
-               302 LOAD_NAME               41 (callable)
-               304 BUILD_TUPLE              2
-               306 LOAD_CONST              23 (<code object base_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 54>)
-               308 MAKE_FUNCTION            4 (annotations)
-               310 STORE_NAME              42 (base_script_tag)
-   
-    78         312 LOAD_CONST              24 (<code object format_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 78>)
-               314 MAKE_FUNCTION            0
-               316 STORE_NAME              43 (format_script_tag)
-   
-    81         318 LOAD_CONST              25 (<code object format_css_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 81>)
-               320 MAKE_FUNCTION            0
-               322 STORE_NAME              44 (format_css_tag)
-   
-    84         324 LOAD_CONST              26 ('globlocks_js')
-               326 STORE_NAME              45 (globlocks_js_hook_name)
-   
-    85         328 PUSH_NULL
-               330 LOAD_NAME               37 (register)
-               332 LOAD_METHOD             39 (simple_tag)
-               354 LOAD_NAME               45 (globlocks_js_hook_name)
-               356 LOAD_CONST              18 (True)
-               358 KW_NAMES                19
-               360 PRECALL                  2
-               364 CALL                     2
-   
-    86         374 PUSH_NULL
-               376 LOAD_NAME               42 (base_script_tag)
-               378 LOAD_NAME               28 (staticfiles_globlocks_js)
-               380 LOAD_NAME               45 (globlocks_js_hook_name)
-               382 LOAD_NAME               43 (format_script_tag)
-               384 PRECALL                  3
-               388 CALL                     3
-   
-    85         398 PRECALL                  1
-               402 CALL                     1
-               412 POP_TOP
-   
-    89         414 LOAD_CONST              27 ('globlocks_css')
-               416 STORE_NAME              46 (globlocks_css_hook_name)
-   
-    90         418 PUSH_NULL
-               420 LOAD_NAME               37 (register)
-               422 LOAD_METHOD             39 (simple_tag)
-               444 LOAD_NAME               46 (globlocks_css_hook_name)
-               446 LOAD_CONST              18 (True)
-               448 KW_NAMES                19
-               450 PRECALL                  2
-               454 CALL                     2
-   
-    91         464 PUSH_NULL
-               466 LOAD_NAME               42 (base_script_tag)
-               468 LOAD_NAME               30 (staticfiles_globlocks_css)
-               470 LOAD_NAME               46 (globlocks_css_hook_name)
-               472 LOAD_NAME               44 (format_css_tag)
-               474 PRECALL                  3
-               478 CALL                     3
-   
-    90         488 PRECALL                  1
-               492 CALL                     1
-               502 POP_TOP
-   
-    95         504 PUSH_NULL
-               506 LOAD_NAME               35 (re)
-               508 LOAD_ATTR               47 (compile)
-               518 LOAD_CONST              28 ('^[a-zA-Z0-9]+://')
-               520 PRECALL                  1
-               524 CALL                     1
-               534 STORE_NAME              48 (HAS_PROTO_RE)
-   
-    96         536 LOAD_NAME                2 (Union)
-   
-    97         538 LOAD_NAME               34 (components)
-               540 LOAD_ATTR               49 (LinkValue)
-   
-    98         550 LOAD_NAME               14 (Page)
-               552 LOAD_NAME               16 (AbstractDocument)
-   
-    99         554 LOAD_NAME               50 (str)
-               556 LOAD_NAME                1 (Any)
-   
-    97         558 BUILD_TUPLE              5
-   
-    96         560 BINARY_SUBSCR
-               570 STORE_NAME              51 (POSSIBLE_LINK_TYPES)
-   
-   103         572 LOAD_NAME               37 (register)
-               574 LOAD_METHOD             39 (simple_tag)
-               596 LOAD_CONST              29 ('link')
-               598 LOAD_CONST              18 (True)
-               600 KW_NAMES                19
-               602 PRECALL                  2
-               606 CALL                     2
-   
-   104         616 LOAD_CONST              38 ((False,))
-               618 LOAD_CONST              30 ('value')
-               620 LOAD_NAME               51 (POSSIBLE_LINK_TYPES)
-               622 LOAD_CONST              31 ('full')
-               624 LOAD_NAME               52 (bool)
-               626 LOAD_CONST              22 ('return')
-               628 LOAD_NAME               50 (str)
-               630 BUILD_TUPLE              6
-               632 LOAD_CONST              32 (<code object do_link, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 103>)
-               634 MAKE_FUNCTION            5 (defaults, annotations)
-   
-   103         636 PRECALL                  0
-               640 CALL                     0
-   
-   104         650 STORE_NAME              53 (do_link)
-   
-   146         652 PUSH_NULL
-               654 LOAD_BUILD_CLASS
-               656 LOAD_CONST              33 (<code object FragmentNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 146>)
-               658 MAKE_FUNCTION            0
-               660 LOAD_CONST              34 ('FragmentNode')
-               662 LOAD_NAME                4 (template)
-               664 LOAD_ATTR               54 (Node)
-               674 PRECALL                  3
-               678 CALL                     3
-               688 STORE_NAME              55 (FragmentNode)
-   
-   168         690 LOAD_NAME               37 (register)
-               692 LOAD_METHOD             56 (tag)
-               714 LOAD_CONST              35 ('block_fragment')
-               716 KW_NAMES                36
-               718 PRECALL                  1
-               722 CALL                     1
-   
-   169         732 LOAD_CONST              37 (<code object fragment, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 168>)
-               734 MAKE_FUNCTION            0
-   
-   168         736 PRECALL                  0
-               740 CALL                     0
-   
-   169         750 STORE_NAME              57 (fragment)
-               752 LOAD_CONST              15 (None)
-               754 RETURN_VALUE
+    18         166 LOAD_CONST               0 (0)
+               168 LOAD_CONST              13 (('globlocks_js', 'globlocks_css'))
+               170 IMPORT_NAME             29 (globlocks.staticfiles)
+               172 IMPORT_FROM             30 (globlocks_js)
+               174 STORE_NAME              31 (staticfiles_globlocks_js)
+               176 IMPORT_FROM             32 (globlocks_css)
+               178 STORE_NAME              33 (staticfiles_globlocks_css)
+               180 POP_TOP
+   
+    22         182 LOAD_CONST               0 (0)
+               184 LOAD_CONST              14 (('get_hooks',))
+               186 IMPORT_NAME             34 (globlocks.util)
+               188 IMPORT_FROM             35 (get_hooks)
+               190 STORE_NAME              35 (get_hooks)
+               192 POP_TOP
+   
+    25         194 LOAD_CONST               0 (0)
+               196 LOAD_CONST              15 (('components',))
+               198 IMPORT_NAME             36 (globlocks.blocks)
+               200 IMPORT_FROM             37 (components)
+               202 STORE_NAME              37 (components)
+               204 POP_TOP
+   
+    29         206 LOAD_CONST               0 (0)
+               208 LOAD_CONST              16 (None)
+               210 IMPORT_NAME             38 (re)
+               212 STORE_NAME              38 (re)
+   
+    32         214 PUSH_NULL
+               216 LOAD_NAME               10 (library)
+               218 LOAD_ATTR               39 (Library)
+               228 PRECALL                  0
+               232 CALL                     0
+               242 STORE_NAME              40 (register)
+   
+    35         244 LOAD_CONST              17 (<code object format_static_file, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 35>)
+               246 MAKE_FUNCTION            0
+               248 STORE_NAME              41 (format_static_file)
+   
+    44         250 LOAD_NAME               40 (register)
+               252 LOAD_METHOD             42 (simple_tag)
+               274 LOAD_CONST              18 ('render_as_preview')
+               276 LOAD_CONST              19 (True)
+               278 KW_NAMES                20
+               280 PRECALL                  2
+               284 CALL                     2
+   
+    45         294 LOAD_CONST              39 ((False,))
+               296 LOAD_CONST              22 (<code object render_as_preview, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 44>)
+               298 MAKE_FUNCTION            1 (defaults)
+   
+    44         300 PRECALL                  0
+               304 CALL                     0
+   
+    45         314 STORE_NAME              43 (render_as_preview)
+   
+    55         316 LOAD_CONST              23 ('return')
+               318 LOAD_NAME               44 (callable)
+               320 BUILD_TUPLE              2
+               322 LOAD_CONST              24 (<code object base_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 55>)
+               324 MAKE_FUNCTION            4 (annotations)
+               326 STORE_NAME              45 (base_script_tag)
+   
+    79         328 LOAD_CONST              25 (<code object format_script_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 79>)
+               330 MAKE_FUNCTION            0
+               332 STORE_NAME              46 (format_script_tag)
+   
+    82         334 LOAD_CONST              26 (<code object format_css_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 82>)
+               336 MAKE_FUNCTION            0
+               338 STORE_NAME              47 (format_css_tag)
+   
+    85         340 LOAD_CONST              27 ('globlocks_js')
+               342 STORE_NAME              48 (globlocks_js_hook_name)
+   
+    86         344 PUSH_NULL
+               346 LOAD_NAME               40 (register)
+               348 LOAD_METHOD             42 (simple_tag)
+               370 LOAD_NAME               48 (globlocks_js_hook_name)
+               372 LOAD_CONST              19 (True)
+               374 KW_NAMES                20
+               376 PRECALL                  2
+               380 CALL                     2
+   
+    87         390 PUSH_NULL
+               392 LOAD_NAME               45 (base_script_tag)
+               394 LOAD_NAME               31 (staticfiles_globlocks_js)
+               396 LOAD_NAME               48 (globlocks_js_hook_name)
+               398 LOAD_NAME               46 (format_script_tag)
+               400 PRECALL                  3
+               404 CALL                     3
+   
+    86         414 PRECALL                  1
+               418 CALL                     1
+               428 POP_TOP
+   
+    90         430 LOAD_CONST              28 ('globlocks_css')
+               432 STORE_NAME              49 (globlocks_css_hook_name)
+   
+    91         434 PUSH_NULL
+               436 LOAD_NAME               40 (register)
+               438 LOAD_METHOD             42 (simple_tag)
+               460 LOAD_NAME               49 (globlocks_css_hook_name)
+               462 LOAD_CONST              19 (True)
+               464 KW_NAMES                20
+               466 PRECALL                  2
+               470 CALL                     2
+   
+    92         480 PUSH_NULL
+               482 LOAD_NAME               45 (base_script_tag)
+               484 LOAD_NAME               33 (staticfiles_globlocks_css)
+               486 LOAD_NAME               49 (globlocks_css_hook_name)
+               488 LOAD_NAME               47 (format_css_tag)
+               490 PRECALL                  3
+               494 CALL                     3
+   
+    91         504 PRECALL                  1
+               508 CALL                     1
+               518 POP_TOP
+   
+    96         520 PUSH_NULL
+               522 LOAD_NAME               38 (re)
+               524 LOAD_ATTR               50 (compile)
+               534 LOAD_CONST              29 ('^[a-zA-Z0-9]+://')
+               536 PRECALL                  1
+               540 CALL                     1
+               550 STORE_NAME              51 (HAS_PROTO_RE)
+   
+    97         552 LOAD_NAME                2 (Union)
+   
+    98         554 LOAD_NAME               37 (components)
+               556 LOAD_ATTR               52 (LinkValue)
+   
+    99         566 LOAD_NAME               16 (Page)
+               568 LOAD_NAME               19 (AbstractDocument)
+   
+   100         570 LOAD_NAME               53 (str)
+               572 LOAD_NAME                1 (Any)
+   
+    98         574 BUILD_TUPLE              5
+   
+    97         576 BINARY_SUBSCR
+               586 STORE_NAME              54 (POSSIBLE_LINK_TYPES)
+   
+   104         588 LOAD_NAME               40 (register)
+               590 LOAD_METHOD             42 (simple_tag)
+               612 LOAD_CONST              30 ('link')
+               614 LOAD_CONST              19 (True)
+               616 KW_NAMES                20
+               618 PRECALL                  2
+               622 CALL                     2
+   
+   105         632 LOAD_CONST              39 ((False,))
+               634 LOAD_CONST              31 ('value')
+               636 LOAD_NAME               54 (POSSIBLE_LINK_TYPES)
+               638 LOAD_CONST              32 ('full')
+               640 LOAD_NAME               55 (bool)
+               642 LOAD_CONST              23 ('return')
+               644 LOAD_NAME               53 (str)
+               646 BUILD_TUPLE              6
+               648 LOAD_CONST              33 (<code object do_link, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 104>)
+               650 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   104         652 PRECALL                  0
+               656 CALL                     0
+   
+   105         666 STORE_NAME              56 (do_link)
+   
+   147         668 PUSH_NULL
+               670 LOAD_BUILD_CLASS
+               672 LOAD_CONST              34 (<code object FragmentNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 147>)
+               674 MAKE_FUNCTION            0
+               676 LOAD_CONST              35 ('FragmentNode')
+               678 LOAD_NAME                4 (template)
+               680 LOAD_ATTR               57 (Node)
+               690 PRECALL                  3
+               694 CALL                     3
+               704 STORE_NAME              58 (FragmentNode)
+   
+   169         706 LOAD_NAME               40 (register)
+               708 LOAD_METHOD             59 (tag)
+               730 LOAD_CONST              36 ('block_fragment')
+               732 KW_NAMES                37
+               734 PRECALL                  1
+               738 CALL                     1
+   
+   170         748 LOAD_CONST              38 (<code object fragment, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 169>)
+               750 MAKE_FUNCTION            0
+   
+   169         752 PRECALL                  0
+               756 CALL                     0
+   
+   170         766 STORE_NAME              60 (fragment)
+               768 LOAD_CONST              16 (None)
+               770 RETURN_VALUE
    consts
       0
       ('Any', 'Union')
       ('template',)
+      ('reverse',)
       ('HttpRequest',)
       ('library',)
       ('mark_safe',)
       ('static',)
-      ('Page',)
+      ('Page', 'PAGE_TEMPLATE_VAR')
       ('AbstractDocument',)
       ('AbstractImage', 'AbstractRendition')
       ('PreviewUnavailable', 'preview_of_block')
       ('GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG')
       ('globlocks_js', 'globlocks_css')
       ('get_hooks',)
       ('components',)
@@ -337,101 +347,101 @@
          stacksize : 4
          flags     : 3
          code
             0x9700640144005d1b7d017c00a000000000000000000000000000000000
             00000000007c01a6010000ab01000000000000000072047c006302010053
             008c1c7403000000000000000000007c00a6010000ab0100000000000000
             005300
-          34           0 RESUME                   0
+          35           0 RESUME                   0
          
-          36           2 LOAD_CONST               1 (('/', 'http://', 'https://'))
+          37           2 LOAD_CONST               1 (('/', 'http://', 'https://'))
                        4 GET_ITER
                  >>    6 FOR_ITER                27 (to 62)
                        8 STORE_FAST               1 (prefix)
          
-          37          10 LOAD_FAST                0 (file)
+          38          10 LOAD_FAST                0 (file)
                       12 LOAD_METHOD              0 (startswith)
                       34 LOAD_FAST                1 (prefix)
                       36 PRECALL                  1
                       40 CALL                     1
                       50 POP_JUMP_FORWARD_IF_FALSE     4 (to 60)
          
-          38          52 LOAD_FAST                0 (file)
+          39          52 LOAD_FAST                0 (file)
                       54 SWAP                     2
                       56 POP_TOP
                       58 RETURN_VALUE
          
-          37     >>   60 JUMP_BACKWARD           28 (to 6)
+          38     >>   60 JUMP_BACKWARD           28 (to 6)
          
-          40     >>   62 LOAD_GLOBAL              3 (NULL + static)
+          41     >>   62 LOAD_GLOBAL              3 (NULL + static)
                       74 LOAD_FAST                0 (file)
                       76 PRECALL                  1
                       80 CALL                     1
                       90 RETURN_VALUE
          consts
             None
             ('/', 'http://', 'https://')
          names      ('startswith', 'static')
          varnames   ('file', 'prefix')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'format_static_file'
-         firstlineno 34
+         firstlineno 35
          lnotab 0x020208012a0108ff0203
       'render_as_preview'
       True
       ('name', 'takes_context')
       False
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 11
          code
             0x970009007401000000000000000000007c017c00660264017c0269017c
             03a4018e017d047c048002640253007c0453002300740200000000000000
             0000002400720501007c016302590053007700780359007701
-          43           0 RESUME                   0
+          44           0 RESUME                   0
          
-          45           2 NOP
+          46           2 NOP
          
-          46           4 LOAD_GLOBAL              1 (NULL + preview_of_block)
+          47           4 LOAD_GLOBAL              1 (NULL + preview_of_block)
                       16 LOAD_FAST                1 (block)
                       18 LOAD_FAST                0 (context)
                       20 BUILD_TUPLE              2
                       22 LOAD_CONST               1 ('fail_silently')
                       24 LOAD_FAST                2 (fail_silently)
                       26 BUILD_MAP                1
                       28 LOAD_FAST                3 (kwargs)
                       30 DICT_MERGE               1
                       32 CALL_FUNCTION_EX         1
                       34 STORE_FAST               4 (v)
          
-          47          36 LOAD_FAST                4 (v)
+          48          36 LOAD_FAST                4 (v)
                       38 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 44)
          
-          48          40 LOAD_CONST               2 ('')
+          49          40 LOAD_CONST               2 ('')
                       42 RETURN_VALUE
          
-          49     >>   44 LOAD_FAST                4 (v)
+          50     >>   44 LOAD_FAST                4 (v)
                       46 RETURN_VALUE
                  >>   48 PUSH_EXC_INFO
          
-          50          50 LOAD_GLOBAL              2 (PreviewUnavailable)
+          51          50 LOAD_GLOBAL              2 (PreviewUnavailable)
                       62 CHECK_EXC_MATCH
                       64 POP_JUMP_FORWARD_IF_FALSE     5 (to 76)
                       66 POP_TOP
          
-          51          68 LOAD_FAST                1 (block)
+          52          68 LOAD_FAST                1 (block)
                       70 SWAP                     2
                       72 POP_EXCEPT
                       74 RETURN_VALUE
          
-          50     >>   76 RERAISE                  0
+          51     >>   76 RERAISE                  0
                  >>   78 COPY                     3
                       80 POP_EXCEPT
                       82 RERAISE                  1
          ExceptionTable:
            4 to 38 -> 48 [0]
            44 to 44 -> 48 [0]
            48 to 70 -> 78 [1] lasti
@@ -442,38 +452,38 @@
             ''
          names      ('preview_of_block', 'PreviewUnavailable')
          varnames   ('context', 'block', 'fail_silently', 'kwargs', 'v')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'render_as_preview'
-         firstlineno 43
+         firstlineno 44
          lnotab 0x020202012001040104010601120108ff
       'return'
       code
          argcount  : 3
          nlocals   : 4
          stacksize : 3
          flags     : 3
          code 0x87008701870297008800880288016603640184087d037c035300
                        0 MAKE_CELL                0 (files_or_hook)
                        2 MAKE_CELL                1 (hook_name)
                        4 MAKE_CELL                2 (format_fn)
          
-          54           6 RESUME                   0
+          55           6 RESUME                   0
          
-          55           8 LOAD_CLOSURE             0 (files_or_hook)
+          56           8 LOAD_CLOSURE             0 (files_or_hook)
                       10 LOAD_CLOSURE             2 (format_fn)
                       12 LOAD_CLOSURE             1 (hook_name)
                       14 BUILD_TUPLE              3
-                      16 LOAD_CONST               1 (<code object _tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 55>)
+                      16 LOAD_CONST               1 (<code object _tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 56>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_FAST               3 (_tag)
          
-          76          22 LOAD_FAST                3 (_tag)
+          77          22 LOAD_FAST                3 (_tag)
                       24 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 6
@@ -491,95 +501,95 @@
                   557c02a0040000000000000000000000000000000000000000020089067c
                   04a6010000ab010000000000000000a6010000ab01000000000000000001
                   008c74740d000000000000000000006403740e000000000000000000009b
                   009d02a00800000000000000000000000000000000000000007c02a60100
                   00ab010000000000000000a6010000ab0100000000000000005300
                              0 COPY_FREE_VARS           3
                
-                55           2 RESUME                   0
+                56           2 RESUME                   0
                
-                56           4 LOAD_FAST                0 (context)
+                57           4 LOAD_FAST                0 (context)
                              6 LOAD_METHOD              0 (get)
                             28 LOAD_CONST               1 ('request')
                             30 LOAD_CONST               0 (None)
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               1 (request)
                
-                58          48 BUILD_LIST               0
+                59          48 BUILD_LIST               0
                             50 STORE_FAST               2 (s)
                
-                60          52 LOAD_DEREF               5 (files_or_hook)
+                61          52 LOAD_DEREF               5 (files_or_hook)
                             54 STORE_FAST               3 (files)
                
-                61          56 BUILD_LIST               0
+                62          56 BUILD_LIST               0
                
-                62          58 LOAD_FAST                3 (files)
+                63          58 LOAD_FAST                3 (files)
                
-                61          60 LIST_EXTEND              1
+                62          60 LIST_EXTEND              1
                
-                63          62 LOAD_GLOBAL              3 (NULL + get_hooks)
+                64          62 LOAD_GLOBAL              3 (NULL + get_hooks)
                             74 LOAD_DEREF               7 (hook_name)
                             76 PRECALL                  1
                             80 CALL                     1
                
-                61          90 LIST_EXTEND              1
+                62          90 LIST_EXTEND              1
                             92 LIST_TO_TUPLE
                             94 STORE_FAST               3 (files)
                
-                66          96 LOAD_FAST                3 (files)
+                67          96 LOAD_FAST                3 (files)
                             98 GET_ITER
                        >>  100 FOR_ITER               115 (to 332)
                            102 STORE_FAST               4 (file)
                
-                67         104 LOAD_GLOBAL              5 (NULL + callable)
+                68         104 LOAD_GLOBAL              5 (NULL + callable)
                            116 LOAD_FAST                4 (file)
                            118 PRECALL                  1
                            122 CALL                     1
                            132 POP_JUMP_FORWARD_IF_FALSE    12 (to 158)
                
-                68         134 PUSH_NULL
+                69         134 PUSH_NULL
                            136 LOAD_FAST                4 (file)
                            138 LOAD_FAST                1 (request)
                            140 LOAD_FAST                0 (context)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_FAST               4 (file)
                
-                70     >>  158 LOAD_GLOBAL              7 (NULL + hasattr)
+                71     >>  158 LOAD_GLOBAL              7 (NULL + hasattr)
                            170 LOAD_FAST                4 (file)
                            172 LOAD_CONST               2 ('__html__')
                            174 PRECALL                  2
                            178 CALL                     2
                            188 POP_JUMP_FORWARD_IF_FALSE    40 (to 270)
                
-                71         190 LOAD_FAST                2 (s)
+                72         190 LOAD_FAST                2 (s)
                            192 LOAD_METHOD              4 (append)
                            214 LOAD_FAST                4 (file)
                            216 LOAD_METHOD              5 (__html__)
                            238 PRECALL                  0
                            242 CALL                     0
                            252 PRECALL                  1
                            256 CALL                     1
                            266 POP_TOP
                            268 JUMP_BACKWARD           85 (to 100)
                
-                73     >>  270 LOAD_FAST                2 (s)
+                74     >>  270 LOAD_FAST                2 (s)
                            272 LOAD_METHOD              4 (append)
                            294 PUSH_NULL
                            296 LOAD_DEREF               6 (format_fn)
                            298 LOAD_FAST                4 (file)
                            300 PRECALL                  1
                            304 CALL                     1
                            314 PRECALL                  1
                            318 CALL                     1
                            328 POP_TOP
                            330 JUMP_BACKWARD          116 (to 100)
                
-                75     >>  332 LOAD_GLOBAL             13 (NULL + mark_safe)
+                76     >>  332 LOAD_GLOBAL             13 (NULL + mark_safe)
                            344 LOAD_CONST               3 ('\n')
                            346 LOAD_GLOBAL             14 (GLOBLOCKS_SCRIPT_INDENT)
                            358 FORMAT_VALUE             0
                            360 BUILD_STRING             2
                            362 LOAD_METHOD              8 (join)
                            384 LOAD_FAST                2 (s)
                            386 PRECALL                  1
@@ -594,37 +604,37 @@
                   '\n'
                names      ('get', 'get_hooks', 'callable', 'hasattr', 'append', '__html__', 'mark_safe', 'GLOBLOCKS_SCRIPT_INDENT', 'join')
                varnames   ('context', 'request', 's', 'files', 'file')
                freevars   ('files_or_hook', 'format_fn', 'hook_name')
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
                name       '_tag'
-               firstlineno 55
+               firstlineno 56
                lnotab
                   0x04012c0204020401020102ff02021cfe060508011e011802200150023e
                   02
          names      ()
          varnames   ('files_or_hook', 'hook_name', 'format_fn', '_tag')
          freevars   ()
          cellvars   ('files_or_hook', 'hook_name', 'format_fn')
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'base_script_tag'
-         firstlineno 54
+         firstlineno 55
          lnotab 0x08010e15
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017401000000000000000000007c00a6010000ab010000000000
             0000009b0064029d035300
-          78           0 RESUME                   0
+          79           0 RESUME                   0
          
-          79           2 LOAD_CONST               1 ('<script src="')
+          80           2 LOAD_CONST               1 ('<script src="')
                        4 LOAD_GLOBAL              1 (NULL + format_static_file)
                       16 LOAD_FAST                0 (file)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 FORMAT_VALUE             0
                       34 LOAD_CONST               2 ('"></script>')
                       36 BUILD_STRING             3
@@ -635,27 +645,27 @@
             '"></script>'
          names      ('format_static_file',)
          varnames   ('file',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'format_script_tag'
-         firstlineno 78
+         firstlineno 79
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017401000000000000000000007c00a6010000ab010000000000
             0000009b0064029d035300
-          81           0 RESUME                   0
+          82           0 RESUME                   0
          
-          82           2 LOAD_CONST               1 ('<link rel="stylesheet" href="')
+          83           2 LOAD_CONST               1 ('<link rel="stylesheet" href="')
                        4 LOAD_GLOBAL              1 (NULL + format_static_file)
                       16 LOAD_FAST                0 (file)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 FORMAT_VALUE             0
                       34 LOAD_CONST               2 ('">')
                       36 BUILD_STRING             3
@@ -666,15 +676,15 @@
             '">'
          names      ('format_static_file',)
          varnames   ('file',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'format_css_tag'
-         firstlineno 81
+         firstlineno 82
          lnotab 0x0201
       'globlocks_js'
       'globlocks_css'
       '^[a-zA-Z0-9]+://'
       'link'
       'value'
       'full'
@@ -710,197 +720,197 @@
             010000ab010000000000000000742000000000000000000000a011000000
             00000000000000000000000000000000007c01a6010000ab010000000000
             0000006702a6010000ab01000000000000000073157c03a0090000000000
             0000000000000000000000000000007c01a6010000ab0100000000000000
             0053007c0153007425000000000000000000006407a6010000ab01000000
             000000000044005d167d0502007c057c017c007c02ac02a6030000ab0300
             000000000000007d067c0672047c066302010053008c177c015300
-         103           0 RESUME                   0
+         104           0 RESUME                   0
          
-         105           2 LOAD_FAST                0 (context)
+         106           2 LOAD_FAST                0 (context)
                        4 LOAD_METHOD              0 (get)
                       26 LOAD_CONST               1 ('request')
                       28 LOAD_CONST               0 (None)
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               3 (request)
          
-         107          46 LOAD_GLOBAL              3 (NULL + isinstance)
+         108          46 LOAD_GLOBAL              3 (NULL + isinstance)
                       58 LOAD_FAST                1 (value)
                       60 LOAD_GLOBAL              4 (components)
                       72 LOAD_ATTR                3 (LinkValue)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE    23 (to 144)
          
-         108          98 LOAD_FAST                1 (value)
+         109          98 LOAD_FAST                1 (value)
                      100 LOAD_METHOD              4 (get_url)
                      122 LOAD_FAST                3 (request)
                      124 LOAD_FAST                2 (full)
                      126 KW_NAMES                 2
                      128 PRECALL                  2
                      132 CALL                     2
                      142 RETURN_VALUE
          
-         110     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+         111     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                      156 LOAD_FAST                1 (value)
                      158 LOAD_GLOBAL             10 (Page)
                      170 PRECALL                  2
                      174 CALL                     2
                      184 POP_JUMP_FORWARD_IF_FALSE    44 (to 274)
          
-         111         186 LOAD_FAST                2 (full)
+         112         186 LOAD_FAST                2 (full)
                      188 POP_JUMP_FORWARD_IF_FALSE    21 (to 232)
          
-         112         190 LOAD_FAST                1 (value)
+         113         190 LOAD_FAST                1 (value)
                      192 LOAD_METHOD              6 (get_full_url)
                      214 LOAD_FAST                3 (request)
                      216 PRECALL                  1
                      220 CALL                     1
                      230 RETURN_VALUE
          
-         113     >>  232 LOAD_FAST                1 (value)
+         114     >>  232 LOAD_FAST                1 (value)
                      234 LOAD_METHOD              4 (get_url)
                      256 LOAD_FAST                3 (request)
                      258 PRECALL                  1
                      262 CALL                     1
                      272 RETURN_VALUE
          
-         115     >>  274 LOAD_GLOBAL              3 (NULL + isinstance)
+         116     >>  274 LOAD_GLOBAL              3 (NULL + isinstance)
                      286 LOAD_FAST                1 (value)
                      288 LOAD_GLOBAL             14 (AbstractImage)
                      300 PRECALL                  2
                      304 CALL                     2
                      314 POP_JUMP_FORWARD_IF_FALSE    56 (to 428)
          
-         116         316 LOAD_FAST                1 (value)
+         117         316 LOAD_FAST                1 (value)
                      318 LOAD_METHOD              8 (get_rendition)
                      340 LOAD_CONST               3 ('original')
                      342 PRECALL                  1
                      346 CALL                     1
                      356 STORE_FAST               4 (rendition)
          
-         117         358 LOAD_FAST                2 (full)
+         118         358 LOAD_FAST                2 (full)
                      360 POP_JUMP_FORWARD_IF_FALSE    26 (to 414)
          
-         118         362 LOAD_FAST                3 (request)
+         119         362 LOAD_FAST                3 (request)
                      364 LOAD_METHOD              9 (build_absolute_uri)
                      386 LOAD_FAST                4 (rendition)
                      388 LOAD_ATTR               10 (url)
                      398 PRECALL                  1
                      402 CALL                     1
                      412 RETURN_VALUE
          
-         119     >>  414 LOAD_FAST                4 (rendition)
+         120     >>  414 LOAD_FAST                4 (rendition)
                      416 LOAD_ATTR               10 (url)
                      426 RETURN_VALUE
          
-         121     >>  428 LOAD_GLOBAL             23 (NULL + hasattr)
+         122     >>  428 LOAD_GLOBAL             23 (NULL + hasattr)
                      440 LOAD_FAST                1 (value)
                      442 LOAD_CONST               4 ('get_absolute_url')
                      444 PRECALL                  2
                      448 CALL                     2
                      458 POP_JUMP_FORWARD_IF_FALSE    21 (to 502)
          
-         122         460 LOAD_FAST                1 (value)
+         123         460 LOAD_FAST                1 (value)
                      462 LOAD_METHOD             12 (get_absolute_url)
                      484 LOAD_FAST                3 (request)
                      486 PRECALL                  1
                      490 CALL                     1
                      500 RETURN_VALUE
          
-         124     >>  502 LOAD_GLOBAL             23 (NULL + hasattr)
+         125     >>  502 LOAD_GLOBAL             23 (NULL + hasattr)
                      514 LOAD_FAST                1 (value)
                      516 LOAD_CONST               5 ('url')
                      518 PRECALL                  2
                      522 CALL                     2
                      532 POP_JUMP_FORWARD_IF_FALSE    35 (to 604)
          
-         125         534 LOAD_FAST                2 (full)
+         126         534 LOAD_FAST                2 (full)
                      536 POP_JUMP_FORWARD_IF_FALSE    26 (to 590)
          
-         126         538 LOAD_FAST                3 (request)
+         127         538 LOAD_FAST                3 (request)
                      540 LOAD_METHOD              9 (build_absolute_uri)
                      562 LOAD_FAST                1 (value)
                      564 LOAD_ATTR               10 (url)
                      574 PRECALL                  1
                      578 CALL                     1
                      588 RETURN_VALUE
          
-         127     >>  590 LOAD_FAST                1 (value)
+         128     >>  590 LOAD_FAST                1 (value)
                      592 LOAD_ATTR               10 (url)
                      602 RETURN_VALUE
          
-         129     >>  604 LOAD_GLOBAL              3 (NULL + isinstance)
+         130     >>  604 LOAD_GLOBAL              3 (NULL + isinstance)
                      616 LOAD_FAST                1 (value)
                      618 LOAD_GLOBAL             26 (str)
                      630 PRECALL                  2
                      634 CALL                     2
                      644 POP_JUMP_FORWARD_IF_FALSE    85 (to 816)
          
-         130         646 LOAD_FAST                2 (full)
+         131         646 LOAD_FAST                2 (full)
                      648 POP_JUMP_FORWARD_IF_FALSE    81 (to 812)
                      650 LOAD_GLOBAL             29 (NULL + any)
          
-         131         662 LOAD_FAST                1 (value)
+         132         662 LOAD_FAST                1 (value)
                      664 LOAD_METHOD             15 (startswith)
                      686 LOAD_CONST               6 ('//')
                      688 PRECALL                  1
                      692 CALL                     1
          
-         132         702 LOAD_GLOBAL             32 (HAS_PROTO_RE)
+         133         702 LOAD_GLOBAL             32 (HAS_PROTO_RE)
                      714 LOAD_METHOD             17 (match)
                      736 LOAD_FAST                1 (value)
                      738 PRECALL                  1
                      742 CALL                     1
          
-         130         752 BUILD_LIST               2
+         131         752 BUILD_LIST               2
                      754 PRECALL                  1
                      758 CALL                     1
                      768 POP_JUMP_FORWARD_IF_TRUE    21 (to 812)
          
-         134         770 LOAD_FAST                3 (request)
+         135         770 LOAD_FAST                3 (request)
                      772 LOAD_METHOD              9 (build_absolute_uri)
                      794 LOAD_FAST                1 (value)
                      796 PRECALL                  1
                      800 CALL                     1
                      810 RETURN_VALUE
          
-         136     >>  812 LOAD_FAST                1 (value)
+         137     >>  812 LOAD_FAST                1 (value)
                      814 RETURN_VALUE
          
-         138     >>  816 LOAD_GLOBAL             37 (NULL + get_hooks)
+         139     >>  816 LOAD_GLOBAL             37 (NULL + get_hooks)
                      828 LOAD_CONST               7 ('generate_link')
                      830 PRECALL                  1
                      834 CALL                     1
                      844 GET_ITER
                  >>  846 FOR_ITER                22 (to 892)
                      848 STORE_FAST               5 (hook)
          
-         139         850 PUSH_NULL
+         140         850 PUSH_NULL
                      852 LOAD_FAST                5 (hook)
                      854 LOAD_FAST                1 (value)
                      856 LOAD_FAST                0 (context)
                      858 LOAD_FAST                2 (full)
                      860 KW_NAMES                 2
                      862 PRECALL                  3
                      866 CALL                     3
                      876 STORE_FAST               6 (result)
          
-         140         878 LOAD_FAST                6 (result)
+         141         878 LOAD_FAST                6 (result)
                      880 POP_JUMP_FORWARD_IF_FALSE     4 (to 890)
          
-         141         882 LOAD_FAST                6 (result)
+         142         882 LOAD_FAST                6 (result)
                      884 SWAP                     2
                      886 POP_TOP
                      888 RETURN_VALUE
          
-         140     >>  890 JUMP_BACKWARD           23 (to 846)
+         141     >>  890 JUMP_BACKWARD           23 (to 846)
          
-         143     >>  892 LOAD_FAST                1 (value)
+         144     >>  892 LOAD_FAST                1 (value)
                      894 RETURN_VALUE
          consts
             None
             'request'
             ('full',)
             'original'
             'get_absolute_url'
@@ -909,42 +919,42 @@
             'generate_link'
          names      ('get', 'isinstance', 'components', 'LinkValue', 'get_url', 'Page', 'get_full_url', 'AbstractImage', 'get_rendition', 'build_absolute_uri', 'url', 'hasattr', 'get_absolute_url', 'str', 'any', 'startswith', 'HAS_PROTO_RE', 'match', 'get_hooks')
          varnames   ('context', 'value', 'full', 'request', 'rendition', 'hook', 'result')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'do_link'
-         firstlineno 103
+         firstlineno 104
          lnotab
             0x02022c0234012e022a0104012a012a022a012a01040134010e0220012a
             022001040134010e022a011001280132fe12042a02040222011c01040108
             ff0203
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0264015a036406640384015a04640484005a0564
             055300
-         146           0 RESUME                   0
+         147           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FragmentNode')
                        8 STORE_NAME               2 (__qualname__)
          
-         147          10 LOAD_CONST               1 ('\n        This generously comes from wagtail.admin.templatetags.wagtailadmin_tags\n    ')
+         148          10 LOAD_CONST               1 ('\n        This generously comes from wagtail.admin.templatetags.wagtailadmin_tags\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         151          14 LOAD_CONST               6 ((False,))
-                      16 LOAD_CONST               3 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 151>)
+         152          14 LOAD_CONST               6 ((False,))
+                      16 LOAD_CONST               3 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 152>)
                       18 MAKE_FUNCTION            1 (defaults)
                       20 STORE_NAME               4 (__init__)
          
-         156          22 LOAD_CONST               4 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 156>)
+         157          22 LOAD_CONST               4 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\__init__.py", line 157>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (render)
                       28 LOAD_CONST               5 (None)
                       30 RETURN_VALUE
          consts
             'FragmentNode'
             '\n        This generously comes from wagtail.admin.templatetags.wagtailadmin_tags\n    '
@@ -953,107 +963,107 @@
                argcount  : 4
                nlocals   : 4
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f02000000000000000064005300
-               151           0 RESUME                   0
+               152           0 RESUME                   0
                
-               152           2 LOAD_FAST                1 (nodelist)
+               153           2 LOAD_FAST                1 (nodelist)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (nodelist)
                
-               153          16 LOAD_FAST                2 (target_var)
+               154          16 LOAD_FAST                2 (target_var)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (target_var)
                
-               154          30 LOAD_FAST                3 (stripped)
+               155          30 LOAD_FAST                3 (stripped)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (stripped)
                             44 LOAD_CONST               0 (None)
                             46 RETURN_VALUE
                consts
                   None
                names      ('nodelist', 'target_var', 'stripped')
                varnames   ('self', 'nodelist', 'target_var', 'stripped')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
                name       '__init__'
-               firstlineno 151
+               firstlineno 152
                lnotab 0x02010e010e01
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000721a7c006a000000000000000000a0
                   0100000000000000000000000000000000000000007c01a6010000ab0100
                   000000000000006e0164017d027c006a0200000000000000007221740700
                   0000000000000000007c02a0040000000000000000000000000000000000
                   000000a6000000ab000000000000000000a6010000ab0100000000000000
                   007d027c027c017c006a0500000000000000003c00000064015300
-               156           0 RESUME                   0
+               157           0 RESUME                   0
                
-               157           2 LOAD_FAST                0 (self)
+               158           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (nodelist)
                             14 POP_JUMP_FORWARD_IF_FALSE    26 (to 68)
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                0 (nodelist)
                             28 LOAD_METHOD              1 (render)
                             50 LOAD_FAST                1 (context)
                             52 PRECALL                  1
                             56 CALL                     1
                             66 JUMP_FORWARD             1 (to 70)
                        >>   68 LOAD_CONST               1 ('')
                        >>   70 STORE_FAST               2 (fragment)
                
-               162          72 LOAD_FAST                0 (self)
+               163          72 LOAD_FAST                0 (self)
                             74 LOAD_ATTR                2 (stripped)
                             84 POP_JUMP_FORWARD_IF_FALSE    33 (to 152)
                
-               163          86 LOAD_GLOBAL              7 (NULL + mark_safe)
+               164          86 LOAD_GLOBAL              7 (NULL + mark_safe)
                             98 LOAD_FAST                2 (fragment)
                            100 LOAD_METHOD              4 (strip)
                            122 PRECALL                  0
                            126 CALL                     0
                            136 PRECALL                  1
                            140 CALL                     1
                            150 STORE_FAST               2 (fragment)
                
-               164     >>  152 LOAD_FAST                2 (fragment)
+               165     >>  152 LOAD_FAST                2 (fragment)
                            154 LOAD_FAST                1 (context)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                5 (target_var)
                            168 STORE_SUBSCR
                
-               165         172 LOAD_CONST               1 ('')
+               166         172 LOAD_CONST               1 ('')
                            174 RETURN_VALUE
                consts
                   None
                   ''
                names      ('nodelist', 'render', 'stripped', 'mark_safe', 'strip', 'target_var')
                varnames   ('self', 'context', 'fragment')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
                name       'render'
-               firstlineno 156
+               firstlineno 157
                lnotab 0x020146050e0142011401
             None
             (False,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'FragmentNode'
-         firstlineno 146
+         firstlineno 147
          lnotab 0x0a0104040805
       'FragmentNode'
       'block_fragment'
       ('name',)
       code
          argcount  : 2
          nlocals   : 8
@@ -1066,76 +1076,76 @@
             000000000000007d067c00a0020000000000000000000000000000000000
             000000a6000000ab00000000000000000001006e2c230074060000000000
             00000000002400721f01007408000000000000000000007214740b000000
             000000000000006a0600000000000000007c02a6010000ab010000000000
             0000008201590064035300770078035900770164047c0476007d07740f00
             0000000000000000007c067c057c07ac05a6030000ab0300000000000000
             005300
-         168           0 RESUME                   0
+         169           0 RESUME                   0
          
-         197           2 LOAD_CONST               1 ('The syntax for fragment is {% fragment as variable_name %}')
+         198           2 LOAD_CONST               1 ('The syntax for fragment is {% fragment as variable_name %}')
                        4 STORE_FAST               2 (error_message)
          
-         199           6 NOP
+         200           6 NOP
          
-         200           8 LOAD_FAST                1 (token)
+         201           8 LOAD_FAST                1 (token)
                       10 LOAD_METHOD              0 (split_contents)
                       32 PRECALL                  0
                       36 CALL                     0
                       46 EXTENDED_ARG             1
                       48 UNPACK_EX              257
                       50 STORE_FAST               3 (tag_name)
                       52 STORE_FAST               4 (options)
                       54 STORE_FAST               5 (target_var)
          
-         201          56 LOAD_FAST                0 (parser)
+         202          56 LOAD_FAST                0 (parser)
                       58 LOAD_METHOD              1 (parse)
                       80 LOAD_CONST               2 (('endblock_fragment',))
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               6 (nodelist)
          
-         202          98 LOAD_FAST                0 (parser)
+         203          98 LOAD_FAST                0 (parser)
                      100 LOAD_METHOD              2 (delete_first_token)
                      122 PRECALL                  0
                      126 CALL                     0
                      136 POP_TOP
                      138 JUMP_FORWARD            44 (to 228)
                  >>  140 PUSH_EXC_INFO
          
-         203         142 LOAD_GLOBAL              6 (ValueError)
+         204         142 LOAD_GLOBAL              6 (ValueError)
                      154 CHECK_EXC_MATCH
                      156 POP_JUMP_FORWARD_IF_FALSE    31 (to 220)
                      158 POP_TOP
          
-         204         160 LOAD_GLOBAL              8 (GLOBLOCKS_DEBUG)
+         205         160 LOAD_GLOBAL              8 (GLOBLOCKS_DEBUG)
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
          
-         205         174 LOAD_GLOBAL             11 (NULL + template)
+         206         174 LOAD_GLOBAL             11 (NULL + template)
                      186 LOAD_ATTR                6 (TemplateSyntaxError)
                      196 LOAD_FAST                2 (error_message)
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         206     >>  214 POP_EXCEPT
+         207     >>  214 POP_EXCEPT
                      216 LOAD_CONST               3 ('')
                      218 RETURN_VALUE
          
-         203     >>  220 RERAISE                  0
+         204     >>  220 RERAISE                  0
                  >>  222 COPY                     3
                      224 POP_EXCEPT
                      226 RERAISE                  1
          
-         208     >>  228 LOAD_CONST               4 ('stripped')
+         209     >>  228 LOAD_CONST               4 ('stripped')
                      230 LOAD_FAST                4 (options)
                      232 CONTAINS_OP              0
                      234 STORE_FAST               7 (stripped)
          
-         210         236 LOAD_GLOBAL             15 (NULL + FragmentNode)
+         211         236 LOAD_GLOBAL             15 (NULL + FragmentNode)
                      248 LOAD_FAST                6 (nodelist)
                      250 LOAD_FAST                5 (target_var)
                      252 LOAD_FAST                7 (stripped)
                      254 KW_NAMES                 5
                      256 PRECALL                  3
                      260 CALL                     3
                      270 RETURN_VALUE
@@ -1152,22 +1162,22 @@
             ('stripped',)
          names      ('split_contents', 'parse', 'delete_first_token', 'ValueError', 'GLOBLOCKS_DEBUG', 'template', 'TemplateSyntaxError', 'FragmentNode')
          varnames   ('parser', 'token', 'error_message', 'tag_name', 'options', 'target_var', 'nodelist', 'stripped')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
          name       'fragment'
-         firstlineno 168
+         firstlineno 169
          lnotab 0x021d0402020130012a012c0112010e01280106fd08050802
       (False,)
-   names      ('typing', 'Any', 'Union', 'django', 'template', 'django.http', 'HttpRequest', 'django.template', 'library', 'django.utils.safestring', 'mark_safe', 'django.templatetags.static', 'static', 'wagtail.models', 'Page', 'wagtail.documents.models', 'AbstractDocument', 'wagtail.images.models', 'AbstractImage', 'AbstractRendition', 'globlocks.preview', 'PreviewUnavailable', 'preview_of_block', 'globlocks.settings', 'GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG', 'globlocks.staticfiles', 'globlocks_js', 'staticfiles_globlocks_js', 'globlocks_css', 'staticfiles_globlocks_css', 'globlocks.util', 'get_hooks', 'globlocks.blocks', 'components', 're', 'Library', 'register', 'format_static_file', 'simple_tag', 'render_as_preview', 'callable', 'base_script_tag', 'format_script_tag', 'format_css_tag', 'globlocks_js_hook_name', 'globlocks_css_hook_name', 'compile', 'HAS_PROTO_RE', 'LinkValue', 'str', 'POSSIBLE_LINK_TYPES', 'bool', 'do_link', 'Node', 'FragmentNode', 'tag', 'fragment')
+   names      ('typing', 'Any', 'Union', 'django', 'template', 'django.urls', 'reverse', 'django.http', 'HttpRequest', 'django.template', 'library', 'django.utils.safestring', 'mark_safe', 'django.templatetags.static', 'static', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'wagtail.documents.models', 'AbstractDocument', 'wagtail.images.models', 'AbstractImage', 'AbstractRendition', 'globlocks.preview', 'PreviewUnavailable', 'preview_of_block', 'globlocks.settings', 'GLOBLOCKS_SCRIPT_INDENT', 'GLOBLOCKS_DEBUG', 'globlocks.staticfiles', 'globlocks_js', 'staticfiles_globlocks_js', 'globlocks_css', 'staticfiles_globlocks_css', 'globlocks.util', 'get_hooks', 'globlocks.blocks', 'components', 're', 'Library', 'register', 'format_static_file', 'simple_tag', 'render_as_preview', 'callable', 'base_script_tag', 'format_script_tag', 'format_css_tag', 'globlocks_js_hook_name', 'globlocks_css_hook_name', 'compile', 'HAS_PROTO_RE', 'LinkValue', 'str', 'POSSIBLE_LINK_TYPES', 'bool', 'do_link', 'Node', 'FragmentNode', 'tag', 'fragment')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c010c010c010c010c020c010c0110051001100110040c
-      030c0408031e0306092c0106ff0e01020a0c180603060304012e0118ff10
-      0404012e0118ff1005200102010c01040104fe02ff0c072c0114ff0e0102
-      2a26162a0104ff0e01
+      0x00ff020110010c010c010c010c010c010c0210010c0110051001100110
+      040c030c0408031e0306092c0106ff0e01020a0c180603060304012e0118
+      ff100404012e0118ff1005200102010c01040104fe02ff0c072c0114ff0e
+      01022a26162a0104ff0e01
```

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc` & `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -32,15 +32,15 @@
     13          44 LOAD_NAME                3 (register)
                 46 LOAD_METHOD              4 (simple_tag)
                 68 LOAD_CONST               2 ('get_from_mapping')
                 70 KW_NAMES                 3
                 72 PRECALL                  1
                 76 CALL                     1
    
-    14          86 LOAD_CONST               4 (<code object do_get_from_mapping, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/globlocks/admin.py", line 13>)
+    14          86 LOAD_CONST               4 (<code object do_get_from_mapping, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\admin.py", line 13>)
                 88 MAKE_FUNCTION            0
    
     13          90 PRECALL                  0
                 94 CALL                     0
    
     14         104 STORE_NAME               5 (do_get_from_mapping)
    
@@ -48,15 +48,15 @@
                108 LOAD_METHOD              4 (simple_tag)
                130 LOAD_CONST               5 ('columns')
                132 KW_NAMES                 3
                134 PRECALL                  1
                138 CALL                     1
    
     25         148 LOAD_CONST               8 ((None, None, None, None, None))
-               150 LOAD_CONST               7 (<code object do_columns, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\.venv\Lib\site-packages\globlocks/templatetags/globlocks/admin.py", line 24>)
+               150 LOAD_CONST               7 (<code object do_columns, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\admin.py", line 24>)
                152 MAKE_FUNCTION            1 (defaults)
    
     24         154 PRECALL                  0
                158 CALL                     0
    
     25         168 STORE_NAME               6 (do_columns)
                170 LOAD_CONST               6 (None)
@@ -116,15 +116,15 @@
             None
             'get'
             '__getitem__'
          names      ('hasattr', 'get', 'getattr')
          varnames   ('mapping', 'key')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/globlocks/admin.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\admin.py'
          name       'do_get_from_mapping'
          firstlineno 13
          lnotab 0x020220012a0220011002
       'columns'
       None
       code
          argcount  : 6
@@ -204,20 +204,20 @@
             ' col-md-'
             ' col-lg-'
             ' col-xl-'
          names      ()
          varnames   ('col_size', 'col_xs', 'col_sm', 'col_md', 'col_lg', 'col_xl')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/globlocks/admin.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\admin.py'
          name       'do_columns'
          firstlineno 24
          lnotab 0x0202180108010801080108010801
       (None, None, None, None, None)
    names      ('django.template', 'library', 'Library', 'register', 'simple_tag', 'do_get_from_mapping', 'do_columns')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\.venv\\Lib\\site-packages\\globlocks/templatetags/globlocks/admin.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\admin.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c021e0a2a0104ff0e01020a2a0106ff0e01
```

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc` & `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc` & `globlocks-1.2.1/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,171 +1,207 @@
 magic:    0xa70d0d0a
-moddate:  0x5958f965 (Tue Mar 19 09:18:17 2024 UTC)
-files sz: 1242
+moddate:  0x88480766 (Fri Mar 29 23:02:32 2024 UTC)
+files sz: 3472
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a020100020065016a030000000000
-      000000a6000000ab0000000000000000005a0464025a0564035a066504a0
-      0700000000000000000000000000000000000000006404ac05a6010000ab
-      01000000000000000064066508660264078404a6000000ab000000000000
-      0000005a096504a00a000000000000000000000000000000000000000064
-      08ac05a6010000ab01000000000000000064096508640a65086406650866
-      06640b8404a6000000ab0000000000000000005a0b6504a00a0000000000
-      000000000000000000000000000000640cac05a6010000ab010000000000
-      00000064096508640a650c640665086606640d8404a6000000ab00000000
-      00000000005a0d640e5300
+      0x9700640064016c006d015a016d025a020100640064026c036d045a0401
+      00640064036c056d065a060100640064046c076d085a080100640064056c
+      096d0a5a0a6d0b5a0b0100020065016a0c0000000000000000a6000000ab
+      0000000000000000005a0d64065a0e64075a0f650da01000000000000000
+      000000000000000000000000006408ac09a6010000ab0100000000000000
+      00640a65116602640b8404a6000000ab0000000000000000005a12650da0
+      130000000000000000000000000000000000000000640cac09a6010000ab
+      010000000000000000640d6511640e6511640a65116606640f8404a60000
+      00ab0000000000000000005a14650da01300000000000000000000000000
+      000000000000006410ac09a6010000ab010000000000000000640d651164
+      0e6515640a6511660664118404a6000000ab0000000000000000005a1664
+      125300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('library', 'TemplateSyntaxError'))
                  6 IMPORT_NAME              0 (django.template)
                  8 IMPORT_FROM              1 (library)
                 10 STORE_NAME               1 (library)
                 12 IMPORT_FROM              2 (TemplateSyntaxError)
                 14 STORE_NAME               2 (TemplateSyntaxError)
                 16 POP_TOP
    
-     3          18 PUSH_NULL
-                20 LOAD_NAME                1 (library)
-                22 LOAD_ATTR                3 (Library)
-                32 PRECALL                  0
-                36 CALL                     0
-                46 STORE_NAME               4 (register)
-   
-     6          48 LOAD_CONST               2 (1)
-                50 STORE_NAME               5 (MIN_SIZE)
-   
-     7          52 LOAD_CONST               3 (6)
-                54 STORE_NAME               6 (MAX_SIZE)
-   
-     9          56 LOAD_NAME                4 (register)
-                58 LOAD_METHOD              7 (simple_tag)
-                80 LOAD_CONST               4 ('class')
-                82 KW_NAMES                 5
-                84 PRECALL                  1
-                88 CALL                     1
-   
-    10          98 LOAD_CONST               6 ('return')
-               100 LOAD_NAME                8 (str)
-               102 BUILD_TUPLE              2
-               104 LOAD_CONST               7 (<code object class_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\utils.py", line 9>)
-               106 MAKE_FUNCTION            4 (annotations)
-   
-     9         108 PRECALL                  0
-               112 CALL                     0
-   
-    10         122 STORE_NAME               9 (class_tag)
-   
-    16         124 LOAD_NAME                4 (register)
-               126 LOAD_METHOD             10 (filter)
-               148 LOAD_CONST               8 ('add_class')
-               150 KW_NAMES                 5
-               152 PRECALL                  1
-               156 CALL                     1
-   
-    17         166 LOAD_CONST               9 ('value')
-               168 LOAD_NAME                8 (str)
-               170 LOAD_CONST              10 ('adder')
-               172 LOAD_NAME                8 (str)
-               174 LOAD_CONST               6 ('return')
-               176 LOAD_NAME                8 (str)
-               178 BUILD_TUPLE              6
-               180 LOAD_CONST              11 (<code object add_class, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\utils.py", line 16>)
-               182 MAKE_FUNCTION            4 (annotations)
-   
-    16         184 PRECALL                  0
-               188 CALL                     0
-   
-    17         198 STORE_NAME              11 (add_class)
-   
-    26         200 LOAD_NAME                4 (register)
-               202 LOAD_METHOD             10 (filter)
-               224 LOAD_CONST              12 ('heading')
-               226 KW_NAMES                 5
-               228 PRECALL                  1
-               232 CALL                     1
-   
-    27         242 LOAD_CONST               9 ('value')
-               244 LOAD_NAME                8 (str)
-               246 LOAD_CONST              10 ('adder')
-               248 LOAD_NAME               12 (int)
-               250 LOAD_CONST               6 ('return')
-               252 LOAD_NAME                8 (str)
-               254 BUILD_TUPLE              6
-               256 LOAD_CONST              13 (<code object heading, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\utils.py", line 26>)
-               258 MAKE_FUNCTION            4 (annotations)
-   
-    26         260 PRECALL                  0
-               264 CALL                     0
-   
-    27         274 STORE_NAME              13 (heading)
-               276 LOAD_CONST              14 (None)
-               278 RETURN_VALUE
+     2          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('reverse',))
+                22 IMPORT_NAME              3 (django.urls)
+                24 IMPORT_FROM              4 (reverse)
+                26 STORE_NAME               4 (reverse)
+                28 POP_TOP
+   
+     3          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('HttpRequest',))
+                34 IMPORT_NAME              5 (django.http)
+                36 IMPORT_FROM              6 (HttpRequest)
+                38 STORE_NAME               6 (HttpRequest)
+                40 POP_TOP
+   
+     4          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               4 (('mark_safe',))
+                46 IMPORT_NAME              7 (django.utils.safestring)
+                48 IMPORT_FROM              8 (mark_safe)
+                50 STORE_NAME               8 (mark_safe)
+                52 POP_TOP
+   
+     5          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('Page', 'PAGE_TEMPLATE_VAR'))
+                58 IMPORT_NAME              9 (wagtail.models)
+                60 IMPORT_FROM             10 (Page)
+                62 STORE_NAME              10 (Page)
+                64 IMPORT_FROM             11 (PAGE_TEMPLATE_VAR)
+                66 STORE_NAME              11 (PAGE_TEMPLATE_VAR)
+                68 POP_TOP
+   
+     7          70 PUSH_NULL
+                72 LOAD_NAME                1 (library)
+                74 LOAD_ATTR               12 (Library)
+                84 PRECALL                  0
+                88 CALL                     0
+                98 STORE_NAME              13 (register)
+   
+    10         100 LOAD_CONST               6 (1)
+               102 STORE_NAME              14 (MIN_SIZE)
+   
+    11         104 LOAD_CONST               7 (6)
+               106 STORE_NAME              15 (MAX_SIZE)
+   
+    13         108 LOAD_NAME               13 (register)
+               110 LOAD_METHOD             16 (simple_tag)
+               132 LOAD_CONST               8 ('class')
+               134 KW_NAMES                 9
+               136 PRECALL                  1
+               140 CALL                     1
+   
+    14         150 LOAD_CONST              10 ('return')
+               152 LOAD_NAME               17 (str)
+               154 BUILD_TUPLE              2
+               156 LOAD_CONST              11 (<code object class_tag, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\utils.py", line 13>)
+               158 MAKE_FUNCTION            4 (annotations)
+   
+    13         160 PRECALL                  0
+               164 CALL                     0
+   
+    14         174 STORE_NAME              18 (class_tag)
+   
+    20         176 LOAD_NAME               13 (register)
+               178 LOAD_METHOD             19 (filter)
+               200 LOAD_CONST              12 ('add_class')
+               202 KW_NAMES                 9
+               204 PRECALL                  1
+               208 CALL                     1
+   
+    21         218 LOAD_CONST              13 ('value')
+               220 LOAD_NAME               17 (str)
+               222 LOAD_CONST              14 ('adder')
+               224 LOAD_NAME               17 (str)
+               226 LOAD_CONST              10 ('return')
+               228 LOAD_NAME               17 (str)
+               230 BUILD_TUPLE              6
+               232 LOAD_CONST              15 (<code object add_class, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\utils.py", line 20>)
+               234 MAKE_FUNCTION            4 (annotations)
+   
+    20         236 PRECALL                  0
+               240 CALL                     0
+   
+    21         250 STORE_NAME              20 (add_class)
+   
+    30         252 LOAD_NAME               13 (register)
+               254 LOAD_METHOD             19 (filter)
+               276 LOAD_CONST              16 ('heading')
+               278 KW_NAMES                 9
+               280 PRECALL                  1
+               284 CALL                     1
+   
+    31         294 LOAD_CONST              13 ('value')
+               296 LOAD_NAME               17 (str)
+               298 LOAD_CONST              14 ('adder')
+               300 LOAD_NAME               21 (int)
+               302 LOAD_CONST              10 ('return')
+               304 LOAD_NAME               17 (str)
+               306 BUILD_TUPLE              6
+               308 LOAD_CONST              17 (<code object heading, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\globlocks\templatetags\globlocks\utils.py", line 30>)
+               310 MAKE_FUNCTION            4 (annotations)
+   
+    30         312 PRECALL                  0
+               316 CALL                     0
+   
+    31         326 STORE_NAME              22 (heading)
+               328 LOAD_CONST              18 (None)
+               330 RETURN_VALUE
    consts
       0
       ('library', 'TemplateSyntaxError')
+      ('reverse',)
+      ('HttpRequest',)
+      ('mark_safe',)
+      ('Page', 'PAGE_TEMPLATE_VAR')
       1
       6
       'class'
       ('name',)
       'return'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 3
          flags     : 7
          code
             0x97006401a00000000000000000000000000000000000000000007c00a6
             010000ab0100000000000000005300
-           9           0 RESUME                   0
+          13           0 RESUME                   0
          
-          14           2 LOAD_CONST               1 (' ')
+          18           2 LOAD_CONST               1 (' ')
                        4 LOAD_METHOD              0 (join)
                       26 LOAD_FAST                0 (args)
                       28 PRECALL                  1
                       32 CALL                     1
                       42 RETURN_VALUE
          consts
             '\n        Helper tag for joining classes together.\n    '
             ' '
          names      ('join',)
          varnames   ('args',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\utils.py'
          name       'class_tag'
-         firstlineno 9
+         firstlineno 13
          lnotab 0x0205
       'add_class'
       'value'
       'adder'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007c00730f7401000000000000000000006401a6010000ab01000000
             000000000082017c009b0064027c019b009d035300
-          16           0 RESUME                   0
+          20           0 RESUME                   0
          
-          21           2 LOAD_FAST                0 (value)
+          25           2 LOAD_FAST                0 (value)
                        4 POP_JUMP_FORWARD_IF_TRUE    15 (to 36)
          
-          22           6 LOAD_GLOBAL              1 (NULL + TemplateSyntaxError)
+          26           6 LOAD_GLOBAL              1 (NULL + TemplateSyntaxError)
                       18 LOAD_CONST               1 ('add_class tag requires a value')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 RAISE_VARARGS            1
          
-          24     >>   36 LOAD_FAST                0 (value)
+          28     >>   36 LOAD_FAST                0 (value)
                       38 FORMAT_VALUE             0
                       40 LOAD_CONST               2 (' ')
                       42 LOAD_FAST                1 (adder)
                       44 FORMAT_VALUE             0
                       46 BUILD_STRING             3
                       48 RETURN_VALUE
          consts
@@ -174,15 +210,15 @@
             ' '
          names      ('TemplateSyntaxError',)
          varnames   ('value', 'adder')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\utils.py'
          name       'add_class'
-         firstlineno 16
+         firstlineno 20
          lnotab 0x020504011e02
       'heading'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
@@ -194,94 +230,94 @@
             0a7c00640364048502190000000000000000007d00090074090000000000
             00000000007c00a6010000ab0100000000000000007d006e1d2300740a00
             0000000000000000002400721001007401000000000000000000006405a6
             010000ab010000000000000000820177007803590077017c007c017a0d00
             007d007c00740c000000000000000000006b00000000007208740c000000
             000000000000007d006e127c00740e000000000000000000006b04000000
             007207740e000000000000000000007d0064027c009b009d025300
-          26           0 RESUME                   0
+          30           0 RESUME                   0
          
-          31           2 LOAD_FAST                0 (value)
+          35           2 LOAD_FAST                0 (value)
                        4 POP_JUMP_FORWARD_IF_TRUE    15 (to 36)
          
-          32           6 LOAD_GLOBAL              1 (NULL + TemplateSyntaxError)
+          36           6 LOAD_GLOBAL              1 (NULL + TemplateSyntaxError)
                       18 LOAD_CONST               1 ('heading tag requires a value')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 RAISE_VARARGS            1
          
-          34     >>   36 LOAD_GLOBAL              3 (NULL + isinstance)
+          38     >>   36 LOAD_GLOBAL              3 (NULL + isinstance)
                       48 LOAD_FAST                0 (value)
                       50 LOAD_GLOBAL              4 (str)
                       62 PRECALL                  2
                       66 CALL                     2
                       76 POP_JUMP_FORWARD_IF_FALSE    31 (to 140)
                       78 LOAD_FAST                0 (value)
                       80 LOAD_METHOD              3 (startswith)
                      102 LOAD_CONST               2 ('h')
                      104 PRECALL                  1
                      108 CALL                     1
                      118 POP_JUMP_FORWARD_IF_FALSE    10 (to 140)
          
-          35         120 LOAD_FAST                0 (value)
+          39         120 LOAD_FAST                0 (value)
                      122 LOAD_CONST               3 (1)
                      124 LOAD_CONST               4 (None)
                      126 BUILD_SLICE              2
                      128 BINARY_SUBSCR
                      138 STORE_FAST               0 (value)
          
-          37     >>  140 NOP
+          41     >>  140 NOP
          
-          38         142 LOAD_GLOBAL              9 (NULL + int)
+          42         142 LOAD_GLOBAL              9 (NULL + int)
                      154 LOAD_FAST                0 (value)
                      156 PRECALL                  1
                      160 CALL                     1
                      170 STORE_FAST               0 (value)
                      172 JUMP_FORWARD            29 (to 232)
                  >>  174 PUSH_EXC_INFO
          
-          39         176 LOAD_GLOBAL             10 (ValueError)
+          43         176 LOAD_GLOBAL             10 (ValueError)
                      188 CHECK_EXC_MATCH
                      190 POP_JUMP_FORWARD_IF_FALSE    16 (to 224)
                      192 POP_TOP
          
-          40         194 LOAD_GLOBAL              1 (NULL + TemplateSyntaxError)
+          44         194 LOAD_GLOBAL              1 (NULL + TemplateSyntaxError)
                      206 LOAD_CONST               5 ('heading tag requires a number')
                      208 PRECALL                  1
                      212 CALL                     1
                      222 RAISE_VARARGS            1
          
-          39     >>  224 RERAISE                  0
+          43     >>  224 RERAISE                  0
                  >>  226 COPY                     3
                      228 POP_EXCEPT
                      230 RERAISE                  1
          
-          42     >>  232 LOAD_FAST                0 (value)
+          46     >>  232 LOAD_FAST                0 (value)
                      234 LOAD_FAST                1 (adder)
                      236 BINARY_OP               13 (+=)
                      240 STORE_FAST               0 (value)
          
-          44         242 LOAD_FAST                0 (value)
+          48         242 LOAD_FAST                0 (value)
                      244 LOAD_GLOBAL             12 (MIN_SIZE)
                      256 COMPARE_OP               0 (<)
                      262 POP_JUMP_FORWARD_IF_FALSE     8 (to 280)
          
-          45         264 LOAD_GLOBAL             12 (MIN_SIZE)
+          49         264 LOAD_GLOBAL             12 (MIN_SIZE)
                      276 STORE_FAST               0 (value)
                      278 JUMP_FORWARD            18 (to 316)
          
-          46     >>  280 LOAD_FAST                0 (value)
+          50     >>  280 LOAD_FAST                0 (value)
                      282 LOAD_GLOBAL             14 (MAX_SIZE)
                      294 COMPARE_OP               4 (>)
                      300 POP_JUMP_FORWARD_IF_FALSE     7 (to 316)
          
-          47         302 LOAD_GLOBAL             14 (MAX_SIZE)
+          51         302 LOAD_GLOBAL             14 (MAX_SIZE)
                      314 STORE_FAST               0 (value)
          
-          49     >>  316 LOAD_CONST               2 ('h')
+          53     >>  316 LOAD_CONST               2 ('h')
                      318 LOAD_FAST                0 (value)
                      320 FORMAT_VALUE             0
                      322 BUILD_STRING             2
                      324 RETURN_VALUE
          ExceptionTable:
            142 to 170 -> 174 [0]
            174 to 224 -> 226 [1] lasti
@@ -294,22 +330,22 @@
             'heading tag requires a number'
          names      ('TemplateSyntaxError', 'isinstance', 'str', 'startswith', 'int', 'ValueError', 'MIN_SIZE', 'MAX_SIZE')
          varnames   ('value', 'adder')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\utils.py'
          name       'heading'
-         firstlineno 26
+         firstlineno 30
          lnotab
             0x020504011e02540114020201220112011eff08030a021601100116010e
             02
       None
-   names      ('django.template', 'library', 'TemplateSyntaxError', 'Library', 'register', 'MIN_SIZE', 'MAX_SIZE', 'simple_tag', 'str', 'class_tag', 'filter', 'add_class', 'int', 'heading')
+   names      ('django.template', 'library', 'TemplateSyntaxError', 'django.urls', 'reverse', 'django.http', 'HttpRequest', 'django.utils.safestring', 'mark_safe', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'Library', 'register', 'MIN_SIZE', 'MAX_SIZE', 'simple_tag', 'str', 'class_tag', 'filter', 'add_class', 'int', 'heading')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\globlocks\\templatetags\\globlocks\\utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110021e03040104022a010aff0e0102062a0112ff0e0102092a
-      0112ff0e01
+      0x00ff020110010c010c010c0110021e03040104022a010aff0e0102062a
+      0112ff0e0102092a0112ff0e01
```

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/admin.py` & `globlocks-1.2.1/globlocks/templatetags/globlocks/admin.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templatetags/globlocks/toolbar.py` & `globlocks-1.2.1/globlocks/templatetags/globlocks/toolbar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/templatetags/orderable_tags.py` & `globlocks-1.2.1/globlocks/templatetags/orderable_tags.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/util.py` & `globlocks-1.2.1/globlocks/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         except AttributeError:
             try:
                 return obj.json()
             except AttributeError:
                 try:
                     return super().default(obj)
                 except Exception as e:
-                    raise Exception(f"Could not serialize {obj} to JSON") from e
+                    raise Exception(f"Could not serialize {obj} ({type(obj)}) to JSON") from e
                 
 
 def get_hooks(hook_name: str):
     """
         Helper function to get hooks from the wagtail hooks registry.
         Namespaced to the globlocks app.
     """
```

### Comparing `globlocks-1.2.0/globlocks/wagtail_hooks/alignment.py` & `globlocks-1.2.1/globlocks/wagtail_hooks/alignment.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/wagtail_hooks/icons.py` & `globlocks-1.2.1/globlocks/wagtail_hooks/icons.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/wagtail_hooks/rt_extensions.py` & `globlocks-1.2.1/globlocks/wagtail_hooks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/widgets/color_input_widget.py` & `globlocks-1.2.1/globlocks/widgets/color_input_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/widgets/fontpicker.py` & `globlocks-1.2.1/globlocks/widgets/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/widgets/justify_widget.py` & `globlocks-1.2.1/globlocks/widgets/justify_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/widgets/orderable.py` & `globlocks-1.2.1/globlocks/widgets/orderable.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks/widgets/range_input.py` & `globlocks-1.2.1/globlocks/widgets/range_input.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/globlocks.egg-info/PKG-INFO` & `globlocks-1.2.1/globlocks.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globlocks
-Version: 1.2.0
+Version: 1.2.1
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/globlocks
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -65,7 +65,34 @@
    INSTALLED_APPS = [
        ...,
        'globlocks',
        'conditional_field',
    ]
    ```
 2. ...
+
+## Richtext Alignment
+
+`globlocks` has a richtext feature for text alignment; without the limits that feature would normally impose.
+
+*Normally* - headings would not be able to get aligned. **This is a problem.**
+
+Luckily, we have the solution! *And you can use it too!*
+
+**To add the alignment features to your richtext**
+
+1. Follow the installation steps for `globlocks`.
+2. Add `text-alignment` to your richtext features. (it is included in default features)
+
+To align it on the frontend too; add the following CSS:
+
+```css
+.text-left {
+    text-align: left;
+}
+.text-center{
+    text-align: center;
+}
+.text-right {
+    text-align: right;
+}
+```
```

### Comparing `globlocks-1.2.0/globlocks.egg-info/SOURCES.txt` & `globlocks-1.2.1/globlocks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,17 @@
 globlocks/blocks/components/menus/__init__.py
 globlocks/blocks/components/menus/flat.py
 globlocks/blocks/components/menus/layered.py
 globlocks/fields/__init__.py
 globlocks/fields/colorfield.py
 globlocks/fields/fontfield.py
 globlocks/fields/orderablefield.py
+globlocks/locale/en/LC_MESSAGES/django.mo
 globlocks/locale/en/LC_MESSAGES/django.po
+globlocks/locale/nl/LC_MESSAGES/django.mo
 globlocks/locale/nl/LC_MESSAGES/django.po
 globlocks/static/globlocks/admin/block_settings.js
 globlocks/static/globlocks/admin/layout.css
 globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
 globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
 globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
 globlocks/static/globlocks/css/blocks.css
```

### Comparing `globlocks-1.2.0/setup.cfg` & `globlocks-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6c6f 626c 6f63 6b73 0d0a 7665   = globlocks..ve
-00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a64  rsion = 1.2.0..d
+00000020: 7273 696f 6e20 3d20 312e 322e 310d 0a64  rsion = 1.2.1..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2041 6e20  escription = An 
 00000040: 6170 706c 6963 6174 696f 6e20 6d61 6465  application made
 00000050: 2066 6f72 2074 6865 2044 6a61 6e67 6f20   for the Django 
 00000060: 5765 6220 4672 616d 6577 6f72 6b2e 0d0a  Web Framework...
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
```

### Comparing `globlocks-1.2.0/tests/testapp/manage.py` & `globlocks-1.2.1/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/tests/testapp/testapp/settings.py` & `globlocks-1.2.1/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.2.0/tests/testapp/testapp/urls.py` & `globlocks-1.2.1/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

