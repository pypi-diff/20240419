# Comparing `tmp/pymc-marketing-0.4.2.tar.gz` & `tmp/pymc_marketing-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-marketing-0.4.2.tar", last modified: Fri Mar 15 20:01:02 2024, max compression
+gzip compressed data, was "pymc_marketing-0.5.0.tar", last modified: Fri Apr 19 07:39:45 2024, max compression
```

## Comparing `pymc-marketing-0.4.2.tar` & `pymc_marketing-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:01:02.037504 pymc-marketing-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-15 20:00:57.000000 pymc-marketing-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-03-15 20:01:02.037504 pymc-marketing-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-03-15 20:00:57.000000 pymc-marketing-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:01:02.033503 pymc-marketing-0.4.2/pymc_marketing/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:01:02.033503 pymc-marketing-0.4.2/pymc_marketing/clv/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13717 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:01:02.033503 pymc-marketing-0.4.2/pymc_marketing/clv/models/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/models/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/models/beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    18143 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/models/gamma_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)    40549 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/models/pareto_nbd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/models/shifted_beta_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/clv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:01:02.037504 pymc-marketing-0.4.2/pymc_marketing/mmm/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47652 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/budget_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43626 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/delayed_saturated_mmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23298 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/mmm/validating.py
--rw-r--r--   0 runner    (1001) docker     (127)    25735 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pymc_marketing/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:01:02.037504 pymc-marketing-0.4.2/pymc_marketing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-03-15 20:01:02.000000 pymc-marketing-0.4.2/pymc_marketing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-15 20:01:02.000000 pymc-marketing-0.4.2/pymc_marketing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 20:01:02.000000 pymc-marketing-0.4.2/pymc_marketing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-15 20:01:02.000000 pymc-marketing-0.4.2/pymc_marketing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-15 20:01:02.000000 pymc-marketing-0.4.2/pymc_marketing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-15 20:00:58.000000 pymc-marketing-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 20:01:02.037504 pymc-marketing-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.507607 pymc_marketing-0.5.0/pymc_marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.507607 pymc_marketing-0.5.0/pymc_marketing/clv/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.507607 pymc_marketing-0.5.0/pymc_marketing/clv/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17844 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/gamma_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40713 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/pareto_nbd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/models/shifted_beta_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22801 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/clv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/pymc_marketing/mmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47999 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/budget_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52249 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/delayed_saturated_mmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/lift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26172 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/mmm/validating.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pymc_marketing/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/pymc_marketing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 07:39:45.000000 pymc_marketing-0.5.0/pymc_marketing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-19 07:39:41.000000 pymc_marketing-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:39:45.511607 pymc_marketing-0.5.0/setup.cfg
```

### Comparing `pymc-marketing-0.4.2/LICENSE` & `pymc_marketing-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.4.2/PKG-INFO` & `pymc_marketing-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.4.2
+Version: 0.5.0
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,15 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/pymc-labs/pymc-marketing
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arviz>=0.13.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: numpy>=1.17
 Requires-Dist: pandas
 Requires-Dist: pymc>=5.10.4
@@ -254,15 +254,14 @@
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # <span style="color:limegreen">PyMC-Marketing</span>: Bayesian Marketing Mix Modeling (MMM) & Customer Lifetime Value (CLV)
 
 ## Marketing Analytics Tools from [PyMC Labs](https://www.pymc-labs.com)
 
-
 Unlock the power of **Marketing Mix Modeling (MMM)** and **Customer Lifetime Value (CLV)** analytics with PyMC-Marketing. This open-source marketing analytics tool empowers businesses to make smarter, data-driven decisions for maximizing ROI in marketing campaigns.
 
 ## Quick Installation Guide for Marketing Mix Modeling (MMM) & CLV
 
 To dive into MMM and CLV analytics, set up a specialized environment, `marketing_env`, via conda-forge:
 
 ```bash
@@ -279,19 +278,19 @@
 ## In-depth Bayesian Marketing Mix Modeling (MMM) in PyMC
 
 Leverage our Bayesian MMM API to tailor your marketing strategies effectively. Based on the research [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017)](https://research.google/pubs/pub46001/),  and integrating the expertise from core PyMC developers, our API provides:
 
 - **Adstock Transformation**: Optimize the carry-over effects in your marketing channels.
 - **Saturation Effects**: Understand the diminishing returns in media investments.
 - **Budget Optimization**: Allocate your marketing spend efficiently across various channels for maximum ROI.
-- **Experiment Calibration**: Fine-tune your model based on empirical experiments for more unified view of marketing.
+- **Experiment Calibration**: Fine-tune your model based on empirical experiments for a more unified view of marketing.
 
 Explore a hands-on [simulated example](https://pymc-marketing.readthedocs.io/en/stable/notebooks/mmm/mmm_example.html) for more insights into MMM with PyMC-Marketing.
 
-### Essential Reading for Marketing Mix Modeling (MMM):
+### Essential Reading for Marketing Mix Modeling (MMM)
 
 - [Bayesian Media Mix Modeling for Marketing Optimization](https://www.pymc-labs.com/blog-posts/bayesian-media-mix-modeling-for-marketing-optimization/)
 - [Improving the Speed and Accuracy of Bayesian Marketing Mix Models](https://www.pymc-labs.com/blog-posts/reducing-customer-acquisition-costs-how-we-helped-optimizing-hellofreshs-marketing-budget/)
 - [Johns, Michael and Wang,  Zhenyu. "A Bayesian Approach to Media Mix Modeling"](https://www.youtube.com/watch?v=UznM_-_760Y)
 - [Orduz, Juan. "Media Effect Estimation with PyMC: Adstock, Saturation & Diminishing Returns"](https://juanitorduz.github.io/pymc_mmm/)
 - [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/resource-center/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
 
@@ -314,15 +313,15 @@
 
 ---
 
 ## Why PyMC-Marketing vs other solutions?
 
 PyMC-Marketing is and will always be free for commercial use, licensed under [Apache 2.0](LICENSE). Developed by core developers behind the popular PyMC package and marketing experts, it provides state-of-the-art measurements and analytics for marketing teams.
 
-Due to its open source nature and active contributor base, new features get added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+Due to its open-source nature and active contributor base, new features are added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
 
 ## Marketing AI Assistant: MMM-GPT with PyMC-Marketing
 
 Not sure how to start or have questions? MMM-GPT is an AI that answers questions and provides expert advice on marketing analytics using PyMC-Marketing.
 
 **[Try MMM-GPT here.](https://mmm-gpt.com/)**
 
@@ -332,11 +331,11 @@
 
 Maximize your marketing ROI with a [free 30-minute strategy session](https://calendly.com/niall-oulton) with our PyMC-Marketing experts. Learn how Bayesian Marketing Mix Modeling and Customer Lifetime Value analytics can boost your organization by making smarter, data-driven decisions.
 
 For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
 
 We provide the following professional services:
 
-- **Custom Models**: We tailor niche marketing anayltics models to fit your organization's unique needs.
-- **Build Within PyMC-Marketing**: Our team are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
+- **Custom Models**: We tailor niche marketing analytics models to fit your organization's unique needs.
+- **Build Within PyMC-Marketing**: Our team members are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
 - **SLA & Coaching**: Get guaranteed support levels and personalized coaching to ensure your team is well-equipped and confident in using our tools and approaches.
 - **SaaS Solutions**: Harness the power of our state-of-the-art software solutions to streamline your data-driven marketing initiatives.
```

### Comparing `pymc-marketing-0.4.2/README.md` & `pymc_marketing-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # <span style="color:limegreen">PyMC-Marketing</span>: Bayesian Marketing Mix Modeling (MMM) & Customer Lifetime Value (CLV)
 
 ## Marketing Analytics Tools from [PyMC Labs](https://www.pymc-labs.com)
 
-
 Unlock the power of **Marketing Mix Modeling (MMM)** and **Customer Lifetime Value (CLV)** analytics with PyMC-Marketing. This open-source marketing analytics tool empowers businesses to make smarter, data-driven decisions for maximizing ROI in marketing campaigns.
 
 ## Quick Installation Guide for Marketing Mix Modeling (MMM) & CLV
 
 To dive into MMM and CLV analytics, set up a specialized environment, `marketing_env`, via conda-forge:
 
 ```bash
@@ -38,19 +37,19 @@
 ## In-depth Bayesian Marketing Mix Modeling (MMM) in PyMC
 
 Leverage our Bayesian MMM API to tailor your marketing strategies effectively. Based on the research [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017)](https://research.google/pubs/pub46001/),  and integrating the expertise from core PyMC developers, our API provides:
 
 - **Adstock Transformation**: Optimize the carry-over effects in your marketing channels.
 - **Saturation Effects**: Understand the diminishing returns in media investments.
 - **Budget Optimization**: Allocate your marketing spend efficiently across various channels for maximum ROI.
-- **Experiment Calibration**: Fine-tune your model based on empirical experiments for more unified view of marketing.
+- **Experiment Calibration**: Fine-tune your model based on empirical experiments for a more unified view of marketing.
 
 Explore a hands-on [simulated example](https://pymc-marketing.readthedocs.io/en/stable/notebooks/mmm/mmm_example.html) for more insights into MMM with PyMC-Marketing.
 
-### Essential Reading for Marketing Mix Modeling (MMM):
+### Essential Reading for Marketing Mix Modeling (MMM)
 
 - [Bayesian Media Mix Modeling for Marketing Optimization](https://www.pymc-labs.com/blog-posts/bayesian-media-mix-modeling-for-marketing-optimization/)
 - [Improving the Speed and Accuracy of Bayesian Marketing Mix Models](https://www.pymc-labs.com/blog-posts/reducing-customer-acquisition-costs-how-we-helped-optimizing-hellofreshs-marketing-budget/)
 - [Johns, Michael and Wang,  Zhenyu. "A Bayesian Approach to Media Mix Modeling"](https://www.youtube.com/watch?v=UznM_-_760Y)
 - [Orduz, Juan. "Media Effect Estimation with PyMC: Adstock, Saturation & Diminishing Returns"](https://juanitorduz.github.io/pymc_mmm/)
 - [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/resource-center/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
 
@@ -73,15 +72,15 @@
 
 ---
 
 ## Why PyMC-Marketing vs other solutions?
 
 PyMC-Marketing is and will always be free for commercial use, licensed under [Apache 2.0](LICENSE). Developed by core developers behind the popular PyMC package and marketing experts, it provides state-of-the-art measurements and analytics for marketing teams.
 
-Due to its open source nature and active contributor base, new features get added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+Due to its open-source nature and active contributor base, new features are added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
 
 ## Marketing AI Assistant: MMM-GPT with PyMC-Marketing
 
 Not sure how to start or have questions? MMM-GPT is an AI that answers questions and provides expert advice on marketing analytics using PyMC-Marketing.
 
 **[Try MMM-GPT here.](https://mmm-gpt.com/)**
 
@@ -91,11 +90,11 @@
 
 Maximize your marketing ROI with a [free 30-minute strategy session](https://calendly.com/niall-oulton) with our PyMC-Marketing experts. Learn how Bayesian Marketing Mix Modeling and Customer Lifetime Value analytics can boost your organization by making smarter, data-driven decisions.
 
 For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
 
 We provide the following professional services:
 
-- **Custom Models**: We tailor niche marketing anayltics models to fit your organization's unique needs.
-- **Build Within PyMC-Marketing**: Our team are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
+- **Custom Models**: We tailor niche marketing analytics models to fit your organization's unique needs.
+- **Build Within PyMC-Marketing**: Our team members are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
 - **SLA & Coaching**: Get guaranteed support levels and personalized coaching to ensure your team is well-equipped and confident in using our tools and approaches.
 - **SaaS Solutions**: Harness the power of our state-of-the-art software solutions to streamline your data-driven marketing initiatives.
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/__init__.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/distributions.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 
         r = np.broadcast_to(r, size)
         alpha = np.broadcast_to(alpha, size)
         s = np.broadcast_to(s, size)
         beta = np.broadcast_to(beta, size)
         T = np.broadcast_to(T, size)
 
-        output = np.zeros(shape=size + (2,))
+        output = np.zeros(shape=size + (2,))  # noqa:RUF005
 
         lam = rng.gamma(shape=r, scale=1 / alpha, size=size)
         mu = rng.gamma(shape=s, scale=1 / beta, size=size)
 
         def sim_data(lam, mu, T):
             t = 0
             n = 0
@@ -346,15 +346,17 @@
 
 
 class ParetoNBD(PositiveContinuous):
     r"""
     Population-level distribution class for a continuous, non-contractual, Pareto/NBD process,
     based on Schmittlein, et al. in [2]_.
 
-    The likelihood function is derived from equations (22) and (23) of [3]_, with terms rearranged for numerical stability.
+    The likelihood function is derived from equations (22) and (23) of [3]_, with terms
+    rearranged for numerical stability.
+
     The modified expression is provided below:
 
     .. math::
 
         \begin{align}
         \text{if }\alpha > \beta: \\
         \\
@@ -385,15 +387,15 @@
     .. [2] David C. Schmittlein, Donald G. Morrison and Richard Colombo.
            "Counting Your Customers: Who Are They and What Will They Do Next."
            Management Science,Vol. 33, No. 1 (Jan., 1987), pp. 1-24.
 
     .. [3] Fader, Peter & G. S. Hardie, Bruce (2005).
            "A Note on Deriving the Pareto/NBD Model and Related Expressions."
            http://brucehardie.com/notes/009/pareto_nbd_derivations_2005-11-05.pdf
-    """
+    """  # noqa: E501
 
     rv_op = pareto_nbd
 
     @classmethod
     def dist(cls, r, alpha, s, beta, T, **kwargs):
         return super().dist([r, alpha, s, beta, T], **kwargs)
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/models/__init__.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/models/basic.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/models/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import warnings
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Dict, Optional, Sequence, cast
+from typing import cast
 
 import arviz as az
 import pandas as pd
 import pymc as pm
 from pymc.backends import NDArray
 from pymc.backends.base import MultiTrace
 from pymc.model.core import Model
@@ -17,16 +18,16 @@
 class CLVModel(ModelBuilder):
     _model_type = "CLVModel"
 
     def __init__(
         self,
         data: pd.DataFrame,
         *,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         super().__init__(model_config, sampler_config)
         self.data = data
 
     @staticmethod
     def _validate_cols(
         data: pd.DataFrame,
@@ -52,15 +53,15 @@
     def _add_fit_data_group(self, data: pd.DataFrame) -> None:
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 category=UserWarning,
                 message="The group fit_data is not defined in the InferenceData scheme",
             )
-            assert self.idata is not None
+            assert self.idata is not None  # noqa: S101
             self.idata.add_groups(fit_data=data.to_xarray())
 
     def fit(  # type: ignore
         self,
         fit_method: str = "mcmc",
         **kwargs,
     ) -> az.InferenceData:
@@ -201,46 +202,46 @@
                 frequency=t["frequency"],
                 recency=t["recency"],
                 T=t["T"],
                 mean_transaction_value=t["monetary_value"],
             )
 
         """
-        self.fit_result  # Raise Error if fit didn't happen yet
-        assert self.idata is not None
+        self.fit_result  # noqa: B018 (Raise Error if fit didn't happen yet)
+        assert self.idata is not None  # noqa: S101
         new_idata = self.idata.isel(draw=slice(None, None, keep_every)).copy()
         return type(self)._build_with_idata(new_idata)
 
     @staticmethod
-    def _create_distribution(dist: Dict, shape=()):
+    def _create_distribution(dist: dict, shape=()):
         try:
             return getattr(pm, dist["dist"]).dist(**dist.get("kwargs", {}), shape=shape)
         except AttributeError:
             raise ValueError(f"Distribution {dist['dist']} does not exist in PyMC")
 
     @property
-    def default_sampler_config(self) -> Dict:
+    def default_sampler_config(self) -> dict:
         return {}
 
     @property
-    def _serializable_model_config(self) -> Dict:
+    def _serializable_model_config(self) -> dict:
         return self.model_config
 
     @property
     def fit_result(self) -> Dataset:
         if self.idata is None or "posterior" not in self.idata:
             raise RuntimeError("The model hasn't been fit yet, call .fit() first")
         return self.idata["posterior"]
 
     @fit_result.setter
     def fit_result(self, res: az.InferenceData) -> None:
         if self.idata is None:
             self.idata = res
         elif "posterior" in self.idata:
-            warnings.warn("Overriding pre-existing fit_result")
+            warnings.warn("Overriding pre-existing fit_result", stacklevel=1)
             self.idata.posterior = res
         else:
             self.idata.posterior = res
 
     def fit_summary(self, **kwargs):
         res = self.fit_result
         # Map fitting only gives one value, so we return it. We use arviz
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/models/beta_geo.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/models/beta_geo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional, Sequence, Union
+from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray as xr
 from pymc.distributions.dist_math import check_parameters
@@ -33,18 +33,20 @@
 
     Parameters
     ----------
     data: pd.DataFrame
         DataFrame containing the following columns:
             * `frequency`: number of repeat purchases (with possible values 0, 1, 2, ...)
             * `recency`: time between the first and the last purchase (with possible values 0, 1, 2, ...)
-            * `T`: time between the first purchase and the end of the observation period (with possible values 0, 1, 2, ...)
+            * `T`: time between the first purchase and the end of the observation
+                period (with possible values 0, 1, 2, ...)
             * `customer_id`: unique customer identifier
     model_config: dict, optional
-        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in
+        the `default_model_config` class attribute.
     sampler_config: dict, optional
         Dictionary of sampler parameters. Defaults to None.
 
     Examples
     --------
     BG/NBD model for customer
 
@@ -101,40 +103,40 @@
     ----------
     .. [1] Fader, P. S., Hardie, B. G., & Lee, K. L. (2005). “Counting your customers”
            the easy way: An alternative to the Pareto/NBD model. Marketing science,
            24(2), 275-284. http://brucehardie.com/papers/018/fader_et_al_mksc_05.pdf
     .. [2] Fader, P. S., Hardie, B. G., & Lee, K. L. (2008). Computing
            P (alive) using the BG/NBD model. Research Note available via
            http://www.brucehardie.com/notes/021/palive_for_BGNBD.pdf.
-    .. [3] Fader, P. S. & Hardie, B. G. (2013) Overcoming the BG/NBD Model’s #NUM!
+    .. [3] Fader, P. S. & Hardie, B. G. (2013) Overcoming the BG/NBD Model's #NUM!
            Error Problem. Research Note available via
            http://brucehardie.com/notes/027/bgnbd_num_error.pdf.
     """
 
     _model_type = "BG/NBD"  # Beta-Geometric Negative Binomial Distribution
 
     def __init__(
         self,
         data: pd.DataFrame,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         self._validate_cols(
             data,
             required_cols=["customer_id", "frequency", "recency", "T"],
             must_be_unique=["customer_id"],
         )
         super().__init__(
             data=data,
             model_config=model_config,
             sampler_config=sampler_config,
         )
 
     @property
-    def default_model_config(self) -> Dict[str, Dict]:
+    def default_model_config(self) -> dict[str, dict]:
         return {
             "a_prior": {"dist": "HalfFlat", "kwargs": {}},
             "b_prior": {"dist": "HalfFlat", "kwargs": {}},
             "alpha_prior": {"dist": "HalfFlat", "kwargs": {}},
             "r_prior": {"dist": "HalfFlat", "kwargs": {}},
         }
 
@@ -205,19 +207,19 @@
         r = trace["r"]
 
         return a, b, alpha, r
 
     # taken from https://lifetimes.readthedocs.io/en/latest/lifetimes.fitters.html
     def expected_num_purchases(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        t: Union[np.ndarray, pd.Series, TensorVariable],
-        frequency: Union[np.ndarray, pd.Series, TensorVariable],
-        recency: Union[np.ndarray, pd.Series, TensorVariable],
-        T: Union[np.ndarray, pd.Series, TensorVariable],
+        customer_id: np.ndarray | pd.Series,
+        t: np.ndarray | pd.Series | TensorVariable,
+        frequency: np.ndarray | pd.Series | TensorVariable,
+        recency: np.ndarray | pd.Series | TensorVariable,
+        T: np.ndarray | pd.Series | TensorVariable,
     ) -> xr.DataArray:
         r"""
         Given a purchase history/profile of :math:`x` and :math:`t_x` for an individual
         customer, this method returns the expected number of future purchases in the
         next time interval of length :math:`t`, i.e. :math:`(T, T + t]`. The closed form
         solution for this equation is available as (10) from [1] linked above. With
         :math:`\text{hyp2f1}` being the Gaussian hypergeometric function, the
@@ -267,18 +269,18 @@
 
         return (numerator / denominator).transpose(
             "chain", "draw", "customer_id", missing_dims="ignore"
         )
 
     def expected_probability_alive(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        frequency: Union[np.ndarray, pd.Series],
-        recency: Union[np.ndarray, pd.Series],
-        T: Union[np.ndarray, pd.Series],
+        customer_id: np.ndarray | pd.Series,
+        frequency: np.ndarray | pd.Series,
+        recency: np.ndarray | pd.Series,
+        T: np.ndarray | pd.Series,
     ) -> xr.DataArray:
         r"""
         Posterior expected value of the probability of being alive at time T. The
         derivation of the closed form solution is available in [2].
 
         .. math::
             P\left( \text{alive} \mid x, t_x, T, r, \alpha, a, b \right)
@@ -304,15 +306,15 @@
 
         return xr.where(frequency == 0, 1.0, expit(-log_div)).transpose(
             "chain", "draw", "customer_id", missing_dims="ignore"
         )
 
     def expected_num_purchases_new_customer(
         self,
-        t: Union[np.ndarray, pd.Series],
+        t: np.ndarray | pd.Series,
     ):
         r"""
         Posterior expected number of purchases for any interval of length :math:`t`. See
         equation (9) of [1].
 
         The customer_id shouldn't matter too much here since no individual-specific data
         is conditioned on.
@@ -339,15 +341,15 @@
 
         return (left_term * right_term).transpose(
             "chain", "draw", "t", missing_dims="ignore"
         )
 
     def _distribution_new_customers(
         self,
-        random_seed: Optional[RandomState] = None,
+        random_seed: RandomState | None = None,
         var_names: Sequence[str] = ("population_dropout", "population_purchase_rate"),
     ) -> xr.Dataset:
         with pm.Model():
             a = pm.HalfFlat("a")
             b = pm.HalfFlat("b")
             alpha = pm.HalfFlat("alpha")
             r = pm.HalfFlat("r")
@@ -366,15 +368,15 @@
                 fit_result,
                 var_names=var_names,
                 random_seed=random_seed,
             ).posterior_predictive
 
     def distribution_new_customer_dropout(
         self,
-        random_seed: Optional[RandomState] = None,
+        random_seed: RandomState | None = None,
     ) -> xr.Dataset:
         """Sample the Beta distribution for the population-level dropout rate.
 
         This is the probability that a new customer will not make another purchase ("drops out")
         immediately after any previous purchase.
 
         Parameters
@@ -390,15 +392,15 @@
         return self._distribution_new_customers(
             random_seed=random_seed,
             var_names=["population_dropout"],
         )["population_dropout"]
 
     def distribution_new_customer_purchase_rate(
         self,
-        random_seed: Optional[RandomState] = None,
+        random_seed: RandomState | None = None,
     ) -> xr.Dataset:
         """Sample the Gamma distribution for the population-level purchase rate.
 
         This is the purchase rate for a new customer and determines the time between
         purchases for any new customer.
 
         Parameters
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/models/gamma_gamma.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/models/gamma_gamma.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict, Optional, Union
-
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor.tensor as pt
 import xarray
 from pymc.util import RandomState
 from pytensor.tensor import TensorVariable
@@ -11,18 +9,18 @@
 from pymc_marketing.clv.models.basic import CLVModel
 from pymc_marketing.clv.utils import customer_lifetime_value, to_xarray
 
 
 class BaseGammaGammaModel(CLVModel):
     def distribution_customer_spend(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        mean_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        frequency: Union[np.ndarray, pd.Series, TensorVariable],
-        random_seed: Optional[RandomState] = None,
+        customer_id: np.ndarray | pd.Series,
+        mean_transaction_value: np.ndarray | pd.Series | TensorVariable,
+        frequency: np.ndarray | pd.Series | TensorVariable,
+        random_seed: RandomState | None = None,
     ) -> xarray.DataArray:
         """Posterior distribution of transaction value per customer"""
 
         x = frequency
         z_mean = mean_transaction_value
 
         coords = {"customer_id": np.unique(customer_id)}
@@ -40,32 +38,33 @@
                 self.idata,
                 var_names=["nu", "mean_spend"],
                 random_seed=random_seed,
             ).posterior_predictive["mean_spend"]
 
     def expected_customer_spend(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        mean_transaction_value: Union[np.ndarray, pd.Series],
-        frequency: Union[np.ndarray, pd.Series],
+        customer_id: np.ndarray | pd.Series,
+        mean_transaction_value: np.ndarray | pd.Series,
+        frequency: np.ndarray | pd.Series,
     ) -> xarray.DataArray:
         """Expected transaction value per customer
 
         Eq 5 from [1], p.3
 
-        Adapted from: https://github.com/CamDavidsonPilon/lifetimes/blob/aae339c5437ec31717309ba0ec394427e19753c4/lifetimes/fitters/gamma_gamma_fitter.py#L117  # noqa: E501
+        Adapted from: https://github.com/CamDavidsonPilon/lifetimes/blob/aae339c5437ec31717309ba0ec394427e19753c4/lifetimes/fitters/gamma_gamma_fitter.py#L117
         """
 
         mean_transaction_value, frequency = to_xarray(
             customer_id, mean_transaction_value, frequency
         )
-        assert self.idata is not None, "Model must be fitted first"
-        p = self.idata.posterior["p"]
-        q = self.idata.posterior["q"]
-        v = self.idata.posterior["v"]
+        posterior = self.fit_result
+
+        p = posterior["p"]
+        q = posterior["q"]
+        v = posterior["v"]
 
         individual_weight = p * frequency / (p * frequency + q - 1)
         population_mean = v * p / (q - 1)
         return (
             1 - individual_weight
         ) * population_mean + individual_weight * mean_transaction_value
 
@@ -87,35 +86,35 @@
                 var_names=["nu", "mean_spend"],
                 random_seed=random_seed,
             ).posterior_predictive["mean_spend"]
 
     def expected_new_customer_spend(self) -> xarray.DataArray:
         """Expected transaction value for a new customer"""
 
-        assert self.idata is not None, "Model must be fitted first"
-        p_mean = self.idata.posterior["p"]
-        q_mean = self.idata.posterior["q"]
-        v_mean = self.idata.posterior["v"]
+        posterior = self.fit_result
+        p_mean = posterior["p"]
+        q_mean = posterior["q"]
+        v_mean = posterior["v"]
 
         # Closed form solution to the posterior of nu
         # Eq 3 from [1], p.3
         mean_spend = p_mean * v_mean / (q_mean - 1)
         # We could also provide the variance
         # var_spend = (p_mean ** 2 * v_mean ** 2) / ((q_mean - 1) ** 2 * (q_mean - 2))
 
         return mean_spend
 
     def expected_customer_lifetime_value(
         self,
         transaction_model: CLVModel,
-        customer_id: Union[np.ndarray, pd.Series],
-        mean_transaction_value: Union[np.ndarray, pd.Series],
-        frequency: Union[np.ndarray, pd.Series],
-        recency: Union[np.ndarray, pd.Series],
-        T: Union[np.ndarray, pd.Series],
+        customer_id: np.ndarray | pd.Series,
+        mean_transaction_value: np.ndarray | pd.Series,
+        frequency: np.ndarray | pd.Series,
+        recency: np.ndarray | pd.Series,
+        T: np.ndarray | pd.Series,
         time: int = 12,
         discount_rate: float = 0.01,
         freq: str = "D",
     ) -> xarray.DataArray:
         """Expected customer lifetime value.
 
         See clv.utils.customer_lifetime_value for details on the meaning of each parameter
@@ -158,15 +157,16 @@
     ----------
     data: pd.DataFrame
         DataFrame containing the following columns:
             - customer_id: Customer labels. Must not repeat.
             - mean_transaction_value: Mean transaction value of each customer.
             - frequency: Number of transactions observed for each customer.
     model_config: dict, optional
-        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the
+        `default_model_config` class attribute.
     sampler_config: dict, optional
         Dictionary of sampler parameters. Defaults to None.
 
     Examples
     --------
         Gamma-Gamma model condioned on mean transaction value
 
@@ -221,28 +221,28 @@
     """
 
     _model_type = "Gamma-Gamma Model (Mean Transactions)"
 
     def __init__(
         self,
         data: pd.DataFrame,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         self._validate_cols(
             data,
             required_cols=["customer_id", "mean_transaction_value", "frequency"],
             must_be_unique=["customer_id"],
         )
         super().__init__(
             data=data, model_config=model_config, sampler_config=sampler_config
         )
 
     @property
-    def default_model_config(self) -> Dict:
+    def default_model_config(self) -> dict:
         return {
             "p_prior": {"dist": "HalfFlat", "kwargs": {}},
             "q_prior": {"dist": "HalfFlat", "kwargs": {}},
             "v_prior": {"dist": "HalfFlat", "kwargs": {}},
         }
 
     def build_model(self):
@@ -291,15 +291,16 @@
     ----------
     data: pd.DataFrame
         Dataframe containing the following columns:
             - customer_id: Customer labels. The same value should be used for each observation
         coming from the same customer.
             - individual_transaction_value: Value of individual transactions.
     model_config: dict, optional
-        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the
+        `default_model_config` class attribute.
     sampler_config: dict, optional
         Dictionary of sampler parameters. Defaults to None.
 
 
     Examples
     --------
 
@@ -356,26 +357,26 @@
     """
 
     _model_type = "Gamma-Gamma Model (Individual Transactions)"
 
     def __init__(
         self,
         data: pd.DataFrame,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         self._validate_cols(
             data, required_cols=["customer_id", "individual_transaction_value"]
         )
         super().__init__(
             data=data, model_config=model_config, sampler_config=sampler_config
         )
 
     @property
-    def default_model_config(self) -> Dict:
+    def default_model_config(self) -> dict:
         return {
             "p_prior": {"dist": "HalfFlat", "kwargs": {}},
             "q_prior": {"dist": "HalfFlat", "kwargs": {}},
             "v_prior": {"dist": "HalfFlat", "kwargs": {}},
         }
 
     def build_model(self):
@@ -413,17 +414,17 @@
         x = gdf["count"]
         z_mean = gdf["mean"]
 
         return customer_id, z_mean, x
 
     def distribution_customer_spend(  # type: ignore [override]
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        random_seed: Optional[RandomState] = None,
+        customer_id: np.ndarray | pd.Series,
+        individual_transaction_value: np.ndarray | pd.Series | TensorVariable,
+        random_seed: RandomState | None = None,
     ) -> xarray.DataArray:
         """Return distribution of transaction value per customer"""
 
         customer_id, z_mean, x = self._summarize_mean_data(
             customer_id, individual_transaction_value
         )
 
@@ -432,17 +433,17 @@
             mean_transaction_value=z_mean,
             frequency=x,
             random_seed=random_seed,
         )
 
     def expected_customer_spend(
         self,
-        customer_id: Union[np.ndarray, pd.Series],
-        individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        random_seed: Optional[RandomState] = None,
+        customer_id: np.ndarray | pd.Series,
+        individual_transaction_value: np.ndarray | pd.Series | TensorVariable,
+        random_seed: RandomState | None = None,
     ) -> xarray.DataArray:
         """Return expected transaction value per customer"""
 
         customer_id, z_mean, x = self._summarize_mean_data(
             customer_id, individual_transaction_value
         )
 
@@ -452,18 +453,18 @@
             frequency=x,
             random_seed=random_seed,  # type: ignore [call-arg]
         )
 
     def expected_customer_lifetime_value(  # type: ignore [override]
         self,
         transaction_model: CLVModel,
-        customer_id: Union[np.ndarray, pd.Series],
-        individual_transaction_value: Union[np.ndarray, pd.Series, TensorVariable],
-        recency: Union[np.ndarray, pd.Series],
-        T: Union[np.ndarray, pd.Series],
+        customer_id: np.ndarray | pd.Series,
+        individual_transaction_value: np.ndarray | pd.Series | TensorVariable,
+        recency: np.ndarray | pd.Series,
+        T: np.ndarray | pd.Series,
         time: int = 12,
         discount_rate: float = 0.01,
         freq: str = "D",
     ) -> xarray.DataArray:
         """Return expected customer lifetime value.
 
         See clv.utils.customer_lifetime_value for details on the meaning of each parameter
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/models/pareto_nbd.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/models/pareto_nbd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
-from typing import Any, Dict, Literal, Optional, Sequence, Union, cast
+from collections.abc import Sequence
+from typing import Any, Literal, cast
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytensor
 import pytensor.tensor as pt
 import xarray
@@ -64,15 +65,16 @@
 
     Parameters
     ----------
     data: pd.DataFrame
         DataFrame containing the following columns:
             * `frequency`: number of repeat purchases
             * `recency`: time between the first and the last purchase
-            * `T`: time between the first purchase and the end of the observation period; model assumptions require T >= recency
+            * `T`: time between the first purchase and the end of the observation period.
+                Model assumptions require T >= recency
             * `customer_id`: unique customer identifier
         Along with optional covariate columns.
 
     model_config: dict, optional
         Dictionary containing model parameters and covariate column names:
             * `r_prior`: Shape parameter of time between purchases; defaults to `Weibull(alpha=2, beta=1)`
             * `alpha_prior`: Scale parameter of time between purchases; defaults to `Weibull(alpha=2, beta=10)`
@@ -169,36 +171,41 @@
 
     _model_type = "Pareto/NBD"  # Pareto Negative-Binomial Distribution
 
     def __init__(
         self,
         data: pd.DataFrame,
         *,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         super().__init__(
             data=data,
             model_config=model_config,
             sampler_config=sampler_config,
         )
         self.purchase_covariate_cols = list(
             self.model_config["purchase_covariate_cols"]
         )
         self.dropout_covariate_cols = list(self.model_config["dropout_covariate_cols"])
         self.covariate_cols = self.purchase_covariate_cols + self.dropout_covariate_cols
         self._validate_cols(
             data,
-            required_cols=["customer_id", "frequency", "recency", "T"]
-            + self.covariate_cols,
+            required_cols=[
+                "customer_id",
+                "frequency",
+                "recency",
+                "T",
+                *self.covariate_cols,
+            ],
             must_be_unique=["customer_id"],
         )
 
     @property
-    def default_model_config(self) -> Dict[str, Any]:
+    def default_model_config(self) -> dict[str, Any]:
         return {
             "r_prior": {"dist": "Weibull", "kwargs": {"alpha": 2, "beta": 1}},
             "alpha_prior": {"dist": "Weibull", "kwargs": {"alpha": 2, "beta": 10}},
             "s_prior": {"dist": "Weibull", "kwargs": {"alpha": 2, "beta": 1}},
             "beta_prior": {"dist": "Weibull", "kwargs": {"alpha": 2, "beta": 10}},
             "purchase_coefficient_prior": {
                 "dist": "Normal",
@@ -324,15 +331,18 @@
             )
             mode = Mode(linker=mode.linker, optimizer=opt_qry)
 
         with pytensor.config.change_flags(mode=mode, on_opt_error="raise"):
             # Suppress annoying warning
             with warnings.catch_warnings():
                 warnings.filterwarnings(
-                    message="Optimization Warning: The Op hyp2f1 does not provide a C implementation. As well as being potentially slow, this also disables loop fusion.",
+                    message="""
+                    Optimization Warning: The Op hyp2f1 does not provide a C implementation.
+                    As well as being potentially slow, this also disables loop fusion.
+                    """,
                     action="ignore",
                     category=UserWarning,
                 )
                 return super().fit(fit_method, **kwargs)
 
     @staticmethod
     def _logp(
@@ -438,17 +448,17 @@
                 beta,
                 *customer_vars,
             )
         )
 
     def expected_purchases(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        future_t: Optional[Union[int, np.ndarray, pd.Series]] = None,
+        future_t: int | np.ndarray | pd.Series | None = None,
     ) -> xarray.DataArray:
         """
         Given *recency*, *frequency*, and *T* for an individual customer, this method predicts the
         expected number of future purchases across *future_t* time periods.
 
         Adapted from equation (41) In Bruce Hardie's notes [2]_, and `lifetimes` package:
         https://github.com/CamDavidsonPilon/lifetimes/blob/41e394923ad72b17b5da93e88cfabab43f51abe2/lifetimes/fitters/pareto_nbd_fitter.py#L242
@@ -456,15 +466,16 @@
         Parameters
         ----------
         data: pd.DataFrame, optional
             Dataframe containing the following columns:
                 * `customer_id`: unique customer identifier
                 * `frequency`: number of repeat purchases
                 * `recency`: time between the first and the last purchase
-                * `T`: time between the first purchase and the end of the observation period, model assumptions require T >= recency
+                * `T`: time between the first purchase and the end of the observation period.
+                    Model assumptions require T >= recency
                 * `future_t`: Number of time periods to predict expected purchases.
                 * covariates: Purchase and dropout covariate columns if original model had any.
             If not provided, the method will use the fit dataset.
         future_t: array_like, optional
             Number of time periods to predict expected purchases.
             Not needed if `data` parameter is provided with a `future_t` column.
 
@@ -511,32 +522,33 @@
 
         return exp_purchases.transpose(
             "chain", "draw", "customer_id", missing_dims="ignore"
         )
 
     def expected_probability_alive(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        future_t: Optional[Union[int, np.ndarray, pd.Series]] = None,
+        future_t: int | np.ndarray | pd.Series | None = None,
     ) -> xarray.DataArray:
         """
         Compute the probability that a customer with history *frequency*, *recency*, and *T*
         is currently active. Can also estimate alive probability for *future_t* periods into the future.
 
         Adapted from equation (18) in Bruce Hardie's notes [3]_.
 
         Parameters
         ----------
         data: pd.DataFrame, optional
             Dataframe containing the following columns:
                 * `customer_id`: unique customer identifier
                 * `frequency`: number of repeat purchases
                 * `recency`: time between the first and the last purchase
-                * `T`: time between the first purchase and the end of the observation period, model assumptions require T >= recency
+                * `T`: time between the first purchase and the end of the observation period.
+                    Model assumptions require T >= recency
                 * `future_t`: Number of time periods in the future to estimate alive probability; defaults to 0.
                 * covariates: Purchase and dropout covariate columns if original model had any.
             If not provided, the method will use the fit dataset.
         future_t: array_like, optional
             Number of time periods in the future to estimate alive probability; defaults to 0.
             Not needed if `data` parameter is provided with a `future_t` column.
 
@@ -578,18 +590,18 @@
 
         return prob_alive.transpose(
             "chain", "draw", "customer_id", missing_dims="ignore"
         )
 
     def expected_purchase_probability(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        n_purchases: Optional[int] = None,
-        future_t: Optional[Union[int, np.ndarray, pd.Series]] = None,
+        n_purchases: int | None = None,
+        future_t: int | np.ndarray | pd.Series | None = None,
     ) -> xarray.DataArray:
         """
         Estimate probability of *n_purchases* over *future_t* time periods,
         given an individual customer's current *frequency*, *recency*, and *T*.
 
 
         Adapted from equation (16) in Bruce Hardie's notes [4]_, and `lifetimes` package:
@@ -598,17 +610,19 @@
         Parameters
         ----------
         data: pd.DataFrame
             Optional dataframe containing the following columns:
                 * `customer_id`: unique customer identifier
                 * `frequency`: number of repeat purchases
                 * `recency`: time between the first and the last purchase
-                * `T`: time between the first purchase and the end of the observation period, model assumptions require T >= recency
+                * `T`: time between the first purchase and the end of the observation period.
+                    Model assumptions require T >= recency
                 * `future_t`: Number of time periods to predict expected purchases.
-                * `n_purchases`: Number of purchases to predict probability for. Currently restricted to the same number for all customers.
+                * `n_purchases`: Number of purchases to predict probability for.
+                    Currently restricted to the same number for all customers.
                 * covariates: Purchase and dropout covariate columns if original model had any.
             If not provided, the method will use the fit dataset.
         n_purchases: int, optional
             Number of purchases predicted.
             Not needed if `data` parameter is provided with a `n_purchases` column.
         future_t: array_like, optional
             Time periods over which the probability should be estimated.
@@ -752,17 +766,17 @@
 
         return purchase_prob.transpose(
             "chain", "draw", "customer_id", missing_dims="ignore"
         )
 
     def expected_purchases_new_customer(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        t: Optional[Union[int, np.ndarray, pd.Series]] = None,
+        t: int | np.ndarray | pd.Series | None = None,
     ) -> xarray.DataArray:
         """
         Expected number of purchases for a new customer across *t* time periods.
 
         In a model with covariates, if `data` is not specified, the dataset used for fitting will be used.
         A prediction will be computed for a new customer with each set of covariates.
         This is not a conditional prediction on the observed customers!
@@ -806,27 +820,28 @@
 
         return (first_term * second_term).transpose(
             "chain", "draw", "customer_id", missing_dims="ignore"
         )
 
     def distribution_new_customer(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        T: Optional[Union[int, np.ndarray, pd.Series]] = None,
-        random_seed: Optional[RandomState] = None,
+        T: int | np.ndarray | pd.Series | None = None,
+        random_seed: RandomState | None = None,
         var_names: Sequence[
             Literal["dropout", "purchase_rate", "recency_frequency"]
         ] = (
             "dropout",
             "purchase_rate",
             "recency_frequency",
         ),
     ) -> xarray.Dataset:
-        """Utility function for posterior predictive sampling of dropout, purchase rate and frequency/recency of new customers.
+        """Utility function for posterior predictive sampling of dropout, purchase rate
+        and frequency/recency of new customers.
 
         In a model with covariates, if `data` is not specified, the dataset used for fitting will be used.
         A prediction will be computed for a new customer with each set of covariates.
         This is not a conditional prediction on the observed customers!
 
         Parameters
         ----------
@@ -902,17 +917,17 @@
                 var_names=var_names,
                 random_seed=random_seed,
                 predictions=True,
             ).predictions
 
     def distribution_new_customer_dropout(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        random_seed: Optional[RandomState] = None,
+        random_seed: RandomState | None = None,
     ) -> xarray.Dataset:
         """Sample from the Gamma distribution representing dropout times for new customers.
 
         This is the duration of time a new customer is active before churning, or dropping out.
 
         Parameters
         ----------
@@ -933,17 +948,17 @@
             data=data,
             random_seed=random_seed,
             var_names=["dropout"],
         )["dropout"]
 
     def distribution_new_customer_purchase_rate(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        random_seed: Optional[RandomState] = None,
+        random_seed: RandomState | None = None,
     ) -> xarray.Dataset:
         """Sample from the Gamma distribution representing purchase rates for new customers.
 
         This is the purchase rate for a new customer and determines the time between
         purchases for any new customer.
 
         Parameters
@@ -965,18 +980,18 @@
             data=data,
             random_seed=random_seed,
             var_names=["purchase_rate"],
         )["purchase_rate"]
 
     def distribution_new_customer_recency_frequency(
         self,
-        data: Optional[pd.DataFrame] = None,
+        data: pd.DataFrame | None = None,
         *,
-        T: Optional[Union[int, np.ndarray, pd.Series]] = None,
-        random_seed: Optional[RandomState] = None,
+        T: int | np.ndarray | pd.Series | None = None,
+        random_seed: RandomState | None = None,
     ) -> xarray.Dataset:
         """Pareto/NBD process representing purchases across the customer population.
 
         This is the distribution of purchase frequencies given 'T' observation periods for each customer.
 
         Parameters
         ----------
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/models/shifted_beta_geo.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/models/shifted_beta_geo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional, Sequence, Union
+from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 from pymc.util import RandomState
 from xarray import DataArray, Dataset
 
@@ -27,15 +27,16 @@
         DataFrame containing the following columns:
             * `customer_id`: Customer labels. There should be one unique label for each customer
             * `t_churn`: Time at which the customer cancelled the contract (starting at 0).
         It should  equal T for users that have not cancelled by the end of the
         observation period
             * `T`: Maximum observed time period (starting at 0)
     model_config: dict, optional
-        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the `default_model_config` class attribute.
+        Dictionary of model prior parameters. If not provided, the model will use default priors specified in the
+        `default_model_config` class attribute.
     sampler_config: dict, optional
         Dictionary of sampler parameters. Defaults to None.
 
 
     Examples
     --------
         .. code-block:: python
@@ -85,16 +86,16 @@
     """
 
     _model_type = "Shifted-Beta-Geometric Model (Individual Customers)"
 
     def __init__(
         self,
         data: pd.DataFrame,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         self._validate_cols(
             data,
             required_cols=["customer_id", "t_churn", "T"],
             must_be_unique=["customer_id"],
         )
 
@@ -108,15 +109,15 @@
                 "Customers that are still alive should have t_churn = T",
             )
         super().__init__(
             data=data, model_config=model_config, sampler_config=sampler_config
         )
 
     @property
-    def default_model_config(self) -> Dict:
+    def default_model_config(self) -> dict:
         return {
             "alpha_prior": {"dist": "HalfFlat", "kwargs": {}},
             "beta_prior": {"dist": "HalfFlat", "kwargs": {}},
         }
 
     def build_model(self):
         alpha_prior = self._create_distribution(self.model_config["alpha_prior"])
@@ -136,15 +137,15 @@
                 lower=None,
                 upper=self.data["T"],
                 observed=self.data["t_churn"],
                 dims=("customer_id",),
             )
 
     def distribution_customer_churn_time(
-        self, customer_id: Union[np.ndarray, pd.Series], random_seed: RandomState = None
+        self, customer_id: np.ndarray | pd.Series, random_seed: RandomState = None
     ) -> DataArray:
         """Sample distribution of churn time for existing customers.
 
         The draws represent the number of periods into the future after which
         a customer cancels their contract.
 
         It ignores that some customers may have already cancelled.
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/plotting.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from typing import Optional, Sequence, Tuple
+from collections.abc import Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.lines import Line2D
 
+from pymc_marketing.clv import BetaGeoModel, ParetoNBDModel
+
 __all__ = [
     "plot_customer_exposure",
     "plot_frequency_recency_matrix",
     "plot_probability_alive_matrix",
 ]
 
 
 def plot_customer_exposure(
     df: pd.DataFrame,
-    linewidth: Optional[float] = None,
-    size: Optional[float] = None,
-    labels: Optional[Sequence[str]] = None,
-    colors: Optional[Sequence[str]] = None,
+    linewidth: float | None = None,
+    size: float | None = None,
+    labels: Sequence[str] | None = None,
+    colors: Sequence[str] | None = None,
     padding: float = 0.25,
-    ax: Optional[plt.Axes] = None,
+    ax: plt.Axes | None = None,
 ) -> plt.Axes:
     """Plot the recency and T of DataFrame of customers.
 
     Plots customers as horizontal lines with markers representing their recency and T starting.
     Order is the same as the DataFrame and plotted from the bottom up.
 
     The lines are colored by recency and T.
@@ -143,41 +145,41 @@
 
     return ax
 
 
 def _create_frequency_recency_meshes(
     max_frequency: int,
     max_recency: int,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     frequency = np.arange(max_frequency + 1)
     recency = np.arange(max_recency + 1)
     mesh_frequency, mesh_recency = np.meshgrid(frequency, recency)
 
     return mesh_frequency, mesh_recency
 
 
 def plot_frequency_recency_matrix(
-    model,
+    model: BetaGeoModel | ParetoNBDModel,
     t=1,
-    max_frequency: Optional[int] = None,
-    max_recency: Optional[int] = None,
-    title: Optional[str] = None,
+    max_frequency: int | None = None,
+    max_recency: int | None = None,
+    title: str | None = None,
     xlabel: str = "Customer's Historical Frequency",
     ylabel: str = "Customer's Recency",
-    ax: Optional[plt.Axes] = None,
+    ax: plt.Axes | None = None,
     **kwargs,
 ) -> plt.Axes:
     """
     Plot recency frequency matrix as heatmap.
     Plot a figure of expected transactions in T next units of time by a customer's frequency and recency.
 
     Parameters
     ----------
-    model: lifetimes model
-        A fitted lifetimes model.
+    model: CLV model
+        A fitted CLV model.
     t: float, optional
         Next units of time to make predictions for
     max_frequency: int, optional
         The maximum frequency to plot. Default is max observed frequency.
     max_recency: int, optional
         The maximum recency to plot. This also determines the age of the customer.
         Default to max observed age.
@@ -193,35 +195,57 @@
         Passed into the matplotlib.imshow command.
 
     Returns
     -------
     axes: matplotlib.AxesSubplot
     """
     if max_frequency is None:
-        max_frequency = int(model.frequency.max())
+        max_frequency = int(model.data["frequency"].max())
 
     if max_recency is None:
-        max_recency = int(model.recency.max())
+        max_recency = int(model.data["recency"].max())
 
     mesh_frequency, mesh_recency = _create_frequency_recency_meshes(
         max_frequency=max_frequency,
         max_recency=max_recency,
     )
 
-    Z = (
-        model.expected_num_purchases(
-            customer_id=np.arange(mesh_recency.size),  # placeholder
-            t=t,
-            frequency=mesh_frequency.ravel(),
-            recency=mesh_recency.ravel(),
-            T=max_recency,
+    # FIXME: This is a hotfix for ParetoNBDModel, as it has a different API from BetaGeoModel
+    #  We should harmonize them!
+    if isinstance(model, ParetoNBDModel):
+        transaction_data = pd.DataFrame(
+            {
+                "customer_id": np.arange(mesh_recency.size),  # placeholder
+                "frequency": mesh_frequency.ravel(),
+                "recency": mesh_recency.ravel(),
+                "T": max_recency,
+            }
         )
-        .mean(("draw", "chain"))
-        .values.reshape(mesh_recency.shape)
-    )
+
+        Z = (
+            model.expected_purchases(
+                data=transaction_data,
+                future_t=t,
+            )
+            .mean(("draw", "chain"))
+            .values.reshape(mesh_recency.shape)
+        )
+    else:
+        Z = (
+            model.expected_num_purchases(
+                customer_id=np.arange(mesh_recency.size),  # placeholder
+                frequency=mesh_frequency.ravel(),
+                recency=mesh_recency.ravel(),
+                T=max_recency,
+                t=t,
+            )
+            .mean(("draw", "chain"))
+            .values.reshape(mesh_recency.shape)
+        )
+
     if ax is None:
         ax = plt.subplot(111)
 
     pcm = ax.imshow(Z, **kwargs)
     if title is None:
         title = (
             "Expected Number of Future Purchases for {} Unit{} of Time,".format(
@@ -241,32 +265,32 @@
     # plot colorbar beside matrix
     plt.colorbar(pcm, ax=ax)
 
     return ax
 
 
 def plot_probability_alive_matrix(
-    model,
-    max_frequency: Optional[int] = None,
-    max_recency: Optional[int] = None,
+    model: BetaGeoModel | ParetoNBDModel,
+    max_frequency: int | None = None,
+    max_recency: int | None = None,
     title: str = "Probability Customer is Alive,\nby Frequency and Recency of a Customer",
     xlabel: str = "Customer's Historical Frequency",
     ylabel: str = "Customer's Recency",
-    ax: Optional[plt.Axes] = None,
+    ax: plt.Axes | None = None,
     **kwargs,
 ) -> plt.Axes:
     """
     Plot probability alive matrix as heatmap.
     Plot a figure of the probability a customer is alive based on their
     frequency and recency.
 
     Parameters
     ----------
-    model: lifetimes model
-        A fitted lifetimes model.
+    model: CLV model
+        A fitted CLV model.
     max_frequency: int, optional
         The maximum frequency to plot. Default is max observed frequency.
     max_recency: int, optional
         The maximum recency to plot. This also determines the age of the customer.
         Default to max observed age.
     title: str, optional
         Figure title
@@ -281,34 +305,54 @@
 
     Returns
     -------
     axes: matplotlib.AxesSubplot
     """
 
     if max_frequency is None:
-        max_frequency = int(model.frequency.max())
+        max_frequency = int(model.data["frequency"].max())
 
     if max_recency is None:
-        max_recency = int(model.recency.max())
+        max_recency = int(model.data["recency"].max())
 
     mesh_frequency, mesh_recency = _create_frequency_recency_meshes(
         max_frequency=max_frequency,
         max_recency=max_recency,
     )
+    # FIXME: This is a hotfix for ParetoNBDModel, as it has a different API from BetaGeoModel
+    #  We should harmonize them!
+    if isinstance(model, ParetoNBDModel):
+        transaction_data = pd.DataFrame(
+            {
+                "customer_id": np.arange(mesh_recency.size),  # placeholder
+                "frequency": mesh_frequency.ravel(),
+                "recency": mesh_recency.ravel(),
+                "T": max_recency,
+            }
+        )
 
-    Z = (
-        model.expected_probability_alive(
-            customer_id=np.arange(mesh_recency.size),  # placeholder
-            frequency=mesh_frequency.ravel(),
-            recency=mesh_recency.ravel(),
-            T=max_recency,
+        Z = (
+            model.expected_probability_alive(
+                data=transaction_data,
+                future_t=0,  # TODO: This can be a function parameter in the case of ParetoNBDModel
+            )
+            .mean(("draw", "chain"))
+            .values.reshape(mesh_recency.shape)
+        )
+    else:
+        Z = (
+            model.expected_probability_alive(
+                customer_id=np.arange(mesh_recency.size),  # placeholder
+                frequency=mesh_frequency.ravel(),
+                recency=mesh_recency.ravel(),
+                T=max_recency,  # type: ignore
+            )
+            .mean(("draw", "chain"))
+            .values.reshape(mesh_recency.shape)
         )
-        .mean(("draw", "chain"))
-        .values.reshape(mesh_recency.shape)
-    )
 
     interpolation = kwargs.pop("interpolation", "none")
 
     if ax is None:
         ax = plt.subplot(111)
 
     pcm = ax.imshow(Z, interpolation=interpolation, **kwargs)
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/clv/utils.py` & `pymc_marketing-0.5.0/pymc_marketing/clv/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import warnings
-from datetime import datetime
-from typing import Optional, Union
+from datetime import date, datetime
 
 import numpy as np
 import pandas as pd
 import xarray
+from numpy import datetime64
 
-__all__ = ["to_xarray", "customer_lifetime_value", "rfm_summary"]
+__all__ = [
+    "to_xarray",
+    "customer_lifetime_value",
+    "rfm_summary",
+    "rfm_train_test_split",
+]
 
 
 def to_xarray(customer_id, *arrays, dim: str = "customer_id"):
     """Convert vector arrays to xarray with a common dim (default "customer_id")."""
     dims = (dim,)
     coords = {dim: np.asarray(customer_id)}
 
@@ -19,19 +24,19 @@
     )
 
     return res[0] if len(arrays) == 1 else res
 
 
 def customer_lifetime_value(
     transaction_model,
-    customer_id: Union[pd.Series, np.ndarray],
-    frequency: Union[pd.Series, np.ndarray],
-    recency: Union[pd.Series, np.ndarray],
-    T: Union[pd.Series, np.ndarray],
-    monetary_value: Union[pd.Series, np.ndarray, xarray.DataArray],
+    customer_id: pd.Series | np.ndarray,
+    frequency: pd.Series | np.ndarray,
+    recency: pd.Series | np.ndarray,
+    T: pd.Series | np.ndarray,
+    monetary_value: pd.Series | np.ndarray | xarray.DataArray,
     time: int = 12,
     discount_rate: float = 0.01,
     freq: str = "D",
 ) -> xarray.DataArray:
     """
     Compute the average lifetime value for a group of one or more customers.
     This method computes the average lifetime value for a group of one or more customers.
@@ -157,19 +162,19 @@
     return clv.transpose("chain", "draw", "customer_id")
 
 
 def _find_first_transactions(
     transactions: pd.DataFrame,
     customer_id_col: str,
     datetime_col: str,
-    monetary_value_col: Optional[str] = None,
-    datetime_format: Optional[str] = None,
-    observation_period_end: Optional[Union[str, pd.Period, datetime]] = None,
+    monetary_value_col: str | None = None,
+    datetime_format: str | None = None,
+    observation_period_end: str | pd.Period | datetime | None = None,
     time_unit: str = "D",
-    sort_transactions: Optional[bool] = True,
+    sort_transactions: bool | None = True,
 ) -> pd.DataFrame:
     """
     Return dataframe with first transactions.
 
     This takes a DataFrame of transaction data of the form:
         customer_id, datetime [, monetary_value]
     and appends a column named 'repeated' to the transaction log which indicates which rows
@@ -253,37 +258,37 @@
         .head(1)
         .index
     )
     # flag first transactions as True
     period_transactions.loc[first_transactions, "first"] = True
     select_columns.append("first")
     # reset datetime_col to period
-    period_transactions.loc[:, datetime_col] = period_transactions[
-        datetime_col
-    ].dt.to_period(time_unit)
+    period_transactions[datetime_col] = period_transactions[datetime_col].dt.to_period(
+        time_unit
+    )
 
     return period_transactions[select_columns]
 
 
 def clv_summary(*args, **kwargs):
-    warnings.warn("clv_summary was renamed to rfm_summary", UserWarning)
+    warnings.warn("clv_summary was renamed to rfm_summary", UserWarning, stacklevel=1)
     return rfm_summary(*args, **kwargs)
 
 
 def rfm_summary(
     transactions: pd.DataFrame,
     customer_id_col: str,
     datetime_col: str,
-    monetary_value_col: Optional[str] = None,
-    datetime_format: Optional[str] = None,
-    observation_period_end: Optional[Union[str, pd.Period, datetime]] = None,
+    monetary_value_col: str | None = None,
+    datetime_format: str | None = None,
+    observation_period_end: str | pd.Period | datetime | None = None,
     time_unit: str = "D",
-    time_scaler: Optional[float] = 1,
-    include_first_transaction: Optional[bool] = False,
-    sort_transactions: Optional[bool] = True,
+    time_scaler: float | None = 1,
+    include_first_transaction: bool | None = False,
+    sort_transactions: bool | None = True,
 ) -> pd.DataFrame:
     """
     Summarize transaction data for use in CLV modeling and/or RFM segmentation.
 
     This transforms a DataFrame of transaction data of the form:
         customer_id, datetime [, monetary_value]
     to a DataFrame of the form:
@@ -406,7 +411,176 @@
 
     summary_df = customers[summary_columns].astype(float)
     summary_df = summary_df.reset_index().rename(
         columns={customer_id_col: "customer_id"}
     )
 
     return summary_df
+
+
+def rfm_train_test_split(
+    transactions: pd.DataFrame,
+    customer_id_col: str,
+    datetime_col: str,
+    train_period_end: float | str | datetime | datetime64 | date,
+    test_period_end: float | str | datetime | datetime64 | date | None = None,
+    time_unit: str = "D",
+    time_scaler: float | None = 1,
+    datetime_format: str | None = None,
+    monetary_value_col: str | None = None,
+    include_first_transaction: bool | None = False,
+    sort_transactions: bool | None = True,
+) -> pd.DataFrame:
+    """
+    Summarize transaction data and split into training and tests datasets for CLV modeling.
+    This can also be used to evaluate the impact of a time-based intervention like a marketing campaign.
+
+    This transforms a DataFrame of transaction data of the form:
+        customer_id, datetime [, monetary_value]
+    to a DataFrame of the form:
+        customer_id, frequency, recency, T [, monetary_value], test_frequency [, test_monetary_value], test_T
+
+    Note this function will exclude new customers whose first transactions occurred during the test period.
+
+    Adapted from lifetimes package
+    https://github.com/CamDavidsonPilon/lifetimes/blob/41e394923ad72b17b5da93e88cfabab43f51abe2/lifetimes/utils.py#L27
+
+    Parameters
+    ----------
+    transactions: :obj: DataFrame
+        A Pandas DataFrame that contains the customer_id col and the datetime col.
+    customer_id_col: string
+        Column in the transactions DataFrame that denotes the customer_id.
+    datetime_col:  string
+        Column in the transactions DataFrame that denotes the datetime the purchase was made.
+    train_period_end: Union[str, pd.Period, datetime], optional
+        A string or datetime to denote the final time period for the training data.
+        Events after this time period are used for the test data.
+    test_period_end: Union[str, pd.Period, datetime], optional
+        A string or datetime to denote the final time period of the study.
+        Events after this date are truncated. If not given, defaults to the max of 'datetime_col'.
+    time_unit: string, optional
+        Time granularity for study.
+        Default: 'D' for days. Possible values listed here:
+        https://numpy.org/devdocs/reference/arrays.datetime.html#datetime-units
+    time_scaler: int, optional
+        Default: 1. Useful for scaling recency & T to a different time granularity. Example:
+        With freq='D' and freq_multiplier=1, we get recency=591 and T=632
+        With freq='h' and freq_multiplier=24, we get recency=590.125 and T=631.375
+        This is useful if predictions in months or years are desired,
+        and can also help with model convergence for study periods of many years.
+    datetime_format: string, optional
+        A string that represents the timestamp format. Useful if Pandas can't understand
+        the provided format.
+    monetary_value_col: string, optional
+        Column in the transactions DataFrame that denotes the monetary value of the transaction.
+        Optional; only needed for spend estimation models like the Gamma-Gamma model.
+    include_first_transaction: bool, optional
+        Default: False
+        For predictive CLV modeling, this should be False.
+        Set to True if performing RFM segmentation.
+    sort_transactions: bool, optional
+        Default: True
+        If raw data is already sorted in chronological order, set to `False` to improve computational efficiency.
+
+    Returns
+    -------
+    :obj: DataFrame:
+        customer_id, frequency, recency, T, test_frequency, test_T [, monetary_value, test_monetary_value]
+    """
+
+    if test_period_end is None:
+        test_period_end = transactions[datetime_col].max()
+
+    transaction_cols = [customer_id_col, datetime_col]
+    if monetary_value_col:
+        transaction_cols.append(monetary_value_col)
+    transactions = transactions[transaction_cols].copy()
+
+    transactions[datetime_col] = pd.to_datetime(
+        transactions[datetime_col], format=datetime_format
+    )
+    test_period_end = pd.to_datetime(test_period_end, format=datetime_format)
+    train_period_end = pd.to_datetime(train_period_end, format=datetime_format)
+
+    # create training dataset
+    training_transactions = transactions.loc[
+        transactions[datetime_col] <= train_period_end
+    ]
+
+    if training_transactions.empty:
+        error_msg = """No data available. Check `test_transactions` and `train_period_end`
+        and confirm values in `transactions` occur prior to those time periods."""
+        raise ValueError(error_msg)
+
+    training_rfm_data = rfm_summary(
+        training_transactions,
+        customer_id_col,
+        datetime_col,
+        monetary_value_col=monetary_value_col,
+        datetime_format=datetime_format,
+        observation_period_end=train_period_end,
+        time_unit=time_unit,
+        time_scaler=time_scaler,
+        include_first_transaction=include_first_transaction,
+        sort_transactions=sort_transactions,
+    )
+
+    # create test dataset
+    test_transactions = transactions.loc[
+        (test_period_end >= transactions[datetime_col])
+        & (transactions[datetime_col] > train_period_end)
+    ].copy()
+
+    if test_transactions.empty:
+        error_msg = """No data available. Check `test_transactions` and `train_period_end`
+        and confirm values in `transactions` occur prior to those time periods."""
+        raise ValueError(error_msg)
+
+    test_transactions[datetime_col] = test_transactions[datetime_col].dt.to_period(
+        time_unit
+    )
+    # create dataframe with customer_id and test_frequency columns
+    test_rfm_data = (
+        test_transactions.groupby([customer_id_col, datetime_col], sort=False)[
+            datetime_col
+        ]
+        .agg(lambda r: 1)
+        .groupby(level=customer_id_col)
+        .count()
+    ).reset_index()
+
+    test_rfm_data = test_rfm_data.rename(
+        columns={"id": "customer_id", "date": "test_frequency"}
+    )
+
+    if monetary_value_col:
+        test_monetary_value = (
+            test_transactions.groupby([customer_id_col, datetime_col])[
+                monetary_value_col
+            ]
+            .sum()
+            .groupby(customer_id_col)
+            .mean()
+        )
+
+        test_rfm_data = test_rfm_data.merge(
+            test_monetary_value,
+            left_on="customer_id",
+            right_on=customer_id_col,
+            how="inner",
+        )
+        test_rfm_data = test_rfm_data.rename(
+            columns={monetary_value_col: "test_monetary_value"}
+        )
+
+    train_test_rfm_data = training_rfm_data.merge(
+        test_rfm_data, on="customer_id", how="left"
+    )
+    train_test_rfm_data.fillna(0, inplace=True)
+
+    time_delta = (
+        test_period_end.to_period(time_unit) - train_period_end.to_period(time_unit)
+    ).n
+    train_test_rfm_data["test_T"] = time_delta / time_scaler  # type: ignore
+
+    return train_test_rfm_data
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/__init__.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/base.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+"""Base class for Marketing Mix Models (MMM)."""
+
 import warnings
+from collections.abc import Callable
 from inspect import (
     getattr_static,
     isdatadescriptor,
     isgetsetdescriptor,
     ismemberdescriptor,
     ismethoddescriptor,
 )
 from itertools import repeat
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any
 
 import arviz as az
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mtick
 import numpy as np
 import pandas as pd
 import pymc as pm
 import seaborn as sns
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import FunctionTransformer
 from xarray import DataArray, Dataset
 
 from pymc_marketing.mmm.budget_optimizer import budget_allocator
+from pymc_marketing.mmm.transformers import michaelis_menten
 from pymc_marketing.mmm.utils import (
     estimate_menten_parameters,
     estimate_sigmoid_parameters,
-    extense_sigmoid,
     find_sigmoid_inflection_point,
-    michaelis_menten,
+    sigmoid_saturation,
     standardize_scenarios_dict_keys,
 )
 from pymc_marketing.mmm.validating import (
     ValidateChannelColumns,
     ValidateDateColumn,
     ValidateTargetColumn,
 )
@@ -43,30 +46,30 @@
     model: pm.Model
     _model_type = "BaseMMM"
     version = "0.0.2"
 
     def __init__(
         self,
         date_column: str,
-        channel_columns: Union[List[str], Tuple[str]],
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        channel_columns: list[str] | tuple[str],
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
         **kwargs,
     ) -> None:
-        self.X: Optional[pd.DataFrame] = None
-        self.y: Optional[Union[pd.Series, np.ndarray]] = None
+        self.X: pd.DataFrame | None = None
+        self.y: pd.Series | np.ndarray | None = None
         self.date_column: str = date_column
-        self.channel_columns: Union[List[str], Tuple[str]] = channel_columns
+        self.channel_columns: list[str] | tuple[str] = channel_columns
         self.n_channel: int = len(channel_columns)
-        self._fit_result: Optional[az.InferenceData] = None
-        self._posterior_predictive: Optional[az.InferenceData] = None
+        self._fit_result: az.InferenceData | None = None
+        self._posterior_predictive: az.InferenceData | None = None
         super().__init__(model_config=model_config, sampler_config=sampler_config)
 
     @property
-    def methods(self) -> List[Any]:
+    def methods(self) -> list[Any]:
         maybe_methods = [getattr_static(self, attr) for attr in dir(self)]
         return [
             method
             for method in maybe_methods
             if callable(method)
             and not (
                 ismethoddescriptor(method)
@@ -75,29 +78,31 @@
                 or ismemberdescriptor(method)
             )
         ]
 
     @property
     def validation_methods(
         self,
-    ) -> Tuple[
-        List[Callable[["BaseMMM", Union[pd.DataFrame, pd.Series, np.ndarray]], None]],
-        List[Callable[["BaseMMM", Union[pd.DataFrame, pd.Series, np.ndarray]], None]],
+    ) -> tuple[
+        list[Callable[["BaseMMM", pd.DataFrame | pd.Series | np.ndarray], None]],
+        list[Callable[["BaseMMM", pd.DataFrame | pd.Series | np.ndarray], None]],
     ]:
         """
         A property that provides validation methods for features ("X") and the target variable ("y").
 
         This property scans the methods of the object and returns those marked for validation.
-        The methods are marked by having a _tags dictionary attribute, with either "validation_X" or "validation_y" set to True.
-        The "validation_X" tag indicates a method used for validating features, and "validation_y" indicates a method used for validating the target variable.
+        The methods are marked by having a _tags dictionary attribute,with either "validation_X" or "validation_y"
+        set to True. The "validation_X" tag indicates a method used for validating features, and "validation_y"
+        indicates a method used for validating the target variable.
 
         Returns
         -------
         tuple of list of Callable[["BaseMMM", pd.DataFrame], None]
-            A tuple where the first element is a list of methods for "X" validation, and the second element is a list of methods for "y" validation.
+            A tuple where the first element is a list of methods for "X" validation, and the second element is
+            a list of methods for "y" validation.
 
         """
         return (
             [
                 method
                 for method in self.methods
                 if getattr(method, "_tags", {}).get("validation_X", False)
@@ -106,15 +111,15 @@
                 method
                 for method in self.methods
                 if getattr(method, "_tags", {}).get("validation_y", False)
             ],
         )
 
     def validate(
-        self, target: str, data: Union[pd.DataFrame, pd.Series, np.ndarray]
+        self, target: str, data: pd.DataFrame | pd.Series | np.ndarray
     ) -> None:
         """
         Validates the input data based on the specified target type.
 
         This function loops over the validation methods specified for
         the target type and applies them to the input data.
 
@@ -140,39 +145,41 @@
 
         for method in validation_methods:
             method(self, data)
 
     @property
     def preprocessing_methods(
         self,
-    ) -> Tuple[
-        List[
+    ) -> tuple[
+        list[
             Callable[
-                ["BaseMMM", Union[pd.DataFrame, pd.Series, np.ndarray]],
-                Union[pd.DataFrame, pd.Series, np.ndarray],
+                ["BaseMMM", pd.DataFrame | pd.Series | np.ndarray],
+                pd.DataFrame | pd.Series | np.ndarray,
             ]
         ],
-        List[
+        list[
             Callable[
-                ["BaseMMM", Union[pd.DataFrame, pd.Series, np.ndarray]],
-                Union[pd.DataFrame, pd.Series, np.ndarray],
+                ["BaseMMM", pd.DataFrame | pd.Series | np.ndarray],
+                pd.DataFrame | pd.Series | np.ndarray,
             ]
         ],
     ]:
         """
         A property that provides preprocessing methods for features ("X") and the target variable ("y").
 
         This property scans the methods of the object and returns those marked for preprocessing.
-        The methods are marked by having a _tags dictionary attribute, with either "preprocessing_X" or "preprocessing_y" set to True.
-        The "preprocessing_X" tag indicates a method used for preprocessing features, and "preprocessing_y" indicates a method used for preprocessing the target variable.
+        The methods are marked by having a _tags dictionary attribute, with either "preprocessing_X"
+        or "preprocessing_y" set to True. The "preprocessing_X" tag indicates a method used for preprocessing
+        features, and "preprocessing_y" indicates a method used for preprocessing the target variable.
 
         Returns
         -------
         tuple of list of Callable[["BaseMMM", pd.DataFrame], pd.DataFrame]
-            A tuple where the first element is a list of methods for "X" preprocessing, and the second element is a list of methods for "y" preprocessing.
+            A tuple where the first element is a list of methods for "X" preprocessing, and the second element is a
+            list of methods for "y" preprocessing.
         """
         return (
             [
                 method
                 for method in self.methods
                 if getattr(method, "_tags", {}).get("preprocessing_X", False)
             ],
@@ -180,21 +187,22 @@
                 method
                 for method in self.methods
                 if getattr(method, "_tags", {}).get("preprocessing_y", False)
             ],
         )
 
     def preprocess(
-        self, target: str, data: Union[pd.DataFrame, pd.Series, np.ndarray]
-    ) -> Union[pd.DataFrame, pd.Series, np.ndarray]:
+        self, target: str, data: pd.DataFrame | pd.Series | np.ndarray
+    ) -> pd.DataFrame | pd.Series | np.ndarray:
         """
         Preprocess the provided data according to the specified target.
 
-        This method applies preprocessing methods to the data ("X" or "y"), which are specified in the preprocessing_methods property of this object.
-        It iteratively applies each method in the appropriate list (either for "X" or "y") to the data.
+        This method applies preprocessing methods to the data ("X" or "y"), which are specified in the
+        preprocessing_methods property of this object. It iteratively applies each method in the appropriate
+        list (either for "X" or "y") to the data.
 
         Parameters
         ----------
         target : str
             Indicates whether the data represents features ("X") or the target variable ("y").
 
         data : Union[pd.DataFrame, pd.Series, np.ndarray]
@@ -380,14 +388,15 @@
         contribution_vars = [
             az.hdi(channel_contributions, hdi_prob=0.94).channel_contributions
         ]
 
         for arg, var_contribution in zip(
             ["control_columns", "yearly_seasonality"],
             ["control_contributions", "fourier_contributions"],
+            strict=True,
         ):
             if getattr(self, arg, None):
                 contributions = self._format_model_contributions(
                     var_contribution=var_contribution
                 )
                 means.append(contributions.mean(["chain", "draw"]))
                 contribution_vars.append(
@@ -401,14 +410,15 @@
                 means,
                 contribution_vars,
                 [
                     "channel_contribution",
                     "control_contribution",
                     "fourier_contribution",
                 ],
+                strict=False,
             )
         ):
             if self.X is not None:
                 ax.fill_between(
                     x=self.X[self.date_column],
                     y1=hdi.isel(hdi=0),
                     y2=hdi.isel(hdi=1),
@@ -492,28 +502,30 @@
             ),
             dims=channel_contribution.dims,
             coords=channel_contribution.coords,
         )
 
     def _estimate_budget_contribution_fit(
         self, channel: str, budget: float, method: str = "sigmoid"
-    ) -> Tuple:
+    ) -> tuple:
         """
         Estimate the lower and upper bounds of the contribution fit for a given channel and budget.
         This function computes the quantiles (0.05 & 0.95) of the channel contributions, estimates
         the parameters of the fit function based on the specified method (either 'sigmoid' or 'michaelis-menten'),
         and calculates the lower and upper bounds of the contribution fit.
 
         The function is used in the `plot_budget_scenearios` function to estimate the contribution fit for each channel
-        and budget scenario. The estimated fit is then used to plot the contribution optimization bounds for each scenario.
+        and budget scenario. The estimated fit is then used to plot the contribution optimization bounds
+        for each scenario.
 
         Parameters
         ----------
         method : str
-            The method used to fit the contribution & spent non-linear relationship. It can be either 'sigmoid' or 'michaelis-menten'.
+            The method used to fit the contribution & spent non-linear relationship.
+            It can be either 'sigmoid' or 'michaelis-menten'.
         channel : str
             The name of the channel for which the contribution fit is being estimated.
         budget : float
             The budget for the channel.
 
         Returns
         -------
@@ -530,15 +542,15 @@
                 q=[0.05, 0.95], dim=["chain", "draw"]
             )
         )
 
         # Estimate parameters based on the method
         if method == "sigmoid":
             estimate_function = estimate_sigmoid_parameters
-            fit_function = extense_sigmoid
+            fit_function = sigmoid_saturation
         elif method == "michaelis-menten":
             estimate_function = estimate_menten_parameters
             fit_function = michaelis_menten
         else:
             raise ValueError("`method` must be either 'michaelis-menten' or 'sigmoid'.")
 
         alpha_limit_upper, lam_constant_upper = estimate_function(
@@ -569,27 +581,30 @@
         Plot a single scenario (bar-plot) on a given axes.
 
         Parameters
         ----------
         ax : matplotlib.axes.Axes
             The axes on which to plot the scenario.
         data : dict
-            Dictionary containing the data for the scenario. Keys are the names of the channels and values are the corresponding values.
+            Dictionary containing the data for the scenario.
+            Keys are the names of the channels and values are the corresponding values.
         label : str
             Label for the scenario.
         color : str
             Color to use for the bars in the plot.
         offset : float
             Offset to apply to the positions of the bars in the plot.
         bar_width: float
             Bar width.
         upper_bound : dict, optional
-            Dictionary containing the upper bounds for the data. Keys should match those in the `data` dictionary. Only used if `contribution` is True.
+            Dictionary containing the upper bounds for the data. Keys should match those in the `data` dictionary.
+            Only used if `contribution` is True.
         lower_bound : dict, optional
-            Dictionary containing the lower bounds for the data. Keys should match those in the `data` dictionary. Only used if `contribution` is True.
+            Dictionary containing the lower bounds for the data. Keys should match those in the `data` dictionary.
+            Only used if `contribution` is True.
         contribution : bool, optional
             If True, plot the upper and lower bounds for the data. Default is False.
 
         Returns
         -------
         None
             The function adds a plot to the provided axes object in-place and doesn't return any object.
@@ -620,15 +635,15 @@
                 height=bar_width,
                 label=label,
                 color=color,
                 alpha=0.85,
             )
 
     def plot_budget_scenearios(
-        self, *, base_data: Dict, method: str = "sigmoid", **kwargs
+        self, *, base_data: dict, method: str = "sigmoid", **kwargs
     ) -> plt.Figure:
         """
         Experimental: Plots the budget and contribution bars side by side for multiple scenarios.
 
         Parameters
         ----------
         base_data : dict
@@ -648,15 +663,15 @@
         scenarios_data = kwargs.get("scenarios_data", [])
         for scenario in scenarios_data:
             standardize_scenarios_dict_keys(scenario, ["contribution", "budget"])
 
         standardize_scenarios_dict_keys(base_data, ["contribution", "budget"])
 
         fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(15, 6))
-        scenarios = [base_data] + list(scenarios_data)
+        scenarios = [base_data, *list(scenarios_data)]
         num_scenarios = len(scenarios)
         bar_width = (
             0.8 / num_scenarios
         )  # bar width calculated based on the number of scenarios
         num_channels = len(base_data["contribution"]) - 1
 
         # Generate upper_bound and lower_bound dictionaries for each scenario
@@ -671,15 +686,15 @@
                     upper_bound[channel] = y_fit_upper
                     lower_bound[channel] = y_fit_lower
             upper_bounds.append(upper_bound)
             lower_bounds.append(lower_bound)
 
         # Plot all scenarios
         for i, (scenario, upper_bound, lower_bound) in enumerate(
-            zip(scenarios, upper_bounds, lower_bounds)
+            zip(scenarios, upper_bounds, lower_bounds, strict=False)
         ):
             color = f"C{i}"
             offset = i * bar_width - 0.4 + bar_width / 2
             label = f"Scenario {i+1}" if i else "Initial"
             self._plot_scenario(
                 axes[0], scenario["budget"], label, color, offset, bar_width
             )
@@ -725,31 +740,34 @@
         xlim_max: int,
         method: str = "sigmoid",
         label: str = "Fit Curve",
     ) -> None:
         """
         Plot the curve fit for the given channel based on the estimation of the parameters.
 
-        The function computes the mean channel contributions, estimates the parameters based on the specified method (either 'sigmoid' or 'michaelis-menten'), and plots
-        the curve fit. An inflection point on the curve is also highlighted.
+        The function computes the mean channel contributions, estimates the parameters based on the specified method
+        (either 'sigmoid' or 'michaelis-menten'), and plots the curve fit. An inflection point on the curve is
+        also highlighted.
 
         Parameters
         ----------
         x : np.ndarray
-            The x-axis data, usually representing the amount of input (e.g., substrate concentration in enzymology terms).
+            The x-axis data, usually representing the amount of
+            input (e.g., substrate concentration in enzymology terms).
         ax : plt.Axes
             The matplotlib axes object where the plot should be drawn.
         channel : str
             The name of the channel for which the curve fit is being plotted.
         color_index : int
             An index used for color selection to ensure distinct colors for multiple plots.
         xlim_max: int
             The maximum value to be plot on the X-axis
         method: str
-            The method used to fit the contribution & spent non-linear relationship. It can be either 'sigmoid' or 'michaelis-menten'.
+            The method used to fit the contribution & spent non-linear relationship.
+            It can be either 'sigmoid' or 'michaelis-menten'.
 
         Returns
         -------
         None
             The function modifies the given axes object in-place and doesn't return any object.
         """
         channel_contributions = self.compute_channel_contribution_original_scale().mean(
@@ -782,15 +800,15 @@
                 original_dataframe=self.X,
                 contributions=channel_contributions_quantiles.sel(quantile=0.05),
             )
 
             x_inflection, y_inflection = find_sigmoid_inflection_point(
                 alpha=alpha_limit, lam=lam_constant
             )
-            fit_function = extense_sigmoid
+            fit_function = sigmoid_saturation
         elif method == "michaelis-menten":
             alpha_limit, lam_constant = estimate_menten_parameters(
                 channel=channel,
                 original_dataframe=self.X,
                 contributions=channel_contributions,
             )
             alpha_limit_upper, lam_constant_upper = estimate_menten_parameters(
@@ -844,31 +862,34 @@
         ax.set(xlabel="Spent", ylabel="Contribution")
         ax.legend()
 
     def optimize_channel_budget_for_maximum_contribution(
         self,
         method: str,
         total_budget: int,
-        budget_bounds: Optional[Dict[str, Tuple[float, float]]] = None,
+        budget_bounds: dict[str, tuple[float, float]] | None = None,
         *,
-        parameters: Dict[str, Tuple[float, float]],
+        parameters: dict[str, tuple[float, float]],
     ) -> pd.DataFrame:
         """
-        Experimental: Optimize the allocation of a given total budget across multiple channels to maximize the expected contribution.
+        Experimental: Optimize the allocation of a given total budget across multiple
+        channels to maximize the expected contribution.
 
         The optimization is based on the method provided, where each channel's contribution
         follows a saturating function of its allocated budget. The function seeks the budget allocation
-        that maximizes the total expected contribution across all channels. The method can be either 'sigmoid' or 'michaelis-menten'.
+        that maximizes the total expected contribution across all channels.
+        The method can be either 'sigmoid' or 'michaelis-menten'.
 
         Parameters
         ----------
         total_budget : int, required
             The total budget to be distributed across channels.
         method : str, required
-            The method used to fit the contribution & spent non-linear relationship. It can be either 'sigmoid' or 'michaelis-menten'.
+            The method used to fit the contribution & spent non-linear relationship.
+            It can be either 'sigmoid' or 'michaelis-menten'.
         parameters : Dict, required
             A dictionary where keys are channel names and values are tuples (L, k) representing the
             parameters for each channel based on the method used.
         budget_bounds : Dict, optional
             An optional dictionary defining the minimum and maximum budget for each channel.
             If not provided, the budget for each channel is constrained between 0 and its L value.
 
@@ -878,59 +899,65 @@
             A pandas DataFrame containing the allocated budget and contribution information.
 
         Raises
         ------
         ValueError
             If any of the required parameters are not provided or have an incorrect type.
         """
-        if not isinstance(budget_bounds, (dict, type(None))):
+        if not isinstance(budget_bounds, dict | type(None)):
             raise TypeError("`budget_ranges` should be a dictionary or None.")
 
-        if not isinstance(total_budget, (int, float)):
+        if not isinstance(total_budget, int | float):
             raise ValueError(
                 "The 'total_budget' parameter must be an integer or float."
             )
 
         if not parameters:
             raise ValueError(
                 "The 'parameters' argument (keyword-only) must be provided and non-empty."
             )
 
-        warnings.warn("This budget allocator method is experimental", UserWarning)
+        warnings.warn(
+            "This budget allocator method is experimental", UserWarning, stacklevel=1
+        )
 
         return budget_allocator(
             method=method,
             total_budget=total_budget,
             channels=list(self.channel_columns),
             parameters=parameters,
             budget_ranges=budget_bounds,
         )
 
     def compute_channel_curve_optimization_parameters_original_scale(
         self, method: str = "sigmoid"
-    ) -> Dict:
+    ) -> dict:
         """
         Experimental: Estimate the parameters for the saturating function of each channel's contribution.
 
-        The function estimates the parameters (alpha, constant) for each channel based on the specified method (either 'sigmoid' or 'michaelis-menten').
-        These parameters represent the maximum possible contribution (alpha) and the constant parameter which vary their definition based on the function (constant) for each channel.
+        The function estimates the parameters (alpha, constant) for each channel based on the specified method
+        (either 'sigmoid' or 'michaelis-menten'). These parameters represent the maximum possible contribution (alpha)
+        and the constant parameter which vary their definition based on the function (constant) for each channel.
 
         Parameters
         ----------
         method : str, required
-            The method used to fit the contribution & spent non-linear relationship. It can be either 'sigmoid' or 'michaelis-menten'.
+            The method used to fit the contribution & spent non-linear relationship.
+            It can be either 'sigmoid' or 'michaelis-menten'.
 
         Returns
         -------
         Dict
             A dictionary where keys are channel names and values are tuples (L, k) representing the
             parameters for each channel based on the method used.
         """
         warnings.warn(
-            "The curve optimization parameters method is experimental", UserWarning
+            "The curve optimization parameters method is experimental",
+            UserWarning,
+            stacklevel=1,
         )
 
         channel_contributions = self.compute_channel_contribution_original_scale().mean(
             ["chain", "draw"]
         )
 
         if method == "michaelis-menten":
@@ -946,30 +973,31 @@
         }
 
     def plot_direct_contribution_curves(
         self,
         show_fit: bool = False,
         xlim_max=None,
         method: str = "sigmoid",
-        channels: Optional[List[str]] = None,
+        channels: list[str] | None = None,
         same_axes: bool = False,
     ) -> plt.Figure:
         """
         Plots the direct contribution curves for each marketing channel. The term "direct" refers to the fact
         we plot costs vs immediate returns and we do not take into account the lagged
         effects of the channels e.g. adstock transformations.
 
         Parameters
         ----------
         show_fit : bool, optional
             If True, the function will also plot the curve fit based on the specified method. Defaults to False.
         xlim_max : int, optional
             The maximum value to be plot on the X-axis. If not provided, the maximum value in the data will be used.
         method : str, optional
-            The method used to fit the contribution & spent non-linear relationship. It can be either 'sigmoid' or 'michaelis-menten'. Defaults to 'sigmoid'.
+            The method used to fit the contribution & spent non-linear relationship.
+            It can be either 'sigmoid' or 'michaelis-menten'. Defaults to 'sigmoid'.
         channels : List[str], optional
             A list of channels to plot. If not provided, all channels will be plotted.
         same_axes : bool, optional
             If True, all channels will be plotted on the same axes. Defaults to False.
 
         Returns
         -------
@@ -1018,15 +1046,15 @@
             figsize=figsize,
             layout="constrained",
         )
 
         axes_channels = (
             zip(repeat(axes), channels_to_plot)
             if same_axes
-            else zip(np.ravel(axes), channels_to_plot)
+            else zip(np.ravel(axes), channels_to_plot, strict=False)
         )
 
         for i, (ax, channel) in enumerate(axes_channels):
             if self.X is not None:
                 x = self.X[channels_to_plot].to_numpy()[:, i]
                 y = channel_contributions.sel(channel=channel).to_numpy()
 
@@ -1054,15 +1082,15 @@
                 )
 
                 ax.set(xlabel="Spent", ylabel="Contribution")
 
         fig.suptitle("Direct response curves", fontsize=16)
         return fig
 
-    def _get_distribution(self, dist: Dict) -> Callable:
+    def _get_distribution(self, dist: dict) -> Callable:
         """
         Retrieve a PyMC distribution callable based on the provided dictionary.
 
         Parameters
         ----------
         dist : Dict
             A dictionary containing the key 'dist' which should correspond to the
@@ -1179,17 +1207,17 @@
                     lambda x: f"channel_{x}" if isinstance(x, int) else x
                 )
             )
         return all_contributions_over_time
 
     def plot_grouped_contribution_breakdown_over_time(
         self,
-        stack_groups: Optional[Dict[str, List[str]]] = None,
+        stack_groups: dict[str, list[str]] | None = None,
         original_scale: bool = False,
-        area_kwargs: Optional[Dict[str, Any]] = None,
+        area_kwargs: dict[str, Any] | None = None,
         **plt_kwargs: Any,
     ) -> plt.Figure:
         """Plot a time series area chart for all channel contributions.
 
         Since a chart like this can become quite crowded if you have many channels or
         control variables, you can group certain variables together using the
         `stack_groups` keyword.
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/budget_optimizer.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/budget_optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# optimization_utils.py
-from typing import Dict, List, Optional, Tuple
+"""Budget optimization module."""
 
 import numpy as np
 from pandas import DataFrame
 from scipy.optimize import minimize
 
-from pymc_marketing.mmm.utils import extense_sigmoid, michaelis_menten
+from pymc_marketing.mmm.transformers import michaelis_menten
+from pymc_marketing.mmm.utils import sigmoid_saturation
 
 
 def calculate_expected_contribution(
     method: str,
-    parameters: Dict[str, Tuple[float, float]],
-    budget: Dict[str, float],
-) -> Dict[str, float]:
+    parameters: dict[str, tuple[float, float]],
+    budget: dict[str, float],
+) -> dict[str, float]:
     """
     Calculate expected contributions using the specified model.
 
     This function calculates the expected contributions for each channel
     based on the chosen model. The selected model can be either the Michaelis-Menten
     model or the sigmoid model, each described by specific parameters.
     As the allocated budget varies, the expected contribution is computed according
@@ -55,31 +55,31 @@
     for channel, channe_budget in budget.items():
         if method == "michaelis-menten":
             L, k = parameters[channel]
             contributions[channel] = michaelis_menten(channe_budget, L, k)
 
         elif method == "sigmoid":
             alpha, lam = parameters[channel]
-            contributions[channel] = extense_sigmoid(channe_budget, alpha, lam)
+            contributions[channel] = sigmoid_saturation(channe_budget, alpha, lam)
 
         else:
             raise ValueError("`method` must be either 'michaelis-menten' or 'sigmoid'.")
 
         total_expected_contribution += contributions[channel]
 
     contributions["total"] = total_expected_contribution
 
     return contributions
 
 
 def objective_distribution(
-    x: List[float],
+    x: list[float],
     method: str,
-    channels: List[str],
-    parameters: Dict[str, Tuple[float, float]],
+    channels: list[str],
+    parameters: dict[str, tuple[float, float]],
 ) -> float:
     """
     Compute the total contribution for a given budget distribution.
 
     This function calculates the negative sum of contributions for a proposed budget
     distribution using the Michaelis-Menten model. This value will be minimized in
     the optimization process to maximize the total expected contribution.
@@ -97,36 +97,36 @@
     -------
     float
         Negative of the total expected contribution for the given budget distribution.
     """
 
     sum_contributions = 0.0
 
-    for channel, budget in zip(channels, x):
+    for channel, budget in zip(channels, x, strict=False):
         if method == "michaelis-menten":
             L, k = parameters[channel]
             sum_contributions += michaelis_menten(budget, L, k)
 
         elif method == "sigmoid":
             alpha, lam = parameters[channel]
-            sum_contributions += extense_sigmoid(budget, alpha, lam)
+            sum_contributions += sigmoid_saturation(budget, alpha, lam)
 
         else:
             raise ValueError("`method` must be either 'michaelis-menten' or 'sigmoid'.")
 
     return -1 * sum_contributions
 
 
 def optimize_budget_distribution(
     method: str,
     total_budget: int,
-    budget_ranges: Optional[Dict[str, Tuple[float, float]]],
-    parameters: Dict[str, Tuple[float, float]],
-    channels: List[str],
-) -> Dict[str, float]:
+    budget_ranges: dict[str, tuple[float, float]] | None,
+    parameters: dict[str, tuple[float, float]],
+    channels: list[str],
+) -> dict[str, float]:
     """
     Optimize the budget allocation across channels to maximize total contribution.
 
     Using the Michaelis-Menten or Sigmoid function, this function seeks the best budget distribution across
     channels that maximizes the total expected contribution.
 
     This function leverages the Sequential Least Squares Quadratic Programming (SLSQP) optimization
@@ -155,15 +155,15 @@
     Returns
     -------
     Dict
         A dictionary with channels as keys and the optimal budget for each channel as values.
     """
 
     # Check if budget_ranges is the correct type
-    if not isinstance(budget_ranges, (dict, type(None))):
+    if not isinstance(budget_ranges, dict | type(None)):
         raise TypeError("`budget_ranges` should be a dictionary or None.")
 
     if budget_ranges is None:
         budget_ranges = {
             channel: (0, min(total_budget, parameters[channel][0]))
             for channel in channels
         }
@@ -178,23 +178,25 @@
         lambda x: objective_distribution(x, method, channels, parameters),
         initial_guess,
         method="SLSQP",
         bounds=bounds,
         constraints=constraints,
     )
 
-    return {channel: budget for channel, budget in zip(channels, result.x)}
+    return {
+        channel: budget for channel, budget in zip(channels, result.x, strict=False)
+    }
 
 
 def budget_allocator(
     method: str,
     total_budget: int,
-    channels: List[str],
-    parameters: Dict[str, Tuple[float, float]],
-    budget_ranges: Optional[Dict[str, Tuple[float, float]]],
+    channels: list[str],
+    parameters: dict[str, tuple[float, float]],
+    budget_ranges: dict[str, tuple[float, float]] | None,
 ) -> DataFrame:
     optimal_budget = optimize_budget_distribution(
         method=method,
         total_budget=total_budget,
         budget_ranges=budget_ranges,
         parameters=parameters,
         channels=channels,
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/delayed_saturated_mmm.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/delayed_saturated_mmm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,85 @@
+"""Media Mix Model with delayed adstock and logistic saturation class."""
+
 import json
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any
 
 import arviz as az
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pymc as pm
 import seaborn as sns
 from pytensor.tensor import TensorVariable
 from xarray import DataArray, Dataset
 
 from pymc_marketing.mmm.base import MMM
+from pymc_marketing.mmm.lift_test import (
+    add_logistic_empirical_lift_measurements_to_likelihood,
+    scale_lift_measurements,
+)
 from pymc_marketing.mmm.preprocessing import MaxAbsScaleChannels, MaxAbsScaleTarget
 from pymc_marketing.mmm.transformers import geometric_adstock, logistic_saturation
 from pymc_marketing.mmm.utils import (
     apply_sklearn_transformer_across_dim,
     create_new_spend_data,
     generate_fourier_modes,
 )
 from pymc_marketing.mmm.validating import ValidateControlColumns
 
 __all__ = ["DelayedSaturatedMMM"]
 
 
 class BaseDelayedSaturatedMMM(MMM):
+    """Base class for a media mix model with delayed adstock and logistic saturation class (see [1]_).
+
+    References
+    ----------
+    .. [1] Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017).
+    """
+
     _model_type = "DelayedSaturatedMMM"
     version = "0.0.2"
 
     def __init__(
         self,
         date_column: str,
-        channel_columns: List[str],
+        channel_columns: list[str],
         adstock_max_lag: int,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
         validate_data: bool = True,
-        control_columns: Optional[List[str]] = None,
-        yearly_seasonality: Optional[int] = None,
+        control_columns: list[str] | None = None,
+        yearly_seasonality: int | None = None,
         **kwargs,
     ) -> None:
-        """Media Mix Model with delayed adstock and logistic saturation class (see [1]_).
+        """Constructor method.
 
         Parameters
         ----------
         date_column : str
             Column name of the date variable.
         channel_columns : List[str]
             Column names of the media channel variables.
         model_config : Dictionary, optional
-            dictionary of parameters that initialise model configuration. Class-default defined by the user default_model_config method.
+            dictionary of parameters that initialise model configuration.
+            Class-default defined by the user default_model_config method.
         sampler_config : Dictionary, optional
-            dictionary of parameters that initialise sampler configuration. Class-default defined by the user default_sampler_config method.
+            dictionary of parameters that initialise sampler configuration.
+            Class-default defined by the user default_sampler_config method.
         validate_data : bool, optional
             Whether to validate the data before fitting to model, by default True.
         control_columns : Optional[List[str]], optional
             Column names of control variables to be added as additional regressors, by default None
         adstock_max_lag : int, optional
             Number of lags to consider in the adstock transformation, by default 4
         yearly_seasonality : Optional[int], optional
             Number of Fourier modes to model yearly seasonality, by default None.
-
-        References
-        ----------
-        .. [1] Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017).
         """
         self.control_columns = control_columns
         self.adstock_max_lag = adstock_max_lag
         self.yearly_seasonality = yearly_seasonality
         self.date_column = date_column
         self.validate_data = validate_data
 
@@ -77,88 +88,88 @@
             channel_columns=channel_columns,
             model_config=model_config,
             sampler_config=sampler_config,
             adstock_max_lag=adstock_max_lag,
         )
 
     @property
-    def default_sampler_config(self) -> Dict:
+    def default_sampler_config(self) -> dict:
         return {}
 
     @property
     def output_var(self):
         """Defines target variable for the model"""
         return "y"
 
     def _generate_and_preprocess_model_data(  # type: ignore
-        self, X: Union[pd.DataFrame, pd.Series], y: Union[pd.Series, np.ndarray]
+        self, X: pd.DataFrame | pd.Series, y: pd.Series | np.ndarray
     ) -> None:
-        """
-        Applies preprocessing to the data before fitting the model.
-        if validate is True, it will check if the data is valid for the model.
+        """Applies preprocessing to the data before fitting the model.
+
+        If validate is True, it will check if the data is valid for the model.
         sets self.model_coords based on provided dataset
 
         Parameters
         ----------
         X : Union[pd.DataFrame, pd.Series], shape (n_obs, n_features)
         y : Union[pd.Series, np.ndarray], shape (n_obs,)
         """
         date_data = X[self.date_column]
         channel_data = X[self.channel_columns]
 
-        self.coords_mutable: Dict[str, Any] = {
+        self.coords_mutable: dict[str, Any] = {
             "date": date_data,
         }
-        coords: Dict[str, Any] = {
+        coords: dict[str, Any] = {
             "channel": self.channel_columns,
         }
 
         new_X_dict = {
             self.date_column: date_data,
         }
         X_data = pd.DataFrame.from_dict(new_X_dict)
         X_data = pd.concat([X_data, channel_data], axis=1)
-        control_data: Optional[Union[pd.DataFrame, pd.Series]] = None
+        control_data: pd.DataFrame | pd.Series | None = None
         if self.control_columns is not None:
             control_data = X[self.control_columns]
             coords["control"] = self.control_columns
             X_data = pd.concat([X_data, control_data], axis=1)
 
-        fourier_features: Optional[pd.DataFrame] = None
+        fourier_features: pd.DataFrame | None = None
         if self.yearly_seasonality is not None:
             fourier_features = self._get_fourier_models_data(X=X)
             self.fourier_columns = fourier_features.columns
             coords["fourier_mode"] = fourier_features.columns.to_numpy()
             X_data = pd.concat([X_data, fourier_features], axis=1)
 
         self.model_coords = coords
         if self.validate_data:
             self.validate("X", X_data)
             self.validate("y", y)
-        self.preprocessed_data: Dict[str, Union[pd.DataFrame, pd.Series]] = {
+        self.preprocessed_data: dict[str, pd.DataFrame | pd.Series] = {
             "X": self.preprocess("X", X_data),  # type: ignore
             "y": self.preprocess("y", y),  # type: ignore
         }
         self.X: pd.DataFrame = X_data
-        self.y: Union[pd.Series, np.ndarray] = y
+        self.y: pd.Series | np.ndarray = y
 
     def _save_input_params(self, idata) -> None:
         """Saves input parameters to the attrs of idata."""
         idata.attrs["date_column"] = json.dumps(self.date_column)
         idata.attrs["control_columns"] = json.dumps(self.control_columns)
         idata.attrs["channel_columns"] = json.dumps(self.channel_columns)
         idata.attrs["adstock_max_lag"] = json.dumps(self.adstock_max_lag)
         idata.attrs["validate_data"] = json.dumps(self.validate_data)
         idata.attrs["yearly_seasonality"] = json.dumps(self.yearly_seasonality)
 
     def _create_likelihood_distribution(
         self,
-        dist: Dict,
+        dist: dict,
         mu: TensorVariable,
-        observed: Union[np.ndarray, pd.Series],
+        observed: np.ndarray | pd.Series,
         dims: str,
     ) -> TensorVariable:
         """
         Create and return a likelihood distribution for the model.
 
         This method prepares the distribution and its parameters as specified in the
         configuration dictionary, validates them, and constructs the likelihood
@@ -197,15 +208,18 @@
             "Gamma",
             "AsymmetricLaplace",
             "VonMises",
         ]
 
         if dist["dist"] not in allowed_distributions:
             raise ValueError(
-                f"The distribution used for the likelihood is not allowed. Please, use one of the following distributions: {allowed_distributions}."
+                f"""
+                The distribution used for the likelihood is not allowed.
+                Please, use one of the following distributions: {allowed_distributions}.
+                """
             )
 
         # Validate that 'kwargs' is present and is a dictionary
         if "kwargs" not in dist or not isinstance(dist["kwargs"], dict):
             raise ValueError(
                 "The 'kwargs' key must be present in the 'dist' dictionary and be a dictionary itself."
             )
@@ -224,20 +238,23 @@
                     raise ValueError(
                         f"The parameter configuration for '{param}' must contain 'kwargs'."
                     )
 
                 parameter_distributions[param] = self._get_distribution(
                     dist=param_config
                 )(**param_config["kwargs"], name=f"likelihood_{param}")
-            elif isinstance(param_config, (int, float)):
+            elif isinstance(param_config, int | float):
                 # Use the value directly
                 parameter_distributions[param] = param_config
             else:
                 raise ValueError(
-                    f"Invalid parameter configuration for '{param}'. It must be either a dictionary with a 'dist' key or a numeric value."
+                    f"""
+                    Invalid parameter configuration for '{param}'.
+                    It must be either a dictionary with a 'dist' key or a numeric value.
+                    """
                 )
 
         # Extract the likelihood distribution name and instantiate it
         likelihood_dist_name = dist["dist"]
         likelihood_dist = self._get_distribution(dist={"dist": likelihood_dist_name})
 
         return likelihood_dist(
@@ -247,15 +264,15 @@
             dims=dims,
             **parameter_distributions,
         )
 
     def build_model(
         self,
         X: pd.DataFrame,
-        y: Union[pd.Series, np.ndarray],
+        y: pd.Series | np.ndarray,
         **kwargs,
     ) -> None:
         """
         Builds a probabilistic model using PyMC for marketing mix modeling.
 
         The model incorporates channels, control variables, and Fourier components, applying
         adstock and saturation transformations to the channel data. The final model is
@@ -377,14 +394,15 @@
             channel_contributions = pm.Deterministic(
                 name="channel_contributions",
                 var=channel_adstock_saturated * beta_channel,
                 dims=("date", "channel"),
             )
 
             mu_var = intercept + channel_contributions.sum(axis=-1)
+
             if (
                 self.control_columns is not None
                 and len(self.control_columns) > 0
                 and all(
                     column in self.preprocessed_data["X"].columns
                     for column in self.control_columns
                 )
@@ -404,14 +422,15 @@
                 control_contributions = pm.Deterministic(
                     name="control_contributions",
                     var=control_data_ * gamma_control,
                     dims=("date", "control"),
                 )
 
                 mu_var += control_contributions.sum(axis=-1)
+
             if (
                 hasattr(self, "fourier_columns")
                 and self.fourier_columns is not None
                 and len(self.fourier_columns) > 0
                 and all(
                     column in self.preprocessed_data["X"].columns
                     for column in self.fourier_columns
@@ -443,15 +462,15 @@
                 dist=self.model_config["likelihood"],
                 mu=mu,
                 observed=target_,
                 dims="date",
             )
 
     @property
-    def default_model_config(self) -> Dict:
+    def default_model_config(self) -> dict:
         return {
             "intercept": {"dist": "Normal", "kwargs": {"mu": 0, "sigma": 2}},
             "beta_channel": {"dist": "HalfNormal", "kwargs": {"sigma": 2}},
             "alpha": {"dist": "Beta", "kwargs": {"alpha": 1, "beta": 3}},
             "lam": {"dist": "Gamma", "kwargs": {"alpha": 3, "beta": 1}},
             "likelihood": {
                 "dist": "Normal",
@@ -481,18 +500,20 @@
             n_order=self.yearly_seasonality,
         )
 
     def channel_contributions_forward_pass(
         self, channel_data: npt.NDArray[np.float_]
     ) -> npt.NDArray[np.float_]:
         """Evaluate the channel contribution for a given channel data and a fitted model, ie. the forward pass.
+
         Parameters
         ----------
         channel_data : array-like
             Input channel data. Result of all the preprocessing steps.
+
         Returns
         -------
         array-like
             Transformed channel data.
         """
         alpha_posterior = self.fit_result["alpha"].to_numpy()
 
@@ -519,16 +540,16 @@
 
         channel_contribution_forward_pass = (
             beta_channel_posterior_expanded * logistic_saturation_posterior
         )
         return channel_contribution_forward_pass.eval()
 
     @property
-    def _serializable_model_config(self) -> Dict[str, Any]:
-        def ndarray_to_list(d: Dict) -> Dict:
+    def _serializable_model_config(self) -> dict[str, Any]:
+        def ndarray_to_list(d: dict) -> dict:
             new_d = d.copy()  # Copy the dictionary to avoid mutating the original one
             for key, value in new_d.items():
                 if isinstance(value, np.ndarray):
                     new_d[key] = value.tolist()
                 elif isinstance(value, dict):
                     new_d[key] = ndarray_to_list(value)
             return new_d
@@ -576,24 +597,24 @@
         model.idata = idata
         dataset = idata.fit_data.to_dataframe()
         X = dataset.drop(columns=[model.output_var])
         y = dataset[model.output_var].values
         model.build_model(X, y)
         # All previously used data is in idata.
         if model.id != idata.attrs["id"]:
-            raise ValueError(
-                f"The file '{fname}' does not contain an inference data of the same model or configuration as '{cls._model_type}'"
-            )
+            error_msg = f"""The file '{fname}' does not contain an inference data of the same model
+        or configuration as '{cls._model_type}'"""
+            raise ValueError(error_msg)
 
         return model
 
     def _data_setter(
         self,
-        X: Union[np.ndarray, pd.DataFrame],
-        y: Optional[Union[np.ndarray, pd.Series]] = None,
+        X: np.ndarray | pd.DataFrame,
+        y: np.ndarray | pd.Series | None = None,
     ) -> None:
         """
         Sets new data in the model.
 
         This function accepts data in various formats and sets them into the
         model using the PyMC's `set_data` method. The data corresponds to the
         channel data and the target.
@@ -621,32 +642,32 @@
         -------
         None
         """
         if not isinstance(X, pd.DataFrame):
             msg = "X must be a pandas DataFrame in order to access the columns"
             raise TypeError(msg)
 
-        new_channel_data: Optional[np.ndarray] = None
+        new_channel_data: np.ndarray | None = None
         coords = {"date": X[self.date_column].to_numpy()}
 
         try:
             new_channel_data = X[self.channel_columns].to_numpy()
         except KeyError as e:
-            raise RuntimeError("New data must contain channel_data!", e)
+            raise RuntimeError("New data must contain channel_data!") from e
 
         def identity(x):
             return x
 
         channel_transformation = (
             identity
             if not hasattr(self, "channel_transformer")
             else self.channel_transformer.transform
         )
 
-        data: Dict[str, Union[np.ndarray, Any]] = {
+        data: dict[str, np.ndarray | Any] = {
             "channel_data": channel_transformation(new_channel_data)
         }
         if self.control_columns is not None:
             control_data = X[self.control_columns].to_numpy()
             control_transformation = (
                 identity
                 if not hasattr(self, "control_transformer")
@@ -670,21 +691,22 @@
             dtype = self.preprocessed_data["y"].dtype  # type: ignore
             data["target"] = np.zeros(X.shape[0], dtype=dtype)  # type: ignore
 
         with self.model:
             pm.set_data(data, coords=coords)
 
     @classmethod
-    def _model_config_formatting(cls, model_config: Dict) -> Dict:
+    def _model_config_formatting(cls, model_config: dict) -> dict:
         """
-        Because of json serialization, model_config values that were originally tuples or numpy are being encoded as lists.
-        This function converts them back to tuples and numpy arrays to ensure correct id encoding.
+        Because of json serialization, model_config values that were originally tuples
+        or numpy are being encoded as lists. This function converts them back to tuples
+        and numpy arrays to ensure correct id encoding.
         """
 
-        def format_nested_dict(d: Dict) -> Dict:
+        def format_nested_dict(d: dict) -> dict:
             for key, value in d.items():
                 if isinstance(value, dict):
                     d[key] = format_nested_dict(value)
                 elif isinstance(value, list):
                     # Check if the key is "dims" to convert it to tuple
                     if key == "dims":
                         d[key] = tuple(value)
@@ -698,21 +720,139 @@
 
 class DelayedSaturatedMMM(
     MaxAbsScaleTarget,
     MaxAbsScaleChannels,
     ValidateControlColumns,
     BaseDelayedSaturatedMMM,
 ):
-    ...
+    """Media Mix Model with delayed adstock and logistic saturation class (see [1]_).
+
+    Given a time series target variable :math:`y_{t}` (e.g. sales on conversions), media variables
+    :math:`x_{m, t}` (e.g. impressions, clicks or costs) and a set of control covariates :math:`z_{c, t}` (e.g. holidays, special events)
+    we consider a Bayesian linear model of the form:
+
+    .. math::
+        y_{t} = \\alpha + \\sum_{m=1}^{M}\\beta_{m}f(x_{m, t}) +  \\sum_{c=1}^{C}\\gamma_{c}z_{c, t} + \\varepsilon_{t},
+
+    where :math:`\\alpha` is the intercept, :math:`f` is a media transformation function and :math:`\\varepsilon_{t}` is the error therm
+    which we assume is normally distributed. The function :math:`f` encodes the contribution of media on the target variable.
+    Typically we consider two types of transformation: adstock (carry-over) and saturation effects.
+
+    Notes
+    -----
+    Here are some important notes about the model:
+
+    1. Before fitting the model, we scale the target variable and the media channels using the maximum absolute value of each variable.
+    This enable us to have a more stable model and better convergence. If control variables are present, we do not scale them!
+    If needed please do it before passing the data to the model.
+
+    2. We allow to add yearly seasonality controls as Fourier modes.
+    You can use the `yearly_seasonality` parameter to specify the number of Fourier modes to include.
+
+    3. This class also allow us to calibrate the model using:
+
+        * Custom priors for the parameters via the `model_config` parameter. You can also set the likelihood distribution.
+
+        * Adding lift tests to the likelihood function via the :meth:`add_lift_test_measurements <pymc_marketing.mmm.delayed_saturated_mmm.DelayedSaturatedMMM.add_lift_test_measurements>` method.
+
+    For details on a vanilla implementation in PyMC, see [2]_.
+
+    Examples
+    --------
+    Here is an example of how to instantiate the model with the default configuration:
+
+    .. code-block:: python
+
+        import numpy as np
+        import pandas as pd
+
+        from pymc_marketing.mmm import DelayedSaturatedMMM
+
+        data_url = "https://raw.githubusercontent.com/pymc-labs/pymc-marketing/main/data/mmm_example.csv"
+        data = pd.read_csv(data_url, parse_dates=["date_week"])
+
+        mmm = DelayedSaturatedMMM(
+            date_column="date_week",
+            channel_columns=["x1", "x2"],
+            control_columns=[
+                "event_1",
+                "event_2",
+                "t",
+            ],
+            adstock_max_lag=8,
+            yearly_seasonality=2,
+        )
+
+    Now we can fit the model with the data:
+
+    .. code-block:: python
+
+        # Set features and target
+        X = data.drop("y", axis=1)
+        y = data["y"]
+
+        # Fit the model
+        idata = mmm.fit(X, y)
+
+    We can also define custom priors for the model:
+
+    .. code-block:: python
+
+        my_model_config = {
+            "beta_channel": {
+                "dist": "LogNormal",
+                "kwargs": {"mu": np.array([2, 1]), "sigma": 1},
+            },
+            "likelihood": {
+                "dist": "Normal",
+                "kwargs": {"sigma": {"dist": "HalfNormal", "kwargs": {"sigma": 2}}},
+            },
+        }
+
+        mmm = DelayedSaturatedMMM(
+            model_config=my_model_config,
+            date_column="date_week",
+            channel_columns=["x1", "x2"],
+            control_columns=[
+                "event_1",
+                "event_2",
+                "t",
+            ],
+            adstock_max_lag=8,
+            yearly_seasonality=2,
+        )
+
+    As you can see, we can configure all prior and likelihood distributions via the `model_config`.
+
+    The `fit` method accepts keyword arguments that are passed to the PyMC sampling method.
+    For example, to change the number of samples and chains, and using a JAX implementation of NUTS we can do:
+
+    .. code-block:: python
+
+        sampler_kwargs = {
+            "draws": 2_000,
+            "target_accept": 0.9,
+            "chains": 5,
+            "random_seed": 42,
+        }
+
+        idata = mmm.fit(X, y, nuts_sampler="numpyro", **sampler_kwargs)
+
+    References
+    ----------
+    .. [1] Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017).
+    .. [2] Orduz, J. `"Media Effect Estimation with PyMC: Adstock, Saturation & Diminishing Returns" <https://juanitorduz.github.io/pymc_mmm/>`_.
+    """  # noqa: E501
 
     def channel_contributions_forward_pass(
         self, channel_data: npt.NDArray[np.float_]
     ) -> npt.NDArray[np.float_]:
         """Evaluate the channel contribution for a given channel data and a fitted model, ie. the forward pass.
         We return the contribution in the original scale of the target variable.
+
         Parameters
         ----------
         channel_data : array-like
             Input channel data. Result of all the preprocessing steps.
         Returns
         -------
         array-like
@@ -727,15 +867,16 @@
             signature="(m, n) -> (m, n)",
         )
         return target_transformed_vectorized(channel_contribution_forward_pass)
 
     def get_channel_contributions_forward_pass_grid(
         self, start: float, stop: float, num: int
     ) -> DataArray:
-        """Generate a grid of scaled channel contributions for a given grid of share values.
+        """Generate a grid of scaled channel contributions for a given grid of shared values.
+
         Parameters
         ----------
         start : float
             Start of the grid. It must be equal or greater than 0.
         stop : float
             End of the grid. It must be greater than start.
         num : int
@@ -774,25 +915,27 @@
         start: float,
         stop: float,
         num: int,
         absolute_xrange: bool = False,
         **plt_kwargs: Any,
     ) -> plt.Figure:
         """Plots a grid of scaled channel contributions for a given grid of share values.
+
         Parameters
         ----------
         start : float
             Start of the grid. It must be equal or greater than 0.
         stop : float
             End of the grid. It must be greater than start.
         num : int
             Number of points in the grid.
         absolute_xrange : bool, optional
             If True, the x-axis is in absolute values (input units), otherwise it is in
             relative percentage values, by default False.
+
         Returns
         -------
         plt.Figure
             Plot of grid of channel contributions.
         """
         share_grid = np.linspace(start=start, stop=stop, num=num)
         contributions = self.get_channel_contributions_forward_pass_grid(
@@ -848,17 +991,17 @@
             xlabel=x_label,
             ylabel="contribution",
         )
         return fig
 
     def new_spend_contributions(
         self,
-        spend: Optional[np.ndarray] = None,
+        spend: np.ndarray | None = None,
         one_time: bool = True,
-        spend_leading_up: Optional[np.ndarray] = None,
+        spend_leading_up: np.ndarray | None = None,
         prior: bool = False,
         original_scale: bool = True,
         **sample_posterior_predictive_kwargs,
     ) -> DataArray:
         """Return the upcoming contributions for a given spend.
 
         The spend can be one time or constant over the period. The spend leading up to the
@@ -980,19 +1123,19 @@
     def plot_new_spend_contributions(
         self,
         spend_amount: float,
         one_time: bool = True,
         lower: float = 0.025,
         upper: float = 0.975,
         ylabel: str = "Sales",
-        idx: Optional[slice] = None,
-        channels: Optional[List[str]] = None,
+        idx: slice | None = None,
+        channels: list[str] | None = None,
         prior: bool = False,
         original_scale: bool = True,
-        ax: Optional[plt.Axes] = None,
+        ax: plt.Axes | None = None,
         **sample_posterior_predictive_kwargs,
     ) -> plt.Axes:
         """Plot the upcoming sales for a given spend amount.
 
         Calls the new_spend_contributions method and plots the results. For more
         control over the plot, use new_spend_contributions directly.
 
@@ -1101,16 +1244,16 @@
             Defaults to True.
         combined: Combine chain and draw dims into sample. Won't work if a dim named sample already exists.
             Defaults to True.
         include_last_observations: Boolean determining whether to include the last observations of the training
             data in order to carry over costs with the adstock transformation.
             Assumes that X_pred are the next predictions following the training data.
             Defaults to False.
-        original_scale: Boolean determining whether to return the predictions in the original scale of the target variable.
-            Defaults to True.
+        original_scale: Boolean determining whether to return the predictions in the original scale
+            of the target variable. Defaults to True.
         **sample_posterior_predictive_kwargs: Additional arguments to pass to pymc.sample_posterior_predictive
 
         Returns
         -------
         posterior_predictive_samples : DataArray, shape (n_pred, samples)
             Posterior predictive samples for each input X_pred
         """
@@ -1142,7 +1285,117 @@
                 data=posterior_predictive_samples,
                 func=self.get_target_transformer().inverse_transform,
                 dim_name="date",
                 combined=combined,
             )
 
         return posterior_predictive_samples
+
+    def add_lift_test_measurements(
+        self,
+        df_lift_test: pd.DataFrame,
+        dist: pm.Distribution = pm.Gamma,
+        name: str = "lift_measurements",
+    ) -> None:
+        """Add lift tests to the model.
+
+        The model difference of a channel's saturation curve is created
+        from `x` and `x + delta_x` for each channel. This random variable is
+        then conditioned using the empirical lift, `delta_y`, and `sigma` of the lift test
+        with the specified distribution `dist`.
+
+        The sudo code for the lift test is as follows:
+
+        .. code-block:: python
+
+            model_estimated_lift = (
+                saturation_curve(x + delta_x)
+                - saturation_curve(x)
+            )
+            empirical_lift = delta_y
+            dist(model_estimated_lift, sigma=sigma, observed=empirical_lift)
+
+
+        The model has to be built before adding the lift tests.
+
+        Parameters
+        ----------
+        df_lift_test : pd.DataFrame
+            DataFrame with lift test results with at least the following columns:
+                * `channel`: channel name. Must be present in `channel_columns`.
+                * `x`: x axis value of the lift test.
+                * `delta_x`: change in x axis value of the lift test.
+                * `delta_y`: change in y axis value of the lift test.
+                * `sigma`: standard deviation of the lift test.
+        dist : pm.Distribution, optional
+            The distribution to use for the likelihood, by default pm.Gamma
+        name : str, optional
+            The name of the likelihood of the lift test contribution(s),
+            by default "lift_measurements". Name change required if calling
+            this method multiple times.
+
+        Raises
+        ------
+        RuntimeError
+            If the model has not been built yet.
+        KeyError
+            If the 'channel' column is not present in df_lift_test.
+
+        Examples
+        --------
+        Build the model first then add lift test measurements.
+
+        .. code-block:: python
+
+            model = DelayedSaturatedMMM(
+                date_column="date_week",
+                channel_columns=["x1", "x2"],
+                control_columns=[
+                    "event_1",
+                    "event_2",
+                ],
+                adstock_max_lag=8,
+                yearly_seasonality=2,
+            )
+
+            X: pd.DataFrame = ...
+            y: np.ndarray = ...
+
+            model.build_model(X, y)
+
+            df_lift_test = pd.DataFrame({
+                "channel": ["x1", "x1"],
+                "x": [1, 1],
+                "delta_x": [0.1, 0.2],
+                "delta_y": [0.1, 0.1],
+                "sigma": [0.1, 0.1],
+            })
+
+            model.add_lift_test_measurements(df_lift_test)
+
+        """
+        if self.model is None:
+            raise RuntimeError(
+                "The model has not been built yet. Please, build the model first."
+            )
+
+        if "channel" not in df_lift_test.columns:
+            raise KeyError(
+                "The 'channel' column is required to map the lift measurements to the model."
+            )
+
+        df_lift_test_scaled = scale_lift_measurements(
+            df_lift_test=df_lift_test,
+            channel_col="channel",
+            channel_columns=self.channel_columns,  # type: ignore
+            channel_transform=self.channel_transformer.transform,
+            target_transform=self.target_transformer.transform,
+        )
+        with self.model:
+            add_logistic_empirical_lift_measurements_to_likelihood(
+                df_lift_test=df_lift_test_scaled,
+                # Based on the model
+                lam_name="lam",
+                beta_name="beta_channel",
+                dist=dist,
+                name=name,
+            )
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/preprocessing.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/preprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-from typing import Any, Callable, List, Tuple, Union
+"""Preprocessing methods for the Marketing Mix Model."""
 
+from collections.abc import Callable
+from typing import Any
+
+import numpy as np
 import pandas as pd
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import MaxAbsScaler, StandardScaler
 
 __all__ = [
     "preprocessing_method_X",
     "preprocessing_method_y",
@@ -27,44 +31,46 @@
     return method
 
 
 class MaxAbsScaleTarget:
     target_transformer: Pipeline
 
     @preprocessing_method_y
-    def max_abs_scale_target_data(self, data: pd.Series) -> pd.Series:
+    def max_abs_scale_target_data(
+        self, data: pd.Series | np.ndarray
+    ) -> np.ndarray | pd.Series:
+        if isinstance(data, pd.Series):
+            data = data.to_numpy()
+
         target_vector = data.reshape(-1, 1)
         transformers = [("scaler", MaxAbsScaler())]
         pipeline = Pipeline(steps=transformers)
         self.target_transformer: Pipeline = pipeline.fit(X=target_vector)
         data = self.target_transformer.transform(X=target_vector).flatten()
         return data
 
 
 class MaxAbsScaleChannels:
-    channel_columns: Union[List[str], Tuple[str]]
+    channel_columns: list[str] | tuple[str]
 
     @preprocessing_method_X
     def max_abs_scale_channel_data(self, data: pd.DataFrame) -> pd.DataFrame:
         data_cp = data.copy()
-        channel_data: Union[
-            pd.DataFrame,
-            pd.Series[Any],
-        ] = data_cp[self.channel_columns]
+        channel_data: pd.DataFrame | pd.Series[Any] = data_cp[self.channel_columns]
         transformers = [("scaler", MaxAbsScaler())]
         pipeline: Pipeline = Pipeline(steps=transformers)
         self.channel_transformer: Pipeline = pipeline.fit(X=channel_data.to_numpy())
         data_cp[self.channel_columns] = self.channel_transformer.transform(
             channel_data.to_numpy()
         )
         return data_cp
 
 
 class StandardizeControls:
-    control_columns: List[str]  # TODO: Handle Optional[List[str]]
+    control_columns: list[str]  # TODO: Handle Optional[List[str]]
 
     @preprocessing_method_X
     def standardize_control_data(self, data: pd.DataFrame) -> pd.DataFrame:
         control_data: pd.DataFrame = data[self.control_columns]
         transformers = [("scaler", StandardScaler())]
         pipeline: Pipeline = Pipeline(steps=transformers)
         self.control_transformer: Pipeline = pipeline.fit(X=control_data.to_numpy())
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/transformers.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/transformers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+"""Media transformation functions for Marketing Mix Models."""
+
 from enum import Enum
-from typing import NamedTuple, Union
+from typing import Any, NamedTuple
 
 import numpy as np
 import numpy.typing as npt
 import pymc as pm
 import pytensor.tensor as pt
 from pytensor.tensor.random.utils import params_broadcast_shapes
 
@@ -21,15 +23,15 @@
     CDF = "CDF"
 
 
 def batched_convolution(
     x,
     w,
     axis: int = 0,
-    mode: Union[ConvMode, str] = ConvMode.After,
+    mode: ConvMode | str = ConvMode.After,
 ):
     R"""Apply a 1D convolution in a vectorized way across multiple batch dimensions.
 
     .. plot::
         :context: close-figs
 
         import matplotlib.pyplot as plt
@@ -59,19 +61,22 @@
         The array to convolve.
     w :
         The weight of the convolution. The last axis of ``w`` determines the number of steps
         to use in the convolution.
     axis : int
         The axis of ``x`` along witch to apply the convolution
     mode : ConvMode, optional
-        The convolution mode determines how the convolution is applied at the boundaries of the input signal, denoted as "x." The default mode is ConvMode.Before.
+        The convolution mode determines how the convolution is applied at the boundaries
+        of the input signal, denoted as "x." The default mode is ConvMode.Before.
 
         - ConvMode.After: Applies the convolution with the "Adstock" effect, resulting in a trailing decay effect.
-        - ConvMode.Before: Applies the convolution with the "Excitement" effect, creating a leading effect similar to the wow factor.
-        - ConvMode.Overlap: Applies the convolution with both "Pull-Forward" and "Pull-Backward" effects, where the effect overlaps with both preceding and succeeding elements.
+        - ConvMode.Before: Applies the convolution with the "Excitement" effect, creating a leading effect
+            similar to the wow factor.
+        - ConvMode.Overlap: Applies the convolution with both "Pull-Forward" and "Pull-Backward" effects,
+            where the effect overlaps with both preceding and succeeding elements.
 
     Returns
     -------
     y :
         The result of convolving ``x`` with ``w`` along the desired axis. The shape of the
         result will match the shape of ``x`` up to broadcasting with ``w``. The convolved
         axis will show the results of left padding zeros to ``x`` while applying the
@@ -83,15 +88,15 @@
     axis = axis if axis >= 0 else orig_ndim + axis
     w = pt.as_tensor(w)
     x = pt.moveaxis(x, axis, -1)
     l_max = w.type.shape[-1]
     if l_max is None:
         try:
             l_max = w.shape[-1].eval()
-        except Exception:
+        except Exception:  # noqa: S110
             pass
     # Get the broadcast shapes of x and w but ignoring their last dimension.
     # The last dimension of x is the "time" axis, which doesn't get broadcast
     # The last dimension of w is the number of time steps that go into the convolution
     x_shape, w_shape = params_broadcast_shapes([x.shape, w.shape], [1, 1])
 
     x = pt.broadcast_to(x, x_shape)
@@ -275,19 +280,20 @@
 
 def weibull_adstock(
     x,
     lam=1,
     k=1,
     l_max: int = 12,
     axis: int = 0,
-    type: Union[WeibullType, str] = WeibullType.PDF,
+    type: WeibullType | str = WeibullType.PDF,
 ):
     R"""Weibull Adstocking Transformation.
 
-    This transformation is similar to geometric adstock transformation but has more degrees of freedom, adding more flexibility.
+    This transformation is similar to geometric adstock transformation but has more
+    degrees of freedom, adding more flexibility.
 
     .. plot::
         :context: close-figs
 
         import matplotlib.pyplot as plt
         import numpy as np
         import arviz as az
@@ -367,15 +373,15 @@
         padded_w = pt.set_subtensor(padded_w[..., 1:], w)
         w = pt.cumprod(padded_w, axis=-1)
     else:
         raise ValueError(f"Wrong WeibullType: {type}, expected of WeibullType")
     return batched_convolution(x, w, axis=axis)
 
 
-def logistic_saturation(x, lam: Union[npt.NDArray[np.float_], float] = 0.5):
+def logistic_saturation(x, lam: npt.NDArray[np.float_] | float = 0.5):
     """Logistic saturation transformation.
 
     .. math::
         f(x) = \\frac{1 - e^{-\lambda x}}{1 + e^{-\lambda x}}
 
     .. plot::
         :context: close-figs
@@ -503,15 +509,15 @@
     -------
     tensor
         Transformed tensor.
 
     References
     ----------
     See https://www.pymc-labs.io/blog-posts/reducing-customer-acquisition-costs-how-we-helped-optimizing-hellofreshs-marketing-budget/ # noqa: E501
-    """
+    """  # noqa: E501
     return b * pt.tanh(x / (b * c))
 
 
 def tanh_saturation_baselined(
     x: pt.TensorLike,
     x0: pt.TensorLike,
     gain: pt.TensorLike = 0.5,
@@ -657,7 +663,96 @@
         Transformed tensor.
 
     References
     ----------
     Developed by Max Kochurov and Aziz Al-Maeeni doing innovative work in `PyMC Labs <pymc-labs.com>`_.
     """
     return gain * x0 * pt.tanh(x * pt.arctanh(r) / x0) / r
+
+
+def michaelis_menten(
+    x: float | np.ndarray | npt.NDArray[np.float64],
+    alpha: float | np.ndarray | npt.NDArray[np.float64],
+    lam: float | np.ndarray | npt.NDArray[np.float64],
+) -> float | Any:
+    r"""
+    Evaluate the Michaelis-Menten function for given values of x, alpha, and lambda.
+
+    The Michaelis-Menten function models enzyme kinetics and describes how the rate of
+    a chemical reaction increases with substrate concentration until it reaches its
+    maximum value.
+
+    .. math::
+        \alpha \cdot \frac{x}{\lambda + x}
+
+    where:
+     - :math:`x`: Channel spend or substrate concentration.
+     - :math:`\alpha`: Maximum contribution or efficiency factor.
+     - :math:`\lambda` (k): Michaelis constant, representing the threshold substrate concentration.
+
+    .. plot::
+        :context: close-figs
+
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from pymc_marketing.mmm.transformers import michaelis_menten
+
+        x = np.linspace(0, 100, 500)
+        alpha = 10
+        lam = 50
+        y = michaelis_menten(x, alpha, lam)
+
+        plt.plot(x, y)
+        plt.xlabel('Spend/Impressions (x)')
+        plt.ylabel('Contribution (y)')
+        plt.title('Michaelis-Menten Function')
+        plt.show()
+
+    .. plot::
+        :context: close-figs
+
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from pymc_marketing.mmm.transformers import michaelis_menten
+
+        x = np.linspace(0, 100, 500)
+        alpha_values = [5, 10, 15]  # Different values of alpha
+        lam_values = [25, 50, 75]  # Different values of lam
+
+        # Plot varying lam
+        plt.figure(figsize=(8, 6))
+        for lam in lam_values:
+            y = michaelis_menten(x, alpha_values[0], lam)
+            plt.plot(x, y, label=f"lam={lam}")
+        plt.xlabel('Spend/Impressions (x)')
+        plt.ylabel('Contribution (y)')
+        plt.title('Michaelis-Menten Function (Varying lam)')
+        plt.legend()
+        plt.show()
+
+        # Plot varying alpha
+        plt.figure(figsize=(8, 6))
+        for alpha in alpha_values:
+            y = michaelis_menten(x, alpha, lam_values[0])
+            plt.plot(x, y, label=f"alpha={alpha}")
+        plt.xlabel('Spend/Impressions (x)')
+        plt.ylabel('Contribution (y)')
+        plt.title('Michaelis-Menten Function (Varying alpha)')
+        plt.legend()
+        plt.show()
+
+    Parameters
+    ----------
+    x : float
+        The spent on a channel.
+    alpha : float
+        The maximum contribution a channel can make.
+    lam : float
+        The Michaelis constant for the given enzyme-substrate system.
+
+    Returns
+    -------
+    float
+        The value of the Michaelis-Menten function given the parameters.
+    """
+
+    return alpha * x / (lam + x)
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/utils.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+"""Utility functions for the Marketing Mix Modeling module."""
+
 import re
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from collections.abc import Callable
+from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import xarray as xr
 from scipy.optimize import curve_fit, minimize_scalar
 
+from pymc_marketing.mmm.transformers import michaelis_menten
+
 
 def generate_fourier_modes(
     periods: npt.NDArray[np.float_], n_order: int
 ) -> pd.DataFrame:
     """Generate Fourier modes.
 
     Parameters
@@ -36,75 +41,20 @@
             f"{func}_order_{order}": getattr(np, func)(2 * np.pi * periods * order)
             for order in range(1, n_order + 1)
             for func in ("sin", "cos")
         }
     )
 
 
-def michaelis_menten(
-    x: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    alpha: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    lam: Union[float, np.ndarray, npt.NDArray[np.float64]],
-) -> Union[float, Any]:
-    """
-    Evaluate the Michaelis-Menten function for given values of x, alpha, and lambda.
-
-    The Michaelis-Menten function is a type of mathematical saturation function commonly used in
-    enzyme kinetics, but it's also applicable in marketing mix models to describe
-    how different channels contribute to a certain outcome (e.g., sales or conversions)
-    as the spending on that channel increases and the contribution saturates.
-
-    Mathematically, it is described as:
-    α * x / (λ + x)
-
-    Parameters
-    ----------
-    x : float
-        The spent on a channel.
-    alpha (Limit/Vmax) : float
-        The maximum contribution a channel can make.
-    lam (k) : float
-        The elbow on the function in `x` (Point where the curve change their direction).
-
-    Returns
-    -------
-    float
-        The value of the Michaelis-Menten function given the parameters.
-    """
-
-    return alpha * x / (lam + x)
-
-
-def extense_sigmoid(
-    x: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    alpha: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    lam: Union[float, np.ndarray, npt.NDArray[np.float64]],
-) -> Union[float, Any]:
-    """
-    Parameters
-    ----------
-    - alpha
-        α (alpha): Represent the Asymptotic Maximum or Ceiling Value.
-    - lam
-        λ (lambda): affects how quickly the function approaches its upper and lower asymptotes. A higher value of
-        lam makes the curve steeper, while a lower value makes it more gradual.
-    """
-
-    if alpha <= 0 or lam <= 0:
-        raise ValueError("alpha and lam must be greater than 0")
-
-    return (alpha - alpha * np.exp(-lam * x)) / (1 + np.exp(-lam * x))
-
-
 def estimate_menten_parameters(
-    channel: Union[str, Any],
-    original_dataframe: Union[pd.DataFrame, Any],
-    contributions: Union[xr.DataArray, Any],
+    channel: str | Any,
+    original_dataframe: pd.DataFrame | Any,
+    contributions: xr.DataArray | Any,
     **kwargs,
-) -> List[float]:
+) -> list[float]:
     """
     Estimate the parameters for the Michaelis-Menten function using curve fitting.
 
     This function extracts the relevant data for the specified channel from both
     the original_dataframe and contributions DataArray resulting from the model.
     It then utilizes scipy's curve_fit method to find the optimal parameters for
     an Menten function, aiming to minimize the least squares difference between
@@ -138,19 +88,19 @@
     popt, pcov = curve_fit(michaelis_menten, x, y, p0=initial_guess, maxfev=maxfev)
 
     # Save the parameters
     return popt
 
 
 def estimate_sigmoid_parameters(
-    channel: Union[str, Any],
-    original_dataframe: Union[pd.DataFrame, Any],
-    contributions: Union[xr.DataArray, Any],
+    channel: str | Any,
+    original_dataframe: pd.DataFrame | Any,
+    contributions: xr.DataArray | Any,
     **kwargs,
-) -> List[float]:
+) -> list[float]:
     """
     Estimate the parameters for the sigmoid function using curve fitting.
 
     This function extracts the relevant data for the specified channel from both
     the original_dataframe and contributions DataArray resulting from the model.
     It then utilizes scipy's curve_fit method to find the optimal parameters for
     an sigmoid function, aiming to minimize the least squares difference between
@@ -176,30 +126,30 @@
     x = kwargs.get("x", original_dataframe[channel].to_numpy())
     y = kwargs.get("y", contributions.sel(channel=channel).to_numpy())
 
     alpha_initial_estimate = kwargs.get("alpha_initial_estimate", 3 * max(y))
 
     parameter_bounds_modified = ([0, 0], [alpha_initial_estimate, np.inf])
     popt, _ = curve_fit(
-        extense_sigmoid,
+        sigmoid_saturation,
         x,
         y,
         p0=[alpha_initial_estimate, lam_initial_estimate],
         bounds=parameter_bounds_modified,
         maxfev=maxfev,
     )
 
     return popt
 
 
 def compute_sigmoid_second_derivative(
-    x: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    alpha: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    lam: Union[float, np.ndarray, npt.NDArray[np.float64]],
-) -> Union[float, Any]:
+    x: float | np.ndarray | npt.NDArray[np.float64],
+    alpha: float | np.ndarray | npt.NDArray[np.float64],
+    lam: float | np.ndarray | npt.NDArray[np.float64],
+) -> float | Any:
     """
     Compute the second derivative of the extended sigmoid function.
 
     The second derivative of a function gives us information about the curvature of the function.
     In the context of the sigmoid function, it helps us identify the inflection point, which is
     the point where the function changes from being concave up to concave down, or vice versa.
 
@@ -224,17 +174,17 @@
         * np.exp(-lam * x)
         * (1 - np.exp(-lam * x) - 2 * lam * x * np.exp(-lam * x))
         / (1 + np.exp(-lam * x)) ** 3
     )
 
 
 def find_sigmoid_inflection_point(
-    alpha: Union[float, np.ndarray, npt.NDArray[np.float64]],
-    lam: Union[float, np.ndarray, npt.NDArray[np.float64]],
-) -> Tuple[Any, float]:
+    alpha: float | np.ndarray | npt.NDArray[np.float64],
+    lam: float | np.ndarray | npt.NDArray[np.float64],
+) -> tuple[Any, float]:
     """
     Find the inflection point of the extended sigmoid function.
 
     The inflection point of a function is the point where the function changes its curvature,
     i.e., it changes from being concave up to concave down, or vice versa. For the sigmoid
     function, this is the point where the function has its maximum rate of growth.
 
@@ -254,25 +204,25 @@
     # Minimize the negative of the absolute value of the second derivative
     result = minimize_scalar(
         lambda x: -abs(compute_sigmoid_second_derivative(x, alpha, lam))
     )
 
     # Evaluate the original function at the inflection point
     x_inflection = result.x
-    y_inflection = extense_sigmoid(x_inflection, alpha, lam)
+    y_inflection = sigmoid_saturation(x_inflection, alpha, lam)
 
     return x_inflection, y_inflection
 
 
-def standardize_scenarios_dict_keys(d: Dict, keywords: List[str]):
+def standardize_scenarios_dict_keys(d: dict, keywords: list[str]):
     """
     Standardize the keys in a dictionary based on a list of keywords.
 
-    This function iterates over the keys in the dictionary and the keywords. If a keyword is found in a key (case-insensitive),
-    the key is replaced with the keyword.
+    This function iterates over the keys in the dictionary and the keywords.
+    If a keyword is found in a key (case-insensitive), the key is replaced with the keyword.
 
     Parameters
     ----------
     d : dict
         The dictionary whose keys are to be standardized.
     keywords : list
         The list of keywords to standardize the keys to.
@@ -326,19 +276,40 @@
         ).squeeze(dim="_")
 
     data.attrs = attrs
 
     return data
 
 
+def sigmoid_saturation(
+    x: float | np.ndarray | npt.NDArray[np.float64],
+    alpha: float | np.ndarray | npt.NDArray[np.float64],
+    lam: float | np.ndarray | npt.NDArray[np.float64],
+) -> float | Any:
+    """
+    Parameters
+    ----------
+    alpha
+        α (alpha): Represent the Asymptotic Maximum or Ceiling Value.
+    lam
+        λ (lambda): affects how quickly the function approaches its upper and lower asymptotes. A higher value of
+        lam makes the curve steeper, while a lower value makes it more gradual.
+    """
+
+    if alpha <= 0 or lam <= 0:
+        raise ValueError("alpha and lam must be greater than 0")
+
+    return (alpha - alpha * np.exp(-lam * x)) / (1 + np.exp(-lam * x))
+
+
 def create_new_spend_data(
     spend: np.ndarray,
     adstock_max_lag: int,
     one_time: bool,
-    spend_leading_up: Optional[np.ndarray] = None,
+    spend_leading_up: np.ndarray | None = None,
 ) -> np.ndarray:
     """Create new spend data for the channel forward pass.
 
     Spends must be the same length as the number of channels.
 
     .. plot::
         :context: close-figs
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/mmm/validating.py` & `pymc_marketing-0.5.0/pymc_marketing/mmm/validating.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Callable, List, Optional, Tuple, Union
+"""Validating methods for MMM classes."""
+
+from collections.abc import Callable
 
 import pandas as pd
 
 __all__ = [
     "validation_method_X",
     "validation_method_y",
     "ValidateControlColumns",
@@ -41,19 +43,19 @@
         if self.date_column not in data.columns:
             raise ValueError(f"date_col {self.date_column} not in data")
         if not data[self.date_column].is_unique:
             raise ValueError(f"date_col {self.date_column} has repeated values")
 
 
 class ValidateChannelColumns:
-    channel_columns: Union[List[str], Tuple[str]]
+    channel_columns: list[str] | tuple[str]
 
     @validation_method_X
     def validate_channel_columns(self, data: pd.DataFrame) -> None:
-        if not isinstance(self.channel_columns, (list, tuple)):
+        if not isinstance(self.channel_columns, list | tuple):
             raise ValueError("channel_columns must be a list or tuple")
         if len(self.channel_columns) == 0:
             raise ValueError("channel_columns must not be empty")
         if not set(self.channel_columns).issubset(data.columns):
             raise ValueError(f"channel_columns {self.channel_columns} not in data")
         if len(set(self.channel_columns)) != len(self.channel_columns):
             raise ValueError(
@@ -62,21 +64,21 @@
         if (data.filter(list(self.channel_columns)) < 0).any().any():
             raise ValueError(
                 f"channel_columns {self.channel_columns} contains negative values"
             )
 
 
 class ValidateControlColumns:
-    control_columns: Optional[List[str]]
+    control_columns: list[str] | None
 
     @validation_method_X
     def validate_control_columns(self, data: pd.DataFrame) -> None:
         if self.control_columns is None:
             return None
-        if not isinstance(self.control_columns, (list, tuple)):
+        if not isinstance(self.control_columns, list | tuple):
             raise ValueError("control_columns must be None, a list or tuple")
         if len(self.control_columns) == 0:
             raise ValueError(
                 "If control_columns is not None, then it must not be empty"
             )
         if not set(self.control_columns).issubset(data.columns):
             raise ValueError(f"control_columns {self.control_columns} not in data")
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing/model_builder.py` & `pymc_marketing-0.5.0/pymc_marketing/model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 import hashlib
 import json
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any
 
 import arviz as az
 import numpy as np
 import pandas as pd
 import pymc as pm
 import xarray as xr
 from pymc.util import RandomState
@@ -45,33 +45,35 @@
     ModelBuilder can be used to provide an easy-to-use API (similar to scikit-learn) for models
     and help with deployment.
     """
 
     _model_type = "BaseClass"
     version = "None"
 
-    X: Optional[pd.DataFrame] = None
-    y: Optional[Union[pd.Series, np.ndarray]] = None
+    X: pd.DataFrame | None = None
+    y: pd.Series | np.ndarray | None = None
 
     def __init__(
         self,
-        model_config: Optional[Dict] = None,
-        sampler_config: Optional[Dict] = None,
+        model_config: dict | None = None,
+        sampler_config: dict | None = None,
     ):
         """
         Initializes model configuration and sampler configuration for the model
 
         Parameters
         ----------
         data : Dictionary, optional
             It is the data we need to train the model on.
         model_config : Dictionary, optional
-            dictionary of parameters that initialise model configuration. Class-default defined by the user default_model_config method.
+            dictionary of parameters that initialise model configuration.
+            Class-default defined by the user default_model_config method.
         sampler_config : Dictionary, optional
-            dictionary of parameters that initialise sampler configuration. Class-default defined by the user default_sampler_config method.
+            dictionary of parameters that initialise sampler configuration.
+            Class-default defined by the user default_sampler_config method.
         Examples
         --------
         >>> class MyModel(ModelBuilder):
         >>>     ...
         >>> model = MyModel(model_config, sampler_config)
         """
         if sampler_config is None:
@@ -80,33 +82,31 @@
             model_config = {}
         self.sampler_config = (
             self.default_sampler_config | sampler_config
         )  # Parameters for fit sampling
         self.model_config = (
             self.default_model_config | model_config
         )  # parameters for priors etc.
-        self.model: Optional[pm.Model] = None  # Set by build_model
-        self.idata: Optional[az.InferenceData] = (
-            None  # idata is generated during fitting
-        )
+        self.model: pm.Model | None = None  # Set by build_model
+        self.idata: az.InferenceData | None = None  # idata is generated during fitting
         self.is_fitted_ = False
 
     def _validate_data(self, X, y=None):
         if y is not None:
             return check_X_y(
                 X, y, accept_sparse=False, y_numeric=True, multi_output=False
             )
         else:
             return check_array(X, accept_sparse=False)
 
     @abstractmethod
     def _data_setter(
         self,
-        X: Union[np.ndarray, pd.DataFrame],
-        y: Optional[Union[np.ndarray, pd.Series]] = None,
+        X: np.ndarray | pd.DataFrame,
+        y: np.ndarray | pd.Series | None = None,
     ) -> None:
         """
         Sets new data in the model.
 
         Parameters
         ----------
         X : array, shape (n_obs, n_features)
@@ -143,15 +143,15 @@
         output_var : str
             Name of the output variable of the model.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def default_model_config(self) -> Dict:
+    def default_model_config(self) -> dict:
         """
         Returns a class default config dict for model builder if no model_config is provided on class initialization
         Useful for understanding structure of required model_config to allow its customization by users
         Examples
         --------
         >>>     @classmethod
         >>>     def default_model_config(self):
@@ -172,15 +172,15 @@
         model_config : dict
             A set of default parameters for predictor distributions that allow to save and recreate the model.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def default_sampler_config(self) -> Dict:
+    def default_sampler_config(self) -> dict:
         """
         Returns a class default sampler dict for model builder if no sampler_config is provided on class initialization
         Useful for understanding structure of required sampler_config to allow its customization by users
         Examples
         --------
         >>>     @classmethod
         >>>     def default_sampler_config(self):
@@ -196,15 +196,15 @@
         sampler_config : dict
             A set of default settings for used by model in fit process.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _generate_and_preprocess_model_data(
-        self, X: Union[pd.DataFrame, pd.Series], y: np.ndarray
+        self, X: pd.DataFrame | pd.Series, y: np.ndarray
     ) -> None:
         """
         Applies preprocessing to the data before fitting the model.
         if validate is True, it will check if the data is valid for the model.
         sets self.model_coords based on provided dataset
 
         In case of optional parameters being passed into the model, this method should implement the conditional
@@ -231,15 +231,15 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def build_model(
         self,
         X: pd.DataFrame,
-        y: Union[pd.Series, np.ndarray],
+        y: pd.Series | np.ndarray,
         **kwargs,
     ) -> None:
         """
         Creates an instance of pm.Model based on provided data and model_config, and
         attaches it to self.
 
         Parameters
@@ -343,18 +343,19 @@
         if self.idata is not None and "posterior" in self.idata:
             file = Path(str(fname))
             self.idata.to_netcdf(str(file))
         else:
             raise RuntimeError("The model hasn't been fit yet, call .fit() first")
 
     @classmethod
-    def _model_config_formatting(cls, model_config: Dict) -> Dict:
+    def _model_config_formatting(cls, model_config: dict) -> dict:
         """
-        Because of json serialization, model_config values that were originally tuples or numpy are being encoded as lists.
-        This function converts them back to tuples and numpy arrays to ensure correct id encoding.
+        Because of json serialization, model_config values that were originally tuples
+        or numpy are being encoded as lists. This function converts them back to tuples
+        and numpy arrays to ensure correct id encoding.
         """
         for key in model_config:
             if isinstance(model_config[key], dict):
                 for sub_key in model_config[key]:
                     if isinstance(model_config[key][sub_key], list):
                         # Check if "dims" key to convert it to tuple
                         if sub_key == "dims":
@@ -408,27 +409,27 @@
         dataset = idata.fit_data.to_dataframe()
         X = dataset.drop(columns=[model.output_var])
         y = dataset[model.output_var]
         model.build_model(X, y)
         # All previously used data is in idata.
 
         if model.id != idata.attrs["id"]:
-            raise ValueError(
-                f"The file '{fname}' does not contain an inference data of the same model or configuration as '{cls._model_type}'"
-            )
+            error_msg = f"""The file '{fname}' does not contain an inference data of the same model
+            or configuration as '{cls._model_type}'"""
+            raise ValueError(error_msg)
 
         return model
 
     def fit(
         self,
         X: pd.DataFrame,
-        y: Optional[Union[pd.Series, np.ndarray]] = None,
+        y: pd.Series | np.ndarray | None = None,
         progressbar: bool = True,
-        predictor_names: Optional[List[str]] = None,
-        random_seed: Optional[RandomState] = None,
+        predictor_names: list[str] | None = None,
+        random_seed: RandomState | None = None,
         **kwargs: Any,
     ) -> az.InferenceData:
         """
         Fit a model using the data passed as a parameter.
         Sets attrs to inference data of the model.
 
 
@@ -438,15 +439,16 @@
             The training input samples.
         y : array-like if sklearn is available, otherwise array, shape (n_obs,)
             The target values (real numbers).
         progressbar : bool
             Specifies whether the fit progressbar should be displayed
         predictor_names: Optional[List[str]] = None,
             Allows for custom naming of predictors given in a form of 2dArray
-            allows for naming of predictors when given in a form of np.ndarray, if not provided the predictors will be named like predictor1, predictor2...
+            Allows for naming of predictors when given in a form of np.ndarray, if not provided
+            the predictors will be named like predictor1, predictor2...
         random_seed : Optional[RandomState]
             Provides sampler with initial random seed for obtaining reproducible samples
         **kwargs : Any
             Custom sampler settings can be provided in form of keyword arguments.
 
         Returns
         -------
@@ -463,43 +465,46 @@
             predictor_names = []
         if y is None:
             y = np.zeros(X.shape[0])
         y_df = pd.DataFrame({self.output_var: y})
         self._generate_and_preprocess_model_data(X, y_df.values.flatten())
         if self.X is None or self.y is None:
             raise ValueError("X and y must be set before calling build_model!")
-        self.build_model(self.X, self.y)
+
+        if self.model is None:
+            self.build_model(self.X, self.y)
 
         sampler_config = self.sampler_config.copy()
         sampler_config["progressbar"] = progressbar
         sampler_config["random_seed"] = random_seed
         sampler_config.update(**kwargs)
 
         sampler_config.update(**kwargs)
         if self.model is not None:
             with self.model:
                 sampler_args = {**self.sampler_config, **kwargs}
                 self.idata = pm.sample(**sampler_args)
 
         X_df = pd.DataFrame(X, columns=X.columns)
         combined_data = pd.concat([X_df, y_df], axis=1)
-        assert all(combined_data.columns), "All columns must have non-empty names"
+        if not all(combined_data.columns):
+            raise ValueError("All columns must have non-empty names")
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore",
                 category=UserWarning,
                 message="The group fit_data is not defined in the InferenceData scheme",
             )
             self.idata.add_groups(fit_data=combined_data.to_xarray())  # type: ignore
         self.set_idata_attrs(self.idata)
         return self.idata  # type: ignore
 
     def predict(
         self,
-        X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
+        X_pred: np.ndarray | pd.DataFrame | pd.Series,
         extend_idata: bool = True,
         **kwargs,
     ) -> np.ndarray:
         """
         Uses model to predict on unseen data and return point prediction of all the samples. The point prediction
         for each input row is the expected output value, computed as the mean of MCMC samples.
 
@@ -539,15 +544,15 @@
         )
         return posterior_means.data
 
     def sample_prior_predictive(
         self,
         X_pred,
         y_pred=None,
-        samples: Optional[int] = None,
+        samples: int | None = None,
         extend_idata: bool = False,
         combined: bool = True,
         **kwargs,
     ):
         """
         Sample from the model's prior predictive distribution.
 
@@ -644,38 +649,38 @@
         Set all the model parameters needed to instantiate the model, not including training data.
         """
         self.model_config = params["model_config"]
         self.sampler_config = params["sampler_config"]
 
     @property
     @abstractmethod
-    def _serializable_model_config(self) -> Dict[str, Union[int, float, Dict]]:
+    def _serializable_model_config(self) -> dict[str, int | float | dict]:
         """
         Converts non-serializable values from model_config to their serializable reversable equivalent.
         Data types like pandas DataFrame, Series or datetime aren't JSON serializable,
         so in order to save the model they need to be formatted.
 
         Returns
         -------
         model_config: dict
         """
 
     def predict_proba(
         self,
-        X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
+        X_pred: np.ndarray | pd.DataFrame | pd.Series,
         extend_idata: bool = True,
         combined: bool = False,
         **kwargs,
     ) -> xr.DataArray:
         """Alias for `predict_posterior`, for consistency with scikit-learn probabilistic estimators."""
         return self.predict_posterior(X_pred, extend_idata, combined, **kwargs)
 
     def predict_posterior(
         self,
-        X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
+        X_pred: np.ndarray | pd.DataFrame | pd.Series,
         extend_idata: bool = True,
         combined: bool = True,
         **kwargs,
     ) -> xr.DataArray:
         """
         Generate posterior predictive samples on unseen data.
 
@@ -708,16 +713,16 @@
         return posterior_predictive_samples[self.output_var]
 
     @property
     def id(self) -> str:
         """
         Generate a unique hash value for the model.
 
-        The hash value is created using the last 16 characters of the SHA256 hash encoding, based on the model configuration,
-        version, and model type.
+        The hash value is created using the last 16 characters of the SHA256 hash encoding,
+        based on the model configuration, version, and model type.
 
         Returns
         -------
         str
             A string of length 16 characters containing a unique hash of the model.
 
         Examples
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing.egg-info/PKG-INFO` & `pymc_marketing-0.5.0/pymc_marketing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-marketing
-Version: 0.4.2
+Version: 0.5.0
 Summary: Marketing Statistical Models in PyMC
 Maintainer-email: PyMC Labs <info@pymc-labs.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,15 +202,15 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: repository, https://github.com/pymc-labs/pymc-marketing
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arviz>=0.13.0
 Requires-Dist: matplotlib>=3.5.1
 Requires-Dist: numpy>=1.17
 Requires-Dist: pandas
 Requires-Dist: pymc>=5.10.4
@@ -254,15 +254,14 @@
 [![PyPI Version](https://img.shields.io/pypi/v/pymc-marketing.svg)](https://pypi.python.org/pypi/pymc-marketing)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # <span style="color:limegreen">PyMC-Marketing</span>: Bayesian Marketing Mix Modeling (MMM) & Customer Lifetime Value (CLV)
 
 ## Marketing Analytics Tools from [PyMC Labs](https://www.pymc-labs.com)
 
-
 Unlock the power of **Marketing Mix Modeling (MMM)** and **Customer Lifetime Value (CLV)** analytics with PyMC-Marketing. This open-source marketing analytics tool empowers businesses to make smarter, data-driven decisions for maximizing ROI in marketing campaigns.
 
 ## Quick Installation Guide for Marketing Mix Modeling (MMM) & CLV
 
 To dive into MMM and CLV analytics, set up a specialized environment, `marketing_env`, via conda-forge:
 
 ```bash
@@ -279,19 +278,19 @@
 ## In-depth Bayesian Marketing Mix Modeling (MMM) in PyMC
 
 Leverage our Bayesian MMM API to tailor your marketing strategies effectively. Based on the research [Jin, Yuxue, et al. “Bayesian methods for media mix modeling with carryover and shape effects.” (2017)](https://research.google/pubs/pub46001/),  and integrating the expertise from core PyMC developers, our API provides:
 
 - **Adstock Transformation**: Optimize the carry-over effects in your marketing channels.
 - **Saturation Effects**: Understand the diminishing returns in media investments.
 - **Budget Optimization**: Allocate your marketing spend efficiently across various channels for maximum ROI.
-- **Experiment Calibration**: Fine-tune your model based on empirical experiments for more unified view of marketing.
+- **Experiment Calibration**: Fine-tune your model based on empirical experiments for a more unified view of marketing.
 
 Explore a hands-on [simulated example](https://pymc-marketing.readthedocs.io/en/stable/notebooks/mmm/mmm_example.html) for more insights into MMM with PyMC-Marketing.
 
-### Essential Reading for Marketing Mix Modeling (MMM):
+### Essential Reading for Marketing Mix Modeling (MMM)
 
 - [Bayesian Media Mix Modeling for Marketing Optimization](https://www.pymc-labs.com/blog-posts/bayesian-media-mix-modeling-for-marketing-optimization/)
 - [Improving the Speed and Accuracy of Bayesian Marketing Mix Models](https://www.pymc-labs.com/blog-posts/reducing-customer-acquisition-costs-how-we-helped-optimizing-hellofreshs-marketing-budget/)
 - [Johns, Michael and Wang,  Zhenyu. "A Bayesian Approach to Media Mix Modeling"](https://www.youtube.com/watch?v=UznM_-_760Y)
 - [Orduz, Juan. "Media Effect Estimation with PyMC: Adstock, Saturation & Diminishing Returns"](https://juanitorduz.github.io/pymc_mmm/)
 - [A Comprehensive Guide to Bayesian Marketing Mix Modeling](https://1749.io/resource-center/f/a-comprehensive-guide-to-bayesian-marketing-mix-modeling)
 
@@ -314,15 +313,15 @@
 
 ---
 
 ## Why PyMC-Marketing vs other solutions?
 
 PyMC-Marketing is and will always be free for commercial use, licensed under [Apache 2.0](LICENSE). Developed by core developers behind the popular PyMC package and marketing experts, it provides state-of-the-art measurements and analytics for marketing teams.
 
-Due to its open source nature and active contributor base, new features get added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
+Due to its open-source nature and active contributor base, new features are added constantly. Missing a feature or want to contribute? Fork our repository and submit a pull request. For any questions, feel free to [open an issue](https://github.com/your-repo/issues).
 
 ## Marketing AI Assistant: MMM-GPT with PyMC-Marketing
 
 Not sure how to start or have questions? MMM-GPT is an AI that answers questions and provides expert advice on marketing analytics using PyMC-Marketing.
 
 **[Try MMM-GPT here.](https://mmm-gpt.com/)**
 
@@ -332,11 +331,11 @@
 
 Maximize your marketing ROI with a [free 30-minute strategy session](https://calendly.com/niall-oulton) with our PyMC-Marketing experts. Learn how Bayesian Marketing Mix Modeling and Customer Lifetime Value analytics can boost your organization by making smarter, data-driven decisions.
 
 For businesses looking to integrate PyMC-Marketing into their operational framework, [PyMC Labs](https://www.pymc-labs.com) offers expert consulting and training. Our team is proficient in state-of-the-art Bayesian modeling techniques, with a focus on Marketing Mix Models (MMMs) and Customer Lifetime Value (CLV). Explore these topics further by watching our video on [Bayesian Marketing Mix Models: State of the Art](https://www.youtube.com/watch?v=xVx91prC81g).
 
 We provide the following professional services:
 
-- **Custom Models**: We tailor niche marketing anayltics models to fit your organization's unique needs.
-- **Build Within PyMC-Marketing**: Our team are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
+- **Custom Models**: We tailor niche marketing analytics models to fit your organization's unique needs.
+- **Build Within PyMC-Marketing**: Our team members are experts leveraging the capabilities of PyMC-Marketing to create robust marketing models for precise insights.
 - **SLA & Coaching**: Get guaranteed support levels and personalized coaching to ensure your team is well-equipped and confident in using our tools and approaches.
 - **SaaS Solutions**: Harness the power of our state-of-the-art software solutions to streamline your data-driven marketing initiatives.
```

### Comparing `pymc-marketing-0.4.2/pymc_marketing.egg-info/SOURCES.txt` & `pymc_marketing-0.5.0/pymc_marketing.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 pymc_marketing/clv/models/gamma_gamma.py
 pymc_marketing/clv/models/pareto_nbd.py
 pymc_marketing/clv/models/shifted_beta_geo.py
 pymc_marketing/mmm/__init__.py
 pymc_marketing/mmm/base.py
 pymc_marketing/mmm/budget_optimizer.py
 pymc_marketing/mmm/delayed_saturated_mmm.py
+pymc_marketing/mmm/lift_test.py
 pymc_marketing/mmm/preprocessing.py
 pymc_marketing/mmm/transformers.py
 pymc_marketing/mmm/utils.py
 pymc_marketing/mmm/validating.py
```

