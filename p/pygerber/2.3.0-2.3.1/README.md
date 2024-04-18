# Comparing `tmp/pygerber-2.3.0.tar.gz` & `tmp/pygerber-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygerber-2.3.0.tar", max compression
+gzip compressed data, was "pygerber-2.3.1.tar", max compression
```

## Comparing `pygerber-2.3.0.tar` & `pygerber-2.3.1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
--rw-r--r--   0        0        0     1069 2024-04-11 23:49:13.911182 pygerber-2.3.0/LICENSE.md
--rw-r--r--   0        0        0    12132 2024-04-11 23:49:13.911182 pygerber-2.3.0/README.md
--rw-r--r--   0        0        0    12976 2024-04-11 23:49:14.043183 pygerber-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      103 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/__init__.py
--rw-r--r--   0        0        0      149 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/__main__.py
--rw-r--r--   0        0        0      858 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/__init__.py
--rw-r--r--   0        0        0       61 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/__init__.py
--rw-r--r--   0        0        0     4205 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/aperture_handle.py
--rw-r--r--   0        0        0     6118 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/backend_cls.py
--rw-r--r--   0        0        0       50 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/__init__.py
--rw-r--r--   0        0        0     3958 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_arc.py
--rw-r--r--   0        0        0     1165 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py
--rw-r--r--   0        0        0     1214 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_circle.py
--rw-r--r--   0        0        0     1007 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_command.py
--rw-r--r--   0        0        0     1226 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_paste.py
--rw-r--r--   0        0        0     1527 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_polygon.py
--rw-r--r--   0        0        0     1323 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py
--rw-r--r--   0        0        0     1395 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_region.py
--rw-r--r--   0        0        0     1707 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py
--rw-r--r--   0        0        0      793 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands_handle.py
--rw-r--r--   0        0        0     1101 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/drawing_target.py
--rw-r--r--   0        0        0      280 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/errors.py
--rw-r--r--   0        0        0      663 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/abstract/result_handle.py
--rw-r--r--   0        0        0       65 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/aperture_handle.py
--rw-r--r--   0        0        0     8530 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/backend_cls.py
--rw-r--r--   0        0        0     8452 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/color_scheme.py
--rw-r--r--   0        0        0       81 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py
--rw-r--r--   0        0        0     1583 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py
--rw-r--r--   0        0        0     1702 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py
--rw-r--r--   0        0        0     2072 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py
--rw-r--r--   0        0        0     2139 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py
--rw-r--r--   0        0        0     1634 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py
--rw-r--r--   0        0        0     1616 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py
--rw-r--r--   0        0        0     1389 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py
--rw-r--r--   0        0        0      317 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands_handle.py
--rw-r--r--   0        0        0     4122 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/drawing_target.py
--rw-r--r--   0        0        0      520 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/errors.py
--rw-r--r--   0        0        0      801 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/image_tools.py
--rw-r--r--   0        0        0     1589 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/backend/rasterized_2d/result_handle.py
--rw-r--r--   0        0        0       53 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/__init__.py
--rw-r--r--   0        0        0      202 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/error.py
--rw-r--r--   0        0        0      369 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/frozen_general_model.py
--rw-r--r--   0        0        0      364 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/general_model.py
--rw-r--r--   0        0        0     2179 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/immutable_map_model.py
--rw-r--r--   0        0        0     2860 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/position.py
--rw-r--r--   0        0        0     4913 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/common/rgba.py
--rw-r--r--   0        0        0       37 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/console/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/console/commands.py
--rw-r--r--   0        0        0     2950 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/console/raster_2d_style.py
--rw-r--r--   0        0        0      925 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/examples/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-11 23:49:14.043183 pygerber-2.3.0/src/pygerber/examples/shape_flashes.grb
--rw-r--r--   0        0        0    49675 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Cu.gbr
--rw-r--r--   0        0        0     3742 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Mask.gbr
--rw-r--r--   0        0        0     2486 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Paste.gbr
--rw-r--r--   0        0        0     9518 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr
--rw-r--r--   0        0        0    10101 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/examples/ucamco_ex_2_shapes.grb
--rw-r--r--   0        0        0       50 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/__init__.py
--rw-r--r--   0        0        0     1130 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/_errors.py
--rw-r--r--   0        0        0    12011 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/_layers.py
--rw-r--r--   0        0        0    13437 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/_v2.py
--rw-r--r--   0        0        0      981 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/api/v2.py
--rw-r--r--   0        0        0      248 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/__main__.py
--rw-r--r--   0        0        0      489 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/__init__.py
--rw-r--r--   0        0        0     4711 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/document.py
--rw-r--r--   0        0        0      167 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/error.py
--rw-r--r--   0        0        0      273 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/errors.py
--rw-r--r--   0        0        0     3891 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/server.py
--rw-r--r--   0        0        0       29 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/linter/__init__.py
--rw-r--r--   0        0        0     6540 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/linter/diagnostic.py
--rw-r--r--   0        0        0       40 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/__init__.py
--rw-r--r--   0        0        0     5229 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/bounding_box.py
--rw-r--r--   0        0        0     4845 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/offset.py
--rw-r--r--   0        0        0      711 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/rotate_point.py
--rw-r--r--   0        0        0     7968 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/math/vector_2d.py
--rw-r--r--   0        0        0       29 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/optimizer/__init__.py
--rw-r--r--   0        0        0       38 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/optimizer/optimizer_pass/__init__.py
--rw-r--r--   0        0        0       23 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/__init__.py
--rw-r--r--   0        0        0     2282 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/errors.py
--rw-r--r--   0        0        0     5942 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/parser.py
--rw-r--r--   0        0        0     6100 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser/state.py
--rw-r--r--   0        0        0       36 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/__init__.py
--rw-r--r--   0        0        0       82 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/aperture2.py
--rw-r--r--   0        0        0     2122 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/block2.py
--rw-r--r--   0        0        0     2071 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/circle2.py
--rw-r--r--   0        0        0     2056 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/macro2.py
--rw-r--r--   0        0        0      789 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/obround2.py
--rw-r--r--   0        0        0     1635 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/polygon2.py
--rw-r--r--   0        0        0     1650 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py
--rw-r--r--   0        0        0     8944 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/attributes2.py
--rw-r--r--   0        0        0     3922 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/command_buffer2.py
--rw-r--r--   0        0        0       88 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/__init__.py
--rw-r--r--   0        0        0      975 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py
--rw-r--r--   0        0        0     4375 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/arc2.py
--rw-r--r--   0        0        0     2952 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py
--rw-r--r--   0        0        0     2258 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/command2.py
--rw-r--r--   0        0        0     2477 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/flash2.py
--rw-r--r--   0        0        0     2688 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/line2.py
--rw-r--r--   0        0        0     1733 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/region2.py
--rw-r--r--   0        0        0    24876 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/context2.py
--rw-r--r--   0        0        0     4052 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/errors2.py
--rw-r--r--   0        0        0       66 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/__init__.py
--rw-r--r--   0        0        0      729 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/assignment2.py
--rw-r--r--   0        0        0      238 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/element2.py
--rw-r--r--   0        0        0      242 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/enums.py
--rw-r--r--   0        0        0       61 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py
--rw-r--r--   0        0        0      674 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py
--rw-r--r--   0        0        0     1207 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py
--rw-r--r--   0        0        0      957 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py
--rw-r--r--   0        0        0      663 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py
--rw-r--r--   0        0        0      757 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/macro2.py
--rw-r--r--   0        0        0      392 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/point2.py
--rw-r--r--   0        0        0       56 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/__init__.py
--rw-r--r--   0        0        0      749 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py
--rw-r--r--   0        0        0      811 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py
--rw-r--r--   0        0        0      791 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py
--rw-r--r--   0        0        0      588 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py
--rw-r--r--   0        0        0      555 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py
--rw-r--r--   0        0        0      849 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py
--rw-r--r--   0        0        0      875 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py
--rw-r--r--   0        0        0      532 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py
--rw-r--r--   0        0        0      786 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py
--rw-r--r--   0        0        0      207 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/primitive2.py
--rw-r--r--   0        0        0      891 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement2.py
--rw-r--r--   0        0        0     1294 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py
--rw-r--r--   0        0        0     5052 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2.py
--rw-r--r--   0        0        0    84548 2024-04-11 23:49:14.047183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks.py
--rw-r--r--   0        0        0    29008 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks_base.py
--rw-r--r--   0        0        0    29444 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/parser2/state2.py
--rw-r--r--   0        0        0      135 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/__init__.py
--rw-r--r--   0        0        0     4767 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/abstract.py
--rw-r--r--   0        0        0      497 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/errors2.py
--rw-r--r--   0        0        0    29641 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/raster.py
--rw-r--r--   0        0        0    29563 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/renderer2/svg.py
--rw-r--r--   0        0        0    14537 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/revisions.py
--rw-r--r--   0        0        0     5321 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/state_enums.py
--rw-r--r--   0        0        0       27 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/__init__.py
--rw-r--r--   0        0        0      936 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/aperture_id.py
--rw-r--r--   0        0        0     1075 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/decorators.py
--rw-r--r--   0        0        0      162 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/errors.py
--rw-r--r--   0        0        0     4459 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.ebnf
--rw-r--r--   0        0        0    38460 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.py
--rw-r--r--   0        0        0       22 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/helpers/__init__.py
--rw-r--r--   0        0        0      509 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/helpers/gerber_code_enum.py
--rw-r--r--   0        0        0     2355 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokenizer.py
--rw-r--r--   0        0        0       32 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/__init__.py
--rw-r--r--   0        0        0     6972 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py
--rw-r--r--   0        0        0    31743 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py
--rw-r--r--   0        0        0     4355 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py
--rw-r--r--   0        0        0     3984 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py
--rw-r--r--   0        0        0       43 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/__init__.py
--rw-r--r--   0        0        0     2369 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py
--rw-r--r--   0        0        0     2388 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py
--rw-r--r--   0        0        0      907 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py
--rw-r--r--   0        0        0     4049 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py
--rw-r--r--   0        0        0     4775 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py
--rw-r--r--   0        0        0      633 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py
--rw-r--r--   0        0        0     2823 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py
--rw-r--r--   0        0        0    10302 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py
--rw-r--r--   0        0        0     4122 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py
--rw-r--r--   0        0        0     4219 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py
--rw-r--r--   0        0        0     3199 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py
--rw-r--r--   0        0        0     1486 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py
--rw-r--r--   0        0        0     7836 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py
--rw-r--r--   0        0        0     1933 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py
--rw-r--r--   0        0        0     2039 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py
--rw-r--r--   0        0        0     2154 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py
--rw-r--r--   0        0        0     2170 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py
--rw-r--r--   0        0        0     1914 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py
--rw-r--r--   0        0        0     2158 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py
--rw-r--r--   0        0        0     1939 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py
--rw-r--r--   0        0        0     2554 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py
--rw-r--r--   0        0        0     2343 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py
--rw-r--r--   0        0        0     2272 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py
--rw-r--r--   0        0        0     2705 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py
--rw-r--r--   0        0        0     2325 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py
--rw-r--r--   0        0        0     2383 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py
--rw-r--r--   0        0        0       20 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/__init__.py
--rw-r--r--   0        0        0      206 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/ast.py
--rw-r--r--   0        0        0     2057 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py
--rw-r--r--   0        0        0     3263 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py
--rw-r--r--   0        0        0     2052 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py
--rw-r--r--   0        0        0     2904 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py
--rw-r--r--   0        0        0     2491 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py
--rw-r--r--   0        0        0     3384 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py
--rw-r--r--   0        0        0     2471 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py
--rw-r--r--   0        0        0     3189 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py
--rw-r--r--   0        0        0     3184 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py
--rw-r--r--   0        0        0     1615 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py
--rw-r--r--   0        0        0     1621 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py
--rw-r--r--   0        0        0     1607 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py
--rw-r--r--   0        0        0     1164 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py
--rw-r--r--   0        0        0     7925 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py
--rw-r--r--   0        0        0       62 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/__init__.py
--rw-r--r--   0        0        0     5585 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py
--rw-r--r--   0        0        0      274 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/errors.py
--rw-r--r--   0        0        0     1776 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py
--rw-r--r--   0        0        0     2135 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py
--rw-r--r--   0        0        0     3647 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py
--rw-r--r--   0        0        0     2431 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py
--rw-r--r--   0        0        0     3660 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py
--rw-r--r--   0        0        0      360 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_context.py
--rw-r--r--   0        0        0     1935 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py
--rw-r--r--   0        0        0       60 2024-04-11 23:49:14.051183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/__init__.py
--rw-r--r--   0        0        0     4874 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py
--rw-r--r--   0        0        0     4264 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py
--rw-r--r--   0        0        0     4006 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py
--rw-r--r--   0        0        0      944 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py
--rw-r--r--   0        0        0      898 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py
--rw-r--r--   0        0        0     5065 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py
--rw-r--r--   0        0        0     4182 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py
--rw-r--r--   0        0        0      866 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py
--rw-r--r--   0        0        0     3980 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py
--rw-r--r--   0        0        0     2204 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py
--rw-r--r--   0        0        0      370 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/primitive.py
--rw-r--r--   0        0        0      953 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py
--rw-r--r--   0        0        0     4388 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py
--rw-r--r--   0        0        0     2711 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py
--rw-r--r--   0        0        0     3801 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py
--rw-r--r--   0        0        0     3090 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py
--rw-r--r--   0        0        0     1892 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py
--rw-r--r--   0        0        0     2122 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py
--rw-r--r--   0        0        0     1477 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py
--rw-r--r--   0        0        0     1724 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py
--rw-r--r--   0        0        0      899 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/sequence_tools.py
--rw-r--r--   0        0        0      491 2024-04-11 23:49:14.055183 pygerber-2.3.0/src/pygerber/warnings.py
--rw-r--r--   0        0        0    14868 1970-01-01 00:00:00.000000 pygerber-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-18 23:23:58.575230 pygerber-2.3.1/LICENSE.md
+-rw-r--r--   0        0        0    12132 2024-04-18 23:23:58.575230 pygerber-2.3.1/README.md
+-rw-r--r--   0        0        0    12976 2024-04-18 23:23:58.707229 pygerber-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/__main__.py
+-rw-r--r--   0        0        0      858 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/__init__.py
+-rw-r--r--   0        0        0     4205 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/aperture_handle.py
+-rw-r--r--   0        0        0     6118 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/backend_cls.py
+-rw-r--r--   0        0        0       50 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/__init__.py
+-rw-r--r--   0        0        0     3958 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_arc.py
+-rw-r--r--   0        0        0     1165 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py
+-rw-r--r--   0        0        0     1214 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_circle.py
+-rw-r--r--   0        0        0     1007 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_command.py
+-rw-r--r--   0        0        0     1226 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_paste.py
+-rw-r--r--   0        0        0     1527 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_polygon.py
+-rw-r--r--   0        0        0     1323 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py
+-rw-r--r--   0        0        0     1395 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_region.py
+-rw-r--r--   0        0        0     1707 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py
+-rw-r--r--   0        0        0      793 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands_handle.py
+-rw-r--r--   0        0        0     1101 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/drawing_target.py
+-rw-r--r--   0        0        0      280 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/errors.py
+-rw-r--r--   0        0        0      663 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/result_handle.py
+-rw-r--r--   0        0        0       65 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/aperture_handle.py
+-rw-r--r--   0        0        0     8530 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/backend_cls.py
+-rw-r--r--   0        0        0     8452 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/color_scheme.py
+-rw-r--r--   0        0        0       81 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py
+-rw-r--r--   0        0        0     1583 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py
+-rw-r--r--   0        0        0     1702 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py
+-rw-r--r--   0        0        0     2072 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py
+-rw-r--r--   0        0        0     2139 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py
+-rw-r--r--   0        0        0     1634 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py
+-rw-r--r--   0        0        0     1616 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py
+-rw-r--r--   0        0        0     1389 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py
+-rw-r--r--   0        0        0      317 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands_handle.py
+-rw-r--r--   0        0        0     4122 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/drawing_target.py
+-rw-r--r--   0        0        0      520 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/errors.py
+-rw-r--r--   0        0        0      801 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/image_tools.py
+-rw-r--r--   0        0        0     1589 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/result_handle.py
+-rw-r--r--   0        0        0       53 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/error.py
+-rw-r--r--   0        0        0      369 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/frozen_general_model.py
+-rw-r--r--   0        0        0      364 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/general_model.py
+-rw-r--r--   0        0        0     2179 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/immutable_map_model.py
+-rw-r--r--   0        0        0     2860 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/position.py
+-rw-r--r--   0        0        0     4913 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/rgba.py
+-rw-r--r--   0        0        0       37 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/console/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/console/commands.py
+-rw-r--r--   0        0        0     2950 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/console/raster_2d_style.py
+-rw-r--r--   0        0        0      925 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/shape_flashes.grb
+-rw-r--r--   0        0        0    49675 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Cu.gbr
+-rw-r--r--   0        0        0     3742 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Mask.gbr
+-rw-r--r--   0        0        0     2486 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Paste.gbr
+-rw-r--r--   0        0        0     9518 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr
+-rw-r--r--   0        0        0    10101 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/ucamco_ex_2_shapes.grb
+-rw-r--r--   0        0        0       50 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/__init__.py
+-rw-r--r--   0        0        0     1130 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/_errors.py
+-rw-r--r--   0        0        0    12011 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/_layers.py
+-rw-r--r--   0        0        0    13437 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/_v2.py
+-rw-r--r--   0        0        0      981 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/v2.py
+-rw-r--r--   0        0        0      248 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/__main__.py
+-rw-r--r--   0        0        0      489 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/__init__.py
+-rw-r--r--   0        0        0     4711 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/document.py
+-rw-r--r--   0        0        0      167 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/error.py
+-rw-r--r--   0        0        0      273 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/errors.py
+-rw-r--r--   0        0        0     3891 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/server.py
+-rw-r--r--   0        0        0       29 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/linter/__init__.py
+-rw-r--r--   0        0        0     6540 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/linter/diagnostic.py
+-rw-r--r--   0        0        0       40 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/__init__.py
+-rw-r--r--   0        0        0     6193 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/bounding_box.py
+-rw-r--r--   0        0        0     5071 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/offset.py
+-rw-r--r--   0        0        0      711 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/rotate_point.py
+-rw-r--r--   0        0        0     8028 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/vector_2d.py
+-rw-r--r--   0        0        0       29 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/optimizer/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/optimizer/optimizer_pass/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/errors.py
+-rw-r--r--   0        0        0     5942 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/parser.py
+-rw-r--r--   0        0        0     6100 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/state.py
+-rw-r--r--   0        0        0       36 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/__init__.py
+-rw-r--r--   0        0        0       82 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/aperture2.py
+-rw-r--r--   0        0        0     2122 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/block2.py
+-rw-r--r--   0        0        0     1942 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/circle2.py
+-rw-r--r--   0        0        0     2056 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/macro2.py
+-rw-r--r--   0        0        0      789 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/obround2.py
+-rw-r--r--   0        0        0     1635 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/polygon2.py
+-rw-r--r--   0        0        0     2007 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py
+-rw-r--r--   0        0        0     8944 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/attributes2.py
+-rw-r--r--   0        0        0     3922 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/command_buffer2.py
+-rw-r--r--   0        0        0       88 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py
+-rw-r--r--   0        0        0     4375 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/arc2.py
+-rw-r--r--   0        0        0     2952 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py
+-rw-r--r--   0        0        0     2258 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/command2.py
+-rw-r--r--   0        0        0     2477 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/flash2.py
+-rw-r--r--   0        0        0     2688 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/line2.py
+-rw-r--r--   0        0        0     1733 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/region2.py
+-rw-r--r--   0        0        0    24876 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/context2.py
+-rw-r--r--   0        0        0     4052 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/errors2.py
+-rw-r--r--   0        0        0       66 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/__init__.py
+-rw-r--r--   0        0        0      729 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/assignment2.py
+-rw-r--r--   0        0        0      238 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/element2.py
+-rw-r--r--   0        0        0      242 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/enums.py
+-rw-r--r--   0        0        0       61 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py
+-rw-r--r--   0        0        0      674 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py
+-rw-r--r--   0        0        0     1207 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py
+-rw-r--r--   0        0        0      957 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py
+-rw-r--r--   0        0        0      663 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py
+-rw-r--r--   0        0        0      757 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/macro2.py
+-rw-r--r--   0        0        0      392 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/point2.py
+-rw-r--r--   0        0        0       56 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py
+-rw-r--r--   0        0        0      811 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py
+-rw-r--r--   0        0        0      791 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py
+-rw-r--r--   0        0        0      588 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py
+-rw-r--r--   0        0        0      555 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py
+-rw-r--r--   0        0        0      849 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py
+-rw-r--r--   0        0        0      875 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py
+-rw-r--r--   0        0        0      532 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py
+-rw-r--r--   0        0        0      786 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py
+-rw-r--r--   0        0        0      207 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/primitive2.py
+-rw-r--r--   0        0        0      891 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement2.py
+-rw-r--r--   0        0        0     1294 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py
+-rw-r--r--   0        0        0     5052 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2.py
+-rw-r--r--   0        0        0    84867 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks.py
+-rw-r--r--   0        0        0    29008 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks_base.py
+-rw-r--r--   0        0        0    29444 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/state2.py
+-rw-r--r--   0        0        0      135 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/__init__.py
+-rw-r--r--   0        0        0     4767 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/abstract.py
+-rw-r--r--   0        0        0      497 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/errors2.py
+-rw-r--r--   0        0        0    30444 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/raster.py
+-rw-r--r--   0        0        0    29602 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/svg.py
+-rw-r--r--   0        0        0    14537 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/revisions.py
+-rw-r--r--   0        0        0     5321 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/state_enums.py
+-rw-r--r--   0        0        0       27 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/__init__.py
+-rw-r--r--   0        0        0      936 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/aperture_id.py
+-rw-r--r--   0        0        0     1075 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/decorators.py
+-rw-r--r--   0        0        0      162 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/errors.py
+-rw-r--r--   0        0        0     4459 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.ebnf
+-rw-r--r--   0        0        0    38460 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.py
+-rw-r--r--   0        0        0       22 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/helpers/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/helpers/gerber_code_enum.py
+-rw-r--r--   0        0        0     2355 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokenizer.py
+-rw-r--r--   0        0        0       32 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/__init__.py
+-rw-r--r--   0        0        0     6972 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py
+-rw-r--r--   0        0        0    31743 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py
+-rw-r--r--   0        0        0     4355 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py
+-rw-r--r--   0        0        0     3984 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py
+-rw-r--r--   0        0        0       43 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/__init__.py
+-rw-r--r--   0        0        0     2369 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py
+-rw-r--r--   0        0        0     2388 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py
+-rw-r--r--   0        0        0      907 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py
+-rw-r--r--   0        0        0     4049 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py
+-rw-r--r--   0        0        0     4775 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py
+-rw-r--r--   0        0        0      633 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py
+-rw-r--r--   0        0        0     2823 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py
+-rw-r--r--   0        0        0    10302 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py
+-rw-r--r--   0        0        0     4122 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py
+-rw-r--r--   0        0        0     4219 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py
+-rw-r--r--   0        0        0     3199 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py
+-rw-r--r--   0        0        0     1486 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py
+-rw-r--r--   0        0        0     7836 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py
+-rw-r--r--   0        0        0     1933 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py
+-rw-r--r--   0        0        0     2039 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py
+-rw-r--r--   0        0        0     2154 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py
+-rw-r--r--   0        0        0     2170 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py
+-rw-r--r--   0        0        0     1914 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py
+-rw-r--r--   0        0        0     2158 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py
+-rw-r--r--   0        0        0     1939 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py
+-rw-r--r--   0        0        0     2554 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py
+-rw-r--r--   0        0        0     2343 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py
+-rw-r--r--   0        0        0     2272 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py
+-rw-r--r--   0        0        0     2705 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py
+-rw-r--r--   0        0        0     2325 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py
+-rw-r--r--   0        0        0     2383 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py
+-rw-r--r--   0        0        0       20 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/ast.py
+-rw-r--r--   0        0        0     2057 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py
+-rw-r--r--   0        0        0     3263 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py
+-rw-r--r--   0        0        0     2052 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py
+-rw-r--r--   0        0        0     2904 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py
+-rw-r--r--   0        0        0     2491 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py
+-rw-r--r--   0        0        0     3384 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py
+-rw-r--r--   0        0        0     2471 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py
+-rw-r--r--   0        0        0     3189 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py
+-rw-r--r--   0        0        0     3184 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py
+-rw-r--r--   0        0        0     1615 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py
+-rw-r--r--   0        0        0     1621 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py
+-rw-r--r--   0        0        0     1607 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py
+-rw-r--r--   0        0        0     1164 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py
+-rw-r--r--   0        0        0     7925 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py
+-rw-r--r--   0        0        0       62 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/__init__.py
+-rw-r--r--   0        0        0     5585 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py
+-rw-r--r--   0        0        0      274 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/errors.py
+-rw-r--r--   0        0        0     1776 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py
+-rw-r--r--   0        0        0     2135 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py
+-rw-r--r--   0        0        0     3647 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py
+-rw-r--r--   0        0        0     2431 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py
+-rw-r--r--   0        0        0     3660 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py
+-rw-r--r--   0        0        0      360 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_context.py
+-rw-r--r--   0        0        0     1935 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py
+-rw-r--r--   0        0        0       60 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/__init__.py
+-rw-r--r--   0        0        0     4874 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py
+-rw-r--r--   0        0        0     4264 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py
+-rw-r--r--   0        0        0     4006 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py
+-rw-r--r--   0        0        0      944 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py
+-rw-r--r--   0        0        0      898 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py
+-rw-r--r--   0        0        0     5065 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py
+-rw-r--r--   0        0        0     4182 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py
+-rw-r--r--   0        0        0      866 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py
+-rw-r--r--   0        0        0     3980 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py
+-rw-r--r--   0        0        0     2204 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py
+-rw-r--r--   0        0        0      370 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/primitive.py
+-rw-r--r--   0        0        0      953 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py
+-rw-r--r--   0        0        0     4388 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py
+-rw-r--r--   0        0        0     2711 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py
+-rw-r--r--   0        0        0     3801 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py
+-rw-r--r--   0        0        0     3090 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py
+-rw-r--r--   0        0        0     1892 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py
+-rw-r--r--   0        0        0     2122 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py
+-rw-r--r--   0        0        0     1477 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py
+-rw-r--r--   0        0        0     1724 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py
+-rw-r--r--   0        0        0      899 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/sequence_tools.py
+-rw-r--r--   0        0        0      491 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/warnings.py
+-rw-r--r--   0        0        0    14868 1970-01-01 00:00:00.000000 pygerber-2.3.1/PKG-INFO
```

### Comparing `pygerber-2.3.0/LICENSE.md` & `pygerber-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/README.md` & `pygerber-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/pyproject.toml` & `pygerber-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygerber"
-version = "2.3.0"
+version = "2.3.1"
 description = "Parsing, formatting and rendering toolkit for Gerber X3 file format"
 authors = ["Krzysztof Wisniewski <argmaster.world@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.facebook.com/pygerber"
 repository = "https://github.com/Argmaster/pygerber"
 documentation = "https://argmaster.github.io/pygerber/latest"
```

### Comparing `pygerber-2.3.0/src/pygerber/backend/__init__.py` & `pygerber-2.3.1/src/pygerber/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/aperture_handle.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/aperture_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/backend_cls.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/backend_cls.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_arc.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_arc.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_circle.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_command.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_paste.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_paste.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_polygon.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_region.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/draw_commands_handle.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/drawing_target.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/drawing_target.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/abstract/result_handle.py` & `pygerber-2.3.1/src/pygerber/backend/abstract/result_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/aperture_handle.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/aperture_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/backend_cls.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/backend_cls.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/color_scheme.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/color_scheme.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/drawing_target.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/drawing_target.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/errors.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/image_tools.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/image_tools.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/backend/rasterized_2d/result_handle.py` & `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/result_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/common/immutable_map_model.py` & `pygerber-2.3.1/src/pygerber/common/immutable_map_model.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/common/position.py` & `pygerber-2.3.1/src/pygerber/common/position.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/common/rgba.py` & `pygerber-2.3.1/src/pygerber/common/rgba.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/console/commands.py` & `pygerber-2.3.1/src/pygerber/console/commands.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/console/raster_2d_style.py` & `pygerber-2.3.1/src/pygerber/console/raster_2d_style.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/__init__.py` & `pygerber-2.3.1/src/pygerber/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/shape_flashes.grb` & `pygerber-2.3.1/src/pygerber/examples/shape_flashes.grb`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Cu.gbr` & `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Cu.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Mask.gbr` & `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Mask.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Paste.gbr` & `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Paste.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr` & `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/examples/ucamco_ex_2_shapes.grb` & `pygerber-2.3.1/src/pygerber/examples/ucamco_ex_2_shapes.grb`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/api/__init__.py` & `pygerber-2.3.1/src/pygerber/gerberx3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/api/_errors.py` & `pygerber-2.3.1/src/pygerber/gerberx3/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/api/_layers.py` & `pygerber-2.3.1/src/pygerber/gerberx3/api/_layers.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/api/_v2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/api/_v2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/api/v2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/api/v2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/language_server/__main__.py` & `pygerber-2.3.1/src/pygerber/gerberx3/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/document.py` & `pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/document.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/language_server/_internals/server.py` & `pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/server.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/linter/diagnostic.py` & `pygerber-2.3.1/src/pygerber/gerberx3/linter/diagnostic.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/math/bounding_box.py` & `pygerber-2.3.1/src/pygerber/gerberx3/math/bounding_box.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Utility class for calculating bounding boxes of drawing elements."""
+
 from __future__ import annotations
 
+import math
 import operator
 from decimal import Decimal
 from typing import Callable, ClassVar, Tuple
 
 from pydantic import Field
 
 from pygerber.common.frozen_general_model import FrozenGeneralModel
@@ -67,14 +69,18 @@
         center_y = (self.max_y + self.min_y) / Offset(value=Decimal(2))
         return Vector2D(x=center_x, y=center_y)
 
     def get_min_vector(self) -> Vector2D:
         """Return Vector2D of min_x and min_y."""
         return Vector2D(x=self.min_x, y=self.min_y)
 
+    def get_max_vector(self) -> Vector2D:
+        """Return Vector2D of min_x and min_y."""
+        return Vector2D(x=self.max_x, y=self.max_y)
+
     def as_pixel_box(
         self,
         dpi: int,
         *,
         dx_max: int = 0,
         dy_max: int = 0,
         dx_min: int = 0,
@@ -152,14 +158,36 @@
         return BoundingBox(
             max_x=new_max_x,
             max_y=new_max_y,
             min_x=new_min_x,
             min_y=new_min_y,
         )
 
+    def get_rotated(self, angle: Decimal) -> BoundingBox:
+        """Return bounding box rotated around (0, 0)."""
+        angle_radians = math.radians(angle)
+        max_x = self.max_x * math.cos(angle_radians) - self.max_y * math.sin(
+            angle_radians,
+        )
+        max_y = self.max_x * math.sin(angle_radians) - self.max_y * math.cos(
+            angle_radians,
+        )
+        min_x = self.min_x * math.cos(angle_radians) - self.min_y * math.sin(
+            angle_radians,
+        )
+        min_y = self.min_x * math.sin(angle_radians) - self.min_y * math.cos(
+            angle_radians,
+        )
+        return BoundingBox(
+            max_x=max(max_x, min_x),
+            max_y=max(max_y, min_y),
+            min_x=min(max_x, min_x),
+            min_y=min(max_y, min_y),
+        )
+
 
 BoundingBox.NULL = BoundingBox(
     max_x=Offset.NULL,
     max_y=Offset.NULL,
     min_x=Offset.NULL,
     min_y=Offset.NULL,
 )
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/math/offset.py` & `pygerber-2.3.1/src/pygerber/gerberx3/math/offset.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,18 @@
 
         return self.as_millimeters()
 
     def as_pixels(self, dpi: int | Decimal) -> int:
         """Offset in pixels with respect to drawing DPI."""
         return int(self.as_inches() * dpi)
 
+    def sqrt(self) -> Offset:
+        """Return square root of the offset."""
+        return Offset(value=self.value.sqrt())
+
     def _compare(
         self,
         other: object,
         op: Callable,
     ) -> bool:
         if isinstance(other, Offset):
             return op(self.value, other.value)  # type: ignore[no-any-return]
@@ -117,14 +121,17 @@
 
     def __truediv__(self, other: object) -> Offset:
         return self._operator(other, operator.truediv)
 
     def __neg__(self) -> Offset:
         return Offset(value=-self.value)
 
+    def __pow__(self, other: object) -> Offset:
+        return self._operator(other, operator.pow)
+
     def _i_operator(
         self,
         other: object,
         op: Callable,
     ) -> Self:
         if isinstance(other, Offset):
             return self.model_copy(
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/math/rotate_point.py` & `pygerber-2.3.1/src/pygerber/gerberx3/math/rotate_point.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/math/vector_2d.py` & `pygerber-2.3.1/src/pygerber/gerberx3/math/vector_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         Mirroring.X: _get_mirrored_x,
         Mirroring.Y: _get_mirrored_y,
         Mirroring.XY: _get_mirrored_xy,
     }
 
     def get_rotated(self, angle: Decimal) -> Self:
         """Get copy of this vector rotated around (0, 0)."""
+        if angle == Decimal("0.0"):
+            return self
         return self.rotate_around_origin(angle)
 
     def get_scaled(self, scale: Decimal) -> Vector2D:
         """Get copy of this vector scaled by factor."""
         if scale == Decimal("1.0"):
             return self
         return self * scale
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser/errors.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser/errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser/parser.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser/state.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser/state.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/aperture2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/aperture2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/block2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/block2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/circle2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/circle2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parser level abstraction of circle aperture info for Gerber AST parser, version 2."""
+
 from __future__ import annotations
 
 from decimal import Decimal
 from typing import TYPE_CHECKING, Optional
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.offset import Offset
@@ -51,11 +52,7 @@
     """Dummy aperture representing case when aperture is not needed but has to be
     given to denote width of draw line command.
     """
 
     def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
         """Render draw operation."""
         renderer.hooks.render_flash_no_circle(command, self)
-
-    def get_bounding_box(self) -> BoundingBox:
-        """Get bounding box of draw operation."""
-        return BoundingBox.NULL
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/macro2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/macro2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/obround2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/obround2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/polygon2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/polygon2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/flash2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,76 @@
-"""Parser level abstraction of rectangle aperture info for Gerber AST parser,
-version 2.
-"""
-
+"""Parser level abstraction of flash operation for Gerber AST parser, version 2."""
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional
+from decimal import Decimal
+from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
-from pygerber.gerberx3.math.offset import Offset
-from pygerber.gerberx3.parser2.apertures2.aperture2 import Aperture2
+from pygerber.gerberx3.math.vector_2d import Vector2D
+from pygerber.gerberx3.parser2.commands2.aperture_draw_command2 import (
+    ApertureDrawCommand2,
+)
+from pygerber.gerberx3.state_enums import Mirroring
 
 if TYPE_CHECKING:
-    from decimal import Decimal
-
     from typing_extensions import Self
 
-    from pygerber.gerberx3.parser2.commands2.flash2 import Flash2
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
-class Rectangle2(Aperture2):
-    """Parser level abstraction of aperture info for rectangle aperture."""
-
-    x_size: Offset
-    y_size: Offset
-    hole_diameter: Optional[Offset]
-
-    def render_flash(self, renderer: Renderer2, command: Flash2) -> None:
-        """Render draw operation."""
-        renderer.hooks.render_flash_rectangle(command, self)
+class Flash2(ApertureDrawCommand2):
+    """Parser level abstraction of flash operation for Gerber AST parser,
+    version 2.
+    """
+
+    flash_point: Vector2D
+
+    def get_mirrored(self, mirror: Mirroring) -> Self:
+        """Get mirrored command.
+
+        Mirroring is a NOOP if mirror is `Mirroring.NoMirroring`.
+        """
+        if mirror == Mirroring.NoMirroring:
+            return self
+        return self.model_copy(
+            update={
+                "flash_point": self.flash_point.get_mirrored(mirror),
+                "aperture": self.aperture.get_mirrored(mirror),
+            },
+        )
 
-    def get_stroke_width(self) -> Offset:
-        """Return stroke width of aperture."""
-        return (self.x_size + self.y_size) / 2
+    def get_transposed(self, vector: Vector2D) -> Self:
+        """Get transposed command."""
+        return self.model_copy(
+            update={
+                "flash_point": self.flash_point + vector,
+            },
+        )
 
-    def get_bounding_box(self) -> BoundingBox:
-        """Return bounding box of aperture."""
-        return BoundingBox.from_rectangle(self.x_size, self.y_size)
+    def get_rotated(self, angle: Decimal) -> Self:
+        """Get copy of this command rotated around (0, 0)."""
+        return self.model_copy(
+            update={
+                "flash_point": self.flash_point.get_rotated(angle),
+                "aperture": self.aperture.get_rotated(angle),
+            },
+        )
 
     def get_scaled(self, scale: Decimal) -> Self:
         """Get copy of this aperture scaled by factor."""
+        if scale == Decimal("1.0"):
+            return self
         return self.model_copy(
             update={
-                "x_size": self.x_size * scale,
-                "y_size": self.y_size * scale,
-                "hole_diameter": (
-                    None if self.hole_diameter is None else self.hole_diameter * scale
-                ),
+                "flash_point": self.flash_point.get_scaled(scale),
+                "aperture": self.aperture.get_scaled(scale),
+                "transform": self.transform.get_scaled(scale),
             },
         )
+
+    def render(self, renderer: Renderer2) -> None:
+        """Render draw operation."""
+        self.aperture.render_flash(renderer, self)
+
+    def get_bounding_box(self) -> BoundingBox:
+        """Get bounding box of draw operation."""
+        return self.aperture.get_bounding_box() + self.flash_point
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/attributes2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/attributes2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/command_buffer2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/command_buffer2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/arc2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/arc2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/command2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/command2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/flash2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/line2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Parser level abstraction of flash operation for Gerber AST parser, version 2."""
+"""Parser level abstraction of draw line operation for Gerber AST parser, version 2."""
 from __future__ import annotations
 
 from decimal import Decimal
 from typing import TYPE_CHECKING
 
 from pygerber.gerberx3.math.bounding_box import BoundingBox
 from pygerber.gerberx3.math.vector_2d import Vector2D
@@ -13,64 +13,68 @@
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from pygerber.gerberx3.renderer2.abstract import Renderer2
 
 
-class Flash2(ApertureDrawCommand2):
-    """Parser level abstraction of flash operation for Gerber AST parser,
+class Line2(ApertureDrawCommand2):
+    """Parser level abstraction of draw line operation for Gerber AST parser,
     version 2.
     """
 
-    flash_point: Vector2D
+    start_point: Vector2D
+    end_point: Vector2D
+
+    def get_bounding_box(self) -> BoundingBox:
+        """Return bounding box of draw operation."""
+        vertex_box = self.aperture.get_bounding_box()
+        return (vertex_box + self.start_point) + (vertex_box + self.end_point)
 
     def get_mirrored(self, mirror: Mirroring) -> Self:
         """Get mirrored command.
 
         Mirroring is a NOOP if mirror is `Mirroring.NoMirroring`.
         """
         if mirror == Mirroring.NoMirroring:
             return self
         return self.model_copy(
             update={
-                "flash_point": self.flash_point.get_mirrored(mirror),
-                "aperture": self.aperture.get_mirrored(mirror),
+                "start_point": self.start_point.get_mirrored(mirror),
+                "end_point": self.end_point.get_mirrored(mirror),
             },
         )
 
     def get_transposed(self, vector: Vector2D) -> Self:
         """Get transposed command."""
         return self.model_copy(
             update={
-                "flash_point": self.flash_point + vector,
+                "start_point": self.start_point + vector,
+                "end_point": self.end_point + vector,
             },
         )
 
     def get_rotated(self, angle: Decimal) -> Self:
         """Get copy of this command rotated around (0, 0)."""
         return self.model_copy(
             update={
-                "flash_point": self.flash_point.get_rotated(angle),
-                "aperture": self.aperture.get_rotated(angle),
+                "start_point": self.start_point.get_rotated(angle),
+                "end_point": self.end_point.get_rotated(angle),
             },
         )
 
     def get_scaled(self, scale: Decimal) -> Self:
         """Get copy of this aperture scaled by factor."""
         if scale == Decimal("1.0"):
             return self
         return self.model_copy(
             update={
-                "flash_point": self.flash_point.get_scaled(scale),
+                "start_point": self.start_point.get_scaled(scale),
+                "end_point": self.end_point.get_scaled(scale),
                 "aperture": self.aperture.get_scaled(scale),
                 "transform": self.transform.get_scaled(scale),
             },
         )
 
     def render(self, renderer: Renderer2) -> None:
         """Render draw operation."""
-        self.aperture.render_flash(renderer, self)
-
-    def get_bounding_box(self) -> BoundingBox:
-        """Get bounding box of draw operation."""
-        return self.aperture.get_bounding_box() + self.flash_point
+        renderer.hooks.render_line(self)
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/commands2/region2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/region2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/context2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/context2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/errors2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/errors2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/assignment2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/assignment2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/macro2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/macro2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implementation of hooks for Gerber AST Parser, version 2."""
+
 # ruff: noqa: D401
 from __future__ import annotations
 
 import math
 from decimal import Decimal
 from types import MappingProxyType
 from typing import TYPE_CHECKING
@@ -183,14 +184,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_macro_statement_buffer()
             return super().on_parser_visit_token(token, context)
 
     class MacroCode1CircleTokenHooks(Parser2HooksBase.MacroCode1CircleTokenHooks):
         """Hooks for visiting macro primitive code 0 circle."""
 
@@ -490,14 +492,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             stmt_buff = context.get_macro_statement_buffer()
             macro_name = token.macro_name
 
             context.set_macro(
                 macro_name,
                 ApertureMacro2(name=macro_name, statements=stmt_buff.get_readonly()),
@@ -519,14 +522,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.push_block_command_buffer()
             # Save state from before block definition started.
             context.push_block_state()
 
             context.set_current_position(Vector2D.NULL)
             context.set_is_aperture_block(is_aperture_block=True)
@@ -548,14 +552,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             command_buffer = context.pop_block_command_buffer()
             identifier = context.get_aperture_block_id()
             if identifier is None:
                 raise UnnamedBlockApertureNotAllowedError(token)
 
             context.set_aperture(
@@ -586,14 +591,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             hole_diameter = (
                 None
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
 
@@ -624,14 +630,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             hole_diameter = (
                 None
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
 
@@ -663,14 +670,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             hole_diameter = (
                 None
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
 
@@ -702,14 +710,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             hole_diameter = (
                 None
                 if token.hole_diameter is None
                 else Offset.new(token.hole_diameter, context.get_draw_units())
             )
             rotation = Decimal("0.0") if token.rotation is None else token.rotation
@@ -744,14 +753,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             macro = context.get_macro(token.aperture_type)
             context.set_macro_eval_buffer()
             context.macro_variable_buffer = {
                 f"${i}": Decimal(param) for i, param in enumerate(token.am_param, 1)
             }
             macro.on_parser2_eval_statement(context)
@@ -903,15 +913,15 @@
                                 [
                                     *primitive.points,
                                     Point2(x=primitive.start_x, y=primitive.start_y),
                                 ],
                             )
                         ],
                     ).get_readonly(),
-                ),
+                ).get_rotated(primitive.rotation.on_parser2_eval_expression(context)),
             )
 
         def on_code_5_polygon(
             self,
             context: Parser2Context,
             primitive: Code5Polygon2,
         ) -> None:
@@ -951,15 +961,15 @@
                             context.get_draw_units(),
                         ),
                         y=Offset.new(
                             primitive.center_y.on_parser2_eval_expression(context),
                             context.get_draw_units(),
                         ),
                     ),
-                ),
+                ).get_rotated(primitive.rotation.on_parser2_eval_expression(context)),
             )
 
         def on_code_6_moire(
             self,
             context: Parser2Context,
             primitive: Code6Moire2,
         ) -> None:
@@ -1016,15 +1026,15 @@
                             context.get_draw_units(),
                         ),
                         y=Offset.new(
                             primitive.end_y.on_parser2_eval_expression(context),
                             context.get_draw_units(),
                         ),
                     ),
-                ),
+                ).get_rotated(primitive.rotation.on_parser2_eval_expression(context)),
             )
 
         def on_code_21_center_line(
             self,
             context: Parser2Context,
             primitive: Code21CenterLine2,
         ) -> None:
@@ -1061,15 +1071,15 @@
                             context.get_draw_units(),
                         ),
                         y=Offset.new(
                             primitive.center_y.on_parser2_eval_expression(context),
                             context.get_draw_units(),
                         ),
                     ),
-                ),
+                ).get_rotated(primitive.rotation.on_parser2_eval_expression(context)),
             )
 
         def on_code_22_lower_left_line(
             self,
             context: Parser2Context,
             primitive: Code22LowerLeftLine2,
         ) -> None:
@@ -1099,14 +1109,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context on which to perform the actions.
+
             """
             context.set_axis_correspondence(token.correspondence)
             return super().on_parser_visit_token(token, context)
 
     class CommandDrawTokenHooks(Parser2HooksBase.CommandDrawTokenHooks):
         """Hooks for visiting draw token (D01)."""
 
@@ -1121,14 +1132,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             self.DRAW_MODE_DISPATCH_TABLE[context.get_draw_mode()](self, token, context)
             return super().on_parser_visit_token(token, context)
 
         def on_parser_visit_token_line(
             self,
             token: D01Draw,
@@ -1140,14 +1152,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             state = context.get_state()
 
             x = state.parse_coordinate(token.x)
             y = state.parse_coordinate(token.y)
 
             start_point = context.get_current_position()
@@ -1181,14 +1194,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             state = context.get_state()
 
             x = state.parse_coordinate(token.x)
             y = state.parse_coordinate(token.y)
             i = state.parse_coordinate(token.i)
             j = state.parse_coordinate(token.j)
@@ -1270,14 +1284,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             state = context.get_state()
 
             x = state.parse_coordinate(token.x)
             y = state.parse_coordinate(token.y)
             i = state.parse_coordinate(token.i)
             j = state.parse_coordinate(token.j)
@@ -1362,14 +1377,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             state = context.get_state()
 
             x = state.parse_coordinate(token.x)
             y = state.parse_coordinate(token.y)
 
             destination_point = Vector2D(x=x, y=y)
@@ -1391,14 +1407,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             state = context.get_state()
 
             x = state.parse_coordinate(token.x)
             y = state.parse_coordinate(token.y)
 
             flash_point = Vector2D(x=x, y=y)
@@ -1445,14 +1462,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_current_aperture_id(token.aperture_id)
             return super().on_parser_visit_token(token, context)
 
     class CoordinateFormatTokenHooks(Parser2HooksBase.CoordinateFormatTokenHooks):
         """Hooks for visiting coordinate format token (FS)."""
 
@@ -1467,14 +1485,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_coordinate_parser(
                 CoordinateParser.new(
                     x_format=token.x_format,
                     y_format=token.y_format,
                     coordinate_mode=token.coordinate_mode,
                     zeros_mode=token.zeros_mode,
@@ -1495,14 +1514,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_draw_mode(DrawMode.Linear)
             return super().on_parser_visit_token(token, context)
 
     class SetClockwiseCircularTokenHooks(
         Parser2HooksBase.SetClockwiseCircularTokenHooks,
     ):
@@ -1519,14 +1539,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_draw_mode(DrawMode.ClockwiseCircular)
             return super().on_parser_visit_token(token, context)
 
     class SetCounterClockwiseCircularTokenHooks(
         Parser2HooksBase.SetCounterClockwiseCircularTokenHooks,
     ):
@@ -1543,14 +1564,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_draw_mode(DrawMode.CounterclockwiseCircular)
             return super().on_parser_visit_token(token, context)
 
     class CommentTokenHooks(Parser2HooksBase.CommentTokenHooks):
         """Hooks for visiting comment token (G04)."""
 
@@ -1568,14 +1590,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_is_region(is_region=True)
             context.set_region_command_buffer()
 
             return super().on_parser_visit_token(token, context)
 
     class EndRegionTokenHooks(Parser2HooksBase.EndRegionTokenHooks):
@@ -1592,14 +1615,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_is_region(is_region=False)
             command_buffer = context.get_region_command_buffer()
 
             context.add_command(
                 Region2(
                     aperture_attributes=context.aperture_attributes,
@@ -1628,14 +1652,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             self.hooks.select_aperture.on_parser_visit_token(token, context)
             return super().on_parser_visit_token(token, context)
 
     class SetUnitInchTokenHooks(Parser2HooksBase.SetUnitInchTokenHooks):
         """Hooks for visiting set unit inch token (G70)."""
 
@@ -1650,14 +1675,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_draw_units(Unit.Inches)
             return super().on_parser_visit_token(token, context)
 
     class SetUnitMillimetersTokenHooks(Parser2HooksBase.SetUnitMillimetersTokenHooks):
         """Hooks for visiting set unit millimeters token (G71)."""
 
@@ -1672,14 +1698,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_draw_units(Unit.Millimeters)
             return super().on_parser_visit_token(token, context)
 
     class SetSingleQuadrantModeTokenHooks(
         Parser2HooksBase.SetSingleQuadrantModeTokenHooks,
     ):
@@ -1696,14 +1723,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_is_multi_quadrant(is_multi_quadrant=False)
             return super().on_parser_visit_token(token, context)
 
     class SetMultiQuadrantModeTokenHooks(
         Parser2HooksBase.SetMultiQuadrantModeTokenHooks,
     ):
@@ -1720,14 +1748,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_is_multi_quadrant(is_multi_quadrant=True)
             return super().on_parser_visit_token(token, context)
 
     class SetCoordinateAbsoluteTokenHooks(
         Parser2HooksBase.SetCoordinateAbsoluteTokenHooks,
     ):
@@ -1744,14 +1773,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             # NOOP - only absolute format supported.
             return super().on_parser_visit_token(token, context)
 
     class SetCoordinateIncrementalTokenHooks(
         Parser2HooksBase.SetCoordinateIncrementalTokenHooks,
     ):
@@ -1768,14 +1798,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             raise IncrementalCoordinatesNotSupported2Error
 
     class ImageNameTokenHooks(Parser2HooksBase.ImageNameTokenHooks):
         """Hooks for visiting image name token (IN)."""
 
         def on_parser_visit_token(
@@ -1789,14 +1820,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_image_name(token.content)
             return super().on_parser_visit_token(token, context)
 
     class InvalidTokenHooks(Parser2HooksBase.InvalidTokenHooks):
         """Hooks for visiting invalid token."""
 
@@ -1814,14 +1846,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_is_output_image_negation_required(
                 value=(token.image_polarity == ImagePolarityEnum.NEGATIVE),
             )
             return super().on_parser_visit_token(token, context)
 
     class LoadMirroringTokenHooks(Parser2HooksBase.LoadMirroringTokenHooks):
@@ -1838,14 +1871,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_mirroring(token.mirroring)
             return super().on_parser_visit_token(token, context)
 
     class LoadNameTokenHooks(Parser2HooksBase.LoadNameTokenHooks):
         """Hooks for visiting load name token (LN)."""
 
@@ -1860,14 +1894,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_file_name(token.content)
             return super().on_parser_visit_token(token, context)
 
     class LoadPolarityTokenHooks(Parser2HooksBase.LoadPolarityTokenHooks):
         """Hooks for visiting load polarity token (LP)."""
 
@@ -1882,14 +1917,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_polarity(token.polarity)
             return super().on_parser_visit_token(token, context)
 
     class LoadRotationTokenHooks(Parser2HooksBase.LoadRotationTokenHooks):
         """Hooks for visiting load rotation token (LR)."""
 
@@ -1904,14 +1940,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_rotation(token.rotation)
             return super().on_parser_visit_token(token, context)
 
     class LoadScalingTokenHooks(Parser2HooksBase.LoadScalingTokenHooks):
         """Hooks for visiting load scaling token (LS)."""
 
@@ -1926,14 +1963,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_scaling(token.scaling)
             return super().on_parser_visit_token(token, context)
 
     class ProgramStopTokenHooks(Parser2HooksBase.ProgramStopTokenHooks):
         """Hooks for visiting program stop token (M00)."""
 
@@ -1948,14 +1986,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_reached_program_stop()
             context.halt_parser()
 
     class OptionalStopTokenHooks(Parser2HooksBase.OptionalStopTokenHooks):
         """Hooks for visiting optional stop token (M01)."""
 
@@ -1981,14 +2020,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_reached_end_of_file()
             context.halt_parser()
 
     class UnitModeTokenHooks(Parser2HooksBase.UnitModeTokenHooks):
         """Hooks for visiting unit mode token (MO)."""
 
@@ -2003,14 +2043,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_draw_units(token.unit)
             return super().on_parser_visit_token(token, context)
 
     class ImageOffsetTokenHooks(Parser2HooksBase.ImageOffsetTokenHooks):
         """Hooks for visiting image offset token (OF)."""
 
@@ -2028,14 +2069,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_state_before_step_and_repeat()
 
             context.set_is_step_and_repeat(is_step_and_repeat=True)
             context.set_x_repeat(token.x_repeat)
             context.set_y_repeat(token.y_repeat)
             context.set_x_step(Offset.new(token.x_step, unit=context.get_draw_units()))
@@ -2058,14 +2100,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             if context.get_is_step_and_repeat() is False:
                 raise StepAndRepeatNotInitializedError(token)
 
             command_buffer = context.get_step_and_repeat_command_buffer().get_readonly()
             commands: list[Command2] = []
 
@@ -2108,14 +2151,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_aperture_attribute(token.name, token.value)
             return super().on_parser_visit_token(token, context)
 
     class DeleteAttributeHooks(Parser2HooksBase.DeleteAttributeHooks):
         """Hooks for visiting delete attribute token (TD)."""
 
@@ -2130,14 +2174,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             if token.name is not None:
                 context.delete_aperture_attribute(token.name)
                 context.delete_object_attribute(token.name)
             else:
                 context.clear_aperture_attributes()
                 context.clear_object_attributes()
@@ -2157,14 +2202,15 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_file_attribute(token.name, token.value)
             return super().on_parser_visit_token(token, context)
 
     class ObjectAttributeHooks(Parser2HooksBase.ObjectAttributeHooks):
         """Hooks for visiting object attribute token (TO)."""
 
@@ -2179,10 +2225,11 @@
 
             Parameters
             ----------
             token: TokenT
                 The token that is being visited.
             context : Parser2Context
                 The context object containing information about the parser state.
+
             """
             context.set_object_attribute(token.name, token.value)
             return super().on_parser_visit_token(token, context)
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/parser2hooks_base.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks_base.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/parser2/state2.py` & `pygerber-2.3.1/src/pygerber/gerberx3/parser2/state2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/renderer2/abstract.py` & `pygerber-2.3.1/src/pygerber/gerberx3/renderer2/abstract.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/renderer2/raster.py` & `pygerber-2.3.1/src/pygerber/gerberx3/renderer2/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,18 +572,35 @@
 
         if raster_aperture is None:
             self.push_render_frame(
                 self.frame_builder.set_polarity(command.transform.polarity)
                 .set_command_buffer_from_list([command])
                 .build(),
             )
+            max_xy = command.flash_point + Vector2D(
+                x=aperture.x_size / 2,
+                y=aperture.y_size / 2,
+            )
+
+            min_xy = command.flash_point - Vector2D(
+                x=aperture.x_size / 2,
+                y=aperture.y_size / 2,
+            )
+
+            start_xy = min_xy.get_rotated(aperture.rotation)
+            end_xy = max_xy.get_rotated(aperture.rotation)
 
-            self.frame.rectangle(
+            self.frame.polygon(
                 Polarity.Dark,
-                self.convert_bbox(command.get_bounding_box()),
+                (
+                    (self.convert_x(start_xy.x), self.convert_y(start_xy.y)),
+                    (self.convert_x(end_xy.x), self.convert_y(start_xy.y)),
+                    (self.convert_x(end_xy.x), self.convert_y(end_xy.y)),
+                    (self.convert_x(start_xy.x), self.convert_y(end_xy.y)),
+                ),
             )
             self._make_hole(command, aperture)
 
             frame = self.pop_render_frame()
             raster_aperture = frame.get_aperture()
             self.set_aperture(aperture_id, raster_aperture)
 
@@ -599,15 +616,18 @@
                 self.frame_builder.set_polarity(command.transform.polarity)
                 .set_command_buffer_from_list([command])
                 .build(),
             )
 
             self.frame.rounded_rectangle(
                 Polarity.Dark,
-                self.convert_bbox(command.get_bounding_box()),
+                self.convert_bbox(
+                    BoundingBox.from_rectangle(aperture.x_size, aperture.y_size)
+                    + command.flash_point,
+                ),
                 radius=min(
                     self.convert_size(aperture.x_size),
                     self.convert_size(aperture.y_size),
                 )
                 / 2,
             )
             self._make_hole(command, aperture)
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/renderer2/svg.py` & `pygerber-2.3.1/src/pygerber/gerberx3/renderer2/svg.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 if IS_SVG_BACKEND_AVAILABLE:
     import drawsvg
 
     @dataclass
     class SvgRenderingFrame:
         """Rendering variable container."""
 
-        command_buffer: ReadonlyCommandBuffer2
         bounding_box: BoundingBox
         normalize_origin_to_0_0: bool
         mask: drawsvg.Mask = field(default_factory=drawsvg.Mask)
         group: drawsvg.Group = field(default_factory=drawsvg.Group)
         polarity: Optional[Polarity] = None
         is_region: bool = False
         flip_y: bool = True
@@ -110,34 +109,32 @@
         if not isinstance(renderer, SvgRenderer2):
             raise NotImplementedError
 
         self.renderer = renderer
         self.command_buffer = command_buffer
         self.rendering_stack: list[SvgRenderingFrame] = [
             SvgRenderingFrame(
-                command_buffer=self.command_buffer,
                 bounding_box=self.command_buffer.get_bounding_box(),
                 normalize_origin_to_0_0=True,
                 flip_y=self.flip_y,
             ),
         ]
         self.apertures: dict[str, drawsvg.Group] = {}
 
     def push_render_frame(
         self,
-        cmd: ReadonlyCommandBuffer2,
+        bbox: BoundingBox,
         *,
         normalize_origin_to_0_0: bool,
         flip_y: bool,
     ) -> None:
         """Push new segment render frame."""
         self.rendering_stack.append(
             SvgRenderingFrame(
-                command_buffer=cmd,
-                bounding_box=cmd.get_bounding_box(),
+                bounding_box=bbox,
                 normalize_origin_to_0_0=normalize_origin_to_0_0,
                 flip_y=flip_y,
             ),
         )
 
     def pop_render_frame(self) -> SvgRenderingFrame:
         """Pop segment render frame."""
@@ -203,18 +200,18 @@
 
     def create_full_mask(self) -> drawsvg.Mask:
         """Create mask covering whole image."""
         bbox = self.base_frame.bounding_box
         mask = drawsvg.Mask()
         mask.append(
             drawsvg.Rectangle(
-                x=0,
-                y=0,
-                width=self.convert_size(bbox.width),
-                height=self.convert_size(bbox.height),
+                x=self.convert_size(-bbox.width / 2),
+                y=self.convert_size(-bbox.height / 2),
+                width=self.convert_size(bbox.width * 2),
+                height=self.convert_size(bbox.height * 2),
                 fill="white",
             ),
         )
         return mask
 
     def create_mask(self, bbox: BoundingBox) -> drawsvg.Mask:
         """Create mask covering specified bounding box."""
@@ -549,14 +546,15 @@
             aperture_group.append(
                 drawsvg.Rectangle(
                     -self.convert_size(aperture.x_size) / 2,
                     -self.convert_size(aperture.y_size) / 2,
                     self.convert_size(aperture.x_size),
                     self.convert_size(aperture.y_size),
                     fill=color,
+                    transform=f"rotate({aperture.rotation})",
                 ),
             )
             self.set_aperture(aperture_id, aperture_group)
 
         self.add_element_to_frame(
             command.transform.polarity,
             drawsvg.Use(
@@ -587,14 +585,15 @@
                     -self.convert_size(aperture.x_size) / 2,
                     -self.convert_size(aperture.y_size) / 2,
                     x_size,
                     y_size,
                     fill=color,
                     rx=radius,
                     ry=radius,
+                    transform=f"rotate({aperture.rotation})",
                 ),
             )
             self.set_aperture(aperture_id, aperture_group)
 
         self.add_element_to_frame(
             command.transform.polarity,
             drawsvg.Use(
@@ -658,15 +657,15 @@
         """Render flash macro aperture to target image."""
         transform = command.transform
         aperture_id = self.get_aperture_id(aperture, transform)
         aperture_group = self.get_aperture(aperture_id)
 
         if aperture_group is None:
             self.push_render_frame(
-                aperture.command_buffer,
+                command.get_bounding_box(),
                 normalize_origin_to_0_0=False,
                 flip_y=False,
             )
             for cmd in aperture.command_buffer:
                 cmd.render(self.renderer)
 
             frame = self.pop_render_frame()
```

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/revisions.py` & `pygerber-2.3.1/src/pygerber/gerberx3/revisions.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/state_enums.py` & `pygerber-2.3.1/src/pygerber/gerberx3/state_enums.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/aperture_id.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/aperture_id.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/decorators.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/decorators.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.ebnf` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.ebnf`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/grammar.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokenizer.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py` & `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/src/pygerber/sequence_tools.py` & `pygerber-2.3.1/src/pygerber/sequence_tools.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.0/PKG-INFO` & `pygerber-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygerber
-Version: 2.3.0
+Version: 2.3.1
 Summary: Parsing, formatting and rendering toolkit for Gerber X3 file format
 Home-page: https://www.facebook.com/pygerber
 License: MIT
 Keywords: gerber,pcb,embedded,images,x3
 Author: Krzysztof Wisniewski
 Author-email: argmaster.world@gmail.com
 Requires-Python: >=3.8,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygerber Version: 2.3.0 Summary: Parsing,
+Metadata-Version: 2.1 Name: pygerber Version: 2.3.1 Summary: Parsing,
 formatting and rendering toolkit for Gerber X3 file format Home-page: https://
 www.facebook.com/pygerber License: MIT Keywords: gerber,pcb,embedded,images,x3
 Author: Krzysztof Wisniewski Author-email: argmaster.world@gmail.com Requires-
 Python: >=3.8,<3.13 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience ::
```

