# Comparing `tmp/cf2tf-0.6.3a27.tar.gz` & `tmp/cf2tf-0.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.6.3a27.tar", max compression
+gzip compressed data, was "cf2tf-0.7.0a0.tar", max compression
```

## Comparing `cf2tf-0.6.3a27.tar` & `cf2tf-0.7.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/LICENSE.txt
--rw-r--r--   0        0        0     7485 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/README.md
--rw-r--r--   0        0        0     1090 2024-04-18 00:06:15.759629 cf2tf-0.6.3a27/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2621 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    31228 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     2026 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    21736 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2673 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2199 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     3995 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     4674 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2673 2024-04-18 00:06:01.267579 cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8534 1970-01-01 00:00:00.000000 cf2tf-0.6.3a27/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/LICENSE.txt
+-rw-r--r--   0        0        0     7485 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/README.md
+-rw-r--r--   0        0        0     1089 2024-04-19 21:26:04.618107 cf2tf-0.7.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2621 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    32491 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2026 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    21718 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2673 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2199 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     3995 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     4674 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2673 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.7.0a0/PKG-INFO
```

### Comparing `cf2tf-0.6.3a27/LICENSE.txt` & `cf2tf-0.7.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/README.md` & `cf2tf-0.7.0a0/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/pyproject.toml` & `cf2tf-0.7.0a0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.6.3a27"
+version = "0.7.0a0"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
```

### Comparing `cf2tf-0.6.3a27/src/cf2tf/app.py` & `cf2tf-0.7.0a0/src/cf2tf/app.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.7.0a0/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/conversion/expressions.py` & `cf2tf-0.7.0a0/src/cf2tf/conversion/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,27 +355,76 @@
     """Converts AWS GetAtt intrinsic function to it's Terraform equivalent.
 
     Args:
         template (Configuration): The template being tested.
         values (Any): The values passed to the function.
 
     Raises:
-        TypeError: If values is not a list.
-        ValueError: If length of values is not 3.
-        TypeError: If the logicalNameOfResource and attributeName are not str.
-        KeyError: If the logicalNameOfResource is not found in the template.
+        TypeError: If values is not a String.
 
     Returns:
-        str: Terraform equivalent expression.
+        LiteralType: Terraform equivalent expression.
     """
 
-    if not isinstance(values, List):
-        raise TypeError(
-            f"Fn::GetAtt - The values must be a List, not {type(values).__name__}."
+    if isinstance(values, (str, StringType)):
+        return _get_att_string(template, values)
+
+    if isinstance(values, list):
+        return _get_att_list(template, values)
+
+    raise TypeError(
+        f"Fn::GetAtt - The value must be a String or List, not {type(values).__name__}."
+    )
+
+
+def _get_att_string(template: "TemplateConverter", values: Any):
+    """Converts AWS GetAtt intrinsic function to it's Terraform equivalent.
+
+    Args:
+        template (Configuration): The template being tested.
+        values (Any): The values passed to the function.
+
+    Raises:
+        ValueError: If the value doesn't contain a resource id and an attribute.
+
+    Returns:
+        LiteralType: Terraform equivalent expression.
+    """
+
+    if "." not in values:
+        raise ValueError(
+            "Fn::GetAtt - The value must contain a resource id and an attribute."
         )
+
+    parts = values.split(".")
+
+    resouce_id = parts[0]
+
+    attributes = ".".join(parts[1:])
+
+    result = _get_att_list(template, [resouce_id, attributes])
+
+    return result
+
+
+def _get_att_list(template: "TemplateConverter", values: Any):
+    """Converts AWS GetAtt intrinsic function to it's Terraform equivalent.
+
+    Args:
+        template (Configuration): The template being tested.
+        values (Any): The values passed to the function.
+
+    Raises:
+        ValueError: If the values length is not 2.
+        TypeError: If the values are not strings.
+
+    Returns:
+        LiteralType: Terraform equivalent expression.
+    """
+
     if not len(values) == 2:
         raise ValueError(
             (
                 "Fn::GetAtt - The values must contain "
                 "the logicalNameOfResource and attributeName."
             )
         )
@@ -708,15 +757,15 @@
         if "." in var:
             parts = var.split(".")
 
             resouce_id = parts[0]
 
             attributes = ".".join(parts[1:])
 
-            result = get_att(template, [resouce_id, attributes])
+            result = _get_att_list(template, [resouce_id, attributes])
         else:
             result = ref(template, var)
 
         return wrap_in_curlys(result)
 
     reVar = r"(?!\$\{\!)\$\{(\w+[^}]*)\}"
 
@@ -771,15 +820,15 @@
         if "." in var:
             parts = var.split(".")
 
             resouce_id = parts[0]
 
             attributes = ".".join(parts[1:])
 
-            result = get_att(template, [resouce_id, attributes])
+            result = _get_att_list(template, [resouce_id, attributes])
         else:
             result = ref(template, var)
 
         return wrap_in_curlys(result)
 
     reVar = r"(?!\$\{\!)\$\{(\w+[^}]*)\}"
 
@@ -978,33 +1027,36 @@
 # functions that are allowed to be nested inside it.
 ALLOWED_FUNCTIONS: Dict[str, Dispatch] = {
     "Fn::And": ALLOWED_NESTED_CONDITIONS,
     "Fn::Equals": {
         **ALLOWED_NESTED_CONDITIONS,
         "Fn::Join": join,
         "Fn::Select": select,
+        "Fn::Sub": sub,
     },
     "Fn::If": {
         "Fn::Base64": base64,
         "Fn::FindInMap": find_in_map,
         "Fn::GetAtt": get_att,
         "Fn::GetAZs": get_azs,
         "Fn::If": if_,
         "Fn::Join": join,
         "Fn::Select": select,
         "Fn::Sub": sub,
         "Ref": ref,
+        "Fn::Split": split,
     },
     "Fn::Not": ALLOWED_NESTED_CONDITIONS,
     "Fn::Or": ALLOWED_NESTED_CONDITIONS,
     "Condition": {},  # Only allows strings
     "Fn::Base64": ALL_FUNCTIONS,
     "Fn::Cidr": {
         "Fn::Select": select,
         "Ref": ref,
+        "Fn::GetAtt": get_att,
     },
     "Fn::FindInMap": {
         "Fn::FindInMap": find_in_map,
         "Ref": ref,
     },
     "Fn::GetAtt": {},  # This one is complicated =/
     "Fn::GetAZs": {
```

### Comparing `cf2tf-0.6.3a27/src/cf2tf/conversion/overrides.py` & `cf2tf-0.7.0a0/src/cf2tf/conversion/overrides.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/convert.py` & `cf2tf-0.7.0a0/src/cf2tf/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,18 +169,15 @@
 
                 if key == "Ref":
                     return functions.ref(self, value)
 
                 # This takes care of keys that not intrinsic functions,
                 #  except for the condition func
                 if "Fn::" not in key and key != "Condition":
-                    data[key] = self.resolve_values(
-                        value,
-                        allowed_func,
-                    )
+                    data[key] = self.resolve_values(value, allowed_func, prev_func)
                     continue
 
                 # Takes care of the tricky 'Condition' key
                 if key == "Condition":
                     # The real fix is to not resolve every key/value in the entire
                     # cloudformation template. We should only attempt to resolve what is needed,
                     # like outputs and resource properties.
@@ -190,31 +187,32 @@
                         continue
 
                     # If it's an intrinsic func
                     if is_condition_func(value):
                         return functions.condition(self, value)
 
                     # Normal key like in an IAM role
-                    data[key] = self.resolve_values(
-                        value,
-                        allowed_func,
-                    )
+                    data[key] = self.resolve_values(value, allowed_func, prev_func)
                     continue
 
                 if key not in allowed_func:
                     raise ValueError(f"{key} not allowed to be nested in {prev_func}.")
 
+                prev_func = key
+
                 value = self.resolve_values(
-                    value, functions.ALLOWED_FUNCTIONS[key], key
+                    value, functions.ALLOWED_FUNCTIONS[key], prev_func
                 )
 
                 try:
                     return allowed_func[key](self, value)
-                except Exception:
-                    return CommentType(f"Unable to resolve {key} with value: {value}")
+                except Exception as e:
+                    return CommentType(
+                        f"Unable to resolve {key} with value: {value} because {e}"
+                    )
 
             return MapType(data)
         elif isinstance(data, list):
             resolved_list_values = [
                 self.resolve_values(item, allowed_func, prev_func) for item in data
             ]
```

### Comparing `cf2tf-0.6.3a27/src/cf2tf/save.py` & `cf2tf-0.7.0a0/src/cf2tf/save.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/blocks.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/blocks.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/code.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/code.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/doc_file.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.6.3a27/PKG-INFO` & `cf2tf-0.7.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.6.3a27
+Version: 0.7.0a0
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.6.3a27 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.7.0a0 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

