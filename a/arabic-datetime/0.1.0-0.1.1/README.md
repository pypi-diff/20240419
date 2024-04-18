# Comparing `tmp/arabic_datetime-0.1.0.tar.gz` & `tmp/arabic_datetime-0.1.1.tar.gz`

## Comparing `arabic_datetime-0.1.0.tar` & `arabic_datetime-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/__init__.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/arabic_date.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/arabic_time.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/arabic_datetime/constants.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/LICENSE
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8889 2020-02-02 00:00:00.000000 arabic_datetime-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/arabic_datetime/__init__.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/arabic_datetime/_constants.py
+-rw-r--r--   0        0        0     8781 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/arabic_datetime/arabic_date.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/arabic_datetime/arabic_time.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/README.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 arabic_datetime-0.1.1/PKG-INFO
```

### Comparing `arabic_datetime-0.1.0/arabic_datetime/arabic_date.py` & `arabic_datetime-0.1.1/arabic_datetime/arabic_date.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,97 @@
 from typing import Union
 import datetime
 
 # Import constants
-from . constants import MONTH_GROUPS, AR_NUMS
+from ._constants import MONTH_GROUPS, AR_NUMS
 
 
-class Arabic_Date:
-    def __init__(self, date_object: Union[datetime.date, datetime.datetime]) -> None:
-        if not isinstance(date_object, datetime.date) and not isinstance(date_object, datetime.datetime):
-            raise TypeError(
-                "Arabic_Date class error: The parameter provided to the instance is not a datetime.date object nor a datetime.datetime object.")
-
+class ArabicDate:
+    def __init__(self, date_object: Union[datetime.date, datetime.datetime] = None) -> None:
+        self._date_object = None
         self.date_object = date_object
 
         self.__year = str(self.date_object.year)
         self.__month = int(self.date_object.month)
         # convert first to `int` to turn 01 into 1
         self.__day = str(int(self.date_object.day))
 
         # string keys in translate table must be of length 1
         self.num_trans_table = str.maketrans(AR_NUMS)
 
+    @property
+    def date_object(self):
+        return self._date_object
+
+    @date_object.setter
+    def date_object(self, value: Union[datetime.date, datetime.datetime] = None) -> None:
+        if value == None:
+            raise TypeError(
+                f"ArabicDate class error: No parameter was passed as date_object or the parameter passed is None. Only datetime.date or datetime.datetime objects are allowed.")
+        elif not isinstance(value, datetime.date) and not isinstance(value, datetime.datetime):
+            raise TypeError(
+                f"ArabicDate class error: The parameter passed as date_object is of type {type(value)}. Only datetime.date or datetime.datetime objects are allowed.")
+        self._date_object = value
+
     # Group Name Methods
     def syriac_names(self, east_nums: bool = False) -> str:
         if not isinstance(east_nums, bool):
             raise TypeError(
-                f"Arabic_Date class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the class method '{self.syriac_names.__name__}'.")
+                f"ArabicDate class error: east_nums must be a boolean. '{east_nums}' is not a boolean and was passed to the class method '{self.syriac_names.__name__}'.")
 
         if east_nums:
             return self.__day.translate(self.num_trans_table) + " " + MONTH_GROUPS["syriac"]["months"][self.__month-1] + " " + self.__year.translate(self.num_trans_table)
         else:
             return self.__day + " " + MONTH_GROUPS["syriac"]["months"][self.__month-1] + " " + self.__year
 
     def roman1_names(self, east_nums: bool = False) -> str:
         if not isinstance(east_nums, bool):
             raise TypeError(
-                f"Arabic_Date class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the class method '{self.roman1_names.__name__}'.")
+                f"ArabicDate class error: east_nums must be a boolean. '{east_nums}' is not a boolean and was passed to the class method '{self.roman1_names.__name__}'.")
 
         if east_nums:
             return self.__day.translate(self.num_trans_table) + " " + MONTH_GROUPS["roman1"]["months"][self.__month-1] + " " + self.__year.translate(self.num_trans_table)
         else:
             return self.__day + " " + MONTH_GROUPS["roman1"]["months"][self.__month-1] + " " + self.__year
 
     def roman2_names(self, east_nums: bool = False) -> str:
         if not isinstance(east_nums, bool):
             raise TypeError(
-                f"Arabic_Date class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the class method '{self.roman2_names.__name__}'.")
+                f"ArabicDate class error: east_nums must be a boolean. '{east_nums}' is not a boolean and was passed to the class method '{self.roman2_names.__name__}'.")
 
         if east_nums:
             return self.__day.translate(self.num_trans_table) + " " + MONTH_GROUPS["roman2"]["months"][self.__month-1] + " " + self.__year.translate(self.num_trans_table)
         else:
             return self.__day + " " + MONTH_GROUPS["roman2"]["months"][self.__month-1] + " " + self.__year
 
     def french_names(self, east_nums: bool = False) -> str:
         if not isinstance(east_nums, bool):
             raise TypeError(
-                f"Arabic_Date class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the class method '{self.french_names.__name__}'.")
+                f"ArabicDate class error: east_nums must be a boolean. '{east_nums}' is not a boolean and was passed to the class method '{self.french_names.__name__}'.")
 
         if east_nums:
             return self.__day.translate(self.num_trans_table) + " " + MONTH_GROUPS["french"]["months"][self.__month-1] + " " + self.__year.translate(self.num_trans_table)
         else:
             return self.__day + " " + MONTH_GROUPS["french"]["months"][self.__month-1] + " " + self.__year
 
     # Dual Name Method
     def dual_names(self, first: str, second: str, east_nums: bool = False) -> str:
         if not isinstance(first, str):
             raise TypeError(
-                f"Arabic_Date class error: Unknown month group name: '{first}' passed as a parameter to the method '{self.dual_names.__name__}'.")
+                f"ArabicDate class error: Unknown month group name: '{first}' passed as a parameter to the method '{self.dual_names.__name__}'.")
         elif not isinstance(second, str):
             raise TypeError(
-                f"Arabic_Date class error: Unknown month group name: '{second}' passed as a parameter to the method '{self.dual_names.__name__}'.")
+                f"ArabicDate class error: Unknown month group name: '{second}' passed as a parameter to the method '{self.dual_names.__name__}'.")
         elif not isinstance(east_nums, bool):
             raise TypeError(
-                f"Arabic_Date class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the method '{self.dual_names.__name__}'.")
+                f"ArabicDate class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the method '{self.dual_names.__name__}'.")
 
         if first.strip().lower() == second.strip().lower():
             raise ValueError(
-                f"Arabic_Date class error: The first group name and the second group name sould not be identicial: '{first}' was passed as the first and the second parameter to the method {self.dual_names.__name__}. Note that these particular parameters are not case sensitive.")
+                f"ArabicDate class error: The first group name and the second group name sould not be identicial: '{first}' was passed as the first and the second parameter to the method {self.dual_names.__name__}. Note that these particular parameters are not case sensitive.")
         valid_first_group = False
         valid_second_group = False
         for group, _ in MONTH_GROUPS.items():
             if first.lower() in group:
                 valid_first_group = True
         for group, _ in MONTH_GROUPS.items():
             if second.lower() in group:
@@ -94,30 +105,30 @@
                 if error_submessage == "":
                     error_submessage += f"Unknown second groupe name '{
                         second}'"
                 else:
                     error_submessage += f" and also unknown second groupe name '{
                         second}'"
             raise ValueError(
-                f"Arabic_Date class error: {error_submessage} in the parameters passed to the method '{self.dual_names.__name__}'.")
+                f"ArabicDate class error: {error_submessage} in the parameters passed to the method '{self.dual_names.__name__}'.")
 
         if east_nums == True:
             return self.__day.translate(self.num_trans_table) + " " + MONTH_GROUPS[first]["months"][self.__month-1] + " (" + MONTH_GROUPS[second]["months"][self.__month-1] + ") " + self.__year.translate(self.num_trans_table)
         else:
             return self.__day + " " + MONTH_GROUPS[first]["months"][self.__month-1] + " (" + MONTH_GROUPS[second]["months"][self.__month-1] + ") " + self.__year
 
     # Date By Country Code Method
     def by_country_code(self, country_code: str, east_nums: bool = None) -> str:
         if not isinstance(country_code, str):
             raise TypeError(
-                f"Arabic_Date class error: The 'country_code' parameter passed to the class method '{self.by_country_code.__name__}' is not a string.")
+                f"ArabicDate class error: The 'country_code' parameter passed to the class method '{self.by_country_code.__name__}' is not a string.")
 
         elif east_nums is not None and not isinstance(east_nums, bool):
             raise TypeError(
-                f"Arabic_Date class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the class method '{self.french_names.__name__}'.")
+                f"ArabicDate class error: east_nums must be a boolean. '{east_nums}' is not boolean and was passed to the class method '{self.french_names.__name__}'.")
 
         for _, group in MONTH_GROUPS.items():
             if country_code.upper() in group["countries"]:
                 if east_nums is not None and east_nums:
                     return self.__day.translate(self.num_trans_table) + " " + group["months"][self.__month-1] + " " + self.__year.translate(self.num_trans_table)
                 elif east_nums is not None and not east_nums:
                     return self.__day + " " + group["months"][self.__month-1] + " " + self.__year
@@ -125,15 +136,15 @@
                     if group["east_nums"]:
                         return self.__day.translate(self.num_trans_table) + " " + group["months"][self.__month-1] + " " + self.__year.translate(self.num_trans_table)
                     else:
                         return self.__day + " " + group["months"][self.__month-1] + " " + self.__year
 
         else:
             raise ValueError(
-                f"Arabic_Date class error: Unknown country code '{country_code}' passed to the class method '{self.by_country_code.__name__}'.")
+                f"ArabicDate class error: Unknown country code '{country_code}' passed to the class method '{self.by_country_code.__name__}'.")
 
     # Eastern Numeric Date Method
     def eastern_numeric_date(self, separator: str = "/") -> str:
         if not isinstance(separator, str):
             raise TypeError(
-                f"Arabic_Date class error: The 'separator' parameter passed to the class method '{self.eastern_numeric_date.__name__}' is not a string.")
+                f"ArabicDate class error: The 'separator' parameter passed to the class method '{self.eastern_numeric_date.__name__}' is not a string.")
         return self.__day.translate(self.num_trans_table) + separator + str(self.__month).translate(self.num_trans_table) + separator + self.__year.translate(self.num_trans_table)
```

### Comparing `arabic_datetime-0.1.0/arabic_datetime/arabic_time.py` & `arabic_datetime-0.1.1/arabic_datetime/arabic_time.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 from typing import Union
 import datetime
 
 # Import from constants
-from . constants import AR_NUMS
+from ._constants import AR_NUMS
 
 
-class Arabic_Time:
-    def __init__(self, time_object: Union[datetime.time, datetime.datetime]) -> None:
-        if not isinstance(time_object, datetime.time) and not isinstance(time_object, datetime.datetime):
-            raise TypeError(
-                f"Arabic_Time class error: The parameter passed to the instance is not a datetime.time object nor a datetime.datetime object.")
+from typing import Union
+import datetime
 
+
+class ArabicTime:
+    def __init__(self, time_object: Union[datetime.time, datetime.datetime] = None) -> None:
+        self._time_object = None
         self.time_object = time_object
 
         # string keys in translate table must be of length 1
         self.num_trans_table = str.maketrans(AR_NUMS)
 
         # convert first to `int` to turn 01 into 1
-        self.__hour = str(int(self.time_object.hour))
-        self.__minute = str(int(self.time_object.minute))
-        self.__second = str(int(self.time_object.second))
-        self.__microsecond = str(int(self.time_object.microsecond))
+        self.__hour = str(int(self._time_object.hour))
+        self.__minute = str(int(self._time_object.minute))
+        self.__second = str(int(self._time_object.second))
+        self.__microsecond = str(int(self._time_object.microsecond))
+
+    @property
+    def time_object(self):
+        return self._time_object
+
+    @time_object.setter
+    def time_object(self, value: Union[datetime.time, datetime.datetime] = None) -> None:
+        if value == None:
+            raise TypeError(
+                f"ArabicTime class error: No parameter was passed as time_object or the parameter passed is None. Only datetime.time or datetime.datetime objects are allowed.")
+        elif not isinstance(value, datetime.time) and not isinstance(value, datetime.datetime):
+            raise TypeError(
+                f"ArabicTime class error: The parameter passed as time_object is of type {type(value)}. Only datetime.time or datetime.datetime objects are allowed.")
+        self._time_object = value
 
     def time(self, format: str = "HMS", separator: str = ":") -> str:
         if not isinstance(format, str):
             raise TypeError(
-                f"Arabic_Date class error: The 'format' parameter passed to the class method '{self.time.__name__}' is not a string.")
+                f"ArabicTime class error: The 'format' parameter passed to the class method '{self.time.__name__}' is not a string.")
         elif not isinstance(separator, str):
             raise TypeError(
-                f"Arabic_Date class error: The 'separator' parameter passed to the class method '{self.time.__name__}' is not a string.")
+                f"ArabicTime class error: The 'separator' parameter passed to the class method '{self.time.__name__}' is not a string.")
 
         if format.upper() not in ["H", "HM", "HMS", "HMSF"]:
             raise ValueError(
-                f"Arabic_Date class error: Invalid format string passed to the class method '{self.time.__name__}'. Valid values are 'HMSF', 'HMS', 'HM' and 'H'.")
+                f"ArabicTime class error: Invalid format string passed to the class method '{self.time.__name__}'. Valid values are 'HMSF', 'HMS', 'HM' and 'H'.")
 
         time_elements = []
         if "H" in format.upper():
             time_elements.append(self.__hour.translate(self.num_trans_table))
         if "M" in format.upper():
             time_elements.append(self.__minute.translate(self.num_trans_table))
         if "S" in format.upper():
```

### Comparing `arabic_datetime-0.1.0/arabic_datetime/constants.py` & `arabic_datetime-0.1.1/arabic_datetime/_constants.py`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.1.0/LICENSE` & `arabic_datetime-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arabic_datetime-0.1.0/README.md` & `arabic_datetime-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 # arabic-datetime - Arabic datetime formatter
 
 _Author_: Khaldevmedia
 
+_Version_: 0.1.2
+
 _Description_: A python installable package that helps you output dates in Arabic as strings with a formatting that is specific to each Arab county.
 
+## Using The Package for Date Formatting
+
+This Python package is designed to simplify Arabic date formating in your project by providing easy-to-use date formatting features.
+For example it can be used to simplify your backend operations. Instead of installing a full internationalization package in your backend, you can use this package to display Arabic dates formatted according to local settings wheather the reponse content type is HTML or json. It's lightweight, efficient, and easy to integrate into your existing project. By using this package, you can keep your backend lean and focused, while still delivering a localized user experience.
+
 ## Month names in Arabic
 
 There are 4 groups of month names in Arabic.
 
 ### Syriac names:
 
 The **Syriac** names of months are used in Syria Palestine Lebanon, Jordan and Iraq:
 
-> <p style=dir=rtl>كانون الثاني، شباط، آذار، نيسان، أيار، حزيران، تموز، آب، أيلول، تشرين الأول، تشرين الثاني، كانون الأول.</p>
+> <p dir="rtl">كانون الثاني، شباط، آذار، نيسان، أيار، حزيران، تموز، آب، أيلول، تشرين الأول، تشرين الثاني، كانون الأول.</p>
 
 ### Roman names (group 1):
 
 The **Roman names (group 1)** of months are used in Egypt, Yemen, Sudan, Libya, Djibouti, Comoro, Somalia, Saudi Arabia, United Arab Emirates, Qatar, Oman, Bahrain and Kuwait:
 
-> <p style=dir=rtl>يناير، فبراير، مارس، أبريل، مايو، يونيو، يوليو، أغسطس، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
+> <p dir="rtl">يناير، فبراير، مارس، أبريل، مايو، يونيو، يوليو، أغسطس، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
 
 ### Roman names (group 2):
 
 The **Roman names (group 2)** of months are used in Morocco and Mauritania:
 
-> <p style=dir=rtl>يناير، فبراير، مارس، أبريل، ماي، يونيو، يوليوز، غشت، شتنبر، أكتوبر، نونبر، دجنبر.</p>
+> <p dir="rtl">يناير، فبراير، مارس، أبريل، ماي، يونيو، يوليوز، غشت، شتنبر، أكتوبر، نونبر، دجنبر.</p>
 
 ### French names:
 
 The **French** names of months are used in Algeria and Tunisia:
 
-> <p style=dir=rtl>جانفي، فيفري، مارس، أفريل، ماي، جوان، جويلية، أوت، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
+> <p dir="rtl">جانفي، فيفري، مارس، أفريل، ماي، جوان، جويلية، أوت، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
 
 ## Arabic Numerals
 
 There are two groups of **Arabic numerals** used in the Arab countries.
 
 ### Eastern Arabic Numerals
 
@@ -44,25 +51,25 @@
 
 ### Western Arabic Numerals
 
 They are used in Algeria, Tunisia, Morocco and Mauritania. However, they are also used in the other Arabe countries that use the eastern Arabic numerals:
 
 > 0 1 2 3 4 5 6 7 8 9
 
-### Numeral Options
+### Numerals Options
 
-You can use the eastern or the western Arabic numeral regardless of the month names group you use. As demonstrated below, there is always a default numerals' type depending on the method used.
+You can use the eastern or the western Arabic numerals regardless of the month names group you use. As demonstrated below, there is always a default numerals' type depending on the method used.
 
 ## Installation
 
 ```bash
 pip install arabic-datetime
 ```
 
-## Example & Usage
+## Examples
 
 ### 1. Date
 
 The Arabic_Date class has several methods that return a date object as string using.
 
 #### A specific method for every month names group
 
@@ -93,41 +100,41 @@
 > ##### Note:
 >
 > When you combine Western arabic numerals or western ponctuations with arabic characters they appear messed up if the text direction in the target is set to `left to right` or `dir=ltr` in `HTML`.
 >
 > In order for the arabic date to appear properly especially, if it uses western arabic numeral the direction of the text in the interface you are using must be `right to left`. If you insert the date into an `HTML` elemnt set text direction to `rtl`. If the text direction in the whole `HTML` document is set `rtl` you should be OK.
 
 ```html
-<p style="dir" ="rtl">16 آب 1980</p>
-<p style="dir" ="rtl">16 أوت 1980</p>
+<p dir="rtl">16 آب 1980</p>
+<p dir="rtl">16 أوت 1980</p>
 ```
 
 > The resut will look like this:
 >
-> <p style=dir=rtl>16 آب 1980</p>
-> <p style=dir=rtl>16 أوت 1980</p>
+> <p dir="rtl">16 آب 1980</p>
+> <p dir="rtl">16 أوت 1980</p>
 
 #### A dual date name method
 
-It's very common that two month names are used at the same time to display the date, with the second one put between parentheses, like this:
+It's very common that two month names are used at the same time to display the date in arabic with the second one put between parentheses, like this:
 
-> <p style=dir=rtl>16 آب (أغسطس) 1980</p>
-> <p style=dir=rtl>١٦ آب (أغسطس) ١٩٨٠</p>
+> <p dir="rtl">16 آب (أغسطس) 1980</p>
+> <p dir="rtl">١٦ آب (أغسطس) ١٩٨٠</p>
 
 To get the Arabic date formated like this, use the `dual_names` method:
 
 ```python
 import datetime
 from arabic_datetime import Arabic_Date
 
 # Create arabic_date object from a python date object
 dt = datetime.date(1980, 8, 16)
 arabic_date = Arabic_Date(dt)
 
-# Use the dual_names() method to create Arabic date string that shows two names of the month.
+# Use the dual_names() method to return Arabic date string that shows two names of the month.
 # This method takes 3 arguments: 2 strings for the month group names  (the second one
 # will be put between parentheses), and a boolean to determine whether to format the
 # Arabic date with the Eastern Numerals or not:
 dual_date_ro_sy = arabic_date.dual_names("syriac", "roman1", False)
 print(dual_date_ro_sy) # output 16 أغسطس (آب) 1980
 
 # If you don't pass the third argument, the default is False. Also you can use
@@ -145,15 +152,15 @@
 ```
 "syriac" : For Syriac names
 "roman1" : For Roman names (group 1)
 "roman2" : For Roman names  (group 2)
 "french" : For French names
 ```
 
-#### A method that takes the country code to return the corresponding date format
+#### A method that takes a country code to return the corresponding date format
 
 ```python
 import datetime
 from arabic_datetime import Arabic_Date
 
 # Create arabic_date object from a python date object
 dt = datetime.date(1980, 8, 16)
@@ -226,22 +233,22 @@
 ```
 
 > #### Note:
 >
 > As explained above, make sure that the direction of the text in which the Arabic time is inserted is `right to left`.
 
 ```html
-<p style="dir" ="rtl">١٢:٣٠:٤٥</p>
-<p style="dir" ="rtl">الساعة حالياً: ١٢:٣٠:٤٥</p>
+<p dir="rtl">١٢:٣٠:٤٥</p>
+<p dir="rtl">الساعة حالياً: ١٢:٣٠:٤٥</p>
 ```
 
 > The resut will look like this:
 >
-> <p style=dir=rtl>١٢:٣٠:٤٥</p>
-> <p style=dir=rtl>الساعة حالياً: ١٢:٣٠:٤٥</p>
+> <p dir="rtl">١٢:٣٠:٤٥</p>
+> <p dir="rtl">الساعة حالياً: ١٢:٣٠:٤٥</p>
 
 ## License
 
 MIT license.
 
 ## Contact
```

### Comparing `arabic_datetime-0.1.0/pyproject.toml` & `arabic_datetime-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "arabic-datetime"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Khaldevmedia", email="khaldevmedia@gmail.com" },
 ]
-description = "For formating arabic date and time"
+description = "A simple package for formating arabic date and time."
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["python", "arabic", "datetime", "date", "time", "arabic numerals"]
+keywords = ["python", "arabic", "datetime", "date", "time", "arabic date", "arabic time", "arabic numerals", "eastern arabic numerals", "month names"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `arabic_datetime-0.1.0/PKG-INFO` & `arabic_datetime-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 Metadata-Version: 2.3
 Name: arabic-datetime
-Version: 0.1.0
-Summary: For formating arabic date and time
+Version: 0.1.1
+Summary: A simple package for formating arabic date and time.
 Project-URL: Homepage, https://github.com/khaldevmedia/arabic-datetime
 Project-URL: Bug Tracker, https://github.com/khaldevmedia/arabic-datetime/issues
 Author-email: Khaldevmedia <khaldevmedia@gmail.com>
 License-File: LICENSE
-Keywords: arabic,arabic numerals,date,datetime,python,time
+Keywords: arabic,arabic date,arabic numerals,arabic time,date,datetime,eastern arabic numerals,month names,python,time
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # arabic-datetime - Arabic datetime formatter
 
 _Author_: Khaldevmedia
 
+_Version_: 0.1.2
+
 _Description_: A python installable package that helps you output dates in Arabic as strings with a formatting that is specific to each Arab county.
 
+## Using The Package for Date Formatting
+
+This Python package is designed to simplify Arabic date formating in your project by providing easy-to-use date formatting features.
+For example it can be used to simplify your backend operations. Instead of installing a full internationalization package in your backend, you can use this package to display Arabic dates formatted according to local settings wheather the reponse content type is HTML or json. It's lightweight, efficient, and easy to integrate into your existing project. By using this package, you can keep your backend lean and focused, while still delivering a localized user experience.
+
 ## Month names in Arabic
 
 There are 4 groups of month names in Arabic.
 
 ### Syriac names:
 
 The **Syriac** names of months are used in Syria Palestine Lebanon, Jordan and Iraq:
 
-> <p style=dir=rtl>كانون الثاني، شباط، آذار، نيسان، أيار، حزيران، تموز، آب، أيلول، تشرين الأول، تشرين الثاني، كانون الأول.</p>
+> <p dir="rtl">كانون الثاني، شباط، آذار، نيسان، أيار، حزيران، تموز، آب، أيلول، تشرين الأول، تشرين الثاني، كانون الأول.</p>
 
 ### Roman names (group 1):
 
 The **Roman names (group 1)** of months are used in Egypt, Yemen, Sudan, Libya, Djibouti, Comoro, Somalia, Saudi Arabia, United Arab Emirates, Qatar, Oman, Bahrain and Kuwait:
 
-> <p style=dir=rtl>يناير، فبراير، مارس، أبريل، مايو، يونيو، يوليو، أغسطس، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
+> <p dir="rtl">يناير، فبراير، مارس، أبريل، مايو، يونيو، يوليو، أغسطس، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
 
 ### Roman names (group 2):
 
 The **Roman names (group 2)** of months are used in Morocco and Mauritania:
 
-> <p style=dir=rtl>يناير، فبراير، مارس، أبريل، ماي، يونيو، يوليوز، غشت، شتنبر، أكتوبر، نونبر، دجنبر.</p>
+> <p dir="rtl">يناير، فبراير، مارس، أبريل، ماي، يونيو، يوليوز، غشت، شتنبر، أكتوبر، نونبر، دجنبر.</p>
 
 ### French names:
 
 The **French** names of months are used in Algeria and Tunisia:
 
-> <p style=dir=rtl>جانفي، فيفري، مارس، أفريل، ماي، جوان، جويلية، أوت، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
+> <p dir="rtl">جانفي، فيفري، مارس، أفريل، ماي، جوان، جويلية، أوت، سبتمبر، أكتوبر، نوفمبر، ديسمبر.</p>
 
 ## Arabic Numerals
 
 There are two groups of **Arabic numerals** used in the Arab countries.
 
 ### Eastern Arabic Numerals
 
@@ -59,25 +66,25 @@
 
 ### Western Arabic Numerals
 
 They are used in Algeria, Tunisia, Morocco and Mauritania. However, they are also used in the other Arabe countries that use the eastern Arabic numerals:
 
 > 0 1 2 3 4 5 6 7 8 9
 
-### Numeral Options
+### Numerals Options
 
-You can use the eastern or the western Arabic numeral regardless of the month names group you use. As demonstrated below, there is always a default numerals' type depending on the method used.
+You can use the eastern or the western Arabic numerals regardless of the month names group you use. As demonstrated below, there is always a default numerals' type depending on the method used.
 
 ## Installation
 
 ```bash
 pip install arabic-datetime
 ```
 
-## Example & Usage
+## Examples
 
 ### 1. Date
 
 The Arabic_Date class has several methods that return a date object as string using.
 
 #### A specific method for every month names group
 
@@ -108,41 +115,41 @@
 > ##### Note:
 >
 > When you combine Western arabic numerals or western ponctuations with arabic characters they appear messed up if the text direction in the target is set to `left to right` or `dir=ltr` in `HTML`.
 >
 > In order for the arabic date to appear properly especially, if it uses western arabic numeral the direction of the text in the interface you are using must be `right to left`. If you insert the date into an `HTML` elemnt set text direction to `rtl`. If the text direction in the whole `HTML` document is set `rtl` you should be OK.
 
 ```html
-<p style="dir" ="rtl">16 آب 1980</p>
-<p style="dir" ="rtl">16 أوت 1980</p>
+<p dir="rtl">16 آب 1980</p>
+<p dir="rtl">16 أوت 1980</p>
 ```
 
 > The resut will look like this:
 >
-> <p style=dir=rtl>16 آب 1980</p>
-> <p style=dir=rtl>16 أوت 1980</p>
+> <p dir="rtl">16 آب 1980</p>
+> <p dir="rtl">16 أوت 1980</p>
 
 #### A dual date name method
 
-It's very common that two month names are used at the same time to display the date, with the second one put between parentheses, like this:
+It's very common that two month names are used at the same time to display the date in arabic with the second one put between parentheses, like this:
 
-> <p style=dir=rtl>16 آب (أغسطس) 1980</p>
-> <p style=dir=rtl>١٦ آب (أغسطس) ١٩٨٠</p>
+> <p dir="rtl">16 آب (أغسطس) 1980</p>
+> <p dir="rtl">١٦ آب (أغسطس) ١٩٨٠</p>
 
 To get the Arabic date formated like this, use the `dual_names` method:
 
 ```python
 import datetime
 from arabic_datetime import Arabic_Date
 
 # Create arabic_date object from a python date object
 dt = datetime.date(1980, 8, 16)
 arabic_date = Arabic_Date(dt)
 
-# Use the dual_names() method to create Arabic date string that shows two names of the month.
+# Use the dual_names() method to return Arabic date string that shows two names of the month.
 # This method takes 3 arguments: 2 strings for the month group names  (the second one
 # will be put between parentheses), and a boolean to determine whether to format the
 # Arabic date with the Eastern Numerals or not:
 dual_date_ro_sy = arabic_date.dual_names("syriac", "roman1", False)
 print(dual_date_ro_sy) # output 16 أغسطس (آب) 1980
 
 # If you don't pass the third argument, the default is False. Also you can use
@@ -160,15 +167,15 @@
 ```
 "syriac" : For Syriac names
 "roman1" : For Roman names (group 1)
 "roman2" : For Roman names  (group 2)
 "french" : For French names
 ```
 
-#### A method that takes the country code to return the corresponding date format
+#### A method that takes a country code to return the corresponding date format
 
 ```python
 import datetime
 from arabic_datetime import Arabic_Date
 
 # Create arabic_date object from a python date object
 dt = datetime.date(1980, 8, 16)
@@ -241,22 +248,22 @@
 ```
 
 > #### Note:
 >
 > As explained above, make sure that the direction of the text in which the Arabic time is inserted is `right to left`.
 
 ```html
-<p style="dir" ="rtl">١٢:٣٠:٤٥</p>
-<p style="dir" ="rtl">الساعة حالياً: ١٢:٣٠:٤٥</p>
+<p dir="rtl">١٢:٣٠:٤٥</p>
+<p dir="rtl">الساعة حالياً: ١٢:٣٠:٤٥</p>
 ```
 
 > The resut will look like this:
 >
-> <p style=dir=rtl>١٢:٣٠:٤٥</p>
-> <p style=dir=rtl>الساعة حالياً: ١٢:٣٠:٤٥</p>
+> <p dir="rtl">١٢:٣٠:٤٥</p>
+> <p dir="rtl">الساعة حالياً: ١٢:٣٠:٤٥</p>
 
 ## License
 
 MIT license.
 
 ## Contact
```

