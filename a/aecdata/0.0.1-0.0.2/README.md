# Comparing `tmp/aecdata-0.0.1.tar.gz` & `tmp/aecdata-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aecdata-0.0.1.tar", last modified: Wed Apr 17 06:54:24 2024, max compression
+gzip compressed data, was "aecdata-0.0.2.tar", last modified: Fri Apr 19 12:57:45 2024, max compression
```

## Comparing `aecdata-0.0.1.tar` & `aecdata-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-17 06:54:24.256415 aecdata-0.0.1/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.1/LICENSE
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16143 2024-04-17 06:54:24.256192 aecdata-0.0.1/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    15540 2024-04-17 06:51:34.000000 aecdata-0.0.1/README.md
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-17 06:54:24.254813 aecdata-0.0.1/aecdata/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.1/aecdata/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2402 2024-04-03 12:58:03.000000 aecdata-0.0.1/aecdata/auth.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9211 2024-04-05 12:23:40.000000 aecdata-0.0.1/aecdata/client.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    40078 2024-04-09 10:55:04.000000 aecdata-0.0.1/aecdata/productdata.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20904 2024-04-12 08:29:30.000000 aecdata-0.0.1/aecdata/utils.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-17 06:54:24.255976 aecdata-0.0.1/aecdata.egg-info/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16143 2024-04-17 06:54:24.000000 aecdata-0.0.1/aecdata.egg-info/PKG-INFO
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-04-17 06:54:24.000000 aecdata-0.0.1/aecdata.egg-info/SOURCES.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-04-17 06:54:24.000000 aecdata-0.0.1/aecdata.egg-info/dependency_links.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       41 2024-04-17 06:54:24.000000 aecdata-0.0.1/aecdata.egg-info/requires.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-04-17 06:54:24.000000 aecdata-0.0.1/aecdata.egg-info/top_level.txt
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-04-17 06:54:24.256453 aecdata-0.0.1/setup.cfg
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      771 2024-04-17 06:45:32.000000 aecdata-0.0.1/setup.py
-drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-17 06:54:24.255824 aecdata-0.0.1/tests/
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.1/tests/__init__.py
--rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.1/tests/test_client.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.620832 aecdata-0.0.2/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      554 2024-04-04 08:44:04.000000 aecdata-0.0.2/LICENSE
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16101 2024-04-19 12:57:45.620582 aecdata-0.0.2/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    15498 2024-04-17 08:11:11.000000 aecdata-0.0.2/README.md
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.619196 aecdata-0.0.2/aecdata/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      104 2024-04-03 12:58:03.000000 aecdata-0.0.2/aecdata/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     2402 2024-04-03 12:58:03.000000 aecdata-0.0.2/aecdata/auth.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)     9211 2024-04-05 12:23:40.000000 aecdata-0.0.2/aecdata/client.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    40812 2024-04-19 09:03:16.000000 aecdata-0.0.2/aecdata/productdata.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    20904 2024-04-12 08:29:30.000000 aecdata-0.0.2/aecdata/utils.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.620348 aecdata-0.0.2/aecdata.egg-info/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)    16101 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/PKG-INFO
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      313 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/SOURCES.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        1 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/dependency_links.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       41 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/requires.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       14 2024-04-19 12:57:45.000000 aecdata-0.0.2/aecdata.egg-info/top_level.txt
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)       38 2024-04-19 12:57:45.620883 aecdata-0.0.2/setup.cfg
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)      771 2024-04-19 12:57:11.000000 aecdata-0.0.2/setup.py
+drwxr-xr-x   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-19 12:57:45.620199 aecdata-0.0.2/tests/
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.2/tests/__init__.py
+-rw-r--r--   0 nicodemosvarnava   (501) staff       (20)        0 2024-04-03 12:58:03.000000 aecdata-0.0.2/tests/test_client.py
```

### Comparing `aecdata-0.0.1/LICENSE` & `aecdata-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.1/PKG-INFO` & `aecdata-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,17 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 
-# 2050 Materials API Client
+# AECData
 
-The 2050 Materials API Client is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
+AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
 - **Flexible Data Retrieval**: Supports fetching data using customizable filters to meet diverse analysis needs.
 - **Data Manipulation and Analysis**: Offers tools for transforming, scaling, and statistically analyzing the data.
 - **Visualization Support**: Provides functionalities for visualizing data distributions and product contributions.
@@ -39,15 +39,15 @@
 3. **Data Manipulation**: Once you have fetched the data, you can construct a `ProductData` object. This object allows for extensive manipulation and transformation of the data, enabling you to prepare it for analysis or visualization in a format that suits your requirements.
    
 4. **Statistical Analysis and Visualization**: For advanced data analysis, the `ProductStatistics` class extends `ProductData` to provide statistical insights. It enables outlier removal, distribution analysis, and more, coupled with visualization capabilities to help interpret the data effectively.
 
 
 ## Installation
 
-The `aecdata` library can be installed directly from PyPI to ensure you have the latest version. Use the following pip command:
+The AECData library can be installed directly from PyPI to ensure you have the latest version. Use the following pip command:
 
 ```
 pip install aecdata
 ```
 
 For source code, issues, and contributions, the project is hosted on GitHub at:
```

### Comparing `aecdata-0.0.1/README.md` & `aecdata-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# 2050 Materials API Client
+# AECData
 
-The 2050 Materials API Client is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
+AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
 - **Flexible Data Retrieval**: Supports fetching data using customizable filters to meet diverse analysis needs.
 - **Data Manipulation and Analysis**: Offers tools for transforming, scaling, and statistically analyzing the data.
 - **Visualization Support**: Provides functionalities for visualizing data distributions and product contributions.
@@ -20,15 +20,15 @@
 3. **Data Manipulation**: Once you have fetched the data, you can construct a `ProductData` object. This object allows for extensive manipulation and transformation of the data, enabling you to prepare it for analysis or visualization in a format that suits your requirements.
    
 4. **Statistical Analysis and Visualization**: For advanced data analysis, the `ProductStatistics` class extends `ProductData` to provide statistical insights. It enables outlier removal, distribution analysis, and more, coupled with visualization capabilities to help interpret the data effectively.
 
 
 ## Installation
 
-The `aecdata` library can be installed directly from PyPI to ensure you have the latest version. Use the following pip command:
+The AECData library can be installed directly from PyPI to ensure you have the latest version. Use the following pip command:
 
 ```
 pip install aecdata
 ```
 
 For source code, issues, and contributions, the project is hosted on GitHub at:
```

### Comparing `aecdata-0.0.1/aecdata/auth.py` & `aecdata-0.0.2/aecdata/auth.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.1/aecdata/client.py` & `aecdata-0.0.2/aecdata/client.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.1/aecdata/productdata.py` & `aecdata-0.0.2/aecdata/productdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,23 +439,35 @@
         return epdx_products_list
 
     def filter_df_by_dict(self, df, filter_dict):
         # Start with the full DataFrame
         filtered_df = df
         # Apply each filter
         for key, value in filter_dict.items():
-            # Check if the column contains lists
-            if df[key].apply(lambda x: isinstance(x, list)).any():
-                # Use apply() to filter rows where the list contains the value
-                filtered_df = filtered_df[filtered_df[key].apply(lambda x: any(value in str(item) for item in x) if x is not None else False)]
+            if isinstance(value, list):
+                # If value is a list, filter using 'isin' for direct matches
+                # or check list columns for any item in the list values
+                if df[key].apply(lambda x: isinstance(x, list)).any():
+                    # Check if any item from the list in 'value' is in any list in the DataFrame
+                    filtered_df = filtered_df[
+                        filtered_df[key].apply(lambda x: any(item in x for item in value) if x is not None else False)]
+                else:
+                    # For normal columns, filter where the column's value is in 'value' list
+                    filtered_df = filtered_df[filtered_df[key].isin(value)]
             else:
-                # If the column does not contain lists, filter normally
-                filtered_df = filtered_df[filtered_df[key] == value]
+                # Check if the column contains lists
+                if df[key].apply(lambda x: isinstance(x, list)).any():
+                    # Use apply() to filter rows where the list contains the value
+                    filtered_df = filtered_df[filtered_df[key].apply(lambda x: value in x if x is not None else False)]
+                else:
+                    # If the column does not contain lists, filter normally
+                    filtered_df = filtered_df[filtered_df[key] == value]
         return filtered_df
 
+
 class ProductStatistics(ProductData):
     def __init__(self, data, unit='declared_unit'):
         # Check if the input is a ProductData instance
         if isinstance(data, ProductData):
             # Directly use the DataFrame from the ProductData instance
             self.dataframe = data.dataframe.copy()  # Make a copy to ensure independence
             self.data = data.data  # Assuming you want to also copy the original data structure
@@ -890,11 +902,10 @@
         plt.xticks(fontsize=12, rotation=45)  # Rotate labels if there are many groups
         plt.yticks(fontsize=12)
         plt.title(f'Distribution of {field} by {group_by_field}', fontsize=15)
         plt.show()
 
     def get_field_distribution_boxplot(self, field, group_by_field, filters=None, include_estimated_values=False, remove_outliers=True, method='IQR', sqrt_tranf=True):
         df = self.filter_dataframe_based_on_field(field, filters, include_estimated_values, remove_outliers, method, sqrt_tranf)
-
         # After preparing and filtering the DataFrame, plot it
         self.plot_distribution_boxplot(df, field, group_by_field)
```

### Comparing `aecdata-0.0.1/aecdata/utils.py` & `aecdata-0.0.2/aecdata/utils.py`

 * *Files identical despite different names*

### Comparing `aecdata-0.0.1/aecdata.egg-info/PKG-INFO` & `aecdata-0.0.2/aecdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aecdata
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library designed to simplify access to the 2050-materials API
 Home-page: https://github.com/2050-Materials/aecdata
 Author: 2050 Materials
 Author-email: nicodemos@2050-materials.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,17 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: pyarrow
 
-# 2050 Materials API Client
+# AECData
 
-The 2050 Materials API Client is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
+AECData is a Python library designed to facilitate seamless interaction with the 2050-materials platform API. By abstracting the complexities of authentication and data retrieval, this library empowers developers to focus on analyzing and utilizing environmental data about construction materials effectively.
 
 ## Key Features
 
 - **Simplified Authentication**: Manages API tokens automatically, streamlining the authentication process.
 - **Flexible Data Retrieval**: Supports fetching data using customizable filters to meet diverse analysis needs.
 - **Data Manipulation and Analysis**: Offers tools for transforming, scaling, and statistically analyzing the data.
 - **Visualization Support**: Provides functionalities for visualizing data distributions and product contributions.
@@ -39,15 +39,15 @@
 3. **Data Manipulation**: Once you have fetched the data, you can construct a `ProductData` object. This object allows for extensive manipulation and transformation of the data, enabling you to prepare it for analysis or visualization in a format that suits your requirements.
    
 4. **Statistical Analysis and Visualization**: For advanced data analysis, the `ProductStatistics` class extends `ProductData` to provide statistical insights. It enables outlier removal, distribution analysis, and more, coupled with visualization capabilities to help interpret the data effectively.
 
 
 ## Installation
 
-The `aecdata` library can be installed directly from PyPI to ensure you have the latest version. Use the following pip command:
+The AECData library can be installed directly from PyPI to ensure you have the latest version. Use the following pip command:
 
 ```
 pip install aecdata
 ```
 
 For source code, issues, and contributions, the project is hosted on GitHub at:
```

### Comparing `aecdata-0.0.1/setup.py` & `aecdata-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aecdata",
-    version="0.0.1",
+    version="0.0.2",
     author="2050 Materials",
     license="Apache License 2.0",
     author_email="nicodemos@2050-materials.com",
     description="A Python library designed to simplify access to the 2050-materials API",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/2050-Materials/aecdata",
```

