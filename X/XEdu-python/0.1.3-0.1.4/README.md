# Comparing `tmp/XEdu-python-0.1.3.tar.gz` & `tmp/XEdu-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XEdu-python-0.1.3.tar", last modified: Wed Mar 20 12:28:47 2024, max compression
+gzip compressed data, was "dist/XEdu-python-0.1.4.tar", last modified: Fri Apr 19 08:28:00 2024, max compression
```

## Comparing `XEdu-python-0.1.3.tar` & `XEdu-python-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.164405 XEdu-python-0.1.3/
--rw-rw-r--   0 user      (1001) user      (1001)      192 2023-12-19 09:45:45.000000 XEdu-python-0.1.3/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      252 2024-03-20 12:28:47.164405 XEdu-python-0.1.3/PKG-INFO
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.156406 XEdu-python-0.1.3/XEdu/
--rw-rw-r--   0 user      (1001) user      (1001)     1160 2023-12-19 09:25:26.000000 XEdu-python-0.1.3/XEdu/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.156406 XEdu-python-0.1.3/XEdu/examples/
--rw-rw-r--   0 user      (1001) user      (1001)      138 2022-08-22 02:06:19.000000 XEdu-python-0.1.3/XEdu/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    14689 2024-03-20 12:25:52.000000 XEdu-python-0.1.3/XEdu/examples/demo.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.156406 XEdu-python-0.1.3/XEdu/hub/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.156406 XEdu-python-0.1.3/XEdu/hub/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-10-07 08:07:43.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    32512 2024-03-15 09:06:21.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    37314 2023-06-26 06:07:55.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    15668 2023-06-26 05:44:24.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 XEdu-python-0.1.3/XEdu/hub/BaseDT/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)    24028 2023-10-20 05:39:29.000000 XEdu-python-0.1.3/XEdu/hub/BaseDeploy.py
--rw-rw-r--   0 user      (1001) user      (1001)      124 2023-12-13 09:25:51.000000 XEdu-python-0.1.3/XEdu/hub/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)    35020 2023-12-18 08:16:14.000000 XEdu-python-0.1.3/XEdu/hub/datatset_class.py
--rw-r--r--   0 user      (1001) user      (1001)     1667 2024-01-31 10:22:57.000000 XEdu-python-0.1.3/XEdu/hub/errorcode.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.156406 XEdu-python-0.1.3/XEdu/hub/font/
--rw-rw-r--   0 user      (1001) user      (1001)  3241748 2023-10-25 09:32:52.000000 XEdu-python-0.1.3/XEdu/hub/font/FZYTK.TTF
--rw-rw-r--   0 user      (1001) user      (1001)   135758 2023-10-19 07:26:34.000000 XEdu-python-0.1.3/XEdu/hub/none.jpg
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.160405 XEdu-python-0.1.3/XEdu/hub/tokenizer/
--rw-r--r--   0 user      (1001) user      (1001)       53 2023-12-18 07:23:59.000000 XEdu-python-0.1.3/XEdu/hub/tokenizer/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)  1356917 2023-12-12 09:36:39.000000 XEdu-python-0.1.3/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 user      (1001) user      (1001)    13159 2023-12-13 09:25:30.000000 XEdu-python-0.1.3/XEdu/hub/tokenizer/clip_tokenizer.py
--rw-r--r--   0 user      (1001) user      (1001)    24841 2023-12-18 08:05:47.000000 XEdu-python-0.1.3/XEdu/hub/tokenizer/qa_squadprocess.py
--rw-r--r--   0 user      (1001) user      (1001)    12359 2023-11-07 13:19:31.000000 XEdu-python-0.1.3/XEdu/hub/tokenizer/qa_tokenizer.py
--rw-r--r--   0 user      (1001) user      (1001)   231508 2018-10-18 22:21:12.000000 XEdu-python-0.1.3/XEdu/hub/tokenizer/qa_vocab.txt
--rw-rw-r--   0 user      (1001) user      (1001)    73413 2024-03-20 12:28:04.000000 XEdu-python-0.1.3/XEdu/hub/workflow.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.160405 XEdu-python-0.1.3/XEdu/utils/
--rw-r--r--   0 user      (1001) user      (1001)       20 2023-12-13 09:36:29.000000 XEdu-python-0.1.3/XEdu/utils/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     3723 2023-12-14 06:42:53.000000 XEdu-python-0.1.3/XEdu/utils/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)     2230 2024-03-20 12:28:34.000000 XEdu-python-0.1.3/XEdu/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 12:28:47.164405 XEdu-python-0.1.3/XEdu_python.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      252 2024-03-20 12:28:47.000000 XEdu-python-0.1.3/XEdu_python.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      964 2024-03-20 12:28:47.000000 XEdu-python-0.1.3/XEdu_python.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-03-20 12:28:47.000000 XEdu-python-0.1.3/XEdu_python.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       45 2024-03-20 12:28:47.000000 XEdu-python-0.1.3/XEdu_python.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       93 2024-03-20 12:28:47.000000 XEdu-python-0.1.3/XEdu_python.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        5 2024-03-20 12:28:47.000000 XEdu-python-0.1.3/XEdu_python.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-12-19 09:50:02.000000 XEdu-python-0.1.3/XEdu_python.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       92 2023-12-21 02:44:37.000000 XEdu-python-0.1.3/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-03-20 12:28:47.164405 XEdu-python-0.1.3/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3575 2024-03-20 12:28:28.000000 XEdu-python-0.1.3/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/
+-rw-rw-r--   0 user      (1001) user      (1001)      192 2023-12-19 09:45:45.000000 XEdu-python-0.1.4/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      252 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/PKG-INFO
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/
+-rw-rw-r--   0 user      (1001) user      (1001)     1160 2023-12-19 09:25:26.000000 XEdu-python-0.1.4/XEdu/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)      138 2022-08-22 02:06:19.000000 XEdu-python-0.1.4/XEdu/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    15534 2024-04-19 08:07:10.000000 XEdu-python-0.1.4/XEdu/examples/demo.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-10-07 08:07:43.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    32512 2024-03-15 09:06:21.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37314 2023-06-26 06:07:55.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    15668 2023-06-26 05:44:24.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 XEdu-python-0.1.4/XEdu/hub/BaseDT/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)    24028 2023-10-20 05:39:29.000000 XEdu-python-0.1.4/XEdu/hub/BaseDeploy.py
+-rw-rw-r--   0 user      (1001) user      (1001)      124 2023-12-13 09:25:51.000000 XEdu-python-0.1.4/XEdu/hub/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)    35020 2023-12-18 08:16:14.000000 XEdu-python-0.1.4/XEdu/hub/datatset_class.py
+-rw-r--r--   0 user      (1001) user      (1001)     1667 2024-01-31 10:22:57.000000 XEdu-python-0.1.4/XEdu/hub/errorcode.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/font/
+-rw-rw-r--   0 user      (1001) user      (1001)  3241748 2023-10-25 09:32:52.000000 XEdu-python-0.1.4/XEdu/hub/font/FZYTK.TTF
+-rw-rw-r--   0 user      (1001) user      (1001)   135758 2023-10-19 07:26:34.000000 XEdu-python-0.1.4/XEdu/hub/none.jpg
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/
+-rw-r--r--   0 user      (1001) user      (1001)       53 2023-12-18 07:23:59.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)  1356917 2023-12-12 09:36:39.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 user      (1001) user      (1001)    13159 2023-12-13 09:25:30.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/clip_tokenizer.py
+-rw-r--r--   0 user      (1001) user      (1001)    24841 2023-12-18 08:05:47.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_squadprocess.py
+-rw-r--r--   0 user      (1001) user      (1001)    12359 2023-11-07 13:19:31.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_tokenizer.py
+-rw-r--r--   0 user      (1001) user      (1001)   231508 2018-10-18 22:21:12.000000 XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_vocab.txt
+-rw-rw-r--   0 user      (1001) user      (1001)    78428 2024-04-19 08:26:59.000000 XEdu-python-0.1.4/XEdu/hub/workflow.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu/utils/
+-rw-r--r--   0 user      (1001) user      (1001)       20 2023-12-13 09:36:29.000000 XEdu-python-0.1.4/XEdu/utils/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     3723 2023-12-14 06:42:53.000000 XEdu-python-0.1.4/XEdu/utils/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2230 2024-04-19 07:31:43.000000 XEdu-python-0.1.4/XEdu/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      252 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      964 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       45 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)      107 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        5 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/XEdu_python.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-12-19 09:50:02.000000 XEdu-python-0.1.4/XEdu_python.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      106 2024-04-19 07:30:10.000000 XEdu-python-0.1.4/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2024-04-19 08:28:00.000000 XEdu-python-0.1.4/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3575 2024-04-19 07:31:31.000000 XEdu-python-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `XEdu-python-0.1.3/XEdu/__init__.py` & `XEdu-python-0.1.4/XEdu/__init__.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/examples/demo.py` & `XEdu-python-0.1.4/XEdu/examples/demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     # print(result)
     re = cls.format_output(lang="zh")
 
 def baseml_demo():
     ml = wf(task='baseml',checkpoint="baseml_ckpt.pkl") # iris act 
     # result = ml.inference(data=[[1,0.5,-1,0]])
     # result = ml.inference(data=[1,0.5,-1,0])
-    result = ml.inference(data=[0.5])
+    result = ml.inference(data=np.array([[0.5,0,1,1]]))
 
 
     re = ml.format_output(lang="zh")
 
 def sup_demo():
     from transformers import AutoTokenizer
     from onnxruntime import InferenceSession
@@ -390,29 +390,41 @@
 
 
     # for single input models only
     result = compiled_model(input_data)[output_layer]
 
     print(result)
 
+def color_demo():
+    from XEdu.hub import Workflow as wf
+    color = wf(task='gen_color',download_path='new_download')# ,checkpoint='/home/user/下载/colorization-master/colorizer_siggraph17.onnx')
+    img = cv2.imread('/home/user/下载/colorization-master/imgs/ansel_adams3.jpg')
+    result = color.inference(data='/home/user/下载/colorization-master/imgs/ansel_adams3.jpg',img_type='pil')
+    color.save(result,"color_ou.jpg")
+
 
 if __name__ == "__main__":
     # pose_infer_demo()
     # det_infer_demo()
     # video_infer_demo()
     # hand_video_demo()
     # coco_det_demo()
     # hand_det_demo()
     # face_det_demo()
     # ocr_demo()
     # mmedu_demo()
     # custom_demo()
     # basenn_demo()
     # cls_demo()
-    baseml_demo()
+    # baseml_demo()
     # style_demo()
     # qa_demo()
     # drive_demo()
     # embedding_demo()
- 
+    color_demo()
+    # from openxlab.model import download
+    # download(model_repo='xedu/hub-model', model_name='gen_color.onnx')
+    # url = "https://download.openxlab.org.cn/repos/file/xedu/hub-model/main?filepath=gen_color.onnx&sign=2838feb49073bb8f756d57a9f78a68ab&nonce=1713425582020"
+    # path = "git-lfs/gen_color.onnx"
+    # downloader = Downloader(url, path)
+    # downloader.start()
 
-
```

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDT/data.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDT/data.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDT/data_image.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDT/dataset.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDT/dataset.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDT/io.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDT/plot.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDT/plot.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDT/utils.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDT/utils.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/BaseDeploy.py` & `XEdu-python-0.1.4/XEdu/hub/BaseDeploy.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/datatset_class.py` & `XEdu-python-0.1.4/XEdu/hub/datatset_class.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/errorcode.py` & `XEdu-python-0.1.4/XEdu/hub/errorcode.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/font/FZYTK.TTF` & `XEdu-python-0.1.4/XEdu/hub/font/FZYTK.TTF`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/none.jpg` & `XEdu-python-0.1.4/XEdu/hub/none.jpg`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz` & `XEdu-python-0.1.4/XEdu/hub/tokenizer/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/tokenizer/clip_tokenizer.py` & `XEdu-python-0.1.4/XEdu/hub/tokenizer/clip_tokenizer.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/tokenizer/qa_squadprocess.py` & `XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_squadprocess.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/tokenizer/qa_tokenizer.py` & `XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_tokenizer.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/tokenizer/qa_vocab.txt` & `XEdu-python-0.1.4/XEdu/hub/tokenizer/qa_vocab.txt`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/hub/workflow.py` & `XEdu-python-0.1.4/XEdu/hub/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import os
 from PIL import Image
 from .tokenizer.qa_tokenizer import *
 from .tokenizer.qa_squadprocess import *
 from .tokenizer.clip_tokenizer import Preprocessor, Tokenizer
 from .datatset_class import coco_class,imagenet_class
 import copy
+import requests
+from tqdm import tqdm
 
 from .errorcode import ErrorCodeFactory as ecf
 T = TypeVar("T")
 
 def to_batches(items: Iterable[T], size: int) -> Iterator[List[T]]:
     """
     Splits an iterable (e.g. a list) into batches of length `size`. Includes
@@ -69,22 +71,56 @@
         "det_hand":"handdetect.onnx",
         "cls_imagenet":"imagenet1k.onnx",
         "gen_style":"gen_style_mosaic.onnx",
         "nlp_qa":"nlp_qa.onnx",
         "drive_perception":"drive_perception.onnx",
         "embedding_image":"embedding_image.onnx",
         "embedding_text":"embedding_text.onnx",
+        "gen_color":"gen_color.onnx",
         "det_face":"...",
         "ocr":"...",
         "mmedu":"...",
         "basenn":"...",
         "baseml":"...",
 }
 style_list = ['mosaic','candy','rain-princess','udnie','pointilism']
 
+class Downloader(object):
+    def __init__(self, url, file_path,model_name=None,output_dir='checkpoints',overwrite=False):
+        self.url = url
+        self.file_path = file_path
+        if model_name is None:
+            self.model_name = os.path.basename(file_path)
+        else:
+            self.model_name = model_name
+        self.output_dir = output_dir
+
+    def start(self):
+        res_length = requests.get(self.url, stream=True)
+        total_size = int(res_length.headers['Content-Length'])
+        if os.path.exists(self.file_path):
+            temp_size = os.path.getsize(self.file_path)
+        else:
+            temp_size = 0
+        print(f"model_repo:xedu/hub-model, model_name:{self.model_name}, output:{self.output_dir}, overwrite:False")
+        headers = {'Range': 'bytes=%d-' % temp_size,
+                   "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:81.0) Gecko/20100101 Firefox/81.0"}
+        res_left = requests.get(self.url, stream=True, headers=headers)
+        total_size_in_bytes = int(res_left.headers['Content-Length'])
+        progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
+
+        with open(self.file_path, "ab") as f:
+            for chunk in res_left.iter_content(chunk_size=1024):
+                temp_size += len(chunk)
+                progress_bar.update(len(chunk))
+                f.write(chunk)
+                
+        progress_bar.close()
+        print(f"download model repo:xedu/hub-model, file_name:{self.model_name} ")
+
 class Workflow:
     """
         Workflow类用于加载预训练模型以解决各类任务。
         目前支持的任务有：
             - pose_body17：人体关键点检测，17个关键点
             - pose_body17_l：人体关键点检测，17个关键点，模型更大
             - pose_body26：人体关键点检测，26个关键点
@@ -175,15 +211,15 @@
             'l_purple':[128,0,128],
         }
         if self.task == 'nlp_qa':
             self.answers = []
             self.questions = []
             self.contexts = []
             self.doc = None
-        default_task = ['det_body','det_body_l','det_coco','det_coco_l','pose_body17','pose_body17_l','pose_body26','pose_wholebody133','pose_face106','pose_hand21','det_hand','cls_imagenet','gen_style','nlp_qa','drive_perception','embedding_image','embedding_text']
+        default_task = ['det_body','det_body_l','det_coco','det_coco_l','pose_body17','pose_body17_l','pose_body26','pose_wholebody133','pose_face106','pose_hand21','det_hand','cls_imagenet','gen_style','nlp_qa','drive_perception','embedding_image','embedding_text','gen_color']
         if checkpoint is None and self.task in default_task: # 若不指定权重文件，则使用对应任务的默认模型
             if self.task == 'gen_style':
                 self.style = kwargs.get('style',None)
                 if isinstance(self.style,int): # 按照索引选择风格
                     style_map = ['mosaic','candy','rain-princess','udnie','pointilism']
                     self.style = style_map[self.style]
                 elif isinstance(self.style,str) and self.style not in ['mosaic','candy','rain-princess','udnie','pointilism']: # 自定义风格
@@ -192,15 +228,15 @@
                 if self.style is  None:
                     self.style = 'mosaic'
                 self.task = 'gen_style_{}'.format(self.style)
                 checkpoint = "gen_style_{}.onnx".format(self.style)
             else:
                 checkpoint = self.task_dict[self.task]
             checkpoint = os.path.join(path, checkpoint)
-            if not os.path.exists(checkpoint): # 下载默认模型
+            if not os.path.exists(checkpoint): # 本地未检测到模型，云端下载默认模型
                 print("本地未检测到{}任务对应模型，云端下载中...".format(self.task))
                 # path = "checkpoints"
                 if not os.path.exists(path):
                     os.mkdir(path)
                 model_name_map = {
                     "pose_body17":"17 body keypoints",
                     "pose_body17_l":"17 body keypoints large model",
@@ -222,16 +258,22 @@
                     "gen_style_pointilism":"pointilism style transfer",
                     "gen_style_custom":"custom style transfer",
                     "nlp_qa":"question answering",
                     "drive_perception":"drive perception",
                     "embedding_image":"clip_image",
                     "embedding_text":"clip_text",
                 }
-                # download('test12318/bert-english',model_name=model_name,output=path)
-                download(model_repo='xedu/hub-model', model_name=model_name_map[self.task],output=path)
+                model_name_map_download = {
+                    "gen_color":"https://download.openxlab.org.cn/repos/file/xedu/hub-model/main?filepath=gen_color.onnx&sign=2838feb49073bb8f756d57a9f78a68ab&nonce=1713425582020",
+                }
+                if self.task in model_name_map_download.keys():
+                    downloader = Downloader(model_name_map_download[self.task], os.path.join(path, self.task_dict[self.task]),output_dir=path)
+                    downloader.start()
+                else:
+                    download(model_repo='xedu/hub-model', model_name=model_name_map[self.task],output=path)
             # download()
             self.model = ort.InferenceSession(checkpoint, None)
 
         # model_path='rtmpose-ort/rtmpose-s-0b29a8.onnx'
         elif self.task =="det_face":
                 self.model = cv2.CascadeClassifier(cv2.data.haarcascades+'haarcascade_frontalface_default.xml')
         elif self.task == "ocr":
@@ -334,15 +376,85 @@
             return self._embedding_image_infer(data)
         elif self.task in ['embedding_text']:
             if isinstance(data, str): # 单个文本
                 data = [data]
             self._tokenizer = Tokenizer()
             self._batch_size = 16
             return self._embedding_text_infer(data)
+        elif self.task in ['gen_color']:
+            return self._gen_color_infer(data,show,img_type)
     
+    def _gen_color_infer(self,data=None,show=False,img_type=None):
+
+        def load_img(img_path):
+            if isinstance(img_path,str):
+                out_np = np.asarray(Image.open(img_path))
+            else:
+                out_np = np.asarray(img_path)
+            if(out_np.ndim==2):
+                out_np = np.tile(out_np[:,:,None],3)
+            return out_np
+
+        def resize_img(img, HW=(256,256), resample=3):
+            return np.asarray(Image.fromarray(img).resize((HW[1],HW[0]), resample=resample))
+
+        def preprocess_img(img_rgb_orig, HW=(256,256), resample=3):
+            img_rgb_rs = resize_img(img_rgb_orig, HW=HW, resample=resample)
+
+            img_rgb_orig = np.float32(img_rgb_orig * (1./255))
+            img_lab_orig = cv2.cvtColor(img_rgb_orig, cv2.COLOR_RGB2LAB)
+
+            img_rgb_rs = np.float32(img_rgb_rs * (1./255))
+            img_lab_rs = cv2.cvtColor(img_rgb_rs, cv2.COLOR_BGR2LAB)
+
+            img_l_orig = img_lab_orig[:,:,0]
+            img_l_rs = img_lab_rs[:,:,0]
+
+            tens_orig_l = img_l_orig[None,None,:,:]
+            tens_rs_l = img_l_rs[None,None,:,:]
+
+            return (tens_orig_l, tens_rs_l)
+
+        def postprocess_tens(tens_orig_l, out_ab, mode='bilinear'):
+            HW_orig = tens_orig_l.shape[2:]
+            HW = out_ab.shape[2:]
+
+            if(HW_orig[0]!=HW[0] or HW_orig[1]!=HW[1]):
+                # out_ab_orig = F.interpolate(out_ab, size=HW_orig, mode='bilinear')
+                out_a = cv2.resize(out_ab[0,0,:,:], (HW_orig[1], HW_orig[0]), interpolation=cv2.INTER_LINEAR)
+                out_b = cv2.resize(out_ab[0,1,:,:], (HW_orig[1], HW_orig[0]), interpolation=cv2.INTER_LINEAR)
+                out_ab_orig = np.concatenate(([out_a],[out_b]),axis=0)
+                out_ab_orig = out_ab_orig[None,...]
+            else:
+                out_ab_orig = out_ab
+
+            out_lab_orig = np.concatenate((tens_orig_l, out_ab_orig), axis=1)
+
+            return cv2.cvtColor(out_lab_orig[0,...].transpose((1,2,0)), cv2.COLOR_LAB2RGB)
+
+        input_name = self.model.get_inputs()[0].name
+        output_name = self.model.get_outputs()[0].name
+        img = load_img(data)
+        (tens_l_orig, tens_l_rs) = preprocess_img(img, HW=(256,256))
+        input_data = tens_l_rs
+        output_data = self.model.run([output_name], {input_name: input_data})[0]
+        color_res = postprocess_tens(tens_l_orig, output_data)
+
+        if img_type:
+            self._get_img = img_type
+            if img_type =='cv2':
+                # image = cv2.cvtcolor(image,cv2.BGR2RGB)
+                color_res = cv2.cvtColor(color_res,cv2.COLOR_BGR2RGB)
+            if show:
+                self.show(color_res)
+            return color_res,color_res
+        else:
+            self._get_img = 'pil'
+        return color_res
+
     def _empty_embedding(self):
         return np.empty((0, 512), dtype=np.float32)
 
     def _embedding_image_infer(self,images: Iterable[Union[Image.Image, np.ndarray]],with_batching: bool = True,):
         """Compute the embeddings for a list of images.
 
         Args:
@@ -495,15 +607,14 @@
         return results
 
     def load_context(self,context):
         self.context = context
         self.doc = read_squad_examples_context(input_data=context)
         return self.doc 
 
-
     def _nlp_qa_infer(self,data=None,context=None):
         if context is not None:
             self.contexts.append(context)
             doc = read_squad_examples_context(input_data=context)
         else:
             if self.doc is None:
                 raise Exception(ecf.LOAD_CONTEXT_BEFORE_INFER())
@@ -561,15 +672,14 @@
         res, answer = write_predictions(eval_examples, extra_data, all_results,
                         n_best_size, max_answer_length,True)
         res = dict(res)["1"]
         self.answers.append(answer)
         return res
     
     def _baseml_infer(self,data=None, show=None, img_type=None):
-        print(self.input_shape)
         if data is not None and self.input_shape is not None: 
             model_input_shape = str(self.input_shape).replace(str(self.input_shape[0]), 'batch')
             assert type(self.demo_input) == type(data), f"Error Code: -309. The data type {type(data)} doesn't match the model input type {type(self.demo_input)}. Example input: {self.demo_input.tolist()}."
             assert self.input_shape[1:] == data.shape[1:], f"Error Code: -309. The data shape {data.shape} doesn't match the model input shape {model_input_shape}. Example input: {self.demo_input.tolist()}."
 
         self.baseml_res = self.model.predict(data)
         if img_type is not None:
@@ -1076,14 +1186,16 @@
             if isinstance(img,tuple):
                 img = img[1]
             cv2.imwrite(save_path,img)
         elif self._get_img.lower() == 'pil':
             if isinstance(img,tuple):
                 img = img[1]
             img = img
+            if img.dtype != 'uint8':
+                img = (img*255).astype('uint8')
             a = Image.fromarray(img)
             a.save(save_path)
             # plt.imshow(img)
             # plt.axis('off')
             # plt.subplots_adjust(top=1,bottom=0,right=1,left=0,hspace=0,wspace=0)
             # plt.margins(0,0)
             # plt.savefig(save_path)
```

### Comparing `XEdu-python-0.1.3/XEdu/utils/utils.py` & `XEdu-python-0.1.4/XEdu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/XEdu/version.py` & `XEdu-python-0.1.4/XEdu/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.3'
+__version__='0.1.4'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `XEdu-python-0.1.3/XEdu_python.egg-info/SOURCES.txt` & `XEdu-python-0.1.4/XEdu_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `XEdu-python-0.1.3/setup.py` & `XEdu-python-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='XEdu-python',
-    version='0.1.3',
+    version='0.1.4',
     description='XEdu',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

