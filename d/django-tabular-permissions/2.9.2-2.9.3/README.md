# Comparing `tmp/django-tabular-permissions-2.9.2.tar.gz` & `tmp/django-tabular-permissions-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tabular-permissions-2.9.2.tar", last modified: Mon Jul 24 20:10:29 2023, max compression
+gzip compressed data, was "django-tabular-permissions-2.9.3.tar", last modified: Fri Apr 19 17:05:08 2024, max compression
```

## Comparing `django-tabular-permissions-2.9.2.tar` & `django-tabular-permissions-2.9.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1296 2015-12-09 21:00:08.000000 django-tabular-permissions-2.9.2/LICENSE
--rw-r--r--   0 ramez     (1000) ramez     (1000)      179 2018-10-08 05:14:58.000000 django-tabular-permissions-2.9.2/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8938 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7680 2023-07-24 19:50:21.000000 django-tabular-permissions-2.9.2/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     8938 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/PKG-INFO
--rw-r--r--   0 ramez     (1000) ramez     (1000)      653 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 ramez     (1000) ramez     (1000)        1 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 ramez     (1000) ramez     (1000)       20 2023-07-24 20:10:29.000000 django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1630 2023-07-24 20:10:27.000000 django-tabular-permissions-2.9.2/setup.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-07-24 19:34:42.000000 django-tabular-permissions-2.9.2/tabular_permissions/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2261 2023-07-24 13:22:48.000000 django-tabular-permissions-2.9.2/tabular_permissions/admin.py
--rw-r--r--   0 ramez     (1000) ramez     (1000)     2101 2020-09-15 11:02:36.000000 django-tabular-permissions-2.9.2/tabular_permissions/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1344 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.2/tabular_permissions/helpers.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/locale/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/
--rw-r--r--   0 ramez     (1000) ramez     (1000)      642 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1039 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/static/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/static/tabular_permissions/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2404 2019-07-25 12:41:51.000000 django-tabular-permissions-2.9.2/tabular_permissions/static/tabular_permissions/tabular_permissions.js
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.132889 django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-07-24 20:10:29.136889 django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/admin/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     7041 2020-02-01 07:47:30.000000 django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8512 2022-06-07 06:36:24.000000 django-tabular-permissions-2.9.2/tabular_permissions/widgets.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1295 2024-03-28 16:31:35.000000 django-tabular-permissions-2.9.3/LICENSE
+-rw-r--r--   0 ramez     (1000) ramez     (1000)      179 2018-10-08 05:14:58.000000 django-tabular-permissions-2.9.3/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8895 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7680 2023-07-24 20:12:02.000000 django-tabular-permissions-2.9.3/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.570730 django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     8895 2024-04-19 17:05:08.000000 django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/PKG-INFO
+-rw-r--r--   0 ramez     (1000) ramez     (1000)      653 2024-04-19 17:05:08.000000 django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/SOURCES.txt
+-rw-r--r--   0 ramez     (1000) ramez     (1000)        1 2024-04-19 17:05:08.000000 django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/dependency_links.txt
+-rw-r--r--   0 ramez     (1000) ramez     (1000)       20 2024-04-19 17:05:08.000000 django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1588 2024-04-19 17:00:49.000000 django-tabular-permissions-2.9.3/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/tabular_permissions/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2024-04-19 17:00:49.000000 django-tabular-permissions-2.9.3/tabular_permissions/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2178 2024-03-28 16:31:35.000000 django-tabular-permissions-2.9.3/tabular_permissions/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2101 2023-07-24 20:12:02.000000 django-tabular-permissions-2.9.3/tabular_permissions/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1298 2024-03-28 16:31:35.000000 django-tabular-permissions-2.9.3/tabular_permissions/helpers.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.570730 django-tabular-permissions-2.9.3/tabular_permissions/locale/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.570730 django-tabular-permissions-2.9.3/tabular_permissions/locale/ar/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/tabular_permissions/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)      642 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.3/tabular_permissions/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1039 2018-06-30 16:09:27.000000 django-tabular-permissions-2.9.3/tabular_permissions/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.570730 django-tabular-permissions-2.9.3/tabular_permissions/static/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/tabular_permissions/static/tabular_permissions/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2461 2024-03-28 16:39:14.000000 django-tabular-permissions-2.9.3/tabular_permissions/static/tabular_permissions/tabular_permissions.js
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.570730 django-tabular-permissions-2.9.3/tabular_permissions/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.570730 django-tabular-permissions-2.9.3/tabular_permissions/templates/tabular_permissions/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2024-04-19 17:05:08.574730 django-tabular-permissions-2.9.3/tabular_permissions/templates/tabular_permissions/admin/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7041 2023-07-24 20:12:02.000000 django-tabular-permissions-2.9.3/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9116 2024-04-19 16:55:14.000000 django-tabular-permissions-2.9.3/tabular_permissions/widgets.py
```

### Comparing `django-tabular-permissions-2.9.2/LICENSE` & `django-tabular-permissions-2.9.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,7 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `django-tabular-permissions-2.9.2/PKG-INFO` & `django-tabular-permissions-2.9.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: django-tabular-permissions
-Version: 2.9.2
+Version: 2.9.3
 Summary: Display django permissions in a tabular format that is user friendly, and highly customisable
 Home-page: https://github.com/RamezIssac/django-tabular-permissions
 Author: Ramez Ashraf
 Author-email: ramez@rasystems.io
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 
 
 django-tabular-permissions
 ##########################
```

### Comparing `django-tabular-permissions-2.9.2/README.rst` & `django-tabular-permissions-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/PKG-INFO` & `django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: django-tabular-permissions
-Version: 2.9.2
+Version: 2.9.3
 Summary: Display django permissions in a tabular format that is user friendly, and highly customisable
 Home-page: https://github.com/RamezIssac/django-tabular-permissions
 Author: Ramez Ashraf
 Author-email: ramez@rasystems.io
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 
 
 django-tabular-permissions
 ##########################
```

### Comparing `django-tabular-permissions-2.9.2/django_tabular_permissions.egg-info/SOURCES.txt` & `django-tabular-permissions-2.9.3/django_tabular_permissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.2/setup.py` & `django-tabular-permissions-2.9.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,38 +5,38 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-tabular-permissions',
-    version='2.9.2',
+    version='2.9.3',
     packages=['tabular_permissions'],
     include_package_data=True,
     license='BSD License',
     description='Display django permissions in a tabular format that is user friendly, and highly customisable',
     long_description=README,
     url='https://github.com/RamezIssac/django-tabular-permissions',
     author='Ramez Ashraf',
     author_email='ramez@rasystems.io',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
-)
+)
```

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/admin.py` & `django-tabular-permissions-2.9.3/tabular_permissions/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from django.core.exceptions import ImproperlyConfigured
 from tabular_permissions.widgets import TabularPermissionsWidget
 from . import app_settings
 
 User = get_user_model()
 
 
-class UserTabularPermissionsMixin(object):
+class UserTabularPermissionsMixin:
 
     def formfield_for_manytomany(self, db_field, request=None, **kwargs):
-        field = super(UserTabularPermissionsMixin, self).formfield_for_manytomany(db_field, request, **kwargs)
+        field = super().formfield_for_manytomany(db_field, request, **kwargs)
         if db_field.name == 'user_permissions':
             field.widget = TabularPermissionsWidget(db_field.verbose_name, db_field.name in self.filter_vertical)
             field.help_text = ''
         return field
 
 
-class GroupTabularPermissionsMixin(object):
+class GroupTabularPermissionsMixin:
     def formfield_for_manytomany(self, db_field, request=None, **kwargs):
-        field = super(GroupTabularPermissionsMixin, self).formfield_for_manytomany(db_field, request, **kwargs)
+        field = super().formfield_for_manytomany(db_field, request, **kwargs)
         if db_field.name == 'permissions':
             field.widget = TabularPermissionsWidget(db_field.verbose_name, db_field.name in self.filter_vertical,
                                                     'permissions')
             field.help_text = ''
         return field
```

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/app_settings.py` & `django-tabular-permissions-2.9.3/tabular_permissions/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/helpers.py` & `django-tabular-permissions-2.9.3/tabular_permissions/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from __future__ import unicode_literals
 from django.utils.translation import gettext_lazy as _
 
 
 def get_perm_name(model_name, perm_name):
-    return '%s_%s' % (perm_name, model_name)
+    return f'{perm_name}_{model_name}'
 
 
 def dummy_permissions_exclude(model):
     """
     A dummy function that excludes nothing,
     :param model:
     :return:
```

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.mo` & `django-tabular-permissions-2.9.3/tabular_permissions/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/locale/ar/LC_MESSAGES/django.po` & `django-tabular-permissions-2.9.3/tabular_permissions/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/static/tabular_permissions/tabular_permissions.js` & `django-tabular-permissions-2.9.3/tabular_permissions/static/tabular_permissions/tabular_permissions.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -27,26 +27,30 @@
         });
         $('.select-all.select-row').on('change', function() {
             var $this = $(this);
             $this.parents('tr').find('.checkbox').not('.select-all').each(function(i, elem) {
                 $(elem).prop('checked', $this.prop('checked'));
             })
         });
-        $('form').on('submit', function() {
-            var user_perms = [];
-            var table_permissions = $('#tabular_permissions');
-            var input_name = table_permissions.attr('data-input-name');
-            table_permissions.find("input[type=checkbox]").not('.select-all').each(function(i, elem) {
-                var $elem = $(elem);
-                if ($(elem).prop('checked')) {
-                    user_perms.push($elem.attr('data-perm-id'))
-                }
-            });
-            var user_group_permissions = $('[name=' + input_name + ']');
-            var output = [];
-            $.each(user_perms, function(key, value) {
-                output.push('<option value="' + value + '" selected="selected" style="display:none"></option>');
-            });
-            user_group_permissions.append(output);
-        })
+        setTimeout(
+            () => $('form').on('submit', function() {
+                var user_perms = [];
+                var table_permissions = $('#tabular_permissions');
+                var input_name = table_permissions.attr('data-input-name');
+                table_permissions.find("input[type=checkbox]").not('.select-all').each(function(i, elem) {
+                    var $elem = $(elem);
+                    if ($(elem).prop('checked')) {
+                        user_perms.push($elem.attr('data-perm-id'))
+                    }
+                });
+                var user_group_permissions = $('[name=' + input_name + ']');
+                var output = [];
+                $.each(user_perms, function(key, value) {
+                    output.push('<option value="' + value + '" selected="selected" style="display:none"></option>');
+                });
+                user_group_permissions.append(output);
+            }),
+            0
+        )
+
     })(django.jQuery);
 };
```

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html` & `django-tabular-permissions-2.9.3/tabular_permissions/templates/tabular_permissions/admin/tabular_permissions.html`

 * *Files identical despite different names*

### Comparing `django-tabular-permissions-2.9.2/tabular_permissions/widgets.py` & `django-tabular-permissions-2.9.3/tabular_permissions/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from __future__ import unicode_literals
-
 from collections import OrderedDict
+from itertools import chain
 
 from django import VERSION
 from django.apps import apps
+from django.contrib.auth import get_permission_codename
 from django.contrib.auth.models import Permission
 from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.contrib.contenttypes.models import ContentType
 from django.forms import SelectMultiple
 from django.template.loader import get_template
 from django.utils.encoding import force_str
 from django.utils.safestring import mark_safe
@@ -27,28 +27,28 @@
 
 
 class TabularPermissionsWidget(FilteredSelectMultiple):
     class Media:
         js = ('tabular_permissions/tabular_permissions.js',)
 
     def __init__(self, verbose_name, is_stacked, input_name='user_permissions', attrs=None, choices=()):
-        super(TabularPermissionsWidget, self).__init__(verbose_name, is_stacked, attrs, choices)
+        super().__init__(verbose_name, is_stacked, attrs, choices)
         self.managed_perms = []
         self.input_name = input_name  # in case of UserAdmin, it's 'user_permissions', GroupAdmin it's 'permissions'
         self.hide_original = True
 
     def render(self, name, value, attrs=None, renderer=None):
         choices = self.choices
         apps_available = OrderedDict()  # []  # main container to send to template
         user_permissions = Permission.objects.filter(id__in=value or []).values_list('id', flat=True)
         all_perms = Permission.objects.all().values('id', 'codename', 'content_type_id').order_by('codename')
-        excluded_perms = set([])
+        excluded_perms = set()
         codename_id_map = {}
         for p in all_perms:
-            codename_id_map['%s_%s' % (p['codename'], p['content_type_id'])] = p['id']
+            codename_id_map['{}_{}'.format(p['codename'], p['content_type_id'])] = p['id']
 
         # reminder_perms used to detect if the tabular permissions covers all permissions,
         # if true, we don't need to make the default widget visible.
         reminder_perms = codename_id_map.copy()
 
         # a global flag to either show or hide the other permission column in the table
         custom_permissions_available = False
@@ -67,54 +67,67 @@
                                                           for_concrete_model=USE_FOR_CONCRETE).pk
 
                 view_perm_name = get_perm_name(model_name, 'view')
                 add_perm_name = get_perm_name(model_name, 'add')
                 change_perm_name = get_perm_name(model_name, 'change')
                 delete_perm_name = get_perm_name(model_name, 'delete')
 
-                view_perm_id = codename_id_map.get('%s_%s' % (view_perm_name, ct_id),
+                view_perm_id = codename_id_map.get(f'{view_perm_name}_{ct_id}',
                                                    False) if 'view' in model._meta.default_permissions else False
-                add_perm_id = codename_id_map.get('%s_%s' % (add_perm_name, ct_id),
+                add_perm_id = codename_id_map.get(f'{add_perm_name}_{ct_id}',
                                                   False) if 'add' in model._meta.default_permissions else False
-                change_perm_id = codename_id_map.get('%s_%s' % (change_perm_name, ct_id),
+                change_perm_id = codename_id_map.get(f'{change_perm_name}_{ct_id}',
                                                      False) if 'change' in model._meta.default_permissions else False
-                delete_perm_id = codename_id_map.get('%s_%s' % (delete_perm_name, ct_id),
+                delete_perm_id = codename_id_map.get(f'{delete_perm_name}_{ct_id}',
                                                      False) if 'delete' in model._meta.default_permissions else False
-                if model._meta.permissions:
+
+                extra_default_permissions = []
+                for action in model._meta.default_permissions:
+                    if action in {'view', 'add', 'change', 'delete'}:
+                        continue
+                    extra_default_permissions.append(
+                        (
+                            get_permission_codename(action, model._meta),
+                            "Can %s %s" % (action, model._meta.verbose_name_raw),
+                        )
+                    )
+
+                if model._meta.permissions or extra_default_permissions:
                     custom_permissions_available = True
-                    for codename, perm_name in model._meta.permissions:
-                        c_perm_id = codename_id_map.get('%s_%s' % (codename, ct_id), False)
+                    for codename, perm_name in chain(model._meta.permissions, extra_default_permissions):
+                        c_perm_id = codename_id_map.get(f'{codename}_{ct_id}', False)
                         verbose_name = TRANSLATION_FUNC(codename, perm_name, ct_id)
                         model_custom_permissions.append(
                             (codename, verbose_name, c_perm_id)
                         )
                         model_custom_permissions_ids.append(c_perm_id)
 
                 if (
                         view_perm_id or add_perm_id or change_perm_id or delete_perm_id or model_custom_permissions):
                     excluded_perms.update(
                         [view_perm_id, add_perm_id, change_perm_id, delete_perm_id] + model_custom_permissions_ids)
-                    reminder_perms.pop('%s_%s' % (view_perm_name, ct_id), False)
-                    reminder_perms.pop('%s_%s' % (add_perm_name, ct_id), False)
-                    reminder_perms.pop('%s_%s' % (change_perm_name, ct_id), False)
-                    reminder_perms.pop('%s_%s' % (delete_perm_name, ct_id), False)
+                    reminder_perms.pop(f'{view_perm_name}_{ct_id}', False)
+                    reminder_perms.pop(f'{add_perm_name}_{ct_id}', False)
+                    reminder_perms.pop(f'{change_perm_name}_{ct_id}', False)
+                    reminder_perms.pop(f'{delete_perm_name}_{ct_id}', False)
                     for c, v, _id in model_custom_permissions:
-                        reminder_perms.pop('%s_%s' % (c, ct_id), False)
+                        reminder_perms.pop(f'{c}_{ct_id}', False)
 
                     # Because the logic of exclusion should/would work on both the tabular_permissin widget
                     # and the normal widget
                     # ie bydefautlwe exclude the session, admin log permissions and we dont want that on either widgets
                     if app.label in EXCLUDE_APPS \
                             or model_name in EXCLUDE_MODELS \
                             or EXCLUDE_FUNCTION(model):
                         continue
 
                     app_dict['models'][model_name] = {
                         'model_name': model_name,
                         'model': model,
+                        'label': force_str(model._meta.label_lower.replace('.', '_')),
                         'verbose_name_plural': force_str(model._meta.verbose_name_plural),
                         'verbose_name': force_str(model._meta.verbose_name),
                         'view_perm_id': view_perm_id,
                         'view_perm_name': view_perm_name,
                         'add_perm_id': add_perm_id,
                         'add_perm_name': add_perm_name,
                         'change_perm_id': change_perm_id,
```

