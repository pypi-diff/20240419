# Comparing `tmp/rk_extractor-0.9.3.tar.gz` & `tmp/rk_extractor-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rk_extractor-0.9.3.tar", last modified: Thu Apr 18 16:02:27 2024, max compression
+gzip compressed data, was "rk_extractor-0.9.4.tar", last modified: Fri Apr 19 14:07:19 2024, max compression
```

## Comparing `rk_extractor-0.9.3.tar` & `rk_extractor-0.9.4.tar`

### file list

```diff
@@ -1,273 +1,275 @@
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      567 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8858 2024-04-18 08:16:26.000000 rk_extractor-0.9.3/README.md
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.353285 rk_extractor-0.9.3/scripts/
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/scripts/jobs/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       35 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/README.txt
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4646 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_check
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      153 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_clean
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4573 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_download
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3584 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/rxe_grid_jobs
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1791 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_ihep_check
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1984 2024-02-05 13:50:39.000000 rk_extractor-0.9.3/scripts/jobs/rxe_ihep_jobs
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3331 2024-04-18 12:55:59.000000 rk_extractor-0.9.3/scripts/jobs/rxe_local
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)    17088 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/rxe_plot_pull
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)    11926 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/rxe_plot_syst
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_run_check
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2687 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/scripts/jobs/rxe_run_toys
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)    10793 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/scripts/jobs/rxe_toys
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/scripts/offline/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5402 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/offline/analyze_result
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1647 2024-02-15 15:58:01.000000 rk_extractor-0.9.3/scripts/offline/brf_tables
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1297 2024-01-19 15:50:57.000000 rk_extractor-0.9.3/scripts/offline/calculate_sigeff
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8172 2024-03-11 18:23:43.000000 rk_extractor-0.9.3/scripts/offline/check_dist
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4570 2024-02-28 17:05:16.000000 rk_extractor-0.9.3/scripts/offline/check_jpsi_misid
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4119 2024-02-27 17:09:40.000000 rk_extractor-0.9.3/scripts/offline/cmb_prec_norm
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3690 2024-01-21 17:43:02.000000 rk_extractor-0.9.3/scripts/offline/make_signal_table
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4102 2024-02-16 14:35:53.000000 rk_extractor-0.9.3/scripts/offline/make_yields_table
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5080 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/offline/plot_check
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3020 2024-01-17 18:03:20.000000 rk_extractor-0.9.3/scripts/offline/rare_bkg_eff
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4836 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/scripts/offline/sbfit_analyze
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/setup.cfg
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1539 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/setup.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7529 2024-02-06 15:53:58.000000 rk_extractor-0.9.3/src/bdt_scale.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3662 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/cmb_ck.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     9085 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/cs_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    22377 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/extractor.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/bdt_eff/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/bdt_eff/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/config/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/config/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      122 2024-04-16 04:17:58.000000 rk_extractor-0.9.3/src/extractor_data/config/v1.toml
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      156 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/src/extractor_data/config/v2.toml
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      768 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/extractor_data/config/v3.toml
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/npr_data/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      750 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      564 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1126 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/rare_sf/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      299 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8685 2024-01-18 13:43:03.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:08:38.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:20:28.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      346 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v10/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-01-18 15:25:44.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v10/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-18 15:39:45.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v10/all_GTIS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v11/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      381 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v11/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v12/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v12/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v13/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v13/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v14/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v14/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v15/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v15/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v16/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      379 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v16/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v17/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v17/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v18/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      721 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v18/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v19/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1585 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v19/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      174 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      176 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      172 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      170 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      175 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v20/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v20/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v21/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v21/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v22/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      431 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v22/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v23/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v23/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v24/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v24/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v25/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1013 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v25/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v26/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      799 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v26/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v27/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1009 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v27/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v28/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1008 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v28/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v29/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v29/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v30/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v30/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v31/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v31/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v32/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v32/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v33/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v33/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v34/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1011 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v34/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v35/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1021 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v35/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v36/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      807 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v36/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v37/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1190 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v37/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v38/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1187 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v38/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v39/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v39/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v40/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v40/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v41/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v41/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v42/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1596 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v42/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v43/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1595 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v43/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1921 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v45/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v45/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v46/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-26 18:26:46.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v46/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      292 2024-02-27 18:46:21.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v46/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      355 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      260 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v6/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v6/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      380 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      281 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 12:23:27.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 12:35:58.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 12:40:49.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 13:55:12.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 15:17:46.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 15:19:35.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/sig_wgt/
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:48.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      529 2024-02-06 15:56:48.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:56:48.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      700 2024-02-06 16:09:04.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:47.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      181 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      184 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:53.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:53.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:56.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1441 2024-02-06 15:53:52.000000 rk_extractor-0.9.3/src/extset.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7485 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/mc_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6270 2024-02-26 17:08:18.000000 rk_extractor-0.9.3/src/model_manager.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12164 2024-02-27 18:42:34.000000 rk_extractor-0.9.3/src/normalizer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8193 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/np_reader.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/rk_extractor.egg-info/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      567 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7961 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      205 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/requires.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       16 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/top_level.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18432 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/rk_model.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18032 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/rkex_model.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    13795 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/scales.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/tests/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      774 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_cmb_eff.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      627 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_cs_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      675 2024-01-18 12:47:43.000000 rk_extractor-0.9.3/tests/test_effcalc.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18502 2024-02-16 12:59:44.000000 rk_extractor-0.9.3/tests/test_extractor.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1167 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_mc_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4786 2024-01-23 12:48:03.000000 rk_extractor-0.9.3/tests/test_model_analyzer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4615 2024-02-26 16:45:13.000000 rk_extractor-0.9.3/tests/test_model_manager.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5005 2024-02-27 18:33:17.000000 rk_extractor-0.9.3/tests/test_normalizer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      611 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/tests/test_np_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10316 2024-04-15 14:22:30.000000 rk_extractor-0.9.3/tests/test_rkmodel.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6686 2024-04-15 11:31:30.000000 rk_extractor-0.9.3/tests/test_rkrx_model.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1992 2024-01-23 12:09:37.000000 rk_extractor-0.9.3/tests/test_scales.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_scl_mkr.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1652 2024-02-06 16:08:51.000000 rk_extractor-0.9.3/tests/test_scl_rdr.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:19.000000 rk_extractor-0.9.4/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      567 2024-04-19 14:07:19.000000 rk_extractor-0.9.4/PKG-INFO
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     9021 2024-04-18 16:29:41.000000 rk_extractor-0.9.4/README.md
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:15.000000 rk_extractor-0.9.4/scripts/
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/scripts/jobs/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)       35 2024-02-07 17:05:40.000000 rk_extractor-0.9.4/scripts/jobs/README.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        2 2024-04-18 09:46:23.000000 rk_extractor-0.9.4/scripts/jobs/fake.sd
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4866 2024-04-19 13:42:04.000000 rk_extractor-0.9.4/scripts/jobs/fit_toys
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4646 2024-01-08 14:38:59.000000 rk_extractor-0.9.4/scripts/jobs/rxe_check
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)      153 2023-11-09 15:10:51.000000 rk_extractor-0.9.4/scripts/jobs/rxe_clean
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4573 2023-12-22 15:49:05.000000 rk_extractor-0.9.4/scripts/jobs/rxe_download
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3584 2024-02-07 14:56:43.000000 rk_extractor-0.9.4/scripts/jobs/rxe_grid_jobs
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1791 2024-01-08 12:36:12.000000 rk_extractor-0.9.4/scripts/jobs/rxe_ihep_check
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1894 2024-04-19 08:38:56.000000 rk_extractor-0.9.4/scripts/jobs/rxe_ihep_jobs
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3331 2024-04-18 08:24:23.000000 rk_extractor-0.9.4/scripts/jobs/rxe_local
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    17088 2024-02-13 18:52:18.000000 rk_extractor-0.9.4/scripts/jobs/rxe_plot_pull
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    11926 2024-02-08 18:55:36.000000 rk_extractor-0.9.4/scripts/jobs/rxe_plot_syst
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1353 2024-01-02 11:14:36.000000 rk_extractor-0.9.4/scripts/jobs/rxe_run_check
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     2687 2024-04-18 15:21:05.000000 rk_extractor-0.9.4/scripts/jobs/rxe_run_toys
+-rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     7432 2024-04-19 14:03:24.000000 rk_extractor-0.9.4/scripts/jobs/rxe_toys
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/scripts/offline/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5402 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/scripts/offline/analyze_result
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1647 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/scripts/offline/brf_tables
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1297 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/scripts/offline/calculate_sigeff
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8172 2024-04-15 13:59:38.000000 rk_extractor-0.9.4/scripts/offline/check_dist
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4570 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/scripts/offline/check_jpsi_misid
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4119 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/scripts/offline/cmb_prec_norm
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     3690 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/scripts/offline/make_signal_table
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4102 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/scripts/offline/make_yields_table
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5080 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/scripts/offline/plot_check
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     3020 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/scripts/offline/rare_bkg_eff
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4836 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/scripts/offline/sbfit_analyze
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)       38 2024-04-19 14:07:19.000000 rk_extractor-0.9.4/setup.cfg
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1539 2024-04-19 12:55:38.000000 rk_extractor-0.9.4/setup.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.9.4/src/__init__.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     7529 2024-02-07 14:42:07.000000 rk_extractor-0.9.4/src/bdt_scale.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     3662 2023-12-31 20:05:12.000000 rk_extractor-0.9.4/src/cmb_ck.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     9085 2023-11-26 15:18:19.000000 rk_extractor-0.9.4/src/cs_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    22377 2024-04-18 15:50:35.000000 rk_extractor-0.9.4/src/extractor.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.9.4/src/extractor_data/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/bdt_eff/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/bdt_eff/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/config/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/config/__init__.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      122 2024-04-15 14:03:50.000000 rk_extractor-0.9.4/src/extractor_data/config/v1.toml
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      156 2024-02-07 17:03:26.000000 rk_extractor-0.9.4/src/extractor_data/config/v2.toml
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      768 2024-04-18 15:09:39.000000 rk_extractor-0.9.4/src/extractor_data/config/v3.toml
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      750 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1486 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      564 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1126 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v1/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v1/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      299 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v1/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v2/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v2/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v2/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:16.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v3/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8685 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v3/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v3/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v4/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v4/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v4/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v5/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v5/eff_real.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/rare_sf/v5/fr_bf.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/__init__.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/2017_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/2017_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/2018_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/2018_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/all_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      346 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/r1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/r1_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v10/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v10/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v10/all_GTIS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v11/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      381 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v11/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v12/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v12/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v13/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v13/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v14/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v14/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v15/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v15/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v16/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      379 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v16/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v17/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v17/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v18/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      721 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v18/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v19/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1585 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v19/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v2/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      174 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v2/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      176 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v2/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      172 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v2/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      170 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v2/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      175 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v20/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v20/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v21/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v21/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v22/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      431 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v22/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v23/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v23/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v24/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v24/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v25/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1013 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v25/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v26/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      799 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v26/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v27/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1009 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v27/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v28/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1008 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v28/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v29/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v29/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v3/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v3/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v3/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v3/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v3/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v30/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v30/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v31/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v31/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v32/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v32/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v33/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v33/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v34/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1011 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v34/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v35/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1021 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v35/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:17.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v36/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      807 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v36/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v37/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1190 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v37/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v38/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1187 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v38/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v39/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v39/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/2017_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/2017_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/2018_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/2018_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/all_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/r1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/r1_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v40/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v40/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v41/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1499 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v41/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v42/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1596 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v42/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v43/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1595 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v43/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v44/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1921 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v44/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v44/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v45/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v45/all_ETOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v46/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v46/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      292 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v46/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/2017_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/2017_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/2017_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      355 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/2018_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/2018_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/2018_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/all_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/r1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/r1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      260 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/r1_MTOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v6/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-28 12:06:32.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v6/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v7/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2023-12-31 20:05:12.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v7/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      380 2023-12-31 20:05:12.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v7/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      281 2023-12-31 20:05:12.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v7/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v8/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v8/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v8/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-15 21:50:12.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v8/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:18.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v9/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-16 12:05:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v9/all_ETOS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-16 12:05:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v9/all_GTIS.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-16 12:05:27.000000 rk_extractor-0.9.4/src/extractor_data/sb_fits/v9/all_MTOS.json
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:15.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:19.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      529 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      700 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      182 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      181 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      184 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      182 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1441 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/src/extset.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     7485 2023-11-27 10:58:34.000000 rk_extractor-0.9.4/src/mc_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     6270 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/model_manager.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    12164 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/src/normalizer.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8193 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/np_reader.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:19.000000 rk_extractor-0.9.4/src/rk_extractor.egg-info/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      567 2024-04-19 14:07:14.000000 rk_extractor-0.9.4/src/rk_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     8004 2024-04-19 14:07:15.000000 rk_extractor-0.9.4/src/rk_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)        1 2024-04-19 14:07:14.000000 rk_extractor-0.9.4/src/rk_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      205 2024-04-19 14:07:14.000000 rk_extractor-0.9.4/src/rk_extractor.egg-info/requires.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)       16 2024-04-19 14:07:14.000000 rk_extractor-0.9.4/src/rk_extractor.egg-info/top_level.txt
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    18432 2024-04-19 13:19:57.000000 rk_extractor-0.9.4/src/rk_model.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    18032 2024-04-18 15:19:15.000000 rk_extractor-0.9.4/src/rkex_model.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    13795 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/src/scales.py
+drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-04-19 14:07:19.000000 rk_extractor-0.9.4/tests/
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      774 2023-12-31 20:05:12.000000 rk_extractor-0.9.4/tests/test_cmb_eff.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      627 2023-11-30 15:15:15.000000 rk_extractor-0.9.4/tests/test_cs_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      675 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/tests/test_effcalc.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    18502 2024-03-11 16:13:59.000000 rk_extractor-0.9.4/tests/test_extractor.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1167 2023-11-27 10:46:34.000000 rk_extractor-0.9.4/tests/test_mc_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4786 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/tests/test_model_analyzer.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     4615 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/tests/test_model_manager.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     5005 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/tests/test_normalizer.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      611 2024-02-06 13:59:27.000000 rk_extractor-0.9.4/tests/test_np_reader.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)    10316 2024-04-16 12:43:12.000000 rk_extractor-0.9.4/tests/test_rkmodel.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     6686 2024-04-15 13:59:38.000000 rk_extractor-0.9.4/tests/test_rkrx_model.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1992 2024-01-30 14:14:06.000000 rk_extractor-0.9.4/tests/test_scales.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2023-12-25 18:44:59.000000 rk_extractor-0.9.4/tests/test_scl_mkr.py
+-rw-r--r--   0 campoverde (12477) lhcb      (1026)     1652 2024-02-07 14:42:09.000000 rk_extractor-0.9.4/tests/test_scl_rdr.py
```

### Comparing `rk_extractor-0.9.3/PKG-INFO` & `rk_extractor-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.9.3
+Version: 0.9.4
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: toml
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
```

### Comparing `rk_extractor-0.9.3/README.md` & `rk_extractor-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -181,31 +181,35 @@
 The code will be installed from zero in each grid node.
 
 ## Local tests
 
 Before submitting one can test locally by running
 
 ```bash
-rxe_local -j 001 -n 1 -s $JOBDIR/extractor -v v3
+rxe_local -j 001 -n 1 -v v3
 ```
 
 where `v3` is the version of the TOML file in `src/extractor_data/config` that specifies the setting. The options mean:
 
 ```bash
 Used to run local tests of toy fits
 
 optional arguments:
   -h, --help            show this help message and exit
   -j JOB_ID, --job_id JOB_ID
                         Index of job
   -n NFITS, --nfits NFITS
                         Number of fits per job
-  -s SNDBX, --sndbx SNDBX
-                        Directory for output
   -v VERS, --vers VERS  Version of output
+  -s SNDBX, --sndbx SNDBX
+                        Directory for output, optional
+  -u {0,1}, --upgrade {0,1}
+                        Will upgrade before running
+  -d DIRNAME, --dirname DIRNAME
+                        Name of directory with code, optional
 ```
 
 ## IHEP tests
 
 For small tests that still require multiple fits but that can be done in the cluster:
 
 ```bash
```

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_check` & `rk_extractor-0.9.4/scripts/jobs/rxe_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_download` & `rk_extractor-0.9.4/scripts/jobs/rxe_download`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_grid_jobs` & `rk_extractor-0.9.4/scripts/jobs/rxe_grid_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_ihep_check` & `rk_extractor-0.9.4/scripts/jobs/rxe_ihep_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_ihep_jobs` & `rk_extractor-0.9.4/scripts/jobs/rxe_ihep_jobs`

 * *Files 7% similar despite different names*

```diff
@@ -69,19 +69,16 @@
     cd $JOBDIR
     OFILE=rk_extractor_%{ClusterId}_%{ProcId}
 
     echo "Jobs: $NJOB"
     echo "NFIT: $NFIT"
     echo "MEMO: $MEMO"
     echo "Queu: $QUEU"
-    echo "DSET: $DSET"
-    echo "VFIX: $VFIX"
-    echo "MODS: $MODS"
 
-    hep_sub -n $NJOB -g lhcb -e $OFILE".err" -o $OFILE".out" -argu %{ProcId} $NFIT $JOBDIR "dset:$DSET,vars:$VFIX,mods:$MODS" -mem $MEMO rxe_local -wt $QUEU 
+    hep_sub -n $NJOB -g lhcb -e $OFILE".err" -o $OFILE".out" -argu "-j\ %{ProcId}\ -n\ $NFIT\ -v\ $VERS" -mem $MEMO rxe_local -wt $QUEU 
 }
 #-----------------------------
 get_args "$@"
 check_args
 prepare
 submit
```

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_local` & `rk_extractor-0.9.4/scripts/jobs/rxe_local`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_plot_pull` & `rk_extractor-0.9.4/scripts/jobs/rxe_plot_pull`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_plot_syst` & `rk_extractor-0.9.4/scripts/jobs/rxe_plot_syst`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_run_check` & `rk_extractor-0.9.4/scripts/jobs/rxe_run_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_run_toys` & `rk_extractor-0.9.4/scripts/jobs/rxe_run_toys`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/jobs/rxe_toys` & `rk_extractor-0.9.4/scripts/jobs/rxe_toys`

 * *Files 24% similar despite different names*

```diff
@@ -5,30 +5,24 @@
 import ROOT
 import zfit
 import glob
 import math
 import toml
 import numpy
 import pprint
-import argparse
-import pandas              as pnd
-import jacobi              as jac
 import logzero
 import tarfile
-import rk.utilities        as rkut
-import utils_noroot        as utnr
+import argparse
+import subprocess
+import jacobi              as jac
 
 from importlib.resources import files
 from pprint     import pformat
-from rk_model   import rk_model  as model
-from np_reader  import np_reader as np_rdr
-from extractor  import extractor as ext
 from logzero    import logger    as log
 from zutils     import utils     as zut
-from cmb_ck     import combiner  as cmb_ck
 from log_store  import log_store
 
 #--------------------------------
 class data:
     bdt_bin = 5
     out_dir = 'results' 
     rk      = 1
@@ -78,104 +72,22 @@
     nsg_ee_err = math.sqrt(nsg_ee_var)
 
     nsg_ee_val = float(nsg_ee_val)
     nsg_ee_err = float(nsg_ee_err)
 
     return [nsg_ee_val, nsg_ee_err]
 #--------------------------------
-def add_ne(d_pos, d_pre):
-    regex='nsg_mm_(.*_TOS_.*)'
-    d_pos_ext = {}
-    for var_name in d_pos:
-        mtch = re.match(regex, var_name)
-        if not mtch:
-            continue
-
-        nsg_mm_name= mtch.group(0)
-        suffix_tos = mtch.group(1)
-        suffix_tis = mtch.group(1).replace('_TOS_', '_TIS_')
-
-        d_pos_ext[f'nsg_ee_{suffix_tos}'] = get_ne(suffix_tos, d_pos, d_pre) 
-        if f'ck_{suffix_tis}' in d_pos:
-            d_pos_ext[f'nsg_ee_{suffix_tis}'] = get_ne(suffix_tis, d_pos, d_pre)
-        else:
-            log.warning(f'TIS ck not found, skiping electron TIS yield')
-
-    d_pos.update(d_pos_ext)
-
-    return d_pos
-#--------------------------------
 def get_data(d_eff=None, d_nent=None, rseed=None): 
     mod        = model(preffix='toys_gen', d_eff=d_eff, d_nent=d_nent, l_dset=data.l_dset)
     mod.bdt_bin= data.bdt_bin 
     mod.kind   = 'nom' 
     d_dat      = mod.get_data(rseed=rseed)
 
     return d_dat
 #--------------------------------
-def fit(rseed=None, l_fix_var=None, mod_var=None):
-    log.info(f'Seed: {rseed:04}')
-    log.info(f'Variable fixed : {l_fix_var}')
-    log.info(f'Model variation: {mod_var}')
-
-    rdr          = np_rdr(sys='v65', sta='v63', yld='v24')
-    cv_sys       = rdr.get_cov(kind='sys')
-    cv_sta       = rdr.get_cov(kind='sta')
-    d_eff        = rdr.get_eff()
-    d_rjpsi      = rdr.get_rjpsi()
-    d_byld       = rdr.get_byields()
-    d_nent       = rkut.average_byields(d_byld, l_exclude=['TIS'])
-    d_rare_yld   = rkut.reso_to_rare(d_nent, kind='jpsi')
-
-    mod          = model(rk=data.rk, preffix='toys_fit', d_eff=d_eff, d_nent=d_rare_yld, l_dset=data.l_dset)
-    mod.bdt_bin  = data.bdt_bin
-    mod.kind     = 'nom' if mod_var is None else mod_var
-    d_mod        = mod.get_model() 
-    d_val, d_var = mod.get_cons() 
-    d_pre        = mod.get_prefit_pars(d_var=d_var, ck_cov=cv_sys+cv_sta)
-
-    if mod_var is None:
-        d_dat    = mod.get_data(rseed=rseed)
-    else:
-        d_dat    = get_data(d_eff=d_eff, d_nent=d_rare_yld, rseed=rseed)
-
-    if data.l_dset == ['all_TOS'] or data.l_dset == ['all_TOS', 'all_TIS']:
-        cmb                 = cmb_ck(rk=data.rk, eff=d_eff, yld=d_rare_yld)
-        cmb.out_dir         = 'plots/combination'
-        t_comb              = cmb.get_combination()
-        d_rjpsi, d_eff, cov = t_comb
-    else:
-        cov = cv_sys + cv_sta
-
-    if   data.l_dset == ['all_TOS']:
-        cov = numpy.array([[cov[0][0]]])
-    elif data.l_dset == ['all_TIS']:
-        cov = numpy.array([[cov[1][1]]])
-
-    obj          = ext(dset=data.l_dset, drop_correlations=False)
-    obj.plt_dir  = f'plots/fits_{rseed:03}'
-    obj.rjpsi    = d_rjpsi
-    obj.eff      = d_eff
-    obj.data     = d_dat
-    obj.model    = d_mod 
-    obj.fix      = l_fix_var
-    obj.cov      = cov 
-    obj.const    = d_val, d_var
-    result       = obj.get_fit_result()
-
-    log.info(f'Calculating errors')
-    result.hesse()
-    d_pos = rkut.result_to_dict(result) 
-    d_pos = add_ne(d_pos, d_pre)
-    result.freeze()
-
-    cleanup_env()
-
-    return result, {'pre' : d_pre, 'pos' : d_pos} 
-#--------------------------------
 def initialize():
     log_store.log_level     = data.log_lvl
     data.l_seed             = get_seeds()
     check_job_kind()
     os.makedirs(data.out_dir, exist_ok=True)
 #--------------------------------
 def check_job_kind():
@@ -195,21 +107,14 @@
         log.info('-------------')
         log.info('Valid:')
         log.info('-------------')
         log.info('nSeed=1; nFix > 0 or  nMod > 0')
         log.info('nSeed>1; nFix = 0 and nMod = 0')
         raise
 #--------------------------------
-def cleanup_env():
-    d_par = zfit.Parameter._existing_params
-    l_key = list(d_par.keys())
-
-    for key in l_key:
-        del(d_par[key])
-#--------------------------------
 def get_args():
     parser = argparse.ArgumentParser(description='Used run toy fits on model used to extract RK')
     parser.add_argument('-l', '--level' , type=int, help='Logging level', choices=[logzero.DEBUG, logzero.INFO, logzero.WARNING], default=logzero.INFO)
     parser.add_argument('-v', '--vers'  , type=str, help='Version of configuration', required=True) 
     args = parser.parse_args()
 
     data.log_lvl = args.level
@@ -255,47 +160,53 @@
     log.info('-' * 40)
     log.info(f'{"Level":<20}{data.log_lvl}')
     log.info(f'{"Datasets":<20}{data.l_dset}')
     log.info(f'{"Vars fixed":<20}{data.l_fixed}')
     log.info(f'{"Models":<20}{data.l_model}')
     log.info('-' * 40)
 #--------------------------------
+def run_command(command, arguments=None):
+    if not isinstance(arguments, list):
+        log.error(f'Invalid options argument: {arguments}')
+        raise ValueError
+
+    log.info('-' * 30)
+    log.info('-' * 30)
+    log.info(f'{command:<10}{str(arguments):<50}')
+    log.info('-' * 30)
+    log.info('-' * 30)
+
+    stat = subprocess.run([command] + arguments)
+
+    if stat.returncode != 0:
+        log.error(f'Process returned exit status: {stat.returncode}')
+        raise
+#--------------------------------
 def run_pull_fits():
     if not data.for_pull:
         return
 
     for rseed in data.l_seed:
-        res, d_inf = fit(rseed=rseed)
-        print(res)
-        utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{rseed:04}.pkl')
-        utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{rseed:04}.json')
+        run_command('fit_toys', arguments=['-s', rseed])
 #--------------------------------
 def run_syst_fits():
     if not data.for_syst:
         return
 
     [rseed] = data.l_seed
-    res, d_inf = fit(rseed=rseed)
-    print(res)
-    utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{rseed:04}.pkl')
-    utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{rseed:04}.json')
+    run_command('fit_toys', arguments=['-s', rseed])
 
     l_fix_var = []
     for fix_var in data.l_fixed:
         l_fix_var.append(fix_var)
-        res, d_inf = fit(rseed=rseed, l_fix_var=l_fix_var)
-        print(res)
-        utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{fix_var}.pkl')
-        utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{fix_var}.json')
+        ' '.join(l_fix_var)
+        run_command('fit_toys', arguments=['-s', rseed, '-f', fix_var])
 
     for mod_var in data.l_model:
-        res, d_inf = fit(rseed=rseed, mod_var=mod_var)
-        print(res)
-        utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{mod_var}.pkl')
-        utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{mod_var}.json')
+        run_command('fit_toys', arguments=['-s', rseed, '-m', mod_var])
 #--------------------------------
 def main():
     get_args()
     print_args()
     initialize()
     run_pull_fits()
     run_syst_fits()
```

### Comparing `rk_extractor-0.9.3/scripts/offline/analyze_result` & `rk_extractor-0.9.4/scripts/offline/analyze_result`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/brf_tables` & `rk_extractor-0.9.4/scripts/offline/brf_tables`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/calculate_sigeff` & `rk_extractor-0.9.4/scripts/offline/calculate_sigeff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/check_dist` & `rk_extractor-0.9.4/scripts/offline/check_dist`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/check_jpsi_misid` & `rk_extractor-0.9.4/scripts/offline/check_jpsi_misid`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/cmb_prec_norm` & `rk_extractor-0.9.4/scripts/offline/cmb_prec_norm`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/make_signal_table` & `rk_extractor-0.9.4/scripts/offline/make_signal_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/make_yields_table` & `rk_extractor-0.9.4/scripts/offline/make_yields_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/plot_check` & `rk_extractor-0.9.4/scripts/offline/plot_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/rare_bkg_eff` & `rk_extractor-0.9.4/scripts/offline/rare_bkg_eff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/scripts/offline/sbfit_analyze` & `rk_extractor-0.9.4/scripts/offline/sbfit_analyze`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/setup.py` & `rk_extractor-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     else:
         raise
 
     return l_pkg
 #----------------------------------------------
 setup(
         name              = 'rk_extractor',
-        version           = '0.9.3',
+        version           = '0.9.4',
         description       = 'Used to extract RK from simultaneous fits',
         scripts           = get_scripts('scripts/jobs') + get_scripts('scripts/offline'),
         long_description  = '',
         packages          = get_packages(),
         package_dir       = {'' : 'src'},
         package_data      = {'extractor_data' : get_data_packages('extractor_data')}, 
         install_requires  = open('requirements.txt').read().splitlines()
```

### Comparing `rk_extractor-0.9.3/src/bdt_scale.py` & `rk_extractor-0.9.4/src/bdt_scale.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/cmb_ck.py` & `rk_extractor-0.9.4/src/cmb_ck.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/cs_reader.py` & `rk_extractor-0.9.4/src/cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor.py` & `rk_extractor-0.9.4/src/extractor.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/config/v3.toml` & `rk_extractor-0.9.4/src/extractor_data/config/v3.toml`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json` & `rk_extractor-0.9.4/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/eff_real.json` & `rk_extractor-0.9.4/src/extractor_data/rare_sf/v1/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/eff_real.json` & `rk_extractor-0.9.4/src/extractor_data/rare_sf/v2/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/eff_real.json` & `rk_extractor-0.9.4/src/extractor_data/rare_sf/v3/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/eff_real.json` & `rk_extractor-0.9.4/src/extractor_data/rare_sf/v4/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/eff_real.json` & `rk_extractor-0.9.4/src/extractor_data/rare_sf/v5/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v18/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v18/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v19/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v19/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v25/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v25/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v26/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v26/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v27/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v27/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v28/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v28/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v34/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v34/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v35/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v35/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v36/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v36/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v37/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v37/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v38/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v38/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v39/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v39/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v40/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v40/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v41/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v41/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v42/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v42/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v43/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v43/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/all_ETOS.json` & `rk_extractor-0.9.4/src/extractor_data/sb_fits/v44/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json` & `rk_extractor-0.9.4/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/extset.py` & `rk_extractor-0.9.4/src/extset.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/mc_reader.py` & `rk_extractor-0.9.4/src/mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/model_manager.py` & `rk_extractor-0.9.4/src/model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/normalizer.py` & `rk_extractor-0.9.4/src/normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/np_reader.py` & `rk_extractor-0.9.4/src/np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/rk_extractor.egg-info/PKG-INFO` & `rk_extractor-0.9.4/src/rk_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.9.3
+Version: 0.9.4
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: toml
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
```

### Comparing `rk_extractor-0.9.3/src/rk_extractor.egg-info/SOURCES.txt` & `rk_extractor-0.9.4/src/rk_extractor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 README.md
 setup.py
 scripts/jobs/README.txt
+scripts/jobs/fake.sd
+scripts/jobs/fit_toys
 scripts/jobs/rxe_check
 scripts/jobs/rxe_clean
 scripts/jobs/rxe_download
 scripts/jobs/rxe_grid_jobs
 scripts/jobs/rxe_ihep_check
 scripts/jobs/rxe_ihep_jobs
 scripts/jobs/rxe_local
```

### Comparing `rk_extractor-0.9.3/src/rk_model.py` & `rk_extractor-0.9.4/src/rk_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/rkex_model.py` & `rk_extractor-0.9.4/src/rkex_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/src/scales.py` & `rk_extractor-0.9.4/src/scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_cmb_eff.py` & `rk_extractor-0.9.4/tests/test_cmb_eff.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_cs_reader.py` & `rk_extractor-0.9.4/tests/test_cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_effcalc.py` & `rk_extractor-0.9.4/tests/test_effcalc.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_extractor.py` & `rk_extractor-0.9.4/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_mc_reader.py` & `rk_extractor-0.9.4/tests/test_mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_model_analyzer.py` & `rk_extractor-0.9.4/tests/test_model_analyzer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_model_manager.py` & `rk_extractor-0.9.4/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_normalizer.py` & `rk_extractor-0.9.4/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_np_reader.py` & `rk_extractor-0.9.4/tests/test_np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_rkmodel.py` & `rk_extractor-0.9.4/tests/test_rkmodel.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_rkrx_model.py` & `rk_extractor-0.9.4/tests/test_rkrx_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_scales.py` & `rk_extractor-0.9.4/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_scl_mkr.py` & `rk_extractor-0.9.4/tests/test_scl_mkr.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.3/tests/test_scl_rdr.py` & `rk_extractor-0.9.4/tests/test_scl_rdr.py`

 * *Files identical despite different names*

