# Comparing `tmp/wedme-plots-2.0.2.tar.gz` & `tmp/wedme_plots-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedme-plots-2.0.2.tar", last modified: Tue Mar 26 16:00:26 2024, max compression
+gzip compressed data, was "wedme_plots-2.0.3.tar", last modified: Fri Apr 19 10:59:03 2024, max compression
```

## Comparing `wedme-plots-2.0.2.tar` & `wedme_plots-2.0.3.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-03-26 16:00:26.549648 wedme-plots-2.0.2/
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     1068 2023-12-13 20:04:39.000000 wedme-plots-2.0.2/LICENSE
--rw-r--r--   0 mruijzendaal   (501) staff       (20)       29 2023-12-14 08:27:42.000000 wedme-plots-2.0.2/MANIFEST.in
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     5885 2024-03-26 16:00:26.549181 wedme-plots-2.0.2/PKG-INFO
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     3772 2024-01-25 15:08:08.000000 wedme-plots-2.0.2/README.md
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      899 2024-03-26 15:56:18.000000 wedme-plots-2.0.2/pyproject.toml
--rw-r--r--   0 mruijzendaal   (501) staff       (20)       38 2024-03-26 16:00:26.549744 wedme-plots-2.0.2/setup.cfg
-drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-03-26 16:00:26.538147 wedme-plots-2.0.2/src/
-drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-03-26 16:00:26.545799 wedme-plots-2.0.2/src/wedme/
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      358 2024-03-26 15:11:33.000000 wedme-plots-2.0.2/src/wedme/__init__.py
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      892 2024-01-25 12:32:37.000000 wedme-plots-2.0.2/src/wedme/a0.mplstyle
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     2401 2024-03-25 07:37:14.000000 wedme-plots-2.0.2/src/wedme/common.mplstyle
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      929 2024-03-05 13:12:47.000000 wedme-plots-2.0.2/src/wedme/const.py
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      814 2024-01-10 12:32:27.000000 wedme-plots-2.0.2/src/wedme/elspaper.mplstyle
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     4421 2024-03-26 15:53:11.000000 wedme-plots-2.0.2/src/wedme/gif.py
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      893 2024-03-05 12:13:18.000000 wedme-plots-2.0.2/src/wedme/slides.mplstyle
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     2876 2024-03-05 13:23:25.000000 wedme-plots-2.0.2/src/wedme/styledefs.py
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     1723 2024-03-19 10:01:36.000000 wedme-plots-2.0.2/src/wedme/util.py
-drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-03-26 16:00:26.548134 wedme-plots-2.0.2/src/wedme_plots.egg-info/
--rw-r--r--   0 mruijzendaal   (501) staff       (20)     5885 2024-03-26 16:00:26.000000 wedme-plots-2.0.2/src/wedme_plots.egg-info/PKG-INFO
--rw-r--r--   0 mruijzendaal   (501) staff       (20)      439 2024-03-26 16:00:26.000000 wedme-plots-2.0.2/src/wedme_plots.egg-info/SOURCES.txt
--rw-r--r--   0 mruijzendaal   (501) staff       (20)        1 2024-03-26 16:00:26.000000 wedme-plots-2.0.2/src/wedme_plots.egg-info/dependency_links.txt
--rw-r--r--   0 mruijzendaal   (501) staff       (20)       72 2024-03-26 16:00:26.000000 wedme-plots-2.0.2/src/wedme_plots.egg-info/requires.txt
--rw-r--r--   0 mruijzendaal   (501) staff       (20)        6 2024-03-26 16:00:26.000000 wedme-plots-2.0.2/src/wedme_plots.egg-info/top_level.txt
+drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-04-19 10:59:03.209770 wedme_plots-2.0.3/
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     1068 2023-12-13 20:04:39.000000 wedme_plots-2.0.3/LICENSE
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       41 2024-04-17 15:14:31.000000 wedme_plots-2.0.3/MANIFEST.in
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     7808 2024-04-19 10:59:03.208480 wedme_plots-2.0.3/PKG-INFO
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     5686 2024-04-19 10:41:57.000000 wedme_plots-2.0.3/README.md
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      907 2024-04-19 10:52:00.000000 wedme_plots-2.0.3/pyproject.toml
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       38 2024-04-19 10:59:03.209998 wedme_plots-2.0.3/setup.cfg
+drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-04-19 10:59:03.194330 wedme_plots-2.0.3/src/
+drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-04-19 10:59:03.198396 wedme_plots-2.0.3/src/wedme/
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      415 2024-04-19 07:57:07.000000 wedme_plots-2.0.3/src/wedme/__init__.py
+drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-04-19 10:59:03.200486 wedme_plots-2.0.3/src/wedme/apply/
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       25 2024-04-17 15:20:41.000000 wedme_plots-2.0.3/src/wedme/apply/a0.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       26 2024-04-17 15:20:54.000000 wedme_plots-2.0.3/src/wedme/apply/dev.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       28 2024-04-17 15:21:04.000000 wedme_plots-2.0.3/src/wedme/apply/paper.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       29 2024-04-17 15:21:13.000000 wedme_plots-2.0.3/src/wedme/apply/slides.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       29 2024-04-17 15:21:25.000000 wedme_plots-2.0.3/src/wedme/apply/thesis.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     1305 2024-04-19 08:39:33.000000 wedme_plots-2.0.3/src/wedme/const.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     4387 2024-03-27 10:41:49.000000 wedme_plots-2.0.3/src/wedme/gif.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     2996 2024-04-19 10:47:13.000000 wedme_plots-2.0.3/src/wedme/shorthands.py
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     1547 2024-04-19 10:49:57.000000 wedme_plots-2.0.3/src/wedme/styledefs.py
+drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-04-19 10:59:03.203484 wedme_plots-2.0.3/src/wedme/stylesheets/
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      892 2024-01-25 12:32:37.000000 wedme_plots-2.0.3/src/wedme/stylesheets/a0.mplstyle
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     2401 2024-03-25 07:37:14.000000 wedme_plots-2.0.3/src/wedme/stylesheets/common.mplstyle
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      814 2024-01-10 12:32:27.000000 wedme_plots-2.0.3/src/wedme/stylesheets/elspaper.mplstyle
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      893 2024-03-05 12:13:18.000000 wedme_plots-2.0.3/src/wedme/stylesheets/slides.mplstyle
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      814 2024-04-10 14:51:50.000000 wedme_plots-2.0.3/src/wedme/stylesheets/thesis.mplstyle
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     2227 2024-04-18 11:59:47.000000 wedme_plots-2.0.3/src/wedme/util.py
+drwxr-xr-x   0 mruijzendaal   (501) staff       (20)        0 2024-04-19 10:59:03.206899 wedme_plots-2.0.3/src/wedme_plots.egg-info/
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)     7808 2024-04-19 10:59:03.000000 wedme_plots-2.0.3/src/wedme_plots.egg-info/PKG-INFO
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)      671 2024-04-19 10:59:03.000000 wedme_plots-2.0.3/src/wedme_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)        1 2024-04-19 10:59:03.000000 wedme_plots-2.0.3/src/wedme_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)       72 2024-04-19 10:59:03.000000 wedme_plots-2.0.3/src/wedme_plots.egg-info/requires.txt
+-rw-r--r--   0 mruijzendaal   (501) staff       (20)        6 2024-04-19 10:59:03.000000 wedme_plots-2.0.3/src/wedme_plots.egg-info/top_level.txt
```

### Comparing `wedme-plots-2.0.2/LICENSE` & `wedme_plots-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wedme-plots-2.0.2/PKG-INFO` & `wedme_plots-2.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,123 @@
-Metadata-Version: 2.1
-Name: wedme-plots
-Version: 2.0.2
-Summary: We Don't Make Embarrassing Plots. Matplotlib styles for papers, posters and presentations.
-Author-email: Martijn Ruijzendaal <martijn.ruijzendaal@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2018 Real Python
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/mruijzendaal/wedme-plots
-Project-URL: documentation, https://github.com/mruijzendaal/wedme-plots
-Keywords: matplotlib
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: importlib_resources
-Provides-Extra: build
-Requires-Dist: build; extra == "build"
-Requires-Dist: twine; extra == "build"
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-
 # 👗 wedme-plots: We Don't Make Embarrassing Plots
 
-Matplotlib styles for papers, posters and presentations. Tailored for academic use.
+Matplotlib styles for papers, posters, presentations and theses. Tailored for academic use.
 
 ## Too long; didn't read
-```python
-import wedme
+1. Pick a style from `paper`, `slide`, `a0`, `thesis`.
+2. Decide the final size of the figure on the chosen medium. 
+For example, the column width (`cw`) and default height (`dh`) for the `paper` style.
+3. Import `wedme`
+4. Before using matplotlib, apply the style using `wedme.apply.[style]_[width]_[height]()`. In the above example, `wedme.apply.paper_cw_dh()`.
 
-# Open a figure in `paper` style, with size (PAPER_CW, PAPER_DH)
-# which equals (journal column width, default height)
-wedme.figure.paper_cw_dh()
-
-# Open a figure with the style `slide` and size (SLIDE_TW, SLIDE_HH) 
-# which equals (1/3 slide width, 1/2 slide height)
-wedme.figure.slide_tw_hh()
+
+## Installation
+Install from [PyPI](https://pypi.org/project/wedme-plots/) using PIP:
+```
+pip install wedme-plots
 ```
 
+For Anaconda users:
+- Open an Anaconda Prompt
+- Optional: if you use an environment other than `base`, open it using `conda activate [my environment]`
+- Install pip using `conda install pip`
+- Install wedme-plots using `pip install wedme-plots`
+
 ## Styling
-We applied a clean style. The style and sizes of `paper` style are compatible with most journals (Nature, Science, Elsevier). The `slide` style is compatible with a Microsoft Powerpoint presentation. `poster`  is compatible with A0 posters.
+Wedme offers multiple styles:
+- `paper`: compatible with most journals (Nature, Science, Elsevier). 
+- `slide`: compatible with a (16:9) Microsoft Powerpoint presentation. 
+- `a0`: A0 poster.
+- `thesis`: (work-in-progress) similar to `paper` but for the B5 page format.
 
 ## Usage
-Import the `wedme` module and apply the desired style. Then proceed with `matplotlib` plotting as you're used to.
+There are two ways of applying a wedme style. 
+
+### 1. Global styling and sizing
+
+Import the `wedme` module and apply the desired style, e.g. `wedme.apply.paper()`. 
+This applies the specified style and its default size to every subsequent figure.
 
 Example:
 ```python
 import wedme
 
 # These commands apply a style to subsequent Matplotlib figures.
 
-# For Elsevier-compatible paper styles
-wedme.paper()
-
-# For a 16:9 Powerpoint slide
-wedme.slide()
+# Pick one:
+wedme.apply.paper()  # For Elsevier-compatible paper styles
+wedme.apply.slide()  # For a 16:9 Powerpoint slide
+wedme.apply.a0()     # For A0 posters
+wedme.apply.thesis() # For B5-paper thesis
 
-# For A0 posters (not implemented yet)
-wedme.poster()
+# Optionally, change the default size:
+wedme.apply.slide_tw_hh()
 
 # Proceed with plotting as usual
-import numpy as np
 import matplotlib.pyplot as plt
 
-x = np.linspace(0, np.pi, 1000)
-
 plt.figure()
-plt.plot(x, np.sin(x), label="Sine")
-plt.plot(x, np.cos(x), label="Cosine")
+plt.plot([1, 2, 3, 4])
 plt.show()
 ```
 
-## Sizing
-For custom figure sizes, we include reference points for every style:
+### 2. Local styling and sizing
 
-- Paper. Default size: `(wedme.PAPER_CW, wedme.paper_GH)`
-  - `wedme.PAPER_FW` is the full textwidth of an Elsevier journal, 190mm.
-  - `wedme.PAPER_CW` is the full columnwidth of an Elsevier journal in two-column layout, 90mm.
-  - `wedme.PAPER_GH` is the height that has a golden ratio (1:1.618) to `wedme.PAPER_CW`.
-- Slide. Default size: `(wedme.SLIDE_TW, wedme.slide_HH)`
-  - `wedme.SLIDE_FW`, `wedme.SLIDE_HW` and `wedme.SLIDE_TW` represent 100%, 50% and 33% of the width of a Powerpoint 16:9 Widescreen slide.
-  - `wedme.SLIDE_FH`, `wedme.SLIDE_HH` and `wedme.SLIDE_TH` represent 100%, 50% and 33% of the height of a Powerpoint 16:9 Widescreen slide.
+Alternatively, one can open figures in a specified style and size using the `wedme` drop-in replacements for `plt.figure()` and `plt.subplots()` as follows:
 
-These can be used as follows:
 ```python
 import wedme
-wedme.slide()
-# Create a new figure that occupies 33% of the width of a ppt slide and 50% its height.
-plt.figure(figsize=(wedme.SLIDE_TW, wedme.SLIDE_HH))
-```
+import matplotlib.pyplot as plt
 
-Alternatively, we provide functions to compress the above code:
-```python
-wedme.figure.slide_tw_hh()
-```
-Such a function exists for every combination of heights and widths for a given style.
+# Open a figure in the `a0` style, 
+# with a size corresponding to half-width and half-height
+wedme.figure.a0_hw_hh()
+plt.plot([1, 2, 3, 4])
+
+# Open a figure with two subplots in the `slide` style,
+# with the figure size corresponding to half-width and half-height
+fig, (ax1, ax2) = wedme.subplots.slide_hw_hh(1, 2)
 
-To open a figure with one of `wedme`'s styles without applying any sizing, use e.g.
-```python
-wedme.figure.slide()
+ax1.plot([1, 2, 3, 4])
+ax2.plot([1, 2, 3, 4])
 ```
 
+Any arguments passed to `wedme.figure.[style]()` and `wedme.subplots.[style]()` are passed on to the equivalent matplotlib functions.
+
+## Sizing
+Matching the matplotlib figure size to the final display size of the figure is critically important: scaling to a different height will change font sizes and line widths.
+
+We include the following breakpoints, with respect to the available width and height (`H`) of the chosen medium:
+| Breakpoint | Ratio |
+| -- | -- |
+| `F` | 100% _("full")_ |
+| `TT` | 2/3 _("two-thirds")_ |
+| `H` | 1/2 _("half")_ |
+| `FT` | 5/12 _("five-twelfth")_ |
+| `T` | 1/3 _("third")_ |
+| `Q` | 1/4 _("quarter")_ |
+| `R` | 1/5 |
+| `S` | 1/6 |
+
+To specify the size using a breakpoint, append `W` (width) or `H` (height). For example, `wedme.figure.a0_hw_hh()` specifies the `a0` style, with a size of half the A0 width and height.
+
+In addition to the breakpoints, some styles include custom sizes:
+- `paper`: `CW` (column width) for two-column papers. `GH` is the height that corresponds to the golden-ratio of `CW`.
+- `thesis`: `LFW` and `LFH` for the landscape full-width and full-height.
+The default width and height `DW` and `DH` correspond to `CW` and `GH` of the `paper` style
+
+</br>
+
+When no size is specified, the following defaults sizes are used:
+- `paper`: `(wedme.PAPER_CW, wedme.paper_GH)`
+- `slide`: `(wedme.SLIDE_TW, wedme.slide_HH)`
+- `a0`:  `(wedme.A0_TW, ...)`
+- `thesis`: `(wedme.THESIS_DW, wedme.paper_DH)`
+
+
 ## Powerpoint
 Powerpoint automatically resizes artwork to a size that is different from the export size. To undo this:
 - Insert the figure in Powerpoint.
 - Picture Format > Reset Picture > Reset Picture & Size.
 
 ## Fonts
 Sans-serif fonts are the standards for figures because they remain readable even when small or pixelated. Helvetica or Arial fonts are preferred by Nature, Science and Elsevier. 
@@ -137,8 +128,14 @@
 `wedme` sets the `pdf.fonttype` parameter to `42` as recommended by Nature. This ensures that the text is editable even after exporting a pdf. `wedme` also changes the parameters `figure.autolayout` and `savefig.bbox` such that the specified sizes are respected.
 
 For saving figures, consider using [pypdfplot](https://github.com/dcmvdbekerom/pypdfplot) to maintain the ability to later change how data is displayed. Of course, we don't make embarassing plots to begin with.
 
 ## Examples
 <img src="https://github.com/mruijzendaal/wedme-plots/blob/main/img/calibration_curve_rot.png?raw=true" width="512">
 
-
+## Utilities
+Other than style sheets, wedme also includes utilities for commonly used operations.
+- Creating animated GIF images from multiple plots. See `wedme.gif`
+- Creating a legend only for unique entries. See `wedme.util.unique_legend()`
+- Specifying the colorbar label easily. See `wedme.util.colorbar()`
+- Specifying the minimum and maximum of the colorbar as a function of percentiles of the shown field. See `wedme.util.imshow()`
+- Making plot colors dependent on some variable. See `weme.util.get_colormap_norm()`
```

### Comparing `wedme-plots-2.0.2/pyproject.toml` & `wedme_plots-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wedme-plots"
-version = "2.0.2"
-description = "We Don't Make Embarrassing Plots. Matplotlib styles for papers, posters and presentations."
+version = "2.0.3"
+description = "We Don't Make Embarrassing Plots. Matplotlib styles for papers, posters, presentations and theses."
 readme = "README.md"
 authors = [{ name = "Martijn Ruijzendaal", email = "martijn.ruijzendaal@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `wedme-plots-2.0.2/src/wedme/a0.mplstyle` & `wedme_plots-2.0.3/src/wedme/stylesheets/a0.mplstyle`

 * *Files identical despite different names*

### Comparing `wedme-plots-2.0.2/src/wedme/common.mplstyle` & `wedme_plots-2.0.3/src/wedme/stylesheets/common.mplstyle`

 * *Files identical despite different names*

### Comparing `wedme-plots-2.0.2/src/wedme/elspaper.mplstyle` & `wedme_plots-2.0.3/src/wedme/stylesheets/elspaper.mplstyle`

 * *Files identical despite different names*

### Comparing `wedme-plots-2.0.2/src/wedme/gif.py` & `wedme_plots-2.0.3/src/wedme/gif.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,16 +124,15 @@
         If this behaviour is not desired, call `close` instead.
 
         Args:
             outname (str): The output filename for the GIF.
             frametime_ms (int, optional): The time in milliseconds between frames. Defaults to 800.
             resize_fac (float, optional): The factor by which to resize the frames. Defaults to 1.0.
         """
-        delay = round(frametime_ms / 10)
-        create_gif(f"{self._tempdir.name}/*.png", outname, resize_fac, delay)
+        create_gif(f"{self._tempdir.name}/*.png", outname, resize_fac, frametime_ms)
 
     def close(self, outname):
         """
         Closes the GIF file by saving it and performing any necessary cleanup.
 
         Args:
             outname (str): The name of the output file.
```

### Comparing `wedme-plots-2.0.2/src/wedme/slides.mplstyle` & `wedme_plots-2.0.3/src/wedme/stylesheets/slides.mplstyle`

 * *Files identical despite different names*

### Comparing `wedme-plots-2.0.2/src/wedme/styledefs.py` & `wedme_plots-2.0.3/src/wedme/shorthands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,88 @@
-import importlib_resources as _resources
+from wedme.styledefs import *
 import matplotlib.pyplot as _plt
 import matplotlib as _mpl
-from wedme.const import *
 
 
-## Functions for applying the wedme styles
-def _apply_style(stylename):
-    with _resources.files("wedme") / f"{stylename}.mplstyle" as file_path:
-        _plt.style.use(file_path)
-
-
-def reset():
-    _mpl.rcParams.update(_mpl.rcParamsDefault)
-
-
-def _common():
-    _apply_style("common")
-
-
-def slide():
-    _common()
-    _apply_style("slides")
-
-
-def paper():
-    _common()
-    _apply_style("elspaper")
-
-
-def dev():
-    paper()
-    _mpl.rcParams["figure.dpi"] = 200
-
-
-def poster():
-    _common()
-    _apply_style("a0")
+def _get_size_for_style(style: str, sizename: str):
+    size_const_name = f"{style}_{sizename}"
+    if size_const_name not in globals():
+        raise ValueError(
+            f"Style `{style.lower()}` does not have a size named `{sizename}`"
+        )
+    return globals()[size_const_name]
+
+
+def _get_style_and_figsize(name: str):
+    nameparts = name.upper().split("_")
+    stylename = nameparts[0]
+    assert get_style(stylename)
+
+    if len(nameparts) == 2 or len(nameparts) > 3:
+        # Not of the form `STYLE_WIDTH_HEIGHT` or `STYLE`
+        raise ValueError(
+            f"Invalid figure type: {name}. The correct form is `STYLE_WIDTH_HEIGHT` or `STYLE`"
+        )
+    elif len(nameparts) == 1:
+        # If the name is of the form `STYLE`, we assume that the figure size is not specified
+        figsize = None
+    else:
+        # Otherwise, we assume it is of the form `TYPE_WIDTH_HEIGHT`
+        # Extract the type, width, and height
+        wname, hname = nameparts[1:]
 
+        if wname.endswith("H"):
+            hname, wname = nameparts[1:]
 
-def apply_style(stylename):
-    # Call the appropriate figure type
-    if stylename == "PAPER":
-        paper()
-    elif stylename == "SLIDE" or stylename == "SLIDES":
-        stylename = "SLIDE"
-        slide()
-    elif stylename == "POSTER":
-        poster()
-    else:
-        raise ValueError(f"Unknown figure type {stylename}")
+        h = _get_size_for_style(stylename, hname)
+        w = _get_size_for_style(stylename, wname)
+        figsize = (w, h)
+    return stylename, figsize
 
 
-## Some more utility functions
 class _metafigure(type):
+    @classmethod
+    def _callfun(cls, *args, **kws):
+        raise NotImplementedError("This method should be overridden by the child class")
+
     # Catch-all for figure types. Any method call to this class will get intercepted here.
     def __getattr__(cls, name: str):
         # `name` is the name of the method that was called
-        nameparts = name.upper().split("_")
-
-        stylename = nameparts[0]
-        if stylename not in ["PAPER", "SLIDE", "POSTER"]:
-            raise ValueError(
-                f"Unknown figure type {stylename}. Must be one of PAPER, SLIDE, or POSTER"
-            )
-        # If the name is not of the form `TYPE_WIDTH_HEIGHT`, then we assume it is just a type
-        if len(nameparts) != 3:
-            figsize = None
-        # Otherwise, we assume it is of the form `TYPE_WIDTH_HEIGHT`
-        else:
-            # Extract the type, width, and height
-            wname, hname = nameparts[1:]
-            if wname.endswith("H"):
-                hname, wname = nameparts[1:]
-
-            wname = "_".join([stylename, wname])
-            hname = "_".join([stylename, hname])
-
-            # Get the width and height from the defined variables in this script
-            h = globals()[hname]
-            w = globals()[wname]
-            figsize = (w, h)
+        stylename, figsize = _get_style_and_figsize(name)
 
         # Define a new function that calls the `figure` method with the appropriate arguments
         def myfig(*args, stylename=stylename, **kwargs):
             # Update the keyword arguments with the figure size
             kws = {}
+            if figsize is not None:
+                kws.update(figsize=figsize)
+
+                if "figsize" in kwargs:
+                    raise ValueError(
+                        f"Cannot specify `figsize` in the keyword arguments when calling `{name}`"
+                    )
             kws.update(kwargs)
-            kws.update(figsize=figsize)
 
             apply_style(stylename)
 
             # Call the figure method with the updated arguments
-            return _plt.figure(*args, **kws)
+            return cls._callfun(*args, **kws)
 
         # Return the new function handle. When one calls `wedme.figure.TYPE_WIDTH_HEIGHT()`,
         # `wedme.figure.TYPE_WIDTH_HEIGHT` returns the function handle `myfig`
         return myfig
 
 
+class apply(metaclass=_metafigure):
+    def _callfun(*args, **kws):
+        if "figsize" in kws:
+            _mpl.rcParams["figure.figsize"] = kws["figsize"]
+
+
 class figure(metaclass=_metafigure):
-    pass
+    def _callfun(*args, **kws):
+        return _plt.figure(*args, **kws)
+
+
+class subplots(metaclass=_metafigure):
+    def _callfun(*args, **kws):
+        return _plt.subplots(*args, **kws)
```

### Comparing `wedme-plots-2.0.2/src/wedme/util.py` & `wedme_plots-2.0.3/src/wedme/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,25 @@
     cmap = _plt.cm.get_cmap(cmap)
     norm = _mpl.colors.Normalize(vmin=min, vmax=max)
 
     return lambda x: cmap(norm(x))
 
 
 def get_colormap_norm_for_colorbar(cmap="viridis", X=None, min=None, max=None):
+    """Generates a colormap and a scalar mappable for use in a colorbar.
+    This might be useful when plotting multiple lines with different colors based on a parameter.
+
+    Example usage:
+        cmap, scalarmappable = wedme.util.get_colormap_norm_for_colorbar("nipy_spectral", min=340, max=386)
+
+        for i, result in enumerate(myresults):
+            plt.plot(result.x, result.y, color=cmap(delay), label=f"{delay}ns")
+
+        wedme.colorbar(scalarmappable, label="Q-switch delay [ns]")
+    """
     if not X is None:
         min = _np.nanmin(_np.array(X))
         max = _np.nanmax(_np.array(X))
 
     cmap = _plt.cm.get_cmap(cmap)
     norm = _mpl.colors.Normalize(vmin=min, vmax=max)
     fun = lambda x: cmap(norm(x))
```

### Comparing `wedme-plots-2.0.2/src/wedme_plots.egg-info/PKG-INFO` & `wedme_plots-2.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wedme-plots
-Version: 2.0.2
-Summary: We Don't Make Embarrassing Plots. Matplotlib styles for papers, posters and presentations.
+Version: 2.0.3
+Summary: We Don't Make Embarrassing Plots. Matplotlib styles for papers, posters, presentations and theses.
 Author-email: Martijn Ruijzendaal <martijn.ruijzendaal@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -41,92 +41,128 @@
 Requires-Dist: twine; extra == "build"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # 👗 wedme-plots: We Don't Make Embarrassing Plots
 
-Matplotlib styles for papers, posters and presentations. Tailored for academic use.
+Matplotlib styles for papers, posters, presentations and theses. Tailored for academic use.
 
 ## Too long; didn't read
-```python
-import wedme
+1. Pick a style from `paper`, `slide`, `a0`, `thesis`.
+2. Decide the final size of the figure on the chosen medium. 
+For example, the column width (`cw`) and default height (`dh`) for the `paper` style.
+3. Import `wedme`
+4. Before using matplotlib, apply the style using `wedme.apply.[style]_[width]_[height]()`. In the above example, `wedme.apply.paper_cw_dh()`.
+
 
-# Open a figure in `paper` style, with size (PAPER_CW, PAPER_DH)
-# which equals (journal column width, default height)
-wedme.figure.paper_cw_dh()
-
-# Open a figure with the style `slide` and size (SLIDE_TW, SLIDE_HH) 
-# which equals (1/3 slide width, 1/2 slide height)
-wedme.figure.slide_tw_hh()
+## Installation
+Install from [PyPI](https://pypi.org/project/wedme-plots/) using PIP:
 ```
+pip install wedme-plots
+```
+
+For Anaconda users:
+- Open an Anaconda Prompt
+- Optional: if you use an environment other than `base`, open it using `conda activate [my environment]`
+- Install pip using `conda install pip`
+- Install wedme-plots using `pip install wedme-plots`
 
 ## Styling
-We applied a clean style. The style and sizes of `paper` style are compatible with most journals (Nature, Science, Elsevier). The `slide` style is compatible with a Microsoft Powerpoint presentation. `poster`  is compatible with A0 posters.
+Wedme offers multiple styles:
+- `paper`: compatible with most journals (Nature, Science, Elsevier). 
+- `slide`: compatible with a (16:9) Microsoft Powerpoint presentation. 
+- `a0`: A0 poster.
+- `thesis`: (work-in-progress) similar to `paper` but for the B5 page format.
 
 ## Usage
-Import the `wedme` module and apply the desired style. Then proceed with `matplotlib` plotting as you're used to.
+There are two ways of applying a wedme style. 
+
+### 1. Global styling and sizing
+
+Import the `wedme` module and apply the desired style, e.g. `wedme.apply.paper()`. 
+This applies the specified style and its default size to every subsequent figure.
 
 Example:
 ```python
 import wedme
 
 # These commands apply a style to subsequent Matplotlib figures.
 
-# For Elsevier-compatible paper styles
-wedme.paper()
-
-# For a 16:9 Powerpoint slide
-wedme.slide()
+# Pick one:
+wedme.apply.paper()  # For Elsevier-compatible paper styles
+wedme.apply.slide()  # For a 16:9 Powerpoint slide
+wedme.apply.a0()     # For A0 posters
+wedme.apply.thesis() # For B5-paper thesis
 
-# For A0 posters (not implemented yet)
-wedme.poster()
+# Optionally, change the default size:
+wedme.apply.slide_tw_hh()
 
 # Proceed with plotting as usual
-import numpy as np
 import matplotlib.pyplot as plt
 
-x = np.linspace(0, np.pi, 1000)
-
 plt.figure()
-plt.plot(x, np.sin(x), label="Sine")
-plt.plot(x, np.cos(x), label="Cosine")
+plt.plot([1, 2, 3, 4])
 plt.show()
 ```
 
-## Sizing
-For custom figure sizes, we include reference points for every style:
+### 2. Local styling and sizing
 
-- Paper. Default size: `(wedme.PAPER_CW, wedme.paper_GH)`
-  - `wedme.PAPER_FW` is the full textwidth of an Elsevier journal, 190mm.
-  - `wedme.PAPER_CW` is the full columnwidth of an Elsevier journal in two-column layout, 90mm.
-  - `wedme.PAPER_GH` is the height that has a golden ratio (1:1.618) to `wedme.PAPER_CW`.
-- Slide. Default size: `(wedme.SLIDE_TW, wedme.slide_HH)`
-  - `wedme.SLIDE_FW`, `wedme.SLIDE_HW` and `wedme.SLIDE_TW` represent 100%, 50% and 33% of the width of a Powerpoint 16:9 Widescreen slide.
-  - `wedme.SLIDE_FH`, `wedme.SLIDE_HH` and `wedme.SLIDE_TH` represent 100%, 50% and 33% of the height of a Powerpoint 16:9 Widescreen slide.
+Alternatively, one can open figures in a specified style and size using the `wedme` drop-in replacements for `plt.figure()` and `plt.subplots()` as follows:
 
-These can be used as follows:
 ```python
 import wedme
-wedme.slide()
-# Create a new figure that occupies 33% of the width of a ppt slide and 50% its height.
-plt.figure(figsize=(wedme.SLIDE_TW, wedme.SLIDE_HH))
-```
+import matplotlib.pyplot as plt
 
-Alternatively, we provide functions to compress the above code:
-```python
-wedme.figure.slide_tw_hh()
-```
-Such a function exists for every combination of heights and widths for a given style.
+# Open a figure in the `a0` style, 
+# with a size corresponding to half-width and half-height
+wedme.figure.a0_hw_hh()
+plt.plot([1, 2, 3, 4])
+
+# Open a figure with two subplots in the `slide` style,
+# with the figure size corresponding to half-width and half-height
+fig, (ax1, ax2) = wedme.subplots.slide_hw_hh(1, 2)
 
-To open a figure with one of `wedme`'s styles without applying any sizing, use e.g.
-```python
-wedme.figure.slide()
+ax1.plot([1, 2, 3, 4])
+ax2.plot([1, 2, 3, 4])
 ```
 
+Any arguments passed to `wedme.figure.[style]()` and `wedme.subplots.[style]()` are passed on to the equivalent matplotlib functions.
+
+## Sizing
+Matching the matplotlib figure size to the final display size of the figure is critically important: scaling to a different height will change font sizes and line widths.
+
+We include the following breakpoints, with respect to the available width and height (`H`) of the chosen medium:
+| Breakpoint | Ratio |
+| -- | -- |
+| `F` | 100% _("full")_ |
+| `TT` | 2/3 _("two-thirds")_ |
+| `H` | 1/2 _("half")_ |
+| `FT` | 5/12 _("five-twelfth")_ |
+| `T` | 1/3 _("third")_ |
+| `Q` | 1/4 _("quarter")_ |
+| `R` | 1/5 |
+| `S` | 1/6 |
+
+To specify the size using a breakpoint, append `W` (width) or `H` (height). For example, `wedme.figure.a0_hw_hh()` specifies the `a0` style, with a size of half the A0 width and height.
+
+In addition to the breakpoints, some styles include custom sizes:
+- `paper`: `CW` (column width) for two-column papers. `GH` is the height that corresponds to the golden-ratio of `CW`.
+- `thesis`: `LFW` and `LFH` for the landscape full-width and full-height.
+The default width and height `DW` and `DH` correspond to `CW` and `GH` of the `paper` style
+
+</br>
+
+When no size is specified, the following defaults sizes are used:
+- `paper`: `(wedme.PAPER_CW, wedme.paper_GH)`
+- `slide`: `(wedme.SLIDE_TW, wedme.slide_HH)`
+- `a0`:  `(wedme.A0_TW, ...)`
+- `thesis`: `(wedme.THESIS_DW, wedme.paper_DH)`
+
+
 ## Powerpoint
 Powerpoint automatically resizes artwork to a size that is different from the export size. To undo this:
 - Insert the figure in Powerpoint.
 - Picture Format > Reset Picture > Reset Picture & Size.
 
 ## Fonts
 Sans-serif fonts are the standards for figures because they remain readable even when small or pixelated. Helvetica or Arial fonts are preferred by Nature, Science and Elsevier. 
@@ -137,8 +173,14 @@
 `wedme` sets the `pdf.fonttype` parameter to `42` as recommended by Nature. This ensures that the text is editable even after exporting a pdf. `wedme` also changes the parameters `figure.autolayout` and `savefig.bbox` such that the specified sizes are respected.
 
 For saving figures, consider using [pypdfplot](https://github.com/dcmvdbekerom/pypdfplot) to maintain the ability to later change how data is displayed. Of course, we don't make embarassing plots to begin with.
 
 ## Examples
 <img src="https://github.com/mruijzendaal/wedme-plots/blob/main/img/calibration_curve_rot.png?raw=true" width="512">
 
-
+## Utilities
+Other than style sheets, wedme also includes utilities for commonly used operations.
+- Creating animated GIF images from multiple plots. See `wedme.gif`
+- Creating a legend only for unique entries. See `wedme.util.unique_legend()`
+- Specifying the colorbar label easily. See `wedme.util.colorbar()`
+- Specifying the minimum and maximum of the colorbar as a function of percentiles of the shown field. See `wedme.util.imshow()`
+- Making plot colors dependent on some variable. See `weme.util.get_colormap_norm()`
```

