# Comparing `tmp/ml_logger-0.9.8.tar.gz` & `tmp/ml_logger-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_logger-0.9.8.tar", max compression
+gzip compressed data, was "ml_logger-0.9.9.tar", max compression
```

## Comparing `ml_logger-0.9.8.tar` & `ml_logger-0.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1523 2021-12-23 17:37:45.000000 ml_logger-0.9.8/LICENSE.md
--rw-r--r--   0        0        0    22970 2022-12-05 02:36:36.448538 ml_logger-0.9.8/README.md
--rw-r--r--   0        0        0    13191 2023-04-03 06:23:26.297176 ml_logger-0.9.8/ml_logger/__init__.py
--rw-r--r--   0        0        0        0 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/caches/__init__.py
--rw-r--r--   0        0        0      683 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/caches/key_value_cache.py
--rw-r--r--   0        0        0     8541 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/caches/summary_cache.py
--rw-r--r--   0        0        0     2529 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/full_duplex.py
--rw-r--r--   0        0        0     3842 2022-07-24 14:29:59.384948 ml_logger-0.9.8/ml_logger/helpers/__init__.py
--rw-r--r--   0        0        0     1520 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/helpers/color_helpers.py
--rw-r--r--   0        0        0      646 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/helpers/data_helpers.py
--rw-r--r--   0        0        0     1088 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/helpers/default_set.py
--rw-r--r--   0        0        0      188 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/helpers/file_helpers.py
--rw-r--r--   0        0        0     2269 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/helpers/func_helpers.py
--rw-r--r--   0        0        0     3354 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/helpers/print_utils.py
--rw-r--r--   0        0        0    15060 2022-11-16 04:29:13.354938 ml_logger-0.9.8/ml_logger/log_client.py
--rw-r--r--   0        0        0   102434 2023-02-04 23:43:23.013332 ml_logger-0.9.8/ml_logger/ml_logger.py
--rw-r--r--   0        0        0     2235 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/nb.py
--rw-r--r--   0        0        0     3235 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/requests.py
--rw-r--r--   0        0        0      473 2021-12-23 17:37:45.000000 ml_logger-0.9.8/ml_logger/serdes.py
--rw-r--r--   0        0        0    21457 2022-11-16 04:29:13.355882 ml_logger-0.9.8/ml_logger/server.py
--rw-r--r--   0        0        0     1359 2022-11-16 04:29:13.356020 ml_logger-0.9.8/ml_logger/structs.py
--rw-r--r--   0        0        0       38 2022-01-26 17:58:03.658633 ml_logger-0.9.8/ml_logger/wrappers/__init__.py
--rw-r--r--   0        0        0     2045 2022-01-27 03:53:48.745709 ml_logger-0.9.8/ml_logger/wrappers/analysis_wrapper.py
--rw-r--r--   0        0        0     2777 2023-04-03 15:14:39.419599 ml_logger-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    24824 1970-01-01 00:00:00.000000 ml_logger-0.9.8/setup.py
--rw-r--r--   0        0        0    24524 1970-01-01 00:00:00.000000 ml_logger-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1523 2021-12-23 17:37:45.000000 ml_logger-0.9.9/LICENSE.md
+-rw-r--r--   0        0        0    22970 2022-12-05 02:36:36.448538 ml_logger-0.9.9/README.md
+-rw-r--r--   0        0        0    13191 2023-04-03 06:23:26.297176 ml_logger-0.9.9/ml_logger/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/caches/__init__.py
+-rw-r--r--   0        0        0      683 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/caches/key_value_cache.py
+-rw-r--r--   0        0        0     8541 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/caches/summary_cache.py
+-rw-r--r--   0        0        0     2529 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/full_duplex.py
+-rw-r--r--   0        0        0     3842 2022-07-24 14:29:59.384948 ml_logger-0.9.9/ml_logger/helpers/__init__.py
+-rw-r--r--   0        0        0     1520 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/helpers/color_helpers.py
+-rw-r--r--   0        0        0      646 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/helpers/data_helpers.py
+-rw-r--r--   0        0        0     1088 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/helpers/default_set.py
+-rw-r--r--   0        0        0      188 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/helpers/file_helpers.py
+-rw-r--r--   0        0        0     2269 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/helpers/func_helpers.py
+-rw-r--r--   0        0        0     3354 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/helpers/print_utils.py
+-rw-r--r--   0        0        0    15060 2022-11-16 04:29:13.354938 ml_logger-0.9.9/ml_logger/log_client.py
+-rw-r--r--   0        0        0   102434 2023-02-04 23:43:23.013332 ml_logger-0.9.9/ml_logger/ml_logger.py
+-rw-r--r--   0        0        0     2235 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/nb.py
+-rw-r--r--   0        0        0     3235 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/requests.py
+-rw-r--r--   0        0        0      473 2021-12-23 17:37:45.000000 ml_logger-0.9.9/ml_logger/serdes.py
+-rw-r--r--   0        0        0    21457 2022-11-16 04:29:13.355882 ml_logger-0.9.9/ml_logger/server.py
+-rw-r--r--   0        0        0     1359 2022-11-16 04:29:13.356020 ml_logger-0.9.9/ml_logger/structs.py
+-rw-r--r--   0        0        0       38 2022-01-26 17:58:03.658633 ml_logger-0.9.9/ml_logger/wrappers/__init__.py
+-rw-r--r--   0        0        0     2045 2022-01-27 03:53:48.745709 ml_logger-0.9.9/ml_logger/wrappers/analysis_wrapper.py
+-rw-r--r--   0        0        0     2791 2023-04-03 15:46:02.314056 ml_logger-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    24824 1970-01-01 00:00:00.000000 ml_logger-0.9.9/setup.py
+-rw-r--r--   0        0        0    24524 1970-01-01 00:00:00.000000 ml_logger-0.9.9/PKG-INFO
```

### Comparing `ml_logger-0.9.8/LICENSE.md` & `ml_logger-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/README.md` & `ml_logger-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/__init__.py` & `ml_logger-0.9.9/ml_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/caches/key_value_cache.py` & `ml_logger-0.9.9/ml_logger/caches/key_value_cache.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/caches/summary_cache.py` & `ml_logger-0.9.9/ml_logger/caches/summary_cache.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/full_duplex.py` & `ml_logger-0.9.9/ml_logger/full_duplex.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/helpers/__init__.py` & `ml_logger-0.9.9/ml_logger/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/helpers/color_helpers.py` & `ml_logger-0.9.9/ml_logger/helpers/color_helpers.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/helpers/data_helpers.py` & `ml_logger-0.9.9/ml_logger/helpers/data_helpers.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/helpers/default_set.py` & `ml_logger-0.9.9/ml_logger/helpers/default_set.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/helpers/func_helpers.py` & `ml_logger-0.9.9/ml_logger/helpers/func_helpers.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/helpers/print_utils.py` & `ml_logger-0.9.9/ml_logger/helpers/print_utils.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/log_client.py` & `ml_logger-0.9.9/ml_logger/log_client.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/ml_logger.py` & `ml_logger-0.9.9/ml_logger/ml_logger.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/nb.py` & `ml_logger-0.9.9/ml_logger/nb.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/requests.py` & `ml_logger-0.9.9/ml_logger/requests.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/server.py` & `ml_logger-0.9.9/ml_logger/server.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/structs.py` & `ml_logger-0.9.9/ml_logger/structs.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/ml_logger/wrappers/analysis_wrapper.py` & `ml_logger-0.9.9/ml_logger/wrappers/analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_logger-0.9.8/pyproject.toml` & `ml_logger-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,26 @@
 
 [project.scripts]
 # Note, add entrypoint name to scripts/completions/install.py to include CLI completion
 ml-download = "ml_scripts.download:entrypoint"
 ml-upload= "ml_scripts.upload:entrypoint"
 
 [tool.setuptools.packages.find]
-include = ["ml_logger"]
+include = ["ml_logger", "ml_scripts"]
 
 [tool.setuptools.package-data]
 "*" = []
 
 # black
 [tool.black]
 line-length = 140
 
 [tool.poetry]
 name = "ml-logger"
-version = "0.9.8"
+version = "0.9.9"
 description = ""
 authors = ["Ge Yang <geyang@mit.edu>"]
 keywords = ["ml_logger", "visualization", "logging", "debug", "debugging"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Science/Research",
```

### Comparing `ml_logger-0.9.8/setup.py` & `ml_logger-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 entry_points = \
 {'console_scripts': ['ml-download = ml_scripts.download:entrypoint',
                      'ml-upload = ml_scripts.upload:entrypoint']}
 
 setup_kwargs = {
     'name': 'ml-logger',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': '',
     'long_description': '# ML-Logger, A Simple and Scalable Logging Utility With a Beautiful Visualization Dashboard That Is Super Fast\n\n[![Downloads](http://pepy.tech/badge/ml-logger)](http://pepy.tech/project/ml-logger)\n\n<img alt="fast" src="figures/ml-dash-v3.gif" align="right" width="50%"/>\n\nML-Logger makes it easy to:\n\n- save data locally and remotely, as **binary**, in a transparent `pickle` file, with the same API and zero \nconfiguration.\n- write from 500+ worker containers to a single instrumentation server\n- visualize `matplotlib.pyplot` figures from a remote server locally with `logger.savefig(\'my_figure.png\')`\n\nAnd ml-logger does all of these with *minimal configuration* — you can use the same logging \ncode both locally and remotely with no code change.\n\nML-logger is highly performant -- the remote writes are asynchronous. For this reason it doesn\'t slow down your training\neven with 100+ metric keys.\n\nWhy did we built this, you might ask? Because we want to make it easy for people in ML to \nuse the same logging code in all of they projects, so that it is easy to get started with \nsomeone else\'s baseline.\n\n\n## Getting Started!\n\nTo **install** `ml_logger`, do:\n```bash\npip install ml-logger\n```\n\n> The landscape of python modules is a lot messier than that of javascript. The most up-to-date `graphene`\xa0requires the following versions:\n> \n> ```\n> yes | pip install graphene==2.1.3\n> yes | pip install graphql-core==2.1\n> yes | pip install graphql-relay==0.4.5\n> yes | pip install graphql-server-core==1.1.1\n> ```\n\nNow you can rock!\n\n```python\nfrom ml_logger import logger\n\nprint(logger)\n# ~> logging data to /tmp/ml-logger-debug\n```\nLog key/value pairs, and metrics:\n```python\nfor i in range(1):\n    logger.log(metrics={\'some_val/smooth\': 10, \'status\': f"step ({i})"}, reward=20, timestep=i)\n    ### flush the data, otherwise the value would be overwritten with new values in the next iteration.\n    logger.flush()\n# outputs ~>\n# ╒════════════════════╤════════════════════════════╕\n# │       reward       │             20             │\n# ├────────────────────┼────────────────────────────┤\n...\n```\n\n## Simple Logging Example\n\nIn your project files, do:\n\n```python\nfrom params_proto import ParamsProto, Proto, Flag\n\nclass Args(ParamsProto):\n    """ CLI Args for the program\n    Try:\n        python3 example.py --help\n    And it should print out the help strings\n    """\n    seed = Proto(1, help="random seed")\n    D_lr = 5e-4\n    G_lr = 1e-4\n    Q_lr = 1e-4\n    T_lr = 1e-4\n    plot_interval = 10\n    verbose = Flag("the verbose flag")\n\nif __name__ == \'__main__\':\n    import scipy\n    import numpy as np\n    from ml_logger import logger, LOGGER_USER\n\n    # Put in your ~/.bashrc\n    # export ML_LOGGER_ROOT = "http://<your-logging-server>:8081"\n    # export ML_LOGGER_USER = $USER\n    logger.configure(prefix=f"{LOGGER_USER}/scratch/your-experiment-prefix!")\n\n\n    logger.log_params(Args=vars(Args))\n    logger.upload_file(__file__)\n\n    for epoch in range(10):\n        logger.log(step=epoch, D_loss=0.2, G_loss=0.1, mutual_information=0.01)\n        logger.log_key_value(epoch, \'some string key\', 0.0012)\n        # when the step index updates, logger flushes all of the key-value pairs to file system/logging server\n\n    logger.flush()\n\n    # Images\n    face = scipy.misc.face()\n    face_bw = scipy.misc.face(gray=True)\n    logger.save_image(face, "figures/face_rgb.png")\n    logger.save_image(face_bw, "figures/face_bw.png")\n    image_bw = np.zeros((64, 64, 1))\n    image_bw_2 = scipy.misc.face(gray=True)[::4, ::4]\n\n    logger.save_video([face] * 5, "videos/face.mp4")\n```\n\nAnd it should print out\n\n\n```bash\n✓ created a new logging client\nDashboard: http://app.dash.ml/user-name/your-experiment-prefix!\nLog_directory: http://<your-server-ip>:8080\n══════════════════════════════════════════\n        Args        \n────────────────────┬─────────────────────\n        seed        │ 1                   \n        D_lr        │ 0.0005              \n        G_lr        │ 0.0001              \n        Q_lr        │ 0.0001              \n        T_lr        │ 0.0001              \n   plot_interval    │ 10                  \n════════════════════╧═════════════════════\n╒════════════════════╤════════════════════╕\n│        step        │         9          │\n├────────────────────┼────────────────────┤\n│       D loss       │       0.200        │\n├────────────────────┼────────────────────┤\n│       G loss       │       0.100        │\n├────────────────────┼────────────────────┤\n│ mutual information │       0.010        │\n╘════════════════════╧════════════════════╛\n\n\nProcess finished with exit code 0\n```\n\n### To View the Results\n\n[![ML-Logger Dashboard](figures/app-dash-ml_setup.png)](https://app.dash.ml/)\n\nNote, the `jwt` based access control has not been implemented yet. So you should leave the token field empty.\n\n### Logging to a Server\n\n**Skip this if you just want to log locally.** When training in parallel, you want to kickstart an logging server (Instrument Server). To do so, run:\n```bash\npython -m ml_logger.server\n```\nUse ssh tunnel if you are running on a managed cluster (with SLURM for instance).\n**Important**: to set allow remote logging, you need to pass in `--host=0.0.0.0` so that the server accepts non-localhost connections.\n\n```bash\npython -m ml_logger.server --host=0.0.0.0\n```\n\n### Asynchronously log the summary of LOTs of training metrics\n\nA common scenario is you only want to upload averaged statistics of your metrics. A pattern\nthat @jachiam uses is the following: `store_metrics()`, `peak_stored_metrics()`, and `log_metrics_summary()`\n\n```python\n# You log lots of metrics during training.\nfor i in range(100):\n    logger.store_metrics(metrics={\'some_val/smooth\': 10}, some=20, timestep=i)\n# you can peak what\'s inside the cache and print out a table like this: \nlogger.peek_stored_metrics(len=4)\n# outputs ~>\n#      some      |   timestep    |some_val/smooth\n# ━━━━━━━━━━━━━━━┿━━━━━━━━━━━━━━━┿━━━━━━━━━━━━━━━\n#       20       |       0       |      10\n#       20       |       1       |      10\n#       20       |       2       |      10\n#       20       |       3       |      10\n\n# The metrics are stored in-memory. Now we need to actually log the summaries:\nlogger.log_metrics_summary(silent=True)\n# outputs ~> . (data is now logged to the server)\n```\n\n## Table of Contents\n\n- logging `matplotlib.pyplot` figures on an headless server\n- [documentation under construction]\n\n## How to Develop\n\nFirst clone repo, install dev dependencies, and install the module under evaluation mode.\n```bash\ngit clone https://github.com/episodeyang/ml_logger.git\ncd ml_logger && cd ml_logger && pip install -r requirements-dev.txt\npip install -e .\n```\n## Testing local-mode (without a server)\n\nYou should be inside ml_logger/ml_logger folder\n```bash\npwd # ~> ml_logger/ml_logger\nmake test\n```\n\n## Testing with a server (You need to do both for an PR)\n\nTo test with a live server, first run (in a separate console)\n```\npython -m ml_logger.server --data-dir /tmp/ml-logger-debug\n```\nor do:\n```bash\nmake start-test-server\n```\n\nThen run this test script with the option:\n```bash\npython -m pytest tests --capture=no --data-dir http://0.0.0.0:8081\n```\nor do\n```bash\nmake test-with-server\n```\n\nYour PR should have both of these two tests working. ToDo: add CI to this repo.\n\n### To Publish\n\nYou need `twine`, `rst-lint` etc, which are included in the `requirements-dev.txt` file.\n\n---\n\n### Logging Matplotlib pyplots\n\n### Configuring The Experiment Folder\n\n```python\nfrom ml_logger import logger, ML_Logger\nfrom datetime import datetime\n\nnow = datetime.now()\nlogger.configure("/tmp/ml-logger-demo", "deep_Q_learning", f"{now:%Y%m%d-%H%M%S}")\n```\nThis is a singleton pattern similar to `matplotlib.pyplot`. However, you could also use the logger constructor\n```python\nlogger = ML_Logger(root_dir="/tmp/ml-logger-demo", prefix=f"deep_Q_learning/{now:%Y%m%d-%H%M%S}")\n```\n\n### Logging Text, and Metrics\n\n```python\nlogger.log({"some_var/smooth": 10}, some=Color(0.85, \'yellow\', percent), step=3)\n```\n\ncolored output: (where the values are yellow)\n```log\n╒════════════════════╤════════════════════╕\n│  some var/smooth   │         10         │\n├────────────────────┼────────────────────┤\n│        some        │       85.0%        │\n╘════════════════════╧════════════════════╛\n```\n\n### Logging Matplotlib Figures\n\nWe have optimized ML-Logger, so it supports any format that `pyplot` supports. To save a figure locally or remotely, \n```python\nimport matplotlib.pyplot as plt\nimport numpy as np\n\nxs = np.linspace(-5, 5)\n\nplt.plot(xs, np.cos(xs), label=\'Cosine Func\')\nlogger.savefig(\'cosine_function.pdf\')\n```\n\n### Logging Videos\n\nIt is especially hard to visualize RL training sessions on a remote computer. With ML-Logger this is easy, and \nsuper fast. We optimized the serialization and transport process, so that a large stack of video tensor gets\nfirst compressed by `ffmepg` before getting sent over the wire. \n\nThe compression rate (and speed boost) can be 2000:1.\n\n```python\nimport numpy as np\n\ndef im(x, y):\n    canvas = np.zeros((200, 200))\n    for i in range(200):\n        for j in range(200):\n            if x - 5 < i < x + 5 and y - 5 < j < y + 5:\n                canvas[i, j] = 1\n    return canvas\n\nframes = [im(100 + i, 80) for i in range(20)]\n\nlogger.log_video(frames, "test_video.mp4")\n```\n\n### Saving PyTorch Modules\n\nPyTorch has a very nice module saving and loading API that has inspired the one in `Keras`. We make it easy to save\nthis state dictionary (`state_dict`) to a server, and load it. This way you can load from 100+ of your previous \nexperiments, without having to download those weights to your code repository.\n\n```python\n# save a module\nlogger.save_module(cnn, "FastCNN.pkl")\n\n# load a module\nlogger.load_module(cnn, f"FastCNN.pkl")\n```\n\n### Saving Tensorflow Models\n\nThe format tensorflow uses to save the models is opaque. I prefer to save model weights in `pickle` as a dictionary. \nThis way the weight files are transparent. ML_Logger offers easy helper functions to save and load from checkpoints \nsaved in this format:\n\n```python\n## To save checkpoint\nfrom ml_logger import logger\nimport tensorflow as tf\n\nlogger.configure(log_directory="/tmp/ml-logger-demos")\n\nx = tf.get_variable(\'x\', shape=[], initializer=tf.constant_initializer(0.0))\ny = tf.get_variable(\'y\', shape=[], initializer=tf.constant_initializer(10.0))\nc = tf.Variable(1000)\n\nsess = tf.InteractiveSession()\nsess.run(tf.global_variables_initializer())\n\ntrainables = tf.trainable_variables()\nlogger.save_variables(trainables, path="variables.pkl", namespace="checkpoints")\n```\nwhich creates a file `checkpoints/variables.pkl` under `/tmp/ml-logger-demos`.\n\n## Visualization\n\nAn idea visualization dashboard would be\n1. **Fast, instantaneous.** On an AWS headless server? View the plots as if they are on your local computer.\n2. **Searchable, performantly.** So that you don\'t have to remember where an experiment is from last week.\n3. **Answer Questions, from 100+ Experiments.** We make available Google\'s internal hyperparameter visualization tool, \non your own computer.\n\n### Searching for Hyper Parameters\n\nExperiments are identified by the `metrics.pkl` file. You can log multiple times to the same `metrics.pkl` file, \nand the later parameter values overwrites earlier ones with the same key. We enforce namespace in this file, so each\nkey/value argument you pass into the `logger.log_parameters` function call has to be a dictionary.\n\n```python\nArgs = dict(\n    learning_rate=10,\n    hidden_size=200\n)\nlogger.log_parameters(Args=Args)\n```\n\n### How to launch the Vis App\n\n**This requires node.js and yarn dev environment** at the moment. We will streamline this process without these \nrequirements soon.\n\n0. download this repository\n1. go to `ml-vis-app` folder\n2. Install the dev dependencies\n    1. install node: [Installation](https://nodejs.org/en/download/)\n    2. install yarn: [Installation](https://yarnpkg.com/lang/en/docs/install/#mac-stable)\n    3. install the dependencies of this visualization app:\n        1. `yarn install`\n3. in that folder, run `yarn`.\n\n**The IP address of the server is currently hard coded \n[here](https://github.com/episodeyang/ml_logger/blob/master/ml-vis-app/src/App.js#L11).** To use this with your own \ninstrumentation server, over-write this line. I\'m planning on making this configuration more accessible.\n\n\n## Full Logging API\n\n```python\nfrom ml_logger import logger, Color, percent\n\nlogger.log_params(G=dict(some_config="hey"))\nlogger.log(some=Color(0.1, \'yellow\'), step=0)\nlogger.log(some=Color(0.28571, \'yellow\', lambda v: "{:.5f}%".format(v * 100)), step=1)\nlogger.log(some=Color(0.85, \'yellow\', percent), step=2)\nlogger.log({"some_var/smooth": 10}, some=Color(0.85, \'yellow\', percent), step=3)\nlogger.log(some=Color(10, \'yellow\'), step=4)\n```\n\ncolored output: (where the values are yellow)\n```log\n╒════════════════════╤════════════════════╕\n│        some        │        0.1         │\n╘════════════════════╧════════════════════╛\n╒════════════════════╤════════════════════╕\n│        some        │     28.57100%      │\n╘════════════════════╧════════════════════╛\n╒════════════════════╤════════════════════╕\n│        some        │       85.0%        │\n╘════════════════════╧════════════════════╛\n╒════════════════════╤════════════════════╕\n│  some var/smooth   │         10         │\n├────────────────────┼────────────────────┤\n│        some        │       85.0%        │\n╘════════════════════╧════════════════════╛\n```\n\nThis version of logger also prints out a tabular printout of the data you are logging to your `stdout`.\n- can silence `stdout` per key (per `logger.log` call)\n- can print with color: `logger.log(timestep, some_key=green(some_data))`\n- can print with custom formatting: `logger.log(timestep, some_key=green(some_data, percent))` where `percent`\n- uses the correct `unix` table characters (please stop using `|` and `+`. **Use `│`, `┼` instead**)\n\nA typical print out of this logger look like the following:\n\n```python\nfrom ml_logger import ML_Logger\n\nlogger = ML_Logger(root_dir=f"/mnt/bucket/deep_Q_learning/{datetime.now(%Y%m%d-%H%M%S.%f):}")\n\nlogger.log_params(G=vars(G), RUN=vars(RUN), Reporting=vars(Reporting))\n```\noutputs the following\n\n```log\n═════════════════════════════════════════════════════\n              G               \n───────────────────────────────┬─────────────────────\n           env_name            │ MountainCar-v0      \n             seed              │ None                \n      stochastic_action        │ True                \n         conv_params           │ None                \n         value_params          │ (64,)               \n        use_layer_norm         │ True                \n         buffer_size           │ 50000               \n      replay_batch_size        │ 32                  \n      prioritized_replay       │ True                \n            alpha              │ 0.6                 \n          beta_start           │ 0.4                 \n           beta_end            │ 1.0                 \n    prioritized_replay_eps     │ 1e-06               \n      grad_norm_clipping       │ 10                  \n           double_q            │ True                \n         use_dueling           │ False               \n     exploration_fraction      │ 0.1                 \n          final_eps            │ 0.1                 \n         n_timesteps           │ 100000              \n        learning_rate          │ 0.001               \n            gamma              │ 1.0                 \n        learning_start         │ 1000                \n        learn_interval         │ 1                   \ntarget_network_update_interval │ 500                 \n═══════════════════════════════╧═════════════════════\n             RUN              \n───────────────────────────────┬─────────────────────\n        log_directory          │ /mnt/slab/krypton/machine_learning/ge_dqn/2017-11-20/162048.353909-MountainCar-v0-prioritized_replay(True)\n          checkpoint           │ checkpoint.cp       \n           log_file            │ output.log          \n═══════════════════════════════╧═════════════════════\n          Reporting           \n───────────────────────────────┬─────────────────────\n     checkpoint_interval       │ 10000               \n        reward_average         │ 100                 \n        print_interval         │ 10                  \n═══════════════════════════════╧═════════════════════\n╒════════════════════╤════════════════════╕\n│      timestep      │        1999        │\n├────────────────────┼────────────────────┤\n│      episode       │         10         │\n├────────────────────┼────────────────────┤\n│    total reward    │       -200.0       │\n├────────────────────┼────────────────────┤\n│ total reward/mean  │       -200.0       │\n├────────────────────┼────────────────────┤\n│  total reward/max  │       -200.0       │\n├────────────────────┼────────────────────┤\n│time spent exploring│       82.0%        │\n├────────────────────┼────────────────────┤\n│    replay beta     │        0.41        │\n╘════════════════════╧════════════════════╛\n```\n\n\n## TODO:\n\n\n## Visualization (Preview):boom:\n\nIn addition, ml-logger also comes with a powerful visualization dashboard that beats tensorboard in every aspect.\n\n![ml visualization dashboard](./figures/ml_visualization_dashboard_preview.png)\n\n#### An Example Log from ML-Logger\n<img alt="example_real_log_output" src="figures/example_log_output.png" align="right"></img>\n\nA common pain that comes after getting to launch ML training jobs on AWS\nis a lack of a good way to manage and visualize your data. So far, a common\npractice is to upload your experiment data to aws s3 or google cloud buckets. \nThen one quickly realizes that downloading data from s3 can be slow. s3 does \n\nnot offer diffsync like gcloud-cli\'s `g rsync`. This makes it hard to sync a \nlarge collection of data that is constantly appended to.\n\nSo far the best way we have found for organizing experimental data is to \nhave a centralized instrumentation server. Compared with managing your data \non S3, a centralized instrumentation server makes it much easier to move \nexperiments around, run analysis that is co-located with your data, and \nhosting visualization dashboards on the same machine. To download data \nlocally, you can use `sshfs`, `smba`, `rsync` or a variety of remote disks. All\nfaster than s3.\n\nML-Logger is the logging utility that allows you to do this. To make ML_logger\neasy to use, we made it so that you can use ml-logger with zero configuration,\nlogging to your local hard-drive by default. When the logging directory field \n`logger.configure(log_directory= <your directory>)` is an http end point, \nthe logger will instantiate a fast, future based logging client that launches \nhttp requests in a separate thread. We optimized the client so that it won\'t \nslow down your training code.\n\nAPI wise, ML-logger makes it easy for you to log textual printouts, simple \nscalars, numpy tensors, image tensors, and `pyplot` figures. Because you might\nalso want to read data from the instrumentation server, we also made it possible to \nload numpy, pickle, text and binary files remotely.\n\nIn the future, we will start building an integrated dashboard with fast search, \nlive figure update and markdown-based reporting/dashboarding to go with ml-logger.\n\nNow give this a try, and profit!\n',
     'author': 'Ge Yang',
     'author_email': 'geyang@mit.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/geyang/ml-logger',
```

### Comparing `ml_logger-0.9.8/PKG-INFO` & `ml_logger-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-logger
-Version: 0.9.8
+Version: 0.9.9
 Summary: 
 Home-page: https://github.com/geyang/ml-logger
 License: MIT
 Keywords: ml_logger,visualization,logging,debug,debugging
 Author: Ge Yang
 Author-email: geyang@mit.edu
 Requires-Python: >=3.8.0
```

