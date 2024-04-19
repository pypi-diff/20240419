# Comparing `tmp/dplib_py-0.7.0.tar.gz` & `tmp/dplib_py-0.7.1.tar.gz`

## Comparing `dplib_py-0.7.0.tar` & `dplib_py-0.7.1.tar`

### file list

```diff
@@ -1,267 +1,266 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.env.example
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.0/mkdocs.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/codecov.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/issue_template.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/stale.yaml
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/workflows/general.yaml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/dialect-full.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/dialect-invalid.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/dialect.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/empty.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-custom-profile.json
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-full.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-invalid-dereferencing.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-invalid.json
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/profile.json
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource-full.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource-invalid-dereferencing.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource-invalid.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource.yaml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema-full.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema-invalid.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema-types.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/text.txt
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_check_package_custom_profile.yaml
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_dialect_profile.yaml
--rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_package_profile.yaml
--rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_resource_profile.yaml
--rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_schema_profile.yaml
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/ckan/package.json
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/datacite/package.json
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/dcat/package.xml
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/github/package.json
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/zenodo/package.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/changelog.md
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/contributing.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/converting-metadata.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/index.md
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/installation.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/validating-metadata.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/working-with-models.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/.theme/.keep
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/dialect.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/package.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/resource.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/schema.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon-color.png
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon-shaddow.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon.ico
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon.png
--rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/logo-dark.svg
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/logo-light.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/dialect.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/package.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/resource.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/schema.md
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/ckan.md
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/cli.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/datacite.md
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/dcat.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/github.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/pandas.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/polars.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/sql.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/zenodo.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/conftest.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/py.typed
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/settings.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_dialect_check.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_package_check.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_resource_check.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_schema_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/dialect/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/dialect/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/metadata/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/metadata/check.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/metadata/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/package/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/package/check.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/package/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/resource/__init__.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/resource/check.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/resource/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/schema/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/schema/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/errors/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/errors/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/data.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/file.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/path.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/profile.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/resource.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/__init__.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/contributor.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/license.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/source.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/dialect.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/__spec__/__init__.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/__spec__/test_dialect.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/field.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/types.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/__spec__/test_field.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/base.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/collection.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/json.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/string.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/value.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/any.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/array.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/base.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/boolean.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/date.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/datetime.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/duration.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/geojson.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/geopoint.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/integer.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/list.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/number.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/object.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/string.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/time.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/year.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/yearmonth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/__init__.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/__spec__/__init__.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/__spec__/test_package.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/hash.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/__spec__/__init__.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/__spec__/test_resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/datatypes/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/datatypes/table.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/foreignKey.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/schema.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/__spec__/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/organization.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/package.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/resource.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/__main__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/program.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/main.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/__spec__/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/__spec__/test_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/dialect/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/dialect/check.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/dialect/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/check.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/convert.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/check.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/convert.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/main.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/schema/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/schema/check.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/schema/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/helpers/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/helpers/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/convert.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/path.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/contributor.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/description.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/identifier.py
--rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/package.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/rights.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/subject.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/title.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/dumpers.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/helpers.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/loaders.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/namespaces.py
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/package.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/resource.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/license.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/owner.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/package.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/__init__.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/field.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/__spec__/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/field.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/__spec__/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/__init__.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/field.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/schema.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/creator.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/files.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/metadata.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/package.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/pid.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/resource.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/__spec__/test_package.py
--rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/datapackage.json
--rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/dataresource.json
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/tabledialect.json
--rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/tableschema.json
--rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/datapackage.json
--rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/dataresource.json
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/tabledialect.json
--rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/tableschema.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/__init__.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/__spec__/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/__spec__/test_model.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.0/README.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 dplib_py-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 dplib_py-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.1/mkdocs.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/codecov.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/issue_template.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/stale.yaml
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.github/workflows/general.yaml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/dialect-full.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/dialect-invalid.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/dialect.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/empty.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-custom-profile.json
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-full.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-invalid-dereferencing.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package-invalid.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/profile.json
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource-full.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource-invalid-dereferencing.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource-invalid.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/resource.yaml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema-full.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema-invalid.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema-types.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/schema.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/text.txt
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_check_package_custom_profile.yaml
+-rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_dialect_profile.yaml
+-rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_package_profile.yaml
+-rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_resource_profile.yaml
+-rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/cassettes/test_schema_profile.yaml
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/ckan/package.json
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/datacite/package.json
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/dcat/package.xml
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/github/package.json
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.1/data/plugins/zenodo/package.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/changelog.md
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/contributing.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/converting-metadata.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/index.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/installation.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/validating-metadata.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/working-with-models.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/.theme/.keep
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/dialect.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/package.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/resource.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/actions/schema.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon-color.png
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon-shaddow.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon.ico
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/favicon.png
+-rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/logo-dark.svg
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/assets/logo-light.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/dialect.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/package.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/resource.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/models/schema.md
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/ckan.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/cli.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/datacite.md
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/dcat.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/github.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/pandas.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/polars.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/sql.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.1/docs/plugins/zenodo.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/conftest.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/py.typed
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/settings.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_dialect_check.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_package_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_resource_check.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/__spec__/test_schema_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/dialect/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/dialect/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/metadata/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/metadata/check.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/metadata/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/package/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/package/check.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/package/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/resource/__init__.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/resource/check.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/resource/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/schema/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/actions/schema/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/errors/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/errors/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/data.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/file.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/path.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/profile.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/helpers/resource.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/__init__.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/contributor.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/license.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/source.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/dialect.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/__spec__/__init__.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/dialect/__spec__/test_dialect.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/field.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/types.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/__spec__/test_field.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/base.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/collection.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/json.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/string.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/constraints/value.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/any.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/array.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/base.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/boolean.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/date.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/datetime.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/duration.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/geojson.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/geopoint.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/integer.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/list.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/number.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/object.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/string.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/time.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/year.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/field/datatypes/yearmonth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/__init__.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/__spec__/__init__.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/package/__spec__/test_package.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/hash.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/__spec__/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/__spec__/test_resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/datatypes/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/resource/datatypes/table.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/foreignKey.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/schema.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/__spec__/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/models/schema/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/organization.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/package.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/resource.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/ckan/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/__main__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/program.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/main.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/__spec__/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/__spec__/test_version.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/dialect/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/dialect/check.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/dialect/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/check.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/convert.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/package/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/check.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/convert.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/resource/main.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/schema/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/schema/check.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/commands/schema/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/helpers/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/convert.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/path.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/cli/options/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/contributor.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/description.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/identifier.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/package.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/rights.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/subject.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/title.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/datacite/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/dumpers.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/helpers.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/loaders.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/namespaces.py
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/package.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/resource.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/dcat/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/license.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/owner.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/package.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/github/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/field.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/pandas/models/__spec__/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/field.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/polars/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/field.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/schema.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/sql/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/creator.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/files.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/metadata.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/package.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/pid.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/resource.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/plugins/zenodo/models/__spec__/test_package.py
+-rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/datapackage.json
+-rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/dataresource.json
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/tabledialect.json
+-rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/1.0/tableschema.json
+-rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/datapackage.json
+-rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/dataresource.json
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/tabledialect.json
+-rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/profiles/2.0/tableschema.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/__init__.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/__spec__/__init__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.7.1/dplib/system/__spec__/test_model.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 dplib_py-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.1/README.md
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 dplib_py-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 dplib_py-0.7.1/PKG-INFO
```

### Comparing `dplib_py-0.7.0/mkdocs.yaml` & `dplib_py-0.7.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/.github/stale.yaml` & `dplib_py-0.7.1/.github/stale.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/.github/workflows/general.yaml` & `dplib_py-0.7.1/.github/workflows/general.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,14 @@
         uses: actions/checkout@v2
       - name: Install Python
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Prepare environment
         run: pip3 install hatch
-      - name: Prepare variables
-        run: cp .env.example .env
       - name: Test software
         run: hatch run +py=${{ matrix.py || matrix.python-version }} ci:test
       - name: Report coverage
         uses: codecov/codecov-action@v2
 
   # Test (MacOS)
 
@@ -47,16 +45,14 @@
         uses: actions/checkout@v2
       - name: Install Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.10"
       - name: Prepare environment
         run: pip3 install hatch
-      - name: Prepare variables
-        run: cp .env.example .env
       - name: Test software
         # https://stackoverflow.com/questions/9678408/cant-install-psycopg2-with-pip-in-virtualenv-on-mac-os-x-10-7
         run: LDFLAGS=`echo $(pg_config --ldflags)` hatch run +py=3.10 ci:test
 
   # Test (Windows)
 
   test-windows:
@@ -67,16 +63,14 @@
         uses: actions/checkout@v2
       - name: Install Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.10"
       - name: Prepare environment
         run: pip3 install hatch
-      - name: Prepare variables
-        run: cp .env.example .env
       - name: Test software
         run: hatch run +py=3.10 ci:test
 
   # Deploy
 
   deploy:
     if: github.event_name == 'push'
```

### Comparing `dplib_py-0.7.0/data/package-full.json` & `dplib_py-0.7.1/data/package-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/schema-full.json` & `dplib_py-0.7.1/data/schema-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/schema-types.json` & `dplib_py-0.7.1/data/schema-types.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/cassettes/test_check_package_custom_profile.yaml` & `dplib_py-0.7.1/data/cassettes/test_check_package_custom_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/cassettes/test_dialect_profile.yaml` & `dplib_py-0.7.1/data/cassettes/test_dialect_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/cassettes/test_package_profile.yaml` & `dplib_py-0.7.1/data/cassettes/test_package_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/cassettes/test_resource_profile.yaml` & `dplib_py-0.7.1/data/cassettes/test_resource_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/cassettes/test_schema_profile.yaml` & `dplib_py-0.7.1/data/cassettes/test_schema_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/plugins/ckan/package.json` & `dplib_py-0.7.1/data/plugins/ckan/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/plugins/datacite/package.json` & `dplib_py-0.7.1/data/plugins/datacite/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/plugins/dcat/package.xml` & `dplib_py-0.7.1/data/plugins/dcat/package.xml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/plugins/github/package.json` & `dplib_py-0.7.1/data/plugins/github/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/data/plugins/zenodo/package.json` & `dplib_py-0.7.1/data/plugins/zenodo/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/contributing.md` & `dplib_py-0.7.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/converting-metadata.md` & `dplib_py-0.7.1/docs/converting-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/index.md` & `dplib_py-0.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/validating-metadata.md` & `dplib_py-0.7.1/docs/validating-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/working-with-models.md` & `dplib_py-0.7.1/docs/working-with-models.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/assets/favicon-shaddow.png` & `dplib_py-0.7.1/docs/assets/favicon-shaddow.png`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/assets/favicon.ico` & `dplib_py-0.7.1/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/assets/logo-dark.svg` & `dplib_py-0.7.1/docs/assets/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/assets/logo-light.svg` & `dplib_py-0.7.1/docs/assets/logo-light.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/models/package.md` & `dplib_py-0.7.1/docs/models/package.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/models/resource.md` & `dplib_py-0.7.1/docs/models/resource.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/models/schema.md` & `dplib_py-0.7.1/docs/models/schema.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/ckan.md` & `dplib_py-0.7.1/docs/plugins/ckan.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/cli.md` & `dplib_py-0.7.1/docs/plugins/cli.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/datacite.md` & `dplib_py-0.7.1/docs/plugins/datacite.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/dcat.md` & `dplib_py-0.7.1/docs/plugins/dcat.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/github.md` & `dplib_py-0.7.1/docs/plugins/github.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/pandas.md` & `dplib_py-0.7.1/docs/plugins/pandas.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/polars.md` & `dplib_py-0.7.1/docs/plugins/polars.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/sql.md` & `dplib_py-0.7.1/docs/plugins/sql.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/docs/plugins/zenodo.md` & `dplib_py-0.7.1/docs/plugins/zenodo.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/settings.py` & `dplib_py-0.7.1/dplib/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Version
 
-VERSION = "0.7.0"
+VERSION = "0.7.1"
 
 # Profiles
 
 PROFILE_BASEURL = "https://datapackage.org/profiles"
 PROFILE_BASEDIR = os.path.join(os.path.dirname(__file__), "profiles")
 
 PROFILE_DEFAULT = "1.0"
```

### Comparing `dplib_py-0.7.0/dplib/actions/__spec__/test_dialect_check.py` & `dplib_py-0.7.1/dplib/actions/__spec__/test_dialect_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/__spec__/test_package_check.py` & `dplib_py-0.7.1/dplib/actions/__spec__/test_package_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/__spec__/test_resource_check.py` & `dplib_py-0.7.1/dplib/actions/__spec__/test_resource_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/__spec__/test_schema_check.py` & `dplib_py-0.7.1/dplib/actions/__spec__/test_schema_check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/dialect/check.py` & `dplib_py-0.7.1/dplib/actions/dialect/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ... import types
 from ...errors.metadata import MetadataError
 from ...models import Dialect
 from ..metadata.check import check_metadata
 
 
-def check_dialect(dialect: Union[str, types.IData, Dialect]) -> List[MetadataError]:
+def check_dialect(dialect: Union[str, types.IDict, Dialect]) -> List[MetadataError]:
     """Check the validity of a Table Dialect descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         dialect: The Table Dialect descriptor
```

### Comparing `dplib_py-0.7.0/dplib/actions/metadata/check.py` & `dplib_py-0.7.1/dplib/actions/metadata/check.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ... import settings, types
 from ...errors.metadata import MetadataError
 from ...helpers.data import read_data
 from ...helpers.profile import check_profile
 
 
 def check_metadata(
-    metadata: Union[str, types.IData], *, type: types.IMetadataType
+    metadata: Union[str, types.IDict], *, type: types.IMetadataType
 ) -> List[MetadataError]:
     if isinstance(metadata, str):
         metadata = read_data(metadata)
 
     # Get default profile
     if type == "dialect":
         default_profile = settings.PROFILE_DEFAULT_DIALECT
```

### Comparing `dplib_py-0.7.0/dplib/actions/metadata/convert.py` & `dplib_py-0.7.1/dplib/actions/metadata/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/package/check.py` & `dplib_py-0.7.1/dplib/actions/package/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ...errors.metadata import MetadataError
 from ...helpers.data import read_data
 from ...helpers.path import infer_basepath
 from ...models import Package
 from ..metadata.check import check_metadata
 
 
-def check_package(package: Union[str, types.IData, Package]) -> List[MetadataError]:
+def check_package(package: Union[str, types.IDict, Package]) -> List[MetadataError]:
     """Check the validity of a Data Package descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         package: The Data Package descriptor
```

### Comparing `dplib_py-0.7.0/dplib/actions/package/convert.py` & `dplib_py-0.7.1/dplib/actions/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/resource/check.py` & `dplib_py-0.7.1/dplib/actions/resource/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ...errors.metadata import MetadataError
 from ...helpers.data import read_data
 from ...helpers.path import infer_basepath
 from ...models import Resource
 from ..metadata.check import check_metadata
 
 
-def check_resource(resource: Union[str, types.IData, Resource]) -> List[MetadataError]:
+def check_resource(resource: Union[str, types.IDict, Resource]) -> List[MetadataError]:
     """Check the validity of a Data Resource descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         resource: The Data Resource descriptor
```

### Comparing `dplib_py-0.7.0/dplib/actions/resource/convert.py` & `dplib_py-0.7.1/dplib/actions/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/actions/schema/check.py` & `dplib_py-0.7.1/dplib/actions/schema/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ... import types
 from ...errors.metadata import MetadataError
 from ...models import Schema
 from ..metadata.check import check_metadata
 
 
-def check_schema(schema: Union[str, types.IData, Schema]) -> List[MetadataError]:
+def check_schema(schema: Union[str, types.IDict, Schema]) -> List[MetadataError]:
     """Check the validity of a Table Schema descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         schema: The Table Schema descriptor
```

### Comparing `dplib_py-0.7.0/dplib/errors/metadata.py` & `dplib_py-0.7.1/dplib/errors/metadata.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/helpers/data.py` & `dplib_py-0.7.1/dplib/helpers/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,54 +8,54 @@
 from ..error import Error
 from .file import read_file, write_file
 from .path import infer_format
 
 
 def read_data(
     path: str, *, format: Optional[str] = None, basepath: Optional[str] = None
-) -> types.IData:
+) -> types.IDict:
     if not format:
         format = infer_format(path, raise_missing=True)
     text = read_file(path, basepath=basepath)
     data = load_data(text, format=format)
     return data
 
 
-def write_data(path: str, data: types.IData, *, format: Optional[str] = None):
+def write_data(path: str, data: types.IDict, *, format: Optional[str] = None):
     if not format:
         format = infer_format(path, raise_missing=True)
     text = dump_data(data, format=format)
     write_file(path, text)
 
 
-def load_data(text: str, *, format: str) -> types.IData:
+def load_data(text: str, *, format: str) -> types.IDict:
     try:
         if format == "json":
             return json.loads(text)
         elif format == "yaml":
             yaml = import_module("yaml")
             return yaml.safe_load(text)
     except Exception:
         raise Error(f'Cannot load "{format}" data from text: {text}')
     raise Error(f"Cannot load data from text with format: {format}")
 
 
-def dump_data(data: types.IData, *, format: str) -> str:
+def dump_data(data: types.IDict, *, format: str) -> str:
     try:
         if format == "json":
             return json.dumps(data, indent=2)
         elif format == "yaml":
             yaml = import_module("yaml")
             return yaml.dump(data)
     except Exception:
         raise Error(f'Cannot dump "{format}" text from data: {data}')
     raise Error(f"Cannot dump data to text with format: {format}")
 
 
-def clean_data(data: types.IData):
+def clean_data(data: types.IDict):
     for key, value in list(data.items()):
         if isinstance(value, dict):
             clean_data(value)  # type: ignore
         elif isinstance(value, list):
             for item in value:  # type: ignore
                 if isinstance(item, dict):
                     clean_data(item)  # type: ignore
```

### Comparing `dplib_py-0.7.0/dplib/helpers/file.py` & `dplib_py-0.7.1/dplib/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/helpers/path.py` & `dplib_py-0.7.1/dplib/helpers/path.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/helpers/profile.py` & `dplib_py-0.7.1/dplib/helpers/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 from ..errors.metadata import MetadataError
 from .data import load_data
 from .file import read_file
 
 # TODO: implement additional user-side profile caching
 
 
-def check_profile(*, metadata: types.IData, profile: str) -> List[MetadataError]:
+def check_profile(*, metadata: types.IDict, profile: str) -> List[MetadataError]:
     # Prepare validator
     jsonSchema = read_profile(profile=profile)
     Validator = validator_for(jsonSchema)  # type: ignore
     validator = Validator(jsonSchema)  # type: ignore
 
     # Validate metadata
     errors: List[MetadataError] = []
     for validation_error in validator.iter_errors(metadata):  # type: ignore
         errors.append(MetadataError(validation_error))  # type: ignore
 
     return errors
 
 
 @lru_cache
-def read_profile(*, profile: str) -> types.IData:
+def read_profile(*, profile: str) -> types.IDict:
     parts = parse_profile(profile)
 
     # Replace with builtin copy
     if parts:
         version, filename = parts
         profile = os.path.join(settings.PROFILE_BASEDIR, version, filename)
```

### Comparing `dplib_py-0.7.0/dplib/models/contributor.py` & `dplib_py-0.7.1/dplib/models/contributor.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     roles: List[str] = []
     organization: Optional[str] = None
 
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def compat(cls, data: types.IData):
+    def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
 
         # contributor.role
         if not data.get("roles"):
             role = data.pop("role", None)
             if role:
```

### Comparing `dplib_py-0.7.0/dplib/models/dialect/dialect.py` & `dplib_py-0.7.1/dplib/models/dialect/dialect.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/dialect/__spec__/test_dialect.py` & `dplib_py-0.7.1/dplib/models/dialect/__spec__/test_dialect.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/types.py` & `dplib_py-0.7.1/dplib/models/field/types.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/__init__.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/base.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     A list of field values to consider as null values
     """
 
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def compat(cls, data: types.IData):
+    def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
 
         # field.format
         format = data.get("format")
         if format:
             if format.startswith("fmt:"):
```

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/boolean.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/boolean.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/geojson.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/geojson.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/geopoint.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/geopoint.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/integer.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/integer.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/list.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/list.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/number.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/number.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/field/datatypes/string.py` & `dplib_py-0.7.1/dplib/models/field/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/package/package.py` & `dplib_py-0.7.1/dplib/models/package/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/package/__spec__/test_package.py` & `dplib_py-0.7.1/dplib/models/package/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/resource/hash.py` & `dplib_py-0.7.1/dplib/models/resource/hash.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/resource/resource.py` & `dplib_py-0.7.1/dplib/models/resource/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
         Returns:
             The full path of the resource
         """
         if self.path and isinstance(self.path, str):
             return join_basepath(self.path, self.basepath)
 
-    def get_source(self) -> Optional[Union[str, types.IData]]:
+    def get_source(self) -> Optional[Union[str, types.IDict]]:
         """Get the source of the resource
 
         Returns:
             Data or full path
         """
         return self.data if self.data is not None else self.get_fullpath()
 
@@ -179,15 +179,15 @@
         if isinstance(self.schema, str):
             self.schema = Schema.from_path(self.schema, basepath=self.basepath)  # type: ignore
 
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def compat(cls, data: types.IData):
+    def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
 
         # resource.url
         if not data.get("path"):
             url = data.pop("url", None)
             if url:
```

### Comparing `dplib_py-0.7.0/dplib/models/resource/__spec__/test_resource.py` & `dplib_py-0.7.1/dplib/models/resource/__spec__/test_resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/models/schema/foreignKey.py` & `dplib_py-0.7.1/dplib/models/schema/foreignKey.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     fields: List[str] = []
     resource: Optional[str] = None
 
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def compat(cls, data: types.IData):
+    def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
 
         # foreignKey.reference.fields
         fields = data.get("fields", None)
         if isinstance(fields, str):
             data["fields"] = [fields]
@@ -32,15 +32,15 @@
     fields: List[str] = []
     reference: ForeignKeyReference = pydantic.Field(default_factory=ForeignKeyReference)
 
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def compat(cls, data: types.IData):
+    def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
 
         # foreignKey.fields
         fields = data.get("fields", None)
         if isinstance(fields, str):
             data["fields"] = [fields]
```

### Comparing `dplib_py-0.7.0/dplib/models/schema/schema.py` & `dplib_py-0.7.1/dplib/models/schema/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         """
         self.fields.append(field)
 
     # Compat
 
     @pydantic.model_validator(mode="before")
     @classmethod
-    def compat(cls, data: types.IData):
+    def compat(cls, data: types.IDict):
         if not isinstance(data, dict):  # type: ignore
             return data
 
         # schema.primaryKey
         primaryKey = data.get("primaryKey", None)
         if isinstance(primaryKey, str):
             data["primaryKey"] = [primaryKey]
```

### Comparing `dplib_py-0.7.0/dplib/models/schema/__spec__/test_schema.py` & `dplib_py-0.7.1/dplib/models/schema/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/ckan/models/package.py` & `dplib_py-0.7.1/dplib/plugins/ckan/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/ckan/models/resource.py` & `dplib_py-0.7.1/dplib/plugins/ckan/models/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,21 @@
 
     def to_dp(self) -> Resource:
         """Convert to Data Package resource
 
         Returns:
            Data Resource
         """
+        # Path/Name
         resource = Resource(path=self.name, name=slugify_name(self.name))
 
+        # Description
+        if self.description:
+            resource.description = self.description
+
         # Format
         if self.format:
             resource.format = self.format.lower()
 
         # Mediatype
         if self.mimetype:
             resource.mediatype = self.mimetype
@@ -61,14 +66,18 @@
         """
         if not resource.path or not isinstance(resource.path, str):
             return
 
         # Path
         ckan = CkanResource(name=resource.path)
 
+        # Description
+        if resource.description:
+            ckan.description = resource.description
+
         # Format
         if resource.format:
             ckan.format = resource.format.upper()
 
         # Mediatype
         if resource.mediatype:
             ckan.mimetype = resource.mediatype
```

### Comparing `dplib_py-0.7.0/dplib/plugins/ckan/models/__spec__/test_package.py` & `dplib_py-0.7.1/dplib/plugins/ckan/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/cli/program.py` & `dplib_py-0.7.1/dplib/plugins/cli/program.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/cli/commands/main.py` & `dplib_py-0.7.1/dplib/plugins/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/cli/commands/package/convert.py` & `dplib_py-0.7.1/dplib/plugins/cli/commands/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/cli/commands/resource/convert.py` & `dplib_py-0.7.1/dplib/plugins/cli/commands/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/cli/helpers/check.py` & `dplib_py-0.7.1/dplib/plugins/cli/helpers/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/datacite/models/contributor.py` & `dplib_py-0.7.1/dplib/plugins/datacite/models/contributor.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/datacite/models/package.py` & `dplib_py-0.7.1/dplib/plugins/datacite/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/datacite/models/__spec__/test_package.py` & `dplib_py-0.7.1/dplib/plugins/datacite/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/dcat/models/helpers.py` & `dplib_py-0.7.1/dplib/plugins/dcat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/dcat/models/loaders.py` & `dplib_py-0.7.1/dplib/plugins/dcat/models/loaders.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/dcat/models/namespaces.py` & `dplib_py-0.7.1/dplib/plugins/dcat/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/dcat/models/package.py` & `dplib_py-0.7.1/dplib/plugins/dcat/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/dcat/models/resource.py` & `dplib_py-0.7.1/dplib/plugins/dcat/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/dcat/models/__spec__/test_package.py` & `dplib_py-0.7.1/dplib/plugins/dcat/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/github/models/package.py` & `dplib_py-0.7.1/dplib/plugins/github/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/github/models/resource.py` & `dplib_py-0.7.1/dplib/plugins/github/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/github/models/__spec__/test_package.py` & `dplib_py-0.7.1/dplib/plugins/github/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/pandas/models/field.py` & `dplib_py-0.7.1/dplib/plugins/pandas/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/pandas/models/schema.py` & `dplib_py-0.7.1/dplib/plugins/pandas/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/polars/models/field.py` & `dplib_py-0.7.1/dplib/plugins/polars/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/polars/models/schema.py` & `dplib_py-0.7.1/dplib/plugins/polars/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/polars/models/__spec__/test_schema.py` & `dplib_py-0.7.1/dplib/plugins/polars/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/sql/models/field.py` & `dplib_py-0.7.1/dplib/plugins/sql/models/field.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/sql/models/schema.py` & `dplib_py-0.7.1/dplib/plugins/sql/models/schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/sql/models/__spec__/test_schema.py` & `dplib_py-0.7.1/dplib/plugins/sql/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/zenodo/models/creator.py` & `dplib_py-0.7.1/dplib/plugins/zenodo/models/creator.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/zenodo/models/package.py` & `dplib_py-0.7.1/dplib/plugins/zenodo/models/package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/zenodo/models/resource.py` & `dplib_py-0.7.1/dplib/plugins/zenodo/models/resource.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/plugins/zenodo/models/__spec__/test_package.py` & `dplib_py-0.7.1/dplib/plugins/zenodo/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/1.0/datapackage.json` & `dplib_py-0.7.1/dplib/profiles/1.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/1.0/dataresource.json` & `dplib_py-0.7.1/dplib/profiles/1.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/1.0/tabledialect.json` & `dplib_py-0.7.1/dplib/profiles/1.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/1.0/tableschema.json` & `dplib_py-0.7.1/dplib/profiles/1.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/2.0/datapackage.json` & `dplib_py-0.7.1/dplib/profiles/2.0/datapackage.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/2.0/dataresource.json` & `dplib_py-0.7.1/dplib/profiles/2.0/dataresource.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/2.0/tabledialect.json` & `dplib_py-0.7.1/dplib/profiles/2.0/tabledialect.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/profiles/2.0/tableschema.json` & `dplib_py-0.7.1/dplib/profiles/2.0/tableschema.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/dplib/system/model.py` & `dplib_py-0.7.1/dplib/system/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         return pprint.pformat(self.to_dict(), sort_dicts=False)
 
     @property
-    def custom(self) -> types.IData:
+    def custom(self) -> types.IDict:
         assert self.model_extra is not None
         return self.model_extra
 
     # Converters
 
     def to_path(self, path: str, *, format: Optional[str] = None):
         if not format:
@@ -58,15 +58,15 @@
 
     def to_dict(self):
         data = self.model_dump(mode="json", exclude_none=True, exclude_defaults=True)
         clean_data(data)
         return data
 
     @classmethod
-    def from_dict(cls, data: types.IData, *, basepath: Optional[str] = None) -> Self:
+    def from_dict(cls, data: types.IDict, *, basepath: Optional[str] = None) -> Self:
         if basepath and cls.model_fields.get("basepath"):
             data["basepath"] = basepath
         return cls(**data)
 
 
 # Although pydantic@2 moved all the model methods to the "model_" namespace
 # the "schema" method is still in the root namespace
```

### Comparing `dplib_py-0.7.0/dplib/system/__spec__/test_model.py` & `dplib_py-0.7.1/dplib/system/__spec__/test_model.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/.gitignore` & `dplib_py-0.7.1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -76,20 +76,14 @@
 
 # dotenv
 .env
 
 # Spyder project settings
 .spyderproject
 
-# Livemark
-/blog/**/*.html
-/docs/**/*.html
-/index.html
-/404.html
-
 # Extras
 .frictionless/
 .google.json
 coverage/
 .vscode/
 .server/
 site/
```

### Comparing `dplib_py-0.7.0/LICENSE.md` & `dplib_py-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/README.md` & `dplib_py-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.7.0/pyproject.toml` & `dplib_py-0.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -44,35 +44,32 @@
 [project.optional-dependencies]
 cli = ["typer>=0.12", "rich>=10.0"]
 dcat = ["rdflib>=6.0"]
 pandas = ["pandas>=1.0", "pandas-stubs>=1.0", "numpy>=1.0", "isodate>=0.6"]
 polars = ["polars-lts-cpu>=0.10"]
 sql = ["sqlalchemy>=1.4"]
 dev = [
-    "moto",
     "ruff",
-    "httpx",
     "hatch",
-    "yattag",
     "neovim",
-    "pytest",
-    "mkdocs",
     "pyright",
     "ipython",
+    # mkdocs
+    "mkdocs",
+    "mkdocstrings[python]",
+    "mkdocs-material",
+    # pytest
+    "pytest",
     "pytest-cov",
     "pytest-vcr",
     "pytest-mock",
     "pytest-only",
-    "oauth2client",
-    "requests-mock",
     "pytest-dotenv",
     "pytest-timeout",
     "pytest-lazy-fixtures",
-    "mkdocstrings[python]",
-    "mkdocs-material",
 ]
 
 [project.scripts]
 dp = "dplib.plugins.cli.__main__:program"
 
 [tool.hatch.version]
 path = "dplib/settings.py"
@@ -157,19 +154,12 @@
 
 [tool.pytest.ini_options]
 testpaths = ["dplib"]
 env_files = [".env"]
 markers = [
     "ci: integrational tests (select with '--ci')",
 ]
-filterwarnings = [
-    "ignore::DeprecationWarning:boto.*",
-    "ignore::DeprecationWarning:moto.*",
-    "ignore::DeprecationWarning:grako.*",
-    "ignore::DeprecationWarning:savWriter.*",
-    "ignore::Warning:duckdb_engine.*",
-]
 
 [tool.pyright]
 strict = ["dplib"]
 include = ["dplib"]
 ignore = ["**/__init__.py"]
```

### Comparing `dplib_py-0.7.0/PKG-INFO` & `dplib_py-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dplib-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python implementation of the Data Package standard
 Project-URL: homepage, https://github.com/frictionlessdata/dplib-py
 Author-email: Open Knowledge Foundation <info@okfn.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: data package,data validation,json schema,json table schema,open data,tabular data package
 Classifier: Development Status :: 4 - Beta
@@ -30,34 +30,29 @@
 Provides-Extra: cli
 Requires-Dist: rich>=10.0; extra == 'cli'
 Requires-Dist: typer>=0.12; extra == 'cli'
 Provides-Extra: dcat
 Requires-Dist: rdflib>=6.0; extra == 'dcat'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
-Requires-Dist: httpx; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mkdocs; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mkdocstrings[python]; extra == 'dev'
-Requires-Dist: moto; extra == 'dev'
 Requires-Dist: neovim; extra == 'dev'
-Requires-Dist: oauth2client; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-dotenv; extra == 'dev'
 Requires-Dist: pytest-lazy-fixtures; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest-only; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
 Requires-Dist: pytest-vcr; extra == 'dev'
-Requires-Dist: requests-mock; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
-Requires-Dist: yattag; extra == 'dev'
 Provides-Extra: pandas
 Requires-Dist: isodate>=0.6; extra == 'pandas'
 Requires-Dist: numpy>=1.0; extra == 'pandas'
 Requires-Dist: pandas-stubs>=1.0; extra == 'pandas'
 Requires-Dist: pandas>=1.0; extra == 'pandas'
 Provides-Extra: polars
 Requires-Dist: polars-lts-cpu>=0.10; extra == 'polars'
```

