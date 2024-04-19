# Comparing `tmp/amsdal_utils-0.1.1.tar.gz` & `tmp/amsdal_utils-0.1.2.tar.gz`

## Comparing `amsdal_utils-0.1.1.tar` & `amsdal_utils-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/.editorconfig
--rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/Third-Party Materials - AMSDAL Dependencies - License Notices.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/classes/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/classes/metadata_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/classes/transaction_manager.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/classes/version_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/enums.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/amsdal_config.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/connection_config.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/integration_config.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/repository_config.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/resources_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/lifecycle/__init__.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/lifecycle/consumer.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/lifecycle/enum.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/lifecycle/producer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/base.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/enums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/__init__.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/address.py
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/metadata.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/reference.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/table_schema.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/transaction.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/mixins/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/mixins/cached_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/utils/__init__.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/utils/get_subclasses.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/models/utils/reference_builders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/enums.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/mixin.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/pull_out_filter.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/split.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/data_models/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/data_models/filter.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/data_models/order_by.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/data_models/paginator.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/query/data_models/query_specifier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/utils/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/utils/classes.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/utils/identifier.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/utils/lazy_object.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/utils/singleton.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/src/amsdal_utils/utils/text.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/.gitignore
--rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0    28395 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/README.md
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    57431 2020-02-02 00:00:00.000000 amsdal_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/.editorconfig
+-rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/Third-Party Materials - AMSDAL Dependencies - License Notices.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/classes/__init__.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/classes/metadata_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/classes/transaction_manager.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/classes/version_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/enums.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/amsdal_config.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/connection_config.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/integration_config.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/repository_config.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/resources_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/lifecycle/__init__.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/lifecycle/consumer.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/lifecycle/enum.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/lifecycle/producer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/base.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/enums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/__init__.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/address.py
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/metadata.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/reference.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/table_schema.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/transaction.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/mixins/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/mixins/cached_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/utils/__init__.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/utils/get_subclasses.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/models/utils/reference_builders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/enums.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/mixin.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/pull_out_filter.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/split.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/data_models/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/data_models/filter.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/data_models/order_by.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/data_models/paginator.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/query/data_models/query_specifier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/utils/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/utils/classes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/utils/identifier.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/utils/lazy_object.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/utils/singleton.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/src/amsdal_utils/utils/text.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/.gitignore
+-rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0    28395 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/README.md
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    57431 2020-02-02 00:00:00.000000 amsdal_utils-0.1.2/PKG-INFO
```

### Comparing `amsdal_utils-0.1.1/.editorconfig` & `amsdal_utils-0.1.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/Third-Party Materials - AMSDAL Dependencies - License Notices.md` & `amsdal_utils-0.1.2/src/amsdal_utils/Third-Party Materials - AMSDAL Dependencies - License Notices.md`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/classes/metadata_manager.py` & `amsdal_utils-0.1.2/src/amsdal_utils/classes/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/classes/transaction_manager.py` & `amsdal_utils-0.1.2/src/amsdal_utils/classes/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/classes/version_manager.py` & `amsdal_utils-0.1.2/src/amsdal_utils/classes/version_manager.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/config/manager.py` & `amsdal_utils-0.1.2/src/amsdal_utils/config/manager.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/amsdal_config.py` & `amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/amsdal_config.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/config/data_models/connection_config.py` & `amsdal_utils-0.1.2/src/amsdal_utils/config/data_models/connection_config.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/lifecycle/consumer.py` & `amsdal_utils-0.1.2/src/amsdal_utils/lifecycle/consumer.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/lifecycle/producer.py` & `amsdal_utils-0.1.2/src/amsdal_utils/lifecycle/producer.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/address.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/address.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/metadata.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/metadata.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/reference.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/reference.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/table_schema.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/table_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 class DictSchemaModel(BaseModel):
     key_type: type
     value_type: Union['DictSchemaModel', 'NestedSchemaModel', 'ArraySchemaModel', type[JsonSchemaModel], type]
 
 
 class TableColumnSchema(BaseModel):
     name: str
+    field_id: str
     type: type | NestedSchemaModel | ArraySchemaModel | DictSchemaModel | type[JsonSchemaModel]
     default: Any
     nullable: bool = True
+    is_deleted: bool = False
 
 
 class TableIndexSchema(BaseModel):
     column_name: str
     index_type: str = ''
```

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/data_models/transaction.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/data_models/transaction.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/mixins/cached_mixin.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/mixins/cached_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/utils/get_subclasses.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/utils/get_subclasses.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/models/utils/reference_builders.py` & `amsdal_utils-0.1.2/src/amsdal_utils/models/utils/reference_builders.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/query/pull_out_filter.py` & `amsdal_utils-0.1.2/src/amsdal_utils/query/pull_out_filter.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/query/split.py` & `amsdal_utils-0.1.2/src/amsdal_utils/query/split.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/query/utils.py` & `amsdal_utils-0.1.2/src/amsdal_utils/query/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/query/data_models/filter.py` & `amsdal_utils-0.1.2/src/amsdal_utils/query/data_models/filter.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/utils/lazy_object.py` & `amsdal_utils-0.1.2/src/amsdal_utils/utils/lazy_object.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/utils/singleton.py` & `amsdal_utils-0.1.2/src/amsdal_utils/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/src/amsdal_utils/utils/text.py` & `amsdal_utils-0.1.2/src/amsdal_utils/utils/text.py`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/LICENSE.txt` & `amsdal_utils-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/README.md` & `amsdal_utils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amsdal_utils-0.1.1/pyproject.toml` & `amsdal_utils-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,17 @@
 init_typed = true
 warn_required_dynamic_aliases = true
 
 [tool.ruff]
 target-version = "py310"
 line-length = 120
 
+[tool.ruff.format]
+quote-style = "single"
+
 [tool.ruff.lint]
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
```

### Comparing `amsdal_utils-0.1.1/PKG-INFO` & `amsdal_utils-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: amsdal_utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils for AMSDAL data framework
 Project-URL: Documentation, https://pypi.org/project/amsdal_utils/#readme
 Project-URL: Issues, https://pypi.org/project/amsdal_utils/#issues
 Project-URL: Source, https://pypi.org/project/amsdal_utils/
 Author-email: "A. Michael Salem" <ams@amsdal.com>
 License: AMSDAL End User License Agreement
```

