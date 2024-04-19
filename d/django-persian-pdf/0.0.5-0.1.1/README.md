# Comparing `tmp/django_persian_pdf-0.0.5.tar.gz` & `tmp/django_persian_pdf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_persian_pdf-0.0.5.tar", last modified: Thu Apr 18 07:52:55 2024, max compression
+gzip compressed data, was "django_persian_pdf-0.1.1.tar", last modified: Fri Apr 19 07:57:51 2024, max compression
```

## Comparing `django_persian_pdf-0.0.5.tar` & `django_persian_pdf-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-18 07:52:55.072569 django_persian_pdf-0.0.5/
--rw-rw-r--   0 druid     (1000) druid     (1000)      183 2024-04-18 07:51:02.000000 django_persian_pdf-0.0.5/CHANGELOG.rst
--rw-rw-r--   0 druid     (1000) druid     (1000)     1090 2024-03-14 12:36:31.000000 django_persian_pdf-0.0.5/LICENSE
--rw-rw-r--   0 druid     (1000) druid     (1000)      115 2024-03-08 22:52:06.000000 django_persian_pdf-0.0.5/MANIFEST.in
--rw-r--r--   0 druid     (1000) druid     (1000)     4838 2024-04-18 07:52:55.072569 django_persian_pdf-0.0.5/PKG-INFO
--rw-rw-r--   0 druid     (1000) druid     (1000)     3451 2024-04-18 07:50:13.000000 django_persian_pdf-0.0.5/README.rst
--rw-rw-r--   0 druid     (1000) druid     (1000)     1977 2024-04-18 07:50:24.000000 django_persian_pdf-0.0.5/pyproject.toml
--rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-04-18 07:52:55.072569 django_persian_pdf-0.0.5/setup.cfg
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-18 07:52:55.068569 django_persian_pdf-0.0.5/src/
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-18 07:52:55.072569 django_persian_pdf-0.0.5/src/django_persian_pdf/
--rw-rw-r--   0 druid     (1000) druid     (1000)      104 2024-04-18 07:50:13.000000 django_persian_pdf-0.0.5/src/django_persian_pdf/__init__.py
--rw-rw-r--   0 druid     (1000) druid     (1000)      185 2024-04-04 18:58:41.000000 django_persian_pdf-0.0.5/src/django_persian_pdf/apps.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     2948 2024-01-12 14:26:45.000000 django_persian_pdf-0.0.5/src/django_persian_pdf/compilers.py
--rw-rw-r--   0 druid     (1000) druid     (1000)        0 2024-03-08 22:52:06.000000 django_persian_pdf-0.0.5/src/django_persian_pdf/py.typed
--rw-rw-r--   0 druid     (1000) druid     (1000)      236 2024-01-08 10:03:12.000000 django_persian_pdf-0.0.5/src/django_persian_pdf/responses.py
--rw-rw-r--   0 druid     (1000) druid     (1000)     1808 2024-04-18 07:50:13.000000 django_persian_pdf-0.0.5/src/django_persian_pdf/views.py
-drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-18 07:52:55.072569 django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/
--rw-r--r--   0 druid     (1000) druid     (1000)     4838 2024-04-18 07:52:55.000000 django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 druid     (1000) druid     (1000)      490 2024-04-18 07:52:55.000000 django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)        1 2024-04-18 07:52:55.000000 django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)       12 2024-04-18 07:52:55.000000 django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/requires.txt
--rw-rw-r--   0 druid     (1000) druid     (1000)       19 2024-04-18 07:52:55.000000 django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/top_level.txt
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 07:57:51.167474 django_persian_pdf-0.1.1/
+-rw-rw-r--   0 druid     (1000) druid     (1000)      285 2024-04-19 07:35:17.000000 django_persian_pdf-0.1.1/CHANGELOG.rst
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1090 2024-03-14 12:36:31.000000 django_persian_pdf-0.1.1/LICENSE
+-rw-rw-r--   0 druid     (1000) druid     (1000)      115 2024-03-08 22:52:06.000000 django_persian_pdf-0.1.1/MANIFEST.in
+-rw-r--r--   0 druid     (1000) druid     (1000)     5850 2024-04-19 07:57:51.167474 django_persian_pdf-0.1.1/PKG-INFO
+-rw-rw-r--   0 druid     (1000) druid     (1000)     4463 2024-04-19 07:57:30.000000 django_persian_pdf-0.1.1/README.rst
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1977 2024-04-19 07:34:33.000000 django_persian_pdf-0.1.1/pyproject.toml
+-rw-rw-r--   0 druid     (1000) druid     (1000)       38 2024-04-19 07:57:51.167474 django_persian_pdf-0.1.1/setup.cfg
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 07:57:51.159474 django_persian_pdf-0.1.1/src/
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 07:57:51.163474 django_persian_pdf-0.1.1/src/django_persian_pdf/
+-rw-rw-r--   0 druid     (1000) druid     (1000)      108 2024-04-19 07:20:34.000000 django_persian_pdf-0.1.1/src/django_persian_pdf/__init__.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)      185 2024-04-04 18:58:41.000000 django_persian_pdf-0.1.1/src/django_persian_pdf/apps.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     2948 2024-01-12 14:26:45.000000 django_persian_pdf-0.1.1/src/django_persian_pdf/compilers.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)        0 2024-03-08 22:52:06.000000 django_persian_pdf-0.1.1/src/django_persian_pdf/py.typed
+-rw-rw-r--   0 druid     (1000) druid     (1000)      236 2024-01-08 10:03:12.000000 django_persian_pdf-0.1.1/src/django_persian_pdf/responses.py
+-rw-rw-r--   0 druid     (1000) druid     (1000)     1812 2024-04-19 07:20:34.000000 django_persian_pdf-0.1.1/src/django_persian_pdf/views.py
+drwxrwxr-x   0 druid     (1000) druid     (1000)        0 2024-04-19 07:57:51.167474 django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/
+-rw-r--r--   0 druid     (1000) druid     (1000)     5850 2024-04-19 07:57:51.000000 django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 druid     (1000) druid     (1000)      490 2024-04-19 07:57:51.000000 django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)        1 2024-04-19 07:57:51.000000 django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)       12 2024-04-19 07:57:51.000000 django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/requires.txt
+-rw-rw-r--   0 druid     (1000) druid     (1000)       19 2024-04-19 07:57:51.000000 django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/top_level.txt
```

### Comparing `django_persian_pdf-0.0.5/LICENSE` & `django_persian_pdf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_persian_pdf-0.0.5/PKG-INFO` & `django_persian_pdf-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-persian-pdf
-Version: 0.0.5
+Version: 0.1.1
 Summary: Django class based views to generate pdf files using html or latex template.
 Author-email: Ali Abharya <abharya.dev@gmail.com>
 Maintainer-email: Ali Abharya <abharya.dev@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/bindruid/django-persian-pdf/blob/master/CHANGELOG.rst
 Project-URL: Repository, https://github.com/bindruid/django-persian-pdf
 Keywords: pdf,django,persian,xelatex
@@ -34,34 +34,35 @@
 Django Persian PDF
 =========================
 
 Django Persian PDF is a set of class based views allowing you to generate PDF reports
 using html or latex templates.
 Django Persian PDF under the hood uses two compiler to render template
 and build the actual pdf file:
--  Xelatex
--  Google Chrome
+
+-  **Xelatex**
+-  **Google Chrome**
 
 Using this approach avoids regular overhead for parsing html tags, improving overall
 response time and memory usage when generating large pdf files.
-Django Persian PDF follows django class based views and base on the compiler provide 4 generic view classes.
+Django Persian PDF follows django class based views and base on the compilers provide 4 generic view classes.
 The only difference is that these classes render their associated template and return a pdf file as response.
 Just like django views you can pass queryset or make context to be used in template.
-Here are the view classes available in `django_persian_pdf`:
+Here are the view classes available in **django_persian_pdf**:
 
--  `ChromePDFTemplateView` is an extension of django `TemplateView` which uses chrome and .html template to generate pdf file.
--  `ChromePDFDetailView` is an extension of django `DetailView` which uses chrome and .html template  to generate pdf file.
--  `LatexPDFTemplateView` is an extension of django `TemplateView` which uses latex and .tex template to generate pdf file.
--  `LatexPDFDetailView` is an extension of django `DetailView` which uses latex to and .tex template to generate pdf file.
+-  ``HTMLToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.html`` template to generate pdf file.
+-  ``HTMLToPDFDetailView`` is an extension of django ``DetailView`` using ``.html`` template  to generate pdf file.
+-  ``LatexToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.tex`` template to generate pdf file.
+-  ``LatexToPDFDetailView`` is an extension of django ``DetailView`` using ``.tex`` template to generate pdf file.
 
 Status
 ------
 
 .. image:: https://github.com/bindruid/django-persian-pdf/workflows/Test/badge.svg?branch=master
-   :target: https://github.com/bindruid/django-persian-pdf/actions
+   :target: https://github.com/bindruid/django-persian-pdf/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-persian-pdf.svg
    :target: https://pypi.python.org/pypi/django-persian-pdf
 
 .. image:: https://img.shields.io/pypi/pyversions/django-persian-pdf.svg
    :target: https://pypi.org/project/django-persian-pdf
 
@@ -78,57 +79,102 @@
 Install
 -------
 
 .. code-block:: bash
 
    pip install django-persian-pdf
 
+- Make sure you have installed either ``google-chrome-stable`` or ``texlive-xetex`` on your machine.
+
+.. code-block:: bash
+
+
+   sudo apt install google-chrome-stable
+   sudo apt install texlive-xetex
+
 Usage
 -----
 
-0. Make sure you have installed either `chrome_stable_` or `xelatex` on your machine.
-
 1. Edit settings.py and add `django_persian_pdf` to your `INSTALLED_APPS`.
 
 2. Inherit your views from appropriate Template or Detail view classes.
 
+Example #1: Using HTML Template to generate a PDF response
+
 .. code-block:: python
 
-    from django_persian_pdf import views
+    from django_persian_pdf import views as pdf_views
 
-    class TemplatePrint(views.ChromePDFTemplateView):
+    class TemplatePrint(pdf_views.HTMLToPDFTemplateView):
         template_name = 'payment_reports.html'
 
         def get_context_data(self, **kwargs):
             context = super().get_context_data()
             context['payments'] = Payments.objects.all()
             return context
 
-    class DetailPrint(views.ChromePDFDetailView):
+    class DetailPrint(pdf_views.HTMLToPDFDetailView):
         template_name = 'payment_detail.html'
         queryset = Payments.objects.all()
 
 
+
+Example #2: Using LaTeX Template to generate a PDF response
+
 .. code-block:: python
 
-    from django_persian_pdf import views
+    from django_persian_pdf import views as pdf_views
 
-    class TemplatePrint(views.LatexPDFTemplateView):
+    class TemplatePrint(pdf_views.LatexToPDFTemplateView):
         template_name = 'payment_reports.tex'
 
         def get_context_data(self, **kwargs):
             context = super().get_context_data()
             context['payments'] = Payments.objects.all()
             return context
 
-    class DetailPrint(views.LatexPDFDetailView):
+    class DetailPrint(pdf_views.LatexToPDFDetailView):
         template_name = 'payment_detail.tex'
         queryset = Payments.objects.all()
 
-3. Using latex template for persian requires you to have installed your persian fonts in home.
+Notes on LaTeX
+----------------
+
+1. Using latex template for with persian fonts requires you to have installed your persian fonts in home directory.
 
 .. code-block:: bash
 
 
    mkdir -p ~/.fonts
    cp /path_to_fonts/Vazirmatn.ttf ~/.fonts/
    fc-cache -f -v
+
+2. In latex template make sure you have used ``xepersian`` package as last package.
+
+3. Define persian fonts in latex template.
+
+4. You can use django template tags in latex template.
+
+Here is an example of latex template for a given view:
+
+.. code-block:: latex
+
+    \documentclass[a4paper,9pt]{letter}
+    \usepackage[portrait,margin=0.1in]{geometry}
+    \usepackage{xepersian}
+
+    \settextfont{Vazirmatn}
+    \setlatintextfont{Vazirmatn}
+    \setdigitfont[Scale=1.1]{Vazirmatn}
+
+
+    \begin{document}
+
+      {% for payment in payments %}
+        {{ payment.trace_code }}
+        \newline
+        {{ payment.amount }}
+        \newline
+      {% endfor %}
+
+    \end{document}
+
```

### Comparing `django_persian_pdf-0.0.5/pyproject.toml` & `django_persian_pdf-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools",
 ]
 
 [project]
 name = "django-persian-pdf"
-version = "0.0.5"
+version = "0.1.1"
 description = "Django class based views to generate pdf files using html or latex template."
 keywords = [
   "pdf",
   "django",
   "persian",
   "xelatex",
 ]
```

### Comparing `django_persian_pdf-0.0.5/src/django_persian_pdf/compilers.py` & `django_persian_pdf-0.1.1/src/django_persian_pdf/compilers.py`

 * *Files identical despite different names*

### Comparing `django_persian_pdf-0.0.5/src/django_persian_pdf/views.py` & `django_persian_pdf-0.1.1/src/django_persian_pdf/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 
     def get(self, request, *args, **kwargs):
         self.object = self.get_object()
         context = self.get_context_data(object=self.object)
         return self.render_to_response(context)
 
 
-class LatexPDFTemplateView(PDFTemplateView):
+class LatexToPDFTemplateView(PDFTemplateView):
     compiler_class = LatexCompiler
 
 
-class LatexPDFDetailView(PDFDetailView):
+class LatexToPDFDetailView(PDFDetailView):
     compiler_class = LatexCompiler
 
 
-class ChromePDFTemplateView(PDFTemplateView):
+class HTMLToPDFTemplateView(PDFTemplateView):
     compiler_class = ChromeCompiler
 
 
-class ChromePDFDetailView(PDFDetailView):
+class HTMLToPDFDetailView(PDFDetailView):
     compiler_class = ChromeCompiler
```

### Comparing `django_persian_pdf-0.0.5/src/django_persian_pdf.egg-info/PKG-INFO` & `django_persian_pdf-0.1.1/src/django_persian_pdf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-persian-pdf
-Version: 0.0.5
+Version: 0.1.1
 Summary: Django class based views to generate pdf files using html or latex template.
 Author-email: Ali Abharya <abharya.dev@gmail.com>
 Maintainer-email: Ali Abharya <abharya.dev@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/bindruid/django-persian-pdf/blob/master/CHANGELOG.rst
 Project-URL: Repository, https://github.com/bindruid/django-persian-pdf
 Keywords: pdf,django,persian,xelatex
@@ -34,34 +34,35 @@
 Django Persian PDF
 =========================
 
 Django Persian PDF is a set of class based views allowing you to generate PDF reports
 using html or latex templates.
 Django Persian PDF under the hood uses two compiler to render template
 and build the actual pdf file:
--  Xelatex
--  Google Chrome
+
+-  **Xelatex**
+-  **Google Chrome**
 
 Using this approach avoids regular overhead for parsing html tags, improving overall
 response time and memory usage when generating large pdf files.
-Django Persian PDF follows django class based views and base on the compiler provide 4 generic view classes.
+Django Persian PDF follows django class based views and base on the compilers provide 4 generic view classes.
 The only difference is that these classes render their associated template and return a pdf file as response.
 Just like django views you can pass queryset or make context to be used in template.
-Here are the view classes available in `django_persian_pdf`:
+Here are the view classes available in **django_persian_pdf**:
 
--  `ChromePDFTemplateView` is an extension of django `TemplateView` which uses chrome and .html template to generate pdf file.
--  `ChromePDFDetailView` is an extension of django `DetailView` which uses chrome and .html template  to generate pdf file.
--  `LatexPDFTemplateView` is an extension of django `TemplateView` which uses latex and .tex template to generate pdf file.
--  `LatexPDFDetailView` is an extension of django `DetailView` which uses latex to and .tex template to generate pdf file.
+-  ``HTMLToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.html`` template to generate pdf file.
+-  ``HTMLToPDFDetailView`` is an extension of django ``DetailView`` using ``.html`` template  to generate pdf file.
+-  ``LatexToPDFTemplateView`` is an extension of django ``TemplateView`` using ``.tex`` template to generate pdf file.
+-  ``LatexToPDFDetailView`` is an extension of django ``DetailView`` using ``.tex`` template to generate pdf file.
 
 Status
 ------
 
 .. image:: https://github.com/bindruid/django-persian-pdf/workflows/Test/badge.svg?branch=master
-   :target: https://github.com/bindruid/django-persian-pdf/actions
+   :target: https://github.com/bindruid/django-persian-pdf/actions?workflow=Test
 
 .. image:: https://img.shields.io/pypi/v/django-persian-pdf.svg
    :target: https://pypi.python.org/pypi/django-persian-pdf
 
 .. image:: https://img.shields.io/pypi/pyversions/django-persian-pdf.svg
    :target: https://pypi.org/project/django-persian-pdf
 
@@ -78,57 +79,102 @@
 Install
 -------
 
 .. code-block:: bash
 
    pip install django-persian-pdf
 
+- Make sure you have installed either ``google-chrome-stable`` or ``texlive-xetex`` on your machine.
+
+.. code-block:: bash
+
+
+   sudo apt install google-chrome-stable
+   sudo apt install texlive-xetex
+
 Usage
 -----
 
-0. Make sure you have installed either `chrome_stable_` or `xelatex` on your machine.
-
 1. Edit settings.py and add `django_persian_pdf` to your `INSTALLED_APPS`.
 
 2. Inherit your views from appropriate Template or Detail view classes.
 
+Example #1: Using HTML Template to generate a PDF response
+
 .. code-block:: python
 
-    from django_persian_pdf import views
+    from django_persian_pdf import views as pdf_views
 
-    class TemplatePrint(views.ChromePDFTemplateView):
+    class TemplatePrint(pdf_views.HTMLToPDFTemplateView):
         template_name = 'payment_reports.html'
 
         def get_context_data(self, **kwargs):
             context = super().get_context_data()
             context['payments'] = Payments.objects.all()
             return context
 
-    class DetailPrint(views.ChromePDFDetailView):
+    class DetailPrint(pdf_views.HTMLToPDFDetailView):
         template_name = 'payment_detail.html'
         queryset = Payments.objects.all()
 
 
+
+Example #2: Using LaTeX Template to generate a PDF response
+
 .. code-block:: python
 
-    from django_persian_pdf import views
+    from django_persian_pdf import views as pdf_views
 
-    class TemplatePrint(views.LatexPDFTemplateView):
+    class TemplatePrint(pdf_views.LatexToPDFTemplateView):
         template_name = 'payment_reports.tex'
 
         def get_context_data(self, **kwargs):
             context = super().get_context_data()
             context['payments'] = Payments.objects.all()
             return context
 
-    class DetailPrint(views.LatexPDFDetailView):
+    class DetailPrint(pdf_views.LatexToPDFDetailView):
         template_name = 'payment_detail.tex'
         queryset = Payments.objects.all()
 
-3. Using latex template for persian requires you to have installed your persian fonts in home.
+Notes on LaTeX
+----------------
+
+1. Using latex template for with persian fonts requires you to have installed your persian fonts in home directory.
 
 .. code-block:: bash
 
 
    mkdir -p ~/.fonts
    cp /path_to_fonts/Vazirmatn.ttf ~/.fonts/
    fc-cache -f -v
+
+2. In latex template make sure you have used ``xepersian`` package as last package.
+
+3. Define persian fonts in latex template.
+
+4. You can use django template tags in latex template.
+
+Here is an example of latex template for a given view:
+
+.. code-block:: latex
+
+    \documentclass[a4paper,9pt]{letter}
+    \usepackage[portrait,margin=0.1in]{geometry}
+    \usepackage{xepersian}
+
+    \settextfont{Vazirmatn}
+    \setlatintextfont{Vazirmatn}
+    \setdigitfont[Scale=1.1]{Vazirmatn}
+
+
+    \begin{document}
+
+      {% for payment in payments %}
+        {{ payment.trace_code }}
+        \newline
+        {{ payment.amount }}
+        \newline
+      {% endfor %}
+
+    \end{document}
+
```

