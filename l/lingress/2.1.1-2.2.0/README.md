# Comparing `tmp/lingress-2.1.1.tar.gz` & `tmp/lingress-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingress-2.1.1.tar", last modified: Thu Apr 18 08:40:46 2024, max compression
+gzip compressed data, was "lingress-2.2.0.tar", last modified: Fri Apr 19 05:00:21 2024, max compression
```

## Comparing `lingress-2.1.1.tar` & `lingress-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-18 08:40:46.263654 lingress-2.1.1/
--rw-r--r--   0 aeiwz      (501) staff       (20)     1066 2024-02-28 15:01:52.000000 lingress-2.1.1/LICENSE
--rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-18 08:40:46.263587 lingress-2.1.1/PKG-INFO
--rw-r--r--   0 aeiwz      (501) staff       (20)     2220 2024-02-28 15:12:10.000000 lingress-2.1.1/README.rst
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-18 08:40:46.262547 lingress-2.1.1/lingress/
--rw-r--r--   0 aeiwz      (501) staff       (20)      119 2024-04-18 08:39:34.000000 lingress-2.1.1/lingress/__init__.py
--rw-r--r--   0 aeiwz      (501) staff       (20)    42166 2024-03-29 03:04:47.000000 lingress-2.1.1/lingress/lingress.py
--rw-r--r--   0 aeiwz      (501) staff       (20)     3083 2024-04-18 07:55:24.000000 lingress-2.1.1/lingress/utility.py
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-18 08:40:46.263357 lingress-2.1.1/lingress.egg-info/
--rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-18 08:40:46.000000 lingress-2.1.1/lingress.egg-info/PKG-INFO
--rw-r--r--   0 aeiwz      (501) staff       (20)      258 2024-04-18 08:40:46.000000 lingress-2.1.1/lingress.egg-info/SOURCES.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)        1 2024-04-18 08:40:46.000000 lingress-2.1.1/lingress.egg-info/dependency_links.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)       90 2024-04-18 08:40:46.000000 lingress-2.1.1/lingress.egg-info/requires.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)        9 2024-04-18 08:40:46.000000 lingress-2.1.1/lingress.egg-info/top_level.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)       80 2024-04-18 08:40:46.263841 lingress-2.1.1/setup.cfg
--rw-r--r--   0 aeiwz      (501) staff       (20)     1378 2024-04-18 08:39:53.000000 lingress-2.1.1/setup.py
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 05:00:21.979332 lingress-2.2.0/
+-rw-r--r--   0 aeiwz      (501) staff       (20)     1066 2024-02-28 15:01:52.000000 lingress-2.2.0/LICENSE
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-19 05:00:21.979253 lingress-2.2.0/PKG-INFO
+-rw-r--r--   0 aeiwz      (501) staff       (20)     2220 2024-02-28 15:12:10.000000 lingress-2.2.0/README.rst
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 05:00:21.977167 lingress-2.2.0/lingress/
+-rw-r--r--   0 aeiwz      (501) staff       (20)      119 2024-04-18 08:39:34.000000 lingress-2.2.0/lingress/__init__.py
+-rw-r--r--   0 aeiwz      (501) staff       (20)    42166 2024-03-29 03:04:47.000000 lingress-2.2.0/lingress/lingress.py
+-rw-r--r--   0 aeiwz      (501) staff       (20)     5919 2024-04-19 04:58:25.000000 lingress-2.2.0/lingress/utility.py
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 05:00:21.978899 lingress-2.2.0/lingress.egg-info/
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/PKG-INFO
+-rw-r--r--   0 aeiwz      (501) staff       (20)      258 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/SOURCES.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)        1 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/dependency_links.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)       90 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/requires.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)        9 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/top_level.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)       80 2024-04-19 05:00:21.979777 lingress-2.2.0/setup.cfg
+-rw-r--r--   0 aeiwz      (501) staff       (20)     1378 2024-04-19 04:59:18.000000 lingress-2.2.0/setup.py
```

### Comparing `lingress-2.1.1/LICENSE` & `lingress-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lingress-2.1.1/PKG-INFO` & `lingress-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lingress
-Version: 2.1.1
+Version: 2.2.0
 Summary: Metabolomics data analysis with univariate (linear regression) and visualization tools.
 Home-page: https://github.com/aeiwz/lingress.git
-Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.1.1.tar.gz
+Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.0.tar.gz
 Author: aeiwz
 Author-email: theerayut_aeiw_123@hotmail.com
 License: MIT
 Keywords: Omics,Chemometrics,Visualization,Data Analysis,Univariate,Linear Regression
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lingress-2.1.1/README.rst` & `lingress-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `lingress-2.1.1/lingress/lingress.py` & `lingress-2.2.0/lingress/lingress.py`

 * *Files identical despite different names*

### Comparing `lingress-2.1.1/lingress/utility.py` & `lingress-2.2.0/lingress/utility.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,27 +15,29 @@
         
         self.spectra = spectra
         self.ppm = ppm
         self.label = label
 
 
     def median_spectra_group(self, color_map=None, 
-                    title='<b>Medien Spectra of <sup>1</sup>H NMR data</b>', title_font_size=28, 
+                    title='<b>Median Spectra of <sup>1</sup>H NMR data</b>', title_font_size=28, 
                     legend_name='<b>Group</b>', legend_font_size=20, 
                     axis_font_size=20, 
                     fig_height = 800, fig_width = 2000,
                     line_width = 1.5, legend_order=None
                     ):
 
         from plotly import graph_objs as go
         from plotly import express as px
 
-        spectra = self.spectra
+        spectra = pd.DataFrame(self.spectra)
+        spectra.columns = self.ppm
         ppm = self.ppm
         label = self.label
+
         
 
         df_mean = spectra.groupby(label).median()
 
         #check if color_map is provided
         if color_map is None:
             color_map = dict(zip(df_mean.index, px.colors.qualitative.Plotly))
@@ -81,14 +83,89 @@
         #Add legend
 
         fig.update_layout(legend=dict( title=legend_name, font=dict(size=legend_font_size)))
         #Invert x-axis
         fig.update_xaxes(autorange="reversed")
         #Alpha background
         fig.update_layout(paper_bgcolor='rgba(0,0,0,0)',plot_bgcolor='rgba(0,0,0,0)')
-        #fig.update_layout(title='Medien Spectra', xaxis_title='δ <sup>1</sup>H', yaxis_title='Intensity')
+        #fig.update_layout(title='Median Spectra', xaxis_title='δ <sup>1</sup>H', yaxis_title='Intensity')
 
         #set y-axis tick format to scientific notation with 4 decimal places
         fig.update_layout(yaxis=dict(tickformat=".2e"))
 
         return fig
 
+
+    def single_spectra(self, color_map=None, 
+                    title='<b>Spectra of <sup>1</sup>H NMR data</b>', title_font_size=28, 
+                    legend_name='<b>Group</b>', legend_font_size=20, 
+                    axis_font_size=20, 
+                    fig_height = 800, fig_width = 2000,
+                    line_width = 1.5, legend_order=None
+                    ):
+
+        from plotly import graph_objs as go
+        from plotly import express as px
+
+        spectra = self.spectra
+        ppm = self.ppm
+        label = self.label
+        
+
+        df_spectra = pd.DataFrame(spectra)
+        df_spectra.columns = ppm
+
+        #check if color_map is provided
+        if color_map is None:
+            color_map = dict(zip(df_spectra.index, px.colors.qualitative.Plotly))
+        else:
+            if len(color_map) != len(df_spectra.index):
+                raise ValueError('Color map must have the same length as group labels')
+            else:
+                color_map = color_map
+
+        
+
+        #plot spectra
+        fig = go.Figure()
+        for i in df_spectra.index:
+            fig.add_trace(go.Scatter(x=ppm, y=df_spectra.loc[i,:], mode='lines', name=i, line=dict(color=color_map[i], width=line_width)))
+
+        fig.update_layout(
+            autosize=False,
+            width=fig_width,
+            height=fig_height,
+            margin=dict(
+                l=50,
+                r=50,
+                b=100,
+                t=100,
+                pad=4
+            )
+        )
+
+        fig.update_xaxes(showline=True, showgrid=False, linewidth=1, linecolor='rgb(82, 82, 82)', mirror=True)
+        fig.update_yaxes(showline=True, showgrid=False, linewidth=1, linecolor='rgb(82, 82, 82)', mirror=True)
+
+        #Set font size of label
+        fig.update_layout(font=go.layout.Font(size=axis_font_size))
+        #Add title
+        fig.update_layout(title={'text': title, 'xanchor': 'center', 'yanchor': 'top'}, 
+                        title_x=0.5, 
+                        xaxis_title="<b>δ<sup>1</sup>H</b>", yaxis_title="<b>Intensity</b>",
+                        title_font_size=title_font_size,
+                        title_yanchor="top",
+                        title_xanchor="center")
+
+        #Add legend
+
+        fig.update_layout(legend=dict( title=legend_name, font=dict(size=legend_font_size)))
+        #Invert x-axis
+        fig.update_xaxes(autorange="reversed")
+        #Alpha background
+        fig.update_layout(paper_bgcolor='rgba(0,0,0,0)',plot_bgcolor='rgba(0,0,0,0)')
+        #fig.update_layout(title='Median Spectra', xaxis_title='δ <sup>1</sup>H', yaxis_title='Intensity')
+
+        #set y-axis tick format to scientific notation with 4 decimal places
+        fig.update_layout(yaxis=dict(tickformat=".2e"))
+
+        return fig
```

### Comparing `lingress-2.1.1/lingress.egg-info/PKG-INFO` & `lingress-2.2.0/lingress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lingress
-Version: 2.1.1
+Version: 2.2.0
 Summary: Metabolomics data analysis with univariate (linear regression) and visualization tools.
 Home-page: https://github.com/aeiwz/lingress.git
-Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.1.1.tar.gz
+Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.0.tar.gz
 Author: aeiwz
 Author-email: theerayut_aeiw_123@hotmail.com
 License: MIT
 Keywords: Omics,Chemometrics,Visualization,Data Analysis,Univariate,Linear Regression
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lingress-2.1.1/setup.py` & `lingress-2.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'lingress',      
   packages = ['lingress'], 
-  version = '2.1.1',  
+  version = '2.2.0',  
   license='MIT', 
   description = 'Metabolomics data analysis with univariate (linear regression) and visualization tools.',
   long_description=DESCRIPTION,
   author = 'aeiwz',                 
   author_email = 'theerayut_aeiw_123@hotmail.com',     
   url = 'https://github.com/aeiwz/lingress.git',  
-  download_url = 'https://github.com/aeiwz/lingress/archive/refs/tags/v2.1.1.tar.gz',  
+  download_url = 'https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.0.tar.gz',  
   keywords = ['Omics', 'Chemometrics', 'Visualization', 'Data Analysis', 'Univariate', 'Linear Regression'],
   install_requires=[            
           'scikit-learn',
           'pandas',
           'numpy',
           'matplotlib',
           'seaborn',
```

