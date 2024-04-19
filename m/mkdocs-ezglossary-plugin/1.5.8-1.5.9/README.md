# Comparing `tmp/mkdocs-ezglossary-plugin-1.5.8.tar.gz` & `tmp/mkdocs_ezglossary_plugin-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-ezglossary-plugin-1.5.8.tar", last modified: Fri Mar  8 15:13:57 2024, max compression
+gzip compressed data, was "mkdocs_ezglossary_plugin-1.5.9.tar", last modified: Fri Apr 19 08:54:49 2024, max compression
```

## Comparing `mkdocs-ezglossary-plugin-1.5.8.tar` & `mkdocs_ezglossary_plugin-1.5.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:57.142470 mkdocs-ezglossary-plugin-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-08 15:13:57.142470 mkdocs-ezglossary-plugin-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-08 15:13:57.142470 mkdocs-ezglossary-plugin-1.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:57.134471 mkdocs-ezglossary-plugin-1.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:57.138471 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:57.138471 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/definition.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/refs-list.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/refs-short.html
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/summary-table.html
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:57.142470 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-08 15:13:57.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-08 15:13:57.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:13:57.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-08 15:13:57.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-08 15:13:57.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-08 15:13:57.000000 mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:13:57.142470 mkdocs-ezglossary-plugin-1.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/tests/test_page_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-03-08 15:13:33.000000 mkdocs-ezglossary-plugin-1.5.8/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:49.402922 mkdocs_ezglossary_plugin-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-19 08:54:49.402922 mkdocs_ezglossary_plugin-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-19 08:54:49.402922 mkdocs_ezglossary_plugin-1.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:49.398922 mkdocs_ezglossary_plugin-1.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:49.398922 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:49.402922 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/definition.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/refs-list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/refs-short.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/summary-table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:49.402922 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-19 08:54:49.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-19 08:54:49.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:54:49.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 08:54:49.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 08:54:49.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 08:54:49.000000 mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:54:49.402922 mkdocs_ezglossary_plugin-1.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/tests/test_page_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-19 08:54:22.000000 mkdocs_ezglossary_plugin-1.5.9/tests/test_summary.py
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/LICENSE` & `mkdocs_ezglossary_plugin-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/PKG-INFO` & `mkdocs_ezglossary_plugin-1.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.5.8
+Version: 1.5.9
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/README.md` & `mkdocs_ezglossary_plugin-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/setup.cfg` & `mkdocs_ezglossary_plugin-1.5.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-ezglossary-plugin
-version = 1.5.8
+version = 1.5.9
 description = manage multiple glossaries in mkdocs
 keywords = mkdocs, glossary, plugin, references, links
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://github.com/realtimeprojects/mkdocs-ezglossary
 	Bug Tracker = https://github.com/realtimeprojects/mkdocs-ezglossary/issues
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/glossary.py` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/glossary.py`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/plugin.py` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.ws = r"[\n ]*"
         self.section = r"(\w+)"
         self.term = r"([\w -]+)"
         self.text = r"([^>]+)"
         self.dt = rf"<dt>(<.*>)?{self.section}:{self.term}(<.*>)?<\/dt>"
         self.dt_default = rf"<dt>(<.*>)?{self.term}(<.*>)?<\/dt>"
         self.dd = r"<dd>\n?((.|\n)+?)<\/dd>"
-        self.options = r"([\|\=\w\+]+)"
+        self.options = r"([\\\|\=\w\+]+)"
 
 
 _re = __re()
 
 
 class GlossaryConfig(config.base.Config):
     tooltip = config.config_options.Choice(('none', 'heading', 'full'), default="none")
@@ -142,48 +142,48 @@
                 log.warning("list_definitons and list_references disabled, summary will be empty")
 
             if not self._glossary.has(section=section):
                 log.warning(f"no section '{section}' found in glossary")
 
             terms = self._glossary.terms(section)
             theme = ""
-            for option in options.split("|"):
+            for option in options.replace("\\|", "|").split("|"):
                 if "theme" in option:
                     theme = "-" + option.split("=")[1]
             return template.render(f"summary{theme}.html",
                                    self.config,
                                    glossary=self._glossary,
                                    types=types,
                                    section=section,
                                    terms=terms,
                                    root=root)
             return html
 
-        regex = rf"<glossary::{_re.section}\|?{_re.options}?>"
+        regex = rf"<glossary::{_re.section}\\?\|?{_re.options}?>"
         return re.sub(regex, _replace, html)
 
     def _register_glossary_links(self, output, page):
         def _replace(mo):
             section = mo.group(1)
             section = "_" if section == "default" else section
             term = mo.group(2)
-            text = mo.group(3)[1:] if mo.group(3) else term
+            text = mo.group(3).lstrip("\\|") if mo.group(3) else term
             _id = self._glossary.add(section, term, 'refs', page)
             return f"{self._uuid}:{section}:{term}:<{text}>:{_id}"
 
         def _replace_default(mo):
             section = "_"
             term = mo.group(1)
-            text = mo.group(2)[1:] if mo.group(2) else term
+            text = mo.group(2).lstrip("\\|") if mo.group(2) else term
             _id = self._glossary.add(section, term, 'refs', page)
             return f"{self._uuid}:{section}:{term}:<{text}>:{_id}"
 
-        regex = rf"<{_re.section}\:{_re.term}(\|{_re.text})?>"
+        regex = rf"<{_re.section}\:{_re.term}(\\?\|{_re.text})?>"
         output = re.sub(regex, _replace, output)
-        regex = rf"<{_re.term}\:(\|{_re.text})?>"
+        regex = rf"<{_re.term}\:(\\?\|{_re.text})?>"
         return re.sub(regex, _replace_default, output)
 
     def _replace_inline_refs(self, output, page, root):
         def _replace(mo):
             section = mo.group(1)
             term = mo.group(2)
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/template.py` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/template.py`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/summary-detailed.html`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/summary-table.html` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/summary-table.html`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin/templates/summary.html` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin/templates/summary.html`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,18 @@
            title="{{ def.definition }}">{{term}}</a>
         {% else %}
         {{ term }}
         {% endif %}
     </dt>
     <dd>
         <ul>
-            {% for entry in glossary.get(section, term, 'refs') %}
+	    {% for type in types %}
+            {% for entry in glossary.get(section, term, type) %}
                 <li>
                     <a href="{{ root }}{{ entry.page.url }}#{{ entry.target }}">{{ entry.page.title }}</a>
                 </li>
             {% endfor %}
+	    {% endfor %}
         </ul>
     </dd>
     {% endfor %}
 </dl>
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ezglossary-plugin
-Version: 1.5.8
+Version: 1.5.9
 Summary: manage multiple glossaries in mkdocs
 Project-URL: Homepage, https://github.com/realtimeprojects/mkdocs-ezglossary
 Project-URL: Bug Tracker, https://github.com/realtimeprojects/mkdocs-ezglossary/issues
 Project-URL: Documentation, https://realtimeprojects.github.io/mkdocs-ezglossary
 Keywords: mkdocs,glossary,plugin,references,links
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt` & `mkdocs_ezglossary_plugin-1.5.9/src/mkdocs_ezglossary_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/tests/test_definitions.py` & `mkdocs_ezglossary_plugin-1.5.9/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/tests/test_link.py` & `mkdocs_ezglossary_plugin-1.5.9/tests/test_link.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,31 +45,36 @@
     config['tooltip'] = "full"
     html = mock.render_single(simple, config)
     log.debug(html)
 
     dl = xpath.body.p.a(name="test_second_refs_0",
                         title="*this text is formatted",
                         href="../simple.md#test_second_defs_0",
-                        text="second")
+                        text="mysecond")
     assert len(html.xpath(str(dl))) == 1
 
 
 def test_link_second_ref(simple, summary, config):
     config['tooltip'] = "full"
     summary = mock.render([simple, summary], config)['summary.md']
     log.debug(summary)
 
     dl = xpath.body.p.a(name="test_third_refs_1",
                         title="*third term",
                         href="../simple.md#test_third_defs_0",
                         text="third")
     assert len(summary.xpath(str(dl))) == 1
+    dl = xpath.body.p.a(name="test_third_refs_2",
+                        title="*third term",
+                        href="../simple.md#test_third_defs_0",
+                        text="mythird")
+    assert len(summary.xpath(str(dl))) == 1
 
 
-def test_link_default_ref_disabled(simple, summary, config):
+def test_link_default_ref_dis(simple, summary, config):
     """ Ensure definitions for the default sections are
         ignored when the configuration `use_default` is set
         to `False`.
     """
     summary = mock.render([simple, summary], config)['summary.md']
     log.debug(summary)
 
@@ -92,7 +97,19 @@
 
     dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
                         name="__default_refs_0",
                         title="",
                         href="../simple.md#__default_defs_0",
                         text="default")
     assert len(summary.xpath(str(dl))) == 1
+    dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
+                        name="__default2_refs_0",
+                        title="",
+                        href="../simple.md#__default2_defs_0",
+                        text="mydef2")
+    assert len(summary.xpath(str(dl))) == 1
+    dl = xpath.body.p.a(_class="mkdocs-ezglossary-link",
+                        name="__default3_refs_0",
+                        title="",
+                        href="../simple.md#__default3_defs_0",
+                        text="mydef3")
+    assert len(summary.xpath(str(dl))) == 1
```

### Comparing `mkdocs-ezglossary-plugin-1.5.8/tests/test_page_ref.py` & `mkdocs_ezglossary_plugin-1.5.9/tests/test_page_ref.py`

 * *Files identical despite different names*

### Comparing `mkdocs-ezglossary-plugin-1.5.8/tests/test_summary.py` & `mkdocs_ezglossary_plugin-1.5.9/tests/test_summary.py`

 * *Files identical despite different names*

