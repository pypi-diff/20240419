# Comparing `tmp/nyckel-0.4.0.tar.gz` & `tmp/nyckel-0.4.1.tar.gz`

## Comparing `nyckel-0.4.0.tar` & `nyckel-0.4.1.tar`

### file list

```diff
@@ -1,66 +1,70 @@
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 nyckel-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.0/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.0/.vscode/extensions.json
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 nyckel-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/credentials.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/image_classification.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/merge_labels.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/data_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 nyckel-0.4.0/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_field_handler.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_image_decoder.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_sample_handler.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_text_tags_function.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/test_white_background.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/fixtures/flower.jpg
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.0/tests/fixtures/mixed-alpha-background.png
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.0/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.0/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.1/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 nyckel-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/credentials.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/image_classification.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/image_tags.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/merge_labels.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/tabular_classification.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/image_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/image_tags.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.1/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_image_tags_function.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_text_tags_function.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.1/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.1/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.1/PKG-INFO
```

### Comparing `nyckel-0.4.0/mkdocs.yml` & `nyckel-0.4.1/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     - Delete samples: delete_samples.md
     - Multimodal classification: multimodal_classification.md
   - Reference:
     - Image Classification: image_classification.md
     - Text Classification: text_classification.md
     - Tabular Classification: tabular_classification.md
     - Text Tags: text_tags.md
+    - Image Tags: image_tags.md
     - Credentials: credentials.md
     - Data classes: data_classes.md
 theme: 
   name: 'material'
   features:
     - content.code.copy
   logo: assets/nyckel-logo.png
```

### Comparing `nyckel-0.4.0/.github/workflows/build.yml` & `nyckel-0.4.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/.github/workflows/docs.yml` & `nyckel-0.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/.github/workflows/test.yml` & `nyckel-0.4.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/.vscode/settings.json` & `nyckel-0.4.1/.vscode/settings.json`

 * *Files 13% similar despite different names*

```diff
@@ -23,10 +23,11 @@
         "getpixel",
         "Gruezi",
         "Hola",
         "Multimodal",
         "ncols",
         "nyckel",
         "pytest",
+        "Resizer",
         "tqdm"
     ],
 }
```

### Comparing `nyckel-0.4.0/docs/copy_function.md` & `nyckel-0.4.1/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/delete_label.md` & `nyckel-0.4.1/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/delete_samples.md` & `nyckel-0.4.1/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/index.md` & `nyckel-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/merge_labels.md` & `nyckel-0.4.1/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/multimodal_classification.md` & `nyckel-0.4.1/docs/multimodal_classification.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/quickstart.md` & `nyckel-0.4.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/assets/favicon.ico` & `nyckel-0.4.1/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/docs/assets/nyckel-logo.png` & `nyckel-0.4.1/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/__init__.py` & `nyckel-0.4.1/src/nyckel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,7 +33,8 @@
     ImageClassificationFunction,  # noqa: F401
     ImageDecoder,  # noqa: F401
     ImageEncoder,  # noqa: F401
 )
 from .functions.classification.tabular_classification import TabularClassificationFunction  # noqa: F401
 from .functions.classification.text_classification import TextClassificationFunction  # noqa: F401
 from .functions.tags.text_tags import TextTagsFunction  # noqa: F401
+from .functions.tags.image_tags import ImageTagsFunction  # noqa: F401
```

### Comparing `nyckel-0.4.0/src/nyckel/auth.py` & `nyckel-0.4.1/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/request_utils.py` & `nyckel-0.4.1/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.1/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.1/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.1/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.1/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.1/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.1/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.1/src/nyckel/functions/classification/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.1/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.1/src/nyckel/functions/tags/tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.1/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import time
 
 from nyckel import Credentials
-from nyckel.functions.tags import text_tags
+from nyckel.functions.tags import image_tags, text_tags
 from nyckel.functions.tags.tags_function_handler import TagsFunctionHandler
 from nyckel.functions.utils import strip_nyckel_prefix
 
 
 class TagsFunctionFactory:
 
     def __init__(self) -> None:
         self.function_type_by_input = {
             "Text": text_tags.TextTagsFunction,
-            # "Image": image_classification.ImageClassificationFunction,
+            "Image": image_tags.ImageTagsFunction,
             # "Tabular": tabular_classification.TabularClassificationFunction,
         }
 
     @classmethod
     def load(self, function_id: str, credentials: Credentials):
         function_handler = TagsFunctionHandler(function_id, credentials)
         input_modality = function_handler.get_input_modality()
```

### Comparing `nyckel-0.4.0/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.1/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.1/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import time
 from typing import Any, Callable, Dict, List, Tuple, Union
 
+from tqdm import tqdm
+
 from nyckel import (
     ClassificationPrediction,
     Credentials,
     ImageTagsSample,
     TabularTagsSample,
     TagsPrediction,
     TextTagsSample,
 )
 from nyckel.functions.tags.tags import TagsFunctionURLHandler
 from nyckel.functions.utils import strip_nyckel_prefix
 from nyckel.request_utils import ParallelDeleter, ParallelPoster, SequentialGetter
 from nyckel.utils import chunkify_list
-from tqdm import tqdm
 
 TagsSampleList = Union[List[TextTagsSample], List[ImageTagsSample], List[TabularTagsSample]]
 
 
 class TagsSampleHandler:
 
     def __init__(self, function_id: str, credentials: Credentials) -> None:
@@ -130,15 +131,15 @@
         if not response.status_code == 200:
             raise RuntimeError(
                 f"{response.status_code=}, {response.text=}. Unable to fetch sample {sample_id} "
                 f"from {self._url_handler.train_page}"
             )
         return response.json()
 
-    def update_annotation(self, sample: TextTagsSample) -> None:
+    def update_annotation(self, sample: Union[TextTagsSample, ImageTagsSample]) -> None:
         session = self._credentials.get_session()
         assert sample.annotation
         response = session.put(
             self._url_handler.api_endpoint(path=f"samples/{sample.id}/annotation", api_version="v0.9"),
             json=[
                 {
                     "labelName": entry.label_name,
```

### Comparing `nyckel-0.4.0/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.1/src/nyckel/functions/tags/text_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,25 +159,26 @@
                     label_name=label_name_by_id[strip_nyckel_prefix(entry["labelId"])],
                     present=entry["present"],
                 )
                 for entry in sample_dict["annotation"]
             ]
         else:
             annotation = None
+
         if "prediction" in sample_dict:
             prediction = [
                 ClassificationPrediction(
                     confidence=entry["confidence"],
                     label_name=label_name_by_id[strip_nyckel_prefix(entry["labelId"])],
                 )
                 for entry in sample_dict["prediction"]
             ]
-
         else:
             prediction = None
+
         return TextTagsSample(
             id=strip_nyckel_prefix(sample_dict["id"]),
             data=sample_dict["data"],
             external_id=sample_dict["externalId"] if "externalId" in sample_dict else None,
             annotation=annotation,
             prediction=prediction,
         )
```

### Comparing `nyckel-0.4.0/tests/conftest.py` & `nyckel-0.4.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from nyckel import (
     ClassificationAnnotation,
     ClassificationFunction,
     ClassificationLabel,
     Credentials,
     ImageClassificationFunction,
     ImageClassificationSample,
+    ImageTagsFunction,
     TabularClassificationFunction,
     TabularClassificationSample,
     TextClassificationFunction,
     TextClassificationSample,
     TextTagsFunction,
 )
 from nyckel.functions.classification.image_classification import ImageEncoder
@@ -134,14 +135,21 @@
 @pytest.fixture
 def text_tags_function(auth_test_credentials: Credentials) -> Iterator[TextTagsFunction]:
     func = TextTagsFunction.create("PYTHON-SDK TEXT TAGS TEST FUNCTION", auth_test_credentials)
     yield func
     func.delete()
 
 
+@pytest.fixture
+def image_tags_function(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
+    func = ImageTagsFunction.create("PYTHON-SDK IMAGE TAGS TEST FUNCTION", auth_test_credentials)
+    yield func
+    func.delete()
+
+
 def get_test_credentials() -> Credentials:
     if "NYCKEL_PYTHON_SDK_CLIENT_SECRET" in os.environ:
         credentials = Credentials(
             client_id="python-sdk-test",
             client_secret=os.environ["NYCKEL_PYTHON_SDK_CLIENT_SECRET"],
             server_url="https://www.nyckel-staging.com",
         )
```

### Comparing `nyckel-0.4.0/tests/test_duplicates_handling.py` & `nyckel-0.4.1/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_field_handler.py` & `nyckel-0.4.1/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_image_classification_function.py` & `nyckel-0.4.1/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_image_decoder.py` & `nyckel-0.4.1/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_label_handler.py` & `nyckel-0.4.1/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_sample_handler.py` & `nyckel-0.4.1/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_tabular_classification_function.py` & `nyckel-0.4.1/tests/test_tabular_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_text_classification_function.py` & `nyckel-0.4.1/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/test_text_tags_function.py` & `nyckel-0.4.1/tests/test_text_tags_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -94,14 +94,43 @@
     sample_ids = func.create_samples(samples)
     time.sleep(1)
     func.delete_samples(sample_ids[0:1])
     time.sleep(1)
     assert len(func.list_samples()) == 1
 
 
+def test_new_labels(text_tags_function: TextTagsFunction) -> None:
+
+    func = text_tags_function
+
+    func.create_labels([ClassificationLabel(name="label1")])
+    time.sleep(0.5)
+    sample_1_id = func.create_samples([TextTagsSample(data="sample1", annotation=[TagsAnnotation("label1")])])[0]
+
+    func.create_labels([ClassificationLabel(name="label2")])
+    time.sleep(0.5)
+    sample_2_id = func.create_samples([TextTagsSample(data="sample2", annotation=[TagsAnnotation("label1")])])[0]
+
+    sample1 = func.read_sample(sample_1_id)
+
+    # When sample1 was created, label2 wasn't present yet.
+    # So sample1 doesn't have an "opinion" about that label.
+    # This means that it's not present in the annotation field.
+    assert len(sample1.annotation) == 1
+    assert TagsAnnotation("label1") in sample1.annotation
+    assert TagsAnnotation("label2", present=False) not in sample1.annotation
+    time.sleep(0.5)
+    sample2 = func.read_sample(sample_2_id)
+    # When sample2 was created, both labels were present.
+    # Since we didn't give an annotation for label2, it was set to not present.
+    assert len(sample2.annotation) == 2
+    assert TagsAnnotation("label1") in sample2.annotation
+    assert TagsAnnotation("label2", present=False) in sample2.annotation
+
+
 def test_end_to_end(text_tags_function: TextTagsFunction) -> None:
     func = text_tags_function
 
     labels_to_create = [ClassificationLabel(name="Nice"), ClassificationLabel(name="Boo")]
     func.create_labels(labels_to_create)
 
     samples = [
@@ -113,15 +142,17 @@
     ]
 
     func.create_samples(samples)
 
     while not func.has_trained_model():
         print("-> No trained model yet. Sleeping 1 sec...")
         time.sleep(1)
-    pred = func.invoke(["Howdy"])[0]
-    assert isinstance(pred[0], ClassificationPrediction)
 
-    assert len(func.invoke(["Hej", "Hola", "Gruezi"])) == 3
+    predictions = func.invoke(["Hej", "Hola", "Gruezi"])
+    assert len(predictions) == 3
+    for prediction in predictions:
+        if len(prediction) > 0:
+            assert isinstance(prediction[0], ClassificationPrediction)
 
     returned_samples = func.list_samples()
     assert len(samples) == len(returned_samples)
     assert isinstance(returned_samples[0], TextTagsSample)
```

### Comparing `nyckel-0.4.0/tests/test_white_background.py` & `nyckel-0.4.1/tests/test_white_background.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/fixtures/flower.jpg` & `nyckel-0.4.1/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/tests/fixtures/mixed-alpha-background.png` & `nyckel-0.4.1/tests/fixtures/mixed-alpha-background.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/.gitignore` & `nyckel-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/LICENSE` & `nyckel-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/README.md` & `nyckel-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.0/pyproject.toml` & `nyckel-0.4.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.4.0"
+version = "0.4.1"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.4.0/PKG-INFO` & `nyckel-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

