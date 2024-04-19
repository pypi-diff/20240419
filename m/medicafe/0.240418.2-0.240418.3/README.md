# Comparing `tmp/medicafe-0.240418.2.tar.gz` & `tmp/medicafe-0.240418.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240418.2.tar", last modified: Fri Apr 19 07:22:07 2024, max compression
+gzip compressed data, was "medicafe-0.240418.3.tar", last modified: Fri Apr 19 07:49:59 2024, max compression
```

## Comparing `medicafe-0.240418.2.tar` & `medicafe-0.240418.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:22:07.949000 medicafe-0.240418.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240418.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-19 07:22:07.400000 medicafe-0.240418.2/MediBot/
--rw-rw-rw-   0        0        0    15371 2024-04-19 06:59:16.000000 medicafe-0.240418.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240418.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    12503 2024-04-19 03:45:33.000000 medicafe-0.240418.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     9281 2024-04-19 03:05:07.000000 medicafe-0.240418.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-19 03:00:07.000000 medicafe-0.240418.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240418.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240418.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240418.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240418.2/MediBot/update_json.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:22:07.783000 medicafe-0.240418.2/MediLink/
--rw-rw-rw-   0        0        0    13842 2024-04-19 02:21:32.000000 medicafe-0.240418.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240418.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    22116 2024-04-19 00:09:39.000000 medicafe-0.240418.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    32894 2024-04-19 00:37:58.000000 medicafe-0.240418.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3206 2024-04-19 07:02:03.000000 medicafe-0.240418.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0     7078 2024-04-19 05:37:41.000000 medicafe-0.240418.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     8306 2024-04-19 00:12:45.000000 medicafe-0.240418.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8769 2024-04-19 00:19:03.000000 medicafe-0.240418.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0      133 2024-03-27 01:07:04.000000 medicafe-0.240418.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240418.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240418.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4409 2024-04-18 02:17:49.000000 medicafe-0.240418.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     6080 2024-04-18 21:27:03.000000 medicafe-0.240418.2/MediLink/MediLink_Up.py
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240418.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240418.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-04-19 07:22:07.936000 medicafe-0.240418.2/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240418.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:22:07.922000 medicafe-0.240418.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-04-19 07:22:06.000000 medicafe-0.240418.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      883 2024-04-19 07:22:06.000000 medicafe-0.240418.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:22:06.000000 medicafe-0.240418.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240418.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2024-04-19 07:22:06.000000 medicafe-0.240418.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-19 07:22:06.000000 medicafe-0.240418.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 07:22:07.946000 medicafe-0.240418.2/setup.cfg
--rw-rw-rw-   0        0        0      984 2024-04-19 07:08:22.000000 medicafe-0.240418.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:49:59.166000 medicafe-0.240418.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240418.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-19 07:49:58.510000 medicafe-0.240418.3/MediBot/
+-rw-rw-rw-   0        0        0    15311 2024-04-19 07:34:15.000000 medicafe-0.240418.3/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240418.3/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    12503 2024-04-19 03:45:33.000000 medicafe-0.240418.3/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     9190 2024-04-19 07:40:55.000000 medicafe-0.240418.3/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-19 03:00:07.000000 medicafe-0.240418.3/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240418.3/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240418.3/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240418.3/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240418.3/MediBot/update_json.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:49:58.933000 medicafe-0.240418.3/MediLink/
+-rw-rw-rw-   0        0        0    13842 2024-04-19 02:21:32.000000 medicafe-0.240418.3/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240418.3/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    22116 2024-04-19 00:09:39.000000 medicafe-0.240418.3/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    32894 2024-04-19 00:37:58.000000 medicafe-0.240418.3/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3206 2024-04-19 07:02:03.000000 medicafe-0.240418.3/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0     7078 2024-04-19 05:37:41.000000 medicafe-0.240418.3/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     8306 2024-04-19 00:12:45.000000 medicafe-0.240418.3/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8769 2024-04-19 00:19:03.000000 medicafe-0.240418.3/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0      133 2024-03-27 01:07:04.000000 medicafe-0.240418.3/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240418.3/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240418.3/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4409 2024-04-18 02:17:49.000000 medicafe-0.240418.3/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     6080 2024-04-18 21:27:03.000000 medicafe-0.240418.3/MediLink/MediLink_Up.py
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240418.3/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240418.3/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-04-19 07:49:59.147000 medicafe-0.240418.3/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240418.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:49:59.125000 medicafe-0.240418.3/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-04-19 07:49:57.000000 medicafe-0.240418.3/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-04-19 07:49:58.000000 medicafe-0.240418.3/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:49:57.000000 medicafe-0.240418.3/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240418.3/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2024-04-19 07:49:57.000000 medicafe-0.240418.3/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 07:49:57.000000 medicafe-0.240418.3/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:49:59.161000 medicafe-0.240418.3/setup.cfg
+-rw-rw-rw-   0        0        0      998 2024-04-19 07:48:42.000000 medicafe-0.240418.3/setup.py
```

### Comparing `medicafe-0.240418.2/LICENSE` & `medicafe-0.240418.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediBot/MediBot.py` & `medicafe-0.240418.3/MediBot/MediBot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tempfile
 import traceback
 import re  #for addresses
 from collections import OrderedDict
 import MediBot_dataformat_library
 import MediBot_Preprocessor
 from MediBot_Preprocessor import initialize, AHK_EXECUTABLE, CSV_FILE_PATH, field_mapping
-from MediBot_UI import manage_script_pause, user_interaction, MEDISOFT_SHORTCUT, MAPAT_MED_PATH
+import MediBot_UI
 
 # Add parent directory of the project to the Python path
 import sys
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediLink import MediLink_ConfigLoader
@@ -113,23 +113,23 @@
     except Exception as e:
         return handle_error(e, medisoft_field, last_processed_entry, csv_data)
 
 def handle_error(error, medisoft_field, last_processed_entry, csv_data):
     print("An error occurred while processing {0}: {1}".format(medisoft_field, error))
     # Assuming the interaction mode is 'error' in this case
     interaction_mode = 'error'
-    response = user_interaction(csv_data, interaction_mode, error, e_state.reverse_mapping)
+    response = MediBot_UI.user_interaction(csv_data, interaction_mode, error, reverse_mapping)
     return response, last_processed_entry
 
 # iterating through each field defined in the field_mapping.
 def iterate_fields(csv_row, field_mapping, parsed_address_components, reverse_mapping, csv_data, fixed_values):
     global last_processed_entry
     # Check for user action at the start of each field processing
     for medisoft_field in field_mapping.keys():
-        action = manage_script_pause(csv_data,'',reverse_mapping) # per-field pause availability. Necessary to provide frequent opportunities for the user to pause the script.
+        action = MediBot_UI.manage_script_pause(csv_data,'',reverse_mapping) # per-field pause availability. Necessary to provide frequent opportunities for the user to pause the script.
         if action != 0:  # If action is either 'Retry' (-1) or 'Skip' (1)
             return action  # Break out and pass the action up
         
         # Process each field in the row
         _, last_processed_entry = process_field(medisoft_field, csv_row, parsed_address_components, reverse_mapping, csv_data, fixed_values)
         
     return 0 # Default action to continue
@@ -140,15 +140,15 @@
     error_message = ''  # Initialize error_message once
     current_row_index = 0
 
     while current_row_index < len(csv_data):
         row = csv_data[current_row_index]
         
         # Handle script pause at the start of each row (patient record). 
-        manage_script_pause(csv_data, error_message, reverse_mapping)
+        MediBot_UI.manage_script_pause(csv_data, error_message, reverse_mapping)
         error_message = ''  # Clear error message for the next iteration
         
         if script_paused:
             continue  # Skip processing this row if the script is paused
 
         # I feel like this is overwriting what would have already been idenfitied in the mapping. 
         # This probably needs to be initialized differently.
@@ -246,27 +246,27 @@
         reverse_mapping = {v: k for k, v in identified_fields.items()}
 
         # CSV Patient Triage
         interaction_mode = 'triage'  # Start in triage mode
         error_message = ""  # This will be filled if an error has occurred
         #print("Debug - Identified fields mapping (main): {}".format(identified_fields)) # Debug Line
         
-        proceed, selected_patient_ids, selected_indices, fixed_values = user_interaction(csv_data, interaction_mode, error_message, e_state.reverse_mapping)
+        proceed, selected_patient_ids, selected_indices, fixed_values = MediBot_UI.user_interaction(csv_data, interaction_mode, error_message, reverse_mapping)
 
         if proceed:
             # Filter csv_data for selected patients from Triage mode.
             csv_data = [row for index, row in enumerate(csv_data) if index in selected_indices]
             existing_patients, patients_to_process = MediBot_Preprocessor.check_existing_patients(selected_patient_ids, MAPAT_MED_PATH)
             
             if existing_patients:
                 print("\nNOTE: The following patient(s) already EXIST in the system and \nwill be excluded from processing:")
                 for patient_id, patient_name in existing_patients:
                     print("(ID: {0}) {1}".format(patient_id, patient_name))
                 # Update csv_data to exclude existing patients
-                csv_data = [row for row in csv_data if row[e_state.reverse_mapping['Patient ID #2']] in patients_to_process]
+                csv_data = [row for row in csv_data if row[reverse_mapping['Patient ID #2']] in patients_to_process]
             else:
                 print("\nSelected patient(s) are NEW patients and will be processed.")
 
             proceed = input("\nDo you want to proceed with the {} remaining patient(s)? (yes/no): ".format(len(patients_to_process))).lower().strip() in ['yes', 'y']
     
             if proceed:
             
@@ -285,28 +285,28 @@
                 print("\nRemember, when in Medisoft:")
                 print("  Press 'F8'  to create a New Patient.")
                 print("  Press 'F12' to begin data entry.")
                 print("  Press 'F11' at any time to Pause.")
                 input("\n*** Press [Enter] when ready to begin! ***\n")
                 open_medisoft(MEDISOFT_SHORTCUT)
                 script_paused = True
-                _ = manage_script_pause(csv_data, error_message, e_state.reverse_mapping)
-                data_entry_loop(csv_data, field_mapping, e_state.reverse_mapping, fixed_values)
+                _ = MediBot_UI.manage_script_pause(csv_data, error_message, reverse_mapping)
+                data_entry_loop(csv_data, field_mapping, reverse_mapping, fixed_values)
                 cleanup()                
             else:
                 print("Data entry canceled by user.")
     except Exception as e:
         if e_state:
             interaction_mode = 'error'  # Switch to error mode
             error_message = str(e)  # Capture the error message
         print("An error occurred: {0}".format(e))
         # Handle the error by calling user interaction with the error information
         # Ensure that identified_fields is defined before using it in user interaction
         if 'identified_fields' in locals():
-            _ = user_interaction(csv_data, interaction_mode, error_message, e_state.reverse_mapping)
+            _ = MediBot_UI.user_interaction(csv_data, interaction_mode, error_message, reverse_mapping)
         else:
             print("Please ensure CSV headers match expected field names in config file, then re-run Medibot.")
 
 # Performance: Process flow (25px - 13 min)
 # 2:00 Internet connect & Email 
 # 6:00 6 px medicare
 # 1:00 menu handling for privado
```

### Comparing `medicafe-0.240418.2/MediBot/MediBot_Charges.py` & `medicafe-0.240418.3/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240418.3/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediBot/MediBot_UI.py` & `medicafe-0.240418.3/MediBot/MediBot_UI.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,23 +150,20 @@
             print("Exiting the script.")
             exit()
         else:
             print("Invalid choice. Please enter a valid number.")
 
 def user_interaction(csv_data, interaction_mode, error_message, reverse_mapping):
     # Consider logging the actions taken during user interaction for audit purposes.
-    
+    global MAPAT_MED_PATH, MEDISOFT_SHORTCUT # Initialize global constants
     selected_patient_ids = []
     selected_indices = []
 
     if interaction_mode == 'triage':
     
-        global MAPAT_MED_PATH # Initialize global constant for MAPAT path
-        global MEDISOFT_SHORTCUT # Initialize global constant for LNK path
-        
         display_menu_header("            =(^.^)= Welcome to MediBot! =(^.^)=")
         
         while True:
             response = input("\nAm I processing Medicare patients? (yes/no): ").lower().strip()
             if response:  # Check if the response is not empty
                 if response in ['yes', 'y']:
                     proceed_as_medicare = True
```

### Comparing `medicafe-0.240418.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240418.3/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240418.3/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediBot/update_json.py` & `medicafe-0.240418.3/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink.py` & `medicafe-0.240418.3/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240418.3/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240418.3/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240418.3/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240418.3/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240418.3/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_Down.py` & `medicafe-0.240418.3/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240418.3/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240418.3/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_UI.py` & `medicafe-0.240418.3/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/MediLink/MediLink_Up.py` & `medicafe-0.240418.3/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/PKG-INFO` & `medicafe-0.240418.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240418.2
+Version: 0.240418.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240418.2/README.md` & `medicafe-0.240418.3/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240418.3/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240418.2
+Version: 0.240418.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240418.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240418.3/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240418.2/setup.py` & `medicafe-0.240418.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version='0.240418.2',
+    version='0.240418.3',
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'requests',
         'argparse',
-        'logging',
-        'pandas'
+        'numpy==1.11.3',
+        'pandas==0.20.0'
     ],
     zip_safe=False
 )
```

