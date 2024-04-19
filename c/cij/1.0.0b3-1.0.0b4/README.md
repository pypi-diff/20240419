# Comparing `tmp/cij-1.0.0b3.tar.gz` & `tmp/cij-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cij-1.0.0b3.tar", last modified: Sat May 22 01:46:22 2021, max compression
+gzip compressed data, was "cij-1.0.0b4.tar", last modified: Fri Apr 19 14:16:29 2024, max compression
```

## Comparing `cij-1.0.0b3.tar` & `cij-1.0.0b4.tar`

### file list

```diff
@@ -1,92 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.907570 cij-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-05-22 01:46:14.000000 cij-1.0.0b3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     6917 2021-05-22 01:46:22.907570 cij-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5352 2021-05-22 01:46:14.000000 cij-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.899570 cij-1.0.0b3/cij/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/cij.py
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/fill.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/geotherm.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/modes.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8020 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/cli/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/core/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19152 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4920 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/full_modulus.py
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/mode_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)    10143 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/modulus_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/core/phonon_contribution/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/phonon_contribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11742 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/phonon_contribution/nonshear.py
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/phonon_contribution/shear.py
--rw-r--r--   0 runner    (1001) docker     (121)     6728 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/qha_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10446 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/data/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/data/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/cubic
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/hexagonal
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/monoclinic
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/orthorhombic
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/tetragonal6
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/tetragonal7
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/triclinic
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/trigonal6
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/constraints/trigonal7
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/data/default/
--rw-r--r--   0 runner    (1001) docker     (121)      545 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/default/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/data/output/
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/output/writer_rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/data/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     6426 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/data/schema/config.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/io/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/io/config/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/config/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/config/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/io/output/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/output/results_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.903570 cij-1.0.0b3/cij/io/traditional/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/traditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/traditional/elast_dat.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/traditional/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/traditional/qha_input.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/io/traditional/qha_output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.907570 cij-1.0.0b3/cij/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/misc/eig_sort_freqs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/misc/evec_disp2eig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/misc/evec_load.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/misc/evec_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.907570 cij-1.0.0b3/cij/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/color_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/modes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/pvticker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/quick.py
--rw-r--r--   0 runner    (1001) docker     (121)     4058 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/plot/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.907570 cij-1.0.0b3/cij/util/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/util/compliance.py
--rw-r--r--   0 runner    (1001) docker     (121)     4225 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/util/fill.py
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/util/static_eos.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/util/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/util/voigt.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-05-22 01:46:14.000000 cij-1.0.0b3/cij/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-22 01:46:22.899570 cij-1.0.0b3/cij.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6917 2021-05-22 01:46:22.000000 cij-1.0.0b3/cij.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-05-22 01:46:22.000000 cij-1.0.0b3/cij.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-22 01:46:22.000000 cij-1.0.0b3/cij.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-05-22 01:46:22.000000 cij-1.0.0b3/cij.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-05-22 01:46:22.000000 cij-1.0.0b3/cij.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-05-22 01:46:22.000000 cij-1.0.0b3/cij.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-22 01:46:22.907570 cij-1.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-05-22 01:46:14.000000 cij-1.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.634740 cij-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-19 14:16:16.000000 cij-1.0.0b4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-19 14:16:29.634740 cij-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-19 14:16:16.000000 cij-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.618740 cij-1.0.0b4/cij/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.622740 cij-1.0.0b4/cij/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/cij.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/geotherm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/cli/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.622740 cij-1.0.0b4/cij/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/full_modulus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/mode_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/modulus_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.622740 cij-1.0.0b4/cij/core/phonon_contribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/phonon_contribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/phonon_contribution/nonshear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/phonon_contribution/shear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/qha_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.622740 cij-1.0.0b4/cij/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/data/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/cubic
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/hexagonal
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/monoclinic
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/orthorhombic
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/tetragonal6
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/tetragonal7
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/triclinic
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/trigonal6
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/constraints/trigonal7
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/data/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/default/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/output/writer_rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/data/schema/config.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/io/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/config/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/io/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/output/results_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.626741 cij-1.0.0b4/cij/io/traditional/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/traditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/traditional/elast_dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/traditional/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/traditional/qha_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/io/traditional/qha_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.630741 cij-1.0.0b4/cij/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/misc/eig_sort_freqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/misc/evec_disp2eig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/misc/evec_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/misc/evec_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.630741 cij-1.0.0b4/cij/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/pvticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/quick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/plot/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.630741 cij-1.0.0b4/cij/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/util/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/util/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/util/static_eos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/util/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/util/voigt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 14:16:16.000000 cij-1.0.0b4/cij/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.634740 cij-1.0.0b4/cij.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-19 14:16:29.000000 cij-1.0.0b4/cij.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-19 14:16:29.000000 cij-1.0.0b4/cij.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:16:29.000000 cij-1.0.0b4/cij.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 14:16:29.000000 cij-1.0.0b4/cij.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 14:16:29.000000 cij-1.0.0b4/cij.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 14:16:29.000000 cij-1.0.0b4/cij.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:16:29.634740 cij-1.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 14:16:16.000000 cij-1.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:16:29.630741 cij-1.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_cli_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_cli_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_io_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_io_traditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_misc_evec_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_misc_evec_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_util_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_util_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 14:16:16.000000 cij-1.0.0b4/tests/test_cij_util_voigt.py
```

### Comparing `cij-1.0.0b3/LICENCE` & `cij-1.0.0b4/LICENCE`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/PKG-INFO` & `cij-1.0.0b4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,170 +1,189 @@
 Metadata-Version: 2.1
 Name: cij
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: High temperature thermal elasticity
 Home-page: https://github.com/MineralsCloud/cij/
 Author: Chenxing Luo
 Author-email: chenxing.luo@columbia.edu
-License: UNKNOWN
-Description: # <i>C<sub>ij</sub></i>: Semiemperical thermal elasticity
-        
-        Calculate high temperature thermal elasticity in Python.
-        
-        ## Installation
-        
-        The package can be installed with `pip` package manager.
-        
-        ### Install from PyPI (Python package index)
-        
-        ```shell
-        $ python3 -m pip install cij
-        ```
-        
-        ### Manual install
-        
-        At the command prompt, one should navigate to the directory that contains the
-        `setup.py` script and execute `pip install .`. Then, the package should be ready for use.
-        
-        ## Usage
-        
-        ### Command-line programs
-        
-        After installation, the Cij program can be started by typing `cij` at your 
-        command prompt:
-        
-        ```
-        Usage: cij [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          --version  Show the version and exit.
-          --help     Show this message and exit.
-        
-        Commands:
-          extract           Create data table at specific P or T.
-          extract-geotherm  Create data table at geotherm PT.
-          fill              Fill non-zero Cij terms based on symmetry.
-          modes             Plot interpolated mode frequency vs volume.
-          plot              Plot SAM-Cij calculation results.
-          run               Perform SAM-Cij calculation.
-          run-static        Calculate elastic moduli and acoustic velocities.
-        ```
-        
-        ### SAM-Cij calculations with `cij run`
-        
-        #### Calculation settings file and example
-        
-        The `settings.yaml` file is home to all calculation settings. One needs to specify calculation parameters, such as thermal EoS fitting parameters, phonon interpolation settings, input data location, and output variables to store in YAML format. The following is an example settings file.
-        
-        ```yml
-        qha:
-          input: input01
-          settings:
-            # similar to settings in qha
-            DT: 100
-            P_MIN: 0
-            DELTA_P: 0.5
-            NTV: 81
-            order: 3
-            static_only: False
-            T_MIN: 0
-            NT: 31
-            DT_SAMPLE: 100
-            DELTA_P_SAMPLE: 5
-            volume_ratio: 1.2
-        elast:
-          input: elast.dat
-          settings:
-            mode_gamma:
-              interpolator: spline
-              order: 3
-            system: cubic
-        output:
-          pressure_base:
-            - cij
-            - vs
-            - vp
-            - bm_V
-            - bm_R
-            - bm_VRH
-            - G_V
-            - G_R
-            - G_VRH
-            - v
-          volume_base:
-            - p
-            # ...
-        
-        ```
-        
-        #### Input data
-        
-        Input data include a QHA input data file (`input01`) and a static elasticity input data (`elast.dat`). See the paper or detailed documentation for description and the [`examples`](./examples) folder for detailed example.
-        
-        #### Command line arguments
-        
-        ```txt
-        Usage: cij run [OPTIONS] SETTINGS_FILENAME
-        
-          Perform SAM-Cij calculation.
-        
-        Options:
-          --version                       Show the version and exit.
-          --debug [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]
-                                          Logging level
-          --help                          Show this message and exit.
-        ```
-        
-        
-        ## Structure of the `cij` package
-        
-        The cij package is written in Python 3. The Python source code is located in the `cij` sub-folder.
-        Input for three examples in the `examples` sub-folder, documentation in the `docs` sub-folder, and the installation script `setup.py`.
-        
-        The Python code is organized into several modules:
-        
-        - **`cij.core`**: Core functionalities
-        	- `calculator`: The calculator that controls the workflow.
-        	- `mode_gamma`: Interpolate phonon frequencies and calculate mode Grüneisen parameters.
-        	- `phonon_contribution`: Calculate phonon *c<sub>ij</sub>*<sup>ph</sup>.
-        	full_modulus – Interpolate *c<sub>ij</sub>*<sup>st</sup> vs. *V*, and calculate *c<sub>ij</sub><sup>S</sup>* and *c<sub>ij</sub><sup>T</sup>*.
-        tasks – Handles the ordering of *c<sub>ij</sub>*<sup>ph</sup> calculation.
-        - **`cij.util`**: Methods used in the main program
-        	- `voigt`: Convert between Voigt (*c<sub>ij</sub>*) and regular (*c<sub>ijkl</sub>*) notations of elastic coefficients.
-        	- `units`: Handle unit conversion.
-        - **`cij.io`**: Input output functions and classes.
-        - **`cij.plot`**: Plotting functionalities.
-        - **`cij.cli`**: Command-line programs
-        	- `cij run` (`main.py`) – Perform a SAM-Cij calculation.
-        	- `cij run-static` (`static.py`) – Calculate static elastic properties.
-        	- `cij extract` (`extract.py`) – Extract calculation results for a specific *T* or *P* to a table.
-        	- `cij extract-geotherm` (`geotherm.py`) – Extract calculation results along geotherm *PT* (given as input) to a table.
-        	- `cij plot` (`plot.py`) – Convert output data table to PNG plot.
-        	- `cij modes` (`modes.py`) – Plot phonon frequency interpolation results.
-          - `cij fill` (`fill.py`) – Fill all the non-zero terms for elastic coefficients given the constraint of a crystal system.
-        - **`cij.data`**: Data distributed with the program, e.g., the relationship between *c<sub>ij</sub>*’s for different crystal systems, the naming scheme for output files, etc.
-        - **`cij.misc`**: Miscellaneous functionalities that are not used in the main program, e.g., methods that facilitate the preparation of input files.
-        
-        ## Author
-        
-        The code in this repo is initially authored by [Chenxing Luo][1].
-        
-        [1]: https://github.com/chazeon
-        
-        ## Documentation
-        
-        See [GitHub pages][2].
-        
-        [2]: https://mineralscloud.github.io/cij
-        
-        ## Build status
-        
-        ![GitHub Actions](https://github.com/MineralsCloud/cij/actions/workflows/main.yml/badge.svg)
-        [![codecov](https://codecov.io/gh/MineralsCloud/cij/branch/dev/graph/badge.svg?token=Ln1Fo4vNBE)](https://codecov.io/gh/MineralsCloud/cij)
-        [![pypi](https://img.shields.io/pypi/v/cij.svg)](https://pypi.org/project/cij/)
-        
-        ## Licence
-        
-        Released under [GNU GPLv3](./LICENCE) license.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy>=1.10.0
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: qha
+Requires-Dist: lazy_property
+Requires-Dist: pint>=0.10
+Requires-Dist: networkx
+Requires-Dist: click
+Requires-Dist: jsonschema
+Requires-Dist: sympy
+
+# <i>C<sub>ij</sub></i>: Semiemperical thermal elasticity
+
+Calculate high temperature thermal elasticity in Python.
+
+## Installation
+
+The package can be installed with `pip` package manager.
+
+### Install from PyPI (Python package index)
+
+```shell
+$ python3 -m pip install cij
+```
+
+### Manual install
+
+At the command prompt, one should navigate to the directory that contains the
+`setup.py` script and execute `pip install .`. Then, the package should be ready for use.
+
+## Usage
+
+### Command-line programs
+
+After installation, the Cij program can be started by typing `cij` at your 
+command prompt:
+
+```
+Usage: cij [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  extract           Create data table at specific P or T.
+  extract-geotherm  Create data table at geotherm PT.
+  fill              Fill non-zero Cij terms based on symmetry.
+  modes             Plot interpolated mode frequency vs volume.
+  plot              Plot SAM-Cij calculation results.
+  run               Perform SAM-Cij calculation.
+  run-static        Calculate elastic moduli and acoustic velocities.
+```
+
+### SAM-Cij calculations with `cij run`
+
+#### Calculation settings file and example
+
+The `settings.yaml` file is home to all calculation settings. One needs to specify calculation parameters, such as thermal EoS fitting parameters, phonon interpolation settings, input data location, and output variables to store in YAML format. The following is an example settings file.
+
+```yml
+qha:
+  input: input01
+  settings:
+    # similar to settings in qha
+    DT: 100
+    P_MIN: 0
+    DELTA_P: 0.5
+    NTV: 81
+    order: 3
+    static_only: False
+    T_MIN: 0
+    NT: 31
+    DT_SAMPLE: 100
+    DELTA_P_SAMPLE: 5
+    volume_ratio: 1.2
+elast:
+  input: elast.dat
+  settings:
+    mode_gamma:
+      interpolator: spline
+      order: 3
+    symmetry:
+      system: cubic
+output:
+  pressure_base:
+    - cij
+    - vs
+    - vp
+    - bm_V
+    - bm_R
+    - bm_VRH
+    - G_V
+    - G_R
+    - G_VRH
+    - v
+  volume_base:
+    - p
+    # ...
+
+```
+
+#### Input data
+
+Input data include a QHA input data file (`input01`) and a static elasticity input data (`elast.dat`). See the paper or detailed documentation for description and the [`examples`](./examples) folder for detailed example.
+
+#### Command line arguments
+
+```txt
+Usage: cij run [OPTIONS] SETTINGS_FILENAME
+
+  Perform SAM-Cij calculation.
+
+Options:
+  --version                       Show the version and exit.
+  --debug [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]
+                                  Logging level
+  --help                          Show this message and exit.
+```
+
+
+## Structure of the `cij` package
+
+The cij package is written in Python 3. The Python source code is located in the `cij` sub-folder.
+Input for three examples in the `examples` sub-folder, documentation in the `docs` sub-folder, and the installation script `setup.py`.
+
+The Python code is organized into several modules:
+
+- **`cij.core`**: Core functionalities
+	- `calculator`: The calculator that controls the workflow.
+	- `mode_gamma`: Interpolate phonon frequencies and calculate mode Grüneisen parameters.
+	- `phonon_contribution`: Calculate phonon *c<sub>ij</sub>*<sup>ph</sup>.
+	full_modulus – Interpolate *c<sub>ij</sub>*<sup>st</sup> vs. *V*, and calculate *c<sub>ij</sub><sup>S</sup>* and *c<sub>ij</sub><sup>T</sup>*.
+tasks – Handles the ordering of *c<sub>ij</sub>*<sup>ph</sup> calculation.
+- **`cij.util`**: Methods used in the main program
+	- `voigt`: Convert between Voigt (*c<sub>ij</sub>*) and regular (*c<sub>ijkl</sub>*) notations of elastic coefficients.
+	- `units`: Handle unit conversion.
+- **`cij.io`**: Input output functions and classes.
+- **`cij.plot`**: Plotting functionalities.
+- **`cij.cli`**: Command-line programs
+	- `cij run` (`main.py`) – Perform a SAM-Cij calculation.
+	- `cij run-static` (`static.py`) – Calculate static elastic properties.
+	- `cij extract` (`extract.py`) – Extract calculation results for a specific *T* or *P* to a table.
+	- `cij extract-geotherm` (`geotherm.py`) – Extract calculation results along geotherm *PT* (given as input) to a table.
+	- `cij plot` (`plot.py`) – Convert output data table to PNG plot.
+	- `cij modes` (`modes.py`) – Plot phonon frequency interpolation results.
+  - `cij fill` (`fill.py`) – Fill all the non-zero terms for elastic coefficients given the constraint of a crystal system.
+- **`cij.data`**: Data distributed with the program, e.g., the relationship between *c<sub>ij</sub>*’s for different crystal systems, the naming scheme for output files, etc.
+- **`cij.misc`**: Miscellaneous functionalities that are not used in the main program, e.g., methods that facilitate the preparation of input files.
+
+## Author
+
+The code in this repo is initially authored by [Chenxing Luo][1].
+
+[1]: https://github.com/chazeon
+
+## Documentation
+
+See [GitHub pages][2].
+
+[2]: https://mineralscloud.github.io/cij
+
+## Build status
+
+![GitHub Actions](https://github.com/MineralsCloud/cij/actions/workflows/main.yml/badge.svg)
+[![codecov](https://codecov.io/gh/MineralsCloud/cij/branch/dev/graph/badge.svg?token=Ln1Fo4vNBE)](https://codecov.io/gh/MineralsCloud/cij)
+[![pypi](https://img.shields.io/pypi/v/cij.svg)](https://pypi.org/project/cij/)
+[![pypi](https://img.shields.io/pypi/dm/cij.svg)](https://pypi.org/project/cij/)
+
+## How to cite
+
+If you use this software in any publication, please cite:
+
+Luo, C., Deng, X., Wang, W., Shukla, G., Wu, Z., & Wentzcovitch, R. M. (2021). cij: A Python code for quasiharmonic thermoelasticity. *Computer Physics Communications*, 108067. https://doi.org/10.1016/j.cpc.2021.108067
+
+The paper is also available from arXiv: https://arxiv.org/abs/2101.12596
+
+## Licence
+
+Released under [GNU GPLv3](./LICENCE) license.
```

### Comparing `cij-1.0.0b3/README.md` & `cij-1.0.0b4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     volume_ratio: 1.2
 elast:
   input: elast.dat
   settings:
     mode_gamma:
       interpolator: spline
       order: 3
-    system: cubic
+    symmetry:
+      system: cubic
 output:
   pressure_base:
     - cij
     - vs
     - vp
     - bm_V
     - bm_R
@@ -149,11 +150,20 @@
 [2]: https://mineralscloud.github.io/cij
 
 ## Build status
 
 ![GitHub Actions](https://github.com/MineralsCloud/cij/actions/workflows/main.yml/badge.svg)
 [![codecov](https://codecov.io/gh/MineralsCloud/cij/branch/dev/graph/badge.svg?token=Ln1Fo4vNBE)](https://codecov.io/gh/MineralsCloud/cij)
 [![pypi](https://img.shields.io/pypi/v/cij.svg)](https://pypi.org/project/cij/)
+[![pypi](https://img.shields.io/pypi/dm/cij.svg)](https://pypi.org/project/cij/)
+
+## How to cite
+
+If you use this software in any publication, please cite:
+
+Luo, C., Deng, X., Wang, W., Shukla, G., Wu, Z., & Wentzcovitch, R. M. (2021). cij: A Python code for quasiharmonic thermoelasticity. *Computer Physics Communications*, 108067. https://doi.org/10.1016/j.cpc.2021.108067
+
+The paper is also available from arXiv: https://arxiv.org/abs/2101.12596
 
 ## Licence
 
 Released under [GNU GPLv3](./LICENCE) license.
```

### Comparing `cij-1.0.0b3/cij/cli/cij.py` & `cij-1.0.0b4/cij/cli/cij.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/cli/extract.py` & `cij-1.0.0b4/cij/cli/extract.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/cli/fill.py` & `cij-1.0.0b4/cij/cli/fill.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/cli/geotherm.py` & `cij-1.0.0b4/cij/cli/geotherm.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/cli/main.py` & `cij-1.0.0b4/cij/cli/main.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/cli/modes.py` & `cij-1.0.0b4/cij/cli/modes.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/cli/static.py` & `cij-1.0.0b4/cij/cli/static.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/core/calculator.py` & `cij-1.0.0b4/cij/core/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     def shear_modulus_reuss(self) -> numpy.ndarray:
         '''Reuss average of shear modulus :math:`K_\\text{R}(T, V)` as a function
         of temperature and volume.
 
         .. math::
             G_\\text{R} = 15 / [
                   4 (s_{11} + s_{22} + s_{33})
-                + 2 (s_{12} + s_{23} + s_{31})
+                - 4 (s_{12} + s_{23} + s_{31})
                 + 3 (s_{44} + s_{55} + s_{66})
             ]
         ''' 
         return 15 / ( \
             + 4 * (self.s11 + self.s22 + self.s33) \
             - 4 * (self.s12 + self.s23 + self.s13) \
             + 3 * (self.s44 + self.s55 + self.s66))
@@ -301,15 +301,15 @@
     
     @property
     def primary_velocities(self) -> numpy.ndarray:
         '''Primary accoustic wave velocity :math:`v_\\text{p}(T, V)` as a
         function of temperature and volume.
 
         .. math::
-            v_\\text{p} = \\sqrt{\\frac{K_\\text{VRH} + 3/4 \, G_\\text{VRH} }{\\rho}}
+            v_\\text{p} = \\sqrt{\\frac{K_\\text{VRH} + 4/3 \, G_\\text{VRH} }{\\rho}}
         '''
         e = units.Quantity((self.bulk_modulus_voigt_reuss_hill + 4 / 3 * self.shear_modulus_voigt_reuss_hill) * self.v_array, units.rydberg).to(units.kg * units.km ** 2 / units.s ** 2).magnitude
         return numpy.sqrt(e / self.mass)
 
     @property
     def secondary_velocities(self) -> numpy.ndarray:
         '''Secondary accoustic wave velocity :math:`v_\\text{s}(T, V)` as a
@@ -459,15 +459,15 @@
     def shear_modulus_reuss(self) -> numpy.ndarray:
         '''Reuss average of shear modulus :math:`G_\\text{R}(T, P)` as a function
         of temperature and pressure.
 
         .. math::
             G_\\text{R} = 15 / [
                   4 (s_{11} + s_{22} + s_{33})
-                + 2 (s_{12} + s_{23} + s_{31})
+                - 4 (s_{12} + s_{23} + s_{31})
                 + 3 (s_{44} + s_{55} + s_{66})
             ] 
         '''
         return self.v2p(self.calculator.volume_base.shear_modulus_reuss)
 
     @property
     def shear_modulus_voigt_reuss_hill(self) -> numpy.ndarray:
@@ -486,15 +486,15 @@
     
     @property
     def primary_velocities(self) -> numpy.ndarray:
         '''Primary accoustic wave velocity :math:`v_\\text{p}(T, P)` as a
         function of temperature and pressure.
 
         .. math::
-            v_\\text{p} = \\sqrt{\\frac{K_\\text{VRH} + 3/4 \, G_\\text{VRH} }{\\rho}}
+            v_\\text{p} = \\sqrt{\\frac{K_\\text{VRH} + 4/3 \, G_\\text{VRH} }{\\rho}}
         '''
         return self.v2p(self.calculator.volume_base.primary_velocities)
 
     @property
     def secondary_velocities(self) -> numpy.ndarray:
         '''Secondary accoustic wave velocity :math:`v_\\text{s}(T, P)` as a
         function of temperature and pressure.
```

### Comparing `cij-1.0.0b3/cij/core/full_modulus.py` & `cij-1.0.0b4/cij/core/full_modulus.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/core/mode_gamma.py` & `cij-1.0.0b4/cij/core/mode_gamma.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/core/modulus_worker.py` & `cij-1.0.0b4/cij/core/modulus_worker.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/core/phonon_contribution/nonshear.py` & `cij-1.0.0b4/cij/core/phonon_contribution/nonshear.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     '''Calculate sum of physical quantity over :math:`3N` phonon modes and
     :math:`N_q` :math:`q`-points (:math:`\\sum_{qm}`) except for accoustic modes
     at \\Gamma point (first :math:`q`-point and first three modes).
 
     :param amount: :math:`X_{qm}`
     :param q_weights: :math:`q`-point multiplicities :math:`w_q`
 
-    :returns: Sum :math:`\\bar X = \sum_{qm} X_{qm} w_q`
+    :returns: Sum :math:`\\bar X = \\sum_{qm} X_{qm} w_q`
     '''
     dims = len(amount.shape)
     _amount = amount.copy()
     clear_gamma_point(_amount)
 
     return numpy.average(
         numpy.average(_amount, axis=dims - 1),
@@ -113,53 +113,53 @@
         )
 
     @LazyProperty
     def Q(self) -> numpy.ndarray:
         '''Value of expression :math:`Q_{qm}(T, V)`
 
         .. math::
-            Q_{qm}(T, V) = \\frac{\hbar\omega_{qm}(V)}{k_\\text{B}T}
+            Q_{qm}(T, V) = \\frac{\\hbar\\omega_{qm}(V)}{k_\\text{B}T}
         '''
         return  h_div_k * (self.freq_array[nax,:,:,:] / self.t_array[:,nax,nax,nax])
 
     @LazyProperty
     def Q1(self) -> numpy.ndarray:
         '''Value of expression
 
         .. math::
-            \\frac{Q_{qm}(T, V)}{\exp Q_{qm}(T, V) - 1}
+            \\frac{Q_{qm}(T, V)}{\\exp Q_{qm}(T, V) - 1}
 
-        where :math:`Q_{qm}(T, V) = \\frac{\hbar\omega_{qm}(V)}{k_\\text{B}T}`
+        where :math:`Q_{qm}(T, V) = \\frac{\\hbar\\omega_{qm}(V)}{k_\\text{B}T}`
         '''
         return self.Q / (numpy.exp(self.Q) - 1)
 
     @LazyProperty
     def Q2(self) -> numpy.ndarray:
         '''Value of expression
 
         .. math::
-            \\frac{Q_{qm}^2(T, V) \exp Q_{qm}(T, V) }{(\exp Q_{qm}(T, V) - 1) ^ 2}
+            \\frac{Q_{qm}^2(T, V) \\exp Q_{qm}(T, V) }{(\\exp Q_{qm}(T, V) - 1) ^ 2}
 
-        where :math:`Q_{qm}(T, V) = \\frac{\hbar\omega_{qm}(V)}{k_\\text{B}T}`
+        where :math:`Q_{qm}(T, V) = \\frac{\\hbar\\omega_{qm}(V)}{k_\\text{B}T}`
         '''
         return self.Q ** 2 * numpy.exp(self.Q) / (numpy.exp(self.Q) - 1) ** 2
 
 
     @LazyProperty
     def zero_point_contribution(self) -> numpy.ndarray:
         '''The zero-point motion contribution to the
         vibrational part of the longitudinal elastic modulus
         (:math:`c_{iiii}`, :math:`i = 1-3`).
 
         .. math::
             c^{\\text{zpm}}_{iiii}
-                = \\frac{\hbar}{2V}\\sum_{qm}
+                = \\frac{\\hbar}{2V}\\sum_{qm}
                     \\left(\\frac{\\partial^2\\omega_{qm} (V)}{\\partial e_{ii} ^ 2}\\right)
-                = \\frac{\hbar}{2V}\\sum_{qm}
-                    \\left(\\gamma^{ii}_{qm}\\gamma^{ii}_{qm} - \\frac{\\partial \\gamma^{ii}_{qm}}{\\partial e_{ii}} + \gamma^{ii}_{qm}\\right) \\omega_{qm}
+                = \\frac{\\hbar}{2V}\\sum_{qm}
+                    \\left(\\gamma^{ii}_{qm}\\gamma^{ii}_{qm} - \\frac{\\partial \\gamma^{ii}_{qm}}{\\partial e_{ii}} + \\gamma^{ii}_{qm}\\right) \\omega_{qm}
         '''
         h = units.Quantity(_h, units.J * units.m).to(units.rydberg * units.cm).magnitude
         return h / 2 / self.v_array \
             * self.average_over_modes(
                 + self.mode_gamma[2] * self.freq_array
                 - self.mode_gamma[0] * self.freq_array
                 + self.mode_gamma[1][0] * self.freq_array
@@ -270,17 +270,17 @@
     def zero_point_contribution(self):
         '''The zero-point motion contribution to the
         vibrational part of the longitudinal elastic modulus
         (:math:`c^\\text{zpm}_{iijj}`, :math:`i,j = 1-3`, :math:`i \\neq j`).
 
         .. math::
             c^{\\text{zpm}}_{iijj}
-                = \\frac{\hbar}{2V}\\sum_{qm}
+                = \\frac{\\hbar}{2V}\\sum_{qm}
                     \\left(\\frac{\\partial^2\\omega_{qm} (V)}{\\partial e_{ii} \\partial e_{jj}}\\right)
-                = \\frac{\hbar}{2V}\\sum_{qm}
+                = \\frac{\\hbar}{2V}\\sum_{qm}
                     \\left(\\gamma^{ii}_{qm}\\gamma^{jj}_{qm} - \\frac{\\partial \\gamma^{ii}_{qm}}{\\partial e_{jj}}\\right) \\omega_{qm}
         '''
         h = units.Quantity(_h, units.J * units.m).to(units.rydberg * units.cm).magnitude
         return h / 2 / self.v_array \
             * self.average_over_modes(
                 + self.mode_gamma[2] * self.freq_array
                 - self.mode_gamma[0] * self.freq_array
```

### Comparing `cij-1.0.0b3/cij/core/phonon_contribution/shear.py` & `cij-1.0.0b4/cij/core/phonon_contribution/shear.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/core/qha_adapter.py` & `cij-1.0.0b4/cij/core/qha_adapter.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/core/tasks.py` & `cij-1.0.0b4/cij/core/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''This module analysis the basic units (task) of phonon contribution
 calculation to be performed, and the order they are conducted.
 '''
 
 import numpy
 import itertools
-from networkx import nx
+import networkx as nx
 from typing import List, Union, NamedTuple, Tuple, Iterable
 from collections import UserList, UserDict
 
 from cij.util import c_, C_, ElasticModulusCalculationType
 from .phonon_contribution import (
     ShearElasticModulusPhononContribution,
     LongitudinalElasticModulusPhononContribution,
```

### Comparing `cij-1.0.0b3/cij/data/default/settings.yaml` & `cij-1.0.0b4/cij/data/default/settings.yaml`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/data/output/writer_rules.yml` & `cij-1.0.0b4/cij/data/output/writer_rules.yml`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/data/schema/config.schema.json` & `cij-1.0.0b4/cij/data/schema/config.schema.json`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/io/config/config.py` & `cij-1.0.0b4/cij/io/config/config.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/io/config/validate.py` & `cij-1.0.0b4/cij/io/config/validate.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/io/output/results_writer.py` & `cij-1.0.0b4/cij/io/output/results_writer.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/io/traditional/elast_dat.py` & `cij-1.0.0b4/cij/io/traditional/elast_dat.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/io/traditional/qha_input.py` & `cij-1.0.0b4/cij/io/traditional/qha_input.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/misc/eig_sort_freqs.py` & `cij-1.0.0b4/cij/misc/eig_sort_freqs.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/misc/evec_disp2eig.py` & `cij-1.0.0b4/cij/misc/evec_disp2eig.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/misc/evec_load.py` & `cij-1.0.0b4/cij/misc/evec_load.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/misc/evec_sort.py` & `cij-1.0.0b4/cij/misc/evec_sort.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/plot/color_map.py` & `cij-1.0.0b4/cij/plot/color_map.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/plot/modes.py` & `cij-1.0.0b4/cij/plot/modes.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/plot/plotter.py` & `cij-1.0.0b4/cij/plot/plotter.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/plot/pvticker.py` & `cij-1.0.0b4/cij/plot/pvticker.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/plot/quick.py` & `cij-1.0.0b4/cij/plot/quick.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/plot/tasks.py` & `cij-1.0.0b4/cij/plot/tasks.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/util/compliance.py` & `cij-1.0.0b4/cij/util/compliance.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/util/fill.py` & `cij-1.0.0b4/cij/util/fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     nsym = len(symbols)
 
     # known variables
 
     a = []
     b = []
 
-    for sym, col in elast.iteritems():
+    for sym, col in elast.items():
         sym = sym.lower()   # Warning: user may use upper case "Cij" instead of "cij"!
         if not re.search(r"c(\d)(\d)", sym): continue
         _a = numpy.zeros(nsym)
         _a[list(symbols.keys()).index(sym)] = 1
         a.append(_a)
         b.append(col.to_numpy())
 
@@ -120,14 +120,14 @@
 
     for index, col in zip(symbols, x):
         key = next((key for key in elast.columns.tolist() if key.lower() == index), index)
         elast.loc[:, key] = col
     
     # drop empty columns
 
-    for index, col in list(elast.iteritems()):
+    for index, col in list(elast.items()):
         if numpy.allclose(col.to_numpy(), 0, atol=drop_atol):
             elast = elast.drop(index, axis=1)
 
 #     elast = elast.reset_index()
 
     return elast
```

### Comparing `cij-1.0.0b3/cij/util/static_eos.py` & `cij-1.0.0b4/cij/util/static_eos.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/util/units.py` & `cij-1.0.0b4/cij/util/units.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij/util/voigt.py` & `cij-1.0.0b4/cij/util/voigt.py`

 * *Files identical despite different names*

### Comparing `cij-1.0.0b3/cij.egg-info/PKG-INFO` & `cij-1.0.0b4/cij.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,170 +1,189 @@
 Metadata-Version: 2.1
 Name: cij
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: High temperature thermal elasticity
 Home-page: https://github.com/MineralsCloud/cij/
 Author: Chenxing Luo
 Author-email: chenxing.luo@columbia.edu
-License: UNKNOWN
-Description: # <i>C<sub>ij</sub></i>: Semiemperical thermal elasticity
-        
-        Calculate high temperature thermal elasticity in Python.
-        
-        ## Installation
-        
-        The package can be installed with `pip` package manager.
-        
-        ### Install from PyPI (Python package index)
-        
-        ```shell
-        $ python3 -m pip install cij
-        ```
-        
-        ### Manual install
-        
-        At the command prompt, one should navigate to the directory that contains the
-        `setup.py` script and execute `pip install .`. Then, the package should be ready for use.
-        
-        ## Usage
-        
-        ### Command-line programs
-        
-        After installation, the Cij program can be started by typing `cij` at your 
-        command prompt:
-        
-        ```
-        Usage: cij [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          --version  Show the version and exit.
-          --help     Show this message and exit.
-        
-        Commands:
-          extract           Create data table at specific P or T.
-          extract-geotherm  Create data table at geotherm PT.
-          fill              Fill non-zero Cij terms based on symmetry.
-          modes             Plot interpolated mode frequency vs volume.
-          plot              Plot SAM-Cij calculation results.
-          run               Perform SAM-Cij calculation.
-          run-static        Calculate elastic moduli and acoustic velocities.
-        ```
-        
-        ### SAM-Cij calculations with `cij run`
-        
-        #### Calculation settings file and example
-        
-        The `settings.yaml` file is home to all calculation settings. One needs to specify calculation parameters, such as thermal EoS fitting parameters, phonon interpolation settings, input data location, and output variables to store in YAML format. The following is an example settings file.
-        
-        ```yml
-        qha:
-          input: input01
-          settings:
-            # similar to settings in qha
-            DT: 100
-            P_MIN: 0
-            DELTA_P: 0.5
-            NTV: 81
-            order: 3
-            static_only: False
-            T_MIN: 0
-            NT: 31
-            DT_SAMPLE: 100
-            DELTA_P_SAMPLE: 5
-            volume_ratio: 1.2
-        elast:
-          input: elast.dat
-          settings:
-            mode_gamma:
-              interpolator: spline
-              order: 3
-            system: cubic
-        output:
-          pressure_base:
-            - cij
-            - vs
-            - vp
-            - bm_V
-            - bm_R
-            - bm_VRH
-            - G_V
-            - G_R
-            - G_VRH
-            - v
-          volume_base:
-            - p
-            # ...
-        
-        ```
-        
-        #### Input data
-        
-        Input data include a QHA input data file (`input01`) and a static elasticity input data (`elast.dat`). See the paper or detailed documentation for description and the [`examples`](./examples) folder for detailed example.
-        
-        #### Command line arguments
-        
-        ```txt
-        Usage: cij run [OPTIONS] SETTINGS_FILENAME
-        
-          Perform SAM-Cij calculation.
-        
-        Options:
-          --version                       Show the version and exit.
-          --debug [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]
-                                          Logging level
-          --help                          Show this message and exit.
-        ```
-        
-        
-        ## Structure of the `cij` package
-        
-        The cij package is written in Python 3. The Python source code is located in the `cij` sub-folder.
-        Input for three examples in the `examples` sub-folder, documentation in the `docs` sub-folder, and the installation script `setup.py`.
-        
-        The Python code is organized into several modules:
-        
-        - **`cij.core`**: Core functionalities
-        	- `calculator`: The calculator that controls the workflow.
-        	- `mode_gamma`: Interpolate phonon frequencies and calculate mode Grüneisen parameters.
-        	- `phonon_contribution`: Calculate phonon *c<sub>ij</sub>*<sup>ph</sup>.
-        	full_modulus – Interpolate *c<sub>ij</sub>*<sup>st</sup> vs. *V*, and calculate *c<sub>ij</sub><sup>S</sup>* and *c<sub>ij</sub><sup>T</sup>*.
-        tasks – Handles the ordering of *c<sub>ij</sub>*<sup>ph</sup> calculation.
-        - **`cij.util`**: Methods used in the main program
-        	- `voigt`: Convert between Voigt (*c<sub>ij</sub>*) and regular (*c<sub>ijkl</sub>*) notations of elastic coefficients.
-        	- `units`: Handle unit conversion.
-        - **`cij.io`**: Input output functions and classes.
-        - **`cij.plot`**: Plotting functionalities.
-        - **`cij.cli`**: Command-line programs
-        	- `cij run` (`main.py`) – Perform a SAM-Cij calculation.
-        	- `cij run-static` (`static.py`) – Calculate static elastic properties.
-        	- `cij extract` (`extract.py`) – Extract calculation results for a specific *T* or *P* to a table.
-        	- `cij extract-geotherm` (`geotherm.py`) – Extract calculation results along geotherm *PT* (given as input) to a table.
-        	- `cij plot` (`plot.py`) – Convert output data table to PNG plot.
-        	- `cij modes` (`modes.py`) – Plot phonon frequency interpolation results.
-          - `cij fill` (`fill.py`) – Fill all the non-zero terms for elastic coefficients given the constraint of a crystal system.
-        - **`cij.data`**: Data distributed with the program, e.g., the relationship between *c<sub>ij</sub>*’s for different crystal systems, the naming scheme for output files, etc.
-        - **`cij.misc`**: Miscellaneous functionalities that are not used in the main program, e.g., methods that facilitate the preparation of input files.
-        
-        ## Author
-        
-        The code in this repo is initially authored by [Chenxing Luo][1].
-        
-        [1]: https://github.com/chazeon
-        
-        ## Documentation
-        
-        See [GitHub pages][2].
-        
-        [2]: https://mineralscloud.github.io/cij
-        
-        ## Build status
-        
-        ![GitHub Actions](https://github.com/MineralsCloud/cij/actions/workflows/main.yml/badge.svg)
-        [![codecov](https://codecov.io/gh/MineralsCloud/cij/branch/dev/graph/badge.svg?token=Ln1Fo4vNBE)](https://codecov.io/gh/MineralsCloud/cij)
-        [![pypi](https://img.shields.io/pypi/v/cij.svg)](https://pypi.org/project/cij/)
-        
-        ## Licence
-        
-        Released under [GNU GPLv3](./LICENCE) license.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy>=1.10.0
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: qha
+Requires-Dist: lazy_property
+Requires-Dist: pint>=0.10
+Requires-Dist: networkx
+Requires-Dist: click
+Requires-Dist: jsonschema
+Requires-Dist: sympy
+
+# <i>C<sub>ij</sub></i>: Semiemperical thermal elasticity
+
+Calculate high temperature thermal elasticity in Python.
+
+## Installation
+
+The package can be installed with `pip` package manager.
+
+### Install from PyPI (Python package index)
+
+```shell
+$ python3 -m pip install cij
+```
+
+### Manual install
+
+At the command prompt, one should navigate to the directory that contains the
+`setup.py` script and execute `pip install .`. Then, the package should be ready for use.
+
+## Usage
+
+### Command-line programs
+
+After installation, the Cij program can be started by typing `cij` at your 
+command prompt:
+
+```
+Usage: cij [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  extract           Create data table at specific P or T.
+  extract-geotherm  Create data table at geotherm PT.
+  fill              Fill non-zero Cij terms based on symmetry.
+  modes             Plot interpolated mode frequency vs volume.
+  plot              Plot SAM-Cij calculation results.
+  run               Perform SAM-Cij calculation.
+  run-static        Calculate elastic moduli and acoustic velocities.
+```
+
+### SAM-Cij calculations with `cij run`
+
+#### Calculation settings file and example
+
+The `settings.yaml` file is home to all calculation settings. One needs to specify calculation parameters, such as thermal EoS fitting parameters, phonon interpolation settings, input data location, and output variables to store in YAML format. The following is an example settings file.
+
+```yml
+qha:
+  input: input01
+  settings:
+    # similar to settings in qha
+    DT: 100
+    P_MIN: 0
+    DELTA_P: 0.5
+    NTV: 81
+    order: 3
+    static_only: False
+    T_MIN: 0
+    NT: 31
+    DT_SAMPLE: 100
+    DELTA_P_SAMPLE: 5
+    volume_ratio: 1.2
+elast:
+  input: elast.dat
+  settings:
+    mode_gamma:
+      interpolator: spline
+      order: 3
+    symmetry:
+      system: cubic
+output:
+  pressure_base:
+    - cij
+    - vs
+    - vp
+    - bm_V
+    - bm_R
+    - bm_VRH
+    - G_V
+    - G_R
+    - G_VRH
+    - v
+  volume_base:
+    - p
+    # ...
+
+```
+
+#### Input data
+
+Input data include a QHA input data file (`input01`) and a static elasticity input data (`elast.dat`). See the paper or detailed documentation for description and the [`examples`](./examples) folder for detailed example.
+
+#### Command line arguments
+
+```txt
+Usage: cij run [OPTIONS] SETTINGS_FILENAME
+
+  Perform SAM-Cij calculation.
+
+Options:
+  --version                       Show the version and exit.
+  --debug [CRITICAL|ERROR|WARNING|INFO|DEBUG|NOTSET]
+                                  Logging level
+  --help                          Show this message and exit.
+```
+
+
+## Structure of the `cij` package
+
+The cij package is written in Python 3. The Python source code is located in the `cij` sub-folder.
+Input for three examples in the `examples` sub-folder, documentation in the `docs` sub-folder, and the installation script `setup.py`.
+
+The Python code is organized into several modules:
+
+- **`cij.core`**: Core functionalities
+	- `calculator`: The calculator that controls the workflow.
+	- `mode_gamma`: Interpolate phonon frequencies and calculate mode Grüneisen parameters.
+	- `phonon_contribution`: Calculate phonon *c<sub>ij</sub>*<sup>ph</sup>.
+	full_modulus – Interpolate *c<sub>ij</sub>*<sup>st</sup> vs. *V*, and calculate *c<sub>ij</sub><sup>S</sup>* and *c<sub>ij</sub><sup>T</sup>*.
+tasks – Handles the ordering of *c<sub>ij</sub>*<sup>ph</sup> calculation.
+- **`cij.util`**: Methods used in the main program
+	- `voigt`: Convert between Voigt (*c<sub>ij</sub>*) and regular (*c<sub>ijkl</sub>*) notations of elastic coefficients.
+	- `units`: Handle unit conversion.
+- **`cij.io`**: Input output functions and classes.
+- **`cij.plot`**: Plotting functionalities.
+- **`cij.cli`**: Command-line programs
+	- `cij run` (`main.py`) – Perform a SAM-Cij calculation.
+	- `cij run-static` (`static.py`) – Calculate static elastic properties.
+	- `cij extract` (`extract.py`) – Extract calculation results for a specific *T* or *P* to a table.
+	- `cij extract-geotherm` (`geotherm.py`) – Extract calculation results along geotherm *PT* (given as input) to a table.
+	- `cij plot` (`plot.py`) – Convert output data table to PNG plot.
+	- `cij modes` (`modes.py`) – Plot phonon frequency interpolation results.
+  - `cij fill` (`fill.py`) – Fill all the non-zero terms for elastic coefficients given the constraint of a crystal system.
+- **`cij.data`**: Data distributed with the program, e.g., the relationship between *c<sub>ij</sub>*’s for different crystal systems, the naming scheme for output files, etc.
+- **`cij.misc`**: Miscellaneous functionalities that are not used in the main program, e.g., methods that facilitate the preparation of input files.
+
+## Author
+
+The code in this repo is initially authored by [Chenxing Luo][1].
+
+[1]: https://github.com/chazeon
+
+## Documentation
+
+See [GitHub pages][2].
+
+[2]: https://mineralscloud.github.io/cij
+
+## Build status
+
+![GitHub Actions](https://github.com/MineralsCloud/cij/actions/workflows/main.yml/badge.svg)
+[![codecov](https://codecov.io/gh/MineralsCloud/cij/branch/dev/graph/badge.svg?token=Ln1Fo4vNBE)](https://codecov.io/gh/MineralsCloud/cij)
+[![pypi](https://img.shields.io/pypi/v/cij.svg)](https://pypi.org/project/cij/)
+[![pypi](https://img.shields.io/pypi/dm/cij.svg)](https://pypi.org/project/cij/)
+
+## How to cite
+
+If you use this software in any publication, please cite:
+
+Luo, C., Deng, X., Wang, W., Shukla, G., Wu, Z., & Wentzcovitch, R. M. (2021). cij: A Python code for quasiharmonic thermoelasticity. *Computer Physics Communications*, 108067. https://doi.org/10.1016/j.cpc.2021.108067
+
+The paper is also available from arXiv: https://arxiv.org/abs/2101.12596
+
+## Licence
+
+Released under [GNU GPLv3](./LICENCE) license.
```

### Comparing `cij-1.0.0b3/cij.egg-info/SOURCES.txt` & `cij-1.0.0b4/cij.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -65,8 +65,18 @@
 cij/plot/quick.py
 cij/plot/tasks.py
 cij/util/__init__.py
 cij/util/compliance.py
 cij/util/fill.py
 cij/util/static_eos.py
 cij/util/units.py
-cij/util/voigt.py
+cij/util/voigt.py
+tests/test_cij_cli_fill.py
+tests/test_cij_cli_run.py
+tests/test_cij_cli_static.py
+tests/test_cij_io_config.py
+tests/test_cij_io_traditional.py
+tests/test_cij_misc_evec_load.py
+tests/test_cij_misc_evec_sort.py
+tests/test_cij_util_fill.py
+tests/test_cij_util_units.py
+tests/test_cij_util_voigt.py
```

### Comparing `cij-1.0.0b3/setup.py` & `cij-1.0.0b4/setup.py`

 * *Files identical despite different names*

