# Comparing `tmp/ultralytics-8.2.1.tar.gz` & `tmp/ultralytics-8.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.2.1.tar", last modified: Thu Apr 18 03:05:44 2024, max compression
+gzip compressed data, was "ultralytics-8.2.2.tar", last modified: Fri Apr 19 03:48:43 2024, max compression
```

## Comparing `ultralytics-8.2.1.tar` & `ultralytics-8.2.2.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.205335 ultralytics-8.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-18 03:04:01.000000 ultralytics-8.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40387 2024-04-18 03:05:44.205335 ultralytics-8.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36684 2024-04-18 03:04:01.000000 ultralytics-8.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-18 03:04:01.000000 ultralytics-8.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:05:44.205335 ultralytics-8.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.161336 ultralytics-8.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-18 03:04:01.000000 ultralytics-8.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-18 03:04:01.000000 ultralytics-8.2.1/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-18 03:04:01.000000 ultralytics-8.2.1/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 03:04:01.000000 ultralytics-8.2.1/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-18 03:04:01.000000 ultralytics-8.2.1/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    22960 2024-04-18 03:04:01.000000 ultralytics-8.2.1/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.161336 ultralytics-8.2.1/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.165336 ultralytics-8.2.1/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.165336 ultralytics-8.2.1/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.169336 ultralytics-8.2.1/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.157336 ultralytics-8.2.1/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.169336 ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.169336 ultralytics-8.2.1/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.169336 ultralytics-8.2.1/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.169336 ultralytics-8.2.1/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.173336 ultralytics-8.2.1/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.173336 ultralytics-8.2.1/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.173336 ultralytics-8.2.1/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.177336 ultralytics-8.2.1/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.177336 ultralytics-8.2.1/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.177336 ultralytics-8.2.1/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.181336 ultralytics-8.2.1/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54507 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34989 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.181336 ultralytics-8.2.1/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.181336 ultralytics-8.2.1/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.181336 ultralytics-8.2.1/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.181336 ultralytics-8.2.1/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.185335 ultralytics-8.2.1/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.185335 ultralytics-8.2.1/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.185335 ultralytics-8.2.1/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.185335 ultralytics-8.2.1/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.185335 ultralytics-8.2.1/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.185335 ultralytics-8.2.1/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.189335 ultralytics-8.2.1/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.189335 ultralytics-8.2.1/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.189335 ultralytics-8.2.1/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.189335 ultralytics-8.2.1/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.189335 ultralytics-8.2.1/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.189335 ultralytics-8.2.1/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.193336 ultralytics-8.2.1/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.193336 ultralytics-8.2.1/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.193336 ultralytics-8.2.1/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.193336 ultralytics-8.2.1/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.197336 ultralytics-8.2.1/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    39292 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.201336 ultralytics-8.2.1/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    47558 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-18 03:04:01.000000 ultralytics-8.2.1/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:05:44.201336 ultralytics-8.2.1/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40387 2024-04-18 03:05:44.000000 ultralytics-8.2.1/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-18 03:05:44.000000 ultralytics-8.2.1/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:05:44.000000 ultralytics-8.2.1/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 03:05:44.000000 ultralytics-8.2.1/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-18 03:05:44.000000 ultralytics-8.2.1/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 03:05:44.000000 ultralytics-8.2.1/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.182316 ultralytics-8.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-19 03:47:33.000000 ultralytics-8.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-19 03:48:43.182316 ultralytics-8.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36682 2024-04-19 03:47:33.000000 ultralytics-8.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-19 03:47:33.000000 ultralytics-8.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:48:43.182316 ultralytics-8.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-04-19 03:47:33.000000 ultralytics-8.2.2/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.146317 ultralytics-8.2.2/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    21312 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/african-wildlife.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/brain-tumor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/lvis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.138317 ultralytics-8.2.2/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.150317 ultralytics-8.2.2/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.154317 ultralytics-8.2.2/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-world.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.154317 ultralytics-8.2.2/ultralytics/cfg/models/v9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.154317 ultralytics-8.2.2/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.158317 ultralytics-8.2.2/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57741 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.158317 ultralytics-8.2.2/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.158317 ultralytics-8.2.2/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54507 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40019 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34987 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.162317 ultralytics-8.2.2/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29125 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.166317 ultralytics-8.2.2/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/models/yolo/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/world/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/models/yolo/world/train_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.170317 ultralytics-8.2.2/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/queue_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.174317 ultralytics-8.2.2/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.178316 ultralytics-8.2.2/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    39286 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.178316 ultralytics-8.2.2/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27971 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32717 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53518 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33309 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47332 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-19 03:47:33.000000 ultralytics-8.2.2/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:48:43.178316 ultralytics-8.2.2/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 03:48:43.000000 ultralytics-8.2.2/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.2.1/LICENSE` & `ultralytics-8.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/PKG-INFO` & `ultralytics-8.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.1
+Version: 8.2.2
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
@@ -164,15 +164,15 @@
 from ultralytics import YOLO
 
 # Load a model
 model = YOLO("yolov8n.yaml")  # build a new model from scratch
 model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
 # Use the model
-model.train(data="coco128.yaml", epochs=3)  # train the model
+model.train(data="coco8.yaml", epochs=3)  # train the model
 metrics = model.val()  # evaluate model performance on the validation set
 results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
 path = model.export(format="onnx")  # export the model to ONNX format
 ```
 
 See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/python) for more examples.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.1 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.2 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
@@ -95,15 +95,15 @@
 ``` `yolo` can be used for a variety of tasks and modes and accepts additional
 arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
 docs.ultralytics.com/usage/cli) for examples. ### Python YOLOv8 may also be
 used directly in a Python environment, and accepts the same [arguments](https:/
 /docs.ultralytics.com/usage/cfg/) as in the CLI example above: ```python from
 ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
 new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model model.train(data="coco128.yaml",
+(recommended for training) # Use the model model.train(data="coco8.yaml",
 epochs=3) # train the model metrics = model.val() # evaluate model performance
 on the validation set results = model("https://ultralytics.com/images/bus.jpg")
 # predict on an image path = model.export(format="onnx") # export the model to
 ONNX format ``` See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/
 python) for more examples. ### Notebooks Ultralytics provides interactive
 notebooks for YOLOv8, covering training, validation, tracking, and more. Each
 notebook is paired with a [YouTube](https://youtube.com/ultralytics) tutorial,
```

### Comparing `ultralytics-8.2.1/README.md` & `ultralytics-8.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 from ultralytics import YOLO
 
 # Load a model
 model = YOLO("yolov8n.yaml")  # build a new model from scratch
 model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
 # Use the model
-model.train(data="coco128.yaml", epochs=3)  # train the model
+model.train(data="coco8.yaml", epochs=3)  # train the model
 metrics = model.val()  # evaluate model performance on the validation set
 results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
 path = model.export(format="onnx")  # export the model to ONNX format
 ```
 
 See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/python) for more examples.
```

#### html2text {}

```diff
@@ -45,15 +45,15 @@
 ``` `yolo` can be used for a variety of tasks and modes and accepts additional
 arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
 docs.ultralytics.com/usage/cli) for examples. ### Python YOLOv8 may also be
 used directly in a Python environment, and accepts the same [arguments](https:/
 /docs.ultralytics.com/usage/cfg/) as in the CLI example above: ```python from
 ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
 new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model model.train(data="coco128.yaml",
+(recommended for training) # Use the model model.train(data="coco8.yaml",
 epochs=3) # train the model metrics = model.val() # evaluate model performance
 on the validation set results = model("https://ultralytics.com/images/bus.jpg")
 # predict on an image path = model.export(format="onnx") # export the model to
 ONNX format ``` See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/
 python) for more examples. ### Notebooks Ultralytics provides interactive
 notebooks for YOLOv8, covering training, validation, tracking, and more. Each
 notebook is paired with a [YouTube](https://youtube.com/ultralytics) tutorial,
```

### Comparing `ultralytics-8.2.1/pyproject.toml` & `ultralytics-8.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/tests/test_cli.py` & `ultralytics-8.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/tests/test_cuda.py` & `ultralytics-8.2.2/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/tests/test_engine.py` & `ultralytics-8.2.2/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/tests/test_explorer.py` & `ultralytics-8.2.2/tests/test_explorer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from ultralytics import Explorer
 from ultralytics.utils import ASSETS
 
 
 @pytest.mark.slow
 def test_similarity():
     """Test similarity calculations and SQL queries for correctness and response length."""
-    exp = Explorer()
+    exp = Explorer(data="coco8.yaml")
     exp.create_embeddings_table()
     similar = exp.get_similar(idx=1)
-    assert len(similar) == 25
-    similar = exp.get_similar(img=ASSETS / "zidane.jpg")
-    assert len(similar) == 25
-    similar = exp.get_similar(idx=[1, 2], limit=10)
-    assert len(similar) == 10
+    assert len(similar) == 4
+    similar = exp.get_similar(img=ASSETS / "bus.jpg")
+    assert len(similar) == 4
+    similar = exp.get_similar(idx=[1, 2], limit=2)
+    assert len(similar) == 2
     sim_idx = exp.similarity_index()
-    assert len(sim_idx) > 0
-    sql = exp.sql_query("WHERE labels LIKE '%person%'")
-    assert len(sql) > 0
+    assert len(sim_idx) == 4
+    sql = exp.sql_query("WHERE labels LIKE '%zebra%'")
+    assert len(sql) == 1
 
 
 @pytest.mark.slow
 def test_det():
     """Test detection functionalities and ensure the embedding table has bounding boxes."""
     exp = Explorer(data="coco8.yaml", model="yolov8n.pt")
     exp.create_embeddings_table(force=True)
```

### Comparing `ultralytics-8.2.1/tests/test_integrations.py` & `ultralytics-8.2.2/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/tests/test_python.py` & `ultralytics-8.2.2/tests/test_python.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,31 +636,36 @@
 
 @pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="YOLOWorld with CLIP is not supported in Python 3.12")
 def test_yolo_world():
     model = YOLO("yolov8s-world.pt")  # no YOLOv8n-world model yet
     model.set_classes(["tree", "window"])
     model(ASSETS / "bus.jpg", conf=0.01)
 
-    # Training from yaml
-    model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
-    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
-
     model = YOLO("yolov8s-worldv2.pt")  # no YOLOv8n-world model yet
-    # val
-    model.val(data="coco8.yaml", imgsz=32, save_txt=True, save_json=True)
-    # Training from pretrain
-    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
+    # Training from pretrain, evaluation process is included at the final stage of training.
+    # Use dota8.yaml which has less categories to reduce the inference time of CLIP model
+    model.train(
+        data="dota8.yaml",
+        epochs=1,
+        imgsz=32,
+        cache="disk",
+        batch=4,
+        close_mosaic=1,
+        name="yolo-world",
+        save_txt=True,
+        save_json=True,
+    )
 
     # test WorWorldTrainerFromScratch
     from ultralytics.models.yolo.world.train_world import WorldTrainerFromScratch
 
     model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
     model.train(
-        data={"train": {"yolo_data": ["coco8.yaml"]}, "val": {"yolo_data": ["coco8.yaml"]}},
-        epochs=2,
+        data={"train": {"yolo_data": ["dota8.yaml"]}, "val": {"yolo_data": ["dota8.yaml"]}},
+        epochs=1,
         imgsz=32,
         cache="disk",
-        batch=-1,
+        batch=4,
         close_mosaic=1,
         name="yolo-world",
         trainer=WorldTrainerFromScratch,
     )
```

### Comparing `ultralytics-8.2.1/ultralytics/__init__.py` & `ultralytics-8.2.2/ultralytics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.2.1"
+__version__ = "8.2.2"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `ultralytics-8.2.1/ultralytics/assets/bus.jpg` & `ultralytics-8.2.2/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/assets/zidane.jpg` & `ultralytics-8.2.2/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/__init__.py` & `ultralytics-8.2.2/ultralytics/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 
         Where   TASK (optional) is one of {TASKS}
                 MODE (required) is one of {MODES}
                 ARGS (optional) are any number of custom 'arg=value' pairs like 'imgsz=320' that override defaults.
                     See all ARGS at https://docs.ultralytics.com/usage/cfg or with 'yolo cfg'
 
     1. Train a detection model for 10 epochs with an initial learning_rate of 0.01
-        yolo train data=coco128.yaml model=yolov8n.pt epochs=10 lr0=0.01
+        yolo train data=coco8.yaml model=yolov8n.pt epochs=10 lr0=0.01
 
     2. Predict a YouTube video using a pretrained segmentation model at image size 320:
         yolo predict model=yolov8n-seg.pt source='https://youtu.be/LNwODJXcvt4' imgsz=320
 
     3. Val a pretrained detection model at batch-size 1 and image size 640:
-        yolo val model=yolov8n.pt data=coco128.yaml batch=1 imgsz=640
+        yolo val model=yolov8n.pt data=coco8.yaml batch=1 imgsz=640
 
     4. Export a YOLOv8n classification model to ONNX format at image size 224 by 128 (no TASK required)
         yolo export model=yolov8n-cls.pt format=onnx imgsz=224,128
 
     6. Explore your datasets using semantic search and SQL with a simple GUI powered by Ultralytics Explorer API
         yolo explorer
```

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/african-wildlife.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/african-wildlife.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/brain-tumor.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/brain-tumor.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/lvis.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/lvis.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.2.2/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/default.yaml` & `ultralytics-8.2.2/ultralytics/cfg/default.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Default training settings and hyperparameters for medium-augmentation COCO training
 
 task: detect # (str) YOLO task, i.e. detect, segment, classify, pose
 mode: train # (str) YOLO mode, i.e. train, val, predict, export, track, benchmark
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model: # (str, optional) path to model file, i.e. yolov8n.pt, yolov8n.yaml
-data: # (str, optional) path to data file, i.e. coco128.yaml
+data: # (str, optional) path to data file, i.e. coco8.yaml
 epochs: 100 # (int) number of epochs to train for
 time: # (float, optional) number of hours to train for, overrides epochs if supplied
 patience: 100 # (int) epochs to wait for no observable improvement for early stopping of training
 batch: 16 # (int) number of images per batch (-1 for AutoBatch)
 imgsz: 640 # (int | list) input images size as int for train and val modes, or list[w,h] for predict and export modes
 save: True # (bool) save train checkpoints and predict results
 save_period: -1 # (int) Save checkpoint every x epochs (disabled if < 1)
```

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-world.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-world.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8-worldv2.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8-worldv2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9c-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9c.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9e-seg.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/models/v9/yolov9e.yaml` & `ultralytics-8.2.2/ultralytics/cfg/models/v9/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.2.2/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.2.2/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/__init__.py` & `ultralytics-8.2.2/ultralytics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/annotator.py` & `ultralytics-8.2.2/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/augment.py` & `ultralytics-8.2.2/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/base.py` & `ultralytics-8.2.2/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/build.py` & `ultralytics-8.2.2/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/converter.py` & `ultralytics-8.2.2/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/dataset.py` & `ultralytics-8.2.2/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/explorer/explorer.py` & `ultralytics-8.2.2/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.2.2/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/explorer/utils.py` & `ultralytics-8.2.2/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/loaders.py` & `ultralytics-8.2.2/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/split_dota.py` & `ultralytics-8.2.2/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/data/utils.py` & `ultralytics-8.2.2/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/engine/exporter.py` & `ultralytics-8.2.2/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/engine/model.py` & `ultralytics-8.2.2/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/engine/predictor.py` & `ultralytics-8.2.2/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/engine/results.py` & `ultralytics-8.2.2/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/engine/trainer.py` & `ultralytics-8.2.2/ultralytics/engine/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Train a model on a dataset.
 
 Usage:
-    $ yolo mode=train model=yolov8n.pt data=coco128.yaml imgsz=640 epochs=100 batch=16
+    $ yolo mode=train model=yolov8n.pt data=coco8.yaml imgsz=640 epochs=100 batch=16
 """
 
 import gc
 import math
 import os
 import subprocess
 import time
```

### Comparing `ultralytics-8.2.1/ultralytics/engine/tuner.py` & `ultralytics-8.2.2/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/engine/validator.py` & `ultralytics-8.2.2/ultralytics/engine/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 """
 Check a model's accuracy on a test or val split of a dataset.
 
 Usage:
-    $ yolo mode=val model=yolov8n.pt data=coco128.yaml imgsz=640
+    $ yolo mode=val model=yolov8n.pt data=coco8.yaml imgsz=640
 
 Usage - formats:
     $ yolo mode=val model=yolov8n.pt                 # PyTorch
                           yolov8n.torchscript        # TorchScript
                           yolov8n.onnx               # ONNX Runtime or OpenCV DNN with dnn=True
                           yolov8n_openvino_model     # OpenVINO
                           yolov8n.engine             # TensorRT
```

### Comparing `ultralytics-8.2.1/ultralytics/hub/__init__.py` & `ultralytics-8.2.2/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/hub/auth.py` & `ultralytics-8.2.2/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/hub/session.py` & `ultralytics-8.2.2/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/hub/utils.py` & `ultralytics-8.2.2/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/fastsam/model.py` & `ultralytics-8.2.2/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/fastsam/predict.py` & `ultralytics-8.2.2/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.2.2/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/fastsam/utils.py` & `ultralytics-8.2.2/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/fastsam/val.py` & `ultralytics-8.2.2/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/nas/model.py` & `ultralytics-8.2.2/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/nas/predict.py` & `ultralytics-8.2.2/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/nas/val.py` & `ultralytics-8.2.2/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/rtdetr/model.py` & `ultralytics-8.2.2/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.2.2/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/rtdetr/train.py` & `ultralytics-8.2.2/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/rtdetr/val.py` & `ultralytics-8.2.2/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/amg.py` & `ultralytics-8.2.2/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/build.py` & `ultralytics-8.2.2/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/model.py` & `ultralytics-8.2.2/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.2.2/ultralytics/models/sam/modules/decoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.2.2/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.2.2/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.2.2/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.2.2/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/sam/predict.py` & `ultralytics-8.2.2/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/utils/loss.py` & `ultralytics-8.2.2/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/utils/ops.py` & `ultralytics-8.2.2/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.2.2/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.2.2/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.2.2/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.2.2/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.2.2/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.2.2/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/model.py` & `ultralytics-8.2.2/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.2.2/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.2.2/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.2.2/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.2.2/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.2.2/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.2.2/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.2.2/ultralytics/models/yolo/segment/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.2.2/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.2.2/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/world/train.py` & `ultralytics-8.2.2/ultralytics/models/yolo/world/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/models/yolo/world/train_world.py` & `ultralytics-8.2.2/ultralytics/models/yolo/world/train_world.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/__init__.py` & `ultralytics-8.2.2/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/autobackend.py` & `ultralytics-8.2.2/ultralytics/nn/autobackend.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,16 +230,19 @@
             check_version(trt.__version__, "7.0.0", hard=True)  # require tensorrt>=7.0.0
             if device.type == "cpu":
                 device = torch.device("cuda:0")
             Binding = namedtuple("Binding", ("name", "dtype", "shape", "data", "ptr"))
             logger = trt.Logger(trt.Logger.INFO)
             # Read file
             with open(w, "rb") as f, trt.Runtime(logger) as runtime:
-                meta_len = int.from_bytes(f.read(4), byteorder="little")  # read metadata length
-                metadata = json.loads(f.read(meta_len).decode("utf-8"))  # read metadata
+                try:
+                    meta_len = int.from_bytes(f.read(4), byteorder="little")  # read metadata length
+                    metadata = json.loads(f.read(meta_len).decode("utf-8"))  # read metadata
+                except UnicodeDecodeError:
+                    f.seek(0)  # engine file may lack embedded Ultralytics metadata
                 model = runtime.deserialize_cuda_engine(f.read())  # read engine
 
             # Model context
             try:
                 context = model.create_execution_context()
             except Exception as e:  # model is None
                 LOGGER.error(f"ERROR: TensorRT model exported with a different version than {trt.__version__}\n")
```

### Comparing `ultralytics-8.2.1/ultralytics/nn/modules/__init__.py` & `ultralytics-8.2.2/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/modules/block.py` & `ultralytics-8.2.2/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/modules/conv.py` & `ultralytics-8.2.2/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/modules/head.py` & `ultralytics-8.2.2/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/modules/transformer.py` & `ultralytics-8.2.2/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/modules/utils.py` & `ultralytics-8.2.2/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/nn/tasks.py` & `ultralytics-8.2.2/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/solutions/ai_gym.py` & `ultralytics-8.2.2/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.2.2/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/solutions/heatmap.py` & `ultralytics-8.2.2/ultralytics/solutions/heatmap.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/solutions/object_counter.py` & `ultralytics-8.2.2/ultralytics/solutions/object_counter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/solutions/queue_management.py` & `ultralytics-8.2.2/ultralytics/solutions/queue_management.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.2.2/ultralytics/solutions/speed_estimation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/basetrack.py` & `ultralytics-8.2.2/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/bot_sort.py` & `ultralytics-8.2.2/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.2.2/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/track.py` & `ultralytics-8.2.2/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.2.2/ultralytics/trackers/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.2.2/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/trackers/utils/matching.py` & `ultralytics-8.2.2/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/__init__.py` & `ultralytics-8.2.2/ultralytics/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         from ultralytics import YOLO
 
         # Load a model
         model = YOLO('yolov8n.yaml')  # build a new model from scratch
         model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
         # Use the model
-        results = model.train(data="coco128.yaml", epochs=3)  # train the model
+        results = model.train(data="coco8.yaml", epochs=3)  # train the model
         results = model.val()  # evaluate model performance on the validation set
         results = model('https://ultralytics.com/images/bus.jpg')  # predict on an image
         success = model.export(format='onnx')  # export the model to ONNX format
 
     3. Use the command line interface (CLI):
 
         YOLOv8 'yolo' CLI commands use the following syntax:
@@ -74,21 +74,21 @@
 
             Where   TASK (optional) is one of [detect, segment, classify]
                     MODE (required) is one of [train, val, predict, export]
                     ARGS (optional) are any number of custom 'arg=value' pairs like 'imgsz=320' that override defaults.
                         See all ARGS at https://docs.ultralytics.com/usage/cfg or with 'yolo cfg'
 
         - Train a detection model for 10 epochs with an initial learning_rate of 0.01
-            yolo detect train data=coco128.yaml model=yolov8n.pt epochs=10 lr0=0.01
+            yolo detect train data=coco8.yaml model=yolov8n.pt epochs=10 lr0=0.01
 
         - Predict a YouTube video using a pretrained segmentation model at image size 320:
             yolo segment predict model=yolov8n-seg.pt source='https://youtu.be/LNwODJXcvt4' imgsz=320
 
         - Val a pretrained detection model at batch-size 1 and image size 640:
-            yolo detect val model=yolov8n.pt data=coco128.yaml batch=1 imgsz=640
+            yolo detect val model=yolov8n.pt data=coco8.yaml batch=1 imgsz=640
 
         - Export a YOLOv8n classification model to ONNX format at image size 224 by 128 (no TASK required)
             yolo export model=yolov8n-cls.pt format=onnx imgsz=224,128
 
         - Run special commands:
             yolo help
             yolo checks
```

### Comparing `ultralytics-8.2.1/ultralytics/utils/autobatch.py` & `ultralytics-8.2.2/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/benchmarks.py` & `ultralytics-8.2.2/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/base.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.2.2/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/checks.py` & `ultralytics-8.2.2/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/dist.py` & `ultralytics-8.2.2/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/downloads.py` & `ultralytics-8.2.2/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/errors.py` & `ultralytics-8.2.2/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/files.py` & `ultralytics-8.2.2/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/instance.py` & `ultralytics-8.2.2/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/loss.py` & `ultralytics-8.2.2/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/metrics.py` & `ultralytics-8.2.2/ultralytics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/ops.py` & `ultralytics-8.2.2/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/patches.py` & `ultralytics-8.2.2/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/plotting.py` & `ultralytics-8.2.2/ultralytics/utils/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,20 +436,17 @@
 
         max_text_width = max([size[0] for size in t_sizes])
         max_text_height = max([size[1] for size in t_sizes])
 
         text_x = self.im.shape[1] - int(self.im.shape[1] * 0.025 + max_text_width)
         text_y = int(self.im.shape[0] * 0.025)
 
-        # Calculate dynamic gap between each count value based on the width of the image
-        dynamic_gap = max(1, self.im.shape[1] // 100) * tf
-
         for i, count in enumerate(counts):
             text_x_pos = text_x
-            text_y_pos = text_y + i * dynamic_gap  # Adjust vertical position with dynamic gap
+            text_y_pos = text_y + i * (max_text_height + 25 * tf)
 
             # Draw the border
             cv2.rectangle(
                 self.im,
                 (text_x_pos - (10 * tf), text_y_pos - (10 * tf)),
                 (text_x_pos + max_text_width + (10 * tf), text_y_pos + max_text_height + (10 * tf)),
                 count_bg_color,
@@ -464,16 +461,14 @@
                 0,
                 fontScale=self.sf,
                 color=count_txt_color,
                 thickness=self.tf,
                 lineType=cv2.LINE_AA,
             )
 
-            text_y_pos += tf * max_text_height
-
     @staticmethod
     def estimate_pose_angle(a, b, c):
         """
         Calculate the pose angle for object.
 
         Args:
             a (float) : The value of pose point a
```

### Comparing `ultralytics-8.2.1/ultralytics/utils/tal.py` & `ultralytics-8.2.2/ultralytics/utils/tal.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/torch_utils.py` & `ultralytics-8.2.2/ultralytics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/triton.py` & `ultralytics-8.2.2/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics/utils/tuner.py` & `ultralytics-8.2.2/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.2.2/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.2.1
+Version: 8.2.2
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
@@ -164,15 +164,15 @@
 from ultralytics import YOLO
 
 # Load a model
 model = YOLO("yolov8n.yaml")  # build a new model from scratch
 model = YOLO("yolov8n.pt")  # load a pretrained model (recommended for training)
 
 # Use the model
-model.train(data="coco128.yaml", epochs=3)  # train the model
+model.train(data="coco8.yaml", epochs=3)  # train the model
 metrics = model.val()  # evaluate model performance on the validation set
 results = model("https://ultralytics.com/images/bus.jpg")  # predict on an image
 path = model.export(format="onnx")  # export the model to ONNX format
 ```
 
 See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/python) for more examples.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.2.1 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.2.2 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
@@ -95,15 +95,15 @@
 ``` `yolo` can be used for a variety of tasks and modes and accepts additional
 arguments, i.e. `imgsz=640`. See the YOLOv8 [CLI Docs](https://
 docs.ultralytics.com/usage/cli) for examples. ### Python YOLOv8 may also be
 used directly in a Python environment, and accepts the same [arguments](https:/
 /docs.ultralytics.com/usage/cfg/) as in the CLI example above: ```python from
 ultralytics import YOLO # Load a model model = YOLO("yolov8n.yaml") # build a
 new model from scratch model = YOLO("yolov8n.pt") # load a pretrained model
-(recommended for training) # Use the model model.train(data="coco128.yaml",
+(recommended for training) # Use the model model.train(data="coco8.yaml",
 epochs=3) # train the model metrics = model.val() # evaluate model performance
 on the validation set results = model("https://ultralytics.com/images/bus.jpg")
 # predict on an image path = model.export(format="onnx") # export the model to
 ONNX format ``` See YOLOv8 [Python Docs](https://docs.ultralytics.com/usage/
 python) for more examples. ### Notebooks Ultralytics provides interactive
 notebooks for YOLOv8, covering training, validation, tracking, and more. Each
 notebook is paired with a [YouTube](https://youtube.com/ultralytics) tutorial,
```

### Comparing `ultralytics-8.2.1/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.2.2/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.2.1/ultralytics.egg-info/requires.txt` & `ultralytics-8.2.2/ultralytics.egg-info/requires.txt`

 * *Files identical despite different names*

