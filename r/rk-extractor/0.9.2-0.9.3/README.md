# Comparing `tmp/rk_extractor-0.9.2.tar.gz` & `tmp/rk_extractor-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rk_extractor-0.9.2.tar", last modified: Thu Apr 18 08:17:55 2024, max compression
+gzip compressed data, was "rk_extractor-0.9.3.tar", last modified: Thu Apr 18 16:02:27 2024, max compression
```

## Comparing `rk_extractor-0.9.2.tar` & `rk_extractor-0.9.3.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.307170 rk_extractor-0.9.2/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      567 2024-04-18 08:17:55.307170 rk_extractor-0.9.2/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8858 2024-04-18 08:16:26.000000 rk_extractor-0.9.2/README.md
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.247170 rk_extractor-0.9.2/scripts/
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.257170 rk_extractor-0.9.2/scripts/jobs/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       35 2024-02-15 15:33:22.000000 rk_extractor-0.9.2/scripts/jobs/README.txt
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4646 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/jobs/rxe_check
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      153 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/jobs/rxe_clean
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4573 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/jobs/rxe_download
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3584 2024-02-15 15:33:22.000000 rk_extractor-0.9.2/scripts/jobs/rxe_grid_jobs
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1791 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/jobs/rxe_ihep_check
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1984 2024-02-05 13:50:39.000000 rk_extractor-0.9.2/scripts/jobs/rxe_ihep_jobs
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3325 2024-04-18 08:16:26.000000 rk_extractor-0.9.2/scripts/jobs/rxe_local
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)    17088 2024-02-15 15:33:22.000000 rk_extractor-0.9.2/scripts/jobs/rxe_plot_pull
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)    11926 2024-02-15 15:33:22.000000 rk_extractor-0.9.2/scripts/jobs/rxe_plot_syst
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1353 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/jobs/rxe_run_check
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2470 2024-04-18 08:16:26.000000 rk_extractor-0.9.2/scripts/jobs/rxe_run_toys
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)    11182 2024-04-15 11:15:40.000000 rk_extractor-0.9.2/scripts/jobs/rxe_toys
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.257170 rk_extractor-0.9.2/scripts/offline/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5402 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/offline/analyze_result
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1647 2024-02-15 15:58:01.000000 rk_extractor-0.9.2/scripts/offline/brf_tables
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1297 2024-01-19 15:50:57.000000 rk_extractor-0.9.2/scripts/offline/calculate_sigeff
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8172 2024-03-11 18:23:43.000000 rk_extractor-0.9.2/scripts/offline/check_dist
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4570 2024-02-28 17:05:16.000000 rk_extractor-0.9.2/scripts/offline/check_jpsi_misid
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4119 2024-02-27 17:09:40.000000 rk_extractor-0.9.2/scripts/offline/cmb_prec_norm
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3690 2024-01-21 17:43:02.000000 rk_extractor-0.9.2/scripts/offline/make_signal_table
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4102 2024-02-16 14:35:53.000000 rk_extractor-0.9.2/scripts/offline/make_yields_table
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5080 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/scripts/offline/plot_check
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3020 2024-01-17 18:03:20.000000 rk_extractor-0.9.2/scripts/offline/rare_bkg_eff
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4836 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/scripts/offline/sbfit_analyze
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-04-18 08:17:55.307170 rk_extractor-0.9.2/setup.cfg
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1539 2024-04-18 08:15:41.000000 rk_extractor-0.9.2/setup.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7529 2024-02-06 15:53:58.000000 rk_extractor-0.9.2/src/bdt_scale.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3662 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/cmb_ck.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     9085 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/cs_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    22377 2024-01-24 11:07:35.000000 rk_extractor-0.9.2/src/extractor.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/bdt_eff/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/bdt_eff/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/config/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/config/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      122 2024-04-16 04:17:58.000000 rk_extractor-0.9.2/src/extractor_data/config/v1.toml
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      156 2024-02-15 15:33:22.000000 rk_extractor-0.9.2/src/extractor_data/config/v2.toml
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      740 2024-04-15 13:53:55.000000 rk_extractor-0.9.2/src/extractor_data/config/v3.toml
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/npr_data/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      750 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      564 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1126 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/rare_sf/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/rare_sf/v1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v1/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      299 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v1/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/rare_sf/v2/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v2/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v2/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/rare_sf/v3/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8685 2024-01-18 13:43:03.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v3/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v3/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/rare_sf/v4/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:08:38.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v4/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v4/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/rare_sf/v5/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:20:28.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v5/eff_real.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.2/src/extractor_data/rare_sf/v5/fr_bf.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.267170 rk_extractor-0.9.2/src/extractor_data/sb_fits/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      346 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v10/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-01-18 15:25:44.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v10/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-18 15:39:45.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v10/all_GTIS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v11/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      381 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v11/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v12/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v12/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v13/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v13/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v14/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v14/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v15/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v15/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v16/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      379 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v16/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v17/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v17/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v18/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      721 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v18/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v19/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1585 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v19/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v2/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      174 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v2/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      176 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v2/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      172 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v2/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      170 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v2/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      175 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v20/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v20/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v21/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v21/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v22/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      431 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v22/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v23/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v23/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v24/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v24/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v25/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1013 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v25/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v26/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      799 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v26/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.277170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v27/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1009 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v27/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v28/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1008 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v28/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v29/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v29/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v3/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v3/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v3/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v3/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v3/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v30/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v30/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v31/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v31/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v32/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v32/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v33/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v33/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v34/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1011 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v34/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v35/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1021 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v35/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v36/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      807 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v36/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v37/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1190 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v37/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v38/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1187 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v38/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v39/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v39/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v40/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v40/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v41/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v41/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v42/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1596 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v42/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v43/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1595 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v43/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.287170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v44/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1921 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v44/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v44/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v45/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v45/all_ETOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v46/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-26 18:26:46.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v46/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      292 2024-02-27 18:46:21.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v46/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      355 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      260 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v6/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v6/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v7/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v7/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      380 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v7/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      281 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v7/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v8/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 12:23:27.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v8/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 12:35:58.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v8/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 12:40:49.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v8/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.297170 rk_extractor-0.9.2/src/extractor_data/sb_fits/v9/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 13:55:12.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v9/all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 15:17:46.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v9/all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 15:19:35.000000 rk_extractor-0.9.2/src/extractor_data/sb_fits/v9/all_MTOS.json
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.257170 rk_extractor-0.9.2/src/extractor_data/sig_wgt/
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.307170 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:48.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      529 2024-02-06 15:56:48.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:56:48.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      700 2024-02-06 16:09:04.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:47.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      181 2024-02-16 14:25:16.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      184 2024-02-16 14:25:16.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:53.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:53.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:56.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1441 2024-02-06 15:53:52.000000 rk_extractor-0.9.2/src/extset.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7485 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/src/mc_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6270 2024-02-26 17:08:18.000000 rk_extractor-0.9.2/src/model_manager.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12164 2024-02-27 18:42:34.000000 rk_extractor-0.9.2/src/normalizer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8193 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/np_reader.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.307170 rk_extractor-0.9.2/src/rk_extractor.egg-info/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      567 2024-04-18 08:17:55.000000 rk_extractor-0.9.2/src/rk_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7961 2024-04-18 08:17:55.000000 rk_extractor-0.9.2/src/rk_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-04-18 08:17:55.000000 rk_extractor-0.9.2/src/rk_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      205 2024-04-18 08:17:55.000000 rk_extractor-0.9.2/src/rk_extractor.egg-info/requires.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       16 2024-04-18 08:17:55.000000 rk_extractor-0.9.2/src/rk_extractor.egg-info/top_level.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18432 2024-04-16 04:15:23.000000 rk_extractor-0.9.2/src/rk_model.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    17951 2024-04-15 12:41:07.000000 rk_extractor-0.9.2/src/rkex_model.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    13795 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/src/scales.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 08:17:55.307170 rk_extractor-0.9.2/tests/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      774 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/tests/test_cmb_eff.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      627 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/tests/test_cs_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      675 2024-01-18 12:47:43.000000 rk_extractor-0.9.2/tests/test_effcalc.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18502 2024-02-16 12:59:44.000000 rk_extractor-0.9.2/tests/test_extractor.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1167 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/tests/test_mc_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4786 2024-01-23 12:48:03.000000 rk_extractor-0.9.2/tests/test_model_analyzer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4615 2024-02-26 16:45:13.000000 rk_extractor-0.9.2/tests/test_model_manager.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5005 2024-02-27 18:33:17.000000 rk_extractor-0.9.2/tests/test_normalizer.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      611 2024-02-05 11:35:54.000000 rk_extractor-0.9.2/tests/test_np_reader.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10316 2024-04-15 14:22:30.000000 rk_extractor-0.9.2/tests/test_rkmodel.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6686 2024-04-15 11:31:30.000000 rk_extractor-0.9.2/tests/test_rkrx_model.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1992 2024-01-23 12:09:37.000000 rk_extractor-0.9.2/tests/test_scales.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-01-13 16:48:29.000000 rk_extractor-0.9.2/tests/test_scl_mkr.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1652 2024-02-06 16:08:51.000000 rk_extractor-0.9.2/tests/test_scl_rdr.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      567 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8858 2024-04-18 08:16:26.000000 rk_extractor-0.9.3/README.md
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.353285 rk_extractor-0.9.3/scripts/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/scripts/jobs/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       35 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/README.txt
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4646 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_check
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      153 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_clean
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4573 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_download
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3584 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/rxe_grid_jobs
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1791 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_ihep_check
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1984 2024-02-05 13:50:39.000000 rk_extractor-0.9.3/scripts/jobs/rxe_ihep_jobs
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3331 2024-04-18 12:55:59.000000 rk_extractor-0.9.3/scripts/jobs/rxe_local
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)    17088 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/rxe_plot_pull
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)    11926 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/scripts/jobs/rxe_plot_syst
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/jobs/rxe_run_check
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2687 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/scripts/jobs/rxe_run_toys
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)    10793 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/scripts/jobs/rxe_toys
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/scripts/offline/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5402 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/offline/analyze_result
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1647 2024-02-15 15:58:01.000000 rk_extractor-0.9.3/scripts/offline/brf_tables
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1297 2024-01-19 15:50:57.000000 rk_extractor-0.9.3/scripts/offline/calculate_sigeff
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8172 2024-03-11 18:23:43.000000 rk_extractor-0.9.3/scripts/offline/check_dist
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4570 2024-02-28 17:05:16.000000 rk_extractor-0.9.3/scripts/offline/check_jpsi_misid
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4119 2024-02-27 17:09:40.000000 rk_extractor-0.9.3/scripts/offline/cmb_prec_norm
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3690 2024-01-21 17:43:02.000000 rk_extractor-0.9.3/scripts/offline/make_signal_table
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4102 2024-02-16 14:35:53.000000 rk_extractor-0.9.3/scripts/offline/make_yields_table
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5080 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/scripts/offline/plot_check
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3020 2024-01-17 18:03:20.000000 rk_extractor-0.9.3/scripts/offline/rare_bkg_eff
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4836 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/scripts/offline/sbfit_analyze
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/setup.cfg
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1539 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/setup.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7529 2024-02-06 15:53:58.000000 rk_extractor-0.9.3/src/bdt_scale.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3662 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/cmb_ck.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9085 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/cs_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    22377 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/extractor.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/bdt_eff/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/bdt_eff/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/config/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/config/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      122 2024-04-16 04:17:58.000000 rk_extractor-0.9.3/src/extractor_data/config/v1.toml
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      156 2024-02-15 15:33:22.000000 rk_extractor-0.9.3/src/extractor_data/config/v2.toml
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      768 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/extractor_data/config/v3.toml
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/npr_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      750 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      564 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1126 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/rare_sf/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      299 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8685 2024-01-18 13:43:03.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:08:38.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:20:28.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      346 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v10/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-01-18 15:25:44.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v10/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-18 15:39:45.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v10/all_GTIS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v11/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      381 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v11/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v12/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v12/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v13/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v13/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v14/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v14/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v15/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v15/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v16/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      379 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v16/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v17/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v17/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v18/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      721 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v18/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v19/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1585 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v19/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      174 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      176 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      172 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      170 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      175 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v20/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v20/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v21/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v21/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v22/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      431 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v22/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v23/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v23/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v24/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v24/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v25/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1013 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v25/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v26/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      799 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v26/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v27/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1009 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v27/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v28/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1008 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v28/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v29/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v29/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v30/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v30/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v31/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v31/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v32/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v32/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v33/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v33/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v34/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1011 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v34/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v35/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1021 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v35/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v36/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      807 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v36/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v37/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1190 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v37/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v38/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1187 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v38/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v39/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v39/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v40/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v40/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v41/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v41/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v42/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1596 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v42/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v43/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1595 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v43/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1921 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v45/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v45/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.373285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v46/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-26 18:26:46.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v46/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      292 2024-02-27 18:46:21.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v46/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      355 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      260 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v6/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v6/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      380 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      281 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v7/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 12:23:27.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 12:35:58.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 12:40:49.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v8/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 13:55:12.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 15:17:46.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 15:19:35.000000 rk_extractor-0.9.3/src/extractor_data/sb_fits/v9/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.363285 rk_extractor-0.9.3/src/extractor_data/sig_wgt/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:48.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      529 2024-02-06 15:56:48.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:56:48.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      700 2024-02-06 16:09:04.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:47.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      181 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      184 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:53.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:53.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:56.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1441 2024-02-06 15:53:52.000000 rk_extractor-0.9.3/src/extset.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7485 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/src/mc_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6270 2024-02-26 17:08:18.000000 rk_extractor-0.9.3/src/model_manager.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12164 2024-02-27 18:42:34.000000 rk_extractor-0.9.3/src/normalizer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8193 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/np_reader.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/src/rk_extractor.egg-info/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      567 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7961 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      205 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/requires.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       16 2024-04-18 16:02:27.000000 rk_extractor-0.9.3/src/rk_extractor.egg-info/top_level.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18432 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/rk_model.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18032 2024-04-18 16:02:06.000000 rk_extractor-0.9.3/src/rkex_model.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    13795 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/src/scales.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-18 16:02:27.383285 rk_extractor-0.9.3/tests/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      774 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_cmb_eff.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      627 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_cs_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      675 2024-01-18 12:47:43.000000 rk_extractor-0.9.3/tests/test_effcalc.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18502 2024-02-16 12:59:44.000000 rk_extractor-0.9.3/tests/test_extractor.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1167 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_mc_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4786 2024-01-23 12:48:03.000000 rk_extractor-0.9.3/tests/test_model_analyzer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4615 2024-02-26 16:45:13.000000 rk_extractor-0.9.3/tests/test_model_manager.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5005 2024-02-27 18:33:17.000000 rk_extractor-0.9.3/tests/test_normalizer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      611 2024-02-05 11:35:54.000000 rk_extractor-0.9.3/tests/test_np_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10316 2024-04-15 14:22:30.000000 rk_extractor-0.9.3/tests/test_rkmodel.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6686 2024-04-15 11:31:30.000000 rk_extractor-0.9.3/tests/test_rkrx_model.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1992 2024-01-23 12:09:37.000000 rk_extractor-0.9.3/tests/test_scales.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-01-13 16:48:29.000000 rk_extractor-0.9.3/tests/test_scl_mkr.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1652 2024-02-06 16:08:51.000000 rk_extractor-0.9.3/tests/test_scl_rdr.py
```

### Comparing `rk_extractor-0.9.2/PKG-INFO` & `rk_extractor-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.9.2
+Version: 0.9.3
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: toml
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
```

### Comparing `rk_extractor-0.9.2/README.md` & `rk_extractor-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_check` & `rk_extractor-0.9.3/scripts/jobs/rxe_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_download` & `rk_extractor-0.9.3/scripts/jobs/rxe_download`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_grid_jobs` & `rk_extractor-0.9.3/scripts/jobs/rxe_grid_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_ihep_check` & `rk_extractor-0.9.3/scripts/jobs/rxe_ihep_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_ihep_jobs` & `rk_extractor-0.9.3/scripts/jobs/rxe_ihep_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_local` & `rk_extractor-0.9.3/scripts/jobs/rxe_local`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #----------------------------
 def get_args():
     parser = argparse.ArgumentParser(description='Used to run local tests of toy fits')
     parser.add_argument('-j', '--job_id' , type=int, help='Index of job'                         , required=True)
     parser.add_argument('-n', '--nfits'  , type=int, help='Number of fits per job'               , required=True)
     parser.add_argument('-v', '--vers'   , type=str, help='Version of output'                    , required=True)
     parser.add_argument('-s', '--sndbx'  , type=str, help='Directory for output, optional'       , default=data.sandbox)
-    parser.add_argument('-u', '--upgrade', type=int, help='Will upgrade before running'          , default=0, choices=[0, 1])
+    parser.add_argument('-u', '--upgrade', type=str, help='Will upgrade before running'          , default='0', choices=['0', '1'])
     parser.add_argument('-d', '--dirname', type=str, help='Name of directory with code, optional', default=data.sft_name)
     args = parser.parse_args()
 
     data.jobid   = args.job_id
     data.nfits   = args.nfits
     data.vers    = args.vers
     data.sandbox = f'{args.sndbx}/{str(data.jobid).rjust(3, "0")}_{str(data.nfits).rjust(3, "0")}'
```

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_plot_pull` & `rk_extractor-0.9.3/scripts/jobs/rxe_plot_pull`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_plot_syst` & `rk_extractor-0.9.3/scripts/jobs/rxe_plot_syst`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_run_check` & `rk_extractor-0.9.3/scripts/jobs/rxe_run_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_run_toys` & `rk_extractor-0.9.3/scripts/jobs/rxe_run_toys`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 #!/usr/bin/env bash
 
 #--------------------------------------
+set_vars()
+{
+    echo "Turning off multithreading"
+    export MKL_NUM_THREADS=1
+    export NUMEXPR_NUM_THREADS=1
+    export OMP_NUM_THREADS=1
+    export OPENBLAS_NUM_THREADS=1
+}
+#--------------------------------------
 set_paths()
 {
     if   [[   -z $RK_TOY ]];then
 	echo "No toy path found"
         VENV=$PWD/RK_TOY
 	INSTALL=1
     elif [[ ! -d $RK_TOY ]];then
@@ -87,22 +96,23 @@
     pip install --upgrade rx_tools
     pip install --upgrade rk_extractor
 }
 #--------------------------------------
 run()
 {
     echo "--------------------"
-    echo "Running rxe_run_toys with args: $VERS" 
     PYPATH=$(which python)
     echo "Using python $PYPATH"
+    echo "Running: ./rxe_toys -v $VERS"
     ./rxe_toys -v $VERS 
     echo "--------------------"
 }
 #--------------------------------------
 VERS=$1
 UPGR=$2
 
 set_paths
+set_vars
 install_sft
 upgrade
 run
```

### Comparing `rk_extractor-0.9.2/scripts/jobs/rxe_toys` & `rk_extractor-0.9.3/scripts/jobs/rxe_toys`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 import argparse
 import pandas              as pnd
 import jacobi              as jac
 import logzero
 import tarfile
 import rk.utilities        as rkut
 import utils_noroot        as utnr
-import concurrent.futures  as cf
 
 from importlib.resources import files
 from pprint     import pformat
 from rk_model   import rk_model  as model
 from np_reader  import np_reader as np_rdr
 from extractor  import extractor as ext
 from logzero    import logger    as log
 from zutils     import utils     as zut
 from cmb_ck     import combiner  as cmb_ck
+from log_store  import log_store
 
 #--------------------------------
 class data:
     bdt_bin = 5
     out_dir = 'results' 
     rk      = 1
     l_seed  = None
@@ -169,16 +169,16 @@
     result.freeze()
 
     cleanup_env()
 
     return result, {'pre' : d_pre, 'pos' : d_pos} 
 #--------------------------------
 def initialize():
-    log.setLevel(data.log_lvl)
-    data.l_seed  = get_seeds()
+    log_store.log_level     = data.log_lvl
+    data.l_seed             = get_seeds()
     check_job_kind()
     os.makedirs(data.out_dir, exist_ok=True)
 #--------------------------------
 def check_job_kind():
     nseed = len(data.l_seed)
     nfix  = len(data.l_fixed)
     nmod  = len(data.l_model)
@@ -260,47 +260,39 @@
     log.info('-' * 40)
 #--------------------------------
 def run_pull_fits():
     if not data.for_pull:
         return
 
     for rseed in data.l_seed:
-        with cf.ProcessPoolExecutor(max_workers=1) as executor:
-            res, d_inf = executor.submit(fit, **{'rseed': rseed}).result()
-
+        res, d_inf = fit(rseed=rseed)
         print(res)
         utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{rseed:04}.pkl')
         utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{rseed:04}.json')
 #--------------------------------
 def run_syst_fits():
     if not data.for_syst:
         return
 
     [rseed] = data.l_seed
-    with cf.ProcessPoolExecutor(max_workers=1) as executor:
-        res, d_inf = executor.submit(fit, **{'rseed': rseed}).result()
-
+    res, d_inf = fit(rseed=rseed)
     print(res)
     utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{rseed:04}.pkl')
     utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{rseed:04}.json')
 
     l_fix_var = []
     for fix_var in data.l_fixed:
         l_fix_var.append(fix_var)
-        with cf.ProcessPoolExecutor(max_workers=1) as executor:
-            res, d_inf = executor.submit(fit, **{'rseed': rseed, 'l_fix_var' : l_fix_var}).result()
-
+        res, d_inf = fit(rseed=rseed, l_fix_var=l_fix_var)
         print(res)
         utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{fix_var}.pkl')
         utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{fix_var}.json')
 
     for mod_var in data.l_model:
-        with cf.ProcessPoolExecutor(max_workers=1) as executor:
-            res, d_inf = executor.submit(fit, **{'rseed': rseed, 'mod_var' : mod_var}).result()
-
+        res, d_inf = fit(rseed=rseed, mod_var=mod_var)
         print(res)
         utnr.dump_pickle(res, f'{data.out_dir}/result_pkl/result_{mod_var}.pkl')
         utnr.dump_json(d_inf, f'{data.out_dir}/result_jsn/result_{mod_var}.json')
 #--------------------------------
 def main():
     get_args()
     print_args()
```

### Comparing `rk_extractor-0.9.2/scripts/offline/analyze_result` & `rk_extractor-0.9.3/scripts/offline/analyze_result`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/brf_tables` & `rk_extractor-0.9.3/scripts/offline/brf_tables`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/calculate_sigeff` & `rk_extractor-0.9.3/scripts/offline/calculate_sigeff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/check_dist` & `rk_extractor-0.9.3/scripts/offline/check_dist`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/check_jpsi_misid` & `rk_extractor-0.9.3/scripts/offline/check_jpsi_misid`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/cmb_prec_norm` & `rk_extractor-0.9.3/scripts/offline/cmb_prec_norm`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/make_signal_table` & `rk_extractor-0.9.3/scripts/offline/make_signal_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/make_yields_table` & `rk_extractor-0.9.3/scripts/offline/make_yields_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/plot_check` & `rk_extractor-0.9.3/scripts/offline/plot_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/rare_bkg_eff` & `rk_extractor-0.9.3/scripts/offline/rare_bkg_eff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/scripts/offline/sbfit_analyze` & `rk_extractor-0.9.3/scripts/offline/sbfit_analyze`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/setup.py` & `rk_extractor-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     else:
         raise
 
     return l_pkg
 #----------------------------------------------
 setup(
         name              = 'rk_extractor',
-        version           = '0.9.2',
+        version           = '0.9.3',
         description       = 'Used to extract RK from simultaneous fits',
         scripts           = get_scripts('scripts/jobs') + get_scripts('scripts/offline'),
         long_description  = '',
         packages          = get_packages(),
         package_dir       = {'' : 'src'},
         package_data      = {'extractor_data' : get_data_packages('extractor_data')}, 
         install_requires  = open('requirements.txt').read().splitlines()
```

### Comparing `rk_extractor-0.9.2/src/bdt_scale.py` & `rk_extractor-0.9.3/src/bdt_scale.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/cmb_ck.py` & `rk_extractor-0.9.3/src/cmb_ck.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/cs_reader.py` & `rk_extractor-0.9.3/src/cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor.py` & `rk_extractor-0.9.3/src/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         return mod_mm
     #--------------------------------
     def _add_fixed_par(self, par):
         par.floating          = False
         self._d_fix['Name']  += [par.name]
         self._d_fix['Value'] += [float(par.numpy())]
 
-        log.warning(f'{par.name:<20}{"=":20}{par.value():<20.3e}')
+        log.warning(f'{par.name:<60}{"=":20}{par.value():<20.3e}')
     #--------------------------------
     def _get_yld(self, model, preffix):
         l_param   = model.get_params(is_yield=True)
 
         l_sig_yld = [ param for param in l_param if param.name.startswith(preffix)]
         [sig_yld] = l_sig_yld
```

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json` & `rk_extractor-0.9.3/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/rare_sf/v1/eff_real.json` & `rk_extractor-0.9.3/src/extractor_data/rare_sf/v1/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/rare_sf/v2/eff_real.json` & `rk_extractor-0.9.3/src/extractor_data/rare_sf/v2/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/rare_sf/v3/eff_real.json` & `rk_extractor-0.9.3/src/extractor_data/rare_sf/v3/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/rare_sf/v4/eff_real.json` & `rk_extractor-0.9.3/src/extractor_data/rare_sf/v4/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/rare_sf/v5/eff_real.json` & `rk_extractor-0.9.3/src/extractor_data/rare_sf/v5/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v18/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v18/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v19/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v19/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v25/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v25/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v26/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v26/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v27/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v27/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v28/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v28/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v34/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v34/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v35/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v35/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v36/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v36/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v37/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v37/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v38/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v38/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v39/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v39/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v40/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v40/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v41/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v41/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v42/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v42/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v43/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v43/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sb_fits/v44/all_ETOS.json` & `rk_extractor-0.9.3/src/extractor_data/sb_fits/v44/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json` & `rk_extractor-0.9.3/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/extset.py` & `rk_extractor-0.9.3/src/extset.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/mc_reader.py` & `rk_extractor-0.9.3/src/mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/model_manager.py` & `rk_extractor-0.9.3/src/model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/normalizer.py` & `rk_extractor-0.9.3/src/normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/np_reader.py` & `rk_extractor-0.9.3/src/np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/rk_extractor.egg-info/PKG-INFO` & `rk_extractor-0.9.3/src/rk_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.9.2
+Version: 0.9.3
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: toml
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
```

### Comparing `rk_extractor-0.9.2/src/rk_extractor.egg-info/SOURCES.txt` & `rk_extractor-0.9.3/src/rk_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/src/rk_model.py` & `rk_extractor-0.9.3/src/rk_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,19 +469,19 @@
         -----------
         d_val, d_var: Tuple of dictionaries pairing parameter name with value (mu of Gaussian) and 
         variance respectively.
         '''
         self._initialize()
 
         log.debug('-' * 20)
-        log.debug(f'{"Name":<40}{"Value":<15}{"Variance":<15}')
+        log.debug(f'{"Name":<60}{"Value":<15}{"Variance":<15}')
         log.debug('-' * 20)
         for name in self._d_val:
             val = self._d_val[name]
             var = self._d_var[name]
 
-            log.debug(f'{name:<40}{val:<15.3f}{var:<15.3f}')
+            log.debug(f'{name:<60}{val:<15.3f}{var:<15.3f}')
         log.debug('-' * 20)
 
         return self._d_val, self._d_var
 #---------------------------------------------------------------
```

### Comparing `rk_extractor-0.9.2/src/rkex_model.py` & `rk_extractor-0.9.3/src/rkex_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,43 +400,46 @@
 
         Parameters:
         -----------------
         rseed  (int):  Random seed
 
         Returns:
         -----------------
-        d_data (dict): Dictionary with dataset and tuple of zfit data objects paired, i.e. {r1_TOS : (pdf_mm, pdf_ee) }
+        d_data (dict): Dictionary with dataset and tuple of zfit data objects paired, i.e. {r1_TOS : (zdata_mm, zdata_ee) }
 
         For muon, TIS dataset is the TOS one.
         '''
         self._initialize()
 
         zfit.settings.set_seed(rseed)
 
         d_data     = {}
         dst_mm_tos = None
         for ds, (pdf_mm, pdf_ee) in self._d_mod.items():
-            dst_mm         = pdf_mm.create_sampler(fixed_params=False)
-            dst_ee         = pdf_ee.create_sampler(fixed_params=False)
+            dst_mm         = pdf_mm.create_sampler()
+            dst_ee         = pdf_ee.create_sampler()
 
             if 'TIS' in ds:
                 dst_mm = dst_mm_tos
             else:
                 dst_mm_tos = dst_mm
 
             arr_mm = dst_mm.value().numpy().flatten()
             arr_ee = dst_ee.value().numpy().flatten()
 
-            d_data[ds]     = arr_mm, arr_ee
-
             self._plot_data(f'{ds}_mm', arr_mm)
             self._plot_data(f'{ds}_ee', arr_ee)
 
-            log.debug(f'Electron data: {dst_ee.numpy().shape[0]}')
-            log.debug(f'Muon data: {dst_mm.numpy().shape[0]}')
+            log.debug(f'Muon data: {arr_mm.shape}')
+            log.debug(f'Electron data: {arr_ee.shape}')
+
+            zdat_mm = zfit.Data.from_numpy(self._obs, array=arr_mm)
+            zdat_ee = zfit.Data.from_numpy(self._obs, array=arr_ee)
+
+            d_data[ds] = zdat_mm, zdat_ee
 
         return d_data
     #----------------------------------------------------
     @staticmethod
     def show(d_mod):
         s_dset = { key.split('_')[0] for key in d_mod }
         for dset in s_dset:
```

### Comparing `rk_extractor-0.9.2/src/scales.py` & `rk_extractor-0.9.3/src/scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_cmb_eff.py` & `rk_extractor-0.9.3/tests/test_cmb_eff.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_cs_reader.py` & `rk_extractor-0.9.3/tests/test_cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_effcalc.py` & `rk_extractor-0.9.3/tests/test_effcalc.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_extractor.py` & `rk_extractor-0.9.3/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_mc_reader.py` & `rk_extractor-0.9.3/tests/test_mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_model_analyzer.py` & `rk_extractor-0.9.3/tests/test_model_analyzer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_model_manager.py` & `rk_extractor-0.9.3/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_normalizer.py` & `rk_extractor-0.9.3/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_np_reader.py` & `rk_extractor-0.9.3/tests/test_np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_rkmodel.py` & `rk_extractor-0.9.3/tests/test_rkmodel.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_rkrx_model.py` & `rk_extractor-0.9.3/tests/test_rkrx_model.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_scales.py` & `rk_extractor-0.9.3/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_scl_mkr.py` & `rk_extractor-0.9.3/tests/test_scl_mkr.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.9.2/tests/test_scl_rdr.py` & `rk_extractor-0.9.3/tests/test_scl_rdr.py`

 * *Files identical despite different names*

