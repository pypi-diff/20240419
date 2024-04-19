# Comparing `tmp/dplib_py-0.7.1.tar.gz` & `tmp/dplib_py-0.7.2.tar.gz`

## Comparing `dplib_py-0.7.1.tar` & `dplib_py-0.7.2.tar`

### file list

```diff
@@ -1,266 +1,266 @@
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.1/mkdocs.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/codecov.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/issue_template.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/stale.yaml
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/workflows/general.yaml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/dialect-full.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/dialect-invalid.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/dialect.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/empty.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-custom-profile.json
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-full.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-invalid-dereferencing.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-invalid.json
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/profile.json
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource-full.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource-invalid-dereferencing.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource-invalid.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource.yaml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema-full.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema-invalid.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema-types.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/text.txt
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_check_package_custom_profile.yaml
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_dialect_profile.yaml
--rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_package_profile.yaml
--rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_resource_profile.yaml
--rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_schema_profile.yaml
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/ckan/package.json
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/datacite/package.json
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/dcat/package.xml
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/github/package.json
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/zenodo/package.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/changelog.md
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/contributing.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/converting-metadata.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/index.md
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/installation.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/validating-metadata.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/working-with-models.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/.theme/.keep
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/dialect.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/package.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/resource.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/schema.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon-color.png
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon-shaddow.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon.ico
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon.png
--rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/logo-dark.svg
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/logo-light.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/dialect.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/package.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/resource.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/schema.md
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/ckan.md
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/cli.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/datacite.md
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/dcat.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/github.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/pandas.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/polars.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/sql.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/zenodo.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/conftest.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/py.typed
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/settings.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_dialect_check.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_package_check.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_resource_check.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_schema_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/dialect/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/dialect/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/metadata/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/metadata/check.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/metadata/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/package/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/package/check.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/package/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/resource/__init__.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/resource/check.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/resource/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/schema/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/schema/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/errors/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/errors/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/data.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/file.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/path.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/profile.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/resource.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/__init__.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/contributor.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/license.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/source.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/dialect.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/__spec__/__init__.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/__spec__/test_dialect.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/field.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/types.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/__spec__/test_field.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/base.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/collection.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/json.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/string.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/value.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/any.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/array.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/base.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/boolean.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/date.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/datetime.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/duration.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/geojson.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/geopoint.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/integer.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/list.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/number.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/object.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/string.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/time.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/year.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/yearmonth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/__init__.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/__spec__/__init__.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/__spec__/test_package.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/hash.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/__spec__/__init__.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/__spec__/test_resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/datatypes/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/datatypes/table.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/foreignKey.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/schema.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/__spec__/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/organization.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/package.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/resource.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/__main__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/program.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/main.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/__spec__/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/__spec__/test_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/dialect/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/dialect/check.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/dialect/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/check.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/convert.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/check.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/convert.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/main.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/schema/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/schema/check.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/schema/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/helpers/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/helpers/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/convert.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/path.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/contributor.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/description.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/identifier.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/package.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/rights.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/subject.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/title.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/dumpers.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/helpers.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/loaders.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/namespaces.py
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/package.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/resource.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/license.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/owner.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/package.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/field.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/__spec__/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/field.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/__spec__/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/__init__.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/field.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/schema.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/creator.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/files.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/metadata.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/package.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/pid.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/resource.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/__spec__/test_package.py
--rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/datapackage.json
--rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/dataresource.json
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/tabledialect.json
--rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/tableschema.json
--rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/datapackage.json
--rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/dataresource.json
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/tabledialect.json
--rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/tableschema.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/__init__.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/__spec__/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/__spec__/test_model.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.1/LICENSE.md
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.1/README.md
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 dplib_py-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 dplib_py-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.2/mkdocs.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.2/.github/codecov.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.2/.github/issue_template.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.2/.github/stale.yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.2/.github/workflows/general.yaml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/dialect-full.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/dialect-invalid.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/dialect.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/empty.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/package-custom-profile.json
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/package-full.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/package-invalid-dereferencing.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/package-invalid.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/profile.json
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/resource-full.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/resource-invalid-dereferencing.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/resource-invalid.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/resource.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/resource.yaml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/schema-full.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/schema-invalid.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/schema-types.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/schema.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/text.txt
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/cassettes/test_check_package_custom_profile.yaml
+-rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/cassettes/test_dialect_profile.yaml
+-rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/cassettes/test_package_profile.yaml
+-rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/cassettes/test_resource_profile.yaml
+-rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/cassettes/test_schema_profile.yaml
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/plugins/ckan/package.json
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/plugins/datacite/package.json
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/plugins/dcat/package.xml
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/plugins/github/package.json
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.2/data/plugins/zenodo/package.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/changelog.md
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/contributing.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/converting-metadata.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/index.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/installation.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/validating-metadata.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/working-with-models.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/.theme/.keep
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/actions/dialect.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/actions/package.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/actions/resource.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/actions/schema.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/assets/favicon-color.png
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/assets/favicon-shaddow.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/assets/favicon.ico
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/assets/favicon.png
+-rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/assets/logo-dark.svg
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/assets/logo-light.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/models/dialect.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/models/package.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/models/resource.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/models/schema.md
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/ckan.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/cli.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/datacite.md
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/dcat.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/github.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/pandas.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/polars.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/sql.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.2/docs/plugins/zenodo.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/conftest.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/py.typed
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/settings.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/__spec__/test_dialect_check.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/__spec__/test_package_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/__spec__/test_resource_check.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/__spec__/test_schema_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/dialect/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/dialect/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/metadata/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/metadata/check.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/metadata/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/package/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/package/check.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/package/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/resource/__init__.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/resource/check.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/resource/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/schema/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/actions/schema/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/errors/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/errors/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/helpers/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/helpers/data.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/helpers/file.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/helpers/path.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/helpers/profile.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/helpers/resource.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/__init__.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/contributor.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/license.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/source.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/dialect/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/dialect/dialect.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/dialect/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/dialect/__spec__/__init__.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/dialect/__spec__/test_dialect.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/field.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/types.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/__spec__/test_field.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/constraints/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/constraints/base.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/constraints/collection.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/constraints/json.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/constraints/string.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/constraints/value.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/any.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/array.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/base.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/boolean.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/date.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/datetime.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/duration.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/geojson.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/geopoint.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/integer.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/list.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/number.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/object.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/string.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/time.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/year.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/field/datatypes/yearmonth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/package/__init__.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/package/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/package/__spec__/__init__.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/package/__spec__/test_package.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/hash.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/__spec__/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/__spec__/test_resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/datatypes/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/resource/datatypes/table.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/schema/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/schema/foreignKey.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/schema/schema.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/schema/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/schema/__spec__/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/models/schema/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/organization.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/package.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/resource.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/ckan/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/__main__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/program.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/main.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/__spec__/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/__spec__/test_version.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/dialect/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/dialect/check.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/dialect/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/package/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/package/check.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/package/convert.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/package/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/resource/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/resource/check.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/resource/convert.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/resource/main.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/schema/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/schema/check.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/commands/schema/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/helpers/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/options/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/options/convert.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/options/path.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/cli/options/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/contributor.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/description.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/identifier.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/package.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/rights.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/subject.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/title.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/datacite/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/dumpers.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/helpers.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/loaders.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/namespaces.py
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/package.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/resource.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/dcat/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/license.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/owner.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/package.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/github/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/pandas/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/pandas/models/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/pandas/models/field.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/pandas/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/pandas/models/__spec__/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/polars/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/polars/models/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/polars/models/field.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/polars/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/polars/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/polars/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/models/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/models/field.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/models/schema.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/models/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/sql/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/creator.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/files.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/metadata.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/package.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/pid.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/resource.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/plugins/zenodo/models/__spec__/test_package.py
+-rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/1.0/datapackage.json
+-rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/1.0/dataresource.json
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/1.0/tabledialect.json
+-rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/1.0/tableschema.json
+-rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/2.0/datapackage.json
+-rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/2.0/dataresource.json
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/2.0/tabledialect.json
+-rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/profiles/2.0/tableschema.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/system/__init__.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/system/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/system/__spec__/__init__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.7.2/dplib/system/__spec__/test_model.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.2/README.md
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 dplib_py-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 dplib_py-0.7.2/PKG-INFO
```

### Comparing `dplib_py-0.7.1/mkdocs.yaml` & `dplib_py-0.7.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/.github/stale.yaml` & `dplib_py-0.7.2/.github/stale.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/.github/workflows/general.yaml` & `dplib_py-0.7.2/.github/workflows/general.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/package-full.json` & `dplib_py-0.7.2/data/package-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/schema-full.json` & `dplib_py-0.7.2/data/schema-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/schema-types.json` & `dplib_py-0.7.2/data/schema-types.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/cassettes/test_check_package_custom_profile.yaml` & `dplib_py-0.7.2/data/cassettes/test_check_package_custom_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/cassettes/test_dialect_profile.yaml` & `dplib_py-0.7.2/data/cassettes/test_dialect_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/cassettes/test_package_profile.yaml` & `dplib_py-0.7.2/data/cassettes/test_package_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/cassettes/test_resource_profile.yaml` & `dplib_py-0.7.2/data/cassettes/test_resource_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/cassettes/test_schema_profile.yaml` & `dplib_py-0.7.2/data/cassettes/test_schema_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/plugins/ckan/package.json` & `dplib_py-0.7.2/data/plugins/ckan/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/plugins/datacite/package.json` & `dplib_py-0.7.2/data/plugins/datacite/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/plugins/dcat/package.xml` & `dplib_py-0.7.2/data/plugins/dcat/package.xml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/plugins/github/package.json` & `dplib_py-0.7.2/data/plugins/github/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/data/plugins/zenodo/package.json` & `dplib_py-0.7.2/data/plugins/zenodo/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/contributing.md` & `dplib_py-0.7.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/converting-metadata.md` & `dplib_py-0.7.2/docs/converting-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/index.md` & `dplib_py-0.7.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/validating-metadata.md` & `dplib_py-0.7.2/docs/validating-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/working-with-models.md` & `dplib_py-0.7.2/docs/working-with-models.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/assets/favicon-shaddow.png` & `dplib_py-0.7.2/docs/assets/favicon-shaddow.png`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/assets/favicon.ico` & `dplib_py-0.7.2/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/assets/logo-dark.svg` & `dplib_py-0.7.2/docs/assets/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/assets/logo-light.svg` & `dplib_py-0.7.2/docs/assets/logo-light.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/models/package.md` & `dplib_py-0.7.2/docs/models/package.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/models/resource.md` & `dplib_py-0.7.2/docs/models/resource.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/models/schema.md` & `dplib_py-0.7.2/docs/models/schema.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/ckan.md` & `dplib_py-0.7.2/docs/plugins/ckan.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/cli.md` & `dplib_py-0.7.2/docs/plugins/cli.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/datacite.md` & `dplib_py-0.7.2/docs/plugins/datacite.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/dcat.md` & `dplib_py-0.7.2/docs/plugins/dcat.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/github.md` & `dplib_py-0.7.2/docs/plugins/github.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/pandas.md` & `dplib_py-0.7.2/docs/plugins/pandas.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/polars.md` & `dplib_py-0.7.2/docs/plugins/polars.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/sql.md` & `dplib_py-0.7.2/docs/plugins/sql.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/docs/plugins/zenodo.md` & `dplib_py-0.7.2/docs/plugins/zenodo.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/settings.py` & `dplib_py-0.7.2/dplib/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Version
 
-VERSION = "0.7.1"
+VERSION = "0.7.2"
 
 # Profiles
 
 PROFILE_BASEURL = "https://datapackage.org/profiles"
 PROFILE_BASEDIR = os.path.join(os.path.dirname(__file__), "profiles")
 
 PROFILE_DEFAULT = "1.0"
```

### Comparing `dplib_py-0.7.1/dplib/actions/__spec__/test_dialect_check.py` & `dplib_py-0.7.2/dplib/actions/__spec__/test_dialect_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/__spec__/test_package_check.py` & `dplib_py-0.7.2/dplib/actions/__spec__/test_package_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/__spec__/test_resource_check.py` & `dplib_py-0.7.2/dplib/actions/__spec__/test_resource_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/__spec__/test_schema_check.py` & `dplib_py-0.7.2/dplib/actions/__spec__/test_schema_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/dialect/check.py` & `dplib_py-0.7.2/dplib/actions/dialect/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/metadata/check.py` & `dplib_py-0.7.2/dplib/actions/metadata/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/metadata/convert.py` & `dplib_py-0.7.2/dplib/actions/metadata/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/package/check.py` & `dplib_py-0.7.2/dplib/actions/package/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/package/convert.py` & `dplib_py-0.7.2/dplib/actions/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/resource/check.py` & `dplib_py-0.7.2/dplib/actions/resource/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/resource/convert.py` & `dplib_py-0.7.2/dplib/actions/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/actions/schema/check.py` & `dplib_py-0.7.2/dplib/actions/schema/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/errors/metadata.py` & `dplib_py-0.7.2/dplib/errors/metadata.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/helpers/data.py` & `dplib_py-0.7.2/dplib/helpers/data.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/helpers/file.py` & `dplib_py-0.7.2/dplib/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/helpers/path.py` & `dplib_py-0.7.2/dplib/helpers/path.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/helpers/profile.py` & `dplib_py-0.7.2/dplib/helpers/profile.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/contributor.py` & `dplib_py-0.7.2/dplib/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/dialect/dialect.py` & `dplib_py-0.7.2/dplib/models/dialect/dialect.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/dialect/__spec__/test_dialect.py` & `dplib_py-0.7.2/dplib/models/dialect/__spec__/test_dialect.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/types.py` & `dplib_py-0.7.2/dplib/models/field/types.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/__init__.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/base.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/boolean.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/boolean.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/geojson.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/geojson.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/geopoint.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/geopoint.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/integer.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/integer.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/list.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/list.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/number.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/number.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/field/datatypes/string.py` & `dplib_py-0.7.2/dplib/models/field/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/package/package.py` & `dplib_py-0.7.2/dplib/models/package/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/package/__spec__/test_package.py` & `dplib_py-0.7.2/dplib/models/package/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/resource/hash.py` & `dplib_py-0.7.2/dplib/models/resource/hash.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/resource/resource.py` & `dplib_py-0.7.2/dplib/models/resource/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/resource/__spec__/test_resource.py` & `dplib_py-0.7.2/dplib/models/resource/__spec__/test_resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/schema/foreignKey.py` & `dplib_py-0.7.2/dplib/models/schema/foreignKey.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/schema/schema.py` & `dplib_py-0.7.2/dplib/models/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/models/schema/__spec__/test_schema.py` & `dplib_py-0.7.2/dplib/models/schema/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/ckan/models/package.py` & `dplib_py-0.7.2/dplib/plugins/ckan/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/ckan/models/resource.py` & `dplib_py-0.7.2/dplib/plugins/ckan/models/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
+import os
 from typing import Optional
 
 from dplib.helpers.resource import slugify_name
 from dplib.models import Resource
 from dplib.system import Model
 
 
 class CkanResource(Model):
     """CKAN Resource model"""
 
+    url: str
     name: str
     created: Optional[str] = None
     description: Optional[str] = None
     format: Optional[str] = None  # NOTE: uppercased
     hash: Optional[str] = None
     id: Optional[str] = None
     last_modified: Optional[str] = None
@@ -26,15 +28,15 @@
     def to_dp(self) -> Resource:
         """Convert to Data Package resource
 
         Returns:
            Data Resource
         """
         # Path/Name
-        resource = Resource(path=self.name, name=slugify_name(self.name))
+        resource = Resource(path=self.url, name=slugify_name(self.name))
 
         # Description
         if self.description:
             resource.description = self.description
 
         # Format
         if self.format:
@@ -63,16 +65,16 @@
 
         Returns:
             CKAN Resource
         """
         if not resource.path or not isinstance(resource.path, str):
             return
 
-        # Path
-        ckan = CkanResource(name=resource.path)
+        # Path/Name
+        ckan = CkanResource(url=resource.path, name=os.path.basename(resource.path))
 
         # Description
         if resource.description:
             ckan.description = resource.description
 
         # Format
         if resource.format:
```

### Comparing `dplib_py-0.7.1/dplib/plugins/ckan/models/__spec__/test_package.py` & `dplib_py-0.7.2/dplib/plugins/ckan/models/__spec__/test_package.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,18 @@
     assert package.name == "sample-dataset-1"
     assert package.title == "Sample Dataset"
     assert package.version == "1.0"
     assert package.licenses[0].name == "cc-by"
     assert len(package.resources) == 9
     assert len(package.keywords) == 8
     assert len(package.contributors) == 2
-    assert package.resources[0].path == "sample-linked.csv"
+    assert (
+        package.resources[0].path
+        == "https://raw.githubusercontent.com/datopian/CKAN_Demo_Datasets/main/resources/org1_sample.csv"
+    )
     assert package.keywords[0] == "csv"
     assert package.contributors[0].title == "Test Author"
     assert package.contributors[0].roles == ["author"]
     assert package.custom["ckan:id"] == "c322307a-b871-44fe-a602-32ee8437ff04"
 
 
 def test_ckan_package_from_dp():
@@ -55,14 +58,14 @@
     )
     assert package.name == "sample-dataset-1"
     assert package.title == "Sample Dataset"
     assert package.version == "1.0"
     assert package.license_id == "cc-by"
     assert len(package.resources) == 9
     assert len(package.tags) == 8
-    assert package.resources[0].name == "sample-linked.csv"
+    assert package.resources[0].name == "org1_sample.csv"
     assert package.tags[0].name == "csv"
 
 
 def test_ckan_package_from_dp_inline_resource():
     package = CkanPackage.from_dp(Package(resources=[Resource(data=[])]))
     assert package.to_dict() == {}
```

### Comparing `dplib_py-0.7.1/dplib/plugins/cli/program.py` & `dplib_py-0.7.2/dplib/plugins/cli/program.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/cli/commands/main.py` & `dplib_py-0.7.2/dplib/plugins/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/cli/commands/package/convert.py` & `dplib_py-0.7.2/dplib/plugins/cli/commands/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/cli/commands/resource/convert.py` & `dplib_py-0.7.2/dplib/plugins/cli/commands/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/cli/helpers/check.py` & `dplib_py-0.7.2/dplib/plugins/cli/helpers/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/datacite/models/contributor.py` & `dplib_py-0.7.2/dplib/plugins/datacite/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/datacite/models/package.py` & `dplib_py-0.7.2/dplib/plugins/datacite/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/datacite/models/__spec__/test_package.py` & `dplib_py-0.7.2/dplib/plugins/datacite/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/dcat/models/helpers.py` & `dplib_py-0.7.2/dplib/plugins/dcat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/dcat/models/loaders.py` & `dplib_py-0.7.2/dplib/plugins/dcat/models/loaders.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/dcat/models/namespaces.py` & `dplib_py-0.7.2/dplib/plugins/dcat/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/dcat/models/package.py` & `dplib_py-0.7.2/dplib/plugins/dcat/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/dcat/models/resource.py` & `dplib_py-0.7.2/dplib/plugins/dcat/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/dcat/models/__spec__/test_package.py` & `dplib_py-0.7.2/dplib/plugins/dcat/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/github/models/package.py` & `dplib_py-0.7.2/dplib/plugins/github/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/github/models/resource.py` & `dplib_py-0.7.2/dplib/plugins/github/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/github/models/__spec__/test_package.py` & `dplib_py-0.7.2/dplib/plugins/github/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/pandas/models/field.py` & `dplib_py-0.7.2/dplib/plugins/pandas/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/pandas/models/schema.py` & `dplib_py-0.7.2/dplib/plugins/pandas/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/polars/models/field.py` & `dplib_py-0.7.2/dplib/plugins/polars/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/polars/models/schema.py` & `dplib_py-0.7.2/dplib/plugins/polars/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/polars/models/__spec__/test_schema.py` & `dplib_py-0.7.2/dplib/plugins/polars/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/sql/models/field.py` & `dplib_py-0.7.2/dplib/plugins/sql/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/sql/models/schema.py` & `dplib_py-0.7.2/dplib/plugins/sql/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/sql/models/__spec__/test_schema.py` & `dplib_py-0.7.2/dplib/plugins/sql/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/zenodo/models/creator.py` & `dplib_py-0.7.2/dplib/plugins/zenodo/models/creator.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/zenodo/models/package.py` & `dplib_py-0.7.2/dplib/plugins/zenodo/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/zenodo/models/resource.py` & `dplib_py-0.7.2/dplib/plugins/zenodo/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/plugins/zenodo/models/__spec__/test_package.py` & `dplib_py-0.7.2/dplib/plugins/zenodo/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/1.0/datapackage.json` & `dplib_py-0.7.2/dplib/profiles/1.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/1.0/dataresource.json` & `dplib_py-0.7.2/dplib/profiles/1.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/1.0/tabledialect.json` & `dplib_py-0.7.2/dplib/profiles/1.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/1.0/tableschema.json` & `dplib_py-0.7.2/dplib/profiles/1.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/2.0/datapackage.json` & `dplib_py-0.7.2/dplib/profiles/2.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/2.0/dataresource.json` & `dplib_py-0.7.2/dplib/profiles/2.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/2.0/tabledialect.json` & `dplib_py-0.7.2/dplib/profiles/2.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/profiles/2.0/tableschema.json` & `dplib_py-0.7.2/dplib/profiles/2.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/system/model.py` & `dplib_py-0.7.2/dplib/system/model.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/dplib/system/__spec__/test_model.py` & `dplib_py-0.7.2/dplib/system/__spec__/test_model.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/.gitignore` & `dplib_py-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/LICENSE.md` & `dplib_py-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/README.md` & `dplib_py-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/pyproject.toml` & `dplib_py-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.1/PKG-INFO` & `dplib_py-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dplib-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python implementation of the Data Package standard
 Project-URL: homepage, https://github.com/frictionlessdata/dplib-py
 Author-email: Open Knowledge Foundation <info@okfn.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: data package,data validation,json schema,json table schema,open data,tabular data package
 Classifier: Development Status :: 4 - Beta
```

