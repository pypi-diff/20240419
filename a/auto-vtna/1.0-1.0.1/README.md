# Comparing `tmp/auto_vtna-1.0.tar.gz` & `tmp/auto_vtna-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_vtna-1.0.tar", last modified: Thu Apr 18 14:34:38 2024, max compression
+gzip compressed data, was "auto_vtna-1.0.1.tar", last modified: Fri Apr 19 11:29:36 2024, max compression
```

## Comparing `auto_vtna-1.0.tar` & `auto_vtna-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:38.151407 auto_vtna-1.0/
--rw-rw-rw-   0        0        0      537 2024-04-18 14:34:38.149397 auto_vtna-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:38.121111 auto_vtna-1.0/auto_vtna/
--rw-rw-rw-   0        0        0   139045 2024-04-16 13:50:48.000000 auto_vtna-1.0/auto_vtna/Auto_VTNA_GUI.py
--rw-rw-rw-   0        0        0    22398 2024-04-16 15:37:30.000000 auto_vtna-1.0/auto_vtna/Automatic_VTNA.py
--rw-rw-rw-   0        0        0    23291 2024-04-12 13:10:19.000000 auto_vtna-1.0/auto_vtna/Normal_VTNA.py
--rw-rw-rw-   0        0        0    45069 2024-04-17 20:37:40.000000 auto_vtna-1.0/auto_vtna/VTNA_functions.py
--rw-rw-rw-   0        0        0    46238 2024-04-12 11:59:57.000000 auto_vtna-1.0/auto_vtna/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:34:38.145866 auto_vtna-1.0/auto_vtna.egg-info/
--rw-rw-rw-   0        0        0      537 2024-04-18 14:34:37.000000 auto_vtna-1.0/auto_vtna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-18 14:34:37.000000 auto_vtna-1.0/auto_vtna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:34:37.000000 auto_vtna-1.0/auto_vtna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-18 14:34:37.000000 auto_vtna-1.0/auto_vtna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 14:34:37.000000 auto_vtna-1.0/auto_vtna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 14:34:38.151407 auto_vtna-1.0/setup.cfg
--rw-rw-rw-   0        0        0      925 2023-11-07 22:50:37.000000 auto_vtna-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:29:36.163051 auto_vtna-1.0.1/
+-rw-rw-rw-   0        0        0      539 2024-04-19 11:29:36.162050 auto_vtna-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:29:36.137359 auto_vtna-1.0.1/auto_vtna/
+-rw-rw-rw-   0        0        0   139688 2024-04-19 11:26:22.000000 auto_vtna-1.0.1/auto_vtna/Auto_VTNA_GUI.py
+-rw-rw-rw-   0        0        0    22228 2024-04-18 20:28:15.000000 auto_vtna-1.0.1/auto_vtna/Automatic_VTNA.py
+-rw-rw-rw-   0        0        0    23125 2024-04-18 20:28:15.000000 auto_vtna-1.0.1/auto_vtna/Normal_VTNA.py
+-rw-rw-rw-   0        0        0    44993 2024-04-18 20:28:15.000000 auto_vtna-1.0.1/auto_vtna/VTNA_functions.py
+-rw-rw-rw-   0        0        0    48521 2024-04-19 11:25:57.000000 auto_vtna-1.0.1/auto_vtna/__init__.py
+-rw-rw-rw-   0        0        0     2813 2024-04-19 11:24:17.000000 auto_vtna-1.0.1/auto_vtna/running_codes 23dec.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:29:36.159043 auto_vtna-1.0.1/auto_vtna.egg-info/
+-rw-rw-rw-   0        0        0      539 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:29:36.164054 auto_vtna-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      929 2024-04-19 11:29:24.000000 auto_vtna-1.0.1/setup.py
```

### Comparing `auto_vtna-1.0/PKG-INFO` & `auto_vtna-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vtna
-Version: 1.0
+Version: 1.0.1
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0/auto_vtna/Auto_VTNA_GUI.py` & `auto_vtna-1.0.1/auto_vtna/Auto_VTNA_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import PySimpleGUI as sg
 import threading
 import pandas as pd
 import numpy as np
+import matplotlib
+#matplotlib.use('Qt5Agg')
+matplotlib.use('TkAgg')
 import matplotlib.pyplot as plt
 import auto_vtna
 import tkinter as tk
-from pandastable import Table
 from auto_vtna.Normal_VTNA import Normal_VTNA
 from auto_vtna.VTNA_functions import VTNA_omissions
 from auto_vtna.Automatic_VTNA import Automatic_VTNA
-from openpyxl.drawing.image import Image
+import openpyxl.cell._writer
 import copy
 import re
 import csv
 import tkinter as tk
 from tkinter import scrolledtext
 
 def extract_range_info(values,data):
@@ -190,21 +192,23 @@
         # Obtain species and stochiometry lists from dict input.
         species = list(stochiometry_list.keys())
         stochiometry = list(float(i) for i in stochiometry_list.values())
         # plot the data with mass balance. 
         auto_vtna.plot_data_MB(data, species, stochiometry, ylim=settings['ylim'],
                 t_unit=settings['t_unit'],y_unit=settings['y_unit'],
                 fig_size_scaler=settings['size_scaler'],plot_mode=plot_mode,
-                DP_scaler=settings['DP_scaler'],legend_outside=legend_outside)
+                DP_scaler=settings['DP_scaler'],legend_outside=legend_outside,
+                linewidth=settings['linewidth'])
     else:
         # Plot the data without mass balance shown. 
         auto_vtna.plot_data(data, ylim=settings['ylim'],
                 t_unit=settings['t_unit'],y_unit=settings['y_unit'],
                 fig_size_scaler=settings['size_scaler'],plot_mode=plot_mode,
-                DP_scaler=settings['DP_scaler'],legend_outside=legend_outside)
+                DP_scaler=settings['DP_scaler'],legend_outside=legend_outside,
+                linewidth=settings['linewidth'])
 
 def is_float(value):
     "Checks if a variable can be converted to a float."
     try:
         float(value)
         return True
     except ValueError:
@@ -383,15 +387,15 @@
     '''Plots concentration profiles using the plot_data_together function from
     auto_vtna. Applies keyword arguments based on the plot settings dictionary.'''
     legend_outside=True if settings['legend_position']=='outside' else False
     # Ensure that all exisiting plots are closed to avoid bugs.
     plt.close('all')
     auto_vtna.plot_data_together(kinetic_data, selected_species,ylim=settings['ylim'],
      y_unit=settings['y_unit'], t_unit=settings['t_unit'],legend_outside=legend_outside,
-     fig_size_scaler=settings['size_scaler'],DP_scaler=settings['DP_scaler'])
+     fig_size_scaler=settings['size_scaler'],DP_scaler=settings['DP_scaler'],linewidth=settings['linewidth'])
     
 def main():
     # NB: some parts of the main GUI code was written with help from OpenAI's ChatGTP.
     img = None # Placeholder for overlay score versus order plot image.
     fixed_orders={} # Placeholder for fixed_orders dictionary
     enable_plot_button = False  # Flag to track whether the calculation has been run
     # Define settings dictionaries for automatic VTNA calculation, the overlay score versus order plot, 
@@ -400,15 +404,15 @@
                             "iterations": 7, "constraint": 'monotonic', "score_interval": 0.15,
                             "fixed_order_species": None,"initial_mesh_denser":'True'}
     order_vs_overlay_plot_settings = {"y_unit":'M',"size_scaler1":1,"popup_scaler":1,"colour_scaler":1,
                             "contour_resolution":None,"datapoints":False,"interval":False,"zoom":'None',
                             "contour_cbar_max":None,"contour_cbar_min":None, "custom_title":None,"show_legend_popup":True,
                             'show_legend_main':True,'decimals_cbar':3,'annotate':True,"plot_score_interval":None}
     data_plotting_settings={"ylim":None,"t_unit":None,'y_unit':'M',"size_scaler":1,'DP_scaler':1,"mode":'Together',\
-                            "significant_figs":3,'legend_position':'Inside'}
+                            "significant_figs":3,'legend_position':'Inside','linewidth':1}
     overlay_plot_settings={'y_unit':'M',"size_scaler":1,"tt_scaler":1,"grid":False,"custom_title":None,"check_score":False,\
                            "check_fit":False,"constraint":'monotonic','deg':5,"fit_metric":'RMSE',
                            'score_settings_visibility':False,'DP_scaler':1,'xtick_rotation':0,'legend':True,
                            'legend_position':'Inside','extra_legend':'True','save':False,'saved_values':{},'line_scaler':1,
                            'tT_notation':'Automatic'}
     # Define placeholder dict for the Automatic VTNA results. 
     auto_vtna_results={"best_order_dict":{'':'','\t':'','\r':''},"order_vs_overlay_table":None,"interval_table":None,"plot_image":None}
@@ -693,15 +697,15 @@
                             if VTNA_auto_calculation.deg==1:
                                 # Determine a sensible number of decimals to include for the slope value. 
                                 rounding=6
                                 slope=VTNA_auto_calculation.best_slope
                                 order_of_magnitude_slope=round(np.log10(slope))
                                 rounding+=(-order_of_magnitude_slope)
                                 # Add the slope to the overlay score string. 
-                                overlay_score_string=overlay_score_string+f'\nSlope of linear fit at optimal orders (no data scaling): {round(VTNA_auto_calculation.best_slope,rounding)}'
+                                overlay_score_string=overlay_score_string+f'\nSlope of linear fit w/ best orders (w/o data scaling): {round(VTNA_auto_calculation.best_slope,rounding)}'
                             # Update the interval table using the intervals from the automatic VTNA calculation. 
                             df_interval=VTNA_auto_calculation.interval.round(decimals=5)
                             table_values=df_interval.values.tolist()
                             for i,value in enumerate(table_values):
                                 table_values[i]=tuple(value)
                             window['interval_table'].update(values=table_values)
                             window["Overlay Score"].update(overlay_score_string)
@@ -1673,15 +1677,17 @@
                      sg.Text("Time unit:"),
                      sg.InputText(key="t_unit", size=(5, 1),default_text=str(data_plotting_settings["t_unit"]))],
                     [sg.Text("Figure size scaler:"),
                      sg.InputText(key="size_scaler", size=(5, 1),default_text=float(data_plotting_settings["size_scaler"])),
                      sg.Text("Max y:"),
                      sg.InputText(key="ylim", size=(5, 1),default_text=str(data_plotting_settings["ylim"]))],
                     [sg.Text("Datapoint size scaler:"),
-                     sg.InputText(key="DP_scaler", size=(5, 1),default_text=float(data_plotting_settings["DP_scaler"]))],
+                     sg.InputText(key="DP_scaler", size=(4, 1),default_text=float(data_plotting_settings["DP_scaler"])),
+                     sg.Text("Linewidth:"),
+                     sg.InputText(key="linewidth", size=(4, 1),default_text=float(data_plotting_settings["linewidth"]))],
                     [sg.Text("Legend position:"),
                      sg.Combo(['Inside','outside'], default_value=data_plotting_settings["legend_position"],key="legend_position", enable_events=True, readonly=True)],
                     [sg.Text("Significant figures for initial conc. table:"),
                      sg.InputText(key="SF", size=(5, 1),default_text=float(data_plotting_settings["significant_figs"]))],
                     [sg.Text("Mode for visualising kinetic data:"),sg.Combo(['Scroll', 'Together', 'Separate'], default_value=data_plotting_settings["mode"],
                             key="mode", enable_events=True, readonly=True)],
                 ])],
@@ -1705,42 +1711,46 @@
                         y_unit = values_inspect_kinetic_data["y_unit"]
                         t_unit = values_inspect_kinetic_data["t_unit"]
                         if not is_float(values_inspect_kinetic_data["SF"]):
                             raise ValueError("Significant figures for initial concentration table must be a numerical value.")
                         significant_figures=int(abs(float(values_inspect_kinetic_data["SF"])))
                         data_plotting_settings["legend_position"]=values_inspect_kinetic_data["legend_position"]
                         DP_scaler = float(values_inspect_kinetic_data["DP_scaler"])
+                        linewidth = float(values_inspect_kinetic_data["linewidth"])
                         mode = values_inspect_kinetic_data["mode"]
                         if len(t_unit)==0 or t_unit=='None':
                             t_unit=None
                         size_scaler = float(values_inspect_kinetic_data["size_scaler"])
-                        data_plotting_settings["size_scaler"]=size_scaler
-                        data_plotting_settings["ylim"]=ylim
-                        data_plotting_settings["y_unit"]=y_unit
-                        data_plotting_settings["t_unit"]=t_unit
-                        data_plotting_settings["mode"]=mode
-                        data_plotting_settings["DP_scaler"]=DP_scaler
                         # Check that inputs are correctly defined to avoid errors. 
                         # Generate error pop-up windows if there are issues. 
                         if not (0.1 < size_scaler <= 3):
                             raise ValueError("Invalid figure size scaler. Must be between 0.1 and 3.")
                         if not (0 <= DP_scaler <= 5):
                             raise ValueError("Invalid datapoint size scaler. Must be between 0 and 5.")
+                        if not (0 <= linewidth <= 5):
+                            raise ValueError("Invalid linewidth. Must be between 0 and 5.")
                         if type(ylim)==float:
                             if not (0 < ylim):
                                 raise ValueError("Invalid concentration axis limit. Must be a number above 0.")
                         if type(ylim)==str:
                             if ylim!='None' and ylim!='':
                                 raise ValueError("Concentration axis limit must be a numerical value.")
                         if significant_figures==0 or significant_figures>9:
                             raise ValueError("Significant figures for initial concentration must be between 1 and 9.")
                         if type(ylim)==str:
                             if ylim!='None' and ylim!='':
                                 raise ValueError("Concentration axis limit must be a numerical value.")
                         data_plotting_settings["significant_figs"]=int(significant_figures)
+                        data_plotting_settings["size_scaler"]=size_scaler
+                        data_plotting_settings["ylim"]=ylim
+                        data_plotting_settings["y_unit"]=y_unit
+                        data_plotting_settings["t_unit"]=t_unit
+                        data_plotting_settings["mode"]=mode
+                        data_plotting_settings["DP_scaler"]=DP_scaler
+                        data_plotting_settings["linewidth"]=linewidth
                     except ValueError as e:
                             sg.popup_error(f"Invalid input: {e}")
                             continue
                 # React to the specifics of the users button click. 
                 if event_inspect_kinetic_data == "Generate Initial Concentration Table":
                     generate_initial_concentration_table(data,size_scaler,y_unit,significant_figures=data_plotting_settings["significant_figs"])
                 elif event_inspect_kinetic_data == "Plot Kinetic Data":
```

### Comparing `auto_vtna-1.0/auto_vtna/Automatic_VTNA.py` & `auto_vtna-1.0.1/auto_vtna/Automatic_VTNA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from auto_vtna.VTNA_functions import VTNA_orders, on_click
 import numpy as np
 import pandas as pd
-from num2words import num2words
-from sklearn.metrics import r2_score
-from sklearn.metrics import mean_squared_error
-from scipy.optimize import curve_fit
 import itertools
 from functools import partial
 import matplotlib.pyplot as plt
 from openpyxl.drawing.image import Image
 from io import BytesIO
-import copy
 import matplotlib.ticker as tkr
 import warnings
 
 class Automatic_VTNA:
     def __init__(self,data,VTNA_selection,order_range=[-1.5,2.5],resolution=10,deg=5, \
                  fit_metric='SE',iterations=4,constraint='monotonic',score_interval=0.15,\
                 fixed_order_species=None,initial_mesh_denser=True):
```

### Comparing `auto_vtna-1.0/auto_vtna/Normal_VTNA.py` & `auto_vtna-1.0.1/auto_vtna/Normal_VTNA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from auto_vtna.VTNA_functions import VTNA_new,data_scaling_y,score_fit,origin_line,simple_line
 import numpy as np
-from num2words import num2words
-from sklearn.metrics import r2_score
-from sklearn.metrics import mean_squared_error
 from scipy.optimize import curve_fit
 import matplotlib.pyplot as plt
 from polyfit import PolynomRegressor, Constraints
 import warnings
-from matplotlib.ticker import ScalarFormatter
 
 class Normal_VTNA:
     def __init__(self,data,VTNA_selection):
         # Initialise the Normal VTNA class. 
         self.data=data
         self.VTNA_selection=VTNA_selection
         # Perform normal VTNA calculation:
```

### Comparing `auto_vtna-1.0/auto_vtna/VTNA_functions.py` & `auto_vtna-1.0.1/auto_vtna/VTNA_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import pandas as pd
 from polyfit import PolynomRegressor, Constraints
 from num2words import num2words
 from sklearn.metrics import r2_score
 from sklearn.metrics import mean_squared_error
 from scipy.optimize import curve_fit
 import itertools
-from multiprocessing import Pool, cpu_count
 import copy
-from functools import partial
 import matplotlib.pyplot as plt
 import warnings
 
 def VTNA_orders(data,VTNA_selection,order_range=[-1.5,2.5],resolution=8,deg=5,fit_metric='RMSE',iterations=6,constraint='monotonic',
                 score_interval=0.15,fixed_order_species=None,initial_mesh_denser=True):
         """
         Calculates the overlay score across different reaction order values for each normalised species in the \
```

### Comparing `auto_vtna-1.0/auto_vtna/__init__.py` & `auto_vtna-1.0.1/auto_vtna/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -295,15 +295,16 @@
     reaction_species=data[experiments[0]].columns[1:]
     # Loop through each experiment and obtain the intial concentration of each reaction species.
     initial_conc_dict={'Reaction species':reaction_species}
     for j in experiments:
         initial_conc_dict[f'{j} init. conc.']=data[j].iloc[0,1:].to_numpy()
     return pd.DataFrame(initial_conc_dict)
 
-def plot_data(data, ylim=None, y_unit='M', t_unit=None, fig_size_scaler=1,plot_mode='together',legend_outside=False, DP_scaler=1):
+def plot_data(data, ylim=None, y_unit='M', t_unit=None, fig_size_scaler=1,plot_mode='together',
+    legend_outside=False, DP_scaler=1,linewidth=1):
     """
     Inputs the kinetic data "data" that has been imported from an excel file using pd.read_excel() \
     as a dictionary of DataFrames containing the concentration profiles for each different excess \
     experiment. Plots the concentration profiles of each each experiment in separate plots unless \
     plot_mode is set to 'together' or 'scrollable'.
     Args:
         data (dict): Kinetic data as a dictionary of Pandas dataframes.
@@ -311,15 +312,22 @@
         y_unit (str, optional): Concentration unit to be included in the Y axis label. 
         t_unit (str, optional): Time unit to be included in the X axis label. 
         fig_size_scaler (float or int, optional): Scaler to adjust the size of the graphs by the \
         selected factor.
         plot_mode (str): Either set to "scrollable" to generate a single graph which updates \
         to the next or previous graph by clicking right or left arrow keys, or 'together' to \
         plot graphs for each experiment together. If plot_mode is set to something else, \
-        graphs will pop-up one after the other. 
+        graphs will pop-up one after the other.
+        legend_outside (bol): Set to True to ensure that the to place the plot legend to the right \
+        of the plot axis object, or in a separate box if plot_mode=together. Set to False (by default) \
+        to show the legend in the main plot(s)
+        DP_scaler (float or int): Number by which the datapoints are scaled away from the standard size of 6. \
+        Can be set to 0 to remove datapoints all together.  
+        linewidth (float or int): Defines the linewidth of the graphs in the plot. Can be set to 0 to remove \
+        lines all together.  
     """
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
     if plot_mode=='together':
         addition=0
         if legend_outside:
@@ -339,15 +347,15 @@
             else:
                 row, col = divmod(i, num_cols)
                 ax = axs[row, col]
             time = rm_data[rm_data.columns[0]]
             ax.set_title(rm_name)
             # Plot kinetic profiles for each reaction species for a given reaction mixture data set
             for j in rm_data.columns[1:]:
-                ax.plot(time, rm_data[j], label=j, linestyle='-', marker='o',markersize=6*DP_scaler)
+                ax.plot(time, rm_data[j], label=j, linestyle='-', marker='o',markersize=6*DP_scaler,linewidth=linewidth)
             ax.set_xlabel(rm_data.columns[0])
             # Add a unit to the time axis title is specified. 
             if t_unit is not None:
                 ax.set_xlabel(f'{rm_data.columns[0]} / {t_unit}')
             ax.set_ylabel(f'Concentration / {y_unit}')
             # Define y-axis range up to ylim if defined.
             if ylim is not None:
@@ -377,33 +385,34 @@
         # Remove empty subplots if there are any
         for i in range(len(data)+addition, num_cols * num_rows):
             fig.delaxes(axs.flatten()[i])
         plt.show()
     elif plot_mode=='scrollable':
         # Define a class for creating scrollable plots
         class ScrollablePlot:
-            def __init__(self, data_dict, ylim=None, y_unit='M', t_unit=None, fig_size_scaler=1,legend_outside=legend_outside,DP_scaler=1):
+            def __init__(self, data_dict, ylim=None, y_unit='M', t_unit=None, fig_size_scaler=1,legend_outside=legend_outside,DP_scaler=1,linewidth=linewidth):
                 # Extract data and labels from the given dictionary
                 data_1 = [data_dict[i] for i, j in data_dict.items()]
                 data_labels = list(data_dict.keys())
                 # Initialize instance variables
                 self.data = data_1
                 self.labels = data_labels
                 self.current_plot_index = 0
                 self.ylim = ylim
                 self.y_unit = y_unit
                 self.t_unit = t_unit
                 self.fig_size_scaler = fig_size_scaler
                 self.legend_outside=legend_outside
                 self.DP_scaler=DP_scaler
+                self.linewidth=linewidth
                 # Create a Matplotlib figure and axis
                 self.fig, self.ax = plt.subplots()
                 # Create a note to inform user of scrolling feature.
                 note_text = 'NB: Use left or right arrows to scroll to other experiments.'
-                self.fig.text(0.5, 0.003, note_text, ha='left', color='gray')
+                self.fig.text(0.5, -0.05, note_text, ha='center', color='gray')
                 # Plot the initial data
                 self.plot_current_data()
                 # Enable hovering using mplcursors
                 mplcursors.cursor(hover=True)
                 # Connect the key press event to the corresponding method
                 self.fig.canvas.mpl_connect('key_press_event', self.on_key_press)
 
@@ -416,15 +425,15 @@
                 # Extract time and concentration data
                 t = current_data.columns[0]
                 time_column = current_data[t]
                 # Plot each concentration profile
                 for i in current_data.keys():
                     if i == t:
                         continue
-                    self.ax.plot(time_column, current_data[i], label=i, marker='o',markersize=6*self.DP_scaler)
+                    self.ax.plot(time_column, current_data[i], label=i, marker='o',markersize=6*self.DP_scaler,linewidth=self.linewidth)
                 # Set the figure size
                 self.fig.set_size_inches(7 *0.8* self.fig_size_scaler, 5 *0.8* self.fig_size_scaler)
                 # Set plot title
                 self.ax.set_title(f'Concentration profiles in {current_label}')
                 # Set x-axis label
                 if self.t_unit is not None:
                     self.ax.set_xlabel(f'Time / {self.t_unit}')
@@ -433,15 +442,15 @@
                 # Set y-axis label
                 self.ax.set_ylabel(f'Concentration / {self.y_unit}')
                 # Set y-axis limit if specified
                 if self.ylim is not None and isinstance(self.ylim, (float, int)):
                     self.ax.set_ylim(0, self.ylim)
                 # Display legend
                 if self.legend_outside:
-                    self.ax.legend(bbox_to_anchor=(1, 0.5))
+                    self.ax.legend(bbox_to_anchor=(1, 0.78))
                 else:
                     self.ax.legend()
                 # Adjust layout to prevent overlapping of titles and labels
                 plt.tight_layout()
                 # Redraw the plot
                 plt.draw()
             def on_key_press(self, event):
@@ -468,15 +477,15 @@
         for i in data.keys():
             plt.figure(figsize=(7*0.8*fig_size_scaler, 5*0.8*fig_size_scaler))
             time=data[i][t]
             # plot kinetic profiles for each reaction species for a given reaction mixture data set
             for j in data[i].keys():
                 if j==t:
                     continue
-                plt.plot(time,data[i][j],label=j,linestyle='-',marker='o',markersize=6*DP_scaler)
+                plt.plot(time,data[i][j],label=j,linestyle='-',marker='o',markersize=6*DP_scaler,linewidth=linewidth)
                 plt.title(i)
                 plt.xlabel(t)
                 if t_unit!=None:
                     plt.xlabel(f'{t} / {t_unit}')
                 plt.ylabel(f'Concentration / {y_unit}')
             # Define y-axis range up to ylim if defined. 
             if legend_outside:
@@ -489,40 +498,49 @@
                 fig_box = plt.gcf().get_window_extent()
                 fig_width_display = fig_box.width
                 # See by what fraction the figure width needs to be extended for outside legend.
                 legend_width_scaled=legend_width/fig_width_display
                 # Scale the right argument according to the legend width
                 plt.subplots_adjust(right=1 - legend_width_scaled)
                 # Place the legend outside the axis
-                plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+                plt.legend(loc='center left', bbox_to_anchor=(1, 0.78))
                 # Adjust figure size to increase width according to the outside legend width
                 fig_size = plt.gcf().get_size_inches()
                 fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                 plt.gcf().set_size_inches(fig_size)
             else:
                 plt.legend()
             if ylim!=None:
                 plt.ylim(0,ylim)
             #Use plt.show to complete plot and move to the next reaction mixture data set
             plt.show()
 
-def plot_data_together(data,species,ylim=None,y_unit='mM',fig_size_scaler=1,t_unit=None,legend_outside=False,DP_scaler=1):
+def plot_data_together(data,species,ylim=None,y_unit='mM',fig_size_scaler=1,t_unit=None,legend_outside=False,
+    DP_scaler=1,linewidth=1):
     """
     Inputs the kinetic data "data" that has been imported from an excel file using Pd.read_excel() \
     as a dictionary of DataFrames containing the concentration profiles for each different excess \
     experiment. Creates a plot with the concentration profiles of the selected reaction species from \
     each experiment. 
     Args:
         data (dict): Kinetic data as a dictionary of Pandas dataframes.
         species (list): List containing the reaction species whose concentration profiles \
         will be plotted. 
         ylim (float or int, optional): Y axis upper cutoff value so that Y∈[0,ylim]. 
         y_unit (str, optional): Concentration unit to be included in the Y axis label.
         fig_size_scaler (float or int, optional): Scaler to adjust the size of the graphs by the \
         selected factor.
+        t_unit (str): Unit of the time axis. Set to None by default (assuming the time unit is already \
+        provided in the time column of the kinetic data). Can be set to any string like 'min' or 'h'.
+        legend_outside (bol): Set to True to ensure that the to place the plot legend to the right \
+        of the plot axis object. Set to False (by default) to show the legend in the main plot window.\
+        DP_scaler (float or int): Number by which the datapoints are scaled away from the standard size of 6. \
+        Can be set to 0 to remove datapoints all together.  
+        linewidth (float or int): Defines the linewidth of the graphs in the plot. Can be set to 0 to remove \
+        lines all together.  
     """
     # Identify the first key in the data dictionary
     RM1=list(data.keys())[0]
     # Identify the time column unit for the first reaction mixture data set
     t=data[RM1].columns[0]
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
@@ -533,15 +551,15 @@
     fig, ax = plt.subplots(figsize=(7*0.8*fig_size_scaler, 5*0.8*fig_size_scaler))
     for i in data.keys():
         time=data[i][t]
         # plot kinetic profiles for the chosen species for each reaction mixture data set
         for j in data[i].keys():
             if j==t or j not in species:
                 continue
-            ax.plot(time,data[i][j],label=f'{i},{j}',linestyle='-',marker='o',markersize=6*DP_scaler)
+            ax.plot(time,data[i][j],label=f'{i}, {j}',linestyle='-',marker='o',markersize=6*DP_scaler,linewidth=linewidth)
             ax.set_title(f'concentration profiles for {species}')
             ax.set_xlabel(t_label)
             ax.set_ylabel(f'concentration / {y_unit}')
         # Define y-axis range up to ylim if defined.
         if ylim!=None:
             ax.ylim(0,ylim)
     if legend_outside:
@@ -554,25 +572,26 @@
         fig_box = plt.gcf().get_window_extent()
         fig_width_display = fig_box.width
         # See by what fraction the figure width needs to be extended for outside legend.
         legend_width_scaled=legend_width/fig_width_display
         # Scale the right argument according to the legend width
         plt.subplots_adjust(right=1 - legend_width_scaled)
         # Place the legend outside the axis
-        plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+        plt.legend(loc='center left', bbox_to_anchor=(1, 0.78))
         # Adjust figure size to increase width according to the outside legend width
         fig_size = plt.gcf().get_size_inches()
         fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
         plt.gcf().set_size_inches(fig_size)
     else:
         ax.legend()
     plt.tight_layout()
     plt.show()
 
-def plot_data_MB(data, species, stochiometry, scaler=1, ylim=None, t_unit=None, y_unit='mM', fig_size_scaler=1,plot_mode='together',legend_outside=False,DP_scaler=1):
+def plot_data_MB(data, species, stochiometry, scaler=1, ylim=None, t_unit=None, y_unit='mM', 
+    fig_size_scaler=1,plot_mode='together',legend_outside=False,DP_scaler=1,linewidth=1):
     """
     Inputs the kinetic data "data" that has been imported from an excel file using Pd.read_excel() \
     as a dictionary of DataFrames containing the concentration profiles for each different excess \
     experiment. Plots the concentration profiles of each each experiment with the mass balance relative \
     to time=0 of the chosen reaction species and their stochiometries. The graphs can be plotted in one \
     figure (plot_mode = 'together'), in separate pop-up figures (plot_mode='separate') or in a single \
     figure that can be updated upon 
@@ -586,14 +605,21 @@
         y_unit (str, optional): Concentration unit to be included in the Y axis label.
         fig_size_scaler (float or int, optional): Scaler to adjust the size of the graphs by the \
         selected factor.
         plot_mode (str): Either set to "scrollable" to generate a single graph which updates \
         to the next or previous graph by clicking right or left arrow keys, or 'together' to \
         plot graphs for each experiment together. If plot_mode is set to something else, \
         graphs will pop-up one after the other. 
+        legend_outside (bol): Set to True to ensure that the to place the plot legend to the right \
+        of the plot axis object, or in a separate box if plot_mode=together. Set to False (by default) \
+        to show the legend in the main plot(s)
+        DP_scaler (float or int): Number by which the datapoints are scaled away from the standard size of 6. \
+        Can be set to 0 to remove datapoints all together.  
+        linewidth (float or int): Defines the linewidth of the graphs in the plot. Can be set to 0 to remove \
+        lines all together.  
     """
     # Find the title of the time column of the experiment datasets
     RM1 = list(data.keys())[0]
     t = data[RM1].columns[0]
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
@@ -626,15 +652,15 @@
             Concs = []
             largest_conc = []
             time = data[i][t]
             # Create a curve for each reaction species
             for j in data[i].keys():
                 if j == t:
                     continue
-                ax.plot(time, data[i][j], label=j, linestyle='-', marker='o', markersize=6*DP_scaler)
+                ax.plot(time, data[i][j], label=j, linestyle='-', marker='o', markersize=6*DP_scaler,linewidth=linewidth)
                 ax.set_title(i)
                 ax.set_xlabel(t)
                 ax.set_ylabel(f'concentration / {y_unit}')
                 if ylim is not None:
                     ax.set_ylim(0, ylim)
                 largest_conc.append(max(data[i][j].to_numpy()))
                 if t_unit is not None:
@@ -647,15 +673,15 @@
             sums = np.zeros(len(Concs[0]))
             for i in Concs:
                 sums = sums + i
             # Use sums to find the % mass balance at each time relative to the initial value.
             MB = sums / sums[0] * 100 * scaler
             ax2 = ax.twinx()
             ax2.set_ylabel(f'Mass balance for:\n {MB_title_string[:-2]}', color="purple")
-            ax2.plot(time, MB, label="Mass balance %", linestyle='-', marker='o', color="purple",markersize=6*DP_scaler)
+            ax2.plot(time, MB, label="Mass balance %", linestyle='-', marker='o', color="purple",markersize=6*DP_scaler,linewidth=linewidth)
             ax2.plot([0, max(time)], [100, 100], linestyle='--', marker='', color='purple')
             ax2.legend(loc='upper center')
             # Ensure appropriate y limits with space for legends.
             ax2.set_ylim(0, max(MB) + 28)
             ax.set_ylim(0, max(largest_conc) + max(largest_conc) * 0.15)
         ax = axes[idx+1]
         handles, labels = axes[0].get_legend_handles_labels()
@@ -689,14 +715,15 @@
                 self.ylim=ylim
                 self.fig_size_scaler=fig_size_scaler
                 self.species=species
                 self.stochiometry=stochiometry
                 self.MB_title_string=MB_title_string
                 self.legend_outside=legend_outside
                 self.DP_scaler=DP_scaler
+                self.linewidth=linewidth
                 mplcursors.cursor(hover=True)
                 self.fig, self.ax = plt.subplots(figsize=(7 *0.8* fig_size_scaler, 5 *0.8* fig_size_scaler))
                 # Create a note to inform user of scrolling feature.
                 note_text = 'NB: Use left or right arrows to scroll to other experiments.'
                 self.fig.text(0.5, 0.003, note_text, ha='center', color='gray')
                 self.ax2=self.ax.twinx()
                 self.plot_current_data()
@@ -710,15 +737,15 @@
                 t=current_data.columns[0]
                 time_column=current_data[t]
                 Concs=[]
                 largest_conc=[]
                 for j in current_data.keys():
                     if j==t:
                         continue
-                    self.ax.plot(time_column,current_data[j],label=j,linestyle='-',marker='o',markersize=6*self.DP_scaler)
+                    self.ax.plot(time_column,current_data[j],label=j,linestyle='-',marker='o',markersize=6*self.DP_scaler,linewidth=self.linewidth)
                     self.ax.set_title(f'Concentration profiles in {current_label}')
                     self.fig.set_size_inches(7*0.8*self.fig_size_scaler, 5*0.8*self.fig_size_scaler)
                     self.ax.set_xlabel(t)
                     self.ax.set_ylabel(f'concentration / {self.y_unit}')
                     if self.ylim!=None:
                         self.ax.set_ylim(0,self.ylim)
                     largest_conc.append(max(current_data[j].to_numpy()))
@@ -732,15 +759,15 @@
                 sums=np.zeros(len(Concs[0]))
                 for i in Concs:
                     sums=sums+i
                 # Use sums to find the % mass balance at each time relative to the intial value.
                 MB=sums/sums[0]*100* scaler
                 self.ax2.set_ylabel(f'Mass balance for:\n {self.MB_title_string[:-2]}',color="purple")
                 self.ax2.yaxis.set_label_position('right')
-                self.ax2.plot(time_column,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*self.DP_scaler)
+                self.ax2.plot(time_column,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*self.DP_scaler,linewidth=self.linewidth)
                 self.ax2.plot([0,max(time_column)],[100,100],linestyle='--',marker='',color='purple')
                 self.ax2.legend(loc='upper center')
                 # Ensure appropriate y limits with space for legends. 
                 self.ax2.set_ylim(0,max(MB)+28)
                 self.ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
                 if self.legend_outside:
                     # Calculate the width of the legend dynamically based on the longest text element
@@ -752,15 +779,15 @@
                     fig_box = plt.gcf().get_window_extent()
                     fig_width_display = fig_box.width
                     # See by what fraction the figure width needs to be extended for outside legend.
                     legend_width_scaled=legend_width/fig_width_display
                     # Scale the right argument according to the legend width
                     self.fig.subplots_adjust(right=1 - legend_width_scaled)
                     # Place the legend outside the axis
-                    self.ax.legend(loc='center left', bbox_to_anchor=(1.17, 0.5))
+                    self.ax.legend(loc='center left', bbox_to_anchor=(1.17, 0.8))
                     # Adjust figure size to increase width according to the outside legend width
                     fig_size = plt.gcf().get_size_inches()
                     fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                     plt.gcf().set_size_inches(fig_size)
                 else:
                     self.ax.legend()
                 plt.tight_layout()
@@ -788,22 +815,22 @@
             largest_conc=[]
             fig,ax = plt.subplots(figsize=(7*0.8*fig_size_scaler, 5*0.8*fig_size_scaler))
             time=data[i][t]
             # Create a curve for each reaction species
             for j in data[i].keys():
                 if j==t:
                     continue
-                ax.plot(time,data[i][j],label=j,linestyle='-',marker='o',markersize=6*DP_scaler)
+                ax.plot(time,data[i][j],label=j,linestyle='-',marker='o',markersize=6*DP_scaler,linewidth=linewidth)
                 ax.set_title(i)
                 ax.set_xlabel(t)
                 ax.set_ylabel(f'concentration / {y_unit}')
                 if ylim!=None:
                     ax.set_ylim(0,ylim)
                 if legend_outside:
-                    ax.legend(bbox_to_anchor=(1,1))
+                    ax.legend(bbox_to_anchor=(1,0.78))
                 else:
                     ax.legend()
                 largest_conc.append(max(data[i][j].to_numpy()))
                 if t_unit!=None:
                     plt.xlabel(f'{t} / {t_unit}')
                 if j==t or j not in species:
                     continue
@@ -813,15 +840,15 @@
             sums=np.zeros(len(Concs[0]))
             for i in Concs:
                 sums=sums+i
             # Use sums to find the % mass balance at each time relative to the intial value.
             MB=sums/sums[0]*100*scaler
             ax2=ax.twinx()
             ax2.set_ylabel(f'Mass balance for:\n {MB_title_string[:-2]}',color="purple")
-            ax2.plot(time,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*DP_scaler)
-            ax2.plot([0,max(time)],[100,100],linestyle='--',marker='',color='purple',markersize=6*DP_scaler)
+            ax2.plot(time,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*DP_scaler,linewidth=linewidth)
+            ax2.plot([0,max(time)],[100,100],linestyle='--',marker='',color='purple',markersize=6*DP_scaler,linewidth=linewidth)
             ax2.legend(loc='upper center')
             # Ensure appropriate y limits with space for legends. 
             ax2.set_ylim(0,max(MB)+28)
             ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
             plt.show()
```

### Comparing `auto_vtna-1.0/auto_vtna.egg-info/PKG-INFO` & `auto_vtna-1.0.1/auto_vtna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-vtna
-Version: 1.0
+Version: 1.0.1
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0/setup.py` & `auto_vtna-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import path
 
 # Meta-data of the package.
 NAME = 'auto_vtna'
 DESCRIPTION = 'A Python package for efficient and automatic VTNA analysis'
 EMAIL = 'dd4518@ic.ac.uk'
 AUTHOR = 'Daniel Dalland'
-VERSION = 1.0
+VERSION = "1.0.1"
 REQUIRED = [
     'numpy',
     'pandas',
     'matplotlib',
     'polyfit',
     'num2words',
     'scikit-learn',
```

