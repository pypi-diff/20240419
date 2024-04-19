# Comparing `tmp/jetline-0.0.51.tar.gz` & `tmp/jetline-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.0.51.tar", last modified: Tue Mar  5 16:12:45 2024, max compression
+gzip compressed data, was "jetline-0.0.52.tar", last modified: Fri Apr 19 11:53:11 2024, max compression
```

## Comparing `jetline-0.0.51.tar` & `jetline-0.0.52.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.582869 jetline-0.0.51/
--rw-rw-rw-   0        0        0     1055 2024-03-05 16:12:45.579501 jetline-0.0.51/PKG-INFO
--rw-rw-rw-   0        0        0      145 2024-02-29 14:18:44.000000 jetline-0.0.51/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.495504 jetline-0.0.51/jetline/
--rw-rw-rw-   0        0        0        0 2024-02-29 15:38:51.000000 jetline-0.0.51/jetline/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.533077 jetline-0.0.51/jetline/commands/
--rw-rw-rw-   0        0        0        0 2024-02-29 12:00:34.000000 jetline-0.0.51/jetline/commands/__init__.py
--rw-rw-rw-   0        0        0      667 2024-03-04 20:36:19.000000 jetline-0.0.51/jetline/commands/_helper.py
--rw-rw-rw-   0        0        0    10445 2024-03-04 21:49:43.000000 jetline-0.0.51/jetline/commands/analyze_project.py
--rw-rw-rw-   0        0        0     4256 2024-03-02 21:52:33.000000 jetline-0.0.51/jetline/commands/create_pipe.py
--rw-rw-rw-   0        0        0     2137 2024-03-02 18:06:44.000000 jetline-0.0.51/jetline/commands/info.py
--rw-rw-rw-   0        0        0     4184 2024-03-02 18:15:37.000000 jetline-0.0.51/jetline/commands/installer.py
--rw-rw-rw-   0        0        0     1134 2024-03-03 09:05:27.000000 jetline-0.0.51/jetline/commands/run_pipeline.py
--rw-rw-rw-   0        0        0    13646 2024-03-04 17:44:01.000000 jetline-0.0.51/jetline/commands/to_exe.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.544624 jetline-0.0.51/jetline/data/
--rw-rw-rw-   0        0        0        0 2024-02-29 18:34:29.000000 jetline-0.0.51/jetline/data/__init__.py
--rw-rw-rw-   0        0        0     4206 2024-03-04 19:55:22.000000 jetline-0.0.51/jetline/data/data.py
--rw-rw-rw-   0        0        0     2777 2024-03-03 16:27:32.000000 jetline-0.0.51/jetline/data/helper.py
--rw-rw-rw-   0        0        0     2340 2024-03-04 20:04:31.000000 jetline-0.0.51/jetline/logging.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.554767 jetline-0.0.51/jetline/pipeline/
--rw-rw-rw-   0        0        0        0 2024-02-29 13:33:00.000000 jetline-0.0.51/jetline/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-03-02 20:20:55.000000 jetline-0.0.51/jetline/pipeline/node.py
--rw-rw-rw-   0        0        0     5035 2024-03-02 20:21:10.000000 jetline-0.0.51/jetline/pipeline/pipeline.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.570897 jetline-0.0.51/jetline/templates/
--rw-rw-rw-   0        0        0        0 2024-02-29 15:43:55.000000 jetline-0.0.51/jetline/templates/__init__.py
--rw-rw-rw-   0        0        0      334 2024-03-04 17:12:27.000000 jetline-0.0.51/jetline/templates/data.py
--rw-rw-rw-   0        0        0      652 2024-03-02 21:39:34.000000 jetline-0.0.51/jetline/templates/main.py
--rw-rw-rw-   0        0        0      630 2024-03-02 20:24:14.000000 jetline-0.0.51/jetline/templates/nodes.py
--rw-rw-rw-   0        0        0      476 2024-03-02 20:22:38.000000 jetline-0.0.51/jetline/templates/pipeline.py
-drwxrwxrwx   0        0        0        0 2024-03-05 16:12:45.576164 jetline-0.0.51/jetline.egg-info/
--rw-rw-rw-   0        0        0     1055 2024-03-05 16:12:45.000000 jetline-0.0.51/jetline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-03-05 16:12:45.000000 jetline-0.0.51/jetline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 16:12:45.000000 jetline-0.0.51/jetline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      317 2024-03-05 16:12:45.000000 jetline-0.0.51/jetline.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2024-03-05 16:12:45.000000 jetline-0.0.51/jetline.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-05 16:12:45.000000 jetline-0.0.51/jetline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-05 16:12:45.583526 jetline-0.0.51/setup.cfg
--rw-rw-rw-   0        0        0     1678 2024-03-05 16:12:35.000000 jetline-0.0.51/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.939147 jetline-0.0.52/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1028 2024-04-19 11:53:11.938927 jetline-0.0.52/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      137 2024-04-19 10:26:37.000000 jetline-0.0.52/README.txt
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.933938 jetline-0.0.52/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.936707 jetline-0.0.52/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1998 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10737 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/analyze_project.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4145 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2866 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1210 2024-04-19 11:38:04.000000 jetline-0.0.52/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    13304 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.937179 jetline-0.0.52/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     3242 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2743 2024-04-19 11:33:50.000000 jetline-0.0.52/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.937620 jetline-0.0.52/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1684 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6042 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.938345 jetline-0.0.52/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      709 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      664 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      603 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      804 2024-04-19 10:26:39.000000 jetline-0.0.52/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:53:11.938615 jetline-0.0.52/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1028 2024-04-19 11:53:11.000000 jetline-0.0.52/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      777 2024-04-19 11:53:11.000000 jetline-0.0.52/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-19 11:53:11.000000 jetline-0.0.52/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-19 11:53:11.000000 jetline-0.0.52/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      109 2024-04-19 11:53:11.000000 jetline-0.0.52/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-19 11:53:11.000000 jetline-0.0.52/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-19 11:53:11.939195 jetline-0.0.52/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1626 2024-04-19 11:50:33.000000 jetline-0.0.52/setup.py
```

### Comparing `jetline-0.0.51/PKG-INFO` & `jetline-0.0.52/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: jetline
-Version: 0.0.51
-Summary: Automated Pipeline Builder
-Home-page: https://github.com/your_username/jetline
-Author: Johannes Kanthak
-Author-email: johannes.kanthak@kdc-solutions.de
-License: MIT
-Keywords: pipeline automation
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: click==8.1.7
-Requires-Dist: colorama==0.4.6
-Requires-Dist: toml==0.10.2
-Requires-Dist: pandas==2.2.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: coloredlogs==15.0.1
-Requires-Dist: fastapi==0.110.0
+Metadata-Version: 2.1
+Name: jetline
+Version: 0.0.52
+Summary: Automated Pipeline Builder
+Home-page: https://github.com/your_username/jetline
+Author: Johannes Kanthak
+Author-email: johannes.kanthak@kdc-solutions.de
+License: MIT
+Keywords: pipeline automation
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: click==8.1.7
+Requires-Dist: colorama==0.4.6
+Requires-Dist: toml==0.10.2
+Requires-Dist: pandas==2.2.0
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: fastapi==0.110.0
```

### Comparing `jetline-0.0.51/jetline/commands/create_pipe.py` & `jetline-0.0.52/jetline/commands/create_pipe.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import click
-import os
-from pathlib import Path
-from colorama import Fore, Style
-import shutil
-import toml
-
-def update_pipeline_order(pipeline_name):
-    """
-    Update the PIPELINE_ORDER list in the main.py file with the given pipeline name.
-
-    Args:
-        pipeline_name (str): The name of the pipeline to be added to the PIPELINE_ORDER list.
-    """
-    current_directory = os.getcwd()
-    main_py_path = os.path.join(current_directory, 'main.py')
-    print(main_py_path)
-    if not os.path.exists(main_py_path):
-        click.echo(f"{Fore.RED}main.py file not found in the current directory.{Style.RESET_ALL}")
-        return
-
-    pipeline_found = False  # Variable to track if PIPELINE_ORDER was found
-
-    try:
-        with open(main_py_path, 'r') as f:
-            lines = f.readlines()
-
-        for i, line in enumerate(lines):
-
-            if 'PIPELINE_ORDER' in line:
-                start_index = line.find('[')
-                end_index = line.rfind(']')
-                pipeline_order = line[start_index+1:end_index]
-                pipeline_order = [element.strip() for element in pipeline_order.split(',') if element.strip()]
-                pipeline_order.append(f'"{pipeline_name}"')
-
-                for j in range(len(pipeline_order) - 1):
-                    if not pipeline_order[j].endswith('"') and not pipeline_order[j+1].startswith('"'):
-                        pipeline_order[j] += ','
-
-                new_line = f'        PIPELINE_ORDER = [{", ".join(pipeline_order)}] if pipes is None else pipes.split(\',\')\n'
-                lines[i] = new_line
-                pipeline_found = True  # Set to True when PIPELINE_ORDER is found
-                break
-
-        # Check if PIPELINE_ORDER was not found
-        if not pipeline_found:
-            raise ValueError('PIPELINE_ORDER must be set in main.py and a valid list with "" separation')
-
-        with open(main_py_path, 'w') as f:
-            f.writelines(lines)
-
-        click.echo(f"{Fore.GREEN}PIPELINE_ORDER updated successfully.{Style.RESET_ALL}")
-
-    except Exception as e:
-        click.echo(f"{Fore.RED}Error updating PIPELINE_ORDER: {e}{Style.RESET_ALL}")
-
-
-@click.command()
-@click.option('--pipeline-name', prompt=f'{Fore.YELLOW}Please enter the pipeline name{Style.RESET_ALL}',help='Name of the project')
-def main(pipeline_name):
-    """
-    Create a new pipeline with the given name.
-
-    Args:
-        pipeline_name (str): The name of the pipeline to be created.
-    """
-    current_directory = os.getcwd()
-    toml_path = os.path.join(current_directory, 'project.toml')
-    if not os.path.exists(toml_path):
-        click.echo(f"{Fore.RED}project.toml file not found in the current directory.{Style.RESET_ALL}")
-        return
-
-    with open(toml_path, 'r') as f:
-        project_config = toml.load(f)
-        pipeline_folder = project_config['project']['place']
-
-    pipeline_folder = os.path.join(current_directory, pipeline_folder, pipeline_name)
-    if os.path.exists(pipeline_folder):
-        click.echo(f"{Fore.RED}Pipeline '{pipeline_name}' already exists.{Style.RESET_ALL}")
-        return
-
-    os.makedirs(pipeline_folder)
-    init_file = os.path.join(pipeline_folder, "__init__.py")
-    Path(init_file).touch()
-
-    templates_folder = os.path.join(os.path.dirname(__file__), '..', 'templates')
-
-    # Copy pipeline.py from the template folder to the pipeline folder
-    pipeline_py_path = os.path.join(pipeline_folder, 'pipeline.py')
-    shutil.copy(os.path.join(templates_folder, 'pipeline.py'), pipeline_py_path)
-
-    # Replace __PIPE__ with the actual pipeline name in pipeline.py
-    with open(pipeline_py_path, 'r') as f:
-        pipeline_content = f.read()
-
-    new_content = pipeline_content.replace('__PIPE__', pipeline_name)
-
-    with open(pipeline_py_path, 'w') as f:
-        f.write(new_content)
-
-    # Copy nodes.py from the template folder to the pipeline folder
-    shutil.copy(os.path.join(templates_folder, 'nodes.py'), pipeline_folder)
-
-    update_pipeline_order(pipeline_name)
-
-    click.echo(f"{Fore.GREEN}New pipeline '{pipeline_name}' created successfully.{Style.RESET_ALL}")
-
-
-if __name__ == '__main__':
-    main()
+import click
+import os
+from pathlib import Path
+from colorama import Fore, Style
+import shutil
+import toml
+
+def update_pipeline_order(pipeline_name):
+    """
+    Update the PIPELINE_ORDER list in the main.py file with the given pipeline name.
+
+    Args:
+        pipeline_name (str): The name of the pipeline to be added to the PIPELINE_ORDER list.
+    """
+    current_directory = os.getcwd()
+    main_py_path = os.path.join(current_directory, 'main.py')
+    print(main_py_path)
+    if not os.path.exists(main_py_path):
+        click.echo(f"{Fore.RED}main.py file not found in the current directory.{Style.RESET_ALL}")
+        return
+
+    pipeline_found = False  # Variable to track if PIPELINE_ORDER was found
+
+    try:
+        with open(main_py_path, 'r') as f:
+            lines = f.readlines()
+
+        for i, line in enumerate(lines):
+
+            if 'PIPELINE_ORDER' in line:
+                start_index = line.find('[')
+                end_index = line.rfind(']')
+                pipeline_order = line[start_index+1:end_index]
+                pipeline_order = [element.strip() for element in pipeline_order.split(',') if element.strip()]
+                pipeline_order.append(f'"{pipeline_name}"')
+
+                for j in range(len(pipeline_order) - 1):
+                    if not pipeline_order[j].endswith('"') and not pipeline_order[j+1].startswith('"'):
+                        pipeline_order[j] += ','
+
+                new_line = f'        PIPELINE_ORDER = [{", ".join(pipeline_order)}] if pipes is None else pipes.split(\',\')\n'
+                lines[i] = new_line
+                pipeline_found = True  # Set to True when PIPELINE_ORDER is found
+                break
+
+        # Check if PIPELINE_ORDER was not found
+        if not pipeline_found:
+            raise ValueError('PIPELINE_ORDER must be set in main.py and a valid list with "" separation')
+
+        with open(main_py_path, 'w') as f:
+            f.writelines(lines)
+
+        click.echo(f"{Fore.GREEN}PIPELINE_ORDER updated successfully.{Style.RESET_ALL}")
+
+    except Exception as e:
+        click.echo(f"{Fore.RED}Error updating PIPELINE_ORDER: {e}{Style.RESET_ALL}")
+
+
+@click.command()
+@click.option('--pipeline-name', prompt=f'{Fore.YELLOW}Please enter the pipeline name{Style.RESET_ALL}',help='Name of the project')
+def main(pipeline_name):
+    """
+    Create a new pipeline with the given name.
+
+    Args:
+        pipeline_name (str): The name of the pipeline to be created.
+    """
+    current_directory = os.getcwd()
+    toml_path = os.path.join(current_directory, 'project.toml')
+    if not os.path.exists(toml_path):
+        click.echo(f"{Fore.RED}project.toml file not found in the current directory.{Style.RESET_ALL}")
+        return
+
+    with open(toml_path, 'r') as f:
+        project_config = toml.load(f)
+        pipeline_folder = project_config['project']['place']
+
+    pipeline_folder = os.path.join(current_directory, pipeline_folder, pipeline_name)
+    if os.path.exists(pipeline_folder):
+        click.echo(f"{Fore.RED}Pipeline '{pipeline_name}' already exists.{Style.RESET_ALL}")
+        return
+
+    os.makedirs(pipeline_folder)
+    init_file = os.path.join(pipeline_folder, "__init__.py")
+    Path(init_file).touch()
+
+    templates_folder = os.path.join(os.path.dirname(__file__), '..', 'templates')
+
+    # Copy pipeline.py from the template folder to the pipeline folder
+    pipeline_py_path = os.path.join(pipeline_folder, 'pipeline.py')
+    shutil.copy(os.path.join(templates_folder, 'pipeline.py'), pipeline_py_path)
+
+    # Replace __PIPE__ with the actual pipeline name in pipeline.py
+    with open(pipeline_py_path, 'r') as f:
+        pipeline_content = f.read()
+
+    new_content = pipeline_content.replace('__PIPE__', pipeline_name)
+
+    with open(pipeline_py_path, 'w') as f:
+        f.write(new_content)
+
+    # Copy nodes.py from the template folder to the pipeline folder
+    shutil.copy(os.path.join(templates_folder, 'nodes.py'), pipeline_folder)
+
+    update_pipeline_order(pipeline_name)
+
+    click.echo(f"{Fore.GREEN}New pipeline '{pipeline_name}' created successfully.{Style.RESET_ALL}")
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `jetline-0.0.51/jetline/commands/info.py` & `jetline-0.0.52/jetline/commands/info.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import click
-from colorama import Fore, Style
-
-@click.command()
-def main():
-    """
-    Print information about jetline.
-    """
-    click.echo(f"{Fore.BLUE}What is jetline?{Style.RESET_ALL}")
-    click.echo("jetline is a powerful, lightweight pipeline builder designed to simplify the creation and management of data processing pipelines.")
-    click.echo("\n")
-
-    click.echo(f"{Fore.BLUE}What can you do with jetline?{Style.RESET_ALL}")
-    click.echo("With jetline, you can define, organize, and execute complex data processing workflows with ease.")
-    click.echo("\n")
-
-    click.echo(f"{Fore.BLUE}Documentation:{Style.RESET_ALL}")
-    click.echo("For more information and detailed documentation, visit:")
-    click.echo("https://jetline.readthedocs.io/en/latest/")
-    click.echo("\n")
-
-    click.echo(f"{Fore.BLUE}GitHub Repository:{Style.RESET_ALL}")
-    click.echo("Find the jetline source code and contribute on GitHub:")
-    click.echo("https://github.com/yourusername/jetline")
-    click.echo("\n")
-
-    click.echo(f"{Fore.BLUE}PyPI Package:{Style.RESET_ALL}")
-    click.echo("jetline is available as a Python package on PyPI. Install it via pip:")
-    click.echo("pip install jetline")
-    click.echo("\n")
-
-
-    click.echo(f"{Fore.BLUE}Welcome to jetline!{Style.RESET_ALL}")
-    click.echo("This command will guide you through setting up a new jetline project.")
-    click.echo("It will create the necessary project structure and files.")
-    click.echo("\n")
-    click.echo("To set up the project, run the following commands:")
-    click.echo("1. jetline-setup")
-    click.echo("2. Follow the prompts to provide project details.")
-    click.echo("\n")
-
-    click.echo(f"{Fore.BLUE}Creating a new pipeline!{Style.RESET_ALL}")
-    click.echo("This command will create a new pipeline in your jetline project.")
-    click.echo("It will set up the necessary files and configurations.")
-    click.echo("\n")
-    click.echo("To create a new pipeline, run the following command:")
-    click.echo("jetline-new-pipe")
-    click.echo("\n")
-
-
-if __name__ == '__main__':
+import click
+from colorama import Fore, Style
+
+@click.command()
+def main():
+    """
+    Print information about jetline.
+    """
+    click.echo(f"{Fore.BLUE}What is jetline?{Style.RESET_ALL}")
+    click.echo("jetline is a powerful, lightweight pipeline builder designed to simplify the creation and management of data processing pipelines.")
+    click.echo("\n")
+
+    click.echo(f"{Fore.BLUE}What can you do with jetline?{Style.RESET_ALL}")
+    click.echo("With jetline, you can define, organize, and execute complex data processing workflows with ease.")
+    click.echo("\n")
+
+    click.echo(f"{Fore.BLUE}Documentation:{Style.RESET_ALL}")
+    click.echo("For more information and detailed documentation, visit:")
+    click.echo("https://jetline.readthedocs.io/en/latest/")
+    click.echo("\n")
+
+    click.echo(f"{Fore.BLUE}GitHub Repository:{Style.RESET_ALL}")
+    click.echo("Find the jetline source code and contribute on GitHub:")
+    click.echo("https://github.com/yourusername/jetline")
+    click.echo("\n")
+
+    click.echo(f"{Fore.BLUE}PyPI Package:{Style.RESET_ALL}")
+    click.echo("jetline is available as a Python package on PyPI. Install it via pip:")
+    click.echo("pip install jetline")
+    click.echo("\n")
+
+
+    click.echo(f"{Fore.BLUE}Welcome to jetline!{Style.RESET_ALL}")
+    click.echo("This command will guide you through setting up a new jetline project.")
+    click.echo("It will create the necessary project structure and files.")
+    click.echo("\n")
+    click.echo("To set up the project, run the following commands:")
+    click.echo("1. jetline-setup")
+    click.echo("2. Follow the prompts to provide project details.")
+    click.echo("\n")
+
+    click.echo(f"{Fore.BLUE}Creating a new pipeline!{Style.RESET_ALL}")
+    click.echo("This command will create a new pipeline in your jetline project.")
+    click.echo("It will set up the necessary files and configurations.")
+    click.echo("\n")
+    click.echo("To create a new pipeline, run the following command:")
+    click.echo("jetline-new-pipe")
+    click.echo("\n")
+
+
+if __name__ == '__main__':
     main()
```

### Comparing `jetline-0.0.51/jetline/commands/run_pipeline.py` & `jetline-0.0.52/jetline/commands/run_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-import click
-import os
-
-@click.command()
-@click.argument('pipeline_name', default=None, required=False)
-def main(pipeline_name):
-    """
-     Run a pipeline or all pipelines if pipeline_name is None. This is a command line tool to run a pipeline or all pipelines in the current directory.
-     
-     Args:
-     	 pipeline_name: Name of the pipeline to run or None
-    """
-    main_file = "main.py"
-    current_directory = os.getcwd()
-    main_path = os.path.join(current_directory, main_file)
-
-    if os.path.isfile(main_path):
-        if pipeline_name is not None:
-            click.secho(f"Directory successfully located. Running pipeline(s) '{pipeline_name}'...", fg='green')
-            os.system(f'python -c "from main import run_pipelines; run_pipelines(\'{pipeline_name}\')"')
-        else:
-            click.secho("Directory successfully located. Running Pipelines...", fg='green')
-            os.system('python -c "from main import run_pipelines; run_pipelines()"')
-    else:
-        click.secho(f"{main_file} not found in the current directory.", fg='red')
-
-if __name__ == "__main__":
-    main()
+import click
+import os
+import sys
+
+python_cmd = 'python'
+if sys.version_info >= (3, 0):
+    python_cmd = 'python3'
+@click.command()
+@click.argument('pipeline_name', default=None, required=False)
+def main(pipeline_name):
+    """
+     Run a pipeline or all pipelines if pipeline_name is None. This is a command line tool to run a pipeline or all pipelines in the current directory.
+     
+     Args:
+     	 pipeline_name: Name of the pipeline to run or None
+    """
+    main_file = "main.py"
+    current_directory = os.getcwd()
+    main_path = os.path.join(current_directory, main_file)
+
+    if os.path.isfile(main_path):
+        if pipeline_name is not None:
+            click.secho(f"Directory successfully located. Running pipeline(s) '{pipeline_name}'...", fg='green')
+            os.system(f'{python_cmd} -c "from main import run_pipelines; run_pipelines(\'{pipeline_name}\')"')
+        else:
+            click.secho("Directory successfully located. Running Pipelines...", fg='green')
+            os.system(f'{python_cmd} -c "from main import run_pipelines; run_pipelines()"')
+    else:
+        click.secho(f"{main_file} not found in the current directory.", fg='red')
+
+if __name__ == "__main__":
+    main()
```

### Comparing `jetline-0.0.51/jetline/commands/to_exe.py` & `jetline-0.0.52/jetline/commands/to_exe.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,342 +1,342 @@
-import click
-import os
-import re
-import vulture
-import toml
-def _read_main_file_content(main_path):
-    """
-    Liest den Inhalt der Hauptdatei (main.py).
-
-    :param main_path: Der Pfad zur Hauptdatei.
-    :return: Der Inhalt der Hauptdatei.
-    """
-    with open(main_path, 'r') as file:
-        return file.read()
-
-
-def _extract_pipeline_order(main_content):
-    """
-    Extrahiert die PIPELINE_ORDER-Liste aus dem Inhalt der Hauptdatei.
-
-    :param main_content: Der Inhalt der Hauptdatei.
-    :return: Die extrahierte PIPELINE_ORDER-Liste oder None, falls nicht gefunden.
-    """
-    pipeline_order_match = re.search(r'PIPELINE_ORDER\s*=\s*\[([^\]]+)\]', main_content)
-    if pipeline_order_match:
-        return pipeline_order_match.group(1).replace("'", "").replace('"', "").split(',')
-    return None
-
-
-def _find_folders(directory, folder_list):
-    """
-    Sucht nach Ordnern in einem Verzeichnis basierend auf einer Liste von Ordnernamen.
-
-    :param directory: Das Verzeichnis, in dem nach den Ordnern gesucht werden soll.
-    :param folder_list: Die Liste von Ordnernamen, nach denen gesucht werden soll.
-    """
-    for folder_name in folder_list:
-        folder_path = os.path.join(directory, folder_name)
-        if os.path.isdir(folder_path):
-            click.echo(f"Ordner '{folder_name}' gefunden: {folder_path}")
-        else:
-            click.echo(f"Ordner '{folder_name}' nicht gefunden.")
-
-
-
-
-def _extract_project_info(caller_path):
-    """
-    Extrahiert den Namen und den Ort (place) aus der project.toml-Datei.
-
-    :param caller_path: Der Pfad des aufrufenden Verzeichnisses.
-    :return: Ein Tupel (name, place) des extrahierten Projekts oder (None, None), falls nicht gefunden.
-    """
-
-    if os.path.exists(caller_path):
-       
-        with open(caller_path, 'r') as f:
-            toml_data = toml.load(f)
-            project_info = toml_data.get('project', {})
-            place = project_info.get('place')
-            name = project_info.get('name')
-            return place, name
-    return None, None
-
-
-def _copy_nodes_content(folder_name, folder_path):
-    """
-    Kopiert den Inhalt der 'nodes.py'-Datei im angegebenen Ordner und fügt ihn in die 'exe.py'-Datei ein.
-
-    :param folder_name: Der Name des Ordners, in dem 'nodes.py' gefunden wurde.
-    :param folder_path: Der Pfad zum Ordner, in dem 'nodes.py' gefunden wurde.
-    """
-    nodes_file_path = os.path.join(folder_path, 'nodes.py')
-    if os.path.exists(nodes_file_path):
-     
-        with open(nodes_file_path, 'r') as nodes_file:
-            nodes_content = nodes_file.read()
-            if nodes_content.strip(): 
-                _modify_exe_file(f"Nodes content from '{folder_name}'", nodes_content.strip())
-            else:
-                click.echo(f"Die 'nodes.py'-Datei in '{folder_name}' ist leer.")
-    else:
-        click.echo(f"Die 'nodes.py'-Datei wurde in '{folder_name}' nicht gefunden.")
-
-def _extract_node_functions(pipeline_content):
-    extracted_functions = []
-    lines = pipeline_content.split('\n')
-    for line in lines:
-        if 'Node(' in line:
-            function_name = None
-            inputs = None
-            outputs = None
-            
-            # Extrahiere Funktion
-            if 'function=' in line:
-                function_start = line.find('function=') + len('function=')
-                function_end = line.find(',', function_start)
-                function_name = line[function_start:function_end].strip().split('.')[-1]
-            
-            # Extrahiere Inputs
-            if 'inputs=[' in line:
-                inputs_start = line.find('inputs=[') + len('inputs=[')
-                inputs_end = line.find(']', inputs_start)
-                inputs = line[inputs_start:inputs_end].strip().replace('"', '').replace("'", '').split(',')
-                inputs = [inp.strip() + ".data" for inp in inputs]
-
-            # Extrahiere Outputs
-            if 'outputs=[' in line:
-                outputs_start = line.find('outputs=[') + len('outputs=[')
-                outputs_end = line.find(']', outputs_start)
-                outputs = line[outputs_start:outputs_end].strip().replace('"', '').replace("'", '').split(',')
-                outputs = [out.strip() + ".data" for out in outputs]
-                
-            # Erstelle die Funktionseinträge
-            if function_name and inputs:
-                if outputs:
-                    extracted_functions.append(f"{', '.join(outputs)} = {function_name}({', '.join(inputs)})")
-                else:
-                    extracted_functions.append(f"{function_name}({', '.join(inputs)})")
-    return extracted_functions
-
-
-def _call_node_functions(folder_name, folder_path):
-  
-    pipeline_file_path = os.path.join(folder_path, 'pipeline.py')
-    if os.path.exists(pipeline_file_path):
-     
-        with open(pipeline_file_path, 'r') as nodes_file:
-            pipeline_content = nodes_file.read()
-            if pipeline_content.strip(): 
-               
-                modified_content = "\n".join(_extract_node_functions(pipeline_content))
-                _modify_exe_file(f"Nodes content from '{folder_name}'",modified_content )
-            else:
-                click.echo(f"Die 'nodes.py'-Datei in '{folder_name}' ist leer.")
-    else:
-        click.echo(f"Die 'pipeline.py'-Datei wurde in '{folder_name}' nicht gefunden.")
-
-def _search_folders(place_directory, pipeline_order):
-    """
-    Sucht nach den Ordnern im angegebenen Verzeichnis basierend auf der extrahierten Liste.
-
-    :param place_directory: Das Verzeichnis, in dem gesucht werden soll.
-    :param pipeline_order: Die Liste von Ordnernamen, nach denen gesucht werden soll.
-    """
-    if os.path.exists(place_directory):
-        click.echo(f"Suche nach Ordnern in '{place_directory}':")
-        for folder_name in pipeline_order:
-            folder_name = folder_name.strip()
-            folder_path = os.path.join(place_directory, folder_name)
-            if os.path.isdir(folder_path):
-                click.echo(f"Ordner '{folder_name}' gefunden: {folder_path}")
-                _copy_nodes_content(folder_name, folder_path)
-                _call_node_functions(folder_name, folder_path)
-            else:
-                click.echo(f"Ordner '{folder_name}' nicht gefunden.")
-    else:
-        click.echo(f"Ort '{place_directory}' nicht gefunden.")
-
-
-def _create_exe_file(project_name):
-    """
-    Erstellt eine exe.py im aktuellen Verzeichnis.
-    """
-    exe_file_path = os.path.join(os.getcwd(), 'exe.py')
-    with open(exe_file_path, 'w') as exe_file:
-        exe_file.write(f"# This is the compiles Source Code of your Pipeline project called '{project_name}'\n")
-
-
-def _modify_exe_file(comment, value):
-    """
-    Modifiziert die exe.py-Datei im aktuellen Verzeichnis.
-
-    :param comment: Der Kommentar, der zur letzten Zeile hinzugefügt werden soll.
-    :param value: Der Wert, der hinzugefügt werden soll.
-    """
-    exe_file_path = os.path.join(os.getcwd(), 'exe.py')
-    with open(exe_file_path, 'r') as exe_file:
-        lines = exe_file.readlines()
-
-    # Finde die letzte Zeile, füge den Kommentar hinzu und aktualisiere den Wert
-    last_line_index = len(lines) - 1
-    lines[last_line_index] = lines[last_line_index].rstrip() + f"\n\n# {comment}\n"
-    lines.append(f"{value}\n")
-
-    with open(exe_file_path, 'w') as exe_file:
-        exe_file.writelines(lines)
-
-
-def _copy_jetline_functions():
-    """
-    Kopiert die Funktionen aus dem Modul jetline.data.helper und gibt sie als Text zurück.
-    """
-    try:
-        # Pfad zum Modul jetline.data.helper
-        module_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "data", "helper.py")
-
-        # Funktionen aus dem Modul lesen und als Text zurückgeben
-        with open(module_path, 'r') as module_file:
-            module_content = module_file.read()
-            return module_content
-    except FileNotFoundError:
-        print("Modul jetline.data.helper nicht gefunden.")
-    except Exception as e:
-        print(f"Fehler beim Lesen des Moduls jetline.data.helper: {e}")
-
-
-def clean_exe_file():
-    exe_file_path = os.path.join(os.getcwd(), 'exe.py')
-
-    # Vulture verwenden, um nicht verwendeten Code zu finden
-    def vulture_scan():
-        v = vulture.Vulture()
-        v.scan(open(exe_file_path).read())
-
-        # Zeilennummern des nicht verwendeten Codes extrahieren
-        unused_code_lines = set()
-        for item in v.get_unused_code():
-            unused_code_lines.update(range(item.first_lineno, item.last_lineno + 1))
-
-        # Alle Zeilen mit nicht verwendeten Code oder Kommentaren in """ entfernen
-        if unused_code_lines:
-            with open(exe_file_path, 'r') as f:
-                lines = f.readlines()
-
-            modified_lines = []
-            in_multiline_comment = False
-            for line_number, line in enumerate(lines, start=1):
-                # Überprüfen, ob die Zeile in einem mehrzeiligen Kommentar ist
-                if '"""' in line:
-                    if not in_multiline_comment:
-                        in_multiline_comment = True
-                    else:
-                        in_multiline_comment = False
-                        continue
-                if in_multiline_comment:
-                    continue
-                
-                # Überprüfen, ob die Zeile nicht verwendet wird oder leer ist
-                if line_number not in unused_code_lines and line.strip():  # strip entfernt Whitespace am Anfang und Ende
-                    modified_lines.append(line)
-
-            with open(exe_file_path, 'w') as f:
-                f.writelines(modified_lines)
-
-    vulture_scan()
-    vulture_scan()
-    print("Nicht verwendeten Code erfolgreich entfernt.")
-    
-
-def _find_classes():
-    """
-    Sucht nach Klassen in der data.py-Datei im aktuellen Verzeichnis und initialisiert sie in der exe.py-Datei.
-    """
-    current_directory = os.getcwd()
-    data_file_path = os.path.join(current_directory, 'data.py')
-
-    if os.path.exists(data_file_path):
-        with open(data_file_path, 'r') as file:
-            file_content = file.read()
-            if file_content.strip():  # Überprüfen, ob die Dateiinhalt nicht leer ist
-                # Kopieren von Funktionen aus jetline-Modulen
-                copied_functions = _copy_jetline_functions()
-                _modify_exe_file("Helper", copied_functions.strip())
-
-                # Entfernen von 'Data' innerhalb von Klammern
-
-                file_content = re.sub(r'^(?:from\s+jetline.*|import\s+jetline.*)$', '', file_content, flags=re.MULTILINE)
-                file_content = "class Data:\n    def __init__(self, name, data):\n        self.name = name\n        self.data = data\n\n" + file_content
-
-                _modify_exe_file("Data Classes", file_content.strip())
-
-                # Finden aller Klassendefinitionen
-                class_definitions = re.findall(r'class\s+(\w+)\(.*?\):', file_content)
-
-                # Initialisieren von Klassen in exe.py
-                initialization_lines = []
-                for class_name in class_definitions:
-                    class_content = re.search(r'class\s+' + class_name + r'\(.*?\):(.+?)(?=class|\Z)', file_content, re.DOTALL)
-                    if class_content:
-                        name_assignment = re.search(r'name\s*=\s*["\']([^"\']+)["\']', class_content.group(1))
-                        if name_assignment:
-                            initialization_line = f"{name_assignment.group(1)} = {class_name}()"
-                            initialization_lines.append(initialization_line)
-
-
-                # Verbinden der Initialisierungszeilen
-                initialization_content = '\n'.join(initialization_lines)
-
-                # Ändern der exe.py-Datei
-                _modify_exe_file("Your data classes", initialization_content)
-                print("Klassen aus data.py erfolgreich in exe.py kopiert.")
-            else:
-                print("Die data.py-Datei ist leer.")
-    else:
-        print("data.py-Datei nicht gefunden.")
-
-
-@click.command()
-@click.argument('output_name', default='output', required=False)
-def main(output_name):
-    """
-    Erstellt eine ausführbare Datei aus der Hauptdatei (main.py) und extrahiert die PIPELINE_ORDER-Liste.
-
-    :param output_name: Der Name der Ausgabedatei (Standard: 'output')
-    """
-    # Aktuelles Verzeichnis
-    current_directory = os.getcwd()
-    place_folder = None
-    
-    # Pfad zur Hauptdatei
-    main_path = os.path.join(current_directory, 'main.py')
-    
-    main_content = _read_main_file_content(main_path)
-    pipeline_order = _extract_pipeline_order(main_content)
-
-    if pipeline_order:
-        # Pfad zur project.toml-Datei
-        project_toml_path = os.path.join(current_directory, 'project.toml')
-
-        place_folder, project_name = _extract_project_info(project_toml_path)
-
-        if place_folder:
-            place_directory = os.path.join(current_directory, place_folder)
-        else:
-            click.echo("Ort (place) nicht gefunden.")
-    else:
-        click.echo("PIPELINE_ORDER nicht gefunden.")
-
-    # Erstelle und modifiziere die exe.py-Datei
-    _create_exe_file(project_name)
-    _find_classes()
-    _search_folders(place_directory, pipeline_order)
-    clean_exe_file()
- 
-    
-
-    
-
-
-if __name__ == "__main__":
-    main()
+import click
+import os
+import re
+import vulture
+import toml
+def _read_main_file_content(main_path):
+    """
+    Liest den Inhalt der Hauptdatei (main.py).
+
+    :param main_path: Der Pfad zur Hauptdatei.
+    :return: Der Inhalt der Hauptdatei.
+    """
+    with open(main_path, 'r') as file:
+        return file.read()
+
+
+def _extract_pipeline_order(main_content):
+    """
+    Extrahiert die PIPELINE_ORDER-Liste aus dem Inhalt der Hauptdatei.
+
+    :param main_content: Der Inhalt der Hauptdatei.
+    :return: Die extrahierte PIPELINE_ORDER-Liste oder None, falls nicht gefunden.
+    """
+    pipeline_order_match = re.search(r'PIPELINE_ORDER\s*=\s*\[([^\]]+)\]', main_content)
+    if pipeline_order_match:
+        return pipeline_order_match.group(1).replace("'", "").replace('"', "").split(',')
+    return None
+
+
+def _find_folders(directory, folder_list):
+    """
+    Sucht nach Ordnern in einem Verzeichnis basierend auf einer Liste von Ordnernamen.
+
+    :param directory: Das Verzeichnis, in dem nach den Ordnern gesucht werden soll.
+    :param folder_list: Die Liste von Ordnernamen, nach denen gesucht werden soll.
+    """
+    for folder_name in folder_list:
+        folder_path = os.path.join(directory, folder_name)
+        if os.path.isdir(folder_path):
+            click.echo(f"Ordner '{folder_name}' gefunden: {folder_path}")
+        else:
+            click.echo(f"Ordner '{folder_name}' nicht gefunden.")
+
+
+
+
+def _extract_project_info(caller_path):
+    """
+    Extrahiert den Namen und den Ort (place) aus der project.toml-Datei.
+
+    :param caller_path: Der Pfad des aufrufenden Verzeichnisses.
+    :return: Ein Tupel (name, place) des extrahierten Projekts oder (None, None), falls nicht gefunden.
+    """
+
+    if os.path.exists(caller_path):
+       
+        with open(caller_path, 'r') as f:
+            toml_data = toml.load(f)
+            project_info = toml_data.get('project', {})
+            place = project_info.get('place')
+            name = project_info.get('name')
+            return place, name
+    return None, None
+
+
+def _copy_nodes_content(folder_name, folder_path):
+    """
+    Kopiert den Inhalt der 'nodes.py'-Datei im angegebenen Ordner und fügt ihn in die 'exe.py'-Datei ein.
+
+    :param folder_name: Der Name des Ordners, in dem 'nodes.py' gefunden wurde.
+    :param folder_path: Der Pfad zum Ordner, in dem 'nodes.py' gefunden wurde.
+    """
+    nodes_file_path = os.path.join(folder_path, 'nodes.py')
+    if os.path.exists(nodes_file_path):
+     
+        with open(nodes_file_path, 'r') as nodes_file:
+            nodes_content = nodes_file.read()
+            if nodes_content.strip(): 
+                _modify_exe_file(f"Nodes content from '{folder_name}'", nodes_content.strip())
+            else:
+                click.echo(f"Die 'nodes.py'-Datei in '{folder_name}' ist leer.")
+    else:
+        click.echo(f"Die 'nodes.py'-Datei wurde in '{folder_name}' nicht gefunden.")
+
+def _extract_node_functions(pipeline_content):
+    extracted_functions = []
+    lines = pipeline_content.split('\n')
+    for line in lines:
+        if 'Node(' in line:
+            function_name = None
+            inputs = None
+            outputs = None
+            
+            # Extrahiere Funktion
+            if 'function=' in line:
+                function_start = line.find('function=') + len('function=')
+                function_end = line.find(',', function_start)
+                function_name = line[function_start:function_end].strip().split('.')[-1]
+            
+            # Extrahiere Inputs
+            if 'inputs=[' in line:
+                inputs_start = line.find('inputs=[') + len('inputs=[')
+                inputs_end = line.find(']', inputs_start)
+                inputs = line[inputs_start:inputs_end].strip().replace('"', '').replace("'", '').split(',')
+                inputs = [inp.strip() + ".data" for inp in inputs]
+
+            # Extrahiere Outputs
+            if 'outputs=[' in line:
+                outputs_start = line.find('outputs=[') + len('outputs=[')
+                outputs_end = line.find(']', outputs_start)
+                outputs = line[outputs_start:outputs_end].strip().replace('"', '').replace("'", '').split(',')
+                outputs = [out.strip() + ".data" for out in outputs]
+                
+            # Erstelle die Funktionseinträge
+            if function_name and inputs:
+                if outputs:
+                    extracted_functions.append(f"{', '.join(outputs)} = {function_name}({', '.join(inputs)})")
+                else:
+                    extracted_functions.append(f"{function_name}({', '.join(inputs)})")
+    return extracted_functions
+
+
+def _call_node_functions(folder_name, folder_path):
+  
+    pipeline_file_path = os.path.join(folder_path, 'pipeline.py')
+    if os.path.exists(pipeline_file_path):
+     
+        with open(pipeline_file_path, 'r') as nodes_file:
+            pipeline_content = nodes_file.read()
+            if pipeline_content.strip(): 
+               
+                modified_content = "\n".join(_extract_node_functions(pipeline_content))
+                _modify_exe_file(f"Nodes content from '{folder_name}'",modified_content )
+            else:
+                click.echo(f"Die 'nodes.py'-Datei in '{folder_name}' ist leer.")
+    else:
+        click.echo(f"Die 'pipeline.py'-Datei wurde in '{folder_name}' nicht gefunden.")
+
+def _search_folders(place_directory, pipeline_order):
+    """
+    Sucht nach den Ordnern im angegebenen Verzeichnis basierend auf der extrahierten Liste.
+
+    :param place_directory: Das Verzeichnis, in dem gesucht werden soll.
+    :param pipeline_order: Die Liste von Ordnernamen, nach denen gesucht werden soll.
+    """
+    if os.path.exists(place_directory):
+        click.echo(f"Suche nach Ordnern in '{place_directory}':")
+        for folder_name in pipeline_order:
+            folder_name = folder_name.strip()
+            folder_path = os.path.join(place_directory, folder_name)
+            if os.path.isdir(folder_path):
+                click.echo(f"Ordner '{folder_name}' gefunden: {folder_path}")
+                _copy_nodes_content(folder_name, folder_path)
+                _call_node_functions(folder_name, folder_path)
+            else:
+                click.echo(f"Ordner '{folder_name}' nicht gefunden.")
+    else:
+        click.echo(f"Ort '{place_directory}' nicht gefunden.")
+
+
+def _create_exe_file(project_name):
+    """
+    Erstellt eine exe.py im aktuellen Verzeichnis.
+    """
+    exe_file_path = os.path.join(os.getcwd(), 'exe.py')
+    with open(exe_file_path, 'w') as exe_file:
+        exe_file.write(f"# This is the compiles Source Code of your Pipeline project called '{project_name}'\n")
+
+
+def _modify_exe_file(comment, value):
+    """
+    Modifiziert die exe.py-Datei im aktuellen Verzeichnis.
+
+    :param comment: Der Kommentar, der zur letzten Zeile hinzugefügt werden soll.
+    :param value: Der Wert, der hinzugefügt werden soll.
+    """
+    exe_file_path = os.path.join(os.getcwd(), 'exe.py')
+    with open(exe_file_path, 'r') as exe_file:
+        lines = exe_file.readlines()
+
+    # Finde die letzte Zeile, füge den Kommentar hinzu und aktualisiere den Wert
+    last_line_index = len(lines) - 1
+    lines[last_line_index] = lines[last_line_index].rstrip() + f"\n\n# {comment}\n"
+    lines.append(f"{value}\n")
+
+    with open(exe_file_path, 'w') as exe_file:
+        exe_file.writelines(lines)
+
+
+def _copy_jetline_functions():
+    """
+    Kopiert die Funktionen aus dem Modul jetline.data.helper und gibt sie als Text zurück.
+    """
+    try:
+        # Pfad zum Modul jetline.data.helper
+        module_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "data", "helper.py")
+
+        # Funktionen aus dem Modul lesen und als Text zurückgeben
+        with open(module_path, 'r') as module_file:
+            module_content = module_file.read()
+            return module_content
+    except FileNotFoundError:
+        print("Modul jetline.data.helper nicht gefunden.")
+    except Exception as e:
+        print(f"Fehler beim Lesen des Moduls jetline.data.helper: {e}")
+
+
+def clean_exe_file():
+    exe_file_path = os.path.join(os.getcwd(), 'exe.py')
+
+    # Vulture verwenden, um nicht verwendeten Code zu finden
+    def vulture_scan():
+        v = vulture.Vulture()
+        v.scan(open(exe_file_path).read())
+
+        # Zeilennummern des nicht verwendeten Codes extrahieren
+        unused_code_lines = set()
+        for item in v.get_unused_code():
+            unused_code_lines.update(range(item.first_lineno, item.last_lineno + 1))
+
+        # Alle Zeilen mit nicht verwendeten Code oder Kommentaren in """ entfernen
+        if unused_code_lines:
+            with open(exe_file_path, 'r') as f:
+                lines = f.readlines()
+
+            modified_lines = []
+            in_multiline_comment = False
+            for line_number, line in enumerate(lines, start=1):
+                # Überprüfen, ob die Zeile in einem mehrzeiligen Kommentar ist
+                if '"""' in line:
+                    if not in_multiline_comment:
+                        in_multiline_comment = True
+                    else:
+                        in_multiline_comment = False
+                        continue
+                if in_multiline_comment:
+                    continue
+                
+                # Überprüfen, ob die Zeile nicht verwendet wird oder leer ist
+                if line_number not in unused_code_lines and line.strip():  # strip entfernt Whitespace am Anfang und Ende
+                    modified_lines.append(line)
+
+            with open(exe_file_path, 'w') as f:
+                f.writelines(modified_lines)
+
+    vulture_scan()
+    vulture_scan()
+    print("Nicht verwendeten Code erfolgreich entfernt.")
+    
+
+def _find_classes():
+    """
+    Sucht nach Klassen in der data.py-Datei im aktuellen Verzeichnis und initialisiert sie in der exe.py-Datei.
+    """
+    current_directory = os.getcwd()
+    data_file_path = os.path.join(current_directory, 'data.py')
+
+    if os.path.exists(data_file_path):
+        with open(data_file_path, 'r') as file:
+            file_content = file.read()
+            if file_content.strip():  # Überprüfen, ob die Dateiinhalt nicht leer ist
+                # Kopieren von Funktionen aus jetline-Modulen
+                copied_functions = _copy_jetline_functions()
+                _modify_exe_file("Helper", copied_functions.strip())
+
+                # Entfernen von 'Data' innerhalb von Klammern
+
+                file_content = re.sub(r'^(?:from\s+jetline.*|import\s+jetline.*)$', '', file_content, flags=re.MULTILINE)
+                file_content = "class Data:\n    def __init__(self, name, data):\n        self.name = name\n        self.data = data\n\n" + file_content
+
+                _modify_exe_file("Data Classes", file_content.strip())
+
+                # Finden aller Klassendefinitionen
+                class_definitions = re.findall(r'class\s+(\w+)\(.*?\):', file_content)
+
+                # Initialisieren von Klassen in exe.py
+                initialization_lines = []
+                for class_name in class_definitions:
+                    class_content = re.search(r'class\s+' + class_name + r'\(.*?\):(.+?)(?=class|\Z)', file_content, re.DOTALL)
+                    if class_content:
+                        name_assignment = re.search(r'name\s*=\s*["\']([^"\']+)["\']', class_content.group(1))
+                        if name_assignment:
+                            initialization_line = f"{name_assignment.group(1)} = {class_name}()"
+                            initialization_lines.append(initialization_line)
+
+
+                # Verbinden der Initialisierungszeilen
+                initialization_content = '\n'.join(initialization_lines)
+
+                # Ändern der exe.py-Datei
+                _modify_exe_file("Your data classes", initialization_content)
+                print("Klassen aus data.py erfolgreich in exe.py kopiert.")
+            else:
+                print("Die data.py-Datei ist leer.")
+    else:
+        print("data.py-Datei nicht gefunden.")
+
+
+@click.command()
+@click.argument('output_name', default='output', required=False)
+def main(output_name):
+    """
+    Erstellt eine ausführbare Datei aus der Hauptdatei (main.py) und extrahiert die PIPELINE_ORDER-Liste.
+
+    :param output_name: Der Name der Ausgabedatei (Standard: 'output')
+    """
+    # Aktuelles Verzeichnis
+    current_directory = os.getcwd()
+    place_folder = None
+    
+    # Pfad zur Hauptdatei
+    main_path = os.path.join(current_directory, 'main.py')
+    
+    main_content = _read_main_file_content(main_path)
+    pipeline_order = _extract_pipeline_order(main_content)
+
+    if pipeline_order:
+        # Pfad zur project.toml-Datei
+        project_toml_path = os.path.join(current_directory, 'project.toml')
+
+        place_folder, project_name = _extract_project_info(project_toml_path)
+
+        if place_folder:
+            place_directory = os.path.join(current_directory, place_folder)
+        else:
+            click.echo("Ort (place) nicht gefunden.")
+    else:
+        click.echo("PIPELINE_ORDER nicht gefunden.")
+
+    # Erstelle und modifiziere die exe.py-Datei
+    _create_exe_file(project_name)
+    _find_classes()
+    _search_folders(place_directory, pipeline_order)
+    clean_exe_file()
+ 
+    
+
+    
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `jetline-0.0.51/jetline/logging.py` & `jetline-0.0.52/jetline/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,81 @@
-import logging
-import coloredlogs
-from colorama import Fore, Style, init
-
-
-init(autoreset=True)
-
-class CustomFormatter(coloredlogs.ColoredFormatter):
-    """
-    Log message formatter to apply custom color rules.
-    """
-
-    def format(self, record):
-        # Apply standard formatting first
-        s = super().format(record)
-
-
-        s = s.replace(" - ", Fore.LIGHTBLACK_EX + " - " + Style.RESET_ALL)
-
-        # Coloring filename and lineno together for consistency
-        filename_lineno = f"{Fore.WHITE}{record.filename}-{record.lineno}{Style.RESET_ALL}"
-        s = s.replace(f"{record.filename} - {record.lineno}", filename_lineno)
-
-        # Applying color to levelname according to the level_styles
-        levelname_color = self.level_styles.get(record.levelname.lower(), {}).get('color', 'white')
-        s = s.replace(record.levelname, getattr(Fore, levelname_color.upper(), Fore.WHITE) + record.levelname + Style.RESET_ALL)
-
-        # Ensuring date is colored the same as filename
-        s = s.replace(".py:", Fore.LIGHTBLACK_EX + ".py:" + Style.RESET_ALL)
-
-        return s
-
-# Initialize logger
-logger = logging.getLogger(__name__)
-
-field_styles = coloredlogs.DEFAULT_FIELD_STYLES.copy()
-field_styles['name'] = {'color': 'white'}
-field_styles['filename'] = {'color': 'white'}
-field_styles['lineno'] = {'color': 'white'}
-
-# Set colors for different log levels
-level_styles = {
-    'debug': {'color': 'green'},
-    'info': {'color': 'blue'},
-    'warning': {'color': 'yellow'},
-    'error': {'color': 'red'},
-    'critical': {'color': 'red', 'bold': True},
-}
-
-fmt = '%(asctime)s - %(name)s - %(levelname)s - %(message)s - %(filename)s:%(lineno)d'
-datefmt = '%Y-%m-%d %H:%M:%S'
-
-coloredlogs.install(level='DEBUG',
-                    logger=logger,
-                    fmt=fmt,
-                    datefmt=datefmt,
-                    level_styles=level_styles,
-                    field_styles=field_styles)
-
-for handler in logger.handlers:
-    handler.setFormatter(CustomFormatter(fmt, datefmt, level_styles=level_styles, field_styles=field_styles))
-
-handler = logging.FileHandler('app.log')
-handler.setLevel(logging.DEBUG)
-handler.setFormatter(CustomFormatter(fmt, datefmt, level_styles=level_styles, field_styles=field_styles))
-logger.addHandler(handler)
+import logging
+import coloredlogs
+from colorama import Fore, Style, init
+
+init(autoreset=True)
+
+
+class CustomFormatter(coloredlogs.ColoredFormatter):
+    """
+    CustomFormatter extends coloredlogs.ColoredFormatter to customize the log format.
+
+    Methods:
+        format(self, record): Formats the log record.
+
+    """
+    def format(self, record):
+        s = super().format(record)
+        s = s.replace(" - ", format_text(" - ", Fore.LIGHTBLACK_EX))
+        filename_lineno = format_text(f"{record.filename}-{record.lineno}", Fore.WHITE)
+        s = s.replace(f"{record.filename} - {record.lineno}", filename_lineno)
+        levelname_color = self.level_styles.get(record.levelname.lower(), {}).get('color', 'white')
+        s = s.replace(record.levelname,
+                      format_text(record.levelname, getattr(Fore, levelname_color.upper(), Fore.WHITE)))
+        s = s.replace(".py:", format_text(".py:", Fore.LIGHTBLACK_EX))
+        return s
+
+
+def format_text(text, fore_color):
+    """
+    Apply the given fore_color to the provided text.
+
+    :param text: The input text to be formatted.
+    :param fore_color: The color to apply to the text.
+    :return: The formatted text with the specified color.
+    """
+    return fore_color + text + Style.RESET_ALL
+
+
+def config_logger(logger):
+    """
+    Configure the logger with specific formatting and level settings.
+
+    Parameters:
+    - logger (logging.Logger): The logger object to configure.
+
+    Returns:
+    - None
+    """
+    field_styles = coloredlogs.DEFAULT_FIELD_STYLES.copy()
+    field_styles.update({'name': {'color': 'white'}, 'filename': {'color': 'white'}, 'lineno': {'color': 'white'}})
+
+    level_styles = {
+        'debug': {'color': 'green'},
+        'info': {'color': 'blue'},
+        'warning': {'color': 'yellow'},
+        'error': {'color': 'red'},
+        'critical': {'color': 'red', 'bold': True},
+    }
+
+    fmt = '%(asctime)s - %(name)s - %(levelname)s - %(message)s - %(filename)s:%(lineno)d'
+    datefmt = '%Y-%m-%d %H:%M:%S'
+
+    coloredlogs.install(level='DEBUG',
+                        logger=logger,
+                        fmt=fmt,
+                        datefmt=datefmt,
+                        level_styles=level_styles,
+                        field_styles=field_styles)
+
+    for handler in logger.handlers:
+        handler.setFormatter(CustomFormatter(fmt, datefmt, level_styles=level_styles, field_styles=field_styles))
+
+    handler = logging.FileHandler('app.log')
+    handler.setLevel(logging.DEBUG)
+    handler.setFormatter(CustomFormatter(fmt, datefmt, level_styles=level_styles, field_styles=field_styles))
+    logger.addHandler(handler)
+
+
+# Initialize and configure logger
+logger = logging.getLogger(__name__)
+config_logger(logger)
```

### Comparing `jetline-0.0.51/jetline/templates/nodes.py` & `jetline-0.0.52/jetline/templates/nodes.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-def node_function_1(data):
-    """
-    An example function that processes data and returns a modified version.
-
-    Args:
-        data: The input data to be processed.
-
-    Returns:
-        str: The processed data.
-    """
-    print("Input Data:", data)
-    processed_data = data + "asasdasdd"
-    print("Processed Data:", processed_data)
-    return processed_data
-
-def node_function_2(data):
-    """
-    An example function that returns the input data unchanged.
-
-    Args:
-        data: The input data.
-
-    Returns:
-        str: The input data.
-    """
-    print("Input Data:", data)
-    return data
+def node_function_1(data):
+    """
+    An example function that processes data and returns a modified version.
+
+    Args:
+        data: The input data to be processed.
+
+    Returns:
+        str: The processed data.
+    """
+    print("Input Data:", data)
+    processed_data = data + "asasdasdd"
+    print("Processed Data:", processed_data)
+    return processed_data
+
+def node_function_2(data):
+    """
+    An example function that returns the input data unchanged.
+
+    Args:
+        data: The input data.
+
+    Returns:
+        str: The input data.
+    """
+    print("Input Data:", data)
+    return data
```

### Comparing `jetline-0.0.51/jetline.egg-info/PKG-INFO` & `jetline-0.0.52/jetline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: jetline
-Version: 0.0.51
-Summary: Automated Pipeline Builder
-Home-page: https://github.com/your_username/jetline
-Author: Johannes Kanthak
-Author-email: johannes.kanthak@kdc-solutions.de
-License: MIT
-Keywords: pipeline automation
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: click==8.1.7
-Requires-Dist: colorama==0.4.6
-Requires-Dist: toml==0.10.2
-Requires-Dist: pandas==2.2.0
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: coloredlogs==15.0.1
-Requires-Dist: fastapi==0.110.0
+Metadata-Version: 2.1
+Name: jetline
+Version: 0.0.52
+Summary: Automated Pipeline Builder
+Home-page: https://github.com/your_username/jetline
+Author: Johannes Kanthak
+Author-email: johannes.kanthak@kdc-solutions.de
+License: MIT
+Keywords: pipeline automation
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: click==8.1.7
+Requires-Dist: colorama==0.4.6
+Requires-Dist: toml==0.10.2
+Requires-Dist: pandas==2.2.0
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: fastapi==0.110.0
```

### Comparing `jetline-0.0.51/jetline.egg-info/SOURCES.txt` & `jetline-0.0.52/jetline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jetline-0.0.51/setup.py` & `jetline-0.0.52/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from setuptools import setup, find_packages
-
-classifiers = [
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'License :: OSI Approved :: MIT License',
-    'Operating System :: OS Independent',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Topic :: Software Development :: Libraries :: Python Modules'
-]
-
-install_requires = [
-    'click==8.1.7',
-    'colorama==0.4.6',
-    'toml==0.10.2',
-    'pandas==2.2.0',
-    'openpyxl==3.1.2',
-    'coloredlogs==15.0.1',
-    'fastapi==0.110.0',
-    
-
-]
-
-setup(
-    name='jetline',
-    version='0.0.51',
-    description='Automated Pipeline Builder',
-    url='https://github.com/your_username/jetline',
-    author='Johannes Kanthak',
-    author_email='johannes.kanthak@kdc-solutions.de',
-    license='MIT',
-    classifiers=classifiers,
-    keywords='pipeline automation',
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=install_requires,
-    entry_points={
-        'console_scripts': [
-            'jetline = jetline.commands.info:main',
-            'jetline-setup = jetline.commands.installer:main',
-            'jetline-create-pipe = jetline.commands.create_pipe:main',
-            'jetline-analyze = jetline.commands.analyze_project:main',
-            'jetline-run = jetline.commands.run_pipeline:main [args]',
-            'jetline-to-exe = jetline.commands.to_exe:main'
-        ],
-    },
-)
+from setuptools import setup, find_packages
+
+classifiers = [
+    'Development Status :: 3 - Alpha',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Topic :: Software Development :: Libraries :: Python Modules'
+]
+
+install_requires = [
+    'click==8.1.7',
+    'colorama==0.4.6',
+    'toml==0.10.2',
+    'pandas==2.2.0',
+    'openpyxl==3.1.2',
+    'coloredlogs==15.0.1',
+    'fastapi==0.110.0',
+    
+
+]
+
+setup(
+    name='jetline',
+    version='0.0.52',
+    description='Automated Pipeline Builder',
+    url='https://github.com/your_username/jetline',
+    author='Johannes Kanthak',
+    author_email='johannes.kanthak@kdc-solutions.de',
+    license='MIT',
+    classifiers=classifiers,
+    keywords='pipeline automation',
+    packages=find_packages(),
+    include_package_data=True,
+    install_requires=install_requires,
+    entry_points={
+        'console_scripts': [
+            'jetline = jetline.commands.info:main',
+            'jetline-setup = jetline.commands.installer:main',
+            'jetline-create-pipe = jetline.commands.create_pipe:main',
+            'jetline-analyze = jetline.commands.analyze_project:main',
+            'jetline-run = jetline.commands.run_pipeline:main [args]',
+            'jetline-to-exe = jetline.commands.to_exe:main'
+        ],
+    },
+)
```

