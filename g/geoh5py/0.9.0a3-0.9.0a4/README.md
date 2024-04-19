# Comparing `tmp/geoh5py-0.9.0a3.tar.gz` & `tmp/geoh5py-0.9.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.9.0a3.tar", max compression
+gzip compressed data, was "geoh5py-0.9.0a4.tar", max compression
```

## Comparing `geoh5py-0.9.0a3.tar` & `geoh5py-0.9.0a4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0      841 2024-04-12 18:06:37.656160 geoh5py-0.9.0a3/geoh5py/__init__.py
--rw-r--r--   0        0        0     1574 2024-01-31 17:10:26.210995 geoh5py-0.9.0a3/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2024-01-31 17:10:26.210995 geoh5py-0.9.0a3/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     2005 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/data/boolean_data.py
--rw-r--r--   0        0        0     3756 2024-04-12 17:42:35.137291 geoh5py-0.9.0a3/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8914 2024-04-12 17:42:35.137291 geoh5py-0.9.0a3/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.212998 geoh5py-0.9.0a3/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0    13377 2024-04-12 17:42:35.137291 geoh5py-0.9.0a3/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.213988 geoh5py-0.9.0a3/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2024-01-31 17:10:26.213988 geoh5py-0.9.0a3/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3690 2024-01-31 17:10:26.213988 geoh5py-0.9.0a3/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1787 2024-01-31 17:10:26.214988 geoh5py-0.9.0a3/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2024-01-31 17:10:26.214988 geoh5py-0.9.0a3/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     1709 2024-01-31 17:10:26.214988 geoh5py-0.9.0a3/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     4001 2024-01-31 17:10:26.215988 geoh5py-0.9.0a3/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1121 2024-01-31 17:10:26.215988 geoh5py-0.9.0a3/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     2896 2024-04-12 17:42:35.138630 geoh5py-0.9.0a3/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2024-01-31 17:10:26.216996 geoh5py-0.9.0a3/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     5093 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1573 2024-01-31 17:10:26.216996 geoh5py-0.9.0a3/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     4559 2024-01-31 17:10:26.217996 geoh5py-0.9.0a3/geoh5py/data/visual_parameters.py
--rw-r--r--   0        0        0     1587 2024-01-31 17:10:26.217996 geoh5py-0.9.0a3/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1441 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1474 2024-04-12 17:42:35.139243 geoh5py-0.9.0a3/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1797 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1444 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     7068 2024-04-12 17:42:35.139513 geoh5py-0.9.0a3/geoh5py/groups/group.py
--rw-r--r--   0        0        0     2517 2024-04-12 17:42:35.139932 geoh5py-0.9.0a3/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     6714 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1295 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1414 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     7843 2024-04-12 17:42:35.139932 geoh5py-0.9.0a3/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2024-01-31 17:10:26.221995 geoh5py-0.9.0a3/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2053 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1322 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2024-01-31 17:10:26.228996 geoh5py-0.9.0a3/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17355 2024-04-12 17:42:35.139932 geoh5py-0.9.0a3/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    34866 2024-04-12 17:42:35.141445 geoh5py-0.9.0a3/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     2403 2024-01-31 17:10:26.229997 geoh5py-0.9.0a3/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9440 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7874 2024-01-31 17:10:26.230995 geoh5py-0.9.0a3/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6300 2024-04-12 17:42:35.141445 geoh5py-0.9.0a3/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     6204 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    26674 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    21664 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    14054 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4879 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1957 2024-01-31 17:10:26.233995 geoh5py-0.9.0a3/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2921 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2686 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    21773 2024-04-12 17:42:35.141445 geoh5py-0.9.0a3/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     1098 2024-04-12 17:42:35.142822 geoh5py-0.9.0a3/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13455 2024-04-12 17:42:35.142822 geoh5py-0.9.0a3/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5354 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2024-01-31 17:10:26.236988 geoh5py-0.9.0a3/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2024-01-31 17:10:26.236988 geoh5py-0.9.0a3/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14521 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2024-01-31 17:10:26.237995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     3660 2024-01-31 17:10:26.238995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
--rw-r--r--   0        0        0     3629 2024-01-31 17:10:26.238995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    36522 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0     6925 2024-01-31 17:10:26.239995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_fem.py
--rw-r--r--   0        0        0     6937 2024-01-31 17:10:26.240997 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2615 2024-01-31 17:10:26.240997 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     6605 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2024-01-31 17:10:26.241996 geoh5py-0.9.0a3/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2023-05-16 13:39:30.036442 geoh5py-0.9.0a3/geoh5py/py.typed
--rw-r--r--   0        0        0     1013 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0     1057 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/concatenation/__init__.py
--rw-r--r--   0        0        0     1847 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenated.py
--rw-r--r--   0        0        0    25972 2024-04-12 17:42:35.144031 geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenator.py
--rw-r--r--   0        0        0     3029 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/concatenation/data.py
--rw-r--r--   0        0        0    14282 2024-04-12 17:42:35.144031 geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillhole.py
--rw-r--r--   0        0        0    15847 2024-04-12 17:42:35.144771 geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillholes_group_table.py
--rw-r--r--   0        0        0     6729 2024-04-12 17:42:35.145267 geoh5py-0.9.0a3/geoh5py/shared/concatenation/object.py
--rw-r--r--   0        0        0     5193 2024-04-12 17:42:35.145267 geoh5py-0.9.0a3/geoh5py/shared/concatenation/property_group.py
--rw-r--r--   0        0        0      937 2024-01-31 17:10:26.245988 geoh5py-0.9.0a3/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4426 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     5694 2024-01-31 17:10:26.247000 geoh5py-0.9.0a3/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0    10840 2024-01-31 17:10:26.247996 geoh5py-0.9.0a3/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    10730 2024-04-12 17:42:35.145267 geoh5py-0.9.0a3/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     7630 2024-04-12 17:42:35.146468 geoh5py-0.9.0a3/geoh5py/shared/entity_container.py
--rw-r--r--   0        0        0     8632 2024-04-12 17:42:35.146468 geoh5py-0.9.0a3/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     8353 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0      923 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/merging/__init__.py
--rw-r--r--   0        0        0     7734 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/merging/base.py
--rw-r--r--   0        0        0     2336 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/merging/cell.py
--rw-r--r--   0        0        0     6105 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/merging/drape_model.py
--rw-r--r--   0        0        0     1845 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/merging/points.py
--rw-r--r--   0        0        0    21424 2024-04-12 17:42:35.147275 geoh5py-0.9.0a3/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8847 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2024-01-31 17:10:26.252997 geoh5py-0.9.0a3/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      959 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2991 2024-01-31 17:10:26.253990 geoh5py-0.9.0a3/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0     1983 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/descriptors.py
--rw-r--r--   0        0        0    11461 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/enforcers.py
--rw-r--r--   0        0        0    18309 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/forms.py
--rw-r--r--   0        0        0    18789 2024-04-12 17:42:35.147275 geoh5py-0.9.0a3/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0     4945 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/parameters.py
--rw-r--r--   0        0        0    15250 2024-04-12 17:42:35.148339 geoh5py-0.9.0a3/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0     5076 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/ui_json.py
--rw-r--r--   0        0        0    11199 2024-04-12 17:42:35.148922 geoh5py-0.9.0a3/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    11408 2024-04-12 17:42:35.148922 geoh5py-0.9.0a3/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2024-01-31 17:10:26.258592 geoh5py-0.9.0a3/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    50970 2024-04-12 17:42:35.150153 geoh5py-0.9.0a3/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2024-01-31 17:10:26.259585 geoh5py-0.9.0a3/package.rst
--rw-r--r--   0        0        0     2211 2024-04-12 18:06:37.656160 geoh5py-0.9.0a3/pyproject.toml
--rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 geoh5py-0.9.0a3/PKG-INFO
+-rw-r--r--   0        0        0      841 2024-04-19 19:50:27.441074 geoh5py-0.9.0a4/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1574 2024-01-31 17:10:26.210995 geoh5py-0.9.0a4/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2024-01-31 17:10:26.210995 geoh5py-0.9.0a4/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     2005 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/data/boolean_data.py
+-rw-r--r--   0        0        0     3756 2024-04-12 17:42:35.137291 geoh5py-0.9.0a4/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8914 2024-04-12 17:42:35.137291 geoh5py-0.9.0a4/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.212998 geoh5py-0.9.0a4/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0    13377 2024-04-12 17:42:35.137291 geoh5py-0.9.0a4/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.213988 geoh5py-0.9.0a4/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2024-01-31 17:10:26.213988 geoh5py-0.9.0a4/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3690 2024-01-31 17:10:26.213988 geoh5py-0.9.0a4/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1787 2024-01-31 17:10:26.214988 geoh5py-0.9.0a4/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2024-01-31 17:10:26.214988 geoh5py-0.9.0a4/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     1709 2024-01-31 17:10:26.214988 geoh5py-0.9.0a4/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     4001 2024-01-31 17:10:26.215988 geoh5py-0.9.0a4/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1121 2024-01-31 17:10:26.215988 geoh5py-0.9.0a4/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     2896 2024-04-12 17:42:35.138630 geoh5py-0.9.0a4/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2024-01-31 17:10:26.216996 geoh5py-0.9.0a4/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     5093 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1573 2024-01-31 17:10:26.216996 geoh5py-0.9.0a4/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     4559 2024-01-31 17:10:26.217996 geoh5py-0.9.0a4/geoh5py/data/visual_parameters.py
+-rw-r--r--   0        0        0     1587 2024-01-31 17:10:26.217996 geoh5py-0.9.0a4/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1441 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1474 2024-04-12 17:42:35.139243 geoh5py-0.9.0a4/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1797 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1444 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     7068 2024-04-12 17:42:35.139513 geoh5py-0.9.0a4/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     2517 2024-04-12 17:42:35.139932 geoh5py-0.9.0a4/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     6714 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1295 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1414 2024-04-12 17:41:26.545326 geoh5py-0.9.0a4/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     7843 2024-04-12 17:42:35.139932 geoh5py-0.9.0a4/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2024-01-31 17:10:26.221995 geoh5py-0.9.0a4/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2053 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1322 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2024-01-31 17:10:26.228996 geoh5py-0.9.0a4/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17355 2024-04-12 17:42:35.139932 geoh5py-0.9.0a4/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    34805 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2403 2024-01-31 17:10:26.229997 geoh5py-0.9.0a4/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9440 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7873 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6300 2024-04-12 17:42:35.141445 geoh5py-0.9.0a4/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     6204 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    26674 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    21867 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    14054 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4879 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1957 2024-01-31 17:10:26.233995 geoh5py-0.9.0a4/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2921 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2686 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    21991 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     1098 2024-04-12 17:42:35.142822 geoh5py-0.9.0a4/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13455 2024-04-12 17:42:35.142822 geoh5py-0.9.0a4/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5353 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2024-01-31 17:10:26.236988 geoh5py-0.9.0a4/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2024-01-31 17:10:26.236988 geoh5py-0.9.0a4/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14521 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2024-01-31 17:10:26.237995 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2024-01-31 17:10:26.238995 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2024-01-31 17:10:26.238995 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    36522 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2024-01-31 17:10:26.239995 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     6937 2024-01-31 17:10:26.240997 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2024-01-31 17:10:26.240997 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6605 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2024-01-31 17:10:26.241996 geoh5py-0.9.0a4/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:39:30.036442 geoh5py-0.9.0a4/geoh5py/py.typed
+-rw-r--r--   0        0        0     1013 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/concatenation/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/concatenation/concatenated.py
+-rw-r--r--   0        0        0    25972 2024-04-12 17:42:35.144031 geoh5py-0.9.0a4/geoh5py/shared/concatenation/concatenator.py
+-rw-r--r--   0        0        0     3029 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/concatenation/data.py
+-rw-r--r--   0        0        0    14282 2024-04-12 17:42:35.144031 geoh5py-0.9.0a4/geoh5py/shared/concatenation/drillhole.py
+-rw-r--r--   0        0        0    15847 2024-04-12 17:42:35.144771 geoh5py-0.9.0a4/geoh5py/shared/concatenation/drillholes_group_table.py
+-rw-r--r--   0        0        0     6729 2024-04-12 17:42:35.145267 geoh5py-0.9.0a4/geoh5py/shared/concatenation/object.py
+-rw-r--r--   0        0        0     5193 2024-04-12 17:42:35.145267 geoh5py-0.9.0a4/geoh5py/shared/concatenation/property_group.py
+-rw-r--r--   0        0        0      937 2024-01-31 17:10:26.245988 geoh5py-0.9.0a4/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4426 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     5629 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0    10840 2024-01-31 17:10:26.247996 geoh5py-0.9.0a4/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    10730 2024-04-12 17:42:35.145267 geoh5py-0.9.0a4/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     7630 2024-04-12 17:42:35.146468 geoh5py-0.9.0a4/geoh5py/shared/entity_container.py
+-rw-r--r--   0        0        0     8632 2024-04-12 17:42:35.146468 geoh5py-0.9.0a4/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     8353 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0      923 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/merging/__init__.py
+-rw-r--r--   0        0        0     7734 2024-04-12 17:41:26.560944 geoh5py-0.9.0a4/geoh5py/shared/merging/base.py
+-rw-r--r--   0        0        0     2336 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/shared/merging/cell.py
+-rw-r--r--   0        0        0     6105 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/shared/merging/drape_model.py
+-rw-r--r--   0        0        0     1845 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/shared/merging/points.py
+-rw-r--r--   0        0        0    21424 2024-04-12 17:42:35.147275 geoh5py-0.9.0a4/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     8847 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2024-01-31 17:10:26.252997 geoh5py-0.9.0a4/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      959 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2991 2024-01-31 17:10:26.253990 geoh5py-0.9.0a4/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0     1983 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/ui_json/descriptors.py
+-rw-r--r--   0        0        0    11461 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/ui_json/enforcers.py
+-rw-r--r--   0        0        0    18309 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/ui_json/forms.py
+-rw-r--r--   0        0        0    18789 2024-04-12 17:42:35.147275 geoh5py-0.9.0a4/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0     4945 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/ui_json/parameters.py
+-rw-r--r--   0        0        0    15250 2024-04-12 17:42:35.148339 geoh5py-0.9.0a4/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0     5076 2024-04-12 17:41:26.576578 geoh5py-0.9.0a4/geoh5py/ui_json/ui_json.py
+-rw-r--r--   0        0        0    11199 2024-04-12 17:42:35.148922 geoh5py-0.9.0a4/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    11408 2024-04-12 17:42:35.148922 geoh5py-0.9.0a4/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2024-01-31 17:10:26.258592 geoh5py-0.9.0a4/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    51060 2024-04-19 19:49:37.873903 geoh5py-0.9.0a4/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2024-01-31 17:10:26.259585 geoh5py-0.9.0a4/package.rst
+-rw-r--r--   0        0        0     2211 2024-04-19 19:50:27.441074 geoh5py-0.9.0a4/pyproject.toml
+-rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 geoh5py-0.9.0a4/PKG-INFO
```

### Comparing `geoh5py-0.9.0a3/geoh5py/__init__.py` & `geoh5py-0.9.0a4/geoh5py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.9.0-alpha.3"
+__version__ = "0.9.0-alpha.4"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.9.0a3/geoh5py/data/__init__.py` & `geoh5py-0.9.0a4/geoh5py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/blob_data.py` & `geoh5py-0.9.0a4/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/boolean_data.py` & `geoh5py-0.9.0a4/geoh5py/data/boolean_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/color_map.py` & `geoh5py-0.9.0a4/geoh5py/data/color_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/data.py` & `geoh5py-0.9.0a4/geoh5py/data/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/data_association_enum.py` & `geoh5py-0.9.0a4/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/data_type.py` & `geoh5py-0.9.0a4/geoh5py/data/data_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/data_unit.py` & `geoh5py-0.9.0a4/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/datetime_data.py` & `geoh5py-0.9.0a4/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/filename_data.py` & `geoh5py-0.9.0a4/geoh5py/data/filename_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/float_data.py` & `geoh5py-0.9.0a4/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.9.0a4/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/integer_data.py` & `geoh5py-0.9.0a4/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/numeric_data.py` & `geoh5py-0.9.0a4/geoh5py/data/numeric_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.9.0a4/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/reference_value_map.py` & `geoh5py-0.9.0a4/geoh5py/data/reference_value_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/referenced_data.py` & `geoh5py-0.9.0a4/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/text_data.py` & `geoh5py-0.9.0a4/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/unknown_data.py` & `geoh5py-0.9.0a4/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/data/visual_parameters.py` & `geoh5py-0.9.0a4/geoh5py/data/visual_parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/__init__.py` & `geoh5py-0.9.0a4/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/container_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/custom_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/custom_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/drillhole_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/giftools_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/group.py` & `geoh5py-0.9.0a4/geoh5py/groups/group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/group_type.py` & `geoh5py-0.9.0a4/geoh5py/groups/group_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/integrator_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/integrator_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/maps_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/maps_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/notype_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/property_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/root_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/simpeg_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/simpeg_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/groups/survey_group.py` & `geoh5py-0.9.0a4/geoh5py/groups/survey_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/io/__init__.py` & `geoh5py-0.9.0a4/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/io/h5_reader.py` & `geoh5py-0.9.0a4/geoh5py/io/h5_reader.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/io/h5_writer.py` & `geoh5py-0.9.0a4/geoh5py/io/h5_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,35 +273,36 @@
             name = channel.replace("/", "\u2044")
             try:
                 del attr_handle[name]
                 entity.workspace.repack = True
             except KeyError:
                 pass
 
-            dict_values = getattr(entity, attribute)
+            values = getattr(entity, attribute).get(channel, None)
 
-            if channel in dict_values and len(dict_values[channel]) > 0:
+            if values is None:
+                return
 
-                values = dict_values[channel].copy()
+            if isinstance(values, np.ndarray):
 
-                if isinstance(values, np.ndarray):
+                if np.issubdtype(values.dtype, np.floating):
+                    values = values.astype(np.float32)
 
-                    if np.issubdtype(values.dtype, np.floating):
+                    if len(values) > 0:
                         values[np.isnan(values)] = FLOAT_NDV
-                        values = values.astype(np.float32)
 
-                    if np.issubdtype(values.dtype, np.str_):
-                        values = values.astype(h5py.special_dtype(vlen=str))
+                if np.issubdtype(values.dtype, np.str_):
+                    values = values.astype(h5py.special_dtype(vlen=str))
 
-                attr_handle.create_dataset(
-                    name,
-                    data=values,
-                    compression="gzip",
-                    compression_opts=9,
-                )
+            attr_handle.create_dataset(
+                name,
+                data=values,
+                compression="gzip",
+                compression_opts=9,
+            )
 
     @classmethod
     def update_field(
         cls,
         file: str | h5py.File,
         entity,
         attribute: str,
```

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/__init__.py` & `geoh5py-0.9.0a4/geoh5py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/block_model.py` & `geoh5py-0.9.0a4/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/cell_object.py` & `geoh5py-0.9.0a4/geoh5py/objects/cell_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         """
         Safely remove cells and corresponding data entries.
 
         :param indices: Indices of cells to be removed.
         :param clear_cache: Clear cache of data values.
         """
 
-        if self._cells is None:
+        if self.cells is None:
             warnings.warn("No cells to be removed.", UserWarning)
             return
 
         if isinstance(indices, (list, tuple)):
             indices = np.array(indices)
 
         if not isinstance(indices, np.ndarray):
```

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/curve.py` & `geoh5py-0.9.0a4/geoh5py/objects/curve.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/drape_model.py` & `geoh5py-0.9.0a4/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/drillhole.py` & `geoh5py-0.9.0a4/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/geo_image.py` & `geoh5py-0.9.0a4/geoh5py/objects/geo_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,16 @@
         """
         Create a :obj:`~geoh5py.data.filename_data.FilenameData`
         from dictionary of name and arguments.
         The provided arguments can be any property of the target Data class.
 
         :return: List of new Data objects.
         """
+        convert_to_grid = False
+        # todo: this should be changed in the future to accept tiff images
         if isinstance(image, np.ndarray) and image.ndim in [2, 3]:
             if image.ndim == 3 and image.shape[2] != 3:
                 raise ValueError(
                     "Shape of the 'image' must be a 2D or "
                     "a 3D array with shape(*,*, 3) representing 'RGB' values."
                 )
             value = image
@@ -367,29 +369,27 @@
             image = Image.fromarray(value)
 
         elif isinstance(image, str):
             if not Path(image).is_file():
                 raise ValueError(f"Input image file {image} does not exist.")
 
             image = Image.open(image)
-
-            # if the image is a tiff save tag information
-            if isinstance(image, TiffImageFile):
-                self.tag = image
-
         elif isinstance(image, bytes):
             image = Image.open(BytesIO(image))
-        elif isinstance(image, TiffImageFile):
-            self.tag = image
+
         elif not isinstance(image, Image.Image):
             raise ValueError(
                 "Input 'value' for the 'image' property must be "
                 "a 2D or 3D numpy.ndarray, bytes, PIL.Image or a path to an existing image."
                 f"Get type {type(image)} instead."
             )
+        # if the image is a tiff save tag information
+        if isinstance(image, TiffImageFile):
+            self.tag = image
+            convert_to_grid = True
 
         with TemporaryDirectory() as tempdir:
             if image.mode not in PILLOW_ARGUMENTS:
                 raise NotImplementedError(
                     f"The mode {image.mode} of the image is not supported."
                 )
 
@@ -399,14 +399,18 @@
             if self.image_data is not None:
                 self.workspace.remove_entity(self.image_data)
 
             image = self.add_file(str(temp_file))
             image.name = "GeoImageMesh_Image"
             image.entity_type.name = "GeoImageMesh_Image"
 
+        # quick and dirty fix: create a grid if image is tiff
+        if convert_to_grid:
+            self.to_grid2d(name=self.name + "_grid2d")
+
     @property
     def image_data(self):
         """
         Get the FilenameData entity holding the image.
         """
         for child in self.children:
             if isinstance(child, FilenameData) and child.name == "GeoImageMesh_Image":
```

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/grid2d.py` & `geoh5py-0.9.0a4/geoh5py/objects/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/grid_object.py` & `geoh5py-0.9.0a4/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/integrator.py` & `geoh5py-0.9.0a4/geoh5py/objects/integrator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/label.py` & `geoh5py-0.9.0a4/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/notype_object.py` & `geoh5py-0.9.0a4/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/object_base.py` & `geoh5py-0.9.0a4/geoh5py/objects/object_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,19 +531,23 @@
             indices = np.array(indices)
 
         if not isinstance(indices, np.ndarray):
             raise TypeError("Indices must be a list or numpy array.")
 
         for child in self.children:
             if (
-                getattr(child, "values", None) is not None
+                hasattr(child, "_values")
                 and isinstance(child.association, DataAssociationEnum)
                 and child.association.name == association
             ):
-                child.values = np.delete(child.values, indices, axis=0)
+                # accessing values with no property as the vertices had changed
+                values = getattr(child, "_values", None)
+                if values is None:
+                    values = child.workspace.fetch_values(child)
+                child.values = np.delete(values, indices, axis=0)
                 if clear_cache:
                     clear_array_attributes(child)
 
     @property
     def vertices(self) -> np.ndarray:
         r"""
         :obj:`numpy.array` of :obj:`float`, shape (\*, 3): Array of x, y, z coordinates
```

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/object_type.py` & `geoh5py-0.9.0a4/geoh5py/objects/object_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/octree.py` & `geoh5py-0.9.0a4/geoh5py/objects/octree.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/points.py` & `geoh5py-0.9.0a4/geoh5py/objects/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         """
         Safely remove vertices and corresponding data entries.
 
         :param indices: Indices of vertices to remove.
         :param clear_cache: Clear cached data and attributes.
         """
 
-        if self._vertices is None:
+        if self.vertices is None:
             warnings.warn("No vertices to be removed.", UserWarning)
             return
 
         if isinstance(indices, list):
             indices = np.array(indices)
 
         if not isinstance(indices, np.ndarray):
```

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surface.py` & `geoh5py-0.9.0a4/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/airborne_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/airborne_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/base.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_fem.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/ground_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_tem.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/ground_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.9.0a4/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/__init__.py` & `geoh5py-0.9.0a4/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/__init__.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenated.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/concatenated.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenator.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/concatenator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/data.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillhole.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillholes_group_table.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/drillholes_group_table.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/object.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/concatenation/property_group.py` & `geoh5py-0.9.0a4/geoh5py/shared/concatenation/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.9.0a4/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/conversion/base.py` & `geoh5py-0.9.0a4/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.9.0a4/geoh5py/shared/conversion/geo_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,42 +72,42 @@
     @staticmethod
     def add_gray_data(values: np.ndarray, output: Grid2D):
         """
         Send the image as gray in the new :obj:'geoh5py.objects.grid2d.Grid2D'.
         :param values: Input image values as an array of int.
         :param output: the new :obj:'geoh5py.objects.grid2d.Grid2D'.
         """
-        if values.ndim > 1:
-            values = np.asarray(Image.fromarray(values).convert("L"))
+        if values.ndim != 2:
+            raise ValueError("To export to gray image, the array must be 2d. ")
 
         output.add_data(
             data={
                 "band[0]": {
-                    "values": values.astype(np.uint32)[::-1].flatten(),
+                    "values": values[::-1].flatten(),
                     "association": "CELL",
                 }
             }
         )
 
     @staticmethod
     def add_color_data(values: np.ndarray, output: Grid2D):
         """
-        Send the image color bands to :obj:'geoh5py.data.integer_data.IntegerData'.
+        Send the image color bands to data.
 
         :param values: Input image values as an array of int.
         :param output: the new :obj:'geoh5py.objects.grid2d.Grid2D'.
         """
         if values.ndim != 3:
             raise IndexError("To export to color image, the array must be 3d.")
 
         for ind in range(values.shape[2]):
             output.add_data(
                 {
                     f"band[{ind}]": {
-                        "values": values.astype(np.uint32)[::-1, :, ind].flatten(),
+                        "values": values[::-1, :, ind].flatten(),
                         "association": "CELL",
                     }
                 }
             )
 
     @staticmethod
     def add_data_2dgrid(geoimage: Image, output: Grid2D):
```

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.9.0a4/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/entity.py` & `geoh5py-0.9.0a4/geoh5py/shared/entity.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/entity_container.py` & `geoh5py-0.9.0a4/geoh5py/shared/entity_container.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/entity_type.py` & `geoh5py-0.9.0a4/geoh5py/shared/entity_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/exceptions.py` & `geoh5py-0.9.0a4/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/merging/__init__.py` & `geoh5py-0.9.0a4/geoh5py/shared/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/merging/base.py` & `geoh5py-0.9.0a4/geoh5py/shared/merging/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/merging/cell.py` & `geoh5py-0.9.0a4/geoh5py/shared/merging/cell.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/merging/drape_model.py` & `geoh5py-0.9.0a4/geoh5py/shared/merging/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/merging/points.py` & `geoh5py-0.9.0a4/geoh5py/shared/merging/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/utils.py` & `geoh5py-0.9.0a4/geoh5py/shared/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/validators.py` & `geoh5py-0.9.0a4/geoh5py/shared/validators.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/shared/weakref_utils.py` & `geoh5py-0.9.0a4/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/__init__.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/constants.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/descriptors.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/descriptors.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/enforcers.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/enforcers.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/forms.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/forms.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/input_file.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/input_file.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/parameters.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/templates.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/templates.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/ui_json.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/ui_json.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/utils.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/ui_json/validation.py` & `geoh5py-0.9.0a4/geoh5py/ui_json/validation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/workspace/__init__.py` & `geoh5py-0.9.0a4/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/geoh5py/workspace/workspace.py` & `geoh5py-0.9.0a4/geoh5py/workspace/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,29 +715,32 @@
             entity_type = "group"
         elif isinstance(entity, ObjectBase):
             entity_type = "object"
 
         if isinstance(entity, RootGroup) and not entity.on_file:
             children_list = {child.uid: "" for child in entity.children}
 
-        elif isinstance(entity, Concatenator):
-            if any(entity.children):
-                return entity.children
-
-            cat_children = entity.fetch_concatenated_objects()
-            children_list = {
-                str2uuid(as_str_if_utf8_bytes(uid)): attr
-                for uid, attr in cat_children.items()
-            }
-
         else:
+
             children_list = self._io_call(
                 H5Reader.fetch_children, entity.uid, entity_type, mode="r"
             )
 
+            if isinstance(entity, Concatenator):
+                if any(entity.children):
+                    return entity.children
+
+                cat_children = entity.fetch_concatenated_objects()
+                children_list.update(
+                    {
+                        str2uuid(as_str_if_utf8_bytes(uid)): attr
+                        for uid, attr in cat_children.items()
+                    }
+                )
+
         family_tree = []
         for uid, child_type in children_list.items():
             recovered_object = self.get_entity(uid)[0]
             if recovered_object is None and not isinstance(entity, PropertyGroup):
                 recovered_object = self.load_entity(uid, child_type, parent=entity)
             if not (
                 recovered_object is None or isinstance(recovered_object, PropertyGroup)
```

### Comparing `geoh5py-0.9.0a3/package.rst` & `geoh5py-0.9.0a4/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a3/pyproject.toml` & `geoh5py-0.9.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.9.0-alpha.3"
+version = "0.9.0-alpha.4"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
 documentation = "https://geoh5py.readthedocs.io/en/latest/"
 homepage = "https://mirageoscience.com"
 readme = "package.rst"
```

### Comparing `geoh5py-0.9.0a3/PKG-INFO` & `geoh5py-0.9.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.9.0a3
+Version: 0.9.0a4
 Summary: Python API for geoh5, an open file format for geoscientific data
 Home-page: https://mirageoscience.com
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.8,<3.11
```

