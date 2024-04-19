# Comparing `tmp/stimulsoft_dashboards-2024.2.3.tar.gz` & `tmp/stimulsoft_dashboards-2024.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimulsoft_dashboards-2024.2.3.tar", last modified: Tue Apr  2 07:47:48 2024, max compression
+gzip compressed data, was "stimulsoft_dashboards-2024.2.4.tar", last modified: Thu Apr 18 09:32:54 2024, max compression
```

## Comparing `stimulsoft_dashboards-2024.2.3.tar` & `stimulsoft_dashboards-2024.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:48.231904 stimulsoft_dashboards-2024.2.3/
--rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_dashboards-2024.2.3/LICENSE.md
--rw-rw-rw-   0        0        0     8477 2024-04-02 07:47:48.231904 stimulsoft_dashboards-2024.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     7676 2024-03-05 12:00:02.000000 stimulsoft_dashboards-2024.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 07:47:48.231904 stimulsoft_dashboards-2024.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1217 2024-03-27 13:55:18.000000 stimulsoft_dashboards-2024.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:48.224343 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:48.230400 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/report/
--rw-rw-rw-   0        0        0      167 2024-02-16 16:29:50.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/report/StiDashboard.py
--rw-rw-rw-   0        0        0       40 2024-02-19 15:40:28.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/report/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:48.231904 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/
--rw-rw-rw-   0        0        0      660 2024-02-16 16:35:24.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/StiResourcesHelper.py
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:48.231904 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/scripts/
--rw-rw-rw-   0        0        0      502 2024-02-16 16:24:27.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/scripts/StiScriptResource.py
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/scripts/__init__.py
--rw-rw-rw-   0        0        0   702893 2024-04-02 07:20:36.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js
--rw-rw-rw-   0        0        0   195202 2024-04-02 07:23:18.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.pack.js
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:48.229347 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/
--rw-rw-rw-   0        0        0     8477 2024-04-02 07:47:48.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2024-04-02 07:47:48.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:47:48.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-02 07:47:48.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-02 07:47:48.000000 stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.181113 stimulsoft_dashboards-2024.2.4/
+-rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_dashboards-2024.2.4/LICENSE.md
+-rw-rw-rw-   0        0        0     8477 2024-04-18 09:32:54.181113 stimulsoft_dashboards-2024.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7676 2024-03-05 12:00:02.000000 stimulsoft_dashboards-2024.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 09:32:54.181113 stimulsoft_dashboards-2024.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2024-04-16 11:07:52.000000 stimulsoft_dashboards-2024.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.175079 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.177280 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/report/
+-rw-rw-rw-   0        0        0      167 2024-02-16 16:29:50.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/report/StiDashboard.py
+-rw-rw-rw-   0        0        0       40 2024-02-19 15:40:28.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/report/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.178107 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/
+-rw-rw-rw-   0        0        0      660 2024-02-16 16:35:24.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/StiResourcesHelper.py
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.180113 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/
+-rw-rw-rw-   0        0        0      502 2024-02-16 16:24:27.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/StiScriptResource.py
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/__init__.py
+-rw-rw-rw-   0        0        0   703179 2024-04-18 06:24:26.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js
+-rw-rw-rw-   0        0        0   195252 2024-04-18 06:27:06.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.pack.js
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:54.176229 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/
+-rw-rw-rw-   0        0        0     8477 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-18 09:32:54.000000 stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/top_level.txt
```

### Comparing `stimulsoft_dashboards-2024.2.3/LICENSE.md` & `stimulsoft_dashboards-2024.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.3/PKG-INFO` & `stimulsoft_dashboards-2024.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft_dashboards
-Version: 2024.2.3
+Version: 2024.2.4
 Summary: Data visualization in Python applications.
 Home-page: https://www.stimulsoft.com/en/products/dashboards-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_dashboards-2024.2.3/README.md` & `stimulsoft_dashboards-2024.2.4/README.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.3/setup.py` & `stimulsoft_dashboards-2024.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as file:
     readmeFile = file.read()
 
 setup(
     name = 'stimulsoft_dashboards',
-    version = '2024.2.3',
+    version = '2024.2.4',
     author = 'Stimulsoft',
     author_email = 'info@stimulsoft.com',
     description = 'Data visualization in Python applications.',
     long_description = readmeFile,
     long_description_content_type = 'text/markdown',
     url = 'https://www.stimulsoft.com/en/products/dashboards-python',
     license = 'https://www.stimulsoft.com/en/licensing/developers',
@@ -20,12 +20,12 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Office/Business',
         'Topic :: Software Development'
     ],
-    install_requires = ['stimulsoft-reports==2024.2.3'],
+    install_requires = ['stimulsoft-reports==2024.2.4'],
     packages = find_packages(include=['stimulsoft_dashboards', 'stimulsoft_dashboards.*']),
     package_data = {'stimulsoft_dashboards': ['**/scripts/*.js']},
     python_requires = '>=3.10'
 )
```

### Comparing `stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/StiResourcesHelper.py` & `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/StiResourcesHelper.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js` & `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 /*
 Stimulsoft.Dashboards.JS
-Version: 2024.2.3
-Build date: 2024.04.02
+Version: 2024.2.4
+Build date: 2024.04.18
 License: https://www.stimulsoft.com/en/licensing/reports
 */
 ! function(t) {
     var e;
     "undefined" != typeof process && process.__nwjs || "object" != typeof exports || "undefined" == typeof module ? "function" == typeof define && define.amd ? define(["./stimulsoft.reports"], e => Object.assign(e, t(e.Stimulsoft))) : window.Stimulsoft ? window.Stimulsoft.Report && window.Stimulsoft.Report.StiReport ? Object.assign(window, t(window.Stimulsoft)) : window.Stimulsoft.dashboardsFactory = t : window.Stimulsoft = {
         dashboardsFactory: t
     } : module.exports = (e = require("./stimulsoft.reports"), Object.assign(e, t(e.Stimulsoft)))
 }(function(L) {
     var Z = L.StiOptions;
 
     function y(e, t) {
         for (var r in t) r in e ? y(e[r], t[r]) : e[r] = t[r];
         return e
     }
-    L && (L.__engineVersion && "2024.2.3" !== L.__engineVersion ? console.warn("Scripts versions mismatch: engine ver. = %s; dashboards ver. = 2024.2.3", L.__engineVersion) : "2024.2.3" !== L.__reportsVersion && console.warn("Scripts versions mismatch: reports ver. = %s; dashboards ver. = 2024.2.3", L.__reportsVersion));
+    L && (L.__engineVersion && "2024.2.4" !== L.__engineVersion ? console.warn("Scripts versions mismatch: engine ver. = %s; dashboards ver. = 2024.2.4", L.__engineVersion) : "2024.2.4" !== L.__reportsVersion && console.warn("Scripts versions mismatch: reports ver. = %s; dashboards ver. = 2024.2.4", L.__reportsVersion));
     var L = y(L || {}, {
             Dashboard: {
                 Components: {
                     Panel: {},
                     Button: {},
                     Cards: {},
                     Helpers: {},
@@ -9765,16 +9765,27 @@
                 }
             }
             static imageDraw(e, t, r) {
                 let i = Lu.getImageBytesFromObject(r);
                 e.drawImage(i, t)
             }
             static drawWordWrapText(e, t, r, i, s, n, l, a, o) {
-                let u = Gu.getStringFormatGeom(e),
-                    h = (u.alignment = mn.Far, 0),
+                let u = e.getGenericStringFormat();
+                switch (u.trimming = Du.None, u.lineAlignment = mn.Center, s) {
+                    case z.Left:
+                        u.alignment = mn.Near;
+                        break;
+                    case z.Center:
+                        u.alignment = mn.Center;
+                        break;
+                    case z.Right:
+                        u.alignment = mn.Far;
+                        break
+                }
+                let h = 0,
                     m = (l.width < a.width ? l : a).width,
                     c = Nu.CenterCenter;
                 switch (s) {
                     case z.Left:
                         h = l.x;
                         break;
                     case z.Center:
@@ -9794,15 +9805,15 @@
                         break;
                     case Wt.Bottom:
                         d = l.y + l.height - a.height;
                         break
                 }
                 let g = new j(h, d, m, a.height),
                     p = F.t.StiCardsVisual.getFontGeom(r, o);
-                e.drawRotatedString6(t, p, i, g, e.getDefaultStringFormat(), c, 0, !0, l.width)
+                e.drawRotatedString6(t, p, i, g, u, c, 0, !0, l.width)
             }
             static drawText(e, t, r, i, s, n, l, a, o) {
                 let u = Gu.getStringFormatGeom(e),
                     h = (u.alignment = mn.Far, 0),
                     m = (l.width < a.width ? l : a).width;
                 switch (s) {
                     case z.Left:
@@ -10021,18 +10032,25 @@
                                     r = c.x + c.width - t;
                                     break
                             }
                             let i = new j(r, c.y, t, c.height);
                             Yu.imageDraw(g, i, l)
                         } else {
                             let e = this.processRowValue(l, n),
-                                t = ts.formatBasedOnColumnType2(S, n.textFormat, n, e),
-                                r = g.measureString(t, new ku(o.fontFamily.name, o.size, o.style, L.System.Drawing.GraphicsUnit.Point)),
-                                i = n.as(_t);
-                            null != i && i.wordWrap ? Yu.drawWordWrapText(g, t, o, a, n.horAlignment, n.vertAlignment, c, r, x) : Yu.drawText(g, t, o, a, n.horAlignment, n.vertAlignment, c, r, x)
+                                r = ts.formatBasedOnColumnType2(S, n.textFormat, n, e),
+                                t = n.as(_t),
+                                i = new ku(o.fontFamily.name, o.size, o.style, L.System.Drawing.GraphicsUnit.Point);
+                            if (null != t && t.wordWrap) {
+                                let e = g.getGenericStringFormat(),
+                                    t = (e.trimming = Du.None, e.alignment = mn.Center, e.lineAlignment = mn.Center, g.measureString2(r, i, c.width, e));
+                                Yu.drawWordWrapText(g, r, o, a, n.horAlignment, n.vertAlignment, c, t, x)
+                            } else {
+                                let e = g.measureString(r, i);
+                                Yu.drawText(g, r, o, a, n.horAlignment, n.vertAlignment, c, e, x)
+                            }
                         }
                     }
                 }
                 g.popClip();
                 let l = new Ku(C.lineColor, 1);
                 if (null == S.cards.cornerRadius || S.cards.cornerRadius.isEmpty) g.drawRectangle(l, r);
                 else {
@@ -14005,16 +14023,15 @@
                 h.popClip()
             }
             drawPieProgress(u, e, h, t, m, c, r) {
                 let i = this.processTrackColor(this.style.trackColor, m),
                     s = (u.fillEllipse2(i, e, null), 0 != t ? 360 / t * Math.abs(m.value) : t),
                     n = (360 < s && (s = 360), new P([new Rc(e, -90, s, null, null, null)]));
                 if (u.fillPath(r, n, e, null), c >= this.minFontSize) {
-                    let e = this.processFontName(
-                            this.element.font.fontFamily.name, m),
+                    let e = this.processFontName(this.element.font.fontFamily.name, m),
                         t = this.processFontStyle(this.element.font, m),
                         r = new H(e, c, t),
                         i = new ku(r.fontFamily.name, c, r.style, r.unit),
                         s = Nu.CenterCenter,
                         n = new Yl,
                         l = {
                             ref: Nu.CenterCenter
```

### Comparing `stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/PKG-INFO` & `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft-dashboards
-Version: 2024.2.3
+Version: 2024.2.4
 Summary: Data visualization in Python applications.
 Home-page: https://www.stimulsoft.com/en/products/dashboards-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_dashboards-2024.2.3/stimulsoft_dashboards.egg-info/SOURCES.txt` & `stimulsoft_dashboards-2024.2.4/stimulsoft_dashboards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

