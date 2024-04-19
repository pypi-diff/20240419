# Comparing `tmp/torch_geometric-2.5.2.tar.gz` & `tmp/torch_geometric-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_geometric-2.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "torch_geometric-2.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `torch_geometric-2.5.2.tar` & `torch_geometric-2.5.3.tar`

### file list

```diff
@@ -1,606 +1,606 @@
--rw-r--r--   0        0        0    61058 2024-03-20 18:30:51.578597 torch_geometric-2.5.2/README.md
--rw-r--r--   0        0        0     5178 2024-03-20 18:31:22.923835 torch_geometric-2.5.2/pyproject.toml
--rw-r--r--   0        0        0     1197 2024-03-20 18:31:22.924398 torch_geometric-2.5.2/torch_geometric/__init__.py
--rw-r--r--   0        0        0     1053 2024-01-16 19:07:07.463648 torch_geometric-2.5.2/torch_geometric/_compile.py
--rw-r--r--   0        0        0     1575 2024-02-15 14:55:33.351472 torch_geometric-2.5.2/torch_geometric/backend.py
--rw-r--r--   0        0        0    16514 2023-12-21 07:51:56.890107 torch_geometric-2.5.2/torch_geometric/config_store.py
--rw-r--r--   0        0        0      352 2023-04-09 09:43:57.297670 torch_geometric-2.5.2/torch_geometric/contrib/__init__.py
--rw-r--r--   0        0        0       23 2023-04-09 09:43:57.297729 torch_geometric-2.5.2/torch_geometric/contrib/datasets/__init__.py
--rw-r--r--   0        0        0      396 2023-09-21 09:55:53.973502 torch_geometric-2.5.2/torch_geometric/contrib/explain/__init__.py
--rw-r--r--   0        0        0    16972 2023-12-21 07:51:56.890605 torch_geometric-2.5.2/torch_geometric/contrib/explain/pgm_explainer.py
--rw-r--r--   0        0        0       72 2023-04-09 09:43:57.298115 torch_geometric-2.5.2/torch_geometric/contrib/nn/__init__.py
--rw-r--r--   0        0        0       23 2023-04-09 09:43:57.298178 torch_geometric-2.5.2/torch_geometric/contrib/nn/conv/__init__.py
--rw-r--r--   0        0        0      113 2023-04-09 09:43:57.298237 torch_geometric-2.5.2/torch_geometric/contrib/nn/models/__init__.py
--rw-r--r--   0        0        0    33280 2023-11-23 19:01:39.064213 torch_geometric-2.5.2/torch_geometric/contrib/nn/models/rbcd_attack.py
--rw-r--r--   0        0        0       23 2023-04-09 09:43:57.298451 torch_geometric-2.5.2/torch_geometric/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3882 2024-02-15 14:55:33.351611 torch_geometric-2.5.2/torch_geometric/data/__init__.py
--rw-r--r--   0        0        0     8767 2023-12-28 11:34:13.526894 torch_geometric-2.5.2/torch_geometric/data/batch.py
--rw-r--r--   0        0        0    12471 2024-01-07 13:37:00.549321 torch_geometric-2.5.2/torch_geometric/data/collate.py
--rw-r--r--   0        0        0    43328 2023-12-21 07:51:56.891442 torch_geometric-2.5.2/torch_geometric/data/data.py
--rw-r--r--   0        0        0    21247 2023-12-31 08:35:31.851688 torch_geometric-2.5.2/torch_geometric/data/database.py
--rw-r--r--   0        0        0     3083 2023-12-28 11:34:13.528318 torch_geometric-2.5.2/torch_geometric/data/datapipes.py
--rw-r--r--   0        0        0    16402 2024-03-05 12:38:29.026374 torch_geometric-2.5.2/torch_geometric/data/dataset.py
--rw-r--r--   0        0        0     1889 2024-02-15 14:55:33.351729 torch_geometric-2.5.2/torch_geometric/data/download.py
--rw-r--r--   0        0        0     2324 2023-12-28 11:34:13.528775 torch_geometric-2.5.2/torch_geometric/data/extract.py
--rw-r--r--   0        0        0    20805 2024-03-20 18:30:51.591644 torch_geometric-2.5.2/torch_geometric/data/feature_store.py
--rw-r--r--   0        0        0    13916 2024-03-20 18:30:51.591937 torch_geometric-2.5.2/torch_geometric/data/graph_store.py
--rw-r--r--   0        0        0    47550 2024-02-15 14:55:33.351880 torch_geometric-2.5.2/torch_geometric/data/hetero_data.py
--rw-r--r--   0        0        0     8294 2023-12-28 11:34:13.529285 torch_geometric-2.5.2/torch_geometric/data/hypergraph_data.py
--rw-r--r--   0        0        0    13513 2024-03-05 12:38:29.027252 torch_geometric-2.5.2/torch_geometric/data/in_memory_dataset.py
--rw-r--r--   0        0        0      178 2023-04-09 09:43:57.300134 torch_geometric-2.5.2/torch_geometric/data/lightning/__init__.py
--rw-r--r--   0        0        0    29244 2024-02-15 14:55:33.352116 torch_geometric-2.5.2/torch_geometric/data/lightning/datamodule.py
--rw-r--r--   0        0        0      463 2023-11-23 19:01:39.066347 torch_geometric-2.5.2/torch_geometric/data/makedirs.py
--rw-r--r--   0        0        0     6629 2023-12-28 11:34:13.529685 torch_geometric-2.5.2/torch_geometric/data/on_disk_dataset.py
--rw-r--r--   0        0        0     4503 2023-12-28 11:34:13.530160 torch_geometric-2.5.2/torch_geometric/data/remote_backend_utils.py
--rw-r--r--   0        0        0     5319 2023-12-31 08:35:31.852239 torch_geometric-2.5.2/torch_geometric/data/separate.py
--rw-r--r--   0        0        0    31562 2024-02-15 14:55:33.352303 torch_geometric-2.5.2/torch_geometric/data/storage.py
--rw-r--r--   0        0        0     5375 2023-12-28 11:34:13.531203 torch_geometric-2.5.2/torch_geometric/data/summary.py
--rw-r--r--   0        0        0    10055 2023-12-21 07:51:56.893168 torch_geometric-2.5.2/torch_geometric/data/temporal.py
--rw-r--r--   0        0        0     1089 2023-12-21 07:51:56.893489 torch_geometric-2.5.2/torch_geometric/data/view.py
--rw-r--r--   0        0        0     5637 2023-11-23 19:01:39.067314 torch_geometric-2.5.2/torch_geometric/datasets/__init__.py
--rw-r--r--   0        0        0     4471 2023-12-21 07:51:56.893651 torch_geometric-2.5.2/torch_geometric/datasets/actor.py
--rw-r--r--   0        0        0     5666 2023-12-21 07:51:56.893783 torch_geometric-2.5.2/torch_geometric/datasets/airfrans.py
--rw-r--r--   0        0        0     3913 2023-12-21 07:51:56.893895 torch_geometric-2.5.2/torch_geometric/datasets/airports.py
--rw-r--r--   0        0        0     3179 2023-12-21 07:51:56.894019 torch_geometric-2.5.2/torch_geometric/datasets/amazon.py
--rw-r--r--   0        0        0     3362 2023-12-21 07:51:56.894133 torch_geometric-2.5.2/torch_geometric/datasets/amazon_book.py
--rw-r--r--   0        0        0     3964 2024-02-15 14:55:33.352468 torch_geometric-2.5.2/torch_geometric/datasets/amazon_products.py
--rw-r--r--   0        0        0     5178 2023-12-21 07:51:56.894398 torch_geometric-2.5.2/torch_geometric/datasets/aminer.py
--rw-r--r--   0        0        0     5455 2023-12-21 07:51:56.894546 torch_geometric-2.5.2/torch_geometric/datasets/aqsol.py
--rw-r--r--   0        0        0     5975 2024-02-15 14:55:33.352805 torch_geometric-2.5.2/torch_geometric/datasets/attributed_graph_dataset.py
--rw-r--r--   0        0        0     4258 2023-12-21 07:51:56.894811 torch_geometric-2.5.2/torch_geometric/datasets/ba2motif_dataset.py
--rw-r--r--   0        0        0     3700 2023-12-21 07:51:56.894907 torch_geometric-2.5.2/torch_geometric/datasets/ba_multi_shapes.py
--rw-r--r--   0        0        0     3904 2023-12-21 07:51:56.895012 torch_geometric-2.5.2/torch_geometric/datasets/ba_shapes.py
--rw-r--r--   0        0        0     4404 2023-12-21 07:51:56.895155 torch_geometric-2.5.2/torch_geometric/datasets/bitcoin_otc.py
--rw-r--r--   0        0        0     3959 2023-12-21 07:51:56.895693 torch_geometric-2.5.2/torch_geometric/datasets/brca_tgca.py
--rw-r--r--   0        0        0     4458 2023-12-21 07:51:56.895825 torch_geometric-2.5.2/torch_geometric/datasets/citation_full.py
--rw-r--r--   0        0        0     3138 2023-12-21 07:51:56.895951 torch_geometric-2.5.2/torch_geometric/datasets/coauthor.py
--rw-r--r--   0        0        0     4734 2023-12-21 07:51:56.896208 torch_geometric-2.5.2/torch_geometric/datasets/coma.py
--rw-r--r--   0        0        0     5416 2023-12-21 07:51:56.896338 torch_geometric-2.5.2/torch_geometric/datasets/dblp.py
--rw-r--r--   0        0        0     5707 2024-02-15 14:55:33.353020 torch_geometric-2.5.2/torch_geometric/datasets/dbp15k.py
--rw-r--r--   0        0        0     2511 2023-12-21 07:51:56.896613 torch_geometric-2.5.2/torch_geometric/datasets/deezer_europe.py
--rw-r--r--   0        0        0     4035 2023-12-21 07:51:56.896734 torch_geometric-2.5.2/torch_geometric/datasets/dgraph.py
--rw-r--r--   0        0        0     6041 2023-12-21 07:51:56.896863 torch_geometric-2.5.2/torch_geometric/datasets/dynamic_faust.py
--rw-r--r--   0        0        0     4605 2023-12-21 07:51:56.897104 torch_geometric-2.5.2/torch_geometric/datasets/elliptic.py
--rw-r--r--   0        0        0     3188 2023-11-30 06:56:02.055205 torch_geometric-2.5.2/torch_geometric/datasets/elliptic_temporal.py
--rw-r--r--   0        0        0     2834 2023-12-21 07:51:56.897222 torch_geometric-2.5.2/torch_geometric/datasets/email_eu_core.py
--rw-r--r--   0        0        0     7312 2024-03-20 18:30:51.592190 torch_geometric-2.5.2/torch_geometric/datasets/entities.py
--rw-r--r--   0        0        0     6103 2023-12-21 07:51:56.897750 torch_geometric-2.5.2/torch_geometric/datasets/explainer_dataset.py
--rw-r--r--   0        0        0     2431 2023-12-21 07:51:56.897836 torch_geometric-2.5.2/torch_geometric/datasets/facebook.py
--rw-r--r--   0        0        0    10554 2024-01-07 13:37:00.549728 torch_geometric-2.5.2/torch_geometric/datasets/fake.py
--rw-r--r--   0        0        0     4076 2023-12-21 07:51:56.898087 torch_geometric-2.5.2/torch_geometric/datasets/faust.py
--rw-r--r--   0        0        0     3964 2024-02-15 14:55:33.353369 torch_geometric-2.5.2/torch_geometric/datasets/flickr.py
--rw-r--r--   0        0        0     4080 2023-12-21 07:51:56.898313 torch_geometric-2.5.2/torch_geometric/datasets/freebase.py
--rw-r--r--   0        0        0     3598 2023-12-21 07:51:56.898404 torch_geometric-2.5.2/torch_geometric/datasets/gdelt.py
--rw-r--r--   0        0        0     3189 2023-12-21 07:51:56.898486 torch_geometric-2.5.2/torch_geometric/datasets/gdelt_lite.py
--rw-r--r--   0        0        0     9511 2024-02-15 14:55:33.353533 torch_geometric-2.5.2/torch_geometric/datasets/ged_dataset.py
--rw-r--r--   0        0        0     2820 2023-12-21 07:51:56.898839 torch_geometric-2.5.2/torch_geometric/datasets/gemsec.py
--rw-r--r--   0        0        0     4223 2023-12-21 07:51:56.898997 torch_geometric-2.5.2/torch_geometric/datasets/geometry.py
--rw-r--r--   0        0        0     2687 2023-12-21 07:51:56.899128 torch_geometric-2.5.2/torch_geometric/datasets/github.py
--rw-r--r--   0        0        0     6940 2023-12-21 07:51:56.899254 torch_geometric-2.5.2/torch_geometric/datasets/gnn_benchmark_dataset.py
--rw-r--r--   0        0        0      272 2024-01-16 19:07:07.464900 torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/__init__.py
--rw-r--r--   0        0        0      965 2023-04-09 09:43:57.304447 torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-r--r--   0        0        0      939 2023-12-21 07:51:56.899387 torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/base.py
--rw-r--r--   0        0        0      918 2023-04-09 09:43:57.304551 torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/er_graph.py
--rw-r--r--   0        0        0     1159 2023-04-09 09:43:57.304609 torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-r--r--   0        0        0     2599 2024-01-16 19:07:07.464998 torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/tree_graph.py
--rw-r--r--   0        0        0     4224 2023-12-21 07:51:56.899658 torch_geometric-2.5.2/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-r--r--   0        0        0     8846 2024-02-15 14:55:33.353696 torch_geometric-2.5.2/torch_geometric/datasets/hgb_dataset.py
--rw-r--r--   0        0        0     6763 2023-12-21 07:51:56.900559 torch_geometric-2.5.2/torch_geometric/datasets/hm.py
--rw-r--r--   0        0        0    11417 2023-12-21 07:51:56.900734 torch_geometric-2.5.2/torch_geometric/datasets/hydro_net.py
--rw-r--r--   0        0        0     4735 2023-12-21 07:51:56.900899 torch_geometric-2.5.2/torch_geometric/datasets/icews.py
--rw-r--r--   0        0        0     4611 2023-12-21 07:51:56.901264 torch_geometric-2.5.2/torch_geometric/datasets/igmc_dataset.py
--rw-r--r--   0        0        0     4223 2023-12-21 07:51:56.901418 torch_geometric-2.5.2/torch_geometric/datasets/imdb.py
--rw-r--r--   0        0        0     7293 2023-12-21 07:51:56.901564 torch_geometric-2.5.2/torch_geometric/datasets/infection_dataset.py
--rw-r--r--   0        0        0     3643 2023-12-21 07:51:56.901672 torch_geometric-2.5.2/torch_geometric/datasets/jodie.py
--rw-r--r--   0        0        0     3445 2023-11-23 19:01:39.073186 torch_geometric-2.5.2/torch_geometric/datasets/karate.py
--rw-r--r--   0        0        0     4572 2023-12-21 07:51:56.901818 torch_geometric-2.5.2/torch_geometric/datasets/last_fm.py
--rw-r--r--   0        0        0     2486 2023-12-21 07:51:56.901934 torch_geometric-2.5.2/torch_geometric/datasets/lastfm_asia.py
--rw-r--r--   0        0        0     6864 2024-02-15 14:55:33.353977 torch_geometric-2.5.2/torch_geometric/datasets/linkx_dataset.py
--rw-r--r--   0        0        0    11746 2023-12-21 07:51:56.902238 torch_geometric-2.5.2/torch_geometric/datasets/lrgb.py
--rw-r--r--   0        0        0     5244 2023-12-21 07:51:56.902365 torch_geometric-2.5.2/torch_geometric/datasets/malnet_tiny.py
--rw-r--r--   0        0        0    16734 2023-12-21 07:51:56.902710 torch_geometric-2.5.2/torch_geometric/datasets/md17.py
--rw-r--r--   0        0        0     3951 2023-12-21 07:51:56.902835 torch_geometric-2.5.2/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-r--r--   0        0        0     3317 2023-12-21 07:51:56.902958 torch_geometric-2.5.2/torch_geometric/datasets/mnist_superpixels.py
--rw-r--r--   0        0        0     5347 2023-12-21 07:51:56.903210 torch_geometric-2.5.2/torch_geometric/datasets/modelnet.py
--rw-r--r--   0        0        0     6783 2023-12-21 07:51:56.903365 torch_geometric-2.5.2/torch_geometric/datasets/molecule_net.py
--rw-r--r--   0        0        0      272 2024-01-16 19:07:07.465139 torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/__init__.py
--rw-r--r--   0        0        0      900 2023-12-21 07:51:56.903471 torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/base.py
--rw-r--r--   0        0        0     1278 2023-12-21 07:51:56.903565 torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/custom.py
--rw-r--r--   0        0        0      983 2024-01-16 19:07:07.465273 torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/cycle.py
--rw-r--r--   0        0        0     1099 2024-01-16 19:07:07.465364 torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/grid.py
--rw-r--r--   0        0        0      814 2023-12-21 07:51:56.903671 torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/house.py
--rw-r--r--   0        0        0     4033 2023-12-21 07:51:56.903779 torch_geometric-2.5.2/torch_geometric/datasets/movie_lens.py
--rw-r--r--   0        0        0     6057 2023-12-21 07:51:56.903937 torch_geometric-2.5.2/torch_geometric/datasets/movie_lens_100k.py
--rw-r--r--   0        0        0     5396 2023-12-21 07:51:56.904066 torch_geometric-2.5.2/torch_geometric/datasets/movie_lens_1m.py
--rw-r--r--   0        0        0     3008 2023-12-21 07:51:56.904161 torch_geometric-2.5.2/torch_geometric/datasets/myket.py
--rw-r--r--   0        0        0     2863 2023-12-31 08:35:31.852876 torch_geometric-2.5.2/torch_geometric/datasets/nell.py
--rw-r--r--   0        0        0     5196 2024-03-20 18:30:51.592412 torch_geometric-2.5.2/torch_geometric/datasets/neurograph.py
--rw-r--r--   0        0        0     7481 2023-12-21 07:51:56.904554 torch_geometric-2.5.2/torch_geometric/datasets/ogb_mag.py
--rw-r--r--   0        0        0     3585 2023-12-21 07:51:56.904682 torch_geometric-2.5.2/torch_geometric/datasets/omdb.py
--rw-r--r--   0        0        0     5161 2023-12-21 07:51:56.904814 torch_geometric-2.5.2/torch_geometric/datasets/ose_gvcs.py
--rw-r--r--   0        0        0     4162 2023-12-21 07:51:56.904940 torch_geometric-2.5.2/torch_geometric/datasets/particle.py
--rw-r--r--   0        0        0    12031 2023-12-21 07:51:56.905083 torch_geometric-2.5.2/torch_geometric/datasets/pascal.py
--rw-r--r--   0        0        0     4791 2023-12-21 07:51:56.905217 torch_geometric-2.5.2/torch_geometric/datasets/pascal_pf.py
--rw-r--r--   0        0        0     5897 2023-12-21 07:51:56.905357 torch_geometric-2.5.2/torch_geometric/datasets/pcpnet_dataset.py
--rw-r--r--   0        0        0     3813 2023-12-21 07:51:56.905459 torch_geometric-2.5.2/torch_geometric/datasets/pcqm4m.py
--rw-r--r--   0        0        0     7201 2023-12-21 07:51:56.905713 torch_geometric-2.5.2/torch_geometric/datasets/planetoid.py
--rw-r--r--   0        0        0     3045 2023-12-21 07:51:56.905813 torch_geometric-2.5.2/torch_geometric/datasets/polblogs.py
--rw-r--r--   0        0        0     4999 2023-12-21 07:51:56.905939 torch_geometric-2.5.2/torch_geometric/datasets/ppi.py
--rw-r--r--   0        0        0     3325 2023-12-21 07:51:56.906048 torch_geometric-2.5.2/torch_geometric/datasets/qm7.py
--rw-r--r--   0        0        0    17158 2023-12-21 07:51:56.906164 torch_geometric-2.5.2/torch_geometric/datasets/qm9.py
--rw-r--r--   0        0        0     5304 2024-02-15 14:55:33.354170 torch_geometric-2.5.2/torch_geometric/datasets/rcdd.py
--rw-r--r--   0        0        0     3122 2023-12-21 07:51:56.906502 torch_geometric-2.5.2/torch_geometric/datasets/reddit.py
--rw-r--r--   0        0        0     4282 2024-02-15 14:55:33.354362 torch_geometric-2.5.2/torch_geometric/datasets/reddit2.py
--rw-r--r--   0        0        0     4535 2023-12-21 07:51:56.906762 torch_geometric-2.5.2/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-r--r--   0        0        0     4492 2023-12-21 07:51:56.906884 torch_geometric-2.5.2/torch_geometric/datasets/s3dis.py
--rw-r--r--   0        0        0     8816 2023-12-28 11:34:13.531778 torch_geometric-2.5.2/torch_geometric/datasets/sbm_dataset.py
--rw-r--r--   0        0        0     8504 2023-12-21 07:51:56.907179 torch_geometric-2.5.2/torch_geometric/datasets/shapenet.py
--rw-r--r--   0        0        0     6316 2023-12-21 07:51:56.907413 torch_geometric-2.5.2/torch_geometric/datasets/shrec2016.py
--rw-r--r--   0        0        0     9304 2023-12-21 07:51:56.907572 torch_geometric-2.5.2/torch_geometric/datasets/snap_dataset.py
--rw-r--r--   0        0        0     3278 2023-12-21 07:51:56.907670 torch_geometric-2.5.2/torch_geometric/datasets/suite_sparse.py
--rw-r--r--   0        0        0     4170 2023-12-21 07:51:56.907790 torch_geometric-2.5.2/torch_geometric/datasets/taobao.py
--rw-r--r--   0        0        0     4632 2023-12-21 07:51:56.907904 torch_geometric-2.5.2/torch_geometric/datasets/tosca.py
--rw-r--r--   0        0        0     7847 2023-12-31 08:35:31.853471 torch_geometric-2.5.2/torch_geometric/datasets/tu_dataset.py
--rw-r--r--   0        0        0     3658 2023-12-21 07:51:56.908132 torch_geometric-2.5.2/torch_geometric/datasets/twitch.py
--rw-r--r--   0        0        0     7001 2024-02-15 14:55:33.354555 torch_geometric-2.5.2/torch_geometric/datasets/upfd.py
--rw-r--r--   0        0        0      182 2023-05-17 17:44:44.813472 torch_geometric-2.5.2/torch_geometric/datasets/utils/__init__.py
--rw-r--r--   0        0        0     1835 2023-12-21 07:51:56.908367 torch_geometric-2.5.2/torch_geometric/datasets/utils/cheatsheet.py
--rw-r--r--   0        0        0     4889 2023-12-21 07:51:56.908697 torch_geometric-2.5.2/torch_geometric/datasets/webkb.py
--rw-r--r--   0        0        0     3884 2023-12-21 07:51:56.908797 torch_geometric-2.5.2/torch_geometric/datasets/wikics.py
--rw-r--r--   0        0        0     4947 2024-02-15 14:55:33.354736 torch_geometric-2.5.2/torch_geometric/datasets/wikidata.py
--rw-r--r--   0        0        0     6640 2023-12-21 07:51:56.909027 torch_geometric-2.5.2/torch_geometric/datasets/wikipedia_network.py
--rw-r--r--   0        0        0     7017 2023-12-21 07:51:56.909158 torch_geometric-2.5.2/torch_geometric/datasets/willow_object_class.py
--rw-r--r--   0        0        0     8158 2023-12-21 07:51:56.909388 torch_geometric-2.5.2/torch_geometric/datasets/word_net.py
--rw-r--r--   0        0        0     3959 2024-02-15 14:55:33.354864 torch_geometric-2.5.2/torch_geometric/datasets/yelp.py
--rw-r--r--   0        0        0     6347 2023-12-21 07:51:56.909622 torch_geometric-2.5.2/torch_geometric/datasets/zinc.py
--rw-r--r--   0        0        0     1295 2023-12-21 07:51:56.909709 torch_geometric-2.5.2/torch_geometric/debug.py
--rw-r--r--   0        0        0      858 2023-12-21 07:51:56.909796 torch_geometric-2.5.2/torch_geometric/deprecation.py
--rw-r--r--   0        0        0      589 2023-11-23 19:01:39.080087 torch_geometric-2.5.2/torch_geometric/distributed/__init__.py
--rw-r--r--   0        0        0      418 2023-08-02 10:48:33.251092 torch_geometric-2.5.2/torch_geometric/distributed/dist_context.py
--rw-r--r--   0        0        0     4933 2024-02-15 14:55:33.355095 torch_geometric-2.5.2/torch_geometric/distributed/dist_link_neighbor_loader.py
--rw-r--r--   0        0        0     6492 2024-02-15 14:55:33.355288 torch_geometric-2.5.2/torch_geometric/distributed/dist_loader.py
--rw-r--r--   0        0        0     4372 2024-02-15 14:55:33.355525 torch_geometric-2.5.2/torch_geometric/distributed/dist_neighbor_loader.py
--rw-r--r--   0        0        0    42406 2024-02-15 14:55:33.356032 torch_geometric-2.5.2/torch_geometric/distributed/dist_neighbor_sampler.py
--rw-r--r--   0        0        0     3309 2023-12-21 07:51:56.910896 torch_geometric-2.5.2/torch_geometric/distributed/event_loop.py
--rw-r--r--   0        0        0    19018 2024-02-15 14:55:33.356215 torch_geometric-2.5.2/torch_geometric/distributed/local_feature_store.py
--rw-r--r--   0        0        0     8408 2024-02-15 14:55:33.356438 torch_geometric-2.5.2/torch_geometric/distributed/local_graph_store.py
--rw-r--r--   0        0        0    14675 2024-02-15 14:55:33.356739 torch_geometric-2.5.2/torch_geometric/distributed/partition.py
--rw-r--r--   0        0        0     5753 2024-02-15 14:55:33.356938 torch_geometric-2.5.2/torch_geometric/distributed/rpc.py
--rw-r--r--   0        0        0     6567 2024-02-15 14:55:33.357113 torch_geometric-2.5.2/torch_geometric/distributed/utils.py
--rw-r--r--   0        0        0    61285 2024-03-20 18:30:51.593150 torch_geometric-2.5.2/torch_geometric/edge_index.py
--rw-r--r--   0        0        0     4756 2023-12-21 07:51:56.911426 torch_geometric-2.5.2/torch_geometric/experimental.py
--rw-r--r--   0        0        0      359 2023-04-09 09:43:57.309954 torch_geometric-2.5.2/torch_geometric/explain/__init__.py
--rw-r--r--   0        0        0      496 2023-09-21 09:55:53.976137 torch_geometric-2.5.2/torch_geometric/explain/algorithm/__init__.py
--rw-r--r--   0        0        0     4545 2023-11-23 19:01:39.081865 torch_geometric-2.5.2/torch_geometric/explain/algorithm/attention_explainer.py
--rw-r--r--   0        0        0     6935 2023-11-23 19:01:39.082059 torch_geometric-2.5.2/torch_geometric/explain/algorithm/base.py
--rw-r--r--   0        0        0    12857 2023-11-30 06:56:02.065723 torch_geometric-2.5.2/torch_geometric/explain/algorithm/captum.py
--rw-r--r--   0        0        0     7346 2023-11-30 06:56:02.065986 torch_geometric-2.5.2/torch_geometric/explain/algorithm/captum_explainer.py
--rw-r--r--   0        0        0     2872 2023-11-23 19:01:39.082529 torch_geometric-2.5.2/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-r--r--   0        0        0    12454 2023-11-23 19:01:39.082709 torch_geometric-2.5.2/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-r--r--   0        0        0    21389 2023-11-23 19:01:39.082845 torch_geometric-2.5.2/torch_geometric/explain/algorithm/graphmask_explainer.py
--rw-r--r--   0        0        0    10371 2023-11-23 19:01:39.083036 torch_geometric-2.5.2/torch_geometric/explain/algorithm/pg_explainer.py
--rw-r--r--   0        0        0     2564 2023-11-23 19:01:39.083156 torch_geometric-2.5.2/torch_geometric/explain/algorithm/utils.py
--rw-r--r--   0        0        0     7834 2023-04-09 09:43:57.310831 torch_geometric-2.5.2/torch_geometric/explain/config.py
--rw-r--r--   0        0        0    10667 2023-11-23 19:01:39.083333 torch_geometric-2.5.2/torch_geometric/explain/explainer.py
--rw-r--r--   0        0        0    14934 2024-02-15 14:55:33.357475 torch_geometric-2.5.2/torch_geometric/explain/explanation.py
--rw-r--r--   0        0        0      301 2023-04-09 09:43:57.311049 torch_geometric-2.5.2/torch_geometric/explain/metric/__init__.py
--rw-r--r--   0        0        0     1888 2023-11-23 19:01:39.083621 torch_geometric-2.5.2/torch_geometric/explain/metric/basic.py
--rw-r--r--   0        0        0     3063 2023-04-09 09:43:57.311165 torch_geometric-2.5.2/torch_geometric/explain/metric/faithfulness.py
--rw-r--r--   0        0        0     6157 2023-11-23 19:01:39.083749 torch_geometric-2.5.2/torch_geometric/explain/metric/fidelity.py
--rw-r--r--   0        0        0     1815 2023-06-15 08:50:09.287832 torch_geometric-2.5.2/torch_geometric/graphgym/__init__.py
--rw-r--r--   0        0        0      510 2023-04-09 09:43:57.311384 torch_geometric-2.5.2/torch_geometric/graphgym/benchmark.py
--rw-r--r--   0        0        0     2371 2023-04-09 09:43:57.311450 torch_geometric-2.5.2/torch_geometric/graphgym/checkpoint.py
--rw-r--r--   0        0        0      738 2023-04-09 09:43:57.311504 torch_geometric-2.5.2/torch_geometric/graphgym/cmd_args.py
--rw-r--r--   0        0        0    17197 2023-11-30 06:56:02.066436 torch_geometric-2.5.2/torch_geometric/graphgym/config.py
--rw-r--r--   0        0        0      389 2023-04-09 09:43:57.311792 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.311851 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/act/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.311908 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/config/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.311966 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/encoder/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312019 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/head/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312073 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-r--r--   0        0        0     8435 2023-11-23 19:01:39.084105 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/layer/generalconv.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312204 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/loader/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312257 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/loss/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312309 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/network/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312361 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312413 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/pooling/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312465 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/stage/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312519 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/train/__init__.py
--rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312571 torch_geometric-2.5.2/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-r--r--   0        0        0      375 2023-04-09 09:43:57.312622 torch_geometric-2.5.2/torch_geometric/graphgym/imports.py
--rw-r--r--   0        0        0      521 2023-11-23 19:01:39.084212 torch_geometric-2.5.2/torch_geometric/graphgym/init.py
--rw-r--r--   0        0        0    11605 2023-11-23 19:01:39.084371 torch_geometric-2.5.2/torch_geometric/graphgym/loader.py
--rw-r--r--   0        0        0    11314 2023-11-23 19:01:39.084670 torch_geometric-2.5.2/torch_geometric/graphgym/logger.py
--rw-r--r--   0        0        0     1445 2023-11-23 19:01:39.084807 torch_geometric-2.5.2/torch_geometric/graphgym/loss.py
--rw-r--r--   0        0        0     3110 2023-05-17 17:44:44.813938 torch_geometric-2.5.2/torch_geometric/graphgym/model_builder.py
--rw-r--r--   0        0        0     1121 2023-04-09 09:43:57.313035 torch_geometric-2.5.2/torch_geometric/graphgym/models/__init__.py
--rw-r--r--   0        0        0      855 2023-09-21 09:55:53.976881 torch_geometric-2.5.2/torch_geometric/graphgym/models/act.py
--rw-r--r--   0        0        0     3034 2023-11-23 19:01:39.084923 torch_geometric-2.5.2/torch_geometric/graphgym/models/encoder.py
--rw-r--r--   0        0        0     6373 2023-09-21 09:55:53.977064 torch_geometric-2.5.2/torch_geometric/graphgym/models/gnn.py
--rw-r--r--   0        0        0     4603 2023-09-21 09:55:53.977157 torch_geometric-2.5.2/torch_geometric/graphgym/models/head.py
--rw-r--r--   0        0        0    12500 2023-12-04 06:33:33.769780 torch_geometric-2.5.2/torch_geometric/graphgym/models/layer.py
--rw-r--r--   0        0        0      288 2023-04-09 09:43:57.313417 torch_geometric-2.5.2/torch_geometric/graphgym/models/pooling.py
--rw-r--r--   0        0        0     1383 2023-11-23 19:01:39.085023 torch_geometric-2.5.2/torch_geometric/graphgym/models/transform.py
--rw-r--r--   0        0        0     2544 2023-04-09 09:43:57.313526 torch_geometric-2.5.2/torch_geometric/graphgym/optim.py
--rw-r--r--   0        0        0     3954 2023-11-23 19:01:39.085131 torch_geometric-2.5.2/torch_geometric/graphgym/register.py
--rw-r--r--   0        0        0     2653 2023-09-21 09:55:53.977362 torch_geometric-2.5.2/torch_geometric/graphgym/train.py
--rw-r--r--   0        0        0        0 2023-04-09 09:43:57.313667 torch_geometric-2.5.2/torch_geometric/graphgym/utils/LICENSE
--rw-r--r--   0        0        0      641 2023-04-09 09:43:57.313725 torch_geometric-2.5.2/torch_geometric/graphgym/utils/__init__.py
--rw-r--r--   0        0        0     9349 2023-11-30 06:56:02.066772 torch_geometric-2.5.2/torch_geometric/graphgym/utils/agg_runs.py
--rw-r--r--   0        0        0     3045 2023-11-23 19:01:39.085413 torch_geometric-2.5.2/torch_geometric/graphgym/utils/comp_budget.py
--rw-r--r--   0        0        0     1342 2023-11-23 19:01:39.085516 torch_geometric-2.5.2/torch_geometric/graphgym/utils/device.py
--rw-r--r--   0        0        0      690 2023-04-09 09:43:57.313975 torch_geometric-2.5.2/torch_geometric/graphgym/utils/epoch.py
--rw-r--r--   0        0        0     2049 2023-11-30 06:56:02.067070 torch_geometric-2.5.2/torch_geometric/graphgym/utils/io.py
--rw-r--r--   0        0        0      624 2023-11-23 19:01:39.085735 torch_geometric-2.5.2/torch_geometric/graphgym/utils/plot.py
--rw-r--r--   0        0        0      199 2023-11-23 19:01:39.085842 torch_geometric-2.5.2/torch_geometric/graphgym/utils/tools.py
--rw-r--r--   0        0        0      790 2024-01-16 19:07:07.467913 torch_geometric-2.5.2/torch_geometric/home.py
--rw-r--r--   0        0        0    19217 2024-03-20 18:31:22.924739 torch_geometric-2.5.2/torch_geometric/inspector.py
--rw-r--r--   0        0        0      528 2023-03-19 07:56:22.191105 torch_geometric-2.5.2/torch_geometric/io/__init__.py
--rw-r--r--   0        0        0     6567 2024-02-28 12:41:28.382709 torch_geometric-2.5.2/torch_geometric/io/fs.py
--rw-r--r--   0        0        0     1177 2023-08-04 14:13:46.021779 torch_geometric-2.5.2/torch_geometric/io/npz.py
--rw-r--r--   0        0        0     1088 2023-12-21 07:51:56.911732 torch_geometric-2.5.2/torch_geometric/io/obj.py
--rw-r--r--   0        0        0     2762 2023-12-21 07:51:56.911821 torch_geometric-2.5.2/torch_geometric/io/off.py
--rw-r--r--   0        0        0     4667 2024-01-07 13:37:00.550342 torch_geometric-2.5.2/torch_geometric/io/planetoid.py
--rw-r--r--   0        0        0      489 2023-12-21 07:51:56.912040 torch_geometric-2.5.2/torch_geometric/io/ply.py
--rw-r--r--   0        0        0     1170 2023-12-21 07:51:56.912128 torch_geometric-2.5.2/torch_geometric/io/sdf.py
--rw-r--r--   0        0        0     4918 2023-12-21 07:51:56.912246 torch_geometric-2.5.2/torch_geometric/io/tu.py
--rw-r--r--   0        0        0      910 2023-12-21 07:51:56.912343 torch_geometric-2.5.2/torch_geometric/io/txt_array.py
--rw-r--r--   0        0        0      935 2023-11-30 06:56:02.067286 torch_geometric-2.5.2/torch_geometric/isinstance.py
--rw-r--r--   0        0        0      908 2023-12-21 07:51:56.912433 torch_geometric-2.5.2/torch_geometric/lazy_loader.py
--rw-r--r--   0        0        0     1835 2023-11-23 19:01:39.086566 torch_geometric-2.5.2/torch_geometric/loader/__init__.py
--rw-r--r--   0        0        0     1615 2023-12-21 07:51:56.912528 torch_geometric-2.5.2/torch_geometric/loader/base.py
--rw-r--r--   0        0        0     2106 2023-09-21 09:55:53.978071 torch_geometric-2.5.2/torch_geometric/loader/cache.py
--rw-r--r--   0        0        0    13196 2024-02-15 14:55:33.357892 torch_geometric-2.5.2/torch_geometric/loader/cluster.py
--rw-r--r--   0        0        0     1459 2023-11-23 19:01:39.086733 torch_geometric-2.5.2/torch_geometric/loader/data_list_loader.py
--rw-r--r--   0        0        0     3527 2023-12-21 07:51:56.912619 torch_geometric-2.5.2/torch_geometric/loader/dataloader.py
--rw-r--r--   0        0        0     1685 2023-06-27 06:01:05.570350 torch_geometric-2.5.2/torch_geometric/loader/dense_data_loader.py
--rw-r--r--   0        0        0     4163 2023-11-23 19:01:39.086987 torch_geometric-2.5.2/torch_geometric/loader/dynamic_batch_sampler.py
--rw-r--r--   0        0        0     8448 2023-04-09 09:43:57.315992 torch_geometric-2.5.2/torch_geometric/loader/graph_saint.py
--rw-r--r--   0        0        0     6012 2023-05-29 07:55:13.277083 torch_geometric-2.5.2/torch_geometric/loader/hgt_loader.py
--rw-r--r--   0        0        0    31462 2023-11-23 19:01:39.087102 torch_geometric-2.5.2/torch_geometric/loader/ibmb_loader.py
--rw-r--r--   0        0        0     3754 2023-04-09 09:43:57.316342 torch_geometric-2.5.2/torch_geometric/loader/imbalanced_sampler.py
--rw-r--r--   0        0        0    16207 2024-02-15 14:55:33.358040 torch_geometric-2.5.2/torch_geometric/loader/link_loader.py
--rw-r--r--   0        0        0    14383 2024-02-15 14:55:33.358200 torch_geometric-2.5.2/torch_geometric/loader/link_neighbor_loader.py
--rw-r--r--   0        0        0    10931 2023-12-21 07:51:56.912890 torch_geometric-2.5.2/torch_geometric/loader/mixin.py
--rw-r--r--   0        0        0    12452 2023-11-23 19:01:39.087825 torch_geometric-2.5.2/torch_geometric/loader/neighbor_loader.py
--rw-r--r--   0        0        0     8513 2023-04-09 09:43:57.316687 torch_geometric-2.5.2/torch_geometric/loader/neighbor_sampler.py
--rw-r--r--   0        0        0    11848 2024-02-15 14:55:33.358394 torch_geometric-2.5.2/torch_geometric/loader/node_loader.py
--rw-r--r--   0        0        0     3236 2023-11-23 19:01:39.088138 torch_geometric-2.5.2/torch_geometric/loader/prefetch.py
--rw-r--r--   0        0        0     2196 2023-04-09 09:43:57.316820 torch_geometric-2.5.2/torch_geometric/loader/random_node_loader.py
--rw-r--r--   0        0        0     4173 2023-04-09 09:43:57.316884 torch_geometric-2.5.2/torch_geometric/loader/shadow.py
--rw-r--r--   0        0        0     2248 2023-08-07 04:56:40.199958 torch_geometric-2.5.2/torch_geometric/loader/temporal_dataloader.py
--rw-r--r--   0        0        0    14818 2023-12-31 08:35:31.855122 torch_geometric-2.5.2/torch_geometric/loader/utils.py
--rw-r--r--   0        0        0     3518 2023-05-29 07:55:13.278120 torch_geometric-2.5.2/torch_geometric/loader/zip_loader.py
--rw-r--r--   0        0        0      858 2023-12-21 07:51:56.913129 torch_geometric-2.5.2/torch_geometric/logging.py
--rw-r--r--   0        0        0      296 2024-02-15 14:55:33.358581 torch_geometric-2.5.2/torch_geometric/metrics/__init__.py
--rw-r--r--   0        0        0     7521 2024-03-05 12:38:29.028824 torch_geometric-2.5.2/torch_geometric/metrics/link_pred.py
--rw-r--r--   0        0        0      847 2023-05-29 07:55:13.278204 torch_geometric-2.5.2/torch_geometric/nn/__init__.py
--rw-r--r--   0        0        0     1451 2023-11-23 19:01:39.088653 torch_geometric-2.5.2/torch_geometric/nn/aggr/__init__.py
--rw-r--r--   0        0        0     3003 2023-11-23 19:01:39.088759 torch_geometric-2.5.2/torch_geometric/nn/aggr/attention.py
--rw-r--r--   0        0        0     8110 2024-03-20 18:30:51.593987 torch_geometric-2.5.2/torch_geometric/nn/aggr/base.py
--rw-r--r--   0        0        0    11011 2023-11-23 19:01:39.089265 torch_geometric-2.5.2/torch_geometric/nn/aggr/basic.py
--rw-r--r--   0        0        0     2650 2023-11-23 19:01:39.089413 torch_geometric-2.5.2/torch_geometric/nn/aggr/deep_sets.py
--rw-r--r--   0        0        0     6639 2023-11-23 19:01:39.089545 torch_geometric-2.5.2/torch_geometric/nn/aggr/equilibrium.py
--rw-r--r--   0        0        0    12276 2023-11-23 19:01:39.089987 torch_geometric-2.5.2/torch_geometric/nn/aggr/fused.py
--rw-r--r--   0        0        0     3801 2023-06-27 13:28:15.074839 torch_geometric-2.5.2/torch_geometric/nn/aggr/gmt.py
--rw-r--r--   0        0        0     2193 2024-03-20 18:30:51.594154 torch_geometric-2.5.2/torch_geometric/nn/aggr/gru.py
--rw-r--r--   0        0        0     4190 2023-11-23 19:01:39.090090 torch_geometric-2.5.2/torch_geometric/nn/aggr/lcm.py
--rw-r--r--   0        0        0     2214 2023-06-27 13:28:15.075215 torch_geometric-2.5.2/torch_geometric/nn/aggr/lstm.py
--rw-r--r--   0        0        0     2514 2024-03-20 18:30:51.594344 torch_geometric-2.5.2/torch_geometric/nn/aggr/mlp.py
--rw-r--r--   0        0        0     8170 2023-06-10 14:35:51.129653 torch_geometric-2.5.2/torch_geometric/nn/aggr/multi.py
--rw-r--r--   0        0        0     6189 2023-11-23 19:01:39.090353 torch_geometric-2.5.2/torch_geometric/nn/aggr/quantile.py
--rw-r--r--   0        0        0     4638 2023-07-21 07:41:11.167904 torch_geometric-2.5.2/torch_geometric/nn/aggr/scaler.py
--rw-r--r--   0        0        0     2446 2023-11-23 19:01:39.090464 torch_geometric-2.5.2/torch_geometric/nn/aggr/set2set.py
--rw-r--r--   0        0        0     4207 2023-08-24 05:09:46.603743 torch_geometric-2.5.2/torch_geometric/nn/aggr/set_transformer.py
--rw-r--r--   0        0        0     2507 2023-06-27 13:28:15.076321 torch_geometric-2.5.2/torch_geometric/nn/aggr/sort.py
--rw-r--r--   0        0        0     8338 2023-11-23 19:01:39.090753 torch_geometric-2.5.2/torch_geometric/nn/aggr/utils.py
--rw-r--r--   0        0        0       76 2023-06-15 08:50:09.288170 torch_geometric-2.5.2/torch_geometric/nn/attention/__init__.py
--rw-r--r--   0        0        0     7357 2023-11-23 19:01:39.090903 torch_geometric-2.5.2/torch_geometric/nn/attention/performer.py
--rw-r--r--   0        0        0     3515 2024-02-11 12:50:44.321572 torch_geometric-2.5.2/torch_geometric/nn/conv/__init__.py
--rw-r--r--   0        0        0     3077 2024-01-07 13:37:00.550514 torch_geometric-2.5.2/torch_geometric/nn/conv/agnn_conv.py
--rw-r--r--   0        0        0     4387 2023-11-23 19:01:39.091295 torch_geometric-2.5.2/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-r--r--   0        0        0     5983 2024-01-16 19:07:07.468736 torch_geometric-2.5.2/torch_geometric/nn/conv/appnp.py
--rw-r--r--   0        0        0     6585 2024-01-16 19:07:07.468883 torch_geometric-2.5.2/torch_geometric/nn/conv/arma_conv.py
--rw-r--r--   0        0        0     4014 2024-01-07 13:37:00.551165 torch_geometric-2.5.2/torch_geometric/nn/conv/cg_conv.py
--rw-r--r--   0        0        0     6423 2024-01-07 13:37:00.551338 torch_geometric-2.5.2/torch_geometric/nn/conv/cheb_conv.py
--rw-r--r--   0        0        0     5255 2024-01-16 19:07:07.469025 torch_geometric-2.5.2/torch_geometric/nn/conv/cluster_gcn_conv.py
--rw-r--r--   0        0        0     5300 2024-03-20 18:30:51.595502 torch_geometric-2.5.2/torch_geometric/nn/conv/collect.jinja
--rw-r--r--   0        0        0      251 2023-04-09 09:43:57.321325 torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/__init__.py
--rw-r--r--   0        0        0     8212 2024-03-20 18:30:51.597303 torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/base.py
--rw-r--r--   0        0        0     2846 2024-03-20 18:30:51.597557 torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-r--r--   0        0        0     4212 2024-03-20 18:30:51.597743 torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-r--r--   0        0        0     2802 2024-03-20 18:30:51.597898 torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-r--r--   0        0        0     2440 2023-11-23 19:01:39.092177 torch_geometric-2.5.2/torch_geometric/nn/conv/dir_gnn_conv.py
--rw-r--r--   0        0        0    12241 2024-01-07 13:37:00.551656 torch_geometric-2.5.2/torch_geometric/nn/conv/dna_conv.py
--rw-r--r--   0        0        0     5389 2024-01-07 13:37:00.551824 torch_geometric-2.5.2/torch_geometric/nn/conv/edge_conv.py
--rw-r--r--   0        0        0     2216 2024-02-28 12:41:28.383671 torch_geometric-2.5.2/torch_geometric/nn/conv/edge_updater.jinja
--rw-r--r--   0        0        0    10742 2024-01-16 19:07:07.469443 torch_geometric-2.5.2/torch_geometric/nn/conv/eg_conv.py
--rw-r--r--   0        0        0     9065 2024-01-16 19:07:07.469669 torch_geometric-2.5.2/torch_geometric/nn/conv/fa_conv.py
--rw-r--r--   0        0        0     4430 2024-01-07 13:37:00.552728 torch_geometric-2.5.2/torch_geometric/nn/conv/feast_conv.py
--rw-r--r--   0        0        0     6314 2024-01-07 13:37:00.552962 torch_geometric-2.5.2/torch_geometric/nn/conv/film_conv.py
--rw-r--r--   0        0        0     4502 2023-12-29 09:32:12.742136 torch_geometric-2.5.2/torch_geometric/nn/conv/fused_gat_conv.py
--rw-r--r--   0        0        0    16091 2024-01-16 19:07:07.469955 torch_geometric-2.5.2/torch_geometric/nn/conv/gat_conv.py
--rw-r--r--   0        0        0     3518 2024-01-16 19:07:07.470092 torch_geometric-2.5.2/torch_geometric/nn/conv/gated_graph_conv.py
--rw-r--r--   0        0        0    13639 2024-01-16 19:07:07.470276 torch_geometric-2.5.2/torch_geometric/nn/conv/gatv2_conv.py
--rw-r--r--   0        0        0     7001 2024-01-16 19:07:07.470403 torch_geometric-2.5.2/torch_geometric/nn/conv/gcn2_conv.py
--rw-r--r--   0        0        0    10415 2024-01-16 19:07:07.470579 torch_geometric-2.5.2/torch_geometric/nn/conv/gcn_conv.py
--rw-r--r--   0        0        0     9722 2024-02-15 14:55:33.359459 torch_geometric-2.5.2/torch_geometric/nn/conv/gen_conv.py
--rw-r--r--   0        0        0     7591 2024-01-16 19:07:07.470714 torch_geometric-2.5.2/torch_geometric/nn/conv/general_conv.py
--rw-r--r--   0        0        0     7411 2024-01-16 19:07:07.470852 torch_geometric-2.5.2/torch_geometric/nn/conv/gin_conv.py
--rw-r--r--   0        0        0     8315 2024-01-16 19:07:07.471060 torch_geometric-2.5.2/torch_geometric/nn/conv/gmm_conv.py
--rw-r--r--   0        0        0     6672 2023-06-15 08:50:09.288360 torch_geometric-2.5.2/torch_geometric/nn/conv/gps_conv.py
--rw-r--r--   0        0        0     3455 2024-01-16 19:07:07.471198 torch_geometric-2.5.2/torch_geometric/nn/conv/graph_conv.py
--rw-r--r--   0        0        0     4951 2024-01-16 19:07:07.471345 torch_geometric-2.5.2/torch_geometric/nn/conv/gravnet_conv.py
--rw-r--r--   0        0        0     7198 2024-02-15 14:55:33.359644 torch_geometric-2.5.2/torch_geometric/nn/conv/han_conv.py
--rw-r--r--   0        0        0     6084 2024-01-16 19:07:07.471657 torch_geometric-2.5.2/torch_geometric/nn/conv/heat_conv.py
--rw-r--r--   0        0        0     6555 2023-11-23 19:01:39.095192 torch_geometric-2.5.2/torch_geometric/nn/conv/hetero_conv.py
--rw-r--r--   0        0        0     9043 2024-02-15 14:55:33.359787 torch_geometric-2.5.2/torch_geometric/nn/conv/hgt_conv.py
--rw-r--r--   0        0        0     8691 2024-02-15 14:55:33.359940 torch_geometric-2.5.2/torch_geometric/nn/conv/hypergraph_conv.py
--rw-r--r--   0        0        0     3494 2024-01-07 13:37:00.555150 torch_geometric-2.5.2/torch_geometric/nn/conv/le_conv.py
--rw-r--r--   0        0        0     2369 2024-01-16 19:07:07.471811 torch_geometric-2.5.2/torch_geometric/nn/conv/lg_conv.py
--rw-r--r--   0        0        0    41798 2024-03-20 18:31:22.925350 torch_geometric-2.5.2/torch_geometric/nn/conv/message_passing.py
--rw-r--r--   0        0        0     4340 2024-01-16 19:07:07.472405 torch_geometric-2.5.2/torch_geometric/nn/conv/mf_conv.py
--rw-r--r--   0        0        0     4554 2024-01-16 19:07:07.472547 torch_geometric-2.5.2/torch_geometric/nn/conv/mixhop_conv.py
--rw-r--r--   0        0        0     4759 2024-01-07 13:37:00.555995 torch_geometric-2.5.2/torch_geometric/nn/conv/nn_conv.py
--rw-r--r--   0        0        0     4908 2024-01-16 19:07:07.472693 torch_geometric-2.5.2/torch_geometric/nn/conv/pan_conv.py
--rw-r--r--   0        0        0     4892 2024-02-15 14:55:33.360118 torch_geometric-2.5.2/torch_geometric/nn/conv/pdn_conv.py
--rw-r--r--   0        0        0     8325 2024-01-07 13:37:00.556429 torch_geometric-2.5.2/torch_geometric/nn/conv/pna_conv.py
--rw-r--r--   0        0        0     4508 2024-01-07 13:37:00.556571 torch_geometric-2.5.2/torch_geometric/nn/conv/point_conv.py
--rw-r--r--   0        0        0     3278 2024-01-07 13:37:00.556824 torch_geometric-2.5.2/torch_geometric/nn/conv/point_gnn_conv.py
--rw-r--r--   0        0        0     5878 2024-01-07 13:37:00.557040 torch_geometric-2.5.2/torch_geometric/nn/conv/point_transformer_conv.py
--rw-r--r--   0        0        0     5363 2024-01-16 19:07:07.473113 torch_geometric-2.5.2/torch_geometric/nn/conv/ppf_conv.py
--rw-r--r--   0        0        0     7080 2024-02-28 12:41:28.384436 torch_geometric-2.5.2/torch_geometric/nn/conv/propagate.jinja
--rw-r--r--   0        0        0     5217 2024-01-16 19:07:07.473478 torch_geometric-2.5.2/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-r--r--   0        0        0    22863 2024-01-16 19:07:07.473800 torch_geometric-2.5.2/torch_geometric/nn/conv/rgat_conv.py
--rw-r--r--   0        0        0    15705 2024-01-16 19:07:07.473996 torch_geometric-2.5.2/torch_geometric/nn/conv/rgcn_conv.py
--rw-r--r--   0        0        0     5812 2024-01-16 19:07:07.474135 torch_geometric-2.5.2/torch_geometric/nn/conv/sage_conv.py
--rw-r--r--   0        0        0     4543 2024-01-16 19:07:07.474274 torch_geometric-2.5.2/torch_geometric/nn/conv/sg_conv.py
--rw-r--r--   0        0        0     6190 2024-01-16 19:07:07.474416 torch_geometric-2.5.2/torch_geometric/nn/conv/signed_conv.py
--rw-r--r--   0        0        0     3888 2024-01-16 19:07:07.474543 torch_geometric-2.5.2/torch_geometric/nn/conv/simple_conv.py
--rw-r--r--   0        0        0     6314 2024-01-07 13:37:00.558683 torch_geometric-2.5.2/torch_geometric/nn/conv/spline_conv.py
--rw-r--r--   0        0        0     5131 2024-01-16 19:07:07.474692 torch_geometric-2.5.2/torch_geometric/nn/conv/ssg_conv.py
--rw-r--r--   0        0        0    12420 2024-01-07 13:37:00.558982 torch_geometric-2.5.2/torch_geometric/nn/conv/supergat_conv.py
--rw-r--r--   0        0        0     4164 2024-01-16 19:07:07.474827 torch_geometric-2.5.2/torch_geometric/nn/conv/tag_conv.py
--rw-r--r--   0        0        0    10407 2024-01-16 19:07:07.475006 torch_geometric-2.5.2/torch_geometric/nn/conv/transformer_conv.py
--rw-r--r--   0        0        0      852 2023-11-23 19:01:39.099644 torch_geometric-2.5.2/torch_geometric/nn/conv/utils/__init__.py
--rw-r--r--   0        0        0     2792 2023-11-23 19:01:39.099742 torch_geometric-2.5.2/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-r--r--   0        0        0     3140 2023-11-23 19:01:39.100026 torch_geometric-2.5.2/torch_geometric/nn/conv/wl_conv.py
--rw-r--r--   0        0        0     2777 2024-01-16 19:07:07.475144 torch_geometric-2.5.2/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-r--r--   0        0        0     5956 2023-11-23 19:01:39.100257 torch_geometric-2.5.2/torch_geometric/nn/conv/x_conv.py
--rw-r--r--   0        0        0     4764 2023-11-23 19:01:39.100399 torch_geometric-2.5.2/torch_geometric/nn/data_parallel.py
--rw-r--r--   0        0        0      847 2023-11-23 19:01:39.100545 torch_geometric-2.5.2/torch_geometric/nn/dense/__init__.py
--rw-r--r--   0        0        0     4238 2023-11-23 19:01:39.100672 torch_geometric-2.5.2/torch_geometric/nn/dense/dense_gat_conv.py
--rw-r--r--   0        0        0     3002 2023-11-23 19:01:39.100781 torch_geometric-2.5.2/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-r--r--   0        0        0     2361 2023-11-23 19:01:39.100890 torch_geometric-2.5.2/torch_geometric/nn/dense/dense_gin_conv.py
--rw-r--r--   0        0        0     2751 2023-11-23 19:01:39.101001 torch_geometric-2.5.2/torch_geometric/nn/dense/dense_graph_conv.py
--rw-r--r--   0        0        0     2672 2023-11-23 19:01:39.101109 torch_geometric-2.5.2/torch_geometric/nn/dense/dense_sage_conv.py
--rw-r--r--   0        0        0     3051 2023-11-23 19:01:39.101231 torch_geometric-2.5.2/torch_geometric/nn/dense/diff_pool.py
--rw-r--r--   0        0        0     6115 2023-12-05 06:32:32.915671 torch_geometric-2.5.2/torch_geometric/nn/dense/dmon_pool.py
--rw-r--r--   0        0        0    17702 2024-02-15 14:55:33.360239 torch_geometric-2.5.2/torch_geometric/nn/dense/linear.py
--rw-r--r--   0        0        0     4111 2023-11-23 19:01:39.101632 torch_geometric-2.5.2/torch_geometric/nn/dense/mincut_pool.py
--rw-r--r--   0        0        0     3115 2024-02-15 14:55:33.360364 torch_geometric-2.5.2/torch_geometric/nn/encoding.py
--rw-r--r--   0        0        0      129 2023-11-23 19:01:39.101834 torch_geometric-2.5.2/torch_geometric/nn/functional/__init__.py
--rw-r--r--   0        0        0     1549 2023-04-09 09:43:57.329579 torch_geometric-2.5.2/torch_geometric/nn/functional/bro.py
--rw-r--r--   0        0        0      863 2023-04-09 09:43:57.329650 torch_geometric-2.5.2/torch_geometric/nn/functional/gini.py
--rw-r--r--   0        0        0    16055 2023-11-23 19:01:39.102054 torch_geometric-2.5.2/torch_geometric/nn/fx.py
--rw-r--r--   0        0        0     1088 2023-04-09 09:43:57.329812 torch_geometric-2.5.2/torch_geometric/nn/glob.py
--rw-r--r--   0        0        0     2457 2023-04-09 09:43:57.329913 torch_geometric-2.5.2/torch_geometric/nn/inits.py
--rw-r--r--   0        0        0      290 2023-11-23 19:01:39.102166 torch_geometric-2.5.2/torch_geometric/nn/kge/__init__.py
--rw-r--r--   0        0        0     5902 2023-11-23 19:01:39.102288 torch_geometric-2.5.2/torch_geometric/nn/kge/base.py
--rw-r--r--   0        0        0     3234 2023-04-09 09:43:57.330136 torch_geometric-2.5.2/torch_geometric/nn/kge/complex.py
--rw-r--r--   0        0        0     2462 2023-04-09 09:43:57.330226 torch_geometric-2.5.2/torch_geometric/nn/kge/distmult.py
--rw-r--r--   0        0        0      771 2023-04-09 09:43:57.330284 torch_geometric-2.5.2/torch_geometric/nn/kge/loader.py
--rw-r--r--   0        0        0     3208 2023-04-09 09:43:57.330367 torch_geometric-2.5.2/torch_geometric/nn/kge/rotate.py
--rw-r--r--   0        0        0     3088 2023-04-09 09:43:57.330433 torch_geometric-2.5.2/torch_geometric/nn/kge/transe.py
--rw-r--r--   0        0        0     8937 2023-04-09 09:43:57.330505 torch_geometric-2.5.2/torch_geometric/nn/lr_scheduler.py
--rw-r--r--   0        0        0     9512 2023-11-30 06:56:02.068638 torch_geometric-2.5.2/torch_geometric/nn/model_hub.py
--rw-r--r--   0        0        0     1909 2023-12-21 07:51:56.913362 torch_geometric-2.5.2/torch_geometric/nn/models/__init__.py
--rw-r--r--   0        0        0     6634 2024-01-16 19:07:07.475306 torch_geometric-2.5.2/torch_geometric/nn/models/attentive_fp.py
--rw-r--r--   0        0        0    10770 2023-11-23 19:01:39.102686 torch_geometric-2.5.2/torch_geometric/nn/models/autoencoder.py
--rw-r--r--   0        0        0    31225 2024-01-16 19:07:07.475459 torch_geometric-2.5.2/torch_geometric/nn/models/basic_gnn.py
--rw-r--r--   0        0        0     3971 2023-11-23 19:01:39.103036 torch_geometric-2.5.2/torch_geometric/nn/models/captum.py
--rw-r--r--   0        0        0     6827 2023-11-23 19:01:39.103200 torch_geometric-2.5.2/torch_geometric/nn/models/correct_and_smooth.py
--rw-r--r--   0        0        0     4197 2023-11-23 19:01:39.103325 torch_geometric-2.5.2/torch_geometric/nn/models/deep_graph_infomax.py
--rw-r--r--   0        0        0     4339 2023-11-23 19:01:39.103464 torch_geometric-2.5.2/torch_geometric/nn/models/deepgcn.py
--rw-r--r--   0        0        0    36172 2024-03-20 18:30:51.598496 torch_geometric-2.5.2/torch_geometric/nn/models/dimenet.py
--rw-r--r--   0        0        0     5107 2023-11-23 19:01:39.103871 torch_geometric-2.5.2/torch_geometric/nn/models/dimenet_utils.py
--rw-r--r--   0        0        0     7873 2023-11-23 19:01:39.104032 torch_geometric-2.5.2/torch_geometric/nn/models/gnnff.py
--rw-r--r--   0        0        0     9246 2023-11-23 19:01:39.104224 torch_geometric-2.5.2/torch_geometric/nn/models/graph_mixer.py
--rw-r--r--   0        0        0     5395 2023-11-23 19:01:39.104370 torch_geometric-2.5.2/torch_geometric/nn/models/graph_unet.py
--rw-r--r--   0        0        0     3450 2023-11-23 19:01:39.104562 torch_geometric-2.5.2/torch_geometric/nn/models/jumping_knowledge.py
--rw-r--r--   0        0        0     3908 2024-01-16 19:07:07.475623 torch_geometric-2.5.2/torch_geometric/nn/models/label_prop.py
--rw-r--r--   0        0        0    12465 2023-11-23 19:01:39.104875 torch_geometric-2.5.2/torch_geometric/nn/models/lightgcn.py
--rw-r--r--   0        0        0     5812 2024-01-16 19:07:07.475775 torch_geometric-2.5.2/torch_geometric/nn/models/linkx.py
--rw-r--r--   0        0        0     2580 2023-11-23 19:01:39.105180 torch_geometric-2.5.2/torch_geometric/nn/models/mask_label.py
--rw-r--r--   0        0        0     6540 2023-11-23 19:01:39.105344 torch_geometric-2.5.2/torch_geometric/nn/models/meta.py
--rw-r--r--   0        0        0    10798 2023-11-23 19:01:39.105532 torch_geometric-2.5.2/torch_geometric/nn/models/metapath2vec.py
--rw-r--r--   0        0        0    10315 2023-11-23 19:01:39.105734 torch_geometric-2.5.2/torch_geometric/nn/models/mlp.py
--rw-r--r--   0        0        0     2378 2023-11-23 19:01:39.105813 torch_geometric-2.5.2/torch_geometric/nn/models/neural_fingerprint.py
--rw-r--r--   0        0        0     7731 2023-11-23 19:01:39.105980 torch_geometric-2.5.2/torch_geometric/nn/models/node2vec.py
--rw-r--r--   0        0        0     3538 2023-11-23 19:01:39.106116 torch_geometric-2.5.2/torch_geometric/nn/models/pmlp.py
--rw-r--r--   0        0        0     8986 2023-11-23 19:01:39.106289 torch_geometric-2.5.2/torch_geometric/nn/models/re_net.py
--rw-r--r--   0        0        0     2808 2024-01-16 19:07:07.475934 torch_geometric-2.5.2/torch_geometric/nn/models/rect.py
--rw-r--r--   0        0        0    11796 2024-03-05 12:38:29.030106 torch_geometric-2.5.2/torch_geometric/nn/models/rev_gnn.py
--rw-r--r--   0        0        0    16619 2023-12-05 07:08:51.296448 torch_geometric-2.5.2/torch_geometric/nn/models/schnet.py
--rw-r--r--   0        0        0     9839 2023-11-23 19:01:39.106956 torch_geometric-2.5.2/torch_geometric/nn/models/signed_gcn.py
--rw-r--r--   0        0        0    11814 2024-03-20 18:30:51.598726 torch_geometric-2.5.2/torch_geometric/nn/models/tgn.py
--rw-r--r--   0        0        0    43192 2024-02-15 14:55:33.360667 torch_geometric-2.5.2/torch_geometric/nn/models/visnet.py
--rw-r--r--   0        0        0     2373 2023-11-23 19:01:39.109159 torch_geometric-2.5.2/torch_geometric/nn/module_dict.py
--rw-r--r--   0        0        0      669 2023-11-23 19:01:39.109307 torch_geometric-2.5.2/torch_geometric/nn/norm/__init__.py
--rw-r--r--   0        0        0     8283 2023-11-23 19:01:39.109506 torch_geometric-2.5.2/torch_geometric/nn/norm/batch_norm.py
--rw-r--r--   0        0        0     4722 2023-11-23 19:01:39.109638 torch_geometric-2.5.2/torch_geometric/nn/norm/diff_group_norm.py
--rw-r--r--   0        0        0     2727 2023-11-23 19:01:39.109771 torch_geometric-2.5.2/torch_geometric/nn/norm/graph_norm.py
--rw-r--r--   0        0        0     1491 2023-11-23 19:01:39.109886 torch_geometric-2.5.2/torch_geometric/nn/norm/graph_size_norm.py
--rw-r--r--   0        0        0     4685 2023-11-23 19:01:39.110017 torch_geometric-2.5.2/torch_geometric/nn/norm/instance_norm.py
--rw-r--r--   0        0        0     7831 2023-11-23 19:01:39.110157 torch_geometric-2.5.2/torch_geometric/nn/norm/layer_norm.py
--rw-r--r--   0        0        0     1322 2024-02-15 14:55:33.360823 torch_geometric-2.5.2/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-r--r--   0        0        0     1662 2023-11-23 19:01:39.110373 torch_geometric-2.5.2/torch_geometric/nn/norm/msg_norm.py
--rw-r--r--   0        0        0     2824 2023-11-23 19:01:39.110475 torch_geometric-2.5.2/torch_geometric/nn/norm/pair_norm.py
--rw-r--r--   0        0        0     2410 2023-11-23 19:01:39.110589 torch_geometric-2.5.2/torch_geometric/nn/parameter_dict.py
--rw-r--r--   0        0        0    13497 2024-03-20 18:30:51.598948 torch_geometric-2.5.2/torch_geometric/nn/pool/__init__.py
--rw-r--r--   0        0        0     3967 2023-05-29 07:55:13.280050 torch_geometric-2.5.2/torch_geometric/nn/pool/approx_knn.py
--rw-r--r--   0        0        0     6683 2024-01-16 19:07:07.476171 torch_geometric-2.5.2/torch_geometric/nn/pool/asap.py
--rw-r--r--   0        0        0     3966 2023-05-17 17:44:44.818765 torch_geometric-2.5.2/torch_geometric/nn/pool/avg_pool.py
--rw-r--r--   0        0        0      287 2023-11-23 19:01:39.111020 torch_geometric-2.5.2/torch_geometric/nn/pool/connect/__init__.py
--rw-r--r--   0        0        0     4094 2023-11-23 19:01:39.111130 torch_geometric-2.5.2/torch_geometric/nn/pool/connect/base.py
--rw-r--r--   0        0        0     2190 2023-11-23 19:01:39.111323 torch_geometric-2.5.2/torch_geometric/nn/pool/connect/filter_edges.py
--rw-r--r--   0        0        0      273 2023-03-19 07:56:22.204784 torch_geometric-2.5.2/torch_geometric/nn/pool/consecutive.py
--rw-r--r--   0        0        0     1601 2023-10-08 19:44:11.501231 torch_geometric-2.5.2/torch_geometric/nn/pool/decimation.py
--rw-r--r--   0        0        0     8581 2023-11-23 19:01:39.111494 torch_geometric-2.5.2/torch_geometric/nn/pool/edge_pool.py
--rw-r--r--   0        0        0     3492 2023-11-23 19:01:39.111597 torch_geometric-2.5.2/torch_geometric/nn/pool/glob.py
--rw-r--r--   0        0        0     1291 2023-11-23 19:01:39.111702 torch_geometric-2.5.2/torch_geometric/nn/pool/graclus.py
--rw-r--r--   0        0        0     7506 2024-03-20 18:30:51.599150 torch_geometric-2.5.2/torch_geometric/nn/pool/knn.py
--rw-r--r--   0        0        0     4262 2023-05-17 17:44:44.819217 torch_geometric-2.5.2/torch_geometric/nn/pool/max_pool.py
--rw-r--r--   0        0        0     5377 2023-11-23 19:01:39.111840 torch_geometric-2.5.2/torch_geometric/nn/pool/mem_pool.py
--rw-r--r--   0        0        0     4366 2023-11-23 19:01:39.111961 torch_geometric-2.5.2/torch_geometric/nn/pool/pan_pool.py
--rw-r--r--   0        0        0      631 2023-04-09 09:43:57.335862 torch_geometric-2.5.2/torch_geometric/nn/pool/pool.py
--rw-r--r--   0        0        0     5838 2023-11-23 19:01:39.112087 torch_geometric-2.5.2/torch_geometric/nn/pool/sag_pool.py
--rw-r--r--   0        0        0      254 2023-11-23 19:01:39.112224 torch_geometric-2.5.2/torch_geometric/nn/pool/select/__init__.py
--rw-r--r--   0        0        0     3311 2023-07-21 07:41:11.173771 torch_geometric-2.5.2/torch_geometric/nn/pool/select/base.py
--rw-r--r--   0        0        0     5305 2023-11-23 19:01:39.112366 torch_geometric-2.5.2/torch_geometric/nn/pool/select/topk.py
--rw-r--r--   0        0        0     5159 2023-11-23 19:01:39.112544 torch_geometric-2.5.2/torch_geometric/nn/pool/topk_pool.py
--rw-r--r--   0        0        0     2736 2023-11-23 19:01:39.112832 torch_geometric-2.5.2/torch_geometric/nn/pool/voxel_grid.py
--rw-r--r--   0        0        0      426 2023-11-23 19:01:39.112997 torch_geometric-2.5.2/torch_geometric/nn/reshape.py
--rw-r--r--   0        0        0     6155 2023-05-17 17:44:44.820088 torch_geometric-2.5.2/torch_geometric/nn/resolver.py
--rw-r--r--   0        0        0     1054 2024-02-15 14:55:33.361163 torch_geometric-2.5.2/torch_geometric/nn/sequential.jinja
--rw-r--r--   0        0        0     5534 2024-02-15 14:55:33.361344 torch_geometric-2.5.2/torch_geometric/nn/sequential.py
--rw-r--r--   0        0        0     5821 2023-08-24 05:09:46.605208 torch_geometric-2.5.2/torch_geometric/nn/summary.py
--rw-r--r--   0        0        0     1282 2023-04-09 09:43:57.336993 torch_geometric-2.5.2/torch_geometric/nn/to_fixed_size_transformer.py
--rw-r--r--   0        0        0     6519 2024-01-07 13:37:00.562075 torch_geometric-2.5.2/torch_geometric/nn/to_hetero_module.py
--rw-r--r--   0        0        0    18407 2023-11-23 19:01:39.113471 torch_geometric-2.5.2/torch_geometric/nn/to_hetero_transformer.py
--rw-r--r--   0        0        0    23121 2023-11-23 19:01:39.113662 torch_geometric-2.5.2/torch_geometric/nn/to_hetero_with_bases_transformer.py
--rw-r--r--   0        0        0      129 2023-11-23 19:01:39.113907 torch_geometric-2.5.2/torch_geometric/nn/unpool/__init__.py
--rw-r--r--   0        0        0     2586 2023-11-23 19:01:39.114022 torch_geometric-2.5.2/torch_geometric/nn/unpool/knn_interpolate.py
--rw-r--r--   0        0        0      863 2023-12-21 07:51:56.913994 torch_geometric-2.5.2/torch_geometric/profile/__init__.py
--rw-r--r--   0        0        0     5256 2023-11-23 19:01:39.114260 torch_geometric-2.5.2/torch_geometric/profile/benchmark.py
--rw-r--r--   0        0        0    11793 2023-12-21 07:51:56.914151 torch_geometric-2.5.2/torch_geometric/profile/profile.py
--rw-r--r--   0        0        0    16640 2023-11-23 19:01:39.114432 torch_geometric-2.5.2/torch_geometric/profile/profiler.py
--rw-r--r--   0        0        0     5497 2023-12-21 07:51:56.914275 torch_geometric-2.5.2/torch_geometric/profile/utils.py
--rw-r--r--   0        0        0     1273 2023-12-21 07:51:56.914372 torch_geometric-2.5.2/torch_geometric/resolver.py
--rw-r--r--   0        0        0      512 2023-11-23 19:01:39.114690 torch_geometric-2.5.2/torch_geometric/sampler/__init__.py
--rw-r--r--   0        0        0    25968 2024-02-15 14:55:33.361475 torch_geometric-2.5.2/torch_geometric/sampler/base.py
--rw-r--r--   0        0        0     2721 2023-11-23 19:01:39.114973 torch_geometric-2.5.2/torch_geometric/sampler/hgt_sampler.py
--rw-r--r--   0        0        0    33850 2024-02-11 12:50:44.324845 torch_geometric-2.5.2/torch_geometric/sampler/neighbor_sampler.py
--rw-r--r--   0        0        0     5492 2023-12-31 08:35:31.856681 torch_geometric-2.5.2/torch_geometric/sampler/utils.py
--rw-r--r--   0        0        0      372 2023-12-21 07:51:56.914460 torch_geometric-2.5.2/torch_geometric/seed.py
--rw-r--r--   0        0        0     1040 2024-03-05 12:38:29.030270 torch_geometric-2.5.2/torch_geometric/template.py
--rw-r--r--   0        0        0     1161 2024-03-20 18:30:51.599301 torch_geometric-2.5.2/torch_geometric/testing/__init__.py
--rw-r--r--   0        0        0     4606 2023-12-21 07:51:56.914584 torch_geometric-2.5.2/torch_geometric/testing/asserts.py
--rw-r--r--   0        0        0     2604 2023-12-21 07:51:56.914840 torch_geometric-2.5.2/torch_geometric/testing/data.py
--rw-r--r--   0        0        0     6736 2024-03-20 18:30:51.599528 torch_geometric-2.5.2/torch_geometric/testing/decorators.py
--rw-r--r--   0        0        0     2181 2024-03-20 18:30:51.599718 torch_geometric-2.5.2/torch_geometric/testing/feature_store.py
--rw-r--r--   0        0        0     1044 2023-12-21 07:51:56.915619 torch_geometric-2.5.2/torch_geometric/testing/graph_store.py
--rw-r--r--   0        0        0     4181 2023-08-24 05:09:46.605333 torch_geometric-2.5.2/torch_geometric/transforms/__init__.py
--rw-r--r--   0        0        0    14223 2023-12-31 08:35:31.857021 torch_geometric-2.5.2/torch_geometric/transforms/add_metapaths.py
--rw-r--r--   0        0        0     6051 2024-03-20 18:30:51.599923 torch_geometric-2.5.2/torch_geometric/transforms/add_positional_encoding.py
--rw-r--r--   0        0        0     2085 2023-12-21 07:51:56.916523 torch_geometric-2.5.2/torch_geometric/transforms/add_remaining_self_loops.py
--rw-r--r--   0        0        0     2024 2023-12-21 07:51:56.916642 torch_geometric-2.5.2/torch_geometric/transforms/add_self_loops.py
--rw-r--r--   0        0        0     1298 2023-05-29 07:55:13.281284 torch_geometric-2.5.2/torch_geometric/transforms/base_transform.py
--rw-r--r--   0        0        0     2464 2023-12-21 07:51:56.917071 torch_geometric-2.5.2/torch_geometric/transforms/cartesian.py
--rw-r--r--   0        0        0      645 2023-11-23 19:01:39.116658 torch_geometric-2.5.2/torch_geometric/transforms/center.py
--rw-r--r--   0        0        0     1658 2023-05-29 07:55:13.281683 torch_geometric-2.5.2/torch_geometric/transforms/compose.py
--rw-r--r--   0        0        0     2005 2023-12-21 07:51:56.917174 torch_geometric-2.5.2/torch_geometric/transforms/constant.py
--rw-r--r--   0        0        0     1264 2023-12-21 07:51:56.917270 torch_geometric-2.5.2/torch_geometric/transforms/delaunay.py
--rw-r--r--   0        0        0     2360 2023-12-21 07:51:56.917398 torch_geometric-2.5.2/torch_geometric/transforms/distance.py
--rw-r--r--   0        0        0     1083 2023-12-21 07:51:56.917497 torch_geometric-2.5.2/torch_geometric/transforms/face_to_edge.py
--rw-r--r--   0        0        0     3056 2023-12-21 07:51:56.917600 torch_geometric-2.5.2/torch_geometric/transforms/feature_propagation.py
--rw-r--r--   0        0        0     2426 2023-12-21 07:51:56.917699 torch_geometric-2.5.2/torch_geometric/transforms/fixed_points.py
--rw-r--r--   0        0        0     1397 2023-05-29 07:55:13.282572 torch_geometric-2.5.2/torch_geometric/transforms/gcn_norm.py
--rw-r--r--   0        0        0    20201 2023-12-21 07:51:56.918013 torch_geometric-2.5.2/torch_geometric/transforms/gdc.py
--rw-r--r--   0        0        0     1021 2024-03-20 18:30:51.600089 torch_geometric-2.5.2/torch_geometric/transforms/generate_mesh_normals.py
--rw-r--r--   0        0        0     2564 2023-12-21 07:51:56.918223 torch_geometric-2.5.2/torch_geometric/transforms/grid_sampling.py
--rw-r--r--   0        0        0     4102 2023-12-21 07:51:56.918364 torch_geometric-2.5.2/torch_geometric/transforms/half_hop.py
--rw-r--r--   0        0        0     2536 2023-12-21 07:51:56.918475 torch_geometric-2.5.2/torch_geometric/transforms/knn_graph.py
--rw-r--r--   0        0        0     2497 2023-12-21 07:51:56.918581 torch_geometric-2.5.2/torch_geometric/transforms/laplacian_lambda_max.py
--rw-r--r--   0        0        0     2161 2024-02-15 14:55:33.362033 torch_geometric-2.5.2/torch_geometric/transforms/largest_connected_components.py
--rw-r--r--   0        0        0     3730 2023-12-21 07:51:56.918778 torch_geometric-2.5.2/torch_geometric/transforms/line_graph.py
--rw-r--r--   0        0        0     1997 2023-11-23 19:01:39.117385 torch_geometric-2.5.2/torch_geometric/transforms/linear_transformation.py
--rw-r--r--   0        0        0     2144 2023-12-21 07:51:56.918876 torch_geometric-2.5.2/torch_geometric/transforms/local_cartesian.py
--rw-r--r--   0        0        0     1480 2023-12-21 07:51:56.918976 torch_geometric-2.5.2/torch_geometric/transforms/local_degree_profile.py
--rw-r--r--   0        0        0     4813 2023-12-21 07:51:56.919110 torch_geometric-2.5.2/torch_geometric/transforms/mask.py
--rw-r--r--   0        0        0     6088 2023-11-23 19:01:39.117647 torch_geometric-2.5.2/torch_geometric/transforms/node_property_split.py
--rw-r--r--   0        0        0     1028 2023-05-29 07:55:13.284273 torch_geometric-2.5.2/torch_geometric/transforms/normalize_features.py
--rw-r--r--   0        0        0     1782 2023-12-21 07:51:56.919212 torch_geometric-2.5.2/torch_geometric/transforms/normalize_rotation.py
--rw-r--r--   0        0        0      666 2023-12-21 07:51:56.919305 torch_geometric-2.5.2/torch_geometric/transforms/normalize_scale.py
--rw-r--r--   0        0        0     1584 2023-12-21 07:51:56.919388 torch_geometric-2.5.2/torch_geometric/transforms/one_hot_degree.py
--rw-r--r--   0        0        0    21047 2023-12-21 07:51:56.919508 torch_geometric-2.5.2/torch_geometric/transforms/pad.py
--rw-r--r--   0        0        0     1794 2023-11-23 19:01:39.117925 torch_geometric-2.5.2/torch_geometric/transforms/point_pair_features.py
--rw-r--r--   0        0        0     2213 2023-12-21 07:51:56.919629 torch_geometric-2.5.2/torch_geometric/transforms/polar.py
--rw-r--r--   0        0        0     2043 2023-12-21 07:51:56.919729 torch_geometric-2.5.2/torch_geometric/transforms/radius_graph.py
--rw-r--r--   0        0        0     1033 2023-12-21 07:51:56.919836 torch_geometric-2.5.2/torch_geometric/transforms/random_flip.py
--rw-r--r--   0        0        0     1721 2023-12-21 07:51:56.919934 torch_geometric-2.5.2/torch_geometric/transforms/random_jitter.py
--rw-r--r--   0        0        0    15174 2023-12-21 07:51:56.920164 torch_geometric-2.5.2/torch_geometric/transforms/random_link_split.py
--rw-r--r--   0        0        0     5853 2023-12-21 07:51:56.920287 torch_geometric-2.5.2/torch_geometric/transforms/random_node_split.py
--rw-r--r--   0        0        0     1946 2023-12-21 07:51:56.920388 torch_geometric-2.5.2/torch_geometric/transforms/random_rotate.py
--rw-r--r--   0        0        0     1261 2023-12-21 07:51:56.920489 torch_geometric-2.5.2/torch_geometric/transforms/random_scale.py
--rw-r--r--   0        0        0     1365 2023-12-21 07:51:56.920588 torch_geometric-2.5.2/torch_geometric/transforms/random_shear.py
--rw-r--r--   0        0        0     1929 2023-12-21 07:51:56.920688 torch_geometric-2.5.2/torch_geometric/transforms/remove_duplicated_edges.py
--rw-r--r--   0        0        0     2449 2023-12-21 07:51:56.920778 torch_geometric-2.5.2/torch_geometric/transforms/remove_isolated_nodes.py
--rw-r--r--   0        0        0      932 2023-07-21 07:41:11.175066 torch_geometric-2.5.2/torch_geometric/transforms/remove_training_classes.py
--rw-r--r--   0        0        0     6509 2023-12-21 07:51:56.920901 torch_geometric-2.5.2/torch_geometric/transforms/rooted_subgraph.py
--rw-r--r--   0        0        0     2214 2024-03-20 18:30:51.600256 torch_geometric-2.5.2/torch_geometric/transforms/sample_points.py
--rw-r--r--   0        0        0     2329 2023-12-31 08:35:31.857403 torch_geometric-2.5.2/torch_geometric/transforms/sign.py
--rw-r--r--   0        0        0     2320 2023-12-21 07:51:56.921167 torch_geometric-2.5.2/torch_geometric/transforms/spherical.py
--rw-r--r--   0        0        0     1009 2023-12-21 07:51:56.921248 torch_geometric-2.5.2/torch_geometric/transforms/svd_feature_reduction.py
--rw-r--r--   0        0        0     1659 2023-12-21 07:51:56.921334 torch_geometric-2.5.2/torch_geometric/transforms/target_indegree.py
--rw-r--r--   0        0        0     2456 2023-12-21 07:51:56.921417 torch_geometric-2.5.2/torch_geometric/transforms/to_dense.py
--rw-r--r--   0        0        0     1470 2023-12-21 07:51:56.921516 torch_geometric-2.5.2/torch_geometric/transforms/to_device.py
--rw-r--r--   0        0        0     5544 2023-12-21 07:51:56.921652 torch_geometric-2.5.2/torch_geometric/transforms/to_sparse_tensor.py
--rw-r--r--   0        0        0     2697 2023-12-21 07:51:56.921749 torch_geometric-2.5.2/torch_geometric/transforms/to_superpixels.py
--rw-r--r--   0        0        0     2972 2023-05-29 07:55:13.287697 torch_geometric-2.5.2/torch_geometric/transforms/to_undirected.py
--rw-r--r--   0        0        0     1295 2023-12-21 07:51:56.921852 torch_geometric-2.5.2/torch_geometric/transforms/two_hop.py
--rw-r--r--   0        0        0     2860 2023-12-21 07:51:56.921942 torch_geometric-2.5.2/torch_geometric/transforms/virtual_node.py
--rw-r--r--   0        0        0    13164 2024-03-20 18:30:51.600510 torch_geometric-2.5.2/torch_geometric/typing.py
--rw-r--r--   0        0        0     4762 2024-03-20 18:30:51.600922 torch_geometric-2.5.2/torch_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2347 2023-12-21 07:51:56.922253 torch_geometric-2.5.2/torch_geometric/utils/_assortativity.py
--rw-r--r--   0        0        0     6769 2024-02-15 14:55:33.362583 torch_geometric-2.5.2/torch_geometric/utils/_coalesce.py
--rw-r--r--   0        0        0     1017 2023-12-21 07:51:56.922548 torch_geometric-2.5.2/torch_geometric/utils/_degree.py
--rw-r--r--   0        0        0     2562 2023-12-21 07:51:56.922604 torch_geometric-2.5.2/torch_geometric/utils/_grid.py
--rw-r--r--   0        0        0     5090 2023-12-21 07:51:56.922694 torch_geometric-2.5.2/torch_geometric/utils/_homophily.py
--rw-r--r--   0        0        0     1283 2024-01-07 13:37:00.562198 torch_geometric-2.5.2/torch_geometric/utils/_index_sort.py
--rw-r--r--   0        0        0     1403 2023-12-21 07:51:56.922813 torch_geometric-2.5.2/torch_geometric/utils/_lexsort.py
--rw-r--r--   0        0        0    14672 2023-12-21 07:51:56.922888 torch_geometric-2.5.2/torch_geometric/utils/_negative_sampling.py
--rw-r--r--   0        0        0     1167 2023-12-21 07:51:56.923075 torch_geometric-2.5.2/torch_geometric/utils/_normalized_cut.py
--rw-r--r--   0        0        0     1404 2023-12-21 07:51:56.923295 torch_geometric-2.5.2/torch_geometric/utils/_one_hot.py
--rw-r--r--   0        0        0    11532 2024-03-20 18:30:51.601163 torch_geometric-2.5.2/torch_geometric/utils/_scatter.py
--rw-r--r--   0        0        0     1868 2024-03-20 18:30:51.601356 torch_geometric-2.5.2/torch_geometric/utils/_segment.py
--rw-r--r--   0        0        0     2439 2023-12-21 07:51:56.923526 torch_geometric-2.5.2/torch_geometric/utils/_select.py
--rw-r--r--   0        0        0     3177 2024-03-20 18:30:51.601503 torch_geometric-2.5.2/torch_geometric/utils/_softmax.py
--rw-r--r--   0        0        0     4500 2024-02-15 14:55:33.362919 torch_geometric-2.5.2/torch_geometric/utils/_sort_edge_index.py
--rw-r--r--   0        0        0     5542 2024-03-20 18:30:51.601718 torch_geometric-2.5.2/torch_geometric/utils/_spmm.py
--rw-r--r--   0        0        0    18311 2024-01-16 19:07:07.477049 torch_geometric-2.5.2/torch_geometric/utils/_subgraph.py
--rw-r--r--   0        0        0     3606 2023-12-21 07:51:56.924061 torch_geometric-2.5.2/torch_geometric/utils/_to_dense_adj.py
--rw-r--r--   0        0        0     4582 2023-12-21 07:51:56.924154 torch_geometric-2.5.2/torch_geometric/utils/_to_dense_batch.py
--rw-r--r--   0        0        0     3569 2023-12-21 07:51:56.924210 torch_geometric-2.5.2/torch_geometric/utils/_train_test_split_edges.py
--rw-r--r--   0        0        0     5300 2023-12-21 07:51:56.924298 torch_geometric-2.5.2/torch_geometric/utils/_tree_decomposition.py
--rw-r--r--   0        0        0     8412 2024-03-20 18:30:51.601932 torch_geometric-2.5.2/torch_geometric/utils/_trim_to_layer.py
--rw-r--r--   0        0        0     2378 2023-12-21 07:51:56.924478 torch_geometric-2.5.2/torch_geometric/utils/_unbatch.py
--rw-r--r--   0        0        0     8601 2023-12-21 07:51:56.924662 torch_geometric-2.5.2/torch_geometric/utils/augmentation.py
--rw-r--r--   0        0        0    21571 2023-12-21 07:51:56.924784 torch_geometric-2.5.2/torch_geometric/utils/convert.py
--rw-r--r--   0        0        0     3047 2023-12-21 07:51:56.924887 torch_geometric-2.5.2/torch_geometric/utils/cross_entropy.py
--rw-r--r--   0        0        0    11416 2024-01-07 13:37:00.563553 torch_geometric-2.5.2/torch_geometric/utils/dropout.py
--rw-r--r--   0        0        0     1675 2023-12-21 07:51:56.925133 torch_geometric-2.5.2/torch_geometric/utils/embedding.py
--rw-r--r--   0        0        0      703 2023-11-23 19:01:39.121419 torch_geometric-2.5.2/torch_geometric/utils/functions.py
--rw-r--r--   0        0        0     4626 2024-03-20 18:30:51.602158 torch_geometric-2.5.2/torch_geometric/utils/geodesic.py
--rw-r--r--   0        0        0     5542 2024-02-15 14:55:33.363124 torch_geometric-2.5.2/torch_geometric/utils/hetero.py
--rw-r--r--   0        0        0     3588 2023-12-21 07:51:56.925463 torch_geometric-2.5.2/torch_geometric/utils/isolated.py
--rw-r--r--   0        0        0     3695 2023-12-21 07:51:56.925525 torch_geometric-2.5.2/torch_geometric/utils/laplacian.py
--rw-r--r--   0        0        0    22950 2024-03-20 18:30:51.602366 torch_geometric-2.5.2/torch_geometric/utils/loop.py
--rw-r--r--   0        0        0     5674 2023-12-21 07:51:56.925752 torch_geometric-2.5.2/torch_geometric/utils/map.py
--rw-r--r--   0        0        0     2340 2023-11-23 19:01:39.122614 torch_geometric-2.5.2/torch_geometric/utils/mask.py
--rw-r--r--   0        0        0     4387 2023-12-21 07:51:56.925857 torch_geometric-2.5.2/torch_geometric/utils/mesh_laplacian.py
--rw-r--r--   0        0        0      699 2023-12-21 07:51:56.925943 torch_geometric-2.5.2/torch_geometric/utils/mixin.py
--rw-r--r--   0        0        0     3310 2023-12-21 07:51:56.926263 torch_geometric-2.5.2/torch_geometric/utils/nested.py
--rw-r--r--   0        0        0     3750 2023-12-21 07:51:56.926325 torch_geometric-2.5.2/torch_geometric/utils/noise_scheduler.py
--rw-r--r--   0        0        0     2176 2024-01-16 19:07:07.477793 torch_geometric-2.5.2/torch_geometric/utils/num_nodes.py
--rw-r--r--   0        0        0     4055 2023-12-31 08:35:31.857981 torch_geometric-2.5.2/torch_geometric/utils/ppr.py
--rw-r--r--   0        0        0     5148 2023-11-23 19:01:39.123097 torch_geometric-2.5.2/torch_geometric/utils/random.py
--rw-r--r--   0        0        0      815 2023-06-10 14:35:51.131530 torch_geometric-2.5.2/torch_geometric/utils/repeat.py
--rw-r--r--   0        0        0     6242 2023-12-21 07:51:56.926536 torch_geometric-2.5.2/torch_geometric/utils/smiles.py
--rw-r--r--   0        0        0    25034 2024-01-16 19:07:07.478083 torch_geometric-2.5.2/torch_geometric/utils/sparse.py
--rw-r--r--   0        0        0     6222 2023-12-21 07:51:56.927152 torch_geometric-2.5.2/torch_geometric/utils/undirected.py
--rw-r--r--   0        0        0      154 2023-11-23 19:01:39.124605 torch_geometric-2.5.2/torch_geometric/visualization/__init__.py
--rw-r--r--   0        0        0     4813 2024-02-15 14:55:33.363335 torch_geometric-2.5.2/torch_geometric/visualization/graph.py
--rw-r--r--   0        0        0      477 2023-12-21 07:51:56.927546 torch_geometric-2.5.2/torch_geometric/visualization/influence.py
--rw-r--r--   0        0        0      413 2024-01-07 13:37:00.563808 torch_geometric-2.5.2/torch_geometric/warnings.py
--rw-r--r--   0        0        0    64156 1970-01-01 00:00:00.000000 torch_geometric-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0    61058 2024-04-19 11:45:50.596416 torch_geometric-2.5.3/README.md
+-rw-r--r--   0        0        0     5178 2024-04-19 11:45:50.608879 torch_geometric-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1197 2024-04-19 11:45:50.627499 torch_geometric-2.5.3/torch_geometric/__init__.py
+-rw-r--r--   0        0        0     1053 2024-01-16 19:07:07.463648 torch_geometric-2.5.3/torch_geometric/_compile.py
+-rw-r--r--   0        0        0     1575 2024-02-15 14:55:33.351472 torch_geometric-2.5.3/torch_geometric/backend.py
+-rw-r--r--   0        0        0    16514 2023-12-21 07:51:56.890107 torch_geometric-2.5.3/torch_geometric/config_store.py
+-rw-r--r--   0        0        0      352 2023-04-09 09:43:57.297670 torch_geometric-2.5.3/torch_geometric/contrib/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-09 09:43:57.297729 torch_geometric-2.5.3/torch_geometric/contrib/datasets/__init__.py
+-rw-r--r--   0        0        0      396 2023-09-21 09:55:53.973502 torch_geometric-2.5.3/torch_geometric/contrib/explain/__init__.py
+-rw-r--r--   0        0        0    16972 2023-12-21 07:51:56.890605 torch_geometric-2.5.3/torch_geometric/contrib/explain/pgm_explainer.py
+-rw-r--r--   0        0        0       72 2023-04-09 09:43:57.298115 torch_geometric-2.5.3/torch_geometric/contrib/nn/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-09 09:43:57.298178 torch_geometric-2.5.3/torch_geometric/contrib/nn/conv/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-09 09:43:57.298237 torch_geometric-2.5.3/torch_geometric/contrib/nn/models/__init__.py
+-rw-r--r--   0        0        0    33280 2023-11-23 19:01:39.064213 torch_geometric-2.5.3/torch_geometric/contrib/nn/models/rbcd_attack.py
+-rw-r--r--   0        0        0       23 2023-04-09 09:43:57.298451 torch_geometric-2.5.3/torch_geometric/contrib/transforms/__init__.py
+-rw-r--r--   0        0        0     3882 2024-02-15 14:55:33.351611 torch_geometric-2.5.3/torch_geometric/data/__init__.py
+-rw-r--r--   0        0        0     8767 2023-12-28 11:34:13.526894 torch_geometric-2.5.3/torch_geometric/data/batch.py
+-rw-r--r--   0        0        0    12471 2024-01-07 13:37:00.549321 torch_geometric-2.5.3/torch_geometric/data/collate.py
+-rw-r--r--   0        0        0    43328 2023-12-21 07:51:56.891442 torch_geometric-2.5.3/torch_geometric/data/data.py
+-rw-r--r--   0        0        0    21247 2024-04-19 11:45:50.628121 torch_geometric-2.5.3/torch_geometric/data/database.py
+-rw-r--r--   0        0        0     3083 2023-12-28 11:34:13.528318 torch_geometric-2.5.3/torch_geometric/data/datapipes.py
+-rw-r--r--   0        0        0    16402 2024-03-05 12:38:29.026374 torch_geometric-2.5.3/torch_geometric/data/dataset.py
+-rw-r--r--   0        0        0     1889 2024-02-15 14:55:33.351729 torch_geometric-2.5.3/torch_geometric/data/download.py
+-rw-r--r--   0        0        0     2324 2023-12-28 11:34:13.528775 torch_geometric-2.5.3/torch_geometric/data/extract.py
+-rw-r--r--   0        0        0    20805 2024-04-19 11:45:50.628632 torch_geometric-2.5.3/torch_geometric/data/feature_store.py
+-rw-r--r--   0        0        0    13916 2024-04-19 11:45:50.629014 torch_geometric-2.5.3/torch_geometric/data/graph_store.py
+-rw-r--r--   0        0        0    47550 2024-02-15 14:55:33.351880 torch_geometric-2.5.3/torch_geometric/data/hetero_data.py
+-rw-r--r--   0        0        0     8294 2023-12-28 11:34:13.529285 torch_geometric-2.5.3/torch_geometric/data/hypergraph_data.py
+-rw-r--r--   0        0        0    13513 2024-03-05 12:38:29.027252 torch_geometric-2.5.3/torch_geometric/data/in_memory_dataset.py
+-rw-r--r--   0        0        0      178 2023-04-09 09:43:57.300134 torch_geometric-2.5.3/torch_geometric/data/lightning/__init__.py
+-rw-r--r--   0        0        0    29244 2024-02-15 14:55:33.352116 torch_geometric-2.5.3/torch_geometric/data/lightning/datamodule.py
+-rw-r--r--   0        0        0      463 2023-11-23 19:01:39.066347 torch_geometric-2.5.3/torch_geometric/data/makedirs.py
+-rw-r--r--   0        0        0     6629 2023-12-28 11:34:13.529685 torch_geometric-2.5.3/torch_geometric/data/on_disk_dataset.py
+-rw-r--r--   0        0        0     4503 2023-12-28 11:34:13.530160 torch_geometric-2.5.3/torch_geometric/data/remote_backend_utils.py
+-rw-r--r--   0        0        0     5319 2023-12-31 08:35:31.852239 torch_geometric-2.5.3/torch_geometric/data/separate.py
+-rw-r--r--   0        0        0    31562 2024-04-19 11:45:50.629589 torch_geometric-2.5.3/torch_geometric/data/storage.py
+-rw-r--r--   0        0        0     5375 2023-12-28 11:34:13.531203 torch_geometric-2.5.3/torch_geometric/data/summary.py
+-rw-r--r--   0        0        0    10055 2023-12-21 07:51:56.893168 torch_geometric-2.5.3/torch_geometric/data/temporal.py
+-rw-r--r--   0        0        0     1089 2023-12-21 07:51:56.893489 torch_geometric-2.5.3/torch_geometric/data/view.py
+-rw-r--r--   0        0        0     5637 2024-04-19 11:45:50.629941 torch_geometric-2.5.3/torch_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4471 2023-12-21 07:51:56.893651 torch_geometric-2.5.3/torch_geometric/datasets/actor.py
+-rw-r--r--   0        0        0     5666 2023-12-21 07:51:56.893783 torch_geometric-2.5.3/torch_geometric/datasets/airfrans.py
+-rw-r--r--   0        0        0     3913 2023-12-21 07:51:56.893895 torch_geometric-2.5.3/torch_geometric/datasets/airports.py
+-rw-r--r--   0        0        0     3179 2023-12-21 07:51:56.894019 torch_geometric-2.5.3/torch_geometric/datasets/amazon.py
+-rw-r--r--   0        0        0     3362 2023-12-21 07:51:56.894133 torch_geometric-2.5.3/torch_geometric/datasets/amazon_book.py
+-rw-r--r--   0        0        0     3964 2024-02-15 14:55:33.352468 torch_geometric-2.5.3/torch_geometric/datasets/amazon_products.py
+-rw-r--r--   0        0        0     5178 2023-12-21 07:51:56.894398 torch_geometric-2.5.3/torch_geometric/datasets/aminer.py
+-rw-r--r--   0        0        0     5455 2023-12-21 07:51:56.894546 torch_geometric-2.5.3/torch_geometric/datasets/aqsol.py
+-rw-r--r--   0        0        0     5975 2024-02-15 14:55:33.352805 torch_geometric-2.5.3/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-r--r--   0        0        0     4258 2023-12-21 07:51:56.894811 torch_geometric-2.5.3/torch_geometric/datasets/ba2motif_dataset.py
+-rw-r--r--   0        0        0     3700 2023-12-21 07:51:56.894907 torch_geometric-2.5.3/torch_geometric/datasets/ba_multi_shapes.py
+-rw-r--r--   0        0        0     3904 2023-12-21 07:51:56.895012 torch_geometric-2.5.3/torch_geometric/datasets/ba_shapes.py
+-rw-r--r--   0        0        0     4404 2023-12-21 07:51:56.895155 torch_geometric-2.5.3/torch_geometric/datasets/bitcoin_otc.py
+-rw-r--r--   0        0        0     3959 2023-12-21 07:51:56.895693 torch_geometric-2.5.3/torch_geometric/datasets/brca_tgca.py
+-rw-r--r--   0        0        0     4458 2023-12-21 07:51:56.895825 torch_geometric-2.5.3/torch_geometric/datasets/citation_full.py
+-rw-r--r--   0        0        0     3138 2023-12-21 07:51:56.895951 torch_geometric-2.5.3/torch_geometric/datasets/coauthor.py
+-rw-r--r--   0        0        0     4734 2023-12-21 07:51:56.896208 torch_geometric-2.5.3/torch_geometric/datasets/coma.py
+-rw-r--r--   0        0        0     5416 2023-12-21 07:51:56.896338 torch_geometric-2.5.3/torch_geometric/datasets/dblp.py
+-rw-r--r--   0        0        0     5707 2024-02-15 14:55:33.353020 torch_geometric-2.5.3/torch_geometric/datasets/dbp15k.py
+-rw-r--r--   0        0        0     2511 2023-12-21 07:51:56.896613 torch_geometric-2.5.3/torch_geometric/datasets/deezer_europe.py
+-rw-r--r--   0        0        0     4035 2023-12-21 07:51:56.896734 torch_geometric-2.5.3/torch_geometric/datasets/dgraph.py
+-rw-r--r--   0        0        0     6041 2023-12-21 07:51:56.896863 torch_geometric-2.5.3/torch_geometric/datasets/dynamic_faust.py
+-rw-r--r--   0        0        0     4605 2023-12-21 07:51:56.897104 torch_geometric-2.5.3/torch_geometric/datasets/elliptic.py
+-rw-r--r--   0        0        0     3188 2023-11-30 06:56:02.055205 torch_geometric-2.5.3/torch_geometric/datasets/elliptic_temporal.py
+-rw-r--r--   0        0        0     2834 2023-12-21 07:51:56.897222 torch_geometric-2.5.3/torch_geometric/datasets/email_eu_core.py
+-rw-r--r--   0        0        0     7312 2024-04-19 11:45:50.630358 torch_geometric-2.5.3/torch_geometric/datasets/entities.py
+-rw-r--r--   0        0        0     6103 2023-12-21 07:51:56.897750 torch_geometric-2.5.3/torch_geometric/datasets/explainer_dataset.py
+-rw-r--r--   0        0        0     2431 2023-12-21 07:51:56.897836 torch_geometric-2.5.3/torch_geometric/datasets/facebook.py
+-rw-r--r--   0        0        0    10554 2024-01-07 13:37:00.549728 torch_geometric-2.5.3/torch_geometric/datasets/fake.py
+-rw-r--r--   0        0        0     4076 2023-12-21 07:51:56.898087 torch_geometric-2.5.3/torch_geometric/datasets/faust.py
+-rw-r--r--   0        0        0     3964 2024-02-15 14:55:33.353369 torch_geometric-2.5.3/torch_geometric/datasets/flickr.py
+-rw-r--r--   0        0        0     4080 2023-12-21 07:51:56.898313 torch_geometric-2.5.3/torch_geometric/datasets/freebase.py
+-rw-r--r--   0        0        0     3598 2023-12-21 07:51:56.898404 torch_geometric-2.5.3/torch_geometric/datasets/gdelt.py
+-rw-r--r--   0        0        0     3189 2023-12-21 07:51:56.898486 torch_geometric-2.5.3/torch_geometric/datasets/gdelt_lite.py
+-rw-r--r--   0        0        0     9511 2024-02-15 14:55:33.353533 torch_geometric-2.5.3/torch_geometric/datasets/ged_dataset.py
+-rw-r--r--   0        0        0     2820 2023-12-21 07:51:56.898839 torch_geometric-2.5.3/torch_geometric/datasets/gemsec.py
+-rw-r--r--   0        0        0     4223 2023-12-21 07:51:56.898997 torch_geometric-2.5.3/torch_geometric/datasets/geometry.py
+-rw-r--r--   0        0        0     2687 2023-12-21 07:51:56.899128 torch_geometric-2.5.3/torch_geometric/datasets/github.py
+-rw-r--r--   0        0        0     6940 2024-04-19 11:45:50.630658 torch_geometric-2.5.3/torch_geometric/datasets/gnn_benchmark_dataset.py
+-rw-r--r--   0        0        0      272 2024-01-16 19:07:07.464900 torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/__init__.py
+-rw-r--r--   0        0        0      965 2023-04-09 09:43:57.304447 torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-r--r--   0        0        0      939 2023-12-21 07:51:56.899387 torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/base.py
+-rw-r--r--   0        0        0      918 2023-04-09 09:43:57.304551 torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-r--r--   0        0        0     1159 2023-04-09 09:43:57.304609 torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-r--r--   0        0        0     2599 2024-01-16 19:07:07.464998 torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/tree_graph.py
+-rw-r--r--   0        0        0     4224 2023-12-21 07:51:56.899658 torch_geometric-2.5.3/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-r--r--   0        0        0     8846 2024-02-15 14:55:33.353696 torch_geometric-2.5.3/torch_geometric/datasets/hgb_dataset.py
+-rw-r--r--   0        0        0     6763 2023-12-21 07:51:56.900559 torch_geometric-2.5.3/torch_geometric/datasets/hm.py
+-rw-r--r--   0        0        0    11417 2023-12-21 07:51:56.900734 torch_geometric-2.5.3/torch_geometric/datasets/hydro_net.py
+-rw-r--r--   0        0        0     4735 2023-12-21 07:51:56.900899 torch_geometric-2.5.3/torch_geometric/datasets/icews.py
+-rw-r--r--   0        0        0     4611 2023-12-21 07:51:56.901264 torch_geometric-2.5.3/torch_geometric/datasets/igmc_dataset.py
+-rw-r--r--   0        0        0     4223 2023-12-21 07:51:56.901418 torch_geometric-2.5.3/torch_geometric/datasets/imdb.py
+-rw-r--r--   0        0        0     7293 2023-12-21 07:51:56.901564 torch_geometric-2.5.3/torch_geometric/datasets/infection_dataset.py
+-rw-r--r--   0        0        0     3643 2023-12-21 07:51:56.901672 torch_geometric-2.5.3/torch_geometric/datasets/jodie.py
+-rw-r--r--   0        0        0     3445 2023-11-23 19:01:39.073186 torch_geometric-2.5.3/torch_geometric/datasets/karate.py
+-rw-r--r--   0        0        0     4572 2023-12-21 07:51:56.901818 torch_geometric-2.5.3/torch_geometric/datasets/last_fm.py
+-rw-r--r--   0        0        0     2486 2023-12-21 07:51:56.901934 torch_geometric-2.5.3/torch_geometric/datasets/lastfm_asia.py
+-rw-r--r--   0        0        0     6864 2024-02-15 14:55:33.353977 torch_geometric-2.5.3/torch_geometric/datasets/linkx_dataset.py
+-rw-r--r--   0        0        0    11746 2023-12-21 07:51:56.902238 torch_geometric-2.5.3/torch_geometric/datasets/lrgb.py
+-rw-r--r--   0        0        0     5244 2023-12-21 07:51:56.902365 torch_geometric-2.5.3/torch_geometric/datasets/malnet_tiny.py
+-rw-r--r--   0        0        0    16734 2023-12-21 07:51:56.902710 torch_geometric-2.5.3/torch_geometric/datasets/md17.py
+-rw-r--r--   0        0        0     3951 2023-12-21 07:51:56.902835 torch_geometric-2.5.3/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-r--r--   0        0        0     3317 2023-12-21 07:51:56.902958 torch_geometric-2.5.3/torch_geometric/datasets/mnist_superpixels.py
+-rw-r--r--   0        0        0     5347 2023-12-21 07:51:56.903210 torch_geometric-2.5.3/torch_geometric/datasets/modelnet.py
+-rw-r--r--   0        0        0     6783 2024-04-19 11:45:50.630950 torch_geometric-2.5.3/torch_geometric/datasets/molecule_net.py
+-rw-r--r--   0        0        0      272 2024-01-16 19:07:07.465139 torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/__init__.py
+-rw-r--r--   0        0        0      900 2023-12-21 07:51:56.903471 torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/base.py
+-rw-r--r--   0        0        0     1278 2023-12-21 07:51:56.903565 torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/custom.py
+-rw-r--r--   0        0        0      983 2024-01-16 19:07:07.465273 torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/cycle.py
+-rw-r--r--   0        0        0     1099 2024-01-16 19:07:07.465364 torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/grid.py
+-rw-r--r--   0        0        0      814 2023-12-21 07:51:56.903671 torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/house.py
+-rw-r--r--   0        0        0     4033 2023-12-21 07:51:56.903779 torch_geometric-2.5.3/torch_geometric/datasets/movie_lens.py
+-rw-r--r--   0        0        0     6057 2023-12-21 07:51:56.903937 torch_geometric-2.5.3/torch_geometric/datasets/movie_lens_100k.py
+-rw-r--r--   0        0        0     5396 2023-12-21 07:51:56.904066 torch_geometric-2.5.3/torch_geometric/datasets/movie_lens_1m.py
+-rw-r--r--   0        0        0     3008 2023-12-21 07:51:56.904161 torch_geometric-2.5.3/torch_geometric/datasets/myket.py
+-rw-r--r--   0        0        0     2863 2023-12-31 08:35:31.852876 torch_geometric-2.5.3/torch_geometric/datasets/nell.py
+-rw-r--r--   0        0        0     5196 2024-04-19 11:45:50.631225 torch_geometric-2.5.3/torch_geometric/datasets/neurograph.py
+-rw-r--r--   0        0        0     7481 2023-12-21 07:51:56.904554 torch_geometric-2.5.3/torch_geometric/datasets/ogb_mag.py
+-rw-r--r--   0        0        0     3585 2023-12-21 07:51:56.904682 torch_geometric-2.5.3/torch_geometric/datasets/omdb.py
+-rw-r--r--   0        0        0     5161 2023-12-21 07:51:56.904814 torch_geometric-2.5.3/torch_geometric/datasets/ose_gvcs.py
+-rw-r--r--   0        0        0     4162 2023-12-21 07:51:56.904940 torch_geometric-2.5.3/torch_geometric/datasets/particle.py
+-rw-r--r--   0        0        0    12031 2024-04-19 11:45:50.631566 torch_geometric-2.5.3/torch_geometric/datasets/pascal.py
+-rw-r--r--   0        0        0     4791 2023-12-21 07:51:56.905217 torch_geometric-2.5.3/torch_geometric/datasets/pascal_pf.py
+-rw-r--r--   0        0        0     5897 2023-12-21 07:51:56.905357 torch_geometric-2.5.3/torch_geometric/datasets/pcpnet_dataset.py
+-rw-r--r--   0        0        0     3813 2024-04-19 11:45:50.631884 torch_geometric-2.5.3/torch_geometric/datasets/pcqm4m.py
+-rw-r--r--   0        0        0     7201 2023-12-21 07:51:56.905713 torch_geometric-2.5.3/torch_geometric/datasets/planetoid.py
+-rw-r--r--   0        0        0     3045 2023-12-21 07:51:56.905813 torch_geometric-2.5.3/torch_geometric/datasets/polblogs.py
+-rw-r--r--   0        0        0     4999 2023-12-21 07:51:56.905939 torch_geometric-2.5.3/torch_geometric/datasets/ppi.py
+-rw-r--r--   0        0        0     3325 2023-12-21 07:51:56.906048 torch_geometric-2.5.3/torch_geometric/datasets/qm7.py
+-rw-r--r--   0        0        0    17158 2023-12-21 07:51:56.906164 torch_geometric-2.5.3/torch_geometric/datasets/qm9.py
+-rw-r--r--   0        0        0     5304 2024-02-15 14:55:33.354170 torch_geometric-2.5.3/torch_geometric/datasets/rcdd.py
+-rw-r--r--   0        0        0     3122 2023-12-21 07:51:56.906502 torch_geometric-2.5.3/torch_geometric/datasets/reddit.py
+-rw-r--r--   0        0        0     4282 2024-02-15 14:55:33.354362 torch_geometric-2.5.3/torch_geometric/datasets/reddit2.py
+-rw-r--r--   0        0        0     4535 2023-12-21 07:51:56.906762 torch_geometric-2.5.3/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-r--r--   0        0        0     4492 2023-12-21 07:51:56.906884 torch_geometric-2.5.3/torch_geometric/datasets/s3dis.py
+-rw-r--r--   0        0        0     8816 2023-12-28 11:34:13.531778 torch_geometric-2.5.3/torch_geometric/datasets/sbm_dataset.py
+-rw-r--r--   0        0        0     8504 2023-12-21 07:51:56.907179 torch_geometric-2.5.3/torch_geometric/datasets/shapenet.py
+-rw-r--r--   0        0        0     6316 2023-12-21 07:51:56.907413 torch_geometric-2.5.3/torch_geometric/datasets/shrec2016.py
+-rw-r--r--   0        0        0     9304 2024-04-19 11:45:50.632528 torch_geometric-2.5.3/torch_geometric/datasets/snap_dataset.py
+-rw-r--r--   0        0        0     3278 2023-12-21 07:51:56.907670 torch_geometric-2.5.3/torch_geometric/datasets/suite_sparse.py
+-rw-r--r--   0        0        0     4170 2023-12-21 07:51:56.907790 torch_geometric-2.5.3/torch_geometric/datasets/taobao.py
+-rw-r--r--   0        0        0     4632 2023-12-21 07:51:56.907904 torch_geometric-2.5.3/torch_geometric/datasets/tosca.py
+-rw-r--r--   0        0        0     7847 2023-12-31 08:35:31.853471 torch_geometric-2.5.3/torch_geometric/datasets/tu_dataset.py
+-rw-r--r--   0        0        0     3658 2023-12-21 07:51:56.908132 torch_geometric-2.5.3/torch_geometric/datasets/twitch.py
+-rw-r--r--   0        0        0     7001 2024-02-15 14:55:33.354555 torch_geometric-2.5.3/torch_geometric/datasets/upfd.py
+-rw-r--r--   0        0        0      182 2023-05-17 17:44:44.813472 torch_geometric-2.5.3/torch_geometric/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1835 2023-12-21 07:51:56.908367 torch_geometric-2.5.3/torch_geometric/datasets/utils/cheatsheet.py
+-rw-r--r--   0        0        0     4889 2023-12-21 07:51:56.908697 torch_geometric-2.5.3/torch_geometric/datasets/webkb.py
+-rw-r--r--   0        0        0     3884 2023-12-21 07:51:56.908797 torch_geometric-2.5.3/torch_geometric/datasets/wikics.py
+-rw-r--r--   0        0        0     4947 2024-02-15 14:55:33.354736 torch_geometric-2.5.3/torch_geometric/datasets/wikidata.py
+-rw-r--r--   0        0        0     6640 2023-12-21 07:51:56.909027 torch_geometric-2.5.3/torch_geometric/datasets/wikipedia_network.py
+-rw-r--r--   0        0        0     7017 2024-04-19 11:45:50.632839 torch_geometric-2.5.3/torch_geometric/datasets/willow_object_class.py
+-rw-r--r--   0        0        0     8158 2023-12-21 07:51:56.909388 torch_geometric-2.5.3/torch_geometric/datasets/word_net.py
+-rw-r--r--   0        0        0     3959 2024-02-15 14:55:33.354864 torch_geometric-2.5.3/torch_geometric/datasets/yelp.py
+-rw-r--r--   0        0        0     6347 2023-12-21 07:51:56.909622 torch_geometric-2.5.3/torch_geometric/datasets/zinc.py
+-rw-r--r--   0        0        0     1295 2023-12-21 07:51:56.909709 torch_geometric-2.5.3/torch_geometric/debug.py
+-rw-r--r--   0        0        0      858 2023-12-21 07:51:56.909796 torch_geometric-2.5.3/torch_geometric/deprecation.py
+-rw-r--r--   0        0        0      589 2023-11-23 19:01:39.080087 torch_geometric-2.5.3/torch_geometric/distributed/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-02 10:48:33.251092 torch_geometric-2.5.3/torch_geometric/distributed/dist_context.py
+-rw-r--r--   0        0        0     4933 2024-02-15 14:55:33.355095 torch_geometric-2.5.3/torch_geometric/distributed/dist_link_neighbor_loader.py
+-rw-r--r--   0        0        0     6492 2024-02-15 14:55:33.355288 torch_geometric-2.5.3/torch_geometric/distributed/dist_loader.py
+-rw-r--r--   0        0        0     4372 2024-02-15 14:55:33.355525 torch_geometric-2.5.3/torch_geometric/distributed/dist_neighbor_loader.py
+-rw-r--r--   0        0        0    42406 2024-02-15 14:55:33.356032 torch_geometric-2.5.3/torch_geometric/distributed/dist_neighbor_sampler.py
+-rw-r--r--   0        0        0     3309 2023-12-21 07:51:56.910896 torch_geometric-2.5.3/torch_geometric/distributed/event_loop.py
+-rw-r--r--   0        0        0    19018 2024-02-15 14:55:33.356215 torch_geometric-2.5.3/torch_geometric/distributed/local_feature_store.py
+-rw-r--r--   0        0        0     8408 2024-02-15 14:55:33.356438 torch_geometric-2.5.3/torch_geometric/distributed/local_graph_store.py
+-rw-r--r--   0        0        0    14675 2024-02-15 14:55:33.356739 torch_geometric-2.5.3/torch_geometric/distributed/partition.py
+-rw-r--r--   0        0        0     5753 2024-02-15 14:55:33.356938 torch_geometric-2.5.3/torch_geometric/distributed/rpc.py
+-rw-r--r--   0        0        0     6567 2024-02-15 14:55:33.357113 torch_geometric-2.5.3/torch_geometric/distributed/utils.py
+-rw-r--r--   0        0        0    61285 2024-04-19 11:45:50.633128 torch_geometric-2.5.3/torch_geometric/edge_index.py
+-rw-r--r--   0        0        0     4756 2023-12-21 07:51:56.911426 torch_geometric-2.5.3/torch_geometric/experimental.py
+-rw-r--r--   0        0        0      359 2023-04-09 09:43:57.309954 torch_geometric-2.5.3/torch_geometric/explain/__init__.py
+-rw-r--r--   0        0        0      496 2023-09-21 09:55:53.976137 torch_geometric-2.5.3/torch_geometric/explain/algorithm/__init__.py
+-rw-r--r--   0        0        0     4545 2023-11-23 19:01:39.081865 torch_geometric-2.5.3/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-r--r--   0        0        0     6935 2023-11-23 19:01:39.082059 torch_geometric-2.5.3/torch_geometric/explain/algorithm/base.py
+-rw-r--r--   0        0        0    12857 2023-11-30 06:56:02.065723 torch_geometric-2.5.3/torch_geometric/explain/algorithm/captum.py
+-rw-r--r--   0        0        0     7346 2023-11-30 06:56:02.065986 torch_geometric-2.5.3/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-r--r--   0        0        0     2872 2023-11-23 19:01:39.082529 torch_geometric-2.5.3/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-r--r--   0        0        0    12454 2023-11-23 19:01:39.082709 torch_geometric-2.5.3/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-r--r--   0        0        0    21389 2024-04-19 11:45:50.634100 torch_geometric-2.5.3/torch_geometric/explain/algorithm/graphmask_explainer.py
+-rw-r--r--   0        0        0    10371 2023-11-23 19:01:39.083036 torch_geometric-2.5.3/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-r--r--   0        0        0     2564 2023-11-23 19:01:39.083156 torch_geometric-2.5.3/torch_geometric/explain/algorithm/utils.py
+-rw-r--r--   0        0        0     7834 2023-04-09 09:43:57.310831 torch_geometric-2.5.3/torch_geometric/explain/config.py
+-rw-r--r--   0        0        0    10667 2023-11-23 19:01:39.083333 torch_geometric-2.5.3/torch_geometric/explain/explainer.py
+-rw-r--r--   0        0        0    14934 2024-02-15 14:55:33.357475 torch_geometric-2.5.3/torch_geometric/explain/explanation.py
+-rw-r--r--   0        0        0      301 2023-04-09 09:43:57.311049 torch_geometric-2.5.3/torch_geometric/explain/metric/__init__.py
+-rw-r--r--   0        0        0     1888 2023-11-23 19:01:39.083621 torch_geometric-2.5.3/torch_geometric/explain/metric/basic.py
+-rw-r--r--   0        0        0     3063 2023-04-09 09:43:57.311165 torch_geometric-2.5.3/torch_geometric/explain/metric/faithfulness.py
+-rw-r--r--   0        0        0     6157 2023-11-23 19:01:39.083749 torch_geometric-2.5.3/torch_geometric/explain/metric/fidelity.py
+-rw-r--r--   0        0        0     1815 2023-06-15 08:50:09.287832 torch_geometric-2.5.3/torch_geometric/graphgym/__init__.py
+-rw-r--r--   0        0        0      510 2023-04-09 09:43:57.311384 torch_geometric-2.5.3/torch_geometric/graphgym/benchmark.py
+-rw-r--r--   0        0        0     2371 2023-04-09 09:43:57.311450 torch_geometric-2.5.3/torch_geometric/graphgym/checkpoint.py
+-rw-r--r--   0        0        0      738 2023-04-09 09:43:57.311504 torch_geometric-2.5.3/torch_geometric/graphgym/cmd_args.py
+-rw-r--r--   0        0        0    17197 2023-11-30 06:56:02.066436 torch_geometric-2.5.3/torch_geometric/graphgym/config.py
+-rw-r--r--   0        0        0      389 2023-04-09 09:43:57.311792 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.311851 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/act/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.311908 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/config/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.311966 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/encoder/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312019 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/head/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312073 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-r--r--   0        0        0     8435 2023-11-23 19:01:39.084105 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/layer/generalconv.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312204 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/loader/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312257 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/loss/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312309 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/network/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312361 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/optimizer/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312413 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/pooling/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312465 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/stage/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312519 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/train/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-09 09:43:57.312571 torch_geometric-2.5.3/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-09 09:43:57.312622 torch_geometric-2.5.3/torch_geometric/graphgym/imports.py
+-rw-r--r--   0        0        0      521 2023-11-23 19:01:39.084212 torch_geometric-2.5.3/torch_geometric/graphgym/init.py
+-rw-r--r--   0        0        0    11605 2023-11-23 19:01:39.084371 torch_geometric-2.5.3/torch_geometric/graphgym/loader.py
+-rw-r--r--   0        0        0    11314 2023-11-23 19:01:39.084670 torch_geometric-2.5.3/torch_geometric/graphgym/logger.py
+-rw-r--r--   0        0        0     1445 2023-11-23 19:01:39.084807 torch_geometric-2.5.3/torch_geometric/graphgym/loss.py
+-rw-r--r--   0        0        0     3110 2023-05-17 17:44:44.813938 torch_geometric-2.5.3/torch_geometric/graphgym/model_builder.py
+-rw-r--r--   0        0        0     1121 2023-04-09 09:43:57.313035 torch_geometric-2.5.3/torch_geometric/graphgym/models/__init__.py
+-rw-r--r--   0        0        0      855 2023-09-21 09:55:53.976881 torch_geometric-2.5.3/torch_geometric/graphgym/models/act.py
+-rw-r--r--   0        0        0     3034 2023-11-23 19:01:39.084923 torch_geometric-2.5.3/torch_geometric/graphgym/models/encoder.py
+-rw-r--r--   0        0        0     6373 2023-09-21 09:55:53.977064 torch_geometric-2.5.3/torch_geometric/graphgym/models/gnn.py
+-rw-r--r--   0        0        0     4603 2023-09-21 09:55:53.977157 torch_geometric-2.5.3/torch_geometric/graphgym/models/head.py
+-rw-r--r--   0        0        0    12500 2023-12-04 06:33:33.769780 torch_geometric-2.5.3/torch_geometric/graphgym/models/layer.py
+-rw-r--r--   0        0        0      288 2023-04-09 09:43:57.313417 torch_geometric-2.5.3/torch_geometric/graphgym/models/pooling.py
+-rw-r--r--   0        0        0     1383 2023-11-23 19:01:39.085023 torch_geometric-2.5.3/torch_geometric/graphgym/models/transform.py
+-rw-r--r--   0        0        0     2544 2023-04-09 09:43:57.313526 torch_geometric-2.5.3/torch_geometric/graphgym/optim.py
+-rw-r--r--   0        0        0     3954 2023-11-23 19:01:39.085131 torch_geometric-2.5.3/torch_geometric/graphgym/register.py
+-rw-r--r--   0        0        0     2653 2023-09-21 09:55:53.977362 torch_geometric-2.5.3/torch_geometric/graphgym/train.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:43:57.313667 torch_geometric-2.5.3/torch_geometric/graphgym/utils/LICENSE
+-rw-r--r--   0        0        0      641 2023-04-09 09:43:57.313725 torch_geometric-2.5.3/torch_geometric/graphgym/utils/__init__.py
+-rw-r--r--   0        0        0     9349 2023-11-30 06:56:02.066772 torch_geometric-2.5.3/torch_geometric/graphgym/utils/agg_runs.py
+-rw-r--r--   0        0        0     3045 2023-11-23 19:01:39.085413 torch_geometric-2.5.3/torch_geometric/graphgym/utils/comp_budget.py
+-rw-r--r--   0        0        0     1342 2023-11-23 19:01:39.085516 torch_geometric-2.5.3/torch_geometric/graphgym/utils/device.py
+-rw-r--r--   0        0        0      690 2023-04-09 09:43:57.313975 torch_geometric-2.5.3/torch_geometric/graphgym/utils/epoch.py
+-rw-r--r--   0        0        0     2049 2023-11-30 06:56:02.067070 torch_geometric-2.5.3/torch_geometric/graphgym/utils/io.py
+-rw-r--r--   0        0        0      624 2023-11-23 19:01:39.085735 torch_geometric-2.5.3/torch_geometric/graphgym/utils/plot.py
+-rw-r--r--   0        0        0      199 2023-11-23 19:01:39.085842 torch_geometric-2.5.3/torch_geometric/graphgym/utils/tools.py
+-rw-r--r--   0        0        0      790 2024-01-16 19:07:07.467913 torch_geometric-2.5.3/torch_geometric/home.py
+-rw-r--r--   0        0        0    19217 2024-04-19 11:45:50.634492 torch_geometric-2.5.3/torch_geometric/inspector.py
+-rw-r--r--   0        0        0      528 2023-03-19 07:56:22.191105 torch_geometric-2.5.3/torch_geometric/io/__init__.py
+-rw-r--r--   0        0        0     6567 2024-02-28 12:41:28.382709 torch_geometric-2.5.3/torch_geometric/io/fs.py
+-rw-r--r--   0        0        0     1177 2023-08-04 14:13:46.021779 torch_geometric-2.5.3/torch_geometric/io/npz.py
+-rw-r--r--   0        0        0     1088 2023-12-21 07:51:56.911732 torch_geometric-2.5.3/torch_geometric/io/obj.py
+-rw-r--r--   0        0        0     2762 2023-12-21 07:51:56.911821 torch_geometric-2.5.3/torch_geometric/io/off.py
+-rw-r--r--   0        0        0     4667 2024-01-07 13:37:00.550342 torch_geometric-2.5.3/torch_geometric/io/planetoid.py
+-rw-r--r--   0        0        0      489 2023-12-21 07:51:56.912040 torch_geometric-2.5.3/torch_geometric/io/ply.py
+-rw-r--r--   0        0        0     1170 2023-12-21 07:51:56.912128 torch_geometric-2.5.3/torch_geometric/io/sdf.py
+-rw-r--r--   0        0        0     4918 2023-12-21 07:51:56.912246 torch_geometric-2.5.3/torch_geometric/io/tu.py
+-rw-r--r--   0        0        0      910 2023-12-21 07:51:56.912343 torch_geometric-2.5.3/torch_geometric/io/txt_array.py
+-rw-r--r--   0        0        0      935 2023-11-30 06:56:02.067286 torch_geometric-2.5.3/torch_geometric/isinstance.py
+-rw-r--r--   0        0        0      908 2023-12-21 07:51:56.912433 torch_geometric-2.5.3/torch_geometric/lazy_loader.py
+-rw-r--r--   0        0        0     1835 2023-11-23 19:01:39.086566 torch_geometric-2.5.3/torch_geometric/loader/__init__.py
+-rw-r--r--   0        0        0     1615 2023-12-21 07:51:56.912528 torch_geometric-2.5.3/torch_geometric/loader/base.py
+-rw-r--r--   0        0        0     2106 2023-09-21 09:55:53.978071 torch_geometric-2.5.3/torch_geometric/loader/cache.py
+-rw-r--r--   0        0        0    13196 2024-02-15 14:55:33.357892 torch_geometric-2.5.3/torch_geometric/loader/cluster.py
+-rw-r--r--   0        0        0     1459 2023-11-23 19:01:39.086733 torch_geometric-2.5.3/torch_geometric/loader/data_list_loader.py
+-rw-r--r--   0        0        0     3527 2023-12-21 07:51:56.912619 torch_geometric-2.5.3/torch_geometric/loader/dataloader.py
+-rw-r--r--   0        0        0     1685 2023-06-27 06:01:05.570350 torch_geometric-2.5.3/torch_geometric/loader/dense_data_loader.py
+-rw-r--r--   0        0        0     4163 2023-11-23 19:01:39.086987 torch_geometric-2.5.3/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-r--r--   0        0        0     8448 2023-04-09 09:43:57.315992 torch_geometric-2.5.3/torch_geometric/loader/graph_saint.py
+-rw-r--r--   0        0        0     6012 2023-05-29 07:55:13.277083 torch_geometric-2.5.3/torch_geometric/loader/hgt_loader.py
+-rw-r--r--   0        0        0    31462 2023-11-23 19:01:39.087102 torch_geometric-2.5.3/torch_geometric/loader/ibmb_loader.py
+-rw-r--r--   0        0        0     3754 2023-04-09 09:43:57.316342 torch_geometric-2.5.3/torch_geometric/loader/imbalanced_sampler.py
+-rw-r--r--   0        0        0    16207 2024-02-15 14:55:33.358040 torch_geometric-2.5.3/torch_geometric/loader/link_loader.py
+-rw-r--r--   0        0        0    14383 2024-02-15 14:55:33.358200 torch_geometric-2.5.3/torch_geometric/loader/link_neighbor_loader.py
+-rw-r--r--   0        0        0    10931 2023-12-21 07:51:56.912890 torch_geometric-2.5.3/torch_geometric/loader/mixin.py
+-rw-r--r--   0        0        0    12452 2023-11-23 19:01:39.087825 torch_geometric-2.5.3/torch_geometric/loader/neighbor_loader.py
+-rw-r--r--   0        0        0     8513 2023-04-09 09:43:57.316687 torch_geometric-2.5.3/torch_geometric/loader/neighbor_sampler.py
+-rw-r--r--   0        0        0    11848 2024-02-15 14:55:33.358394 torch_geometric-2.5.3/torch_geometric/loader/node_loader.py
+-rw-r--r--   0        0        0     3236 2023-11-23 19:01:39.088138 torch_geometric-2.5.3/torch_geometric/loader/prefetch.py
+-rw-r--r--   0        0        0     2196 2023-04-09 09:43:57.316820 torch_geometric-2.5.3/torch_geometric/loader/random_node_loader.py
+-rw-r--r--   0        0        0     4173 2023-04-09 09:43:57.316884 torch_geometric-2.5.3/torch_geometric/loader/shadow.py
+-rw-r--r--   0        0        0     2248 2023-08-07 04:56:40.199958 torch_geometric-2.5.3/torch_geometric/loader/temporal_dataloader.py
+-rw-r--r--   0        0        0    14818 2023-12-31 08:35:31.855122 torch_geometric-2.5.3/torch_geometric/loader/utils.py
+-rw-r--r--   0        0        0     3518 2023-05-29 07:55:13.278120 torch_geometric-2.5.3/torch_geometric/loader/zip_loader.py
+-rw-r--r--   0        0        0      858 2023-12-21 07:51:56.913129 torch_geometric-2.5.3/torch_geometric/logging.py
+-rw-r--r--   0        0        0      296 2024-02-15 14:55:33.358581 torch_geometric-2.5.3/torch_geometric/metrics/__init__.py
+-rw-r--r--   0        0        0     7521 2024-03-05 12:38:29.028824 torch_geometric-2.5.3/torch_geometric/metrics/link_pred.py
+-rw-r--r--   0        0        0      847 2023-05-29 07:55:13.278204 torch_geometric-2.5.3/torch_geometric/nn/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-19 11:45:50.634844 torch_geometric-2.5.3/torch_geometric/nn/aggr/__init__.py
+-rw-r--r--   0        0        0     3003 2023-11-23 19:01:39.088759 torch_geometric-2.5.3/torch_geometric/nn/aggr/attention.py
+-rw-r--r--   0        0        0     8110 2024-04-19 11:45:50.634988 torch_geometric-2.5.3/torch_geometric/nn/aggr/base.py
+-rw-r--r--   0        0        0    11011 2023-11-23 19:01:39.089265 torch_geometric-2.5.3/torch_geometric/nn/aggr/basic.py
+-rw-r--r--   0        0        0     2650 2023-11-23 19:01:39.089413 torch_geometric-2.5.3/torch_geometric/nn/aggr/deep_sets.py
+-rw-r--r--   0        0        0     6639 2023-11-23 19:01:39.089545 torch_geometric-2.5.3/torch_geometric/nn/aggr/equilibrium.py
+-rw-r--r--   0        0        0    12276 2023-11-23 19:01:39.089987 torch_geometric-2.5.3/torch_geometric/nn/aggr/fused.py
+-rw-r--r--   0        0        0     3801 2023-06-27 13:28:15.074839 torch_geometric-2.5.3/torch_geometric/nn/aggr/gmt.py
+-rw-r--r--   0        0        0     2193 2024-04-19 11:45:50.635249 torch_geometric-2.5.3/torch_geometric/nn/aggr/gru.py
+-rw-r--r--   0        0        0     4190 2023-11-23 19:01:39.090090 torch_geometric-2.5.3/torch_geometric/nn/aggr/lcm.py
+-rw-r--r--   0        0        0     2214 2023-06-27 13:28:15.075215 torch_geometric-2.5.3/torch_geometric/nn/aggr/lstm.py
+-rw-r--r--   0        0        0     2514 2024-04-19 11:45:50.635391 torch_geometric-2.5.3/torch_geometric/nn/aggr/mlp.py
+-rw-r--r--   0        0        0     8170 2023-06-10 14:35:51.129653 torch_geometric-2.5.3/torch_geometric/nn/aggr/multi.py
+-rw-r--r--   0        0        0     6189 2023-11-23 19:01:39.090353 torch_geometric-2.5.3/torch_geometric/nn/aggr/quantile.py
+-rw-r--r--   0        0        0     4638 2023-07-21 07:41:11.167904 torch_geometric-2.5.3/torch_geometric/nn/aggr/scaler.py
+-rw-r--r--   0        0        0     2446 2023-11-23 19:01:39.090464 torch_geometric-2.5.3/torch_geometric/nn/aggr/set2set.py
+-rw-r--r--   0        0        0     4207 2023-08-24 05:09:46.603743 torch_geometric-2.5.3/torch_geometric/nn/aggr/set_transformer.py
+-rw-r--r--   0        0        0     2507 2023-06-27 13:28:15.076321 torch_geometric-2.5.3/torch_geometric/nn/aggr/sort.py
+-rw-r--r--   0        0        0     8338 2023-11-23 19:01:39.090753 torch_geometric-2.5.3/torch_geometric/nn/aggr/utils.py
+-rw-r--r--   0        0        0       76 2023-06-15 08:50:09.288170 torch_geometric-2.5.3/torch_geometric/nn/attention/__init__.py
+-rw-r--r--   0        0        0     7357 2023-11-23 19:01:39.090903 torch_geometric-2.5.3/torch_geometric/nn/attention/performer.py
+-rw-r--r--   0        0        0     3515 2024-02-11 12:50:44.321572 torch_geometric-2.5.3/torch_geometric/nn/conv/__init__.py
+-rw-r--r--   0        0        0     3077 2024-01-07 13:37:00.550514 torch_geometric-2.5.3/torch_geometric/nn/conv/agnn_conv.py
+-rw-r--r--   0        0        0     4387 2023-11-23 19:01:39.091295 torch_geometric-2.5.3/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-r--r--   0        0        0     5983 2024-01-16 19:07:07.468736 torch_geometric-2.5.3/torch_geometric/nn/conv/appnp.py
+-rw-r--r--   0        0        0     6585 2024-01-16 19:07:07.468883 torch_geometric-2.5.3/torch_geometric/nn/conv/arma_conv.py
+-rw-r--r--   0        0        0     4014 2024-01-07 13:37:00.551165 torch_geometric-2.5.3/torch_geometric/nn/conv/cg_conv.py
+-rw-r--r--   0        0        0     6423 2024-01-07 13:37:00.551338 torch_geometric-2.5.3/torch_geometric/nn/conv/cheb_conv.py
+-rw-r--r--   0        0        0     5255 2024-01-16 19:07:07.469025 torch_geometric-2.5.3/torch_geometric/nn/conv/cluster_gcn_conv.py
+-rw-r--r--   0        0        0     5300 2024-04-19 11:45:50.635802 torch_geometric-2.5.3/torch_geometric/nn/conv/collect.jinja
+-rw-r--r--   0        0        0      251 2023-04-09 09:43:57.321325 torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-r--r--   0        0        0     8212 2024-04-19 11:45:50.636249 torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/base.py
+-rw-r--r--   0        0        0     2846 2024-04-19 11:45:50.636599 torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-r--r--   0        0        0     4212 2024-04-19 11:45:50.636721 torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-r--r--   0        0        0     2802 2024-04-19 11:45:50.636833 torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-r--r--   0        0        0     2440 2023-11-23 19:01:39.092177 torch_geometric-2.5.3/torch_geometric/nn/conv/dir_gnn_conv.py
+-rw-r--r--   0        0        0    12241 2024-01-07 13:37:00.551656 torch_geometric-2.5.3/torch_geometric/nn/conv/dna_conv.py
+-rw-r--r--   0        0        0     5389 2024-01-07 13:37:00.551824 torch_geometric-2.5.3/torch_geometric/nn/conv/edge_conv.py
+-rw-r--r--   0        0        0     2216 2024-02-28 12:41:28.383671 torch_geometric-2.5.3/torch_geometric/nn/conv/edge_updater.jinja
+-rw-r--r--   0        0        0    10742 2024-01-16 19:07:07.469443 torch_geometric-2.5.3/torch_geometric/nn/conv/eg_conv.py
+-rw-r--r--   0        0        0     9065 2024-01-16 19:07:07.469669 torch_geometric-2.5.3/torch_geometric/nn/conv/fa_conv.py
+-rw-r--r--   0        0        0     4430 2024-01-07 13:37:00.552728 torch_geometric-2.5.3/torch_geometric/nn/conv/feast_conv.py
+-rw-r--r--   0        0        0     6314 2024-01-07 13:37:00.552962 torch_geometric-2.5.3/torch_geometric/nn/conv/film_conv.py
+-rw-r--r--   0        0        0     4502 2023-12-29 09:32:12.742136 torch_geometric-2.5.3/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-r--r--   0        0        0    16091 2024-01-16 19:07:07.469955 torch_geometric-2.5.3/torch_geometric/nn/conv/gat_conv.py
+-rw-r--r--   0        0        0     3518 2024-01-16 19:07:07.470092 torch_geometric-2.5.3/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-r--r--   0        0        0    13639 2024-01-16 19:07:07.470276 torch_geometric-2.5.3/torch_geometric/nn/conv/gatv2_conv.py
+-rw-r--r--   0        0        0     7001 2024-01-16 19:07:07.470403 torch_geometric-2.5.3/torch_geometric/nn/conv/gcn2_conv.py
+-rw-r--r--   0        0        0    10415 2024-01-16 19:07:07.470579 torch_geometric-2.5.3/torch_geometric/nn/conv/gcn_conv.py
+-rw-r--r--   0        0        0     9722 2024-02-15 14:55:33.359459 torch_geometric-2.5.3/torch_geometric/nn/conv/gen_conv.py
+-rw-r--r--   0        0        0     7591 2024-01-16 19:07:07.470714 torch_geometric-2.5.3/torch_geometric/nn/conv/general_conv.py
+-rw-r--r--   0        0        0     7411 2024-01-16 19:07:07.470852 torch_geometric-2.5.3/torch_geometric/nn/conv/gin_conv.py
+-rw-r--r--   0        0        0     8315 2024-01-16 19:07:07.471060 torch_geometric-2.5.3/torch_geometric/nn/conv/gmm_conv.py
+-rw-r--r--   0        0        0     6672 2023-06-15 08:50:09.288360 torch_geometric-2.5.3/torch_geometric/nn/conv/gps_conv.py
+-rw-r--r--   0        0        0     3455 2024-04-19 11:45:50.637134 torch_geometric-2.5.3/torch_geometric/nn/conv/graph_conv.py
+-rw-r--r--   0        0        0     4951 2024-01-16 19:07:07.471345 torch_geometric-2.5.3/torch_geometric/nn/conv/gravnet_conv.py
+-rw-r--r--   0        0        0     7198 2024-02-15 14:55:33.359644 torch_geometric-2.5.3/torch_geometric/nn/conv/han_conv.py
+-rw-r--r--   0        0        0     6084 2024-01-16 19:07:07.471657 torch_geometric-2.5.3/torch_geometric/nn/conv/heat_conv.py
+-rw-r--r--   0        0        0     6555 2023-11-23 19:01:39.095192 torch_geometric-2.5.3/torch_geometric/nn/conv/hetero_conv.py
+-rw-r--r--   0        0        0     9043 2024-02-15 14:55:33.359787 torch_geometric-2.5.3/torch_geometric/nn/conv/hgt_conv.py
+-rw-r--r--   0        0        0     8691 2024-02-15 14:55:33.359940 torch_geometric-2.5.3/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-r--r--   0        0        0     3494 2024-01-07 13:37:00.555150 torch_geometric-2.5.3/torch_geometric/nn/conv/le_conv.py
+-rw-r--r--   0        0        0     2369 2024-01-16 19:07:07.471811 torch_geometric-2.5.3/torch_geometric/nn/conv/lg_conv.py
+-rw-r--r--   0        0        0    42600 2024-04-19 11:45:50.637387 torch_geometric-2.5.3/torch_geometric/nn/conv/message_passing.py
+-rw-r--r--   0        0        0     4340 2024-01-16 19:07:07.472405 torch_geometric-2.5.3/torch_geometric/nn/conv/mf_conv.py
+-rw-r--r--   0        0        0     4554 2024-01-16 19:07:07.472547 torch_geometric-2.5.3/torch_geometric/nn/conv/mixhop_conv.py
+-rw-r--r--   0        0        0     4759 2024-01-07 13:37:00.555995 torch_geometric-2.5.3/torch_geometric/nn/conv/nn_conv.py
+-rw-r--r--   0        0        0     4908 2024-01-16 19:07:07.472693 torch_geometric-2.5.3/torch_geometric/nn/conv/pan_conv.py
+-rw-r--r--   0        0        0     4892 2024-02-15 14:55:33.360118 torch_geometric-2.5.3/torch_geometric/nn/conv/pdn_conv.py
+-rw-r--r--   0        0        0     8325 2024-01-07 13:37:00.556429 torch_geometric-2.5.3/torch_geometric/nn/conv/pna_conv.py
+-rw-r--r--   0        0        0     4508 2024-01-07 13:37:00.556571 torch_geometric-2.5.3/torch_geometric/nn/conv/point_conv.py
+-rw-r--r--   0        0        0     3278 2024-01-07 13:37:00.556824 torch_geometric-2.5.3/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-r--r--   0        0        0     5878 2024-01-07 13:37:00.557040 torch_geometric-2.5.3/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-r--r--   0        0        0     5363 2024-01-16 19:07:07.473113 torch_geometric-2.5.3/torch_geometric/nn/conv/ppf_conv.py
+-rw-r--r--   0        0        0     7080 2024-04-19 11:45:50.637910 torch_geometric-2.5.3/torch_geometric/nn/conv/propagate.jinja
+-rw-r--r--   0        0        0     5217 2024-01-16 19:07:07.473478 torch_geometric-2.5.3/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-r--r--   0        0        0    22863 2024-01-16 19:07:07.473800 torch_geometric-2.5.3/torch_geometric/nn/conv/rgat_conv.py
+-rw-r--r--   0        0        0    15705 2024-01-16 19:07:07.473996 torch_geometric-2.5.3/torch_geometric/nn/conv/rgcn_conv.py
+-rw-r--r--   0        0        0     5812 2024-01-16 19:07:07.474135 torch_geometric-2.5.3/torch_geometric/nn/conv/sage_conv.py
+-rw-r--r--   0        0        0     4543 2024-01-16 19:07:07.474274 torch_geometric-2.5.3/torch_geometric/nn/conv/sg_conv.py
+-rw-r--r--   0        0        0     6190 2024-01-16 19:07:07.474416 torch_geometric-2.5.3/torch_geometric/nn/conv/signed_conv.py
+-rw-r--r--   0        0        0     3888 2024-01-16 19:07:07.474543 torch_geometric-2.5.3/torch_geometric/nn/conv/simple_conv.py
+-rw-r--r--   0        0        0     6314 2024-01-07 13:37:00.558683 torch_geometric-2.5.3/torch_geometric/nn/conv/spline_conv.py
+-rw-r--r--   0        0        0     5131 2024-01-16 19:07:07.474692 torch_geometric-2.5.3/torch_geometric/nn/conv/ssg_conv.py
+-rw-r--r--   0        0        0    12420 2024-01-07 13:37:00.558982 torch_geometric-2.5.3/torch_geometric/nn/conv/supergat_conv.py
+-rw-r--r--   0        0        0     4164 2024-01-16 19:07:07.474827 torch_geometric-2.5.3/torch_geometric/nn/conv/tag_conv.py
+-rw-r--r--   0        0        0    10407 2024-01-16 19:07:07.475006 torch_geometric-2.5.3/torch_geometric/nn/conv/transformer_conv.py
+-rw-r--r--   0        0        0      852 2023-11-23 19:01:39.099644 torch_geometric-2.5.3/torch_geometric/nn/conv/utils/__init__.py
+-rw-r--r--   0        0        0     2792 2023-11-23 19:01:39.099742 torch_geometric-2.5.3/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-r--r--   0        0        0     3140 2023-11-23 19:01:39.100026 torch_geometric-2.5.3/torch_geometric/nn/conv/wl_conv.py
+-rw-r--r--   0        0        0     2777 2024-01-16 19:07:07.475144 torch_geometric-2.5.3/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-r--r--   0        0        0     5956 2023-11-23 19:01:39.100257 torch_geometric-2.5.3/torch_geometric/nn/conv/x_conv.py
+-rw-r--r--   0        0        0     4764 2023-11-23 19:01:39.100399 torch_geometric-2.5.3/torch_geometric/nn/data_parallel.py
+-rw-r--r--   0        0        0      847 2023-11-23 19:01:39.100545 torch_geometric-2.5.3/torch_geometric/nn/dense/__init__.py
+-rw-r--r--   0        0        0     4238 2023-11-23 19:01:39.100672 torch_geometric-2.5.3/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-r--r--   0        0        0     3002 2023-11-23 19:01:39.100781 torch_geometric-2.5.3/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-r--r--   0        0        0     2361 2023-11-23 19:01:39.100890 torch_geometric-2.5.3/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-r--r--   0        0        0     2751 2023-11-23 19:01:39.101001 torch_geometric-2.5.3/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-r--r--   0        0        0     2672 2023-11-23 19:01:39.101109 torch_geometric-2.5.3/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-r--r--   0        0        0     3051 2023-11-23 19:01:39.101231 torch_geometric-2.5.3/torch_geometric/nn/dense/diff_pool.py
+-rw-r--r--   0        0        0     6115 2023-12-05 06:32:32.915671 torch_geometric-2.5.3/torch_geometric/nn/dense/dmon_pool.py
+-rw-r--r--   0        0        0    17702 2024-02-15 14:55:33.360239 torch_geometric-2.5.3/torch_geometric/nn/dense/linear.py
+-rw-r--r--   0        0        0     4111 2023-11-23 19:01:39.101632 torch_geometric-2.5.3/torch_geometric/nn/dense/mincut_pool.py
+-rw-r--r--   0        0        0     3115 2024-02-15 14:55:33.360364 torch_geometric-2.5.3/torch_geometric/nn/encoding.py
+-rw-r--r--   0        0        0      129 2023-11-23 19:01:39.101834 torch_geometric-2.5.3/torch_geometric/nn/functional/__init__.py
+-rw-r--r--   0        0        0     1549 2023-04-09 09:43:57.329579 torch_geometric-2.5.3/torch_geometric/nn/functional/bro.py
+-rw-r--r--   0        0        0      863 2023-04-09 09:43:57.329650 torch_geometric-2.5.3/torch_geometric/nn/functional/gini.py
+-rw-r--r--   0        0        0    16055 2023-11-23 19:01:39.102054 torch_geometric-2.5.3/torch_geometric/nn/fx.py
+-rw-r--r--   0        0        0     1088 2023-04-09 09:43:57.329812 torch_geometric-2.5.3/torch_geometric/nn/glob.py
+-rw-r--r--   0        0        0     2457 2023-04-09 09:43:57.329913 torch_geometric-2.5.3/torch_geometric/nn/inits.py
+-rw-r--r--   0        0        0      290 2023-11-23 19:01:39.102166 torch_geometric-2.5.3/torch_geometric/nn/kge/__init__.py
+-rw-r--r--   0        0        0     5902 2023-11-23 19:01:39.102288 torch_geometric-2.5.3/torch_geometric/nn/kge/base.py
+-rw-r--r--   0        0        0     3234 2023-04-09 09:43:57.330136 torch_geometric-2.5.3/torch_geometric/nn/kge/complex.py
+-rw-r--r--   0        0        0     2462 2023-04-09 09:43:57.330226 torch_geometric-2.5.3/torch_geometric/nn/kge/distmult.py
+-rw-r--r--   0        0        0      771 2023-04-09 09:43:57.330284 torch_geometric-2.5.3/torch_geometric/nn/kge/loader.py
+-rw-r--r--   0        0        0     3208 2023-04-09 09:43:57.330367 torch_geometric-2.5.3/torch_geometric/nn/kge/rotate.py
+-rw-r--r--   0        0        0     3088 2023-04-09 09:43:57.330433 torch_geometric-2.5.3/torch_geometric/nn/kge/transe.py
+-rw-r--r--   0        0        0     8937 2023-04-09 09:43:57.330505 torch_geometric-2.5.3/torch_geometric/nn/lr_scheduler.py
+-rw-r--r--   0        0        0     9512 2023-11-30 06:56:02.068638 torch_geometric-2.5.3/torch_geometric/nn/model_hub.py
+-rw-r--r--   0        0        0     1909 2023-12-21 07:51:56.913362 torch_geometric-2.5.3/torch_geometric/nn/models/__init__.py
+-rw-r--r--   0        0        0     6634 2024-01-16 19:07:07.475306 torch_geometric-2.5.3/torch_geometric/nn/models/attentive_fp.py
+-rw-r--r--   0        0        0    10770 2023-11-23 19:01:39.102686 torch_geometric-2.5.3/torch_geometric/nn/models/autoencoder.py
+-rw-r--r--   0        0        0    31225 2024-01-16 19:07:07.475459 torch_geometric-2.5.3/torch_geometric/nn/models/basic_gnn.py
+-rw-r--r--   0        0        0     3971 2023-11-23 19:01:39.103036 torch_geometric-2.5.3/torch_geometric/nn/models/captum.py
+-rw-r--r--   0        0        0     6827 2023-11-23 19:01:39.103200 torch_geometric-2.5.3/torch_geometric/nn/models/correct_and_smooth.py
+-rw-r--r--   0        0        0     4197 2023-11-23 19:01:39.103325 torch_geometric-2.5.3/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-r--r--   0        0        0     4339 2023-11-23 19:01:39.103464 torch_geometric-2.5.3/torch_geometric/nn/models/deepgcn.py
+-rw-r--r--   0        0        0    36172 2024-04-19 11:45:50.638327 torch_geometric-2.5.3/torch_geometric/nn/models/dimenet.py
+-rw-r--r--   0        0        0     5107 2023-11-23 19:01:39.103871 torch_geometric-2.5.3/torch_geometric/nn/models/dimenet_utils.py
+-rw-r--r--   0        0        0     7873 2023-11-23 19:01:39.104032 torch_geometric-2.5.3/torch_geometric/nn/models/gnnff.py
+-rw-r--r--   0        0        0     9246 2023-11-23 19:01:39.104224 torch_geometric-2.5.3/torch_geometric/nn/models/graph_mixer.py
+-rw-r--r--   0        0        0     5395 2023-11-23 19:01:39.104370 torch_geometric-2.5.3/torch_geometric/nn/models/graph_unet.py
+-rw-r--r--   0        0        0     3450 2023-11-23 19:01:39.104562 torch_geometric-2.5.3/torch_geometric/nn/models/jumping_knowledge.py
+-rw-r--r--   0        0        0     3908 2024-01-16 19:07:07.475623 torch_geometric-2.5.3/torch_geometric/nn/models/label_prop.py
+-rw-r--r--   0        0        0    12465 2023-11-23 19:01:39.104875 torch_geometric-2.5.3/torch_geometric/nn/models/lightgcn.py
+-rw-r--r--   0        0        0     5812 2024-01-16 19:07:07.475775 torch_geometric-2.5.3/torch_geometric/nn/models/linkx.py
+-rw-r--r--   0        0        0     2580 2023-11-23 19:01:39.105180 torch_geometric-2.5.3/torch_geometric/nn/models/mask_label.py
+-rw-r--r--   0        0        0     6540 2023-11-23 19:01:39.105344 torch_geometric-2.5.3/torch_geometric/nn/models/meta.py
+-rw-r--r--   0        0        0    10798 2024-04-19 11:45:50.638715 torch_geometric-2.5.3/torch_geometric/nn/models/metapath2vec.py
+-rw-r--r--   0        0        0    10315 2023-11-23 19:01:39.105734 torch_geometric-2.5.3/torch_geometric/nn/models/mlp.py
+-rw-r--r--   0        0        0     2378 2023-11-23 19:01:39.105813 torch_geometric-2.5.3/torch_geometric/nn/models/neural_fingerprint.py
+-rw-r--r--   0        0        0     7731 2023-11-23 19:01:39.105980 torch_geometric-2.5.3/torch_geometric/nn/models/node2vec.py
+-rw-r--r--   0        0        0     3538 2023-11-23 19:01:39.106116 torch_geometric-2.5.3/torch_geometric/nn/models/pmlp.py
+-rw-r--r--   0        0        0     8986 2023-11-23 19:01:39.106289 torch_geometric-2.5.3/torch_geometric/nn/models/re_net.py
+-rw-r--r--   0        0        0     2808 2024-01-16 19:07:07.475934 torch_geometric-2.5.3/torch_geometric/nn/models/rect.py
+-rw-r--r--   0        0        0    11796 2024-03-05 12:38:29.030106 torch_geometric-2.5.3/torch_geometric/nn/models/rev_gnn.py
+-rw-r--r--   0        0        0    16619 2023-12-05 07:08:51.296448 torch_geometric-2.5.3/torch_geometric/nn/models/schnet.py
+-rw-r--r--   0        0        0     9839 2023-11-23 19:01:39.106956 torch_geometric-2.5.3/torch_geometric/nn/models/signed_gcn.py
+-rw-r--r--   0        0        0    11814 2024-04-19 11:45:50.639063 torch_geometric-2.5.3/torch_geometric/nn/models/tgn.py
+-rw-r--r--   0        0        0    43192 2024-02-15 14:55:33.360667 torch_geometric-2.5.3/torch_geometric/nn/models/visnet.py
+-rw-r--r--   0        0        0     2373 2023-11-23 19:01:39.109159 torch_geometric-2.5.3/torch_geometric/nn/module_dict.py
+-rw-r--r--   0        0        0      669 2023-11-23 19:01:39.109307 torch_geometric-2.5.3/torch_geometric/nn/norm/__init__.py
+-rw-r--r--   0        0        0     8283 2023-11-23 19:01:39.109506 torch_geometric-2.5.3/torch_geometric/nn/norm/batch_norm.py
+-rw-r--r--   0        0        0     4722 2023-11-23 19:01:39.109638 torch_geometric-2.5.3/torch_geometric/nn/norm/diff_group_norm.py
+-rw-r--r--   0        0        0     2727 2023-11-23 19:01:39.109771 torch_geometric-2.5.3/torch_geometric/nn/norm/graph_norm.py
+-rw-r--r--   0        0        0     1491 2023-11-23 19:01:39.109886 torch_geometric-2.5.3/torch_geometric/nn/norm/graph_size_norm.py
+-rw-r--r--   0        0        0     4685 2023-11-23 19:01:39.110017 torch_geometric-2.5.3/torch_geometric/nn/norm/instance_norm.py
+-rw-r--r--   0        0        0     7831 2023-11-23 19:01:39.110157 torch_geometric-2.5.3/torch_geometric/nn/norm/layer_norm.py
+-rw-r--r--   0        0        0     1322 2024-02-15 14:55:33.360823 torch_geometric-2.5.3/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-r--r--   0        0        0     1662 2023-11-23 19:01:39.110373 torch_geometric-2.5.3/torch_geometric/nn/norm/msg_norm.py
+-rw-r--r--   0        0        0     2824 2023-11-23 19:01:39.110475 torch_geometric-2.5.3/torch_geometric/nn/norm/pair_norm.py
+-rw-r--r--   0        0        0     2410 2023-11-23 19:01:39.110589 torch_geometric-2.5.3/torch_geometric/nn/parameter_dict.py
+-rw-r--r--   0        0        0    13497 2024-04-19 11:45:50.639761 torch_geometric-2.5.3/torch_geometric/nn/pool/__init__.py
+-rw-r--r--   0        0        0     3967 2023-05-29 07:55:13.280050 torch_geometric-2.5.3/torch_geometric/nn/pool/approx_knn.py
+-rw-r--r--   0        0        0     6683 2024-01-16 19:07:07.476171 torch_geometric-2.5.3/torch_geometric/nn/pool/asap.py
+-rw-r--r--   0        0        0     3966 2023-05-17 17:44:44.818765 torch_geometric-2.5.3/torch_geometric/nn/pool/avg_pool.py
+-rw-r--r--   0        0        0      287 2023-11-23 19:01:39.111020 torch_geometric-2.5.3/torch_geometric/nn/pool/connect/__init__.py
+-rw-r--r--   0        0        0     4094 2023-11-23 19:01:39.111130 torch_geometric-2.5.3/torch_geometric/nn/pool/connect/base.py
+-rw-r--r--   0        0        0     2190 2023-11-23 19:01:39.111323 torch_geometric-2.5.3/torch_geometric/nn/pool/connect/filter_edges.py
+-rw-r--r--   0        0        0      273 2023-03-19 07:56:22.204784 torch_geometric-2.5.3/torch_geometric/nn/pool/consecutive.py
+-rw-r--r--   0        0        0     1601 2023-10-08 19:44:11.501231 torch_geometric-2.5.3/torch_geometric/nn/pool/decimation.py
+-rw-r--r--   0        0        0     8581 2023-11-23 19:01:39.111494 torch_geometric-2.5.3/torch_geometric/nn/pool/edge_pool.py
+-rw-r--r--   0        0        0     3492 2023-11-23 19:01:39.111597 torch_geometric-2.5.3/torch_geometric/nn/pool/glob.py
+-rw-r--r--   0        0        0     1291 2023-11-23 19:01:39.111702 torch_geometric-2.5.3/torch_geometric/nn/pool/graclus.py
+-rw-r--r--   0        0        0     7506 2024-04-19 11:45:50.640222 torch_geometric-2.5.3/torch_geometric/nn/pool/knn.py
+-rw-r--r--   0        0        0     4262 2023-05-17 17:44:44.819217 torch_geometric-2.5.3/torch_geometric/nn/pool/max_pool.py
+-rw-r--r--   0        0        0     5377 2023-11-23 19:01:39.111840 torch_geometric-2.5.3/torch_geometric/nn/pool/mem_pool.py
+-rw-r--r--   0        0        0     4366 2023-11-23 19:01:39.111961 torch_geometric-2.5.3/torch_geometric/nn/pool/pan_pool.py
+-rw-r--r--   0        0        0      631 2024-04-19 11:45:50.640562 torch_geometric-2.5.3/torch_geometric/nn/pool/pool.py
+-rw-r--r--   0        0        0     5838 2023-11-23 19:01:39.112087 torch_geometric-2.5.3/torch_geometric/nn/pool/sag_pool.py
+-rw-r--r--   0        0        0      254 2023-11-23 19:01:39.112224 torch_geometric-2.5.3/torch_geometric/nn/pool/select/__init__.py
+-rw-r--r--   0        0        0     3311 2023-07-21 07:41:11.173771 torch_geometric-2.5.3/torch_geometric/nn/pool/select/base.py
+-rw-r--r--   0        0        0     5305 2023-11-23 19:01:39.112366 torch_geometric-2.5.3/torch_geometric/nn/pool/select/topk.py
+-rw-r--r--   0        0        0     5159 2023-11-23 19:01:39.112544 torch_geometric-2.5.3/torch_geometric/nn/pool/topk_pool.py
+-rw-r--r--   0        0        0     2736 2023-11-23 19:01:39.112832 torch_geometric-2.5.3/torch_geometric/nn/pool/voxel_grid.py
+-rw-r--r--   0        0        0      426 2023-11-23 19:01:39.112997 torch_geometric-2.5.3/torch_geometric/nn/reshape.py
+-rw-r--r--   0        0        0     6155 2023-05-17 17:44:44.820088 torch_geometric-2.5.3/torch_geometric/nn/resolver.py
+-rw-r--r--   0        0        0     1054 2024-02-15 14:55:33.361163 torch_geometric-2.5.3/torch_geometric/nn/sequential.jinja
+-rw-r--r--   0        0        0     5534 2024-04-19 11:45:50.641153 torch_geometric-2.5.3/torch_geometric/nn/sequential.py
+-rw-r--r--   0        0        0     5821 2023-08-24 05:09:46.605208 torch_geometric-2.5.3/torch_geometric/nn/summary.py
+-rw-r--r--   0        0        0     1282 2023-04-09 09:43:57.336993 torch_geometric-2.5.3/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-r--r--   0        0        0     6519 2024-01-07 13:37:00.562075 torch_geometric-2.5.3/torch_geometric/nn/to_hetero_module.py
+-rw-r--r--   0        0        0    18407 2023-11-23 19:01:39.113471 torch_geometric-2.5.3/torch_geometric/nn/to_hetero_transformer.py
+-rw-r--r--   0        0        0    23121 2023-11-23 19:01:39.113662 torch_geometric-2.5.3/torch_geometric/nn/to_hetero_with_bases_transformer.py
+-rw-r--r--   0        0        0      129 2023-11-23 19:01:39.113907 torch_geometric-2.5.3/torch_geometric/nn/unpool/__init__.py
+-rw-r--r--   0        0        0     2586 2023-11-23 19:01:39.114022 torch_geometric-2.5.3/torch_geometric/nn/unpool/knn_interpolate.py
+-rw-r--r--   0        0        0      863 2023-12-21 07:51:56.913994 torch_geometric-2.5.3/torch_geometric/profile/__init__.py
+-rw-r--r--   0        0        0     5256 2023-11-23 19:01:39.114260 torch_geometric-2.5.3/torch_geometric/profile/benchmark.py
+-rw-r--r--   0        0        0    11793 2023-12-21 07:51:56.914151 torch_geometric-2.5.3/torch_geometric/profile/profile.py
+-rw-r--r--   0        0        0    16640 2023-11-23 19:01:39.114432 torch_geometric-2.5.3/torch_geometric/profile/profiler.py
+-rw-r--r--   0        0        0     5497 2023-12-21 07:51:56.914275 torch_geometric-2.5.3/torch_geometric/profile/utils.py
+-rw-r--r--   0        0        0     1273 2023-12-21 07:51:56.914372 torch_geometric-2.5.3/torch_geometric/resolver.py
+-rw-r--r--   0        0        0      512 2023-11-23 19:01:39.114690 torch_geometric-2.5.3/torch_geometric/sampler/__init__.py
+-rw-r--r--   0        0        0    25968 2024-02-15 14:55:33.361475 torch_geometric-2.5.3/torch_geometric/sampler/base.py
+-rw-r--r--   0        0        0     2721 2023-11-23 19:01:39.114973 torch_geometric-2.5.3/torch_geometric/sampler/hgt_sampler.py
+-rw-r--r--   0        0        0    33850 2024-02-11 12:50:44.324845 torch_geometric-2.5.3/torch_geometric/sampler/neighbor_sampler.py
+-rw-r--r--   0        0        0     5492 2023-12-31 08:35:31.856681 torch_geometric-2.5.3/torch_geometric/sampler/utils.py
+-rw-r--r--   0        0        0      372 2023-12-21 07:51:56.914460 torch_geometric-2.5.3/torch_geometric/seed.py
+-rw-r--r--   0        0        0     1060 2024-04-08 11:55:46.871626 torch_geometric-2.5.3/torch_geometric/template.py
+-rw-r--r--   0        0        0     1161 2024-04-19 11:45:50.641478 torch_geometric-2.5.3/torch_geometric/testing/__init__.py
+-rw-r--r--   0        0        0     4606 2023-12-21 07:51:56.914584 torch_geometric-2.5.3/torch_geometric/testing/asserts.py
+-rw-r--r--   0        0        0     2604 2023-12-21 07:51:56.914840 torch_geometric-2.5.3/torch_geometric/testing/data.py
+-rw-r--r--   0        0        0     6736 2024-04-19 11:45:50.641835 torch_geometric-2.5.3/torch_geometric/testing/decorators.py
+-rw-r--r--   0        0        0     2181 2024-04-19 11:45:50.642157 torch_geometric-2.5.3/torch_geometric/testing/feature_store.py
+-rw-r--r--   0        0        0     1044 2023-12-21 07:51:56.915619 torch_geometric-2.5.3/torch_geometric/testing/graph_store.py
+-rw-r--r--   0        0        0     4181 2023-08-24 05:09:46.605333 torch_geometric-2.5.3/torch_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0    14223 2023-12-31 08:35:31.857021 torch_geometric-2.5.3/torch_geometric/transforms/add_metapaths.py
+-rw-r--r--   0        0        0     6051 2024-04-19 11:45:50.642511 torch_geometric-2.5.3/torch_geometric/transforms/add_positional_encoding.py
+-rw-r--r--   0        0        0     2085 2023-12-21 07:51:56.916523 torch_geometric-2.5.3/torch_geometric/transforms/add_remaining_self_loops.py
+-rw-r--r--   0        0        0     2024 2023-12-21 07:51:56.916642 torch_geometric-2.5.3/torch_geometric/transforms/add_self_loops.py
+-rw-r--r--   0        0        0     1298 2023-05-29 07:55:13.281284 torch_geometric-2.5.3/torch_geometric/transforms/base_transform.py
+-rw-r--r--   0        0        0     2464 2023-12-21 07:51:56.917071 torch_geometric-2.5.3/torch_geometric/transforms/cartesian.py
+-rw-r--r--   0        0        0      645 2023-11-23 19:01:39.116658 torch_geometric-2.5.3/torch_geometric/transforms/center.py
+-rw-r--r--   0        0        0     1658 2023-05-29 07:55:13.281683 torch_geometric-2.5.3/torch_geometric/transforms/compose.py
+-rw-r--r--   0        0        0     2005 2023-12-21 07:51:56.917174 torch_geometric-2.5.3/torch_geometric/transforms/constant.py
+-rw-r--r--   0        0        0     1264 2023-12-21 07:51:56.917270 torch_geometric-2.5.3/torch_geometric/transforms/delaunay.py
+-rw-r--r--   0        0        0     2360 2023-12-21 07:51:56.917398 torch_geometric-2.5.3/torch_geometric/transforms/distance.py
+-rw-r--r--   0        0        0     1083 2023-12-21 07:51:56.917497 torch_geometric-2.5.3/torch_geometric/transforms/face_to_edge.py
+-rw-r--r--   0        0        0     3056 2023-12-21 07:51:56.917600 torch_geometric-2.5.3/torch_geometric/transforms/feature_propagation.py
+-rw-r--r--   0        0        0     2426 2023-12-21 07:51:56.917699 torch_geometric-2.5.3/torch_geometric/transforms/fixed_points.py
+-rw-r--r--   0        0        0     1397 2023-05-29 07:55:13.282572 torch_geometric-2.5.3/torch_geometric/transforms/gcn_norm.py
+-rw-r--r--   0        0        0    20201 2023-12-21 07:51:56.918013 torch_geometric-2.5.3/torch_geometric/transforms/gdc.py
+-rw-r--r--   0        0        0     1021 2024-04-19 11:45:50.642851 torch_geometric-2.5.3/torch_geometric/transforms/generate_mesh_normals.py
+-rw-r--r--   0        0        0     2564 2023-12-21 07:51:56.918223 torch_geometric-2.5.3/torch_geometric/transforms/grid_sampling.py
+-rw-r--r--   0        0        0     4102 2023-12-21 07:51:56.918364 torch_geometric-2.5.3/torch_geometric/transforms/half_hop.py
+-rw-r--r--   0        0        0     2536 2023-12-21 07:51:56.918475 torch_geometric-2.5.3/torch_geometric/transforms/knn_graph.py
+-rw-r--r--   0        0        0     2497 2024-04-19 11:45:50.643317 torch_geometric-2.5.3/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-r--r--   0        0        0     2161 2024-02-15 14:55:33.362033 torch_geometric-2.5.3/torch_geometric/transforms/largest_connected_components.py
+-rw-r--r--   0        0        0     3730 2023-12-21 07:51:56.918778 torch_geometric-2.5.3/torch_geometric/transforms/line_graph.py
+-rw-r--r--   0        0        0     1997 2023-11-23 19:01:39.117385 torch_geometric-2.5.3/torch_geometric/transforms/linear_transformation.py
+-rw-r--r--   0        0        0     2144 2023-12-21 07:51:56.918876 torch_geometric-2.5.3/torch_geometric/transforms/local_cartesian.py
+-rw-r--r--   0        0        0     1480 2023-12-21 07:51:56.918976 torch_geometric-2.5.3/torch_geometric/transforms/local_degree_profile.py
+-rw-r--r--   0        0        0     4813 2023-12-21 07:51:56.919110 torch_geometric-2.5.3/torch_geometric/transforms/mask.py
+-rw-r--r--   0        0        0     6088 2023-11-23 19:01:39.117647 torch_geometric-2.5.3/torch_geometric/transforms/node_property_split.py
+-rw-r--r--   0        0        0     1028 2023-05-29 07:55:13.284273 torch_geometric-2.5.3/torch_geometric/transforms/normalize_features.py
+-rw-r--r--   0        0        0     1782 2023-12-21 07:51:56.919212 torch_geometric-2.5.3/torch_geometric/transforms/normalize_rotation.py
+-rw-r--r--   0        0        0      666 2023-12-21 07:51:56.919305 torch_geometric-2.5.3/torch_geometric/transforms/normalize_scale.py
+-rw-r--r--   0        0        0     1584 2023-12-21 07:51:56.919388 torch_geometric-2.5.3/torch_geometric/transforms/one_hot_degree.py
+-rw-r--r--   0        0        0    21047 2023-12-21 07:51:56.919508 torch_geometric-2.5.3/torch_geometric/transforms/pad.py
+-rw-r--r--   0        0        0     1794 2023-11-23 19:01:39.117925 torch_geometric-2.5.3/torch_geometric/transforms/point_pair_features.py
+-rw-r--r--   0        0        0     2213 2023-12-21 07:51:56.919629 torch_geometric-2.5.3/torch_geometric/transforms/polar.py
+-rw-r--r--   0        0        0     2043 2023-12-21 07:51:56.919729 torch_geometric-2.5.3/torch_geometric/transforms/radius_graph.py
+-rw-r--r--   0        0        0     1033 2023-12-21 07:51:56.919836 torch_geometric-2.5.3/torch_geometric/transforms/random_flip.py
+-rw-r--r--   0        0        0     1721 2023-12-21 07:51:56.919934 torch_geometric-2.5.3/torch_geometric/transforms/random_jitter.py
+-rw-r--r--   0        0        0    15174 2023-12-21 07:51:56.920164 torch_geometric-2.5.3/torch_geometric/transforms/random_link_split.py
+-rw-r--r--   0        0        0     5853 2023-12-21 07:51:56.920287 torch_geometric-2.5.3/torch_geometric/transforms/random_node_split.py
+-rw-r--r--   0        0        0     1946 2023-12-21 07:51:56.920388 torch_geometric-2.5.3/torch_geometric/transforms/random_rotate.py
+-rw-r--r--   0        0        0     1261 2023-12-21 07:51:56.920489 torch_geometric-2.5.3/torch_geometric/transforms/random_scale.py
+-rw-r--r--   0        0        0     1365 2023-12-21 07:51:56.920588 torch_geometric-2.5.3/torch_geometric/transforms/random_shear.py
+-rw-r--r--   0        0        0     1929 2023-12-21 07:51:56.920688 torch_geometric-2.5.3/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-r--r--   0        0        0     2449 2023-12-21 07:51:56.920778 torch_geometric-2.5.3/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-r--r--   0        0        0      932 2023-07-21 07:41:11.175066 torch_geometric-2.5.3/torch_geometric/transforms/remove_training_classes.py
+-rw-r--r--   0        0        0     6509 2023-12-21 07:51:56.920901 torch_geometric-2.5.3/torch_geometric/transforms/rooted_subgraph.py
+-rw-r--r--   0        0        0     2214 2024-04-19 11:45:50.643595 torch_geometric-2.5.3/torch_geometric/transforms/sample_points.py
+-rw-r--r--   0        0        0     2329 2023-12-31 08:35:31.857403 torch_geometric-2.5.3/torch_geometric/transforms/sign.py
+-rw-r--r--   0        0        0     2320 2023-12-21 07:51:56.921167 torch_geometric-2.5.3/torch_geometric/transforms/spherical.py
+-rw-r--r--   0        0        0     1009 2023-12-21 07:51:56.921248 torch_geometric-2.5.3/torch_geometric/transforms/svd_feature_reduction.py
+-rw-r--r--   0        0        0     1659 2023-12-21 07:51:56.921334 torch_geometric-2.5.3/torch_geometric/transforms/target_indegree.py
+-rw-r--r--   0        0        0     2456 2023-12-21 07:51:56.921417 torch_geometric-2.5.3/torch_geometric/transforms/to_dense.py
+-rw-r--r--   0        0        0     1470 2023-12-21 07:51:56.921516 torch_geometric-2.5.3/torch_geometric/transforms/to_device.py
+-rw-r--r--   0        0        0     5544 2024-04-19 11:45:50.643728 torch_geometric-2.5.3/torch_geometric/transforms/to_sparse_tensor.py
+-rw-r--r--   0        0        0     2697 2023-12-21 07:51:56.921749 torch_geometric-2.5.3/torch_geometric/transforms/to_superpixels.py
+-rw-r--r--   0        0        0     2972 2023-05-29 07:55:13.287697 torch_geometric-2.5.3/torch_geometric/transforms/to_undirected.py
+-rw-r--r--   0        0        0     1295 2023-12-21 07:51:56.921852 torch_geometric-2.5.3/torch_geometric/transforms/two_hop.py
+-rw-r--r--   0        0        0     2860 2023-12-21 07:51:56.921942 torch_geometric-2.5.3/torch_geometric/transforms/virtual_node.py
+-rw-r--r--   0        0        0    13164 2024-04-19 11:45:50.644317 torch_geometric-2.5.3/torch_geometric/typing.py
+-rw-r--r--   0        0        0     4762 2024-04-19 11:45:50.644526 torch_geometric-2.5.3/torch_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2347 2023-12-21 07:51:56.922253 torch_geometric-2.5.3/torch_geometric/utils/_assortativity.py
+-rw-r--r--   0        0        0     6769 2024-02-15 14:55:33.362583 torch_geometric-2.5.3/torch_geometric/utils/_coalesce.py
+-rw-r--r--   0        0        0     1017 2023-12-21 07:51:56.922548 torch_geometric-2.5.3/torch_geometric/utils/_degree.py
+-rw-r--r--   0        0        0     2562 2023-12-21 07:51:56.922604 torch_geometric-2.5.3/torch_geometric/utils/_grid.py
+-rw-r--r--   0        0        0     5090 2023-12-21 07:51:56.922694 torch_geometric-2.5.3/torch_geometric/utils/_homophily.py
+-rw-r--r--   0        0        0     1283 2024-03-24 11:16:57.302966 torch_geometric-2.5.3/torch_geometric/utils/_index_sort.py
+-rw-r--r--   0        0        0     1403 2023-12-21 07:51:56.922813 torch_geometric-2.5.3/torch_geometric/utils/_lexsort.py
+-rw-r--r--   0        0        0    14672 2023-12-21 07:51:56.922888 torch_geometric-2.5.3/torch_geometric/utils/_negative_sampling.py
+-rw-r--r--   0        0        0     1167 2023-12-21 07:51:56.923075 torch_geometric-2.5.3/torch_geometric/utils/_normalized_cut.py
+-rw-r--r--   0        0        0     1404 2023-12-21 07:51:56.923295 torch_geometric-2.5.3/torch_geometric/utils/_one_hot.py
+-rw-r--r--   0        0        0    11532 2024-04-19 11:45:50.644857 torch_geometric-2.5.3/torch_geometric/utils/_scatter.py
+-rw-r--r--   0        0        0     1868 2024-04-19 11:45:50.645080 torch_geometric-2.5.3/torch_geometric/utils/_segment.py
+-rw-r--r--   0        0        0     2439 2023-12-21 07:51:56.923526 torch_geometric-2.5.3/torch_geometric/utils/_select.py
+-rw-r--r--   0        0        0     3177 2024-04-19 11:45:50.645215 torch_geometric-2.5.3/torch_geometric/utils/_softmax.py
+-rw-r--r--   0        0        0     4500 2024-02-15 14:55:33.362919 torch_geometric-2.5.3/torch_geometric/utils/_sort_edge_index.py
+-rw-r--r--   0        0        0     5542 2024-04-19 11:45:50.645352 torch_geometric-2.5.3/torch_geometric/utils/_spmm.py
+-rw-r--r--   0        0        0    18311 2024-01-16 19:07:07.477049 torch_geometric-2.5.3/torch_geometric/utils/_subgraph.py
+-rw-r--r--   0        0        0     3606 2023-12-21 07:51:56.924061 torch_geometric-2.5.3/torch_geometric/utils/_to_dense_adj.py
+-rw-r--r--   0        0        0     4582 2023-12-21 07:51:56.924154 torch_geometric-2.5.3/torch_geometric/utils/_to_dense_batch.py
+-rw-r--r--   0        0        0     3569 2023-12-21 07:51:56.924210 torch_geometric-2.5.3/torch_geometric/utils/_train_test_split_edges.py
+-rw-r--r--   0        0        0     5300 2023-12-21 07:51:56.924298 torch_geometric-2.5.3/torch_geometric/utils/_tree_decomposition.py
+-rw-r--r--   0        0        0     8412 2024-04-19 11:45:50.645538 torch_geometric-2.5.3/torch_geometric/utils/_trim_to_layer.py
+-rw-r--r--   0        0        0     2378 2023-12-21 07:51:56.924478 torch_geometric-2.5.3/torch_geometric/utils/_unbatch.py
+-rw-r--r--   0        0        0     8601 2023-12-21 07:51:56.924662 torch_geometric-2.5.3/torch_geometric/utils/augmentation.py
+-rw-r--r--   0        0        0    21571 2024-04-19 11:45:50.646174 torch_geometric-2.5.3/torch_geometric/utils/convert.py
+-rw-r--r--   0        0        0     3047 2023-12-21 07:51:56.924887 torch_geometric-2.5.3/torch_geometric/utils/cross_entropy.py
+-rw-r--r--   0        0        0    11416 2024-01-07 13:37:00.563553 torch_geometric-2.5.3/torch_geometric/utils/dropout.py
+-rw-r--r--   0        0        0     1675 2023-12-21 07:51:56.925133 torch_geometric-2.5.3/torch_geometric/utils/embedding.py
+-rw-r--r--   0        0        0      703 2023-11-23 19:01:39.121419 torch_geometric-2.5.3/torch_geometric/utils/functions.py
+-rw-r--r--   0        0        0     4626 2024-04-19 11:45:50.646546 torch_geometric-2.5.3/torch_geometric/utils/geodesic.py
+-rw-r--r--   0        0        0     5542 2024-02-15 14:55:33.363124 torch_geometric-2.5.3/torch_geometric/utils/hetero.py
+-rw-r--r--   0        0        0     3588 2023-12-21 07:51:56.925463 torch_geometric-2.5.3/torch_geometric/utils/isolated.py
+-rw-r--r--   0        0        0     3695 2023-12-21 07:51:56.925525 torch_geometric-2.5.3/torch_geometric/utils/laplacian.py
+-rw-r--r--   0        0        0    22950 2024-04-19 11:45:50.647510 torch_geometric-2.5.3/torch_geometric/utils/loop.py
+-rw-r--r--   0        0        0     5674 2024-04-19 11:45:50.647701 torch_geometric-2.5.3/torch_geometric/utils/map.py
+-rw-r--r--   0        0        0     2340 2023-11-23 19:01:39.122614 torch_geometric-2.5.3/torch_geometric/utils/mask.py
+-rw-r--r--   0        0        0     4387 2023-12-21 07:51:56.925857 torch_geometric-2.5.3/torch_geometric/utils/mesh_laplacian.py
+-rw-r--r--   0        0        0      699 2023-12-21 07:51:56.925943 torch_geometric-2.5.3/torch_geometric/utils/mixin.py
+-rw-r--r--   0        0        0     3310 2023-12-21 07:51:56.926263 torch_geometric-2.5.3/torch_geometric/utils/nested.py
+-rw-r--r--   0        0        0     3750 2023-12-21 07:51:56.926325 torch_geometric-2.5.3/torch_geometric/utils/noise_scheduler.py
+-rw-r--r--   0        0        0     2176 2024-01-16 19:07:07.477793 torch_geometric-2.5.3/torch_geometric/utils/num_nodes.py
+-rw-r--r--   0        0        0     4055 2023-12-31 08:35:31.857981 torch_geometric-2.5.3/torch_geometric/utils/ppr.py
+-rw-r--r--   0        0        0     5148 2023-11-23 19:01:39.123097 torch_geometric-2.5.3/torch_geometric/utils/random.py
+-rw-r--r--   0        0        0      815 2023-06-10 14:35:51.131530 torch_geometric-2.5.3/torch_geometric/utils/repeat.py
+-rw-r--r--   0        0        0     6242 2023-12-21 07:51:56.926536 torch_geometric-2.5.3/torch_geometric/utils/smiles.py
+-rw-r--r--   0        0        0    25034 2024-04-19 11:45:50.648278 torch_geometric-2.5.3/torch_geometric/utils/sparse.py
+-rw-r--r--   0        0        0     6222 2023-12-21 07:51:56.927152 torch_geometric-2.5.3/torch_geometric/utils/undirected.py
+-rw-r--r--   0        0        0      154 2023-11-23 19:01:39.124605 torch_geometric-2.5.3/torch_geometric/visualization/__init__.py
+-rw-r--r--   0        0        0     4813 2024-02-15 14:55:33.363335 torch_geometric-2.5.3/torch_geometric/visualization/graph.py
+-rw-r--r--   0        0        0      477 2023-12-21 07:51:56.927546 torch_geometric-2.5.3/torch_geometric/visualization/influence.py
+-rw-r--r--   0        0        0      413 2024-01-07 13:37:00.563808 torch_geometric-2.5.3/torch_geometric/warnings.py
+-rw-r--r--   0        0        0    64156 1970-01-01 00:00:00.000000 torch_geometric-2.5.3/PKG-INFO
```

### Comparing `torch_geometric-2.5.2/README.md` & `torch_geometric-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/pyproject.toml` & `torch_geometric-2.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="torch_geometric"
-version="2.5.2"
+version="2.5.3"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.8"
 keywords=[
```

### Comparing `torch_geometric-2.5.2/torch_geometric/__init__.py` & `torch_geometric-2.5.3/torch_geometric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.5.2'
+__version__ = '2.5.3'
 
 __all__ = [
     'EdgeIndex',
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
     'compile',
```

### Comparing `torch_geometric-2.5.2/torch_geometric/_compile.py` & `torch_geometric-2.5.3/torch_geometric/_compile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/backend.py` & `torch_geometric-2.5.3/torch_geometric/backend.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/config_store.py` & `torch_geometric-2.5.3/torch_geometric/config_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/contrib/explain/pgm_explainer.py` & `torch_geometric-2.5.3/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/contrib/nn/models/rbcd_attack.py` & `torch_geometric-2.5.3/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/__init__.py` & `torch_geometric-2.5.3/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/batch.py` & `torch_geometric-2.5.3/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/collate.py` & `torch_geometric-2.5.3/torch_geometric/data/collate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/data.py` & `torch_geometric-2.5.3/torch_geometric/data/data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/database.py` & `torch_geometric-2.5.3/torch_geometric/data/database.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/datapipes.py` & `torch_geometric-2.5.3/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/dataset.py` & `torch_geometric-2.5.3/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/download.py` & `torch_geometric-2.5.3/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/extract.py` & `torch_geometric-2.5.3/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/feature_store.py` & `torch_geometric-2.5.3/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/graph_store.py` & `torch_geometric-2.5.3/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/hetero_data.py` & `torch_geometric-2.5.3/torch_geometric/data/hetero_data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/hypergraph_data.py` & `torch_geometric-2.5.3/torch_geometric/data/hypergraph_data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/in_memory_dataset.py` & `torch_geometric-2.5.3/torch_geometric/data/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/lightning/datamodule.py` & `torch_geometric-2.5.3/torch_geometric/data/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/on_disk_dataset.py` & `torch_geometric-2.5.3/torch_geometric/data/on_disk_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/remote_backend_utils.py` & `torch_geometric-2.5.3/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/separate.py` & `torch_geometric-2.5.3/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/storage.py` & `torch_geometric-2.5.3/torch_geometric/data/storage.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/summary.py` & `torch_geometric-2.5.3/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/temporal.py` & `torch_geometric-2.5.3/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/data/view.py` & `torch_geometric-2.5.3/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/__init__.py` & `torch_geometric-2.5.3/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/actor.py` & `torch_geometric-2.5.3/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/airfrans.py` & `torch_geometric-2.5.3/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/airports.py` & `torch_geometric-2.5.3/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/amazon.py` & `torch_geometric-2.5.3/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/amazon_book.py` & `torch_geometric-2.5.3/torch_geometric/datasets/amazon_book.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/amazon_products.py` & `torch_geometric-2.5.3/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/aminer.py` & `torch_geometric-2.5.3/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/aqsol.py` & `torch_geometric-2.5.3/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/attributed_graph_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ba2motif_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ba_multi_shapes.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ba_shapes.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/bitcoin_otc.py` & `torch_geometric-2.5.3/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/brca_tgca.py` & `torch_geometric-2.5.3/torch_geometric/datasets/brca_tgca.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/citation_full.py` & `torch_geometric-2.5.3/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/coauthor.py` & `torch_geometric-2.5.3/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/coma.py` & `torch_geometric-2.5.3/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/dblp.py` & `torch_geometric-2.5.3/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/dbp15k.py` & `torch_geometric-2.5.3/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/deezer_europe.py` & `torch_geometric-2.5.3/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/dgraph.py` & `torch_geometric-2.5.3/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/dynamic_faust.py` & `torch_geometric-2.5.3/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/elliptic.py` & `torch_geometric-2.5.3/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/elliptic_temporal.py` & `torch_geometric-2.5.3/torch_geometric/datasets/elliptic_temporal.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/email_eu_core.py` & `torch_geometric-2.5.3/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/entities.py` & `torch_geometric-2.5.3/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/explainer_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/facebook.py` & `torch_geometric-2.5.3/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/fake.py` & `torch_geometric-2.5.3/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/faust.py` & `torch_geometric-2.5.3/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/flickr.py` & `torch_geometric-2.5.3/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/freebase.py` & `torch_geometric-2.5.3/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/gdelt.py` & `torch_geometric-2.5.3/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/gdelt_lite.py` & `torch_geometric-2.5.3/torch_geometric/datasets/gdelt_lite.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ged_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/gemsec.py` & `torch_geometric-2.5.3/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/geometry.py` & `torch_geometric-2.5.3/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/github.py` & `torch_geometric-2.5.3/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/gnn_benchmark_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/ba_graph.py` & `torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/base.py` & `torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/er_graph.py` & `torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/grid_graph.py` & `torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/graph_generator/tree_graph.py` & `torch_geometric-2.5.3/torch_geometric/datasets/graph_generator/tree_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/heterophilous_graph_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/hgb_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/hm.py` & `torch_geometric-2.5.3/torch_geometric/datasets/hm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/hydro_net.py` & `torch_geometric-2.5.3/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/icews.py` & `torch_geometric-2.5.3/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/igmc_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/igmc_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/imdb.py` & `torch_geometric-2.5.3/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/infection_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/jodie.py` & `torch_geometric-2.5.3/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/karate.py` & `torch_geometric-2.5.3/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/last_fm.py` & `torch_geometric-2.5.3/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/lastfm_asia.py` & `torch_geometric-2.5.3/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/linkx_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/lrgb.py` & `torch_geometric-2.5.3/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/malnet_tiny.py` & `torch_geometric-2.5.3/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/md17.py` & `torch_geometric-2.5.3/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/mnist_superpixels.py` & `torch_geometric-2.5.3/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/modelnet.py` & `torch_geometric-2.5.3/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/molecule_net.py` & `torch_geometric-2.5.3/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/base.py` & `torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/custom.py` & `torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/cycle.py` & `torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/grid.py` & `torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/grid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/motif_generator/house.py` & `torch_geometric-2.5.3/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/movie_lens.py` & `torch_geometric-2.5.3/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/movie_lens_100k.py` & `torch_geometric-2.5.3/torch_geometric/datasets/movie_lens_100k.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/movie_lens_1m.py` & `torch_geometric-2.5.3/torch_geometric/datasets/movie_lens_1m.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/myket.py` & `torch_geometric-2.5.3/torch_geometric/datasets/myket.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/nell.py` & `torch_geometric-2.5.3/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/neurograph.py` & `torch_geometric-2.5.3/torch_geometric/datasets/neurograph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ogb_mag.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/omdb.py` & `torch_geometric-2.5.3/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ose_gvcs.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ose_gvcs.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/particle.py` & `torch_geometric-2.5.3/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/pascal.py` & `torch_geometric-2.5.3/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/pascal_pf.py` & `torch_geometric-2.5.3/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/pcpnet_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/pcqm4m.py` & `torch_geometric-2.5.3/torch_geometric/datasets/pcqm4m.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/planetoid.py` & `torch_geometric-2.5.3/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/polblogs.py` & `torch_geometric-2.5.3/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/ppi.py` & `torch_geometric-2.5.3/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/qm7.py` & `torch_geometric-2.5.3/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/qm9.py` & `torch_geometric-2.5.3/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/rcdd.py` & `torch_geometric-2.5.3/torch_geometric/datasets/rcdd.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/reddit.py` & `torch_geometric-2.5.3/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/reddit2.py` & `torch_geometric-2.5.3/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/rel_link_pred_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/s3dis.py` & `torch_geometric-2.5.3/torch_geometric/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/sbm_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/shapenet.py` & `torch_geometric-2.5.3/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/shrec2016.py` & `torch_geometric-2.5.3/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/snap_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/suite_sparse.py` & `torch_geometric-2.5.3/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/taobao.py` & `torch_geometric-2.5.3/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/tosca.py` & `torch_geometric-2.5.3/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/tu_dataset.py` & `torch_geometric-2.5.3/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/twitch.py` & `torch_geometric-2.5.3/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/upfd.py` & `torch_geometric-2.5.3/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/utils/cheatsheet.py` & `torch_geometric-2.5.3/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/webkb.py` & `torch_geometric-2.5.3/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/wikics.py` & `torch_geometric-2.5.3/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/wikidata.py` & `torch_geometric-2.5.3/torch_geometric/datasets/wikidata.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/wikipedia_network.py` & `torch_geometric-2.5.3/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/willow_object_class.py` & `torch_geometric-2.5.3/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/word_net.py` & `torch_geometric-2.5.3/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/yelp.py` & `torch_geometric-2.5.3/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/datasets/zinc.py` & `torch_geometric-2.5.3/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/debug.py` & `torch_geometric-2.5.3/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/deprecation.py` & `torch_geometric-2.5.3/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/__init__.py` & `torch_geometric-2.5.3/torch_geometric/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/dist_link_neighbor_loader.py` & `torch_geometric-2.5.3/torch_geometric/distributed/dist_link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/dist_loader.py` & `torch_geometric-2.5.3/torch_geometric/distributed/dist_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/dist_neighbor_loader.py` & `torch_geometric-2.5.3/torch_geometric/distributed/dist_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/dist_neighbor_sampler.py` & `torch_geometric-2.5.3/torch_geometric/distributed/dist_neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/event_loop.py` & `torch_geometric-2.5.3/torch_geometric/distributed/event_loop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/local_feature_store.py` & `torch_geometric-2.5.3/torch_geometric/distributed/local_feature_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/local_graph_store.py` & `torch_geometric-2.5.3/torch_geometric/distributed/local_graph_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/partition.py` & `torch_geometric-2.5.3/torch_geometric/distributed/partition.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/rpc.py` & `torch_geometric-2.5.3/torch_geometric/distributed/rpc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/distributed/utils.py` & `torch_geometric-2.5.3/torch_geometric/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/edge_index.py` & `torch_geometric-2.5.3/torch_geometric/edge_index.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/experimental.py` & `torch_geometric-2.5.3/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/attention_explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/base.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/captum.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/captum_explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/dummy_explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/gnn_explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/graphmask_explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/pg_explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/algorithm/utils.py` & `torch_geometric-2.5.3/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/config.py` & `torch_geometric-2.5.3/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/explainer.py` & `torch_geometric-2.5.3/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/explanation.py` & `torch_geometric-2.5.3/torch_geometric/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/metric/basic.py` & `torch_geometric-2.5.3/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/metric/faithfulness.py` & `torch_geometric-2.5.3/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/explain/metric/fidelity.py` & `torch_geometric-2.5.3/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/__init__.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/checkpoint.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/cmd_args.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/config.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/contrib/layer/generalconv.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/init.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/init.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/loader.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/logger.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/loss.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/model_builder.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/__init__.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/act.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/encoder.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/gnn.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/head.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/layer.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/models/transform.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/optim.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/register.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/train.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/__init__.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/agg_runs.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/comp_budget.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/device.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/epoch.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/io.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/graphgym/utils/plot.py` & `torch_geometric-2.5.3/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/home.py` & `torch_geometric-2.5.3/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/inspector.py` & `torch_geometric-2.5.3/torch_geometric/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/__init__.py` & `torch_geometric-2.5.3/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/fs.py` & `torch_geometric-2.5.3/torch_geometric/io/fs.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/npz.py` & `torch_geometric-2.5.3/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/obj.py` & `torch_geometric-2.5.3/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/off.py` & `torch_geometric-2.5.3/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/planetoid.py` & `torch_geometric-2.5.3/torch_geometric/io/planetoid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/sdf.py` & `torch_geometric-2.5.3/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/tu.py` & `torch_geometric-2.5.3/torch_geometric/io/tu.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/io/txt_array.py` & `torch_geometric-2.5.3/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/isinstance.py` & `torch_geometric-2.5.3/torch_geometric/isinstance.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/lazy_loader.py` & `torch_geometric-2.5.3/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/__init__.py` & `torch_geometric-2.5.3/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/base.py` & `torch_geometric-2.5.3/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/cache.py` & `torch_geometric-2.5.3/torch_geometric/loader/cache.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/cluster.py` & `torch_geometric-2.5.3/torch_geometric/loader/cluster.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/data_list_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/dataloader.py` & `torch_geometric-2.5.3/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/dense_data_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/dynamic_batch_sampler.py` & `torch_geometric-2.5.3/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/graph_saint.py` & `torch_geometric-2.5.3/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/hgt_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/ibmb_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/ibmb_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/imbalanced_sampler.py` & `torch_geometric-2.5.3/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/link_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/link_neighbor_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/mixin.py` & `torch_geometric-2.5.3/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/neighbor_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/neighbor_sampler.py` & `torch_geometric-2.5.3/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/node_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/prefetch.py` & `torch_geometric-2.5.3/torch_geometric/loader/prefetch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/random_node_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/shadow.py` & `torch_geometric-2.5.3/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/temporal_dataloader.py` & `torch_geometric-2.5.3/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/utils.py` & `torch_geometric-2.5.3/torch_geometric/loader/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/loader/zip_loader.py` & `torch_geometric-2.5.3/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/logging.py` & `torch_geometric-2.5.3/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/metrics/link_pred.py` & `torch_geometric-2.5.3/torch_geometric/metrics/link_pred.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/attention.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/base.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/basic.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/deep_sets.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/equilibrium.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/equilibrium.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/fused.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/gmt.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/gru.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/lcm.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/lcm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/lstm.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/mlp.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/multi.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/quantile.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/quantile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/scaler.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/set2set.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/set_transformer.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/sort.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/aggr/utils.py` & `torch_geometric-2.5.3/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/attention/performer.py` & `torch_geometric-2.5.3/torch_geometric/nn/attention/performer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/agnn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/antisymmetric_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/appnp.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/arma_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cg_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cheb_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cluster_gcn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/collect.jinja` & `torch_geometric-2.5.3/torch_geometric/nn/conv/collect.jinja`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/base.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/gat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/cugraph/sage_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/dir_gnn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/dir_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/dna_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/edge_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/edge_updater.jinja` & `torch_geometric-2.5.3/torch_geometric/nn/conv/edge_updater.jinja`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/eg_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/fa_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/feast_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/film_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/fused_gat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gated_graph_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gatv2_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gcn2_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gcn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gen_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/general_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gin_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gmm_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gps_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/graph_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/gravnet_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/han_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/heat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/hetero_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/hgt_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/hypergraph_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/le_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/lg_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/message_passing.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/message_passing.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,20 +163,23 @@
         self._edge_update_forward_hooks: HookDict = OrderedDict()
 
         root_dir = osp.dirname(osp.realpath(__file__))
         jinja_prefix = f'{self.__module__}_{self.__class__.__name__}'
         # Optimize `propagate()` via `*.jinja` templates:
         if not self.propagate.__module__.startswith(jinja_prefix):
             try:
+                if 'propagate' in self.__class__.__dict__:
+                    raise ValueError("Cannot compile custom 'propagate' "
+                                     "method")
                 module = module_from_template(
                     module_name=f'{jinja_prefix}_propagate',
                     template_path=osp.join(root_dir, 'propagate.jinja'),
                     tmp_dirname='message_passing',
                     # Keyword arguments:
-                    module=self.inspector._modules,
+                    modules=self.inspector._modules,
                     collect_name='collect',
                     signature=self._get_propagate_signature(),
                     collect_param_dict=self.inspector.get_flat_param_dict(
                         ['message', 'aggregate', 'update']),
                     message_args=self.inspector.get_param_names('message'),
                     aggregate_args=self.inspector.get_param_names('aggregate'),
                     message_and_aggregate_args=self.inspector.get_param_names(
@@ -194,14 +197,17 @@
                 self.__class__._orig_propagate = self.__class__.propagate
                 self.__class__._jinja_propagate = self.__class__.propagate
 
         # Optimize `edge_updater()` via `*.jinja` templates (if implemented):
         if (self.inspector.implements('edge_update')
                 and not self.edge_updater.__module__.startswith(jinja_prefix)):
             try:
+                if 'edge_updater' in self.__class__.__dict__:
+                    raise ValueError("Cannot compile custom 'edge_updater' "
+                                     "method")
                 module = module_from_template(
                     module_name=f'{jinja_prefix}_edge_updater',
                     template_path=osp.join(root_dir, 'edge_updater.jinja'),
                     tmp_dirname='message_passing',
                     # Keyword arguments:
                     modules=self.inspector._modules,
                     collect_name='edge_collect',
@@ -223,14 +229,15 @@
         # Explainability:
         self._explain: Optional[bool] = None
         self._edge_mask: Optional[Tensor] = None
         self._loop_mask: Optional[Tensor] = None
         self._apply_sigmoid: bool = True
 
         # Inference Decomposition:
+        self._decomposed_layers = 1
         self.decomposed_layers = decomposed_layers
 
     def reset_parameters(self) -> None:
         r"""Resets all learnable parameters of the module."""
         if self.aggr_module is not None:
             self.aggr_module.reset_parameters()
 
@@ -707,57 +714,66 @@
 
     @decomposed_layers.setter
     def decomposed_layers(self, decomposed_layers: int) -> None:
         if torch.jit.is_scripting():
             raise ValueError("Inference decomposition of message passing "
                              "modules is only supported on the Python module")
 
+        if decomposed_layers == self._decomposed_layers:
+            return  # Abort early if nothing to do.
+
         self._decomposed_layers = decomposed_layers
 
         if decomposed_layers != 1:
-            self.propagate = self.__class__._orig_propagate.__get__(
-                self, MessagePassing)
+            if hasattr(self.__class__, '_orig_propagate'):
+                self.propagate = self.__class__._orig_propagate.__get__(
+                    self, MessagePassing)
 
-        elif ((self.explain is None or self.explain is False)
-              and not self.propagate.__module__.endswith('_propagate')):
-            self.propagate = self.__class__._jinja_propagate.__get__(
-                self, MessagePassing)
+        elif self.explain is None or self.explain is False:
+            if hasattr(self.__class__, '_jinja_propagate'):
+                self.propagate = self.__class__._jinja_propagate.__get__(
+                    self, MessagePassing)
 
     # Explainability ##########################################################
 
     @property
     def explain(self) -> Optional[bool]:
         return self._explain
 
     @explain.setter
     def explain(self, explain: Optional[bool]) -> None:
         if torch.jit.is_scripting():
             raise ValueError("Explainability of message passing modules "
                              "is only supported on the Python module")
 
+        if explain == self._explain:
+            return  # Abort early if nothing to do.
+
         self._explain = explain
 
         if explain is True:
             assert self.decomposed_layers == 1
             self.inspector.remove_signature(self.explain_message)
             self.inspector.inspect_signature(self.explain_message, exclude=[0])
             self._user_args = self.inspector.get_flat_param_names(
                 funcs=['message', 'explain_message', 'aggregate', 'update'],
                 exclude=self.special_args,
             )
-            self.propagate = self.__class__._orig_propagate.__get__(
-                self, MessagePassing)
+            if hasattr(self.__class__, '_orig_propagate'):
+                self.propagate = self.__class__._orig_propagate.__get__(
+                    self, MessagePassing)
         else:
             self._user_args = self.inspector.get_flat_param_names(
                 funcs=['message', 'aggregate', 'update'],
                 exclude=self.special_args,
             )
             if self.decomposed_layers == 1:
-                self.propagate = self.__class__._jinja_propagate.__get__(
-                    self, MessagePassing)
+                if hasattr(self.__class__, '_jinja_propagate'):
+                    self.propagate = self.__class__._jinja_propagate.__get__(
+                        self, MessagePassing)
 
     def explain_message(
         self,
         inputs: Tensor,
         dim_size: Optional[int],
     ) -> Tensor:
         # NOTE Replace this method in custom explainers per message-passing
```

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/mf_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/mixhop_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/mixhop_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/nn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/pan_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/pdn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/pna_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/point_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/point_gnn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/point_transformer_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/ppf_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/propagate.jinja` & `torch_geometric-2.5.3/torch_geometric/nn/conv/propagate.jinja`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/res_gated_graph_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/rgat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/rgcn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/sage_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/sg_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/signed_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/simple_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/spline_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/ssg_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/supergat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/tag_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/transformer_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/utils/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/utils/cheatsheet.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/wl_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/wl_conv_continuous.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/conv/x_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/data_parallel.py` & `torch_geometric-2.5.3/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/dense_gat_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/dense_gcn_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/dense_gin_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/dense_graph_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/dense_sage_conv.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/diff_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/dmon_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/linear.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/dense/mincut_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/encoding.py` & `torch_geometric-2.5.3/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/functional/bro.py` & `torch_geometric-2.5.3/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/functional/gini.py` & `torch_geometric-2.5.3/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/fx.py` & `torch_geometric-2.5.3/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/glob.py` & `torch_geometric-2.5.3/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/inits.py` & `torch_geometric-2.5.3/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/kge/base.py` & `torch_geometric-2.5.3/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/kge/complex.py` & `torch_geometric-2.5.3/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/kge/distmult.py` & `torch_geometric-2.5.3/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/kge/loader.py` & `torch_geometric-2.5.3/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/kge/rotate.py` & `torch_geometric-2.5.3/torch_geometric/nn/kge/rotate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/kge/transe.py` & `torch_geometric-2.5.3/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/lr_scheduler.py` & `torch_geometric-2.5.3/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/model_hub.py` & `torch_geometric-2.5.3/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/attentive_fp.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/autoencoder.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/basic_gnn.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/basic_gnn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/captum.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/correct_and_smooth.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/deep_graph_infomax.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/deepgcn.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/dimenet.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/dimenet_utils.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/gnnff.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/graph_mixer.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/graph_mixer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/graph_unet.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/jumping_knowledge.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/label_prop.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/lightgcn.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/linkx.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/mask_label.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/meta.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/metapath2vec.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/mlp.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/neural_fingerprint.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/neural_fingerprint.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/node2vec.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/pmlp.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/pmlp.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/re_net.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/rect.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/rev_gnn.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/schnet.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/signed_gcn.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/tgn.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/models/visnet.py` & `torch_geometric-2.5.3/torch_geometric/nn/models/visnet.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/module_dict.py` & `torch_geometric-2.5.3/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/batch_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/diff_group_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/graph_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/graph_size_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/instance_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/layer_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/mean_subtraction_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/msg_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/norm/pair_norm.py` & `torch_geometric-2.5.3/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/parameter_dict.py` & `torch_geometric-2.5.3/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/__init__.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/approx_knn.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/approx_knn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/asap.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/avg_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/connect/base.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/connect/filter_edges.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/connect/filter_edges.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/decimation.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/edge_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/glob.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/graclus.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/knn.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/knn.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/max_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/mem_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/pan_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/sag_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/select/base.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/select/topk.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/select/topk.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/topk_pool.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/pool/voxel_grid.py` & `torch_geometric-2.5.3/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/resolver.py` & `torch_geometric-2.5.3/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/sequential.jinja` & `torch_geometric-2.5.3/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/sequential.py` & `torch_geometric-2.5.3/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/summary.py` & `torch_geometric-2.5.3/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/to_fixed_size_transformer.py` & `torch_geometric-2.5.3/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/to_hetero_module.py` & `torch_geometric-2.5.3/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/to_hetero_transformer.py` & `torch_geometric-2.5.3/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `torch_geometric-2.5.3/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/nn/unpool/knn_interpolate.py` & `torch_geometric-2.5.3/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/profile/__init__.py` & `torch_geometric-2.5.3/torch_geometric/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/profile/benchmark.py` & `torch_geometric-2.5.3/torch_geometric/profile/benchmark.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/profile/profile.py` & `torch_geometric-2.5.3/torch_geometric/profile/profile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/profile/profiler.py` & `torch_geometric-2.5.3/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/profile/utils.py` & `torch_geometric-2.5.3/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/resolver.py` & `torch_geometric-2.5.3/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/sampler/__init__.py` & `torch_geometric-2.5.3/torch_geometric/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/sampler/base.py` & `torch_geometric-2.5.3/torch_geometric/sampler/base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/sampler/hgt_sampler.py` & `torch_geometric-2.5.3/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/sampler/neighbor_sampler.py` & `torch_geometric-2.5.3/torch_geometric/sampler/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/sampler/utils.py` & `torch_geometric-2.5.3/torch_geometric/sampler/utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/template.py` & `torch_geometric-2.5.3/torch_geometric/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     with tempfile.NamedTemporaryFile(
             mode='w',
             prefix=f'{module_name}_',
             suffix='.py',
             delete=False,
     ) as tmp:
         tmp.write(module_repr)
+        tmp.flush()
 
     spec = importlib.util.spec_from_file_location(module_name, tmp.name)
     assert spec is not None
     module = importlib.util.module_from_spec(spec)
     sys.modules[module_name] = module
     assert spec.loader is not None
     spec.loader.exec_module(module)
```

### Comparing `torch_geometric-2.5.2/torch_geometric/testing/__init__.py` & `torch_geometric-2.5.3/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/testing/asserts.py` & `torch_geometric-2.5.3/torch_geometric/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/testing/data.py` & `torch_geometric-2.5.3/torch_geometric/testing/data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/testing/decorators.py` & `torch_geometric-2.5.3/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/testing/feature_store.py` & `torch_geometric-2.5.3/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/testing/graph_store.py` & `torch_geometric-2.5.3/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/__init__.py` & `torch_geometric-2.5.3/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/add_metapaths.py` & `torch_geometric-2.5.3/torch_geometric/transforms/add_metapaths.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/add_positional_encoding.py` & `torch_geometric-2.5.3/torch_geometric/transforms/add_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/add_remaining_self_loops.py` & `torch_geometric-2.5.3/torch_geometric/transforms/add_remaining_self_loops.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/add_self_loops.py` & `torch_geometric-2.5.3/torch_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/base_transform.py` & `torch_geometric-2.5.3/torch_geometric/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/cartesian.py` & `torch_geometric-2.5.3/torch_geometric/transforms/cartesian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/center.py` & `torch_geometric-2.5.3/torch_geometric/transforms/center.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/compose.py` & `torch_geometric-2.5.3/torch_geometric/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/constant.py` & `torch_geometric-2.5.3/torch_geometric/transforms/constant.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/delaunay.py` & `torch_geometric-2.5.3/torch_geometric/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/distance.py` & `torch_geometric-2.5.3/torch_geometric/transforms/distance.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/face_to_edge.py` & `torch_geometric-2.5.3/torch_geometric/transforms/face_to_edge.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/feature_propagation.py` & `torch_geometric-2.5.3/torch_geometric/transforms/feature_propagation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/fixed_points.py` & `torch_geometric-2.5.3/torch_geometric/transforms/fixed_points.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/gcn_norm.py` & `torch_geometric-2.5.3/torch_geometric/transforms/gcn_norm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/gdc.py` & `torch_geometric-2.5.3/torch_geometric/transforms/gdc.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/generate_mesh_normals.py` & `torch_geometric-2.5.3/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/grid_sampling.py` & `torch_geometric-2.5.3/torch_geometric/transforms/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/half_hop.py` & `torch_geometric-2.5.3/torch_geometric/transforms/half_hop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/knn_graph.py` & `torch_geometric-2.5.3/torch_geometric/transforms/knn_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/laplacian_lambda_max.py` & `torch_geometric-2.5.3/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/largest_connected_components.py` & `torch_geometric-2.5.3/torch_geometric/transforms/largest_connected_components.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/line_graph.py` & `torch_geometric-2.5.3/torch_geometric/transforms/line_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/linear_transformation.py` & `torch_geometric-2.5.3/torch_geometric/transforms/linear_transformation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/local_cartesian.py` & `torch_geometric-2.5.3/torch_geometric/transforms/local_cartesian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/local_degree_profile.py` & `torch_geometric-2.5.3/torch_geometric/transforms/local_degree_profile.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/mask.py` & `torch_geometric-2.5.3/torch_geometric/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/node_property_split.py` & `torch_geometric-2.5.3/torch_geometric/transforms/node_property_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/normalize_features.py` & `torch_geometric-2.5.3/torch_geometric/transforms/normalize_features.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/normalize_rotation.py` & `torch_geometric-2.5.3/torch_geometric/transforms/normalize_rotation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/normalize_scale.py` & `torch_geometric-2.5.3/torch_geometric/transforms/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/one_hot_degree.py` & `torch_geometric-2.5.3/torch_geometric/transforms/one_hot_degree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/pad.py` & `torch_geometric-2.5.3/torch_geometric/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/point_pair_features.py` & `torch_geometric-2.5.3/torch_geometric/transforms/point_pair_features.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/polar.py` & `torch_geometric-2.5.3/torch_geometric/transforms/polar.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/radius_graph.py` & `torch_geometric-2.5.3/torch_geometric/transforms/radius_graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_flip.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_flip.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_jitter.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_jitter.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_link_split.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_link_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_node_split.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_node_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_rotate.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_rotate.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_scale.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_scale.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/random_shear.py` & `torch_geometric-2.5.3/torch_geometric/transforms/random_shear.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/remove_duplicated_edges.py` & `torch_geometric-2.5.3/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/remove_isolated_nodes.py` & `torch_geometric-2.5.3/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/remove_training_classes.py` & `torch_geometric-2.5.3/torch_geometric/transforms/remove_training_classes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/rooted_subgraph.py` & `torch_geometric-2.5.3/torch_geometric/transforms/rooted_subgraph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/sample_points.py` & `torch_geometric-2.5.3/torch_geometric/transforms/sample_points.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/sign.py` & `torch_geometric-2.5.3/torch_geometric/transforms/sign.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/spherical.py` & `torch_geometric-2.5.3/torch_geometric/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/svd_feature_reduction.py` & `torch_geometric-2.5.3/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/target_indegree.py` & `torch_geometric-2.5.3/torch_geometric/transforms/target_indegree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/to_dense.py` & `torch_geometric-2.5.3/torch_geometric/transforms/to_dense.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/to_device.py` & `torch_geometric-2.5.3/torch_geometric/transforms/to_device.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/to_sparse_tensor.py` & `torch_geometric-2.5.3/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/to_superpixels.py` & `torch_geometric-2.5.3/torch_geometric/transforms/to_superpixels.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/to_undirected.py` & `torch_geometric-2.5.3/torch_geometric/transforms/to_undirected.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/two_hop.py` & `torch_geometric-2.5.3/torch_geometric/transforms/two_hop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/transforms/virtual_node.py` & `torch_geometric-2.5.3/torch_geometric/transforms/virtual_node.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/typing.py` & `torch_geometric-2.5.3/torch_geometric/typing.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/__init__.py` & `torch_geometric-2.5.3/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_assortativity.py` & `torch_geometric-2.5.3/torch_geometric/utils/_assortativity.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_coalesce.py` & `torch_geometric-2.5.3/torch_geometric/utils/_coalesce.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_degree.py` & `torch_geometric-2.5.3/torch_geometric/utils/_degree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_grid.py` & `torch_geometric-2.5.3/torch_geometric/utils/_grid.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_homophily.py` & `torch_geometric-2.5.3/torch_geometric/utils/_homophily.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_index_sort.py` & `torch_geometric-2.5.3/torch_geometric/utils/_index_sort.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_lexsort.py` & `torch_geometric-2.5.3/torch_geometric/utils/_lexsort.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_negative_sampling.py` & `torch_geometric-2.5.3/torch_geometric/utils/_negative_sampling.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_normalized_cut.py` & `torch_geometric-2.5.3/torch_geometric/utils/_normalized_cut.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_one_hot.py` & `torch_geometric-2.5.3/torch_geometric/utils/_one_hot.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_scatter.py` & `torch_geometric-2.5.3/torch_geometric/utils/_scatter.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_segment.py` & `torch_geometric-2.5.3/torch_geometric/utils/_segment.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_select.py` & `torch_geometric-2.5.3/torch_geometric/utils/_select.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_softmax.py` & `torch_geometric-2.5.3/torch_geometric/utils/_softmax.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_sort_edge_index.py` & `torch_geometric-2.5.3/torch_geometric/utils/_sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_spmm.py` & `torch_geometric-2.5.3/torch_geometric/utils/_spmm.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_subgraph.py` & `torch_geometric-2.5.3/torch_geometric/utils/_subgraph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_to_dense_adj.py` & `torch_geometric-2.5.3/torch_geometric/utils/_to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_to_dense_batch.py` & `torch_geometric-2.5.3/torch_geometric/utils/_to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_train_test_split_edges.py` & `torch_geometric-2.5.3/torch_geometric/utils/_train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_tree_decomposition.py` & `torch_geometric-2.5.3/torch_geometric/utils/_tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_trim_to_layer.py` & `torch_geometric-2.5.3/torch_geometric/utils/_trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/_unbatch.py` & `torch_geometric-2.5.3/torch_geometric/utils/_unbatch.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/augmentation.py` & `torch_geometric-2.5.3/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/convert.py` & `torch_geometric-2.5.3/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/cross_entropy.py` & `torch_geometric-2.5.3/torch_geometric/utils/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/dropout.py` & `torch_geometric-2.5.3/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/embedding.py` & `torch_geometric-2.5.3/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/functions.py` & `torch_geometric-2.5.3/torch_geometric/utils/functions.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/geodesic.py` & `torch_geometric-2.5.3/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/hetero.py` & `torch_geometric-2.5.3/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/isolated.py` & `torch_geometric-2.5.3/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/laplacian.py` & `torch_geometric-2.5.3/torch_geometric/utils/laplacian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/loop.py` & `torch_geometric-2.5.3/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/map.py` & `torch_geometric-2.5.3/torch_geometric/utils/map.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/mask.py` & `torch_geometric-2.5.3/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/mesh_laplacian.py` & `torch_geometric-2.5.3/torch_geometric/utils/mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/mixin.py` & `torch_geometric-2.5.3/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/nested.py` & `torch_geometric-2.5.3/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/noise_scheduler.py` & `torch_geometric-2.5.3/torch_geometric/utils/noise_scheduler.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/num_nodes.py` & `torch_geometric-2.5.3/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/ppr.py` & `torch_geometric-2.5.3/torch_geometric/utils/ppr.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/random.py` & `torch_geometric-2.5.3/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/repeat.py` & `torch_geometric-2.5.3/torch_geometric/utils/repeat.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/smiles.py` & `torch_geometric-2.5.3/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/sparse.py` & `torch_geometric-2.5.3/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/utils/undirected.py` & `torch_geometric-2.5.3/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/torch_geometric/visualization/graph.py` & `torch_geometric-2.5.3/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `torch_geometric-2.5.2/PKG-INFO` & `torch_geometric-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_geometric
-Version: 2.5.2
+Version: 2.5.3
 Summary: Graph Neural Network Library for PyTorch
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
 Author-email: Matthias Fey <matthias@pyg.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

