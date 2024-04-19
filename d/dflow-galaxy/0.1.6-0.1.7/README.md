# Comparing `tmp/dflow_galaxy-0.1.6.tar.gz` & `tmp/dflow_galaxy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.6.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.7.tar", max compression
```

## Comparing `dflow_galaxy-0.1.6.tar` & `dflow_galaxy-0.1.7.tar`

### file list

```diff
@@ -1,78 +1,80 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.6/LICENSE
--rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.6/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.6/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.6/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2167 2024-04-10 12:51:32.469597 dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     7015 2024-04-11 08:26:42.339456 dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     2006 2024-04-10 13:00:43.009583 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4853 2024-04-11 08:26:42.339456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0     2493 2024-04-11 08:26:42.339456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/report.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0    15556 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/report.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.6/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.6/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.6/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.6/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.6/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.6/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/main.py
--rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.6/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.6/dflow_galaxy/res/dynacat/tesla_template.yml
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.6/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6339 2024-04-10 05:02:53.113820 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9692 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8057 2024-04-11 02:42:29.459986 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     8185 2024-04-11 01:41:14.700081 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      561 2024-04-11 08:27:34.919457 dflow_galaxy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2010 2024-04-12 09:29:48.592387 dflow_galaxy-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.7/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.7/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2498 2024-04-19 08:40:55.003134 dflow_galaxy-0.1.7/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2167 2024-04-10 12:51:32.469597 dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     7139 2024-04-19 09:47:38.573186 dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     2006 2024-04-10 13:00:43.009583 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4874 2024-04-19 08:41:31.523135 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0     2525 2024-04-11 09:39:14.159344 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/report.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    16373 2024-04-19 09:26:16.823169 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/report.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.7/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.7/dflow_galaxy/core/dflow.py
+-rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.7/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.7/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.7/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.7/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.7/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.7/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1128 2024-04-19 08:58:50.173149 dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/deepmd.json
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0      906 2024-04-18 09:39:30.561274 dflow_galaxy-0.1.7/dflow_galaxy/util.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.7/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6339 2024-04-10 05:02:53.113820 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9692 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8057 2024-04-11 02:42:29.459986 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8185 2024-04-11 01:41:14.700081 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      560 2024-04-19 09:48:39.823185 dflow_galaxy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.7/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.6/LICENSE` & `dflow_galaxy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from dflow.plugins import bohrium
 import dflow
 
 from dflow_galaxy.core.log import get_logger
 logger = get_logger(__name__)
 
 
-class DFlowOptions(BaseModel):
+class DFlowOptionsMixin:
     bh_username: Optional[BohriumUsername]
     bh_ticket: Optional[BohriumTicket]
     bh_project_id: Optional[BohriumProjectId]
 
     dflow_labels: Optional[DflowLabels]
     dflow_argo_api_server: Optional[DflowArgoAPIServer]
     dflow_k8s_api_server: Optional[DflowK8sAPIServer]
     dflow_access_token: Optional[DflowAccessToken]
     dflow_storage_endpoint: Optional[DflowStorageEndpoint]
     dflow_storage_repository: Optional[DflowStorageRepository]
 
 
-def setup_dflow_context(opts: DFlowOptions):
+def setup_dflow_context(opts: DFlowOptionsMixin):
     """
     setup dflow context based on:
     https://dptechnology.feishu.cn/docx/HYjmdDj36oAksixbviKcbgUinUf
     """
 
     dflow_config = {
         'host': opts.dflow_argo_api_server,
```

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath, Optional
-from dp.launching.typing import Int, String, Enum, Float, Boolean
+from dp.launching.typing import Int, String, Enum, Float, Boolean, Set
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 
-from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context
+from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context
 from dflow_galaxy.res import get_cp2k_data_dir
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
 from ai2_kit.tool.ase import AseHelper
 from ai2_kit.tool.dpdata import DpdataHelper
 
 from pathlib import Path
@@ -71,15 +71,15 @@
     ECP_POTENTIALS_pob_TZVP_rev2 = "ECP_POTENTIALS_pob-TZVP-rev2"
     ECP_POTENTIALS = "ECP_POTENTIALS"
     NLCC_POTENTIALS = "NLCC_POTENTIALS"
     AcPP1_POTENTIALS = "AcPP1_POTENTIALS"
     LnPP1_POTENTIALS = "LnPP1_POTENTIALS"
 
 
-class Cp2kLightningArgs(DFlowOptions):
+class Cp2kLightningArgs(BaseModel, DFlowOptionsMixin):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
         description="A system file as the initial structure of AIMD simulation, can be xyz, cif, POSCAR format")
@@ -100,16 +100,17 @@
         default=1000,
         description="Number of steps in the simulation")
 
     timestep: Float = Field(
         default=0.5,
         description="Time step of the simulation in fs")
 
-    basis_set: BasicSetOptions = Field(
-        default=BasicSetOptions.BASIS_MOLOPT,
+    basis_set: Set[BasicSetOptions] = Field(
+        default=[BasicSetOptions.BASIS_MOLOPT],
+        min_items=1,
         description='Select the basis set for the simulation')
 
     potential: PotentialOptions = Field(
         default=PotentialOptions.GTH_POTENTIALS,
         description='Select the potential for the simulation')
 
     output_dir: OutputDirectory = Field(
@@ -135,35 +136,38 @@
         ]),
         format='multi-line',
         description="Script to run CP2K simulation, note that it depends on the docker image")
 
 
 def launch_app(args: Cp2kLightningArgs) -> int:
     # stage 1: generate cp2k input file
-    basis_set_file = get_cp2k_data_file(args.basis_set.value)
-    potential_file = get_cp2k_data_file(args.potential.value)
-    # copy data file to cwd
-    # don't use absolute path as the config file will be use in docker
-    shutil.copy(basis_set_file, '.')
-    shutil.copy(potential_file, '.')
+    basis_set_files = [v.value for v in args.basis_set]
+    assert len(basis_set_files) > 0, 'basis_set must be set'
+    potential_file = args.potential.value
+    for f in basis_set_files + [potential_file]:
+        f = get_cp2k_data_file(f)
+        # copy data file to cwd
+        # don't use absolute path as the config file will be use in docker
+        shutil.copy(f, '.')
+
     system_file = args.system_file.get_full_path()
 
     # create a closure to generate cp2k input file
     def _gen_cp2k_input(out_dir: str, aimd: bool):
         config_builder = ai2cat.ConfigBuilder()
         config_builder.load_system(system_file).gen_cp2k_input(
             out_dir=out_dir,
             aimd=aimd,
             # common options
             style=args.system_type.value,
             temp=args.temperature,
             steps=args.steps,
             timestep=args.timestep,
-            basic_set_file=args.basis_set.value,
-            potential_file=args.potential.value,
+            basis_set_file=basis_set_files,
+            potential_file=potential_file,
             parameter_file='dftd3.dat',
         )
     _gen_cp2k_input('aimd', aimd=True)
     _gen_cp2k_input('dft', aimd=False)
 
     out_dir = Path(args.output_dir)
     shutil.move('aimd/cp2k.inp', out_dir / 'cp2k.aimd.inp')
```

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath, Optional, Dict
 from dp.launching.typing import Int, String, Enum, Float, Boolean
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 
-from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context, EnsembleOptions
+from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context, EnsembleOptions
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
 from ai2_kit.core.util import dump_text, dump_json
 
 
 from pathlib import Path
 import shutil
@@ -15,15 +15,15 @@
 
 from .dflow import run_lammps_workflow
 from .report import gen_report
 
 logger = get_logger(__name__)
 
 
-class DynaCatMdArgs(DFlowOptions):
+class DynaCatMdArgs(BaseModel, DFlowOptionsMixin):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
         description="A system file as the initial structure of LAMMPS simulation, can be xyz, cif, POSCAR, etc.")
```

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/report.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'tooltip': {
             'trigger': 'axis'
         },
         'legend': {
             'data': header[1:],
         },
         'xAxis': {
-            'type': 'category',
+            'type': 'category',  # FIXME: should use value type
             'name': header[0],
             'data': [row[0] for row in rows],
         },
         'yAxis': {
             'type': 'value',
             'name': 'y-axis'
         },
```

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/main.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath
 from dp.launching.typing import Int, String, Enum, Float, Boolean, List, Optional, Dict
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 from dp.launching.report import Report, ReportSection, ChartReportElement
 
-from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context, EnsembleOptions
+from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context, EnsembleOptions
 from dflow_galaxy.res import get_res_path
 from dflow_galaxy.core.log import get_logger
 from dflow_galaxy.core.util import parse_string_array, str_or_none
 
 from dflow_galaxy.workflow.tesla.main import build_tesla_workflow
 
 from ai2_kit.core.util import dump_json, load_text, load_json
@@ -69,14 +69,18 @@
         default=True,
         description="Compress the model after training")
 
     concurrency: Int = Field(
         default=4,
         description="Number of concurrent run")
 
+    steps: Optional[Int] = Field(
+        default=400000,
+        description="Number of steps for DeepMD training, leave it empty will use the numb_steps defined in the input template")
+
     cmd: String = Field(
         default='dp',
         description="Command to run DeepMD, note that it depends on the docker image you used")
 
     setup_script: String = Field(
         default='',
         format='multi-line',
@@ -175,32 +179,32 @@
             '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k || which cp2k.psmp)")/../../data" || true',
             'source /opt/cp2k-toolchain/install/setup',
         ]),
         format='multi-line',
         description="Setup script for CP2K simulation, note that it depends on the docker image you used")
 
 
-class DynacatTeslaArgs(DFlowOptions):
+class DynacatTeslaArgs(BaseModel, DFlowOptionsMixin):
     deepmd_dataset : InputFilePath = Field(
         title='DeepMD Dataset',
         description="DeepMD in zip or tgz format, for example: deepmd-dataset.tgz")
 
-    deepmd_input_template: InputFilePath = Field(
+    deepmd_input_template: Optional[InputFilePath] = Field(
         title='DeepMD Input Template',
-        description="Input template file for DeepMD training, in json format, for example: deepmd.json")
+        description="Input template file for DeepMD training, in json format, for example: deepmd.json, if not provided, the build-in template will be used")
 
     lammps_system_file: InputFilePath = Field(
-        description="Structure file in xyz format use for LAMMPS simulation, for example h2o.xyz")
+        description="Structure file in xyz format use for LAMMPS simulation, for example h2o.xyz, the xyz file may contain multiple structures")
 
     cp2k_input_template: InputFilePath = Field(
         description="Input template file for CP2K simulation, for example: cp2k.inp")
 
     dry_run: Boolean = Field(
         default = True,
-        description="Generate configuration file without running the simulation")
+        description="Generate configuration file without running the workflow")
 
     max_iters: Int = Field(
         default = 7,
         description="Maximum iterations of the workflow")
 
     s3_prefix: Optional[String] = Field(
         description="Specify the S3 prefix of DFlow. By default a random prefix will be used for different jobs. Jobs use the same prefix will share the same working directory, which allow you to inherit the state of previous run.")
@@ -348,16 +352,26 @@
 def _get_workflow_config(args: DynacatTeslaArgs, dp_dataset_config: dict):
     # process system file
     explore_data_file = args.lammps_system_file.get_full_path()
     explore_data_key = os.path.basename(explore_data_file)
     atoms = ase.io.read(explore_data_file, index=0)
     type_map, mass_map = ai2cat.get_type_map(atoms)  # type: ignore
 
+    if args.deepmd_input_template:
+        deepmd_template_file = args.deepmd_input_template.get_full_path()
+    else:
+        deepmd_template_file = str(get_res_path() / 'dynacat' / 'deepmd.json')
+    deepmd_template = load_json(deepmd_template_file)
     cp2k_input_template = load_text(args.cp2k_input_template.get_full_path())
-    deepmd_template = load_json(args.deepmd_input_template.get_full_path())
+
+    if args.deepmd.steps and args.deepmd.steps > 0:
+        deepmd_template['training']['numb_steps'] = args.deepmd.steps
+    assert deepmd_template['training']['numb_steps'] > 0, 'numb_steps is required in the input template or input'
+    deepmd_template['training']['disp_file'] = 'lcurve.out'  # force to use lcurve.out
+
     product_vars, broadcast_vars = _get_lammps_vars(args.lammps.explore_vars)
 
     return {
         'datasets': {
             **dp_dataset_config,
             explore_data_key: {  # data key must be a normal file name or else ase cannot detect the format
                 'url': explore_data_file,
```

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/report.py` & `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/report.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.7/dflow_galaxy/core/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.7/dflow_galaxy/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.7/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.7/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/res/dynacat/tesla_template.yml` & `dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/tesla_template.yml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.6/pyproject.toml` & `dflow_galaxy-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydflow = "1.8.60"
 dpdispatcher = "^0.6.4"
-ai2-kit= "0.15.10"
+ai2-kit= "0.16.0"
 dp-launching-sdk = "^0.12.0"
 lbg = "^1.2.24"
 cp2kdata = "^0.6.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.0"
```

### Comparing `dflow_galaxy-0.1.6/PKG-INFO` & `dflow_galaxy-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ai2-kit (==0.15.10)
+Requires-Dist: ai2-kit (==0.16.0)
 Requires-Dist: cp2kdata (>=0.6.6,<0.7.0)
 Requires-Dist: dp-launching-sdk (>=0.12.0,<0.13.0)
 Requires-Dist: dpdispatcher (>=0.6.4,<0.7.0)
 Requires-Dist: lbg (>=1.2.24,<2.0.0)
 Requires-Dist: pydflow (==1.8.60)
 Description-Content-Type: text/markdown
 
@@ -24,18 +24,27 @@
 [![Downloads](https://pepy.tech/badge/dflow-galaxy)](https://pepy.tech/project/dflow-galaxy)
 [![Docker](https://img.shields.io/docker/v/link89/dflow-galaxy?label=docker&logo=docker)](https://hub.docker.com/repository/docker/link89/dflow-galaxy/general)
 
 
 Collection of workflows and tools built on top of DFlow and [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
 ## Features
+
+### Tools
 * DFlowBuilder: A type friendly wrapper for `DFlow` to build workflows in a more intuitive way.
-* Workflows:
-  * TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow designed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), ported from [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
+### Workflow
+* TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow developed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), ported from [ai2-kit](https://github.com/chenggroup/ai2-kit).
+
+### [Bohrium Apps](https://bohrium.dp.tech/apps)
+Bohrium Apps are cloud native apps that can be run on Bohrium Platform. 
+
+* CP2K Lightning: Run CP2K without building input files from scratch.
+* DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat.
+* DynaCat MD: Run MD simulations with DeepMD potential for DynaCat. 
 
 ## Get Started
 `dflow-galaxy` requires Python 3.9+ since it depends on `typing.Annotated`.
 
 To use `dflow-galaxy` as a library, you can install it via pip:
 
 ```bash
@@ -45,22 +54,19 @@
 For developers, please use `poetry` to bootstrap the development environment:
 
 ```bash
 poetry install
 poetry shell
 ```
 
-## Bohrium Launch App
-This repository also contains some launch apps for Bohrium. The entry of the Bohrium launch app is in the `launch_app` directory, and relative modules are in the `dflow_galaxy/app` directory.
+## Bohrium App
+The entry of the Bohrium App are in the [launch_app](./launch_app/) directory, and the actual implementation are in the [dflow_galaxy/app](./dflow_galaxy/app/) directory.
 
-Currently, the following launch apps are available:
+Document for Bohrium App development can be found [here](https://dptechnology.feishu.cn/docx/JPqgdmN1woxO8jxRtMycqWPQnIg)
 
-* CP2K Lightning: Run CP2K without building input files from scratch.
-* DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat.
-* DynaCat MD: Run MD simulations with DeepMD potential for DynaCat. 
 
 
 ## Distribution
 ### PyPI
 ```bash
 poetry publish --build
 ```
```

