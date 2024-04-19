# Comparing `tmp/crc-6.1.2.tar.gz` & `tmp/crc-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-6.1.2.tar", max compression
+gzip compressed data, was "crc-7.0.0.tar", max compression
```

## Comparing `crc-6.1.2.tar` & `crc-7.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1305 2024-04-14 09:08:43.976723 crc-6.1.2/LICENSE.txt
--rw-r--r--   0        0        0     4471 2024-04-14 09:08:43.976723 crc-6.1.2/README.md
--rw-r--r--   0        0        0     1779 2024-04-14 09:08:43.980723 crc-6.1.2/pyproject.toml
--rw-r--r--   0        0        0      437 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/__init__.py
--rw-r--r--   0        0        0      208 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/__main__.py
--rw-r--r--   0        0        0    16895 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/_crc.py
--rw-r--r--   0        0        0        0 2024-04-14 09:08:43.980723 crc-6.1.2/src/crc/py.typed
--rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 crc-6.1.2/setup.py
--rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 crc-6.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1305 2024-04-19 16:25:50.883526 crc-7.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4604 2024-04-19 16:25:50.883526 crc-7.0.0/README.md
+-rw-r--r--   0        0        0     2050 2024-04-19 16:25:50.887526 crc-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0      437 2024-04-19 16:25:50.887526 crc-7.0.0/src/crc/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-19 16:25:50.887526 crc-7.0.0/src/crc/__main__.py
+-rw-r--r--   0        0        0    17092 2024-04-19 16:25:50.887526 crc-7.0.0/src/crc/_crc.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:25:50.887526 crc-7.0.0/src/crc/py.typed
+-rw-r--r--   0        0        0     5569 1970-01-01 00:00:00.000000 crc-7.0.0/setup.py
+-rw-r--r--   0        0        0     5998 1970-01-01 00:00:00.000000 crc-7.0.0/PKG-INFO
```

### Comparing `crc-6.1.2/LICENSE.txt` & `crc-7.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crc-6.1.2/README.md` & `crc-7.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,21 +30,22 @@
 * Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)
 * Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)
 ---
 
 ## Available CRC Configurations
 For convenience various frequently used crc configurations ship with the library out of the box.
 
-| CRC8 | CRC16    | CRC32 | CRC64 |
-|------|----------|-------|-------|
-| CCITT | CCITT    | CRC32 | CRC64 |
-| AUTOSAR | GSM      | AUTOSAR | |
-| SAEJ1850 | PROFIBUS | BZIP2 | |
-| BLUETOOTH | MODBUS   | POSIX | |
-| MAXIM-DOW | IBM-3740 | | | |
+| CRC8          | CRC16    | CRC32   | CRC64 |
+|---------------|----------|---------|-------|
+| CCITT         | XMODEM   | CRC32   | CRC64 |
+| AUTOSAR       | GSM      | AUTOSAR |       |
+| SAEJ1850      | PROFIBUS | BZIP2   |       |
+| SAEJ1850_ZERO | MODBUS   | POSIX   |       |
+| BLUETOOTH     | IBM-3740 |         |       |
+| MAXIM-DOW     | KERMIT   |         |       | 
 
 If you find yourself in the position, where having a new configuration available out of the
 box would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).
 
 ## Custom Configurations
 
 If you want to create a custom configuration, you should have the following information available:
```

#### html2text {}

```diff
@@ -3,34 +3,34 @@
                            custom CRC configurations
  _[_C_h_e_c_k_s_ _M_a_s_t_e_r_]_[_C_o_v_e_r_a_g_e_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_y_P_i
                                    _P_a_c_k_a_g_e_]
 --- * Documentation: [https://nicoretti.github.io/crc](https://
 nicoretti.github.io/crc) * Source Code: [https://github.com/Nicoretti/crc]
 (https://github.com/Nicoretti/crc) --- ## Available CRC Configurations For
 convenience various frequently used crc configurations ship with the library
-out of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |------|----------|-------|---
-----| | CCITT | CCITT | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR | | |
-SAEJ1850 | PROFIBUS | BZIP2 | | | BLUETOOTH | MODBUS | POSIX | | | MAXIM-DOW |
-IBM-3740 | | | | If you find yourself in the position, where having a new
-configuration available out of the box would be desirable, feel free to create
-a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://
-github.com/Nicoretti/crc/issues). ## Custom Configurations If you want to
-create a custom configuration, you should have the following information
-available: ð Note: This library currently only supports bit widths of full
-bytes 8, 16, 24, 32, ... * **width** * **polynom** * **init value** * **final
-xor value** * **reversed input** * **reversed output** In case you only have a
-name of a specific crc configuration/algorithm and you are unsure what are the
-specific parameters of it, a look into this [crc-catalogue](http://
-reveng.sourceforge.net/crc-catalogue/all.htm) might help. ## Requirements *
-[\>= Python 3.8](https://www.python.org) ## Installation ```shell pip install
-crc ``` ## Examples ### Create a Calculator #### Pre defined configuration
-```python from crc import Calculator, Crc8 calculator = Calculator(Crc8.CCITT)
-``` #### Custom configuration ```python from crc import Calculator,
-Configuration config = Configuration( width=8, polynomial=0x07,
-init_value=0x00, final_xor_value=0x00, reverse_input=False,
+out of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |---------------|----------|--
+-------|-------| | CCITT | XMODEM | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR |
+| | SAEJ1850 | PROFIBUS | BZIP2 | | | SAEJ1850_ZERO | MODBUS | POSIX | | |
+BLUETOOTH | IBM-3740 | | | | MAXIM-DOW | KERMIT | | | If you find yourself in
+the position, where having a new configuration available out of the box would
+be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/
+pulls) or file an [issue](https://github.com/Nicoretti/crc/issues). ## Custom
+Configurations If you want to create a custom configuration, you should have
+the following information available: ð Note: This library currently only
+supports bit widths of full bytes 8, 16, 24, 32, ... * **width** * **polynom**
+* **init value** * **final xor value** * **reversed input** * **reversed
+output** In case you only have a name of a specific crc configuration/algorithm
+and you are unsure what are the specific parameters of it, a look into this
+[crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might
+help. ## Requirements * [\>= Python 3.8](https://www.python.org) ##
+Installation ```shell pip install crc ``` ## Examples ### Create a Calculator
+#### Pre defined configuration ```python from crc import Calculator, Crc8
+calculator = Calculator(Crc8.CCITT) ``` #### Custom configuration ```python
+from crc import Calculator, Configuration config = Configuration( width=8,
+polynomial=0x07, init_value=0x00, final_xor_value=0x00, reverse_input=False,
 reverse_output=False, ) calculator = Calculator(config) ``` ### Calculate a
 checksum #### Standard ```python from crc import Calculator, Crc8 expected =
 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT)
 assert expected == calculator.checksum(data) ``` #### Optimized for speed
 ```python from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1,
 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT, optimized=True) assert
 expected == calculator.checksum(data) ``` ### Verify a checksum #### Standard
```

### Comparing `crc-6.1.2/pyproject.toml` & `crc-7.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 [tool.poetry]
 name = "crc"
-version = "6.1.2"
+version = "7.0.0"
 description = "Library and CLI to calculate and verify all kinds of CRC checksums"
 packages = [
     { include = "crc", from = "src" },
 ]
 authors = ["Nicola Coretti <nico.coretti@gmail.com>"]
 maintainers = ["Nicola Coretti <nico.coretti@gmail.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 keywords = ['CRC', 'CRC8', 'CRC16', 'CRC32', 'CRC64']
 repository = "https://github.com/Nicoretti/crc"
 
 [tool.poetry.urls]
 "Homepage" = "https://nicoretti.github.io/crc/"
 "Documentation" = "https://nicoretti.github.io/crc/"
```

### Comparing `crc-6.1.2/src/crc/_crc.py` & `crc-7.0.0/src/crc/_crc.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,15 +477,15 @@
         reverse_input=True,
         reverse_output=True,
     )
 
 
 @enum.unique
 class Crc16(enum.Enum):
-    CCITT = Configuration(
+    XMODEM = Configuration(
         width=16,
         polynomial=0x1021,
         init_value=0x0000,
         final_xor_value=0x0000,
         reverse_input=False,
         reverse_output=False,
     )
@@ -522,14 +522,23 @@
         polynomial=0x1021,
         init_value=0xFFFF,
         final_xor_value=0x0000,
         reverse_input=False,
         reverse_output=False,
     )
 
+    KERMIT = Configuration(
+        width=16,
+        polynomial=0x1021,
+        init_value=0x0000,
+        final_xor_value=0x0000,
+        reverse_input=True,
+        reverse_output=True,
+    )
+
 
 @enum.unique
 class Crc32(enum.Enum):
     CRC32 = Configuration(
         width=32,
         polynomial=0x04C11DB7,
         init_value=0xFFFFFFFF,
```

### Comparing `crc-6.1.2/setup.py` & `crc-7.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['crc = crc._crc:main']}
 
 setup_kwargs = {
     'name': 'crc',
-    'version': '6.1.2',
+    'version': '7.0.0',
     'description': 'Library and CLI to calculate and verify all kinds of CRC checksums',
-    'long_description': '<h1 align="center">CRC</h1>\n<p align="center">\n\nCalculate CRC checksums, verify CRC checksum, predefined CRC configurations, custom CRC configurations\n</p>\n\n<p align="center">\n\n<a href="https://github.com/Nicoretti/crc/actions">\n    <img src="https://img.shields.io/github/checks-status/nicoretti/crc/master" alt="Checks Master">\n</a>\n<a href="https://coveralls.io/github/Nicoretti/crc">\n    <img src="https://img.shields.io/coverallsCoverage/github/Nicoretti/crc" alt="Coverage">\n</a>\n<a href="https://opensource.org/licenses/BSD-2-Clause">\n    <img src="https://img.shields.io/pypi/l/crc" alt="License">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/dm/crc" alt="Downloads">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/pyversions/crc" alt="Supported Python Versions">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/v/crc" alt="PyPi Package">\n</a>\n</p>\n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor convenience various frequently used crc configurations ship with the library out of the box.\n\n| CRC8 | CRC16    | CRC32 | CRC64 |\n|------|----------|-------|-------|\n| CCITT | CCITT    | CRC32 | CRC64 |\n| AUTOSAR | GSM      | AUTOSAR | |\n| SAEJ1850 | PROFIBUS | BZIP2 | |\n| BLUETOOTH | MODBUS   | POSIX | |\n| MAXIM-DOW | IBM-3740 | | | |\n\nIf you find yourself in the position, where having a new configuration available out of the\nbox would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to create a custom configuration, you should have the following information available:\n\n🗒 Note:\n\n    This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n* **final xor value**\n* **reversed input**\n* **reversed output**\n\nIn case you only have a name of a specific crc configuration/algorithm and you are unsure what are the specific parameters\nof it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig = Configuration(\n    width=8,\n    polynomial=0x07,\n    init_value=0x00,\n    final_xor_value=0x00,\n    reverse_input=False,\n    reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected == calculator.checksum(data)\n```\n\n### Verify a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert calculator.verify(data, expected)\n```\n\n### Calculate a checksum with raw registers\n\n#### Register\n\n```python\nfrom crc import Crc8, Register\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = Register(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n#### TableBasedRegister\n\n```python\nfrom crc import Crc8, TableBasedRegister\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = TableBasedRegister(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n\nReferences & Resources\n-----------------------\n* [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)\n* [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n',
+    'long_description': '<h1 align="center">CRC</h1>\n<p align="center">\n\nCalculate CRC checksums, verify CRC checksum, predefined CRC configurations, custom CRC configurations\n</p>\n\n<p align="center">\n\n<a href="https://github.com/Nicoretti/crc/actions">\n    <img src="https://img.shields.io/github/checks-status/nicoretti/crc/master" alt="Checks Master">\n</a>\n<a href="https://coveralls.io/github/Nicoretti/crc">\n    <img src="https://img.shields.io/coverallsCoverage/github/Nicoretti/crc" alt="Coverage">\n</a>\n<a href="https://opensource.org/licenses/BSD-2-Clause">\n    <img src="https://img.shields.io/pypi/l/crc" alt="License">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/dm/crc" alt="Downloads">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/pyversions/crc" alt="Supported Python Versions">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/v/crc" alt="PyPi Package">\n</a>\n</p>\n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor convenience various frequently used crc configurations ship with the library out of the box.\n\n| CRC8          | CRC16    | CRC32   | CRC64 |\n|---------------|----------|---------|-------|\n| CCITT         | XMODEM   | CRC32   | CRC64 |\n| AUTOSAR       | GSM      | AUTOSAR |       |\n| SAEJ1850      | PROFIBUS | BZIP2   |       |\n| SAEJ1850_ZERO | MODBUS   | POSIX   |       |\n| BLUETOOTH     | IBM-3740 |         |       |\n| MAXIM-DOW     | KERMIT   |         |       | \n\nIf you find yourself in the position, where having a new configuration available out of the\nbox would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to create a custom configuration, you should have the following information available:\n\n🗒 Note:\n\n    This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n* **final xor value**\n* **reversed input**\n* **reversed output**\n\nIn case you only have a name of a specific crc configuration/algorithm and you are unsure what are the specific parameters\nof it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig = Configuration(\n    width=8,\n    polynomial=0x07,\n    init_value=0x00,\n    final_xor_value=0x00,\n    reverse_input=False,\n    reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected == calculator.checksum(data)\n```\n\n### Verify a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert calculator.verify(data, expected)\n```\n\n### Calculate a checksum with raw registers\n\n#### Register\n\n```python\nfrom crc import Crc8, Register\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = Register(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n#### TableBasedRegister\n\n```python\nfrom crc import Crc8, TableBasedRegister\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = TableBasedRegister(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n\nReferences & Resources\n-----------------------\n* [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)\n* [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n',
     'author': 'Nicola Coretti',
     'author_email': 'nico.coretti@gmail.com',
     'maintainer': 'Nicola Coretti',
     'maintainer_email': 'nico.coretti@gmail.com',
     'url': 'https://github.com/Nicoretti/crc',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['crc'] package_data = \ {'': ['*']} entry_points = \
 {'console_scripts': ['crc = crc._crc:main']} setup_kwargs = { 'name': 'crc',
-'version': '6.1.2', 'description': 'Library and CLI to calculate and verify all
+'version': '7.0.0', 'description': 'Library and CLI to calculate and verify all
 kinds of CRC checksums', 'long_description': '
                                ************ CCRRCC ************
 \n
        \n\nCalculate CRC checksums, verify CRC checksum, predefined CRC
                   configurations, custom CRC configurations\n
 \n\n
 \n\n_\_n_ _[_C_h_e_c_k_s_ _M_a_s_t_e_r_]_\_n\n_\_n_ _[_C_o_v_e_r_a_g_e_]_\_n\n_\_n_ _[_L_i_c_e_n_s_e_]_\_n\n_\_n_ _[_D_o_w_n_l_o_a_d_s_]_\_n\n_\_n
              _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_\_n\n_\_n_ _[_P_y_P_i_ _P_a_c_k_a_g_e_]_\_n\n
 \n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://
 nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc]
 (https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor
 convenience various frequently used crc configurations ship with the library
-out of the box.\n\n| CRC8 | CRC16 | CRC32 | CRC64 |\n|------|----------|-------
-|-------|\n| CCITT | CCITT | CRC32 | CRC64 |\n| AUTOSAR | GSM | AUTOSAR | |\n|
-SAEJ1850 | PROFIBUS | BZIP2 | |\n| BLUETOOTH | MODBUS | POSIX | |\n| MAXIM-DOW
-| IBM-3740 | | | |\n\nIf you find yourself in the position, where having a new
-configuration available out of the\nbox would be desirable, feel free to create
-a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://
-github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to
-create a custom configuration, you should have the following information
-available:\n\nð Note:\n\n This library currently only supports bit widths of
-full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init
-value**\n* **final xor value**\n* **reversed input**\n* **reversed
-output**\n\nIn case you only have a name of a specific crc configuration/
-algorithm and you are unsure what are the specific parameters\nof it, a look
-into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)
-might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://
-www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n##
-Examples\n\n### Create a Calculator\n\n#### Pre defined
-configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator =
-Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc
-import Calculator, Configuration\n\nconfig = Configuration(\n width=8,\n
-polynomial=0x07,\n init_value=0x00,\n final_xor_value=0x00,\n
-reverse_input=False,\n reverse_output=False,\n)\n\ncalculator = Calculator
-(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom
-crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
-5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected ==
-calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom
-crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
+out of the box.\n\n| CRC8 | CRC16 | CRC32 | CRC64 |\n|---------------|---------
+-|---------|-------|\n| CCITT | XMODEM | CRC32 | CRC64 |\n| AUTOSAR | GSM |
+AUTOSAR | |\n| SAEJ1850 | PROFIBUS | BZIP2 | |\n| SAEJ1850_ZERO | MODBUS |
+POSIX | |\n| BLUETOOTH | IBM-3740 | | |\n| MAXIM-DOW | KERMIT | | | \n\nIf you
+find yourself in the position, where having a new configuration available out
+of the\nbox would be desirable, feel free to create a [PR](https://github.com/
+Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/
+issues).\n\n## Custom Configurations\n\nIf you want to create a custom
+configuration, you should have the following information available:\n\nð
+Note:\n\n This library currently only supports bit widths of full bytes 8, 16,
+24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n* **final xor
+value**\n* **reversed input**\n* **reversed output**\n\nIn case you only have a
+name of a specific crc configuration/algorithm and you are unsure what are the
+specific parameters\nof it, a look into this [crc-catalogue](http://
+reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n##
+Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n##
+Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a
+Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import
+Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom
+configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig
+= Configuration(\n width=8,\n polynomial=0x07,\n init_value=0x00,\n
+final_xor_value=0x00,\n reverse_input=False,\n
+reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n###
+Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator,
+Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator =
+Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum
+(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import
+Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected ==
 calculator.checksum(data)\n```\n\n### Verify a checksum\n\n####
 Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected =
 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator
 (Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized
 for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected =
 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT,
```

### Comparing `crc-6.1.2/PKG-INFO` & `crc-7.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc
-Version: 6.1.2
+Version: 7.0.0
 Summary: Library and CLI to calculate and verify all kinds of CRC checksums
 Home-page: https://github.com/Nicoretti/crc
 License: BSD-2-Clause
 Keywords: CRC,CRC8,CRC16,CRC32,CRC64
 Author: Nicola Coretti
 Author-email: nico.coretti@gmail.com
 Maintainer: Nicola Coretti
@@ -12,14 +12,20 @@
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Project-URL: Changelog, https://nicoretti.github.io/crc/changelog/unreleased/
 Project-URL: Documentation, https://nicoretti.github.io/crc/
 Project-URL: Homepage, https://nicoretti.github.io/crc/
 Project-URL: Issues, https://github.com/Nicoretti/crc/issues
 Project-URL: Repository, https://github.com/Nicoretti/crc
 Project-URL: Source, https://github.com/Nicoretti/crc
 Description-Content-Type: text/markdown
@@ -56,21 +62,22 @@
 * Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)
 * Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)
 ---
 
 ## Available CRC Configurations
 For convenience various frequently used crc configurations ship with the library out of the box.
 
-| CRC8 | CRC16    | CRC32 | CRC64 |
-|------|----------|-------|-------|
-| CCITT | CCITT    | CRC32 | CRC64 |
-| AUTOSAR | GSM      | AUTOSAR | |
-| SAEJ1850 | PROFIBUS | BZIP2 | |
-| BLUETOOTH | MODBUS   | POSIX | |
-| MAXIM-DOW | IBM-3740 | | | |
+| CRC8          | CRC16    | CRC32   | CRC64 |
+|---------------|----------|---------|-------|
+| CCITT         | XMODEM   | CRC32   | CRC64 |
+| AUTOSAR       | GSM      | AUTOSAR |       |
+| SAEJ1850      | PROFIBUS | BZIP2   |       |
+| SAEJ1850_ZERO | MODBUS   | POSIX   |       |
+| BLUETOOTH     | IBM-3740 |         |       |
+| MAXIM-DOW     | KERMIT   |         |       | 
 
 If you find yourself in the position, where having a new configuration available out of the
 box would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).
 
 ## Custom Configurations
 
 If you want to create a custom configuration, you should have the following information available:
```

#### html2text {}

```diff
@@ -1,16 +1,20 @@
-Metadata-Version: 2.1 Name: crc Version: 6.1.2 Summary: Library and CLI to
+Metadata-Version: 2.1 Name: crc Version: 7.0.0 Summary: Library and CLI to
 calculate and verify all kinds of CRC checksums Home-page: https://github.com/
 Nicoretti/crc License: BSD-2-Clause Keywords: CRC,CRC8,CRC16,CRC32,CRC64
 Author: Nicola Coretti Author-email: nico.coretti@gmail.com Maintainer: Nicola
 Coretti Maintainer-email: nico.coretti@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Changelog, https://nicoretti.github.io/crc/changelog/unreleased/
 Project-URL: Documentation, https://nicoretti.github.io/crc/ Project-URL:
 Homepage, https://nicoretti.github.io/crc/ Project-URL: Issues, https://
 github.com/Nicoretti/crc/issues Project-URL: Repository, https://github.com/
 Nicoretti/crc Project-URL: Source, https://github.com/Nicoretti/crc
 Description-Content-Type: text/markdown
                                ************ CCRRCC ************
@@ -18,34 +22,34 @@
                            custom CRC configurations
  _[_C_h_e_c_k_s_ _M_a_s_t_e_r_]_[_C_o_v_e_r_a_g_e_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_y_P_i
                                    _P_a_c_k_a_g_e_]
 --- * Documentation: [https://nicoretti.github.io/crc](https://
 nicoretti.github.io/crc) * Source Code: [https://github.com/Nicoretti/crc]
 (https://github.com/Nicoretti/crc) --- ## Available CRC Configurations For
 convenience various frequently used crc configurations ship with the library
-out of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |------|----------|-------|---
-----| | CCITT | CCITT | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR | | |
-SAEJ1850 | PROFIBUS | BZIP2 | | | BLUETOOTH | MODBUS | POSIX | | | MAXIM-DOW |
-IBM-3740 | | | | If you find yourself in the position, where having a new
-configuration available out of the box would be desirable, feel free to create
-a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://
-github.com/Nicoretti/crc/issues). ## Custom Configurations If you want to
-create a custom configuration, you should have the following information
-available: ð Note: This library currently only supports bit widths of full
-bytes 8, 16, 24, 32, ... * **width** * **polynom** * **init value** * **final
-xor value** * **reversed input** * **reversed output** In case you only have a
-name of a specific crc configuration/algorithm and you are unsure what are the
-specific parameters of it, a look into this [crc-catalogue](http://
-reveng.sourceforge.net/crc-catalogue/all.htm) might help. ## Requirements *
-[\>= Python 3.8](https://www.python.org) ## Installation ```shell pip install
-crc ``` ## Examples ### Create a Calculator #### Pre defined configuration
-```python from crc import Calculator, Crc8 calculator = Calculator(Crc8.CCITT)
-``` #### Custom configuration ```python from crc import Calculator,
-Configuration config = Configuration( width=8, polynomial=0x07,
-init_value=0x00, final_xor_value=0x00, reverse_input=False,
+out of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |---------------|----------|--
+-------|-------| | CCITT | XMODEM | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR |
+| | SAEJ1850 | PROFIBUS | BZIP2 | | | SAEJ1850_ZERO | MODBUS | POSIX | | |
+BLUETOOTH | IBM-3740 | | | | MAXIM-DOW | KERMIT | | | If you find yourself in
+the position, where having a new configuration available out of the box would
+be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/
+pulls) or file an [issue](https://github.com/Nicoretti/crc/issues). ## Custom
+Configurations If you want to create a custom configuration, you should have
+the following information available: ð Note: This library currently only
+supports bit widths of full bytes 8, 16, 24, 32, ... * **width** * **polynom**
+* **init value** * **final xor value** * **reversed input** * **reversed
+output** In case you only have a name of a specific crc configuration/algorithm
+and you are unsure what are the specific parameters of it, a look into this
+[crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might
+help. ## Requirements * [\>= Python 3.8](https://www.python.org) ##
+Installation ```shell pip install crc ``` ## Examples ### Create a Calculator
+#### Pre defined configuration ```python from crc import Calculator, Crc8
+calculator = Calculator(Crc8.CCITT) ``` #### Custom configuration ```python
+from crc import Calculator, Configuration config = Configuration( width=8,
+polynomial=0x07, init_value=0x00, final_xor_value=0x00, reverse_input=False,
 reverse_output=False, ) calculator = Calculator(config) ``` ### Calculate a
 checksum #### Standard ```python from crc import Calculator, Crc8 expected =
 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT)
 assert expected == calculator.checksum(data) ``` #### Optimized for speed
 ```python from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1,
 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT, optimized=True) assert
 expected == calculator.checksum(data) ``` ### Verify a checksum #### Standard
```

