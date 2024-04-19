# Comparing `tmp/cyclonedx_python_lib-7.1.0.tar.gz` & `tmp/cyclonedx_python_lib-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_python_lib-7.1.0.tar", max compression
+gzip compressed data, was "cyclonedx_python_lib-7.2.0.tar", max compression
```

## Comparing `cyclonedx_python_lib-7.1.0.tar` & `cyclonedx_python_lib-7.2.0.tar`

### file list

```diff
@@ -1,1135 +1,1135 @@
--rw-r--r--   0        0        0   225753 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/LICENSE
--rw-r--r--   0        0        0      147 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/NOTICE
--rw-r--r--   0        0        0     4569 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/README.md
--rw-r--r--   0        0        0      850 2024-04-10 09:25:20.688415 cyclonedx_python_lib-7.1.0/cyclonedx/__init__.py
--rw-r--r--   0        0        0      731 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/_internal/__init__.py
--rw-r--r--   0        0        0     1734 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/_internal/compare.py
--rw-r--r--   0        0        0     1164 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/_internal/hash.py
--rw-r--r--   0        0        0      847 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/_internal/time.py
--rw-r--r--   0        0        0      993 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/exception/__init__.py
--rw-r--r--   0        0        0     1536 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/exception/factory.py
--rw-r--r--   0        0        0     3685 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/exception/model.py
--rw-r--r--   0        0        0     1136 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/exception/output.py
--rw-r--r--   0        0        0     1730 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/exception/serialization.py
--rw-r--r--   0        0        0      680 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/factory/__init__.py
--rw-r--r--   0        0        0     3233 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/factory/license.py
--rw-r--r--   0        0        0    43540 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/__init__.py
--rw-r--r--   0        0        0    26098 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/bom.py
--rw-r--r--   0        0        0     2179 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/bom_ref.py
--rw-r--r--   0        0        0    57519 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/component.py
--rw-r--r--   0        0        0    11789 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/contact.py
--rw-r--r--   0        0        0    48270 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/crypto.py
--rw-r--r--   0        0        0     3766 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/dependency.py
--rw-r--r--   0        0        0     3568 2024-04-10 09:24:57.751950 cyclonedx_python_lib-7.1.0/cyclonedx/model/impact_analysis.py
--rw-r--r--   0        0        0     7024 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/model/issue.py
--rw-r--r--   0        0        0    10127 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/model/license.py
--rw-r--r--   0        0        0     8623 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/model/release_note.py
--rw-r--r--   0        0        0    12798 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/model/service.py
--rw-r--r--   0        0        0    43655 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/model/vulnerability.py
--rw-r--r--   0        0        0     5872 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/output/__init__.py
--rw-r--r--   0        0        0     4270 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/output/json.py
--rw-r--r--   0        0        0     4285 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/output/xml.py
--rw-r--r--   0        0        0      153 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/py.typed
--rw-r--r--   0        0        0     3018 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/__init__.py
--rw-r--r--   0        0        0     2127 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/README.md
--rw-r--r--   0        0        0     2493 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/__init__.py
--rw-r--r--   0        0        0    13604 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
--rw-r--r--   0        0        0    39716 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
--rw-r--r--   0        0        0    37194 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    36226 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    76383 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
--rw-r--r--   0        0        0    40408 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    39348 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    88794 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
--rw-r--r--   0        0        0    72383 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   133792 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
--rw-r--r--   0        0        0   164772 2024-04-10 09:24:57.755950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   311805 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
--rw-r--r--   0        0        0   252643 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   492947 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd
--rw-r--r--   0        0        0     8058 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    14269 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   165694 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
--rw-r--r--   0        0        0     2573 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/schema/schema.py
--rw-r--r--   0        0        0     6576 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/serialization/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/spdx.py
--rw-r--r--   0        0        0     3701 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/validation/__init__.py
--rw-r--r--   0        0        0     4817 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/validation/json.py
--rw-r--r--   0        0        0      853 2024-04-10 09:24:57.759950 cyclonedx_python_lib-7.1.0/cyclonedx/validation/model.py
--rw-r--r--   0        0        0     3672 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/cyclonedx/validation/xml.py
--rw-r--r--   0        0        0      634 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/Makefile
--rw-r--r--   0        0        0     1524 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/architecture.rst
--rw-r--r--   0        0        0      686 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/changelog.rst
--rw-r--r--   0        0        0     2657 2024-04-10 09:25:20.688415 cyclonedx_python_lib-7.1.0/docs/conf.py
--rw-r--r--   0        0        0       34 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/contributing.rst
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/examples.rst
--rw-r--r--   0        0        0     1857 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/index.rst
--rw-r--r--   0        0        0     1499 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/install.rst
--rw-r--r--   0        0        0      800 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/make.bat
--rw-r--r--   0        0        0     3275 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/modelling.rst
--rw-r--r--   0        0        0     2269 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/outputting.rst
--rw-r--r--   0        0        0       81 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     6132 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/schema-support.rst
--rw-r--r--   0        0        0     1329 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/docs/support.rst
--rw-r--r--   0        0        0      176 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/examples/README.md
--rw-r--r--   0        0        0     8164 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/examples/complex_deserialize.py
--rw-r--r--   0        0        0     4081 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/examples/complex_serialize.py
--rw-r--r--   0        0        0     4227 2024-04-10 09:25:20.688415 cyclonedx_python_lib-7.1.0/pyproject.toml
--rw-r--r--   0        0        0     6717 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/__init__.py
--rw-r--r--   0        0        0      704 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/__init__.py
--rw-r--r--   0        0        0    42374 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/models.py
--rw-r--r--   0        0        0       16 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/own/README.md
--rw-r--r--   0        0        0     1309 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     2461 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/own/xml/1.4/bom_setuptools.xml
--rw-r--r--   0        0        0    98508 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/own/xml/1.4/webgoat-6.1.xml
--rw-r--r--   0        0        0     3723 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
--rw-r--r--   0        0        0     1195 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
--rw-r--r--   0        0        0      559 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
--rw-r--r--   0        0        0      313 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
--rw-r--r--   0        0        0      246 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
--rw-r--r--   0        0        0      830 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
--rw-r--r--   0        0        0      801 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
--rw-r--r--   0        0        0      793 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
--rw-r--r--   0        0        0      769 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
--rw-r--r--   0        0        0      705 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
--rw-r--r--   0        0        0     1303 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
--rw-r--r--   0        0        0    16515 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
--rw-r--r--   0        0        0    16513 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
--rw-r--r--   0        0        0     1328 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
--rw-r--r--   0        0        0     1366 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
--rw-r--r--   0        0        0      302 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
--rw-r--r--   0        0        0    21038 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
--rw-r--r--   0        0        0      348 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
--rw-r--r--   0        0        0    21026 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
--rw-r--r--   0        0        0    21039 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
--rw-r--r--   0        0        0     1217 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
--rw-r--r--   0        0        0      704 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
--rw-r--r--   0        0        0      965 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
--rw-r--r--   0        0        0      186 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
--rw-r--r--   0        0        0    22339 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
--rw-r--r--   0        0        0     1210 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
--rw-r--r--   0        0        0     1214 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
--rw-r--r--   0        0        0     1226 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
--rw-r--r--   0        0        0      317 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
--rw-r--r--   0        0        0    21121 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
--rw-r--r--   0        0        0    10048 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
--rw-r--r--   0        0        0      165 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
--rw-r--r--   0        0        0      560 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
--rw-r--r--   0        0        0      385 2024-04-10 09:24:57.763950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
--rw-r--r--   0        0        0      433 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
--rw-r--r--   0        0        0      249 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
--rw-r--r--   0        0        0      314 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
--rw-r--r--   0        0        0      667 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
--rw-r--r--   0        0        0      809 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
--rw-r--r--   0        0        0      247 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
--rw-r--r--   0        0        0      856 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
--rw-r--r--   0        0        0      831 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
--rw-r--r--   0        0        0      827 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
--rw-r--r--   0        0        0      802 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
--rw-r--r--   0        0        0      819 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
--rw-r--r--   0        0        0      794 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
--rw-r--r--   0        0        0      795 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
--rw-r--r--   0        0        0      770 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
--rw-r--r--   0        0        0      731 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
--rw-r--r--   0        0        0      706 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
--rw-r--r--   0        0        0     1184 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
--rw-r--r--   0        0        0     1554 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
--rw-r--r--   0        0        0      515 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
--rw-r--r--   0        0        0     1304 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
--rw-r--r--   0        0        0    15788 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
--rw-r--r--   0        0        0    16516 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
--rw-r--r--   0        0        0      428 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
--rw-r--r--   0        0        0    16514 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
--rw-r--r--   0        0        0     1329 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
--rw-r--r--   0        0        0     1367 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
--rw-r--r--   0        0        0      209 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      244 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      303 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
--rw-r--r--   0        0        0    21039 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
--rw-r--r--   0        0        0     1185 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
--rw-r--r--   0        0        0     1555 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
--rw-r--r--   0        0        0      275 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
--rw-r--r--   0        0        0      349 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
--rw-r--r--   0        0        0      148 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
--rw-r--r--   0        0        0    21027 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
--rw-r--r--   0        0        0      416 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
--rw-r--r--   0        0        0      363 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
--rw-r--r--   0        0        0      361 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
--rw-r--r--   0        0        0      548 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
--rw-r--r--   0        0        0      792 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
--rw-r--r--   0        0        0    20390 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
--rw-r--r--   0        0        0    24278 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
--rw-r--r--   0        0        0     2163 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
--rw-r--r--   0        0        0     1897 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
--rw-r--r--   0        0        0      705 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
--rw-r--r--   0        0        0      456 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
--rw-r--r--   0        0        0     1342 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
--rw-r--r--   0        0        0     1346 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
--rw-r--r--   0        0        0      892 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
--rw-r--r--   0        0        0     1223 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
--rw-r--r--   0        0        0      693 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
--rw-r--r--   0        0        0      824 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
--rw-r--r--   0        0        0      161 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
--rw-r--r--   0        0        0      187 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
--rw-r--r--   0        0        0    22340 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
--rw-r--r--   0        0        0      438 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
--rw-r--r--   0        0        0     1211 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
--rw-r--r--   0        0        0     1215 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
--rw-r--r--   0        0        0      440 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
--rw-r--r--   0        0        0     1227 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
--rw-r--r--   0        0        0      333 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
--rw-r--r--   0        0        0      438 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
--rw-r--r--   0        0        0      417 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
--rw-r--r--   0        0        0      468 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
--rw-r--r--   0        0        0      224 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      254 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      605 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
--rw-r--r--   0        0        0      654 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
--rw-r--r--   0        0        0      253 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
--rw-r--r--   0        0        0      318 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
--rw-r--r--   0        0        0     2465 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
--rw-r--r--   0        0        0     3337 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
--rw-r--r--   0        0        0    21122 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
--rw-r--r--   0        0        0     2308 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json
--rw-r--r--   0        0        0     2693 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
--rw-r--r--   0        0        0      419 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
--rw-r--r--   0        0        0      495 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
--rw-r--r--   0        0        0    11181 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
--rw-r--r--   0        0        0      165 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
--rw-r--r--   0        0        0      560 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
--rw-r--r--   0        0        0      385 2024-04-10 09:24:57.767950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
--rw-r--r--   0        0        0      433 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
--rw-r--r--   0        0        0      249 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
--rw-r--r--   0        0        0      314 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
--rw-r--r--   0        0        0      667 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
--rw-r--r--   0        0        0      809 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
--rw-r--r--   0        0        0      197 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
--rw-r--r--   0        0        0      247 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
--rw-r--r--   0        0        0      856 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
--rw-r--r--   0        0        0      831 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
--rw-r--r--   0        0        0      827 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
--rw-r--r--   0        0        0      802 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
--rw-r--r--   0        0        0      819 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
--rw-r--r--   0        0        0      794 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
--rw-r--r--   0        0        0      795 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
--rw-r--r--   0        0        0      770 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
--rw-r--r--   0        0        0      731 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
--rw-r--r--   0        0        0      706 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
--rw-r--r--   0        0        0     1184 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
--rw-r--r--   0        0        0     1554 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
--rw-r--r--   0        0        0      515 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
--rw-r--r--   0        0        0     1304 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
--rw-r--r--   0        0        0    15788 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
--rw-r--r--   0        0        0    16516 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
--rw-r--r--   0        0        0      428 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
--rw-r--r--   0        0        0    16514 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
--rw-r--r--   0        0        0     1329 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
--rw-r--r--   0        0        0     1367 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
--rw-r--r--   0        0        0      277 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
--rw-r--r--   0        0        0      319 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      209 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      244 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      228 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
--rw-r--r--   0        0        0      303 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
--rw-r--r--   0        0        0    21039 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
--rw-r--r--   0        0        0     1185 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
--rw-r--r--   0        0        0     1555 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
--rw-r--r--   0        0        0      275 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
--rw-r--r--   0        0        0      349 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
--rw-r--r--   0        0        0      148 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
--rw-r--r--   0        0        0    21027 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
--rw-r--r--   0        0        0      416 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
--rw-r--r--   0        0        0      548 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
--rw-r--r--   0        0        0      792 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
--rw-r--r--   0        0        0    20390 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
--rw-r--r--   0        0        0    24278 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
--rw-r--r--   0        0        0     2163 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
--rw-r--r--   0        0        0     1897 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
--rw-r--r--   0        0        0      705 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
--rw-r--r--   0        0        0      456 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
--rw-r--r--   0        0        0     1342 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
--rw-r--r--   0        0        0     1346 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
--rw-r--r--   0        0        0      892 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
--rw-r--r--   0        0        0     1223 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
--rw-r--r--   0        0        0     1497 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
--rw-r--r--   0        0        0     1983 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
--rw-r--r--   0        0        0      693 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
--rw-r--r--   0        0        0      824 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
--rw-r--r--   0        0        0      161 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
--rw-r--r--   0        0        0      187 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
--rw-r--r--   0        0        0     1384 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
--rw-r--r--   0        0        0     1596 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
--rw-r--r--   0        0        0    22340 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
--rw-r--r--   0        0        0     1117 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
--rw-r--r--   0        0        0     1324 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
--rw-r--r--   0        0        0      438 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
--rw-r--r--   0        0        0     1211 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
--rw-r--r--   0        0        0     1215 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
--rw-r--r--   0        0        0      440 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
--rw-r--r--   0        0        0     1227 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
--rw-r--r--   0        0        0      333 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
--rw-r--r--   0        0        0      279 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
--rw-r--r--   0        0        0      321 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      438 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
--rw-r--r--   0        0        0      417 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
--rw-r--r--   0        0        0      468 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
--rw-r--r--   0        0        0      224 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      254 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      605 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
--rw-r--r--   0        0        0      654 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
--rw-r--r--   0        0        0      253 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
--rw-r--r--   0        0        0      318 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
--rw-r--r--   0        0        0     2465 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
--rw-r--r--   0        0        0     3337 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
--rw-r--r--   0        0        0      983 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
--rw-r--r--   0        0        0     1213 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
--rw-r--r--   0        0        0    21122 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
--rw-r--r--   0        0        0     2308 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json
--rw-r--r--   0        0        0     2693 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
--rw-r--r--   0        0        0      419 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
--rw-r--r--   0        0        0      495 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
--rw-r--r--   0        0        0    11181 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
--rw-r--r--   0        0        0      165 2024-04-10 09:24:57.771950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
--rw-r--r--   0        0        0      560 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
--rw-r--r--   0        0        0      385 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
--rw-r--r--   0        0        0      433 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
--rw-r--r--   0        0        0      249 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
--rw-r--r--   0        0        0      314 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
--rw-r--r--   0        0        0      667 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
--rw-r--r--   0        0        0      809 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
--rw-r--r--   0        0        0      197 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
--rw-r--r--   0        0        0      247 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
--rw-r--r--   0        0        0      856 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
--rw-r--r--   0        0        0      831 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
--rw-r--r--   0        0        0      827 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
--rw-r--r--   0        0        0      802 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
--rw-r--r--   0        0        0      819 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
--rw-r--r--   0        0        0      794 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
--rw-r--r--   0        0        0      795 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
--rw-r--r--   0        0        0      770 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
--rw-r--r--   0        0        0      731 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
--rw-r--r--   0        0        0      706 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
--rw-r--r--   0        0        0     1184 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
--rw-r--r--   0        0        0     1554 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
--rw-r--r--   0        0        0      515 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
--rw-r--r--   0        0        0     1304 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
--rw-r--r--   0        0        0    15788 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
--rw-r--r--   0        0        0    16516 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
--rw-r--r--   0        0        0      428 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
--rw-r--r--   0        0        0    16514 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
--rw-r--r--   0        0        0     1329 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
--rw-r--r--   0        0        0     1367 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
--rw-r--r--   0        0        0      277 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
--rw-r--r--   0        0        0      319 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      209 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      244 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      228 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
--rw-r--r--   0        0        0      303 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
--rw-r--r--   0        0        0    21039 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
--rw-r--r--   0        0        0     1185 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
--rw-r--r--   0        0        0     1555 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
--rw-r--r--   0        0        0      275 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
--rw-r--r--   0        0        0      349 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
--rw-r--r--   0        0        0      148 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
--rw-r--r--   0        0        0    21027 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
--rw-r--r--   0        0        0      416 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
--rw-r--r--   0        0        0      548 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
--rw-r--r--   0        0        0      792 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
--rw-r--r--   0        0        0    20390 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
--rw-r--r--   0        0        0    24278 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
--rw-r--r--   0        0        0     2163 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
--rw-r--r--   0        0        0     1897 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
--rw-r--r--   0        0        0      705 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
--rw-r--r--   0        0        0      456 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
--rw-r--r--   0        0        0     1342 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
--rw-r--r--   0        0        0     1346 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
--rw-r--r--   0        0        0      892 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
--rw-r--r--   0        0        0     1223 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
--rw-r--r--   0        0        0     1497 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
--rw-r--r--   0        0        0     1983 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
--rw-r--r--   0        0        0      693 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
--rw-r--r--   0        0        0      824 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
--rw-r--r--   0        0        0      161 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
--rw-r--r--   0        0        0      187 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
--rw-r--r--   0        0        0     1384 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
--rw-r--r--   0        0        0     1596 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
--rw-r--r--   0        0        0    22340 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
--rw-r--r--   0        0        0     1117 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
--rw-r--r--   0        0        0     1324 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
--rw-r--r--   0        0        0      438 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
--rw-r--r--   0        0        0     1211 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
--rw-r--r--   0        0        0     1215 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
--rw-r--r--   0        0        0      440 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
--rw-r--r--   0        0        0     1227 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
--rw-r--r--   0        0        0      333 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
--rw-r--r--   0        0        0      279 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
--rw-r--r--   0        0        0      321 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      438 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
--rw-r--r--   0        0        0      417 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
--rw-r--r--   0        0        0      468 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
--rw-r--r--   0        0        0      224 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      254 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      605 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
--rw-r--r--   0        0        0      654 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
--rw-r--r--   0        0        0      227 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
--rw-r--r--   0        0        0      281 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
--rw-r--r--   0        0        0     2465 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
--rw-r--r--   0        0        0     3337 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
--rw-r--r--   0        0        0      983 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
--rw-r--r--   0        0        0     1213 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
--rw-r--r--   0        0        0    21122 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
--rw-r--r--   0        0        0     5338 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
--rw-r--r--   0        0        0     6828 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
--rw-r--r--   0        0        0     2312 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json
--rw-r--r--   0        0        0     2693 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
--rw-r--r--   0        0        0      419 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
--rw-r--r--   0        0        0      495 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
--rw-r--r--   0        0        0     9733 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
--rw-r--r--   0        0        0     4274 2024-04-10 09:24:57.775950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
--rw-r--r--   0        0        0     5987 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
--rw-r--r--   0        0        0    11181 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
--rw-r--r--   0        0        0      165 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
--rw-r--r--   0        0        0      508 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
--rw-r--r--   0        0        0      866 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
--rw-r--r--   0        0        0      385 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
--rw-r--r--   0        0        0      433 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
--rw-r--r--   0        0        0      249 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
--rw-r--r--   0        0        0      314 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
--rw-r--r--   0        0        0      746 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
--rw-r--r--   0        0        0     1086 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
--rw-r--r--   0        0        0      197 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
--rw-r--r--   0        0        0      247 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
--rw-r--r--   0        0        0      856 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
--rw-r--r--   0        0        0      831 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
--rw-r--r--   0        0        0      827 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
--rw-r--r--   0        0        0      802 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
--rw-r--r--   0        0        0      819 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
--rw-r--r--   0        0        0      794 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
--rw-r--r--   0        0        0      795 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
--rw-r--r--   0        0        0      770 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
--rw-r--r--   0        0        0      731 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
--rw-r--r--   0        0        0      706 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
--rw-r--r--   0        0        0     1184 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
--rw-r--r--   0        0        0     1554 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
--rw-r--r--   0        0        0      515 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
--rw-r--r--   0        0        0     1304 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
--rw-r--r--   0        0        0    15788 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
--rw-r--r--   0        0        0    16516 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
--rw-r--r--   0        0        0      428 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
--rw-r--r--   0        0        0    16514 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
--rw-r--r--   0        0        0     1329 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
--rw-r--r--   0        0        0     1367 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
--rw-r--r--   0        0        0      277 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
--rw-r--r--   0        0        0      319 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      209 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      244 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0      228 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
--rw-r--r--   0        0        0      303 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
--rw-r--r--   0        0        0    21039 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
--rw-r--r--   0        0        0     1185 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
--rw-r--r--   0        0        0     1555 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
--rw-r--r--   0        0        0      275 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
--rw-r--r--   0        0        0      349 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
--rw-r--r--   0        0        0      148 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
--rw-r--r--   0        0        0    21027 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
--rw-r--r--   0        0        0      416 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
--rw-r--r--   0        0        0     2527 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
--rw-r--r--   0        0        0     3596 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
--rw-r--r--   0        0        0      548 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
--rw-r--r--   0        0        0      792 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
--rw-r--r--   0        0        0    20390 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
--rw-r--r--   0        0        0    24278 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
--rw-r--r--   0        0        0     2163 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
--rw-r--r--   0        0        0     1897 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
--rw-r--r--   0        0        0      705 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
--rw-r--r--   0        0        0      456 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
--rw-r--r--   0        0        0     1342 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
--rw-r--r--   0        0        0     1346 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
--rw-r--r--   0        0        0      892 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
--rw-r--r--   0        0        0     1223 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
--rw-r--r--   0        0        0     1810 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
--rw-r--r--   0        0        0     2449 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
--rw-r--r--   0        0        0      693 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
--rw-r--r--   0        0        0      824 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
--rw-r--r--   0        0        0      161 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
--rw-r--r--   0        0        0      187 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
--rw-r--r--   0        0        0     3189 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
--rw-r--r--   0        0        0     4519 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
--rw-r--r--   0        0        0    22340 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
--rw-r--r--   0        0        0     1117 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
--rw-r--r--   0        0        0     1324 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
--rw-r--r--   0        0        0     7703 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
--rw-r--r--   0        0        0    11757 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
--rw-r--r--   0        0        0      473 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
--rw-r--r--   0        0        0     1270 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
--rw-r--r--   0        0        0      467 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
--rw-r--r--   0        0        0     1236 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
--rw-r--r--   0        0        0     1539 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
--rw-r--r--   0        0        0     2197 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
--rw-r--r--   0        0        0      477 2024-04-10 09:24:57.779950 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
--rw-r--r--   0        0        0     1248 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
--rw-r--r--   0        0        0    98548 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
--rw-r--r--   0        0        0   100112 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
--rw-r--r--   0        0        0      333 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
--rw-r--r--   0        0        0      279 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
--rw-r--r--   0        0        0      321 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      436 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
--rw-r--r--   0        0        0      624 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
--rw-r--r--   0        0        0      507 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
--rw-r--r--   0        0        0      537 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
--rw-r--r--   0        0        0      482 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
--rw-r--r--   0        0        0      509 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
--rw-r--r--   0        0        0      224 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      254 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0     1162 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
--rw-r--r--   0        0        0     1471 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
--rw-r--r--   0        0        0      605 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
--rw-r--r--   0        0        0      654 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
--rw-r--r--   0        0        0      227 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
--rw-r--r--   0        0        0      281 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
--rw-r--r--   0        0        0     2465 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
--rw-r--r--   0        0        0     3337 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
--rw-r--r--   0        0        0     1520 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
--rw-r--r--   0        0        0     1660 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
--rw-r--r--   0        0        0    21122 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
--rw-r--r--   0        0        0     5338 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
--rw-r--r--   0        0        0     6828 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
--rw-r--r--   0        0        0     9412 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
--rw-r--r--   0        0        0    12249 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
--rw-r--r--   0        0        0     2312 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json
--rw-r--r--   0        0        0     2693 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
--rw-r--r--   0        0        0      419 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
--rw-r--r--   0        0        0      495 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
--rw-r--r--   0        0        0     9733 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
--rw-r--r--   0        0        0    17746 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
--rw-r--r--   0        0        0    19794 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
--rw-r--r--   0        0        0    11181 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
--rw-r--r--   0        0        0      165 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-bomformat-1.6.json
--rw-r--r--   0        0        0      508 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.json
--rw-r--r--   0        0        0      866 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml
--rw-r--r--   0        0        0      385 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.json
--rw-r--r--   0        0        0      433 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.xml
--rw-r--r--   0        0        0      249 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.json
--rw-r--r--   0        0        0      314 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.xml
--rw-r--r--   0        0        0      746 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json
--rw-r--r--   0        0        0     1086 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml
--rw-r--r--   0        0        0      197 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.json
--rw-r--r--   0        0        0      247 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.xml
--rw-r--r--   0        0        0      856 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json
--rw-r--r--   0        0        0      831 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml
--rw-r--r--   0        0        0      827 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json
--rw-r--r--   0        0        0      802 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml
--rw-r--r--   0        0        0      819 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json
--rw-r--r--   0        0        0      794 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml
--rw-r--r--   0        0        0      795 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json
--rw-r--r--   0        0        0      770 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml
--rw-r--r--   0        0        0      731 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json
--rw-r--r--   0        0        0      706 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml
--rw-r--r--   0        0        0     1184 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json
--rw-r--r--   0        0        0     1554 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml
--rw-r--r--   0        0        0      515 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json
--rw-r--r--   0        0        0     1304 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml
--rw-r--r--   0        0        0    15788 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json
--rw-r--r--   0        0        0    16516 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml
--rw-r--r--   0        0        0      428 2024-04-10 09:24:57.783951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.json
--rw-r--r--   0        0        0    16514 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml
--rw-r--r--   0        0        0     1329 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml
--rw-r--r--   0        0        0      360 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.json
--rw-r--r--   0        0        0      466 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.xml
--rw-r--r--   0        0        0     1367 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml
--rw-r--r--   0        0        0      277 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.json
--rw-r--r--   0        0        0      319 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.xml
--rw-r--r--   0        0        0      209 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.json
--rw-r--r--   0        0        0      244 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.xml
--rw-r--r--   0        0        0      228 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.json
--rw-r--r--   0        0        0      303 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.xml
--rw-r--r--   0        0        0    21039 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml
--rw-r--r--   0        0        0     1185 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json
--rw-r--r--   0        0        0     1555 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml
--rw-r--r--   0        0        0     1290 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json
--rw-r--r--   0        0        0     1504 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml
--rw-r--r--   0        0        0      275 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.json
--rw-r--r--   0        0        0      349 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.xml
--rw-r--r--   0        0        0      148 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.json
--rw-r--r--   0        0        0    21027 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.json
--rw-r--r--   0        0        0      416 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.xml
--rw-r--r--   0        0        0     2527 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json
--rw-r--r--   0        0        0     3596 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml
--rw-r--r--   0        0        0      548 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json
--rw-r--r--   0        0        0      792 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml
--rw-r--r--   0        0        0     5654 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json
--rw-r--r--   0        0        0     7084 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml
--rw-r--r--   0        0        0     6538 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json
--rw-r--r--   0        0        0    24921 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml
--rw-r--r--   0        0        0     2163 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json
--rw-r--r--   0        0        0     1897 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml
--rw-r--r--   0        0        0      750 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json
--rw-r--r--   0        0        0      865 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml
--rw-r--r--   0        0        0      394 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.json
--rw-r--r--   0        0        0      705 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml
--rw-r--r--   0        0        0      456 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.json
--rw-r--r--   0        0        0      492 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.xml
--rw-r--r--   0        0        0     1342 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json
--rw-r--r--   0        0        0     1346 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml
--rw-r--r--   0        0        0      892 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json
--rw-r--r--   0        0        0     1223 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml
--rw-r--r--   0        0        0     1810 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json
--rw-r--r--   0        0        0     2449 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml
--rw-r--r--   0        0        0     2978 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json
--rw-r--r--   0        0        0     4629 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml
--rw-r--r--   0        0        0     1459 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json
--rw-r--r--   0        0        0     2217 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml
--rw-r--r--   0        0        0      693 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json
--rw-r--r--   0        0        0      824 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml
--rw-r--r--   0        0        0      161 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.json
--rw-r--r--   0        0        0      187 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.xml
--rw-r--r--   0        0        0     4432 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json
--rw-r--r--   0        0        0     6383 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml
--rw-r--r--   0        0        0    22340 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml
--rw-r--r--   0        0        0     1117 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json
--rw-r--r--   0        0        0     1324 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml
--rw-r--r--   0        0        0     7703 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json
--rw-r--r--   0        0        0    11757 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml
--rw-r--r--   0        0        0      514 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json
--rw-r--r--   0        0        0     1297 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml
--rw-r--r--   0        0        0      510 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.json
--rw-r--r--   0        0        0     1263 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml
--rw-r--r--   0        0        0     1539 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json
--rw-r--r--   0        0        0     2197 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml
--rw-r--r--   0        0        0      477 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.json
--rw-r--r--   0        0        0     1248 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml
--rw-r--r--   0        0        0    98548 2024-04-10 09:24:57.787951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json
--rw-r--r--   0        0        0   100112 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml
--rw-r--r--   0        0        0     1835 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json
--rw-r--r--   0        0        0     2811 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml
--rw-r--r--   0        0        0      333 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.json
--rw-r--r--   0        0        0      430 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.xml
--rw-r--r--   0        0        0      432 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.json
--rw-r--r--   0        0        0      456 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.xml
--rw-r--r--   0        0        0      436 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.json
--rw-r--r--   0        0        0      624 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml
--rw-r--r--   0        0        0      521 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json
--rw-r--r--   0        0        0      551 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml
--rw-r--r--   0        0        0      508 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.json
--rw-r--r--   0        0        0      539 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml
--rw-r--r--   0        0        0      482 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.json
--rw-r--r--   0        0        0      509 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.xml
--rw-r--r--   0        0        0      224 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.json
--rw-r--r--   0        0        0      254 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.xml
--rw-r--r--   0        0        0     1162 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json
--rw-r--r--   0        0        0     1471 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml
--rw-r--r--   0        0        0      605 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json
--rw-r--r--   0        0        0      654 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml
--rw-r--r--   0        0        0      227 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.json
--rw-r--r--   0        0        0      281 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.xml
--rw-r--r--   0        0        0     2465 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json
--rw-r--r--   0        0        0     3337 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml
--rw-r--r--   0        0        0     1894 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json
--rw-r--r--   0        0        0     1872 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml
--rw-r--r--   0        0        0    21122 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml
--rw-r--r--   0        0        0     5338 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json
--rw-r--r--   0        0        0     6828 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml
--rw-r--r--   0        0        0     9412 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json
--rw-r--r--   0        0        0    12249 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml
--rw-r--r--   0        0        0     2312 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json
--rw-r--r--   0        0        0     2693 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml
--rw-r--r--   0        0        0      419 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.json
--rw-r--r--   0        0        0      495 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.xml
--rw-r--r--   0        0        0     9733 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json
--rw-r--r--   0        0        0     1902 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json
--rw-r--r--   0        0        0     2747 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml
--rw-r--r--   0        0        0      491 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.json
--rw-r--r--   0        0        0      870 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml
--rw-r--r--   0        0        0    17746 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json
--rw-r--r--   0        0        0    19794 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml
--rw-r--r--   0        0        0    11181 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml
--rw-r--r--   0        0        0      157 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/README.md
--rwxr-xr-x   0        0        0      745 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/fetch.sh
--rw-r--r--   0        0        0      391 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/README.md
--rw-r--r--   0        0        0      579 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
--rw-r--r--   0        0        0      649 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
--rw-r--r--   0        0        0     1050 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
--rw-r--r--   0        0        0     1055 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
--rw-r--r--   0        0        0     1050 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
--rw-r--r--   0        0        0     1055 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
--rw-r--r--   0        0        0     2128 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
--rw-r--r--   0        0        0     2211 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
--rw-r--r--   0        0        0     2264 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
--rw-r--r--   0        0        0     2326 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
--rw-r--r--   0        0        0     2264 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin
--rw-r--r--   0        0        0     2326 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin
--rw-r--r--   0        0        0      806 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
--rw-r--r--   0        0        0      949 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
--rw-r--r--   0        0        0     1835 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
--rw-r--r--   0        0        0     1806 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
--rw-r--r--   0        0        0     1835 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
--rw-r--r--   0        0        0     1806 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
--rw-r--r--   0        0        0     2808 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
--rw-r--r--   0        0        0     2877 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
--rw-r--r--   0        0        0     3596 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
--rw-r--r--   0        0        0     3640 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
--rw-r--r--   0        0        0     3788 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin
--rw-r--r--   0        0        0     3831 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
--rw-r--r--   0        0        0      944 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
--rw-r--r--   0        0        0      865 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
--rw-r--r--   0        0        0      944 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
--rw-r--r--   0        0        0      865 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
--rw-r--r--   0        0        0     2085 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
--rw-r--r--   0        0        0     2072 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
--rw-r--r--   0        0        0     2221 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
--rw-r--r--   0        0        0     2187 2024-04-10 09:24:57.791951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
--rw-r--r--   0        0        0     2221 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin
--rw-r--r--   0        0        0     2187 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
--rw-r--r--   0        0        0      496 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
--rw-r--r--   0        0        0      893 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin
--rw-r--r--   0        0        0      812 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
--rw-r--r--   0        0        0      893 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin
--rw-r--r--   0        0        0      812 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
--rw-r--r--   0        0        0     2013 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin
--rw-r--r--   0        0        0     2002 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
--rw-r--r--   0        0        0     2149 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin
--rw-r--r--   0        0        0     2117 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
--rw-r--r--   0        0        0     2149 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin
--rw-r--r--   0        0        0     2117 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
--rw-r--r--   0        0        0     4485 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
--rw-r--r--   0        0        0     4434 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
--rw-r--r--   0        0        0     4801 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
--rw-r--r--   0        0        0     4434 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
--rw-r--r--   0        0        0     4801 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
--rw-r--r--   0        0        0     5562 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
--rw-r--r--   0        0        0     5999 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
--rw-r--r--   0        0        0     5947 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
--rw-r--r--   0        0        0     6363 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
--rw-r--r--   0        0        0     5991 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin
--rw-r--r--   0        0        0     6407 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin
--rw-r--r--   0        0        0      749 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
--rw-r--r--   0        0        0      793 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
--rw-r--r--   0        0        0     1894 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
--rw-r--r--   0        0        0     1461 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
--rw-r--r--   0        0        0     1894 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
--rw-r--r--   0        0        0     1461 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
--rw-r--r--   0        0        0     3014 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
--rw-r--r--   0        0        0     2651 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
--rw-r--r--   0        0        0     3150 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
--rw-r--r--   0        0        0     2766 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
--rw-r--r--   0        0        0     3150 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin
--rw-r--r--   0        0        0     2766 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
--rw-r--r--   0        0        0     2092 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
--rw-r--r--   0        0        0     2289 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
--rw-r--r--   0        0        0     2228 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
--rw-r--r--   0        0        0     2404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
--rw-r--r--   0        0        0     2228 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin
--rw-r--r--   0        0        0     2404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
--rw-r--r--   0        0        0     3282 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
--rw-r--r--   0        0        0     3686 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
--rw-r--r--   0        0        0     3418 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
--rw-r--r--   0        0        0     3801 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
--rw-r--r--   0        0        0     3418 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin
--rw-r--r--   0        0        0     3801 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
--rw-r--r--   0        0        0     1827 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
--rw-r--r--   0        0        0     2023 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
--rw-r--r--   0        0        0     1963 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
--rw-r--r--   0        0        0     2138 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
--rw-r--r--   0        0        0     1963 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin
--rw-r--r--   0        0        0     2138 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
--rw-r--r--   0        0        0     2577 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
--rw-r--r--   0        0        0     2822 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
--rw-r--r--   0        0        0     2713 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
--rw-r--r--   0        0        0     2937 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
--rw-r--r--   0        0        0     2713 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin
--rw-r--r--   0        0        0     2937 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
--rw-r--r--   0        0        0     1081 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
--rw-r--r--   0        0        0     1083 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
--rw-r--r--   0        0        0     1081 2024-04-10 09:24:57.795951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
--rw-r--r--   0        0        0     1083 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2201 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
--rw-r--r--   0        0        0     2273 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2337 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
--rw-r--r--   0        0        0     2388 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
--rw-r--r--   0        0        0     2337 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin
--rw-r--r--   0        0        0     2388 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
--rw-r--r--   0        0        0      886 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
--rw-r--r--   0        0        0      821 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
--rw-r--r--   0        0        0      886 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
--rw-r--r--   0        0        0      821 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2006 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
--rw-r--r--   0        0        0     2011 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2142 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
--rw-r--r--   0        0        0     2126 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
--rw-r--r--   0        0        0     2142 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin
--rw-r--r--   0        0        0     2126 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
--rw-r--r--   0        0        0     2014 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
--rw-r--r--   0        0        0     2243 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
--rw-r--r--   0        0        0     2150 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
--rw-r--r--   0        0        0     2358 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
--rw-r--r--   0        0        0     2150 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin
--rw-r--r--   0        0        0     2358 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
--rw-r--r--   0        0        0     2025 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
--rw-r--r--   0        0        0     2268 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
--rw-r--r--   0        0        0     2161 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
--rw-r--r--   0        0        0     2383 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
--rw-r--r--   0        0        0     2161 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin
--rw-r--r--   0        0        0     2383 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin
--rw-r--r--   0        0        0      596 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
--rw-r--r--   0        0        0      695 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
--rw-r--r--   0        0        0     1561 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
--rw-r--r--   0        0        0     1597 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
--rw-r--r--   0        0        0     1561 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
--rw-r--r--   0        0        0     1597 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
--rw-r--r--   0        0        0     2702 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
--rw-r--r--   0        0        0     2804 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
--rw-r--r--   0        0        0     2838 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
--rw-r--r--   0        0        0     2919 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
--rw-r--r--   0        0        0     2838 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin
--rw-r--r--   0        0        0     2919 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin
--rw-r--r--   0        0        0      662 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
--rw-r--r--   0        0        0      678 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
--rw-r--r--   0        0        0     1385 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
--rw-r--r--   0        0        0     1402 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
--rw-r--r--   0        0        0     1385 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
--rw-r--r--   0        0        0     1402 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
--rw-r--r--   0        0        0     2526 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
--rw-r--r--   0        0        0     2609 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
--rw-r--r--   0        0        0     2662 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
--rw-r--r--   0        0        0     2724 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
--rw-r--r--   0        0        0     2662 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin
--rw-r--r--   0        0        0     2724 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
--rw-r--r--   0        0        0      847 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
--rw-r--r--   0        0        0     1085 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
--rw-r--r--   0        0        0     1163 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
--rw-r--r--   0        0        0     1085 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
--rw-r--r--   0        0        0     1163 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
--rw-r--r--   0        0        0     2205 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
--rw-r--r--   0        0        0     2353 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
--rw-r--r--   0        0        0     2341 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
--rw-r--r--   0        0        0     2468 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
--rw-r--r--   0        0        0     2341 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin
--rw-r--r--   0        0        0     2468 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
--rw-r--r--   0        0        0     8540 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
--rw-r--r--   0        0        0     8315 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
--rw-r--r--   0        0        0    10266 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
--rw-r--r--   0        0        0     9628 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
--rw-r--r--   0        0        0    13173 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
--rw-r--r--   0        0        0    12575 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
--rw-r--r--   0        0        0    13309 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
--rw-r--r--   0        0        0    12690 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
--rw-r--r--   0        0        0    14474 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin
--rw-r--r--   0        0        0    14004 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-04-10 09:24:57.799951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin
--rw-r--r--   0        0        0     2739 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin
--rw-r--r--   0        0        0     3108 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin
--rw-r--r--   0        0        0     2449 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin
--rw-r--r--   0        0        0     2636 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin
--rw-r--r--   0        0        0     3086 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin
--rw-r--r--   0        0        0     3518 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin
--rw-r--r--   0        0        0     2634 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin
--rw-r--r--   0        0        0     2831 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
--rw-r--r--   0        0        0     2164 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
--rw-r--r--   0        0        0     2217 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
--rw-r--r--   0        0        0     2164 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin
--rw-r--r--   0        0        0     2217 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin
--rw-r--r--   0        0        0     1199 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
--rw-r--r--   0        0        0     4993 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
--rw-r--r--   0        0        0     7631 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
--rw-r--r--   0        0        0     7396 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
--rw-r--r--   0        0        0     8830 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
--rw-r--r--   0        0        0     8293 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
--rw-r--r--   0        0        0    11737 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
--rw-r--r--   0        0        0    11240 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
--rw-r--r--   0        0        0    11873 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
--rw-r--r--   0        0        0    11355 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
--rw-r--r--   0        0        0    12042 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin
--rw-r--r--   0        0        0    11556 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin
--rw-r--r--   0        0        0      307 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
--rw-r--r--   0        0        0      477 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
--rw-r--r--   0        0        0      860 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
--rw-r--r--   0        0        0      859 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
--rw-r--r--   0        0        0      860 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
--rw-r--r--   0        0        0      859 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
--rw-r--r--   0        0        0     1980 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
--rw-r--r--   0        0        0     2049 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
--rw-r--r--   0        0        0     2116 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
--rw-r--r--   0        0        0     2164 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
--rw-r--r--   0        0        0     2116 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin
--rw-r--r--   0        0        0     2164 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin
--rw-r--r--   0        0        0      395 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
--rw-r--r--   0        0        0      572 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
--rw-r--r--   0        0        0      952 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
--rw-r--r--   0        0        0      961 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
--rw-r--r--   0        0        0      952 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
--rw-r--r--   0        0        0      961 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
--rw-r--r--   0        0        0     2093 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
--rw-r--r--   0        0        0     2168 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
--rw-r--r--   0        0        0     2229 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
--rw-r--r--   0        0        0     2283 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
--rw-r--r--   0        0        0     2229 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin
--rw-r--r--   0        0        0     2283 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
--rw-r--r--   0        0        0     3848 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
--rw-r--r--   0        0        0     3888 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
--rw-r--r--   0        0        0     3984 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
--rw-r--r--   0        0        0     4003 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
--rw-r--r--   0        0        0     3984 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin
--rw-r--r--   0        0        0     4003 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin
--rw-r--r--   0        0        0     2164 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin
--rw-r--r--   0        0        0     2217 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin
--rw-r--r--   0        0        0     3918 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin
--rw-r--r--   0        0        0     4052 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
--rw-r--r--   0        0        0     5189 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
--rw-r--r--   0        0        0     5704 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
--rw-r--r--   0        0        0     5325 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
--rw-r--r--   0        0        0     5819 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
--rw-r--r--   0        0        0     5518 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin
--rw-r--r--   0        0        0     6044 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin
--rw-r--r--   0        0        0      448 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
--rw-r--r--   0        0        0     1056 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
--rw-r--r--   0        0        0     1071 2024-04-10 09:24:57.803951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
--rw-r--r--   0        0        0     1243 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
--rw-r--r--   0        0        0     1214 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
--rw-r--r--   0        0        0     2384 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
--rw-r--r--   0        0        0     2421 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
--rw-r--r--   0        0        0     2520 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
--rw-r--r--   0        0        0     2536 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
--rw-r--r--   0        0        0     2520 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin
--rw-r--r--   0        0        0     2536 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin
--rw-r--r--   0        0        0      655 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
--rw-r--r--   0        0        0      980 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
--rw-r--r--   0        0        0     1582 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
--rw-r--r--   0        0        0     1579 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
--rw-r--r--   0        0        0     1769 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
--rw-r--r--   0        0        0     1722 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
--rw-r--r--   0        0        0     2889 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
--rw-r--r--   0        0        0     2912 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
--rw-r--r--   0        0        0     3025 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
--rw-r--r--   0        0        0     3027 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
--rw-r--r--   0        0        0     3025 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin
--rw-r--r--   0        0        0     3027 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin
--rw-r--r--   0        0        0      654 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
--rw-r--r--   0        0        0     1045 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
--rw-r--r--   0        0        0     1562 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
--rw-r--r--   0        0        0     1749 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
--rw-r--r--   0        0        0     2890 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
--rw-r--r--   0        0        0     3026 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
--rw-r--r--   0        0        0     3042 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
--rw-r--r--   0        0        0     3026 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin
--rw-r--r--   0        0        0     3042 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
--rw-r--r--   0        0        0      431 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
--rw-r--r--   0        0        0      629 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
--rw-r--r--   0        0        0      666 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
--rw-r--r--   0        0        0      792 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
--rw-r--r--   0        0        0      797 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
--rw-r--r--   0        0        0     1933 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
--rw-r--r--   0        0        0     2004 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
--rw-r--r--   0        0        0     2069 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
--rw-r--r--   0        0        0     2119 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
--rw-r--r--   0        0        0     2069 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin
--rw-r--r--   0        0        0     2119 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin
--rw-r--r--   0        0        0      516 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      814 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     2131 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
--rw-r--r--   0        0        0     2058 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     2231 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
--rw-r--r--   0        0        0     2149 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     3288 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
--rw-r--r--   0        0        0     3288 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     3424 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
--rw-r--r--   0        0        0     3403 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
--rw-r--r--   0        0        0     3507 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin
--rw-r--r--   0        0        0     3458 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin
--rw-r--r--   0        0        0      448 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
--rw-r--r--   0        0        0     1575 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
--rw-r--r--   0        0        0     1762 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
--rw-r--r--   0        0        0     2903 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
--rw-r--r--   0        0        0     3039 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
--rw-r--r--   0        0        0     3042 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
--rw-r--r--   0        0        0     3039 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin
--rw-r--r--   0        0        0     3042 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin
--rw-r--r--   0        0        0      245 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      459 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     1475 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
--rw-r--r--   0        0        0     1382 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     1649 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
--rw-r--r--   0        0        0     1533 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     2748 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
--rw-r--r--   0        0        0     2706 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     2884 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
--rw-r--r--   0        0        0     2821 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
--rw-r--r--   0        0        0     2884 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin
--rw-r--r--   0        0        0     2821 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
--rw-r--r--   0        0        0     3900 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
--rw-r--r--   0        0        0     4021 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
--rw-r--r--   0        0        0     4263 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
--rw-r--r--   0        0        0     4295 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
--rw-r--r--   0        0        0     7224 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
--rw-r--r--   0        0        0     7288 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
--rw-r--r--   0        0        0     7360 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
--rw-r--r--   0        0        0     7403 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
--rw-r--r--   0        0        0     7915 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin
--rw-r--r--   0        0        0     8054 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
--rw-r--r--   0        0        0     2106 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
--rw-r--r--   0        0        0     2196 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
--rw-r--r--   0        0        0     2469 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
--rw-r--r--   0        0        0     2470 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
--rw-r--r--   0        0        0     5430 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
--rw-r--r--   0        0        0     5463 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
--rw-r--r--   0        0        0     5566 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
--rw-r--r--   0        0        0     5578 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
--rw-r--r--   0        0        0     5735 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin
--rw-r--r--   0        0        0     5779 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
--rw-r--r--   0        0        0     1030 2024-04-10 09:24:57.807951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
--rw-r--r--   0        0        0     1040 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
--rw-r--r--   0        0        0     1030 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
--rw-r--r--   0        0        0     1040 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
--rw-r--r--   0        0        0     2171 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
--rw-r--r--   0        0        0     2247 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
--rw-r--r--   0        0        0     2307 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
--rw-r--r--   0        0        0     2362 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
--rw-r--r--   0        0        0     2307 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin
--rw-r--r--   0        0        0     2362 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin
--rw-r--r--   0        0        0     2957 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_component.py
--rw-r--r--   0        0        0     3283 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_deserialize_json.py
--rw-r--r--   0        0        0     1764 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_deserialize_xml.py
--rw-r--r--   0        0        0    19038 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_enums.py
--rw-r--r--   0        0        0     4389 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_factory_license.py
--rw-r--r--   0        0        0    22602 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model.py
--rw-r--r--   0        0        0    13254 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_bom.py
--rw-r--r--   0        0        0     2782 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_bom_ref.py
--rw-r--r--   0        0        0    18544 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_component.py
--rw-r--r--   0        0        0     1793 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_dependency.py
--rw-r--r--   0        0        0     4064 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_issue.py
--rw-r--r--   0        0        0     4295 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_license.py
--rw-r--r--   0        0        0     2758 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_release_note.py
--rw-r--r--   0        0        0     3390 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_service.py
--rw-r--r--   0        0        0    14370 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_model_vulnerability.py
--rw-r--r--   0        0        0     3154 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_output.py
--rw-r--r--   0        0        0     4587 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_output_json.py
--rw-r--r--   0        0        0     4029 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_output_xml.py
--rw-r--r--   0        0        0     1307 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_real_world_examples.py
--rw-r--r--   0        0        0     2509 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_schema_SchemaVersion.py
--rw-r--r--   0        0        0     1248 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_schema__res.py
--rw-r--r--   0        0        0     2873 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_spdx.py
--rw-r--r--   0        0        0     1977 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_validation.py
--rw-r--r--   0        0        0     4529 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_validation_json.py
--rw-r--r--   0        0        0     3061 2024-04-10 09:24:57.811951 cyclonedx_python_lib-7.1.0/tests/test_validation_xml.py
--rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 cyclonedx_python_lib-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0   226311 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/LICENSE
+-rw-r--r--   0        0        0      147 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/NOTICE
+-rw-r--r--   0        0        0     4569 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/README.md
+-rw-r--r--   0        0        0      850 2024-04-19 11:19:33.305857 cyclonedx_python_lib-7.2.0/cyclonedx/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/_internal/__init__.py
+-rw-r--r--   0        0        0     1734 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/_internal/compare.py
+-rw-r--r--   0        0        0     1164 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/_internal/hash.py
+-rw-r--r--   0        0        0      847 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/_internal/time.py
+-rw-r--r--   0        0        0      993 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/exception/__init__.py
+-rw-r--r--   0        0        0     1536 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/exception/factory.py
+-rw-r--r--   0        0        0     3685 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/exception/model.py
+-rw-r--r--   0        0        0     1136 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/exception/output.py
+-rw-r--r--   0        0        0     1730 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/exception/serialization.py
+-rw-r--r--   0        0        0      680 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/factory/__init__.py
+-rw-r--r--   0        0        0     3233 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/factory/license.py
+-rw-r--r--   0        0        0    43540 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/model/__init__.py
+-rw-r--r--   0        0        0    26098 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/model/bom.py
+-rw-r--r--   0        0        0     2179 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/model/bom_ref.py
+-rw-r--r--   0        0        0    57519 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/model/component.py
+-rw-r--r--   0        0        0    11789 2024-04-19 11:19:12.933684 cyclonedx_python_lib-7.2.0/cyclonedx/model/contact.py
+-rw-r--r--   0        0        0    48270 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/crypto.py
+-rw-r--r--   0        0        0     3766 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/dependency.py
+-rw-r--r--   0        0        0     3568 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/impact_analysis.py
+-rw-r--r--   0        0        0     7024 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/issue.py
+-rw-r--r--   0        0        0    13004 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/license.py
+-rw-r--r--   0        0        0     8623 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/release_note.py
+-rw-r--r--   0        0        0    12798 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/service.py
+-rw-r--r--   0        0        0    43655 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/model/vulnerability.py
+-rw-r--r--   0        0        0     5872 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/output/__init__.py
+-rw-r--r--   0        0        0     4270 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/output/json.py
+-rw-r--r--   0        0        0     4285 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/output/xml.py
+-rw-r--r--   0        0        0      153 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/py.typed
+-rw-r--r--   0        0        0     3018 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/__init__.py
+-rw-r--r--   0        0        0     2127 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/README.md
+-rw-r--r--   0        0        0     2493 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/__init__.py
+-rw-r--r--   0        0        0    13604 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    39716 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    37194 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    36226 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    76383 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    40408 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    39348 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    88794 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    72383 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   133792 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   164772 2024-04-19 11:19:12.937684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   311805 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   252643 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   492947 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     8058 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    14269 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   165694 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     2573 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/schema/schema.py
+-rw-r--r--   0        0        0     6576 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/serialization/__init__.py
+-rw-r--r--   0        0        0     2503 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/spdx.py
+-rw-r--r--   0        0        0     3701 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/validation/__init__.py
+-rw-r--r--   0        0        0     4817 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/validation/json.py
+-rw-r--r--   0        0        0      853 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/validation/model.py
+-rw-r--r--   0        0        0     3672 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/cyclonedx/validation/xml.py
+-rw-r--r--   0        0        0      634 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1524 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/docs/architecture.rst
+-rw-r--r--   0        0        0      686 2024-04-19 11:19:12.941684 cyclonedx_python_lib-7.2.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2657 2024-04-19 11:19:33.305857 cyclonedx_python_lib-7.2.0/docs/conf.py
+-rw-r--r--   0        0        0       34 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/examples.rst
+-rw-r--r--   0        0        0     1857 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/index.rst
+-rw-r--r--   0        0        0     1499 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/install.rst
+-rw-r--r--   0        0        0      800 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/make.bat
+-rw-r--r--   0        0        0     3275 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/modelling.rst
+-rw-r--r--   0        0        0     2269 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/outputting.rst
+-rw-r--r--   0        0        0       81 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     8093 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/schema-support.rst
+-rw-r--r--   0        0        0     1329 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/docs/support.rst
+-rw-r--r--   0        0        0      176 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/examples/README.md
+-rw-r--r--   0        0        0     8164 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/examples/complex_deserialize.py
+-rw-r--r--   0        0        0     4081 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/examples/complex_serialize.py
+-rw-r--r--   0        0        0     4227 2024-04-19 11:19:33.305857 cyclonedx_python_lib-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6967 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/__init__.py
+-rw-r--r--   0        0        0    42995 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/models.py
+-rw-r--r--   0        0        0       16 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/own/README.md
+-rw-r--r--   0        0        0     1309 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     2461 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/own/xml/1.4/bom_setuptools.xml
+-rw-r--r--   0        0        0    98508 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/own/xml/1.4/webgoat-6.1.xml
+-rw-r--r--   0        0        0     3723 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
+-rw-r--r--   0        0        0     1195 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
+-rw-r--r--   0        0        0      559 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      313 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
+-rw-r--r--   0        0        0      246 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
+-rw-r--r--   0        0        0      830 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
+-rw-r--r--   0        0        0      801 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
+-rw-r--r--   0        0        0      793 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
+-rw-r--r--   0        0        0      769 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
+-rw-r--r--   0        0        0      705 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
+-rw-r--r--   0        0        0     1303 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
+-rw-r--r--   0        0        0    16515 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
+-rw-r--r--   0        0        0    16513 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1328 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
+-rw-r--r--   0        0        0     1366 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
+-rw-r--r--   0        0        0      302 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
+-rw-r--r--   0        0        0    21038 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
+-rw-r--r--   0        0        0      348 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
+-rw-r--r--   0        0        0    21026 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
+-rw-r--r--   0        0        0    21039 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
+-rw-r--r--   0        0        0     1217 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
+-rw-r--r--   0        0        0      704 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      965 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
+-rw-r--r--   0        0        0      186 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
+-rw-r--r--   0        0        0    22339 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
+-rw-r--r--   0        0        0     1210 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
+-rw-r--r--   0        0        0     1214 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1226 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
+-rw-r--r--   0        0        0      317 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
+-rw-r--r--   0        0        0    21121 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
+-rw-r--r--   0        0        0    10048 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
+-rw-r--r--   0        0        0      165 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
+-rw-r--r--   0        0        0      560 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      385 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
+-rw-r--r--   0        0        0      433 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
+-rw-r--r--   0        0        0      249 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
+-rw-r--r--   0        0        0      314 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
+-rw-r--r--   0        0        0      667 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
+-rw-r--r--   0        0        0      809 2024-04-19 11:19:12.945684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
+-rw-r--r--   0        0        0      247 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
+-rw-r--r--   0        0        0      856 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
+-rw-r--r--   0        0        0      831 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
+-rw-r--r--   0        0        0      827 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
+-rw-r--r--   0        0        0      802 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
+-rw-r--r--   0        0        0      819 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
+-rw-r--r--   0        0        0      794 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
+-rw-r--r--   0        0        0      795 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
+-rw-r--r--   0        0        0      770 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
+-rw-r--r--   0        0        0      731 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
+-rw-r--r--   0        0        0      706 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
+-rw-r--r--   0        0        0     1184 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
+-rw-r--r--   0        0        0     1554 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
+-rw-r--r--   0        0        0      515 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
+-rw-r--r--   0        0        0     1304 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
+-rw-r--r--   0        0        0    15788 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
+-rw-r--r--   0        0        0    16516 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
+-rw-r--r--   0        0        0      428 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
+-rw-r--r--   0        0        0    16514 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
+-rw-r--r--   0        0        0     1329 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
+-rw-r--r--   0        0        0     1367 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
+-rw-r--r--   0        0        0      209 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      244 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      303 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
+-rw-r--r--   0        0        0    21039 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
+-rw-r--r--   0        0        0     1185 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
+-rw-r--r--   0        0        0     1555 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
+-rw-r--r--   0        0        0      275 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
+-rw-r--r--   0        0        0      349 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
+-rw-r--r--   0        0        0      148 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
+-rw-r--r--   0        0        0    21027 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
+-rw-r--r--   0        0        0      416 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
+-rw-r--r--   0        0        0      363 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
+-rw-r--r--   0        0        0      361 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
+-rw-r--r--   0        0        0      548 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
+-rw-r--r--   0        0        0      792 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
+-rw-r--r--   0        0        0    20390 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
+-rw-r--r--   0        0        0    24278 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
+-rw-r--r--   0        0        0     2163 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
+-rw-r--r--   0        0        0     1897 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
+-rw-r--r--   0        0        0      705 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      456 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
+-rw-r--r--   0        0        0     1342 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
+-rw-r--r--   0        0        0     1346 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
+-rw-r--r--   0        0        0      892 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
+-rw-r--r--   0        0        0     1223 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
+-rw-r--r--   0        0        0      693 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
+-rw-r--r--   0        0        0      824 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
+-rw-r--r--   0        0        0      161 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
+-rw-r--r--   0        0        0      187 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
+-rw-r--r--   0        0        0    22340 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
+-rw-r--r--   0        0        0      438 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
+-rw-r--r--   0        0        0     1211 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
+-rw-r--r--   0        0        0     1215 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
+-rw-r--r--   0        0        0      440 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
+-rw-r--r--   0        0        0     1227 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
+-rw-r--r--   0        0        0      333 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
+-rw-r--r--   0        0        0      438 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
+-rw-r--r--   0        0        0      417 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
+-rw-r--r--   0        0        0      468 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
+-rw-r--r--   0        0        0      224 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      254 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      605 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
+-rw-r--r--   0        0        0      654 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
+-rw-r--r--   0        0        0      253 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
+-rw-r--r--   0        0        0      318 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
+-rw-r--r--   0        0        0     2465 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
+-rw-r--r--   0        0        0     3337 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
+-rw-r--r--   0        0        0    21122 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
+-rw-r--r--   0        0        0     2308 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json
+-rw-r--r--   0        0        0     2693 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
+-rw-r--r--   0        0        0      419 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
+-rw-r--r--   0        0        0      495 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
+-rw-r--r--   0        0        0    11181 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
+-rw-r--r--   0        0        0      165 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
+-rw-r--r--   0        0        0      560 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      385 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
+-rw-r--r--   0        0        0      433 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
+-rw-r--r--   0        0        0      249 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
+-rw-r--r--   0        0        0      314 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
+-rw-r--r--   0        0        0      667 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
+-rw-r--r--   0        0        0      809 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
+-rw-r--r--   0        0        0      197 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
+-rw-r--r--   0        0        0      247 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
+-rw-r--r--   0        0        0      856 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
+-rw-r--r--   0        0        0      831 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
+-rw-r--r--   0        0        0      827 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
+-rw-r--r--   0        0        0      802 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
+-rw-r--r--   0        0        0      819 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
+-rw-r--r--   0        0        0      794 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
+-rw-r--r--   0        0        0      795 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
+-rw-r--r--   0        0        0      770 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
+-rw-r--r--   0        0        0      731 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
+-rw-r--r--   0        0        0      706 2024-04-19 11:19:12.949684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
+-rw-r--r--   0        0        0     1184 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
+-rw-r--r--   0        0        0     1554 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
+-rw-r--r--   0        0        0      515 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
+-rw-r--r--   0        0        0     1304 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
+-rw-r--r--   0        0        0    15788 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
+-rw-r--r--   0        0        0    16516 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
+-rw-r--r--   0        0        0      428 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
+-rw-r--r--   0        0        0    16514 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
+-rw-r--r--   0        0        0     1329 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
+-rw-r--r--   0        0        0     1367 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
+-rw-r--r--   0        0        0      277 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      319 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      209 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      244 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      228 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
+-rw-r--r--   0        0        0      303 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
+-rw-r--r--   0        0        0    21039 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
+-rw-r--r--   0        0        0     1185 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
+-rw-r--r--   0        0        0     1555 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
+-rw-r--r--   0        0        0      275 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
+-rw-r--r--   0        0        0      349 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
+-rw-r--r--   0        0        0      148 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
+-rw-r--r--   0        0        0    21027 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
+-rw-r--r--   0        0        0      416 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
+-rw-r--r--   0        0        0      548 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
+-rw-r--r--   0        0        0      792 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
+-rw-r--r--   0        0        0    20390 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
+-rw-r--r--   0        0        0    24278 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
+-rw-r--r--   0        0        0     2163 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
+-rw-r--r--   0        0        0     1897 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
+-rw-r--r--   0        0        0      705 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      456 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
+-rw-r--r--   0        0        0     1342 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
+-rw-r--r--   0        0        0     1346 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
+-rw-r--r--   0        0        0      892 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
+-rw-r--r--   0        0        0     1223 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
+-rw-r--r--   0        0        0     1497 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
+-rw-r--r--   0        0        0     1983 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
+-rw-r--r--   0        0        0      693 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
+-rw-r--r--   0        0        0      824 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
+-rw-r--r--   0        0        0      161 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
+-rw-r--r--   0        0        0      187 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
+-rw-r--r--   0        0        0     1384 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
+-rw-r--r--   0        0        0     1596 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
+-rw-r--r--   0        0        0    22340 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
+-rw-r--r--   0        0        0     1117 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
+-rw-r--r--   0        0        0     1324 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
+-rw-r--r--   0        0        0      438 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
+-rw-r--r--   0        0        0     1211 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
+-rw-r--r--   0        0        0     1215 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
+-rw-r--r--   0        0        0      440 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
+-rw-r--r--   0        0        0     1227 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
+-rw-r--r--   0        0        0      333 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
+-rw-r--r--   0        0        0      279 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      321 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      438 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
+-rw-r--r--   0        0        0      417 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
+-rw-r--r--   0        0        0      468 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
+-rw-r--r--   0        0        0      224 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      254 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      605 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
+-rw-r--r--   0        0        0      654 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
+-rw-r--r--   0        0        0      253 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
+-rw-r--r--   0        0        0      318 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
+-rw-r--r--   0        0        0     2465 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
+-rw-r--r--   0        0        0     3337 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
+-rw-r--r--   0        0        0      983 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
+-rw-r--r--   0        0        0     1213 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
+-rw-r--r--   0        0        0    21122 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
+-rw-r--r--   0        0        0     2308 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json
+-rw-r--r--   0        0        0     2693 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
+-rw-r--r--   0        0        0      419 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
+-rw-r--r--   0        0        0      495 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
+-rw-r--r--   0        0        0    11181 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
+-rw-r--r--   0        0        0      165 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
+-rw-r--r--   0        0        0      560 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      385 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
+-rw-r--r--   0        0        0      433 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
+-rw-r--r--   0        0        0      249 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
+-rw-r--r--   0        0        0      314 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
+-rw-r--r--   0        0        0      667 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
+-rw-r--r--   0        0        0      809 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
+-rw-r--r--   0        0        0      197 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
+-rw-r--r--   0        0        0      247 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
+-rw-r--r--   0        0        0      856 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
+-rw-r--r--   0        0        0      831 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
+-rw-r--r--   0        0        0      827 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
+-rw-r--r--   0        0        0      802 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
+-rw-r--r--   0        0        0      819 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
+-rw-r--r--   0        0        0      794 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
+-rw-r--r--   0        0        0      795 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
+-rw-r--r--   0        0        0      770 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
+-rw-r--r--   0        0        0      731 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
+-rw-r--r--   0        0        0      706 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
+-rw-r--r--   0        0        0     1184 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
+-rw-r--r--   0        0        0     1554 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
+-rw-r--r--   0        0        0      515 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
+-rw-r--r--   0        0        0     1304 2024-04-19 11:19:12.953684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
+-rw-r--r--   0        0        0    15788 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
+-rw-r--r--   0        0        0    16516 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
+-rw-r--r--   0        0        0      428 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
+-rw-r--r--   0        0        0    16514 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
+-rw-r--r--   0        0        0     1329 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
+-rw-r--r--   0        0        0     1367 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
+-rw-r--r--   0        0        0      277 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      319 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      209 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      244 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      228 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
+-rw-r--r--   0        0        0      303 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
+-rw-r--r--   0        0        0    21039 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
+-rw-r--r--   0        0        0     1185 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
+-rw-r--r--   0        0        0     1555 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
+-rw-r--r--   0        0        0      275 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
+-rw-r--r--   0        0        0      349 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
+-rw-r--r--   0        0        0      148 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
+-rw-r--r--   0        0        0    21027 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
+-rw-r--r--   0        0        0      416 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
+-rw-r--r--   0        0        0      548 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
+-rw-r--r--   0        0        0      792 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
+-rw-r--r--   0        0        0    20390 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
+-rw-r--r--   0        0        0    24278 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
+-rw-r--r--   0        0        0     2163 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
+-rw-r--r--   0        0        0     1897 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
+-rw-r--r--   0        0        0      705 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      456 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
+-rw-r--r--   0        0        0     1342 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
+-rw-r--r--   0        0        0     1346 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
+-rw-r--r--   0        0        0      892 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
+-rw-r--r--   0        0        0     1223 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
+-rw-r--r--   0        0        0     1497 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
+-rw-r--r--   0        0        0     1983 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
+-rw-r--r--   0        0        0      693 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
+-rw-r--r--   0        0        0      824 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
+-rw-r--r--   0        0        0      161 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
+-rw-r--r--   0        0        0      187 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
+-rw-r--r--   0        0        0     1384 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
+-rw-r--r--   0        0        0     1596 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
+-rw-r--r--   0        0        0    22340 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
+-rw-r--r--   0        0        0     1117 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
+-rw-r--r--   0        0        0     1324 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
+-rw-r--r--   0        0        0      438 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
+-rw-r--r--   0        0        0     1211 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
+-rw-r--r--   0        0        0     1215 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
+-rw-r--r--   0        0        0      440 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
+-rw-r--r--   0        0        0     1227 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
+-rw-r--r--   0        0        0      333 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
+-rw-r--r--   0        0        0      279 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      321 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      438 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
+-rw-r--r--   0        0        0      417 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
+-rw-r--r--   0        0        0      468 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
+-rw-r--r--   0        0        0      224 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      254 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      605 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
+-rw-r--r--   0        0        0      654 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
+-rw-r--r--   0        0        0      227 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
+-rw-r--r--   0        0        0      281 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
+-rw-r--r--   0        0        0     2465 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
+-rw-r--r--   0        0        0     3337 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
+-rw-r--r--   0        0        0      983 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
+-rw-r--r--   0        0        0     1213 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
+-rw-r--r--   0        0        0    21122 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
+-rw-r--r--   0        0        0     5338 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
+-rw-r--r--   0        0        0     6828 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
+-rw-r--r--   0        0        0     2312 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json
+-rw-r--r--   0        0        0     2693 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
+-rw-r--r--   0        0        0      419 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
+-rw-r--r--   0        0        0      495 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
+-rw-r--r--   0        0        0     9733 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
+-rw-r--r--   0        0        0     4274 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
+-rw-r--r--   0        0        0     5987 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
+-rw-r--r--   0        0        0    11181 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
+-rw-r--r--   0        0        0      165 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
+-rw-r--r--   0        0        0      508 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
+-rw-r--r--   0        0        0      866 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      385 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
+-rw-r--r--   0        0        0      433 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
+-rw-r--r--   0        0        0      249 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
+-rw-r--r--   0        0        0      314 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
+-rw-r--r--   0        0        0      746 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
+-rw-r--r--   0        0        0     1086 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
+-rw-r--r--   0        0        0      197 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
+-rw-r--r--   0        0        0      247 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
+-rw-r--r--   0        0        0      856 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
+-rw-r--r--   0        0        0      831 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
+-rw-r--r--   0        0        0      827 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
+-rw-r--r--   0        0        0      802 2024-04-19 11:19:12.957684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
+-rw-r--r--   0        0        0      819 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
+-rw-r--r--   0        0        0      794 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
+-rw-r--r--   0        0        0      795 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
+-rw-r--r--   0        0        0      770 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
+-rw-r--r--   0        0        0      731 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
+-rw-r--r--   0        0        0      706 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
+-rw-r--r--   0        0        0     1184 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
+-rw-r--r--   0        0        0     1554 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
+-rw-r--r--   0        0        0      515 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
+-rw-r--r--   0        0        0     1304 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
+-rw-r--r--   0        0        0    15788 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
+-rw-r--r--   0        0        0    16516 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
+-rw-r--r--   0        0        0      428 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
+-rw-r--r--   0        0        0    16514 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1329 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
+-rw-r--r--   0        0        0     1367 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
+-rw-r--r--   0        0        0      277 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      319 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      209 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      244 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0      228 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
+-rw-r--r--   0        0        0      303 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
+-rw-r--r--   0        0        0    21039 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
+-rw-r--r--   0        0        0     1185 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
+-rw-r--r--   0        0        0     1555 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
+-rw-r--r--   0        0        0      275 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
+-rw-r--r--   0        0        0      349 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
+-rw-r--r--   0        0        0      148 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
+-rw-r--r--   0        0        0    21027 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
+-rw-r--r--   0        0        0      416 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
+-rw-r--r--   0        0        0     2527 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
+-rw-r--r--   0        0        0     3596 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
+-rw-r--r--   0        0        0      548 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
+-rw-r--r--   0        0        0      792 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
+-rw-r--r--   0        0        0    20390 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
+-rw-r--r--   0        0        0    24278 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
+-rw-r--r--   0        0        0     2163 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
+-rw-r--r--   0        0        0     1897 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
+-rw-r--r--   0        0        0      705 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      456 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
+-rw-r--r--   0        0        0     1342 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
+-rw-r--r--   0        0        0     1346 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
+-rw-r--r--   0        0        0      892 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
+-rw-r--r--   0        0        0     1223 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
+-rw-r--r--   0        0        0     1810 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
+-rw-r--r--   0        0        0     2449 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
+-rw-r--r--   0        0        0      693 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
+-rw-r--r--   0        0        0      824 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
+-rw-r--r--   0        0        0      161 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
+-rw-r--r--   0        0        0      187 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
+-rw-r--r--   0        0        0     3189 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
+-rw-r--r--   0        0        0     4519 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
+-rw-r--r--   0        0        0    22340 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
+-rw-r--r--   0        0        0     1117 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
+-rw-r--r--   0        0        0     1324 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
+-rw-r--r--   0        0        0     7703 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
+-rw-r--r--   0        0        0    11757 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
+-rw-r--r--   0        0        0      473 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
+-rw-r--r--   0        0        0     1270 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
+-rw-r--r--   0        0        0      467 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
+-rw-r--r--   0        0        0     1236 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1539 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
+-rw-r--r--   0        0        0     2197 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
+-rw-r--r--   0        0        0      477 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
+-rw-r--r--   0        0        0     1248 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
+-rw-r--r--   0        0        0    98548 2024-04-19 11:19:12.961684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
+-rw-r--r--   0        0        0   100112 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
+-rw-r--r--   0        0        0      333 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
+-rw-r--r--   0        0        0      279 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      321 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      436 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
+-rw-r--r--   0        0        0      624 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
+-rw-r--r--   0        0        0      507 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
+-rw-r--r--   0        0        0      537 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
+-rw-r--r--   0        0        0      482 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
+-rw-r--r--   0        0        0      509 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
+-rw-r--r--   0        0        0      224 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      254 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0     1162 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
+-rw-r--r--   0        0        0     1471 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
+-rw-r--r--   0        0        0      605 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
+-rw-r--r--   0        0        0      654 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
+-rw-r--r--   0        0        0      227 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
+-rw-r--r--   0        0        0      281 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
+-rw-r--r--   0        0        0     2465 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
+-rw-r--r--   0        0        0     3337 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
+-rw-r--r--   0        0        0     1520 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
+-rw-r--r--   0        0        0     1660 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
+-rw-r--r--   0        0        0    21122 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
+-rw-r--r--   0        0        0     5338 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
+-rw-r--r--   0        0        0     6828 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
+-rw-r--r--   0        0        0     9412 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
+-rw-r--r--   0        0        0    12249 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
+-rw-r--r--   0        0        0     2312 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json
+-rw-r--r--   0        0        0     2693 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
+-rw-r--r--   0        0        0      419 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
+-rw-r--r--   0        0        0      495 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
+-rw-r--r--   0        0        0     9733 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
+-rw-r--r--   0        0        0    17746 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
+-rw-r--r--   0        0        0    19794 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
+-rw-r--r--   0        0        0    11181 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
+-rw-r--r--   0        0        0      165 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-bomformat-1.6.json
+-rw-r--r--   0        0        0      508 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.json
+-rw-r--r--   0        0        0      866 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml
+-rw-r--r--   0        0        0      385 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.json
+-rw-r--r--   0        0        0      433 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.xml
+-rw-r--r--   0        0        0      249 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.json
+-rw-r--r--   0        0        0      314 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.xml
+-rw-r--r--   0        0        0      746 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json
+-rw-r--r--   0        0        0     1086 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml
+-rw-r--r--   0        0        0      197 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.json
+-rw-r--r--   0        0        0      247 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.xml
+-rw-r--r--   0        0        0      856 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json
+-rw-r--r--   0        0        0      831 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml
+-rw-r--r--   0        0        0      827 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json
+-rw-r--r--   0        0        0      802 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml
+-rw-r--r--   0        0        0      819 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json
+-rw-r--r--   0        0        0      794 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml
+-rw-r--r--   0        0        0      795 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json
+-rw-r--r--   0        0        0      770 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml
+-rw-r--r--   0        0        0      731 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json
+-rw-r--r--   0        0        0      706 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml
+-rw-r--r--   0        0        0     1184 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json
+-rw-r--r--   0        0        0     1554 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml
+-rw-r--r--   0        0        0      515 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json
+-rw-r--r--   0        0        0     1304 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml
+-rw-r--r--   0        0        0    15788 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json
+-rw-r--r--   0        0        0    16516 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml
+-rw-r--r--   0        0        0      428 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.json
+-rw-r--r--   0        0        0    16514 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml
+-rw-r--r--   0        0        0     1329 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml
+-rw-r--r--   0        0        0      360 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.json
+-rw-r--r--   0        0        0      466 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.xml
+-rw-r--r--   0        0        0     1367 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml
+-rw-r--r--   0        0        0      277 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.json
+-rw-r--r--   0        0        0      319 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.xml
+-rw-r--r--   0        0        0      209 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.json
+-rw-r--r--   0        0        0      244 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.xml
+-rw-r--r--   0        0        0      228 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.json
+-rw-r--r--   0        0        0      303 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.xml
+-rw-r--r--   0        0        0    21039 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml
+-rw-r--r--   0        0        0     1185 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json
+-rw-r--r--   0        0        0     1555 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml
+-rw-r--r--   0        0        0     1290 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json
+-rw-r--r--   0        0        0     1504 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml
+-rw-r--r--   0        0        0      275 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.json
+-rw-r--r--   0        0        0      349 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.xml
+-rw-r--r--   0        0        0      148 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.json
+-rw-r--r--   0        0        0    21027 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.json
+-rw-r--r--   0        0        0      416 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.xml
+-rw-r--r--   0        0        0     2527 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json
+-rw-r--r--   0        0        0     3596 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml
+-rw-r--r--   0        0        0      548 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json
+-rw-r--r--   0        0        0      792 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml
+-rw-r--r--   0        0        0     5654 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json
+-rw-r--r--   0        0        0     7084 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml
+-rw-r--r--   0        0        0     6538 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json
+-rw-r--r--   0        0        0    24921 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml
+-rw-r--r--   0        0        0     2163 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json
+-rw-r--r--   0        0        0     1897 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml
+-rw-r--r--   0        0        0      750 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json
+-rw-r--r--   0        0        0      865 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml
+-rw-r--r--   0        0        0      394 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.json
+-rw-r--r--   0        0        0      705 2024-04-19 11:19:12.965684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml
+-rw-r--r--   0        0        0      456 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.json
+-rw-r--r--   0        0        0      492 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.xml
+-rw-r--r--   0        0        0     1342 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json
+-rw-r--r--   0        0        0     1346 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml
+-rw-r--r--   0        0        0      892 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json
+-rw-r--r--   0        0        0     1223 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml
+-rw-r--r--   0        0        0     1810 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json
+-rw-r--r--   0        0        0     2449 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml
+-rw-r--r--   0        0        0     2978 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json
+-rw-r--r--   0        0        0     4629 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml
+-rw-r--r--   0        0        0     1459 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json
+-rw-r--r--   0        0        0     2217 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml
+-rw-r--r--   0        0        0      693 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json
+-rw-r--r--   0        0        0      824 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml
+-rw-r--r--   0        0        0      161 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.json
+-rw-r--r--   0        0        0      187 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.xml
+-rw-r--r--   0        0        0     4432 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json
+-rw-r--r--   0        0        0     6383 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml
+-rw-r--r--   0        0        0    22340 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml
+-rw-r--r--   0        0        0     1117 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json
+-rw-r--r--   0        0        0     1324 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml
+-rw-r--r--   0        0        0     7703 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json
+-rw-r--r--   0        0        0    11757 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml
+-rw-r--r--   0        0        0      514 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json
+-rw-r--r--   0        0        0     1297 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml
+-rw-r--r--   0        0        0      510 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.json
+-rw-r--r--   0        0        0     1263 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml
+-rw-r--r--   0        0        0     1539 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json
+-rw-r--r--   0        0        0     2197 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml
+-rw-r--r--   0        0        0      477 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.json
+-rw-r--r--   0        0        0     1248 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml
+-rw-r--r--   0        0        0    98548 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json
+-rw-r--r--   0        0        0   100112 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml
+-rw-r--r--   0        0        0     1835 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json
+-rw-r--r--   0        0        0     2811 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml
+-rw-r--r--   0        0        0      333 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.json
+-rw-r--r--   0        0        0      430 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.xml
+-rw-r--r--   0        0        0      432 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.json
+-rw-r--r--   0        0        0      456 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.xml
+-rw-r--r--   0        0        0      436 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.json
+-rw-r--r--   0        0        0      624 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml
+-rw-r--r--   0        0        0      521 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json
+-rw-r--r--   0        0        0      551 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml
+-rw-r--r--   0        0        0      508 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.json
+-rw-r--r--   0        0        0      539 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml
+-rw-r--r--   0        0        0      482 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.json
+-rw-r--r--   0        0        0      509 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.xml
+-rw-r--r--   0        0        0      224 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.json
+-rw-r--r--   0        0        0      254 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.xml
+-rw-r--r--   0        0        0     1162 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json
+-rw-r--r--   0        0        0     1471 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml
+-rw-r--r--   0        0        0      605 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json
+-rw-r--r--   0        0        0      654 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml
+-rw-r--r--   0        0        0      227 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.json
+-rw-r--r--   0        0        0      281 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.xml
+-rw-r--r--   0        0        0     2465 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json
+-rw-r--r--   0        0        0     3337 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml
+-rw-r--r--   0        0        0     1894 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json
+-rw-r--r--   0        0        0     1872 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml
+-rw-r--r--   0        0        0    21122 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml
+-rw-r--r--   0        0        0     5338 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json
+-rw-r--r--   0        0        0     6828 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml
+-rw-r--r--   0        0        0     9412 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json
+-rw-r--r--   0        0        0    12249 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml
+-rw-r--r--   0        0        0     2312 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json
+-rw-r--r--   0        0        0     2693 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml
+-rw-r--r--   0        0        0      419 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.json
+-rw-r--r--   0        0        0      495 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.xml
+-rw-r--r--   0        0        0     9733 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json
+-rw-r--r--   0        0        0     1902 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json
+-rw-r--r--   0        0        0     2747 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml
+-rw-r--r--   0        0        0      491 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.json
+-rw-r--r--   0        0        0      870 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml
+-rw-r--r--   0        0        0    17746 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json
+-rw-r--r--   0        0        0    19794 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml
+-rw-r--r--   0        0        0    11181 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml
+-rw-r--r--   0        0        0      157 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/README.md
+-rwxr-xr-x   0        0        0      745 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/fetch.sh
+-rw-r--r--   0        0        0      391 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/README.md
+-rw-r--r--   0        0        0      579 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
+-rw-r--r--   0        0        0      649 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
+-rw-r--r--   0        0        0     1050 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
+-rw-r--r--   0        0        0     1055 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
+-rw-r--r--   0        0        0     1050 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
+-rw-r--r--   0        0        0     1055 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
+-rw-r--r--   0        0        0     2128 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
+-rw-r--r--   0        0        0     2211 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
+-rw-r--r--   0        0        0     2264 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
+-rw-r--r--   0        0        0     2326 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
+-rw-r--r--   0        0        0     2264 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin
+-rw-r--r--   0        0        0     2326 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin
+-rw-r--r--   0        0        0      806 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
+-rw-r--r--   0        0        0      949 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
+-rw-r--r--   0        0        0     1835 2024-04-19 11:19:12.969684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
+-rw-r--r--   0        0        0     1806 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
+-rw-r--r--   0        0        0     1835 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
+-rw-r--r--   0        0        0     1806 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
+-rw-r--r--   0        0        0     2808 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
+-rw-r--r--   0        0        0     2877 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
+-rw-r--r--   0        0        0     3596 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
+-rw-r--r--   0        0        0     3640 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
+-rw-r--r--   0        0        0     3788 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin
+-rw-r--r--   0        0        0     3831 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
+-rw-r--r--   0        0        0      944 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
+-rw-r--r--   0        0        0      865 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
+-rw-r--r--   0        0        0      944 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
+-rw-r--r--   0        0        0      865 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
+-rw-r--r--   0        0        0     2085 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
+-rw-r--r--   0        0        0     2072 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
+-rw-r--r--   0        0        0     2221 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
+-rw-r--r--   0        0        0     2187 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
+-rw-r--r--   0        0        0     2221 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin
+-rw-r--r--   0        0        0     2187 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
+-rw-r--r--   0        0        0      496 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
+-rw-r--r--   0        0        0      893 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin
+-rw-r--r--   0        0        0      812 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
+-rw-r--r--   0        0        0      893 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin
+-rw-r--r--   0        0        0      812 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
+-rw-r--r--   0        0        0     2013 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin
+-rw-r--r--   0        0        0     2002 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
+-rw-r--r--   0        0        0     2149 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin
+-rw-r--r--   0        0        0     2117 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
+-rw-r--r--   0        0        0     2149 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin
+-rw-r--r--   0        0        0     2117 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
+-rw-r--r--   0        0        0     4485 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
+-rw-r--r--   0        0        0     4434 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
+-rw-r--r--   0        0        0     4801 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
+-rw-r--r--   0        0        0     4434 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
+-rw-r--r--   0        0        0     4801 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
+-rw-r--r--   0        0        0     5562 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
+-rw-r--r--   0        0        0     5999 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
+-rw-r--r--   0        0        0     5947 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
+-rw-r--r--   0        0        0     6363 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
+-rw-r--r--   0        0        0     5991 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin
+-rw-r--r--   0        0        0     6407 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin
+-rw-r--r--   0        0        0      749 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
+-rw-r--r--   0        0        0      793 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
+-rw-r--r--   0        0        0     1894 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
+-rw-r--r--   0        0        0     1461 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
+-rw-r--r--   0        0        0     1894 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
+-rw-r--r--   0        0        0     1461 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
+-rw-r--r--   0        0        0     3014 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
+-rw-r--r--   0        0        0     2651 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
+-rw-r--r--   0        0        0     3150 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
+-rw-r--r--   0        0        0     2766 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
+-rw-r--r--   0        0        0     3150 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin
+-rw-r--r--   0        0        0     2766 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
+-rw-r--r--   0        0        0     2092 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
+-rw-r--r--   0        0        0     2289 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
+-rw-r--r--   0        0        0     2228 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
+-rw-r--r--   0        0        0     2404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
+-rw-r--r--   0        0        0     2228 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin
+-rw-r--r--   0        0        0     2404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
+-rw-r--r--   0        0        0     3282 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
+-rw-r--r--   0        0        0     3686 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
+-rw-r--r--   0        0        0     3418 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
+-rw-r--r--   0        0        0     3801 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
+-rw-r--r--   0        0        0     3418 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin
+-rw-r--r--   0        0        0     3801 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
+-rw-r--r--   0        0        0     1827 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
+-rw-r--r--   0        0        0     2023 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
+-rw-r--r--   0        0        0     1963 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
+-rw-r--r--   0        0        0     2138 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
+-rw-r--r--   0        0        0     1963 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin
+-rw-r--r--   0        0        0     2138 2024-04-19 11:19:12.973684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
+-rw-r--r--   0        0        0     2577 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
+-rw-r--r--   0        0        0     2822 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
+-rw-r--r--   0        0        0     2713 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
+-rw-r--r--   0        0        0     2937 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
+-rw-r--r--   0        0        0     2713 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin
+-rw-r--r--   0        0        0     2937 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
+-rw-r--r--   0        0        0     1081 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
+-rw-r--r--   0        0        0     1083 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
+-rw-r--r--   0        0        0     1081 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
+-rw-r--r--   0        0        0     1083 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2201 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2273 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2337 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2388 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
+-rw-r--r--   0        0        0     2337 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin
+-rw-r--r--   0        0        0     2388 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
+-rw-r--r--   0        0        0      886 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
+-rw-r--r--   0        0        0      821 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
+-rw-r--r--   0        0        0      886 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
+-rw-r--r--   0        0        0      821 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2006 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2011 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2142 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2126 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
+-rw-r--r--   0        0        0     2142 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin
+-rw-r--r--   0        0        0     2126 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
+-rw-r--r--   0        0        0     2014 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
+-rw-r--r--   0        0        0     2243 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
+-rw-r--r--   0        0        0     2150 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
+-rw-r--r--   0        0        0     2358 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
+-rw-r--r--   0        0        0     2150 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin
+-rw-r--r--   0        0        0     2358 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
+-rw-r--r--   0        0        0     2025 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
+-rw-r--r--   0        0        0     2268 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
+-rw-r--r--   0        0        0     2161 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
+-rw-r--r--   0        0        0     2383 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
+-rw-r--r--   0        0        0     2161 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin
+-rw-r--r--   0        0        0     2383 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin
+-rw-r--r--   0        0        0      596 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
+-rw-r--r--   0        0        0      695 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1561 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
+-rw-r--r--   0        0        0     1597 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1561 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
+-rw-r--r--   0        0        0     1597 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2702 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
+-rw-r--r--   0        0        0     2804 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2838 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
+-rw-r--r--   0        0        0     2919 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
+-rw-r--r--   0        0        0     2838 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin
+-rw-r--r--   0        0        0     2919 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin
+-rw-r--r--   0        0        0      662 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
+-rw-r--r--   0        0        0      678 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1385 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
+-rw-r--r--   0        0        0     1402 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1385 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
+-rw-r--r--   0        0        0     1402 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2526 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
+-rw-r--r--   0        0        0     2609 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2662 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
+-rw-r--r--   0        0        0     2724 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
+-rw-r--r--   0        0        0     2662 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin
+-rw-r--r--   0        0        0     2724 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
+-rw-r--r--   0        0        0      847 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
+-rw-r--r--   0        0        0     1085 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
+-rw-r--r--   0        0        0     1163 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
+-rw-r--r--   0        0        0     1085 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
+-rw-r--r--   0        0        0     1163 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
+-rw-r--r--   0        0        0     2205 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
+-rw-r--r--   0        0        0     2353 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
+-rw-r--r--   0        0        0     2341 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
+-rw-r--r--   0        0        0     2468 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
+-rw-r--r--   0        0        0     2341 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin
+-rw-r--r--   0        0        0     2468 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
+-rw-r--r--   0        0        0     8540 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
+-rw-r--r--   0        0        0     8315 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
+-rw-r--r--   0        0        0    10266 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
+-rw-r--r--   0        0        0     9628 2024-04-19 11:19:12.977684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
+-rw-r--r--   0        0        0    13173 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
+-rw-r--r--   0        0        0    12575 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
+-rw-r--r--   0        0        0    13309 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
+-rw-r--r--   0        0        0    12690 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
+-rw-r--r--   0        0        0    14474 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin
+-rw-r--r--   0        0        0    14004 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin
+-rw-r--r--   0        0        0     2739 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin
+-rw-r--r--   0        0        0     3108 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin
+-rw-r--r--   0        0        0     2449 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin
+-rw-r--r--   0        0        0     2636 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin
+-rw-r--r--   0        0        0     3086 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin
+-rw-r--r--   0        0        0     3518 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin
+-rw-r--r--   0        0        0     2634 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin
+-rw-r--r--   0        0        0     2831 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
+-rw-r--r--   0        0        0     2164 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
+-rw-r--r--   0        0        0     2217 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
+-rw-r--r--   0        0        0     2164 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin
+-rw-r--r--   0        0        0     2217 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin
+-rw-r--r--   0        0        0     1199 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
+-rw-r--r--   0        0        0     4993 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
+-rw-r--r--   0        0        0     7631 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
+-rw-r--r--   0        0        0     7396 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
+-rw-r--r--   0        0        0     8830 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
+-rw-r--r--   0        0        0     8293 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
+-rw-r--r--   0        0        0    11737 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
+-rw-r--r--   0        0        0    11240 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
+-rw-r--r--   0        0        0    11873 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
+-rw-r--r--   0        0        0    11355 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
+-rw-r--r--   0        0        0    12042 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin
+-rw-r--r--   0        0        0    11556 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin
+-rw-r--r--   0        0        0      307 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
+-rw-r--r--   0        0        0      477 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
+-rw-r--r--   0        0        0      860 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
+-rw-r--r--   0        0        0      859 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
+-rw-r--r--   0        0        0      860 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
+-rw-r--r--   0        0        0      859 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
+-rw-r--r--   0        0        0     1980 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
+-rw-r--r--   0        0        0     2049 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
+-rw-r--r--   0        0        0     2116 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
+-rw-r--r--   0        0        0     2164 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
+-rw-r--r--   0        0        0     2116 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin
+-rw-r--r--   0        0        0     2164 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin
+-rw-r--r--   0        0        0      395 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
+-rw-r--r--   0        0        0      572 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
+-rw-r--r--   0        0        0      952 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
+-rw-r--r--   0        0        0      961 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
+-rw-r--r--   0        0        0      952 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
+-rw-r--r--   0        0        0      961 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
+-rw-r--r--   0        0        0     2093 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
+-rw-r--r--   0        0        0     2168 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
+-rw-r--r--   0        0        0     2229 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
+-rw-r--r--   0        0        0     2283 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
+-rw-r--r--   0        0        0     2229 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin
+-rw-r--r--   0        0        0     2283 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
+-rw-r--r--   0        0        0     3848 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
+-rw-r--r--   0        0        0     3888 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
+-rw-r--r--   0        0        0     3984 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
+-rw-r--r--   0        0        0     4003 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
+-rw-r--r--   0        0        0     3984 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin
+-rw-r--r--   0        0        0     4003 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin
+-rw-r--r--   0        0        0     2164 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin
+-rw-r--r--   0        0        0     2217 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin
+-rw-r--r--   0        0        0     3918 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin
+-rw-r--r--   0        0        0     4052 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
+-rw-r--r--   0        0        0     5189 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
+-rw-r--r--   0        0        0     5704 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
+-rw-r--r--   0        0        0     5325 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
+-rw-r--r--   0        0        0     5819 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
+-rw-r--r--   0        0        0     5518 2024-04-19 11:19:12.981684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin
+-rw-r--r--   0        0        0     6044 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin
+-rw-r--r--   0        0        0      448 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
+-rw-r--r--   0        0        0     1056 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
+-rw-r--r--   0        0        0     1071 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
+-rw-r--r--   0        0        0     1243 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
+-rw-r--r--   0        0        0     1214 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
+-rw-r--r--   0        0        0     2384 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
+-rw-r--r--   0        0        0     2421 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
+-rw-r--r--   0        0        0     2520 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
+-rw-r--r--   0        0        0     2536 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
+-rw-r--r--   0        0        0     2520 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin
+-rw-r--r--   0        0        0     2536 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin
+-rw-r--r--   0        0        0      655 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
+-rw-r--r--   0        0        0      980 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
+-rw-r--r--   0        0        0     1582 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
+-rw-r--r--   0        0        0     1579 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
+-rw-r--r--   0        0        0     1769 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
+-rw-r--r--   0        0        0     1722 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
+-rw-r--r--   0        0        0     2889 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
+-rw-r--r--   0        0        0     2912 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
+-rw-r--r--   0        0        0     3025 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
+-rw-r--r--   0        0        0     3027 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
+-rw-r--r--   0        0        0     3025 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin
+-rw-r--r--   0        0        0     3027 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin
+-rw-r--r--   0        0        0      654 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
+-rw-r--r--   0        0        0     1045 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
+-rw-r--r--   0        0        0     1562 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
+-rw-r--r--   0        0        0     1749 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
+-rw-r--r--   0        0        0     2890 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
+-rw-r--r--   0        0        0     3026 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
+-rw-r--r--   0        0        0     3042 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
+-rw-r--r--   0        0        0     3026 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin
+-rw-r--r--   0        0        0     3042 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
+-rw-r--r--   0        0        0      431 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
+-rw-r--r--   0        0        0      629 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
+-rw-r--r--   0        0        0      666 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
+-rw-r--r--   0        0        0      792 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
+-rw-r--r--   0        0        0      797 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
+-rw-r--r--   0        0        0     1933 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
+-rw-r--r--   0        0        0     2004 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
+-rw-r--r--   0        0        0     2069 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
+-rw-r--r--   0        0        0     2119 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
+-rw-r--r--   0        0        0     2069 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin
+-rw-r--r--   0        0        0     2119 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin
+-rw-r--r--   0        0        0      516 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      966 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     2553 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     2362 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     2653 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     2453 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     3710 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     3592 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     3846 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     3707 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0     4016 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin
+-rw-r--r--   0        0        0     3817 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin
+-rw-r--r--   0        0        0      448 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
+-rw-r--r--   0        0        0     1575 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
+-rw-r--r--   0        0        0     1762 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
+-rw-r--r--   0        0        0     2903 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
+-rw-r--r--   0        0        0     3039 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
+-rw-r--r--   0        0        0     3042 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
+-rw-r--r--   0        0        0     3039 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin
+-rw-r--r--   0        0        0     3042 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin
+-rw-r--r--   0        0        0      245 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      459 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     1475 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     1382 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     1649 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     1533 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     2748 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     2706 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     2884 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     2821 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0     2884 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin
+-rw-r--r--   0        0        0     2821 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
+-rw-r--r--   0        0        0     3900 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
+-rw-r--r--   0        0        0     4021 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
+-rw-r--r--   0        0        0     4263 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
+-rw-r--r--   0        0        0     4295 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
+-rw-r--r--   0        0        0     7224 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
+-rw-r--r--   0        0        0     7288 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
+-rw-r--r--   0        0        0     7360 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
+-rw-r--r--   0        0        0     7403 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
+-rw-r--r--   0        0        0     7915 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin
+-rw-r--r--   0        0        0     8054 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
+-rw-r--r--   0        0        0     2106 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
+-rw-r--r--   0        0        0     2196 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
+-rw-r--r--   0        0        0     2469 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
+-rw-r--r--   0        0        0     2470 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
+-rw-r--r--   0        0        0     5430 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
+-rw-r--r--   0        0        0     5463 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
+-rw-r--r--   0        0        0     5566 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
+-rw-r--r--   0        0        0     5578 2024-04-19 11:19:12.985684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
+-rw-r--r--   0        0        0     5735 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin
+-rw-r--r--   0        0        0     5779 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
+-rw-r--r--   0        0        0     1030 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
+-rw-r--r--   0        0        0     1040 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
+-rw-r--r--   0        0        0     1030 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
+-rw-r--r--   0        0        0     1040 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
+-rw-r--r--   0        0        0     2171 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
+-rw-r--r--   0        0        0     2247 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
+-rw-r--r--   0        0        0     2307 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
+-rw-r--r--   0        0        0     2362 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
+-rw-r--r--   0        0        0     2307 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin
+-rw-r--r--   0        0        0     2362 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin
+-rw-r--r--   0        0        0     2957 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_component.py
+-rw-r--r--   0        0        0     3283 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_deserialize_json.py
+-rw-r--r--   0        0        0     1764 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_deserialize_xml.py
+-rw-r--r--   0        0        0    19038 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_enums.py
+-rw-r--r--   0        0        0     4389 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_factory_license.py
+-rw-r--r--   0        0        0    22602 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model.py
+-rw-r--r--   0        0        0    13254 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_bom.py
+-rw-r--r--   0        0        0     2782 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_bom_ref.py
+-rw-r--r--   0        0        0    18544 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_component.py
+-rw-r--r--   0        0        0     1793 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_dependency.py
+-rw-r--r--   0        0        0     4064 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_issue.py
+-rw-r--r--   0        0        0     4295 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_license.py
+-rw-r--r--   0        0        0     2758 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_release_note.py
+-rw-r--r--   0        0        0     3390 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_service.py
+-rw-r--r--   0        0        0    14370 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_model_vulnerability.py
+-rw-r--r--   0        0        0     3154 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_output.py
+-rw-r--r--   0        0        0     4587 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_output_json.py
+-rw-r--r--   0        0        0     4029 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_output_xml.py
+-rw-r--r--   0        0        0     1307 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_real_world_examples.py
+-rw-r--r--   0        0        0     2509 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_schema_SchemaVersion.py
+-rw-r--r--   0        0        0     1248 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_schema__res.py
+-rw-r--r--   0        0        0     2873 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_spdx.py
+-rw-r--r--   0        0        0     1977 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_validation.py
+-rw-r--r--   0        0        0     4547 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_validation_json.py
+-rw-r--r--   0        0        0     3079 2024-04-19 11:19:12.989684 cyclonedx_python_lib-7.2.0/tests/test_validation_xml.py
+-rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 cyclonedx_python_lib-7.2.0/PKG-INFO
```

### Comparing `cyclonedx_python_lib-7.1.0/CHANGELOG.md` & `cyclonedx_python_lib-7.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v7.1.0 (2024-04-10)
+
+### Documentation
+
+* docs: missing schema support table &amp; update schema support to reflect version 7.0.0 (#584)
+
+Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`d230e67`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/d230e67188661a5fb94730e52bf59c11c965c8d7))
+
+### Feature
+
+* feat: support `bom.properties` for CycloneDX v1.5+ (#585)
+
+Signed-off-by: Paul Horton &lt;paul.horton@owasp.org&gt; ([`1d1c45a`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/1d1c45ac82c7927acc388489228a9b5990f68aa7))
+
+
 ## v7.0.0 (2024-04-09)
 
 ### Breaking
 
 * feat!: Support for CycloneDX v1.6
 
 * added draft v1.6 schemas and boilerplate for v1.6
```

### Comparing `cyclonedx_python_lib-7.1.0/LICENSE` & `cyclonedx_python_lib-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/README.md` & `cyclonedx_python_lib-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 """
 Python library for CycloneDX
 """
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "7.1.0"  # noqa:Q000
+__version__ = "7.2.0"  # noqa:Q000
```

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/_internal/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/_internal/compare.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/_internal/compare.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/_internal/hash.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/_internal/hash.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/_internal/time.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/_internal/time.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/exception/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/exception/factory.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/exception/factory.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/exception/model.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/exception/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/exception/output.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/exception/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/exception/serialization.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/exception/serialization.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/factory/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/factory/license.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/factory/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/bom.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/bom_ref.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/component.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/contact.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/contact.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/crypto.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/crypto.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/dependency.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/impact_analysis.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/impact_analysis.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/issue.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/license.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/license.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,37 +29,66 @@
 
 from .._internal.compare import ComparableTuple as _ComparableTuple
 from ..exception.model import MutuallyExclusivePropertiesException
 from ..schema.schema import SchemaVersion1Dot6
 from . import AttachedText, XsUri
 
 
+@serializable.serializable_enum
+class LicenseAcknowledgement(str, Enum):
+    """
+    This is our internal representation of the `type_licenseAcknowledgementEnumerationType` ENUM type
+    within the CycloneDX standard.
+
+    .. note::
+        Introduced in CycloneDX v1.6
+
+    .. note::
+        See the CycloneDX Schema for hashType:
+        https://cyclonedx.org/docs/1.6/#type_licenseAcknowledgementEnumerationType
+    """
+
+    CONCLUDED = 'concluded'
+    DECLARED = 'declared'
+
+
+# In an error, the name of the enum was `LicenseExpressionAcknowledgement`.
+# Even though this was changed, there might be some downstream usage of this symbol, so we keep it around ...
+LicenseExpressionAcknowledgement = LicenseAcknowledgement
+"""Deprecated alias for :class:`LicenseAcknowledgement`"""
+
+
 @serializable.serializable_class(name='license')
 class DisjunctiveLicense:
     """
     This is our internal representation of `licenseType` complex type that can be used in multiple places within
     a CycloneDX BOM document.
 
     .. note::
         See the CycloneDX Schema definition: https://cyclonedx.org/docs/1.4/json/#components_items_licenses
     """
 
-    def __init__(self, *, id: Optional[str] = None, name: Optional[str] = None,
-                 text: Optional[AttachedText] = None, url: Optional[XsUri] = None) -> None:
+    def __init__(
+        self, *,
+        id: Optional[str] = None, name: Optional[str] = None,
+        text: Optional[AttachedText] = None, url: Optional[XsUri] = None,
+        acknowledgement: Optional[LicenseAcknowledgement] = None
+    ) -> None:
         if not id and not name:
             raise MutuallyExclusivePropertiesException('Either `id` or `name` MUST be supplied')
         if id and name:
             warn(
                 'Both `id` and `name` have been supplied - `name` will be ignored!',
                 category=RuntimeWarning, stacklevel=1
             )
         self._id = id
         self._name = name if not id else None
         self._text = text
         self._url = url
+        self._acknowledgement = acknowledgement
 
     @property
     @serializable.xml_sequence(1)
     def id(self) -> Optional[str]:
         """
         A SPDX license ID.
 
@@ -125,22 +154,70 @@
     @url.setter
     def url(self, url: Optional[XsUri]) -> None:
         self._url = url
 
     # @property
     # ...
     # @serializable.view(SchemaVersion1Dot5)
-    # @serializable.xml_sequence(4)
+    # @serializable.view(SchemaVersion1Dot6)
+    # @serializable.xml_sequence(5)
     # def licensing(self) -> ...:
     #     ...  # TODO since CDX1.5
     #
     # @licensing.setter
     # def licensing(self, ...) -> None:
     #     ...  # TODO since CDX1.5
 
+    # @property
+    # ...
+    # @serializable.view(SchemaVersion1Dot5)
+    # @serializable.view(SchemaVersion1Dot6)
+    # @serializable.xml_sequence(6)
+    # def properties(self) -> ...:
+    #     ...  # TODO since CDX1.5
+    #
+    # @licensing.setter
+    # def properties(self, ...) -> None:
+    #     ...  # TODO since CDX1.5
+
+    # @property
+    # @serializable.json_name('bom-ref')
+    # @serializable.type_mapping(BomRefHelper)
+    # @serializable.view(SchemaVersion1Dot5)
+    # @serializable.view(SchemaVersion1Dot6)
+    # @serializable.xml_attribute()
+    # @serializable.xml_name('bom-ref')
+    # def bom_ref(self) -> BomRef:
+    #     ...  # TODO since CDX1.5
+
+    @property
+    @serializable.view(SchemaVersion1Dot6)
+    @serializable.xml_attribute()
+    def acknowledgement(self) -> Optional[LicenseAcknowledgement]:
+        """
+        Declared licenses and concluded licenses represent two different stages in the licensing process within
+        software development.
+
+        Declared licenses refer to the initial intention of the software authors regarding the
+        licensing terms under which their code is released. On the other hand, concluded licenses are the result of a
+        comprehensive analysis of the project's codebase to identify and confirm the actual licenses of the components
+        used, which may differ from the initially declared licenses. While declared licenses provide an upfront
+        indication of the licensing intentions, concluded licenses offer a more thorough understanding of the actual
+        licensing within a project, facilitating proper compliance and risk management. Observed licenses are defined
+        in evidence.licenses. Observed licenses form the evidence necessary to substantiate a concluded license.
+
+        Returns:
+            `LicenseAcknowledgement` or `None`
+        """
+        return self._acknowledgement
+
+    @acknowledgement.setter
+    def acknowledgement(self, acknowledgement: Optional[LicenseAcknowledgement]) -> None:
+        self._acknowledgement = acknowledgement
+
     def __eq__(self, other: object) -> bool:
         if isinstance(other, DisjunctiveLicense):
             return hash(other) == hash(self)
         return False
 
     def __lt__(self, other: Any) -> bool:
         if isinstance(other, DisjunctiveLicense):
@@ -150,101 +227,95 @@
                 other._id, other._name
             ))
         if isinstance(other, LicenseExpression):
             return False  # self after any LicenseExpression
         return NotImplemented
 
     def __hash__(self) -> int:
-        return hash((self._id, self._name, self._text, self._url))
+        return hash((self._id, self._name, self._text, self._url, self._acknowledgement))
 
     def __repr__(self) -> str:
         return f'<License id={self._id!r}, name={self._name!r}>'
 
 
-@serializable.serializable_enum
-class LicenseExpressionAcknowledgement(str, Enum):
-    """
-    This is our internal representation of the `type_licenseAcknowledgementEnumerationType` ENUM type
-    within the CycloneDX standard.
-
-    .. note::
-        Introduced in CycloneDX v1.6
-
-    .. note::
-        See the CycloneDX Schema for hashType:
-        https://cyclonedx.org/docs/1.6/#type_licenseAcknowledgementEnumerationType
-    """
-
-    CONCLUDED = 'concluded'
-    DECLARED = 'declared'
-
-
 @serializable.serializable_class(name='expression')
 class LicenseExpression:
     """
     This is our internal representation of `licenseType`'s  expression type that can be used in multiple places within
     a CycloneDX BOM document.
 
     .. note::
         See the CycloneDX Schema definition:
         https://cyclonedx.org/docs/1.4/json/#components_items_licenses_items_expression
     """
 
-    def __init__(self, value: str,
-                 acknowledgement: Optional[LicenseExpressionAcknowledgement] = None) -> None:
+    def __init__(
+        self, value: str,
+        acknowledgement: Optional[LicenseAcknowledgement] = None
+    ) -> None:
+        self._value = value
+        self._acknowledgement = acknowledgement
+
+    @property
+    @serializable.xml_name('.')
+    @serializable.json_name('expression')
+    def value(self) -> str:
+        """
+        Value of this LicenseExpression.
+
+        Returns:
+             `str`
+        """
+        return self._value
+
+    @value.setter
+    def value(self, value: str) -> None:
         self._value = value
-        self.acknowledgement = acknowledgement
+
+    # @property
+    # @serializable.json_name('bom-ref')
+    # @serializable.type_mapping(BomRefHelper)
+    # @serializable.view(SchemaVersion1Dot5)
+    # @serializable.view(SchemaVersion1Dot6)
+    # @serializable.xml_attribute()
+    # @serializable.xml_name('bom-ref')
+    # def bom_ref(self) -> BomRef:
+    #     ...  # TODO since CDX1.5
 
     @property
     @serializable.view(SchemaVersion1Dot6)
     @serializable.xml_attribute()
-    def acknowledgement(self) -> Optional[LicenseExpressionAcknowledgement]:
+    def acknowledgement(self) -> Optional[LicenseAcknowledgement]:
         """
         Declared licenses and concluded licenses represent two different stages in the licensing process within
         software development.
 
         Declared licenses refer to the initial intention of the software authors regarding the
         licensing terms under which their code is released. On the other hand, concluded licenses are the result of a
         comprehensive analysis of the project's codebase to identify and confirm the actual licenses of the components
         used, which may differ from the initially declared licenses. While declared licenses provide an upfront
         indication of the licensing intentions, concluded licenses offer a more thorough understanding of the actual
         licensing within a project, facilitating proper compliance and risk management. Observed licenses are defined
         in evidence.licenses. Observed licenses form the evidence necessary to substantiate a concluded license.
 
         Returns:
-            `LicenseExpressionAcknowledgement` or `None`
+            `LicenseAcknowledgement` or `None`
         """
         return self._acknowledgement
 
     @acknowledgement.setter
-    def acknowledgement(self, acknowledgement: Optional[LicenseExpressionAcknowledgement]) -> None:
+    def acknowledgement(self, acknowledgement: Optional[LicenseAcknowledgement]) -> None:
         self._acknowledgement = acknowledgement
 
-    @property
-    @serializable.xml_name('.')
-    @serializable.json_name('expression')
-    def value(self) -> str:
-        """
-        Value of this LicenseExpression.
-
-        Returns:
-             `str`
-        """
-        return self._value
-
-    @value.setter
-    def value(self, value: str) -> None:
-        self._value = value
-
     def __hash__(self) -> int:
-        return hash(self._value)
+        return hash((self._value, self._acknowledgement))
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, LicenseExpression):
-            return self._value == other._value
+            return hash(other) == hash(self)
         return False
 
     def __lt__(self, other: Any) -> bool:
         if isinstance(other, LicenseExpression):
             return self._value < other._value
         if isinstance(other, DisjunctiveLicense):
             return True  # self before any DisjunctiveLicense
```

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/release_note.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/service.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/model/vulnerability.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/model/vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/output/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/output/json.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/output/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/output/xml.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/output/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/README.md` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/schema/schema.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/serialization/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/spdx.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/validation/__init__.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/validation/json.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/validation/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/validation/model.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/validation/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/cyclonedx/validation/xml.py` & `cyclonedx_python_lib-7.2.0/cyclonedx/validation/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/Makefile` & `cyclonedx_python_lib-7.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/architecture.rst` & `cyclonedx_python_lib-7.2.0/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/changelog.rst` & `cyclonedx_python_lib-7.2.0/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/conf.py` & `cyclonedx_python_lib-7.2.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 project = 'CycloneDX Python Library'
 copyright = '2022, Copyright (c) OWASP Foundation'
 author = 'Paul Horton, Jan Kowalleck, Steve Springett, Patrick Dwyer'
 
 # The full version, including alpha/beta/rc tags
 # !! version is managed by semantic_release
-release = '7.1.0'
+release = '7.2.0'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `cyclonedx_python_lib-7.1.0/docs/examples.rst` & `cyclonedx_python_lib-7.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/index.rst` & `cyclonedx_python_lib-7.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/install.rst` & `cyclonedx_python_lib-7.2.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/make.bat` & `cyclonedx_python_lib-7.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/modelling.rst` & `cyclonedx_python_lib-7.2.0/docs/modelling.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/outputting.rst` & `cyclonedx_python_lib-7.2.0/docs/outputting.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/docs/schema-support.rst` & `cyclonedx_python_lib-7.2.0/docs/schema-support.rst`

 * *Files 24% similar despite different names*

```diff
@@ -17,24 +17,27 @@
 
 This library has partial support for the CycloneDX specification (we continue to grow support).
 
 The following sub-sections aim to explain what support this library provides and any known gaps in support. We do this
 by calling out support for data as defined in the latest CycloneDX standard specification, regardless of whether it is
 supported in prior versions of the CycloneDX schema.
 
+Root Level Schema Support
+-------------------------
+
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | Data Path                  | Supported?    | Notes                                                                                             |
 +============================+===============+===================================================================================================+
 | ``bom[@version]``          | Yes           |                                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | ``bom[@serialNumber]``     | Yes           |                                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
-| ``bom.metadata``           | Yes           |                                                                                                   |
+| ``bom.metadata``           | Yes           | Not supported: ``lifecycles``                                                                     |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
-| ``bom.components``         | Yes           | Not supported: ``modified`` (as it is deprecated), ``signature``.                                 |
+| ``bom.components``         | Yes           | Not supported: ``modified`` (as it is deprecated), ``modelCard``, ``data``, ``signature``.        |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | ``bom.services``           | Yes           | Not supported: ``signature``.                                                                     |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | ``bom.externalReferences`` | Yes           |                                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | ``bom.dependencies``       | Yes           | Since ``2.3.0``                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
@@ -52,9 +55,26 @@
 | ``bom.declarations``       | No            |                                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | ``bom.definitions``        | No            |                                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 | ``bom.signature``          | No            |                                                                                                   |
 +----------------------------+---------------+---------------------------------------------------------------------------------------------------+
 
+Internal Model Schema Support
+-----------------------------
+
++----------------------------+---------------+----------------------------------------------------------------------------------------------+
+| Internal Model             | Supported?    | Notes                                                                                        |
++============================+===============+==============================================================================================+
+| ``ComponentEvidence``      |Yes            | Not currently supported: ``callstack``, ``identity``, ``occurrences``.                       |
++----------------------------+---------------+----------------------------------------------------------------------------------------------+
+| ``DisjunctiveLicense``     |Yes            | Not currently supported: ``@bom-ref``, ``licensing``, ``properties``.                        |
++----------------------------+---------------+----------------------------------------------------------------------------------------------+
+| ``LicenseExpression``      |Yes            | Not currently supported: ``@bom-ref``                                                        |
++----------------------------+---------------+----------------------------------------------------------------------------------------------+
+| ``OrganizationalContact``  |Yes            | Not currently supported: ``@bom-ref``                                                        |
++----------------------------+---------------+----------------------------------------------------------------------------------------------+
+| ``OrganizationalEntity``   |Yes            | Not currently supported: ``@bom-ref``                                                        |
++----------------------------+---------------+----------------------------------------------------------------------------------------------+
 
 .. _schema specification bug 130: https://github.com/CycloneDX/specification/issues/130
+
```

### Comparing `cyclonedx_python_lib-7.1.0/docs/support.rst` & `cyclonedx_python_lib-7.2.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/examples/complex_deserialize.py` & `cyclonedx_python_lib-7.2.0/examples/complex_deserialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/examples/complex_serialize.py` & `cyclonedx_python_lib-7.2.0/examples/complex_serialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/pyproject.toml` & `cyclonedx_python_lib-7.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cyclonedx-python-lib"
 # !! version is managed by semantic_release
-version = "7.1.0"
+version = "7.2.0"
 description = "Python library for CycloneDX"
 authors = [
   "Paul Horton <phorton@sonatype.com>",
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
 ]
 maintainers = [
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/__init__.py` & `cyclonedx_python_lib-7.2.0/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright (c) OWASP Foundation. All Rights Reserved.
 import re
 from os import getenv, path
-from os.path import join
-from typing import TYPE_CHECKING, Any, Generator, Iterable, List, Optional, TypeVar, Union
+from os.path import basename, join, splitext
+from typing import TYPE_CHECKING, Any, Generator, Iterable, List, Optional, Tuple, TypeVar, Union
 from unittest import TestCase
 from uuid import UUID
 
 from sortedcontainers import SortedSet
 
 from cyclonedx.output import BomRefDiscriminator as _BomRefDiscriminator
 from cyclonedx.schema import OutputFormat, SchemaVersion
@@ -179,7 +179,14 @@
                 return False
 
     return True
 
 
 def mksname(purpose: Union[Any], sv: SchemaVersion, f: OutputFormat) -> str:
     return f'{_get_purpose_as_str(purpose)}-{sv.to_version()}.{_SNAME_EXT[f]}'
+
+
+class DpTuple(Tuple[SchemaVersion, str]):
+    @property
+    def __name__(self) -> str:
+        schema_version, test_data_file = self
+        return f'{schema_version.to_version()}-{splitext(basename(test_data_file))[0]}'
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/__init__.py` & `cyclonedx_python_lib-7.2.0/tests/_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/models.py` & `cyclonedx_python_lib-7.2.0/tests/_data/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 from cyclonedx.model.impact_analysis import (
     ImpactAnalysisAffectedStatus,
     ImpactAnalysisJustification,
     ImpactAnalysisResponse,
     ImpactAnalysisState,
 )
 from cyclonedx.model.issue import IssueClassification, IssueType, IssueTypeSource
-from cyclonedx.model.license import DisjunctiveLicense, License, LicenseExpression, LicenseExpressionAcknowledgement
+from cyclonedx.model.license import DisjunctiveLicense, License, LicenseAcknowledgement, LicenseExpression
 from cyclonedx.model.release_note import ReleaseNotes
 from cyclonedx.model.service import Service
 from cyclonedx.model.vulnerability import (
     BomTarget,
     BomTargetVersionRange,
     Vulnerability,
     VulnerabilityAdvisory,
@@ -944,28 +944,34 @@
             licenses=[DisjunctiveLicense(id='CC-BY-1.0')],
             component=Component(name='app', type=ComponentType.APPLICATION, bom_ref='my-app',
                                 licenses=[DisjunctiveLicense(name='proprietary')])
         ),
         components=[
             Component(name='c-with-expression', type=ComponentType.LIBRARY, bom_ref='C1',
                       licenses=[LicenseExpression(value='Apache-2.0 OR MIT',
-                                                  acknowledgement=LicenseExpressionAcknowledgement.CONCLUDED)]),
+                                                  acknowledgement=LicenseAcknowledgement.CONCLUDED)]),
             Component(name='c-with-SPDX', type=ComponentType.LIBRARY, bom_ref='C2',
-                      licenses=[DisjunctiveLicense(id='Apache-2.0')]),
+                      licenses=[DisjunctiveLicense(id='Apache-2.0',
+                                                   url=XsUri('https://www.apache.org/licenses/LICENSE-2.0.html'),
+                                                   acknowledgement=LicenseAcknowledgement.CONCLUDED)]),
             Component(name='c-with-name', type=ComponentType.LIBRARY, bom_ref='C3',
-                      licenses=[DisjunctiveLicense(name='(c) ACME Inc.')]),
+                      licenses=[DisjunctiveLicense(name='some commercial license',
+                                                   text=AttachedText(content='this is a license text'))]),
         ],
         services=[
             Service(name='s-with-expression', bom_ref='S1',
                     licenses=[LicenseExpression(value='Apache-2.0 OR MIT',
-                                                acknowledgement=LicenseExpressionAcknowledgement.DECLARED)]),
+                                                acknowledgement=LicenseAcknowledgement.DECLARED)]),
             Service(name='s-with-SPDX', bom_ref='S2',
-                    licenses=[DisjunctiveLicense(id='Apache-2.0')]),
+                    licenses=[DisjunctiveLicense(id='Apache-2.0',
+                                                 url=XsUri('https://www.apache.org/licenses/LICENSE-2.0.html'),
+                                                 acknowledgement=LicenseAcknowledgement.DECLARED)]),
             Service(name='s-with-name', bom_ref='S3',
-                    licenses=[DisjunctiveLicense(name='(c) ACME Inc.')]),
+                    licenses=[DisjunctiveLicense(name='some commercial license',
+                                                 text=AttachedText(content='this is a license text'))]),
         ])
 
 
 def get_bom_metadata_licenses_invalid() -> Bom:
     return Bom(metadata=BomMetaData(licenses=get_invalid_license_repository()))
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.2.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.2.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.2.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/own/xml/1.4/bom_setuptools.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/own/xml/1.4/bom_setuptools.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/own/xml/1.4/webgoat-6.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/own/xml/1.4/webgoat-6.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/schemaTestData/fetch.sh` & `cyclonedx_python_lib-7.2.0/tests/_data/schemaTestData/fetch.sh`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin`

 * *Files 16% similar despite different names*

#### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin`

```diff
@@ -3,14 +3,15 @@
   <components>
     <component type="library" bom-ref="C2">
       <name>c-with-SPDX</name>
       <version/>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </component>
     <component type="library" bom-ref="C1">
       <name>c-with-expression</name>
       <version/>
       <licenses>
@@ -18,13 +19,14 @@
       </licenses>
     </component>
     <component type="library" bom-ref="C3">
       <name>c-with-name</name>
       <version/>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </component>
   </components>
 </bom>
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969135802469135%*

 * *Differences: {"'components'": "{0: {'licenses': {0: {'license': {'url': "*

 * *                 "'https://www.apache.org/licenses/LICENSE-2.0.html'}}}}, 2: {'licenses': {0: "*

 * *                 "{'license': {'name': 'some commercial license', 'text': OrderedDict([('content', "*

 * *                 "'this is a license text'), ('contentType', 'text/plain')])}}}}}",*

 * * "'services'": "{0: {'licenses': {0: {'license': {'url': "*

 * *               "'https://www.apache.org/licenses/LICENSE-2.0.html'}}}}, 2: {'licenses': {0: "*

 * *               "{ […]*

```diff
@@ -3,15 +3,16 @@
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "C2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "c-with-SPDX",
             "type": "library",
             "version": ""
         },
@@ -27,15 +28,19 @@
             "version": ""
         },
         {
             "bom-ref": "C3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "c-with-name",
             "type": "library",
             "version": ""
         }
@@ -89,15 +94,16 @@
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
     "services": [
         {
             "bom-ref": "S2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "s-with-SPDX"
         },
         {
             "bom-ref": "S1",
@@ -109,15 +115,19 @@
             "name": "s-with-expression"
         },
         {
             "bom-ref": "S3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "s-with-name"
         }
     ],
     "specVersion": "1.2",
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin`

 * *Files 7% similar despite different names*

#### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin`

```diff
@@ -22,14 +22,15 @@
   <components>
     <component type="library" bom-ref="C2">
       <name>c-with-SPDX</name>
       <version/>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </component>
     <component type="library" bom-ref="C1">
       <name>c-with-expression</name>
       <version/>
       <licenses>
@@ -37,39 +38,42 @@
       </licenses>
     </component>
     <component type="library" bom-ref="C3">
       <name>c-with-name</name>
       <version/>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </component>
   </components>
   <services>
     <service bom-ref="S2">
       <name>s-with-SPDX</name>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </service>
     <service bom-ref="S1">
       <name>s-with-expression</name>
       <licenses>
         <expression>Apache-2.0 OR MIT</expression>
       </licenses>
     </service>
     <service bom-ref="S3">
       <name>s-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </service>
   </services>
   <dependencies>
     <dependency ref="C1"/>
     <dependency ref="C2"/>
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6585648148148148%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.4.schema.json'",*

 * * "'components'": "{0: {'bom-ref': 'pkg:pypi/toml@0.10.2?extension=tar.gz', 'name': 'toml', "*

 * *                 "'version': '0.10.2', 'externalReferences': [OrderedDict([('comment', 'No "*

 * *                 "comment'), ('hashes', [OrderedDict([('alg', 'SHA-256'), ('content', "*

 * *                 "'806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b')])]), "*

 * *                 "('type', 'distribution'), ('url', 'https://cyclonedx.org')]) […]*

```diff
@@ -1,132 +1,105 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.3a.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.4.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
-            "bom-ref": "C2",
-            "licenses": [
-                {
-                    "license": {
-                        "id": "Apache-2.0"
-                    }
-                }
-            ],
-            "name": "c-with-SPDX",
-            "type": "library",
-            "version": ""
-        },
-        {
-            "bom-ref": "C1",
-            "licenses": [
+            "bom-ref": "pkg:pypi/toml@0.10.2?extension=tar.gz",
+            "externalReferences": [
                 {
-                    "expression": "Apache-2.0 OR MIT"
+                    "comment": "No comment",
+                    "hashes": [
+                        {
+                            "alg": "SHA-256",
+                            "content": "806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"
+                        }
+                    ],
+                    "type": "distribution",
+                    "url": "https://cyclonedx.org"
                 }
             ],
-            "name": "c-with-expression",
-            "type": "library",
-            "version": ""
-        },
-        {
-            "bom-ref": "C3",
-            "licenses": [
+            "hashes": [
                 {
-                    "license": {
-                        "name": "(c) ACME Inc."
-                    }
+                    "alg": "SHA-256",
+                    "content": "806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"
                 }
             ],
-            "name": "c-with-name",
+            "name": "toml",
+            "purl": "pkg:pypi/toml@0.10.2?extension=tar.gz",
             "type": "library",
-            "version": ""
+            "version": "0.10.2"
         }
     ],
     "dependencies": [
         {
-            "ref": "C1"
-        },
-        {
-            "ref": "C2"
-        },
-        {
-            "ref": "C3"
-        },
-        {
-            "ref": "S1"
-        },
-        {
-            "ref": "S2"
-        },
-        {
-            "ref": "S3"
+            "dependsOn": [
+                "pkg:pypi/toml@0.10.2?extension=tar.gz"
+            ],
+            "ref": "pkg:pypi/setuptools@50.3.2?extension=tar.gz"
         },
         {
-            "ref": "my-app"
+            "ref": "pkg:pypi/toml@0.10.2?extension=tar.gz"
         }
     ],
     "metadata": {
         "component": {
-            "bom-ref": "my-app",
+            "author": "Test Author",
+            "bom-ref": "pkg:pypi/setuptools@50.3.2?extension=tar.gz",
             "licenses": [
                 {
                     "license": {
-                        "name": "proprietary"
+                        "id": "MIT"
                     }
                 }
             ],
-            "name": "app",
-            "type": "application",
-            "version": ""
+            "name": "setuptools",
+            "purl": "pkg:pypi/setuptools@50.3.2?extension=tar.gz",
+            "type": "library",
+            "version": "50.3.2"
         },
-        "licenses": [
-            {
-                "license": {
-                    "id": "CC-BY-1.0"
-                }
-            }
-        ],
         "timestamp": "2023-01-07T13:44:32.312678+00:00",
         "tools": [
             {
+                "externalReferences": [
+                    {
+                        "type": "build-system",
+                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/actions"
+                    },
+                    {
+                        "type": "distribution",
+                        "url": "https://pypi.org/project/cyclonedx-python-lib/"
+                    },
+                    {
+                        "type": "documentation",
+                        "url": "https://cyclonedx-python-library.readthedocs.io/"
+                    },
+                    {
+                        "type": "issue-tracker",
+                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/issues"
+                    },
+                    {
+                        "type": "license",
+                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/blob/main/LICENSE"
+                    },
+                    {
+                        "type": "release-notes",
+                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/blob/main/CHANGELOG.md"
+                    },
+                    {
+                        "type": "vcs",
+                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib"
+                    },
+                    {
+                        "type": "website",
+                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/#readme"
+                    }
+                ],
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "services": [
-        {
-            "bom-ref": "S2",
-            "licenses": [
-                {
-                    "license": {
-                        "id": "Apache-2.0"
-                    }
-                }
-            ],
-            "name": "s-with-SPDX"
-        },
-        {
-            "bom-ref": "S1",
-            "licenses": [
-                {
-                    "expression": "Apache-2.0 OR MIT"
-                }
-            ],
-            "name": "s-with-expression"
-        },
-        {
-            "bom-ref": "S3",
-            "licenses": [
-                {
-                    "license": {
-                        "name": "(c) ACME Inc."
-                    }
-                }
-            ],
-            "name": "s-with-name"
-        }
-    ],
-    "specVersion": "1.3",
+    "specVersion": "1.4",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8715663580246914%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.3a.schema.json'",*

 * * "'components'": "{0: {'licenses': {0: {'license': {'url': "*

 * *                 "'https://www.apache.org/licenses/LICENSE-2.0.html'}}}, 'version': ''}, 1: "*

 * *                 "{'version': ''}, 2: {'licenses': {0: {'license': {'name': 'some commercial "*

 * *                 "license', 'text': OrderedDict([('content', 'this is a license text'), "*

 * *                 "('contentType', 'text/plain')])}}}, 'version': ''}}",*

 * * "'metadata'": "{'component': {' […]*

```diff
@@ -1,44 +1,52 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.4.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.3a.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "C2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "c-with-SPDX",
-            "type": "library"
+            "type": "library",
+            "version": ""
         },
         {
             "bom-ref": "C1",
             "licenses": [
                 {
                     "expression": "Apache-2.0 OR MIT"
                 }
             ],
             "name": "c-with-expression",
-            "type": "library"
+            "type": "library",
+            "version": ""
         },
         {
             "bom-ref": "C3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "c-with-name",
-            "type": "library"
+            "type": "library",
+            "version": ""
         }
     ],
     "dependencies": [
         {
             "ref": "C1"
         },
         {
@@ -67,74 +75,42 @@
                 {
                     "license": {
                         "name": "proprietary"
                     }
                 }
             ],
             "name": "app",
-            "type": "application"
+            "type": "application",
+            "version": ""
         },
         "licenses": [
             {
                 "license": {
                     "id": "CC-BY-1.0"
                 }
             }
         ],
         "timestamp": "2023-01-07T13:44:32.312678+00:00",
         "tools": [
             {
-                "externalReferences": [
-                    {
-                        "type": "build-system",
-                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/actions"
-                    },
-                    {
-                        "type": "distribution",
-                        "url": "https://pypi.org/project/cyclonedx-python-lib/"
-                    },
-                    {
-                        "type": "documentation",
-                        "url": "https://cyclonedx-python-library.readthedocs.io/"
-                    },
-                    {
-                        "type": "issue-tracker",
-                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/issues"
-                    },
-                    {
-                        "type": "license",
-                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/blob/main/LICENSE"
-                    },
-                    {
-                        "type": "release-notes",
-                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/blob/main/CHANGELOG.md"
-                    },
-                    {
-                        "type": "vcs",
-                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib"
-                    },
-                    {
-                        "type": "website",
-                        "url": "https://github.com/CycloneDX/cyclonedx-python-lib/#readme"
-                    }
-                ],
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
     "services": [
         {
             "bom-ref": "S2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "s-with-SPDX"
         },
         {
             "bom-ref": "S1",
@@ -146,17 +122,21 @@
             "name": "s-with-expression"
         },
         {
             "bom-ref": "S3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "s-with-name"
         }
     ],
-    "specVersion": "1.4",
+    "specVersion": "1.3",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin`

 * *Files 6% similar despite different names*

#### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin`

```diff
@@ -51,52 +51,56 @@
   </metadata>
   <components>
     <component type="library" bom-ref="C2">
       <name>c-with-SPDX</name>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </component>
     <component type="library" bom-ref="C1">
       <name>c-with-expression</name>
       <licenses>
         <expression>Apache-2.0 OR MIT</expression>
       </licenses>
     </component>
     <component type="library" bom-ref="C3">
       <name>c-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </component>
   </components>
   <services>
     <service bom-ref="S2">
       <name>s-with-SPDX</name>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </service>
     <service bom-ref="S1">
       <name>s-with-expression</name>
       <licenses>
         <expression>Apache-2.0 OR MIT</expression>
       </licenses>
     </service>
     <service bom-ref="S3">
       <name>s-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </service>
   </services>
   <dependencies>
     <dependency ref="C1"/>
     <dependency ref="C2"/>
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7969618055555555%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.4.schema.json'",*

 * * "'components'": "{0: {'licenses': {0: {'license': {'url': "*

 * *                 "'https://www.apache.org/licenses/LICENSE-2.0.html'}}}}, 2: {'licenses': {0: "*

 * *                 "{'license': {'name': 'some commercial license', 'text': OrderedDict([('content', "*

 * *                 "'this is a license text'), ('contentType', 'text/plain')])}}}}}",*

 * * "'services'": "{0: {'licenses': {0: {'license': {'url': "*

 * *               "'https://www.apache.org/lice […]*

```diff
@@ -1,17 +1,18 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.4.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "C2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "c-with-SPDX",
             "type": "library"
         },
         {
@@ -25,15 +26,19 @@
             "type": "library"
         },
         {
             "bom-ref": "C3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "c-with-name",
             "type": "library"
         }
     ],
@@ -119,32 +124,23 @@
                 ],
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
-    "properties": [
-        {
-            "name": "key1",
-            "value": "val1"
-        },
-        {
-            "name": "key2",
-            "value": "val2"
-        }
-    ],
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
     "services": [
         {
             "bom-ref": "S2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "s-with-SPDX"
         },
         {
             "bom-ref": "S1",
@@ -156,17 +152,21 @@
             "name": "s-with-expression"
         },
         {
             "bom-ref": "S3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "s-with-name"
         }
     ],
-    "specVersion": "1.5",
+    "specVersion": "1.4",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin`

 * *Files 4% similar despite different names*

#### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin`

```diff
@@ -51,52 +51,56 @@
   </metadata>
   <components>
     <component type="library" bom-ref="C2">
       <name>c-with-SPDX</name>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </component>
     <component type="library" bom-ref="C1">
       <name>c-with-expression</name>
       <licenses>
         <expression>Apache-2.0 OR MIT</expression>
       </licenses>
     </component>
     <component type="library" bom-ref="C3">
       <name>c-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </component>
   </components>
   <services>
     <service bom-ref="S2">
       <name>s-with-SPDX</name>
       <licenses>
         <license>
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </service>
     <service bom-ref="S1">
       <name>s-with-expression</name>
       <licenses>
         <expression>Apache-2.0 OR MIT</expression>
       </licenses>
     </service>
     <service bom-ref="S3">
       <name>s-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </service>
   </services>
   <dependencies>
     <dependency ref="C1"/>
     <dependency ref="C2"/>
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.89453125%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.5.schema.json'",*

 * * "'components'": "{0: {'licenses': {0: {'license': {'url': "*

 * *                 "'https://www.apache.org/licenses/LICENSE-2.0.html'}}}}, 1: {'licenses': {0: "*

 * *                 "{delete: ['acknowledgement']}}}, 2: {'licenses': {0: {'license': {'name': 'some "*

 * *                 "commercial license', 'text': OrderedDict([('content', 'this is a license text'), "*

 * *                 "('contentType', 'text/plain')])}}}}}",*

 * * "'services'": "{0: {'licenses […]*

```diff
@@ -1,40 +1,44 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "C2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "c-with-SPDX",
             "type": "library"
         },
         {
             "bom-ref": "C1",
             "licenses": [
                 {
-                    "acknowledgement": "concluded",
                     "expression": "Apache-2.0 OR MIT"
                 }
             ],
             "name": "c-with-expression",
             "type": "library"
         },
         {
             "bom-ref": "C3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "c-with-name",
             "type": "library"
         }
     ],
@@ -137,38 +141,42 @@
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
     "services": [
         {
             "bom-ref": "S2",
             "licenses": [
                 {
                     "license": {
-                        "id": "Apache-2.0"
+                        "id": "Apache-2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html"
                     }
                 }
             ],
             "name": "s-with-SPDX"
         },
         {
             "bom-ref": "S1",
             "licenses": [
                 {
-                    "acknowledgement": "declared",
                     "expression": "Apache-2.0 OR MIT"
                 }
             ],
             "name": "s-with-expression"
         },
         {
             "bom-ref": "S3",
             "licenses": [
                 {
                     "license": {
-                        "name": "(c) ACME Inc."
+                        "name": "some commercial license",
+                        "text": {
+                            "content": "this is a license text",
+                            "contentType": "text/plain"
+                        }
                     }
                 }
             ],
             "name": "s-with-name"
         }
     ],
-    "specVersion": "1.6",
+    "specVersion": "1.5",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin`

 * *Files 8% similar despite different names*

#### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin`

```diff
@@ -49,54 +49,58 @@
       </license>
     </licenses>
   </metadata>
   <components>
     <component type="library" bom-ref="C2">
       <name>c-with-SPDX</name>
       <licenses>
-        <license>
+        <license acknowledgement="concluded">
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </component>
     <component type="library" bom-ref="C1">
       <name>c-with-expression</name>
       <licenses>
         <expression acknowledgement="concluded">Apache-2.0 OR MIT</expression>
       </licenses>
     </component>
     <component type="library" bom-ref="C3">
       <name>c-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </component>
   </components>
   <services>
     <service bom-ref="S2">
       <name>s-with-SPDX</name>
       <licenses>
-        <license>
+        <license acknowledgement="declared">
           <id>Apache-2.0</id>
+          <url>https://www.apache.org/licenses/LICENSE-2.0.html</url>
         </license>
       </licenses>
     </service>
     <service bom-ref="S1">
       <name>s-with-expression</name>
       <licenses>
         <expression acknowledgement="declared">Apache-2.0 OR MIT</expression>
       </licenses>
     </service>
     <service bom-ref="S3">
       <name>s-with-name</name>
       <licenses>
         <license>
-          <name>(c) ACME Inc.</name>
+          <name>some commercial license</name>
+          <text content-type="text/plain">this is a license text</text>
         </license>
       </licenses>
     </service>
   </services>
   <dependencies>
     <dependency ref="C1"/>
     <dependency ref="C2"/>
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.5.schema.json'",*

 * * "'properties'": "[OrderedDict([('name', 'key1'), ('value', 'val1')]), OrderedDict([('name', "*

 * *                 "'key2'), ('value', 'val2')])]",*

 * * "'specVersion'": "'1.5'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.4.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "pkg:pypi/toml@0.10.2?extension=tar.gz",
             "externalReferences": [
                 {
                     "comment": "No comment",
@@ -95,11 +95,21 @@
                 ],
                 "name": "cyclonedx-python-lib",
                 "vendor": "CycloneDX",
                 "version": "TESTING"
             }
         ]
     },
+    "properties": [
+        {
+            "name": "key1",
+            "value": "val1"
+        },
+        {
+            "name": "key2",
+            "value": "val2"
+        }
+    ],
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "specVersion": "1.4",
+    "specVersion": "1.5",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.6.schema.json'", "'specVersion'": "'1.6'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
     "bomFormat": "CycloneDX",
     "components": [
         {
             "bom-ref": "pkg:pypi/toml@0.10.2?extension=tar.gz",
             "externalReferences": [
                 {
                     "comment": "No comment",
@@ -106,10 +106,10 @@
         },
         {
             "name": "key2",
             "value": "val2"
         }
     ],
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "specVersion": "1.5",
+    "specVersion": "1.6",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6571428571428571%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.5.schema.json'",*

 * * "'dependencies'": "{1: {'ref': 'my-specific-bom-ref-for-my-first-service', delete: "*

 * *                   "['dependsOn']}, 2: {'ref': 'my-specific-bom-ref-for-my-second-service'}, "*

 * *                   "insert: [(0, OrderedDict([('ref', 'my-specific-bom-ref-for-cpl')]))]}",*

 * * "'metadata'": "{'component': {'bom-ref': 'my-specific-bom-ref-for-cpl', 'name': "*

 * *               "'cyclonedx-python-lib', 'version': '1.0.0', delete: ['author', 'licenses' […]*

```diff
@@ -1,64 +1,27 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
     "bomFormat": "CycloneDX",
-    "components": [
-        {
-            "bom-ref": "pkg:pypi/toml@0.10.2?extension=tar.gz",
-            "externalReferences": [
-                {
-                    "comment": "No comment",
-                    "hashes": [
-                        {
-                            "alg": "SHA-256",
-                            "content": "806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"
-                        }
-                    ],
-                    "type": "distribution",
-                    "url": "https://cyclonedx.org"
-                }
-            ],
-            "hashes": [
-                {
-                    "alg": "SHA-256",
-                    "content": "806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"
-                }
-            ],
-            "name": "toml",
-            "purl": "pkg:pypi/toml@0.10.2?extension=tar.gz",
-            "type": "library",
-            "version": "0.10.2"
-        }
-    ],
     "dependencies": [
         {
-            "dependsOn": [
-                "pkg:pypi/toml@0.10.2?extension=tar.gz"
-            ],
-            "ref": "pkg:pypi/setuptools@50.3.2?extension=tar.gz"
+            "ref": "my-specific-bom-ref-for-cpl"
+        },
+        {
+            "ref": "my-specific-bom-ref-for-my-first-service"
         },
         {
-            "ref": "pkg:pypi/toml@0.10.2?extension=tar.gz"
+            "ref": "my-specific-bom-ref-for-my-second-service"
         }
     ],
     "metadata": {
         "component": {
-            "author": "Test Author",
-            "bom-ref": "pkg:pypi/setuptools@50.3.2?extension=tar.gz",
-            "licenses": [
-                {
-                    "license": {
-                        "id": "MIT"
-                    }
-                }
-            ],
-            "name": "setuptools",
-            "purl": "pkg:pypi/setuptools@50.3.2?extension=tar.gz",
+            "bom-ref": "my-specific-bom-ref-for-cpl",
+            "name": "cyclonedx-python-lib",
             "type": "library",
-            "version": "50.3.2"
+            "version": "1.0.0"
         },
         "timestamp": "2023-01-07T13:44:32.312678+00:00",
         "tools": [
             {
                 "externalReferences": [
                     {
                         "type": "build-system",
@@ -106,10 +69,20 @@
         },
         {
             "name": "key2",
             "value": "val2"
         }
     ],
     "serialNumber": "urn:uuid:1441d33a-e0fc-45b5-af3b-61ee52a88bac",
-    "specVersion": "1.6",
+    "services": [
+        {
+            "bom-ref": "my-specific-bom-ref-for-my-first-service",
+            "name": "my-first-service"
+        },
+        {
+            "bom-ref": "my-specific-bom-ref-for-my-second-service",
+            "name": "my-second-service"
+        }
+    ],
+    "specVersion": "1.5",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'$schema'": "'http://cyclonedx.org/schema/bom-1.6.schema.json'", "'specVersion'": "'1.6'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://cyclonedx.org/schema/bom-1.5.schema.json",
+    "$schema": "http://cyclonedx.org/schema/bom-1.6.schema.json",
     "bomFormat": "CycloneDX",
     "dependencies": [
         {
             "ref": "my-specific-bom-ref-for-cpl"
         },
         {
             "ref": "my-specific-bom-ref-for-my-first-service"
@@ -79,10 +79,10 @@
             "name": "my-first-service"
         },
         {
             "bom-ref": "my-specific-bom-ref-for-my-second-service",
             "name": "my-second-service"
         }
     ],
-    "specVersion": "1.5",
+    "specVersion": "1.6",
     "version": 1
 }
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin` & `cyclonedx_python_lib-7.2.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_component.py` & `cyclonedx_python_lib-7.2.0/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_deserialize_json.py` & `cyclonedx_python_lib-7.2.0/tests/test_deserialize_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_deserialize_xml.py` & `cyclonedx_python_lib-7.2.0/tests/test_deserialize_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_enums.py` & `cyclonedx_python_lib-7.2.0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_factory_license.py` & `cyclonedx_python_lib-7.2.0/tests/test_factory_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model.py` & `cyclonedx_python_lib-7.2.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_bom.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_bom_ref.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_component.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_dependency.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_issue.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_license.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_release_note.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_service.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_model_vulnerability.py` & `cyclonedx_python_lib-7.2.0/tests/test_model_vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_output.py` & `cyclonedx_python_lib-7.2.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_output_json.py` & `cyclonedx_python_lib-7.2.0/tests/test_output_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_output_xml.py` & `cyclonedx_python_lib-7.2.0/tests/test_output_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_real_world_examples.py` & `cyclonedx_python_lib-7.2.0/tests/test_real_world_examples.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_schema_SchemaVersion.py` & `cyclonedx_python_lib-7.2.0/tests/test_schema_SchemaVersion.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_schema__res.py` & `cyclonedx_python_lib-7.2.0/tests/test_schema__res.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_spdx.py` & `cyclonedx_python_lib-7.2.0/tests/test_spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_validation.py` & `cyclonedx_python_lib-7.2.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_validation_json.py` & `cyclonedx_python_lib-7.2.0/tests/test_validation_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 from unittest import TestCase
 
 from ddt import data, ddt, idata, unpack
 
 from cyclonedx.exception import MissingOptionalDependencyException
 from cyclonedx.schema import OutputFormat, SchemaVersion
 from cyclonedx.validation.json import JsonStrictValidator, JsonValidator
-from tests import SCHEMA_TESTDATA_DIRECTORY
+from tests import SCHEMA_TESTDATA_DIRECTORY, DpTuple
 
 UNSUPPORTED_SCHEMA_VERSIONS = {SchemaVersion.V1_0, SchemaVersion.V1_1, }
 
 
 def _dp(prefix: str) -> Generator:
     return (
-        (sv, tf) for sv in SchemaVersion if sv not in UNSUPPORTED_SCHEMA_VERSIONS
+        DpTuple((sv, tf)) for sv in SchemaVersion if sv not in UNSUPPORTED_SCHEMA_VERSIONS
         for tf in iglob(join(SCHEMA_TESTDATA_DIRECTORY, sv.to_version(), f'{prefix}-*.json'))
     )
 
 
 @ddt
 class TestJsonValidator(TestCase):
```

### Comparing `cyclonedx_python_lib-7.1.0/tests/test_validation_xml.py` & `cyclonedx_python_lib-7.2.0/tests/test_validation_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 from unittest import TestCase
 
 from ddt import ddt, idata, unpack
 
 from cyclonedx.exception import MissingOptionalDependencyException
 from cyclonedx.schema import OutputFormat, SchemaVersion
 from cyclonedx.validation.xml import XmlValidator
-from tests import SCHEMA_TESTDATA_DIRECTORY
+from tests import SCHEMA_TESTDATA_DIRECTORY, DpTuple
 
 UNSUPPORTED_SCHEMA_VERSIONS = set()
 
 
 def _dp(prefix: str) -> Generator:
     return (
-        (sv, tf) for sv in SchemaVersion if sv not in UNSUPPORTED_SCHEMA_VERSIONS
+        DpTuple((sv, tf)) for sv in SchemaVersion if sv not in UNSUPPORTED_SCHEMA_VERSIONS
         for tf in iglob(join(SCHEMA_TESTDATA_DIRECTORY, sv.to_version(), f'{prefix}-*.xml'))
     )
 
 
 @ddt
 class TestXmlValidator(TestCase):
```

### Comparing `cyclonedx_python_lib-7.1.0/PKG-INFO` & `cyclonedx_python_lib-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-python-lib
-Version: 7.1.0
+Version: 7.2.0
 Summary: Python library for CycloneDX
 Home-page: https://github.com/CycloneDX/cyclonedx-python-lib/#readme
 License: Apache-2.0
 Keywords: CycloneDX,library,OWASP,SCA,Software Bill of Materials,Bill of Materials,BOM,SBOM,VEX,VDR,OBOM,MBOM,SaaSBOM,SPDX,PackageURL,PURL
 Author: Paul Horton
 Author-email: phorton@sonatype.com
 Maintainer: Jan Kowalleck
```

