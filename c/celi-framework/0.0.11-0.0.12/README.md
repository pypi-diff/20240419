# Comparing `tmp/celi_framework-0.0.11.tar.gz` & `tmp/celi_framework-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celi_framework-0.0.11.tar", max compression
+gzip compressed data, was "celi_framework-0.0.12.tar", max compression
```

## Comparing `celi_framework-0.0.11.tar` & `celi_framework-0.0.12.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1084 2024-04-19 03:13:27.169492 celi_framework-0.0.11/LICENSE
--rw-r--r--   0        0        0    21905 2024-04-19 03:13:27.169492 celi_framework-0.0.11/README.md
--rw-r--r--   0        0        0    10399 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/job_description.py
--rw-r--r--   0        0        0    23124 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/monitor.py
--rw-r--r--   0        0        0    11301 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/mt_factory.py
--rw-r--r--   0        0        0    14719 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/post_monitor.py
--rw-r--r--   0        0        0    59120 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/processor.py
--rw-r--r--   0        0        0     3060 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/runner.py
--rw-r--r--   0        0        0    23630 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/core/templates.py
--rw-r--r--   0        0        0    13793 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/reporting_template/job_description.py
--rw-r--r--   0        0        0    10317 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/reporting_template/tools.py
--rw-r--r--   0        0        0     6133 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/Index_cache.py
--rw-r--r--   0        0        0     7692 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
--rw-r--r--   0        0        0     5552 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/eval/run_eval.py
--rw-r--r--   0        0        0      530 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/eval/test_sets.json
--rw-r--r--   0        0        0      851 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/eval/test_sets_large.json
--rw-r--r--   0        0        0      161 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/example_config.json
--rw-r--r--   0        0        0    13742 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/index.py
--rw-r--r--   0        0        0    13330 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/job_description.py
--rw-r--r--   0        0        0     7111 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/loader.py
--rw-r--r--   0        0        0    14758 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/tools.py
--rw-r--r--   0        0        0      549 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/examples/wikipedia/wikipedia_utils.py
--rw-r--r--   0        0        0    12668 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/embeddor.py
--rw-r--r--   0        0        0     7936 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/mapper.py
--rw-r--r--   0        0        0     1354 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/mechanic.py
--rw-r--r--   0        0        0        0 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/__init__.py
--rw-r--r--   0        0        0    23634 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/pre-processor.py
--rw-r--r--   0        0        0       94 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
--rw-r--r--   0        0        0     8832 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
--rw-r--r--   0        0        0     2056 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
--rw-r--r--   0        0        0    10669 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
--rw-r--r--   0        0        0     7835 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
--rw-r--r--   0        0        0     5471 2024-04-19 03:13:27.169492 celi_framework-0.0.11/celi_framework/experimental/task_builder/factory.py
--rw-r--r--   0        0        0     4242 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/task_builder/llm_helper_funcs.py
--rw-r--r--   0        0        0     4352 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/task_builder/llms.py
--rw-r--r--   0        0        0     5939 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/task_builder/template.py
--rw-r--r--   0        0        0     9914 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/utils/ada.py
--rw-r--r--   0        0        0    19041 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/utils/mapper_utils.py
--rw-r--r--   0        0        0    13615 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
--rw-r--r--   0        0        0     5118 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
--rw-r--r--   0        0        0     5458 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/utils/postprocessor_utils.py
--rw-r--r--   0        0        0     9091 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/experimental/utils/synthetic_data.py
--rw-r--r--   0        0        0     1350 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/logging_config.json
--rw-r--r--   0        0        0     2171 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/logging_setup.py
--rw-r--r--   0        0        0     6716 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/main.py
--rw-r--r--   0        0        0        0 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/__init__.py
--rw-r--r--   0        0        0    10889 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/codex.py
--rw-r--r--   0        0        0      461 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/exceptions.py
--rw-r--r--   0        0        0    22485 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/llmcore_utils.py
--rw-r--r--   0        0        0    10021 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/llms.py
--rw-r--r--   0        0        0       77 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/log.py
--rw-r--r--   0        0        0    10717 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/sql_utils.py
--rw-r--r--   0        0        0    10871 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/token_counters.py
--rw-r--r--   0        0        0    28482 2024-04-19 03:13:27.173492 celi_framework-0.0.11/celi_framework/utils/utils.py
--rw-r--r--   0        0        0     1758 2024-04-19 03:14:17.557198 celi_framework-0.0.11/pyproject.toml
--rw-r--r--   0        0        0    23341 1970-01-01 00:00:00.000000 celi_framework-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-19 03:46:42.886429 celi_framework-0.0.12/LICENSE
+-rw-r--r--   0        0        0    12806 2024-04-19 03:46:42.890429 celi_framework-0.0.12/README.md
+-rw-r--r--   0        0        0    10399 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/job_description.py
+-rw-r--r--   0        0        0    23124 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/monitor.py
+-rw-r--r--   0        0        0    11301 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/mt_factory.py
+-rw-r--r--   0        0        0    14719 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/post_monitor.py
+-rw-r--r--   0        0        0    59120 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/processor.py
+-rw-r--r--   0        0        0     3060 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/runner.py
+-rw-r--r--   0        0        0    23630 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/core/templates.py
+-rw-r--r--   0        0        0    13793 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/reporting_template/job_description.py
+-rw-r--r--   0        0        0    10317 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/reporting_template/tools.py
+-rw-r--r--   0        0        0     6133 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/Index_cache.py
+-rw-r--r--   0        0        0     7694 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
+-rw-r--r--   0        0        0     5552 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/eval/run_eval.py
+-rw-r--r--   0        0        0      530 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/eval/test_sets.json
+-rw-r--r--   0        0        0      851 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/eval/test_sets_large.json
+-rw-r--r--   0        0        0      161 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/example_config.json
+-rw-r--r--   0        0        0    13742 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/index.py
+-rw-r--r--   0        0        0    13330 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/job_description.py
+-rw-r--r--   0        0        0     7111 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/loader.py
+-rw-r--r--   0        0        0    14758 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/tools.py
+-rw-r--r--   0        0        0      549 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/examples/wikipedia/wikipedia_utils.py
+-rw-r--r--   0        0        0    12668 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/embeddor.py
+-rw-r--r--   0        0        0     7936 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/mapper.py
+-rw-r--r--   0        0        0     1354 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/mechanic.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/__init__.py
+-rw-r--r--   0        0        0    23634 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/pre-processor.py
+-rw-r--r--   0        0        0       94 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
+-rw-r--r--   0        0        0     8832 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
+-rw-r--r--   0        0        0     2056 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
+-rw-r--r--   0        0        0    10669 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
+-rw-r--r--   0        0        0     7835 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
+-rw-r--r--   0        0        0     5471 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/task_builder/factory.py
+-rw-r--r--   0        0        0     4242 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/task_builder/llm_helper_funcs.py
+-rw-r--r--   0        0        0     4352 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/task_builder/llms.py
+-rw-r--r--   0        0        0     5939 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/task_builder/template.py
+-rw-r--r--   0        0        0     9914 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/utils/ada.py
+-rw-r--r--   0        0        0    19041 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/utils/mapper_utils.py
+-rw-r--r--   0        0        0    13615 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
+-rw-r--r--   0        0        0     5118 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
+-rw-r--r--   0        0        0     5458 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/utils/postprocessor_utils.py
+-rw-r--r--   0        0        0     9091 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/experimental/utils/synthetic_data.py
+-rw-r--r--   0        0        0     1350 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/logging_config.json
+-rw-r--r--   0        0        0     2171 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/logging_setup.py
+-rw-r--r--   0        0        0     6716 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/main.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/utils/__init__.py
+-rw-r--r--   0        0        0    10889 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/utils/codex.py
+-rw-r--r--   0        0        0      461 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/utils/exceptions.py
+-rw-r--r--   0        0        0    22485 2024-04-19 03:46:42.890429 celi_framework-0.0.12/celi_framework/utils/llmcore_utils.py
+-rw-r--r--   0        0        0    10021 2024-04-19 03:46:42.894429 celi_framework-0.0.12/celi_framework/utils/llms.py
+-rw-r--r--   0        0        0       77 2024-04-19 03:46:42.894429 celi_framework-0.0.12/celi_framework/utils/log.py
+-rw-r--r--   0        0        0    10717 2024-04-19 03:46:42.894429 celi_framework-0.0.12/celi_framework/utils/sql_utils.py
+-rw-r--r--   0        0        0    10871 2024-04-19 03:46:42.894429 celi_framework-0.0.12/celi_framework/utils/token_counters.py
+-rw-r--r--   0        0        0    28482 2024-04-19 03:46:42.894429 celi_framework-0.0.12/celi_framework/utils/utils.py
+-rw-r--r--   0        0        0     1758 2024-04-19 03:47:12.730501 celi_framework-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0    14242 1970-01-01 00:00:00.000000 celi_framework-0.0.12/PKG-INFO
```

### Comparing `celi_framework-0.0.11/LICENSE` & `celi_framework-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/job_description.py` & `celi_framework-0.0.12/celi_framework/core/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/monitor.py` & `celi_framework-0.0.12/celi_framework/core/monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/mt_factory.py` & `celi_framework-0.0.12/celi_framework/core/mt_factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/post_monitor.py` & `celi_framework-0.0.12/celi_framework/core/post_monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/processor.py` & `celi_framework-0.0.12/celi_framework/core/processor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/runner.py` & `celi_framework-0.0.12/celi_framework/core/runner.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/core/templates.py` & `celi_framework-0.0.12/celi_framework/core/templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/reporting_template/job_description.py` & `celi_framework-0.0.12/celi_framework/examples/reporting_template/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/reporting_template/tools.py` & `celi_framework-0.0.12/celi_framework/examples/reporting_template/tools.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/Index_cache.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/Index_cache.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 Modified to use a requests_caching.
 Beautiful Soup Web scraper."""
 
 import logging
 from typing import Any, Callable, Dict, List, Optional, Tuple
 from urllib.parse import urljoin
+from requests import Session
 
 from llama_index.core.bridge.pydantic import PrivateAttr
 from llama_index.core.readers.base import BasePydanticReader
 from llama_index.core.schema import Document
-from pytest import Session
 
 logger = logging.getLogger(__name__)
 
 
 def _substack_reader(soup: Any, **kwargs) -> Tuple[str, Dict[str, Any]]:
     """Extract text from Substack blog post."""
     extra_info = {
```

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/eval/run_eval.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/eval/run_eval.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/eval/test_sets.json` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/eval/test_sets.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/eval/test_sets_large.json` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/eval/test_sets_large.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/index.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/index.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/job_description.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/loader.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/loader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/tools.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/tools.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/examples/wikipedia/wikipedia_utils.py` & `celi_framework-0.0.12/celi_framework/examples/wikipedia/wikipedia_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/embeddor.py` & `celi_framework-0.0.12/celi_framework/experimental/embeddor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/mapper.py` & `celi_framework-0.0.12/celi_framework/experimental/mapper.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/mechanic.py` & `celi_framework-0.0.12/celi_framework/experimental/mechanic.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/preprocessing/pre-processor.py` & `celi_framework-0.0.12/celi_framework/experimental/preprocessing/pre-processor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py` & `celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py` & `celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py` & `celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py` & `celi_framework-0.0.12/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/task_builder/factory.py` & `celi_framework-0.0.12/celi_framework/experimental/task_builder/factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/task_builder/llm_helper_funcs.py` & `celi_framework-0.0.12/celi_framework/experimental/task_builder/llm_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/task_builder/llms.py` & `celi_framework-0.0.12/celi_framework/experimental/task_builder/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/task_builder/template.py` & `celi_framework-0.0.12/celi_framework/experimental/task_builder/template.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/utils/ada.py` & `celi_framework-0.0.12/celi_framework/experimental/utils/ada.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/utils/mapper_utils.py` & `celi_framework-0.0.12/celi_framework/experimental/utils/mapper_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py` & `celi_framework-0.0.12/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py` & `celi_framework-0.0.12/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/utils/postprocessor_utils.py` & `celi_framework-0.0.12/celi_framework/experimental/utils/postprocessor_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/experimental/utils/synthetic_data.py` & `celi_framework-0.0.12/celi_framework/experimental/utils/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/logging_config.json` & `celi_framework-0.0.12/celi_framework/logging_config.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/logging_setup.py` & `celi_framework-0.0.12/celi_framework/logging_setup.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/main.py` & `celi_framework-0.0.12/celi_framework/main.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/utils/codex.py` & `celi_framework-0.0.12/celi_framework/utils/codex.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/utils/llmcore_utils.py` & `celi_framework-0.0.12/celi_framework/utils/llmcore_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/utils/llms.py` & `celi_framework-0.0.12/celi_framework/utils/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/utils/sql_utils.py` & `celi_framework-0.0.12/celi_framework/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/utils/token_counters.py` & `celi_framework-0.0.12/celi_framework/utils/token_counters.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/celi_framework/utils/utils.py` & `celi_framework-0.0.12/celi_framework/utils/utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.11/pyproject.toml` & `celi_framework-0.0.12/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celi-framework"
-version = "0.0.11"
+version = "0.0.12"
 description = "Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment."
 authors = ["Jan-Samuel Wagner <jwab@genmab.com>","Dave DeCaprio <daved@alum.mit.edu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/x3n0cr4735/celi"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

