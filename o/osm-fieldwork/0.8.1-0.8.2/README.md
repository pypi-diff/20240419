# Comparing `tmp/osm-fieldwork-0.8.1.tar.gz` & `tmp/osm-fieldwork-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.8.1.tar", last modified: Mon Apr 15 09:15:34 2024, max compression
+gzip compressed data, was "osm-fieldwork-0.8.2.tar", last modified: Fri Apr 19 15:41:07 2024, max compression
```

## Comparing `osm-fieldwork-0.8.1.tar` & `osm-fieldwork-0.8.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0    34102 2024-04-15 09:15:24.193102 osm-fieldwork-0.8.1/LICENSE.md
--rw-r--r--   0        0        0    14494 2024-04-15 09:15:24.193102 osm-fieldwork-0.8.1/README.md
--rwxr-xr-x   0        0        0    13091 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5037 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     5072 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     4919 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    60904 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/OdkCentral.py
--rwxr-xr-x   0        0        0    24065 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/OdkCentralAsync.py
--rw-r--r--   0        0        0       99 2024-04-15 09:15:24.197102 osm-fieldwork-0.8.1/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       22 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0    20165 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0    11364 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      883 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/__init__.py
--rw-r--r--   0        0        0      387 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      348 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      247 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      777 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      126 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      437 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      126 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      490 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0      193 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/highways.yaml
--rw-r--r--   0        0        0       80 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0       90 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0       88 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0       91 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0        0 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/taginfo-db.db
--rw-r--r--   0        0        0      253 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4391 2024-04-15 09:15:24.201102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      415 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      185 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      128 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     8929 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/filter_data.py
--rw-r--r--   0        0        0      798 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/imagery.yaml
--rwxr-xr-x   0        0        0    15977 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0     7371 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/make_data_extract.py
--rw-r--r--   0        0        0     3405 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/models.yaml
--rwxr-xr-x   0        0        0     5416 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0     4298 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/odk2geojson.py
--rwxr-xr-x   0        0        0     5348 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/odk2osm.py
--rwxr-xr-x   0        0        0    17845 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0    23342 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0     5302 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/osm2favorities.py
--rwxr-xr-x   0        0        0    15231 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     9381 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     3717 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0     3795 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0     1151 2024-04-15 09:15:24.205102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2024-04-15 09:15:24.209102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2024-04-15 09:15:24.209102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2024-04-15 09:15:24.217102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0      299 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/entities/__init__.py
--rw-r--r--   0        0        0   111104 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/entities/registration_form.xls
--rw-r--r--   0        0        0     3039 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/entities/registration_form.xml
--rw-r--r--   0        0        0    69120 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    40448 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/highways.xls
--rw-r--r--   0        0        0    22528 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0   115963 2024-04-15 09:15:24.221102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   265216 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/test.xls
--rw-r--r--   0        0        0   353280 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/thamel.xls
--rw-r--r--   0        0        0   118272 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     5443 2024-04-15 09:15:24.225102 osm-fieldwork-0.8.1/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     3599 2024-04-15 09:15:24.229102 osm-fieldwork-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    15261 1970-01-01 00:00:00.000000 osm-fieldwork-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34102 2024-04-19 15:40:57.748119 osm-fieldwork-0.8.2/LICENSE.md
+-rw-r--r--   0        0        0    14494 2024-04-19 15:40:57.748119 osm-fieldwork-0.8.2/README.md
+-rwxr-xr-x   0        0        0    13091 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5037 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     5072 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4919 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    61173 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/OdkCentral.py
+-rwxr-xr-x   0        0        0    25540 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/OdkCentralAsync.py
+-rw-r--r--   0        0        0       99 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0    20165 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0    11364 2024-04-19 15:40:57.756119 osm-fieldwork-0.8.2/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      883 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      348 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      247 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      777 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      126 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      437 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      126 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      490 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0      193 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/highways.yaml
+-rw-r--r--   0        0        0       80 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0       90 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0       88 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0       91 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0        0 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/taginfo-db.db
+-rw-r--r--   0        0        0      253 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4391 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      415 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      185 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      128 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     8929 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/filter_data.py
+-rw-r--r--   0        0        0      798 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/imagery.yaml
+-rwxr-xr-x   0        0        0    15977 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0     7371 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/make_data_extract.py
+-rw-r--r--   0        0        0     3405 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/models.yaml
+-rwxr-xr-x   0        0        0     5416 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4298 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0     5348 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/odk2osm.py
+-rwxr-xr-x   0        0        0    17845 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0    23342 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5302 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    15231 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     9381 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     3717 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0     3795 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0     1151 2024-04-19 15:40:57.760119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2024-04-19 15:40:57.764119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2024-04-19 15:40:57.764119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0      299 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/entities/__init__.py
+-rw-r--r--   0        0        0   111104 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/entities/registration_form.xls
+-rw-r--r--   0        0        0     3039 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/entities/registration_form.xml
+-rw-r--r--   0        0        0    69120 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    40448 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/highways.xls
+-rw-r--r--   0        0        0    22528 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2024-04-19 15:40:57.776119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0   115963 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   265216 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/test.xls
+-rw-r--r--   0        0        0   353280 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/thamel.xls
+-rw-r--r--   0        0        0   118272 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2024-04-19 15:40:57.780119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2024-04-19 15:40:57.784119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2024-04-19 15:40:57.784119 osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     5443 2024-04-19 15:40:57.784119 osm-fieldwork-0.8.2/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     3599 2024-04-19 15:40:57.784119 osm-fieldwork-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    15261 1970-01-01 00:00:00.000000 osm-fieldwork-0.8.2/PKG-INFO
```

### Comparing `osm-fieldwork-0.8.1/LICENSE.md` & `osm-fieldwork-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/README.md` & `osm-fieldwork-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.8.2/osm_fieldwork/CSVDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.8.2/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.8.2/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/ODKInstance.py` & `osm-fieldwork-0.8.2/osm_fieldwork/ODKInstance.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.8.2/osm_fieldwork/OdkCentral.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,26 +181,32 @@
             self.user = user
         if not self.passwd:
             self.passwd = passwd
         # Enable persistent connection, create a cookie for this session
         self.session.headers.update({"accept": "odkcentral"})
 
         # Get a session token
-        response = self.session.post(
-            f"{self.base}sessions",
-            json={
-                "email": self.user,
-                "password": self.passwd,
-            },
-        )
+        try:
+            response = self.session.post(
+                f"{self.base}sessions",
+                json={
+                    "email": self.user,
+                    "password": self.passwd,
+                },
+            )
+        except requests.exceptions.ConnectionError as request_error:
+            # URL does not exist
+            raise ConnectionError("Failed to connect to Central. Is the URL valid?") from request_error
+
         if response.status_code == 401:
             # Unauthorized, invalid credentials
-            raise ValueError("ODK credentials are invalid, or may have been updated. Please update them.")
+            raise ConnectionError("ODK credentials are invalid, or may have changed. Please update them.") from None
         elif not response.ok:
-            response.raise_for_status()  # Handle other errors
+            # Handle other errors
+            response.raise_for_status()
 
         self.session.headers.update({"Authorization": f"Bearer {response.json().get('token')}"})
 
         # Connect to the server
         return self.session.get(self.url, verify=self.verify)
 
     def listProjects(self):
```

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/OdkCentralAsync.py` & `osm-fieldwork-0.8.2/osm_fieldwork/OdkCentralAsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,26 @@
     async def __aexit__(self, exc_type, exc_value, traceback):
         """Async object close."""
         if self.session:
             await self.session.close()
 
     async def authenticate(self):
         """Authenticate to an ODK Central server."""
-        async with self.session.post(f"{self.base}sessions", json={"email": self.user, "password": self.passwd}) as response:
-            token = (await response.json())["token"]
-            self.session.headers.update({"Authorization": f"Bearer {token}"})
+        try:
+            async with self.session.post(f"{self.base}sessions", json={"email": self.user, "password": self.passwd}) as response:
+                token = (await response.json())["token"]
+                self.session.headers.update({"Authorization": f"Bearer {token}"})
+        except aiohttp.ClientConnectorError as request_error:
+            await self.session.close()
+            raise ConnectionError("Failed to connect to Central. Is the URL valid?") from request_error
+        except aiohttp.ClientResponseError as response_error:
+            await self.session.close()
+            if response_error.status == 401:
+                raise ConnectionError("ODK credentials are invalid, or may have changed. Please update them.") from response_error
+            raise response_error
 
 
 class OdkProject(OdkCentral):
     """Class to manipulate a project on an ODK Central server."""
 
     def __init__(
         self,
@@ -286,14 +295,43 @@
         self,
         projectId: int,
         datasetName: str,
         entityUuid: str,
     ) -> dict:
         """Get a single Entity by it's UUID for a project.
 
+        JSON response:
+        {
+        "uuid": "a54400b6-49fe-4787-9ab8-7e2f56ff52bc",
+        "createdAt": "2024-04-15T09:26:08.209Z",
+        "creatorId": 5,
+        "updatedAt": null,
+        "deletedAt": null,
+        "conflict": null,
+        "currentVersion": {
+            "createdAt": "2024-04-15T09:26:08.209Z",
+            "current": true,
+            "label": "test entity",
+            "creatorId": 5,
+            "userAgent": "Python/3.10 aiohttp/3.9.3",
+            "data": {
+                "osm_id": "1",
+                "geometry": "test"
+            },
+            "version": 1,
+            "baseVersion": null,
+            "dataReceived": {
+                "label": "test entity",
+                "osm_id": "1",
+                "geometry": "test"
+            },
+            "conflictingProperties": null
+        }
+        }
+
         Args:
             projectId (int): The ID of the project on ODK Central.
             datasetName (str): The name of a dataset, specific to a project.
             entityUuid (str): Unique itentifier of the entity in the dataset.
 
         Returns:
             dict: the JSON entity details, for a specific dataset.
@@ -412,19 +450,21 @@
         entity_data = []
 
         entity_tasks = [self.createEntity(projectId, datasetName, label, data) for label, data in labelDataDict.items()]
         log.info(f"Creating ({len(entity_tasks)}) entities for project " f"({projectId}) dataset ({datasetName})")
         entities = await gather(*entity_tasks, return_exceptions=True)
 
         for entity in entities:
-            if isinstance(entity, Exception):
-                log.error(f"Failed to upload entity: {entity}")
+            if not entity or isinstance(entity, Exception):
                 continue
             entity_data.append(entity)
 
+        if not entities:
+            log.warning(f"No entities were uploaded for ODK project ({projectId}) dataset name ({datasetName})")
+
         return entity_data
 
     async def updateEntity(
         self,
         projectId: int,
         datasetName: str,
         entityUuid: str,
```

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.8.2/osm_fieldwork/basemapper.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/convert.py` & `osm-fieldwork-0.8.2/osm_fieldwork/convert.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.8.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/data_models/__init__.py` & `osm-fieldwork-0.8.2/osm_fieldwork/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.8.2/osm_fieldwork/data_models/category.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.8.2/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.8.2/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.8.2/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.8.2/osm_fieldwork/filter_data.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/imagery.yaml` & `osm-fieldwork-0.8.2/osm_fieldwork/imagery.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.8.2/osm_fieldwork/json2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.8.2/osm_fieldwork/make_data_extract.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/models.yaml` & `osm-fieldwork-0.8.2/osm_fieldwork/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.8.2/osm_fieldwork/odk2csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/odk2geojson.py` & `osm-fieldwork-0.8.2/osm_fieldwork/odk2geojson.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/odk2osm.py` & `osm-fieldwork-0.8.2/osm_fieldwork/odk2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.8.2/osm_fieldwork/odk_client.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/odk_merge.py` & `osm-fieldwork-0.8.2/osm_fieldwork/odk_merge.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/osm2favorities.py` & `osm-fieldwork-0.8.2/osm_fieldwork/osm2favorities.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.8.2/osm_fieldwork/osmfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.8.2/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xforms.yaml` & `osm-fieldwork-0.8.2/osm_fieldwork/xforms.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/Makefile`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/entities/registration_form.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/entities/registration_form.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/entities/registration_form.xml` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/entities/registration_form.xml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/highways.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/highways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/test.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/test.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/thamel.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/thamel.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.8.2/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.8.2/osm_fieldwork/yamlfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.8.1/pyproject.toml` & `osm-fieldwork-0.8.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.8.1"
+version = "0.8.2"
 
 [project.urls]
 homepage = "https://github.com/hotosm/osm-fieldwork/wiki"
 documentation = "https://hotosm.github.io/osm-fieldwork"
 repository = "https://github.com/hotosm/osm-fieldwork"
 
 [project.scripts]
@@ -74,15 +74,15 @@
     "tests",
 ]
 pythonpath = "osm_fieldwork"
 asyncio_mode = "auto"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.1"
+version = "0.8.2"
 version_files = [
     "pyproject.toml:version",
     "osm_fieldwork/__version__.py",
     "Makefile:VERSION",
 ]
 update_changelog_on_bump = true
```

### Comparing `osm-fieldwork-0.8.1/PKG-INFO` & `osm-fieldwork-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.8.1
+Version: 0.8.2
 Summary: Processing field data from ODK to OpenStreetMap format.
 License: GPL-3.0-only
 Keywords: hot,odk,openstreetmap,fmtm
 Author-email: Rob Savoye <rob.savoye@hotosm.org>,Sam Woodcock <sam.woodcock@hotosm.org>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-fieldwork Version: 0.8.1 Summary: Processing
+Metadata-Version: 2.1 Name: osm-fieldwork Version: 0.8.2 Summary: Processing
 field data from ODK to OpenStreetMap format. License: GPL-3.0-only Keywords:
 hot,odk,openstreetmap,fmtm Author-email: Rob Savoye
 hotosm.org>,Sam Woodcock
 hotosm.org> Requires-Python: >=3.10 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```

