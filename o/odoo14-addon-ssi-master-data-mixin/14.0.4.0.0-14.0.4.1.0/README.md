# Comparing `tmp/odoo14_addon_ssi_master_data_mixin-14.0.4.0.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_master_data_mixin-14.0.4.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 54205 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1278 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/__init__.py
--rw-r--r--  2.0 unx      544 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/__manifest__.py
--rw-r--r--  2.0 unx      192 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/models/__init__.py
--rw-r--r--  2.0 unx     2541 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     2405 b- defN 24-Apr-15 07:39 odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml
--rw-r--r--  2.0 unx     1862 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-15 07:39 odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD
-11 files, 58634 bytes uncompressed, 52077 bytes compressed:  11.2%
+Zip file size: 54295 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1278 b- defN 24-Apr-19 03:22 odoo/addons/ssi_master_data_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 24-Apr-19 03:22 odoo/addons/ssi_master_data_mixin/__init__.py
+-rw-r--r--  2.0 unx      544 b- defN 24-Apr-19 03:23 odoo/addons/ssi_master_data_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      192 b- defN 24-Apr-19 03:22 odoo/addons/ssi_master_data_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     2719 b- defN 24-Apr-19 03:22 odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-Apr-19 03:22 odoo/addons/ssi_master_data_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     2932 b- defN 24-Apr-19 03:22 odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml
+-rw-r--r--  2.0 unx     1862 b- defN 24-Apr-19 03:23 odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 03:23 odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-19 03:23 odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 24-Apr-19 03:23 odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/RECORD
+11 files, 59339 bytes uncompressed, 52167 bytes compressed:  12.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_master_data_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_master_data_mixin/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "Master Data Mixin",
-    "version": "14.0.4.0.0",
+    "version": "14.0.4.1.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "mail",
         "ssi_print_mixin",
```

## odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py

```diff
@@ -72,14 +72,22 @@
                 )
                 raise UserError(error_message)
 
     def action_generate_code(self):
         for record in self.sudo():
             record._create_sequence()
 
+    def action_reset_code(self):
+        for record in self.sudo():
+            record.write(
+                {
+                    "code": "/",
+                }
+            )
+
     def name_get(self):
         result = []
         for record in self:
             if self._show_code_on_display_name:
                 name = "[%s] %s" % (record.code, record.name)
             else:
                 name = record.name
```

## odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml

### odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml

```diff
@@ -15,14 +15,18 @@
     </field>
   </record>
   <record id="mixin_master_data_view_tree" model="ir.ui.view">
     <field name="name">mixin.master_data -tree</field>
     <field name="model">mixin.master_data</field>
     <field name="arch" type="xml">
       <tree>
+        <header>
+          <button name="action_reset_code" type="object" string="Reset code" confirm="Reset code. Are you sure?"/>
+          <button name="action_generate_code" type="object" string="Generate code" confirm="Generate code. Are you sure?"/>
+        </header>
         <field name="id" optional="hide"/>
         <field name="code"/>
         <field name="name"/>
         <field name="activity_ids" widget="list_activity" optional="show"/>
         <field name="active" widget="boolean_toggle"/>
       </tree>
     </field>
```

## Comparing `odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA` & `odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-master-data-mixin
-Version: 14.0.4.0.0
+Version: 14.0.4.1.0
 Summary: Master Data Mixin
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD` & `odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_master_data_mixin/README.rst,sha256=lLjXhCxU_VIVtry1OgQuBcHYRjVO-ENZiENQp9GdwFQ,1278
 odoo/addons/ssi_master_data_mixin/__init__.py,sha256=_euh7OtzMTDmyHY0E3tvYRWTi0ufnrMCH3IH8ZLtu0s,181
-odoo/addons/ssi_master_data_mixin/__manifest__.py,sha256=Ijj9Kyo-ltyI21i2IR4ToMa0TYvGqH7NSpfbO_GtsD0,544
+odoo/addons/ssi_master_data_mixin/__manifest__.py,sha256=e1pnxYTYQA-kWJtU_dP98QTcrnXeN4y3cw8T9lZFhvU,544
 odoo/addons/ssi_master_data_mixin/models/__init__.py,sha256=MH-geBjhVAfrd9wgl2Z6Ojz-WndWU4Sxeo-9yfB0hLE,192
-odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py,sha256=prhSjF8i8J-BXTNgp6atRjgZaC-FJDXofEUio1Myp0g,2541
+odoo/addons/ssi_master_data_mixin/models/mixin_master_data.py,sha256=9d3I8NGqgKO0KL8upGc2S5ocoH6PWZ-DQwzL99FP_W8,2719
 odoo/addons/ssi_master_data_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml,sha256=YUudvAOkcpWzf0XUvvGJYYaSaTC65GfNFZDbRcvWlN0,2405
-odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/METADATA,sha256=0Ref6div4mhaPIPRNtmLjVBNuUPb_hQfIYWdEPio-ys,1862
-odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_master_data_mixin-14.0.4.0.0.dist-info/RECORD,,
+odoo/addons/ssi_master_data_mixin/views/mixin_master_data_views.xml,sha256=PgcOOgaHa7UdZaxG73SoQ8xjXFksN9Pax6QFpY5ZJNk,2932
+odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/METADATA,sha256=-ZYWojW8TG_i7vZ_h-BLI3tZ3sCewHqt2odZtag7zow,1862
+odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_master_data_mixin-14.0.4.1.0.dist-info/RECORD,,
```

