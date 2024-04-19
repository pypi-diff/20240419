# Comparing `tmp/alphapulldown-2.0.0b1.tar.gz` & `tmp/alphapulldown-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphapulldown-2.0.0b1.tar", last modified: Tue Apr  9 14:04:56 2024, max compression
+gzip compressed data, was "alphapulldown-2.0.0b2.tar", last modified: Fri Apr 19 12:40:35 2024, max compression
```

## Comparing `alphapulldown-2.0.0b1.tar` & `alphapulldown-2.0.0b2.tar`

### file list

```diff
@@ -1,237 +1,236 @@
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.993713 alphapulldown-2.0.0b1/
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.547797 alphapulldown-2.0.0b1/AlphaLink2/
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.716786 alphapulldown-2.0.0b1/AlphaLink2/unifold/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       72 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10975 2024-03-18 14:19:42.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/alphalink_inference.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    29224 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/config.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.809846 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      633 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    48256 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/data_ops.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19395 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_pairing.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3169 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_subsampling.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8898 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    14694 2024-03-07 11:29:35.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process_multimer.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11218 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/protein.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40939 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/residue_constants.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4177 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/data/utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    24281 2024-03-07 12:08:05.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    20784 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset_inference.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10430 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/homo_search.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9126 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/inference.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7587 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/inference_symmetry.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9457 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/loss.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.864779 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2023-11-23 12:19:01.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9122 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/auxillary.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7332 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/chain_align.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5179 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/fape.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    13287 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/geometry.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      723 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17784 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/violation.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1367 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/model.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.945772 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      118 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    16455 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/alphafold.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    12363 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/attentions.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5316 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/auxillary_heads.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10489 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/common.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5573 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/confidence.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8923 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/embedders.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11196 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/evoformer.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6428 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/featurization.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1822 2023-11-23 12:23:14.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/flash_attention.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17109 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/frame.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    18180 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/structure_module.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9593 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/template.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5518 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/triangle_multiplication.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.994772 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       45 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17687 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/mmcif.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3130 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/msa_identifiers.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    23274 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/parsers.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11235 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/pipeline.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    44767 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/templates.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2681 2023-11-23 12:23:17.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/utils.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.062766 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      842 2023-11-23 12:23:20.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4276 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/assemble.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      910 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/config.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2065 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/dataset.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6782 2023-11-23 12:23:23.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/geometry_utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       23 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/loss.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10094 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/model.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7246 2023-11-23 12:23:22.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/modules.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2523 2023-11-23 12:23:23.000000 alphapulldown-2.0.0b1/AlphaLink2/unifold/task.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.553800 alphapulldown-2.0.0b1/ColabFold/
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.122766 alphapulldown-2.0.0b1/ColabFold/colabfold/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-03-08 10:44:51.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    82218 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/batch.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7301 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/citations.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    28656 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/colabfold.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5308 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/download.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2120 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/pdb.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5392 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/plot.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3139 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/relax.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10468 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b1/ColabFold/colabfold/utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    35149 2022-08-09 10:02:13.000000 alphapulldown-2.0.0b1/LICENSE
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       34 2023-11-15 13:03:52.000000 alphapulldown-2.0.0b1/MANIFEST.in
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7244 2024-04-09 14:04:55.947719 alphapulldown-2.0.0b1/PKG-INFO
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6235 2024-04-05 14:09:33.000000 alphapulldown-2.0.0b1/README.md
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.844742 alphapulldown-2.0.0b1/alphafold/
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.189763 alphapulldown-2.0.0b1/alphafold/alphafold/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      663 2023-05-16 14:00:32.000000 alphapulldown-2.0.0b1/alphafold/alphafold/__init__.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.227760 alphapulldown-2.0.0b1/alphafold/alphafold/common/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      655 2023-05-16 14:00:32.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7973 2024-03-01 11:31:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1434 2024-03-01 11:31:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7561 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/mmcif_metadata.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    22147 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/protein.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5791 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/protein_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    35625 2024-03-01 11:31:47.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9256 2023-05-16 14:00:33.000000 alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants_test.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.265762 alphapulldown-2.0.0b1/alphafold/alphafold/data/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      634 2023-05-16 14:00:34.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8575 2024-04-02 11:51:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/feature_processing.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    14182 2024-03-01 11:03:59.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/mmcif_parsing.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3122 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_identifiers.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17203 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_pairing.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    21397 2023-05-16 14:00:35.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/parsers.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10419 2024-03-01 11:03:59.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11126 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline_multimer.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40791 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/templates.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.299756 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      639 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5504 2024-03-01 11:04:00.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhblits.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3601 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhsearch.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4576 2023-12-19 15:12:27.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4556 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8386 2024-03-01 11:04:00.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3387 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/kalign.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1223 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/utils.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.428756 alphapulldown-2.0.0b1/alphafold/alphafold/model/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      617 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    47028 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40145 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_multimer.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4706 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5957 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/common_modules.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    26814 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/config.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1097 2023-05-16 14:00:39.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/data.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3795 2024-03-27 11:08:31.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/features.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    37264 2023-05-16 14:00:39.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/folding.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    42494 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/folding_multimer.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.490743 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1172 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4148 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5751 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7745 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4166 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/test_utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      853 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6896 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/vector.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9134 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10315 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3505 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2384 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7963 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/mapping.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6613 2024-03-29 15:44:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/model.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    74087 2024-03-01 11:33:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/modules.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    42351 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/modules_multimer.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1978 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/prng.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1202 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/prng_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17388 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5038 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10935 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/r3.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.553752 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      633 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    21489 2024-03-27 11:00:48.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/data_transforms.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5357 2024-03-27 11:04:53.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5051 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1822 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6344 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1415 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1318 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      812 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1276 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5448 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/model/utils.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.590739 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      626 2023-05-16 14:00:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6628 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9273 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.641764 alphapulldown-2.0.0b1/alphafold/alphafold/relax/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      618 2023-05-16 14:00:45.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19096 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4348 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4820 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6164 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3288 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3827 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2501 2023-10-26 14:36:43.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1996 2023-05-16 14:00:48.000000 alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils_test.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19606 2023-06-06 10:25:24.000000 alphapulldown-2.0.0b1/alphafold/alphafold/run_alphafold.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      674 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b1/alphafold/alphafold/version.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    22575 2024-03-01 11:31:54.000000 alphapulldown-2.0.0b1/alphafold/run_alphafold.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.660742 alphapulldown-2.0.0b1/alphapulldown/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       24 2024-04-09 13:56:06.000000 alphapulldown-2.0.0b1/alphapulldown/__init__.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.686738 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8145 2024-04-05 14:23:20.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2_3dmol.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:54.579793 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.700736 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3745 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11001 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       21 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/version.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7544 2023-11-21 13:30:28.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/calculate_mpdockq.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6588 2024-04-05 14:09:34.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/create_notebook.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7190 2024-04-09 14:01:52.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/get_good_inter_pae.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3891 2024-01-04 12:01:24.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/test_create_notebook.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1078 2024-04-05 14:09:35.000000 alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/utils.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.738734 alphapulldown-2.0.0b1/alphapulldown/folding_backend/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2820 2024-04-05 14:23:20.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    25303 2024-04-05 14:29:45.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/alphafold_backend.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3320 2024-04-05 14:29:39.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/alphalink_backend.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2302 2024-04-05 14:23:21.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/folding_backend.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3570 2024-04-05 14:23:21.000000 alphapulldown-2.0.0b1/alphapulldown/folding_backend/unifold_backend.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    28295 2024-04-09 14:01:53.000000 alphapulldown-2.0.0b1/alphapulldown/objects.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.890725 alphapulldown-2.0.0b1/alphapulldown/package_data/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9119 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b1/alphapulldown/package_data/stereo_chemical_props.txt
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    12618 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b1/alphapulldown/predict_structure.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.782763 alphapulldown-2.0.0b1/alphapulldown/scripts/
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)    48825 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/convert_to_modelcif.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    15939 2024-04-09 14:01:54.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/create_individual_features.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1276 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/generate_crosslink_pickle.py
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1166 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/prepare_seq_names.py
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1240 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/rename_colab_search_a3m.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8881 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/run_multimer_jobs.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11865 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b1/alphapulldown/scripts/run_structure_prediction.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3038 2024-03-12 10:27:02.000000 alphapulldown-2.0.0b1/alphapulldown/test_new_mmt.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.839764 alphapulldown-2.0.0b1/alphapulldown/utils/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-04-05 14:23:24.000000 alphapulldown-2.0.0b1/alphapulldown/utils/__init__.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4400 2024-04-05 14:23:24.000000 alphapulldown-2.0.0b1/alphapulldown/utils/calculate_rmsd.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1838 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/create_combinations.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7919 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/create_custom_template_db.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4897 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/file_handling.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17488 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/modelling_setup.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7019 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/multimeric_template_utils.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1100 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b1/alphapulldown/utils/plotting.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1447 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b1/alphapulldown/utils/post_modelling.py
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)    15228 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b1/alphapulldown/utils/remove_clashes_low_plddt.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7884 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b1/alphapulldown/utils/save_meta_data.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.943731 alphapulldown-2.0.0b1/alphapulldown.egg-info/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7244 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/PKG-INFO
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8555 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/SOURCES.txt
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)        1 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/dependency_links.txt
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)      271 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/requires.txt
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)       69 2024-04-09 14:04:54.000000 alphapulldown-2.0.0b1/alphapulldown.egg-info/top_level.txt
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2357 2024-04-09 14:04:55.997715 alphapulldown-2.0.0b1/setup.cfg
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)      124 2023-11-15 13:03:57.000000 alphapulldown-2.0.0b1/setup.py
-drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-09 14:04:55.940720 alphapulldown-2.0.0b1/test/
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1043 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_alphalink2_folding_backend.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8545 2024-04-05 14:09:40.000000 alphapulldown-2.0.0b1/test/test_create_monomeric_objects.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1332 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_create_multimeric_objects.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2830 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_create_multimeric_template_features.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2845 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b1/test/test_crosslink_inference.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2215 2023-11-14 10:55:56.000000 alphapulldown-2.0.0b1/test/test_crosslink_input.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3071 2024-04-05 14:23:33.000000 alphapulldown-2.0.0b1/test/test_custom_db.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3621 2024-04-05 14:09:46.000000 alphapulldown-2.0.0b1/test/test_features.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8145 2024-04-05 14:23:33.000000 alphapulldown-2.0.0b1/test/test_features_with_templates.py
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)      712 2023-11-15 13:06:08.000000 alphapulldown-2.0.0b1/test/test_predictions_slurm.py
--rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1726 2024-04-05 14:23:34.000000 alphapulldown-2.0.0b1/test/test_python_imports.py
--rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1494 2024-04-05 14:23:34.000000 alphapulldown-2.0.0b1/test/test_remove_clashes_low_plddt.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.441599 alphapulldown-2.0.0b2/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:33.925687 alphapulldown-2.0.0b2/AlphaLink2/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.231673 alphapulldown-2.0.0b2/AlphaLink2/unifold/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       72 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10975 2024-03-18 14:19:42.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/alphalink_inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    29224 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/config.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.361688 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      633 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    48256 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/data_ops.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19395 2023-11-23 12:22:57.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/msa_pairing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3169 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/msa_subsampling.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8898 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/process.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    14694 2024-03-07 11:29:35.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/process_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11218 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/protein.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40939 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/residue_constants.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4177 2023-11-23 12:22:58.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/data/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    24281 2024-03-07 12:08:05.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/dataset.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    20784 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/dataset_inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10430 2023-11-23 12:23:02.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/homo_search.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9126 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/inference.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7587 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/inference_symmetry.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9457 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/loss.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.401683 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2023-11-23 12:19:01.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9122 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/auxillary.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7332 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/chain_align.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5179 2023-11-23 12:23:03.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/fape.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    13287 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/geometry.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      723 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17784 2023-11-23 12:23:04.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/violation.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1367 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/model.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.454671 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      118 2023-11-23 12:23:07.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    16455 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/alphafold.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    12363 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/attentions.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5316 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/auxillary_heads.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10489 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/common.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5573 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/confidence.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8923 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/embedders.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11196 2023-11-23 12:23:08.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/evoformer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6428 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/featurization.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1822 2023-11-23 12:23:14.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/flash_attention.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17109 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/frame.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    18180 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/structure_module.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9593 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/template.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5518 2023-11-23 12:23:09.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/triangle_multiplication.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.488664 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       45 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17687 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/mmcif.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3130 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/msa_identifiers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    23274 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/parsers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11235 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/pipeline.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    44767 2023-11-23 12:23:15.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/templates.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2681 2023-11-23 12:23:17.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.538652 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      842 2023-11-23 12:23:20.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4276 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/assemble.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      910 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/config.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2065 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/dataset.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6782 2023-11-23 12:23:23.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/geometry_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       23 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/loss.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10094 2023-11-23 12:23:21.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/model.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7246 2023-11-23 12:23:22.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/modules.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2523 2023-11-23 12:23:23.000000 alphapulldown-2.0.0b2/AlphaLink2/unifold/task.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:33.931697 alphapulldown-2.0.0b2/ColabFold/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.566653 alphapulldown-2.0.0b2/ColabFold/colabfold/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-03-08 10:44:51.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    82218 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/batch.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7301 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/citations.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    28656 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/colabfold.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5308 2024-03-08 10:44:52.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/download.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2120 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/pdb.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5392 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/plot.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3139 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/relax.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10468 2024-03-08 10:44:54.000000 alphapulldown-2.0.0b2/ColabFold/colabfold/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    35149 2022-08-09 10:02:13.000000 alphapulldown-2.0.0b2/LICENSE
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       34 2023-11-15 13:03:52.000000 alphapulldown-2.0.0b2/MANIFEST.in
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7315 2024-04-19 12:40:35.395602 alphapulldown-2.0.0b2/PKG-INFO
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6306 2024-04-10 10:01:29.000000 alphapulldown-2.0.0b2/README.md
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.258619 alphapulldown-2.0.0b2/alphafold/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.594664 alphapulldown-2.0.0b2/alphafold/alphafold/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      663 2023-05-16 14:00:32.000000 alphapulldown-2.0.0b2/alphafold/alphafold/__init__.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.630652 alphapulldown-2.0.0b2/alphafold/alphafold/common/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      655 2023-05-16 14:00:32.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7973 2024-03-01 11:31:45.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/confidence.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1434 2024-03-01 11:31:45.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/confidence_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7561 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/mmcif_metadata.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    22147 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/protein.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5791 2024-03-01 11:31:46.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/protein_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    35625 2024-03-01 11:31:47.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/residue_constants.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9256 2023-05-16 14:00:33.000000 alphapulldown-2.0.0b2/alphafold/alphafold/common/residue_constants_test.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.673647 alphapulldown-2.0.0b2/alphafold/alphafold/data/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      634 2023-05-16 14:00:34.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8575 2024-04-02 11:51:51.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/feature_processing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    14182 2024-03-01 11:03:59.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3122 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/msa_identifiers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17203 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/msa_pairing.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    21397 2023-05-16 14:00:35.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/parsers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10419 2024-03-01 11:03:59.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/pipeline.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11126 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40791 2024-03-01 11:31:49.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/templates.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.757661 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      639 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5504 2024-03-01 11:04:00.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hhblits.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3601 2023-05-16 14:00:36.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4576 2023-12-19 15:12:27.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4556 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8386 2024-03-01 11:04:00.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3387 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/kalign.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1223 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.882668 alphapulldown-2.0.0b2/alphafold/alphafold/model/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      617 2023-05-16 14:00:37.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    47028 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/all_atom.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    40145 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4706 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/all_atom_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5957 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/common_modules.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    26814 2023-05-16 14:00:38.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/config.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1097 2023-05-16 14:00:39.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/data.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3795 2024-03-27 11:08:31.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    37264 2023-05-16 14:00:39.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/folding.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    42494 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/folding_multimer.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.923641 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1172 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4148 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5751 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7745 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4166 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      853 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6896 2023-05-16 14:00:40.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/vector.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9134 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/layer_stack.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10315 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/layer_stack_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3505 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/lddt.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2384 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/lddt_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7963 2023-05-16 14:00:41.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/mapping.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6797 2024-04-16 15:36:01.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/model.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    74087 2024-03-01 11:33:45.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/modules.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    42351 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/modules_multimer.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1978 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/prng.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1202 2024-03-01 11:31:50.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/prng_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17388 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/quat_affine.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5038 2023-05-16 14:00:42.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/quat_affine_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10935 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/r3.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.967627 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      633 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    21489 2024-03-27 11:00:48.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5357 2024-03-27 11:04:53.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5051 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/protein_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1822 2023-05-16 14:00:43.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6344 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1415 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1318 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      812 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1276 2023-05-16 14:00:44.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5448 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b2/alphafold/alphafold/model/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:34.985628 alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      626 2023-05-16 14:00:45.000000 alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6628 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9273 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.072717 alphapulldown-2.0.0b2/alphafold/alphafold/relax/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      618 2023-05-16 14:00:45.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19096 2024-03-01 11:31:51.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/amber_minimize.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4348 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4820 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/cleanup.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6164 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/cleanup_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3288 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/relax.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3827 2023-05-16 14:00:46.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/relax_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2501 2023-10-26 14:36:43.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1996 2023-05-16 14:00:48.000000 alphapulldown-2.0.0b2/alphafold/alphafold/relax/utils_test.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    19606 2023-06-06 10:25:24.000000 alphapulldown-2.0.0b2/alphafold/alphafold/run_alphafold.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      674 2024-03-01 11:31:52.000000 alphapulldown-2.0.0b2/alphafold/alphafold/version.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    22575 2024-03-01 11:31:54.000000 alphapulldown-2.0.0b2/alphafold/run_alphafold.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.103618 alphapulldown-2.0.0b2/alphapulldown/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       24 2024-04-19 12:38:03.000000 alphapulldown-2.0.0b2/alphapulldown/__init__.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.155639 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8145 2024-04-05 14:23:20.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2_3dmol.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:33.987683 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.174616 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/af2plots/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3745 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11001 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       21 2023-08-29 10:45:59.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/af2plots/version.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7544 2023-11-21 13:30:28.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/calculate_mpdockq.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     6588 2024-04-05 14:09:34.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/create_notebook.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     6321 2024-04-19 11:29:47.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/get_good_inter_pae.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    11298 2024-04-16 10:06:58.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/pdb_analyser.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3891 2024-01-04 12:01:24.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/test_create_notebook.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1151 2024-04-13 11:38:08.000000 alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/utils.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.187623 alphapulldown-2.0.0b2/alphapulldown/folding_backend/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2820 2024-04-05 14:23:20.000000 alphapulldown-2.0.0b2/alphapulldown/folding_backend/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    29673 2024-04-19 11:03:55.000000 alphapulldown-2.0.0b2/alphapulldown/folding_backend/alphafold_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3320 2024-04-05 14:29:39.000000 alphapulldown-2.0.0b2/alphapulldown/folding_backend/alphalink_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2302 2024-04-05 14:23:21.000000 alphapulldown-2.0.0b2/alphapulldown/folding_backend/folding_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3570 2024-04-10 12:57:39.000000 alphapulldown-2.0.0b2/alphapulldown/folding_backend/unifold_backend.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    28323 2024-04-17 11:54:35.000000 alphapulldown-2.0.0b2/alphapulldown/objects.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.365605 alphapulldown-2.0.0b2/alphapulldown/package_data/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     9119 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b2/alphapulldown/package_data/stereo_chemical_props.txt
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.206619 alphapulldown-2.0.0b2/alphapulldown/scripts/
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)    48825 2024-04-05 14:23:22.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/convert_to_modelcif.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    15939 2024-04-09 14:01:54.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/create_individual_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1276 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/generate_crosslink_pickle.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1166 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/prepare_seq_names.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1240 2024-04-05 14:23:23.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/rename_colab_search_a3m.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     5959 2024-04-19 11:03:23.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/run_multimer_jobs.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    10730 2024-04-19 11:03:03.000000 alphapulldown-2.0.0b2/alphapulldown/scripts/run_structure_prediction.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 10:48:36.000000 alphapulldown-2.0.0b2/alphapulldown/test_import_flags.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      458 2024-04-19 10:49:22.000000 alphapulldown-2.0.0b2/alphapulldown/test_model_relax.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.255610 alphapulldown-2.0.0b2/alphapulldown/utils/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        0 2024-04-05 14:23:24.000000 alphapulldown-2.0.0b2/alphapulldown/utils/__init__.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4400 2024-04-05 14:23:24.000000 alphapulldown-2.0.0b2/alphapulldown/utils/calculate_rmsd.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1838 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b2/alphapulldown/utils/create_combinations.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7905 2024-04-17 11:54:35.000000 alphapulldown-2.0.0b2/alphapulldown/utils/create_custom_template_db.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     4899 2024-04-17 11:54:35.000000 alphapulldown-2.0.0b2/alphapulldown/utils/file_handling.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)    17340 2024-04-17 11:54:35.000000 alphapulldown-2.0.0b2/alphapulldown/utils/modelling_setup.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7019 2024-04-05 14:23:25.000000 alphapulldown-2.0.0b2/alphapulldown/utils/multimeric_template_utils.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1124 2024-04-15 12:32:06.000000 alphapulldown-2.0.0b2/alphapulldown/utils/plotting.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1585 2024-04-19 11:04:35.000000 alphapulldown-2.0.0b2/alphapulldown/utils/post_modelling.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)    15228 2024-04-05 14:23:26.000000 alphapulldown-2.0.0b2/alphapulldown/utils/remove_clashes_low_plddt.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7864 2024-04-17 11:54:36.000000 alphapulldown-2.0.0b2/alphapulldown/utils/save_meta_data.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.392611 alphapulldown-2.0.0b2/alphapulldown.egg-info/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7315 2024-04-19 12:40:33.000000 alphapulldown-2.0.0b2/alphapulldown.egg-info/PKG-INFO
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8535 2024-04-19 12:40:33.000000 alphapulldown-2.0.0b2/alphapulldown.egg-info/SOURCES.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)        1 2024-04-19 12:40:33.000000 alphapulldown-2.0.0b2/alphapulldown.egg-info/dependency_links.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)      271 2024-04-19 12:40:33.000000 alphapulldown-2.0.0b2/alphapulldown.egg-info/requires.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)       69 2024-04-19 12:40:33.000000 alphapulldown-2.0.0b2/alphapulldown.egg-info/top_level.txt
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2357 2024-04-19 12:40:35.444600 alphapulldown-2.0.0b2/setup.cfg
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)      124 2023-11-15 13:03:57.000000 alphapulldown-2.0.0b2/setup.py
+drwxr-xr-x   0 dingquanyu (24600) kosinski   (721)        0 2024-04-19 12:40:35.390608 alphapulldown-2.0.0b2/test/
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8606 2024-04-17 11:54:37.000000 alphapulldown-2.0.0b2/test/test_create_monomeric_objects.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1332 2024-04-05 14:23:32.000000 alphapulldown-2.0.0b2/test/test_create_multimeric_objects.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     2762 2024-04-17 11:54:37.000000 alphapulldown-2.0.0b2/test/test_create_multimeric_template_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3071 2024-04-05 14:23:33.000000 alphapulldown-2.0.0b2/test/test_custom_db.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     3615 2024-04-17 11:54:37.000000 alphapulldown-2.0.0b2/test/test_features.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     8145 2024-04-05 14:23:33.000000 alphapulldown-2.0.0b2/test/test_features_with_templates.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     7371 2024-04-17 11:54:37.000000 alphapulldown-2.0.0b2/test/test_postprocessing.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1791 2024-04-17 11:54:37.000000 alphapulldown-2.0.0b2/test/test_predictions_slurm.py
+-rw-r--r--   0 dingquanyu (24600) kosinski   (721)     1668 2024-04-17 11:54:38.000000 alphapulldown-2.0.0b2/test/test_python_imports.py
+-rwxr-xr-x   0 dingquanyu (24600) kosinski   (721)     1494 2024-04-05 14:23:34.000000 alphapulldown-2.0.0b2/test/test_remove_clashes_low_plddt.py
```

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/alphalink_inference.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/alphalink_inference.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/config.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/__init__.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/data_ops.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/data_ops.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_pairing.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/msa_subsampling.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/msa_subsampling.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/process.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/process_multimer.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/process_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/protein.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/residue_constants.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/data/utils.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/data/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/dataset_inference.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/dataset_inference.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/homo_search.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/homo_search.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/inference.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/inference.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/inference_symmetry.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/inference_symmetry.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/loss.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/loss.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/auxillary.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/auxillary.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/chain_align.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/chain_align.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/fape.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/fape.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/geometry.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/geometry.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/utils.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/losses/violation.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/losses/violation.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/model.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/alphafold.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/attentions.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/auxillary_heads.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/auxillary_heads.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/common.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/common.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/confidence.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/embedders.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/embedders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/evoformer.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/evoformer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/featurization.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/featurization.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/flash_attention.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/flash_attention.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/frame.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/frame.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/structure_module.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/structure_module.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/template.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/template.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/modules/triangle_multiplication.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/modules/triangle_multiplication.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/mmcif.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/mmcif.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/msa_identifiers.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/parsers.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/pipeline.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/templates.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/msa/utils.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/msa/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/__init__.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/assemble.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/assemble.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/config.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/dataset.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/geometry_utils.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/model.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/symmetry/modules.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/symmetry/modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/AlphaLink2/unifold/task.py` & `alphapulldown-2.0.0b2/AlphaLink2/unifold/task.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/batch.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/batch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/citations.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/citations.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/colabfold.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/colabfold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/download.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/download.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/pdb.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/pdb.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/plot.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/plot.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/relax.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/ColabFold/colabfold/utils.py` & `alphapulldown-2.0.0b2/ColabFold/colabfold/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/LICENSE` & `alphapulldown-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/PKG-INFO` & `alphapulldown-2.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphapulldown
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Pipeline allows massive screening using alphafold
 Home-page: https://github.com/KosinskiLab/AlphaPulldown
 Author: Dingquan Yu
 Author-email: dingquan.yu@embl-hamburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,26 +29,27 @@
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: jupyterlab
 Requires-Dist: ipywidgets
 
 # AlphaPulldown
 [![Downloads](https://static.pepy.tech/badge/alphapulldown)](https://pepy.tech/project/alphapulldown)  [![python3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) ![GPL3 license](https://img.shields.io/badge/license-GPLv3-green)
 
-## 🥳 AlphaPulldown has entered the era of version 1.x
+## 🥳 AlphaPulldown has entered the era of version 2.0 (beta)
 We have brought some exciting useful features to AlphaPulldown and updated its computing environment. 
 
 
 AlphaPulldown is a Python package that streamlines protein-protein interaction screens and high-throughput modelling of higher-order oligomers using AlphaFold-Multimer:
 * provides a convenient command line interface to screen a bait protein against many candidates, calculate all-versus-all pairwise comparisons, test alternative homo-oligomeric states, and model various parts of a larger complex
 * separates the CPU stages (MSA and template feature generation) from GPU stages (the actual modeling)
 * allows modeling fragments of proteins without recalculation of MSAs and keeping the original full-length residue numbering in the models
 * summarizes the results in a CSV table with AlphaFold scores, pDockQ and mpDockQ, PI-score, and various physical parameters of the interface
 * provides a Jupyter notebook for an interactive analysis of PAE plots and models
+* 🆕 refactorised codes and removed redundancy
+* 🆕 added a new way of integrating experimental models into AlphaFold pipeline using custom multimeric databases
 * 🆕 integrates cross-link mass spec data with AlphaFold predictions via [AlphaLink2](https://github.com/Rappsilber-Laboratory/AlphaLink2/tree/main) models
-* 🆕 able to integrate experimental models into AlphaFold pipeline using custom multimeric databases
 
 ## Pre-installation
 Check if you have downloaded necessary parameters and databases (e.g. BFD, MGnify etc.) as instructed in [AlphFold's documentation](https://github.com/deepmind/alphafold). You should have a directory like below:
  ```
  alphafold_database/                             # Total: ~ 2.2 TB (download: 438 GB)
     bfd/                                   # ~ 1.7 TB (download: 271.6 GB)
         # 6 files.
@@ -94,15 +95,15 @@
 
 ## Installation using pip
 
 Activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 
-python3 -m pip install alphapulldown==1.0.4
+python3 -m pip install alphapulldown==2.0.0b1
 pip install jax==0.4.23 jaxlib==0.4.23+cuda11.cudnn86 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **For older versions of AlphaFold**: 
 If you haven't updated your databases according to the requirements of AlphaFold 2.3.0, you can still use AlphaPulldown with your older version of AlphaFold database. Please follow the installation instructions on the [dedicated branch](https://github.com/KosinskiLab/AlphaPulldown/tree/AlphaFold-2.2.0)
 
 ## How to develop
```

### Comparing `alphapulldown-2.0.0b1/README.md` & `alphapulldown-2.0.0b2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # AlphaPulldown
 [![Downloads](https://static.pepy.tech/badge/alphapulldown)](https://pepy.tech/project/alphapulldown)  [![python3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) ![GPL3 license](https://img.shields.io/badge/license-GPLv3-green)
 
-## 🥳 AlphaPulldown has entered the era of version 1.x
+## 🥳 AlphaPulldown has entered the era of version 2.0 (beta)
 We have brought some exciting useful features to AlphaPulldown and updated its computing environment. 
 
 
 AlphaPulldown is a Python package that streamlines protein-protein interaction screens and high-throughput modelling of higher-order oligomers using AlphaFold-Multimer:
 * provides a convenient command line interface to screen a bait protein against many candidates, calculate all-versus-all pairwise comparisons, test alternative homo-oligomeric states, and model various parts of a larger complex
 * separates the CPU stages (MSA and template feature generation) from GPU stages (the actual modeling)
 * allows modeling fragments of proteins without recalculation of MSAs and keeping the original full-length residue numbering in the models
 * summarizes the results in a CSV table with AlphaFold scores, pDockQ and mpDockQ, PI-score, and various physical parameters of the interface
 * provides a Jupyter notebook for an interactive analysis of PAE plots and models
+* 🆕 refactorised codes and removed redundancy
+* 🆕 added a new way of integrating experimental models into AlphaFold pipeline using custom multimeric databases
 * 🆕 integrates cross-link mass spec data with AlphaFold predictions via [AlphaLink2](https://github.com/Rappsilber-Laboratory/AlphaLink2/tree/main) models
-* 🆕 able to integrate experimental models into AlphaFold pipeline using custom multimeric databases
 
 ## Pre-installation
 Check if you have downloaded necessary parameters and databases (e.g. BFD, MGnify etc.) as instructed in [AlphFold's documentation](https://github.com/deepmind/alphafold). You should have a directory like below:
  ```
  alphafold_database/                             # Total: ~ 2.2 TB (download: 438 GB)
     bfd/                                   # ~ 1.7 TB (download: 271.6 GB)
         # 6 files.
@@ -62,15 +63,15 @@
 
 ## Installation using pip
 
 Activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 
-python3 -m pip install alphapulldown==1.0.4
+python3 -m pip install alphapulldown==2.0.0b1
 pip install jax==0.4.23 jaxlib==0.4.23+cuda11.cudnn86 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **For older versions of AlphaFold**: 
 If you haven't updated your databases according to the requirements of AlphaFold 2.3.0, you can still use AlphaPulldown with your older version of AlphaFold database. Please follow the installation instructions on the [dedicated branch](https://github.com/KosinskiLab/AlphaPulldown/tree/AlphaFold-2.2.0)
 
 ## How to develop
```

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/confidence_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/confidence_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/mmcif_metadata.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/mmcif_metadata.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/protein.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/protein_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/protein_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/common/residue_constants_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/common/residue_constants_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/feature_processing.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/feature_processing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/mmcif_parsing.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/mmcif_parsing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_identifiers.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/msa_pairing.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/parsers.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/pipeline_multimer.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/pipeline_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/templates.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhblits.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hhblits.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hhsearch.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hhsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmbuild.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hmmbuild.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/hmmsearch.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/hmmsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/jackhmmer.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/jackhmmer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/kalign.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/kalign.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/data/tools/utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/data/tools/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/all_atom.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_multimer.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/all_atom_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/all_atom_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/all_atom_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/common_modules.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/common_modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/config.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/data.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/data.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/features.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/folding.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/folding.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/folding_multimer.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/folding_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rigid_matrix_vector.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/rigid_matrix_vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/rotation_matrix.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/struct_of_array.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/struct_of_array.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/test_utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/test_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/geometry/vector.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/layer_stack.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/layer_stack_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/lddt.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/lddt_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/lddt_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/mapping.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/mapping.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/model.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,17 +161,20 @@
     Returns:
       A dictionary of model outputs.
     """
     self.init_params(feat)
     logging.info('Running predict with shape(feat) = %s',
                  tree.map_structure(lambda x: x.shape, feat))
     result = self.apply(self.params, jax.random.PRNGKey(random_seed), feat)
-
+    logging.info(f"PAE has keys: {result['predicted_aligned_error'].keys()}")
     # This block is to ensure benchmark timings are accurate. Some blocking is
     # already happening when computing get_confidence_metrics, and this ensures
     # all outputs are blocked on.
     jax.tree_map(lambda x: x.block_until_ready(), result)
-    result.update(
-        get_confidence_metrics(result, multimer_mode=self.multimer_mode))
+    # result.update(
+        # get_confidence_metrics(result, multimer_mode=self.multimer_mode))
+    result.update({"plddt": confidence.compute_plddt(
+      result['predicted_lddt']['logits'])})
+    
     logging.info('Output shape was %s',
                  tree.map_structure(lambda x: x.shape, result))
     return result
```

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/modules.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/modules_multimer.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/modules_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/prng.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/prng.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/prng_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/prng_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/quat_affine.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/quat_affine_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/quat_affine_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/r3.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/r3.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/data_transforms.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/data_transforms.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/input_pipeline.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/protein_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/protein_features_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/protein_features_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/proteins_dataset.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/proteins_dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/shape_helpers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_helpers_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/shape_helpers_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/shape_placeholders.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/shape_placeholders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/tf/utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/tf/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/model/utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/model/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/notebooks/notebook_utils_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/notebooks/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/__init__.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/amber_minimize.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/amber_minimize_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/amber_minimize_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/cleanup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/cleanup_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/cleanup_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/relax_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/relax_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/relax/utils_test.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/relax/utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/run_alphafold.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/alphafold/version.py` & `alphapulldown-2.0.0b2/alphafold/alphafold/version.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphafold/run_alphafold.py` & `alphapulldown-2.0.0b2/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2_3dmol.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2_3dmol.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/calculate_mpdockq.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/calculate_mpdockq.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/create_notebook.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/test_create_notebook.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/test_create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/analysis_pipeline/utils.py` & `alphapulldown-2.0.0b2/alphapulldown/analysis_pipeline/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from configparser import Interpolation
 import IPython.display as display
 import ipywidgets as widgets
 import matplotlib.pyplot as plt
 import matplotlib.image as mpimg
 import os
 import re
+import pandas as pd
+from absl import logging
+import subprocess
+import sys
 #from analysis_pipeline.af2hyde_mod import plot_predicted_alignment_error
 from af2plots.plotter import plotter
 
 
 def display_pae_plots(subdir,figsize=(50, 50)):
     """A function to display all the pae plots in the subdir"""
     pattern = r"ranked_(\d+)\.png"
@@ -23,8 +27,8 @@
         #plt.show()
     else:
         #plot_predicted_alignment_error(subdir)
         af2o = plotter()
         dd = af2o.parse_model_pickles(subdir)
         ff = af2o.plot_predicted_alignment_error(dd)
 
-    plt.show()
+    plt.show()
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/folding_backend/__init__.py` & `alphapulldown-2.0.0b2/alphapulldown/folding_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/folding_backend/alphafold_backend.py` & `alphapulldown-2.0.0b2/alphapulldown/folding_backend/alphafold_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,40 +5,49 @@
     Author: Valentin Maurer <valentin.maurer@embl-hamburg.de>
             Dmitry Molodenskiy <dmitry.molodenskiy@embl-hamburg.de> 
             Dingquan Yu <dingquan.yu@embl-hamburg.de>
 """
 import time
 import json
 import pickle
-import tempfile
-from typing import Dict, Union, List
-from os.path import join, exists
+import subprocess
+import enum
+from typing import Dict, Union, List, Any
+import os
 from absl import logging
 import numpy as np
+from copy import copy
 import jax.numpy as jnp
 from alphapulldown.utils.plotting import plot_pae_from_matrix
 from alphapulldown.objects import MultimericObject, MonomericObject, ChoppedObject
 from alphapulldown.utils.post_modelling import post_prediction_process
-from alphapulldown.utils.calculate_rmsd import calculate_rmsd_and_superpose
+#from alphapulldown.utils.calculate_rmsd import calculate_rmsd_and_superpose
 from alphapulldown.utils.modelling_setup import pad_input_features
-# Avoid module not found error by importing after AP
-from run_alphafold import ModelsToRelax
 from alphafold.relax import relax
 from alphafold.common import protein, residue_constants, confidence
 from .folding_backend import FoldingBackend
 logging.set_verbosity(logging.INFO)
 
+
+# Relaxation parameters.
 MAX_TEMPLATE_HITS = 20
 RELAX_MAX_ITERATIONS = 0
 RELAX_ENERGY_TOLERANCE = 2.39
 RELAX_STIFFNESS = 10.0
 RELAX_EXCLUDE_RESIDUES = []
 RELAX_MAX_OUTER_ITERATIONS = 3
 
 
+@enum.unique
+class ModelsToRelax(enum.Enum):
+  ALL = 0
+  BEST = 1
+  NONE = 2
+
+
 def _jnp_to_np(output):
     """Recursively changes jax arrays to numpy arrays."""
     for k, v in output.items():
         if isinstance(v, dict):
             output[k] = _jnp_to_np(v)
         elif isinstance(v, jnp.ndarray):
             output[k] = np.array(v)
@@ -52,37 +61,37 @@
     Args:
     pae: The n_res x n_res PAE array.
     max_pae: The maximum possible PAE value.
     output_dir: Directory to which files are saved.
     model_name: Name of a model.
     """
     pae_json = confidence.pae_json(pae, max_pae)
-    pae_json_output_path = join(output_dir, f'pae_{model_name}.json')
+    pae_json_output_path = os.path.join(output_dir, f'pae_{model_name}.json')
     with open(pae_json_output_path, 'w') as f:
         f.write(pae_json)
 
 
 def _save_confidence_json_file(plddt: np.ndarray, output_dir: str, model_name: str) -> None:
     """
     Check prediction result for confidence data and save to a JSON file if present.
     Args:
         plddt: The n_res x 1 pLDDT array.
         output_dir: Directory to which files are saved.
         model_name: Name of a model.
     """
     confidence_json = confidence.confidence_json(plddt)
-    confidence_json_output_path = join(
+    confidence_json_output_path = os.path.join(
         output_dir, f'confidence_{model_name}.json')
     with open(confidence_json_output_path, 'w') as f:
         f.write(confidence_json)
 
 
 def _read_from_json_if_exists(json_path: str) -> Dict:
     """Reads a JSON file or creates it with default data if it does not exist."""
-    if exists(json_path):
+    if os.path.exists(json_path):
         with open(json_path, "r") as f:
             data = json.load(f)
     else:
         data = {}
     return data
 
 
@@ -272,53 +281,53 @@
             If multimeric mode is enabled but no valid templates are found.
         ValueError
             If multimeric mode and skip templates are enabled at the same time
         """
         timings = {}
         prediction_results = {}
         START = 0
-        multimeric_mode = multimeric_object.multimeric_mode
+        multimeric_mode = multimeric_object.multimeric_mode if hasattr(multimeric_object, "multimeric_mode") else None
         t_0 = time.time()
-
+        original_feature_dict = copy(multimeric_object.feature_dict)
+        total_num_res = sum([len(s) for s in multimeric_object.input_seqs]) if hasattr(multimeric_object, "input_seqs") else len(multimeric_object.sequence)
         if allow_resume:
             logging.info(
-            f"Now runing predictions on {multimeric_object.description}. Checking existing results...")
+            f"Now running predictions on {multimeric_object.description}. Checking existing results...")
             for model_index, (model_name, model_runner) in enumerate(model_runners.items()):
-                unrelaxed_pdb_path = join(
+                unrelaxed_pdb_path = os.path.join(
                     output_dir, f"unrelaxed_{model_name}.pdb")
-                result_output_path = join(
+                result_output_path = os.path.join(
                     output_dir, f"result_{model_name}.pkl")
-                if exists(unrelaxed_pdb_path) and exists(result_output_path):
+                if os.path.exists(unrelaxed_pdb_path) and os.path.exists(result_output_path):
                     START = model_index + 1
                 else:
                     break
-
         # first check whether the desired num_res and num_msa are specified for padding
         desired_num_res, desired_num_msa = kwargs.get(
             "desired_num_res", None), kwargs.get("desired_num_msa", None)
-        if (desired_num_res is not None) and (desired_num_msa is not None):
+        if (desired_num_res is not None) and (desired_num_msa is not None) and type(multimeric_object) == MultimericObject:
             # This means padding is required to speed up the process
-            pad_input_features(feature_dict=multimeric_object.feature_dict,
+            pad_input_features(feature_dict=original_feature_dict,
                                desired_num_msa=desired_num_msa, desired_num_res=desired_num_res)
-            multimeric_object.feature_dict['num_alignments'] = np.array([desired_num_msa])
+            original_feature_dict['num_alignments'] = np.array([desired_num_msa])
         num_models = len(model_runners)
         for model_index, (model_name, model_runner) in enumerate(model_runners.items()):
             model_random_seed = model_index + random_seed * num_models
             processed_feature_dict = model_runner.process_features(
-                multimeric_object.feature_dict, random_seed=model_random_seed
+                original_feature_dict, random_seed=model_random_seed
             )
             # Read prediction results from results.pkl und unrelaxed.pdb
             if model_index < START:
-                result_output_path = join(
+                result_output_path = os.path.join(
                     output_dir, f"result_{model_name}.pkl")
                 with open(result_output_path, "rb") as f:
                     prediction_result = pickle.load(f)
                     # Update prediction_result with input seqs and unrelaxed protein
                     prediction_result.update(
-                        {"seqs": multimeric_object.input_seqs})
+                        {"seqs": multimeric_object.input_seqs if hasattr(multimeric_object,"input_seqs") else [multimeric_object.sequence]})
                     plddt_b_factors = np.repeat(
                         prediction_result['plddt'][:,
                                                    None], residue_constants.atom_type_num, axis=-1
                     )
                     unrelaxed_protein = protein.from_prediction(
                         features=processed_feature_dict,
                         result=prediction_result,
@@ -348,51 +357,52 @@
                         )
                 else:
                     raise ValueError(
                         "No template_all_atom_positions key found in processed_feature_dict."
                     )
             t_0 = time.time()
             logging.info(
-                f"Now runing predictions on {multimeric_object.description} using {model_name}")
+                f"Now running predictions on {multimeric_object.description} using {model_name}")
             prediction_result = model_runner.predict(
                 processed_feature_dict, random_seed=model_random_seed
             )
             t_diff = time.time() - t_0
             timings[f"predict_and_compile_{model_name}"] = t_diff
             logging.info(f"prediction costs : {t_diff} s")
 
             # Update prediction_result with input seqs and unrelaxed protein
-            prediction_result.update({"seqs": multimeric_object.input_seqs})
             plddt_b_factors = np.repeat(
                 prediction_result['plddt'][:,
                                            None], residue_constants.atom_type_num, axis=-1
             )
             unrelaxed_protein = protein.from_prediction(
                 features=processed_feature_dict,
                 result=prediction_result,
                 b_factors=plddt_b_factors,
                 remove_leading_feature_dimension=not model_runner.multimer_mode,
             )
 
             # Remove jax dependency from results
             np_prediction_result = _jnp_to_np(dict(prediction_result))
             # Save prediction results to pickle file
-            result_output_path = join(output_dir, f"result_{model_name}.pkl")
+            result_output_path = os.path.join(output_dir, f"result_{model_name}.pkl")
             with open(result_output_path, "wb") as f:
                 pickle.dump(np_prediction_result, f, protocol=4)
+            prediction_result.update(
+                        {"seqs": multimeric_object.input_seqs if hasattr(multimeric_object,"input_seqs") else [multimeric_object.sequence]})
             prediction_result.update({"unrelaxed_protein": unrelaxed_protein})
             prediction_results.update({model_name: prediction_result})
             # Save predictions to pdb files
-            unrelaxed_pdb_path = join(
+            unrelaxed_pdb_path = os.path.join(
                 output_dir, f"unrelaxed_{model_name}.pdb")
 
             with open(unrelaxed_pdb_path, "w") as f:
                 f.write(protein.to_pdb(unrelaxed_protein))
             # Save timings to json file
-            timings_output_path = join(output_dir, "timings.json")
+            timings_output_path = os.path.join(output_dir, "timings.json")
             with open(timings_output_path, "w") as f:
                 f.write(json.dumps(timings, indent=4))
 
         return prediction_results
 
     @staticmethod
     def predict(model_runners: Dict,
@@ -408,27 +418,71 @@
                 multimeric_object=object_to_model,
                 allow_resume=allow_resume,
                 skip_templates=skip_templates,
                 output_dir=output_dir,
                 random_seed=random_seed,
                 **kwargs
             )
+            
             yield {object_to_model: {"prediction_results": prediction_results,
                                      "output_dir": output_dir}}
+            
+    @staticmethod
+    def recalculate_confidence(prediction_results: Dict, multimer_mode:bool, 
+                               total_num_res: int) -> Dict[str, Any]:
+        """A method that remove pae values of padded residues and recalculate iptm_ptm score again """
+        if type(prediction_results['predicted_aligned_error']) == np.ndarray:
+            return prediction_results
+        else:
+            output = {}
+            plddt = prediction_results['plddt'][:total_num_res]
+            if 'predicted_aligned_error' in prediction_results:
+                ptm = confidence.predicted_tm_score(
+                logits=prediction_results['predicted_aligned_error']['logits'][:total_num_res,:total_num_res],
+                breaks=prediction_results['predicted_aligned_error']['breaks'],
+                asym_id=None)
+                
+                pae = confidence.compute_predicted_aligned_error(
+                logits=prediction_results['predicted_aligned_error']['logits'],
+                breaks=prediction_results['predicted_aligned_error']['breaks'])
+                max_pae = pae.pop('max_predicted_aligned_error')
+                
+                for k,v in pae.items():
+                    output.update({k:v[:total_num_res, :total_num_res]})
+                output['max_predicted_aligned_error'] = max_pae
+                if multimer_mode:
+                # Compute the ipTM only for the multimer model.
+                    iptm = confidence.predicted_tm_score(
+                    logits=prediction_results['predicted_aligned_error']['logits'][:total_num_res,:total_num_res],
+                    breaks=prediction_results['predicted_aligned_error']['breaks'],
+                    asym_id=prediction_results['predicted_aligned_error']['asym_id'][:total_num_res],
+                    interface=True)
+                    output.update({'iptm' : iptm})
+                    ranking_confidence = 0.8 * iptm + 0.2 * ptm
+                    output.update({'ranking_confidence' : ranking_confidence})
+                if not multimer_mode:
+                    # Monomer models use mean pLDDT for model ranking.
+                    ranking_confidence =  np.mean(
+                        plddt)
+                    output.update({'ranking_confidence' : ranking_confidence})
+            
+            return output
 
     @staticmethod
     def postprocess(
         prediction_results: Dict,
         multimeric_object: MultimericObject,
         output_dir: str,
+        features_directory: str,
         models_to_relax: ModelsToRelax,
         zip_pickles: bool = False,
         remove_pickles: bool = False,
         use_gpu_relax: bool = True,
         pae_plot_style: str = "red_blue",
+
         **kwargs: Dict,
     ) -> None:
         """
         Performs post-processing operations on predicted protein structures and
         writes results and plots to output_dir.
 
         Parameters
@@ -436,14 +490,16 @@
         prediction_results: Dict
             A dictionary mapping model names with corresponding prediction results.
         multimeric_object : MultimericObject
             The multimeric object containing the predicted structures and
             associated data.
         output_dir : str
             The directory where post-processed files and plots will be saved.
+        features_directory: str
+            The directory containing the features used for prediction. Used by the convert_to_modelcif script.
         models_to_relax : object
             Specifies which models' predictions to relax, defaults to ModelsToRelax enum.
         zip_pickles : bool, optional
             If True, zips the pickle files containing prediction results.
             Default is False.
         remove_pickles : bool, optional
             If True, removes the pickle files after post-processing is complete.
@@ -454,61 +510,68 @@
             The style of the PAE plot, red and blue or AF database style, default is "red_blue".
         **kwargs : dict
             Additional keyword arguments for future extensions or custom
             post-processing steps.
         """
         relaxed_pdbs = {}
         ranking_confidences = {}
+        iptm_scores = {}
+        multimer_mode = type(multimeric_object) == MultimericObject
         # Read timings.json if exists
-        timings_path = join(output_dir, 'timings.json')
+        timings_path = os.path.join(output_dir, 'timings.json')
         timings = _read_from_json_if_exists(timings_path)
-        relax_metrics_path = join(output_dir, 'relax_metrics.json')
+        relax_metrics_path = os.path.join(output_dir, 'relax_metrics.json')
         relax_metrics = _read_from_json_if_exists(relax_metrics_path)
-        multimeric_mode = multimeric_object.multimeric_mode
-        ranking_path = join(output_dir, "ranking_debug.json")
+
+        ranking_path = os.path.join(output_dir, "ranking_debug.json")
+        multimeric_mode = multimeric_object.multimeric_mode if hasattr(multimeric_object, "multimeric_mode") else None
+
         label = 'plddts'
-        total_num_res = sum([len(s) for s in multimeric_object.input_seqs])
+        total_num_res = sum([len(s) for s in multimeric_object.input_seqs]) if multimer_mode else len(multimeric_object.sequence)
         # Save plddt json files.
         for model_name, prediction_result in prediction_results.items():
+            prediction_result.update(AlphaFoldBackend.recalculate_confidence(prediction_result,multimer_mode,
+                                                                         total_num_res))
             if 'iptm' in prediction_result:
                 label = 'iptm+ptm'
-            plddt = prediction_result['plddt'][:total_num_res]
+                iptm_scores[model_name] = float(prediction_result['iptm'])
+            plddt = prediction_result['plddt']
             _save_confidence_json_file(plddt, output_dir, model_name)
             ranking_confidences[model_name] = prediction_result['ranking_confidence']
             # Save and plot PAE if predicting multimer.
             if (
                     'predicted_aligned_error' in prediction_result
                     and 'max_predicted_aligned_error' in prediction_result
             ):
-                pae = prediction_result['predicted_aligned_error'][:total_num_res,:total_num_res]
+                pae = prediction_result['predicted_aligned_error']
 
                 max_pae = prediction_result['max_predicted_aligned_error']
                 _save_pae_json_file(pae, float(max_pae),
                                     output_dir, model_name)
 
         # Rank by model confidence.
         ranked_order = [
             model_name for model_name, confidence in
             sorted(ranking_confidences.items(), key=lambda x: x[1], reverse=True)]
 
         # Save pae plots as *.png files.
         for idx, model_name in enumerate(ranked_order):
             prediction_result = prediction_results[model_name]
-            figure_name = join(
+            figure_name = os.path.join(
                 output_dir, f"{multimeric_object.description}_pae_plot_ranked_{idx}_{model_name}.png")
             plot_pae_from_matrix(
                 seqs=prediction_result['seqs'],
-                pae_matrix=pae,
-                figure_name=figure_name
+                pae_matrix=prediction_result['predicted_aligned_error'],
+                figure_name=figure_name,ranking=idx
             )
 
         # Save ranking_debug.json.
         with open(ranking_path, 'w') as f:
             f.write(json.dumps(
-                {label: ranking_confidences, 'order': ranked_order}, indent=4))
+                {label: ranking_confidences, 'order': ranked_order, "iptm": iptm_scores}, indent=4))
 
         # Relax.
         amber_relaxer = relax.AmberRelaxation(
             max_iterations=RELAX_MAX_ITERATIONS,
             tolerance=RELAX_ENERGY_TOLERANCE,
             stiffness=RELAX_STIFFNESS,
             exclude_residues=RELAX_EXCLUDE_RESIDUES,
@@ -530,34 +593,34 @@
             relaxed_pdb_str, _, violations = amber_relaxer.process(
                 prot=unrelaxed_protein)
             relax_metrics[model_name] = {
                 'remaining_violations': violations,
                 'remaining_violations_count': sum(violations)
             }
             timings[f'relax_{model_name}'] = time.time() - t_0
-            relax_metrics_path = join(output_dir, 'relax_metrics.json')
+            relax_metrics_path = os.path.join(output_dir, 'relax_metrics.json')
             with open(relax_metrics_path, 'w') as f:
                 f.write(json.dumps(relax_metrics, indent=4))
             relaxed_pdbs[model_name] = relaxed_pdb_str
             # Save the relaxed PDB.
-            relaxed_output_path = join(
+            relaxed_output_path = os.path.join(
                 output_dir, f'relaxed_{model_name}.pdb')
             with open(relaxed_output_path, 'w') as f:
                 f.write(relaxed_pdb_str)
 
         with open(timings_path, 'w') as f:
             f.write(json.dumps(timings, indent=4))
               # Write out PDBs in rank order.
         for idx, model_name in enumerate(ranked_order):
             if model_name in relaxed_pdbs:
                 protein_instance = relaxed_pdbs[model_name]
             else:
                 protein_instance = protein.to_pdb(
                     prediction_results[model_name]['unrelaxed_protein'])
-            ranked_output_path = join(output_dir, f'ranked_{idx}.pdb')
+            ranked_output_path = os.path.join(output_dir, f'ranked_{idx}.pdb')
             with open(ranked_output_path, 'w') as f:
                 f.write(protein_instance)
         # Extract multimeric template if multimeric mode is enabled.
         # if multimeric_mode:
         #     feature_dict = multimeric_object.feature_dict
         #     template_mask = feature_dict["template_all_atom_mask"][0]
         #     template_protein = protein.Protein(
@@ -576,12 +639,27 @@
         #         with open(template_file_path, "w") as file:
         #             file.write(pdb_string)
         #         # TODO: use template_sequence for alignment
         #         calculate_rmsd_and_superpose(
         #             template_file_path, ranked_output_path, temp_dir
         #         )
 
+        #Call convert_to_modelcif script
+        # parent_dir = os.path.dirname(os.path.dirname((os.path.abspath(__file__))))
+        # command = f"python3 {parent_dir}/scripts/convert_to_modelcif.py " \
+        #           f"--ap_output {output_dir} " \
+        #           f"--monomer_objects_dir {''.join(features_directory)}"
+
+        #result = subprocess.run(command,
+        #                        check=True,
+        #                        shell=True,
+        #                        capture_output=True,
+        #                        text=True)
+
+        #logging.info(result.stdout)
+        #if result.stderr:
+        #    logging.error("Error:", result.stderr)
         post_prediction_process(
-            output_dir,
-            zip_pickles=zip_pickles,
-            remove_pickles=remove_pickles,
+           output_dir,
+           zip_pickles=zip_pickles,
+           remove_pickles=remove_pickles,
         )
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/folding_backend/alphalink_backend.py` & `alphapulldown-2.0.0b2/alphapulldown/folding_backend/alphalink_backend.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/folding_backend/folding_backend.py` & `alphapulldown-2.0.0b2/alphapulldown/folding_backend/folding_backend.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/folding_backend/unifold_backend.py` & `alphapulldown-2.0.0b2/alphapulldown/folding_backend/unifold_backend.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/objects.py` & `alphapulldown-2.0.0b2/alphapulldown/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,38 +424,38 @@
     """
     multimeric objects with features for multimer
 
     Args
     index: assign a unique index ranging from 0 just to identify different multimer jobs
     interactors: individual interactors that are to be concatenated
     pair_msa: boolean, tells the programme whether to pair MSA or not
-    multimeric_mode: boolean, tells the programme whether use multimeric templates or not
+    multimeric_template: boolean, tells the programme whether use multimeric templates or not
     multimeric_template_meta_data: a csv with the format {"monomer_A":{"xxx.cif":"chainID"},"monomer_B":{"yyy.cif":"chainID"}}
     multimeric_template_dir: a directory where all the multimeric templates mmcifs files are stored
     """
 
     def __init__(self, interactors: list, pair_msa: bool = True, 
-                 multimeric_mode: bool = False, 
+                 multimeric_template: bool = False,
                  multimeric_template_meta_data: str = None,
                  multimeric_template_dir:str = None) -> None:
         self.description = ""
         self.interactors = interactors
         self.build_description_monomer_mapping()
         self.pair_msa = pair_msa
-        self.multimeric_mode = multimeric_mode
+        self.multimeric_template = multimeric_template
         self.chain_id_map = dict()
         self.input_seqs = []
         self.multimeric_template_dir = multimeric_template_dir
         self.create_output_name()
 
         if multimeric_template_meta_data is not None:
             self.multimeric_template_meta_data = prepare_multimeric_template_meta_info(multimeric_template_meta_data,
                                                                                        self.multimeric_template_dir)
             
-        if self.multimeric_mode:
+        if self.multimeric_template:
             self.create_multimeric_template_features()
         self.create_all_chain_features()
         pass
     
     def build_description_monomer_mapping(self):
         """This method constructs a dictionary {description: monomer}"""
         self.monomers_mapping = {m.description: m for m in self.interactors}
@@ -529,15 +529,15 @@
         multichain_mask = np.zeros((len(pdb_map), len(pdb_map)), dtype=int)
         for index1, id1 in enumerate(pdb_map):
             for index2, id2 in enumerate(pdb_map):
                 # and (no_gap_map[index1] and no_gap_map[index2]):
                 if (id1[:4] == id2[:4]):
                     multichain_mask[index1, index2] = 1
         # DEBUG
-        self.save_binary_matrix(multichain_mask, "multichain_mask.png")
+        #self.save_binary_matrix(multichain_mask, "multichain_mask.png")
         return multichain_mask
     
     def create_multimeric_template_features(self):
         """A method of creating multimeric template features"""
         if self.multimeric_template_dir is None or not hasattr(self,"multimeric_template_meta_data"):
             logging.warning(f"""
 You chose to use multimeric template modelling 
@@ -614,15 +614,15 @@
         """
         concatenate and create all chain features
 
         Args
         uniprot_runner: a jackhammer runner with path to the uniprot database
         msa_pairing: boolean pairs msas or not
         """
-        if self.multimeric_mode:
+        if self.multimeric_template:
             logging.info("Running in TrueMultimer mode")
             self.multichain_mask = self.create_multichain_mask()
         self.create_chain_id_map()
         all_chain_features = {}
         sequence_features = {}
         count = 0  # keep the index of input_seqs
         for chain_id, fasta_chain in self.chain_id_map.items():
@@ -641,15 +641,15 @@
             all_chain_features=self.all_chain_features
         )
         self.feature_dict = pipeline_multimer.pad_msa(self.feature_dict, 512)
 
         # make integer to np.array
         for k in ['num_alignments']:
             self.feature_dict[k] = np.array([self.feature_dict[k]])
-        if self.multimeric_mode:
+        if self.multimeric_template:
             self.feature_dict['template_sequence'] = []
             self.feature_dict['multichain_mask'] = self.multichain_mask
             # save used templates
             for i in self.interactors:
                 logging.info(
                     "Used multimeric templates for protein {}".format(i.description))
                 logging.info(i.feature_dict['template_domain_names'])
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/package_data/stereo_chemical_props.txt` & `alphapulldown-2.0.0b2/alphapulldown/package_data/stereo_chemical_props.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/scripts/convert_to_modelcif.py` & `alphapulldown-2.0.0b2/alphapulldown/scripts/convert_to_modelcif.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/scripts/create_individual_features.py` & `alphapulldown-2.0.0b2/alphapulldown/scripts/create_individual_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/scripts/generate_crosslink_pickle.py` & `alphapulldown-2.0.0b2/alphapulldown/scripts/generate_crosslink_pickle.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/scripts/prepare_seq_names.py` & `alphapulldown-2.0.0b2/alphapulldown/scripts/prepare_seq_names.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/scripts/rename_colab_search_a3m.py` & `alphapulldown-2.0.0b2/alphapulldown/scripts/rename_colab_search_a3m.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/calculate_rmsd.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/calculate_rmsd.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/create_combinations.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/create_combinations.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/create_custom_template_db.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/create_custom_template_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Can be used as a standalone script.
 
 """
 
 import os
 import hashlib
 import base64
-import string
 from pathlib import Path
 from absl import logging, flags, app
 from alphapulldown.utils.remove_clashes_low_plddt import MmcifChainFiltered
 from colabfold.batch import validate_and_fix_mmcif
 from alphafold.common.protein import _from_bio_structure, to_mmcif
 
 FLAGS = flags.FLAGS
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/file_handling.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/file_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from absl import logging
 import csv
 import contextlib
 import tempfile
+
+
 @contextlib.contextmanager
 def temp_fasta_file(sequence_str):
     """function that create temp file"""
     with tempfile.NamedTemporaryFile("w", suffix=".fasta") as fasta_file:
         fasta_file.write(sequence_str)
         fasta_file.seek(0)
         yield fasta_file.name
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/modelling_setup.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/modelling_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import alphafold
 from alphafold.data import parsers
 from alphafold.data.tools import jackhmmer
 from alphafold.model import config
 from alphafold.model import model
 from alphafold.model import data
 from alphafold.data import templates
-from alphapulldown.objects import MonomericObject, ChoppedObject
-from alphafold.model.tf.data_transforms import make_fixed_size
+from alphapulldown.objects import MonomericObject
 from os.path import exists,join
 from alphapulldown.objects import ChoppedObject
 from alphapulldown.utils.file_handling import make_dir_monomer_dictionary
-from ml_collections import ConfigDict
 from absl import logging
-import tensorflow as tf
 logging.set_verbosity(logging.INFO)
 
-def parse_fold(args):
+
+def parse_fold(input, features_directory, protein_delimiter):
     all_folding_jobs = []
-    for i in args.input:
+    for i in input:
         formatted_folds, missing_features, unique_features = [], [], []
-        protein_folds = [x.split(":") for x in i.split(args.protein_delimiter)]
+        protein_folds = [x.split(":") for x in i.split(protein_delimiter)]
         for protein_fold in protein_folds:
             name, number, region = None, 1, "all"
 
             match len(protein_fold):
                 case 1:
                     name = protein_fold[0]
                 case 2:
@@ -52,26 +50,25 @@
             if len(region) != 2 and region != "all":
                 raise ValueError(f"Region {region} is malformatted expected start-stop.")
 
             if len(region) == 2:
                 region = [tuple(int(x) for x in region)]
 
             unique_features.append(name)
-            if not any([exists(join(monomer_dir, f"{name}.pkl")) for monomer_dir in args.features_directory]):
+            if not any([exists(join(monomer_dir, f"{name}.pkl")) for monomer_dir in features_directory]):
                 missing_features.append(name)
 
             formatted_folds.extend([{name: region} for _ in range(number)])
         all_folding_jobs.append(formatted_folds)
         missing_features = set(missing_features)
         if len(missing_features):
             raise FileNotFoundError(
-                f"{missing_features} not found in {args.features_directory}"
+                f"{missing_features} not found in {features_directory}"
             )
-    args.parsed_input = all_folding_jobs
-    return args
+    return all_folding_jobs
 
 def pad_input_features(feature_dict: dict, 
                        desired_num_res : int, desired_num_msa : int) -> None:
     
     """
     A function that pads input feature numpy arrays based on desired number of residues 
     and desired number of msas
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/multimeric_template_utils.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/multimeric_template_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/plotting.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/plotting.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # the script to plot PAEs after predicting structures
 # #
 import matplotlib
 matplotlib.use("agg")
 import matplotlib.pyplot as plt
 
 
-def plot_pae_from_matrix(seqs,pae_matrix,figure_name=''):
+def plot_pae_from_matrix(seqs,pae_matrix,figure_name='',ranking:int = 0):
     xticks = []
     initial_tick = 0
     for s in seqs:
         initial_tick = initial_tick + len(s)
         xticks.append(initial_tick)
 
     xticks_labels = []
@@ -30,9 +30,9 @@
 
     ax1.set_xticklabels(xticks_labels, size="large")
     ax1.set_yticklabels(yticks_labels,size="large")
     fig.colorbar(pos).ax.set_title("unit: Angstrom")
     for t in xticks:
         ax1.axhline(t, color="black", linewidth=3.5)
         ax1.axvline(t, color="black", linewidth=3.5)
-    plt.title("ranked_{}".format(i))
+    plt.title(f"ranked_{ranking}".format(i))
     plt.savefig(figure_name)
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/post_modelling.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/post_modelling.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,27 @@
         results = subprocess.run(cmd,shell=True,capture_output=True,text=True)
     except subprocess.CalledProcessError as e:
         print(f"Error while compressing result pickles: {e.returncode}")
         print(f"Command output: {e.output}")
 
 def post_prediction_process(output_path,zip_pickles = False,remove_pickles = False):
     """A function to process resulted files after the prediction"""
-    if remove_pickles:
+    if remove_pickles and zip_pickles:
         remove_irrelavent_pickles(output_path)
-    if zip_pickles:
-        zip_result_pickles(output_path)
+    else:
+        if zip_pickles:
+            zip_result_pickles(output_path)
+        if remove_pickles:
+            remove_irrelavent_pickles(output_path)
 
 def remove_irrelavent_pickles(output_path):
     """Remove result pickles that do not belong to the best model"""
     try:
         best_model = json.load(open(os.path.join(output_path,"ranking_debug.json"),'rb'))['order'][0]
-        pickle_to_remove = [i for i in os.listdir(output_path) if (i.endswith('pkl')) and (best_model not in i)]
+        pickle_to_remove = [os.path.join(output_path,i) for i in os.listdir(output_path) if (i.endswith('pkl')) and (best_model not in i)]
         cmd = ['rm'] + pickle_to_remove
         results = subprocess.run(cmd)
     except FileNotFoundError:
         print(f"ranking_debug.json does not exist in : {output_path}. Please check your inputs.")
     except subprocess.CalledProcessError as e:
         print(f"Error while removing result pickles: {e.returncode}")
         print(f"Command output: {e.output}")
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/remove_clashes_low_plddt.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/remove_clashes_low_plddt.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/alphapulldown/utils/save_meta_data.py` & `alphapulldown-2.0.0b2/alphapulldown/utils/save_meta_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #
 # Author: Dingquan Yu
 # A script containing utility functions
-# 
-import contextlib
-
+#
 from alphapulldown import __version__ as AP_VERSION
 from alphafold.version import __version__ as AF_VERSION
 import json
 import os
 from absl import logging
 from alphapulldown.utils.file_handling import ensure_directory_exists
 import subprocess
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown.egg-info/PKG-INFO` & `alphapulldown-2.0.0b2/alphapulldown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphapulldown
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Pipeline allows massive screening using alphafold
 Home-page: https://github.com/KosinskiLab/AlphaPulldown
 Author: Dingquan Yu
 Author-email: dingquan.yu@embl-hamburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,26 +29,27 @@
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: jupyterlab
 Requires-Dist: ipywidgets
 
 # AlphaPulldown
 [![Downloads](https://static.pepy.tech/badge/alphapulldown)](https://pepy.tech/project/alphapulldown)  [![python3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) ![GPL3 license](https://img.shields.io/badge/license-GPLv3-green)
 
-## 🥳 AlphaPulldown has entered the era of version 1.x
+## 🥳 AlphaPulldown has entered the era of version 2.0 (beta)
 We have brought some exciting useful features to AlphaPulldown and updated its computing environment. 
 
 
 AlphaPulldown is a Python package that streamlines protein-protein interaction screens and high-throughput modelling of higher-order oligomers using AlphaFold-Multimer:
 * provides a convenient command line interface to screen a bait protein against many candidates, calculate all-versus-all pairwise comparisons, test alternative homo-oligomeric states, and model various parts of a larger complex
 * separates the CPU stages (MSA and template feature generation) from GPU stages (the actual modeling)
 * allows modeling fragments of proteins without recalculation of MSAs and keeping the original full-length residue numbering in the models
 * summarizes the results in a CSV table with AlphaFold scores, pDockQ and mpDockQ, PI-score, and various physical parameters of the interface
 * provides a Jupyter notebook for an interactive analysis of PAE plots and models
+* 🆕 refactorised codes and removed redundancy
+* 🆕 added a new way of integrating experimental models into AlphaFold pipeline using custom multimeric databases
 * 🆕 integrates cross-link mass spec data with AlphaFold predictions via [AlphaLink2](https://github.com/Rappsilber-Laboratory/AlphaLink2/tree/main) models
-* 🆕 able to integrate experimental models into AlphaFold pipeline using custom multimeric databases
 
 ## Pre-installation
 Check if you have downloaded necessary parameters and databases (e.g. BFD, MGnify etc.) as instructed in [AlphFold's documentation](https://github.com/deepmind/alphafold). You should have a directory like below:
  ```
  alphafold_database/                             # Total: ~ 2.2 TB (download: 438 GB)
     bfd/                                   # ~ 1.7 TB (download: 271.6 GB)
         # 6 files.
@@ -94,15 +95,15 @@
 
 ## Installation using pip
 
 Activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 
-python3 -m pip install alphapulldown==1.0.4
+python3 -m pip install alphapulldown==2.0.0b1
 pip install jax==0.4.23 jaxlib==0.4.23+cuda11.cudnn86 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **For older versions of AlphaFold**: 
 If you haven't updated your databases according to the requirements of AlphaFold 2.3.0, you can still use AlphaPulldown with your older version of AlphaFold database. Please follow the installation instructions on the [dedicated branch](https://github.com/KosinskiLab/AlphaPulldown/tree/AlphaFold-2.2.0)
 
 ## How to develop
```

### Comparing `alphapulldown-2.0.0b1/alphapulldown.egg-info/SOURCES.txt` & `alphapulldown-2.0.0b2/alphapulldown.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,21 @@
 ./alphafold/alphafold/relax/cleanup_test.py
 ./alphafold/alphafold/relax/relax.py
 ./alphafold/alphafold/relax/relax_test.py
 ./alphafold/alphafold/relax/utils.py
 ./alphafold/alphafold/relax/utils_test.py
 ./alphapulldown/__init__.py
 ./alphapulldown/objects.py
-./alphapulldown/predict_structure.py
-./alphapulldown/test_new_mmt.py
+./alphapulldown/test_import_flags.py
+./alphapulldown/test_model_relax.py
 ./alphapulldown/analysis_pipeline/af2_3dmol.py
 ./alphapulldown/analysis_pipeline/calculate_mpdockq.py
 ./alphapulldown/analysis_pipeline/create_notebook.py
 ./alphapulldown/analysis_pipeline/get_good_inter_pae.py
+./alphapulldown/analysis_pipeline/pdb_analyser.py
 ./alphapulldown/analysis_pipeline/test_create_notebook.py
 ./alphapulldown/analysis_pipeline/utils.py
 ./alphapulldown/analysis_pipeline/af2plots/af2plots/__main__.py
 ./alphapulldown/analysis_pipeline/af2plots/af2plots/plotter.py
 ./alphapulldown/analysis_pipeline/af2plots/af2plots/version.py
 ./alphapulldown/folding_backend/__init__.py
 ./alphapulldown/folding_backend/alphafold_backend.py
@@ -189,19 +190,17 @@
 alphafold/run_alphafold.py
 alphapulldown.egg-info/PKG-INFO
 alphapulldown.egg-info/SOURCES.txt
 alphapulldown.egg-info/dependency_links.txt
 alphapulldown.egg-info/requires.txt
 alphapulldown.egg-info/top_level.txt
 alphapulldown/package_data/stereo_chemical_props.txt
-test/test_alphalink2_folding_backend.py
 test/test_create_monomeric_objects.py
 test/test_create_multimeric_objects.py
 test/test_create_multimeric_template_features.py
-test/test_crosslink_inference.py
-test/test_crosslink_input.py
 test/test_custom_db.py
 test/test_features.py
 test/test_features_with_templates.py
+test/test_postprocessing.py
 test/test_predictions_slurm.py
 test/test_python_imports.py
 test/test_remove_clashes_low_plddt.py
```

### Comparing `alphapulldown-2.0.0b1/setup.cfg` & `alphapulldown-2.0.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/test/test_alphalink2_folding_backend.py` & `alphapulldown-2.0.0b2/test/test_create_multimeric_objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-import gzip
 import unittest
 from alphapulldown.objects import MultimericObject
 import pickle
-from folding_backend.alphalink_backend import AlphaLinkBackend
+import numpy as np
 
-class TestAlphaLink2Backend(unittest.TestCase):
+
+class TestCreateMultimericObject(unittest.TestCase):
+    """A class that test major functions of creating feature_dict of a MultimericObject object"""
 
     def setUp(self) -> None:
-        self.monomer1 = pickle.load(open("./test/test_data/H1134_A.pkl",'rb'))
-        self.monomer2 = pickle.load(open("./test/test_data/H1134_B.pkl",'rb'))
-        self.multimericObj = MultimericObject([self.monomer1,self.monomer2])
-        self.alphalink2_weights = '/g/alphafold/alphalink_weights/AlphaLink-Multimer_SDA_v3.pt'
-        self.xl_info = "./test/test_data/test_xl_input.pkl.gz"
-        return super().setUp()
+        self.monomer1 = pickle.load(open("./test/test_data/H1142_A.pkl", "rb"))
+        self.monomer2 = pickle.load(open("./test/example_data/H1142_B.pkl", "rb"))
+    
+    def test_1_initiate_default_multimericobject(self) -> MultimericObject:
+        multimer_obj = MultimericObject([self.monomer1, self.monomer2])
+        return multimer_obj
     
-    def test_1_initialise_folding_backend(self):
-        beckend = AlphaLinkBackend
-        model_config = beckend.setup(self.alphalink2_weights,
-                                                             self.xl_info)
-        beckend.predict(**model_config,multimeric_object = self.multimericObj,output_dir= "./test/test_data")
+    def test_1_initiate_multimericobject_without_msa_pairing(self) -> MultimericObject:
+        multimer_obj = MultimericObject([self.monomer1, self.monomer2],pair_msa=False)
+        return multimer_obj
+
+    def test_2_check_residue_indexes(self):
+        multimer_obj = self.test_1_initiate_default_multimericobject()
+        seq_1_length = self.monomer1.feature_dict['seq_length'][0]
+        seq_2_length = self.monomer2.feature_dict['seq_length'][0]
+        expected_residue_index=np.array(list(range(seq_1_length)) + list(range(seq_2_length)))
+        self.assertTrue(np.array_equal(multimer_obj.feature_dict['residue_index'],expected_residue_index))
 
-if __name__ == "__main__":
+if __name__=="__main__":
     unittest.main()
```

### Comparing `alphapulldown-2.0.0b1/test/test_create_monomeric_objects.py` & `alphapulldown-2.0.0b2/test/test_create_monomeric_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 or MultimericObject works
 """
 import unittest
 from alphapulldown.objects import MonomericObject
 import shutil
 from alphafold.data.pipeline import DataPipeline
 from alphafold.data.tools import hmmsearch
-from alphapulldown.utils import parse_fasta, create_uniprot_runner, create_model_runners_and_random_seed, templates
+from alphapulldown.utils.file_handling import parse_fasta
+from alphapulldown.utils.modelling_setup import create_uniprot_runner, create_model_runners_and_random_seed, templates
 import os
 from colabfold.utils import DEFAULT_API_SERVER
 
 class TestCreateObjects(unittest.TestCase):
     def setUp(self) -> None:
         self.jackhmmer_binary_path = shutil.which("jackhmmer")
         self.hmmsearch_binary_path = shutil.which("hmmsearch")
```

### Comparing `alphapulldown-2.0.0b1/test/test_create_multimeric_template_features.py` & `alphapulldown-2.0.0b2/test/test_create_multimeric_template_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest 
-import numpy as np
 import gzip,pickle,shutil
-from alphapulldown.objects import MultimericObject
 from alphafold.data.templates import _build_query_to_hit_index_mapping
 from alphapulldown.utils import multimeric_template_utils
+
+
 class TestMultimericTemplateFeatures(unittest.TestCase):
     def setUp(self):
         self.mmcif_file = "./test/test_data/true_multimer/3L4Q.cif"
         self.monomer1 = pickle.load(open("./test/test_data/true_multimer/features/3L4Q_A.pkl",'rb'))
         self.monomer2 = pickle.load(open("./test/test_data/true_multimer/features/3L4Q_C.pkl",'rb'))
         self.kalign_binary_path = shutil.which('kalign')
         self.mmt_dir = './test/test_data/true_multimer/'
```

### Comparing `alphapulldown-2.0.0b1/test/test_custom_db.py` & `alphapulldown-2.0.0b2/test/test_custom_db.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/test/test_features.py` & `alphapulldown-2.0.0b2/test/test_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import subprocess
 from pathlib import Path
 from absl.testing import absltest
-import alphapulldown.create_individual_features as run_features_generation
+import alphapulldown.scripts.create_individual_features as run_features_generation
 import tempfile
-import shutil
 import time
 import os
 
 
 class TestCreateIndividualFeaturesWithTemplates(absltest.TestCase):
     def setUp(self):
         super().setUp()
```

### Comparing `alphapulldown-2.0.0b1/test/test_features_with_templates.py` & `alphapulldown-2.0.0b2/test/test_features_with_templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-2.0.0b1/test/test_python_imports.py` & `alphapulldown-2.0.0b2/test/test_python_imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from alphapulldown.utils import *
 from alphapulldown.folding_backend import *
 import io
 import warnings
 import subprocess
 from absl import app
 import os
-from alphapulldown.predict_structure import ModelsToRelax
 from alphapulldown.utils.modelling_setup import get_run_alphafold
 from alphapulldown.utils.create_combinations import process_files
 
 import argparse
 from os import makedirs
 from typing import Dict, List
 from os.path import exists, join
```

### Comparing `alphapulldown-2.0.0b1/test/test_remove_clashes_low_plddt.py` & `alphapulldown-2.0.0b2/test/test_remove_clashes_low_plddt.py`

 * *Files identical despite different names*

