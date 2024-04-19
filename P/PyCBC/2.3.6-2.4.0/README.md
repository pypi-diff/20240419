# Comparing `tmp/PyCBC-2.3.6.tar.gz` & `tmp/PyCBC-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCBC-2.3.6.tar", last modified: Thu Feb 22 16:26:35 2024, max compression
+gzip compressed data, was "PyCBC-2.4.0.tar", last modified: Tue Oct 17 13:36:46 2023, max compression
```

## Comparing `PyCBC-2.3.6.tar` & `PyCBC-2.4.0.tar`

### file list

```diff
@@ -1,847 +1,842 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.541947 PyCBC-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-02-22 16:26:30.000000 PyCBC-2.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-22 16:26:30.000000 PyCBC-2.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-02-22 16:26:35.541947 PyCBC-2.3.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.461947 PyCBC-2.3.6/PyCBC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-02-22 16:26:35.000000 PyCBC-2.3.6/PyCBC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-02-22 16:26:35.000000 PyCBC-2.3.6/PyCBC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 16:26:35.000000 PyCBC-2.3.6/PyCBC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-22 16:26:35.000000 PyCBC-2.3.6/PyCBC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 16:26:35.000000 PyCBC-2.3.6/PyCBC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-02-22 16:26:30.000000 PyCBC-2.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.465947 PyCBC-2.3.6/bin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.469947 PyCBC-2.3.6/bin/all_sky_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)    30077 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_add_statmap
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_apply_rerank
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_average_psd
--rwxr-xr-x   0 runner    (1001) docker     (127)     1968 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_bin_templates
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_bin_trigger_rates_dq
--rwxr-xr-x   0 runner    (1001) docker     (127)     5429 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_calculate_psd
--rw-r--r--   0 runner    (1001) docker     (127)    23029 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_findtrigs
--rwxr-xr-x   0 runner    (1001) docker     (127)    14130 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_hdfinjfind
--rwxr-xr-x   0 runner    (1001) docker     (127)     6063 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_mergetrigs
--rwxr-xr-x   0 runner    (1001) docker     (127)    22105 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_statmap
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_statmap_inj
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_combine_coincident_events
--rwxr-xr-x   0 runner    (1001) docker     (127)     8372 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_combine_statmap
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_distribute_background_bins
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_dtphase
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_exclude_zerolag
--rw-r--r--   0 runner    (1001) docker     (127)    19688 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_binned
--rwxr-xr-x   0 runner    (1001) docker     (127)    16639 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_by_template
--rwxr-xr-x   0 runner    (1001) docker     (127)    16723 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_over_multiparam
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_over_param
--rw-r--r--   0 runner    (1001) docker     (127)    23645 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_split_binned
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_followup_file
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_foreground_censor
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_get_loudest_params
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_make_bayestar_skymap
--rwxr-xr-x   0 runner    (1001) docker     (127)     2475 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_merge_psds
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_plot_kde_vals
--rwxr-xr-x   0 runner    (1001) docker     (127)     8687 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_prepare_xml_for_gracedb
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_reduce_template_bank
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_rerank_passthrough
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_findtrigs
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_pastro
--rwxr-xr-x   0 runner    (1001) docker     (127)    17587 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_statmap
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_statmap_inj
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_strip_injections
--rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_template_kde_calc
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_template_kde_max
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_template_recovery_hist
--rwxr-xr-x   0 runner    (1001) docker     (127)     5713 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/all_sky_search/pycbc_upload_single_event_to_gracedb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.469947 PyCBC-2.3.6/bin/bank/
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_aligned_bank_cat
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_aligned_stoch_bank
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_bank_verification
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_brute_bank
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_coinc_bank2hdf
--rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_geom_aligned_2dstack
--rw-r--r--   0 runner    (1001) docker     (127)    23518 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_geom_aligned_bank
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_geom_nonspinbank
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/bank/pycbc_tmpltbank_to_chi_params
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.469947 PyCBC-2.3.6/bin/hwinj/
--rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/hwinj/pycbc_generate_hwinj
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/hwinj/pycbc_generate_hwinj_from_xml
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/hwinj/pycbc_insert_frame_hwinj
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/hwinj/pycbc_plot_hwinj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.473947 PyCBC-2.3.6/bin/inference/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_create_fits
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_extract_samples
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_model_stats
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_monitor
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_acceptance_rate
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_acf
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_acl
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_dynesty_run
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_dynesty_traceplot
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_gelman_rubin
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_geweke
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_inj_recovery
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_mcmc_history
--rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_movie
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_posterior
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_pp
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_prior
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_samples
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_skymap
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_plot_thermodynamic_integrand
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_pp_table_summary
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_start_from_samples
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_inference_table_summary
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/pycbc_validate_test_posterior
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/inference/run_pycbc_inference
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.473947 PyCBC-2.3.6/bin/live/
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/live/pycbc_live_combine_single_fits
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/live/pycbc_live_plot_combined_single_fits
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/live/pycbc_live_plot_single_trigger_fits
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/live/pycbc_live_single_trigger_fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.473947 PyCBC-2.3.6/bin/minifollowups/
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_foreground_minifollowup
--rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_injection_minifollowup
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_page_coincinfo
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_page_injinfo
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_page_snglinfo
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_plot_chigram
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_plot_trigger_timeseries
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_single_template_plot
--rw-r--r--   0 runner    (1001) docker     (127)    14983 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_sngl_minifollowup
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/minifollowups/pycbc_upload_prep_minifollowup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.481947 PyCBC-2.3.6/bin/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_banksim_plot_eff_fitting_factor
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_banksim_plot_fitting_factors
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_banksim_table_point_injs
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_create_html_snippet
--rwxr-xr-x   0 runner    (1001) docker     (127)     5359 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_faithsim_plots
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_ifar_catalog
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_mass_area_plot
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_mchirp_plots
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_banktriggerrate
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_coinc_snrchi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_dq_table
--rwxr-xr-x   0 runner    (1001) docker     (127)     8484 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_foreground
--rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_foundmissed
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_ifar
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_injtable
--rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_recovery
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_segments
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_segplot
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_segtable
--rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_sensitivity
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_snrchi
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_snrifar
--rwxr-xr-x   0 runner    (1001) docker     (127)    10366 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_snrratehist
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_template_bin_table
--rwxr-xr-x   0 runner    (1001) docker     (127)     2226 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_versioning
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_page_vetotable
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_background_coincs
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_bank_bins
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_bank_corner
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_dq_flag_likelihood
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_dq_likelihood_vs_time
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_dq_percentiles
--rwxr-xr-x   0 runner    (1001) docker     (127)     8101 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_gate_triggers
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_gating
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_hist
--rwxr-xr-x   0 runner    (1001) docker     (127)    11670 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_multiifo_dtphase
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_psd_file
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_psd_timefreq
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_qscan
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_range
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_range_vs_mtot
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_singles_timefreq
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_singles_vs_params
--rwxr-xr-x   0 runner    (1001) docker     (127)     2937 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_throughput
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_trigrate
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_vt_ratio
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/plotting/pycbc_plot_waveform
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.481947 PyCBC-2.3.6/bin/population/
--rw-r--r--   0 runner    (1001) docker     (127)    16341 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/population/pycbc_multiifo_pastro
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/population/pycbc_population_plots
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/population/pycbc_population_rates
--rw-r--r--   0 runner    (1001) docker     (127)    19520 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_banksim
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_banksim_combine_banks
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_banksim_match_combine
--rw-r--r--   0 runner    (1001) docker     (127)    22157 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_banksim_skymax
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_coinc_time
--rwxr-xr-x   0 runner    (1001) docker     (127)     9082 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_compress_bank
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_condition_strain
--rwxr-xr-x   0 runner    (1001) docker     (127)     6869 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_convertinjfiletohdf
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_copy_output_map
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_create_injections
--rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_data_store
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_faithsim
--rwxr-xr-x   0 runner    (1001) docker     (127)     2395 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_faithsim_collect_results
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_fit_sngl_trigs
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_get_ffinal
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_gwosc_segment_query
--rwxr-xr-x   0 runner    (1001) docker     (127)     5952 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_hdf5_splitbank
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_hdf_splitinj
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_inj_cut
--rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_inspiral
--rwxr-xr-x   0 runner    (1001) docker     (127)    18972 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_inspiral_skymax
--rwxr-xr-x   0 runner    (1001) docker     (127)    60013 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_live
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_live_nagios_monitor
--rw-r--r--   0 runner    (1001) docker     (127)    17345 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_make_banksim
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_make_faithsim
--rw-r--r--   0 runner    (1001) docker     (127)    11717 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_make_html_page
--rwxr-xr-x   0 runner    (1001) docker     (127)    25365 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_make_skymap
--rwxr-xr-x   0 runner    (1001) docker     (127)     3782 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_merge_inj_hdf
--rwxr-xr-x   0 runner    (1001) docker     (127)    33869 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_multi_inspiral
--rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_optimal_snr
--rwxr-xr-x   0 runner    (1001) docker     (127)    14318 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_optimize_snr
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_process_sngls
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_randomize_inj_dist_by_optsnr
--rwxr-xr-x   0 runner    (1001) docker     (127)    20946 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_single_template
--rwxr-xr-x   0 runner    (1001) docker     (127)     3992 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_source_probability_offline
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_split_inspinj
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_splitbank
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_stageout_failed_workflow
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_submit_dax
--rwxr-xr-x   0 runner    (1001) docker     (127)    11868 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pycbc_upload_xml_to_gracedb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.481947 PyCBC-2.3.6/bin/pygrb/
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_grb_inj_combiner
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_grb_inj_finder
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_grb_trig_cluster
--rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_grb_trig_combiner
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_make_offline_grb_workflow
--rw-r--r--   0 runner    (1001) docker     (127)    27170 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_efficiency
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_grb_info_table
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_minifollowups
--rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_page_tables
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_chisq_veto
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr
--rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_injs_results
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_null_stats
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_skygrid
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_snr_timeseries
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_stats_distribution
--rw-r--r--   0 runner    (1001) docker     (127)    18850 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_pp_workflow
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.449947 PyCBC-2.3.6/bin/workflow_comparisons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.481947 PyCBC-2.3.6/bin/workflow_comparisons/offline_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12151 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons
--rwxr-xr-x   0 runner    (1001) docker     (127)    21916 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison
--rwxr-xr-x   0 runner    (1001) docker     (127)     2768 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/bin/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_bank_verifier_workflow
--rwxr-xr-x   0 runner    (1001) docker     (127)     4599 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_faithsim_workflow
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_inference_inj_workflow
--rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_inference_plots_workflow
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_inference_workflow
--rwxr-xr-x   0 runner    (1001) docker     (127)    37755 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_offline_search_workflow
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_psd_estimation_workflow
--rw-r--r--   0 runner    (1001) docker     (127)    16316 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_sbank_workflow
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-02-22 16:26:30.000000 PyCBC-2.3.6/bin/workflows/pycbc_make_uberbank_workflow
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/banksim/
--rw-r--r--   0 runner    (1001) docker     (127)    21402 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/banksim/injection0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/banksim/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.453947 PyCBC-2.3.6/examples/cal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/catalog/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/catalog/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/catalog/what.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/dataquality/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/dataquality/hwinj.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/dataquality/on.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/detector/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/detector/ant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/detector/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/detector/delay.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/detector/loc.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/detector/travel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/distributions/list_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/distributions/mass_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/distributions/mchirp_q_from_uniform_m1m2_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/distributions/sampling_from_config_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/distributions/spin_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/distributions/spin_spatial_distr_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/faith/
--rw-r--r--   0 runner    (1001) docker     (127)    21402 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/faith/injection0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/faith/pegasus_workflow_create.sh
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/faith/pegasus_workflow_submit.sh
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/faith/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/filter/chisq.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/filter/fir.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/filter/pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/filter/snr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/gw150914/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/gw150914/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/gw150914/gw150914_h1_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/gw150914/gw150914_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.485947 PyCBC-2.3.6/examples/inference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/analytic-normal2d/
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/analytic-normal2d/make_movie.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      292 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/analytic-normal2d/plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/analytic-normal2d/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/bbh-injection/
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/bbh-injection/make_injection.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/bbh-injection/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      967 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/bbh-injection/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/gw150914/
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/gw150914/plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/gw150914/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1149 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/gw150914/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/hierarchical/
--rwxr-xr-x   0 runner    (1001) docker     (127)      269 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/hierarchical/make_injections.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/hierarchical/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      565 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/hierarchical/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/lisa_smbhb_inj/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_inj/injection_smbhb.sh
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_inj/plot.sh
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_inj/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/advanced_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/get.sh
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/plot.sh
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/list_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/margtime/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/margtime/get.sh
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/margtime/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/margtime/run_inj.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/multisignal/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/multisignal/get.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/multisignal/make_injections.sh
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/multisignal/rel.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/multisignal/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/multisignal/single.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/relative/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/relative/get.sh
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/relative/plot.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      139 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/relative/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/relmarg/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/relmarg/get.sh
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/relmarg/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/samplers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/samplers/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inference/single/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/single/get.sh
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/single/plot.sh
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/single/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/single/run_instant.sh
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inference/single/run_marg.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.489947 PyCBC-2.3.6/examples/inspiral/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inspiral/check_GW150914_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inspiral/clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3683 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/inspiral/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/live/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8211 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/live/check_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1508 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/live/generate_injections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/live/make_singles_fits_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6995 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/live/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/make_skymap/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/make_skymap/GW150914.sh
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/make_skymap/GW170817.sh
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/make_skymap/simulated_data.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/multi_inspiral/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/multi_inspiral/check_faceon_faceaway_trigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/multi_inspiral/check_gw170817_trigs.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/multi_inspiral/clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2736 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/multi_inspiral/faceon_faceaway.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2482 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/multi_inspiral/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/noise/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/noise/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/noise/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/overlap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/psd/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/psd/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/psd/estimate.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/psd/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/search/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/bank.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/check_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/gen.sh
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/get.sh
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/master.sh
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/stats.sh
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/search/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/tmpltbank/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.493947 PyCBC-2.3.6/examples/tmpltbank/bank_workflow_test/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/bank_workflow_test/gen.sh
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/cleanOutput.sh
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/make_cache.sh
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testAligned.sh
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testAligned2.sh
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testAligned3.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      649 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testNonspin.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      495 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testNonspin2.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      327 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testNonspin3.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      675 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testStoch.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testStoch2.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testStoch3.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/tmpltbank/testStoch4.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/add_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/higher_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/match_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/plot_detwaveform.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/plot_fd_td.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/plot_freq.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/plot_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/plot_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/waveform/what_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.453947 PyCBC-2.3.6/examples/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/data_checker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6801 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/data_checker/daily_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/data_checker/get_data_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/data_checker/run_daily_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/data_checker/run_get_data_example.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/dayhopecheck/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7198 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/dayhopecheck/dayhopecheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/dayhopecheck/run_dayhopecheck.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.453947 PyCBC-2.3.6/examples/workflow/generic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/generic/multilevel_subworkflow_data/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/generic/multilevel_subworkflow_data/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/generic/multilevel_subworkflow_data/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/generic/simple_subworkflow_data/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/generic/simple_subworkflow_data/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/generic/simple_subworkflow_data/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.453947 PyCBC-2.3.6/examples/workflow/inference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/inference/bbh_inj-dynesty/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/inference/gw150914_gw170814-dynesty/
--rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/inference/gw150914_gw170814-dynesty/create_workflow.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/inference/gw150914_gw170814-emcee_pt/
--rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/inference/gw150914_gw170814-emcee_pt/create_workflow.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/inference/small_test/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/inference/small_test/gen.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.453947 PyCBC-2.3.6/examples/workflow/pygrb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/pygrb/ER7/
--rwxr-xr-x   0 runner    (1001) docker     (127)      739 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/pygrb/ER8/
--rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      822 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.497947 PyCBC-2.3.6/examples/workflow/pygrb/S6/
--rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-02-22 16:26:30.000000 PyCBC-2.3.6/examples/workflow/pygrb/S6/run_s6_pygrb.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.501947 PyCBC-2.3.6/pycbc/
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/_version_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21555 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/boundaries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.501947 PyCBC-2.3.6/pycbc/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    62478 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    23038 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)    30530 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.501947 PyCBC-2.3.6/pycbc/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/angular.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/bounded.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/fixedsamples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/power_law.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/qnm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/sky_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/spins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/uniform_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/distributions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/dq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.505947 PyCBC-2.3.6/pycbc/events/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/coherent.py
--rw-r--r--   0 runner    (1001) docker     (127)    53115 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/coinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/coinc_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/cuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    50001 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/eventmgr_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    17954 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/significance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/simd_threshold_ccode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/simd_threshold_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/single.py
--rw-r--r--   0 runner    (1001) docker     (127)    90026 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/threshold_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/threshold_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/trigger_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/events/veto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.505947 PyCBC-2.3.6/pycbc/fft/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/backend_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/backend_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/backend_mkl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/backend_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/class_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/cuda_pyfft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/cufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/fft_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    22788 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/fftw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/fftw_pruned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/fftw_pruned_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/func_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/mkl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/npfft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/fft/parser_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.505947 PyCBC-2.3.6/pycbc/filter/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/fotonfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    83046 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/matchedfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/matchedfilter_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/matchedfilter_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/matchedfilter_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/qtransform.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/simd_correlate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/simd_correlate_ccode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/simd_correlate_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/filter/zpk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.509947 PyCBC-2.3.6/pycbc/frame/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35954 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/frame/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/frame/gwosc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/frame/store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.509947 PyCBC-2.3.6/pycbc/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30844 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/burn_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/evidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/gelman_rubin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/geweke.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.509947 PyCBC-2.3.6/pycbc/inference/io/
--rw-r--r--   0 runner    (1001) docker     (127)    32158 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/base_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36040 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/base_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/base_multitemper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/base_nested_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/cpnest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/dynesty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/emcee.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/emcee_pt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/epsie.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/multinest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/posterior.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/ptemcee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/io/ultranest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.509947 PyCBC-2.3.6/pycbc/inference/jump/
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/jump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/jump/angular.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/jump/bounded_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/jump/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/jump/normal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.513947 PyCBC-2.3.6/pycbc/inference/models/
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)    33142 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/base_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/brute_marg.py
--rw-r--r--   0 runner    (1001) docker     (127)    23677 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30889 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/gated_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    49252 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    25771 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    32995 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/marginalized_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    32610 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/relbin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20731 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/relbin_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/single_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/option_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.513947 PyCBC-2.3.6/pycbc/inference/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/base_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    36376 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/base_mcmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16327 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/base_multitemper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/cpnest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23999 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/dynesty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/emcee.py
--rw-r--r--   0 runner    (1001) docker     (127)    18909 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/emcee_pt.py
--rw-r--r--   0 runner    (1001) docker     (127)    19831 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/epsie.py
--rw-r--r--   0 runner    (1001) docker     (127)    15427 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/multinest.py
--rw-r--r--   0 runner    (1001) docker     (127)    27259 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/ptemcee.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inference/sampler/ultranest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.513947 PyCBC-2.3.6/pycbc/inject/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48285 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inject/inject.py
--rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/inject/injfilterrejector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.513947 PyCBC-2.3.6/pycbc/io/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55616 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/io/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/io/ligolw.py
--rw-r--r--   0 runner    (1001) docker     (127)    24406 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/io/live.py
--rw-r--r--   0 runner    (1001) docker     (127)    77875 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/io/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/libutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.513947 PyCBC-2.3.6/pycbc/live/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/live/snr_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/mchirp_area.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.517947 PyCBC-2.3.6/pycbc/neutron_stars/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/neutron_stars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/neutron_stars/eos_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.517947 PyCBC-2.3.6/pycbc/neutron_stars/ns_data/
--rw-r--r--   0 runner    (1001) docker     (127)    53263 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/neutron_stars/ns_data/equil_2H.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/neutron_stars/pg_isso_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.517947 PyCBC-2.3.6/pycbc/noise/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/noise/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/noise/reproduceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    41015 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/pnutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.517947 PyCBC-2.3.6/pycbc/population/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30477 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/fgmc_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/fgmc_laguerre.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/fgmc_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/live_pastro.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/live_pastro_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16559 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/population_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13826 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/rates_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/population/scale_injections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.517947 PyCBC-2.3.6/pycbc/psd/
--rw-r--r--   0 runner    (1001) docker     (127)    28796 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/psd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/psd/analytical.py
--rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/psd/analytical_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/psd/estimate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/psd/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/psd/variation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/rate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.517947 PyCBC-2.3.6/pycbc/results/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/dq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/followup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/mpld3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/psd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/pygrb_plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33850 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/pygrb_postprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/render.py
--rw-r--r--   0 runner    (1001) docker     (127)    33143 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/scatter_histograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/snr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/pycbc/results/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/pycbc/results/static/css/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/css/bootstrap/3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)   117150 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   117150 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/pycbc/results/static/css/fancybox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/css/fancybox/2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/css/pycbc/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/css/pycbc/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/css/pycbc/red.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.css
--rw-r--r--   0 runner    (1001) docker     (127)   258264 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.eot
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.html
--rw-r--r--   0 runner    (1001) docker     (127)   658924 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   312760 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.woff
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.css
--rw-r--r--   0 runner    (1001) docker     (127)   270560 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.eot
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.html
--rw-r--r--   0 runner    (1001) docker     (127)   702616 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   326132 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/pycbc/results/static/js/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.521947 PyCBC-2.3.6/pycbc/results/static/js/bootstrap/3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    35452 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/pycbc/results/static/js/fancybox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    48706 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    23135 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/pycbc/results/static/js/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/results/static/js/jquery/1.10.2/
--rw-r--r--   0 runner    (1001) docker     (127)    93107 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/results/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/results/templates/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/files/file_default.html
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/files/file_glitchgram.html
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/files/file_img.html
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/files/file_pre.html
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/files/file_tmplt.html
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/orange.html
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/red.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/results/templates/wells/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/wells/sitemap.html
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/templates/wells/two_column.html
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/results/versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/strain/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/strain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/strain/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/strain/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/strain/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/strain/recalibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    93321 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/strain/strain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/tmpltbank/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/bank_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/bank_output_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23515 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/brute_force_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    23569 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/calc_moments.py
--rw-r--r--   0 runner    (1001) docker     (127)    33431 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/coord_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/lambda_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/lattice_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    57353 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/option_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28141 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/tmpltbank/partitioned_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)    84293 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.525947 PyCBC-2.3.6/pycbc/types/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/aligned.py
--rw-r--r--   0 runner    (1001) docker     (127)    39845 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/array_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/array_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    28875 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25727 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/frequencyseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/optparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    46916 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/types/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-22 16:26:33.000000 PyCBC-2.3.6/pycbc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.529947 PyCBC-2.3.6/pycbc/vetoes/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/autochisq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/bank_chisq.py
--rw-r--r--   0 runner    (1001) docker     (127)    19668 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/chisq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/chisq_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/chisq_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/vetoes/sgchisq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.529947 PyCBC-2.3.6/pycbc/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/SpinTaylorF2.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39507 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/bank.py
--rw-r--r--   0 runner    (1001) docker     (127)    30086 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/decompress_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/decompress_cpu_ccode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/decompress_cpu_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/decompress_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    51496 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/multiband.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/nltides.py
--rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/premerger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/pycbc_phenomC_tmplt.py
--rw-r--r--   0 runner    (1001) docker     (127)    54746 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/ringdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/sinegauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/spa_tmplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/spa_tmplt_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/spa_tmplt_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/supernovae.py
--rw-r--r--   0 runner    (1001) docker     (127)    19760 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/utils_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/utils_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    57725 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/waveform/waveform_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.533947 PyCBC-2.3.6/pycbc/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32083 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/coincidence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/configparser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    91247 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    48940 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/datafind.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/dq.py
--rw-r--r--   0 runner    (1001) docker     (127)    33027 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/grb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42899 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/inference_followups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    50769 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/jobsetup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/matched_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    51180 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/minifollowups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.533947 PyCBC-2.3.6/pycbc/workflow/pegasus_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/pegasus_files/pegasus-properties.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/pegasus_sites.py
--rw-r--r--   0 runner    (1001) docker     (127)    32719 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/pegasus_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    22889 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/psd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/psdfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19687 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/splittable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14333 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/tmpltbank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pycbc/workflow/versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 16:26:30.000000 PyCBC-2.3.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 16:26:35.541947 PyCBC-2.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10711 2024-02-22 16:26:30.000000 PyCBC-2.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/bankvetotest.py
--rw-r--r--   0 runner    (1001) docker     (127)    37722 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/fft_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16620 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/lalsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_array_lal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_autochisq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_chisq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_coinc_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_correlate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_cuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_fft_mkl_threaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_fft_unthreaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_fftw_openmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_fftw_pthreads.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_frequencyseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_infmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_io_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_live_coinc_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_matchedfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_pnutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_psd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_schemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_significance_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_skymax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_spatmplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)    26161 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    27104 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_tmpltbank.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/test_waveform_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38174 2024-02-22 16:26:30.000000 PyCBC-2.3.6/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.457947 PyCBC-2.3.6/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/tools/benchmarking/
--rwxr-xr-x   0 runner    (1001) docker     (127)      822 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/benchmarking/absolute_times.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/tools/einsteinathome/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/einsteinathome/check_GW150914_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/tools/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/tools/static/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/static/hooks/hook-pycbc.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/static/runtime-scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/static/runtime-tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/tools/timing/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2286 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/timing/arr_perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:26:35.537947 PyCBC-2.3.6/tools/timing/banksim/
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/timing/banksim/banksim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/timing/correlate_perf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2935 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/timing/fft_perf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3154 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/timing/match_perf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2472 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tools/timing/wav_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-22 16:26:30.000000 PyCBC-2.3.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2023-10-17 13:36:38.000000 PyCBC-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-17 13:36:38.000000 PyCBC-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2023-10-17 13:36:46.014504 PyCBC-2.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.938502 PyCBC-2.4.0/PyCBC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2023-10-17 13:36:45.000000 PyCBC-2.4.0/PyCBC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24280 2023-10-17 13:36:45.000000 PyCBC-2.4.0/PyCBC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 13:36:45.000000 PyCBC-2.4.0/PyCBC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2023-10-17 13:36:45.000000 PyCBC-2.4.0/PyCBC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-17 13:36:45.000000 PyCBC-2.4.0/PyCBC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-10-17 13:36:38.000000 PyCBC-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.942502 PyCBC-2.4.0/bin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.946502 PyCBC-2.4.0/bin/all_sky_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29582 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_add_statmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_apply_rerank
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_average_psd
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_bin_trigger_rates_dq
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_calculate_dq
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_calculate_dqflag
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5444 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_calculate_psd
+-rw-r--r--   0 runner    (1001) docker     (127)    23095 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_findtrigs
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14222 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_hdfinjfind
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6098 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_mergetrigs
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21685 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_statmap
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_statmap_inj
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_combine_coincident_events
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_combine_statmap
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_distribute_background_bins
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_dtphase
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_exclude_zerolag
+-rw-r--r--   0 runner    (1001) docker     (127)    19787 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_binned
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16852 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_by_template
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16797 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_over_multiparam
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_over_param
+-rw-r--r--   0 runner    (1001) docker     (127)    21126 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_split_binned
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_followup_file
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_foreground_censor
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_get_loudest_params
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2490 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_merge_psds
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_plot_kde_vals
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_reduce_template_bank
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_rerank_dq
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_rerank_passthrough
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_findtrigs
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_pastro
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17203 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_statmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_statmap_inj
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_strip_injections
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_template_kde_calc
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_template_kde_max
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/all_sky_search/pycbc_template_recovery_hist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.946502 PyCBC-2.4.0/bin/bank/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_aligned_bank_cat
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_aligned_stoch_bank
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_bank_verification
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_brute_bank
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_coinc_bank2hdf
+-rw-r--r--   0 runner    (1001) docker     (127)    17389 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_geom_aligned_2dstack
+-rw-r--r--   0 runner    (1001) docker     (127)    23518 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_geom_aligned_bank
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_geom_nonspinbank
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/bank/pycbc_tmpltbank_to_chi_params
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.946502 PyCBC-2.4.0/bin/hwinj/
+-rw-r--r--   0 runner    (1001) docker     (127)    22443 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/hwinj/pycbc_generate_hwinj
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/hwinj/pycbc_generate_hwinj_from_xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/hwinj/pycbc_insert_frame_hwinj
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/hwinj/pycbc_plot_hwinj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.950502 PyCBC-2.4.0/bin/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_create_fits
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_extract_samples
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_model_stats
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_monitor
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_acceptance_rate
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_acf
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_acl
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_dynesty_run
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_dynesty_traceplot
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_gelman_rubin
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_geweke
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_inj_recovery
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_mcmc_history
+-rw-r--r--   0 runner    (1001) docker     (127)    15034 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_movie
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_posterior
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_pp
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_prior
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_samples
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_skymap
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_plot_thermodynamic_integrand
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_pp_table_summary
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_start_from_samples
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_inference_table_summary
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/pycbc_validate_test_posterior
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/inference/run_pycbc_inference
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.950502 PyCBC-2.4.0/bin/live/
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/live/pycbc_live_combine_single_fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/live/pycbc_live_plot_combined_single_fits
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/live/pycbc_live_plot_single_trigger_fits
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/live/pycbc_live_single_trigger_fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.950502 PyCBC-2.4.0/bin/minifollowups/
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_foreground_minifollowup
+-rw-r--r--   0 runner    (1001) docker     (127)    16334 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_injection_minifollowup
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_page_coincinfo
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_page_injinfo
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_page_snglinfo
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_plot_chigram
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_plot_trigger_timeseries
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_single_template_plot
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/minifollowups/pycbc_sngl_minifollowup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.958502 PyCBC-2.4.0/bin/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_banksim_plot_eff_fitting_factor
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_banksim_plot_fitting_factors
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_banksim_table_point_injs
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_create_html_snippet
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5359 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_faithsim_plots
+-rw-r--r--   0 runner    (1001) docker     (127)    10855 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_ifar_catalog
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_mass_area_plot
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_mchirp_plots
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_banktriggerrate
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_coinc_snrchi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8484 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_foreground
+-rw-r--r--   0 runner    (1001) docker     (127)    11408 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_foundmissed
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_ifar
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_injtable
+-rw-r--r--   0 runner    (1001) docker     (127)     9894 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_recovery
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_segments
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_segplot
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_segtable
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_sensitivity
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_snrchi
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_snrifar
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10366 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_snrratehist
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2226 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_versioning
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_page_vetotable
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_background_coincs
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_bank_bins
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_bank_corner
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_dq_flag_likelihood
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_dq_likelihood_vs_time
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_dq_percentiles
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8101 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_gate_triggers
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_gating
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_hist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11670 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_multiifo_dtphase
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_psd_file
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_psd_timefreq
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_qscan
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_range
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_range_vs_mtot
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_singles_timefreq
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_singles_vs_params
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2937 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_throughput
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_trigrate
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_vt_ratio
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/plotting/pycbc_plot_waveform
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.958502 PyCBC-2.4.0/bin/population/
+-rw-r--r--   0 runner    (1001) docker     (127)    16341 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/population/pycbc_multiifo_pastro
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/population/pycbc_population_plots
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/population/pycbc_population_rates
+-rw-r--r--   0 runner    (1001) docker     (127)    19520 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_banksim
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_banksim_combine_banks
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_banksim_match_combine
+-rw-r--r--   0 runner    (1001) docker     (127)    22157 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_banksim_skymax
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_coinc_time
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9082 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_compress_bank
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_condition_strain
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6670 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_convertinjfiletohdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_copy_output_map
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_create_injections
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_data_store
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_faithsim
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2395 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_faithsim_collect_results
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_fit_sngl_trigs
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_get_ffinal
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_gwosc_segment_query
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5952 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_hdf5_splitbank
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_hdf_splitinj
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_inj_cut
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_inspiral
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18972 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_inspiral_skymax
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60013 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_live
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_live_nagios_monitor
+-rw-r--r--   0 runner    (1001) docker     (127)    17345 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_make_banksim
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_make_faithsim
+-rw-r--r--   0 runner    (1001) docker     (127)    11717 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_make_html_page
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25365 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_make_skymap
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3782 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_merge_inj_hdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33869 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_multi_inspiral
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_optimal_snr
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14318 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_optimize_snr
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_process_sngls
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_randomize_inj_dist_by_optsnr
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20946 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_single_template
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3992 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_source_probability_offline
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_split_inspinj
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_splitbank
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_stageout_failed_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_submit_dax
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11868 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pycbc_upload_xml_to_gracedb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.958502 PyCBC-2.4.0/bin/pygrb/
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_grb_inj_combiner
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_grb_inj_finder
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_grb_trig_cluster
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_grb_trig_combiner
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_make_offline_grb_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)    27170 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_efficiency
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_grb_info_table
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_minifollowups
+-rw-r--r--   0 runner    (1001) docker     (127)    38056 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_page_tables
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_chisq_veto
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr
+-rw-r--r--   0 runner    (1001) docker     (127)    20941 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_injs_results
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_null_stats
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_skygrid
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_snr_timeseries
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_stats_distribution
+-rw-r--r--   0 runner    (1001) docker     (127)    18850 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_pp_workflow
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.930502 PyCBC-2.4.0/bin/workflow_comparisons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.958502 PyCBC-2.4.0/bin/workflow_comparisons/offline_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12151 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21916 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2768 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.958502 PyCBC-2.4.0/bin/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    16323 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_bank_verifier_workflow
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4599 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_faithsim_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_inference_inj_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)    10783 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_inference_plots_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_inference_workflow
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37959 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_offline_search_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_psd_estimation_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)    16316 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_sbank_workflow
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2023-10-17 13:36:38.000000 PyCBC-2.4.0/bin/workflows/pycbc_make_uberbank_workflow
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/banksim/
+-rw-r--r--   0 runner    (1001) docker     (127)    21402 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/banksim/injection0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/banksim/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.930502 PyCBC-2.4.0/examples/cal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/catalog/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/catalog/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/catalog/what.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/dataquality/hwinj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/dataquality/on.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/detector/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/detector/ant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/detector/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/detector/delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/detector/loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/detector/travel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/distributions/list_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/distributions/mass_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/distributions/mchirp_q_from_uniform_m1m2_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/distributions/sampling_from_config_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/distributions/spin_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/distributions/spin_spatial_distr_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/faith/
+-rw-r--r--   0 runner    (1001) docker     (127)    21402 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/faith/injection0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/faith/pegasus_workflow_create.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/faith/pegasus_workflow_submit.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/faith/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/filter/chisq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/filter/fir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/filter/pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/filter/snr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/gw150914/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/gw150914/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/gw150914/gw150914_h1_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/gw150914/gw150914_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/inference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/inference/analytic-normal2d/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/analytic-normal2d/make_movie.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      292 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/analytic-normal2d/plot.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/analytic-normal2d/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.962503 PyCBC-2.4.0/examples/inference/bbh-injection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/bbh-injection/make_injection.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/bbh-injection/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      967 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/bbh-injection/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/gw150914/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/gw150914/plot.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      656 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/gw150914/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1149 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/gw150914/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/hierarchical/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      269 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/hierarchical/make_injections.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      230 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/hierarchical/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      565 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/hierarchical/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/lisa_smbhb_inj/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_inj/injection_smbhb.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_inj/plot.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_inj/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/advanced_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/get.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/plot.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/list_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/margtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/margtime/get.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/margtime/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/margtime/run_inj.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/multisignal/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/multisignal/get.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/multisignal/make_injections.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/multisignal/rel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/multisignal/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/multisignal/single.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/relative/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/relative/get.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/relative/plot.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      139 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/relative/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/relmarg/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/relmarg/get.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/relmarg/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/samplers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/samplers/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inference/single/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/single/get.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/single/plot.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/single/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/single/run_instant.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inference/single/run_marg.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/inspiral/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inspiral/check_GW150914_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inspiral/clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3683 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/inspiral/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/live/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8211 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/live/check_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1508 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/live/generate_injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/live/make_singles_fits_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6995 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/live/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.966503 PyCBC-2.4.0/examples/make_skymap/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/make_skymap/GW150914.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/make_skymap/GW170817.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/make_skymap/simulated_data.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/multi_inspiral/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/multi_inspiral/check_faceon_faceaway_trigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/multi_inspiral/check_gw170817_trigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/multi_inspiral/clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2736 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/multi_inspiral/faceon_faceaway.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2482 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/multi_inspiral/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/noise/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/noise/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/overlap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/psd/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/psd/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2023-10-17 13:36:38.000000 PyCBC-2.4.0/examples/psd/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/psd/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/bank.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/check_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/gen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/get.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/master.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/stats.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/search/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/tmpltbank/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/tmpltbank/bank_workflow_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/bank_workflow_test/gen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/cleanOutput.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/make_cache.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testAligned.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testAligned2.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testAligned3.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      649 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testNonspin.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      495 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testNonspin2.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      327 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testNonspin3.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      675 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testStoch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      449 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testStoch2.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testStoch3.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      531 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/tmpltbank/testStoch4.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/add_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/higher_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/match_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/plot_detwaveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/plot_fd_td.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/plot_freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/plot_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/plot_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/waveform/what_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/examples/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/workflow/data_checker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6801 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/data_checker/daily_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/data_checker/get_data_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/data_checker/run_daily_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/data_checker/run_get_data_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.970503 PyCBC-2.4.0/examples/workflow/dayhopecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7198 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/dayhopecheck/dayhopecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/dayhopecheck/run_dayhopecheck.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/examples/workflow/generic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/generic/multilevel_subworkflow_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/generic/multilevel_subworkflow_data/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/generic/multilevel_subworkflow_data/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/generic/simple_subworkflow_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/generic/simple_subworkflow_data/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/generic/simple_subworkflow_data/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/examples/workflow/inference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/inference/bbh_inj-dynesty/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/inference/gw150914_gw170814-dynesty/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/inference/gw150914_gw170814-dynesty/create_workflow.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/inference/gw150914_gw170814-emcee_pt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/inference/gw150914_gw170814-emcee_pt/create_workflow.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/inference/small_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/inference/small_test/gen.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/examples/workflow/pygrb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/pygrb/ER7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      739 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/pygrb/ER8/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      825 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      822 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/examples/workflow/pygrb/S6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      866 2023-10-17 13:36:39.000000 PyCBC-2.4.0/examples/workflow/pygrb/S6/run_s6_pygrb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/pycbc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/_version_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21555 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/boundaries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.974503 PyCBC-2.4.0/pycbc/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62478 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23038 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30530 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.978503 PyCBC-2.4.0/pycbc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19645 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/angular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/bounded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/fixedsamples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/power_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/qnm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/sky_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/spins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/uniform_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/distributions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/dq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.978503 PyCBC-2.4.0/pycbc/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/coherent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53385 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/coinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/coinc_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49963 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/eventmgr_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17905 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/significance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/simd_threshold_ccode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/simd_threshold_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88310 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/threshold_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/threshold_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/trigger_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/events/veto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.982503 PyCBC-2.4.0/pycbc/fft/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/backend_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/backend_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/backend_mkl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/backend_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/class_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/cuda_pyfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/cufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/fft_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22788 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/fftw_pruned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/fftw_pruned_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/func_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/mkl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/npfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/fft/parser_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.982503 PyCBC-2.4.0/pycbc/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/fotonfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83046 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/matchedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/matchedfilter_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/matchedfilter_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/matchedfilter_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/qtransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/simd_correlate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/simd_correlate_ccode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/simd_correlate_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/filter/zpk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.982503 PyCBC-2.4.0/pycbc/frame/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33651 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/frame/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/frame/gwosc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/frame/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.982503 PyCBC-2.4.0/pycbc/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30844 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/burn_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/gelman_rubin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/geweke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.986503 PyCBC-2.4.0/pycbc/inference/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    32158 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38576 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/base_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36040 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/base_mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16944 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/base_multitemper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/base_nested_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/cpnest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/dynesty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/emcee_pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/epsie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/ptemcee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/io/ultranest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.986503 PyCBC-2.4.0/pycbc/inference/jump/
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/jump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/jump/angular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/jump/bounded_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/jump/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20231 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/jump/normal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.986503 PyCBC-2.4.0/pycbc/inference/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33142 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/base_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/brute_marg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23677 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30889 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/gated_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49252 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25771 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32995 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/marginalized_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32610 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/relbin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20731 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/relbin_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/single_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36070 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/option_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.986503 PyCBC-2.4.0/pycbc/inference/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/base_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36376 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/base_mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16327 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/base_multitemper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/cpnest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23999 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/dynesty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18909 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/emcee_pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19831 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/epsie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15427 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27259 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/ptemcee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inference/sampler/ultranest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/inject/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48285 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inject/inject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19409 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/inject/injfilterrejector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55333 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/io/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/io/ligolw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24753 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/io/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77875 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/io/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/libutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/live/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/live/snr_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/mchirp_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/neutron_stars/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/neutron_stars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/neutron_stars/eos_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/neutron_stars/ns_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    53263 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/neutron_stars/ns_data/equil_2H.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/neutron_stars/pg_isso_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/noise/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/noise/reproduceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41008 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/pnutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/population/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30477 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/fgmc_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/fgmc_laguerre.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/fgmc_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/live_pastro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/live_pastro_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16559 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/population_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13826 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/rates_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16956 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/population/scale_injections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.990503 PyCBC-2.4.0/pycbc/psd/
+-rw-r--r--   0 runner    (1001) docker     (127)    28796 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/psd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/psd/analytical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26286 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/psd/analytical_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/psd/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/psd/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/psd/variation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.994503 PyCBC-2.4.0/pycbc/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/dq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/followup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/mpld3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/psd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9071 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/pygrb_plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33850 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/pygrb_postprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33143 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/scatter_histograms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/pycbc/results/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.994503 PyCBC-2.4.0/pycbc/results/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/pycbc/results/static/css/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.994503 PyCBC-2.4.0/pycbc/results/static/css/bootstrap/3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)   117150 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   117150 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/pycbc/results/static/css/fancybox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.994503 PyCBC-2.4.0/pycbc/results/static/css/fancybox/2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.994503 PyCBC-2.4.0/pycbc/results/static/css/pycbc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/css/pycbc/orange.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/css/pycbc/red.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.css
+-rw-r--r--   0 runner    (1001) docker     (127)   258264 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.eot
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.html
+-rw-r--r--   0 runner    (1001) docker     (127)   658924 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   312760 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.css
+-rw-r--r--   0 runner    (1001) docker     (127)   270560 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.eot
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.html
+-rw-r--r--   0 runner    (1001) docker     (127)   702616 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   326132 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/pycbc/results/static/js/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/static/js/bootstrap/3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35452 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35452 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/pycbc/results/static/js/fancybox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48706 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23135 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/pycbc/results/static/js/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/static/js/jquery/1.10.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    93107 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/templates/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/files/file_default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/files/file_glitchgram.html
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/files/file_img.html
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/files/file_pre.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/files/file_tmplt.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/orange.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/red.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/results/templates/wells/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/wells/sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/templates/wells/two_column.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/results/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11609 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.998503 PyCBC-2.4.0/pycbc/strain/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/strain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/strain/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/strain/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/strain/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/strain/recalibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93225 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/strain/strain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.002503 PyCBC-2.4.0/pycbc/tmpltbank/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/bank_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/bank_output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23515 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/brute_force_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23569 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/calc_moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33431 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/coord_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10726 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/lambda_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/lattice_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57353 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/option_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28141 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/tmpltbank/partitioned_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84293 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.002503 PyCBC-2.4.0/pycbc/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/aligned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39845 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/array_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/array_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28875 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25727 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/frequencyseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21934 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/optparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46916 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/types/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2023-10-17 13:36:43.000000 PyCBC-2.4.0/pycbc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.002503 PyCBC-2.4.0/pycbc/vetoes/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/autochisq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/bank_chisq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19668 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/chisq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/chisq_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/chisq_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/vetoes/sgchisq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.006503 PyCBC-2.4.0/pycbc/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/SpinTaylorF2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39507 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30086 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/decompress_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/decompress_cpu_ccode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/decompress_cpu_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/decompress_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51496 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/multiband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/nltides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29135 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/premerger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/pycbc_phenomC_tmplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54746 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/ringdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/sinegauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/spa_tmplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/spa_tmplt_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/spa_tmplt_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/supernovae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19760 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/utils_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/utils_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57683 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/waveform/waveform_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.006503 PyCBC-2.4.0/pycbc/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32083 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/coincidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/configparser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17023 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91247 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48940 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/datafind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/dq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33027 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/grb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42899 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/inference_followups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50769 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/jobsetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/matched_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36762 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/minifollowups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.010503 PyCBC-2.4.0/pycbc/workflow/pegasus_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/pegasus_files/pegasus-properties.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11815 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/pegasus_sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32719 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/pegasus_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24469 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/psd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/psdfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19687 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/splittable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14333 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/tmpltbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pycbc/workflow/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-17 13:36:39.000000 PyCBC-2.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 13:36:46.014504 PyCBC-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10711 2023-10-17 13:36:39.000000 PyCBC-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.010503 PyCBC-2.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/bankvetotest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37722 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/fft_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16620 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/lalsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21211 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_array_lal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_autochisq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_chisq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_coinc_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_correlate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_fft_mkl_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_fft_unthreaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_fftw_openmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_fftw_pthreads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24440 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_frequencyseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_infmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_io_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_live_coinc_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_matchedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_pnutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_psd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_significance_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19047 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_skymax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_spatmplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26161 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27104 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_tmpltbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/test_waveform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38174 2023-10-17 13:36:39.000000 PyCBC-2.4.0/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:45.934502 PyCBC-2.4.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/tools/benchmarking/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      822 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/benchmarking/absolute_times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/tools/einsteinathome/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/einsteinathome/check_GW150914_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/tools/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/tools/static/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/static/hooks/hook-pycbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/static/runtime-scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/static/runtime-tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/tools/timing/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2286 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/timing/arr_perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:36:46.014504 PyCBC-2.4.0/tools/timing/banksim/
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/timing/banksim/banksim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/timing/correlate_perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2935 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/timing/fft_perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3154 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/timing/match_perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2472 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tools/timing/wav_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-10-17 13:36:39.000000 PyCBC-2.4.0/tox.ini
```

### Comparing `PyCBC-2.3.6/LICENSE` & `PyCBC-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/PKG-INFO` & `PyCBC-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyCBC
-Version: 2.3.6
+Version: 2.4.0
 Summary: Core library to analyze gravitational-wave data, find signals, and study their parameters.
 Home-page: http://www.pycbc.org/
 Author: The PyCBC team
 Author-email: alex.nitz@gmail.org
 License: UNKNOWN
-Download-URL: https://github.com/gwastro/pycbc/tarball/v2.3.6
+Download-URL: https://github.com/gwastro/pycbc/tarball/v2.4.0
 Description: ![GW150914](https://raw.githubusercontent.com/gwastro/pycbc-logo/master/pycbc_logo_name.png)
         
         [PyCBC](http://pycbc.org) is a software package used to explore astrophysical sources of gravitational waves.
         It contains algorithms to analyze gravitational-wave data,
         detect coalescing compact binaries, and make bayesian inferences from gravitational-wave data.
         PyCBC was used in the [first direct detection of gravitational waves](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.116.061102) and
         is used in flagship analyses of LIGO and Virgo data.
```

### Comparing `PyCBC-2.3.6/PyCBC.egg-info/PKG-INFO` & `PyCBC-2.4.0/PyCBC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyCBC
-Version: 2.3.6
+Version: 2.4.0
 Summary: Core library to analyze gravitational-wave data, find signals, and study their parameters.
 Home-page: http://www.pycbc.org/
 Author: The PyCBC team
 Author-email: alex.nitz@gmail.org
 License: UNKNOWN
-Download-URL: https://github.com/gwastro/pycbc/tarball/v2.3.6
+Download-URL: https://github.com/gwastro/pycbc/tarball/v2.4.0
 Description: ![GW150914](https://raw.githubusercontent.com/gwastro/pycbc-logo/master/pycbc_logo_name.png)
         
         [PyCBC](http://pycbc.org) is a software package used to explore astrophysical sources of gravitational waves.
         It contains algorithms to analyze gravitational-wave data,
         detect coalescing compact binaries, and make bayesian inferences from gravitational-wave data.
         PyCBC was used in the [first direct detection of gravitational waves](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.116.061102) and
         is used in flagship analyses of LIGO and Virgo data.
```

### Comparing `PyCBC-2.3.6/PyCBC.egg-info/SOURCES.txt` & `PyCBC-2.4.0/PyCBC.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,17 @@
 bin/pycbc_splitbank
 bin/pycbc_stageout_failed_workflow
 bin/pycbc_submit_dax
 bin/pycbc_upload_xml_to_gracedb
 bin/all_sky_search/pycbc_add_statmap
 bin/all_sky_search/pycbc_apply_rerank
 bin/all_sky_search/pycbc_average_psd
-bin/all_sky_search/pycbc_bin_templates
 bin/all_sky_search/pycbc_bin_trigger_rates_dq
+bin/all_sky_search/pycbc_calculate_dq
+bin/all_sky_search/pycbc_calculate_dqflag
 bin/all_sky_search/pycbc_calculate_psd
 bin/all_sky_search/pycbc_coinc_findtrigs
 bin/all_sky_search/pycbc_coinc_hdfinjfind
 bin/all_sky_search/pycbc_coinc_mergetrigs
 bin/all_sky_search/pycbc_coinc_statmap
 bin/all_sky_search/pycbc_coinc_statmap_inj
 bin/all_sky_search/pycbc_combine_coincident_events
@@ -71,29 +72,27 @@
 bin/all_sky_search/pycbc_fit_sngls_by_template
 bin/all_sky_search/pycbc_fit_sngls_over_multiparam
 bin/all_sky_search/pycbc_fit_sngls_over_param
 bin/all_sky_search/pycbc_fit_sngls_split_binned
 bin/all_sky_search/pycbc_followup_file
 bin/all_sky_search/pycbc_foreground_censor
 bin/all_sky_search/pycbc_get_loudest_params
-bin/all_sky_search/pycbc_make_bayestar_skymap
 bin/all_sky_search/pycbc_merge_psds
 bin/all_sky_search/pycbc_plot_kde_vals
-bin/all_sky_search/pycbc_prepare_xml_for_gracedb
 bin/all_sky_search/pycbc_reduce_template_bank
+bin/all_sky_search/pycbc_rerank_dq
 bin/all_sky_search/pycbc_rerank_passthrough
 bin/all_sky_search/pycbc_sngls_findtrigs
 bin/all_sky_search/pycbc_sngls_pastro
 bin/all_sky_search/pycbc_sngls_statmap
 bin/all_sky_search/pycbc_sngls_statmap_inj
 bin/all_sky_search/pycbc_strip_injections
 bin/all_sky_search/pycbc_template_kde_calc
 bin/all_sky_search/pycbc_template_kde_max
 bin/all_sky_search/pycbc_template_recovery_hist
-bin/all_sky_search/pycbc_upload_single_event_to_gracedb
 bin/bank/pycbc_aligned_bank_cat
 bin/bank/pycbc_aligned_stoch_bank
 bin/bank/pycbc_bank_verification
 bin/bank/pycbc_brute_bank
 bin/bank/pycbc_coinc_bank2hdf
 bin/bank/pycbc_geom_aligned_2dstack
 bin/bank/pycbc_geom_aligned_bank
@@ -138,39 +137,36 @@
 bin/minifollowups/pycbc_page_coincinfo
 bin/minifollowups/pycbc_page_injinfo
 bin/minifollowups/pycbc_page_snglinfo
 bin/minifollowups/pycbc_plot_chigram
 bin/minifollowups/pycbc_plot_trigger_timeseries
 bin/minifollowups/pycbc_single_template_plot
 bin/minifollowups/pycbc_sngl_minifollowup
-bin/minifollowups/pycbc_upload_prep_minifollowup
 bin/plotting/pycbc_banksim_plot_eff_fitting_factor
 bin/plotting/pycbc_banksim_plot_fitting_factors
 bin/plotting/pycbc_banksim_table_point_injs
 bin/plotting/pycbc_create_html_snippet
 bin/plotting/pycbc_faithsim_plots
 bin/plotting/pycbc_ifar_catalog
 bin/plotting/pycbc_mass_area_plot
 bin/plotting/pycbc_mchirp_plots
 bin/plotting/pycbc_page_banktriggerrate
 bin/plotting/pycbc_page_coinc_snrchi
-bin/plotting/pycbc_page_dq_table
 bin/plotting/pycbc_page_foreground
 bin/plotting/pycbc_page_foundmissed
 bin/plotting/pycbc_page_ifar
 bin/plotting/pycbc_page_injtable
 bin/plotting/pycbc_page_recovery
 bin/plotting/pycbc_page_segments
 bin/plotting/pycbc_page_segplot
 bin/plotting/pycbc_page_segtable
 bin/plotting/pycbc_page_sensitivity
 bin/plotting/pycbc_page_snrchi
 bin/plotting/pycbc_page_snrifar
 bin/plotting/pycbc_page_snrratehist
-bin/plotting/pycbc_page_template_bin_table
 bin/plotting/pycbc_page_versioning
 bin/plotting/pycbc_page_vetotable
 bin/plotting/pycbc_plot_background_coincs
 bin/plotting/pycbc_plot_bank_bins
 bin/plotting/pycbc_plot_bank_corner
 bin/plotting/pycbc_plot_dq_flag_likelihood
 bin/plotting/pycbc_plot_dq_likelihood_vs_time
@@ -552,15 +548,14 @@
 pycbc/results/mpld3_utils.py
 pycbc/results/plot.py
 pycbc/results/psd.py
 pycbc/results/pygrb_plotting_utils.py
 pycbc/results/pygrb_postprocessing_utils.py
 pycbc/results/render.py
 pycbc/results/scatter_histograms.py
-pycbc/results/snr.py
 pycbc/results/str_utils.py
 pycbc/results/table_utils.py
 pycbc/results/versioning.py
 pycbc/results/static/css/bootstrap.min.css
 pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css
 pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css
 pycbc/results/static/css/pycbc/orange.css
```

### Comparing `PyCBC-2.3.6/README.md` & `PyCBC-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_add_statmap` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_add_statmap`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         # Foreground group contains the time information for each ifo so
         # the ifos list can be reconstructed
         istring = ' '.join(sorted([k for k in fi['foreground'].keys()
                          if 'time' in fi['foreground/%s' % k]]))
     return istring
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action="version",
                     version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--statmap-files', nargs='+',
     help="List of coinc files to be combined")
 parser.add_argument('--background-files', nargs='+', default=None,
     help="full data coinc_statmap files for use in background"
          " calculation when used for injections")
 parser.add_argument('--censor-ifar-threshold', type=float, default=0.003,
     help="If provided, only window out foreground triggers with IFAR (years)"
@@ -341,16 +341,14 @@
             significance.get_far(
                 f_in['background_exc/stat'][:],
                 f['foreground/stat'][:],
                 f_in['background_exc/decimation_factor'][:],
                 f_in.attrs['background_time_exc'],
                 **significance_dict[ifo_combo_key])
 
-del ifo_combo_key
-
 logging.info('Combining false alarm rates from all available backgrounds')
 
 # Convert dictionary of whether the ifo combination is available at trigger
 # time into a 2D mask
 # Iterating over all_ifo_combos ensures that ordering remains the same
 isincombo_mask = np.array([list(is_in_combo_time[ct]) for ct in all_ifo_combos])
 
@@ -359,22 +357,16 @@
 fg_fars_exc = np.array([list(far_exc[ct]) for ct in all_ifo_combos])
 
 # Combine the FARs with the mask to obtain the new ifars
 fg_fars_out = np.sum(isincombo_mask * fg_fars, axis=0)
 fg_fars_exc_out = np.sum(isincombo_mask * fg_fars_exc, axis=0)
 
 # Apply any limits as appropriate
-fg_fars_out = significance.apply_far_limit(
-    fg_fars_out,
-    significance_dict,
-    combo=fg_coinc_type)
-fg_fars_exc_out = significance.apply_far_limit(
-    fg_fars_exc_out,
-    significance_dict,
-    combo=fg_coinc_type)
+fg_fars_out = significance.apply_far_limit(fg_fars_out, significance_dict, combo=fg_coinc_type)
+fg_fars_exc_out = significance.apply_far_limit(fg_fars_exc_out, significance_dict, combo=fg_coinc_type)
 
 fg_ifar = conv.sec_to_year(1. / fg_fars_out)
 fg_ifar_exc = conv.sec_to_year(1. / fg_fars_exc_out)
 fg_time = f.attrs['foreground_time']
 del isincombo_mask, fg_fars, fg_fars_exc, _
 
 f.attrs['foreground_time_exc'] = f.attrs['foreground_time']
@@ -566,15 +558,14 @@
                          sep_fg_data[maxcombo].data['stat'][:][max_ifar_idx])
     sep_fg_data[maxcombo] = sep_fg_data[maxcombo].remove(max_ifar_idx)
 
     # Add to final dataset and remove from continuing dataset
     final_combined_fg = final_combined_fg + \
                             combined_fg_data.select(where_combined)
     combined_fg_data = combined_fg_data.remove(where_combined)
-    fg_coinc_type = np.delete(fg_coinc_type, where_combined)
     n_triggers -= 1
 
     logging.info('Removing background triggers at time {} within window '
                  '{}s'.format(maxtime, args.hierarchical_removal_window))
     for combo in all_ifo_combos:
         all_hred_idx = []
         for ifo in all_ifos:
@@ -609,61 +600,44 @@
         bg_t_y = conv.sec_to_year(bg_time_ct[key])
         fg_t_y = conv.sec_to_year(fg_time_ct[key])
         bg_far, fg_far = significance.get_far(
             sep_bg_data[key].data['stat'],
             sep_fg_data[key].data['stat'],
             sep_bg_data[key].data['decimation_factor'],
             bg_t_y,
-            **significance_dict[key])
-        fg_far = significance.apply_far_limit(
-            fg_far,
-            significance_dict,
-            combo=key,
-        )
-        bg_far = significance.apply_far_limit(
-            bg_far,
-            significance_dict,
-            combo=key,
-        )
-
+            **significance_dict[ifo_combo_key])
         sep_bg_data[key].data['ifar'] = 1. / bg_far
         sep_fg_data[key].data['ifar'] = 1. / fg_far
         sep_fg_data[key].data['fap'] = 1 - \
             np.exp(-fg_t_y * fg_far)
 
     logging.info("Recalculating combined IFARs")
     for key in all_ifo_combos:
         _, far[key] = significance.get_far(
             sep_bg_data[key].data['stat'],
             combined_fg_data.data['stat'],
             sep_bg_data[key].data['decimation_factor'],
             bg_time_ct[key],
-            **significance_dict[key])
+            **significance_dict[ifo_combo_key])
         # Set up variable for whether each coincidence is available in each coincidence time
         is_in_combo_time[key] = np.zeros(n_triggers)
         end_times = np.array(f['segments/%s/end' % key][:])
         start_times = np.array(f['segments/%s/start' % key][:])
         idx_within_segment = pycbc.events.indices_within_times(test_times,
                                                                start_times,
                                                                end_times)
         is_in_combo_time[key][idx_within_segment] = \
             np.ones_like(idx_within_segment)
 
     isincombo_mask = np.array([list(is_in_combo_time[ct])
                                for ct in all_ifo_combos])
     fg_fars = np.array([list(far[ct]) for ct in all_ifo_combos])
-    fg_fars_out = np.sum(isincombo_mask * fg_fars, axis=0)
-    fg_fars_out = significance.apply_far_limit(
-        fg_fars_out,
-        significance_dict,
-        combo=fg_coinc_type,
-    )
     # Combine the FARs with the mask to obtain the new ifars
     combined_fg_data.data['ifar'] = conv.sec_to_year(
-        1. / fg_fars_out)
+        1. / np.sum(isincombo_mask * fg_fars, axis=0))
     fg_time -= args.cluster_window
     combined_fg_data.data['fap'] = 1 - \
         np.exp(-conv.sec_to_year(fg_time) / combined_fg_data.data['ifar'])
 
 for combo in all_ifo_combos:
     final_fg_data[combo] = final_fg_data[combo] + sep_fg_data[combo]
     for key in final_fg_data[combo].data:
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_apply_rerank` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_apply_rerank`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 """
 import h5py, numpy, argparse, logging, pycbc
 from pycbc.conversions import sec_to_year
 from pycbc.events import significance
 from shutil import copyfile
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
     version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--stat-files', nargs='+',
     help="Statistic files produced by candidate followup codes")
 parser.add_argument('--followup-file',
     help="File containing the candidate times which were analyzed")
 parser.add_argument('--statmap-file',
     help="The statmap file containing the candidates to rerank")
 significance.insert_significance_option_group(parser)
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_average_psd` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_average_psd`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 import h5py
 import pycbc
 from pycbc.version import git_verbose_msg as version
 from pycbc.types import MultiDetOptionAction, FrequencySeries
 
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version', version=version)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--input-files', nargs='+', required=True, metavar='PATH',
                     help='HDF5 files from pycbc_calculate_psd (one per '
                          'detector) containing the input PSDs to average.')
 parser.add_argument('--time-avg-file', nargs='+', action=MultiDetOptionAction,
                     metavar='DETECTOR:PATH',
                     help='Output file names for single-detector PSDs averaged '
                          'over time.')
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_bin_templates` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_foreground_censor`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 #!/usr/bin/env python
-""" Bin templates by their duration
-"""
-import logging
-import argparse
-import h5py as h5
-import numpy as np
-
-import pycbc
-import pycbc.pnutils
-from pycbc.version import git_verbose_msg as version
-from pycbc.events import background_bin_from_string
+"""Make segment file to blind the results from foreground related triggers """
 
-parser = argparse.ArgumentParser(description=__doc__)
-parser.add_argument('--version', action='version', version=version)
-parser.add_argument('--verbose', action="count")
-parser.add_argument("--ifo", type=str, required=True)
-parser.add_argument("--f-lower", type=float, default=15.,
-                    help='Enforce a uniform low frequency cutoff to '
-                         'calculate template duration over the bank')
-parser.add_argument('--bank-file', help='hdf format template bank file',
-                    required=True)
-parser.add_argument('--background-bins', nargs='+',
-                    help='Used to provide a list of '
-                         'precomputed background bins')
-parser.add_argument("--output-file", required=True)
+import os, argparse, logging, pycbc.version, h5py
+from urllib.parse import urlunparse
+import pycbc.events
+from pycbc.workflow import SegFile
 
+parser = argparse.ArgumentParser(description=__doc__)
+parser.add_argument('--version', action='version', version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
+parser.add_argument('--foreground-triggers',
+                    help="HDF file containing the zerolag foreground triggers "
+                         "from the analysis")
+parser.add_argument('--veto-file',
+                    help="Baseline veto information that is added to the outptut")
+parser.add_argument('--segment-name',
+                    help="Segment name to use from the input veto file")
+parser.add_argument('--output-file', help='Name of the output segment file')
+parser.add_argument('--output-segment-name',
+                    help="(optional), Name of output segment file list",
+                    default="censor_foreground")
 args = parser.parse_args()
 
 pycbc.init_logging(args.verbose)
-logging.info('Starting template binning')
 
-with h5.File(args.bank_file, 'r') as bank:
-    logging.info('Sorting bank into bins')
-    data = {
-        'mass1': bank['mass1'][:],
-        'mass2': bank['mass2'][:],
-        'spin1z': bank['spin1z'][:],
-        'spin2z': bank['spin2z'][:],
-        'f_lower': np.ones_like(bank['mass1'][:]) * args.f_lower
-        }
-
-    bin_dict = background_bin_from_string(args.background_bins, data)
-    bin_names = [b.split(':')[0] for b in args.background_bins]
-
-logging.info('Writing bin template ids to file')
-with h5.File(args.output_file, 'w') as f:
-    ifo_grp = f.create_group(args.ifo)
-    for bin_name in bin_names:
-        bin_tids = bin_dict[bin_name]
-        grp = ifo_grp.create_group(bin_name)
-        grp['tids'] = bin_tids
-    f.attrs['f_lower'] = args.f_lower
-    f.attrs['background_bins'] = args.background_bins
+logging.info('Start')
+
+f = h5py.File(args.foreground_triggers, 'r')
 
-logging.info('Finished')
+start = f['segments/foreground_veto/start'][:]
+end = f['segments/foreground_veto/end'][:]
+vsegs = pycbc.events.start_end_to_segments(start, end)
+
+logging.info('Read in foreground veto segments')
+
+# 2-ifo old style format
+if 'detector_1' in f.attrs:
+    ifo1, ifo2 = f.attrs['detector_1'], f.attrs['detector_2']
+    ifos = [ifo1, ifo2]
+# Multi-ifo format file
+else:
+    ifos = f.attrs['ifos'].split(' ')
+
+fsegs, names = [], []
+for ifo in ifos:
+    segs = pycbc.events.select_segments_by_definer(args.veto_file, args.segment_name, ifo)
+    logging.info('Read in veto segments from %s' % ifo)
+    fsegs += [segs.coalesce() + vsegs.coalesce()]
+    names += [args.output_segment_name]
+
+file_url = urlunparse(['file', 'localhost',
+                       os.path.abspath(args.output_file), None, None, None])
+SegFile.from_multi_segment_list('UNUSED', fsegs, names, ifos, file_url=file_url)
+logging.info('Done')
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_calculate_psd` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_calculate_psd`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from pycbc.version import git_verbose_msg as version
 from pycbc.fft.fftw import set_measure_level
 from pycbc.workflow import resolve_td_option
 from ligo.segments import segmentlist, segment
 set_measure_level(0)
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version', version=version)
+parser.add_argument('--verbose', action="store_true")
 parser.add_argument("--low-frequency-cutoff", type=float, required=True,
                     help="The low frequency cutoff to use for filtering (Hz)")
 parser.add_argument("--analysis-segment-file",  required=True,
                     help="File defining the segments to estimate PSDs over")
 parser.add_argument("--segment-name", help="Name of segment list to use")
 parser.add_argument("--cores", default=1, type=int)
 parser.add_argument("--output-file", required=True)
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_findtrigs` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_findtrigs`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 import h5py, copy, argparse, logging, numpy, numpy.random
 import shutil, uuid, os.path, atexit
 from ligo.segments import infinity
 from pycbc.events import veto, coinc, stat, ranking, cuts
 import pycbc.version
-from pycbc import pool, init_logging
+from pycbc import pool
 from numpy.random import seed, shuffle
 from pycbc.io.hdf import ReadByTemplate
 from pycbc.types.optparse import MultiDetOptionAction
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
+parser.add_argument("--verbose", action="count")
 parser.add_argument("--version", action="version", version=pycbc.version.git_verbose_msg)
 parser.add_argument("--veto-files", nargs='*', action='append', default=[],
                     help="Optional veto file. Triggers within veto segments "
                          "contained in the file are ignored")
 parser.add_argument("--segment-name", nargs='*', action='append', default=[],
                     help="Optional, name of veto segment in veto file")
 parser.add_argument("--gating-veto-windows", nargs='+',
@@ -74,15 +74,17 @@
 args = parser.parse_args()
 
 # flatten the list of lists of filenames to a single list (may be empty)
 args.segment_name = sum(args.segment_name, [])
 args.veto_files = sum(args.veto_files, [])
 args.trigger_files = sum(args.trigger_files, [])
 
-init_logging(args.verbose)
+if args.verbose:
+    logging.basicConfig(format='%(asctime)s : %(message)s', level=logging.DEBUG)
+
 
 def parse_template_range(num_templates, rangestr):
     part = int(rangestr.split('/')[0])
     pieces = int(rangestr.split('/')[1])
     tmin = int(num_templates / float(pieces) * part)
     tmax = int(num_templates / float(pieces) * (part+1))
     return tmin, tmax
@@ -232,24 +234,24 @@
 
 # Gather the coincs from a single template
 def process_template(tnum):
     local_data = copy.deepcopy(data)
     times_full = {}
     sds_full = {}
     tids_full = {}
-    logging.debug('Obtaining trigs for template %i ..' % (tnum))
+    logging.info('Obtaining trigs for template %i ..' % (tnum))
     for i, sngl in zip(trigs.ifos, trigs.singles):
         # Apply cuts to triggers
         tids_uncut = sngl.set_template(tnum)
         trigger_keep_ids = cuts.apply_trigger_cuts(sngl, trigger_cut_dict,
                                                    statistic=rank_method)
 
         tids_full[i] = tids_uncut[trigger_keep_ids]
         times_full[i] = sngl['end_time'][trigger_keep_ids]
-        logging.debug('%s:%s', i, len(tids_uncut))
+        logging.info('%s:%s', i, len(tids_uncut))
         if len(tids_full[i]) < len(tids_uncut):
             logging.info("%s triggers cut",
                          len(tids_uncut) - len(tids_full[i]))
 
 
         # get single-detector statistic
         sds_full[i] = rank_method.single(sngl)[trigger_keep_ids]
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_hdfinjfind` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_hdfinjfind`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Associate coincident triggers with injections listed in one or more LIGOLW
 files.
 """
 
 import argparse, h5py, logging, types, numpy, os.path
 from ligo.lw import lsctables, utils as ligolw_utils
 from ligo import segments
-from pycbc import events, init_logging
+from pycbc import events
 from pycbc.events import indices_within_segments
 from pycbc.types import MultiDetOptionAction
 from pycbc.inject import CBCHDFInjectionSet
 import pycbc.version
 from pycbc.io.ligolw import LIGOLWContentHandler
 
 
@@ -51,15 +51,14 @@
         else:
             new_col = col
         key = os.path.join(hdf_key, new_col)
         hdf_append(hdf_file, key, numpy.array(table.getColumnByName(col),
                                         dtype=numpy.float32))
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--trigger-files', nargs='+', required=True)
 parser.add_argument('--injection-files', nargs='+', required=True)
 parser.add_argument('--veto-file')
 parser.add_argument('--segment-name', default=None,
                     help='Name of segment list to use for vetoes. Optional')
@@ -70,18 +69,21 @@
 parser.add_argument('--optimal-snr-column', nargs='+',
                     action=MultiDetOptionAction, metavar='DETECTOR:COLUMN',
                     help='Names of the sim_inspiral columns containing the'
                     ' optimal SNRs.')
 parser.add_argument('--redshift-column', default=None,
                     help='Name of sim_inspiral column containing redshift. '
                     'Optional')
+parser.add_argument('--verbose', action='count')
 parser.add_argument('--output-file', required=True)
 args = parser.parse_args()
 
-init_logging(args.verbose)
+if args.verbose:
+    log_level = logging.INFO
+    logging.basicConfig(format='%(asctime)s : %(message)s', level=log_level)
 
 fo = h5py.File(args.output_file, 'w')
 
 injection_index = 0
 for trigger_file, injection_file in zip(args.trigger_files,
                                         args.injection_files):
     logging.info('Read in the coinc data: %s' % trigger_file)
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_mergetrigs` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_mergetrigs`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """ This program adds single detector hdf trigger files together.
 """
 
 import numpy, argparse, h5py, logging
 import pycbc.version
-from pycbc import init_logging
+
 
 def changes(arr):
     l = numpy.where(arr[:-1] != arr[1:])[0]
     l = numpy.concatenate(([0], l+1, [len(arr)]))
     return numpy.unique(l)
 
 def collect(key, files):
@@ -26,26 +26,26 @@
     for j in range(len(boundaries) - 1):
         l, r = boundaries[ids[j]], boundaries[ids[j]+1]
         refs.append(dset.regionref[l:r]) 
     f.create_dataset(key+'_template', data=refs,
                      dtype=h5py.special_dtype(ref=h5py.RegionReference))
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--trigger-files', nargs='+')
 parser.add_argument('--output-file', required=True)
 parser.add_argument('--bank-file', required=True)
 parser.add_argument('--compression-level', type=int, default=6,
                     help='Set HDF compression level in the output file '
                          '(default 6)')
+parser.add_argument('--verbose', '-v', action='count')
 args = parser.parse_args()
 
-init_logging(args.verbose)
+logging.basicConfig(format='%(asctime)s : %(message)s', level=logging.INFO)
 
 f = h5py.File(args.output_file, 'w')
 
 logging.info("getting the list of columns from a representative file")
 trigger_columns = []
 for fname in args.trigger_files:
     try:
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_statmap` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_statmap`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,22 @@
             self.f[name][:] = data
 
     def __getitem__(self, *args):
         return self.f.__getitem__(*args)
 
 parser = argparse.ArgumentParser()
 # General required options
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--coinc-files', nargs='+',
                     help='List of coincidence files used to calculate the '
                          'FAP, FAR, etc.')
 parser.add_argument('--ifos', nargs='+',
                     help='List of ifos used in these coincidence files')
+parser.add_argument('--verbose', action='count')
 parser.add_argument('--cluster-window', type=float, default=10,
                     help='Length of time window in seconds to cluster coinc '
                          'events [default=10s]')
 parser.add_argument('--veto-window', type=float, default=.1,
                     help='Time around each zerolag trigger to window out '
                          '[default=.1s]')
 parser.add_argument('--hierarchical-removal-window', type=float, default=1.0,
@@ -253,30 +253,18 @@
 bg_far_exc, fg_far_exc = significance.get_far(
     exc_zero_trigs.stat,
     fore_stat,
     exc_zero_trigs.decimation_factor,
     background_time_exc,
     **significance_dict[ifo_combo])
 
-fg_far = significance.apply_far_limit(
-    fg_far,
-    significance_dict,
-    combo=ifo_combo)
-bg_far = significance.apply_far_limit(
-    bg_far,
-    significance_dict,
-    combo=ifo_combo)
-fg_far_exc = significance.apply_far_limit(
-    fg_far_exc,
-    significance_dict,
-    combo=ifo_combo)
-bg_far_exc = significance.apply_far_limit(
-    bg_far_exc,
-    significance_dict,
-    combo=ifo_combo)
+fg_far = significance.apply_far_limit(fg_far, significance_dict, combo=ifo_combo)
+bg_far = significance.apply_far_limit(bg_far, significance_dict, combo=ifo_combo)
+fg_far_exc = significance.apply_far_limit(fg_far_exc, significance_dict, combo=ifo_combo)
+bg_far_exc = significance.apply_far_limit(bg_far_exc, significance_dict, combo=ifo_combo)
 
 f['background/ifar'] = conv.sec_to_year(1. / bg_far)
 f['background_exc/ifar'] = conv.sec_to_year(1. / bg_far_exc)
 f.attrs['background_time'] = background_time
 f.attrs['foreground_time'] = coinc_time
 f.attrs['background_time_exc'] = background_time_exc
 f.attrs['foreground_time_exc'] = coinc_time_exc
@@ -429,44 +417,28 @@
         back_stat,
         fore_stat,
         all_trigs.decimation_factor[back_locs],
         background_time,
         return_counts=True,
         **significance_dict[ifo_combo])
 
-    fg_far = significance.apply_far_limit(
-        fg_far,
-        significance_dict,
-        combo=ifo_combo
-    )
-    bg_far = significance.apply_far_limit(
-        bg_far,
-        significance_dict,
-        combo=ifo_combo,
-    )
-
     # Update the ifar_foreground criteria depending on whether foreground
     # triggers are being removed via inclusive or exclusive background.   
     if args.hierarchical_removal_against == 'inclusive':
         ifar_foreground = 1. / fg_far
 
     # Exclusive background doesn't change when removing foreground triggers.
     # So we don't have to take background ifar, just repopulate ifar_foreground
     else :
         _, fg_far_exc = significance.get_far(
             exc_zero_trigs.stat,
             fore_stat,
             exc_zero_trigs.decimation_factor,
             background_time_exc,
             **significance_dict[ifo_combo])
-        fg_far_exc = significance.apply_far_limit(
-            fg_far_exc,
-            significance_dict,
-            combo=ifo_combo
-        )
         ifar_foreground = 1. / fg_far_exc
     # ifar_foreground has been updated and the code can continue.
 
     logging.info("Calculating ifar/fap values")
     f['background_h%s/ifar' % h_iterations] = conv.sec_to_year(1. / bg_far)
     f.attrs['background_time_h%s' % h_iterations] = background_time
     f.attrs['foreground_time_h%s' % h_iterations] = coinc_time
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_coinc_statmap_inj` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_coinc_statmap_inj`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 by pycbc_coinc_findtrigs to generated a mapping between SNR and FAP, along
 with producing the combined foreground and background triggers
 """
 import argparse, h5py, logging, itertools, copy, pycbc.io, numpy, lal
 from pycbc.events import veto, coinc, significance
 import pycbc.version
 import pycbc.conversions as conv
-from pycbc import init_logging
 
 parser = argparse.ArgumentParser()
 # General required options
-pycbc.add_common_pycbc_options(parser)
+parser.add_argument('--verbose', action='count')
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--cluster-window', type=float, default=10,
                     help='Length of time window in seconds to cluster coinc '
                          'events [default=10s]')
 parser.add_argument('--zero-lag-coincs', nargs='+',
                     help='Files containing the injection zerolag coincidences')
@@ -28,42 +27,35 @@
                          '[default=.1s]')
 parser.add_argument('--ifos', nargs='+',
                     help='List of ifos used in these coincidence files')
 significance.insert_significance_option_group(parser)
 parser.add_argument('--output-file')
 args = parser.parse_args()
 
-init_logging(args.verbose)
-
 significance.check_significance_options(args, parser)
 
+if args.verbose:
+    log_level = logging.INFO
+    logging.basicConfig(format='%(asctime)s : %(message)s', level=log_level)
+
+ifo_key = ''.join(args.ifos)
+significance_dict = significance.digest_significance_options([ifo_key], args)
 
 window = args.cluster_window
 logging.info("Loading coinc zerolag triggers")
 zdata = pycbc.io.MultiifoStatmapData(files=args.zero_lag_coincs, ifos=args.ifos)
-
-if 'ifos' in zdata.attrs:
-    ifos = zdata.attrs['ifos'].split(' ')
-    logging.info('using ifos from file {}'.format(args.zero_lag_coincs[0]))
-else:
-    ifos = args.ifos
-    logging.info('using ifos from command line input')
-
-ifo_key = ''.join(ifos)
-significance_dict = significance.digest_significance_options([ifo_key], args)
-
 zdata = zdata.cluster(window)
 
 f = h5py.File(args.output_file, "w")
 
 f.attrs['num_of_ifos'] = zdata.attrs['num_of_ifos']
 f.attrs['pivot'] = zdata.attrs['pivot']
 f.attrs['fixed'] = zdata.attrs['fixed']
 f.attrs['timeslide_interval'] = zdata.attrs['timeslide_interval']
-f.attrs['ifos'] = ' '.join(sorted(ifos))
+f.attrs['ifos'] = ' '.join(sorted(args.ifos))
 
 # Copy over the segment for coincs and singles
 for key in zdata.seg.keys():
     f['segments/%s/start' % key] = zdata.seg[key]['start'][:]
     f['segments/%s/end' % key] = zdata.seg[key]['end'][:]
 
 logging.info('writing zero lag triggers')
@@ -94,19 +86,15 @@
     _, fg_far_exc = significance.get_far(
         back_stat,
         zdata.stat,
         dec_fac,
         background_time,
         **significance_dict[ifo_key])
 
-    fg_far_exc = significance.apply_far_limit(
-        fg_far_exc,
-        significance_dict,
-        combo=ifo_key,
-    )
+    fg_far_exc = significance.apply_far_limit(fg_far_exc, significance_dict, combo=ifo_key)
 
     ifar_exc = 1. / fg_far_exc
     fap_exc = 1 - numpy.exp(- coinc_time / ifar_exc)
     f['foreground/ifar_exc'] = conv.sec_to_year(ifar_exc)
     f['foreground/fap_exc'] = fap_exc
 
 else:
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_combine_coincident_events` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_combine_coincident_events`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         new_group = group[:-1] + new_det_num
 
         data_for_catting.append(nfp[new_group][:])
     f[group] = numpy.concatenate(data_for_catting)
     
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action="version", version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--statmap-files', nargs='+',
                     help="List of coinc files to be redistributed")
 parser.add_argument('--output-file', help="name of output file")
 args = parser.parse_args()
 
 pycbc.init_logging(args.verbose)
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_combine_statmap` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_combine_statmap`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 """
 
 import h5py, numpy, argparse, logging, pycbc, pycbc.events, pycbc.io, lal
 import pycbc.version
 from ligo import segments
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action="version", version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--statmap-files', nargs='+',
                     help="List of coinc files to be redistributed")
 parser.add_argument('--cluster-window', type=float)
 parser.add_argument('--censor-ifar-threshold', type=float, default=0.003,
     help="If provided, only window out foreground triggers with IFAR (years)"
          "above the threshold [default=0.003yr]")
 parser.add_argument('--veto-window', type=float, default=0.1,
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_cut_merge_triggers_to_tmpltbank`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 import argparse
 import numpy
 import h5py
 import pycbc
 import pycbc.version
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action="version",
                     version=pycbc.version.git_verbose_msg)
+parser.add_argument("-V", "--verbose", action="store_true",
+                    help="print extra debugging information", default=False)
 parser.add_argument("--input-file", required=True,
                     help="Input merge triggers HDF file.")
 parser.add_argument("--output-file", required=True,
                     help="Output merge triggers HDF file.")
 parser.add_argument("--full-template-bank", required=True,
                     help="The original full template bank HDF file.")
 parser.add_argument("--filter-func-file", required=True,
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_distribute_background_bins` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_distribute_background_bins`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/env python
 import h5py, argparse, numpy, pycbc.events, logging, pycbc.events, pycbc.io
 import pycbc.version
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--version", action=pycbc.version.Version)
-pycbc.add_common_pycbc_options(parser)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--coinc-files', nargs='+',
                     help="List of coinc files to be redistributed")
 parser.add_argument('--background-bins', nargs='+',
                     help="Ordered list of mass bin upper boundaries. "
                          "An ordered list of type-boundary pairs, applied sequentially."
                          "Must provide a name (can be any unique string for tagging "
                          "purposes), the parameter to bin on, and the membership "
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_dtphase` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_dtphase`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 import argparse, h5py, numpy as np, pycbc.detector, logging
 from numpy.random import uniform
 from scipy.stats import norm
 from copy import deepcopy
 
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--ifos', nargs='+',
                     help="The ifos to generate a histogram for")
 parser.add_argument('--sample-size', type=int, required=True,
                     help="Approximate number of independent samples to draw "
                          "for the distribution")
 parser.add_argument('--snr-ratio', type=float, required=True,
                     help="The SNR ratio permitted between reference ifo and "
                          "all others. Ex. giving 4 permits a ratio of "
                          "0.25 -> 4")
 parser.add_argument('--relative-sensitivities', nargs='+', type=float,
                     help="Numbers proportional to horizon distance or "
                          "expected SNR at fixed distance, one for each ifo")
 parser.add_argument('--seed', type=int, default=124)
 parser.add_argument('--output-file', required=True)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--bin-density', type=int, default=1,
                     help="Number of bins per 1 sigma uncertainty in a "
                          "parameter. Higher values increase the resolution of "
                          "the histogram at the expense of storage.")
 parser.add_argument('--smoothing-sigma', type=int, default=2,
                     help="Width of the smoothing kernel in sigmas")
 parser.add_argument('--timing-uncertainty', type=float, default=.001,
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_exclude_zerolag` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_exclude_zerolag`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import h5py, numpy as np, argparse, logging, pycbc, pycbc.io
 import pycbc.version
 from pycbc.events import veto, coinc, significance
 import pycbc.conversions as conv
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action="version",
                     version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--statmap-file', type=str,
     help="Coinc statmap file to be recalculated based on foreground removal")
 parser.add_argument('--other-statmap-files', nargs='+',
     help="List of coinc statmap files from other coincidence types")
 parser.add_argument('--censor-ifar-threshold', type=float, default=0.003,
     help="Only window out foreground triggers with IFAR (years)"
          "above the threshold [default=0.003yr]")
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_binned` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_binned`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 import pycbc.version
 
 #### MAIN ####
 
 parser = argparse.ArgumentParser(usage="",
     description="Perform maximum-likelihood fits of single inspiral trigger"
                 " distributions to various functions")
-pycbc.add_common_pycbc_options(parser)
+
 parser.add_argument("--version", action=pycbc.version.Version)
+parser.add_argument("-V", "--verbose", action="store_true",
+                    help="Print extra debugging information", default=False)
 parser.add_argument("--trigger-file",
                     help="Input hdf5 file containing single triggers. "
                     "Required")
 parser.add_argument("--bank-file", default=None,
                     help="hdf file containing template parameters. Required")
 parser.add_argument("--veto-file", nargs='*', default=[], action='append',
                     help="File(s) in .xml format with veto segments to apply "
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_by_template` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_by_template`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 import sys, h5py
 import argparse, logging
 
 import copy, numpy as np
 
-from pycbc import io, events, init_logging
+from pycbc import io, events
 from pycbc.events import triggers, trigger_fits as trstats
 from pycbc.events import stat as statsmod
 from pycbc.types.optparse import MultiDetOptionAction
 import pycbc.version
 
 #### DEFINITIONS AND FUNCTIONS ####
 
@@ -55,16 +55,18 @@
     return np.concatenate(select), np.concatenate(stat)
 
 #### MAIN ####
 
 parser = argparse.ArgumentParser(usage="",
     description="Perform maximum-likelihood fits of single inspiral trigger"
                 " distributions to various functions")
-pycbc.add_common_pycbc_options(parser)
+
 parser.add_argument("--version", action=pycbc.version.Version)
+parser.add_argument("-V", "--verbose", action="store_true",
+                    help="Print extra debugging information", default=False)
 parser.add_argument("--trigger-file",
                     help="Input hdf5 file containing single triggers. "
                     "Required")
 parser.add_argument("--bank-file", default=None,
                     help="hdf file containing template parameters. Required")
 parser.add_argument("--template-fraction-range", default="0/1",
                     help="Optional, analyze only part of template bank. "
@@ -118,27 +120,31 @@
 parser.add_argument("--approximant", default="SEOBNRv4",
                     help="Approximant for template duration. Default SEOBNRv4")
 
 statsmod.insert_statistic_option_group(parser,
     default_ranking_statistic='single_ranking_only')
 args = parser.parse_args()
 
-init_logging(args.verbose)
-
 args.veto_segment_name = sum(args.veto_segment_name, [])
 args.veto_file = sum(args.veto_file, [])
 
 if len(args.veto_segment_name) != len(args.veto_file):
     raise RuntimeError("Number of veto files much match veto file names")
 
 if (args.prune_param or args.prune_bins or args.prune_number) and not \
    (args.prune_param and args.prune_bins and args.prune_number):
     raise RuntimeError("To prune, need to specify param, number of bins and "
                        "nonzero number to prune in each bin!")
 
+if args.verbose:
+    log_level = logging.DEBUG
+else:
+    log_level = logging.WARN
+logging.basicConfig(format='%(asctime)s : %(message)s', level=log_level)
+
 logging.info('Fitting above threshold %f' % args.stat_threshold)
 
 logging.info('Opening trigger file: %s' % args.trigger_file)
 trigf = h5py.File(args.trigger_file, 'r')
 logging.info('Opening template file: %s' % args.bank_file)
 templatef = h5py.File(args.bank_file, 'r')
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_over_multiparam` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_over_multiparam`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
 # Public License for more details.
 
 
 import sys, h5py, argparse, logging, pycbc.version, numpy
 from scipy.stats import norm
 from pycbc.events import triggers
-from pycbc import init_logging
+
 
 def dist(i1, i2, parvals, smoothing_width):
     """
     Computes the vector of parameter values at index/indices i1 and
     index/indices i2, and gives the Euclidean distance between
     the two with a metric of 1/(smoothing width^2)
     """
@@ -168,16 +168,17 @@
 
 parser = argparse.ArgumentParser(usage="",
     description="Smooth (regress) the dependence of coefficients describing "
                 "single-ifo background trigger distributions on a template "
                 "parameter, to suppress random noise in the resulting "
                 "background model.")
 
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action=pycbc.version.Version)
+parser.add_argument("-V", "--verbose", action="store_true",
+                    help="Print extra debugging information", default=False)
 parser.add_argument("--template-fit-file",
                     help="hdf5 file containing fit coefficients for each"
                          " individual template. Required")
 parser.add_argument("--bank-file", default=None,
                     help="hdf file containing template parameters. Required "
                          "unless reading param from template fit file")
 parser.add_argument("--output", required=True,
@@ -245,15 +246,15 @@
             err_txt = "--smoothing-keywords must take input in the " \
                       "form KWARG1:VALUE1 KWARG2:VALUE2 KWARG3:VALUE3 ... " \
                       "Received {}".format(' '.join(args.smoothing_keywords))
             raise ValueError(err_txt)
 
 assert len(args.log_param) == len(args.fit_param) == len(args.smoothing_width)
 
-init_logging(args.verbose)
+pycbc.init_logging(args.verbose)
 
 fits = h5py.File(args.template_fit_file, 'r')
 
 # get the ifo from the template-level fit
 ifo = fits.attrs['ifo']
 
 # get template id and template parameter values
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_over_param` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_over_param`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 
 import sys, h5py
 import argparse, logging
 
 import numpy as np
 
-from pycbc import init_logging
 from pycbc.events import triggers
 import pycbc.version
 
 parser = argparse.ArgumentParser(usage="",
     description="Smooth (regress) the dependence of coefficients describing "
                 "single-ifo background trigger distributions on a template "
                 "parameter, to suppress random noise in the resulting "
                 "background model.")
 
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action=pycbc.version.Version)
+parser.add_argument("-V", "--verbose", action="store_true",
+                    help="Print extra debugging information", default=False)
 parser.add_argument("--template-fit-file",
                     help="Input hdf5 file containing fit coefficients for each"
                          " individual template. Required")
 parser.add_argument("--bank-file", default=None,
                     help="hdf file containing template parameters. Required "
                          "unless reading param from template fit file")
 parser.add_argument("--output", required=True,
@@ -74,15 +74,19 @@
                          "template duration, try 0.2")
 
 args = parser.parse_args()
 
 if args.regression_method == 'nn' and args.num_neighbors < 1:
     raise RuntimeError("Need to give a positive number of nearest neighbors!")
 
-init_logging(args.verbose)
+if args.verbose:
+    log_level = logging.DEBUG
+else:
+    log_level = logging.WARN
+logging.basicConfig(format='%(asctime)s : %(message)s', level=log_level)
 
 fits = h5py.File(args.template_fit_file, 'r')
 
 # get the ifo from the template-level fit
 ifo = fits.attrs['ifo']
 
 # get template id and template parameter values
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_fit_sngls_split_binned` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_fit_sngls_split_binned`

 * *Files 16% similar despite different names*

```diff
@@ -18,31 +18,30 @@
 
 from matplotlib import use
 use('Agg')
 from matplotlib import pyplot as plt
 import numpy as np
 
 from pycbc import events, bin_utils, results
-from pycbc.io import HFile, SingleDetTriggers
 from pycbc.events import triggers as trigs
 from pycbc.events import trigger_fits as trstats
 from pycbc.events import stat as pystat
 from pycbc.types.optparse import MultiDetOptionAction
 import pycbc.version
 
 parser = argparse.ArgumentParser(usage="",
     description="Plot histograms of triggers split over various parameters")
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--trigger-file", required=True,
                     help="Input hdf5 file containing single triggers. "
                          "Required")
 parser.add_argument("--bank-file", default=None, required=True,
                     help="hdf file containing template parameters. Required")
 parser.add_argument('--output-file', required=True,
                     help="Output image file. Required")
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--bin-param', default='template_duration',
                     help="Parameter for binning within plots, default "
                          "'template_duration'")
 parser.add_argument('--bin-spacing', choices=['linear', 'log'], default='log',
                     help="How to space bin-param bin edges. "
                          "Choices=[linear, log], default log")
 parser.add_argument('--num-bins', type=int, default=6,
@@ -79,34 +78,28 @@
                     action=MultiDetOptionAction,
                     help="Seconds to be vetoed before and after the central time "
                          "of each gate. Given as detector-values pairs, e.g. "
                          "H1:-1,2.5 L1:-1,2.5 V1:0,0")
 parser.add_argument("--stat-fit-threshold", type=float, required=True,
                     help="Only fit triggers with statistic value above this "
                          "threshold. Required")
-parser.add_argument("--plot-lower-stat-limit", type=float, required=True,
-                    help="Plot triggers down to this value. Setting this too"
-                         "low will incur huge memory usage in a full search."
-                         "To avoid this, choose 5.5 or larger.")
 parser.add_argument("--fit-function",
                     choices=["exponential", "rayleigh", "power"],
                     help="Functional form for the maximum likelihood fit")
 parser.add_argument("--prune-number", type=int, default=0,
                     help="Number of loudest events to remove from each split "
                          "histogram, default 0")
 parser.add_argument("--prune-window", type=float, default=0.1,
                     help="Time (s) to remove all triggers around a trigger "
                          "which is loudest in each split, default 0.1s")
 
 pystat.insert_statistic_option_group(parser,
     default_ranking_statistic='single_ranking_only')
 args = parser.parse_args()
 
-assert(args.stat_fit_threshold >= args.plot_lower_stat_limit)
-
 pycbc.init_logging(args.verbose)
 
 logging.info('Opening trigger file: %s' % args.trigger_file)
 trigf = h5py.File(args.trigger_file, 'r')
 
 logging.info('Opening template file: %s' % args.bank_file)
 bank = h5py.File(args.bank_file, 'r')
@@ -125,20 +118,16 @@
              if par in usedparams]
 
 for ex_p in extparams:
     if ex_p == 'template_duration':
         logging.info('Reading duration from trigger file')
         # List comprehension loops over templates; if a template has no triggers, accessing
         # the 0th entry of its region reference will return zero due to a quirk of h5py.
-        params[ex_p] = np.array(
-            [
-                trigf[args.ifo + '/template_duration'][ref][0]
-                for ref in trigf[args.ifo + '/template_duration_template'][:]
-            ]
-        )
+        params[ex_p] = np.array([trigf[args.ifo + '/template_duration'][ref][0]
+                                 for ref in trigf[args.ifo + '/template_duration_template'][:]])
     else:
         logging.info("Calculating " + ex_p + " from template parameters")
         params[ex_p] = trigs.get_param(ex_p, args, params['mass1'],
                                        params['mass2'], params['spin1z'],
                                        params['spin2z'])
 
 # string formats for labels, logging etc.
@@ -205,144 +194,65 @@
 for i, lower_2, upper_2 in zip(range(args.split_two_nbins),
                                sp_two_bounds.lower(), sp_two_bounds.upper()):
     id_in_bin2[i] = np.intersect1d(np.argwhere(params[args.split_param_two] > lower_2),
                                    np.argwhere(params[args.split_param_two] <= upper_2))
 
 logging.info('Getting template boundaries from trigger file')
 boundaries = trigf[args.ifo + '/template_boundaries'][:]
-
-trigf.close()
-
-# Setup a data mask to remove any triggers with SNR below threshold
-# This works as a pre-filter as SNR is always greater than or equal
-# to sngl_ranking, except in the psdvar case, where it could increase.
-with HFile(args.trigger_file, 'r') as trig_file:
-    n_triggers_orig = trig_file[f'{args.ifo}/snr'].size
-    logging.info("Trigger file has %d triggers", n_triggers_orig)
-    logging.info('Generating trigger mask')
-    if f'{args.ifo}/psd_var_val' in trig_file:
-        idx, _, _ = trig_file.select(
-            lambda snr, psdvar: snr / psdvar ** 0.5 >= args.plot_lower_stat_limit,
-            f'{args.ifo}/snr',
-            f'{args.ifo}/psd_var_val',
-            return_indices=True
-        )
-    else:
-        # psd_var_val may not have been calculated
-        idx, _ = trig_file.select(
-            lambda snr: snr >= args.plot_lower_stat_limit,
-            f'{args.ifo}/snr',
-            return_indices=True
-        )
-    data_mask = np.zeros(n_triggers_orig, dtype=bool)
-    data_mask[idx] = True
-
-
-logging.info('Calculating single stat values from trigger file')
-trigs = SingleDetTriggers(
-    args.trigger_file,
-    None,
-    None,
-    None,
-    None,
-    args.ifo,
-    premask=data_mask
-)
-# This is the direct pointer to the HDF file, used later on
-trigf = trigs.trigs_f
-
-stat = trigs.get_ranking(args.sngl_ranking)
-time = trigs.end_time
-
-
-logging.info('Processing template boundaries')
 max_boundary_id = np.argmax(boundaries)
 sorted_boundary_list = np.sort(boundaries)
 
-# In the two blocks of code that follows we are trying to figure out the index
-# ranges in the masked trigger lists corresponding to the "boundaries".
-# We will do this by walking over the boundaries in the order they're
-# stored in the file, adding in the number of triggers not removed by the
-# mask every time.
-
-# First step is to loop over the "boundaries" which gives the start position
-# of each block of triggers (corresponding to one template) in the full trigger
-# merge file.
-# Here we identify the end_idx for the triggers corresponding to each template.
+logging.info('Processing template boundaries')
 where_idx_end = np.zeros_like(boundaries)
 for idx, idx_start in enumerate(boundaries):
     if idx == max_boundary_id:
         where_idx_end[idx] = trigf[args.ifo + '/end_time'].size
     else:
         where_idx_end[idx] = sorted_boundary_list[
             np.argmax(sorted_boundary_list == idx_start) + 1]
 
-# Next we need to map these start/stop indices in the full file, to the start
-# stop indices in the masked list of triggers. We do this by figuring out
-# how many triggers are in the masked list for each template in the order they
-# are stored in the trigger merge file, and keep a running sum.
-curr_count = 0
-mask_start_idx = np.zeros_like(boundaries)
-mask_end_idx = np.zeros_like(boundaries)
-for idx_start in sorted_boundary_list:
-    boundary_idx = np.argmax(boundaries == idx_start)
-    idx_end = where_idx_end[boundary_idx]
-    mask_start_idx[boundary_idx] = curr_count
-    curr_count += np.sum(trigs.mask[idx_start:idx_end])
-    mask_end_idx[boundary_idx] = curr_count
-
+logging.info('Calculating single stat values from trigger file')
+rank_method = pystat.get_statistic_from_opts(args, [args.ifo])
+stat = rank_method.get_sngl_ranking(trigf[args.ifo])
 
 if args.veto_file:
     logging.info('Applying DQ vetoes')
-    remove, junk = events.veto.indices_within_segments(
-        time,
-        [args.veto_file],
-        ifo=args.ifo,
-        segment_name=args.veto_segment_name
-    )
-    # Set stat to zero for triggers being vetoed: given that the fit threshold
-    # is >0 these will not be fitted or plotted.  Avoids complications from
-    # changing the number of triggers, ie changes of template boundary.
-    stat[remove] = 0.
-    time[remove] = 0.
-    logging.info(
-        '%d out of %d trigs removed after vetoing with %s from %s',
-        remove.size,
-        stat.size,
-        args.veto_segment_name,
-        args.veto_file
-    )
+    time = trigf[args.ifo + '/end_time'][:]
+    remove, junk = events.veto.indices_within_segments(time, [args.veto_file],
+                         ifo=args.ifo, segment_name=args.veto_segment_name)
+    # Set stat to zero for triggers being vetoed: given that the fit threshold is
+    # >0 these will not be fitted or plotted.  Avoids complications from changing
+    # the number of triggers, ie changes of template boundary.
+    stat[remove] = np.zeros_like(remove)
+    time[remove] = np.zeros_like(remove)
+    logging.info('{} out of {} trigs removed after vetoing with {} from {}'.format(
+                      remove.size, stat.size, args.veto_segment_name, args.veto_file))
 
 if args.gating_veto_windows:
     logging.info('Applying veto to triggers near gates')
     gating_veto = args.gating_veto_windows[args.ifo].split(',')
     gveto_before = float(gating_veto[0])
     gveto_after = float(gating_veto[1])
     if gveto_before > 0 or gveto_after < 0:
         raise ValueError("Gating veto window values must be negative before "
                          "gates and positive after gates.")
     if not (gveto_before == 0 and gveto_after == 0):
+        time = trigf[args.ifo + '/end_time'][:]
         autogate_times = np.unique(trigf[args.ifo + '/gating/auto/time'][:])
         if args.ifo + '/gating/file' in trigf:
             detgate_times = trigf[args.ifo + '/gating/file/time'][:]
         else:
             detgate_times = []
         gate_times = np.concatenate((autogate_times, detgate_times))
-        gveto_remove = events.veto.indices_within_times(
-            time,
-            gate_times + gveto_before,
-            gate_times + gveto_after
-        )
-        stat[gveto_remove] = 0.
-        time[gveto_remove] = 0.
-        logging.info(
-            '%d out of %d trigs removed after vetoing triggers near gates',
-            gveto_remove.size,
-            stat.size
-        )
+        gveto_remove = events.veto.indices_within_times(time, gate_times + gveto_before,
+                                                        gate_times + gveto_after)
+        stat[gveto_remove] = np.zeros_like(gveto_remove)
+        time[gveto_remove] = np.zeros_like(gveto_remove)
+        logging.info('{} out of {} trigs removed after vetoing triggers near gates'.format(
+                          gveto_remove.size, stat.size))
 
 for x in range(args.split_one_nbins):
     if not args.prune_number:
         logging.info('Not performing any pruning')
         break
     elif args.prune_number and x == 0:
         logging.info('Applying pruning around loudest triggers in each split')
@@ -352,53 +262,50 @@
         # Finding ids of templates in split
         id_in_both = np.intersect1d(id_bin1, id_bin2)
         if len(id_in_both) == 0: continue
         vals_inbin = []
         time_inbin = []
         # getting triggers that are in these templates
         for idx in id_in_both:
-            vals_inbin += list(stat[mask_start_idx[idx]:mask_end_idx[idx]])
-            time_inbin += list(time[mask_start_idx[idx]:mask_end_idx[idx]])
+            where_idx_start = boundaries[idx]
+            vals_inbin += list(stat[where_idx_start:where_idx_end[idx]])
+            time_inbin += list(time[where_idx_start:where_idx_end[idx]])
 
         vals_inbin = np.array(vals_inbin)
         time_inbin = np.array(time_inbin)
 
         count_pruned = 0
         logging.info('Pruning in split {}-{} {}-{}'.format(
                      args.split_param_one, x, args.split_param_two, y))
-        logging.info('Currently have %d triggers', len(vals_inbin))
         while count_pruned < args.prune_number:
             # Getting loudest statistic value in split
             max_val_arg = vals_inbin.argmax()
             max_statval = vals_inbin[max_val_arg]
 
-            remove = np.nonzero(
-                abs(time_inbin[max_val_arg] - time) < args.prune_window
-            )[0]
+            remove = np.nonzero(abs(time_inbin[max_val_arg] - time)
+                                    < args.prune_window)[0]
             # Remove from inbin triggers as well in case there
             # are more pruning iterations
-            remove_inbin = np.nonzero(
-                abs(time_inbin[max_val_arg] - time_inbin) < args.prune_window
-            )[0]
-            logging.info(
-                'Prune %d: removing %d triggers around %.2f, %d in this split',
-                count_pruned,
-                remove.size,
-                time[max_val_arg],
-                remove_inbin.size
-            )
+            remove_inbin = np.nonzero(abs(time_inbin[max_val_arg] - time_inbin)
+                                      < args.prune_window)[0]
+            logging.info('Prune {}: removing {} triggers around time {:.2f},'
+                         ' {} in this split'.format(count_pruned, remove.size,
+                                                    time[max_val_arg],
+                                                    remove_inbin.size))
             # Set pruned triggers' stat values to zero, as above for vetoes
-            vals_inbin[remove_inbin] = 0.
-            time_inbin[remove_inbin] = 0.
-            stat[remove] = 0.
-            time[remove] = 0.
+            vals_inbin[remove_inbin] = np.zeros_like(remove_inbin)
+            time_inbin[remove_inbin] = np.zeros_like(remove_inbin)
+            stat[remove] = np.zeros_like(remove)
+            time[remove] = np.zeros_like(remove)
             count_pruned += 1
 
+trigf.close()
+
 logging.info('Setting up plotting and fitting limit values')
-minplot = max(stat[np.nonzero(stat)].min(), args.plot_lower_stat_limit)
+minplot = max(stat[np.nonzero(stat)].min(), args.stat_fit_threshold - 1)
 min_fit = max(minplot, args.stat_fit_threshold)
 max_fit = 1.05 * stat.max()
 if args.plot_max_x:
     maxplot = args.plot_max_x
 else:
     maxplot = max_fit
 fitrange = np.linspace(min_fit, max_fit, 100)
@@ -444,15 +351,16 @@
         for i, lower, upper in zip(range(args.num_bins), pbins.lower(),
                                    pbins.upper()):
             indices_all_conditions = np.intersect1d(pidx[i], id_in_both)
             logging.info('{} split {}-{}'.format(args.bin_param, lower, upper))
             if len(indices_all_conditions) == 0: continue
             vals_inbin = []
             for idx in indices_all_conditions:
-                vals_inbin += list(stat[mask_start_idx[idx]:mask_end_idx[idx]])
+                where_idx_start = boundaries[idx]
+                vals_inbin += list(stat[where_idx_start:where_idx_end[idx]])
 
             vals_inbin = np.array(vals_inbin)
             vals_above_thresh = vals_inbin[vals_inbin >= args.stat_fit_threshold]
             if not len(vals_above_thresh):
                 logging.info('No triggers above threshold')
                 continue
             else:
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_followup_file` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_followup_file`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/bin/env python
 """Generate the standardized file detailing the candidates/background to
 follow-up.
 """
 import h5py, numpy, argparse, logging, pycbc
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
     version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--statmap-file',
     help="Statmap file containing the candidates/background to follow up")
 parser.add_argument('--bank-file',
     help="HDF format template bank file")
 parser.add_argument('--min-stat', type=float,
     help="Minimum statistic value to follow up")
 parser.add_argument('--foreground-only', action='store_true',
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_get_loudest_params` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_get_loudest_params`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 """
 
 import lal
 import numpy as np
 import h5py
 import argparse
 import logging
-from pycbc import init_logging
 import pycbc.events
 from pycbc.pnutils import mass1_mass2_to_mchirp_eta
 
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.INFO)
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--single-ifo-trigs', type=str, required=True,
         help='HDF file containing single IFO CBC triggers')
 parser.add_argument('--tmpltbank-file', type=str, required=True,
         help='HDF file containing template information for CBC search')
 parser.add_argument('--ifo', type=str, required=True,
         help='IFO, L1 or H1')
 parser.add_argument('--central-time', type=float, required=True,
@@ -31,16 +29,14 @@
         choices=['snr','newsnr'], help='Ranking statistic to use when searching for loudest events')
 parser.add_argument('--output-file', type=str, required=False,
         help='Output hdf file to write parameters')
 parser.add_argument('--print-params', action='store_true', required=False,
         help='Toggle printing parameters to stdout')
 args = parser.parse_args()
 
-init_logging(args.verbose)
-
 logging.info('Reading in HDF files')
 trigs = h5py.File(args.single_ifo_trigs,'r')
 template_file = h5py.File(args.tmpltbank_file,'r')
 
 if args.output_file:
     outfile = h5py.File(args.output_file,'w')
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_merge_psds` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_merge_psds`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 """ Merge hdf psd files
 """
 import logging, argparse, numpy, h5py, pycbc.types
 from pycbc.version import git_verbose_msg as version
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version', version=version)
+parser.add_argument('--verbose', action="store_true")
 parser.add_argument('--psd-files', nargs='+')
 parser.add_argument("--output-file", required=True)
 
 args = parser.parse_args()
 pycbc.init_logging(args.verbose)
 
 outf = h5py.File(args.output_file, 'w')
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_plot_kde_vals` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_plot_kde_vals`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 #!/usr/bin/env python
 
 import numpy, h5py, argparse, logging
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
-from pycbc import init_logging, add_common_pycbc_options
-import logging
 
 parser = argparse.ArgumentParser(description=__doc__)
-add_common_pycbc_options(parser)
 parser.add_argument('--signal-file')
 parser.add_argument('--template-file', required=True)
 parser.add_argument('--param', nargs='+', required=True,
                     help='Specify one parameter name for a kde_vs_param plot, or '
                          'two parameter names for a param_vs_param plot. Param '
                          'names must exist as datasets in the input files')
 parser.add_argument('--log-axis', nargs='+', choices=['True', 'False'], required=True,
                     help='For each parameter, specify True for a log axis and False '
                          'for a linear axis')
 parser.add_argument('--plot-type', choices=['kde_vs_param', 'param_vs_param'])
 parser.add_argument('--which-kde', choices=['signal_kde', 'template_kde', 'ratio_kde'])
 parser.add_argument('--plot-dir', required=True)
+parser.add_argument('--verbose', action='count')
 args = parser.parse_args()
 
-init_logging(args.verbose)
-
 if args.plot_type == 'kde_vs_param':
     if len(args.param) != 1:
         parser.error('For kde_vs_param, give exactly one parameter name')
 else:
     if len(args.param) != 2:
         parser.error('For param_vs_param, give exactly two parameter names')
 if len(args.param) != len(args.log_axis):
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_reduce_template_bank` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_reduce_template_bank`

 * *Files 11% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 import imp
 import argparse
 import h5py
 import pycbc
 import pycbc.version
 
 parser = argparse.ArgumentParser(description=__doc__)
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument("--version", action="version",
                     version=pycbc.version.git_verbose_msg)
+parser.add_argument("-V", "--verbose", action="store_true",
+                    help="print extra debugging information", default=False)
 parser.add_argument("--input-bank", required=True,
                     help="Input template bank HDF file.")
 parser.add_argument("--output-bank", required=True,
                     help="Output template bank HDF file.")
 parser.add_argument("--filter-func-file", required=True,
                     help="This can be provided to give a function to define "
                          "which points are covered by the template bank "
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_rerank_passthrough` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_rerank_passthrough`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/bin/env python
 """Dummy script to pass through stat files and test reranking"""
 import h5py, numpy, argparse, logging, pycbc
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
+
 parser.add_argument('--version', action='version',
     version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--output-file',
     help="File containing the newly assigned statistic values")
 
 # Options related to getting trigger information from workflow products
 parser.add_argument('--input-file',
     help="HDF File which gives the trigger followup information for a set")
 parser.add_argument('--start-index', type=int,
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_findtrigs` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_findtrigs`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pycbc import io
 from pycbc.events import cuts, trigger_fits as trfits
 from pycbc.events.veto import indices_outside_times
 from pycbc.types.optparse import MultiDetOptionAction
 from pycbc import init_logging
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
+parser.add_argument("--verbose", action='count')
 parser.add_argument("--version", action='version',
                     version=pycbc.version.git_verbose_msg)
 # Basic file input options
 parser.add_argument("--trigger-files", type=str, nargs=1,
                     help="File containing single-detector triggers")
 parser.add_argument("--template-bank", required=True,
                     help="Template bank file in HDF format")
@@ -135,18 +135,18 @@
 
 for tnum in template_ids:
     tids_uncut = trigs.set_template(tnum)
 
     trigger_keep_ids = cuts.apply_trigger_cuts(trigs, trigger_cut_dict,
                                                statistic=rank_method)
     tids_full = tids_uncut[trigger_keep_ids]
-    logging.debug('%s:%s', tnum, len(tids_uncut))
+    logging.info('%s:%s', tnum, len(tids_uncut))
     if len(tids_full) < len(tids_uncut):
-        logging.debug("%s triggers cut",
-                      len(tids_uncut) - len(tids_full))
+        logging.info("%s triggers cut",
+                     len(tids_uncut) - len(tids_full))
 
     n_tot_trigs = tids_full.size
     if not n_tot_trigs: continue
 
     # Stat class instance to calculate the ranking statistic
     sds = rank_method.single(trigs)[trigger_keep_ids]
     stat_t = rank_method.rank_stat_single((ifo, sds),
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_pastro` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_pastro`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     'log': 0.,
     'uniform': 5. / 6.,
     'distancesquared': 5. / 3.,
     'volume': 15. / 6.
 }
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
+parser.add_argument("--verbose", action='count')
 parser.add_argument("--version", action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument("--single-statmap-files", nargs='+', required=True,
                     help="Single statmap files for which p_astro is "
                          "calculated.")
 
 # Files to help remove foreground events
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_statmap` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_statmap`

 * *Files 3% similar despite different names*

```diff
@@ -30,22 +30,22 @@
             self.f[name][:] = data
 
     def __getitem__(self, *args):
         return self.f.__getitem__(*args)
 
 parser = argparse.ArgumentParser()
 # General required options
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--sngls-files', nargs='+',
                     help='List of files containing trigger and statistic '
                          'information.')
 parser.add_argument('--ifos', nargs=1,
                     help='List of ifos used in these coincidence files')
+parser.add_argument('--verbose', action='count')
 parser.add_argument('--cluster-window', type=float, default=10,
                     help='Length of time window in seconds to cluster coinc '
                          'events [default=10s]')
 parser.add_argument('--veto-window', type=float, default=.1,
                     help='Time around each zerolag trigger to window out '
                          '[default=.1s]')
 significance.insert_significance_option_group(parser)
@@ -142,24 +142,16 @@
 bg_far, fg_far = significance.get_far(
     back_stat,
     fore_stat,
     bkg_dec_facs,
     fg_time,
     **significance_dict[ifo])
 
-fg_far = significance.apply_far_limit(
-    fg_far,
-    significance_dict,
-    combo=ifo,
-)
-bg_far = significance.apply_far_limit(
-    bg_far,
-    significance_dict,
-    combo=ifo,
-)
+fg_far = significance.apply_far_limit(fg_far, significance_dict, combo=ifo)
+bg_far = significance.apply_far_limit(bg_far, significance_dict, combo=ifo)
 
 bg_ifar = 1. / bg_far
 fg_ifar = 1. / fg_far
 
 f['background/ifar'] = conv.sec_to_year(bg_ifar)
 
 f.attrs['background_time'] = fg_time
@@ -345,26 +337,14 @@
     bg_far, fg_far = significance.get_far(
         back_stat,
         fore_stat,
         numpy.ones_like(back_stat),
         fg_time,
         **significance_dict[ifo])
 
-    fg_far = significance.apply_far_limit(
-        fg_far,
-        significance_dict,
-        combo=ifo,
-    )
-
-    bg_far = significance.apply_far_limit(
-        bg_far,
-        significance_dict,
-        combo=ifo,
-    )
-
     bg_ifar = 1. / bg_far
     fg_ifar = 1. / fg_far
 
     # Update the ifar_louder criteria depending on whether foreground
     # triggers are being removed via inclusive or exclusive background.
     if is_bkg_inc:
         ifar_louder = fg_ifar
@@ -375,20 +355,14 @@
         _, fg_far_exc = significance.get_far(
             back_stat_exc,
             fore_stat,
             numpy.ones_like(back_stat_exc),
             fg_time_exc,
             **significance_dict[ifo])
 
-        fg_far_exc = significance.apply_far_limit(
-            fg_far_exc,
-            significance_dict,
-            combo=ifo,
-        )
-
         fg_ifar_exc = 1. / fg_far_exc
 
         ifar_louder = fg_ifar_exc
 
     # louder_foreground has been updated and the code can continue.
 
     logging.info("Calculating ifar/fap values")
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_sngls_statmap_inj` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_sngls_statmap_inj`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,25 @@
             self.f[name][:] = data
 
     def __getitem__(self, *args):
         return self.f.__getitem__(*args)
 
 parser = argparse.ArgumentParser()
 # General required options
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--sngls-files', nargs='+',
                     help='List of files containign trigger and statistic '
                          'information.')
 parser.add_argument('--full-data-background', required=True,
                     help='background file from full data for use in analyzing '
                          'injection coincs')
 parser.add_argument('--ifos', nargs=1,
                     help='List of ifos used in these coincidence files')
+parser.add_argument('--verbose', action='count')
 parser.add_argument('--cluster-window', type=float, default=10,
                     help='Length of time window in seconds to cluster coinc '
                          'events [default=10s]')
 parser.add_argument('--veto-window', type=float, default=.1,
                     help='Time around each zerolag trigger to window out '
                          '[default=.1s]')
 significance.insert_significance_option_group(parser)
@@ -113,22 +113,16 @@
 bg_far_exc, fg_far_exc = significance.get_far(
     back_stat_exc,
     fore_stat,
     bkg_exc_dec_facs,
     fg_time_exc,
     **significance_dict[ifo])
 
-fg_far_exc = significance.apply_far_limit(
-    fg_far_exc,
-    significance_dict,
-    combo=ifo)
-bg_far_exc = significance.apply_far_limit(
-    bg_far_exc,
-    significance_dict,
-    combo=ifo)
+fg_far_exc = significance.apply_far_limit(fg_far_exc, significance_dict, combo=ifo)
+bg_far_exc = significance.apply_far_limit(bg_far_exc, significance_dict, combo=ifo)
 
 fg_ifar_exc = 1. / fg_far_exc
 bg_ifar_exc = 1. / bg_far_exc
 
 f['background_exc/ifar'] = conv.sec_to_year(bg_ifar_exc)
 f.attrs['background_time_exc'] = fg_time_exc
 f.attrs['foreground_time_exc'] = fg_time_exc
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_strip_injections` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_strip_injections`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 effd = {"H1":"eff_dist_h", "L1":"eff_dist_l", "V1":"eff_dist_v"}
 def remove(l, i):
     to_remove = [l[t] for t in i]
     for r in to_remove:
         l.remove(r)
 
 parser = argparse.ArgumentParser()
-pycbc.add_common_pycbc_options(parser)
 parser.add_argument('--version', action='version', version=pycbc.version.git_verbose_msg)
+parser.add_argument('--verbose', action='store_true')
 parser.add_argument('--injection-file')
 parser.add_argument('--veto-file', 
                       help="File containing segments used to veto injections")
 parser.add_argument('--segment-name', 
                       help="Name of segmentlist within the veto file to veto injections")
 parser.add_argument('--ifos', nargs='+')
 parser.add_argument('--max-effective-chirp-distance', type=float)
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_template_kde_calc` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_template_kde_calc`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
 # Public License for more details.
 
 import numpy, h5py, operator, argparse, logging
-from pycbc import init_logging, add_common_pycbc_options
+from pycbc import init_logging
 import pycbc.conversions as convert
 from pycbc import libutils
 from pycbc.events import triggers
 akde = libutils.import_optional('awkde')
 kf = libutils.import_optional('sklearn.model_selection')
 
+
 parser = argparse.ArgumentParser(description=__doc__)
-add_common_pycbc_options(parser)
 parser.add_argument('--signal-file', help='File with parameters of GW signals '
                     'for KDE calculation')
 parser.add_argument('--template-file', required=True, help='Hdf5 file with '
                     'template masses and spins')
 parser.add_argument('--injection-file', help='Hdf5 file with masses and spins')
 parser.add_argument('--min-mass', type=float, default=None,
                     help='Used only on signal masses: remove all' 
@@ -60,16 +60,17 @@
                     help='Volume covered by the template bank')
 parser.add_argument('--seed', type=int,
                     help='Random number generator seed')
 parser.add_argument('--mchirp-downsample-power', type=float,
                     help='Exponent value for the power law distribution')
 parser.add_argument('--min-ratio', type=float, 
                     help='Minimum ratio for template_kde relative to the maximum')
+parser.add_argument('--verbose', action='store_true')
 args = parser.parse_args()
-init_logging(args.verbose)
+init_logging(verbose=args.verbose, format='%(asctime)s %(message)s')
 
 
 assert len(args.fit_param) == len(args.log_param)
 if args.make_signal_kde + args.make_template_kde + args.make_injection_kde != 1:
     parser.error("Choose exactly one option out of --make-signal-kde, \
                  --make-template-kde, or --make-injection-kde")
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_template_kde_max` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_template_kde_max`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 import numpy, h5py, argparse, logging
-from pycbc import init_logging, add_common_pycbc_options
+from pycbc import init_logging
 
 parser = argparse.ArgumentParser(description=__doc__)
-add_common_pycbc_options(parser)
 parser.add_argument('--kde-files', nargs='+', required=True,
                     help='HDF files with KDE values')
 parser.add_argument('--output-file', required=True, help='Name of output HDF file')
 parser.add_argument('--min-ratio', type=float,
                     help='Minimum ratio for template_kde relative to the maximum')
+parser.add_argument('--verbose', action='store_true')
 args = parser.parse_args()
-init_logging(args.verbose)
+init_logging(verbose=args.verbose, format='%(asctime)s %(message)s')
 
 
 input_kdes = [h5py.File(kfile, 'r') for kfile in args.kde_files]
 if len(input_kdes) < 2:
     raise ValueError("At least two input files are required.")
```

### Comparing `PyCBC-2.3.6/bin/all_sky_search/pycbc_template_recovery_hist` & `PyCBC-2.4.0/bin/all_sky_search/pycbc_template_recovery_hist`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 """ Histogram of templates where injections are found.
 """
 import logging, h5py, argparse, numpy as np
 from matplotlib import use
 use('Agg')
 from matplotlib import pyplot as plt
 from pycbc.events import triggers
-from pycbc import init_logging, add_common_pycbc_options
 
 parser = argparse.ArgumentParser(description=__doc__)
-add_common_pycbc_options(parser)
+parser.add_argument('--verbose', action='count')
 parser.add_argument('--output', required=True)
 parser.add_argument('--found-injection-files', dest='found', nargs='+',
                     help='hdf file(s) with found injections')
 parser.add_argument('--inspiral-trigger-files', dest='trig', nargs='*',
                     default=[],
                     help='hdf files(s) with injection single-ifo triggers, '
                          'if supplied must be one per found injection file')
@@ -26,15 +25,17 @@
                     help='use log bins in parameter')
 parser.add_argument('--min-stat', type=float,
                     help='only plot injections above given stat value')
 parser.add_argument('--min-ifar', type=float,
                     help='only plot injections above given ifar value')
 args = parser.parse_args()
 
-init_logging(args.verbose)
+if args.verbose:
+    log_level = logging.INFO
+    logging.basicConfig(format='%(asctime)s : %(message)s', level=log_level)
 
 # should be same number of inj and trig files
 # and either 0 or 1 bank files or 1 per inj file
 if not(len(args.trig) == 0 or len(args.trig) == len(args.found)):
     raise RuntimeError('If trigger files are given, must be one per injection '
                        'file!')
 if not(len(args.bank_files) < 2 or len(args.bank_files) == len(args.found)):
```

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_aligned_bank_cat` & `PyCBC-2.4.0/bin/bank/pycbc_aligned_bank_cat`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_aligned_stoch_bank` & `PyCBC-2.4.0/bin/bank/pycbc_aligned_stoch_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_bank_verification` & `PyCBC-2.4.0/bin/bank/pycbc_bank_verification`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_brute_bank` & `PyCBC-2.4.0/bin/bank/pycbc_brute_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_coinc_bank2hdf` & `PyCBC-2.4.0/bin/bank/pycbc_coinc_bank2hdf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_geom_aligned_2dstack` & `PyCBC-2.4.0/bin/bank/pycbc_geom_aligned_2dstack`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_geom_aligned_bank` & `PyCBC-2.4.0/bin/bank/pycbc_geom_aligned_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_geom_nonspinbank` & `PyCBC-2.4.0/bin/bank/pycbc_geom_nonspinbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/bank/pycbc_tmpltbank_to_chi_params` & `PyCBC-2.4.0/bin/bank/pycbc_tmpltbank_to_chi_params`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/hwinj/pycbc_generate_hwinj` & `PyCBC-2.4.0/bin/hwinj/pycbc_generate_hwinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/hwinj/pycbc_generate_hwinj_from_xml` & `PyCBC-2.4.0/bin/hwinj/pycbc_generate_hwinj_from_xml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/hwinj/pycbc_insert_frame_hwinj` & `PyCBC-2.4.0/bin/hwinj/pycbc_insert_frame_hwinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/hwinj/pycbc_plot_hwinj` & `PyCBC-2.4.0/bin/hwinj/pycbc_plot_hwinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference` & `PyCBC-2.4.0/bin/inference/pycbc_inference`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_create_fits` & `PyCBC-2.4.0/bin/inference/pycbc_inference_create_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_extract_samples` & `PyCBC-2.4.0/bin/inference/pycbc_inference_extract_samples`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_model_stats` & `PyCBC-2.4.0/bin/inference/pycbc_inference_model_stats`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_monitor` & `PyCBC-2.4.0/bin/inference/pycbc_inference_monitor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_acceptance_rate` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_acceptance_rate`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_acf` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_acf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_acl` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_acl`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_dynesty_run` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_dynesty_run`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_dynesty_traceplot` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_dynesty_traceplot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_gelman_rubin` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_gelman_rubin`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_geweke` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_geweke`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_inj_recovery` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_inj_recovery`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_mcmc_history` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_mcmc_history`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_movie` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_movie`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_posterior` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_posterior`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_pp` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_pp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_prior` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_prior`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_samples` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_samples`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_skymap` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_skymap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_plot_thermodynamic_integrand` & `PyCBC-2.4.0/bin/inference/pycbc_inference_plot_thermodynamic_integrand`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_pp_table_summary` & `PyCBC-2.4.0/bin/inference/pycbc_inference_pp_table_summary`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_start_from_samples` & `PyCBC-2.4.0/bin/inference/pycbc_inference_start_from_samples`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_inference_table_summary` & `PyCBC-2.4.0/bin/inference/pycbc_inference_table_summary`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/inference/pycbc_validate_test_posterior` & `PyCBC-2.4.0/bin/inference/pycbc_validate_test_posterior`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/live/pycbc_live_combine_single_fits` & `PyCBC-2.4.0/bin/live/pycbc_live_combine_single_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/live/pycbc_live_plot_combined_single_fits` & `PyCBC-2.4.0/bin/live/pycbc_live_plot_combined_single_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/live/pycbc_live_plot_single_trigger_fits` & `PyCBC-2.4.0/bin/live/pycbc_live_plot_single_trigger_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/live/pycbc_live_single_trigger_fits` & `PyCBC-2.4.0/bin/live/pycbc_live_single_trigger_fits`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_foreground_minifollowup` & `PyCBC-2.4.0/bin/minifollowups/pycbc_foreground_minifollowup`

 * *Files 24% similar despite different names*

```diff
@@ -12,22 +12,15 @@
 # Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """ Followup foreground events
 """
-import os
-import sys
-import argparse
-import logging
-import re
-import h5py
-
-import pycbc.workflow as wf
+import os, sys, argparse, logging, re, h5py, pycbc.workflow as wf
 from pycbc.results import layout
 from pycbc.types import MultiDetOptionAction
 from pycbc.events import select_segments_by_definer, coinc
 from pycbc.io import get_all_subkeys
 import pycbc.workflow.minifollowups as mini
 from pycbc.workflow.core import resolve_url_to_file
 import pycbc.version
@@ -106,82 +99,65 @@
 
 num_events = int(workflow.cp.get_opt_tags('workflow-minifollowups', 'num-events', ''))
 f = h5py.File(args.statmap_file, 'r')
 file_val = args.analysis_category
 stat = f['{}/stat'.format(file_val)][:]
 
 if args.sort_variable not in f[file_val]:
-    all_datasets = [re.sub(file_val, '', ds).strip('/')
-                    for ds in get_all_subkeys(f, file_val)]
-    raise KeyError(f'Sort variable {args.sort_variable} not in {file_val}: sort'
-                   f'choices in {file_val} are ' + ', '.join(all_datasets))
-
-# In case we are doing background minifollowup with repeated events,
-# we must include the ordering / template / trigger / time info for
-# _many_ more events to make sure we get enough
+    all_datasets = [re.sub(file_val, '', ds).strip('/') for ds in get_all_subkeys(f, file_val)]
+    raise KeyError('Sort variable {0} not in {1}: sort choices in '
+                   '{1} are {2}'.format(args.sort_variable, file_val,
+                                        ', '.join(all_datasets)))
+
 events_to_read = num_events * 100
 
-# We've asked for more events than there are!
 if len(stat) < num_events:
     num_events = len(stat)
 if len(stat) < events_to_read:
     events_to_read = len(stat)
 
-# Get the indices of the events we are considering in the order specified
 sorting = f[file_val + '/' + args.sort_variable][:].argsort()
 if args.sort_order == 'descending':
     sorting = sorting[::-1]
 event_idx = sorting[0:events_to_read]
 stat = stat[event_idx]
 
-# Save the time / trigger / template ids for the events
 times = {}
 tids = {}
+# Version used for multi-ifo coinc code
 ifo_list = f.attrs['ifos'].split(' ')
-f_cat = f[file_val]
 for ifo in ifo_list:
-    times[ifo] = f_cat[ifo]['time'][:][event_idx]
-    tids[ifo] = f_cat[ifo]['trigger_id'][:][event_idx]
-bank_ids = f_cat['template_id'][:][event_idx]
-f.close()
+    times[ifo] = f['{}/{}/time'.format(file_val,ifo)][:][event_idx]
+    tids[ifo] = f['{}/{}/trigger_id'.format(file_val, ifo)][:][event_idx]
 
 bank_data = h5py.File(args.bank_file, 'r')
 
 # loop over number of loudest events to be followed up
 event_times = {}
 skipped_data = []
 event_count = 0
 curr_idx = -1
 while event_count < num_events and curr_idx < (events_to_read - 1):
     curr_idx += 1
     files = wf.FileList([])
-    duplicate = False
 
-    # Times and trig ids for trigger timeseries plot
     ifo_times_strings = []
     ifo_tids_strings = []
-
-    # Mean time to use as reference for zerolag
-    mtime = coinc.mean_if_greater_than_zero(
-        [times[ifo][curr_idx] for ifo in times])[0]
-
+    duplicate = False
     for ifo in times:
-        plottime = times[ifo][curr_idx]
-        if plottime == -1:  # Ifo is not in coinc
-            # Use mean time instead and don't plot special trigger
-            plottime = mtime
-        else:  # Do plot special trigger
-            ifo_tids_strings += ['%s:%s' % (ifo, tids[ifo][curr_idx])]
-        ifo_times_strings += ['%s:%s' % (ifo, plottime)]
+        ifo_times_string = '%s:%s' % (ifo, times[ifo][curr_idx])
+        ifo_tids_string = '%s:%s' % (ifo, tids[ifo][curr_idx])
+        ifo_times_strings += [ifo_times_string]
+        ifo_tids_strings += [ifo_tids_string]
 
-        # For background do not want to follow up 10 background coincs with the
-        # same event in ifo 1 and different events in ifo 2, so record times
+        # For background do not want to follow up 10 background coincs with
+        # the same event in ifo 1 and different events in ifo 2
         if ifo not in event_times:
             event_times[ifo] = []
-        # Only do this for background coincident triggers & not sentinel time -1
+        # Don't skip coincs in zerolag or due to the sentinel time -1
         if 'background' in args.analysis_category and \
                 times[ifo][curr_idx] != -1 and \
                 int(times[ifo][curr_idx]) in event_times[ifo]:
             skipped_data.append((ifo, int(times[ifo][curr_idx])))
             duplicate = True
             break
 
@@ -195,68 +171,75 @@
 
     event_count += 1
     if skipped_data:
         layouts += (mini.make_skipped_html(
                         workflow,
                         skipped_data,
                         args.output_dir,
-                        tags=[f'SKIP_{event_count}']),)
+                        tags=['SKIP_{}'.format(event_count)]),)
         skipped_data = []
 
-    bank_id = bank_ids[curr_idx]
+    bank_id = f['{}/template_id'.format(file_val)][:][sorting][curr_idx]
 
     layouts += (mini.make_coinc_info(workflow, single_triggers, tmpltbank_file,
                               coinc_file, args.output_dir, n_loudest=curr_idx,
                               sort_order=args.sort_order, sort_var=args.sort_variable,
                               tags=args.tags + [str(event_count)]),)
     files += mini.make_trigger_timeseries(workflow, single_triggers,
                              ifo_times, args.output_dir, special_tids=ifo_tids,
                              tags=args.tags + [str(event_count)])
 
-    params = mini.get_single_template_params(
-        curr_idx,
-        times,
-        bank_data,
-        bank_ids[curr_idx],
-        fsdt,
-        tids
-    )
-
-    _, sngl_tmplt_plots = mini.make_single_template_plots(
-        workflow,
-        insp_segs,
-        args.inspiral_data_read_name,
-        args.inspiral_data_analyzed_name,
-        params,
-        args.output_dir,
-        data_segments=insp_data_seglists,
-        tags=args.tags + [str(event_count)]
-    )
-    files += sngl_tmplt_plots
-
+    params = {}
+    for ifo in times:
+        params['%s_end_time' % ifo] = times[ifo][curr_idx]
+        try:
+            # Only present for precessing case
+            params['u_vals_%s'%ifo] = \
+                                 fsdt[ifo][ifo]['u_vals'][tids[ifo][curr_idx]]
+        except:
+            pass
+
+    params['mass1'] = bank_data['mass1'][bank_id]
+    params['mass2'] = bank_data['mass2'][bank_id]
+    params['spin1z'] = bank_data['spin1z'][bank_id]
+    params['spin2z'] = bank_data['spin2z'][bank_id]
+    params['f_lower'] = bank_data['f_lower'][bank_id]
+    # don't require precessing template info if not present
+    try:
+        params['spin1x'] = bank_data['spin1x'][bank_id]
+        params['spin1y'] = bank_data['spin1y'][bank_id]
+        params['spin2x'] = bank_data['spin2x'][bank_id]
+        params['spin2y'] = bank_data['spin2y'][bank_id]
+        params['inclination'] = bank_data['inclination'][bank_id]
+    except KeyError:
+        pass
+
+    files += mini.make_single_template_plots(workflow, insp_segs,
+                                    args.inspiral_data_read_name,
+                                    args.inspiral_data_analyzed_name, params,
+                                    args.output_dir,
+                                    tags=args.tags + [str(event_count)])
 
     for single in single_triggers:
         time = times[single.ifo][curr_idx]
         if time==-1:
-            # If this detector did not trigger, still make the plot, but use
-            # the average time of detectors which did trigger
             time = coinc.mean_if_greater_than_zero([times[sngl.ifo][curr_idx]
                                                     for sngl in single_triggers])[0]
         for seg in insp_analysed_seglists[single.ifo]:
             if time in seg:
                 files += mini.make_singles_timefreq(workflow, single, tmpltbank_file,
                                 time, args.output_dir,
                                 data_segments=insp_data_seglists[single.ifo],
                                 tags=args.tags + [str(event_count)])
                 files += mini.make_qscan_plot\
                     (workflow, single.ifo, time, args.output_dir,
                      data_segments=insp_data_seglists[single.ifo],
                      tags=args.tags + [str(event_count)])
                 break
         else:
-            logging.info(f'Trigger time {time} is not valid in '
-                         f'{single.ifo}, skipping singles plots')
+            logging.info('Trigger time {} is not valid in {}, ' \
+                         'skipping singles plots'.format(time, single.ifo))
 
     layouts += list(layout.grouper(files, 2))
 
 workflow.save()
 layout.two_column_layout(args.output_dir, layouts)
```

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_injection_minifollowup` & `PyCBC-2.4.0/bin/minifollowups/pycbc_injection_minifollowup`

 * *Files 19% similar despite different names*

```diff
@@ -10,120 +10,28 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
 # Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+""" Followup foreground events """
 
-"""Create a workflow for following up missed loud injections."""
-
-import os
-import argparse
-import logging
-import copy
-import numpy
-import h5py
+import os, argparse, numpy, logging, h5py, copy
 import pycbc.workflow as wf
-import pycbc.workflow.minifollowups as mini
-import pycbc.version
 from pycbc.types import MultiDetOptionAction
 from pycbc.events import select_segments_by_definer, coinc
 from pycbc.results import layout
 from pycbc.detector import Detector
+import pycbc.workflow.minifollowups as mini
 from pycbc.workflow.core import resolve_url_to_file
+import pycbc.version, pycbc.pnutils
 from pycbc.io.hdf import SingleDetTriggers, HFile
 
-
-legal_distance_types = [
-    'decisive_optimal_snr',
-    'comb_optimal_snr',
-    'dec_chirp_distance'
-]
-
-
-def sort_injections(args, inj_group, missed):
-    """Return an array of indices to sort the missed injections from most to
-    least likely to be detected, according to a metric of choice.
-
-    Parameters
-    ----------
-    args : object
-        CLI arguments parsed by argparse. Must have a `distance_type` attribute
-        to specify how to sort, which must be one of the values in
-        `legal_distance_types`.
-    inj_group : h5py group object
-        HDF5 group object containing the injection definition.
-    missed : array
-        Array of indices of missed injections into `inj_group`.
-
-    Returns
-    -------
-    missed_sorted : array
-        Array of indices of missed injections sorted as requested.
-    """
-    if not hasattr(args, 'distance_type'):
-        raise ValueError('Distance type not provided')
-    if args.distance_type not in legal_distance_types:
-        raise ValueError(
-            f'Invalid distance type "{args.distance_type}", '
-            f'allowed types are {", ".join(legal_distance_types)}'
-        )
-
-    if 'optimal_snr' in args.distance_type:
-        optimal_snrs = [
-            inj_group[dsn][:][missed] for dsn in inj_group.keys()
-            if dsn.startswith('optimal_snr_')
-        ]
-        assert optimal_snrs, 'These injections do not have optimal SNRs'
-
-    if args.distance_type == 'decisive_optimal_snr':
-        # descending order of decisive (2nd largest) optimal SNR
-        dec_snr = numpy.array([
-            sorted(snrs)[-2] for snrs in zip(*optimal_snrs)
-        ])
-        if args.maximum_decisive_snr is not None:
-            # By setting to 0, these injections will not be considered
-            dec_snr[dec_snr > args.maximum_decisive_snr] = 0
-        sorter = dec_snr.argsort()[::-1]
-        return missed[sorter]
-
-    if args.distance_type == 'comb_optimal_snr':
-        # descending order of network optimal SNR
-        optimal_snrs = numpy.vstack(optimal_snrs)
-        net_opt_snrs_squared = (optimal_snrs ** 2).sum(axis=0)
-        sorter = net_opt_snrs_squared.argsort()[::-1]
-        return missed[sorter]
-
-    if args.distance_type == 'dec_chirp_distance':
-        # ascending order of decisive (2nd smallest) chirp distance
-        from pycbc.conversions import mchirp_from_mass1_mass2, chirp_distance
-
-        eff_dists = []
-        for ifo in args.single_detector_triggers:
-            eff_dist = Detector(ifo).effective_distance(
-                inj_group['distance'][:][missed],
-                inj_group['ra'][:][missed],
-                inj_group['dec'][:][missed],
-                inj_group['polarization'][:][missed],
-                inj_group['tc'][:][missed],
-                inj_group['inclination'][:][missed]
-            )
-            eff_dists.append(eff_dist)
-        dec_eff_dist = sorted(eff_dists)[-2]
-        mchirp = mchirp_from_mass1_mass2(
-            inj_group['mass1'][:][missed],
-            inj_group['mass2'][:][missed]
-        )
-        dec_chirp_dist = chirp_distance(dec_dist, mchirp)
-        sorter = dec_chirp_dist.argsort()
-        return missed[sorter]
-
-
-parser = argparse.ArgumentParser(description=__doc__)
+parser = argparse.ArgumentParser(description=__doc__[1:])
 parser.add_argument('--version', action='version', version=pycbc.version.git_verbose_msg)
 parser.add_argument('--bank-file',
                     help="HDF format template bank file")
 parser.add_argument('--injection-file',
                     help="HDF format injection results file")
 parser.add_argument('--injection-xml-file',
                     help="XML format injection file")
@@ -145,19 +53,14 @@
 parser.add_argument('--maximum-decisive-snr', type=float, default=None,
                     help="If given, only followup injections where the "
                          "decisive SNR is smaller than this value.")
 parser.add_argument('--nearby-triggers-window', type=float, default=0.05,
                     help="Maximum time difference between the missed "
                          "injection and the loudest SNR nearby trigger to "
                          "display, seconds. Default=0.05")
-parser.add_argument('--distance-type',
-                    required=True,
-                    choices=legal_distance_types,
-                    help="How to sort missed injections from most to least "
-                         "likely to be detected")
 wf.add_workflow_command_line_group(parser)
 wf.add_workflow_settings_cli(parser, include_subdax_opts=True)
 args = parser.parse_args()
 
 logging.basicConfig(format='%(asctime)s:%(levelname)s : %(message)s',
                     level=logging.INFO)
 
@@ -177,46 +80,77 @@
 insp_data_seglists = {}
 insp_analysed_seglists = {}
 for ifo in args.single_detector_triggers:
     fname = args.single_detector_triggers[ifo]
     strig_file = resolve_url_to_file(os.path.abspath(fname),
                                      attrs={'ifos': ifo})
     single_triggers.append(strig_file)
-    insp_data_seglists[ifo] = select_segments_by_definer(
-        args.inspiral_segments,
-        segment_name=args.inspiral_data_read_name,
-        ifo=ifo
-    )
-    insp_analysed_seglists[ifo] = select_segments_by_definer(
-        args.inspiral_segments,
-        segment_name=args.inspiral_data_analyzed_name,
-        ifo=ifo
-    )
+    insp_data_seglists[ifo] = select_segments_by_definer\
+        (args.inspiral_segments, segment_name=args.inspiral_data_read_name,
+         ifo=ifo)
+    insp_analysed_seglists[ifo] = select_segments_by_definer\
+        (args.inspiral_segments, segment_name=args.inspiral_data_analyzed_name,
+         ifo=ifo)
     # NOTE: make_singles_timefreq needs a coalesced set of segments. If this is
     #       being used to determine command-line options for other codes,
     #       please think if that code requires coalesced, or not, segments.
     insp_data_seglists[ifo].coalesce()
     insp_analysed_seglists[ifo].coalesce()
 
 f = h5py.File(args.injection_file, 'r')
-inj_def = f['injections']
 missed = f['missed/after_vetoes'][:]
 if args.ifar_threshold is not None:
     try:  # injections may not have (inclusive) IFAR present
         ifars = f['found_after_vetoes']['ifar'][:]
     except KeyError:
         ifars = f['found_after_vetoes']['ifar_exc'][:]
-        logging.warning('Inclusive IFAR not found, using exclusive')
+        logging.warn('Inclusive IFAR not found, using exclusive')
     lgc_arr = ifars < args.ifar_threshold
     missed = numpy.append(missed,
                           f['found_after_vetoes']['injection_index'][lgc_arr])
 
+num_events = int(workflow.cp.get_opt_tags('workflow-injection_minifollowups', 'num-events', ''))
+
+try:
+    optstrings = [os for os in f['injections'].keys() if \
+                  os.startswith('optimal_snr_')]
+    optimal_snr = [f['injections/%s' % os][:][missed] for os in optstrings]
+    # 2nd largest opt SNR
+    dec_snr = [sorted(snrs)[-2] for snrs in zip(*optimal_snr)]
+    dec_snr = numpy.array(dec_snr)
+
+    if args.maximum_decisive_snr is not None:
+        # By setting to 0, these injections will not be considered
+        dec_snr[dec_snr > args.maximum_decisive_snr] = 0
+    sorting = dec_snr.argsort()
+    sorting = sorting[::-1]  # descending order of dec opt SNR
+except KeyError:
+    # Fall back to effective distance if optimal SNR not available
+    eff_dist = {}
+    for trig in single_triggers:
+        ifo = trig.ifo
+        eff_dist[ifo] = Detector(ifo).effective_distance(
+                             f['injections/distance'][:][missed],
+                             f['injections/ra'][:][missed],
+                             f['injections/dec'][:][missed],
+                             f['injections/polarization'][:][missed],
+                             f['injections/tc'][:][missed],
+                             f['injections/inclination'][:][missed])
+
+    dec_dist = numpy.maximum(eff_dist[single_triggers[0].ifo],
+                             eff_dist[single_triggers[1].ifo])
+    mchirp, eta = pycbc.pnutils.mass1_mass2_to_mchirp_eta(\
+                                              f['injections/mass1'][:][missed],
+                                              f['injections/mass2'][:][missed])
+    dec_chirp_dist = pycbc.pnutils.chirp_distance(dec_dist, mchirp)
+    sorting = dec_chirp_dist.argsort()  # ascending order of dec chirp distance
+
 # Get the trigger SNRs and times
 # But only ones which are within a small window of the missed injection
-missed_inj_times = numpy.sort(inj_def['tc'][:][missed])
+missed_inj_times = numpy.sort(f['injections/tc'][:][missed])
 
 # Note: Adding Earth diameter in light seconds to the window here
 # to allow for different IFO's arrival times of the injection
 safe_window = args.nearby_triggers_window + 0.0425
 
 def nearby_missedinj(endtime, snr):
     """
@@ -250,54 +184,43 @@
         trigger_idx[ifo], trigger_times[ifo], trigger_snrs[ifo] = \
             trig_f.select(
                 nearby_missedinj,
                 f'{ifo}/end_time',
                 f'{ifo}/snr',
                 return_indices=True)
 
-# figure out how many injections to follow up
-num_events = int(workflow.cp.get_opt_tags(
-    'workflow-injection_minifollowups',
-    'num-events',
-    ''
-))
 if len(missed) < num_events:
     num_events = len(missed)
 
-# sort the injections
-missed = sort_injections(args, inj_def, missed)
-
-# loop over sorted missed injections to be followed up
+# loop over loudest events to be followed up
 found_inj_idxes = f['found_after_vetoes/injection_index'][:]
 for num_event in range(num_events):
     files = wf.FileList([])
 
-    injection_index = missed[num_event]
-    time = inj_def['tc'][injection_index]
-    lon = inj_def['ra'][injection_index]
-    lat = inj_def['dec'][injection_index]
+    injection_index = missed[sorting][num_event]
+    time = f['injections/tc'][injection_index]
+    lon = f['injections/ra'][injection_index]
+    lat = f['injections/dec'][injection_index]
 
     ifo_times = ''
     inj_params = {}
     for val in ['mass1', 'mass2', 'spin1z', 'spin2z', 'tc']:
-        inj_params[val] = inj_def[val][injection_index]
+        inj_params[val] = f['injections/%s' %(val,)][injection_index]
     for single in single_triggers:
         ifo = single.ifo
         det = Detector(ifo)
         ifo_time = time + det.time_delay_from_earth_center(lon, lat, time)
         for seg in insp_analysed_seglists[ifo]:
             if ifo_time in seg:
                 break
         else:
             ifo_time = -1.0
 
         ifo_times += ' %s:%s ' % (ifo, ifo_time)
         inj_params[ifo + '_end_time'] = ifo_time
-    all_times = [inj_params[sngl.ifo + '_end_time'] for sngl in single_triggers]
-    inj_params['mean_time'] = coinc.mean_if_greater_than_zero(all_times)[0]
 
     layouts += [(mini.make_inj_info(workflow, injection_file, injection_index, num_event,
                                args.output_dir, tags=args.tags + [str(num_event)])[0],)]
     if injection_index in found_inj_idxes:
         trig_id = numpy.where(found_inj_idxes == injection_index)[0][0]
         layouts += [(mini.make_coinc_info
                      (workflow, single_triggers, tmpltbank_file,
@@ -329,64 +252,61 @@
     files += mini.make_trigger_timeseries(workflow, single_triggers,
                               ifo_times, args.output_dir,
                               tags=args.tags + [str(num_event)])
 
     for single in single_triggers:
         checkedtime = time
         if (inj_params[single.ifo + '_end_time'] == -1.0):
-            checkedtime = inj_params['mean_time']
+            all_times = [inj_params[sngl.ifo + '_end_time'] for sngl in single_triggers]
+            checkedtime = coinc.mean_if_greater_than_zero(all_times)[0]
         for seg in insp_analysed_seglists[single.ifo]:
             if checkedtime in seg:
                 files += mini.make_singles_timefreq(workflow, single, tmpltbank_file,
                                 checkedtime, args.output_dir,
                                 data_segments=insp_data_seglists[single.ifo],
                                 tags=args.tags + [str(num_event)])
                 files += mini.make_qscan_plot\
                     (workflow, single.ifo, checkedtime, args.output_dir,
                      data_segments=insp_data_seglists[single.ifo],
                      injection_file=injection_xml_file,
                      tags=args.tags + [str(num_event)])
                 break
         else:
-            logging.info(
-                'Trigger time %s is not valid in %s, skipping singles plots',
-                checkedtime, single.ifo
-            )
+            logging.info('Trigger time {} is not valid in {}, ' \
+                         'skipping singles plots'.format(checkedtime,
+                                                         single.ifo))
 
-    _, norm_plot = mini.make_single_template_plots(workflow, insp_segs,
+    files += mini.make_single_template_plots(workflow, insp_segs,
                             args.inspiral_data_read_name,
                             args.inspiral_data_analyzed_name, inj_params,
                             args.output_dir, inj_file=injection_xml_file,
                             tags=args.tags+['INJ_PARAMS',str(num_event)],
                             params_str='injection parameters as template, ' +\
                                        'here the injection is made as normal',
                             use_exact_inj_params=True)
-    files += norm_plot
 
-    _, inv_plot = mini.make_single_template_plots(workflow, insp_segs,
+    files += mini.make_single_template_plots(workflow, insp_segs,
                             args.inspiral_data_read_name,
                             args.inspiral_data_analyzed_name, inj_params,
                             args.output_dir, inj_file=injection_xml_file,
                             tags=args.tags + ['INJ_PARAMS_INVERTED',
                                               str(num_event)],
                             params_str='injection parameters as template, ' +\
                                        'here the injection is made inverted',
                             use_exact_inj_params=True)
-    files += inv_plot
 
-    _, noinj_plot = mini.make_single_template_plots(workflow, insp_segs,
+    files += mini.make_single_template_plots(workflow, insp_segs,
                             args.inspiral_data_read_name,
                             args.inspiral_data_analyzed_name, inj_params,
                             args.output_dir, inj_file=injection_xml_file,
                             tags=args.tags + ['INJ_PARAMS_NOINJ',
                                               str(num_event)],
                             params_str='injection parameters, here no ' +\
                                        'injection was actually performed',
                             use_exact_inj_params=True)
-    files += noinj_plot
 
     for curr_ifo in args.single_detector_triggers:
         single_fname = args.single_detector_triggers[curr_ifo]
         hd_sngl = SingleDetTriggers(single_fname, args.bank_file, None, None,
                                     None, curr_ifo)
         end_times = hd_sngl.end_time
         # Use SNR here or NewSNR??
@@ -417,19 +337,19 @@
             # Only present for precessing search
             curr_params['u_vals'] = hd_sngl.u_vals[0]
         except:
             pass
 
         curr_tags = ['TMPLT_PARAMS_%s' %(curr_ifo,)]
         curr_tags += [str(num_event)]
-        _, loudest_plot = mini.make_single_template_plots(workflow, insp_segs,
+        files += mini.make_single_template_plots(workflow, insp_segs,
                                 args.inspiral_data_read_name,
                                 args.inspiral_data_analyzed_name, curr_params,
                                 args.output_dir, inj_file=injection_xml_file,
                                 tags=args.tags + curr_tags,
                                 params_str='loudest template in %s' % curr_ifo )
-        files += loudest_plot
 
     layouts += list(layout.grouper(files, 2))
+    num_event += 1
 
 workflow.save()
 layout.two_column_layout(args.output_dir, layouts)
```

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_page_coincinfo` & `PyCBC-2.4.0/bin/minifollowups/pycbc_page_coincinfo`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_page_injinfo` & `PyCBC-2.4.0/bin/minifollowups/pycbc_page_injinfo`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_page_snglinfo` & `PyCBC-2.4.0/bin/minifollowups/pycbc_page_snglinfo`

 * *Files 1% similar despite different names*

```diff
@@ -134,19 +134,16 @@
 elif args.sngl_ranking == "snr":
     sngl_stat_name = "SNR"
 else:
     sngl_stat_name = args.sngl_ranking
 
 if args.ranking_statistic in ["quadsum", "single_ranking_only"]:
     stat_name = sngl_stat_name
-    stat_name_long = sngl_stat_name
 else:
-    # Name would be too long - just call it ranking statistic
-    stat_name = 'Ranking Statistic'
-    stat_name_long = ' with '.join([args.ranking_statistic, args.sngl_ranking])
+    stat_name = '_with_'.join(ranking_statistic, sngl_ranking)
 
 headers.append(stat_name)
 
 # Signal-glitch discrimators
 data[0].append('%5.2f' % sngl_file.rchisq)
 data[0].append('%i' % sngl_file.get_column('chisq_dof'))
 headers.append("&chi;<sup>2</sup><sub>r</sub>")
@@ -200,15 +197,15 @@
         str(pycbc.results.static_table(data, headers))
 ###############################################################################
 
 # Set up default titles and the captions for the file
 if args.n_loudest:
     title = 'Parameters of single-detector event ranked %s' \
         % (args.n_loudest + 1)
-    caption = 'Parameters of the single-detector event ranked number %s by %s. The figures below show the mini-followup data for this event.' % (args.n_loudest + 1, stat_name_long)
+    caption = 'Parameters of the single-detector event ranked number %s by %s. The figures below show the mini-followup data for this event.' % (args.n_loudest + 1, stat_name)
 else:
     title = 'Parameters of single-detector event'
     caption = 'Parameters of the single-detector event. The figures below show the mini-followup data for this event.'
 
 pycbc.results.save_fig_with_metadata(html, args.output_file, {},
                         cmd = ' '.join(sys.argv),
                         title = args.title if args.title else title,
```

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_plot_chigram` & `PyCBC-2.4.0/bin/minifollowups/pycbc_plot_chigram`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_plot_trigger_timeseries` & `PyCBC-2.4.0/bin/minifollowups/pycbc_plot_trigger_timeseries`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
 # Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
 """ Plot the single detector trigger timeseries """
 import argparse, logging, pycbc.version, pycbc.results, sys
 from pycbc.types import MultiDetOptionAction
 from pycbc.events import ranking
 from pycbc.io import HFile, SingleDetTriggers
 import h5py
 import matplotlib; matplotlib.use('Agg'); import pylab
@@ -88,25 +87,33 @@
 
     any_data = True
     logging.info("Keeping %d triggers in the window", len(idx))
 
     logging.info("Getting %s", args.plot_type)
     rank = ranking.get_sngls_ranking_from_trigs(trigs, args.plot_type)
 
+    if all(rank == 1):
+        # This is the default value to say "downranked beyond consideration"
+        # so skip these events
+        pylab.scatter(-2 * args.window, 0,
+                      color=pycbc.results.ifo_color(ifo),
+                      marker='x',
+                      label=ifo)
+        continue
+
     pylab.scatter(trigs['end_time'] - t, rank,
                   color=pycbc.results.ifo_color(ifo), marker='x',
                   label=ifo)
 
-    min_rank = min(min_rank, rank.min())
+    # Minimum rank which hasn't been set to the default of 1
+    min_rank = min(min_rank, rank[rank > 1].min())
 
     if args.special_trigger_ids:
         special_idx = args.special_trigger_ids[ifo]
-        if special_idx == None:  # No special trigger for this ifo
-            continue
-        elif special_idx not in idx:
+        if special_idx not in idx:
             logging.info("IDX %d not in kept list",
                          args.special_trigger_ids[ifo])
             continue
         special_red_idx = numpy.where(idx == special_idx)[0]
 
         pylab.scatter(trigs.trigs_f[f'{ifo}/end_time'][special_idx] - t,
                       rank[special_red_idx], marker='*', s=50, color='yellow')
@@ -124,14 +131,11 @@
 pylab.legend()
 pylab.grid()
 
 logging.info("Saving figure")
 pycbc.results.save_fig_with_metadata(fig, args.output_file,
             cmd = ' '.join(sys.argv),
             title = 'Single Detector Trigger Timeseries (%s)' % args.plot_type,
-            caption = 'Time series showing the single-detector triggers '
-                      'centered around the time of the trigger of interest. '
-                      'Triggers with ranking 1 have been downweighted beyond '
-                      'consideration, but may still form insignificant '
-                      'events.',
+            caption = 'Time series showing the single detector triggers'
+                      ' centered around the time of the trigger of interest.',
          )
 logging.info("Done!")
```

### Comparing `PyCBC-2.3.6/bin/minifollowups/pycbc_single_template_plot` & `PyCBC-2.4.0/bin/minifollowups/pycbc_single_template_plot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_banksim_plot_eff_fitting_factor` & `PyCBC-2.4.0/bin/plotting/pycbc_banksim_plot_eff_fitting_factor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_banksim_plot_fitting_factors` & `PyCBC-2.4.0/bin/plotting/pycbc_banksim_plot_fitting_factors`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_banksim_table_point_injs` & `PyCBC-2.4.0/bin/plotting/pycbc_banksim_table_point_injs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_create_html_snippet` & `PyCBC-2.4.0/bin/plotting/pycbc_create_html_snippet`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_faithsim_plots` & `PyCBC-2.4.0/bin/plotting/pycbc_faithsim_plots`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_ifar_catalog` & `PyCBC-2.4.0/bin/plotting/pycbc_ifar_catalog`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_mass_area_plot` & `PyCBC-2.4.0/bin/plotting/pycbc_mass_area_plot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_mchirp_plots` & `PyCBC-2.4.0/bin/plotting/pycbc_mchirp_plots`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_banktriggerrate` & `PyCBC-2.4.0/bin/plotting/pycbc_page_banktriggerrate`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_coinc_snrchi` & `PyCBC-2.4.0/bin/plotting/pycbc_page_coinc_snrchi`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_foreground` & `PyCBC-2.4.0/bin/plotting/pycbc_page_foreground`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_foundmissed` & `PyCBC-2.4.0/bin/plotting/pycbc_page_foundmissed`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_ifar` & `PyCBC-2.4.0/bin/plotting/pycbc_page_ifar`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_injtable` & `PyCBC-2.4.0/bin/plotting/pycbc_page_injtable`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_recovery` & `PyCBC-2.4.0/bin/plotting/pycbc_page_recovery`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_segments` & `PyCBC-2.4.0/bin/plotting/pycbc_page_segments`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_segplot` & `PyCBC-2.4.0/bin/plotting/pycbc_page_segplot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_segtable` & `PyCBC-2.4.0/bin/plotting/pycbc_page_segtable`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_sensitivity` & `PyCBC-2.4.0/bin/plotting/pycbc_page_sensitivity`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_snrchi` & `PyCBC-2.4.0/bin/plotting/pycbc_page_snrchi`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_snrifar` & `PyCBC-2.4.0/bin/plotting/pycbc_page_snrifar`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_snrratehist` & `PyCBC-2.4.0/bin/plotting/pycbc_page_snrratehist`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_versioning` & `PyCBC-2.4.0/bin/plotting/pycbc_page_versioning`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_page_vetotable` & `PyCBC-2.4.0/bin/plotting/pycbc_page_vetotable`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_background_coincs` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_background_coincs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_bank_bins` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_bank_bins`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_bank_corner` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_bank_corner`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_dq_flag_likelihood` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_dq_flag_likelihood`

 * *Files 17% similar despite different names*

```diff
@@ -2,87 +2,67 @@
 """ Plot the log likelihood percentiles for a DQ bin
 """
 import sys
 import argparse
 import numpy
 import pycbc
 import h5py
-from matplotlib import use as matplotlib_use
+from matplotlib import use; use('Agg')
 from matplotlib import pyplot
 from pycbc.version import git_verbose_msg as version
 import pycbc.results
-matplotlib_use('Agg')
 
 parser = argparse.ArgumentParser(description=__doc__)
 parser.add_argument('--version', action='version', version=version)
 parser.add_argument('--verbose', action="store_true")
 parser.add_argument("--dq-file", required=True)
-parser.add_argument("--dq-label", required=True)
 parser.add_argument("--ifo", type=str, required=True)
 parser.add_argument("--output-file", required=True)
 args = parser.parse_args()
 
 pycbc.init_logging(args.verbose)
 
 ifo = args.ifo
 
 f = h5py.File(args.dq_file, 'r')
-ifo_grp = f[ifo]
+dq_name = f.attrs['stat'].split('-')[1]
+logrates_grp = f[ifo + '/dq_percentiles']
+bin_names = logrates_grp.keys()
+
+# when using a flag, should have exactly 2 dq bins (off and on)
+# times when the flag was on go to the last dq bin
+for b in bin_names:
+    num_bins = len(logrates_grp[b])
+    assert num_bins == 2, f'Flag should have exactly 2 dq bins, found {num_bins}'
+logrates = [logrates_grp[b][-1] for b in bin_names]
+x = numpy.arange(len(logrates))
 
-dq_states = ifo_grp['dq_segments'].keys()
-bin_names = ifo_grp['bins'].keys()
+ymax = 1.2 * max(logrates)
+color = pycbc.results.ifo_color(ifo)
 
-num_bins = len(bin_names)
-x = numpy.arange(num_bins)
-width = 0.25
-
-dq_states = {
-    0: 'Clean',
-    1: 'DQ Flag',
-    2: 'Autogating',
-}
-
-colors = {
-    0: 'green',
-    1: 'gold',
-    2: 'red'
-}
-
-fig, ax = pyplot.subplots(figsize=(9, 6))
+fig = pyplot.figure(0)
+ax = fig.add_subplot(111)
 ax2 = ax.twinx()
 
-ymax = 1
-ymin = 0.9
-for n, dqstate_name in dq_states.items():
-    dq_rates = numpy.array(
-        [ifo_grp['bins'][b]['dq_rates'][n] for b in bin_names])
-    dq_rates = numpy.maximum(dq_rates, 1)
-    logrates = numpy.log(dq_rates)
-
-    ymax = max(ymax, numpy.max(dq_rates))
-
-    offset = width * (n - 1)
-    ax.bar(x + offset, dq_rates, width, label=dqstate_name, color=colors[n])
-
-ymax = ymax**1.05
-ax.set_ylim(ymin, ymax)
+ax2.bar(x, height=logrates, label=ifo, color=color)
+ax2.set_ylabel('DQ Log Likelihood Penalty')
+ax2.legend(loc='upper left', markerscale=5)
+ax2.set_ylim(0, ymax)
+ax2.grid()
+
+yticks = ax.get_yticks()
+
+ax_ymax = numpy.exp(ymax)
+ax.set_ylim(1, ax_ymax)
+new_ticks = range(0, int(numpy.ceil(numpy.log10(ax_ymax))))
+ax.set_yticks([10**t for t in new_ticks])
+ax.set_ylabel('(Rate during DQ Flag)/(Mean Rate) [Min 1]')
 ax.set_yscale('log')
-ax.set_ylabel('(Trigger rate during DQ state)/(Mean Rate) [Min 1]')
-
+ax.set_xlabel('Template Bin Number')
 ax.set_xticks(x)
-ax.set_xlabel('Template Bin Number (Longer duration -> Lower number)')
-ax.legend()
-ax.grid()
-
-ax2.set_ylabel('DQ Log Likelihood Penalty')
-ax2.set_ylim(numpy.log(ymin), numpy.log(ymax))
 
 # add meta data and save figure
-plot_title = f'{ifo}:{args.dq_label} DQ Trigger Rates'
-
-ax.set_title(plot_title)
-
-plot_caption = 'The log likelihood correction \
-      during during each dq state for each template bin.'
-pycbc.results.save_fig_with_metadata(
-    fig, args.output_file, title=plot_title,
-    caption=plot_caption, cmd=' '.join(sys.argv))
+plot_title = f'{ifo}: {dq_name} flag log likelihood'
+plot_caption = f'The log likelihood correction during during times flagged \
+                by the {dq_name} flag'
+pycbc.results.save_fig_with_metadata(fig, args.output_file, title=plot_title,
+                                     caption=plot_caption, cmd=' '.join(sys.argv))
```

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_dq_likelihood_vs_time` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_dq_likelihood_vs_time`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_dq_percentiles` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_dq_percentiles`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_gate_triggers` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_gate_triggers`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_gating` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_gating`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_hist` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_hist`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_multiifo_dtphase` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_multiifo_dtphase`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_psd_file` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_psd_file`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_psd_timefreq` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_psd_timefreq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_qscan` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_qscan`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_range` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_range`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_range_vs_mtot` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_range_vs_mtot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_singles_timefreq` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_singles_timefreq`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_singles_vs_params` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_singles_vs_params`

 * *Files 10% similar despite different names*

```diff
@@ -80,37 +80,20 @@
 parser.add_argument('--max-y', type=float, help='Optional maximum y value')
 parser.add_argument('--min-z', type=float, help='Optional minimum z value')
 parser.add_argument('--max-z', type=float, help='Optional maximum z value')
 opts = parser.parse_args()
 
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.INFO)
 
-data_mask = None
-if opts.min_snr > 0:
-    with pycbc.io.HFile(opts.single_trig_file, 'r') as trig_file:
-        n_triggers_orig = trig_file[f'{opts.detector}/snr'].size
-        logging.info("Trigger file has %d triggers", n_triggers_orig)
-        logging.info('Generating trigger mask (on SNR)')
-        idx, _ = trig_file.select(
-            lambda snr: snr >= opts.min_snr,
-            f'{opts.detector}/snr',
-            return_indices=True
-        )
-        data_mask = np.zeros(n_triggers_orig, dtype=bool)
-        data_mask[idx] = True
-
-trigs = pycbc.io.SingleDetTriggers(
-    opts.single_trig_file,
-    opts.bank_file,
-    opts.veto_file,
-    opts.segment_name,
-    opts.filter_string,
-    opts.detector,
-    premask=data_mask
-)
+snr_filter = '(self.snr>%f)' % (opts.min_snr) if opts.min_snr > 0. else None 
+filts = [f for f in [snr_filter, opts.filter_string] if f is not None]
+filter_func = ' & '.join(filts) if filts else None
+
+trigs = pycbc.io.SingleDetTriggers(opts.single_trig_file, opts.bank_file,
+                  opts.veto_file, opts.segment_name, filter_func, opts.detector)
 
 x = getattr(trigs, opts.x_var)
 y = getattr(trigs, opts.y_var)
 
 mask = np.ones(len(x), dtype=bool)
 if opts.min_x is not None:
     mask = np.logical_and(mask, x >= opts.min_x)
@@ -121,22 +104,18 @@
 if opts.max_y is not None:
     mask = np.logical_and(mask, y <= opts.max_y)
 x = x[mask]
 y = y[mask]
 
 hexbin_style = {
     'gridsize': opts.grid_size,
+    # hexbin shows bins with *less* than mincnt as blank
+    'mincnt': 0,
     'linewidths': 0.03
 }
-
-# In earlier versions mpl will try to take the max over bins with 0 triggers
-# and fail, unless we tell it to leave these blank by setting mincnt
-if matplotlib.__version__ < '3.8.1':
-    hexbin_style['mincnt'] = 0
-
 if opts.log_x:
     hexbin_style['xscale'] = 'log'
 if opts.log_y:
     hexbin_style['yscale'] = 'log'
 minz = opts.min_z if opts.min_z else 1
 maxz = opts.max_z
 hexbin_style['norm'] = LogNorm(vmin=minz, vmax=maxz)
@@ -154,15 +133,15 @@
     z = trigs.get_ranking(opts.z_var)
 
     z = z[mask]
     min_z = z.min() if opts.min_z is None else opts.min_z
     max_z = z.max() if opts.max_z is None else opts.max_z
     if max_z / min_z > 10:
         cb_style['ticks'] = LogLocator(subs=range(10))
-    hb = ax.hexbin(x, y, C=z, reduce_C_function=np.max, **hexbin_style)
+    hb = ax.hexbin(x, y, C=z, reduce_C_function=max, **hexbin_style)
     fig.colorbar(hb, **cb_style)
 else:
     raise RuntimeError('z_var = %s is not recognized!' % (opts.z_var))
 
 ax.set_xlabel(opts.x_var)
 ax.set_ylabel(opts.y_var)
 ax.set_title(opts.z_var.title() + ' of %s triggers ' % (opts.detector))
```

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_throughput` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_throughput`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_trigrate` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_trigrate`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_vt_ratio` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_vt_ratio`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/plotting/pycbc_plot_waveform` & `PyCBC-2.4.0/bin/plotting/pycbc_plot_waveform`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/population/pycbc_multiifo_pastro` & `PyCBC-2.4.0/bin/population/pycbc_multiifo_pastro`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/population/pycbc_population_plots` & `PyCBC-2.4.0/bin/population/pycbc_population_plots`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/population/pycbc_population_rates` & `PyCBC-2.4.0/bin/population/pycbc_population_rates`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_banksim` & `PyCBC-2.4.0/bin/pycbc_banksim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_banksim_combine_banks` & `PyCBC-2.4.0/bin/pycbc_banksim_combine_banks`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_banksim_match_combine` & `PyCBC-2.4.0/bin/pycbc_banksim_match_combine`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_banksim_skymax` & `PyCBC-2.4.0/bin/pycbc_banksim_skymax`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_coinc_time` & `PyCBC-2.4.0/bin/pycbc_coinc_time`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_compress_bank` & `PyCBC-2.4.0/bin/pycbc_compress_bank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_condition_strain` & `PyCBC-2.4.0/bin/pycbc_condition_strain`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_convertinjfiletohdf` & `PyCBC-2.4.0/bin/pycbc_convertinjfiletohdf`

 * *Files 2% similar despite different names*

```diff
@@ -146,19 +146,15 @@
         for lvk_name, pycbc_name in self.columns_in_pycbc_format():
             if lvk_name == 't_co_gps':
                 # Special case
                 data[pycbc_name] = self.get_coalescence_time()
             elif lvk_name == 't_co_gps_add':
                 continue
             else:
-                lvk_file_dset = self.inj_file[f'{self.subdir}/{lvk_name}']
-                if lvk_file_dset.dtype.char in ['U', 'O']:
-                    data[pycbc_name] = lvk_file_dset[:].astype('S')
-                else:
-                    data[pycbc_name] = lvk_file_dset[:]
+                data[pycbc_name] = self.inj_file[f'{self.subdir}/{lvk_name}'][:]
         return data
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--version', action='version',
                     version=pycbc.version.git_verbose_msg)
 parser.add_argument('--injection-file', required=True,
```

### Comparing `PyCBC-2.3.6/bin/pycbc_copy_output_map` & `PyCBC-2.4.0/bin/pycbc_copy_output_map`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_create_injections` & `PyCBC-2.4.0/bin/pycbc_create_injections`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_data_store` & `PyCBC-2.4.0/bin/pycbc_data_store`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_faithsim` & `PyCBC-2.4.0/bin/pycbc_faithsim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_faithsim_collect_results` & `PyCBC-2.4.0/bin/pycbc_faithsim_collect_results`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_fit_sngl_trigs` & `PyCBC-2.4.0/bin/pycbc_fit_sngl_trigs`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_get_ffinal` & `PyCBC-2.4.0/bin/pycbc_get_ffinal`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_gwosc_segment_query` & `PyCBC-2.4.0/bin/pycbc_gwosc_segment_query`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_hdf5_splitbank` & `PyCBC-2.4.0/bin/pycbc_hdf5_splitbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_hdf_splitinj` & `PyCBC-2.4.0/bin/pycbc_hdf_splitinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_inj_cut` & `PyCBC-2.4.0/bin/pycbc_inj_cut`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_inspiral` & `PyCBC-2.4.0/bin/pycbc_inspiral`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_inspiral_skymax` & `PyCBC-2.4.0/bin/pycbc_inspiral_skymax`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_live` & `PyCBC-2.4.0/bin/pycbc_live`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_live_nagios_monitor` & `PyCBC-2.4.0/bin/pycbc_live_nagios_monitor`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_make_banksim` & `PyCBC-2.4.0/bin/pycbc_make_banksim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_make_faithsim` & `PyCBC-2.4.0/bin/pycbc_make_faithsim`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_make_html_page` & `PyCBC-2.4.0/bin/pycbc_make_html_page`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_make_skymap` & `PyCBC-2.4.0/bin/pycbc_make_skymap`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_merge_inj_hdf` & `PyCBC-2.4.0/bin/pycbc_merge_inj_hdf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_multi_inspiral` & `PyCBC-2.4.0/bin/pycbc_multi_inspiral`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_optimal_snr` & `PyCBC-2.4.0/bin/pycbc_optimal_snr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_optimize_snr` & `PyCBC-2.4.0/bin/pycbc_optimize_snr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_process_sngls` & `PyCBC-2.4.0/bin/pycbc_process_sngls`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_randomize_inj_dist_by_optsnr` & `PyCBC-2.4.0/bin/pycbc_randomize_inj_dist_by_optsnr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_single_template` & `PyCBC-2.4.0/bin/pycbc_single_template`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_source_probability_offline` & `PyCBC-2.4.0/bin/pycbc_source_probability_offline`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_split_inspinj` & `PyCBC-2.4.0/bin/pycbc_split_inspinj`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_splitbank` & `PyCBC-2.4.0/bin/pycbc_splitbank`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_stageout_failed_workflow` & `PyCBC-2.4.0/bin/pycbc_stageout_failed_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_submit_dax` & `PyCBC-2.4.0/bin/pycbc_submit_dax`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pycbc_upload_xml_to_gracedb` & `PyCBC-2.4.0/bin/pycbc_upload_xml_to_gracedb`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_grb_inj_combiner` & `PyCBC-2.4.0/bin/pygrb/pycbc_grb_inj_combiner`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_grb_inj_finder` & `PyCBC-2.4.0/bin/pygrb/pycbc_grb_inj_finder`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_grb_trig_cluster` & `PyCBC-2.4.0/bin/pygrb/pycbc_grb_trig_cluster`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_grb_trig_combiner` & `PyCBC-2.4.0/bin/pygrb/pycbc_grb_trig_combiner`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_make_offline_grb_workflow` & `PyCBC-2.4.0/bin/pygrb/pycbc_make_offline_grb_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_efficiency` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_efficiency`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_grb_info_table` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_grb_info_table`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_minifollowups` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_minifollowups`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_page_tables` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_page_tables`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_chisq_veto` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_chisq_veto`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_coh_ifosnr`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_injs_results` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_injs_results`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_null_stats` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_null_stats`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_skygrid` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_skygrid`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_snr_timeseries` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_snr_timeseries`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_plot_stats_distribution` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_plot_stats_distribution`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/pygrb/pycbc_pygrb_pp_workflow` & `PyCBC-2.4.0/bin/pygrb/pycbc_pygrb_pp_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons` & `PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_combine_injection_comparisons`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison` & `PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_injection_set_comparison`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows` & `PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_found_both_workflows`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow` & `PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_plot_injections_missed_one_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar` & `PyCBC-2.4.0/bin/workflow_comparisons/offline_search/pycbc_plot_vt_ratio_vs_ifar`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_bank_verifier_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_bank_verifier_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_faithsim_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_faithsim_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_inference_inj_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_inference_inj_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_inference_plots_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_inference_plots_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_inference_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_inference_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_offline_search_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_offline_search_workflow`

 * *Files 6% similar despite different names*

```diff
@@ -184,25 +184,29 @@
                                    output_dir, tags=['full_data'])
 
 insps = wf.merge_single_detector_hdf_files(workflow, hdfbank,
                                            insps, output_dir,
                                            tags=['full_data'])
 
 # setup sngl trigger distribution fitting jobs
-# 'statfiles' is list of files used in calculating statistic
+# 'statfiles' is list of files used in calculating coinc statistic
 # 'dqfiles' is the subset of files containing data quality information
 statfiles = []
-
-dqfiles, dqfile_labels = wf.setup_dq_reranking(workflow, insps,
-                                               hdfbank, analyzable_file,
-                                               analyzable_name,
-                                               dq_segment_file,
-                                               output_dir='dq',
-                                               tags=['full_data'])
-statfiles += dqfiles
+dqfiles = []
+dqfile_labels = []
+dq_labels = workflow.cp.get_subsections('workflow-data_quality')
+for dq_label in dq_labels:
+    dq_label_files = wf.setup_dq_reranking(workflow, dq_label, insps, hdfbank,
+                                       analyzable_segs, analyzable_file,
+                                       dq_segment_file,
+                                       output_dir='dq',
+                                       tags=['full_data'])
+    statfiles += dq_label_files
+    dqfiles += dq_label_files
+    dqfile_labels += len(dq_label_files) * [dq_label]
 
 statfiles += wf.setup_trigger_fitting(workflow, insps, hdfbank,
                                       final_veto_file, final_veto_name,
                                       output_dir=output_dir,
                                       tags=['full_data'])
 
 # Set up the multi-ifo coinc jobs
@@ -450,16 +454,15 @@
             continue
         sec_name = 'workflow-sngl_minifollowups-{}'.format(subsec)
         dir_str = workflow.cp.get(sec_name, 'section-header')
         currdir = rdir['single_triggers/{}_{}'.format(curr_ifo, dir_str)]
         wf.setup_single_det_minifollowups\
             (workflow, insp_file, hdfbank, insp_files_seg_file,
              data_analysed_name, trig_generated_name, 'daxes', currdir,
-             statfiles=wf.FileList(statfiles),
-             fg_file=censored_veto, fg_name='closed_box',
+             veto_file=censored_veto, veto_segment_name='closed_box',
              tags=insp_file.tags + [subsec])
 
 ##################### COINC FULL_DATA plots ###################################
 
 # Main results with combined file (we mix open and closed box here, but
 # separate them in the result page)
 
@@ -472,25 +475,14 @@
                                  hdfbank, rdir['open_box_result'],
                                  singles=insps, extension='.html',
                                  tags=combined_bg_file.tags)
 
 fore_xmlall = wf.make_foreground_table(workflow, combined_bg_file,
                     hdfbank, rdir['open_box_result'], singles=insps,
                     extension='.xml', tags=["xmlall"])
-
-if workflow.cp.has_option_tags('workflow-minifollowups',
-                               'prepare-gracedb-uploads', ''):
-    # Need to get absolute path here
-    upload_path = os.path.join(workflow.out_dir, 'upload_data')
-    wf.setup_upload_prep_minifollowups(workflow, combined_bg_file, fore_xmlall,
-                                       full_insps, psd_files, hdfbank, insp_files_seg_file,
-                                       data_analysed_name, trig_generated_name,
-                                       'daxes', upload_path,
-                                       tags=combined_bg_file.tags)
-
 fore_xmlloudest = wf.make_foreground_table(workflow, combined_bg_file,
                     hdfbank, rdir['open_box_result'], singles=insps,
                     extension='.xml', tags=["xmlloudest"])
 
 symlink_result(table, 'open_box_result/significance')
 
 # Set html pages
@@ -557,32 +549,40 @@
     snrifar_summ += closed_page
     layout.two_column_layout(closed_dir, closed_page)
 
 #################### Plotting of data quality results #########################
 
 # DQ log likelihood plots
 for dqf, dql in zip(dqfiles, dqfile_labels):
-    ifo = dqf.ifo
-    outdir = rdir[f'data_quality/{dqf.ifo}_DQ_results']
-
-    # plot rates when flag was on
-    wf.make_dq_flag_trigger_rate_plot(workflow, dqf, dql, outdir, tags=[dql])
-
-    # make table of dq segment info
-    wf.make_dq_segment_table(workflow, dqf, outdir, tags=[dql])
-
-    # plot background bins
-    background_bins = workflow.cp.get_opt_tags(
-        'bin_templates', 'background-bins', tags=[ifo])
-    wf.make_template_plot(workflow, hdfbank, outdir,
-                          bins=background_bins,
-                          tags=[ifo, 'dq_bins'] + bank_tags)
-
-    # make table of template bin info
-    wf.make_template_bin_table(workflow, dqf, outdir, tags=[ifo])
+    dq_type = workflow.cp.get_opt_tags('workflow-data_quality', 'dq-type', tags=[dql])
+    tags = [dql, 'full_data']
+    if dq_type == 'timeseries':
+        # plot rates as function of time
+        outdir = rdir[f'data_quality/{dqf.ifo}_{dql}_trigger_rates']
+        wf.make_dq_timeseries_trigger_rate_plot(workflow, [dqf], outdir,
+                                                tags=tags)
+        # plot rates as function of dq percentile
+        outdir = rdir[f'data_quality/{dqf.ifo}_{dql}_percentiles']
+        wf.make_dq_percentile_plot(workflow, [dqf], outdir, tags=tags)
+    elif dq_type == 'flag':
+        # plot rates when flag was on
+        outdir = rdir[f'data_quality/{dqf.ifo}_{dql}_trigger_rates']
+        wf.make_dq_flag_trigger_rate_plot(workflow, [dqf], outdir, tags=[dql])
+
+# DQ background binning plot
+if workflow.cp.has_option_tags('bin_trigger_rates_dq', 'background-bins',
+                               tags=None):
+    background_bins = workflow.cp.get_opt_tags('bin_trigger_rates_dq',
+                                               'background-bins', tags=None)
+    bank_tags = workflow.cp.get_subsections('plot_bank')
+    if len(bank_tags) == 0:
+        bank_tags = ['bank']
+    for b_tag in bank_tags:
+        wf.make_template_plot(workflow, hdfbank, rdir['data_quality'],
+                              bins=background_bins, tags=['dq_bins', b_tag])
 
 ############################## Setup the injection runs #######################
 
 splitbank_files_inj = wf.setup_splittable_workflow(workflow, [hdfbank],
                                                    out_dir="bank",
                                                    tags=['injections'])
```

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_psd_estimation_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_psd_estimation_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_sbank_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_sbank_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/bin/workflows/pycbc_make_uberbank_workflow` & `PyCBC-2.4.0/bin/workflows/pycbc_make_uberbank_workflow`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/banksim/injection0.xml` & `PyCBC-2.4.0/examples/banksim/injection0.xml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh` & `PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/pycbc_check_esd_saturation.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh` & `PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/pycbc_check_pcal_saturation.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh` & `PyCBC-2.4.0/examples/cal/foton_filter_esd_saturation/run_pcal_saturation_example.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/catalog/data.py` & `PyCBC-2.4.0/examples/catalog/data.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/dataquality/on.py` & `PyCBC-2.4.0/examples/dataquality/on.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/detector/ant.py` & `PyCBC-2.4.0/examples/detector/ant.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/detector/custom.py` & `PyCBC-2.4.0/examples/detector/custom.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/detector/delay.py` & `PyCBC-2.4.0/examples/detector/delay.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/detector/loc.py` & `PyCBC-2.4.0/examples/detector/loc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/distributions/mass_examples.py` & `PyCBC-2.4.0/examples/distributions/mass_examples.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/distributions/mchirp_q_from_uniform_m1m2_example.py` & `PyCBC-2.4.0/examples/distributions/mchirp_q_from_uniform_m1m2_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/distributions/sampling_from_config_example.py` & `PyCBC-2.4.0/examples/distributions/sampling_from_config_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/distributions/spin_examples.py` & `PyCBC-2.4.0/examples/distributions/spin_examples.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/distributions/spin_spatial_distr_example.py` & `PyCBC-2.4.0/examples/distributions/spin_spatial_distr_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/faith/injection0.xml` & `PyCBC-2.4.0/examples/faith/injection0.xml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/filter/chisq.py` & `PyCBC-2.4.0/examples/filter/chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/filter/fir.py` & `PyCBC-2.4.0/examples/filter/fir.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/filter/pass.py` & `PyCBC-2.4.0/examples/filter/pass.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/filter/snr.py` & `PyCBC-2.4.0/examples/filter/snr.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/gw150914/audio.py` & `PyCBC-2.4.0/examples/gw150914/audio.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/gw150914/gw150914_h1_snr.py` & `PyCBC-2.4.0/examples/gw150914/gw150914_h1_snr.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/gw150914/gw150914_shape.py` & `PyCBC-2.4.0/examples/gw150914/gw150914_shape.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/bbh-injection/run.sh` & `PyCBC-2.4.0/examples/inference/bbh-injection/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/bbh-injection/run_test.sh` & `PyCBC-2.4.0/examples/inference/bbh-injection/run_test.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/gw150914/plot.sh` & `PyCBC-2.4.0/examples/inference/gw150914/plot.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/gw150914/run.sh` & `PyCBC-2.4.0/examples/inference/gw150914/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/gw150914/run_test.sh` & `PyCBC-2.4.0/examples/inference/gw150914/run_test.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/hierarchical/run_test.sh` & `PyCBC-2.4.0/examples/inference/hierarchical/run_test.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/lisa_smbhb_inj/plot.sh` & `PyCBC-2.4.0/examples/inference/lisa_smbhb_inj/plot.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/advanced_plot.py` & `PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/advanced_plot.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/lisa_smbhb_ldc/get.sh` & `PyCBC-2.4.0/examples/inference/lisa_smbhb_ldc/get.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/margtime/run.sh` & `PyCBC-2.4.0/examples/inference/margtime/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/margtime/run_inj.sh` & `PyCBC-2.4.0/examples/inference/margtime/run_inj.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/relmarg/run.sh` & `PyCBC-2.4.0/examples/inference/relmarg/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/samplers/run.sh` & `PyCBC-2.4.0/examples/inference/samplers/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inference/single/run_marg.sh` & `PyCBC-2.4.0/examples/inference/single/run_marg.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inspiral/check_GW150914_detection.py` & `PyCBC-2.4.0/examples/inspiral/check_GW150914_detection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/inspiral/run.sh` & `PyCBC-2.4.0/examples/inspiral/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/live/check_results.py` & `PyCBC-2.4.0/examples/live/check_results.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/live/generate_injections.py` & `PyCBC-2.4.0/examples/live/generate_injections.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/live/make_singles_fits_file.py` & `PyCBC-2.4.0/examples/live/make_singles_fits_file.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/live/run.sh` & `PyCBC-2.4.0/examples/live/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/make_skymap/GW170817.sh` & `PyCBC-2.4.0/examples/make_skymap/GW170817.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/make_skymap/simulated_data.sh` & `PyCBC-2.4.0/examples/make_skymap/simulated_data.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/multi_inspiral/check_faceon_faceaway_trigs.py` & `PyCBC-2.4.0/examples/multi_inspiral/check_faceon_faceaway_trigs.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/multi_inspiral/check_gw170817_trigs.py` & `PyCBC-2.4.0/examples/multi_inspiral/check_gw170817_trigs.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/multi_inspiral/faceon_faceaway.sh` & `PyCBC-2.4.0/examples/multi_inspiral/faceon_faceaway.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/multi_inspiral/run.sh` & `PyCBC-2.4.0/examples/multi_inspiral/run.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/noise/frequency.py` & `PyCBC-2.4.0/examples/noise/frequency.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/overlap.py` & `PyCBC-2.4.0/examples/overlap.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/psd/analytic.py` & `PyCBC-2.4.0/examples/psd/analytic.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/psd/estimate.py` & `PyCBC-2.4.0/examples/psd/estimate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/psd/read.py` & `PyCBC-2.4.0/examples/psd/read.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/search/check_job.py` & `PyCBC-2.4.0/examples/search/check_job.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/search/stats.sh` & `PyCBC-2.4.0/examples/search/stats.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/tmpltbank/testAligned.sh` & `PyCBC-2.4.0/examples/tmpltbank/testAligned.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/tmpltbank/testAligned2.sh` & `PyCBC-2.4.0/examples/tmpltbank/testAligned2.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/tmpltbank/testAligned3.sh` & `PyCBC-2.4.0/examples/tmpltbank/testAligned3.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/tmpltbank/testNonspin.sh` & `PyCBC-2.4.0/examples/tmpltbank/testNonspin.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/tmpltbank/testStoch.sh` & `PyCBC-2.4.0/examples/tmpltbank/testStoch.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/tmpltbank/testStoch4.sh` & `PyCBC-2.4.0/examples/tmpltbank/testStoch4.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/add_waveform.py` & `PyCBC-2.4.0/examples/waveform/add_waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/higher_modes.py` & `PyCBC-2.4.0/examples/waveform/higher_modes.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/match_waveform.py` & `PyCBC-2.4.0/examples/waveform/match_waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/plot_detwaveform.py` & `PyCBC-2.4.0/examples/waveform/plot_detwaveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/plot_fd_td.py` & `PyCBC-2.4.0/examples/waveform/plot_fd_td.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/plot_freq.py` & `PyCBC-2.4.0/examples/waveform/plot_freq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/waveform/plot_phase.py` & `PyCBC-2.4.0/examples/waveform/plot_phase.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/data_checker/daily_test.py` & `PyCBC-2.4.0/examples/workflow/data_checker/daily_test.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/data_checker/get_data_example.py` & `PyCBC-2.4.0/examples/workflow/data_checker/get_data_example.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/dayhopecheck/dayhopecheck.py` & `PyCBC-2.4.0/examples/workflow/dayhopecheck/dayhopecheck.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/generic/multilevel_subworkflow_data/simple.py` & `PyCBC-2.4.0/examples/workflow/generic/multilevel_subworkflow_data/simple.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/generic/simple_subworkflow_data/simple.py` & `PyCBC-2.4.0/examples/workflow/generic/simple_subworkflow_data/simple.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh` & `PyCBC-2.4.0/examples/workflow/inference/bbh_inj-dynesty/create_inj_workflow.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh` & `PyCBC-2.4.0/examples/workflow/pygrb/ER7/run_er7_pygrb_offline.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh` & `PyCBC-2.4.0/examples/workflow/pygrb/ER8/run_er8_pygrb_offline.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh` & `PyCBC-2.4.0/examples/workflow/pygrb/ER8/run_er8_pygrb_online.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/examples/workflow/pygrb/S6/run_s6_pygrb.sh` & `PyCBC-2.4.0/examples/workflow/pygrb/S6/run_s6_pygrb.sh`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/__init__.py` & `PyCBC-2.4.0/pycbc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,36 +62,15 @@
         s = f"{t}.{int(record.msecs):03d}"
         timezone = ct.strftime('%z')
         timezone_colon = f"{timezone[:-2]}:{timezone[-2:]}"
         s += timezone_colon
         return s
 
 
-def add_common_pycbc_options(parser):
-    """
-    Common utility to add standard options to each PyCBC executable.
-
-    Parameters
-    ----------
-    parser : argparse.ArgumentParser
-        The argument parser to which the options will be added
-    """
-    group = parser.add_argument_group(
-        title="PyCBC common options",
-        description="Common options for PyCBC executables.",
-    )
-    group.add_argument('-V', '--verbose', action='count', default=0,
-                       help='Add verbosity to logging. Adding the option '
-                            'multiple times makes logging progressively '
-                            'more verbose, e.g. --verbose or -V provides '
-                            'logging at the info level, but -VV or '
-                            '--verbose --verbose provides debug logging.')
-
-def init_logging(verbose=False,
-                 format='%(asctime)s %(levelname)s : %(message)s'):
+def init_logging(verbose=False, format='%(asctime)s %(message)s'):
     """Common utility for setting up logging in PyCBC.
 
     Installs a signal handler such that verbosity can be activated at
     run-time by sending a SIGUSR1 to the process.
 
     Parameters
     ----------
```

### Comparing `PyCBC-2.3.6/pycbc/_version_helper.py` & `PyCBC-2.4.0/pycbc/_version_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,118 +60,118 @@
     # get outputs
     out, _ = p.communicate()
 
     # throw exception if process failed
     if p.returncode != 0 and on_error == 'raise':
         raise GitInvocationError('Failed to run "%s"' % " ".join(command))
 
-    out = out.decode('utf-8').strip()
+    out = out.decode('utf-8')
 
     if returncode:
-        return out, p.returncode
-    return out
+        return out.strip(), p.returncode
+    else:
+        return out.strip()
 
 
 def get_build_name(git_path='git'):
     """Find the username of the current builder
     """
-    name, retcode = call(('git', 'config', 'user.name'), returncode=True)
+    name,retcode = call(('git', 'config', 'user.name'), returncode=True)
     if retcode:
         name = "Unknown User"
-    email, retcode = call(('git', 'config', 'user.email'), returncode=True)
+    email,retcode = call(('git', 'config', 'user.email'), returncode=True)
     if retcode:
         email = ""
-    return f"{name} <{email}>"
+    return "%s <%s>" % (name, email)
 
 
 def get_build_date():
     """Returns the current datetime as the git build date
     """
-    return time.strftime(r'%Y-%m-%d %H:%M:%S +0000', time.gmtime())
+    return time.strftime('%Y-%m-%d %H:%M:%S +0000', time.gmtime())
 
 
 def get_last_commit(git_path='git'):
     """Returns the details of the last git commit
 
     Returns a tuple (hash, date, author name, author e-mail,
     committer name, committer e-mail).
     """
-    hash_, udate, aname, amail, cname, cmail = call((
-        git_path,
-        'log',
-        '-1',
-        r'--pretty=format:%H,%ct,%an,%ae,%cn,%ce'
-    )).split(",")
-    date = time.strftime(r'%Y-%m-%d %H:%M:%S +0000', time.gmtime(float(udate)))
-    author = f'{aname} <{amail}>'
-    committer = f'{cname} <{cmail}>'
+    hash_, udate, aname, amail, cname, cmail = (
+        call((git_path, 'log', '-1',
+              '--pretty=format:%H,%ct,%an,%ae,%cn,%ce')).split(","))
+    date = time.strftime('%Y-%m-%d %H:%M:%S +0000', time.gmtime(float(udate)))
+    author = '%s <%s>' % (aname, amail)
+    committer = '%s <%s>' % (cname, cmail)
     return hash_, date, author, committer
 
 
 def get_git_branch(git_path='git'):
     """Returns the name of the current git branch
     """
     branch_match = call((git_path, 'rev-parse', '--symbolic-full-name', 'HEAD'))
     if branch_match == "HEAD":
         return None
-    return os.path.basename(branch_match)
+    else:
+        return os.path.basename(branch_match)
 
 
 def get_git_tag(hash_, git_path='git'):
     """Returns the name of the current git tag
     """
     tag, status = call((git_path, 'describe', '--exact-match',
                         '--tags', hash_), returncode=True)
     if status == 0:
         return tag
-    return None
-
+    else:
+        return None
 
 def get_num_commits():
     return call(('git', 'rev-list', '--count', 'HEAD'))
 
-
 def get_git_status(git_path='git'):
     """Returns the state of the git working copy
     """
     status_output = subprocess.call((git_path, 'diff-files', '--quiet'))
     if status_output != 0:
         return 'UNCLEAN: Modified working tree'
-    # check index for changes
-    status_output = subprocess.call((git_path, 'diff-index', '--cached',
-                                     '--quiet', 'HEAD'))
-    if status_output != 0:
-        return 'UNCLEAN: Modified index'
-    return 'CLEAN: All modifications committed'
-
+    else:
+        # check index for changes
+        status_output = subprocess.call((git_path, 'diff-index', '--cached',
+                                         '--quiet', 'HEAD'))
+        if status_output != 0:
+            return 'UNCLEAN: Modified index'
+        else:
+            return 'CLEAN: All modifications committed'
 
 def determine_latest_release_version():
     """Query the git repository for the last released version of the code.
     """
     git_path = call(('which', 'git'))
 
     # Get all tags
     tag_list = call((git_path, 'tag')).split('\n')
 
     # Reduce to only versions
-    re_magic = re.compile(r"v\d+\.\d+\.\d+$")
-    tag_list = [t[1:] for t in tag_list if re_magic.match(t)]
+    tag_list = [t[1:] for t in tag_list if t.startswith('v')]
 
-    # find latest version
+    # Determine if indeed a tag and store largest
     latest_version = None
     latest_version_string = None
+    re_magic = re.compile("\d+\.\d+\.\d+$")
     for tag in tag_list:
-        curr_version = distutils.version.StrictVersion(tag)
-        if latest_version is None or curr_version > latest_version:
-            latest_version = curr_version
-            latest_version_string = tag
+        # Is this a version string
+        if re_magic.match(tag):
+            curr_version = distutils.version.StrictVersion(tag)
+            if latest_version is None or curr_version > latest_version:
+                latest_version = curr_version
+                latest_version_string = tag
 
     return latest_version_string
 
-
 def generate_git_version_info():
     """Query the git repository information to generate a version module.
     """
     info = GitInfo()
     git_path = call(('which', 'git'))
 
     # get build info
```

### Comparing `PyCBC-2.3.6/pycbc/bin_utils.py` & `PyCBC-2.4.0/pycbc/bin_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/boundaries.py` & `PyCBC-2.4.0/pycbc/boundaries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/catalog/__init__.py` & `PyCBC-2.4.0/pycbc/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/catalog/catalog.py` & `PyCBC-2.4.0/pycbc/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/conversions.py` & `PyCBC-2.4.0/pycbc/conversions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/coordinates.py` & `PyCBC-2.4.0/pycbc/coordinates.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/cosmology.py` & `PyCBC-2.4.0/pycbc/cosmology.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/detector.py` & `PyCBC-2.4.0/pycbc/detector.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/__init__.py` & `PyCBC-2.4.0/pycbc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/angular.py` & `PyCBC-2.4.0/pycbc/distributions/angular.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/arbitrary.py` & `PyCBC-2.4.0/pycbc/distributions/arbitrary.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/bounded.py` & `PyCBC-2.4.0/pycbc/distributions/bounded.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/constraints.py` & `PyCBC-2.4.0/pycbc/distributions/constraints.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/external.py` & `PyCBC-2.4.0/pycbc/distributions/external.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/fixedsamples.py` & `PyCBC-2.4.0/pycbc/distributions/fixedsamples.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/gaussian.py` & `PyCBC-2.4.0/pycbc/distributions/gaussian.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/joint.py` & `PyCBC-2.4.0/pycbc/distributions/joint.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/mass.py` & `PyCBC-2.4.0/pycbc/distributions/mass.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/power_law.py` & `PyCBC-2.4.0/pycbc/distributions/power_law.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/qnm.py` & `PyCBC-2.4.0/pycbc/distributions/qnm.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/sky_location.py` & `PyCBC-2.4.0/pycbc/distributions/sky_location.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/spins.py` & `PyCBC-2.4.0/pycbc/distributions/spins.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/uniform.py` & `PyCBC-2.4.0/pycbc/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/uniform_log.py` & `PyCBC-2.4.0/pycbc/distributions/uniform_log.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/distributions/utils.py` & `PyCBC-2.4.0/pycbc/distributions/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/dq.py` & `PyCBC-2.4.0/pycbc/dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/coherent.py` & `PyCBC-2.4.0/pycbc/events/coherent.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/coinc.py` & `PyCBC-2.4.0/pycbc/events/coinc.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,21 @@
 from .eventmgr_cython import coincbuffer_numgreater
 from .eventmgr_cython import timecoincidence_constructidxs
 from .eventmgr_cython import timecoincidence_constructfold
 from .eventmgr_cython import timecoincidence_getslideint
 from .eventmgr_cython import timecoincidence_findidxlen
 from .eventmgr_cython import timecluster_cython
 
-logger = logging.getLogger('pycbc.events.coinc')
+# Mapping used in background_bin_from_string to select approximant for
+# duration function, if duration-based binning is used.
+_APPROXIMANT_DURATION_MAP = {
+    'SEOBNRv2duration': 'SEOBNRv2',
+    'SEOBNRv4duration': 'SEOBNRv4',
+    'SEOBNRv5duration': 'SEOBNRv5_ROM'
+}
 
 
 def background_bin_from_string(background_bins, data):
     """ Return template ids for each bin as defined by the format string
 
     Parameters
     ----------
@@ -94,31 +100,31 @@
                                                    data['mass1'], data['mass2'])
             elif bin_type == 'eta':
                 vals = pycbc.pnutils.mass1_mass2_to_mchirp_eta(
                                                    data['mass1'], data['mass2'])[1]
             elif bin_type == 'chi_eff':
                 vals = pycbc.conversions.chi_eff(data['mass1'], data['mass2'],
                                                  data['spin1z'], data['spin2z'])
-            elif bin_type.endswith('Peak'):
+            elif bin_type in ['SEOBNRv2Peak', 'SEOBNRv4Peak']:
                 vals = pycbc.pnutils.get_freq(
                     'f' + bin_type,
                     data['mass1'],
                     data['mass2'],
                     data['spin1z'],
                     data['spin2z']
                 )
                 cached_values[bin_type] = vals
-            elif bin_type.endswith('duration'):
+            elif bin_type in _APPROXIMANT_DURATION_MAP:
                 vals = pycbc.pnutils.get_imr_duration(
                     data['mass1'],
                     data['mass2'],
                     data['spin1z'],
                     data['spin2z'],
                     data['f_lower'],
-                    approximant=bin_type.replace('duration', '')
+                    approximant=_APPROXIMANT_DURATION_MAP[bin_type]
                 )
                 cached_values[bin_type] = vals
             else:
                 raise ValueError('Invalid bin type %s' % bin_type)
 
             sub_locs = member_func(vals)
             sub_locs = numpy.where(sub_locs)[0]
@@ -298,15 +304,15 @@
         #  those for which the first out of fixed/pivot forms a coinc with ifo1
         # - At the 2nd iteration, we are left with triggers for which both
         #  fixed and pivot are coincident with ifo1
         # - If there is more than 1 dependent ifo, ones that were previously
         #  tested against fixed and pivot are now present for testing with new
         #  dependent ifos
         for ifo2 in ids:
-            logger.info('added ifo %s, testing against %s' % (ifo1, ifo2))
+            logging.info('added ifo %s, testing against %s' % (ifo1, ifo2))
             w = win(ifo1, ifo2)
             left = time1.searchsorted(ctimes[ifo2] - w)
             right = time1.searchsorted(ctimes[ifo2] + w)
             # Any times within time1 coincident with the time in ifo2 have
             # indices between 'left' and 'right'
             # 'nz' indexes into times in ifo2 which have coincidences with ifo1
             # times
@@ -315,17 +321,17 @@
                 rlmax = (right - left).max()
             if len(nz[0]) and rlmax > 1:
                 # We expect at most one coincident time in ifo1, assuming
                 #  trigger spacing in ifo1 > time window.
                 # However there are rare corner cases at starts/ends of inspiral
                 #  jobs. For these, arbitrarily keep the first trigger and
                 #  discard the second (and any subsequent ones).
-                logger.warning('Triggers in %s are closer than coincidence '
-                               'window, 1 or more coincs will be discarded. '
-                               'This is a warning, not an error.' % ifo1)
+                logging.warning('Triggers in %s are closer than coincidence '
+                                'window, 1 or more coincs will be discarded. '
+                                'This is a warning, not an error.' % ifo1)
             # identify indices of times in ifo1 that form coincs with ifo2
             dep_ids = left[nz]
             # slide is array of slide ids attached to pivot ifo
             slide = slide[nz]
 
             for ifo in ctimes:
                 # cycle over fixed and pivot & any previous additional ifos
@@ -362,32 +368,32 @@
 
     Returns
     -------
     cindex: numpy.ndarray
         The set of indices corresponding to the surviving coincidences.
     """
     if len(time1) == 0 or len(time2) == 0:
-        logger.info('No coinc triggers in one, or both, ifos.')
+        logging.info('No coinc triggers in one, or both, ifos.')
         return numpy.array([])
 
     if numpy.isfinite(slide):
         # for a time shifted coinc, time1 is greater than time2 by approximately timeslide_id*slide
         # adding this quantity gives a mean coinc time located around time1
         time = (time1 + time2 + timeslide_id * slide) / 2
     else:
         time = 0.5 * (time2 + time1)
 
     tslide = timeslide_id.astype(numpy.longdouble)
     time = time.astype(numpy.longdouble)
 
     span = (time.max() - time.min()) + window * 10
     time = time + span * tslide
-    logger.info('Clustering events over %s s window', window)
+    logging.info('Clustering events over %s s window', window)
     cidx = cluster_over_time(stat, time, window, **kwargs)
-    logger.info('%d triggers remaining', len(cidx))
+    logging.info('%d triggers remaining', len(cidx))
     return cidx
 
 
 def cluster_coincs_multiifo(stat, time_coincs, timeslide_id, slide, window,
                             **kwargs):
     """Cluster coincident events for each timeslide separately, across
     templates, based on the ranking statistic
@@ -408,15 +414,15 @@
     Returns
     -------
     cindex: numpy.ndarray
         The set of indices corresponding to the surviving coincidences
     """
     time_coinc_zip = list(zip(*time_coincs))
     if len(time_coinc_zip) == 0:
-        logger.info('No coincident triggers.')
+        logging.info('No coincident triggers.')
         return numpy.array([])
 
     time_avg_num = []
     #find number of ifos and mean time over participating ifos for each coinc
     for tc in time_coinc_zip:
         time_avg_num.append(mean_if_greater_than_zero(tc))
 
@@ -432,17 +438,17 @@
         time_avg = time_avg + (nifos_minusone * timeslide_id * slide)/num_ifos
 
     tslide = timeslide_id.astype(numpy.longdouble)
     time_avg = time_avg.astype(numpy.longdouble)
 
     span = (time_avg.max() - time_avg.min()) + window * 10
     time_avg = time_avg + span * tslide
-    logger.info('Clustering events over %s s window', window)
+    logging.info('Clustering events over %s s window', window)
     cidx = cluster_over_time(stat, time_avg, window, **kwargs)
-    logger.info('%d triggers remaining', len(cidx))
+    logging.info('%d triggers remaining', len(cidx))
 
     return cidx
 
 
 def mean_if_greater_than_zero(vals):
     """ Calculate mean over numerical values, ignoring values less than zero.
     E.g. used for mean time over coincident triggers when timestamps are set
@@ -496,15 +502,15 @@
     stat = stat[time_sorting]
     time = time[time_sorting]
 
     left = time.searchsorted(time - window)
     right = time.searchsorted(time + window)
     indices = numpy.zeros(len(left), dtype=numpy.uint32)
 
-    logger.debug('%d triggers before clustering', len(time))
+    logging.debug('%d triggers before clustering', len(time))
 
     if method == 'cython':
         j = timecluster_cython(indices, left, right, stat, len(left))
     elif method == 'python':
         # i is the index we are inspecting, j is the next one to save
         i = 0
         j = 0
@@ -536,15 +542,15 @@
             elif max_loc < i:
                 i += 1
     else:
         raise ValueError(f'Do not recognize method {method}')
 
     indices = indices[:j]
 
-    logger.debug('%d triggers remaining', len(indices))
+    logging.debug('%d triggers remaining', len(indices))
     return time_sorting[indices]
 
 
 class MultiRingBuffer(object):
     """Dynamic size n-dimensional ring buffer that can expire elements."""
 
     def __init__(self, num_rings, max_time, dtype, min_buffer_size=16,
@@ -931,17 +937,17 @@
                         mifar = ifar
                         mstat = stat
                         mresult = result
 
         # apply trials factor for the best coinc
         if mresult:
             mresult['foreground/ifar'] = mifar / float(trials)
-            logger.info('Found %s coinc with ifar %s',
-                        mresult['foreground/type'],
-                        mresult['foreground/ifar'])
+            logging.info('Found %s coinc with ifar %s',
+                         mresult['foreground/type'],
+                         mresult['foreground/ifar'])
             return mresult
         # If no coinc, just return one of the results dictionaries. They will
         # all contain the same results (i.e. single triggers) in this case.
         else:
             return coinc_results[0]
 
     @classmethod
@@ -1080,15 +1086,15 @@
         # If this *still* didn't work, no triggers in first set, try next time
         if len(self.singles.keys()) == 0:
             return {}
 
         # convert to single detector trigger values
         # FIXME Currently configured to use pycbc live output
         # where chisq is the reduced chisq and chisq_dof is the actual DOF
-        logger.info("adding singles to the background estimate...")
+        logging.info("adding singles to the background estimate...")
         updated_indices = {}
         for ifo in ifos:
             trigs = results[ifo]
 
             if len(trigs['snr'] > 0):
                 trigsc = copy.copy(trigs)
                 trigsc['chisq'] = trigs['chisq'] * trigs['chisq_dof']
@@ -1236,28 +1242,28 @@
                 trigger_ids[fixed_ifo].append(numpy.zeros(len(c)) - 1)
 
         cstat = numpy.concatenate(cstat)
         template_ids = numpy.concatenate(template_ids).astype(numpy.int32)
         for ifo in valid_ifos:
             trigger_ids[ifo] = numpy.concatenate(trigger_ids[ifo]).astype(numpy.int32)
 
-        logger.info(
+        logging.info(
             "%s: %s background and zerolag coincs",
             ppdets(self.ifos, "-"), len(cstat)
         )
 
         # Cluster the triggers we've found
         # (both zerolag and shifted are handled together)
         num_zerolag = 0
         num_background = 0
         if len(cstat) > 0:
             offsets = numpy.concatenate(offsets)
             ctime0 = numpy.concatenate(ctimes[self.ifos[0]]).astype(numpy.float64)
             ctime1 = numpy.concatenate(ctimes[self.ifos[1]]).astype(numpy.float64)
-            logger.info("Clustering %s coincs", ppdets(self.ifos, "-"))
+            logging.info("Clustering %s coincs", ppdets(self.ifos, "-"))
             cidx = cluster_coincs(cstat, ctime0, ctime1, offsets,
                                   self.timeslide_interval,
                                   self.analysis_block + 2*self.time_window,
                                   method='cython')
             offsets = offsets[cidx]
             zerolag_idx = (offsets == 0)
             bkg_idx = (offsets != 0)
@@ -1332,15 +1338,15 @@
 
         Returns
         -------
         coinc_results: dict of arrays
             A dictionary of arrays containing the coincident results.
         """
         # Let's see how large everything is
-        logger.info(
+        logging.info(
             "%s: %s coincs, %s bytes",
             ppdets(self.ifos, "-"), len(self.coincs), self.coincs.nbytes
         )
 
         # If there are no results just return
         valid_ifos = [k for k in results.keys() if results[k] and k in self.ifos]
         if len(valid_ifos) == 0: return {}
```

### Comparing `PyCBC-2.3.6/pycbc/events/coinc_rate.py` & `PyCBC-2.4.0/pycbc/events/coinc_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 """
 
 import itertools
 import logging
 import numpy
 import pycbc.detector
 
-logger = logging.getLogger('pycbc.events.coinc_rate')
-
 
 def multiifo_noise_lograte(log_rates, slop):
     """
     Calculate the expected rate of noise coincidences for multiple
     combinations of detectors
 
     Parameters
@@ -80,17 +78,17 @@
         for timing error
 
     Returns
     -------
     numpy array
         Expected coincidence rate in the combination, units Hz
     """
-    logger.warning('combination_noise_rate() is liable to numerical '
-                   'underflows, use combination_noise_lograte '
-                   'instead')
+    logging.warning('combination_noise_rate() is liable to numerical '
+                    'underflows, use combination_noise_lograte '
+                    'instead')
     log_rates = {k: numpy.log(r) for (k, r) in rates.items()}
     # exp may underflow
     return numpy.exp(combination_noise_lograte(log_rates, slop))
 
 
 def combination_noise_lograte(log_rates, slop):
     """
```

### Comparing `PyCBC-2.3.6/pycbc/events/cuts.py` & `PyCBC-2.4.0/pycbc/events/cuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 from pycbc.io import hdf
 from pycbc.tmpltbank import bank_conversions as bank_conv
 from pycbc.io import get_chisq_from_file_choice
 
 # Only used to check isinstance:
 from pycbc.io.hdf import ReadByTemplate
 
-logger = logging.getLogger('pycbc.events.cuts')
-
 # sngl_rank_keys are the allowed names of reweighted SNR functions
 sngl_rank_keys = ranking.sngls_ranking_function_dict.keys()
 
 trigger_param_choices = list(sngl_rank_keys)
 trigger_param_choices += [cc + '_chisq' for cc in hdf.chisq_choices]
 trigger_param_choices += ['end_time', 'psd_var_val', 'sigmasq',
                           'sigma_multiple']
@@ -95,32 +93,32 @@
     with a tuple of the function to be used in the cut, and
     the float to compare to.
     Do input checks
     """
     try:
         cut_param, cut_value_str, cut_limit = inputstr.split(':')
     except ValueError as value_e:
-        logger.warning("ERROR: Cut string format not correct, please "
-                       "supply as PARAMETER:VALUE:LIMIT")
+        logging.warning("ERROR: Cut string format not correct, please "
+                        "supply as PARAMETER:VALUE:LIMIT")
         raise value_e
 
     if cut_param.lower() not in choices:
         raise NotImplementedError("Cut parameter " + cut_param.lower() + " "
                                   "not recognised, choose from "
                                   + ", ".join(choices))
     if cut_limit.lower() not in ineq_choices:
         raise NotImplementedError("Cut inequality " + cut_limit.lower() + " "
                                   "not recognised, choose from "
                                   + ", ".join(ineq_choices))
 
     try:
         cut_value = float(cut_value_str)
     except ValueError as value_e:
-        logger.warning("ERROR: Cut value must be convertible into a float, "
-                       "got '%s'.", cut_value_str)
+        logging.warning("ERROR: Cut value must be convertible into a float, "
+                        "got '%s'.", cut_value_str)
         raise value_e
 
     return {(cut_param, ineq_functions[cut_limit]): cut_value}
 
 
 def check_update_cuts(cut_dict, new_cut):
     """
@@ -135,36 +133,36 @@
 
     new_cut: single-entry dictionary
         dictionary to define the new cut which is being considered to add
     """
     new_cut_key = list(new_cut.keys())[0]
     if new_cut_key in cut_dict:
         # The cut has already been called
-        logger.warning("WARNING: Cut parameter %s and function %s have "
-                       "already been used. Utilising the strictest cut.",
-                       new_cut_key[0], new_cut_key[1].__name__)
+        logging.warning("WARNING: Cut parameter %s and function %s have "
+                        "already been used. Utilising the strictest cut.",
+                        new_cut_key[0], new_cut_key[1].__name__)
         # Extract the function and work out which is strictest
         cut_function = new_cut_key[1]
         value_new = list(new_cut.values())[0]
         value_old = cut_dict[new_cut_key]
         if cut_function(value_new, value_old):
             # The new threshold would survive the cut of the
             # old threshold, therefore the new threshold is stricter
             # - update it
-            logger.warning("WARNING: New threshold of %.3f is "
-                           "stricter than old threshold %.3f, "
-                           "using cut at %.3f.",
-                           value_new, value_old, value_new)
+            logging.warning("WARNING: New threshold of %.3f is "
+                            "stricter than old threshold %.3f, "
+                            "using cut at %.3f.",
+                            value_new, value_old, value_new)
             cut_dict.update(new_cut)
         else:
             # New cut would not make a difference, ignore it
-            logger.warning("WARNING: New threshold of %.3f is less "
-                           "strict than old threshold %.3f, using "
-                           "cut at %.3f.",
-                           value_new, value_old, value_old)
+            logging.warning("WARNING: New threshold of %.3f is less "
+                            "strict than old threshold %.3f, using "
+                            "cut at %.3f.",
+                            value_new, value_old, value_old)
     else:
         # This is a new cut - add it
         cut_dict.update(new_cut)
 
 
 def ingest_cuts_option_group(args):
     """
```

### Comparing `PyCBC-2.3.6/pycbc/events/eventmgr.py` & `PyCBC-2.4.0/pycbc/events/eventmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 from pycbc.scheme import schemed
 from pycbc.detector import Detector
 
 from . import coinc, ranking
 
 from .eventmgr_cython import findchirp_cluster_over_window_cython
 
-logger = logging.getLogger('pycbc.events.eventmgr')
-
 @schemed("pycbc.events.threshold_")
 def threshold(series, value):
     """Return list of values and indices values over threshold in series.
     """
     err_msg = "This function is a stub that should be overridden using the "
     err_msg += "scheme. You shouldn't be seeing this error!"
     raise ValueError(err_msg)
@@ -194,15 +192,15 @@
         self.write_performance = False
 
     def save_state(self, tnum_finished, filename):
         """Save the current state of the background buffers"""
         from pycbc.io.hdf import dump_state
 
         self.tnum_finished = tnum_finished
-        logger.info('Writing checkpoint file at template %s', tnum_finished)
+        logging.info('Writing checkpoint file at template %s', tnum_finished)
         fp = h5py.File(filename, 'w')
         dump_state(self, fp, protocol=pickle.HIGHEST_PROTOCOL)
         fp.close()
 
     @staticmethod
     def restore_state(filename):
         """Restore state of the background buffers from a file"""
@@ -212,15 +210,15 @@
         try:
             mgr = load_state(fp)
         except Exception as e:
             fp.close()
             raise e
         fp.close()
         next_template = mgr.tnum_finished + 1
-        logger.info('Restoring with checkpoint at template %s', next_template)
+        logging.info('Restoring with checkpoint at template %s', next_template)
         return mgr.tnum_finished + 1, mgr
 
     @classmethod
     def from_multi_ifo_interface(cls, opt, ifo, column, column_types, **kwds):
         """
         To use this for a single ifo from the multi ifo interface requires
         some small fixing of the opt structure. This does that. As we edit the
@@ -349,43 +347,43 @@
 
     def finalize_template_events(self):
         self.accumulate.append(self.template_events)
         self.template_events = numpy.array([], dtype=self.event_dtype)
 
     def consolidate_events(self, opt, gwstrain=None):
         self.events = numpy.concatenate(self.accumulate)
-        logger.info("We currently have %d triggers", len(self.events))
+        logging.info("We currently have %d triggers", len(self.events))
         if opt.chisq_threshold and opt.chisq_bins:
-            logger.info("Removing triggers with poor chisq")
+            logging.info("Removing triggers with poor chisq")
             self.chisq_threshold(opt.chisq_threshold, opt.chisq_bins,
                                  opt.chisq_delta)
-            logger.info("%d remaining triggers", len(self.events))
+            logging.info("%d remaining triggers", len(self.events))
 
         if opt.newsnr_threshold and opt.chisq_bins:
-            logger.info("Removing triggers with NewSNR below threshold")
+            logging.info("Removing triggers with NewSNR below threshold")
             self.newsnr_threshold(opt.newsnr_threshold)
-            logger.info("%d remaining triggers", len(self.events))
+            logging.info("%d remaining triggers", len(self.events))
 
         if opt.keep_loudest_interval:
-            logger.info("Removing triggers not within the top %s "
-                        "loudest of a %s second interval by %s",
-                        opt.keep_loudest_num, opt.keep_loudest_interval,
-                        opt.keep_loudest_stat)
+            logging.info("Removing triggers not within the top %s "
+                         "loudest of a %s second interval by %s",
+                         opt.keep_loudest_num, opt.keep_loudest_interval,
+                         opt.keep_loudest_stat)
             self.keep_loudest_in_interval\
                 (opt.keep_loudest_interval * opt.sample_rate,
                  opt.keep_loudest_num, statname=opt.keep_loudest_stat,
                  log_chirp_width=opt.keep_loudest_log_chirp_window)
-            logger.info("%d remaining triggers", len(self.events))
+            logging.info("%d remaining triggers", len(self.events))
 
         if opt.injection_window and hasattr(gwstrain, 'injections'):
-            logger.info("Keeping triggers within %s seconds of injection",
-                        opt.injection_window)
+            logging.info("Keeping triggers within %s seconds of injection",
+                         opt.injection_window)
             self.keep_near_injection(opt.injection_window,
                                      gwstrain.injections)
-            logger.info("%d remaining triggers", len(self.events))
+            logging.info("%d remaining triggers", len(self.events))
 
         self.accumulate = [self.events]
 
     def finalize_events(self):
         self.events = numpy.concatenate(self.accumulate)
 
     def make_output_dir(self, outname):
```

### Comparing `PyCBC-2.3.6/pycbc/events/eventmgr_cython.pyx` & `PyCBC-2.4.0/pycbc/events/eventmgr_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/ranking.py` & `PyCBC-2.4.0/pycbc/events/ranking.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/significance.py` & `PyCBC-2.4.0/pycbc/events/significance.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 """
 import logging
 import copy
 import lal
 import numpy as np
 from pycbc.events import trigger_fits as trstats
 
-logger = logging.getLogger('pycbc.events.significance')
-
 
 def count_n_louder(bstat, fstat, dec,
                    **kwargs):  # pylint:disable=unused-argument
     """ Calculate for each foreground event the number of background events
     that are louder than it.
 
     Parameters
@@ -278,16 +276,16 @@
 def positive_float(inp):
     """
     Wrapper around float conversion which ensures that the float must be
     positive or zero
     """
     fl_in = float(inp)
     if fl_in < 0:
-        logger.warning("Value provided to positive_float is less than zero, "
-                       "this is not allowed")
+        logging.warning("Value provided to positive_float is less than zero, "
+                        "this is not allowed")
         raise ValueError
     return fl_in
 
 
 def check_significance_options(args, parser):
     """
     Check the significance group options
@@ -404,16 +402,16 @@
     for argument_key, arg_to_unpack, conv_func in lists_to_unpack:
         for combo_value in arg_to_unpack:
             combo, value = tuple(combo_value.split(':'))
             if combo not in significance_dict:
                 # Allow options for detector combos that are not actually
                 # used/required for a given job. Such options have
                 # no effect, but emit a warning for (e.g.) diagnostic checks
-                logger.warning("Key %s not used by this code, uses %s",
-                               combo, combo_keys)
+                logging.warning("Key %s not used by this code, uses %s",
+                                combo, combo_keys)
                 significance_dict[combo] = copy.deepcopy(_default_opt_dict)
             significance_dict[combo][argument_key] = conv_func(value)
 
     return significance_dict
 
 
 def apply_far_limit(far, significance_dict, combo=None):
@@ -440,26 +438,26 @@
     """
     far_out = copy.deepcopy(far)
     if isinstance(combo, str):
         # Single IFO combo used
         if significance_dict[combo]['far_limit'] == 0:
             return far_out
         far_limit_str = f"{significance_dict[combo]['far_limit']:.3e}"
-        logger.info("Applying FAR limit of %s to %s events",
-                    far_limit_str, combo)
+        logging.info("Applying FAR limit of %s to %s events",
+                     far_limit_str, combo)
         far_out = np.maximum(far, significance_dict[combo]['far_limit'])
     else:
         # IFO combo supplied as an array, by e.g. pycbc_add_statmap
         # Need to check which events are in which IFO combo in order to
         # apply the right limit to each
         for ifo_combo in significance_dict:
             if significance_dict[ifo_combo]['far_limit'] == 0:
                 continue
             far_limit_str = f"{significance_dict[ifo_combo]['far_limit']:.3e}"
-            logger.info("Applying FAR limit of %s to %s events",
-                        far_limit_str, ifo_combo)
+            logging.info("Applying FAR limit of %s to %s events",
+                         far_limit_str, ifo_combo)
             this_combo_idx = combo == ifo_combo.encode('utf-8')
             far_out[this_combo_idx] = np.maximum(
                 far[this_combo_idx],
                 significance_dict[ifo_combo]['far_limit']
             )
     return far_out
```

### Comparing `PyCBC-2.3.6/pycbc/events/simd_threshold_ccode.cpp` & `PyCBC-2.4.0/pycbc/events/simd_threshold_ccode.cpp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/simd_threshold_cython.pyx` & `PyCBC-2.4.0/pycbc/events/simd_threshold_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/single.py` & `PyCBC-2.4.0/pycbc/events/single.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import h5py
 import numpy as np
 from pycbc.events import ranking, trigger_fits as fits
 from pycbc.types import MultiDetOptionAction
 from pycbc import conversions as conv
 from pycbc import bin_utils
 
-logger = logging.getLogger('pycbc.events.single')
-
 
 class LiveSingle(object):
     def __init__(self, ifo,
                  newsnr_threshold=10.0,
                  reduced_chisq_threshold=5,
                  duration_threshold=0,
                  fit_file=None,
@@ -196,28 +194,28 @@
         }
         candidate['foreground/stat'] = nsnr
         candidate['foreground/ifar'] = ifar
         candidate['HWINJ'] = data_reader.near_hwinj()
         return candidate
 
     def calculate_ifar(self, sngl_ranking, duration):
-        logger.info("Calculating IFAR")
+        logging.info("Calculating IFAR")
         if self.fixed_ifar and self.ifo in self.fixed_ifar:
             return self.fixed_ifar[self.ifo]
 
         try:
             with h5py.File(self.fit_file, 'r') as fit_file:
                 bin_edges = fit_file['bins_edges'][:]
                 live_time = fit_file[self.ifo].attrs['live_time']
                 thresh = fit_file.attrs['fit_threshold']
                 dist_grp = fit_file[self.ifo][self.sngl_ifar_est_dist]
                 rates = dist_grp['counts'][:] / live_time
                 coeffs = dist_grp['fit_coeff'][:]
         except FileNotFoundError:
-            logger.error(
+            logging.error(
                 'Single fit file %s not found; '
                 'dropping a potential single-detector candidate!',
                 self.fit_file
             )
             return None
 
         bins = bin_utils.IrregularBins(bin_edges)
```

### Comparing `PyCBC-2.3.6/pycbc/events/stat.py` & `PyCBC-2.4.0/pycbc/events/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 import numpy
 import h5py
 from . import ranking
 from . import coinc_rate
 from .eventmgr_cython import logsignalrateinternals_computepsignalbins
 from .eventmgr_cython import logsignalrateinternals_compute2detrate
 
-logger = logging.getLogger('pycbc.events.stat')
-
 
 class Stat(object):
     """Base class which should be extended to provide a coincident statistic"""
 
     def __init__(self, sngl_ranking, files=None, ifos=None, **kwargs):
         """
         Create a statistic class instance
@@ -62,15 +60,15 @@
             with h5py.File(filename, 'r') as f:
                 stat = f.attrs['stat']
             if hasattr(stat, 'decode'):
                 stat = stat.decode()
             if stat in self.files:
                 raise RuntimeError("We already have one file with stat attr ="
                                    " %s. Can't provide more than one!" % stat)
-            logger.info("Found file %s for stat %s", filename, stat)
+            logging.info("Found file %s for stat %s", filename, stat)
             self.files[stat] = filename
 
         # Provide the dtype of the single detector method's output
         # This is used by background estimation codes that need to maintain
         # a buffer of such values.
         self.single_dtype = numpy.float32
         # True if a larger single detector statistic will produce a larger
@@ -209,29 +207,26 @@
         return self.get_sngl_ranking(trigs)
 
     def rank_stat_single(self, single_info,
                          **kwargs): # pylint:disable=unused-argument
         """
         Calculate the statistic for a single detector candidate
 
-        For this statistic this is just passing through the
-        single value, which will be the second entry in the tuple.
-
         Parameters
         ----------
         single_info: tuple
             Tuple containing two values. The first is the ifo (str) and the
             second is the single detector triggers.
 
         Returns
         -------
         numpy.ndarray
             The array of single detector statistics
         """
-        return single_info[1]
+        return self.single(single_info[1])
 
     def rank_stat_coinc(self, sngls_list, slide, step, to_shift,
                         **kwargs): # pylint:disable=unused-argument
         """
         Calculate the coincident detection statistic.
 
         Parameters
@@ -379,24 +374,24 @@
                     continue
                 selected = name
                 break
 
         if selected is None and len(ifos) > 1:
             raise RuntimeError("Couldn't figure out which stat file to use")
 
-        logger.info("Using signal histogram %s for ifos %s", selected, ifos)
+        logging.info("Using signal histogram %s for ifos %s", selected, ifos)
         weights = {}
         param = {}
 
         with h5py.File(self.files[selected], 'r') as histfile:
             self.hist_ifos = histfile.attrs['ifos']
 
             # Patch for pre-hdf5=3.0 histogram files
             try:
-                logger.info("Decoding hist ifos ..")
+                logging.info("Decoding hist ifos ..")
                 self.hist_ifos = [i.decode('UTF-8') for i in self.hist_ifos]
             except (UnicodeDecodeError, AttributeError):
                 pass
 
             # Histogram bin attributes
             self.twidth = histfile.attrs['twidth']
             self.pwidth = histfile.attrs['pwidth']
@@ -664,29 +659,26 @@
         return numpy.array(singles, ndmin=1)
 
     def rank_stat_single(self, single_info,
                          **kwargs): # pylint:disable=unused-argument
         """
         Calculate the statistic for a single detector candidate
 
-        For this statistic this is just passing through the
-        single value, which will be the second entry in the tuple.
-
         Parameters
         ----------
         single_info: tuple
             Tuple containing two values. The first is the ifo (str) and the
             second is the single detector triggers.
 
         Returns
         -------
         numpy.ndarray
             The array of single detector statistics
         """
-        return single_info[1]
+        return self.single(single_info[1])
 
     def rank_stat_coinc(self, sngls_list, slide, step, to_shift,
                         **kwargs):  # pylint:disable=unused-argument
         """
         Calculate the coincident detection statistic, defined in Eq 2 of
         [Nitz et al, 2017](https://doi.org/10.3847/1538-4357/aa8f50).
         """
@@ -1994,26 +1986,32 @@
             attribute which is used to associate them with the appropriate
             statistic class.
         ifos: list of strs, not used here
             The list of detector names
         """
         ExpFitFgBgNormStatistic.__init__(self, sngl_ranking, files=files,
                                          ifos=ifos, **kwargs)
-        self.dq_rates_by_state = {}
-        self.dq_bin_by_tid = {}
-        self.dq_state_segments = {}
-
-        for ifo in self.ifos:
-            key = f'{ifo}-dq_stat_info'
-            if key in self.files.keys():
-                self.dq_rates_by_state[ifo] = self.assign_dq_rates(key)
-                self.dq_bin_by_tid[ifo] = self.assign_template_bins(key)
-                self.dq_state_segments[ifo] = self.setup_segments(key)
+        self.dq_val_by_time = {}
+        self.dq_bin_by_id = {}
+        for k in self.files.keys():
+            parsed_attrs = k.split('-')
+            if len(parsed_attrs) < 3:
+                continue
+            if parsed_attrs[2] == 'dq_ts_reference':
+                ifo = parsed_attrs[0]
+                dq_type = parsed_attrs[1]
+                dq_vals = self.assign_dq_val(k)
+                dq_bins = self.assign_bin_id(k)
+                if ifo not in self.dq_val_by_time:
+                    self.dq_val_by_time[ifo] = {}
+                    self.dq_bin_by_id[ifo] = {}
+                self.dq_val_by_time[ifo][dq_type] = dq_vals
+                self.dq_bin_by_id[ifo][dq_type] = dq_bins
 
-    def assign_template_bins(self, key):
+    def assign_bin_id(self, key):
         """
         Assign bin ID values
         Assign each template id to a bin name based on a
         referenced statistic file.
 
         Parameters
         ----------
@@ -2023,26 +2021,26 @@
         Returns
         ---------
         bin_dict: dict of strs
             Dictionary containing the bin name for each template id
         """
         ifo = key.split('-')[0]
         with h5py.File(self.files[key], 'r') as dq_file:
-            tids = []
-            bin_nums = []
-            bin_grp = dq_file[f'{ifo}/bins']
-            for bin_name in bin_grp.keys():
-                bin_tids = bin_grp[f'{bin_name}/tids'][:]
-                tids = list(tids) + list(bin_tids.astype(int))
-                bin_nums = list(bin_nums) + list([bin_name] * len(bin_tids))
+            bin_names = dq_file.attrs['names'][:]
+            locs = []
+            names = []
+            for bin_name in bin_names:
+                bin_locs = dq_file[ifo + '/locs/' + bin_name][:]
+                locs = list(locs) + list(bin_locs.astype(int))
+                names = list(names) + list([bin_name] * len(bin_locs))
 
-        bin_dict = dict(zip(tids, bin_nums))
+        bin_dict = dict(zip(locs, names))
         return bin_dict
 
-    def assign_dq_rates(self, key):
+    def assign_dq_val(self, key):
         """
         Assign dq values to each time for every bin based on a
         referenced statistic file.
 
         Parameters
         ----------
         key: str
@@ -2053,116 +2051,66 @@
         dq_dict: dict of {time: dq_value} dicts for each bin
             Dictionary containing the mapping between the time
             and the dq value for each individual bin.
 
         """
         ifo = key.split('-')[0]
         with h5py.File(self.files[key], 'r') as dq_file:
-            bin_grp = dq_file[f'{ifo}/bins']
+            times = dq_file[ifo + '/times'][:]
+            bin_names = dq_file.attrs['names'][:]
             dq_dict = {}
-            for bin_name in bin_grp.keys():
-                dq_dict[bin_name] = bin_grp[f'{bin_name}/dq_rates'][:]
+            for bin_name in bin_names:
+                dq_vals = dq_file[ifo + '/dq_vals/' + bin_name][:]
+                dq_dict[bin_name] = dict(zip(times, dq_vals))
 
         return dq_dict
 
-    def setup_segments(self, key):
-        """
-        Check if segments definitions are in stat file
-        If they are, we are running offline and need to store them
-        If they aren't, we are running online
-        """
-        ifo = key.split('-')[0]
-        with h5py.File(self.files[key], 'r') as dq_file:
-            ifo_grp = dq_file[ifo]
-            dq_state_segs_dict = {}
-            for k in ifo_grp['dq_segments'].keys():
-                seg_dict = {}
-                seg_dict['start'] = \
-                    ifo_grp[f'dq_segments/{k}/segment_starts'][:]
-                seg_dict['end'] = \
-                    ifo_grp[f'dq_segments/{k}/segment_ends'][:]
-                dq_state_segs_dict[k] = seg_dict
-
-        return dq_state_segs_dict
-
-    def find_dq_noise_rate(self, trigs, dq_state):
-        """Get dq values for a specific ifo and dq states"""
-
+    def find_dq_val(self, trigs):
+        """Get dq values for a specific ifo and times"""
+        time = trigs['end_time'].astype(int)
         try:
             tnum = trigs.template_num
-        except AttributeError:
-            tnum = trigs['template_id']
-
-        try:
             ifo = trigs.ifo
         except AttributeError:
-            ifo = trigs['ifo']
-            assert len(numpy.unique(ifo)) == 1
+            tnum = trigs['template_id']
+            assert len(self.ifos) == 1
             # Should be exactly one ifo provided
-            ifo = ifo[0]
-
-        dq_val = numpy.zeros(len(dq_state))
-
-        if ifo in self.dq_rates_by_state:
-            for (i, st) in enumerate(dq_state):
-                if isinstance(tnum, numpy.ndarray):
-                    bin_name = self.dq_bin_by_tid[ifo][tnum[i]]
-                else:
-                    bin_name = self.dq_bin_by_tid[ifo][tnum]
-                dq_val[i] = self.dq_rates_by_state[ifo][bin_name][st]
+            ifo = self.ifos[0]
+        dq_val = numpy.zeros(len(time))
+        if ifo in self.dq_val_by_time:
+            for (i, t) in enumerate(time):
+                for k in self.dq_val_by_time[ifo].keys():
+                    if isinstance(tnum, numpy.ndarray):
+                        bin_name = self.dq_bin_by_id[ifo][k][tnum[i]]
+                    else:
+                        bin_name = self.dq_bin_by_id[ifo][k][tnum]
+                    val = self.dq_val_by_time[ifo][k][bin_name][int(t)]
+                    dq_val[i] = max(dq_val[i], val)
         return dq_val
 
-    def find_dq_state_by_time(self, ifo, times):
-        """Get the dq state for an ifo at times"""
-        dq_state = numpy.zeros(len(times), dtype=numpy.uint8)
-        if ifo in self.dq_state_segments:
-            from pycbc.events.veto import indices_within_times
-            for k in self.dq_state_segments[ifo]:
-                starts = self.dq_state_segments[ifo][k]['start']
-                ends = self.dq_state_segments[ifo][k]['end']
-                inds = indices_within_times(times, starts, ends)
-                # states are named in file as 'dq_state_N', need to extract N
-                dq_state[inds] = int(k[9:])
-        return dq_state
-
     def lognoiserate(self, trigs):
         """
         Calculate the log noise rate density over single-ifo ranking
 
         Read in single trigger information, compute the ranking
         and rescale by the fitted coefficients alpha and rate
 
         Parameters
         -----------
         trigs: dict of numpy.ndarrays, h5py group or similar dict-like object
             Object holding single detector trigger information.
 
         Returns
         ---------
-        lognoiserate: numpy.array
+        lognoisel: numpy.array
             Array of log noise rate density for each input trigger.
         """
-
-        # make sure every trig has a dq state
-
-        try:
-            ifo = trigs.ifo
-        except AttributeError:
-            ifo = trigs['ifo']
-            assert len(numpy.unique(ifo)) == 1
-            # Should be exactly one ifo provided
-            ifo = ifo[0]
-
-        dq_state = self.find_dq_state_by_time(ifo, trigs['end_time'][:])
-        dq_rate = self.find_dq_noise_rate(trigs, dq_state)
-        dq_rate = numpy.maximum(dq_rate, 1)
-
         logr_n = ExpFitFgBgNormStatistic.lognoiserate(
                     self, trigs)
-        logr_n += numpy.log(dq_rate)
+        logr_n += self.find_dq_val(trigs)
         return logr_n
 
 
 class DQExpFitFgBgKDEStatistic(DQExpFitFgBgNormStatistic):
     """
     The ExpFitFgBgKDEStatistic with DQ-based reranking.
```

### Comparing `PyCBC-2.3.6/pycbc/events/threshold_cpu.py` & `PyCBC-2.4.0/pycbc/events/threshold_cpu.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/threshold_cuda.py` & `PyCBC-2.4.0/pycbc/events/threshold_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/trigger_fits.py` & `PyCBC-2.4.0/pycbc/events/trigger_fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
 # Public License for more details.
 
 import logging
 import numpy
 from scipy.stats import kstest
 
-logger = logging.getLogger('pycbc.events.trigger_fits')
-
 def exponential_fitalpha(vals, thresh, w):
     """
     Maximum likelihood estimator for the fit factor for
     an exponential decrease model
     """
     return 1. / (numpy.average(vals, weights=w) - thresh)
 
@@ -125,16 +123,16 @@
     if thresh is None:
         thresh = min(vals)
         above_thresh = numpy.ones_like(vals, dtype=bool)
     else:
         above_thresh = vals >= thresh
         if numpy.count_nonzero(above_thresh) == 0:
             # Nothing is above threshold - warn and return -1
-            logger.warning("No values are above the threshold, %.2f, "
-                           "maximum is %.2f.", thresh, vals.max())
+            logging.warning("No values are above the threshold, %.2f, "
+                            "maximum is %.2f.", thresh, vals.max())
             return -1., -1.
 
         vals = vals[above_thresh]
 
     # Set up the weights
     if weights is not None:
         weights = numpy.array(weights)
```

### Comparing `PyCBC-2.3.6/pycbc/events/triggers.py` & `PyCBC-2.4.0/pycbc/events/triggers.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/events/veto.py` & `PyCBC-2.4.0/pycbc/events/veto.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/__init__.py` & `PyCBC-2.4.0/pycbc/fft/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/backend_cpu.py` & `PyCBC-2.4.0/pycbc/fft/backend_cpu.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/backend_cuda.py` & `PyCBC-2.4.0/pycbc/fft/backend_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/backend_mkl.py` & `PyCBC-2.4.0/pycbc/fft/backend_mkl.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/backend_support.py` & `PyCBC-2.4.0/pycbc/fft/backend_support.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/class_api.py` & `PyCBC-2.4.0/pycbc/fft/class_api.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/core.py` & `PyCBC-2.4.0/pycbc/fft/core.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/cuda_pyfft.py` & `PyCBC-2.4.0/pycbc/fft/cuda_pyfft.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/cufft.py` & `PyCBC-2.4.0/pycbc/fft/cufft.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/fft_callback.py` & `PyCBC-2.4.0/pycbc/fft/fft_callback.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/fftw.py` & `PyCBC-2.4.0/pycbc/fft/fftw.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/fftw_pruned.py` & `PyCBC-2.4.0/pycbc/fft/fftw_pruned.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/fftw_pruned_cython.pyx` & `PyCBC-2.4.0/pycbc/fft/fftw_pruned_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/func_api.py` & `PyCBC-2.4.0/pycbc/fft/func_api.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/mkl.py` & `PyCBC-2.4.0/pycbc/fft/mkl.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/npfft.py` & `PyCBC-2.4.0/pycbc/fft/npfft.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/fft/parser_support.py` & `PyCBC-2.4.0/pycbc/fft/parser_support.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/autocorrelation.py` & `PyCBC-2.4.0/pycbc/filter/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/fotonfilter.py` & `PyCBC-2.4.0/pycbc/filter/fotonfilter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/matchedfilter.py` & `PyCBC-2.4.0/pycbc/filter/matchedfilter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/matchedfilter_cpu.pyx` & `PyCBC-2.4.0/pycbc/filter/matchedfilter_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/matchedfilter_cuda.py` & `PyCBC-2.4.0/pycbc/filter/matchedfilter_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/matchedfilter_numpy.py` & `PyCBC-2.4.0/pycbc/filter/matchedfilter_numpy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/qtransform.py` & `PyCBC-2.4.0/pycbc/filter/qtransform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/resample.py` & `PyCBC-2.4.0/pycbc/filter/resample.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/simd_correlate.py` & `PyCBC-2.4.0/pycbc/filter/simd_correlate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/simd_correlate_ccode.cpp` & `PyCBC-2.4.0/pycbc/filter/simd_correlate_ccode.cpp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/simd_correlate_cython.pyx` & `PyCBC-2.4.0/pycbc/filter/simd_correlate_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/filter/zpk.py` & `PyCBC-2.4.0/pycbc/filter/zpk.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/frame/__init__.py` & `PyCBC-2.4.0/pycbc/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/frame/frame.py` & `PyCBC-2.4.0/pycbc/frame/frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,22 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """
 This modules contains functions for reading in data from frame files or caches
 """
 
-import logging
-import warnings
-import os.path
-import glob
-import time
-import math
-import re
-from urllib.parse import urlparse
-import numpy
-import lalframe
+import lalframe, logging
 import lal
+import numpy
+import math
+import os.path, glob, time
 from gwdatafind import find_urls as find_frame_urls
 import pycbc
+from urllib.parse import urlparse
 from pycbc.types import TimeSeries, zeros
 
 
 # map LAL series types to corresponding functions and Numpy types
 _fr_type_map = {
     lal.S_TYPE_CODE: [
         lalframe.FrStreamReadREAL4TimeSeries, numpy.float32,
@@ -257,115 +252,57 @@
             channel_data = _read_channel(channel, stream, start_time, duration)
             lalframe.FrStreamSeek(stream, start_time)
             all_data.append(channel_data)
         return all_data
     else:
         return _read_channel(channels, stream, start_time, duration)
 
-def frame_paths(
-    frame_type, start_time, end_time, server=None, url_type='file', site=None
-):
-    """Return the paths to a span of frame files.
+def frame_paths(frame_type, start_time, end_time, server=None, url_type='file'):
+    """Return the paths to a span of frame files
 
     Parameters
     ----------
     frame_type : string
-        The string representation of the frame type (ex. 'H1_ER_C00_L1').
+        The string representation of the frame type (ex. 'H1_ER_C00_L1')
     start_time : int
         The start time that we need the frames to span.
     end_time : int
         The end time that we need the frames to span.
     server : {None, SERVER:PORT string}, optional
         Optional string to specify the datafind server to use. By default an
         attempt is made to use a local datafind server.
     url_type : string
         Returns only frame URLs with a particular scheme or head such
         as "file" or "https". Default is "file", which queries locally
         stored frames. Option can be disabled if set to None.
-    site : string, optional
-        One-letter string specifying which site you want data from (H, L, V,
-        etc).  If not given, the site is assumed to be the first letter of
-        `frame_type`, which is usually (but not always) a safe assumption.
-
     Returns
     -------
     paths : list of paths
         The list of paths to the frame files.
 
     Examples
     --------
     >>> paths = frame_paths('H1_LDAS_C02_L2', 968995968, 968995968+2048)
     """
-    if site is None:
-        # this case is tolerated for backward compatibility
-        site = frame_type[0]
-        warnings.warn(
-            f'Guessing site {site} from frame type {frame_type}',
-            DeprecationWarning
-        )
+    site = frame_type[0]
     cache = find_frame_urls(site, frame_type, start_time, end_time,
                             urltype=url_type, host=server)
     return [urlparse(entry).path for entry in cache]
 
-
-def get_site_from_type_or_channel(frame_type, channels):
-    """Determine the site for querying gwdatafind (H, L, V, etc) based on
-    substrings of the frame type and channel(s).
-
-    The type should begin with S: or SN:, in which case S is taken as the
-    site.  Otherwise, the same is done with the channel (with the first
-    channel if more than one are given). If that also fails, the site is
-    taken to be the first letter of the frame type, which is usually
-    (but not always) a correct assumption.
-
-    Parameters
-    ----------
-    frame_type : string
-        The frame type, ideally prefixed by the site indicator.
-    channels : string or list of strings
-        The channel name or names.
-
-    Returns
-    -------
-    site : string
-        The site letter.
-    frame_type : string
-        The frame type with the site prefix (if any) removed.
-    """
-    site_re = '^([^:])[^:]?:'
-    m = re.match(site_re, frame_type)
-    if m:
-        return m.groups(1)[0], frame_type[m.end():]
-    chan = channels
-    if isinstance(chan, list):
-        chan = channels[0]
-    m = re.match(site_re, chan)
-    if m:
-        return m.groups(1)[0], frame_type
-    warnings.warn(
-        f'Guessing site {frame_type[0]} from frame type {frame_type}',
-        DeprecationWarning
-    )
-    return frame_type[0], frame_type
-
-
 def query_and_read_frame(frame_type, channels, start_time, end_time,
                          sieve=None, check_integrity=False):
     """Read time series from frame data.
 
-    Query for the location of physical frames matching the frame type. Return
+    Query for the locatin of physical frames matching the frame type. Return
     a time series containing the channel between the given start and end times.
 
     Parameters
     ----------
     frame_type : string
-        The type of frame file that we are looking for. The string should begin
-        with S: or SN:, in which case S is taken as the site to query. If this
-        is not the case, the site will be guessed from the channel name or from
-        the type in a different way, which may not work.
+        The type of frame file that we are looking for.
     channels : string or list of strings
         Either a string that contains the channel name or a list of channel
         name strings.
     start_time : LIGOTimeGPS or int
         The gps start time of the time series. Defaults to reading from the
         beginning of the available frame(s).
     end_time : LIGOTimeGPS or int
@@ -383,46 +320,38 @@
         the frame file/cache for a given channel or channels.
 
     Examples
     --------
     >>> ts = query_and_read_frame('H1_LDAS_C02_L2', 'H1:LDAS-STRAIN',
     >>>                               968995968, 968995968+2048)
     """
-    site, frame_type = get_site_from_type_or_channel(frame_type, channels)
-
     # Allows compatibility with our standard tools
     # We may want to place this into a higher level frame getting tool
     if frame_type in ['LOSC_STRAIN', 'GWOSC_STRAIN']:
         from pycbc.frame.gwosc import read_strain_gwosc
         if not isinstance(channels, list):
             channels = [channels]
         data = [read_strain_gwosc(c[:2], start_time, end_time)
                 for c in channels]
         return data if len(data) > 1 else data[0]
     if frame_type in ['LOSC', 'GWOSC']:
         from pycbc.frame.gwosc import read_frame_gwosc
         return read_frame_gwosc(channels, start_time, end_time)
 
-    logging.info('Querying datafind server')
-    paths = frame_paths(
-        frame_type,
-        int(start_time),
-        int(numpy.ceil(end_time)),
-        site=site
-    )
-    logging.info('Found frame file paths: %s', ' '.join(paths))
-    return read_frame(
-        paths,
-        channels,
-        start_time=start_time,
-        end_time=end_time,
-        sieve=sieve,
-        check_integrity=check_integrity
-    )
+    logging.info('querying datafind server')
+    paths = frame_paths(frame_type, int(start_time), int(numpy.ceil(end_time)))
+    logging.info('found files: %s' % (' '.join(paths)))
+    return read_frame(paths, channels,
+                      start_time=start_time,
+                      end_time=end_time,
+                      sieve=sieve,
+                      check_integrity=check_integrity)
 
+__all__ = ['read_frame', 'frame_paths',
+           'query_and_read_frame']
 
 def write_frame(location, channels, timeseries):
     """Write a list of time series to a single frame file.
 
     Parameters
     ----------
     location : string
@@ -954,19 +883,7 @@
         Parameters
         ----------
         blocksize: int
             The number of seconds to advance the buffers
         """
         self.idq.null_advance(blocksize)
         self.idq_state.null_advance(blocksize)
-
-
-__all__ = [
-    'locations_to_cache',
-    'read_frame',
-    'query_and_read_frame',
-    'frame_paths',
-    'write_frame',
-    'DataBuffer',
-    'StatusBuffer',
-    'iDQBuffer'
-]
```

### Comparing `PyCBC-2.3.6/pycbc/frame/gwosc.py` & `PyCBC-2.4.0/pycbc/frame/gwosc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/frame/store.py` & `PyCBC-2.4.0/pycbc/frame/store.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/burn_in.py` & `PyCBC-2.4.0/pycbc/inference/burn_in.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/entropy.py` & `PyCBC-2.4.0/pycbc/inference/entropy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/evidence.py` & `PyCBC-2.4.0/pycbc/inference/evidence.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/gelman_rubin.py` & `PyCBC-2.4.0/pycbc/inference/gelman_rubin.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/geweke.py` & `PyCBC-2.4.0/pycbc/inference/geweke.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/__init__.py` & `PyCBC-2.4.0/pycbc/inference/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/base_hdf.py` & `PyCBC-2.4.0/pycbc/inference/io/base_hdf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/base_mcmc.py` & `PyCBC-2.4.0/pycbc/inference/io/base_mcmc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/base_multitemper.py` & `PyCBC-2.4.0/pycbc/inference/io/base_multitemper.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/base_nested_sampler.py` & `PyCBC-2.4.0/pycbc/inference/io/base_nested_sampler.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/base_sampler.py` & `PyCBC-2.4.0/pycbc/inference/io/base_sampler.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/cpnest.py` & `PyCBC-2.4.0/pycbc/inference/io/cpnest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/dynesty.py` & `PyCBC-2.4.0/pycbc/inference/io/dynesty.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/emcee.py` & `PyCBC-2.4.0/pycbc/inference/io/emcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/emcee_pt.py` & `PyCBC-2.4.0/pycbc/inference/io/emcee_pt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/epsie.py` & `PyCBC-2.4.0/pycbc/inference/io/epsie.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/multinest.py` & `PyCBC-2.4.0/pycbc/inference/io/multinest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/posterior.py` & `PyCBC-2.4.0/pycbc/inference/io/posterior.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/ptemcee.py` & `PyCBC-2.4.0/pycbc/inference/io/ptemcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/txt.py` & `PyCBC-2.4.0/pycbc/inference/io/txt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/io/ultranest.py` & `PyCBC-2.4.0/pycbc/inference/io/ultranest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/jump/__init__.py` & `PyCBC-2.4.0/pycbc/inference/jump/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/jump/angular.py` & `PyCBC-2.4.0/pycbc/inference/jump/angular.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/jump/bounded_normal.py` & `PyCBC-2.4.0/pycbc/inference/jump/bounded_normal.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/jump/discrete.py` & `PyCBC-2.4.0/pycbc/inference/jump/discrete.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/jump/normal.py` & `PyCBC-2.4.0/pycbc/inference/jump/normal.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/__init__.py` & `PyCBC-2.4.0/pycbc/inference/models/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/analytic.py` & `PyCBC-2.4.0/pycbc/inference/models/analytic.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/base.py` & `PyCBC-2.4.0/pycbc/inference/models/base.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/base_data.py` & `PyCBC-2.4.0/pycbc/inference/models/base_data.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/brute_marg.py` & `PyCBC-2.4.0/pycbc/inference/models/brute_marg.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/data_utils.py` & `PyCBC-2.4.0/pycbc/inference/models/data_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/gated_gaussian_noise.py` & `PyCBC-2.4.0/pycbc/inference/models/gated_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/gaussian_noise.py` & `PyCBC-2.4.0/pycbc/inference/models/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/hierarchical.py` & `PyCBC-2.4.0/pycbc/inference/models/hierarchical.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/marginalized_gaussian_noise.py` & `PyCBC-2.4.0/pycbc/inference/models/marginalized_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/relbin.py` & `PyCBC-2.4.0/pycbc/inference/models/relbin.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/relbin_cpu.pyx` & `PyCBC-2.4.0/pycbc/inference/models/relbin_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/single_template.py` & `PyCBC-2.4.0/pycbc/inference/models/single_template.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/models/tools.py` & `PyCBC-2.4.0/pycbc/inference/models/tools.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/option_utils.py` & `PyCBC-2.4.0/pycbc/inference/option_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/__init__.py` & `PyCBC-2.4.0/pycbc/inference/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/base.py` & `PyCBC-2.4.0/pycbc/inference/sampler/base.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/base_cube.py` & `PyCBC-2.4.0/pycbc/inference/sampler/base_cube.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/base_mcmc.py` & `PyCBC-2.4.0/pycbc/inference/sampler/base_mcmc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/base_multitemper.py` & `PyCBC-2.4.0/pycbc/inference/sampler/base_multitemper.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/cpnest.py` & `PyCBC-2.4.0/pycbc/inference/sampler/cpnest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/dummy.py` & `PyCBC-2.4.0/pycbc/inference/sampler/dummy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/dynesty.py` & `PyCBC-2.4.0/pycbc/inference/sampler/dynesty.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/emcee.py` & `PyCBC-2.4.0/pycbc/inference/sampler/emcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/emcee_pt.py` & `PyCBC-2.4.0/pycbc/inference/sampler/emcee_pt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/epsie.py` & `PyCBC-2.4.0/pycbc/inference/sampler/epsie.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/multinest.py` & `PyCBC-2.4.0/pycbc/inference/sampler/multinest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/ptemcee.py` & `PyCBC-2.4.0/pycbc/inference/sampler/ptemcee.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/refine.py` & `PyCBC-2.4.0/pycbc/inference/sampler/refine.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inference/sampler/ultranest.py` & `PyCBC-2.4.0/pycbc/inference/sampler/ultranest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inject/inject.py` & `PyCBC-2.4.0/pycbc/inject/inject.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/inject/injfilterrejector.py` & `PyCBC-2.4.0/pycbc/inject/injfilterrejector.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/io/__init__.py` & `PyCBC-2.4.0/pycbc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/io/hdf.py` & `PyCBC-2.4.0/pycbc/io/hdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,16 +513,15 @@
                                            cluster_window=10):
         """Edits the mask property of the class to point to the N loudest
         single detector events as ranked by ranking statistic. Events are
         clustered so that no more than 1 event within +/- cluster-window will
         be considered."""
 
         # If this becomes memory intensive we can optimize
-        sds = rank_method.single(self.trig_dict())
-        stat = rank_method.rank_stat_single((self.ifo, sds))
+        stat = rank_method.rank_stat_single((self.ifo, self.trig_dict()))
         if len(stat) == 0:
             # No triggers, so just return here
             self.stat = np.array([])
             return
 
         times = self.end_time
         index = stat.argsort()[::-1]
@@ -959,18 +958,14 @@
                 sngl.event_id = event_id
                 sngl.ifo = ifo
                 net_snrsq += sngl_col_vals['snr'][ifo][0][idx]**2
                 for name in sngl_col_names:
                     val = sngl_col_vals[name][ifo][0][idx]
                     if name == 'end_time':
                         sngl.end = LIGOTimeGPS(val)
-                    elif name == 'chisq':
-                        # Use reduced chisquared to be consistent with Live
-                        dof = 2. * sngl_col_vals['chisq_dof'][ifo][0][idx] - 2.
-                        sngl.chisq = val / dof
                     else:
                         setattr(sngl, name, val)
                 for name in bank_col_names:
                     val = bank_col_vals[name][idx]
                     setattr(sngl, name, val)
                 sngl.mtotal, sngl.eta = pnutils.mass1_mass2_to_mtotal_eta(
                         sngl.mass1, sngl.mass2)
```

### Comparing `PyCBC-2.3.6/pycbc/io/ligolw.py` & `PyCBC-2.4.0/pycbc/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/io/live.py` & `PyCBC-2.4.0/pycbc/io/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from pycbc import pnutils
 from pycbc.io.ligolw import (
     return_empty_sngl,
     create_process_table,
     make_psd_xmldoc,
     snr_series_to_xml
 )
-from pycbc.results import generate_asd_plot, generate_snr_plot
+from pycbc.results import generate_asd_plot
+from pycbc.results import ifo_color
 from pycbc.results import source_color
 from pycbc.mchirp_area import calc_probabilities
 
 
 class CandidateForGraceDB(object):
     """This class provides an interface for uploading candidates to GraceDB.
     """
@@ -441,29 +442,35 @@
 
         # plot the SNR timeseries and noise PSDs
         if self.snr_series is not None:
             snr_series_fname = self.basename + '.hdf'
             snr_series_plot_fname = self.basename + '_snr.png'
             asd_series_plot_fname = self.basename + '_asd.png'
 
-            triggers = {
-                ifo: (self.coinc_results[f'foreground/{ifo}/end_time']
-                      + self.time_offset,
-                      self.coinc_results[f'foreground/{ifo}/snr'])
-                for ifo in self.et_ifos
-                }
+            pl.figure()
             ref_time = int(self.merger_time)
-            generate_snr_plot(self.snr_series, snr_series_plot_fname,
-                              triggers, ref_time)
-
-            generate_asd_plot(self.psds, asd_series_plot_fname)
-
             for ifo in sorted(self.snr_series):
                 curr_snrs = self.snr_series[ifo]
                 curr_snrs.save(snr_series_fname, group='%s/snr' % ifo)
+                pl.plot(curr_snrs.sample_times - ref_time, abs(curr_snrs),
+                        c=ifo_color(ifo), label=ifo)
+                if ifo in self.et_ifos:
+                    base = 'foreground/{}/'.format(ifo)
+                    snr = self.coinc_results[base + 'snr']
+                    mt = (self.coinc_results[base + 'end_time']
+                          + self.time_offset)
+                    pl.plot([mt - ref_time], [snr], c=ifo_color(ifo),
+                            marker='x')
+            pl.legend()
+            pl.xlabel('GPS time from {:d} (s)'.format(ref_time))
+            pl.ylabel('SNR')
+            pl.savefig(snr_series_plot_fname)
+            pl.close()
+
+            generate_asd_plot(self.psds, asd_series_plot_fname)
 
             # Additionally save the PSDs into the snr_series file
             for ifo in sorted(self.psds):
                 # Undo dynamic range factor
                 curr_psd = self.psds[ifo].astype(numpy.float64)
                 curr_psd /= pycbc.DYN_RANGE_FAC ** 2.0
                 curr_psd.save(snr_series_fname, group='%s/psd' % ifo)
```

### Comparing `PyCBC-2.3.6/pycbc/io/record.py` & `PyCBC-2.4.0/pycbc/io/record.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/libutils.py` & `PyCBC-2.4.0/pycbc/libutils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/live/snr_optimizer.py` & `PyCBC-2.4.0/pycbc/live/snr_optimizer.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/mchirp_area.py` & `PyCBC-2.4.0/pycbc/mchirp_area.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/neutron_stars/eos_utils.py` & `PyCBC-2.4.0/pycbc/neutron_stars/eos_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/neutron_stars/ns_data/equil_2H.dat` & `PyCBC-2.4.0/pycbc/neutron_stars/ns_data/equil_2H.dat`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/neutron_stars/pg_isso_solver.py` & `PyCBC-2.4.0/pycbc/neutron_stars/pg_isso_solver.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/noise/gaussian.py` & `PyCBC-2.4.0/pycbc/noise/gaussian.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/noise/reproduceable.py` & `PyCBC-2.4.0/pycbc/noise/reproduceable.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/opt.py` & `PyCBC-2.4.0/pycbc/opt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/pnutils.py` & `PyCBC-2.4.0/pycbc/pnutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,39 +517,39 @@
         Second component dimensionless spin S_2/m_2^2 projected onto L
 
     Returns
     -------
     f : float or numpy.array
         Frequency in Hz
     """
-    params = {"mass1": m1, "mass2": m2, "spin1z": s1z, "spin2z": s2z}
+    params = {"mass1":m1, "mass2":m2, "spin1z":s1z, "spin2z":s2z}
     return named_frequency_cutoffs[name](params)
 
 def _get_imr_duration(m1, m2, s1z, s2z, f_low, approximant="SEOBNRv4"):
     """Wrapper of lalsimulation template duration approximate formula"""
     m1, m2, s1z, s2z, f_low = float(m1), float(m2), float(s1z), float(s2z),\
                               float(f_low)
     if approximant == "SEOBNRv2":
         chi = lalsim.SimIMRPhenomBComputeChi(m1, m2, s1z, s2z)
         time_length = lalsim.SimIMRSEOBNRv2ChirpTimeSingleSpin(
                                 m1 * lal.MSUN_SI, m2 * lal.MSUN_SI, chi, f_low)
-    elif approximant == "IMRPhenomXAS":
+    elif approximant == 'IMRPhenomXAS':
         time_length = lalsim.SimIMRPhenomXASDuration(
                            m1 * lal.MSUN_SI, m2 * lal.MSUN_SI, s1z, s2z, f_low)
     elif approximant == "IMRPhenomD":
         time_length = lalsim.SimIMRPhenomDChirpTime(
                            m1 * lal.MSUN_SI, m2 * lal.MSUN_SI, s1z, s2z, f_low)
-    elif approximant in ["SEOBNRv4", "SEOBNRv4_ROM"]:
-        # NB the LALSim function has f_low as first argument
+    elif approximant == "SEOBNRv4":
+        # NB for no clear reason this function has f_low as first argument
         time_length = lalsim.SimIMRSEOBNRv4ROMTimeOfFrequency(
                            f_low, m1 * lal.MSUN_SI, m2 * lal.MSUN_SI, s1z, s2z)
-    elif approximant in ["SEOBNRv5", "SEOBNRv5_ROM"]:
+    elif approximant == 'SEOBNRv5_ROM':
         time_length = lalsim.SimIMRSEOBNRv5ROMTimeOfFrequency(
                            f_low, m1 * lal.MSUN_SI, m2 * lal.MSUN_SI, s1z, s2z)
-    elif approximant in ["SPAtmplt", "TaylorF2"]:
+    elif approximant == 'SPAtmplt' or approximant == 'TaylorF2':
         chi = lalsim.SimInspiralTaylorF2ReducedSpinComputeChi(
             m1, m2, s1z, s2z
         )
         time_length = lalsim.SimInspiralTaylorF2ReducedSpinChirpTime(
             f_low, m1 * lal.MSUN_SI, m2 * lal.MSUN_SI, chi, -1
         )
     else:
```

### Comparing `PyCBC-2.3.6/pycbc/pool.py` & `PyCBC-2.4.0/pycbc/pool.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/fgmc_functions.py` & `PyCBC-2.4.0/pycbc/population/fgmc_functions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/fgmc_laguerre.py` & `PyCBC-2.4.0/pycbc/population/fgmc_laguerre.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/fgmc_plots.py` & `PyCBC-2.4.0/pycbc/population/fgmc_plots.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/live_pastro.py` & `PyCBC-2.4.0/pycbc/population/live_pastro.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/live_pastro_utils.py` & `PyCBC-2.4.0/pycbc/population/live_pastro_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/population_models.py` & `PyCBC-2.4.0/pycbc/population/population_models.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/rates_functions.py` & `PyCBC-2.4.0/pycbc/population/rates_functions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/population/scale_injections.py` & `PyCBC-2.4.0/pycbc/population/scale_injections.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/psd/__init__.py` & `PyCBC-2.4.0/pycbc/psd/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/psd/analytical.py` & `PyCBC-2.4.0/pycbc/psd/analytical.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/psd/analytical_space.py` & `PyCBC-2.4.0/pycbc/psd/analytical_space.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/psd/estimate.py` & `PyCBC-2.4.0/pycbc/psd/estimate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/psd/read.py` & `PyCBC-2.4.0/pycbc/psd/read.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/psd/variation.py` & `PyCBC-2.4.0/pycbc/psd/variation.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/rate.py` & `PyCBC-2.4.0/pycbc/rate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/color.py` & `PyCBC-2.4.0/pycbc/results/color.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/dq.py` & `PyCBC-2.4.0/pycbc/results/dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/followup.py` & `PyCBC-2.4.0/pycbc/results/followup.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/layout.py` & `PyCBC-2.4.0/pycbc/results/layout.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/metadata.py` & `PyCBC-2.4.0/pycbc/results/metadata.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/mpld3_utils.py` & `PyCBC-2.4.0/pycbc/results/mpld3_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/plot.py` & `PyCBC-2.4.0/pycbc/results/plot.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/psd.py` & `PyCBC-2.4.0/pycbc/results/psd.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/pygrb_plotting_utils.py` & `PyCBC-2.4.0/pycbc/results/pygrb_plotting_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/pygrb_postprocessing_utils.py` & `PyCBC-2.4.0/pycbc/results/pygrb_postprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/render.py` & `PyCBC-2.4.0/pycbc/results/render.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/scatter_histograms.py` & `PyCBC-2.4.0/pycbc/results/scatter_histograms.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css` & `PyCBC-2.4.0/pycbc/results/static/css/bootstrap/3.3.2/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/css/bootstrap.min.css` & `PyCBC-2.4.0/pycbc/results/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css` & `PyCBC-2.4.0/pycbc/results/static/css/fancybox/2.1.5/jquery.fancybox.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/css/pycbc/orange.css` & `PyCBC-2.4.0/pycbc/results/static/css/pycbc/orange.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/css/pycbc/red.css` & `PyCBC-2.4.0/pycbc/results/static/css/pycbc/red.css`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.eot` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.eot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.html` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.ttf` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Light.woff` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Light.woff`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.eot` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.eot`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.html` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.ttf` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/fonts/Lato-Semibold.woff` & `PyCBC-2.4.0/pycbc/results/static/fonts/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js` & `PyCBC-2.4.0/pycbc/results/static/js/bootstrap/3.3.2/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/bootstrap.min.js` & `PyCBC-2.4.0/pycbc/results/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js` & `PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/fancybox-orange.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js` & `PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js` & `PyCBC-2.4.0/pycbc/results/static/js/fancybox/2.1.5/jquery.fancybox.pack.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js` & `PyCBC-2.4.0/pycbc/results/static/js/jquery/1.10.2/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js` & `PyCBC-2.4.0/pycbc/results/static/js/jquery/1.10.2/jquery.mousewheel-3.0.6.pack.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/static/js/jquery.min.js` & `PyCBC-2.4.0/pycbc/results/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/str_utils.py` & `PyCBC-2.4.0/pycbc/results/str_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/table_utils.py` & `PyCBC-2.4.0/pycbc/results/table_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/files/file_default.html` & `PyCBC-2.4.0/pycbc/results/templates/files/file_default.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/files/file_glitchgram.html` & `PyCBC-2.4.0/pycbc/results/templates/files/file_glitchgram.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/files/file_pre.html` & `PyCBC-2.4.0/pycbc/results/templates/files/file_pre.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/files/file_tmplt.html` & `PyCBC-2.4.0/pycbc/results/templates/files/file_tmplt.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/orange.html` & `PyCBC-2.4.0/pycbc/results/templates/orange.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/red.html` & `PyCBC-2.4.0/pycbc/results/templates/red.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/templates/wells/two_column.html` & `PyCBC-2.4.0/pycbc/results/templates/wells/two_column.html`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/results/versioning.py` & `PyCBC-2.4.0/pycbc/results/versioning.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/scheme.py` & `PyCBC-2.4.0/pycbc/scheme.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/sensitivity.py` & `PyCBC-2.4.0/pycbc/sensitivity.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/strain/__init__.py` & `PyCBC-2.4.0/pycbc/strain/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/strain/calibration.py` & `PyCBC-2.4.0/pycbc/strain/calibration.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/strain/gate.py` & `PyCBC-2.4.0/pycbc/strain/gate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/strain/lines.py` & `PyCBC-2.4.0/pycbc/strain/lines.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/strain/recalibrate.py` & `PyCBC-2.4.0/pycbc/strain/recalibrate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/strain/strain.py` & `PyCBC-2.4.0/pycbc/strain/strain.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,18 +500,16 @@
     # Read from hdf store file
     data_reading_group.add_argument("--hdf-store",
                             type=str,
                             help="Store of time series data in hdf format")
     # Use datafind to get frame files
     data_reading_group.add_argument("--frame-type",
                             type=str,
-                            metavar="S:TYPE",
                             help="(optional), replaces frame-files. Use datafind "
-                                 "to get the needed frame file(s) of this type "
-                                 "from site S.")
+                                 "to get the needed frame file(s) of this type.")
     # Filter frame files by URL
     data_reading_group.add_argument("--frame-sieve",
                             type=str,
                             help="(optional), Only use frame files where the "
                                  "URL matches the regular expression given.")
 
     # Generate gaussian noise with given psd
@@ -702,15 +700,15 @@
     # Read from hdf store file
     data_reading_group_multi.add_argument("--hdf-store", type=str, nargs='+',
                             action=MultiDetOptionAction,
                             metavar='IFO:HDF_STORE_FILE',
                             help="Store of time series data in hdf format")
     # Use datafind to get frame files
     data_reading_group_multi.add_argument("--frame-type", type=str, nargs="+",
-                                    action=MultiDetOptionActionSpecial,
+                                    action=MultiDetOptionAction,
                                     metavar='IFO:FRAME_TYPE',
                                     help="(optional) Replaces frame-files. "
                                          "Use datafind to get the needed frame "
                                          "file(s) of this type.")
     # Filter frame files by URL
     data_reading_group_multi.add_argument("--frame-sieve", type=str, nargs="+",
                             action=MultiDetOptionAction,
@@ -1973,20 +1971,17 @@
             idq_channel = ':'.join([ifo, args.idq_channel[ifo]])
 
         idq_state_channel = None
         if args.idq_state_channel and ifo in args.idq_state_channel:
             idq_state_channel = ':'.join([ifo, args.idq_state_channel[ifo]])
 
         if args.frame_type:
-            frame_src = pycbc.frame.frame_paths(
-                args.frame_type[ifo],
-                args.start_time,
-                args.end_time,
-                site=ifo[0]
-            )
+            frame_src = pycbc.frame.frame_paths(args.frame_type[ifo],
+                                                args.start_time,
+                                                args.end_time)
         else:
             frame_src = [args.frame_src[ifo]]
         strain_channel = ':'.join([ifo, args.channel_name[ifo]])
 
         return cls(frame_src, strain_channel,
                    args.start_time, max_buffer=maxlen * 2,
                    state_channel=state_channel,
```

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/bank_conversions.py` & `PyCBC-2.4.0/pycbc/tmpltbank/bank_conversions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/bank_output_utils.py` & `PyCBC-2.4.0/pycbc/tmpltbank/bank_output_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/brute_force_methods.py` & `PyCBC-2.4.0/pycbc/tmpltbank/brute_force_methods.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/calc_moments.py` & `PyCBC-2.4.0/pycbc/tmpltbank/calc_moments.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/coord_utils.py` & `PyCBC-2.4.0/pycbc/tmpltbank/coord_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/lambda_mapping.py` & `PyCBC-2.4.0/pycbc/tmpltbank/lambda_mapping.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/lattice_utils.py` & `PyCBC-2.4.0/pycbc/tmpltbank/lattice_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/option_utils.py` & `PyCBC-2.4.0/pycbc/tmpltbank/option_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/tmpltbank/partitioned_bank.py` & `PyCBC-2.4.0/pycbc/tmpltbank/partitioned_bank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/transforms.py` & `PyCBC-2.4.0/pycbc/transforms.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/aligned.py` & `PyCBC-2.4.0/pycbc/types/aligned.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/array.py` & `PyCBC-2.4.0/pycbc/types/array.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/array_cpu.pyx` & `PyCBC-2.4.0/pycbc/types/array_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/array_cuda.py` & `PyCBC-2.4.0/pycbc/types/array_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/config.py` & `PyCBC-2.4.0/pycbc/types/config.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/frequencyseries.py` & `PyCBC-2.4.0/pycbc/types/frequencyseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/optparse.py` & `PyCBC-2.4.0/pycbc/types/optparse.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/types/timeseries.py` & `PyCBC-2.4.0/pycbc/types/timeseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/vetoes/autochisq.py` & `PyCBC-2.4.0/pycbc/vetoes/autochisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/vetoes/bank_chisq.py` & `PyCBC-2.4.0/pycbc/vetoes/bank_chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/vetoes/chisq.py` & `PyCBC-2.4.0/pycbc/vetoes/chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/vetoes/chisq_cpu.pyx` & `PyCBC-2.4.0/pycbc/vetoes/chisq_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/vetoes/chisq_cuda.py` & `PyCBC-2.4.0/pycbc/vetoes/chisq_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/vetoes/sgchisq.py` & `PyCBC-2.4.0/pycbc/vetoes/sgchisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/SpinTaylorF2.py` & `PyCBC-2.4.0/pycbc/waveform/SpinTaylorF2.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/__init__.py` & `PyCBC-2.4.0/pycbc/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/bank.py` & `PyCBC-2.4.0/pycbc/waveform/bank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/compress.py` & `PyCBC-2.4.0/pycbc/waveform/compress.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/decompress_cpu.py` & `PyCBC-2.4.0/pycbc/waveform/decompress_cpu.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/decompress_cpu_ccode.cpp` & `PyCBC-2.4.0/pycbc/waveform/decompress_cpu_ccode.cpp`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/decompress_cpu_cython.pyx` & `PyCBC-2.4.0/pycbc/waveform/decompress_cpu_cython.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/decompress_cuda.py` & `PyCBC-2.4.0/pycbc/waveform/decompress_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/generator.py` & `PyCBC-2.4.0/pycbc/waveform/generator.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/multiband.py` & `PyCBC-2.4.0/pycbc/waveform/multiband.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/nltides.py` & `PyCBC-2.4.0/pycbc/waveform/nltides.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/parameters.py` & `PyCBC-2.4.0/pycbc/waveform/parameters.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/plugin.py` & `PyCBC-2.4.0/pycbc/waveform/plugin.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/premerger.py` & `PyCBC-2.4.0/pycbc/waveform/premerger.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/pycbc_phenomC_tmplt.py` & `PyCBC-2.4.0/pycbc/waveform/pycbc_phenomC_tmplt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/ringdown.py` & `PyCBC-2.4.0/pycbc/waveform/ringdown.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/sinegauss.py` & `PyCBC-2.4.0/pycbc/waveform/sinegauss.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/spa_tmplt.py` & `PyCBC-2.4.0/pycbc/waveform/spa_tmplt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/spa_tmplt_cpu.pyx` & `PyCBC-2.4.0/pycbc/waveform/spa_tmplt_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/spa_tmplt_cuda.py` & `PyCBC-2.4.0/pycbc/waveform/spa_tmplt_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/supernovae.py` & `PyCBC-2.4.0/pycbc/waveform/supernovae.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/utils.py` & `PyCBC-2.4.0/pycbc/waveform/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/utils_cpu.pyx` & `PyCBC-2.4.0/pycbc/waveform/utils_cpu.pyx`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/utils_cuda.py` & `PyCBC-2.4.0/pycbc/waveform/utils_cuda.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/waveform/waveform.py` & `PyCBC-2.4.0/pycbc/waveform/waveform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1156,16 +1156,15 @@
         apx_int = approximant + '_INTERP'
         cpu_fd[apx_int] = get_interpolated_fd_waveform
         _filter_time_lengths[apx_int] = _filter_time_lengths[approximant]
 
         # We can also make a td version of this
         # This will override any existing approximants with the same name
         # (ex. IMRPhenomXX)
-        if approximant not in td_apx:
-            cpu_td[approximant] = get_td_waveform_from_fd
+        cpu_td[approximant] = get_td_waveform_from_fd
 
 for apx in copy.copy(_filter_time_lengths):
     td_fd_waveform_transform(apx)
 
 
 td_wav = _scheme.ChooseBySchemeDict()
 fd_wav = _scheme.ChooseBySchemeDict()
```

### Comparing `PyCBC-2.3.6/pycbc/waveform/waveform_modes.py` & `PyCBC-2.4.0/pycbc/waveform/waveform_modes.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/__init__.py` & `PyCBC-2.4.0/pycbc/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/coincidence.py` & `PyCBC-2.4.0/pycbc/workflow/coincidence.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/configparser_test.py` & `PyCBC-2.4.0/pycbc/workflow/configparser_test.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/configuration.py` & `PyCBC-2.4.0/pycbc/workflow/configuration.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/core.py` & `PyCBC-2.4.0/pycbc/workflow/core.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/datafind.py` & `PyCBC-2.4.0/pycbc/workflow/datafind.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/dq.py` & `PyCBC-2.4.0/pycbc/workflow/psd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020 Max Trevor and Derek Davis
+# Copyright (C) 2013  Ian Harry
 #
 # This program is free software; you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3 of the License, or (at your
 # option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -10,130 +10,112 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
 # Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-#
-# =============================================================================
-#
-#                                   Preamble
-#
-# =============================================================================
-#
+"""This module is responsible for setting up PSD-related jobs in workflows.
+"""
 
-import logging
-from pycbc.workflow.core import (FileList, Executable, Node, make_analysis_dir)
+from pycbc.workflow.core import FileList, make_analysis_dir, Executable
+from pycbc.workflow.core import SegFile
+from ligo.segments import segmentlist
 
+class CalcPSDExecutable(Executable):
+    current_retention_level = Executable.ALL_TRIGGERS
 
-class PyCBCBinTemplatesDQExecutable(Executable):
+class MergePSDFiles(Executable):
     current_retention_level = Executable.MERGED_TRIGGERS
 
-    def create_node(self, workflow, ifo, template_bank_file):
-        node = Node(self)
-        node.add_opt('--ifo', ifo)
-        node.add_input_opt('--bank-file', template_bank_file)
-        node.new_output_file_opt(
-            workflow.analysis_time, '.hdf', '--output-file')
-        return node
-
+def chunks(l, n):
+    """ Yield n successive chunks from l.
+    """
+    newn = int(len(l) / n)
+    for i in range(0, n-1):
+        yield l[i*newn:i*newn+newn]
+    yield l[n*newn-newn:]
+
+def merge_psds(workflow, files, ifo, out_dir, tags=None):
+    make_analysis_dir(out_dir)
+    tags = [] if not tags else tags
+    node = MergePSDFiles(workflow.cp, 'merge_psds',
+                         ifos=ifo, out_dir=out_dir,
+                         tags=tags).create_node()
+    node.add_input_list_opt('--psd-files', files)
+    node.new_output_file_opt(workflow.analysis_time, '.hdf', '--output-file')
+    workflow += node
+    return node.output_files[0]
+
+def setup_psd_calculate(workflow, frame_files, ifo, segments,
+                        segment_name, out_dir, tags=None):
+    make_analysis_dir(out_dir)
+    tags = [] if not tags else tags
+    if workflow.cp.has_option_tags('workflow-psd', 'parallelization-factor', tags=tags):
+        num_parts = int(workflow.cp.get_opt_tags('workflow-psd',
+                                                 'parallelization-factor',
+                                                 tags=tags))
+    else:
+        num_parts = 1
+
+    # get rid of duplicate segments which happen when splitting the bank
+    segments = segmentlist(frozenset(segments))
+
+    segment_lists = list(chunks(segments, num_parts))
+
+    psd_files = FileList([])
+    for i, segs in enumerate(segment_lists):
+        seg_file = SegFile.from_segment_list('%s_%s' %(segment_name, i),
+                         segmentlist(segs), segment_name, ifo,
+                         valid_segment=workflow.analysis_time,
+                         extension='xml', directory=out_dir)
+
+        psd_files += [make_psd_file(workflow, frame_files, seg_file,
+                                    segment_name, out_dir,
+                                    tags=tags + ['PART%s' % i])]
+
+    if num_parts > 1:
+        return merge_psds(workflow, psd_files, ifo, out_dir, tags=tags)
+    else:
+        return psd_files[0]
+
+def make_psd_file(workflow, frame_files, segment_file, segment_name, out_dir,
+                  tags=None):
+    make_analysis_dir(out_dir)
+    tags = [] if not tags else tags
+    exe = CalcPSDExecutable(workflow.cp, 'calculate_psd',
+                             ifos=segment_file.ifo, out_dir=out_dir,
+                             tags=tags)
+    node = exe.create_node()
+    node.add_input_opt('--analysis-segment-file', segment_file)
+    node.add_opt('--segment-name', segment_name)
+
+    if frame_files and not exe.has_opt('frame-type'):
+        node.add_input_list_opt('--frame-files', frame_files)
+
+    node.new_output_file_opt(workflow.analysis_time, '.hdf', '--output-file')
+    workflow += node
+    return node.output_files[0]
+
+class AvgPSDExecutable(Executable):
+    current_retention_level = Executable.FINAL_RESULT
+
+def make_average_psd(workflow, psd_files, out_dir, tags=None,
+                     output_fmt='.txt'):
+    make_analysis_dir(out_dir)
+    tags = [] if tags is None else tags
+    node = AvgPSDExecutable(workflow.cp, 'average_psd', ifos=workflow.ifos,
+                            out_dir=out_dir, tags=tags).create_node()
+    node.add_input_list_opt('--input-files', psd_files)
+
+    if len(workflow.ifos) > 1:
+        node.new_output_file_opt(workflow.analysis_time, output_fmt,
+                                 '--detector-avg-file')
 
-class PyCBCBinTriggerRatesDQExecutable(Executable):
-    current_retention_level = Executable.MERGED_TRIGGERS
+    node.new_multiifo_output_list_opt('--time-avg-file', workflow.ifos,
+                                 workflow.analysis_time, output_fmt, tags=tags)
 
-    def create_node(self, workflow, flag_file, flag_name,
-                    analysis_segment_file, analysis_segment_name,
-                    trig_file, template_bins_file):
-        node = Node(self)
-        node.add_input_opt('--template-bins-file', template_bins_file)
-        node.add_input_opt('--trig-file', trig_file)
-        node.add_input_opt('--flag-file', flag_file)
-        node.add_opt('--flag-name', flag_name)
-        node.add_input_opt('--analysis-segment-file', analysis_segment_file)
-        node.add_opt('--analysis-segment-name', analysis_segment_name)
-        node.new_output_file_opt(workflow.analysis_time, '.hdf',
-                                 '--output-file')
-        return node
-
-
-def setup_dq_reranking(workflow, insps, bank,
-                       analyzable_seg_file,
-                       analyzable_name,
-                       dq_seg_file,
-                       output_dir=None, tags=None):
-    logging.info("Setting up dq reranking")
-    make_analysis_dir(output_dir)
-    output_files = FileList()
-    output_labels = []
-    if tags is None:
-        tags = []
-
-    dq_labels = workflow.cp.get_subsections('workflow-data_quality')
-
-    dq_ifos = {}
-    dq_names = {}
-    dq_types = {}
-    for dql in dq_labels:
-        dq_ifos[dql] = workflow.cp.get_opt_tags(
-            'workflow-data_quality', 'dq-ifo', [dql])
-        dq_names[dql] = workflow.cp.get_opt_tags(
-            'workflow-data_quality', 'dq-name', [dql])
-        dq_types[dql] = workflow.cp.get_opt_tags(
-            'workflow-data_quality', 'dq-type', [dql])
-
-    ifos = set(dq_ifos.values())
-
-    for ifo in ifos:
-        # get the dq label, type, and name for this ifo
-        ifo_dq_labels = [dql for dql in dq_labels if (dq_ifos[dql] == ifo)]
-        assert len(ifo_dq_labels) < 2, f"Received multiple dq files for {ifo}"
-        dq_label = ifo_dq_labels[0]
-        dq_name = dq_names[dq_label]
-        dq_type = dq_types[dq_label]
-
-        dq_tags = tags + [dq_label]
-
-        # get triggers for this ifo
-        ifo_insp = [insp for insp in insps if (insp.ifo == ifo)]
-        assert len(ifo_insp) == 1, \
-            f"Received more than one inspiral file for {ifo}"
-        ifo_insp = ifo_insp[0]
-
-        # calculate template bins for this ifo
-        bin_templates_exe = PyCBCBinTemplatesDQExecutable(
-            workflow.cp,
-            'bin_templates',
-            ifos=ifo,
-            out_dir=output_dir,
-            tags=tags)
-        bin_templates_node = bin_templates_exe.create_node(workflow, ifo, bank)
-        workflow += bin_templates_node
-        template_bins_file = bin_templates_node.output_file
-
-        if dq_type == 'flag':
-            flag_file = dq_seg_file
-            flag_name = dq_name
-        else:
-            raise ValueError(f"{dq_type} dq support not yet implemented")
-
-        # calculate trigger rates during dq flags
-        bin_triggers_exe = PyCBCBinTriggerRatesDQExecutable(
-            workflow.cp,
-            'bin_trigger_rates_dq',
-            ifos=ifo,
-            out_dir=output_dir,
-            tags=dq_tags)
-        bin_triggers_node = bin_triggers_exe.create_node(
-            workflow,
-            flag_file,
-            flag_name,
-            analyzable_seg_file,
-            analyzable_name,
-            ifo_insp,
-            template_bins_file)
-        workflow += bin_triggers_node
-        output_files += bin_triggers_node.output_files
-        output_labels += [dq_label]
+    workflow += node
+    return node.output_files
 
-    logging.info("Finished setting up dq reranking")
-    return output_files, output_labels
+# keep namespace clean
+__all__ = ['make_psd_file', 'make_average_psd', 'setup_psd_calculate', 'merge_psds']
```

### Comparing `PyCBC-2.3.6/pycbc/workflow/grb_utils.py` & `PyCBC-2.4.0/pycbc/workflow/grb_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/inference_followups.py` & `PyCBC-2.4.0/pycbc/workflow/inference_followups.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/injection.py` & `PyCBC-2.4.0/pycbc/workflow/injection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/jobsetup.py` & `PyCBC-2.4.0/pycbc/workflow/jobsetup.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/matched_filter.py` & `PyCBC-2.4.0/pycbc/workflow/matched_filter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/minifollowups.py` & `PyCBC-2.4.0/pycbc/workflow/minifollowups.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 import logging, os.path
 from ligo import segments
-from pycbc.events import coinc
 from pycbc.workflow.core import Executable, FileList
 from pycbc.workflow.core import makedir, resolve_url_to_file
 from pycbc.workflow.plotting import PlotExecutable, requirestr, excludestr
 try:
     # Python 3
     from itertools import zip_longest
 except ImportError:
@@ -32,16 +31,15 @@
     """ Create a list of n length tuples
     """
     args = [iter(iterable)] * n
     return zip_longest(*args, fillvalue=fillvalue)
 
 def setup_foreground_minifollowups(workflow, coinc_file, single_triggers,
                        tmpltbank_file, insp_segs, insp_data_name,
-                       insp_anal_name, dax_output, out_dir,
-                       tags=None):
+                       insp_anal_name, dax_output, out_dir, tags=None):
     """ Create plots that followup the Nth loudest coincident injection
     from a statmap produced HDF file.
 
     Parameters
     ----------
     workflow: pycbc.workflow.Workflow
         The core workflow instance we are populating
@@ -54,16 +52,14 @@
     insp_segs: SegFile
        The segment file containing the data read and analyzed by each inspiral
        job.
     insp_data_name: str
         The name of the segmentlist storing data read.
     insp_anal_name: str
         The name of the segmentlist storing data analyzed.
-    dax_output : directory
-        Location of the dax outputs
     out_dir: path
         The directory to store minifollowups result plots and files
     tags: {None, optional}
         Tags to add to the minifollowups executables
 
     Returns
     -------
@@ -114,28 +110,26 @@
     workflow += node
 
     # execute this in a sub-workflow
     fil = node.output_files[0]
 
     # determine if a staging site has been specified
     job = SubWorkflow(fil.name, is_planned=False)
-    input_files = [tmpltbank_file, coinc_file, insp_segs] + \
-        single_triggers
+    input_files = [tmpltbank_file, coinc_file, insp_segs] + single_triggers
     job.add_inputs(*input_files)
     job.set_subworkflow_properties(map_file,
                                    staging_site=workflow.staging_site,
                                    cache_file=workflow.cache_file)
     job.add_into_workflow(workflow)
     logging.info('Leaving minifollowups module')
 
 def setup_single_det_minifollowups(workflow, single_trig_file, tmpltbank_file,
                                    insp_segs, insp_data_name, insp_anal_name,
                                    dax_output, out_dir, veto_file=None,
-                                   veto_segment_name=None, fg_file=None,
-                                   fg_name=None, statfiles=None,
+                                   veto_segment_name=None, statfiles=None,
                                    tags=None):
     """ Create plots that followup the Nth loudest clustered single detector
     triggers from a merged single detector trigger HDF file.
 
     Parameters
     ----------
     workflow: pycbc.workflow.Workflow
@@ -194,19 +188,16 @@
     node.add_opt('--inspiral-data-read-name', insp_data_name)
     node.add_opt('--inspiral-data-analyzed-name', insp_anal_name)
     node.add_opt('--instrument', curr_ifo)
     if veto_file is not None:
         assert(veto_segment_name is not None)
         node.add_input_opt('--veto-file', veto_file)
         node.add_opt('--veto-segment-name', veto_segment_name)
-    if fg_file is not None:
-        assert(fg_name is not None)
-        node.add_input_opt('--foreground-censor-file', fg_file)
-        node.add_opt('--foreground-segment-name', fg_name)
     if statfiles:
+        statfiles = statfiles.find_output_with_ifo(curr_ifo)
         node.add_input_list_opt('--statistic-files', statfiles)
     if tags:
         node.add_list_opt('--tags', tags)
     node.new_output_file_opt(workflow.analysis_time, '.dax', '--dax-file')
     node.new_output_file_opt(workflow.analysis_time, '.dax.map',
                              '--output-map')
 
@@ -345,193 +336,18 @@
     """Class to be used for to create workflow.Executable instances for the
     pycbc_plot_qscan executable. Basically inherits directly from
     PlotExecutable.
     """
     time_dependent_options = ['--channel-name', '--frame-type']
 
 
-def get_single_template_params(curr_idx, times, bank_data,
-                               bank_id, fsdt, tids):
-    """
-    A function to get the parameters needed for the make_single_template_files
-    function.
-
-    Parameters
-    ----------
-    curr_idx : int
-        The index of the event in the file
-    times : dictionary keyed on IFO of numpy arrays, dtype float
-        The array of trigger times for each detector
-    bank_data : dictionary or h5py file
-        Structure containing the bank information
-    bank_id : int
-        The template index within the bank
-    fsdt : dictionary of h5py files, keyed on IFO
-        The single-detector TRIGGER_MERGE files, keyed by IFO
-    tids : dictionary keyed on IFO of numpy arrays, dtype int
-        The trigger indexes in fsdt for each IFO
-
-    Returns
-    -------
-    params : dictionary
-        A dictionary containing the parameters needed for the event used
-
-    """
-    params = {}
-    for ifo in times:
-        params['%s_end_time' % ifo] = times[ifo][curr_idx]
-        try:
-            # Only present for precessing, so may not exist
-            params['u_vals_%s' % ifo] = \
-                                 fsdt[ifo][ifo]['u_vals'][tids[ifo][curr_idx]]
-        except:
-            pass
-
-    params['mean_time'] = coinc.mean_if_greater_than_zero(
-        [times[ifo][curr_idx] for ifo in times]
-    )[0]
-
-    params['mass1'] = bank_data['mass1'][bank_id]
-    params['mass2'] = bank_data['mass2'][bank_id]
-    params['spin1z'] = bank_data['spin1z'][bank_id]
-    params['spin2z'] = bank_data['spin2z'][bank_id]
-    params['f_lower'] = bank_data['f_lower'][bank_id]
-    if 'approximant' in bank_data:
-        params['approximant'] = bank_data['approximant'][bank_id]
-    # don't require precessing template info if not present
-    try:
-        params['spin1x'] = bank_data['spin1x'][bank_id]
-        params['spin1y'] = bank_data['spin1y'][bank_id]
-        params['spin2x'] = bank_data['spin2x'][bank_id]
-        params['spin2y'] = bank_data['spin2y'][bank_id]
-        params['inclination'] = bank_data['inclination'][bank_id]
-    except KeyError:
-        pass
-    return params
-
-
-def make_single_template_files(workflow, segs, ifo, data_read_name,
-                               analyzed_name, params, out_dir, inj_file=None,
-                               exclude=None, require=None, tags=None,
-                               store_file=False, use_mean_time=False,
-                               use_exact_inj_params=False):
-    """Function for creating jobs to run the pycbc_single_template code and
-    add these jobs to the workflow.
-
-    Parameters
-    -----------
-    workflow : workflow.Workflow instance
-        The pycbc.workflow.Workflow instance to add these jobs to.
-    segs : workflow.File instance
-        The pycbc.workflow.File instance that points to the XML file containing
-        the segment lists of data read in and data analyzed.
-    ifo: str
-        The name of the interferometer
-    data_read_name : str
-        The name of the segmentlist containing the data read in by each
-        inspiral job in the segs file.
-    analyzed_name : str
-        The name of the segmentlist containing the data analyzed by each
-        inspiral job in the segs file.
-    params : dictionary
-        A dictionary containing the parameters of the template to be used.
-        params[ifo+'end_time'] is required for all ifos in workflow.ifos.
-        If use_exact_inj_params is False then also need to supply values for
-        [mass1, mass2, spin1z, spin2x]. For precessing templates one also
-        needs to supply [spin1y, spin1x, spin2x, spin2y, inclination]
-        additionally for precession one must supply u_vals or
-        u_vals_+ifo for all ifos. u_vals is the ratio between h_+ and h_x to
-        use when constructing h(t). h(t) = (h_+ * u_vals) + h_x.
-    out_dir : str
-        Directory in which to store the output files.
-    inj_file : workflow.File (optional, default=None)
-        If given send this injection file to the job so that injections are
-        made into the data.
-    exclude : list (optional, default=None)
-        If given, then when considering which subsections in the ini file to
-        parse for options to add to single_template_plot, only use subsections
-        that *do not* match strings in this list.
-    require : list (optional, default=None)
-        If given, then when considering which subsections in the ini file to
-        parse for options to add to single_template_plot, only use subsections
-        matching strings in this list.
-    tags : list (optional, default=None)
-        The tags to use for this job.
-    store_file : boolean (optional, default=False)
-        Keep the output files of this job.
-    use_mean_time : boolean (optional, default=False)
-        Use the mean time as the center time for all ifos
-    use_exact_inj_params : boolean (optional, default=False)
-        If True do not use masses and spins listed in the params dictionary
-        but instead use the injection closest to the filter time as a template.
-
-    Returns
-    --------
-    output_files : workflow.FileList
-        The list of workflow.Files created in this function.
-    """
-    tags = [] if tags is None else tags
-    makedir(out_dir)
-    name = 'single_template'
-    secs = requirestr(workflow.cp.get_subsections(name), require)
-    secs = excludestr(secs, exclude)
-    secs = excludestr(secs, workflow.ifo_combinations)
-    # Reanalyze the time around the trigger in each detector
-    curr_exe = SingleTemplateExecutable(workflow.cp, 'single_template',
-                                        ifos=[ifo], out_dir=out_dir,
-                                        tags=tags)
-    start = int(params[ifo + '_end_time'])
-    end = start + 1
-    cseg = segments.segment([start, end])
-    node = curr_exe.create_node(valid_seg=cseg)
-
-    if use_exact_inj_params:
-        node.add_opt('--use-params-of-closest-injection')
-    else:
-        node.add_opt('--mass1', "%.6f" % params['mass1'])
-        node.add_opt('--mass2', "%.6f" % params['mass2'])
-        node.add_opt('--spin1z',"%.6f" % params['spin1z'])
-        node.add_opt('--spin2z',"%.6f" % params['spin2z'])
-        node.add_opt('--template-start-frequency',
-                     "%.6f" % params['f_lower'])
-        # Is this precessing?
-        if 'u_vals' in params or 'u_vals_%s' % ifo in params:
-            node.add_opt('--spin1x',"%.6f" % params['spin1x'])
-            node.add_opt('--spin1y',"%.6f" % params['spin1y'])
-            node.add_opt('--spin2x',"%.6f" % params['spin2x'])
-            node.add_opt('--spin2y',"%.6f" % params['spin2y'])
-            node.add_opt('--inclination',"%.6f" % params['inclination'])
-            try:
-                node.add_opt('--u-val',"%.6f" % params['u_vals'])
-            except:
-                node.add_opt('--u-val',
-                             "%.6f" % params['u_vals_%s' % ifo])
-
-    if params[ifo + '_end_time'] > 0 and not use_mean_time:
-        trig_time = params[ifo + '_end_time']
-    else:
-        trig_time = params['mean_time']
-
-    node.add_opt('--trigger-time', f"{trig_time:.6f}")
-    node.add_input_opt('--inspiral-segments', segs)
-    if inj_file is not None:
-        node.add_input_opt('--injection-file', inj_file)
-    node.add_opt('--data-read-name', data_read_name)
-    node.add_opt('--data-analyzed-name', analyzed_name)
-    node.new_output_file_opt(workflow.analysis_time, '.hdf',
-                             '--output-file', store_file=store_file)
-    workflow += node
-    return node.output_files
-
-
 def make_single_template_plots(workflow, segs, data_read_name, analyzed_name,
-                               params, out_dir, inj_file=None, exclude=None,
-                               data_segments=None,
-                               require=None, tags=None, params_str=None,
-                               use_exact_inj_params=False):
+                                  params, out_dir, inj_file=None, exclude=None,
+                                  require=None, tags=None, params_str=None,
+                                  use_exact_inj_params=False):
     """Function for creating jobs to run the pycbc_single_template code and
     to run the associated plotting code pycbc_single_template_plots and add
     these jobs to the workflow.
 
     Parameters
     -----------
     workflow : workflow.Workflow instance
@@ -563,73 +379,86 @@
         If given, then when considering which subsections in the ini file to
         parse for options to add to single_template_plot, only use subsections
         that *do not* match strings in this list.
     require : list (optional, default=None)
         If given, then when considering which subsections in the ini file to
         parse for options to add to single_template_plot, only use subsections
         matching strings in this list.
-    data_segments : dictionary of segment lists
-        Dictionary of segment lists keyed on the IFO. Used to decide if an
-        IFO is plotted if there is valid data. If not given, will plot if
-        the IFO produced a trigger which contributed to the event
     tags : list (optional, default=None)
         Add this list of tags to all jobs.
     params_str : str (optional, default=None)
         If given add this string to plot title and caption to describe the
         template that was used.
     use_exact_inj_params : boolean (optional, default=False)
         If True do not use masses and spins listed in the params dictionary
         but instead use the injection closest to the filter time as a template.
 
     Returns
     --------
-    hdf_files : workflow.FileList
-        The list of workflow.Files created by single_template jobs
-        in this function.
-    plot_files : workflow.FileList
-        The list of workflow.Files created by single_template_plot jobs
-        in this function.
+    output_files : workflow.FileList
+        The list of workflow.Files created in this function.
     """
     tags = [] if tags is None else tags
     makedir(out_dir)
     name = 'single_template_plot'
     secs = requirestr(workflow.cp.get_subsections(name), require)
     secs = excludestr(secs, exclude)
     secs = excludestr(secs, workflow.ifo_combinations)
-    hdf_files = FileList([])
-    plot_files = FileList([])
-    valid = {}
-    for ifo in workflow.ifos:
-        valid[ifo] = params['mean_time'] in data_segments[ifo] if data_segments \
-                else params['%s_end_time' % ifo] > 0
+    files = FileList([])
     for tag in secs:
         for ifo in workflow.ifos:
-            if not valid[ifo]:
-                # If the IFO is not being used, continue
+            if params['%s_end_time' % ifo] == -1.0:
                 continue
-            data = make_single_template_files(
-                workflow,
-                segs,
-                ifo,
-                data_read_name,
-                analyzed_name,
-                params,
-                out_dir,
-                inj_file=inj_file,
-                exclude=exclude,
-                require=require,
-                tags=tags + [tag],
-                store_file=False,
-                use_exact_inj_params=use_exact_inj_params
-            )
-            hdf_files += data
+            # Reanalyze the time around the trigger in each detector
+            curr_exe = SingleTemplateExecutable(workflow.cp, 'single_template',
+                                                ifos=[ifo], out_dir=out_dir,
+                                                tags=[tag] + tags)
+            start = int(params[ifo + '_end_time'])
+            end = start + 1
+            cseg = segments.segment([start, end])
+            node = curr_exe.create_node(valid_seg=cseg)
+
+            if use_exact_inj_params:
+                node.add_opt('--use-params-of-closest-injection')
+            else:
+                node.add_opt('--mass1', "%.6f" % params['mass1'])
+                node.add_opt('--mass2', "%.6f" % params['mass2'])
+                node.add_opt('--spin1z',"%.6f" % params['spin1z'])
+                node.add_opt('--spin2z',"%.6f" % params['spin2z'])
+                node.add_opt('--template-start-frequency',
+                             "%.6f" % params['f_lower'])
+                # Is this precessing?
+                if 'u_vals' in params or 'u_vals_%s' % ifo in params:
+                    node.add_opt('--spin1x',"%.6f" % params['spin1x'])
+                    node.add_opt('--spin1y',"%.6f" % params['spin1y'])
+                    node.add_opt('--spin2x',"%.6f" % params['spin2x'])
+                    node.add_opt('--spin2y',"%.6f" % params['spin2y'])
+                    node.add_opt('--inclination',"%.6f" % params['inclination'])
+                    try:
+                        node.add_opt('--u-val',"%.6f" % params['u_vals'])
+                    except:
+                        node.add_opt('--u-val',
+                                     "%.6f" % params['u_vals_%s' % ifo])
+
+            # str(numpy.float64) restricts to 2d.p. BE CAREFUL WITH THIS!!!
+            str_trig_time = '%.6f' %(params[ifo + '_end_time'])
+            node.add_opt('--trigger-time', str_trig_time)
+            node.add_input_opt('--inspiral-segments', segs)
+            if inj_file is not None:
+                node.add_input_opt('--injection-file', inj_file)
+            node.add_opt('--data-read-name', data_read_name)
+            node.add_opt('--data-analyzed-name', analyzed_name)
+            node.new_output_file_opt(workflow.analysis_time, '.hdf',
+                                     '--output-file', store_file=False)
+            data = node.output_files[0]
+            workflow += node
             # Make the plot for this trigger and detector
             node = PlotExecutable(workflow.cp, name, ifos=[ifo],
                               out_dir=out_dir, tags=[tag] + tags).create_node()
-            node.add_input_opt('--single-template-file', data[0])
+            node.add_input_opt('--single-template-file', data)
             node.new_output_file_opt(workflow.analysis_time, '.png',
                                      '--output-file')
             title="'%s SNR and chi^2 timeseries" %(ifo)
             if params_str is not None:
                 title+= " using %s" %(params_str)
             title+="'"
             node.add_opt('--plot-title', title)
@@ -641,16 +470,16 @@
             else:
                 caption += ". The template used has the following parameters: "
                 caption += "mass1=%s, mass2=%s, spin1z=%s, spin2z=%s'"\
                        %(params['mass1'], params['mass2'], params['spin1z'],
                          params['spin2z'])
             node.add_opt('--plot-caption', caption)
             workflow += node
-            plot_files += node.output_files
-    return hdf_files, plot_files
+            files += node.output_files
+    return files
 
 def make_plot_waveform_plot(workflow, params, out_dir, ifos, exclude=None,
                             require=None, tags=None):
     """ Add plot_waveform jobs to the workflow.
     """
     tags = [] if tags is None else tags
     makedir(out_dir)
@@ -692,25 +521,25 @@
     node.add_opt('--injection-index', str(injection_index))
     node.add_opt('--n-nearest', str(num))
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     files += node.output_files
     return files
 
-def make_coinc_info(workflow, singles, bank, coinc_file, out_dir,
+def make_coinc_info(workflow, singles, bank, coinc, out_dir,
                     n_loudest=None, trig_id=None, file_substring=None,
                     sort_order=None, sort_var=None, title=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     name = 'page_coincinfo'
     files = FileList([])
     node = PlotExecutable(workflow.cp, name, ifos=workflow.ifos,
                               out_dir=out_dir, tags=tags).create_node()
     node.add_input_list_opt('--single-trigger-files', singles)
-    node.add_input_opt('--statmap-file', coinc_file)
+    node.add_input_opt('--statmap-file', coinc)
     node.add_input_opt('--bank-file', bank)
     if sort_order:
         node.add_opt('--sort-order', sort_order)
     if sort_var:
         node.add_opt('--sort-variable', sort_var)
     if n_loudest is not None:
         node.add_opt('--n-loudest', str(n_loudest))
@@ -722,29 +551,27 @@
         node.add_opt('--statmap-file-subspace-name', file_substring)
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     files += node.output_files
     return files
 
 def make_sngl_ifo(workflow, sngl_file, bank_file, trigger_id, out_dir, ifo,
-                  statfiles=None, title=None, tags=None):
+                  title=None, tags=None):
     """Setup a job to create sngl detector sngl ifo html summary snippet.
     """
     tags = [] if tags is None else tags
     makedir(out_dir)
     name = 'page_snglinfo'
     files = FileList([])
     node = PlotExecutable(workflow.cp, name, ifos=[ifo],
                               out_dir=out_dir, tags=tags).create_node()
     node.add_input_opt('--single-trigger-file', sngl_file)
     node.add_input_opt('--bank-file', bank_file)
     node.add_opt('--trigger-id', str(trigger_id))
     node.add_opt('--instrument', ifo)
-    if statfiles is not None:
-        node.add_input_list_opt('--statistic-files', statfiles)
     if title is not None:
         node.add_opt('--title', f'"{title}"')
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     files += node.output_files
     return files
 
@@ -1015,226 +842,7 @@
 
     node.add_opt('--html-text', html_string)
     node.add_opt('--title', '"Events were skipped"')
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     files = node.output_files
     return files
-
-
-def make_upload_files(workflow, psd_files, snr_timeseries, xml_all,
-                      event_id, approximant, out_dir, channel_name,
-                      tags=None):
-    """
-    Make files including xml, skymap fits and plots for uploading to gracedb
-    for a given event
-
-    Parameters
-    ----------
-    psd_files: FileList([])
-        PSD Files from MERGE_PSDs for the search as appropriate for the
-        event
-    snr_timeseries: FileList([])
-        SNR timeseries files, one from each IFO, to add to the XML and plot
-        output from pysbs_single_template
-    xml_all: pycbc.workflow.core.File instance
-        XML file containing all events from the search
-    event_id: string
-        an integer to describe the event's position in the xml_all file
-    approximant: byte string
-        The approximant used for the template of the event, to be passed
-        to bayestar for sky location
-    out_dir:
-        The directory where all the output files should go
-    channel_name: string
-        Channel name to be added to the XML file to be uploaded
-    tags: {None, optional}
-        Tags to add to the minifollowups executables
-
-    Returns
-    -------
-    all_output_files: FileList
-        List of all output files from this process
-    """
-    indiv_xml_exe = Executable(
-        workflow.cp,
-        'generate_xml',
-        ifos=workflow.ifos, out_dir=out_dir,
-        tags=tags
-    )
-
-    xml_node = indiv_xml_exe.create_node()
-    xml_node.add_input_opt('--input-file', xml_all)
-    xml_node.add_opt('--event-id', event_id)
-    xml_node.add_input_list_opt('--psd-files', psd_files)
-    xml_node.add_input_list_opt('--snr-timeseries', snr_timeseries)
-    xml_node.add_opt('--channel-name', channel_name)
-    xml_node.new_output_file_opt(
-        workflow.analysis_time,
-        '.png',
-        '--snr-timeseries-plot',
-        tags=['snr']
-    )
-    xml_node.new_output_file_opt(
-        workflow.analysis_time,
-        '.png',
-        '--psd-plot',
-        tags=['psd']
-    )
-    xml_out = xml_node.new_output_file_opt(
-        workflow.analysis_time,
-        '.xml',
-        '--output-file'
-    )
-
-    workflow += xml_node
-
-    bayestar_exe = Executable(
-        workflow.cp,
-        'bayestar',
-        ifos=workflow.ifos,
-        out_dir=out_dir,
-        tags=tags
-    )
-
-    bayestar_node = bayestar_exe.create_node()
-    bayestar_node.add_input_opt('--event-xml', xml_out)
-    fits_out = bayestar_node.new_output_file_opt(
-        workflow.analysis_time,
-        '.fits',
-        '--output-file',
-    )
-
-    if approximant == b'SPAtmplt':
-        # Bayestar doesn't use the SPAtmplt approximant
-        approximant = b'TaylorF2'
-    if approximant is not None:
-        bayestar_node.add_opt('--waveform', approximant.decode())
-
-    workflow += bayestar_node
-
-    skymap_plot_exe = PlotExecutable(
-        workflow.cp,
-        'skymap_plot',
-        ifos=workflow.ifos,
-        out_dir=out_dir,
-        tags=tags
-    )
-
-    skymap_plot_node = skymap_plot_exe.create_node()
-    skymap_plot_node.add_input_opt('', fits_out)
-    skymap_plot_node.new_output_file_opt(
-        workflow.analysis_time,
-        '.png',
-        '-o',
-    )
-    workflow += skymap_plot_node
-
-    all_output_files = xml_node.output_files + bayestar_node.output_files + \
-        skymap_plot_node.output_files
-    return all_output_files
-
-
-def setup_upload_prep_minifollowups(workflow, coinc_file, xml_all_file,
-                                    single_triggers, psd_files,
-                                    tmpltbank_file, insp_segs, insp_data_name,
-                                    insp_anal_name, dax_output, out_dir,
-                                    tags=None):
-    """ Create plots that followup the Nth loudest coincident injection
-    from a statmap produced HDF file.
-
-    Parameters
-    ----------
-    workflow: pycbc.workflow.Workflow
-        The core workflow instance we are populating
-    coinc_file:
-    single_triggers: list of pycbc.workflow.File
-        A list cointaining the file objects associated with the merged
-        single detector trigger files for each ifo.
-    psd_files: list of pycbc.workflow.File
-        A list containing the file objects associated with the merged
-        psd files for each ifo.
-    xml_all_file : workflow file object
-        XML File containing all foreground events
-    tmpltbank_file: pycbc.workflow.File
-        The file object pointing to the HDF format template bank
-    insp_segs: SegFile
-       The segment file containing the data read and analyzed by each inspiral
-       job.
-       The segment file containing the data read and analyzed by each inspiral
-       job.
-    insp_data_name: str
-        The name of the segmentlist storing data read.
-    insp_anal_name: str
-        The name of the segmentlist storing data analyzed.
-    dax_output : directory
-        Location of the dax outputs
-    out_dir: path
-        The directory to store minifollowups result plots and files
-    tags: {None, optional}
-        Tags to add to the minifollowups executables
-
-    Returns
-    -------
-    layout: list
-        A list of tuples which specify the displayed file layout for the
-        minifollowups plots.
-    """
-    logging.info('Entering minifollowups module')
-
-    if not workflow.cp.has_section('workflow-minifollowups'):
-        logging.info('There is no [workflow-minifollowups] section in configuration file')
-        logging.info('Leaving minifollowups')
-        return
-
-    tags = [] if tags is None else tags
-    makedir(dax_output)
-    makedir(out_dir)
-
-    # turn the config file into a File class
-    config_path = os.path.abspath(dax_output + '/' + '_'.join(tags) + \
-                                  'upload_prep_minifollowup.ini')
-    workflow.cp.write(open(config_path, 'w'))
-
-    config_file = resolve_url_to_file(config_path)
-
-    exe = Executable(workflow.cp, 'upload_prep_minifollowup',
-                     ifos=workflow.ifos, out_dir=dax_output, tags=tags)
-
-    node = exe.create_node()
-    node.add_input_opt('--config-files', config_file)
-    node.add_input_opt('--xml-all-file', xml_all_file)
-    node.add_input_opt('--bank-file', tmpltbank_file)
-    node.add_input_opt('--statmap-file', coinc_file)
-    node.add_multiifo_input_list_opt('--single-detector-triggers',
-                                     single_triggers)
-    node.add_multiifo_input_list_opt('--psd-files', psd_files)
-    node.add_input_opt('--inspiral-segments', insp_segs)
-    node.add_opt('--inspiral-data-read-name', insp_data_name)
-    node.add_opt('--inspiral-data-analyzed-name', insp_anal_name)
-    if tags:
-        node.add_list_opt('--tags', tags)
-    node.new_output_file_opt(workflow.analysis_time, '.dax', '--dax-file')
-    node.new_output_file_opt(workflow.analysis_time, '.dax.map', '--output-map')
-
-    name = node.output_files[0].name
-    map_file = node.output_files[1]
-
-    node.add_opt('--workflow-name', name)
-    node.add_opt('--output-dir', out_dir)
-    node.add_opt('--dax-file-directory', '.')
-
-    workflow += node
-
-    # execute this in a sub-workflow
-    fil = node.output_files[0]
-
-    # determine if a staging site has been specified
-    job = SubWorkflow(fil.name, is_planned=False)
-    input_files = [xml_all_file, tmpltbank_file, coinc_file, insp_segs] + \
-        single_triggers + psd_files
-    job.add_inputs(*input_files)
-    job.set_subworkflow_properties(map_file,
-                                   staging_site=workflow.staging_site,
-                                   cache_file=workflow.cache_file)
-    job.add_into_workflow(workflow)
-    logging.info('Leaving minifollowups module')
```

### Comparing `PyCBC-2.3.6/pycbc/workflow/pegasus_files/pegasus-properties.conf` & `PyCBC-2.4.0/pycbc/workflow/pegasus_files/pegasus-properties.conf`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/pegasus_sites.py` & `PyCBC-2.4.0/pycbc/workflow/pegasus_sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 import urllib.parse
 from shutil import which
 from urllib.parse import urljoin
 from urllib.request import pathname2url
 from Pegasus.api import Directory, FileServer, Site, Operation, Namespace
 from Pegasus.api import Arch, OS, SiteCatalog
 
-from pycbc.version import last_release, version, release  # noqa
-
-if release == 'True':
-    sing_version = version
-else:
-    sing_version = last_release
+from pycbc.version import last_release  # noqa
 
 # NOTE urllib is weird. For some reason it only allows known schemes and will
 # give *wrong* results, rather then failing, if you use something like gsiftp
 # We can add schemes explicitly, as below, but be careful with this!
 urllib.parse.uses_relative.append('gsiftp')
 urllib.parse.uses_netloc.append('gsiftp')
 
@@ -219,15 +214,15 @@
     site.add_profiles(Namespace.CONDOR, key="+SingularityCleanEnv",
                       value="True")
     site.add_profiles(Namespace.CONDOR, key="Requirements",
                       value="(HAS_SINGULARITY =?= TRUE) && "
                             "(HAS_LIGO_FRAMES =?= True) && "
                             "(IS_GLIDEIN =?= True)")
     cvmfs_loc = '"/cvmfs/singularity.opensciencegrid.org/pycbc/pycbc-el8:v'
-    cvmfs_loc += sing_version + '"'
+    cvmfs_loc += last_release + '"'
     site.add_profiles(Namespace.CONDOR, key="+SingularityImage",
                       value=cvmfs_loc)
     # On OSG failure rate is high
     site.add_profiles(Namespace.DAGMAN, key="retry", value="4")
     site.add_profiles(Namespace.ENV, key="LAL_DATA_PATH",
                       value="/cvmfs/software.igwn.org/pycbc/lalsuite-extra/current/share/lalsimulation")
     # Add MKL location to LD_LIBRARY_PATH for OSG
```

### Comparing `PyCBC-2.3.6/pycbc/workflow/pegasus_workflow.py` & `PyCBC-2.4.0/pycbc/workflow/pegasus_workflow.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/plotting.py` & `PyCBC-2.4.0/pycbc/workflow/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,45 +25,41 @@
 This module is responsible for setting up plotting jobs.
 https://ldas-jobs.ligo.caltech.edu/~cbc/docs/pycbc/NOTYETCREATED.html
 """
 from urllib.request import pathname2url
 from urllib.parse import urljoin
 from pycbc.workflow.core import File, FileList, makedir, Executable
 
-
 def excludestr(tags, substr):
     if substr is None:
         return tags
     if isinstance(substr, list):
         if len(substr) > 1:
             tags = excludestr(tags, substr[1:])
         substr = substr[0]
     return [tag for tag in tags if substr not in tag]
 
-
 def requirestr(tags, substr):
     if substr is None:
         return tags
     return [tag for tag in tags if substr in tag]
 
-
 class PlotExecutable(Executable):
     """ plot executable
     """
     current_retention_level = Executable.FINAL_RESULT
 
     # plots and final results should get the highest priority
     # on the job queue
     def create_node(self, **kwargs):
         node = Executable.create_node(self, **kwargs)
         node.set_priority(1000)
         return node
 
-
-def make_template_plot(workflow, bank_file, out_dir, bins=None,
+def make_template_plot(workflow, bank_file, out_dir,bins=None, 
                        tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'plot_bank', ifos=workflow.ifos,
                           out_dir=out_dir, tags=tags).create_node()
     node.add_input_opt('--bank-file', bank_file)
 
@@ -72,15 +68,14 @@
     if bins:
         node.add_opt('--background-bins', bins)
 
     node.new_output_file_opt(workflow.analysis_time, '.png', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_range_plot(workflow, psd_files, out_dir, exclude=None, require=None,
                    tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_range'), require)
     secs = excludestr(secs, exclude)
     secs = excludestr(secs, workflow.ifo_combinations)
@@ -90,15 +85,14 @@
                               out_dir=out_dir, tags=[tag] + tags).create_node()
         node.add_input_list_opt('--psd-files', psd_files)
         node.new_output_file_opt(workflow.analysis_time, '.png', '--output-file')
         workflow += node
         files += node.output_files
     return files
 
-
 def make_spectrum_plot(workflow, psd_files, out_dir, tags=None,
                        hdf_group=None, precalc_psd_files=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'plot_spectrum', ifos=workflow.ifos,
                           out_dir=out_dir, tags=tags).create_node()
     node.add_input_list_opt('--psd-files', psd_files)
@@ -108,45 +102,41 @@
         node.add_opt('--hdf-group', hdf_group)
     if precalc_psd_files is not None and len(precalc_psd_files) == 1:
         node.add_input_list_opt('--psd-file', precalc_psd_files)
 
     workflow += node
     return node.output_files[0]
 
-
 def make_segments_plot(workflow, seg_files, out_dir, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'plot_segments', ifos=workflow.ifos,
                          out_dir=out_dir, tags=tags).create_node()
     node.add_input_list_opt('--segment-files', seg_files)
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
 
-
 def make_gating_plot(workflow, insp_files, out_dir, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'plot_gating', ifos=workflow.ifos,
                           out_dir=out_dir, tags=tags).create_node()
     node.add_input_list_opt('--input-file', insp_files)
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
 
-
 def make_throughput_plot(workflow, insp_files, out_dir, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'plot_throughput', ifos=workflow.ifos,
                           out_dir=out_dir, tags=tags).create_node()
     node.add_input_list_opt('--input-file', insp_files)
     node.new_output_file_opt(workflow.analysis_time, '.png', '--output-file')
     workflow += node
 
-
 def make_foreground_table(workflow, trig_file, bank_file, out_dir,
                           singles=None, extension='.html', tags=None,
                           hierarchical_level=None):
 
     if hierarchical_level is not None and tags:
         tags = [("HIERARCHICAL_LEVEL_{:02d}".format(
                 hierarchical_level))] + tags
@@ -166,15 +156,14 @@
         node.add_opt('--use-hierarchical-level', hierarchical_level)
     if singles is not None:
         node.add_input_list_opt('--single-detector-triggers', singles)
     node.new_output_file_opt(bank_file.segment, extension, '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_sensitivity_plot(workflow, inj_file, out_dir, exclude=None,
                          require=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_sensitivity'), require)
     secs = excludestr(secs, exclude)
     secs = excludestr(secs, workflow.ifo_combinations)
@@ -184,15 +173,14 @@
                     out_dir=out_dir, tags=[tag] + tags).create_node()
         node.add_input_opt('--injection-file', inj_file)
         node.new_output_file_opt(inj_file.segment, '.png', '--output-file')
         workflow += node
         files += node.output_files
     return files
 
-
 def make_coinc_snrchi_plot(workflow, inj_file, inj_trig, stat_file, trig_file,
                           out_dir, exclude=None, require=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_coinc_snrchi'), require)
     secs = excludestr(secs, exclude)
     secs = excludestr(secs, workflow.ifo_combinations)
@@ -207,15 +195,14 @@
         node.add_input_opt('--coinc-statistic-file', stat_file)
         node.add_input_opt('--single-trigger-file', trig_file)
         node.new_output_file_opt(inj_file.segment, '.png', '--output-file')
         workflow += node
         files += node.output_files
     return files
 
-
 def make_inj_table(workflow, inj_file, out_dir, missed=False, singles=None,
                   tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'page_injections', ifos=workflow.ifos,
                     out_dir=out_dir, tags=tags).create_node()
 
@@ -226,15 +213,14 @@
     if singles is not None:
         node.add_multiifo_input_list_opt('--single-trigger-files', singles)
 
     node.new_output_file_opt(inj_file.segment, '.html', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_seg_table(workflow, seg_files, seg_names, out_dir, tags=None,
                   title_text=None, description=None):
     """ Creates a node in the workflow for writing the segment summary
     table. Returns a File instances for the output file.
     """
     seg_files = list(seg_files)
     seg_names = list(seg_names)
@@ -252,15 +238,14 @@
         node.add_opt('--description', "'" + description + "'")
     if title_text:
         node.add_opt('--title-text', "'" + title_text + "'")
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_veto_table(workflow, out_dir, vetodef_file=None, tags=None):
     """ Creates a node in the workflow for writing the veto_definer
     table. Returns a File instances for the output file.
     """
     if vetodef_file is None:
         if not workflow.cp.has_option_tags("workflow-segments",
                                            "segments-veto-definer-file", []):
@@ -279,15 +264,14 @@
     node = PlotExecutable(workflow.cp, 'page_vetotable', ifos=workflow.ifos,
                     out_dir=out_dir, tags=tags).create_node()
     node.add_input_opt('--veto-definer-file', vdf_file)
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_seg_plot(workflow, seg_files, out_dir, seg_names=None, tags=None):
     """ Creates a node in the workflow for plotting science, and veto segments.
     """
     seg_files = list(seg_files)
     if tags is None: tags = []
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'page_segplot', ifos=workflow.ifos,
@@ -298,15 +282,14 @@
         quoted_seg_names.append("'" + s + "'")
     node.add_opt('--segment-names', ' '.join(quoted_seg_names))
     node.add_opt('--ifos', ' '.join(workflow.ifos))
     node.new_output_file_opt(workflow.analysis_time, '.html', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_ifar_plot(workflow, trigger_file, out_dir, tags=None,
                    hierarchical_level=None, executable='page_ifar'):
     """ Creates a node in the workflow for plotting cumulative histogram
     of IFAR values.
     """
 
     if hierarchical_level is not None and tags:
@@ -324,15 +307,14 @@
     node.add_input_opt('--trigger-file', trigger_file)
     if hierarchical_level is not None:
         node.add_opt('--use-hierarchical-level', hierarchical_level)
     node.new_output_file_opt(workflow.analysis_time, '.png', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_snrchi_plot(workflow, trig_files, veto_file, veto_name,
                      out_dir, exclude=None, require=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_snrchi'), require)
     secs = excludestr(secs, exclude)
     secs = excludestr(secs, workflow.ifo_combinations)
@@ -351,15 +333,14 @@
                 node.add_input_opt('--veto-file', veto_file)
                 node.add_opt('--segment-name', veto_name)
             node.new_output_file_opt(trig_file.segment, '.png', '--output-file')
             workflow += node
             files += node.output_files
     return files
 
-
 def make_foundmissed_plot(workflow, inj_file, out_dir, exclude=None,
                          require=None, tags=None):
     if tags is None:
         tags = []
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_foundmissed'), require)
     secs = excludestr(secs, exclude)
@@ -372,15 +353,14 @@
         ext = '.html' if exe.has_opt('dynamic') else '.png'
         node.add_input_opt('--injection-file', inj_file)
         node.new_output_file_opt(inj_file.segment, ext, '--output-file')
         workflow += node
         files += node.output_files
     return files
 
-
 def make_snrratehist_plot(workflow, bg_file, out_dir, closed_box=False,
                           tags=None, hierarchical_level=None):
 
     if hierarchical_level is not None and tags:
         tags = [("HIERARCHICAL_LEVEL_{:02d}".format(
                 hierarchical_level))] + tags
     elif hierarchical_level is not None and not tags:
@@ -400,15 +380,14 @@
     if closed_box:
         node.add_opt('--closed-box')
 
     node.new_output_file_opt(bg_file.segment, '.png', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_snrifar_plot(workflow, bg_file, out_dir, closed_box=False,
                      cumulative=True, tags=None, hierarchical_level=None):
 
     if hierarchical_level is not None and tags:
         tags = [("HIERARCHICAL_LEVEL_{:02d}".format(
                 hierarchical_level))] + tags
     elif hierarchical_level is not None and not tags:
@@ -430,15 +409,14 @@
     if not cumulative:
         node.add_opt('--not-cumulative')
 
     node.new_output_file_opt(bg_file.segment, '.png', '--output-file')
     workflow += node
     return node.output_files[0]
 
-
 def make_results_web_page(workflow, results_dir, template='orange',
                           explicit_dependencies=None):
     template_path = 'templates/'+template+'.html'
 
     out_dir = workflow.cp.get('results_page', 'output-path')
     makedir(out_dir)
     node = PlotExecutable(workflow.cp, 'results_page', ifos=workflow.ifos,
@@ -446,15 +424,14 @@
     node.add_opt('--plots-dir', results_dir)
     node.add_opt('--template-file', template_path)
     workflow += node
     if explicit_dependencies is not None:
         for dep in explicit_dependencies:
             workflow.add_explicit_dependancy(dep, node)
 
-
 def make_single_hist(workflow, trig_file, veto_file, veto_name,
                      out_dir, bank_file=None, exclude=None,
                      require=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_hist'), require)
     secs = excludestr(secs, exclude)
@@ -472,15 +449,14 @@
         if bank_file:
             node.add_input_opt('--bank-file', bank_file)
         node.new_output_file_opt(trig_file.segment, '.png', '--output-file')
         workflow += node
         files += node.output_files
     return files
 
-
 def make_binned_hist(workflow, trig_file, veto_file, veto_name,
                      out_dir, bank_file, exclude=None,
                      require=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_binnedhist'), require)
     secs = excludestr(secs, exclude)
@@ -498,15 +474,14 @@
         node.add_input_opt('--trigger-file', trig_file)
         node.add_input_opt('--bank-file', bank_file)
         node.new_output_file_opt(trig_file.segment, '.png', '--output-file')
         workflow += node
         files += node.output_files
     return files
 
-
 def make_singles_plot(workflow, trig_files, bank_file, veto_file, veto_name,
                      out_dir, exclude=None, require=None, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
     secs = requirestr(workflow.cp.get_subsections('plot_singles'), require)
     secs = excludestr(secs, exclude)
     secs = excludestr(secs, workflow.ifo_combinations)
@@ -526,45 +501,75 @@
             node.add_opt('--detector', trig_file.ifo)
             node.add_input_opt('--single-trig-file', trig_file)
             node.new_output_file_opt(trig_file.segment, '.png', '--output-file')
             workflow += node
             files += node.output_files
     return files
 
-
-def make_dq_flag_trigger_rate_plot(workflow, dq_file, dq_label, out_dir, tags=None):
+def make_dq_timeseries_trigger_rate_plot(workflow, dq_files, out_dir, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
-    node = PlotExecutable(workflow.cp, 'plot_dq_flag_likelihood',
-                          ifos=dq_file.ifo, out_dir=out_dir,
-                          tags=tags).create_node()
-    node.add_input_opt('--dq-file', dq_file)
-    node.add_opt('--dq-label', dq_label)
-    node.add_opt('--ifo', dq_file.ifo)
-    node.new_output_file_opt(dq_file.segment, '.png', '--output-file')
-    workflow += node
-    return node.output_files[0]
-
+    files = FileList([])
+    for dq_file in dq_files:
+        if workflow.cp.has_option_tags('bin_trigger_rates_dq',
+                                       'background-bins', tags=tags):
+            background_bins = \
+                          workflow.cp.get_opt_tags('bin_trigger_rates_dq',
+                                              'background-bins', tags=tags)
+            bin_names = [tuple(bbin.split(':'))[0] for bbin
+                                             in background_bins.split(' ')]
+        else: bin_names = ['all_bin']
+        for bbin in bin_names:
+            plot_tags = [bbin] + tags
+            node = PlotExecutable(workflow.cp, 'plot_dq_likelihood_vs_time',
+                        ifos=dq_file.ifo,
+                        out_dir=out_dir,
+                        tags=plot_tags).create_node()
+            node.add_opt('--ifo', dq_file.ifo)
+            node.add_opt('--background-bin', bbin)
+            node.add_input_opt('--dq-file', dq_file)
+            node.new_output_file_opt(dq_file.segment, '.png', '--output-file')
+            workflow += node
+            files += node.output_files
+    return files
 
-def make_dq_segment_table(workflow, dq_file, out_dir, tags=None):
+def make_dq_percentile_plot(workflow, dq_files, out_dir, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
-    node = PlotExecutable(workflow.cp, 'page_dq_table', ifos=dq_file.ifo,
-                          out_dir=out_dir, tags=tags).create_node()
-    node.add_input_opt('--dq-file', dq_file)
-    node.add_opt('--ifo', dq_file.ifo)
-    node.new_output_file_opt(dq_file.segment, '.html', '--output-file')
-    workflow += node
-    return node.output_files[0]
-
+    files = FileList([])
+    for dq_file in dq_files:
+        if workflow.cp.has_option_tags('bin_trigger_rates_dq',
+                                       'background-bins', tags=tags):
+            background_bins = \
+                          workflow.cp.get_opt_tags('bin_trigger_rates_dq',
+                                              'background-bins', tags=tags)
+            bin_names = [tuple(bbin.split(':'))[0] for bbin
+                                             in background_bins.split(' ')]
+        else: bin_names = ['all_bin']
+        for bbin in bin_names:
+            plot_tags = [bbin] + tags
+            node = PlotExecutable(workflow.cp, 'plot_dq_percentiles',
+                        ifos=dq_file.ifo,
+                        out_dir=out_dir,
+                        tags=plot_tags).create_node()
+            node.add_opt('--ifo', dq_file.ifo)
+            node.add_opt('--background-bin', bbin)
+            node.add_input_opt('--dq-file', dq_file)
+            node.new_output_file_opt(dq_file.segment, '.png', '--output-file')
+            workflow += node
+            files += node.output_files
+    return files
 
-def make_template_bin_table(workflow, dq_file, out_dir, tags=None):
+def make_dq_flag_trigger_rate_plot(workflow, dq_files, out_dir, tags=None):
     tags = [] if tags is None else tags
     makedir(out_dir)
-    node = PlotExecutable(workflow.cp, 'page_template_bin_table',
-                          ifos=dq_file.ifo, out_dir=out_dir,
-                          tags=tags).create_node()
-    node.add_input_opt('--dq-file', dq_file)
-    node.add_opt('--ifo', dq_file.ifo)
-    node.new_output_file_opt(dq_file.segment, '.html', '--output-file')
-    workflow += node
-    return node.output_files[0]
+    files = FileList([])
+    for dq_file in dq_files:
+        node = PlotExecutable(workflow.cp, 'plot_dq_flag_likelihood',
+                              ifos=dq_file.ifo, out_dir=out_dir,
+                              tags=tags).create_node()
+        node.add_input_opt('--dq-file', dq_file)
+        node.add_opt('--ifo', dq_file.ifo)
+        node.new_output_file_opt(dq_file.segment, '.png', '--output-file')
+        workflow += node
+        files += node.output_files
+    return files
```

### Comparing `PyCBC-2.3.6/pycbc/workflow/psdfiles.py` & `PyCBC-2.4.0/pycbc/workflow/psdfiles.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/segment.py` & `PyCBC-2.4.0/pycbc/workflow/segment.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/splittable.py` & `PyCBC-2.4.0/pycbc/workflow/splittable.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/tmpltbank.py` & `PyCBC-2.4.0/pycbc/workflow/tmpltbank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pycbc/workflow/versioning.py` & `PyCBC-2.4.0/pycbc/workflow/versioning.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/pyproject.toml` & `PyCBC-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/setup.py` & `PyCBC-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             return ''
 
     # If this is a pycbc git repo always populate version information using GIT
     try:
         vinfo = _version_helper.generate_git_version_info()
     except:
         vinfo = vdummy()
-        vinfo.version = '2.3.6'
+        vinfo.version = '2.4.0'
         vinfo.release = 'True'
 
     version_script = f"""# coding: utf-8
 # Generated by setup.py for PyCBC on {vinfo.build_date}.
 
 # general info
 version = '{vinfo.version}'
```

### Comparing `PyCBC-2.3.6/test/bankvetotest.py` & `PyCBC-2.4.0/test/bankvetotest.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/fft_base.py` & `PyCBC-2.4.0/test/fft_base.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/lalsim.py` & `PyCBC-2.4.0/test/lalsim.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_array.py` & `PyCBC-2.4.0/test/test_array.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_array_lal.py` & `PyCBC-2.4.0/test/test_array_lal.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_autochisq.py` & `PyCBC-2.4.0/test/test_autochisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_calibration.py` & `PyCBC-2.4.0/test/test_calibration.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_chisq.py` & `PyCBC-2.4.0/test/test_chisq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_coinc_stat.py` & `PyCBC-2.4.0/test/test_coinc_stat.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_conversions.py` & `PyCBC-2.4.0/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_correlate.py` & `PyCBC-2.4.0/test/test_correlate.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_cuts.py` & `PyCBC-2.4.0/test/test_cuts.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_detector.py` & `PyCBC-2.4.0/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_distributions.py` & `PyCBC-2.4.0/test/test_distributions.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_dq.py` & `PyCBC-2.4.0/test/test_dq.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_fft_mkl_threaded.py` & `PyCBC-2.4.0/test/test_fft_mkl_threaded.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_fft_unthreaded.py` & `PyCBC-2.4.0/test/test_fft_unthreaded.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_fftw_openmp.py` & `PyCBC-2.4.0/test/test_fftw_openmp.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_fftw_pthreads.py` & `PyCBC-2.4.0/test/test_fftw_pthreads.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_frame.py` & `PyCBC-2.4.0/test/test_frame.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_frequencyseries.py` & `PyCBC-2.4.0/test/test_frequencyseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_infmodel.py` & `PyCBC-2.4.0/test/test_infmodel.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_injection.py` & `PyCBC-2.4.0/test/test_injection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_io_live.py` & `PyCBC-2.4.0/test/test_io_live.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_live_coinc_compare.py` & `PyCBC-2.4.0/test/test_live_coinc_compare.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_matchedfilter.py` & `PyCBC-2.4.0/test/test_matchedfilter.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_noise.py` & `PyCBC-2.4.0/test/test_noise.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_pnutils.py` & `PyCBC-2.4.0/test/test_pnutils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_psd.py` & `PyCBC-2.4.0/test/test_psd.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_resample.py` & `PyCBC-2.4.0/test/test_resample.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_schemes.py` & `PyCBC-2.4.0/test/test_schemes.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_significance_module.py` & `PyCBC-2.4.0/test/test_significance_module.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_skymax.py` & `PyCBC-2.4.0/test/test_skymax.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_spatmplt.py` & `PyCBC-2.4.0/test/test_spatmplt.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_threshold.py` & `PyCBC-2.4.0/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_timeseries.py` & `PyCBC-2.4.0/test/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_tmpltbank.py` & `PyCBC-2.4.0/test/test_tmpltbank.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_transforms.py` & `PyCBC-2.4.0/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_waveform.py` & `PyCBC-2.4.0/test/test_waveform.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/test_waveform_utils.py` & `PyCBC-2.4.0/test/test_waveform_utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/test/utils.py` & `PyCBC-2.4.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/benchmarking/absolute_times.py` & `PyCBC-2.4.0/tools/benchmarking/absolute_times.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/einsteinathome/check_GW150914_detection.py` & `PyCBC-2.4.0/tools/einsteinathome/check_GW150914_detection.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/static/hooks/hook-pycbc.py` & `PyCBC-2.4.0/tools/static/hooks/hook-pycbc.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/static/runtime-scipy.py` & `PyCBC-2.4.0/tools/static/runtime-scipy.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/timing/arr_perf.py` & `PyCBC-2.4.0/tools/timing/arr_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/timing/banksim/banksim.py` & `PyCBC-2.4.0/tools/timing/banksim/banksim.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/timing/correlate_perf.py` & `PyCBC-2.4.0/tools/timing/correlate_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/timing/fft_perf.py` & `PyCBC-2.4.0/tools/timing/fft_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/timing/match_perf.py` & `PyCBC-2.4.0/tools/timing/match_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tools/timing/wav_perf.py` & `PyCBC-2.4.0/tools/timing/wav_perf.py`

 * *Files identical despite different names*

### Comparing `PyCBC-2.3.6/tox.ini` & `PyCBC-2.4.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     {[base]deps}
 setenv = PYCBC_TEST_TYPE=inference
 commands = bash tools/pycbc_test_suite.sh
 
 [testenv:py-docs]
 deps =
     {[base]deps}
+    ; Needed for `BBHx` package to work with PyCBC
+    git+https://github.com/mikekatz04/BBHx.git; sys_platform == 'linux'
+    git+https://github.com/ConWea/BBHX-waveform-model.git; sys_platform == 'linux'
 conda_deps=
     mysqlclient
     gcc_linux-64>=12.2.0
     gxx_linux-64>=12.2.0
     binutils_linux-64>=2.39
     gsl
     lapack==3.6.1
```

