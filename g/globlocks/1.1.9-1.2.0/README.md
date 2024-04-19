# Comparing `tmp/globlocks-1.1.9.tar.gz` & `tmp/globlocks-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globlocks-1.1.9.tar", last modified: Fri Apr 19 07:11:30 2024, max compression
+gzip compressed data, was "globlocks-1.2.0.tar", last modified: Fri Apr 19 07:16:01 2024, max compression
```

## Comparing `globlocks-1.1.9.tar` & `globlocks-1.2.0.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.214935 globlocks-1.1.9/
--rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.1.9/LICENSE
--rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1984 2024-04-19 07:11:30.214935 globlocks-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      901 2024-03-19 08:19:55.000000 globlocks-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.429346 globlocks-1.1.9/globlocks/
--rw-rw-rw-   0        0        0      620 2024-04-19 07:11:25.000000 globlocks-1.1.9/globlocks/__init__.py
--rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.461919 globlocks-1.1.9/globlocks/blocks/
--rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.471404 globlocks-1.1.9/globlocks/blocks/bases/
--rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/__init__.py
--rw-rw-rw-   0        0        0    13076 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/baseblock.py
--rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/template.py
--rw-rw-rw-   0        0        0    10194 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/bases/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.477592 globlocks-1.1.9/globlocks/blocks/block_fields/
--rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.480871 globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/
--rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/__init__.py
--rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/colorblock.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.481524 globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/
--rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/__init__.py
--rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/fontpicker.py
--rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/justify.py
--rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/orderable_block.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.488776 globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/
--rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/__init__.py
--rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/rangeslider.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.500032 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/
--rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/__init__.py
--rw-rw-rw-   0        0        0     4956 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/bar.py
--rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/element.py
--rw-rw-rw-   0        0        0      774 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_field.py
--rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
--rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.508710 globlocks-1.1.9/globlocks/blocks/components/
--rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/__init__.py
--rw-rw-rw-   0        0        0     1603 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/heading.py
--rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/image.py
--rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/image_text.py
--rw-rw-rw-   0        0        0     9047 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/link.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.513187 globlocks-1.1.9/globlocks/blocks/components/menus/
--rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/menus/__init__.py
--rw-rw-rw-   0        0        0     2567 2024-03-19 09:11:52.000000 globlocks-1.1.9/globlocks/blocks/components/menus/flat.py
--rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/menus/layered.py
--rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/components/text.py
--rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/richtext.py
--rw-rw-rw-   0        0        0      425 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/blocks/utils.py
--rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/choices.py
--rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/colors.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.520328 globlocks-1.1.9/globlocks/fields/
--rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/__init__.py
--rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/colorfield.py
--rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/fontfield.py
--rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fields/orderablefield.py
--rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/fonts.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.341140 globlocks-1.1.9/globlocks/locale/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.340140 globlocks-1.1.9/globlocks/locale/en/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.532263 globlocks-1.1.9/globlocks/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.342137 globlocks-1.1.9/globlocks/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.546064 globlocks-1.1.9/globlocks/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3549 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/panels.py
--rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/preview.py
--rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/rt_extensions.py
--rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.343141 globlocks-1.1.9/globlocks/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.351616 globlocks-1.1.9/globlocks/static/globlocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.583064 globlocks-1.1.9/globlocks/static/globlocks/admin/
--rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/block_settings.js
--rw-rw-rw-   0        0        0    24293 2024-03-26 09:23:48.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/layout.css
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.622376 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/
--rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
--rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
--rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.645282 globlocks-1.1.9/globlocks/static/globlocks/css/
--rw-rw-rw-   0        0        0     8847 2024-03-19 12:00:45.000000 globlocks-1.1.9/globlocks/static/globlocks/css/blocks.css
--rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.1.9/globlocks/static/globlocks/css/bootstrap.css
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.113700 globlocks-1.1.9/globlocks/static/globlocks/fonts/
--rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Acme-Regular.ttf
--rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
--rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
--rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
--rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
--rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
--rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
--rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
--rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
--rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Inter-Regular.ttf
--rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
--rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
--rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Lato-Regular.ttf
--rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
--rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
--rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
--rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
--rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
--rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
--rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
--rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
--rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
--rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
--rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
--rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
--rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
--rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
--rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
--rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
--rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
--rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
--rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
--rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
--rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
--rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
--rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
--rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
--rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
--rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
--rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.349109 globlocks-1.1.9/globlocks/static/globlocks/richtext/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.132649 globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/
--rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.css
--rw-rw-rw-   0        0        0     5728 2024-04-19 07:10:50.000000 globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.143434 globlocks-1.1.9/globlocks/static/globlocks/richtext/rt_extensions/
--rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.163953 globlocks-1.1.9/globlocks/static/globlocks/widgets/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.289623 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/
--rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/LICENSE
--rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
--rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:49.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
--rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.css
--rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.341792 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/
--rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
--rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
--rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker.css
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.381066 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/
--rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-controller.js
--rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.css
--rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.473830 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/
--rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
--rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.css
--rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.js
--rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.515906 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/
--rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
--rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.css
--rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.js
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.574915 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/
--rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
--rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
--rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
--rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/static/globlocks/widgets/utils.js
--rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.1.9/globlocks/staticfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.375470 globlocks-1.1.9/globlocks/templates/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.373466 globlocks-1.1.9/globlocks/templates/globlocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.368673 globlocks-1.1.9/globlocks/templates/globlocks/blocks/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.367662 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.576258 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/heading/
--rw-rw-rw-   0        0        0      257 2024-03-19 10:10:04.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/heading/heading.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.625806 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/
--rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/full.html
--rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/large.html
--rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/medium.html
--rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image/small.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.664260 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/
--rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image.html
--rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
--rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
--rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.677406 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/link/
--rw-rw-rw-   0        0        0     1655 2024-03-19 08:35:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/link/form.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.366211 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.722663 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/
--rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
--rw-rw-rw-   0        0        0      555 2024-03-19 10:14:53.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
--rw-rw-rw-   0        0        0      908 2024-03-19 10:29:01.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
--rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.732600 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/text/
--rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/text/text_block.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.808965 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/
--rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/heading.html
--rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
--rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/listblock.html
--rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/richtext.html
--rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/settings_form.html
--rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
--rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.369648 globlocks-1.1.9/globlocks/templates/globlocks/icons/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.848629 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/
--rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-center.svg
--rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-justify.svg
--rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-left.svg
--rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/text-align/text-right.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:29.971562 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/
--rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
--rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
--rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
--rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
--rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
--rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
--rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
--rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
--rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
--rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
--rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
--rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.372471 globlocks-1.1.9/globlocks/templates/globlocks/shared/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.010432 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/
--rw-rw-rw-   0        0        0      226 2024-03-19 09:32:33.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/base.html
--rw-rw-rw-   0        0        0      902 2024-03-19 09:26:20.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/heading.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.056198 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/
--rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/base.html
--rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/full.html
--rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/large.html
--rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/medium.html
--rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/images/small.html
--rw-rw-rw-   0        0        0      309 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/listblock.html
--rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/text.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.127220 globlocks-1.1.9/globlocks/templates/globlocks/widgets/
--rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/color-input-widget.html
--rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/font_picker_widget.html
--rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/justify-widget-option.html
--rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/justify-widget.html
--rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/orderable_widget.html
--rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/slider_input.html
--rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/globlocks/widgets/toolbar-widget.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:28.375470 globlocks-1.1.9/globlocks/templates/wagtailadmin/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.164543 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/
--rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block.html
--rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
--rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
--rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/field.html
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.164543 globlocks-1.1.9/globlocks/templatetags/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.171058 globlocks-1.1.9/globlocks/templatetags/__pycache__/
--rw-rw-rw-   0        0        0     4257 2024-03-19 07:31:29.000000 globlocks-1.1.9/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.175860 globlocks-1.1.9/globlocks/templatetags/globlocks/
--rw-rw-rw-   0        0        0     6627 2024-03-19 09:43:06.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.186254 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/
--rw-rw-rw-   0        0        0     9504 2024-03-19 09:43:08.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1469 2024-03-19 07:31:29.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
--rw-rw-rw-   0        0        0     3595 2024-03-19 11:12:51.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
--rw-rw-rw-   0        0        0     2281 2024-03-19 09:18:19.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/admin.py
--rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/toolbar.py
--rw-rw-rw-   0        0        0     1242 2024-03-19 09:18:17.000000 globlocks-1.1.9/globlocks/templatetags/globlocks/utils.py
--rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/templatetags/orderable_tags.py
--rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/tests.py
--rw-rw-rw-   0        0        0     1832 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/util.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.192918 globlocks-1.1.9/globlocks/wagtail_hooks/
--rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/admin_hooks.py
--rw-rw-rw-   0        0        0     4327 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/alignment.py
--rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/wagtail_hooks/rt_extensions.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.198837 globlocks-1.1.9/globlocks/widgets/
--rw-rw-rw-   0        0        0      295 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/color_input_widget.py
--rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/fontpicker.py
--rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/justify_widget.py
--rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/orderable.py
--rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.1.9/globlocks/widgets/range_input.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.214935 globlocks-1.1.9/globlocks.egg-info/
--rw-rw-rw-   0        0        0     1984 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11470 2024-04-19 07:11:28.000000 globlocks-1.1.9/globlocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 07:11:27.000000 globlocks-1.1.9/globlocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.1.9/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2024-04-19 07:11:30.229616 globlocks-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.198837 globlocks-1.1.9/tests/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.205706 globlocks-1.1.9/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.208708 globlocks-1.1.9/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.210371 globlocks-1.1.9/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:11:30.214935 globlocks-1.1.9/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.1.9/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.752883 globlocks-1.2.0/
+-rw-rw-rw-   0        0        0      780 2024-03-12 07:23:28.000000 globlocks-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-03-01 12:36:04.000000 globlocks-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1984 2024-04-19 07:16:01.752883 globlocks-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2024-03-19 08:19:55.000000 globlocks-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.134495 globlocks-1.2.0/globlocks/
+-rw-rw-rw-   0        0        0      620 2024-04-19 07:15:55.000000 globlocks-1.2.0/globlocks/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.217225 globlocks-1.2.0/globlocks/blocks/
+-rw-rw-rw-   0        0        0      591 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.282814 globlocks-1.2.0/globlocks/blocks/bases/
+-rw-rw-rw-   0        0        0      399 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/__init__.py
+-rw-rw-rw-   0        0        0    13076 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/baseblock.py
+-rw-rw-rw-   0        0        0     3594 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/template.py
+-rw-rw-rw-   0        0        0    10194 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/bases/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.310955 globlocks-1.2.0/globlocks/blocks/block_fields/
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.337348 globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/
+-rw-rw-rw-   0        0        0       34 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/__init__.py
+-rw-rw-rw-   0        0        0      778 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/colorblock.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.361510 globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/
+-rw-rw-rw-   0        0        0       39 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/__init__.py
+-rw-rw-rw-   0        0        0     1228 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/fontpicker.py
+-rw-rw-rw-   0        0        0     1017 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/justify.py
+-rw-rw-rw-   0        0        0     2058 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/orderable_block.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.386291 globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/
+-rw-rw-rw-   0        0        0       41 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/__init__.py
+-rw-rw-rw-   0        0        0     1510 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/rangeslider.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.459339 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/
+-rw-rw-rw-   0        0        0      644 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/__init__.py
+-rw-rw-rw-   0        0        0     4956 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/bar.py
+-rw-rw-rw-   0        0        0     4372 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/element.py
+-rw-rw-rw-   0        0        0      774 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_field.py
+-rw-rw-rw-   0        0        0     2651 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_widget.py
+-rw-rw-rw-   0        0        0     5108 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.529148 globlocks-1.2.0/globlocks/blocks/components/
+-rw-rw-rw-   0        0        0      366 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/__init__.py
+-rw-rw-rw-   0        0        0     1603 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/heading.py
+-rw-rw-rw-   0        0        0     1640 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/image.py
+-rw-rw-rw-   0        0        0     2113 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/image_text.py
+-rw-rw-rw-   0        0        0     9047 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/link.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.554771 globlocks-1.2.0/globlocks/blocks/components/menus/
+-rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/menus/__init__.py
+-rw-rw-rw-   0        0        0     2567 2024-03-19 09:11:52.000000 globlocks-1.2.0/globlocks/blocks/components/menus/flat.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/menus/layered.py
+-rw-rw-rw-   0        0        0     1234 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/components/text.py
+-rw-rw-rw-   0        0        0     5408 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/richtext.py
+-rw-rw-rw-   0        0        0      425 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/blocks/utils.py
+-rw-rw-rw-   0        0        0      950 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/choices.py
+-rw-rw-rw-   0        0        0     3134 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.594099 globlocks-1.2.0/globlocks/fields/
+-rw-rw-rw-   0        0        0      154 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/colorfield.py
+-rw-rw-rw-   0        0        0     3568 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/fontfield.py
+-rw-rw-rw-   0        0        0     5396 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fields/orderablefield.py
+-rw-rw-rw-   0        0        0     4533 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/fonts.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.935293 globlocks-1.2.0/globlocks/locale/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.933577 globlocks-1.2.0/globlocks/locale/en/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.605504 globlocks-1.2.0/globlocks/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3183 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.935293 globlocks-1.2.0/globlocks/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.610601 globlocks-1.2.0/globlocks/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3549 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      552 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/panels.py
+-rw-rw-rw-   0        0        0     1682 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/preview.py
+-rw-rw-rw-   0        0        0    10553 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/rt_extensions.py
+-rw-rw-rw-   0        0        0     3108 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.937305 globlocks-1.2.0/globlocks/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.940609 globlocks-1.2.0/globlocks/static/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.639915 globlocks-1.2.0/globlocks/static/globlocks/admin/
+-rw-rw-rw-   0        0        0     1133 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/block_settings.js
+-rw-rw-rw-   0        0        0    24293 2024-03-26 09:23:48.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/layout.css
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.688688 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/
+-rw-rw-rw-   0        0        0     9739 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js
+-rw-rw-rw-   0        0        0     4083 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css
+-rw-rw-rw-   0        0        0     6653 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:59.706876 globlocks-1.2.0/globlocks/static/globlocks/css/
+-rw-rw-rw-   0        0        0     8847 2024-03-19 12:00:45.000000 globlocks-1.2.0/globlocks/static/globlocks/css/blocks.css
+-rw-rw-rw-   0        0        0     9880 2024-03-19 10:21:08.000000 globlocks-1.2.0/globlocks/static/globlocks/css/bootstrap.css
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.200251 globlocks-1.2.0/globlocks/static/globlocks/fonts/
+-rw-rw-rw-   0        0        0    21948 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Acme-Regular.ttf
+-rw-rw-rw-   0        0        0    92956 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf
+-rw-rw-rw-   0        0        0   142696 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf
+-rw-rw-rw-   0        0        0    92468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Bangers-Regular.ttf
+-rw-rw-rw-   0        0        0    57676 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf
+-rw-rw-rw-   0        0        0   256900 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Caveat-Regular.ttf
+-rw-rw-rw-   0        0        0    61368 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Creepster-Regular.ttf
+-rw-rw-rw-   0        0        0    26000 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf
+-rw-rw-rw-   0        0        0    97864 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf
+-rw-rw-rw-   0        0        0   309828 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Inter-Regular.ttf
+-rw-rw-rw-   0        0        0    41676 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf
+-rw-rw-rw-   0        0        0   169744 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Kanit-Regular.ttf
+-rw-rw-rw-   0        0        0    75152 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0        0        0   396740 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Lobster-Regular.ttf
+-rw-rw-rw-   0        0        0   234956 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf
+-rw-rw-rw-   0        0        0    96832 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Manrope-Regular.ttf
+-rw-rw-rw-   0        0        0    49908 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Monoton-Regular.ttf
+-rw-rw-rw-   0        0        0   197976 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf
+-rw-rw-rw-   0        0        0   556216 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf
+-rw-rw-rw-   0        0        0    87252 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0        0        0   169480 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/PTMono-Regular.ttf
+-rw-rw-rw-   0        0        0   315408 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf
+-rw-rw-rw-   0        0        0    33876 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf
+-rw-rw-rw-   0        0        0    73620 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf
+-rw-rw-rw-   0        0        0   109192 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf
+-rw-rw-rw-   0        0        0    65396 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Phudu-Regular.ttf
+-rw-rw-rw-   0        0        0   158240 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Poppins-Regular.ttf
+-rw-rw-rw-   0        0        0   168260 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   166836 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf
+-rw-rw-rw-   0        0        0    86908 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0   119328 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf
+-rw-rw-rw-   0        0        0   207632 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Rubik-Regular.ttf
+-rw-rw-rw-   0        0        0   132092 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf
+-rw-rw-rw-   0        0        0   117132 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf
+-rw-rw-rw-   0        0        0    64808 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf
+-rw-rw-rw-   0        0        0    48468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf
+-rw-rw-rw-   0        0        0    42756 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf
+-rw-rw-rw-   0        0        0    90904 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf
+-rw-rw-rw-   0        0        0    40160 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf
+-rw-rw-rw-   0        0        0   299684 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf
+-rw-rw-rw-   0        0        0    51084 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Ultra-Regular.ttf
+-rw-rw-rw-   0        0        0   244332 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0   192904 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf
+-rw-rw-rw-   0        0        0    57468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.940609 globlocks-1.2.0/globlocks/static/globlocks/richtext/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.239068 globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/
+-rw-rw-rw-   0        0        0      558 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.css
+-rw-rw-rw-   0        0        0     5728 2024-04-19 07:10:50.000000 globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.257279 globlocks-1.2.0/globlocks/static/globlocks/richtext/rt_extensions/
+-rw-rw-rw-   0        0        0     1920 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.275789 globlocks-1.2.0/globlocks/static/globlocks/widgets/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.433244 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/
+-rw-rw-rw-   0        0        0     1097 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/LICENSE
+-rw-rw-rw-   0        0        0      503 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/color-input-widget-telepath.js
+-rw-rw-rw-   0        0        0     3612 2024-03-26 09:19:49.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/color-input-widget.js
+-rw-rw-rw-   0        0        0     9003 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.css
+-rw-rw-rw-   0        0        0    23558 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.483286 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/
+-rw-rw-rw-   0        0        0      581 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js
+-rw-rw-rw-   0        0        0     3307 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js
+-rw-rw-rw-   0        0        0     1070 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker.css
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.533371 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/
+-rw-rw-rw-   0        0        0      577 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-controller.js
+-rw-rw-rw-   0        0        0     2147 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.css
+-rw-rw-rw-   0        0        0     4548 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.633022 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/
+-rw-rw-rw-   0        0        0      516 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js
+-rw-rw-rw-   0        0        0      800 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.css
+-rw-rw-rw-   0        0        0     2222 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.js
+-rw-rw-rw-   0        0        0    44137 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.704619 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/
+-rw-rw-rw-   0        0        0      578 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js
+-rw-rw-rw-   0        0        0     1152 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.css
+-rw-rw-rw-   0        0        0     2164 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.js
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.758651 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/
+-rw-rw-rw-   0        0        0      970 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js
+-rw-rw-rw-   0        0        0      810 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css
+-rw-rw-rw-   0        0        0    16968 2024-03-19 08:44:23.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js
+-rw-rw-rw-   0        0        0      796 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/static/globlocks/widgets/utils.js
+-rw-rw-rw-   0        0        0      380 2024-03-19 10:21:19.000000 globlocks-1.2.0/globlocks/staticfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.955478 globlocks-1.2.0/globlocks/templates/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.955478 globlocks-1.2.0/globlocks/templates/globlocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.950029 globlocks-1.2.0/globlocks/templates/globlocks/blocks/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.949054 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.770710 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/heading/
+-rw-rw-rw-   0        0        0      257 2024-03-19 10:10:04.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/heading/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.809821 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/
+-rw-rw-rw-   0        0        0       78 2024-03-19 11:05:19.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/full.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:29.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/large.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 11:23:32.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/medium.html
+-rw-rw-rw-   0        0        0      113 2024-03-19 11:23:34.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image/small.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.860553 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/
+-rw-rw-rw-   0        0        0      350 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image.html
+-rw-rw-rw-   0        0        0      376 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image_text.html
+-rw-rw-rw-   0        0        0      588 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html
+-rw-rw-rw-   0        0        0      387 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.870458 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/link/
+-rw-rw-rw-   0        0        0     1655 2024-03-19 08:35:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/link/form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.943691 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.923598 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/
+-rw-rw-rw-   0        0        0      306 2024-03-19 10:28:33.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/horizontal.html
+-rw-rw-rw-   0        0        0      555 2024-03-19 10:14:53.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/item.html
+-rw-rw-rw-   0        0        0      908 2024-03-19 10:29:01.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html
+-rw-rw-rw-   0        0        0      105 2024-03-19 09:29:51.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/vertical.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:00.938210 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/text/
+-rw-rw-rw-   0        0        0      118 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/text/text_block.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.015092 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/
+-rw-rw-rw-   0        0        0      221 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/heading.html
+-rw-rw-rw-   0        0        0      355 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/heading_settings_form.html
+-rw-rw-rw-   0        0        0      114 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/listblock.html
+-rw-rw-rw-   0        0        0      241 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/richtext.html
+-rw-rw-rw-   0        0        0      238 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/settings_form.html
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/text_and_settings_form.html
+-rw-rw-rw-   0        0        0      361 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/blocks/richtext/text_settings_form.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.953021 globlocks-1.2.0/globlocks/templates/globlocks/icons/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.064990 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/
+-rw-rw-rw-   0        0        0      465 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-center.svg
+-rw-rw-rw-   0        0        0      468 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-justify.svg
+-rw-rw-rw-   0        0        0      461 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-left.svg
+-rw-rw-rw-   0        0        0      464 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/text-align/text-right.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.191760 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/
+-rw-rw-rw-   0        0        0      549 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-bold.svg
+-rw-rw-rw-   0        0        0      338 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h1.svg
+-rw-rw-rw-   0        0        0      546 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h2.svg
+-rw-rw-rw-   0        0        0      711 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h3.svg
+-rw-rw-rw-   0        0        0      430 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h4.svg
+-rw-rw-rw-   0        0        0      596 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h5.svg
+-rw-rw-rw-   0        0        0      712 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h6.svg
+-rw-rw-rw-   0        0        0      426 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-italic.svg
+-rw-rw-rw-   0        0        0      542 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg
+-rw-rw-rw-   0        0        0      872 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette.svg
+-rw-rw-rw-   0        0        0      654 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg
+-rw-rw-rw-   0        0        0      409 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-underline.svg
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.954018 globlocks-1.2.0/globlocks/templates/globlocks/shared/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.238160 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/
+-rw-rw-rw-   0        0        0      226 2024-03-19 09:32:33.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/base.html
+-rw-rw-rw-   0        0        0      902 2024-03-19 09:26:20.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/heading.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.292489 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/
+-rw-rw-rw-   0        0        0      323 2024-03-19 11:29:35.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/base.html
+-rw-rw-rw-   0        0        0      240 2024-03-19 11:29:30.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/full.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:27.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/large.html
+-rw-rw-rw-   0        0        0      243 2024-03-19 11:29:19.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/medium.html
+-rw-rw-rw-   0        0        0      242 2024-03-19 11:29:24.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/images/small.html
+-rw-rw-rw-   0        0        0      309 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/listblock.html
+-rw-rw-rw-   0        0        0      317 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/text.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.374821 globlocks-1.2.0/globlocks/templates/globlocks/widgets/
+-rw-rw-rw-   0        0        0      363 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/color-input-widget.html
+-rw-rw-rw-   0        0        0     1999 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/font_picker_widget.html
+-rw-rw-rw-   0        0        0      487 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/justify-widget-option.html
+-rw-rw-rw-   0        0        0      421 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/justify-widget.html
+-rw-rw-rw-   0        0        0      624 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/orderable_widget.html
+-rw-rw-rw-   0        0        0      873 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/slider_input.html
+-rw-rw-rw-   0        0        0     1052 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/globlocks/widgets/toolbar-widget.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:15:58.955478 globlocks-1.2.0/globlocks/templates/wagtailadmin/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.418912 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/
+-rw-rw-rw-   0        0        0      794 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_field.html
+-rw-rw-rw-   0        0        0       46 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_settings_field.html
+-rw-rw-rw-   0        0        0     1208 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-rw-   0        0        0      531 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/field.html
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.433614 globlocks-1.2.0/globlocks/templatetags/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.435567 globlocks-1.2.0/globlocks/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0     4257 2024-03-19 07:31:29.000000 globlocks-1.2.0/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.492902 globlocks-1.2.0/globlocks/templatetags/globlocks/
+-rw-rw-rw-   0        0        0     6627 2024-03-19 09:43:06.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.506522 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/
+-rw-rw-rw-   0        0        0     9504 2024-03-19 09:43:08.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1469 2024-03-19 07:31:29.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3595 2024-03-19 11:12:51.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2281 2024-03-19 09:18:19.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0      886 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/admin.py
+-rw-rw-rw-   0        0        0     2273 2024-03-19 11:06:54.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/toolbar.py
+-rw-rw-rw-   0        0        0     1242 2024-03-19 09:18:17.000000 globlocks-1.2.0/globlocks/templatetags/globlocks/utils.py
+-rw-rw-rw-   0        0        0     2463 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/templatetags/orderable_tags.py
+-rw-rw-rw-   0        0        0       63 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/tests.py
+-rw-rw-rw-   0        0        0     1832 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.576413 globlocks-1.2.0/globlocks/wagtail_hooks/
+-rw-rw-rw-   0        0        0       84 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/admin_hooks.py
+-rw-rw-rw-   0        0        0     4327 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/alignment.py
+-rw-rw-rw-   0        0        0      955 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     1511 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/wagtail_hooks/rt_extensions.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.667055 globlocks-1.2.0/globlocks/widgets/
+-rw-rw-rw-   0        0        0      295 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/color_input_widget.py
+-rw-rw-rw-   0        0        0     3341 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/fontpicker.py
+-rw-rw-rw-   0        0        0     1620 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/justify_widget.py
+-rw-rw-rw-   0        0        0     1898 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/orderable.py
+-rw-rw-rw-   0        0        0     1692 2024-03-19 07:31:28.000000 globlocks-1.2.0/globlocks/widgets/range_input.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.748890 globlocks-1.2.0/globlocks.egg-info/
+-rw-rw-rw-   0        0        0     1984 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11470 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 07:15:58.000000 globlocks-1.2.0/globlocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2024-03-01 12:36:04.000000 globlocks-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2024-04-19 07:16:01.764573 globlocks-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-01 12:36:04.000000 globlocks-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.667989 globlocks-1.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.682543 globlocks-1.2.0/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.692248 globlocks-1.2.0/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.692248 globlocks-1.2.0/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:01.742891 globlocks-1.2.0/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3505 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-03-01 12:36:04.000000 globlocks-1.2.0/tests/testapp/testapp/wsgi.py
```

### Comparing `globlocks-1.1.9/LICENSE` & `globlocks-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/PKG-INFO` & `globlocks-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globlocks
-Version: 1.1.9
+Version: 1.2.0
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/globlocks
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `globlocks-1.1.9/README.md` & `globlocks-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/__init__.py` & `globlocks-1.2.0/globlocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/__init__.py` & `globlocks-1.2.0/globlocks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/bases/baseblock.py` & `globlocks-1.2.0/globlocks/blocks/bases/baseblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/bases/template.py` & `globlocks-1.2.0/globlocks/blocks/bases/template.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/bases/visibility.py` & `globlocks-1.2.0/globlocks/blocks/bases/visibility.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/colorblock/colorblock.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/colorblock/colorblock.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/fontpicker/fontpicker.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/fontpicker/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/justify.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/justify.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/orderable_block.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/orderable_block.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/rangeslider/rangeslider.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/rangeslider/rangeslider.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/__init__.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/bar.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/bar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/element.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/element.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_field.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_field.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/toolbar_widget.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/toolbar_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/block_fields/toolbar/tools.py` & `globlocks-1.2.0/globlocks/blocks/block_fields/toolbar/tools.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/components/heading.py` & `globlocks-1.2.0/globlocks/blocks/components/heading.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/components/image.py` & `globlocks-1.2.0/globlocks/blocks/components/image.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/components/image_text.py` & `globlocks-1.2.0/globlocks/blocks/components/image_text.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/components/link.py` & `globlocks-1.2.0/globlocks/blocks/components/link.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/components/menus/flat.py` & `globlocks-1.2.0/globlocks/blocks/components/menus/flat.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/components/text.py` & `globlocks-1.2.0/globlocks/blocks/components/text.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/blocks/richtext.py` & `globlocks-1.2.0/globlocks/blocks/richtext.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/choices.py` & `globlocks-1.2.0/globlocks/choices.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/colors.py` & `globlocks-1.2.0/globlocks/colors.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/fields/fontfield.py` & `globlocks-1.2.0/globlocks/fields/fontfield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/fields/orderablefield.py` & `globlocks-1.2.0/globlocks/fields/orderablefield.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/fonts.py` & `globlocks-1.2.0/globlocks/fonts.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/locale/en/LC_MESSAGES/django.po` & `globlocks-1.2.0/globlocks/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/locale/nl/LC_MESSAGES/django.po` & `globlocks-1.2.0/globlocks/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/panels.py` & `globlocks-1.2.0/globlocks/panels.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/preview.py` & `globlocks-1.2.0/globlocks/preview.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/rt_extensions.py` & `globlocks-1.2.0/globlocks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/settings.py` & `globlocks-1.2.0/globlocks/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/admin/block_settings.js` & `globlocks-1.2.0/globlocks/static/globlocks/admin/block_settings.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/admin/layout.css` & `globlocks-1.2.0/globlocks/static/globlocks/admin/layout.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js` & `globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block-buttons.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css` & `globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js` & `globlocks-1.2.0/globlocks/static/globlocks/admin/toggleable-block/toggleable-block.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/css/blocks.css` & `globlocks-1.2.0/globlocks/static/globlocks/css/blocks.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/css/bootstrap.css` & `globlocks-1.2.0/globlocks/static/globlocks/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Acme-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Acme-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/AlfaSlabOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/AmaticSC-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Bangers-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Bangers-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/BebasNeue-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Caveat-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Caveat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Creepster-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Creepster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/FugazOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Inter-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Inter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/JuliusSansOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Kanit-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Lato-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Lobster-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Lobster-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/LobsterTwo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Manrope-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Monoton-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Monoton-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Oswald-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/PTMono-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/PTMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Pacifico-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/PatuaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/PermanentMarker-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Philosopher-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Phudu-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Phudu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Poppins-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Roboto-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoCondensed-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/RockSalt-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Rubik-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Rubik-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikIso-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/RubikMonoOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Sacramento-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/ShadowsIntoLight-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/ShareTechMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/StintUltraExpanded-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Ultra-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Ultra-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-Italic-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/VictorMono-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf` & `globlocks-1.2.0/globlocks/static/globlocks/fonts/Zeyada-Regular.ttf`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.css` & `globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/richtext/alignment/alignment.js` & `globlocks-1.2.0/globlocks/static/globlocks/richtext/alignment/alignment.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js` & `globlocks-1.2.0/globlocks/static/globlocks/richtext/rt_extensions/word-counter.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/LICENSE` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/LICENSE`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/color-input-widget.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/color-input-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.css` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/color_input/pickr.min.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/color_input/pickr.min.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/font_picker/font-picker.css` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/font_picker/font-picker.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-controller.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.css` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/justify/justify-widget.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/justify/justify-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.css` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/orderable.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/orderable.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/orderable/sortable.min.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/orderable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider-telepath.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.css` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/range_slider/range-slider.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/range_slider/range-slider.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-controller.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.css`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/toolbar/toolbar-widget.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/static/globlocks/widgets/utils.js` & `globlocks-1.2.0/globlocks/static/globlocks/widgets/utils.js`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html` & `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/image_text/image_text_form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/link/form.html` & `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/link/form.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/item.html` & `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/item.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html` & `globlocks-1.2.0/globlocks/templates/globlocks/blocks/components/menus/flat/menu.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-bold.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-bold.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h2.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h2.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h3.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h3.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h5.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h5.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-h6.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-h6.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette-fill.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-palette.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-palette.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg` & `globlocks-1.2.0/globlocks/templates/globlocks/icons/toolbar/text-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/shared/blocks/heading.html` & `globlocks-1.2.0/globlocks/templates/globlocks/shared/blocks/heading.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/widgets/font_picker_widget.html` & `globlocks-1.2.0/globlocks/templates/globlocks/widgets/font_picker_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/widgets/orderable_widget.html` & `globlocks-1.2.0/globlocks/templates/globlocks/widgets/orderable_widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/widgets/slider_input.html` & `globlocks-1.2.0/globlocks/templates/globlocks/widgets/slider_input.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/globlocks/widgets/toolbar-widget.html` & `globlocks-1.2.0/globlocks/templates/globlocks/widgets/toolbar-widget.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block.html` & `globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templates/wagtailadmin/block_forms/field.html` & `globlocks-1.2.0/globlocks/templates/wagtailadmin/block_forms/field.html`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc` & `globlocks-1.2.0/globlocks/templatetags/__pycache__/orderable_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/__init__.py` & `globlocks-1.2.0/globlocks/templatetags/globlocks/__init__.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc` & `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc` & `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc` & `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/toolbar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc` & `globlocks-1.2.0/globlocks/templatetags/globlocks/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/admin.py` & `globlocks-1.2.0/globlocks/templatetags/globlocks/admin.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/toolbar.py` & `globlocks-1.2.0/globlocks/templatetags/globlocks/toolbar.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/globlocks/utils.py` & `globlocks-1.2.0/globlocks/templatetags/globlocks/utils.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/templatetags/orderable_tags.py` & `globlocks-1.2.0/globlocks/templatetags/orderable_tags.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/util.py` & `globlocks-1.2.0/globlocks/util.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/wagtail_hooks/alignment.py` & `globlocks-1.2.0/globlocks/wagtail_hooks/alignment.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/wagtail_hooks/icons.py` & `globlocks-1.2.0/globlocks/wagtail_hooks/icons.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/wagtail_hooks/rt_extensions.py` & `globlocks-1.2.0/globlocks/wagtail_hooks/rt_extensions.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/widgets/color_input_widget.py` & `globlocks-1.2.0/globlocks/widgets/color_input_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/widgets/fontpicker.py` & `globlocks-1.2.0/globlocks/widgets/fontpicker.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/widgets/justify_widget.py` & `globlocks-1.2.0/globlocks/widgets/justify_widget.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/widgets/orderable.py` & `globlocks-1.2.0/globlocks/widgets/orderable.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks/widgets/range_input.py` & `globlocks-1.2.0/globlocks/widgets/range_input.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/globlocks.egg-info/PKG-INFO` & `globlocks-1.2.0/globlocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globlocks
-Version: 1.1.9
+Version: 1.2.0
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/globlocks
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `globlocks-1.1.9/globlocks.egg-info/SOURCES.txt` & `globlocks-1.2.0/globlocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/setup.cfg` & `globlocks-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6c6f 626c 6f63 6b73 0d0a 7665   = globlocks..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 390d 0a64  rsion = 1.1.9..d
+00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a64  rsion = 1.2.0..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2041 6e20  escription = An 
 00000040: 6170 706c 6963 6174 696f 6e20 6d61 6465  application made
 00000050: 2066 6f72 2074 6865 2044 6a61 6e67 6f20   for the Django 
 00000060: 5765 6220 4672 616d 6577 6f72 6b2e 0d0a  Web Framework...
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
```

### Comparing `globlocks-1.1.9/tests/testapp/manage.py` & `globlocks-1.2.0/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/tests/testapp/testapp/settings.py` & `globlocks-1.2.0/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `globlocks-1.1.9/tests/testapp/testapp/urls.py` & `globlocks-1.2.0/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

