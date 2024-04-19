# Comparing `tmp/forecast_combine-0.0.2.tar.gz` & `tmp/forecast_combine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecast_combine-0.0.2.tar", max compression
+gzip compressed data, was "forecast_combine-0.0.3.tar", max compression
```

## Comparing `forecast_combine-0.0.2.tar` & `forecast_combine-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-08-09 11:13:58.574534 forecast_combine-0.0.2/LICENSE
--rw-r--r--   0        0        0     3791 2024-04-18 10:16:14.517329 forecast_combine-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-08-10 11:20:30.403617 forecast_combine-0.0.2/forecast_combine/__init__.py
--rwxr-xr-x   0        0        0    40996 2024-04-17 11:25:40.057693 forecast_combine-0.0.2/forecast_combine/forecast.py
--rwxr-xr-x   0        0        0    44575 2024-04-18 09:45:41.518588 forecast_combine-0.0.2/forecast_combine/model_select.py
--rw-r--r--   0        0        0    13643 2024-04-17 11:56:30.131379 forecast_combine-0.0.2/forecast_combine/reconcile.py
--rw-r--r--   0        0        0     5534 2024-04-12 15:21:42.963039 forecast_combine-0.0.2/forecast_combine/utils/explore.py
--rw-r--r--   0        0        0     3194 2024-04-17 09:26:53.214931 forecast_combine-0.0.2/forecast_combine/utils/metrics.py
--rwxr-xr-x   0        0        0     9434 2024-04-15 11:32:24.768704 forecast_combine-0.0.2/forecast_combine/utils/plotting.py
--rw-r--r--   0        0        0     1282 2024-04-18 10:16:12.237370 forecast_combine-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5082 1970-01-01 00:00:00.000000 forecast_combine-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-09 11:13:58.574534 forecast_combine-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3791 2024-04-18 10:16:14.517329 forecast_combine-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 11:40:31.366849 forecast_combine-0.0.3/forecast_combine/__init__.py
+-rwxr-xr-x   0        0        0    47676 2024-04-19 11:32:34.647494 forecast_combine-0.0.3/forecast_combine/forecast.py
+-rwxr-xr-x   0        0        0    49040 2024-04-19 11:36:03.211712 forecast_combine-0.0.3/forecast_combine/model_select.py
+-rw-r--r--   0        0        0    17317 2024-04-19 11:32:37.711438 forecast_combine-0.0.3/forecast_combine/reconcile.py
+-rw-r--r--   0        0        0     5534 2024-04-12 15:21:42.963039 forecast_combine-0.0.3/forecast_combine/utils/explore.py
+-rw-r--r--   0        0        0     3194 2024-04-17 09:26:53.214931 forecast_combine-0.0.3/forecast_combine/utils/metrics.py
+-rwxr-xr-x   0        0        0     9434 2024-04-15 11:32:24.768704 forecast_combine-0.0.3/forecast_combine/utils/plotting.py
+-rw-r--r--   0        0        0     1329 2024-04-19 11:58:09.803691 forecast_combine-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 forecast_combine-0.0.3/PKG-INFO
```

### Comparing `forecast_combine-0.0.2/LICENSE` & `forecast_combine-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.2/README.md` & `forecast_combine-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.2/forecast_combine/forecast.py` & `forecast_combine-0.0.3/forecast_combine/forecast.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """ Timeseries Forecasting with Insample, Validation and Out-of-Sample predictions"""
 __description__ = "Time Series Forecast"
 __author__ = "Amine Raboun - amineraboun@github.io"
 
 # Filter Warnings
-import logging
-logging.getLogger().setLevel(logging.ERROR)
 import warnings
 warnings.simplefilter('ignore')
-warnings.filterwarnings("ignore")
 
 ##############################################################################
 # Import Libraries & default configuration 
 ##############################################################################
 # Standard Inports
 from typing import Optional, Tuple, List
 import pandas as pd
@@ -72,31 +69,14 @@
 "AutoARIMA": StatsForecastAutoARIMA(),
 "AutoETS": StatsForecastAutoETS(),
 "AutoCES": StatsForecastAutoCES(),
 "AutoTheta": StatsForecastAutoTheta(),
 "AutoTBATS": StatsForecastAutoTBATS(seasonal_periods = 1),
 "Prophet": Prophet(),
 }
-# Pandas frequencies
-pandas_frequency_dict = {
-    "D": "daily",
-    "B": "business days",
-    "W": "weekly (end of week, default on Sunday)",
-    "M": "monthly (end of month)",
-    "Q": "quarterly (end of quarter)",
-    "A": "annual (end of year)",
-    "H": "hourly",
-    "T": "minutely",
-    "S": "secondly",
-    "L": "millisecondly",
-    "U": "microsecondly",
-    "BQ": "business quarterly (business quarter-end)",
-    "BA": "business annual (business year-end)",
-    "BH": "business hourly (business hour)"
-}
 
 ##############################################################################
 # Master Class Definition and Plot
 ##############################################################################
 class Forecast(object):
     """
     Forecast class for managing and evaluating forecast models.
@@ -111,30 +91,49 @@
     - forecaster_name (str, optional): The name of the forecasting model. Default is 'Naive'.
     - forecaster (object, optional): The forecasting model object. Default is None, which will use the model corresponding to forecaster_name.
     - exog_l (list, optional): List of exogenous variables for forecasting. Default is None.
     - freq (str, optional): The frequency of the time series data. Default is 'B' (business days).
 
     Attributes:
     -----------
-    - y (pd.Series): The time series data representing the dependent variable.
-    - X (pd.DataFrame or None): The DataFrame containing exogenous variables or None if there are no exogenous variables.
-    - forecaster_name (str): The name of the forecasting model used.
-    - forecaster (object): The forecasting model object used for forecasting.
-    - fh (ForecastingHorizon): The forecast horizon, i.e., the number of periods ahead to forecast.
-    - initial_window (int): The size of the initial training window.
-    - step_length (int): The step size for expanding window cross-validation.
-    - cv (ExpandingWindowSplitter): The cross-validation window used for expanding window validation.
-    - X_train (pd.DataFrame or None): The DataFrame containing exogenous variables for the training set or None if there are no exogenous variables.
-    - X_test (pd.DataFrame or None): The DataFrame containing exogenous variables for the test set or None if there are no exogenous variables.
-    - y_train (pd.Series): The dependent variable values for the training set.
-    - y_test (pd.Series): The dependent variable values for the test set.
-    - is_fitted (bool): True if the forecaster is fitted, False otherwise.
-    - is_evaluated (bool): True if the forecaster is evaluated on the test set, False otherwise.
-    - rs (numpy.random.RandomState): Random state for reproducibility.
+    - depvar (str): The column name representing the dependent variable for forecasting.
+    - exog_l (list): List of exogenous variables for forecasting.
+    - freq (str): The frequency of the time series data.
+    - forecaster_name (str): The name of the forecasting model.
+    - forecaster (object): The forecasting model object.
+    - _y (pd.Series): The dependent variable for forecasting.
+    - _X (pd.DataFrame): The exogenous variables for forecasting.
+    - _fh (ForecastingHorizon): The forecast horizon.
+    - _initial_window (int): The initial training window size.
+    - _step_length (int): The step size for expanding window cross-validation.
+    - _cv (ExpandingWindowSplitter): The cross-validation window.
+    - _X_train (pd.DataFrame): The training set of exogenous variables.
+    - _X_test (pd.DataFrame): The test set of exogenous variables.
+    - _y_train (pd.Series): The training set of the dependent variable.
+    - _y_test (pd.Series): The test set of the dependent variable.
+    - is_fitted (bool): A flag indicating if the model is fitted.
+    - _fitted (ForecastFit): An instance of the ForecastFit class containing the fitted model and insample performance metrics.
+    - is_evaluated (bool): A flag indicating if the model is evaluated.
+    - _eval (ForecastEval): An instance of the ForecastEval class containing the out-of-sample evaluation results.
     - plot (ForecastPlot): An instance of the ForecastPlot class for plotting utility.
+
+    Methods:
+    --------
+    - split_procedure_summary(verbose: bool=True) -> dict: Generate a summary of the cross-validation procedure.
+    - fit(on: str='all', fh: Optional[ForecastingHorizon]=None) -> ForecastFit: Fit the forecaster and compute insample results.
+    - evaluate() -> ForecastEval: Evaluate the forecaster out-of-sample.
+    - predict(X: Optional[pd.DataFrame]=None, fh: Optional[ForecastingHorizon]=None, coverage: float=0.9, verbose=False) -> Tuple[pd.DataFrame, pd.DataFrame]: Generate predictions using the fitted model.
+    - update(new_y: pd.Series, new_X: Optional[pd.DataFrame]=None, fh: Optional[ForecastingHorizon]=None, coverage: float=0.9, refit: bool=False) -> Tuple[pd.DataFrame, pd.DataFrame]: Update cutoff value to forecast new dates.
+    - get_pred_errors() -> pd.DataFrame: Get the prediction errors.
+
+    Raises:
+    -------
+    - AssertionError: If the provided data is not a DataFrame, or if depvar_str is not a valid column in the data, or if exog_l is not None or an iterable.
+    - AssertionError: If any column in exog_l is not present in the data.
+    - AssertionError: If freq is not a recognized pandas frequency.
     """
 
     # Initializer
     def __init__(self,
                  data: pd.DataFrame,
                  depvar_str: str,
                  fh: int,
@@ -143,15 +142,15 @@
                  forecaster_name: Optional[str] = 'Naive',
                  forecaster: Optional[object] = None,
                  exog_l: Optional[list] = None,
                  freq: Optional[str] = 'D',
                  ) -> None:
         """Initializes the Forecast class with the provided parameters."""
         self.__init_test(data, depvar_str, exog_l, freq)
-        self.y, self.X = self.__clean_data(data=data, 
+        self._y, self._X = self.__clean_data(data=data, 
                                            depvar_str=depvar_str,
                                            exog_l=exog_l,
                                            freq=freq)
         # Forecasting Model Parameters
         self.forecaster_name = forecaster_name
 
         if forecaster is None:
@@ -160,41 +159,41 @@
             assert forecaster_name in CommonForecastingModels.keys(), _err_msg
             self.forecaster = CommonForecastingModels[forecaster_name]
         else:
             self.forecaster = forecaster
 
         # Forecasting parameters
         #1. horizon
-        self.fh = ForecastingHorizon(np.arange(1, fh+1))
+        self._fh = ForecastingHorizon(np.arange(1, fh+1))
         #2. Initial training window
-        self.initial_window = int(len(self.y)*pct_initial_window)
+        self._initial_window = int(len(self._y)*pct_initial_window)
         #3. Step size
-        self.step_length = step_length
+        self._step_length = step_length
 
         #4. Declare the cross validation window
-        self.cv = ExpandingWindowSplitter(initial_window=self.initial_window,
-                                          step_length=self.step_length,
-                                          fh=self.fh)
+        self._cv = ExpandingWindowSplitter(initial_window=self._initial_window,
+                                          step_length=self._step_length,
+                                          fh=self._fh)
 
         # Create the train test sets
-        if self.X is None:
-            self.X_train =  None
-            self.X_test = None
-            self.y_train, self.y_test = temporal_train_test_split(y=self.y, 
-                                                                  train_size=self.initial_window)
+        if self._X is None:
+            self._X_train =  None
+            self._X_test = None
+            self._y_train, self._y_test = temporal_train_test_split(y=self._y, 
+                                                                  train_size=self._initial_window)
         else:
-            self.y_train, self.y_test, self.X_train, self.X_test = temporal_train_test_split(
-            y=self.y, 
-            X=self.X,
-            train_size=self.initial_window)
+            self._y_train, self._y_test, self._X_train, self._X_test = temporal_train_test_split(
+            y=self._y, 
+            X=self._X,
+            train_size=self._initial_window)
 
         self.is_fitted = False
-        self.fitted = None
+        self._fitted = None
         self.is_evaluated = False
-        self.eval = None
+        self._eval = None
 
         # Plots
         self.plot = self.__plot()
 
     def split_procedure_summary(self, verbose: bool=True) -> dict:
         """
         Generate a summary of the cross-validation procedure.
@@ -206,39 +205,28 @@
 
         Returns:
         --------        
             dict
                 A dictionary containing the summary of the cross-validation procedure.
         """
 
-        _n_splits = self.cv.get_n_splits(self.y)
-        cutoffs = [self.y.index[_train[-1]] for (_train, _) in self.cv.split(self.y.index)]
+        _n_splits = self._cv.get_n_splits(self._y)
+        cutoffs = [self._y.index[_train[-1]] for (_train, _) in self._cv.split(self._y.index)]
         _split_proc= {'Number of Folds': _n_splits,
-                      'Initial Window Size': self.cv.initial_window,
-                      'Step Length': self.cv.step_length,
-                      'Forecast Horizon': len(self.cv.fh),
+                      'Initial Window Size': self._cv.initial_window,
+                      'Step Length': self._cv.step_length,
+                      'Forecast Horizon': len(self._cv.fh),
                       'First Cutoff': cutoffs[0],
                       'Last Curoff': cutoffs[-1]
                      }
         if verbose:
             for k, v in _split_proc.items():
                 print(f"{k:<21}: {v}")
         return _split_proc    
 
-    def __plot(self): #-> ForecastPlot
-        """
-        Create an instance of the ForecastPlot class for plotting utility.
-
-        Returns:
-        --------
-            ForecastPlot:
-                An instance of the ForecastPlot class.
-        """
-        return ForecastPlot(self)  
-
     def fit(self, 
             on: str = 'all', 
             fh: Optional[ForecastingHorizon] = None
            ): #-> ForecastFit
         """
         Fit the forecaster and compute insample results.
 
@@ -252,43 +240,43 @@
         Returns:
         --------
             ForecastFit:
                 An instance of the ForecastFit class containing the fitted model and insample performance metrics.
         """
 
         if fh is None:
-            fh =  self.fh
+            fh =  self._fh
 
         if on == 'all':
-            self.forecaster.fit(y=self.y, X=self.X, fh=fh)
+            self.forecaster.fit(y=self._y, X=self._X, fh=fh)
             self.is_fitted = True
 
         elif on=='train':
-            self.forecaster.fit(y=self.y_train, X=self.X_train, fh=fh)
+            self.forecaster.fit(y=self._y_train, X=self._X_train, fh=fh)
             self.is_fitted = False
 
         else: 
             on_values =['all', 'train']
             raise ValueError(f'argument takes 2 possible values {on_values}')
-        self.fitted = ForecastFit(self)   
-        return self.fitted
+        self._fitted = ForecastFit(self)   
+        return self._fitted
 
     def evaluate(self): #-> ForecastEval
         """
         Evaluate the forecaster out-of-sample.
 
         Returns:
         --------
             ForecastEval:
                 An instance of the ForecastEval class containing the out-of-sample evaluation results.
         """
 
-        self.eval = ForecastEval(self)  
+        self._eval = ForecastEval(self)  
         self.is_evaluated = True
-        return self.eval
+        return self._eval
 
     def predict(self, 
                 X: Optional[pd.DataFrame] = None, 
                 fh: Optional[ForecastingHorizon] = None, 
                 coverage: float = 0.9,
                 verbose = False
                ) -> Tuple[pd.DataFrame, pd.DataFrame]:
@@ -312,17 +300,17 @@
         if self.is_fitted==False:
             if verbose:
                 print(f"\n{self.forecaster_name} model not fitted yet, or fitted on a subset only")
                 print("Fitting the model on the entire sample ...")
             self.fit(on='all', fh=fh)
 
         if fh is None:
-            fh =  self.fh
+            fh =  self._fh
         if X is None:
-            X = self.X
+            X = self._X
 
         y_pred = self.forecaster.predict(X=X, fh=fh)
         try:
             y_pred_ints = self.forecaster.predict_interval(X=X, fh=fh, coverage=coverage)
         except Exception as e:
             if verbose:
                 print(f"{self.forecaster_name} does not support prediction intervals")
@@ -363,34 +351,45 @@
             Tuple[pd.DataFrame, pd.DataFrame]:
                 A tuple containing the updated predictions and the updated confidence intervals.
         """
         new_y = new_y.resample(self.freq).last().ffill()
         if new_X is not None:
             new_X = new_X.resample(self.freq).last().ffill()
         self.forecaster.update(y=new_y, X=new_X, update_params=refit)
+        self._y = new_y
+        self._X = new_X
         y_pred, y_pred_ints = self.predict(X=new_X, fh=fh, coverage=coverage)
         return y_pred, y_pred_ints
 
     def get_pred_errors(self):
         """
         Get the prediction errors.
         Returns:
         --------        
             pd.DataFrame:
                 A DataFrame containing the prediction errors.
         """
-        if (self.is_evaluated is False) or (self.eval is None):
-            self.eval = self.evaluate()        
+        if (self.is_evaluated is False) or (self._eval is None):
+            self._eval = self.evaluate()        
         try:
-            pred_errors = self.eval.oos_horizon_df[['cutoff', 'horizon', 'error']]
-        except Exception as e:
+            pred_errors = self._eval._oos_horizon_df[['cutoff', 'horizon', 'error']]
+        except Exception:
             return None
         return pred_errors
         
+    def __plot(self): #-> ForecastPlot
+        """
+        Create an instance of the ForecastPlot class for plotting utility.
 
+        Returns:
+        --------
+            ForecastPlot:
+                An instance of the ForecastPlot class.
+        """
+        return ForecastPlot(self)  
     def __init_test(self,
                     data: pd.DataFrame, 
                     depvar_str: str, 
                     exog_l: Optional[list], 
                     freq: str
                    ) -> None:
         """
@@ -432,14 +431,31 @@
         assert cond1 or cond2, 'exog_l is either None, meaning no X or an iterable object'
         if cond2:
             assert all([c in data.columns for c in exog_l]), 'not all exog variables are in the data'
             self.exog_l = exog_l
         else:
             self.exog_l = exog_l
 
+        # Pandas frequencies
+        pandas_frequency_dict = {
+            "D": "daily",
+            "B": "business days",
+            "W": "weekly (end of week, default on Sunday)",
+            "M": "monthly (end of month)",
+            "Q": "quarterly (end of quarter)",
+            "A": "annual (end of year)",
+            "H": "hourly",
+            "T": "minutely",
+            "S": "secondly",
+            "L": "millisecondly",
+            "U": "microsecondly",
+            "BQ": "business quarterly (business quarter-end)",
+            "BA": "business annual (business year-end)",
+            "BH": "business hourly (business hour)"
+        }
         assert freq in pandas_frequency_dict.keys(), f'Not a pandas recognized frequency. List of pandas frequencies:\n{pandas_frequency_dict}'
         self.freq = freq
 
         return None
 
     def __clean_data(self, 
                      data: pd.DataFrame, 
@@ -448,16 +464,18 @@
                      freq: str
                     ) -> Tuple[pd.Series, pd.DataFrame]:
         """
         Reformat the data taking into account the requested frequency.
         """
 
         _df = data.dropna().resample(freq).last().copy()
+        _df.index.freq = freq
         # Declare and stage the variable to forecast
         y = _df[depvar_str]
+        
 
         # List of Exogenous variables if any
         if exog_l is None:
             X = None
         else:
             assert all([c in _df.columns for c in exog_l]), 'not all columns are not in the data'
             X = _df[exog_l]
@@ -465,32 +483,39 @@
 
 class ForecastPlot:
     """
     Plotting utility class for Forecast.
 
     Parameters:
     -----------    
-        LF : Forecast
-            An instance of the Forecast class
+    - LF (Forecast): An instance of the Forecast class
+
+    Methods:
+    --------
+    - plot_train_test(labels: List[str] = None, xlabel: Optional[str] = None, ylabel: Optional[str] = None, title: str = 'Train-Test sets', ax: Optional[plt.Axes] = None, figsize: Tuple[float, float] = (15, 6)) -> Tuple[plt.Figure, np.array]: Plot the dependent variable separating the train from the test windows.
+    - plot_cv_procedure(ax: Optional[plt.Axes] = None, labels: List[str] = None, ylabel: str = "Window number", xlabel: str = "Time", title: str = "Cross Validation Procedure") -> Tuple[plt.Figure, np.array]: Plot the cross-validation procedure.
+    - plot_prediction(y_pred: pd.Series, y_pred_ints: Optional[pd.DataFrame] = None, interval_label: str = 'CI', labels: List[str] = None, xlabel: Optional[str] = None, ylabel: Optional[str] = None, title: str = 'Prediction', ax: Optional[plt.Axes] = None, figsize: Tuple[float, float] = (15, 6)) -> Tuple[plt.Figure, np.array]: Plot the forecast predictions and the confidence intervals.
+    - plot_prediction_true(y_pred: pd.Series, y_pred_ints: Optional[pd.DataFrame] = None, interval_label: str = 'CI', labels: List[str] = None, xlabel: Optional[str] = None, ylabel: Optional[str] = None, title: str = 'Prediction', ax: Optional[plt.Axes] = None, figsize: Tuple[float, float] = (15, 6)) -> Tuple[plt.Figure, np.array]: Plot the forecast predictions, true values, and the confidence intervals.
     """
 
     def __init__(self, LF: Forecast):
-        self.y_train = LF.y_train
-        self.y_test = LF.y_test
-        self.y = LF.y
-        self.cv = LF.cv
+        self._y_train = LF._y_train
+        self._y_test = LF._y_test
+        self._y = LF._y
+        self._cv = LF._cv
         return None
 
     def plot_train_test(self,
                         labels: List[str] = None,
                         xlabel: Optional[str] = None,
                         ylabel: Optional[str] = None,
                         title: str = 'Train-Test sets',
                         ax: Optional[plt.Axes] = None,
-                        figsize: Tuple[float, float] = (15, 6)) -> None:
+                        figsize: Tuple[float, float] = (15, 6)
+                        ):
         """
         Plot the dependent variable separating the train from the test windows.
 
         Parameters:
         -----------
             labels : List[str], optional
                 Labels for the plot. Default is ["y_train", "y_test"].
@@ -503,33 +528,36 @@
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
 
         Returns:
         --------        
-            None
+            fig : plt.Figure
+                The Figure object containing the plot.
+            axes : np.array
+                An array of Axes objects containing the plot.
         """
         if labels is None:
             labels = ["y_train", "y_test"]
-        return plot_series(self.y_train, self.y_test, 
+        return plot_series(self._y_train, self._y_test, 
                            labels =labels, 
                            ax = ax, 
                            xlabel = xlabel,
                            ylabel = ylabel,
                            title = title,
                            figsize = figsize)
 
     def plot_cv_procedure(self,
                           ax: Optional[plt.Axes] = None,
                           labels: List[str] = None,
                           ylabel: str = "Window number",
                           xlabel: str = "Time",
                           title: str = "Cross Validation Procedure"
-                          ) -> None:
+                          ):
         """
         Plot the cross-validation procedure.
 
         Parameters:
         -----------        
             ax : plt.Axes, optional
                 The Axes object for the plot.
@@ -540,22 +568,25 @@
             xlabel : str, optional
                 Label for the x-axis. Default is "Time".
             title : str, optional
                 The title of the plot. Default is "Cross Validation Procedure".
 
         Returns:
         --------        
-            None
+            fig : plt.Figure
+                The Figure object containing the plot.
+            axes : np.array
+                An array of Axes objects containing the plot.
         """
 
         _train_windows, _test_windows = self._get_windows()
         if labels is None:
             labels = ["Window", "Forecasting horizon"]
             
-        return plot_windows(self.y, 
+        return plot_windows(self._y, 
                             _train_windows,
                             _test_windows,
                             ax = ax,
                             labels = labels,
                             xlabel = xlabel, 
                             ylabel = ylabel,
                             title = title)
@@ -592,18 +623,21 @@
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
 
         Returns:
         -------        
-            None
+            fig : plt.Figure
+                The Figure object containing the plot.
+            axes : np.array
+                An array of Axes objects containing the plot.
         """
 
-        y = self.y
+        y = self._y
         y_train = y.loc[y.index<y_pred.index[0]]
         zoom_y_train = y_train.iloc[-3*len(y_pred):]	
         if labels is None:
             labels = ["y_train", "y_pred"]
         return plot_series(zoom_y_train, y_pred,
                            labels= labels,
                            pred_interval=y_pred_ints,	
@@ -647,24 +681,27 @@
             ax : plt.Axes, optional
                 The Axes object for the plot.
             figsize : Tuple[float, float], optional
                 The figure size. Default is (15, 6).
 
         Returns:
         --------        
-            None
+            fig : plt.Figure
+                The Figure object containing the plot.
+            axes : np.array
+                An array of Axes objects containing the plot.
         """
 
-        y = self.y
+        y = self._y
         y_train = y.loc[y.index<y_pred.index[0]]
         zoom_y_train = y_train.iloc[-5*len(y_pred):]
         true_pred_idx = np.intersect1d(y.index, y_pred.index)
         err_msg = 'No overlap between true values and predicted values.\nIf you want to plot prediction alone use the function plot_prediction'
         assert len(true_pred_idx)>0, err_msg
-        y_true = self.y[true_pred_idx]
+        y_true = self._y[true_pred_idx]
         if labels is None:
             labels = ["y_train", "y_true", "y_pred"]
 
         return plot_series(zoom_y_train, y_true, y_pred,
                            pred_interval=y_pred_ints,
                            interval_label =interval_label,
                            labels=labels, 
@@ -681,16 +718,16 @@
         Returns:
         --------
             tuple:
                 A tuple containing two lists: train_windows and test_windows.
         """
         _train_windows = []
         _test_windows = []
-        _y_index = self.y.index 
-        for _train, _test in self.cv.split(_y_index):
+        _y_index = self._y.index 
+        for _train, _test in self._cv.split(_y_index):
             _train_windows.append(_train)
             _test_windows.append(_test)
         return _train_windows, _test_windows 
 
 ##############################################################################
 # Model Fit and Insample Performance
 ##############################################################################
@@ -707,31 +744,49 @@
     except Exception as e:
         if verbose:
             print(f"Error occured in {intrain.index[-1]}: {e}")
         in_pred = pd.DataFrame()
     return in_pred
 class ForecastFit:
     """
-    Class for fitting the forecast model and computing insample performance metrics.
+    Class for fitting the forecaster and computing insample predictions.
 
     Parameters:
     -----------    
-        Forecast : Forecast
-            An instance of the Forecast class.
+    - Forecast (Forecast): An instance of the Forecast class.
+
+    Attributes:
+    -----------
+    - forecaster (object): The forecasting model object.
+    - forecaster_name (str): The name of the forecasting model.
+    - is_fitted (bool): A flag indicating if the model is fitted.
+    - _y_train (pd.Series): The training set of the dependent variable.
+    - _y (pd.Series): The dependent variable for forecasting.
+    - _X (pd.DataFrame): The exogenous variables for forecasting.
+    - _fh (ForecastingHorizon): The forecast horizon.
+    - _cv (ExpandingWindowSplitter): The cross-validation window.
+    - plot (ForecastFitPlot): An instance of the ForecastFitPlot class for plotting utility.
+    - insample_result_df (pd.DataFrame): A DataFrame containing the insample predictions.
+    - insample_perf_summary (dict): A dictionary containing the computed insample performance metrics.
+
+    Methods:
+    --------
+    - insample_predictions(random_sample: bool=False, nsample: int=100, verbose: bool=False) -> pd.DataFrame: Compute the insample predictions for the fitted model.
+    - insample_perf() -> dict: Compute insample performance metrics (RMSE and MAPE) for the fitted model.
     """
 
     def __init__(self, LF: Forecast):
         self.forecaster = LF.forecaster
         self.forecaster_name = LF.forecaster_name
         self.is_fitted = LF.is_fitted
-        self.y_train = LF.y_train
-        self.y = LF.y
-        self.X = LF.X
-        self.fh = LF.fh
-        self.cv = LF.cv
+        self._y_train = LF._y_train
+        self._y = LF._y
+        self._X = LF._X
+        self._fh = LF._fh
+        self._cv = LF._cv
         self.plot = self.__plot()
 
         self.insample_result_df = None
         self.insample_perf_summary = None
 
     def insample_predictions(self, random_sample=False, nsample: int = 100, verbose=False) -> pd.DataFrame:
         """
@@ -745,31 +800,31 @@
         Returns:
         --------        
             pd.DataFrame
                 A DataFrame containing the insample predictions.
         """
 
         if self.is_fitted:
-            _y = self.y
+            _y = self._y
         else:
-            _y = self.y_train
+            _y = self._y_train
 
-        insample_eval_window = len(_y) - len(self.fh)
+        insample_eval_window = len(_y) - len(self._fh)
         if random_sample:            
             nsample = max(insample_eval_window, nsample)
             # Randomly selecting cutoff points
             _cutoffs = np.random.choice(insample_eval_window, size=nsample, replace=False)
-            cv_in = CutoffSplitter(cutoffs=_cutoffs, window_length=1, fh=self.fh)
+            cv_in = CutoffSplitter(cutoffs=_cutoffs, window_length=1, fh=self._fh)
         else:
             _cutoffs = np.arange(insample_eval_window)
-            cv_in = ExpandingWindowSplitter(initial_window=1, step_length=1, fh=self.fh)
+            cv_in = ExpandingWindowSplitter(initial_window=1, step_length=1, fh=self._fh)
         if verbose:
             print(f"\nComputing {self.forecaster_name} forecaster historic predictions....")        
 
-        params = [(self.forecaster, self.X, intrain, intest, verbose) for intrain, intest in cv_in.split_series(_y)]                
+        params = [(self.forecaster, self._X, intrain, intest, verbose) for intrain, intest in cv_in.split_series(_y)]                
         with Pool() as pool:
             insample_result = list(tqdm(pool.imap(compute_predictions, params), total=len(params)))
 
         insample_result_df = pd.concat(insample_result)
         if insample_result_df.empty:
             print(f"No insample predictions computed {self.forecaster_name}")
         if verbose:
@@ -802,20 +857,23 @@
 
 class ForecastFitPlot:
     """
     Plotting utility class for ForecastFit.
 
     Parameters:
     -----------    
-        LFF : ForecastFit
-            An instance of the ForecastFit class.
+    - LFF (ForecastFit): An instance of the ForecastFit class.
+
+    Methods:
+    --------
+    - plot_insample_performance(metric: str = 'RMSE', title: str = 'Insample Performance') -> Tuple[plt.Figure, np.array]: Plot the insample performance metrics.
     """
 
     def __init__(self, LFF: ForecastFit):
-        self.LFF = LFF
+        self._LFF = LFF
 
     def plot_insample_performance(self,
                                   metric: str = 'RMSE',
                                   title: str = 'Insample Performance'):
         """
         Plot the insample performance metrics.
 
@@ -832,15 +890,15 @@
                 The Figure object containing the plot.
             axes : np.array
                 An array of Axes objects containing the plot.
         """
 
         assert metric in ['RMSE', 'MAPE'], f'{metric} not in summary performance'
         if 'insample_perf_summary' not in self.__dict__.keys():
-            insample_perf_summary = self.LFF.insample_perf()
+            insample_perf_summary = self._LFF.insample_perf()
 
         f, axes = plt.subplots(1,2,figsize=(15,5))
         for i, (_grouper, _df) in enumerate(insample_perf_summary.items()):
             _df[metric].plot(ax= axes[i], style = '-o', title = f'{metric} By {_grouper}')
             axes[i].set_xlabel('')
 
         plt.suptitle(title)
@@ -852,63 +910,85 @@
 ##############################################################################
 class ForecastEval:
     """
     Class for evaluating the forecaster out-of-sample.
 
     Parameters:
     -----------    
-        Forecast : Forecast
-            An instance of the Forecast class.
+    - Forecast (Forecast): An instance of the Forecast class.
+
+    Attributes:
+    -----------
+    - forecaster (object): The forecasting model object.
+    - forecaster_name (str): The name of the forecasting model.
+    - oos_eval (pd.DataFrame): A DataFrame containing the out-of-sample evaluation results.
+    - plot (ForecastEvalPlot): An instance of the ForecastEvalPlot class for plotting utility.
+    - _y (pd.Series): The dependent variable for forecasting.
+    - _X (pd.DataFrame): The exogenous variables for forecasting.
+    - _cv (ExpandingWindowSplitter): The cross-validation window.
+    - _scoring_metrics (list): A list of scoring metrics.    
+    - _oos_horizon_df (pd.DataFrame): A DataFrame containing the out-of-sample predictions and errors per horizon.
+    - _oos_horizon_perf (pd.DataFrame): A DataFrame containing the summary performance metrics per horizon.
+    - _oos_cutoff_perf (pd.DataFrame): A DataFrame containing the summary performance metrics per cutoff.
+    
+
+    Methods:
+    --------
+    - summary_results() -> pd.DataFrame: Generate a summary of out-of-sample forecast results.
+    - summary_cutoff() -> pd.DataFrame: Generate a summary of out-of-sample performance per cutoff.
+    - summary_horizon() -> pd.DataFrame: Generate a summary of out-of-sample performance per horizon.
     """
 
     def __init__(self, LF: Forecast):
         
         self.forecaster = LF.forecaster
         self.forecaster_name = LF.forecaster_name
-        self.y = LF.y
-        self.X = LF.X
-        self.cv = LF.cv
+        self._y = LF._y
+        self._X = LF._X
+        self._cv = LF._cv
 
-        self.scoring_metrics = [MeanSquaredError(square_root=True),
+        self._scoring_metrics = [MeanSquaredError(square_root=True),
                                 MeanAbsoluteError(),
                                 MeanAbsolutePercentageError(), 
                                 MedianAbsoluteError(),
                                 ]
 
         _rename_metrics = {
             'test_MeanSquaredError':'RMSE', 
             'test_MeanAbsoluteError':'MAE',
             'test_MeanAbsolutePercentageError':'MAPE',
             'test_MedianAbsoluteError':'MedianAE',
         }
         print(f"\nStart {self.forecaster_name} forecaster evalution....")
         st = time.time()
-        self.oos_eval = evaluate(forecaster=self.forecaster, 
-                            y=self.y,
-                            X = self.X,
-                            cv=self.cv,
-                            strategy="refit",
-                            return_data=True,
-                            scoring = self.scoring_metrics,
-                            backend ='loky',
-                           )
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            self.oos_eval = evaluate(forecaster=self.forecaster, 
+                                y=self._y,
+                                X = self._X,
+                                cv=self._cv,
+                                strategy="refit",
+                                return_data=True,
+                                scoring = self._scoring_metrics,
+                                backend ='loky',
+                            )
         self.oos_eval = self.oos_eval.set_index('cutoff').sort_index()
         self.oos_eval = self.oos_eval.rename(columns = _rename_metrics)
         et = time.time()
         elapsed_time = et - st
         print(f"Evaluation completed in: {np.around(elapsed_time / 60,3)} minutes")
 
         convert_horizon = self.oos_eval.apply(self.__eval_horizon, axis=1)
         
-        self.oos_horizon_df = pd.concat(convert_horizon.values)
-        self.oos_horizon_perf = summary_perf(self.oos_horizon_df, 
+        self._oos_horizon_df = pd.concat(convert_horizon.values)
+        self._oos_horizon_perf = summary_perf(self._oos_horizon_df, 
                                              grouper='horizon', 
                                              y_true_col = 'y_test', 
                                              y_pred_col = 'y_pred')
-        self.oos_cutoff_perf = summary_perf(self.oos_horizon_df, 
+        self._oos_cutoff_perf = summary_perf(self._oos_horizon_df, 
                                              grouper='cutoff', 
                                              y_true_col = 'y_test', 
                                              y_pred_col = 'y_pred')
 
         self.plot = self.__plot()
         return None
 
@@ -927,39 +1007,39 @@
          'Avg Fit time (s)': self.oos_eval.fit_time.mean(),
          'Avg_pred_time (s)': self.oos_eval.pred_time.mean(),
          'Smallest training window': self.oos_eval.len_train_window.min(),
          'Largest training window':self.oos_eval.len_train_window.max(),
          'First cutoff': self.oos_eval.index[0],
          'Last cutoff': self.oos_eval.index[-1],
         }
-        for _s in self.oos_cutoff_perf.columns:
-            _summary[f'Avg {_s}'] = self.oos_cutoff_perf[_s].mean()
+        for _s in self._oos_cutoff_perf.columns:
+            _summary[f'Avg {_s}'] = self._oos_cutoff_perf[_s].mean()
         return pd.Series(_summary).to_frame().T
 
     def summary_cutoff(self) -> pd.DataFrame:
         """
         Generate a summary of out-of-sample performance per cutoff.
 
         Returns:
         --------        
             pd.DataFrame
                 A DataFrame containing summary performance metrics (RMSE and MAPE) for each horizon.
         """        
-        return self.oos_cutoff_perf
+        return self._oos_cutoff_perf
 
     def summary_horizon(self) -> pd.DataFrame:
         """
         Generate a summary of out-of-sample performance per horizon.
 
         Returns:
         --------        
             pd.DataFrame
                 A DataFrame containing summary performance metrics (RMSE and MAPE) for each horizon.
         """        
-        return self.oos_horizon_perf
+        return self._oos_horizon_perf
 
     def __eval_horizon(self, x):
         _fct = pd.concat([x['y_test'], x['y_pred']], keys=['y_test', 'y_pred'], axis=1)
         _fct['error'] = _fct['y_test'] - _fct['y_pred']
         _fct['error_pct'] = _fct['error'].abs()/ _fct['y_test']
         _fct['horizon'] = np.arange(1, len(_fct)+1)    
         _fct['cutoff'] = x.name
@@ -970,21 +1050,29 @@
 
 class ForecastEvalPlot:
     """
     Plotting utility class for ForecastEval.
 
     Parameters:
     -----------    
-        LFE : ForecastEval
-            An instance of the ForecastEval class.
+    LFE (ForecastEval): An instance of the ForecastEval class.
+
+    Attributes:
+    -----------
+    _oos_horizon_perf (pd.DataFrame): A DataFrame containing the summary performance metrics per horizon.
+    _oos_cutoff_perf (pd.DataFrame): A DataFrame containing the summary performance metrics per cutoff.
+
+    Methods:
+    --------
+    plot_oos_score(score: str = 'RMSE', view: str = 'horizon', xlabel: str = None, ylabel: str = None, title: str = 'Out of Sample Performance', ax: Optional[plt.Axes] = None, figsize: Tuple[float, float] = (15, 6)) -> Tuple[plt.Figure, np.array]: Plot out-of-sample performance metric historically.
     """
 
     def __init__(self, LFE: ForecastEval):
-        self.oos_horizon_perf = LFE.oos_horizon_perf
-        self.oos_cutoff_perf = LFE.oos_cutoff_perf
+        self._oos_horizon_perf = LFE._oos_horizon_perf
+        self._oos_cutoff_perf = LFE._oos_cutoff_perf
         return None
 
     def plot_oos_score(self,
                        score: str = 'RMSE',
                        view: str = 'horizon', 
                        xlabel: str = None,
                        ylabel: str = None,
@@ -1019,19 +1107,19 @@
             fig : plt.Figure
                 The Figure object containing the plot.
             axes : np.array
                 An array of Axes objects containing the plot.
 
         """
         if view == 'horizon':
-            assert score in self.oos_horizon_perf.columns, 'score not computed'
-            to_plot = self.oos_horizon_perf[score]
+            assert score in self._oos_horizon_perf.columns, 'score not computed'
+            to_plot = self._oos_horizon_perf[score]
         elif view == 'cutoff':
-            assert score in self.oos_cutoff_perf.columns, 'score not computed'
-            to_plot = self.oos_cutoff_perf[score]
+            assert score in self._oos_cutoff_perf.columns, 'score not computed'
+            to_plot = self._oos_cutoff_perf[score]
         else:
             raise ValueError('view should be either horizon or cutoff')
 
         if ax is None:
             f, ax = plt.subplots(1,1,figsize=figsize)
 
         ylabel = score if ylabel is None else ylabel
```

### Comparing `forecast_combine-0.0.2/forecast_combine/model_select.py` & `forecast_combine-0.0.3/forecast_combine/model_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """ Combination of timeseries Forecasts"""
 __description__ = "Time Series Forecast Combination"
 __author__ = "Amine Raboun - amineraboun@github.io"
 
-import logging
-logging.getLogger().setLevel(logging.ERROR)
 import warnings
 warnings.filterwarnings("ignore")
-warnings.simplefilter("ignore", category=FutureWarning)
-warnings.simplefilter("ignore", category=DeprecationWarning)
 
 ##############################################################################
 # Import Libraries & default configuration 
 ##############################################################################
 import pandas as pd
 import numpy as np
 from typing import Union, Optional, Tuple, List, Dict, Any
@@ -39,58 +35,109 @@
 
 class ForecastModelSelect:
     """
     Class for model selection and comparison based on out-of-sample performance.
     Evaluate how to best combine the different models based on their oos performance.
 
     The class can be initialized in 2 ways. 
-        Method 1: Requires a list of Forecast objects. It is the preferable instantiation if the models have already been evaluated out of sample.
+    - **Method 1**: Requires a dictionary of forecasting models. A dictionary where the keys are names of forecasts and the values are sktime recognized forecast_models.
+    All the arguments taken by Forecast object must be passed to the initialization of the ForecastModelSelect object.
+    - **Method 2**: Requires a dictionary of trained models. The training and evalutiaon of the models are assumed to be done.
 
-        Method 2: Requires all the arguments taken by Forecast plus a dictionary where the keys are names of forecasts and the values are the forecast_models.
+    There is the possibility to combine the two methods by providing both dictionaries. 
+    In this case, the trained models will be used for evaluation and the non-trained models will be trained and evaluated.
 
     Parameters:
     -----------    
-        forecasters_d : dict, optional
-            A dictionary containing various forecasting models for comparison. 
-            Default is None and assess the most common forecasting models.
-                Naive: NaiveForecaster - Keep the latest value
-                AutoARIMA: StatsForecastAutoARIMA - Auto ARIMA model
-                AutoETS: StatsForecastAutoETS - Auto ETS model
-                AutoTheta: StatsForecastAutoTheta - Auto Theta model
-                TBATS: StatsForecastAutoTBATS - TBATS model
-                LOESS: StatsForecastMSTL - LOESS model
-                Prophet: Prophet - Prophet model
-        trained_forecasters_d : dict, optional
-            A dictionary containing trained Forecast objects. Default is None.
-        mode : str, optional
-            The aggregation mode. Default is 'nbest_average_horizon'.
-        score : str, optional
-            The performance score. Default is 'RMSE'.
-        nbest : int, optional
-            Number of best models to aggregate. Default is 2.
-        kwargs
-            Additional keyword arguments to be passed to the Forecast initialization.
-
+    - forecasters_d (dict): A dictionary containing various forecasting models for comparison. 
+    Default is None and assess the most common forecasting models.
+        - **Naive:** NaiveForecaster - Keep the latest value
+        - **SeasonalNaive:** NaiveForecaster - Keep the value of the same season
+        - **AutoARIMA:** StatsForecastAutoARIMA - Auto ARIMA model
+        - **AutoETS:** StatsForecastAutoETS - Auto ETS model
+        - **AutoCES:** StatsForecastAutoCES - Auto CES model
+        - **AutoTheta:** StatsForecastAutoTheta - Auto Theta model
+        - **AutoTBATS:** StatsForecastAutoTBATS - Auto TBATS model
+        - **Prophet:** Prophet - Prophet model
+    - trained_forecasters_d (dict): A dictionary containing trained Forecast objects. Default is None.
+    - model_exog_d (dict): A dictionary containing exogenous variables for each model. Default is None.
+    - mode (str): The aggregation mode. Default is 'nbest_average_horizon'. Available values are:
+        - best: The prediction is based on the best model.
+        - best_horizon: The prediction is based on the best model for each horizon.
+        - average: The average of the prediction of all models.
+        - inverse_score: The weighted average prediction, where weights are inversely proportional to the model performance score.
+        - nbest_average: Average of the n best models. The n is given by the parameter nbest.
+        - nbest_average_horizon: Average of the n best models for each horizon. The n is given by the parameter nbest.
+        - model: Returns the prediction of a specific model. The model name must be provided in the model_name parameter.
+    - score (str): The performance score. Default is 'RMSE'. Available values are:
+        - RMSE: Root Mean Squared Error.
+        - MAE: Mean Absolute Error.
+        - MAPE: Mean Absolute Percentage Error.
+        - MedianAE: Median Absolute Error.
+        - R2: R-squared.       
+    - nbest (int): Number of best models to aggregate. Default is 2.    
+    - data (pd.DataFrame): A DataFrame containing the input data for forecasting.
+    - depvar_str (str): The column name representing the dependent variable for forecasting.
+    - fh (int): The forecast horizon, i.e., the number of periods ahead to forecast.
+    - pct_initial_window (float): The percentage of data used as the initial training window.
+    - step_length (int): The step size for expanding window cross-validation.    
+    - exog_l (list, optional): List of exogenous variables for forecasting. Default is None.
+    - freq (str, optional): The frequency of the time series data. Default is 'B' (business days).
+
+    Attributes:
+    -----------
+    - LF_d (dict): A dictionary containing the Forecast objects.
+    - summary_horizon (pd.DataFrame): Summary of out-of-sample performance per horizon and per model.
+    - summary_results (pd.DataFrame): Summary of out-of-sample performance per model.
+    - summary_cutoff (pd.DataFrame): Out-of-sample performance based on cutoffs.
+    - model_rank_perhorizon (pd.DataFrame): Rank of models per horizon based on performance.
+    - _mode (str): The aggregation mode.
+    - _score (str): The performance score.
+    - _nbest (int): Number of best models to aggregate.
+    - _eval_models (list): A list of evaluated models.    
+    - _best_x_overall (dict): The best models based on overall performance.
+    - _avg_oos_horizon (dict): The average out-of-sample performance per horizon.
+
+    Methods:
+    --------
+    - split_procedure_summary(): Print the summary of the split procedure for each model.
+    - add_forecaster(forecaster_name, lf): Add a Forecast Object to the list of models to evaluate.
+    - fit(on, fh, force, verbose): Fit the forecasting models for all the underlying Forecast objects.
+    - evaluate(force): Evaluate the underlying Forecast models out of sample.
+    - select_best(score, reestimate): Select the best model based on horizon and overall performance.
+    - summary_per_cutoff(score): Calculate and return the out-of-sample performance based on cutoffs.
+    - predict(X, fh, coverage, mode, score, model_name, ret_underlying): Make forecasts using the specified aggregation mode.
+    - update(new_y, new_X, refit, reevaluate, fh, coverage, mode, score, model_name, ret_underlying): Update the prediction for all the models and aggregate them based on the specific mode.
+    - save(path): Save the model to a file.
+    - get_pred_errors(mode, score, model_name): Get the prediction errors.
+    - plot_model_compare(score, view, model_subset, xlabel, ylabel, title, ax, figsize): Plot a comparison of models based on their out-of-sample performance.
+    - plot_prediction(y_pred, models_preds, y_pred_interval, interval_label, aggregation_label, xlabel, ylabel, title, ax): Plot the prediction.
+    
     Raises:
     -------    
-        AssertionError
-            If the mode, score, or nbest values are not recognized or do not meet the requirements.
-            If both LF_list and forecasters_d are None.
+    - AssertionError: If the trained models are not instances of Forecast.
+    - AssertionError: If there is an overlap between the trained and non-trained dictionaries.
+    - AssertionError: If the mode function is not implemented.
+    - AssertionError: If the performance score is not implemented.
+    - AssertionError: If the number of best models is not an integer.
+    - AssertionError: If the exogenous variables are missing for a model.
+    - ValueError: If the view mode is not 'horizon' or 'cutoff'.
+    - ValueError: If the mode is not 'best', 'best_horizon', 'average', 'inverse_score', 'nbest_average', 'nbest_average_horizon', or 'model'.
     """
 
     def __init__(self, 
                  forecasters_d: Optional[Dict] = None,
                  trained_forecasters_d: Optional[Dict] = None,
                  model_exog_d: Optional[Dict] = None,
                  mode: str = 'best_horizon',
                  score: str = 'RMSE',
                  nbest: int = None,
                  **kwargs: Any
                 ) -> None:
-
+        """Initialize the ForecastModelSelect object."""
         lf_d = {}
         if (trained_forecasters_d is not None):
             # Trained Models must be istance of Forecast object
             assert len(set(forecasters_d.keys()).intersection(set(trained_forecasters_d.keys()))) == 0, 'There is an overlap between the two trained and non trainded dictionaries' 
             if (forecasters_d is not None):
                 # There must be no overlap between the two dictionaries
                 assert all([isinstance(_lf, Forecast) for _lf in trained_forecasters_d.values()]), 'Trained models must be instances of Forecast object'
@@ -121,33 +168,33 @@
                            
         self.LF_d = lf_d
 
         assert isinstance(mode, str), 'mode must be a sting'
         recog_modes = ['best', 'best_horizon', 'average', 'inverse_score', 
                            'nbest_average', 'nbest_average_horizon']
         assert mode in recog_modes, f'mode function not implemented!. Recognized modes are {recog_modes}'
-        self.mode = mode
+        self._mode = mode
 
         recog_scores = ['RMSE', 'MAE', 'MAPE', 'R2', 'MedianAE']
         assert score in recog_scores, f'performance score not implemented!. Recognized scores are {recog_scores}'		
-        self.score = score
+        self._score = score
 
         if nbest is None:
             nbest = 2
         else:
             assert isinstance(nbest, int), 'n best must be an integer'		
-        self.nbest = min(nbest, len(self.LF_d))	
+        self._nbest = min(nbest, len(self.LF_d))	
 
-        self.eval_models = None
+        self._eval_models = None
         self.summary_horizon = None
         self.summary_results = None
-        self.best_x_overall = None
         self.model_rank_perhorizon = None
-        self.avg_oos_horizon = None
-        self.avg_oos_hist = None
+        self._best_x_overall = None
+        self._avg_oos_horizon = None
+        self.summary_cutoff = None
         return None
 
     def split_procedure_summary(self):
         """
         Print the summary of the split procedure for each model.
 
         Returns:
@@ -235,25 +282,25 @@
                     print(f'Error evaluating {_fname}: {e}')
                     print(f'\nmodel {_fname} cannot be evaluated. It will be removed from the list of models')
                     _todrop_evals.append(_fname)
                     continue                
         if len(_todrop_evals)>0:
             for _fname in _todrop_evals:
                 self.LF_d.pop(_fname)
-        self.eval_models = _model_evals
+        self._eval_models = _model_evals
 
         # Step 2: Get the OOS Summary of Performance 
         #per horizon and per model
         _sum_h = {}; _sum_T = {}
-        for _lf_eval in self.eval_models:            
+        for _lf_eval in self._eval_models:            
             _sum_T[_lf_eval.forecaster_name] = _lf_eval.summary_results().squeeze()
             _sum_h[_lf_eval.forecaster_name] = _lf_eval.summary_horizon()
 
-        self.summary_horizon = pd.concat(_sum_h.values(), axis=1, keys = _sum_h.keys())
         self.summary_results = pd.concat(_sum_T.values(), axis=1, keys = _sum_T.keys())
+        self.summary_horizon = pd.concat(_sum_h.values(), axis=1, keys = _sum_h.keys())        
         return self.summary_horizon, self.summary_results
 
     def select_best(self,
                     score: Optional[str] = None,
                     reestimate = False,
                    ) -> pd.DataFrame:
         """
@@ -268,27 +315,27 @@
 
         Returns:
         --------        
             pd.DataFrame
                 model_rank_perhorizon. Rank of models per horizon based on performance.
         """
         if score is None:
-            score = self.score
+            score = self._score
 
-        if (self.model_rank_perhorizon is None) or (self.avg_oos_horizon is None) or reestimate:
+        if (self.model_rank_perhorizon is None) or (self._avg_oos_horizon is None) or reestimate:
 
             # if models are not evaluated yet, run evaluate
-            cond1 = self.eval_models is None
+            cond1 = self._eval_models is None
             cond2 = self.summary_horizon is None
             if cond1 or cond2:	
                 print('\nRun evaluate ...')
                 self.evaluate()
 
             nevals = len(self.LF_d)
-            nbest = self.nbest
+            nbest = self._nbest
             if nbest > nevals:
                 print(f'\nnbest ={nbest} is higher than the number of models evaluated {nevals}')
                 print('All models will be considered. The average best models will be equal to the simple average')
                 nbest = max(nbest, nevals)
 
             best_x_overall = {}
             model_rank_perhorizon = {}
@@ -322,21 +369,21 @@
 
                 # Compute the rank of the models per horizon
                 _rank_perhorizon = r.apply(lambda x: x.nsmallest(nevals).index.tolist(), axis=0)\
                     .reset_index(drop=True).rename(index={i: f'Best_{i+1}' for i in range(nevals)})
                 model_rank_perhorizon[_s] = _rank_perhorizon
                 best_x_overall[_s] = _s_best_x_overall
             
-            self.best_x_overall = best_x_overall
+            self._best_x_overall = best_x_overall
             self.model_rank_perhorizon = model_rank_perhorizon
-            self.avg_oos_horizon = avg_oos_horizon
+            self._avg_oos_horizon = avg_oos_horizon
 
-        return self.model_rank_perhorizon[score], self.avg_oos_horizon[score]
+        return self.model_rank_perhorizon[score], self._avg_oos_horizon[score]
 
-    def oos_per_cutoff(self,
+    def summary_per_cutoff(self,
                        score: Optional[str] = None
                       ) -> pd.DataFrame:
         """
         Calculate and return the out-of-sample performance based on cutoffs.
 
         Parameters:
         -----------        
@@ -347,49 +394,49 @@
 
         Returns:
         --------        
             pd.DataFrame
                 A DataFrame containing the out-of-sample performance per horizon and per model based on the specified score and nbest values.
         """    
         if score is None:
-            score = self.score
+            score = self._score
         
-        if self.avg_oos_hist is None:
-            nbest = self.nbest
+        if self.summary_cutoff is None:
+            nbest = self._nbest
             nevals = len(self.LF_d)
             if nbest > nevals:
                 print(f'\nnbest ={nbest} is higher than the number of models evaluated {nevals}')
                 print(f'The average performance of best models will be computed on {nevals} models instead')
                 nbest = max(nbest, nevals)
 
-            if self.eval_models is None:
+            if self._eval_models is None:
                 print('Run evaluate ...')
                 self.evaluate()
 
             avg_oos_hist = {}
             _perf_metrics = list(self.summary_horizon.columns.levels[1])
             for _s in _perf_metrics:
-                _oos = {_lf_eval.forecaster_name: _lf_eval.oos_cutoff_perf[_s] for _lf_eval in self.eval_models}
+                _oos = {_lf_eval.forecaster_name: _lf_eval._oos_cutoff_perf[_s] for _lf_eval in self._eval_models}
                 _oos = pd.concat(_oos.values(),  axis=1, keys= _oos.keys())
 
                 best_mod = _oos.mean().idxmin()
                 nbest_mods = list(_oos.mean().nsmallest(nbest).index)
                 _aggs = pd.concat([_oos[best_mod], _oos[nbest_mods].mean(axis=1), _oos.mean(axis=1)], axis = 1,
                                   keys = ['Best Model (over all)', f'Best {nbest} Models (over all)','Model Avg (all models)'])
                 avg_oos_hist[_s] = pd.concat([_oos, _aggs], axis=1)
-            self.avg_oos_hist = avg_oos_hist
+            self.summary_cutoff = avg_oos_hist
         
         return avg_oos_hist[score]
 
     def __stage_X(self,
                   LF:Forecast,
                   X: pd.DataFrame
                   ) -> None:
-        if LF.X is not None:
-            _lf_exogs = LF.X.columns
+        if LF._X is not None:
+            _lf_exogs = LF._X.columns
             assert all([_ex in X.columns for _ex in _lf_exogs]), f'Some exogenous variables are missing for model {LF.forecaster_name}'
             _lf_X = X[_lf_exogs]
         else:
             _lf_X = None
         return _lf_X
         
     def predict(self,
@@ -433,15 +480,15 @@
 
         Returns:
         --------        
             tuple
                 A tuple containing the aggregated prediction and prediction intervals.
         """
         if mode is None:
-            mode = self.mode
+            mode = self._mode
         if mode == 'model':
             assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
             _lf_X = self.__stage_X(self.LF_d[model_name], X)
             return self.LF_d[model_name].predict(X=_lf_X, fh=fh, coverage=coverage)
         else:
             preds = {}; pred_ints = {}
             for _fname, _lf in self.LF_d.items():
@@ -505,15 +552,15 @@
 
         Returns:
         -------
             tuple
                 A tuple containing the aggregated prediction and prediction intervals.
         """
         if mode is None:
-            mode = self.mode
+            mode = self._mode
 
         if mode == 'model':
             assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
             _lf_X = self.__stage_X(self.LF_d[model_name], new_X)
             return self.LF_d[model_name].update(new_y=new_y, new_X=_lf_X, fh=fh, coverage=coverage, refit=refit)
         else:
             if reevaluate == False:            
@@ -572,36 +619,36 @@
                         score: Optional[str] = None,
                         model_name = None, 
                         ):
         """
         Get the prediction errors.
         """
         if mode is None:
-            mode = self.mode
+            mode = self._mode
         if mode == 'model':
             assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
             return self.LF_d[model_name].get_pred_errors()
         else:
             if score is None:
-                score = self.score
+                score = self._score
             
             # Using ProcessPoolExecutor to execute computation-heavy tasks in parallel
             with ProcessPoolExecutor() as executor:
                 results = executor.map(fetch_errors, self.LF_d.items())
             errors = {fname: err for fname, err in results}
             for _fname, _lf in self.LF_d.items():
-                _lf.fitted.insample_result_df = errors[_fname]
+                _lf._fitted.insample_result_df = errors[_fname]
 
             # Convert results to dictionary            
             errors_df = pd.concat(errors.values(), keys = errors.keys(), axis=0).reset_index()
             errors_df = errors_df.rename(columns = {'level_0': 'forecaster'})
 
 
             if mode =='best':
-                return errors[self.best_x_overall[score][0]].reset_index(drop=True)
+                return errors[self._best_x_overall[score][0]].reset_index(drop=True)
             
             elif mode =='best_horizon':
                 if self.model_rank_perhorizon is None:
                     self.select_best()
                 best_horizon = self.model_rank_perhorizon[score].loc['Best_1'].to_dict()
                 error_horizon_l = [errors[best_mod_h].loc[errors[best_mod_h]['horizon']==h] for h, best_mod_h in best_horizon.items()]
                 return pd.concat(error_horizon_l, axis=0).reset_index(drop=True)
@@ -615,22 +662,22 @@
                 _score = self.summary_results.loc[f'Avg {score}']
                 _score = _score/_score.sum()
                 errors_df['_score'] = errors_df['forecaster'].map(_score.to_dict())
                 errors_df['weighted_error'] = errors_df['_score']*errors_df['error']
                 return errors_df.groupby(['cutoff', 'horizon']).weighted_error.sum().reset_index()
             
             elif mode =='nbest_average':
-                if self.best_x_overall is None:
+                if self._best_x_overall is None:
                     self.select_best()
-                return errors_df.loc[errors_df.forecaster.isin(self.best_x_overall[score])].groupby(['cutoff', 'horizon']).error.mean().reset_index()
+                return errors_df.loc[errors_df.forecaster.isin(self._best_x_overall[score])].groupby(['cutoff', 'horizon']).error.mean().reset_index()
             
             elif mode =='nbest_average_horizon':
                 if self.model_rank_perhorizon is None:
                     self.select_best()
-                best_horizon = self.model_rank_perhorizon[score].iloc[:self.nbest].T
+                best_horizon = self.model_rank_perhorizon[score].iloc[:self._nbest].T
                 best_horizon = best_horizon.apply(lambda x: x.values, axis=1).to_dict()
                 errors_best_horizon = []
                 for h, best_mod_h in best_horizon.items():
                     errors_best_horizon.append(errors_df.loc[(errors_df.horizon==h) & errors_df.forecaster.isin(best_mod_h)]\
                         .groupby(['cutoff', 'horizon']).error.mean().reset_index())
                 return pd.concat(errors_best_horizon, axis=0).reset_index(drop=True)            
             
@@ -670,22 +717,22 @@
         Returns:
         --------        
             matplotlib.figure.Figure or matplotlib.axes._subplots.AxesSubplot
                 The figure and axes of the plot.
         """
         
         if view =='horizon':
-            if self.avg_oos_horizon is None:
+            if self._avg_oos_horizon is None:
                 self.select_best()
-            toplot = self.avg_oos_horizon[score]
+            toplot = self._avg_oos_horizon[score]
 
         elif view=='cutoff':
-            if self.avg_oos_hist is None:
-                self.oos_per_cutoff()
-            toplot = self.avg_oos_hist[score]
+            if self.summary_cutoff is None:
+                self.summary_per_cutoff()
+            toplot = self.summary_cutoff[score]
 
         else:
             raise ValueError('view can take only 2 values: horizon or cutoff')
 
         if model_subset is not None:
             assert all([m in toplot.columns for m in model_subset]), 'Some models are not in the list of models'
             toplot = toplot[model_subset]
@@ -766,15 +813,15 @@
 
         Returns:
         --------        
             matplotlib.figure.Figure or matplotlib.axes._subplots.AxesSubplot
                 The figure and axes of the plot.
         """
 
-        y = list(self.LF_d.values())[0].y
+        y = list(self.LF_d.values())[0]._y
         y_train = y.loc[y.index<y_pred.index[0]]
         zoom_y_train = y_train.iloc[-3*len(y_pred):]
     
         if models_preds is not None:
             model_names = models_preds.columns
             models_preds = [models_preds[c] for c in model_names]
             labels = ['y'] + list(model_names) + [aggregation_label]
@@ -846,26 +893,26 @@
         """
         _lf  = list(self.LF_d.values())[0]
         return _lf.plot.plot_cv_procedure(**kwargs)
     
     def __aggregate_pred(self, mode, preds, pred_ints, score=None, ret_underlying=False):
 
         if score is None:
-            score = self.score
+            score = self._score
  
-        nbest = self.nbest
+        nbest = self._nbest
         if mode is None:
-            mode = self.mode
+            mode = self._mode
 
-        if  (mode !='average') & (self.best_x_overall is None):
+        if  (mode !='average') & (self._best_x_overall is None):
             self.select_best(score = score)
 
         if mode =='best':
             # returns the prediction of the best model
-            _best_model = self.best_x_overall[score][0]
+            _best_model = self._best_x_overall[score][0]
             y_pred = preds[_best_model]            
             if _best_model in pred_ints.columns:
                 y_pred_int = pred_ints[_best_model]
             else:
                 print(f'Prediction intervals for {_best_model} are not available')
                 y_pred_int = pd.DataFrame()
 
@@ -901,17 +948,17 @@
                     continue
                 else:
                     _weigh_preds_ints = _weigh_preds_ints+ pred_ints[m]*w
             y_pred_int = _weigh_preds_ints.astype('float')
 
         elif mode == 'nbest_average':
             # return the average prediction of nbest models
-            y_pred = preds[self.best_x_overall[score]].mean(axis=1)
-            if all([v in pred_ints.columns for v in self.best_x_overall[score]]):
-                y_pred_int = pred_ints[self.best_x_overall[score]]\
+            y_pred = preds[self._best_x_overall[score]].mean(axis=1)
+            if all([v in pred_ints.columns for v in self._best_x_overall[score]]):
+                y_pred_int = pred_ints[self._best_x_overall[score]]\
             .unstack().unstack(0).mean(axis=1).unstack().T
             else:
                 print(f'Prediction intervals for {nbest} best models are not available')
                 y_pred_int = None
 
         elif mode == 'nbest_average_horizon':
             # return the average prediction on the nbest models per horizon
```

### Comparing `forecast_combine-0.0.2/forecast_combine/reconcile.py` & `forecast_combine-0.0.3/forecast_combine/reconcile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Hierarchical Time Series Forecast Reconciliation."""
 __description__ = "Time Series Forecast Combination"
 __author__ = "Amine Raboun - amineraboun@github.io"
 
-import logging
-logging.getLogger().setLevel(logging.ERROR)
 import warnings
-warnings.simplefilter('ignore')
 warnings.filterwarnings("ignore")
 
 import numpy as np
 import pandas as pd
 from numpy.linalg import pinv
 from typing import Dict, Optional
 
@@ -17,108 +14,153 @@
 from .model_select import ForecastModelSelect
 
 # Plotting packages & configuration
 from forecast_combine.utils.plotting import plot_series
 import matplotlib.pyplot as plt
 
 class ForecastReconciler:
+    """
+    ForecastReconciler class to apply the hiearachical reconciliation of the child node forecast with the total forecast.
+
+    Parameters:
+    -----------
+    - forecasters_d (Dict[str, any]): Dictionary of forecasters to reconcile.
+    - S (pd.DataFrame): Summation matrix.
+    - method (str): Reconciliation method to use. Default is 'mint'. Available methods are 
+        - ols: Ordinary Least Squares
+        - wls: Weighted Least Squares
+        - mint: Minimum Trace
+        - td: Top-Down        
+        - bu: Bottom-Up
+
+    Attributes:
+    -----------
+    - _forecasters_d (Dict[str, any]): Dictionary of forecasters to reconcile.
+    - _Total (str): Name of the total forecast.
+    - _forecasters_order (List[str]): Order of the forecasters.
+    - _S (np.array): Summation matrix.
+    - _method (str): Reconciliation method to use.
+    - _historical_values_d (Dict[str, pd.Series]): Dictionary of historical values for each forecaster.
+    - _historical_errors_d (Dict[str, pd.DataFrame]): Dictionary of historical errors for each forecaster.
+    - _weights (Dict[str, np.array]): Dictionary of weights for each forecaster.
+
+    Methods:
+    --------
+    - fit(refit_models: bool = False, reconciliation_method: Optional[str] = None) -> None:
+        Prepare the reconciliation weights or parameters based on historical data.
+        Optionally refit models.
+    - predict(X: Dict[str, pd.DataFrame] = None, coverage: float = 0.9, reconciliation_method: Optional[str] = None, verbose: bool = False) -> pd.DataFrame:
+        Apply the reconciliation method to the forecasts.
+    - update(new_y:Dict[str, pd.Series], new_X: Dict[str, pd.DataFrame] = None, reconciliation_method: Optional[str] = None, coverage: float = 0.9, refit: bool = False, reevaluate:bool = False, verbose: bool = False) -> pd.DataFrame:
+        Update the forecast with new data.
+    - reconcile_preds(forecast_data: Dict[str, pd.DataFrame], forecast_intervals: Dict[str, pd.DataFrame], reconciliation_method: Optional[str] = None) -> pd.DataFrame:
+        Apply the reconciliation method to the forecasts.
+    - plot_predict(reconciled_preds, reconciled_intervals, interval_label: str = 'CI', title: str = 'Reconciled Predictions') -> None:
+        Plot the reconciled predictions and intervals.
+    
+    Raises:
+    -------
+    - AssertionError: If the number of forecasters does not match the number of rows in S.
+    - AssertionError: If the number of columns in S does not match the number of the child forecasters.
+    - AssertionError: If the index values of S do not match the keys in forecasters_d.
+    - AssertionError: If the reconciliation method is invalid.
+        
+    """
     def __init__(self, 
                  forecasters_d: Dict[str, any], 
                  S: pd.DataFrame, 
                  method: str = 'mint',
                  ):
-        """
-        Initializes the ForecastReconciler class.
-        
-        Parameters:
-        -----------
-        - forecasters_d (Dict[str, any]): Dictionary of forecaster objects for each series.
-        - S (pd.DataFrame): Aggregation matrix indicating how lower levels aggregate into the total.
-        - method (str): Method of reconciliation ('ols', 'wls', 'td', 'mint', 'bu').
-        """
+        """ Inintialize the ForecastReconciler class."""
         assert S.shape[0] == len(forecasters_d), "Number of forecasters must match number of rows in S."
         assert S.shape[1] == S.shape[0]-1, "Number of columns in S must match number of the child forecasters."
         assert all([s in forecasters_d.keys() for s in S.index]), "Index values of S must match keys in forecasters_d."
-        self.methods_l = ['ols', 'wls', 'td', 'mint', 'bu']
-        assert method in self.methods_l, "Invalid reconciliation method."
-        self.forecasters_d = forecasters_d
-        self.Total = S.index[0]
-        self.forecasters_order = S.index
-        self.S = S.values
-        self.method = method
-        self.historical_values_d = None
-        self.historical_errors_d = None
-        self.weights = None
+        self._methods_l = ['ols', 'wls', 'td', 'mint', 'bu']
+        assert method in self._methods_l, "Invalid reconciliation method."
+        self._forecasters_d = forecasters_d
+        self._Total = S.index[0]
+        self._forecasters_order = S.index
+        self._S = S.values
+        self._method = method
+        self._historical_values_d = None
+        self._historical_errors_d = None
+        self._weights = None
    
     def fit(self,
             refit_models: bool = False,
             reconciliation_method: Optional[str] = None
             ) -> None:
         """
         Prepare the reconciliation weights or parameters based on historical data.
         Optionally refit models.
         """
         if refit_models:
-            for forecaster in self.forecasters_d.values():
+            for forecaster in self._forecasters_d.values():
                 forecaster.fit()
         if reconciliation_method is None:
-            reconciliation_method = self.method
+            reconciliation_method = self._method
 
         if reconciliation_method in ['wls', 'mint']:
             print(f"{reconciliation_method} reconciliation method requires the forecasters prediction errors variance-covariance matrix ...")
-            self.historical_errors_d = self.__compute_hist_errors()
-            historical_errors = pd.concat(self.historical_errors_d).reset_index(0).rename(columns={'level_0':'nodes'})
+            self._historical_errors_d = self.__compute_hist_errors()
+            historical_errors = pd.concat(self._historical_errors_d).reset_index(0).rename(columns={'level_0':'nodes'})
 
             if reconciliation_method == 'wls':
                 _wght = {}
                 for horizon, group in historical_errors.groupby('horizon'):
                     _var = group.pivot(index='cutoff', columns='nodes', values='error').var()
-                    _wght[horizon] = np.diag(1 / _var.loc[self.forecasters_order])
-                self.weights = _wght
+                    _wght[horizon] = np.diag(1 / _var.loc[self._forecasters_order])
+                self._weights = _wght
             elif reconciliation_method == 'mint':
                 _wght = {}
                 for horizon, group in historical_errors.groupby('horizon'):
-                    ordered_group = group.pivot(index='cutoff', columns='nodes', values='error')[self.forecasters_order]
+                    ordered_group = group.pivot(index='cutoff', columns='nodes', values='error')[self._forecasters_order]
                     _wght[horizon] = pinv(ordered_group.cov().values)
-                self.weights = _wght
+                self._weights = _wght
         elif reconciliation_method == 'td':
-            self.historical_values_d = self.__compute_hist_values()
-            historical_values_df = pd.concat(self.historical_values_d, axis=1)[self.forecasters_order]
-            historical_values_prop = (historical_values_df.iloc[:, 1:]*self.S[0]).div(historical_values_df[self.Total], axis=0)
+            self._historical_values_d = self.__compute_hist_values()
+            historical_values_df = pd.concat(self._historical_values_d, axis=1)[self._forecasters_order]
+            historical_values_prop = (historical_values_df.iloc[:, 1:]*self._S[0]).div(historical_values_df[self._Total], axis=0)
             historical_values_prop_mean = historical_values_prop.mean().to_dict()
-            historical_values_prop_mean[self.Total] = 1
-            self.weights = historical_values_prop_mean
+            historical_values_prop_mean[self._Total] = 1
+            self._weights = historical_values_prop_mean
         else:
             pass  # No weights needed for 'bu' or 'ols'
    
     def predict(self, 
                 X: Dict[str, pd.DataFrame] = None,
                 coverage: float = 0.9,
                 reconciliation_method: Optional[str] = None,
                 verbose: bool = False
                 ) -> pd.DataFrame:
         """
         Apply the reconciliation method to the forecasts.
         
         Parameters:
         -----------
-        - X (Optional[pd.DataFrame]): DataFrame containing independent variables for prediction, if needed.
-        - coverage (float): Confidence interval for the forecast quantiles.
-        - reconciliation_method (Optional[str]): Override the default method for this prediction.
+            X (Optional[pd.DataFrame]): 
+                DataFrame containing independent variables for prediction, if needed.
+            coverage (float):
+                Confidence interval for the forecast quantiles.
+            reconciliation_method (Optional[str]):
+                Override the default method for this prediction.
         
         Returns:
         --------
-        - pd.DataFrame: Reconciled forecasts.
+            reconciled_preds (Dict[str, pd.Series]):
+                Dictionary of reconciled forecasts.
+            reconciled_intervals (Dict[str, pd.DataFrame]):
+                Dictionary of reconciled forecast intervals.
         """
-        assert reconciliation_method in self.methods_l, "Invalid reconciliation method."
+        assert reconciliation_method in self._methods_l, "Invalid reconciliation method."
         if verbose:
             print("Computing the Hiearchical models forecasts ...")
         forecast_data = {}
         forecast_intervals ={}
-        for name, forecaster in self.forecasters_d.items():
+        for name, forecaster in self._forecasters_d.items():
             if X is None:
                 forecster_X = None
             else:
                 forecster_X = X[name] if name in X.keys() else None
             if verbose:
                 print(f"\tComputing forecasts for {name} ...")
             forecast_data[name], forecast_intervals[name] = forecaster.predict(X=forecster_X, coverage=coverage)
@@ -137,28 +179,36 @@
                verbose: bool = False
               ) -> pd.DataFrame: 
         """
         Update the forecast with new data.
 
         Parameters:
         -----------
-        - newdata (pd.DataFrame): New data to update the forecast.
-        - reconciliation_method (Optional[str]): Override the default method for this prediction.
-        - refit (bool): If True, refit the models before updating the forecast.
+            newdata (pd.DataFrame): 
+                New data to update the forecast.
+            reconciliation_method (Optional[str]):
+                Override the default method for this prediction.
+            refit (bool):
+                If True, refit the models before updating the forecast.
 
         Returns:
         --------
-        - pd.DataFrame: Reconciled forecasts.
+        Returns:
+        --------
+            reconciled_preds (Dict[str, pd.Series]):
+                Dictionary of reconciled forecasts.
+            reconciled_intervals (Dict[str, pd.DataFrame]):
+                Dictionary of reconciled forecast intervals.
         """        
-        assert reconciliation_method in self.methods_l, "Invalid reconciliation method."   
+        assert reconciliation_method in self._methods_l, "Invalid reconciliation method."   
         if verbose:
             print("Computing the Hiearchical models forecasts ...")
         forecast_data = {}
         forecast_intervals = {}
-        for name, forecaster in self.forecasters_d.items():
+        for name, forecaster in self._forecasters_d.items():
             forecaster_y = new_y[name] 
             if new_X is None:
                 forecster_X = None
             else:
                 forecster_X = new_X[name] if name in new_X.keys() else None
             if verbose:
                 print(f"\tComputing forecasts for {name} ...")
@@ -178,61 +228,87 @@
                 reconciliation_method: Optional[str] = None
                 ) -> pd.DataFrame:
         """
         Apply the reconciliation method to the forecasts.
         
         Parameters:
         -----------
-        - forecast_data (Dict[str, pd.DataFrame]): Dictionary of forecasts for each series.
+            forecast_data (Dict[str, pd.DataFrame]): 
+                Dictionary of forecasts for each series.
         
         Returns:
         --------
-        - pd.DataFrame: Reconciled forecasts.
+            reconciled_preds (Dict[str, pd.Series]):
+                Dictionary of reconciled forecasts.
+            reconciled_intervals (Dict[str, pd.DataFrame]):
+                Dictionary of reconciled forecast intervals.           
+            
         """
         if reconciliation_method is None:
-            reconciliation_method = self.method
+            reconciliation_method = self._method
         
         if (reconciliation_method in ['wls', 'mint', 'td']):
             self.fit(reconciliation_method=reconciliation_method)
         
-        y_preds = np.vstack([forecast_data[name] for name in self.forecasters_order])
-        y_preds_lower = np.vstack([forecast_intervals[name].xs('lower', level =2, axis=1).squeeze() for name in self.forecasters_order])
-        y_preds_upper = np.vstack([forecast_intervals[name].xs('upper', level =2, axis=1).squeeze() for name in self.forecasters_order])
+        y_preds = np.vstack([forecast_data[name] for name in self._forecasters_order])
+        y_preds_lower = np.vstack([forecast_intervals[name].xs('lower', level =2, axis=1).squeeze() for name in self._forecasters_order])
+        y_preds_upper = np.vstack([forecast_intervals[name].xs('upper', level =2, axis=1).squeeze() for name in self._forecasters_order])
         
         # Reconcile forecasts and intervals using the same weights and matrices
         reconciled_forecasts = self.__apply_reconciliation(y_preds, reconciliation_method)
         reconciled_lower_bounds = self.__apply_reconciliation(y_preds_lower, reconciliation_method)
         reconciled_upper_bounds = self.__apply_reconciliation(y_preds_upper, reconciliation_method)
 
         # Return the reconciled forecasts and intervals
         reconciled_preds ={}
         reconciled_intervals = {}
-        dates = forecast_data[self.Total].index
-        for i, name in enumerate(self.forecasters_order):
+        dates = forecast_data[self._Total].index
+        for i, name in enumerate(self._forecasters_order):
             reconciled_preds[name] = pd.Series(reconciled_forecasts[i], index = dates).rename(name)
             _interval = pd.DataFrame(np.vstack([reconciled_lower_bounds[i], reconciled_upper_bounds[i]]).T, 
                                                       index = dates, columns = ['lower', 'upper'])
             _interval.columns = forecast_intervals[name].columns
             reconciled_intervals[name] = _interval        
         return reconciled_preds, reconciled_intervals
     
     def plot_predict(self, 
                      reconciled_preds,
                      reconciled_intervals,
                      interval_label: str = 'CI', 
                     title: str = 'Reconciled Predictions',
                     ):
-        self.historical_values_d = self.__compute_hist_values()
+        """
+        Plot the reconciled predictions and intervals.
+
+        Parameters:
+        -----------
+            reconciled_preds (Dict[str, pd.Series]): 
+                Dictionary of reconciled forecasts.
+            reconciled_intervals (Dict[str, pd.DataFrame]):
+                Dictionary of reconciled forecast intervals.
+            interval_label (str):
+                Label for the confidence interval.
+            title (str):
+                Title of the plot.
+
+        Returns:
+        --------
+            fig (plt.Figure):
+                Plot figure.
+            axes (plt.Axes):
+                Plot axes.
+        """
+        self._historical_values_d = self.__compute_hist_values()
         nplots = len(reconciled_preds)
         ncols = 2
         nrows = nplots // ncols + nplots % ncols
         fig, axes = plt.subplots(nrows, ncols, figsize=(20, 6*nrows))
         axes = axes.flatten()
         for i, name in enumerate(reconciled_preds.keys()):
-            y_i = self.historical_values_d[name]
+            y_i = self._historical_values_d[name]
             ypred_i = reconciled_preds[name]
             y_i = y_i.loc[y_i.index<ypred_i.index[0]]
             zoom_y_train = y_i.iloc[-3*len(ypred_i):]
             plot_series(zoom_y_train,
                         ypred_i,
                         labels =['y', 'y_pred'],
                         pred_interval= reconciled_intervals[name],
@@ -242,53 +318,53 @@
                         )
         fig.tight_layout()
         fig.suptitle(title, size="xx-large")
         fig.subplots_adjust(top=0.9)        
         return fig, axes
     
     def __compute_hist_errors(self, verbose=False):
-        if self.historical_errors_d is None:                
+        if self._historical_errors_d is None:                
             if verbose:
                 print("\nComputing the prediction errors for all forecasters ...")
             _d = {}
-            for k, forecaster in self.forecasters_d.items():
+            for k, forecaster in self._forecasters_d.items():
                 if verbose:
                     print(f"\tComputing prediction errors for {k} ...")
                 _d[k] = forecaster.get_pred_errors()
-            self.historical_errors_d = _d
-        return self.historical_errors_d
+            self._historical_errors_d = _d
+        return self._historical_errors_d
     def __compute_hist_values(self, verbose=False):    
-        if self.historical_values_d is None:
+        if self._historical_values_d is None:
             if verbose:
                 print("Computing the historical values for all forecasters ...")
             _d = {}
-            for k, forecaster in self.forecasters_d.items():
+            for k, forecaster in self._forecasters_d.items():
                 if isinstance(forecaster, Forecast):
-                    _d[k] = forecaster.y
+                    _d[k] = forecaster._y
                 elif isinstance(forecaster, ForecastModelSelect):
-                    _d[k] = list(forecaster.LF_d.values())[0].y
-            self.historical_values_d = _d
-        return self.historical_values_d
+                    _d[k] = list(forecaster.LF_d.values())[0]._y
+            self._historical_values_d = _d
+        return self._historical_values_d
     
     def __apply_reconciliation(self, y_preds: np.array, reconciliation_method: str) -> pd.DataFrame:
         """
         Apply the reconciliation method to the forecasts.
         """
         if reconciliation_method == 'td':
             total_forecast = y_preds[0]
-            reconciled_forecasts_d = {name: total_forecast.T * self.weights[name] for name in self.forecasters_order}
+            reconciled_forecasts_d = {name: total_forecast.T * self._weights[name] for name in self._forecasters_order}
             reconciled_forecasts = reconciled_forecasts_d.values()
-            reconciled_forecasts = np.array([total_forecast.T * self.weights[name] for name in self.forecasters_order])  
+            reconciled_forecasts = np.array([total_forecast.T * self._weights[name] for name in self._forecasters_order])  
         elif reconciliation_method == 'bu':
-            reconciled_forecasts = self.S @ y_preds[1:, :]
+            reconciled_forecasts = self._S @ y_preds[1:, :]
         
         elif reconciliation_method == 'ols':
-            M = self.S @ pinv(self.S.T @ self.S) @ self.S.T
+            M = self._S @ pinv(self._S.T @ self._S) @ self._S.T
             reconciled_forecasts = M  @ y_preds
         
         elif reconciliation_method in ['wls', 'mint']:
             reconciled_forecasts = pd.DataFrame()
-            for horizon in self.weights.keys():
-                M = self.S @ pinv(self.S.T @ self.weights[horizon] @ self.S) @ self.S.T @ self.weights[horizon]
+            for horizon in self._weights.keys():
+                M = self._S @ pinv(self._S.T @ self._weights[horizon] @ self._S) @ self._S.T @ self._weights[horizon]
                 reconciled_forecasts = M @ y_preds
 
         return reconciled_forecasts
```

### Comparing `forecast_combine-0.0.2/forecast_combine/utils/explore.py` & `forecast_combine-0.0.3/forecast_combine/utils/explore.py`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.2/forecast_combine/utils/metrics.py` & `forecast_combine-0.0.3/forecast_combine/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.2/forecast_combine/utils/plotting.py` & `forecast_combine-0.0.3/forecast_combine/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.2/pyproject.toml` & `forecast_combine-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forecast_combine"
-version = "0.0.2"
+version = "0.0.3"
 description = "Automation of forecast models testing, combining and predicting"
 authors = ["amineraboun <amineraboun@gmail.com>"]
 repository ="https://github.com/amineraboun/forecast"
 homepage  ="https://github.com/amineraboun/forecast"
 
 readme = "README.md"
 keywords = ["arima", "ets", "theta", "tbats", "prophet"]
@@ -28,14 +28,16 @@
 matplotlib = "^3.7.2"
 seaborn = "^0.12.2"
 sphinx = "^7.1.2"
 nbsphinx = "^0.9.2"
 sphinx-mdinclude = "^0.5.3"
 pandoc = "^2.3"
 openpyxl = "^3.1.2"
+pdoc = "^14.4.0"
+typing-extensions = "^4.11.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
 
 [tool.pytest.ini_options]
```

### Comparing `forecast_combine-0.0.2/PKG-INFO` & `forecast_combine-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecast_combine
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automation of forecast models testing, combining and predicting
 Home-page: https://github.com/amineraboun/forecast
 Keywords: arima,ets,theta,tbats,prophet
 Author: amineraboun
 Author-email: amineraboun@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -14,23 +14,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arch (>=6.3.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: nbsphinx (>=0.9.2,<0.10.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandoc (>=2.3,<3.0)
+Requires-Dist: pdoc (>=14.4.0,<15.0.0)
 Requires-Dist: prophet (>=1.1.4,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: sktime (>=0.28.0,<0.29.0)
 Requires-Dist: sphinx (>=7.1.2,<8.0.0)
 Requires-Dist: sphinx-mdinclude (>=0.5.3,<0.6.0)
 Requires-Dist: statsforecast (>=1.7.4,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tbats (>=1.1.3,<2.0.0)
 Requires-Dist: tqdm (>=4.66.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Project-URL: Repository, https://github.com/amineraboun/forecast
 Description-Content-Type: text/markdown
 
 # forecast_combine
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
```

