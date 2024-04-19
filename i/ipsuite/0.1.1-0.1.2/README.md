# Comparing `tmp/ipsuite-0.1.1.tar.gz` & `tmp/ipsuite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsuite-0.1.1.tar", max compression
+gzip compressed data, was "ipsuite-0.1.2.tar", max compression
```

## Comparing `ipsuite-0.1.1.tar` & `ipsuite-0.1.2.tar`

### file list

```diff
@@ -1,82 +1,87 @@
--rw-r--r--   0        0        0    14197 2023-05-30 11:28:15.453762 ipsuite-0.1.1/LICENSE
--rw-r--r--   0        0        0     1048 2023-11-03 10:30:42.369890 ipsuite-0.1.1/README.md
--rw-r--r--   0        0        0      882 2023-05-30 12:26:18.215627 ipsuite-0.1.1/ipsuite/__init__.py
--rw-r--r--   0        0        0     1345 2023-08-10 12:03:43.037558 ipsuite-0.1.1/ipsuite/analysis/__init__.py
--rw-r--r--   0        0        0     6694 2023-08-10 12:03:43.037558 ipsuite-0.1.1/ipsuite/analysis/bin_property.py
--rw-r--r--   0        0        0     6104 2023-10-24 12:03:42.474054 ipsuite-0.1.1/ipsuite/analysis/bond_stretch.py
--rw-r--r--   0        0        0     3698 2023-10-24 12:03:42.484054 ipsuite-0.1.1/ipsuite/analysis/ensemble.py
--rw-r--r--   0        0        0      685 2023-06-12 15:35:29.165912 ipsuite-0.1.1/ipsuite/analysis/model/__init__.py
--rw-r--r--   0        0        0    15500 2023-10-24 12:03:42.514054 ipsuite-0.1.1/ipsuite/analysis/model/dynamics.py
--rw-r--r--   0        0        0     7936 2023-08-23 08:23:59.028727 ipsuite-0.1.1/ipsuite/analysis/model/dynamics_checks.py
--rw-r--r--   0        0        0     2437 2023-10-24 12:03:42.534054 ipsuite-0.1.1/ipsuite/analysis/model/math.py
--rw-r--r--   0        0        0     3673 2023-08-23 08:24:06.748643 ipsuite-0.1.1/ipsuite/analysis/model/plots.py
--rw-r--r--   0        0        0    18340 2023-10-24 12:03:42.544054 ipsuite-0.1.1/ipsuite/analysis/model/predict.py
--rw-r--r--   0        0        0     5371 2023-10-24 12:03:42.594053 ipsuite-0.1.1/ipsuite/analysis/sensitivity.py
--rw-r--r--   0        0        0      416 2023-05-30 12:26:18.215627 ipsuite-0.1.1/ipsuite/base/__init__.py
--rw-r--r--   0        0        0     7610 2023-10-24 12:03:42.594053 ipsuite-0.1.1/ipsuite/base/base.py
--rw-r--r--   0        0        0      971 2023-03-10 10:05:15.098799 ipsuite-0.1.1/ipsuite/base/protocol.py
--rw-r--r--   0        0        0      336 2023-10-24 12:03:42.624053 ipsuite-0.1.1/ipsuite/bootstrap/__init__.py
--rw-r--r--   0        0        0     5343 2023-10-24 12:03:42.654053 ipsuite-0.1.1/ipsuite/bootstrap/random_displacements.py
--rw-r--r--   0        0        0     7115 2023-10-24 12:03:42.664052 ipsuite-0.1.1/ipsuite/bootstrap/surface_mods.py
--rw-r--r--   0        0        0       97 2023-05-30 11:28:15.573761 ipsuite-0.1.1/ipsuite/calculators/__init__.py
--rw-r--r--   0        0        0      976 2023-11-03 10:30:42.369890 ipsuite-0.1.1/ipsuite/calculators/__init__.pyi
--rw-r--r--   0        0        0     3412 2023-10-24 12:03:42.674052 ipsuite-0.1.1/ipsuite/calculators/apax_jax_md.py
--rw-r--r--   0        0        0     3091 2023-10-24 12:03:42.684052 ipsuite-0.1.1/ipsuite/calculators/ase_geoopt.py
--rw-r--r--   0        0        0    19999 2023-10-24 12:03:42.694052 ipsuite-0.1.1/ipsuite/calculators/ase_md.py
--rw-r--r--   0        0        0     1822 2023-08-10 12:03:43.167557 ipsuite-0.1.1/ipsuite/calculators/ase_standard.py
--rw-r--r--   0        0        0     9403 2023-11-03 10:37:12.725610 ipsuite-0.1.1/ipsuite/calculators/cp2k.py
--rw-r--r--   0        0        0     6777 2023-11-03 10:30:42.369890 ipsuite-0.1.1/ipsuite/calculators/lammps.py
--rw-r--r--   0        0        0     1305 2023-08-10 12:03:43.197557 ipsuite-0.1.1/ipsuite/calculators/orca.py
--rw-r--r--   0        0        0     1069 2023-08-10 12:03:43.207557 ipsuite-0.1.1/ipsuite/calculators/xtb.py
--rw-r--r--   0        0        0     2328 2023-03-17 08:00:52.668953 ipsuite-0.1.1/ipsuite/configuration_comparison/MMKernel.py
--rw-r--r--   0        0        0     2267 2023-03-08 18:22:08.931925 ipsuite-0.1.1/ipsuite/configuration_comparison/REMatch.py
--rw-r--r--   0        0        0      136 2023-04-11 15:30:14.938963 ipsuite-0.1.1/ipsuite/configuration_comparison/__init__.py
--rw-r--r--   0        0        0      164 2023-04-11 15:30:14.938963 ipsuite-0.1.1/ipsuite/configuration_comparison/__init__.pyi
--rw-r--r--   0        0        0    11526 2023-11-03 09:34:01.026511 ipsuite-0.1.1/ipsuite/configuration_comparison/base.py
--rw-r--r--   0        0        0      161 2023-04-11 15:30:14.938963 ipsuite-0.1.1/ipsuite/configuration_generation/__init__.py
--rw-r--r--   0        0        0      219 2023-09-19 16:30:32.989202 ipsuite-0.1.1/ipsuite/configuration_generation/__init__.pyi
--rw-r--r--   0        0        0     3613 2023-10-24 12:03:42.774051 ipsuite-0.1.1/ipsuite/configuration_generation/packmol.py
--rw-r--r--   0        0        0     2289 2023-08-23 08:24:06.768643 ipsuite-0.1.1/ipsuite/configuration_generation/smiles_to_atoms.py
--rw-r--r--   0        0        0      958 2023-05-30 11:28:15.683760 ipsuite-0.1.1/ipsuite/configuration_selection/__init__.py
--rw-r--r--   0        0        0     5316 2023-11-03 10:30:42.379890 ipsuite-0.1.1/ipsuite/configuration_selection/base.py
--rw-r--r--   0        0        0      621 2023-04-05 08:34:02.207584 ipsuite-0.1.1/ipsuite/configuration_selection/index.py
--rw-r--r--   0        0        0     5196 2023-11-03 09:34:01.176510 ipsuite-0.1.1/ipsuite/configuration_selection/kernel.py
--rw-r--r--   0        0        0      609 2023-08-01 07:46:39.263824 ipsuite-0.1.1/ipsuite/configuration_selection/random.py
--rw-r--r--   0        0        0      603 2023-04-05 10:26:28.603373 ipsuite-0.1.1/ipsuite/configuration_selection/split.py
--rw-r--r--   0        0        0     4108 2023-11-03 09:34:01.186509 ipsuite-0.1.1/ipsuite/configuration_selection/threshold.py
--rw-r--r--   0        0        0      945 2023-05-30 11:28:15.723759 ipsuite-0.1.1/ipsuite/configuration_selection/uniform_arange.py
--rw-r--r--   0        0        0     1443 2023-03-17 08:00:52.678953 ipsuite-0.1.1/ipsuite/configuration_selection/uniform_energetic.py
--rw-r--r--   0        0        0      602 2023-03-17 08:00:52.678953 ipsuite-0.1.1/ipsuite/configuration_selection/uniform_temporal.py
--rw-r--r--   0        0        0      186 2023-04-03 18:16:54.459557 ipsuite-0.1.1/ipsuite/data_loading/__init__.py
--rw-r--r--   0        0        0     2630 2023-08-10 12:03:43.287556 ipsuite-0.1.1/ipsuite/data_loading/add_data_ase.py
--rw-r--r--   0        0        0      730 2023-08-10 12:03:43.297556 ipsuite-0.1.1/ipsuite/data_loading/add_data_h5md.py
--rw-r--r--   0        0        0      103 2023-03-21 18:17:21.212138 ipsuite-0.1.1/ipsuite/fields/__init__.py
--rw-r--r--   0        0        0     1711 2023-07-12 16:24:22.603346 ipsuite-0.1.1/ipsuite/fields/atoms.py
--rw-r--r--   0        0        0       88 2023-03-22 18:15:23.427142 ipsuite-0.1.1/ipsuite/geometry/__init__.py
--rw-r--r--   0        0        0     1255 2023-08-10 12:03:43.317555 ipsuite-0.1.1/ipsuite/geometry/barycenter_coarse_grain.py
--rw-r--r--   0        0        0     1236 2023-08-01 07:46:39.263824 ipsuite-0.1.1/ipsuite/geometry/graphs.py
--rw-r--r--   0        0        0     1144 2023-08-10 12:03:43.317555 ipsuite-0.1.1/ipsuite/geometry/mapping.py
--rw-r--r--   0        0        0     2140 2023-08-10 12:03:43.327555 ipsuite-0.1.1/ipsuite/geometry/unwrap.py
--rw-r--r--   0        0        0       97 2023-04-11 15:30:14.938963 ipsuite-0.1.1/ipsuite/models/__init__.py
--rw-r--r--   0        0        0      265 2023-08-10 12:03:43.337555 ipsuite-0.1.1/ipsuite/models/__init__.pyi
--rw-r--r--   0        0        0     4531 2023-10-24 12:03:42.834051 ipsuite-0.1.1/ipsuite/models/apax.py
--rw-r--r--   0        0        0     2606 2023-05-30 11:28:15.773759 ipsuite-0.1.1/ipsuite/models/base.py
--rw-r--r--   0        0        0     2981 2023-10-24 12:03:42.834051 ipsuite-0.1.1/ipsuite/models/ensemble.py
--rw-r--r--   0        0        0    10462 2023-06-12 14:17:19.616546 ipsuite-0.1.1/ipsuite/models/gap.py
--rw-r--r--   0        0        0     4510 2023-11-03 10:30:42.389890 ipsuite-0.1.1/ipsuite/models/mace_model.py
--rw-r--r--   0        0        0     6742 2023-10-24 12:03:42.844051 ipsuite-0.1.1/ipsuite/models/nequip.py
--rw-r--r--   0        0        0     5165 2023-11-03 10:30:42.389890 ipsuite-0.1.1/ipsuite/nodes.py
--rw-r--r--   0        0        0      188 2023-04-03 20:55:43.075074 ipsuite-0.1.1/ipsuite/project/__init__.py
--rw-r--r--   0        0        0       96 2023-04-11 15:30:14.948963 ipsuite-0.1.1/ipsuite/static_data/__init__.py
--rw-r--r--   0        0        0     1609 2023-05-30 11:28:15.843758 ipsuite-0.1.1/ipsuite/static_data/gap.jinja2
--rw-r--r--   0        0        0     2300 2023-11-03 10:30:42.389890 ipsuite-0.1.1/ipsuite/static_data/lammps_npt.jinja2
--rw-r--r--   0        0        0     2046 2023-06-12 08:03:57.512767 ipsuite-0.1.1/ipsuite/static_data/y_log.json
--rw-r--r--   0        0        0      155 2023-04-05 16:53:50.539938 ipsuite-0.1.1/ipsuite/utils/__init__.py
--rw-r--r--   0        0        0     1337 2023-04-13 20:08:01.697728 ipsuite-0.1.1/ipsuite/utils/ase_sim.py
--rw-r--r--   0        0        0     6250 2023-05-30 11:28:15.903757 ipsuite-0.1.1/ipsuite/utils/combine.py
--rw-r--r--   0        0        0     1739 2023-08-10 12:03:43.407554 ipsuite-0.1.1/ipsuite/utils/helpers.py
--rw-r--r--   0        0        0      572 2023-03-09 17:30:00.842723 ipsuite-0.1.1/ipsuite/utils/logs.py
--rw-r--r--   0        0        0      691 2023-04-05 16:53:50.539938 ipsuite-0.1.1/ipsuite/utils/md.py
--rw-r--r--   0        0        0     2490 2023-10-24 12:03:42.874050 ipsuite-0.1.1/ipsuite/utils/metrics.py
--rw-r--r--   0        0        0     2777 2023-11-03 10:38:13.334946 ipsuite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 ipsuite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    14197 2023-05-30 11:28:15.453762 ipsuite-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3553 2024-04-19 12:35:46.388721 ipsuite-0.1.2/README.md
+-rw-r--r--   0        0        0      883 2024-04-18 18:03:34.597181 ipsuite-0.1.2/ipsuite/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-19 12:35:46.398721 ipsuite-0.1.2/ipsuite/analysis/__init__.py
+-rw-r--r--   0        0        0     6369 2024-04-19 12:35:46.398721 ipsuite-0.1.2/ipsuite/analysis/bin_property.py
+-rw-r--r--   0        0        0     6087 2024-04-18 12:18:45.223806 ipsuite-0.1.2/ipsuite/analysis/bond_stretch.py
+-rw-r--r--   0        0        0     3634 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/analysis/ensemble.py
+-rw-r--r--   0        0        0     1120 2024-04-18 16:14:36.413113 ipsuite-0.1.2/ipsuite/analysis/md.py
+-rw-r--r--   0        0        0     1139 2024-04-19 12:35:46.398721 ipsuite-0.1.2/ipsuite/analysis/model/__init__.py
+-rw-r--r--   0        0        0    15233 2024-04-19 12:35:46.398721 ipsuite-0.1.2/ipsuite/analysis/model/dynamics.py
+-rw-r--r--   0        0        0     7889 2024-04-19 12:35:46.398721 ipsuite-0.1.2/ipsuite/analysis/model/dynamics_checks.py
+-rw-r--r--   0        0        0     2437 2023-10-24 12:03:42.534054 ipsuite-0.1.2/ipsuite/analysis/model/math.py
+-rw-r--r--   0        0        0     4317 2024-04-19 12:35:46.398721 ipsuite-0.1.2/ipsuite/analysis/model/plots.py
+-rw-r--r--   0        0        0    20115 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/analysis/model/predict.py
+-rw-r--r--   0        0        0     5342 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/analysis/sensitivity.py
+-rw-r--r--   0        0        0      436 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/base/__init__.py
+-rw-r--r--   0        0        0     7771 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/base/base.py
+-rw-r--r--   0        0        0      972 2023-11-03 15:52:05.240904 ipsuite-0.1.2/ipsuite/base/protocol.py
+-rw-r--r--   0        0        0      579 2024-04-16 14:19:55.044202 ipsuite-0.1.2/ipsuite/bootstrap/__init__.py
+-rw-r--r--   0        0        0     5332 2024-04-18 12:18:45.233806 ipsuite-0.1.2/ipsuite/bootstrap/random_displacements.py
+-rw-r--r--   0        0        0     7042 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/bootstrap/surface_mods.py
+-rw-r--r--   0        0        0      235 2024-04-16 14:19:55.044202 ipsuite-0.1.2/ipsuite/calculators/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-06 21:47:01.535058 ipsuite-0.1.2/ipsuite/calculators/__init__.pyi
+-rw-r--r--   0        0        0     3318 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/calculators/apax_jax_md.py
+-rw-r--r--   0        0        0     3497 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/calculators/ase_geoopt.py
+-rw-r--r--   0        0        0    22233 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/calculators/ase_md.py
+-rw-r--r--   0        0        0     1822 2023-08-10 12:03:43.167557 ipsuite-0.1.2/ipsuite/calculators/ase_standard.py
+-rw-r--r--   0        0        0     9409 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/calculators/cp2k.py
+-rw-r--r--   0        0        0     6777 2024-03-06 21:57:41.978504 ipsuite-0.1.2/ipsuite/calculators/lammps.py
+-rw-r--r--   0        0        0     3943 2024-04-18 10:28:50.530225 ipsuite-0.1.2/ipsuite/calculators/mix.py
+-rw-r--r--   0        0        0     1306 2024-04-19 12:35:46.408721 ipsuite-0.1.2/ipsuite/calculators/orca.py
+-rw-r--r--   0        0        0     6608 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/calculators/torch_d3.py
+-rw-r--r--   0        0        0     1066 2024-04-18 12:18:45.233806 ipsuite-0.1.2/ipsuite/calculators/xtb.py
+-rw-r--r--   0        0        0     2329 2023-11-03 15:52:05.300903 ipsuite-0.1.2/ipsuite/configuration_comparison/MMKernel.py
+-rw-r--r--   0        0        0     2259 2024-04-18 12:18:45.233806 ipsuite-0.1.2/ipsuite/configuration_comparison/REMatch.py
+-rw-r--r--   0        0        0      137 2023-11-03 15:52:05.350903 ipsuite-0.1.2/ipsuite/configuration_comparison/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-11 15:30:14.938963 ipsuite-0.1.2/ipsuite/configuration_comparison/__init__.pyi
+-rw-r--r--   0        0        0    12263 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/configuration_comparison/base.py
+-rw-r--r--   0        0        0      162 2023-11-03 15:52:05.380902 ipsuite-0.1.2/ipsuite/configuration_generation/__init__.py
+-rw-r--r--   0        0        0      249 2023-11-17 13:28:48.496472 ipsuite-0.1.2/ipsuite/configuration_generation/__init__.pyi
+-rw-r--r--   0        0        0     6418 2024-04-18 16:14:36.423113 ipsuite-0.1.2/ipsuite/configuration_generation/packmol.py
+-rw-r--r--   0        0        0     2263 2024-04-18 16:14:36.423113 ipsuite-0.1.2/ipsuite/configuration_generation/smiles_to_atoms.py
+-rw-r--r--   0        0        0     1045 2023-11-10 18:20:58.664738 ipsuite-0.1.2/ipsuite/configuration_selection/__init__.py
+-rw-r--r--   0        0        0     7369 2024-04-18 12:18:45.243806 ipsuite-0.1.2/ipsuite/configuration_selection/base.py
+-rw-r--r--   0        0        0     2223 2023-11-10 18:20:58.684738 ipsuite-0.1.2/ipsuite/configuration_selection/filter.py
+-rw-r--r--   0        0        0      619 2024-04-18 12:18:45.243806 ipsuite-0.1.2/ipsuite/configuration_selection/index.py
+-rw-r--r--   0        0        0     6514 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/configuration_selection/kernel.py
+-rw-r--r--   0        0        0      604 2024-04-18 12:18:45.243806 ipsuite-0.1.2/ipsuite/configuration_selection/random.py
+-rw-r--r--   0        0        0      601 2024-04-18 12:18:45.243806 ipsuite-0.1.2/ipsuite/configuration_selection/split.py
+-rw-r--r--   0        0        0     4962 2023-11-10 18:20:58.684738 ipsuite-0.1.2/ipsuite/configuration_selection/threshold.py
+-rw-r--r--   0        0        0      943 2024-04-18 12:18:45.243806 ipsuite-0.1.2/ipsuite/configuration_selection/uniform_arange.py
+-rw-r--r--   0        0        0     1441 2024-04-18 12:18:45.243806 ipsuite-0.1.2/ipsuite/configuration_selection/uniform_energetic.py
+-rw-r--r--   0        0        0      600 2024-04-18 12:18:45.253805 ipsuite-0.1.2/ipsuite/configuration_selection/uniform_temporal.py
+-rw-r--r--   0        0        0      209 2024-03-06 21:47:01.595057 ipsuite-0.1.2/ipsuite/data_loading/__init__.py
+-rw-r--r--   0        0        0     3358 2024-04-18 16:14:36.423113 ipsuite-0.1.2/ipsuite/data_loading/add_data_ase.py
+-rw-r--r--   0        0        0      731 2023-11-03 15:52:05.850897 ipsuite-0.1.2/ipsuite/data_loading/add_data_h5md.py
+-rw-r--r--   0        0        0      103 2024-04-18 16:14:36.433113 ipsuite-0.1.2/ipsuite/fields/__init__.py
+-rw-r--r--   0        0        0     1712 2024-04-18 16:14:36.433113 ipsuite-0.1.2/ipsuite/fields/atoms.py
+-rw-r--r--   0        0        0      378 2024-04-18 12:18:45.253805 ipsuite-0.1.2/ipsuite/geometry/__init__.py
+-rw-r--r--   0        0        0     1255 2023-08-10 12:03:43.317555 ipsuite-0.1.2/ipsuite/geometry/barycenter_coarse_grain.py
+-rw-r--r--   0        0        0     1236 2023-08-01 07:46:39.263824 ipsuite-0.1.2/ipsuite/geometry/graphs.py
+-rw-r--r--   0        0        0     1145 2023-11-03 15:52:05.880897 ipsuite-0.1.2/ipsuite/geometry/mapping.py
+-rw-r--r--   0        0        0     2140 2023-08-10 12:03:43.327555 ipsuite-0.1.2/ipsuite/geometry/unwrap.py
+-rw-r--r--   0        0        0      713 2024-04-16 14:19:55.044202 ipsuite-0.1.2/ipsuite/models/__init__.py
+-rw-r--r--   0        0        0      265 2023-08-10 12:03:43.337555 ipsuite-0.1.2/ipsuite/models/__init__.pyi
+-rw-r--r--   0        0        0     8310 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/models/apax.py
+-rw-r--r--   0        0        0     2598 2024-04-18 16:14:36.433113 ipsuite-0.1.2/ipsuite/models/base.py
+-rw-r--r--   0        0        0     2846 2024-03-06 21:47:01.635057 ipsuite-0.1.2/ipsuite/models/ensemble.py
+-rw-r--r--   0        0        0    10376 2024-04-18 16:28:18.444852 ipsuite-0.1.2/ipsuite/models/gap.py
+-rw-r--r--   0        0        0     4392 2024-04-18 16:28:18.454851 ipsuite-0.1.2/ipsuite/models/mace_model.py
+-rw-r--r--   0        0        0     6535 2024-04-18 16:28:18.454851 ipsuite-0.1.2/ipsuite/models/nequip.py
+-rw-r--r--   0        0        0     5705 2024-04-19 12:35:46.418721 ipsuite-0.1.2/ipsuite/nodes.py
+-rw-r--r--   0        0        0      189 2023-11-03 15:52:05.970896 ipsuite-0.1.2/ipsuite/project/__init__.py
+-rw-r--r--   0        0        0       97 2023-11-03 15:52:05.980896 ipsuite-0.1.2/ipsuite/static_data/__init__.py
+-rw-r--r--   0        0        0     1609 2023-05-30 11:28:15.843758 ipsuite-0.1.2/ipsuite/static_data/gap.jinja2
+-rw-r--r--   0        0        0     2300 2023-11-03 11:55:59.084040 ipsuite-0.1.2/ipsuite/static_data/lammps_npt.jinja2
+-rw-r--r--   0        0        0     2046 2023-06-12 08:03:57.512767 ipsuite-0.1.2/ipsuite/static_data/y_log.json
+-rw-r--r--   0        0        0      170 2024-04-16 14:19:55.044202 ipsuite-0.1.2/ipsuite/utils/__init__.py
+-rw-r--r--   0        0        0     2415 2023-11-21 17:49:15.516137 ipsuite-0.1.2/ipsuite/utils/ase_sim.py
+-rw-r--r--   0        0        0     6238 2024-04-16 14:19:55.044202 ipsuite-0.1.2/ipsuite/utils/combine.py
+-rw-r--r--   0        0        0      798 2024-04-16 14:19:55.054202 ipsuite-0.1.2/ipsuite/utils/docs.py
+-rw-r--r--   0        0        0     1954 2024-04-18 16:28:18.454851 ipsuite-0.1.2/ipsuite/utils/helpers.py
+-rw-r--r--   0        0        0      573 2023-11-03 15:52:06.020896 ipsuite-0.1.2/ipsuite/utils/logs.py
+-rw-r--r--   0        0        0      691 2023-04-05 16:53:50.539938 ipsuite-0.1.2/ipsuite/utils/md.py
+-rw-r--r--   0        0        0     2573 2024-04-19 12:35:46.418721 ipsuite-0.1.2/ipsuite/utils/metrics.py
+-rw-r--r--   0        0        0     3111 2024-04-19 12:58:49.034754 ipsuite-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 ipsuite-0.1.2/PKG-INFO
```

### Comparing `ipsuite-0.1.1/LICENSE` & `ipsuite-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/__init__.py` & `ipsuite-0.1.2/ipsuite/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The ipsuite package."""
+
 import importlib.metadata
 
 from ipsuite import (
     analysis,
     base,
     bootstrap,
     calculators,
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/__init__.py` & `ipsuite-0.1.2/ipsuite/analysis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,19 @@
     EnergyUncertaintyHistogram,
     ForcesHistogram,
     ForcesUncertaintyHistogram,
     StressHistogram,
 )
 from ipsuite.analysis.bond_stretch import BondStretchAnalyses
 from ipsuite.analysis.ensemble import ModelEnsembleAnalysis
+from ipsuite.analysis.md import AnalyseDensity
 from ipsuite.analysis.model import (
     BoxHeatUp,
     BoxScale,
+    CalibrationMetrics,
     ConnectivityCheck,
     EnergySpikeCheck,
     ForceAngles,
     ForceDecomposition,
     MDStability,
     NaNCheck,
     Prediction,
@@ -34,14 +36,15 @@
     "ForcesHistogram",
     "DipoleHistogram",
     "ModelEnsembleAnalysis",
     "PredictionMetrics",
     "ForceAngles",
     "RattleAnalysis",
     "Prediction",
+    "CalibrationMetrics",
     "BoxScale",
     "BoxHeatUp",
     "NaNCheck",
     "TemperatureCheck",
     "ConnectivityCheck",
     "EnergySpikeCheck",
     "MDStability",
@@ -50,8 +53,9 @@
     "AnalyseSingleForceSensitivity",
     "ForceDecomposition",
     "ThresholdCheck",
     "BondStretchAnalyses",
     "StressHistogram",
     "ForcesUncertaintyHistogram",
     "EnergyUncertaintyHistogram",
+    "AnalyseDensity",
 ]
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/bin_property.py` & `ipsuite-0.1.2/ipsuite/analysis/bin_property.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,43 +3,38 @@
 import numpy as np
 import pandas as pd
 import zntrack
 
 from ipsuite import base
 from ipsuite.analysis.model.math import decompose_stress_tensor
 from ipsuite.analysis.model.plots import get_histogram_figure
-from ipsuite.utils.helpers import get_deps_if_node
 
 
 class LabelHistogram(base.AnalyseAtoms):
     """Base class for creating histogram of a dataset.
 
     Parameters
     ----------
     data: list
         List of Atoms objects.
     bins: int
         Number of bins in the histogram.
     """
 
-    bins: int = zntrack.zn.params(None)
-    x_lim: tuple = zntrack.zn.params(None)
-    y_lim: tuple = zntrack.zn.params(None)
-    plots_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "plots")
-    labels_df: pd.DataFrame = zntrack.zn.plots()
+    bins: int = zntrack.params(None)
+    x_lim: tuple = zntrack.params(None)
+    y_lim: tuple = zntrack.params(None)
+    plots_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "plots")
+    labels_df: pd.DataFrame = zntrack.plots()
     datalabel: str = None
     xlabel: str = None
     ylabel: str = "Occurrences"
     logy_scale: bool = True
 
-    metrics: float = zntrack.zn.metrics()
-
-    def _post_init_(self):
-        """Load metrics - if available."""
-        self.data = get_deps_if_node(self.data, "atoms")
+    metrics: float = zntrack.metrics()
 
     def get_labels(self):
         raise NotImplementedError
 
     def get_hist(self):
         """Create a pandas dataframe from the given data."""
         labels = self.get_labels()
@@ -99,29 +94,29 @@
         labels = np.concatenate([x.get_forces() for x in self.data], axis=0)
         # compute magnitude of vector labels. Histogram works element wise for N-D Arrays
         labels = np.linalg.norm(labels, ord=2, axis=1)
         return labels
 
 
 class ForcesUncertaintyHistogram(LabelHistogram):
-    """Creates a histogram of all force labels contained in a dataset."""
+    """Creates a histogram of all force uncertainties in a prediction."""
 
     datalabel = "forces-uncertainty"
     xlabel = r"$F$ / eV/Ang"
 
     def get_labels(self):
         labels = np.concatenate(
             [x.calc.results["forces_uncertainty"] for x in self.data], axis=0
         )
         labels = np.linalg.norm(labels, ord=2, axis=1)
         return labels
 
 
 class EnergyUncertaintyHistogram(LabelHistogram):
-    """Creates a histogram of all force labels contained in a dataset."""
+    """Creates a histogram of all energy uncertainties in a prediction."""
 
     datalabel = "energy-uncertainty"
     xlabel = r"$F$ / eV/Ang"
 
     def get_labels(self):
         return np.reshape([x.calc.results["energy_uncertainty"] for x in self.data], (-1))
 
@@ -147,24 +142,20 @@
     ----------
     data: list
         List of Atoms objects.
     bins: int
         Number of bins in the histogram.
     """
 
-    bins: int = zntrack.zn.params(None)
-    plots_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "plots")
-    labels_df: pd.DataFrame = zntrack.zn.plots()
+    bins: int = zntrack.params(None)
+    plots_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "plots")
+    labels_df: pd.DataFrame = zntrack.plots()
     ylabel: str = "Occurrences"
     logy_scale: bool = True
 
-    def _post_init_(self):
-        """Load metrics - if available."""
-        self.data = get_deps_if_node(self.data, "atoms")
-
     def get_labels(self):
         labels = np.array([x.get_stress(voigt=False) for x in self.data])
         return labels
 
     def get_hist(self):
         """Create a pandas dataframe from the given data."""
         labels = self.get_labels()
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/bond_stretch.py` & `ipsuite-0.1.2/ipsuite/analysis/bond_stretch.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         used for the bond stretch analyses
     fig_size: (float, float)
         size of the plot
     """
 
     ase_calculator = zntrack.deps()
 
-    idxs = zntrack.zn.params()
-    r_min = zntrack.zn.params()
-    r_max = zntrack.zn.params()
-    n_steps = zntrack.zn.params()
-    data_id: typing.Optional[int] = zntrack.zn.params(0)
-    fig_size = zntrack.zn.params((10, 7))
+    idxs = zntrack.params()
+    r_min = zntrack.params()
+    r_max = zntrack.params()
+    n_steps = zntrack.params()
+    data_id: typing.Optional[int] = zntrack.params(0)
+    fig_size = zntrack.params((10, 7))
 
-    plots_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "plots")
+    plots_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "plots")
 
     def run(self):
         atoms_list = self.get_data()
 
         train_bond_length = []
         for struct in atoms_list:
             train_bond_length.append(struct.get_distance(self.idxs[0], self.idxs[1]))
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/ensemble.py` & `ipsuite-0.1.2/ipsuite/analysis/ensemble.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 import ase.calculators.singlepoint
 import matplotlib.pyplot as plt
 import numpy as np
 import zntrack
 
-from ipsuite import base, utils
+from ipsuite import base
 
 
 def plot_with_uncertainty(value, ylabel: str, xlabel: str, x=None, **kwargs) -> dict:
     """Parameters
     ----------
     value: data of shape (n, m) where n is the number of ensembles.
     x: optional x values of shape (m,)
@@ -53,25 +53,22 @@
     ----------
         models: list of models to ensemble
         data: list of ASE Atoms objects to evaluate against.
     """
 
     models: list = zntrack.deps()
 
-    normal_plot_path = zntrack.dvc.outs(zntrack.nwd / "normal_plot.png")
-    sorted_plot_path = zntrack.dvc.outs(zntrack.nwd / "sorted_plot.png")
-    histogram = zntrack.dvc.outs(zntrack.nwd / "histogram.png")
+    normal_plot_path = zntrack.outs_path(zntrack.nwd / "normal_plot.png")
+    sorted_plot_path = zntrack.outs_path(zntrack.nwd / "sorted_plot.png")
+    histogram = zntrack.outs_path(zntrack.nwd / "histogram.png")
 
-    prediction_list = zntrack.zn.outs()
-    predictions: typing.List[ase.Atoms] = zntrack.zn.outs()
+    prediction_list = zntrack.outs()
+    predictions: typing.List[ase.Atoms] = zntrack.outs()
 
-    bins: int = zntrack.zn.params(100)
-
-    def _post_init_(self):
-        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
+    bins: int = zntrack.params(100)
 
     def run(self):
         # TODO axis labels
         # TODO save indices
         # TODo rewrite this Node based on MLModel and then add a Analysis Node
         self.prediction_list = [model.predict(self.data[:]) for model in self.models]
 
@@ -91,15 +88,18 @@
         figures = self.get_plots()
         figures[0][0].savefig(self.normal_plot_path)
         figures[1][0].savefig(self.sorted_plot_path)
         figures[2].savefig(self.histogram)
 
     def get_plots(self):
         energy = np.stack(
-            [np.stack(x.get_potential_energy() for x in p) for p in self.prediction_list]
+            [
+                np.stack([x.get_potential_energy() for x in p])
+                for p in self.prediction_list
+            ]
         )
 
         figures = []
         # Plot the energy
         figures.append(
             plot_with_uncertainty(
                 energy, figsize=(10, 5), xlabel="data point", ylabel="Energy / a.u."
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/model/dynamics.py` & `ipsuite-0.1.2/ipsuite/analysis/model/dynamics.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,32 +44,29 @@
     factor: float, default = 0.001
         The 'np.linspace(0.0, stop, num) * factor'
     atom_id: int, default = 0
         The atom to pick from self.atoms as a starting point
     """
 
     model: models.MLModel = zntrack.deps()
-    model_outs = zntrack.dvc.outs(zntrack.nwd / "model/")
+    model_outs = zntrack.outs_path(zntrack.nwd / "model/")
 
-    logspace: bool = zntrack.zn.params(True)
-    stop: float = zntrack.zn.params(3.0)
-    factor: float = zntrack.zn.params(0.001)
-    num: int = zntrack.zn.params(100)
+    logspace: bool = zntrack.params(True)
+    stop: float = zntrack.params(3.0)
+    factor: float = zntrack.params(0.001)
+    num: int = zntrack.params(100)
 
-    seed: int = zntrack.zn.params(1234)
-    energies: pd.DataFrame = zntrack.zn.plots(
+    seed: int = zntrack.params(1234)
+    energies: pd.DataFrame = zntrack.plots(
         # x="x",
         # y="y",
         # x_label="stdev of randomly displaced atoms",
         # y_label="predicted energy",
     )
 
-    def post_init(self):
-        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
-
     def run(self):
         self.model_outs.mkdir(parents=True, exist_ok=True)
         (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
 
         if self.logspace:
             stdev_space = (
                 np.logspace(start=0.0, stop=self.stop, num=self.num) * self.factor
@@ -108,33 +105,30 @@
     stop: float, default = 1.0
         The stop value for the generated space of stdev points
     num: int, default = 100
         The size of the generated space of stdev points
     """
 
     model: models.MLModel = zntrack.deps()
-    model_outs = zntrack.dvc.outs(zntrack.nwd / "model")
+    model_outs = zntrack.outs_path(zntrack.nwd / "model")
     mapping: base.Mapping = zntrack.deps(None)
 
-    stop: float = zntrack.zn.params(2.0)
-    num: int = zntrack.zn.params(100)
-    start: float = zntrack.zn.params(1)
+    stop: float = zntrack.params(2.0)
+    num: int = zntrack.params(100)
+    start: float = zntrack.params(1)
 
-    plot = zntrack.dvc.outs(zntrack.nwd / "energy.png")
+    plot = zntrack.outs_path(zntrack.nwd / "energy.png")
 
-    energies: pd.DataFrame = zntrack.zn.plots(
+    energies: pd.DataFrame = zntrack.plots(
         x="x",
         y="y",
         x_label="Scale factor of the initial cell",
         y_label="predicted energy",
     )
 
-    def _post_init_(self):
-        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
-
     def run(self):
         self.model_outs.mkdir(parents=True, exist_ok=True)
         (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
         scale_space = np.linspace(start=self.start, stop=self.stop, num=self.num)
 
         original_atoms = self.get_data()
         cell = original_atoms.copy().cell
@@ -194,29 +188,29 @@
     time_step: float, default = 0.5 fs
         time step of the simulation
     friction: float, default = 0.01
         langevin friction
 
     """
 
-    start_temperature: float = zntrack.zn.params()
-    stop_temperature: float = zntrack.zn.params()
-    steps: int = zntrack.zn.params()
-    time_step: float = zntrack.zn.params(0.5)
-    friction = zntrack.zn.params()
-    repeat = zntrack.zn.params((1, 1, 1))
+    start_temperature: float = zntrack.params()
+    stop_temperature: float = zntrack.params()
+    steps: int = zntrack.params()
+    time_step: float = zntrack.params(0.5)
+    friction = zntrack.params()
+    repeat = zntrack.params((1, 1, 1))
 
-    max_temperature: float = zntrack.zn.params(None)
+    max_temperature: float = zntrack.params(None)
 
-    flux_data = zntrack.zn.plots()
+    flux_data = zntrack.plots()
 
     model = zntrack.deps()
-    model_outs = zntrack.dvc.outs(zntrack.nwd / "model")
+    model_outs = zntrack.outs_path(zntrack.nwd / "model")
 
-    plots = zntrack.dvc.outs(zntrack.nwd / "temperature.png")
+    plots = zntrack.outs_path(zntrack.nwd / "temperature.png")
 
     def get_atoms(self) -> ase.Atoms:
         atoms: ase.Atoms = self.get_data()
         return atoms.repeat(self.repeat)
 
     def plot_temperature(self):
         fig, ax = plt.subplots()
@@ -292,15 +286,15 @@
 
 
 def run_stability_nve(
     atoms: ase.Atoms,
     time_step: float,
     max_steps: int,
     init_temperature: float,
-    checks: list[base.CheckBase],
+    checks: list[base.Check],
     save_last_n: int,
     rng: typing.Optional[np.random.Generator] = None,
 ) -> typing.Tuple[int, list[ase.Atoms]]:
     """
     Runs an NVE trajectory for a single configuration until either max_steps
     is reached or one of the checks fails.
     """
@@ -362,26 +356,26 @@
     distribution.
     save_last_n: how many configurations before the instability should be saved
     bins: number of bins in the histogram
     seed: seed for the MaxwellBoltzmann distribution
     """
 
     model = zntrack.deps()
-    model_outs = zntrack.dvc.outs(zntrack.nwd / "model_outs")
-    max_steps: int = zntrack.zn.params()
+    model_outs = zntrack.outs_path(zntrack.nwd / "model_outs")
+    max_steps: int = zntrack.params()
     checks: list[zntrack.Node] = zntrack.deps()
-    time_step: float = zntrack.zn.params(0.5)
-    initial_temperature: float = zntrack.zn.params(300)
-    save_last_n: int = zntrack.zn.params(1)
-    bins: int = zntrack.zn.params(None)
-    seed: int = zntrack.zn.params(0)
-
-    traj_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "trajectory.h5")
-    plots_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "plots")
-    stable_steps_df: pd.DataFrame = zntrack.zn.plots()
+    time_step: float = zntrack.params(0.5)
+    initial_temperature: float = zntrack.params(300)
+    save_last_n: int = zntrack.params(1)
+    bins: int = zntrack.params(None)
+    seed: int = zntrack.params(0)
+
+    traj_file: pathlib.Path = zntrack.outs_path(zntrack.nwd / "structures.h5")
+    plots_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "plots")
+    stable_steps_df: pd.DataFrame = zntrack.plots()
 
     @property
     def atoms(self) -> typing.List[ase.Atoms]:
         def file_handle(filename):
             file = self.state.fs.open(filename, "rb")
             return h5py.File(file)
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/model/dynamics_checks.py` & `ipsuite-0.1.2/ipsuite/analysis/model/dynamics_checks.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import zntrack
 from ase.neighborlist import build_neighbor_list
 
 from ipsuite import base
 from ipsuite.utils.ase_sim import get_energy
 
 
-class NaNCheck(base.CheckBase):
+class NaNCheck(base.Check):
     """Check Node to see whether positions, energies or forces become NaN
     during a simulation.
     """
 
     def initialize(self, atoms: ase.Atoms) -> None:
         self.is_initialized = True
 
@@ -32,15 +32,15 @@
             )
             return True
         else:
             self.status = "No NaN occurred"
             return False
 
 
-class ConnectivityCheck(base.CheckBase):
+class ConnectivityCheck(base.Check):
     """Check to see whether the covalent connectivity of the system
     changes during a simulation.
     The connectivity is based on ASE's natural cutoffs.
 
     """
 
     def _post_init_(self) -> None:
@@ -64,26 +64,26 @@
             )
             return True
         else:
             self.status = "covalent connectivity of the system is intact"
             return False
 
 
-class EnergySpikeCheck(base.CheckBase):
+class EnergySpikeCheck(base.Check):
     """Check to see whether the potential energy of the system has fallen
     below a minimum or above a maximum threshold.
 
     Attributes
     ----------
     min_factor: Simulation stops if `E(current) > E(initial) * min_factor`
     max_factor: Simulation stops if `E(current) < E(initial) * max_factor`
     """
 
-    min_factor: float = zntrack.zn.params(0.5)
-    max_factor: float = zntrack.zn.params(2.0)
+    min_factor: float = zntrack.params(0.5)
+    max_factor: float = zntrack.params(2.0)
 
     def _post_init_(self) -> None:
         self.max_energy = None
         self.min_energy = None
 
     def initialize(self, atoms: ase.Atoms) -> None:
         epot = atoms.get_potential_energy()
@@ -107,24 +107,24 @@
             )
             return True
         else:
             self.status = "No energy spike occurred"
             return False
 
 
-class TemperatureCheck(base.CheckBase):
+class TemperatureCheck(base.Check):
     """Calculate and check teperature during a MD simulation
 
     Attributes
     ----------
     max_temperature: float
         maximum temperature, when reaching it simulation will be stopped
     """
 
-    max_temperature: float = zntrack.zn.params(10000.0)
+    max_temperature: float = zntrack.params(10000.0)
 
     def initialize(self, atoms: ase.Atoms) -> None:
         self.is_initialized = True
 
     def check(self, atoms):
         self.temperature, _ = get_energy(atoms)
 
@@ -138,15 +138,15 @@
             self.status = (
                 f"Temperature Check: T {self.temperature} K <"
                 f"T_max {self.max_temperature} K"
             )
             return False
 
 
-class ThresholdCheck(base.CheckBase):
+class ThresholdCheck(base.Check):
     """Calculate and check a given threshold and std during a MD simulation
 
     Compute the standard deviation of the selected property.
     If the property is off by more than a selected amount from the
     mean, the simulation will be stopped.
     Furthermore, the simulation will be stopped if the property
     exceeds a threshold value.
@@ -167,20 +167,20 @@
         Minimum number of steps to average over before checking the standard deviation.
         Also minimum number of steps to run, before the simulation can be stopped.
     larger_only: bool, optional
         Only check the standard deviation of points that are larger than the mean.
         E.g. useful for uncertainties, where a lower uncertainty is not a problem.
     """
 
-    value: str = zntrack.zn.params()
-    max_std: float = zntrack.zn.params(None)
-    window_size: int = zntrack.zn.params(500)
-    max_value: float = zntrack.zn.params(None)
-    minimum_window_size: int = zntrack.zn.params(1)
-    larger_only: bool = zntrack.zn.params(False)
+    value: str = zntrack.params()
+    max_std: float = zntrack.params(None)
+    window_size: int = zntrack.params(500)
+    max_value: float = zntrack.params(None)
+    minimum_window_size: int = zntrack.params(1)
+    larger_only: bool = zntrack.params(False)
 
     def _post_init_(self):
         if self.max_std is None and self.max_value is None:
             raise ValueError("Either max_std or max_value must be set")
 
     def _post_load_(self) -> None:
         self.values = collections.deque(maxlen=self.window_size)
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/model/math.py` & `ipsuite-0.1.2/ipsuite/analysis/model/math.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/analysis/model/plots.py` & `ipsuite-0.1.2/ipsuite/analysis/model/plots.py`

 * *Files 19% similar despite different names*

```diff
@@ -63,28 +63,49 @@
     -------
     plt.Figure
 
     """
     sns.set()
     fig, ax = plt.subplots(figsize=figsize)
     ax.plot(true, true, color="grey", zorder=0)  # plot the diagonal in the background
-    bins = 500 if (len(true) / 10) > 500 else int(len(true) * 0.1)
-    if bins < 20:
+    bins = 25
+    if true.shape[0] < 20:
         # don't use density for very small datasets
         ax.scatter(true, prediction, marker="x", s=20.0, label=datalabel)
     else:
         density_scatter(
             ax, true, prediction, bins=bins, marker="x", s=20.0, label=datalabel
         )
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.legend()
     return fig
 
 
+def get_cdf_figure(x, y, figsize: tuple = (10, 7)):
+    """Computes the cumulative distribution function of x and y,
+    then creates a calibration curve for the two variables.
+    """
+    idxs = np.argsort(x)
+    x_sorted = x[idxs]
+    y_sorted = y[np.argsort(y)]
+    x_scaleshift = x_sorted - np.min(x_sorted)
+    x_scaleshift /= np.max(x_scaleshift)
+    y_scaleshift = y_sorted - np.min(y_sorted)
+    y_scaleshift /= np.max(y_scaleshift)
+
+    fig, ax = plt.subplots(figsize=figsize)
+    diag = np.linspace(0, 1.0, 2)
+    ax.plot(diag, diag, "grey", alpha=0.5)
+    ax.plot(x_scaleshift, y_scaleshift)
+    ax.set_xlabel("expected CDF")
+    ax.set_ylabel("observed CDF")
+    return fig
+
+
 def get_hist(data, label, xlabel, ylabel) -> typing.Tuple[plt.Figure, plt.Axes]:
     fig, ax = plt.subplots()
 
     sns.histplot(
         data,
         ax=ax,
         stat="percent",
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/model/predict.py` & `ipsuite-0.1.2/ipsuite/analysis/model/predict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pathlib
 
 import ase
 import numpy as np
-import pandas as pd
 import tqdm
 import zntrack
 from ase.calculators.singlepoint import PropertyNotImplementedError
+from scipy import stats
 
 from ipsuite import base, models, utils
 from ipsuite.analysis.model.math import decompose_stress_tensor, force_decomposition
-from ipsuite.analysis.model.plots import get_figure, get_hist
+from ipsuite.analysis.model.plots import get_cdf_figure, get_figure, get_hist
 from ipsuite.geometry import BarycenterMapping
 from ipsuite.utils.ase_sim import freeze_copy_atoms
 
 
 class Prediction(base.ProcessAtoms):
     """Create and Save the predictions from model on atoms.
 
@@ -45,256 +45,294 @@
                     ValueError,
                 ):  # required for nequip, GAP
                     pass
 
             self.atoms.append(freeze_copy_atoms(atoms))
 
 
-class PredictionMetrics(base.AnalyseProcessAtoms):
+class PredictionMetrics(base.ComparePredictions):
     """Analyse the Models Prediction on standard metrics.
 
     Units are given in:
     - energy: meV/atom
     - forces: meV/Å
     - stress: eV/Å^3
     """
 
-    energy_df_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "energy_df.csv")
-    forces_df_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "forces_df.csv")
-    stress_df_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "stress_df.csv")
-    stress_hydrostatic_df_file: pathlib.Path = zntrack.dvc.outs(
-        zntrack.nwd / "stress_hydrostatic_df.csv"
-    )
-    stress_deviatoric_df_file: pathlib.Path = zntrack.dvc.outs(
-        zntrack.nwd / "stress_deviatoric_df.csv"
-    )
-
-    energy: dict = zntrack.zn.metrics()
-    forces: dict = zntrack.zn.metrics()
-    stress: dict = zntrack.zn.metrics()
-    hydro_stress: dict = zntrack.zn.metrics()
-    deviat_stress: dict = zntrack.zn.metrics()
-
-    plots_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "plots")
-
-    energy_df: pd.DataFrame
-    forces_df: pd.DataFrame
-    stress_df: pd.DataFrame
-    stress_hydro_df: pd.DataFrame
-    stress_deviat_df: pd.DataFrame
+    data_file = zntrack.outs_path(zntrack.nwd / "data.npz")
+
+    energy: dict = zntrack.metrics()
+    forces: dict = zntrack.metrics()
+    stress: dict = zntrack.metrics()
+    stress_hydro: dict = zntrack.metrics()
+    stress_deviat: dict = zntrack.metrics()
+
+    plots_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "plots")
+
+    def _post_init_(self):
+        self.content = {}
 
     def _post_load_(self):
         """Load metrics - if available."""
         try:
-            self.energy_df = pd.read_csv(self.energy_df_file)
-        except FileNotFoundError:
-            self.energy_df = pd.DataFrame({})
-        try:
-            self.forces_df = pd.read_csv(self.forces_df_file)
-        except FileNotFoundError:
-            self.forces_df = pd.DataFrame({})
-        try:
-            self.stress_df = pd.read_csv(self.stress_df_file)
-            self.stress_hydro_df = pd.read_csv(self.stress_hydrostatic_df_file)
-            self.stress_deviat_df = pd.read_csv(self.stress_deviatoric_df_file)
+            with self.state.fs.open(self.data_file, "rb") as f:
+                self.content = dict(np.load(f))
         except FileNotFoundError:
-            self.stress_df = pd.DataFrame({})
-            self.stress_hydro_df = pd.DataFrame({})
-            self.stress_deviat_df = pd.DataFrame({})
-
-    def get_dataframes(self):
-        """Create a pandas dataframe from the given data."""
-        true_data, pred_data = self.get_data()
-
-        self.energy_df = pd.DataFrame(
-            {
-                "true": (
-                    np.array([x.get_potential_energy() / len(x) for x in true_data])
-                    * 1000
-                ),
-                "prediction": (
-                    np.array([x.get_potential_energy() / len(x) for x in pred_data])
-                    * 1000
-                ),
-            }
-        )
+            self.content = {}
 
-        try:
-            true_forces = [np.reshape(x.get_forces(), (-1, 3)) for x in true_data]
+    def get_data(self):
+        """Create dict of all data."""
+        true_keys = self.x[0].calc.results.keys()
+        pred_keys = self.y[0].calc.results.keys()
+
+        energy_true = [x.get_potential_energy() / len(x) for x in self.x]
+        energy_true = np.array(energy_true) * 1000
+        self.content["energy_true"] = energy_true
+
+        energy_prediction = [x.get_potential_energy() / len(x) for x in self.y]
+        energy_prediction = np.array(energy_prediction) * 1000
+        self.content["energy_pred"] = energy_prediction
+
+        if "forces" in true_keys and "forces" in pred_keys:
+            true_forces = [x.get_forces() for x in self.x]
             true_forces = np.concatenate(true_forces, axis=0) * 1000
+            self.content["forces_true"] = np.reshape(true_forces, (-1,))
 
-            pred_forces = [np.reshape(x.get_forces(), (-1, 3)) for x in pred_data]
+            pred_forces = [x.get_forces() for x in self.y]
             pred_forces = np.concatenate(pred_forces, axis=0) * 1000
+            self.content["forces_pred"] = np.reshape(pred_forces, (-1,))
 
-            self.forces_df = pd.DataFrame(
-                {
-                    "true": np.linalg.norm(true_forces, axis=-1),
-                    "true_x": true_forces[:, 0],
-                    "true_y": true_forces[:, 1],
-                    "true_z": true_forces[:, 2],
-                    "prediction": np.linalg.norm(pred_forces, axis=-1),
-                    "prediction_x": pred_forces[:, 0],
-                    "prediction_y": pred_forces[:, 1],
-                    "prediction_z": pred_forces[:, 2],
-                }
-            )
-        except PropertyNotImplementedError:
-            self.forces_df = pd.DataFrame({})
-
-        try:
-            true_stress = [x.get_stress(voigt=False) for x in true_data]
-            pred_stress = [x.get_stress(voigt=False) for x in pred_data]
+        if "stress" in true_keys and "stress" in pred_keys:
+            true_stress = np.array([x.get_stress(voigt=False) for x in self.x])
+            pred_stress = np.array([x.get_stress(voigt=False) for x in self.y])
             hydro_true, deviat_true = decompose_stress_tensor(true_stress)
             hydro_pred, deviat_pred = decompose_stress_tensor(pred_stress)
 
-            true_stress = np.reshape(true_stress, -1)
-            pred_stress = np.reshape(pred_stress, -1)
-            hydro_true = np.reshape(hydro_true, -1)
-            deviat_true = np.reshape(deviat_true, -1)
-            hydro_pred = np.reshape(hydro_pred, -1)
-            deviat_pred = np.reshape(deviat_pred, -1)
-
-            self.stress_df = pd.DataFrame(
-                {
-                    "true": true_stress,
-                    "prediction": pred_stress,
-                }
-            )
-            self.stress_hydro_df = pd.DataFrame(
-                {
-                    "true": hydro_true,
-                    "prediction": hydro_pred,
-                }
-            )
-            self.stress_deviat_df = pd.DataFrame(
-                {
-                    "true": deviat_true,
-                    "prediction": deviat_pred,
-                }
-            )
-        except PropertyNotImplementedError:
-            self.stress_df = pd.DataFrame({})
-            self.stress_hydro_df = pd.DataFrame({})
-            self.stress_deviat_df = pd.DataFrame({})
+            self.content["stress_true"] = np.reshape(true_stress, (-1,))
+            self.content["stress_pred"] = np.reshape(pred_stress, (-1,))
+            self.content["stress_hydro_true"] = np.reshape(hydro_true, (-1,))
+            self.content["stress_hydro_pred"] = np.reshape(hydro_pred, (-1,))
+            self.content["stress_deviat_true"] = np.reshape(deviat_true, (-1,))
+            self.content["stress_deviat_pred"] = np.reshape(deviat_pred, (-1,))
 
     def get_metrics(self):
         """Update the metrics."""
         self.energy = utils.metrics.get_full_metrics(
-            np.array(self.energy_df["true"]), np.array(self.energy_df["prediction"])
+            self.content["energy_true"], self.content["energy_pred"]
         )
 
-        if not self.forces_df.empty:
+        if "forces_true" in self.content.keys():
             self.forces = utils.metrics.get_full_metrics(
-                np.array(self.forces_df["true"]), np.array(self.forces_df["prediction"])
+                self.content["forces_true"], self.content["forces_pred"]
             )
         else:
             self.forces = {}
 
-        if not self.stress_df.empty:
+        if "stress_true" in self.content.keys():
             self.stress = utils.metrics.get_full_metrics(
-                np.array(self.stress_df["true"]), np.array(self.stress_df["prediction"])
+                self.content["stress_true"], self.content["stress_pred"]
+            )
+            self.stress_hydro = utils.metrics.get_full_metrics(
+                self.content["stress_hydro_true"], self.content["stress_hydro_pred"]
             )
-            self.hydro_stress = utils.metrics.get_full_metrics(
-                np.array(self.stress_hydro_df["true"]),
-                np.array(self.stress_hydro_df["prediction"]),
-            )
-            self.deviat_stress = utils.metrics.get_full_metrics(
-                np.array(self.stress_deviat_df["true"]),
-                np.array(self.stress_deviat_df["prediction"]),
+            self.stress_deviat = utils.metrics.get_full_metrics(
+                self.content["stress_deviat_true"], self.content["stress_deviat_pred"]
             )
         else:
             self.stress = {}
-            self.hydro_stress = {}
-            self.deviat_stress = {}
+            self.stress_hydro = {}
+            self.stress_deviat = {}
 
     def get_plots(self, save=False):
         """Create figures for all available data."""
         self.plots_dir.mkdir(exist_ok=True)
 
         energy_plot = get_figure(
-            self.energy_df["true"],
-            self.energy_df["prediction"],
+            self.content["energy_true"],
+            self.content["energy_pred"],
             datalabel=f"MAE: {self.energy['mae']:.2f} meV/atom",
             xlabel=r"$ab~initio$ energy $E$ / meV/atom",
             ylabel=r"predicted energy $E$ / meV/atom",
         )
         if save:
             energy_plot.savefig(self.plots_dir / "energy.png")
 
-        if not self.forces_df.empty:
+        if "forces_true" in self.content:
+            xlabel = r"$ab~initio$ force components per atom $|F|$ / meV$ \cdot \AA^{-1}$"
+            ylabel = r"predicted force components per atom $|F|$ / meV$ \cdot \AA^{-1}$"
             forces_plot = get_figure(
-                self.forces_df["true_x"]
-                + self.forces_df["true_y"]
-                + self.forces_df["true_z"],
-                self.forces_df["prediction_x"]
-                + self.forces_df["prediction_y"]
-                + self.forces_df["prediction_z"],
+                self.content["forces_true"],
+                self.content["forces_pred"],
                 datalabel=rf"MAE: {self.forces['mae']:.2f} meV$ / \AA$",
-                xlabel=(
-                    r"$ab~initio$ magnitude of force per atom $|F|$ / meV$ \cdot"
-                    r" \AA^{-1}$"
-                ),
-                ylabel=(
-                    r"predicted magnitude of force per atom $|F|$ / meV$ \cdot \AA^{-1}$"
-                ),
+                xlabel=xlabel,
+                ylabel=ylabel,
             )
             if save:
                 forces_plot.savefig(self.plots_dir / "forces.png")
 
-        if not self.stress_df.empty:
+        if "stress_true" in self.content:
+            s_true = self.content["stress_true"]
+            s_pred = self.content["stress_pred"]
+            shydro_true = self.content["stress_hydro_true"]
+            shydro_pred = self.content["stress_hydro_pred"]
+            sdeviat_true = self.content["stress_deviat_true"]
+            sdeviat_pred = self.content["stress_deviat_pred"]
+
             stress_plot = get_figure(
-                self.stress_df["true"],
-                self.stress_df["prediction"],
+                s_true,
+                s_pred,
                 datalabel=rf"Max: {self.stress['max']:.4f}",
                 xlabel=r"$ab~initio$ stress",
                 ylabel=r"predicted stress",
             )
-
             hydrostatic_stress_plot = get_figure(
-                self.stress_hydro_df["true"],
-                self.stress_hydro_df["prediction"],
-                datalabel=rf"Max: {self.hydro_stress['max']:.4f}",
+                shydro_true,
+                shydro_pred,
+                datalabel=rf"Max: {self.stress_hydro['max']:.4f}",
                 xlabel=r"$ab~initio$ hydrostatic stress",
                 ylabel=r"predicted hydrostatic stress",
             )
             deviatoric_stress_plot = get_figure(
-                self.stress_deviat_df["true"],
-                self.stress_deviat_df["prediction"],
-                datalabel=rf"Max: {self.deviat_stress['max']:.4f}",
+                sdeviat_true,
+                sdeviat_pred,
+                datalabel=rf"Max: {self.stress_deviat['max']:.4f}",
                 xlabel=r"$ab~initio$ deviatoric stress",
                 ylabel=r"predicted deviatoric stress",
             )
             if save:
                 stress_plot.savefig(self.plots_dir / "stress.png")
                 hydrostatic_stress_plot.savefig(self.plots_dir / "hydrostatic_stress.png")
                 deviatoric_stress_plot.savefig(self.plots_dir / "deviatoric_stress.png")
 
     def run(self):
         self.nwd.mkdir(exist_ok=True, parents=True)
-        self.get_dataframes()
+        self.get_data()
+        np.savez(self.data_file, **self.content)
         self.get_metrics()
         self.get_plots(save=True)
 
-        self.energy_df.to_csv(self.energy_df_file)
-        self.forces_df.to_csv(self.forces_df_file)
-        self.stress_df.to_csv(self.stress_df_file)
-        self.stress_hydro_df.to_csv(self.stress_hydrostatic_df_file)
-        self.stress_deviat_df.to_csv(self.stress_deviatoric_df_file)
+
+class CalibrationMetrics(base.ComparePredictions):
+    """Analyse the calibration of a models uncertainty estimate."""
+
+    data_file = zntrack.outs_path(zntrack.nwd / "data.npz")
+    energy: dict = zntrack.metrics()
+    forces: dict = zntrack.metrics()
+
+    plots_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "plots")
+
+    def _post_init_(self):
+        self.content = {}
+
+    def _post_load_(self):
+        """Load metrics - if available."""
+        try:
+            with self.state.fs.open(self.data_file, "rb") as f:
+                self.content = dict(np.load(f))
+        except FileNotFoundError:
+            self.content = {}
+
+    def get_data(self):
+        """Create dict of all data."""
+        true_keys = self.x[0].calc.results.keys()
+        pred_keys = self.y[0].calc.results.keys()
+
+        energy_true = [a.get_potential_energy() / len(a) for a in self.x]
+        energy_true = np.array(energy_true) * 1000
+        energy_pred = [a.get_potential_energy() / len(a) for a in self.y]
+        energy_pred = np.array(energy_pred) * 1000
+        self.content["energy_err"] = np.abs(energy_true - energy_pred)
+
+        energy_uncertainty = [
+            a.calc.results["energy_uncertainty"] / len(a) for a in self.y
+        ]
+        energy_uncertainty = np.array(energy_uncertainty) * 1000
+        self.content["energy_unc"] = energy_uncertainty
+
+        if "forces" in true_keys and "forces_uncertainty" in pred_keys:
+            true_forces = [a.get_forces() for a in self.x]
+            true_forces = np.concatenate(true_forces, axis=0) * 1000
+            pred_forces = [a.get_forces() for a in self.y]
+            pred_forces = np.concatenate(pred_forces, axis=0) * 1000
+            forces_uncertainty = [x.calc.results["forces_uncertainty"] for x in self.y]
+            forces_uncertainty = np.concatenate(forces_uncertainty, axis=0) * 1000
+
+            self.content["forces_err"] = np.abs(true_forces - pred_forces)
+            self.content["forces_unc"] = forces_uncertainty
+
+    def get_metrics(self):
+        """Update the metrics."""
+        e_err = self.content["energy_err"]
+        e_unc = self.content["energy_unc"]
+        pearsonr = stats.pearsonr(e_err, e_unc)[0]
+        self.energy = {"pearsonr": pearsonr}
+
+        if "forces_err" in self.content.keys():
+            f_err = np.reshape(self.content["forces_err"], (-1,))
+            f_unc = np.reshape(self.content["forces_unc"], (-1,))
+            self.forces = {"pearsonr": stats.pearsonr(f_err, f_unc)[0]}
+        else:
+            self.forces = {}
+
+    def get_plots(self, save=False):
+        """Create figures for all available data."""
+        self.plots_dir.mkdir(exist_ok=True)
+
+        energy_plot = get_figure(
+            self.content["energy_unc"],
+            self.content["energy_err"],
+            datalabel=rf"Pearson: {self.energy['pearsonr']:.4f}",
+            xlabel=r"energy uncertainty $\sigma$ / meV/atom",
+            ylabel=r"energy error $\Delta E$ / meV/atom",
+        )
+        energy_cdf_plot = get_cdf_figure(
+            self.content["energy_err"],
+            self.content["energy_unc"],
+        )
+        if save:
+            energy_plot.savefig(self.plots_dir / "energy.png")
+            energy_cdf_plot.savefig(self.plots_dir / "energy_cdf.png")
+
+        if "forces_err" in self.content:
+            xlabel = r"force uncertainty per atom $\sigma$ / meV$ \cdot \AA^{-1}$"
+            ylabel = r"force components error per atom $\Delta F$ / meV$ \cdot \AA^{-1}$"
+            f_err = np.reshape(self.content["forces_err"], (-1,))
+            f_unc = np.reshape(self.content["forces_unc"], (-1,))
+            forces_plot = get_figure(
+                f_unc,
+                f_err,
+                datalabel=rf"Pearson: {self.forces['pearsonr']:.4f}",
+                xlabel=xlabel,
+                ylabel=ylabel,
+            )
+            forces_cdf_plot = get_cdf_figure(
+                f_err,
+                f_unc,
+            )
+            if save:
+                forces_plot.savefig(self.plots_dir / "forces.png")
+                forces_cdf_plot.savefig(self.plots_dir / "forces_cdf.png")
+
+    def run(self):
+        self.nwd.mkdir(exist_ok=True, parents=True)
+        self.get_data()
+        np.savez(self.data_file, **self.content)
+        self.get_metrics()
+        self.get_plots(save=True)
 
 
-class ForceAngles(base.AnalyseProcessAtoms):
+class ForceAngles(base.ComparePredictions):
     plot: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "angle.png")
     log_plot: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "angle_ylog.png")
 
     angles: dict = zntrack.zn.metrics()
 
     def run(self):
-        true_data, pred_data = self.get_data()
-        true_forces = np.reshape([x.get_forces() for x in true_data], (-1, 3))
-        pred_forces = np.reshape([x.get_forces() for x in pred_data], (-1, 3))
+        true_forces = np.reshape([a.get_forces() for a in self.x], (-1, 3))
+        pred_forces = np.reshape([a.get_forces() for a in self.y], (-1, 3))
 
         angles = utils.metrics.get_angles(true_forces, pred_forces)
 
         self.angles = {
             "rmse": utils.metrics.calculate_l_p_norm(np.zeros_like(angles), angles, p=2),
             "lp4": utils.metrics.calculate_l_p_norm(np.zeros_like(angles), angles, p=4),
             "max": utils.metrics.maximum_error(np.zeros_like(angles), angles),
@@ -308,15 +346,15 @@
             ylabel="Probability / %",
         )
         fig.savefig(self.plot)
         ax.set_yscale("log")
         fig.savefig(self.log_plot)
 
 
-class ForceDecomposition(base.AnalyseProcessAtoms):
+class ForceDecomposition(base.ComparePredictions):
     """Node for decomposing forces in a system of molecular units into
     translational, rotational and vibrational components.
 
     The implementation follows the method described in
     https://doi.org/10.26434/chemrxiv-2022-l4tb9
 
 
@@ -426,39 +464,38 @@
                 self.wasserstein_distance[label][part] = wasserstein_distance(
                     true_bins[0], pred_bins[0]
                 )
 
         fig.savefig(self.histogram_plt, bbox_inches="tight")
 
     def run(self):
-        true_atoms, pred_atoms = self.get_data()
         mapping = BarycenterMapping(data=None)
         # TODO make the force_decomposition return full forces
         # TODO check if you sum the forces they yield the full forces
         # TODO make mapping a 'zn.nodes' with Mapping(species="BF4")
         #  maybe allow smiles and enumeration 0, 1, ...
 
         self.true_forces = {"all": [], "trans": [], "rot": [], "vib": []}
         self.pred_forces = {"all": [], "trans": [], "rot": [], "vib": []}
 
-        for atom in tqdm.tqdm(true_atoms, ncols=70):
+        for atom in tqdm.tqdm(self.x, ncols=70):
             atom_trans_forces, atom_rot_forces, atom_vib_forces = force_decomposition(
                 atom, mapping
             )
             self.true_forces["all"].append(atom.get_forces())
             self.true_forces["trans"].append(atom_trans_forces)
             self.true_forces["rot"].append(atom_rot_forces)
             self.true_forces["vib"].append(atom_vib_forces)
 
         self.true_forces["all"] = np.concatenate(self.true_forces["all"]) * 1000
         self.true_forces["trans"] = np.concatenate(self.true_forces["trans"]) * 1000
         self.true_forces["rot"] = np.concatenate(self.true_forces["rot"]) * 1000
         self.true_forces["vib"] = np.concatenate(self.true_forces["vib"]) * 1000
 
-        for atom in tqdm.tqdm(pred_atoms, ncols=70):
+        for atom in tqdm.tqdm(self.y, ncols=70):
             atom_trans_forces, atom_rot_forces, atom_vib_forces = force_decomposition(
                 atom, mapping
             )
             self.pred_forces["all"].append(atom.get_forces())
             self.pred_forces["trans"].append(atom_trans_forces)
             self.pred_forces["rot"].append(atom_rot_forces)
             self.pred_forces["vib"].append(atom_vib_forces)
```

### Comparing `ipsuite-0.1.1/ipsuite/analysis/sensitivity.py` & `ipsuite-0.1.2/ipsuite/analysis/sensitivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     ax.set_aspect(aspect)
 
 
 class MoveSingleParticle(base.IPSNode):
     """Move a single particle in a given direction."""
 
     atoms_list = zntrack.deps()
-    atoms_list_id = zntrack.zn.params(0)  # the atoms object in the atoms list
-    atom_id = zntrack.zn.params(0)  # the atom id to move
-    scale = zntrack.zn.params(0.5)  # the standard deviation of the normal distribution
-    seed = zntrack.zn.params(1234)
+    atoms_list_id = zntrack.params(0)  # the atoms object in the atoms list
+    atom_id = zntrack.params(0)  # the atom id to move
+    scale = zntrack.params(0.5)  # the standard deviation of the normal distribution
+    seed = zntrack.params(1234)
 
-    samples = zntrack.zn.params(10)  # how many samples to take
+    samples = zntrack.params(10)  # how many samples to take
 
-    atoms: list = zntrack.zn.outs()
-    atoms_path = zntrack.dvc.outs(zntrack.nwd / "atoms")
+    atoms: list = zntrack.outs()
+    atoms_path = zntrack.outs_path(zntrack.nwd / "atoms")
 
     def run(self):
         """ZnTrack run method."""
         self.atoms = []
         np.random.seed(self.seed)
         self.atoms_path.mkdir(parents=True, exist_ok=True)
         for idx in range(self.samples):
@@ -63,15 +63,15 @@
 
     def get_atom_filenames(self):
         return [str(self.atoms_path / f"atoms_{idx}.xyz") for idx in range(self.samples)]
 
 
 class AnalyseGlobalForceSensitivity(base.IPSNode):
     atoms_list = zntrack.deps()
-    plots = zntrack.dvc.outs(zntrack.nwd / "plots")
+    plots = zntrack.outs_path(zntrack.nwd / "plots")
 
     def run(self):
         # assume all atoms have only a single particle changed
         r_ij, d_ij = ase.geometry.get_distances(self.atoms_list[-1].positions)
 
         forces = np.stack([atoms.get_forces() for atoms in self.atoms_list])
         std_forces = np.std(forces, axis=0)
@@ -104,20 +104,20 @@
     radius: float
 
 
 class AnalyseSingleForceSensitivity(base.IPSNode):
     data: list[list[ase.Atoms]] = zntrack.deps()
     sim_list: list = zntrack.deps()  # list["ASEMD"]
 
-    alpha: float = zntrack.zn.params(
+    alpha: float = zntrack.params(
         0.05
     )  # Desired significance level (e.g., 95% confidence interval)
 
-    sensitivity: pd.DataFrame = zntrack.zn.plots()
-    sensitivity_plot: str = zntrack.dvc.outs(zntrack.nwd / "sensitivity.png")
+    sensitivity: pd.DataFrame = zntrack.plots()
+    sensitivity_plot: str = zntrack.outs_path(zntrack.nwd / "sensitivity.png")
 
     def t_confidence_interval(self, data):
         """Returns the confidence interval for the given data and significance level."""
         df = len(data) - 1
 
         sample_variance = np.var(data, ddof=1)
         # lower_chi2 = stats.chi2.ppf(alpha / 2, df)
@@ -135,16 +135,16 @@
 
     def run(self):
         values = []
 
         self.data = [x.atoms if isinstance(x, zntrack.Node) else x for x in self.data]
 
         for atoms, sim in zip(self.data, self.sim_list):
-            radius = sim.constraint_list[0].radius
-            atom_id = sim.constraint_list[0].get_selected_atom_id(atoms[0])
+            radius = sim.constraints[0].radius
+            atom_id = sim.constraints[0].get_selected_atom_id(atoms[0])
 
             value = self.get_values(atoms, atom_id)
             values.append({"radius": radius, "std": value[0], "ci": value[1]})
 
         self.sensitivity = pd.DataFrame(values).set_index("radius").sort_index()
 
         fig, ax = plt.subplots()
```

### Comparing `ipsuite-0.1.1/ipsuite/base/base.py` & `ipsuite-0.1.2/ipsuite/base/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,16 @@
         It does not have to be 'field.Atoms' but can also be e.g. a 'property'.
         Although, we only process a single atoms object, we return a list.
         This could e.g. be the case when we want to create a trajectory
         starting from a single atoms object.
     """
 
     data: typing.Union[ase.Atoms, typing.List[ase.Atoms]] = zntrack.deps()
-    data_file: str = zntrack.dvc.deps(None)
-    data_id: typing.Optional[int] = zntrack.zn.params(0)
+    data_file: str = zntrack.deps_path(None)
+    data_id: typing.Optional[int] = zntrack.params(0)
 
     atoms: typing.List[ase.Atoms] = fields.Atoms()
 
     def get_data(self) -> ase.Atoms:
         """Get the atoms object to process given the 'data' and 'data_id'.
 
         Returns
@@ -126,22 +126,19 @@
     data: list[ase.Atoms]
         The atoms data to analyse. This must be an input to the Node
     """
 
     data: list[ase.Atoms] = zntrack.deps()
 
 
-class AnalyseProcessAtoms(IPSNode):
-    """Analyse the output of a ProcessAtoms Node."""
+class ComparePredictions(IPSNode):
+    """Compare the predictions of two models."""
 
-    data: ProcessAtoms = zntrack.deps()
-
-    def get_data(self) -> typing.Tuple[list[ase.Atoms], list[ase.Atoms]]:
-        self.data.update_data()  # otherwise, data might not be available
-        return self.data.data, self.data.atoms
+    x: list[ase.Atoms] = zntrack.deps()
+    y: list[ase.Atoms] = zntrack.deps()
 
 
 class Mapping(ProcessAtoms):
     """Base class for transforming ASE `Atoms`.
 
     `Mapping` nodes can be used in a more functional manner when initialized
     with `data=None` outside the project graph.
@@ -156,16 +153,16 @@
     Parameters
     ----------
     frozen: bool
         If True, the neighbor list is only constructed for the first configuration.
         The indices of the molecules will be frozen for all configurations.
     """
 
-    molecules: list[ase.Atoms] = zntrack.zn.outs()
-    frozen: bool = zntrack.zn.params(False)
+    molecules: list[ase.Atoms] = zntrack.outs()
+    frozen: bool = zntrack.params(False)
 
     # TODO, should we allow to transfer the frozen mapping to another node?
     #  mapping = Mapping(frozen=True, reference=mapping)
 
     def run(self):
         self.atoms = []
         self.molecules = []
@@ -190,15 +187,15 @@
 
     def backward_mapping(
         self, cg_atoms: ase.Atoms, molecules: list[ase.Atoms]
     ) -> list[ase.Atoms]:
         raise NotImplementedError
 
 
-class CheckBase(IPSNode):
+class Check(IPSNode):
     """Base class for check nodes.
     These are callbacks that can be used to preemptively terminate
     a molecular dynamics simulation if a vertain condition is met.
     """
 
     status: str = None
 
@@ -217,12 +214,21 @@
 
     @abc.abstractmethod
     def get_value(self, atoms: ase.Atoms):
         """Returns the metric that is tracked for stopping."""
         ...
 
     @abc.abstractmethod
-    def get_quantity(self) -> str:
-        ...
+    def get_quantity(self) -> str: ...
 
     def __str__(self):
         return self.status
+
+
+class Modifier(IPSNode):
+    """Base class for modifier nodes.
+    These are callbacks that can be used to alter the dynamics of an MD run.
+    This can be achieved by modifying the thermostat state or atoms in the system.
+    """
+
+    @abc.abstractmethod
+    def modify(self, thermostat: IPSNode, step: int, total_steps: int) -> None: ...
```

### Comparing `ipsuite-0.1.1/ipsuite/base/protocol.py` & `ipsuite-0.1.2/ipsuite/base/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Collection of protocols and complex type hints for type hinting."""
+
 import typing
 
 import ase
 
 
 # Collection of Protocols for type hinting
 class HasAtoms(typing.Protocol):
```

### Comparing `ipsuite-0.1.1/ipsuite/bootstrap/random_displacements.py` & `ipsuite-0.1.2/ipsuite/bootstrap/random_displacements.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     seed: int
         Random seed.
     model: IPSNode
         Any IPSNode that provides a `get_calculator` method to
         label the bootstrapped configurations.
     """
 
-    n_configurations: int = zntrack.zn.params()
-    maximum: float = zntrack.zn.params()
-    include_original: bool = zntrack.zn.params(True)
-    seed: int = zntrack.zn.params(0)
+    n_configurations: int = zntrack.params()
+    maximum: float = zntrack.params()
+    include_original: bool = zntrack.params(True)
+    seed: int = zntrack.params(0)
     model: base.IPSNode = zntrack.deps(None)
-    model_outs = zntrack.dvc.outs(zntrack.nwd / "model_outs")
+    model_outs = zntrack.outs_path(zntrack.nwd / "model_outs")
 
     def run(self) -> None:
         atoms = self.get_data()
         rng = default_rng(self.seed)
         atoms_list = self.bootstrap_configs(
             atoms,
             rng,
```

### Comparing `ipsuite-0.1.1/ipsuite/bootstrap/surface_mods.py` & `ipsuite-0.1.2/ipsuite/bootstrap/surface_mods.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,18 +143,17 @@
 
         # get energy
         true_energies = np.reshape(self.energy_df["true"], shape)
         pred_energies = np.reshape(self.energy_df["prediction"], shape)
 
         # get forces
         shape.append(3)
-        true_data_list, pred_data_list = self.get_data()
 
         forces = []
-        for true_data, pred_data in zip(true_data_list, pred_data_list):
+        for true_data, pred_data in zip(self.x, self.y):
             forces.append([true_data.get_forces(), pred_data.get_forces()])
 
         forces = np.array(forces)[:, :, -1, :] * 1000
         true_forces = np.reshape(forces[:, 0, :], shape)
         pred_forces = np.reshape(forces[:, 1, :], shape)
 
         for i, distance in enumerate(self.scan_node.z_dist_list):
```

### Comparing `ipsuite-0.1.1/ipsuite/calculators/__init__.pyi` & `ipsuite-0.1.2/ipsuite/calculators/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from .apax_jax_md import ApaxJaxMD
 from .ase_geoopt import ASEGeoOpt
 from .ase_md import (
     ASEMD,
     BoxOscillatingRampModifier,
+    FixedLayerConstraint,
     FixedSphereConstraint,
     LangevinThermostat,
     NPTThermostat,
     PressureRampModifier,
     RescaleBoxModifier,
     TemperatureOscillatingRampModifier,
     TemperatureRampModifier,
 )
 from .ase_standard import EMTSinglePoint, LJSinglePoint
 from .cp2k import CP2KSinglePoint, CP2KYaml
 from .lammps import LammpsSimulator
+from .mix import MixCalculator
 from .orca import OrcaSinglePoint
+from .torch_d3 import TorchD3
 from .xtb import xTBSinglePoint
 
 __all__ = [
     "CP2KSinglePoint",
     "CP2KYaml",
     "ASEGeoOpt",
     "ASEMD",
@@ -32,8 +35,11 @@
     "EMTSinglePoint",
     "TemperatureRampModifier",
     "PressureRampModifier",
     "TemperatureOscillatingRampModifier",
     "NPTThermostat",
     "OrcaSinglePoint",
     "LammpsSimulator",
+    "TorchD3",
+    "FixedLayerConstraint",
+    "MixCalculator",
 ]
```

### Comparing `ipsuite-0.1.1/ipsuite/calculators/apax_jax_md.py` & `ipsuite-0.1.2/ipsuite/calculators/apax_jax_md.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import typing
 
 import ase.io
 import h5py
 import yaml
 import znh5md
 import zntrack.utils
-from zntrack import dvc, zn
 
-from ipsuite import utils
 from ipsuite.base import ProcessSingleAtom
 from ipsuite.models import Apax
 from ipsuite.utils.helpers import check_duplicate_keys
 
 log = logging.getLogger(__name__)
 
 
@@ -30,21 +28,23 @@
     md_parameter: dict
         parameter for the MD simulation
     md_parameter_file: str
         path to the MD simulation parameter file
     """
 
     model: Apax = zntrack.deps()
-    repeat = zn.params(None)
+    repeat = zntrack.params(None)
 
-    md_parameter: dict = zn.params(None)
-    md_parameter_file: str = dvc.params(None)
+    md_parameter: dict = zntrack.params(None)
+    md_parameter_file: str = zntrack.params_path(None)
 
-    sim_dir: pathlib.Path = dvc.outs(zntrack.nwd / "md")
-    init_struc_dir: pathlib.Path = dvc.outs(zntrack.nwd / "initial_structure.extxyz")
+    sim_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "md")
+    init_struc_dir: pathlib.Path = zntrack.outs_path(
+        zntrack.nwd / "initial_structure.extxyz"
+    )
 
     def post_init(self):
         if not self.state.loaded:
             dict_supplied = self.md_parameter is None
             file_supplied = self.md_parameter_file is None
 
             if dict_supplied and file_supplied:
@@ -60,16 +60,14 @@
                 )
 
         if not isinstance(self.model, Apax):
             raise TypeError(
                 "Performing simulations with JaxMD requires a apax model Node"
             )
 
-        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
-
     def _handle_parameter_file(self):
         if self.md_parameter_file:
             md_parameter_file_content = pathlib.Path(self.md_parameter_file).read_text()
             self.md_parameter = yaml.safe_load(md_parameter_file_content)
 
         custom_parameters = {
             "sim_dir": self.sim_dir.as_posix(),
@@ -85,15 +83,15 @@
         self._handle_parameter_file()
         atoms = self.get_data()
         if self.repeat is not None:
             atoms = atoms.repeat(self.repeat)
         ase.io.write(self.init_struc_dir.as_posix(), atoms)
 
         self.model._handle_parameter_file()
-        run_md(self.model._parameter, self.md_parameter, log_file="md.log")
+        run_md(self.model._parameter, self.md_parameter)
 
     @functools.cached_property
     def atoms(self) -> typing.List[ase.Atoms]:
         # filename should be changeable
         def file_handle(filename):
             file = self.state.fs.open(filename, "rb")
             return h5py.File(file)
```

### Comparing `ipsuite-0.1.1/ipsuite/calculators/ase_md.py` & `ipsuite-0.1.2/ipsuite/calculators/ase_md.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,36 @@
 from ase import units
 from ase.md.langevin import Langevin
 from ase.md.npt import NPT
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
 from tqdm import trange
 
 from ipsuite import base
-from ipsuite.utils.ase_sim import freeze_copy_atoms, get_energy
+from ipsuite.utils.ase_sim import freeze_copy_atoms, get_box_from_density, get_energy
 
 log = logging.getLogger(__name__)
 
 
-class RescaleBoxModifier(base.IPSNode):
-    cell: int = zntrack.zn.params()
+class RescaleBoxModifier(base.Modifier):
+    cell: int = zntrack.params(None)
+    density: float = zntrack.params(None)
     _initial_cell = None
 
+    # def _post_init_(self):
+    #     super()._post_init_()
+    #     if self.density is not None and self.cell is not None:
+    #         raise ValueError("Only one of density or cell can be given.")
+    #     if self.density is None and self.cell is None:
+    #         raise ValueError("Either density or cell has to be given.")
+    # Currently not possible due to a ZnTrack bug
+
     def modify(self, thermostat, step, total_steps):
         # we use the thermostat, so we can also modify e.g. temperature
+        if self.cell is None:
+            self.cell = get_box_from_density([[thermostat.atoms]], [1], self.density)
         if isinstance(self.cell, int):
             self.cell = np.array(
                 [[self.cell, 0, 0], [0, self.cell, 0], [0, 0, self.cell]]
             )
         elif isinstance(self.cell, list):
             self.cell = np.array(
                 [[self.cell[0], 0, 0], [0, self.cell[1], 0], [0, 0, self.cell[2]]]
@@ -41,34 +52,48 @@
         if self._initial_cell is None:
             self._initial_cell = thermostat.atoms.get_cell()
         percentage = step / (total_steps - 1)
         new_cell = (1 - percentage) * self._initial_cell + percentage * self.cell
         thermostat.atoms.set_cell(new_cell, scale_atoms=True)
 
 
-class BoxOscillatingRampModifier(base.IPSNode):
+class BoxOscillatingRampModifier(base.Modifier):
     """Ramp the simulation cell to a specified end cell with some oscillations.
 
     Attributes
     ----------
     end_cell: float, list[float], optional
         cell to ramp to, cubic or tetragonal. If None, the cell will oscillate
         around the initial cell.
     cell_amplitude: float
         amplitude in oscillations of the diagonal cell elements
     num_oscillations: float
         number of oscillations. No oscillations will occur if set to 0.
     interval: int, default 1
         interval in which the box size is changed.
+    num_ramp_oscillations: float, optional
+        number of oscillations to ramp the box size to the end cell.
+        This value has to be smaller than num_oscillations.
+        For LotF applications, this can prevent a loop of ever decreasing cell sizes.
+        To ensure this use a value of 0.5.
     """
 
-    end_cell: int = zntrack.zn.params(None)
-    cell_amplitude: typing.Union[float, list[float]] = zntrack.zn.params()
-    num_oscillations: float = zntrack.zn.params()
-    interval: int = zntrack.zn.params(1)
+    def _post_init_(self):
+        super()._post_init_()
+        if self.num_ramp_oscillations is not None:
+            if self.num_ramp_oscillations > self.num_oscillations:
+                raise ValueError(
+                    "num_ramp_oscillations has to be smaller than num_oscillations."
+                )
+
+    end_cell: int = zntrack.params(None)
+    cell_amplitude: typing.Union[float, list[float]] = zntrack.params()
+    num_oscillations: float = zntrack.params()
+    num_ramp_oscillations: float = zntrack.params(None)
+    interval: int = zntrack.params(1)
     _initial_cell = None
 
     def modify(self, thermostat, step, total_steps):
         if self.end_cell is None:
             self.end_cell = thermostat.atoms.get_cell()
         if self._initial_cell is None:
             self._initial_cell = thermostat.atoms.get_cell()
@@ -82,41 +107,54 @@
                         [self.end_cell[0], 0, 0],
                         [0, self.end_cell[1], 0],
                         [0, 0, self.end_cell[2]],
                     ]
                 )
 
         percentage = step / (total_steps - 1)
-        ramp = percentage * (self.end_cell - self._initial_cell)
+        # if num_ramp_oscillations is set, the cell size is ramped to end_cell within
+        # num_ramp_oscillations instead of num_oscillations. This can prevent a loop of
+        # ever decreasing cell sizes in LoTF applications where simulations
+        # can be aborted at small cell sizes.
+        if self.num_ramp_oscillations is not None:
+            percentage_per_oscillation = (
+                percentage * self.num_oscillations / self.num_ramp_oscillations
+            )
+            percentage_per_oscillation = min(percentage_per_oscillation, 1)
+        else:
+            # ramp over all oscillations
+            percentage_per_oscillation = percentage
+
+        ramp = percentage_per_oscillation * (self.end_cell - self._initial_cell)
         oscillation = self.cell_amplitude * np.sin(
             2 * np.pi * percentage * self.num_oscillations
         )
         oscillation = np.eye(3) * oscillation
         new_cell = self._initial_cell + ramp + oscillation
 
         if step % self.interval == 0:
             thermostat.atoms.set_cell(new_cell, scale_atoms=True)
 
 
-class TemperatureRampModifier(base.IPSNode):
+class TemperatureRampModifier(base.Modifier):
     """Ramp the temperature from start_temperature to temperature.
 
     Attributes
     ----------
     start_temperature: float, optional
         temperature to start from, if None, the temperature of the thermostat is used.
     temperature: float
         temperature to ramp to.
     interval: int, default 1
         interval in which the temperature is changed.
     """
 
-    start_temperature: float = zntrack.zn.params(None)
-    temperature: float = zntrack.zn.params()
-    interval: int = zntrack.zn.params(1)
+    start_temperature: float = zntrack.params(None)
+    temperature: float = zntrack.params()
+    interval: int = zntrack.params(1)
 
     def modify(self, thermostat, step, total_steps):
         # we use the thermostat, so we can also modify e.g. temperature
         if self.start_temperature is None:
             # different thermostats call the temperature attribute differently
             if hasattr(thermostat, "temp"):
                 start_temperature = thermostat.temp
@@ -128,15 +166,15 @@
         new_temperature = (
             1 - percentage
         ) * self.start_temperature + percentage * self.temperature
         if step % self.interval == 0:
             thermostat.set_temperature(temperature_K=new_temperature)
 
 
-class TemperatureOscillatingRampModifier(base.IPSNode):
+class TemperatureOscillatingRampModifier(base.Modifier):
     """Ramp the temperature from start_temperature to temperature with some oscillations.
 
     Attributes
     ----------
     start_temperature: float, optional
         temperature to start from, if None, the temperature of the thermostat is used.
     end_temperature: float
@@ -145,19 +183,19 @@
         amplitude of temperature oscillations.
     num_oscillations: float
         number of oscillations. No oscillations will occur if set to 0.
     interval: int, default 1
         interval in which the temperature is changed.
     """
 
-    start_temperature: float = zntrack.zn.params(None)
-    end_temperature: float = zntrack.zn.params()
-    temperature_amplitude: float = zntrack.zn.params()
-    num_oscillations: float = zntrack.zn.params()
-    interval: int = zntrack.zn.params(1)
+    start_temperature: float = zntrack.params(None)
+    end_temperature: float = zntrack.params()
+    temperature_amplitude: float = zntrack.params()
+    num_oscillations: float = zntrack.params()
+    interval: int = zntrack.params(1)
 
     def modify(self, thermostat, step, total_steps):
         # we use the thermostat, so we can also modify e.g. temperature
         if self.start_temperature is None:
             # different thermostats call the temperature attribute differently
             if hasattr(thermostat, "temp"):
                 start_temperature = thermostat.temp
@@ -173,32 +211,32 @@
 
         new_temperature = max(0, new_temperature)  # prevent negative temperature
 
         if step % self.interval == 0:
             thermostat.set_temperature(temperature_K=new_temperature)
 
 
-class PressureRampModifier(base.IPSNode):
+class PressureRampModifier(base.Modifier):
     """Ramp the temperature from start_temperature to temperature.
     Works only for the NPT thermostat (not NPTBerendsen).
 
     Attributes
     ----------
     start_pressure_au: float, optional
         pressure to start from, if None, the pressure of the thermostat is used.
         Uses ASE units.
     end_pressure_au: float
         pressure to ramp to. Uses ASE units.
     interval: int, default 1
         interval in which the pressure is changed.
     """
 
-    start_pressure_au: float = zntrack.zn.params(None)
-    end_pressure_au: float = zntrack.zn.params()
-    interval: int = zntrack.zn.params(1)
+    start_pressure_au: float = zntrack.params(None)
+    end_pressure_au: float = zntrack.params()
+    interval: int = zntrack.params(1)
 
     def modify(self, thermostat, step, total_steps):
         if self.start_pressure_au is None:
             self.start_pressure_au = thermostat.externalstress
 
         frac = step / total_steps
         new_pressure = (-self.start_pressure_au[0]) ** (1 - frac)
@@ -220,23 +258,22 @@
         temperature in K to simulate at
 
     friction: float
         friction of the Langevin simulator
 
     """
 
-    time_step: int = zntrack.zn.params()
-    temperature: float = zntrack.zn.params()
-    friction: float = zntrack.zn.params()
+    time_step: int = zntrack.params()
+    temperature: float = zntrack.params()
+    friction: float = zntrack.params()
 
     def get_thermostat(self, atoms):
-        self.time_step *= units.fs
         thermostat = Langevin(
             atoms=atoms,
-            timestep=self.time_step,
+            timestep=self.time_step * units.fs,
             temperature_K=self.temperature,
             friction=self.friction,
         )
         return thermostat
 
 
 class NPTThermostat(base.IPSNode):
@@ -260,22 +297,26 @@
     pfactor: float
         characteristic pressure coupling time in ASE units
 
     tetragonal_strain: bool
         if True allows only the diagonal elements of the box to change,
         i.e. box angles are constant
 
+    fraction_traceless: Union[int, float]
+        How much of the traceless part of the virial to keep.
+        If set to 0, the volume of the cell can change, but the shape cannot.
     """
 
-    time_step: float = zntrack.zn.params()
-    temperature: float = zntrack.zn.params()
-    pressure: float = zntrack.zn.params()
-    ttime: float = zntrack.zn.params()
-    pfactor: float = zntrack.zn.params()
-    tetragonal_strain: bool = zntrack.zn.params(True)
+    time_step: float = zntrack.params()
+    temperature: float = zntrack.params()
+    pressure: float = zntrack.params()
+    ttime: float = zntrack.params()
+    pfactor: float = zntrack.params()
+    tetragonal_strain: bool = zntrack.params(True)
+    fraction_traceless: typing.Union[int, float] = zntrack.params(1)
 
     def get_thermostat(self, atoms):
         if self.tetragonal_strain:
             mask = np.array(
                 [
                     [True, False, False],
                     [False, True, False],
@@ -290,14 +331,15 @@
             self.time_step,
             temperature_K=self.temperature,
             externalstress=self.pressure,
             ttime=self.ttime,
             pfactor=self.pfactor,
             mask=mask,
         )
+        thermostat.set_fraction_traceless(self.fraction_traceless)
         return thermostat
 
 
 class FixedSphereConstraint(base.IPSNode):
     """Attributes
     ----------
     atom_id: int
@@ -307,17 +349,17 @@
         The type of the atom to fix. E.g. if
         atom_type = H, atom_id = 1, the first
         hydrogen atom will be fixed. If None,
         the first atom will be fixed, no matter the type.
     radius: float
     """
 
-    atom_id = zntrack.zn.params(None)
-    atom_type = zntrack.zn.params(None)
-    radius = zntrack.zn.params()
+    atom_id = zntrack.params(None)
+    atom_type = zntrack.params(None)
+    radius = zntrack.params()
 
     def _post_init_(self):
         if self.atom_type is not None and self.atom_id is None:
             raise ValueError("If atom_type is given, atom_id must be given as well.")
 
     def get_selected_atom_id(self, atoms: ase.Atoms) -> int:
         if self.atom_type is not None:
@@ -375,19 +417,20 @@
     ----------
     atoms_lst: list
         list of atoms objects to start simulation from
     start_id: int
         starting id to pick from list of atoms
     model: zntrack.Node
         A node that implements a 'get_calculation' method
-    checker_list: list[CheckNodes]
-        checker, which tracks various metrics and stops the
-        simulation after a threshold is exceeded.
-    constraint_list: list[ConstraintNodes]
-        constraints the atoms within the md simulation
+    checks: list[Check]
+        checks, which track various metrics and stop the
+        simulation if some criterion is met.
+    constraints: list[Constraint]
+        constrains the atoms within the md simulation
+    modifiers: list[Modifier]
     thermostat: ase dynamics
         dynamics method used for simulation
     init_temperature: float
         temperature in K to initialize velocities
     init_velocity: np.array()
         starting velocities to continue a simulation
     steps: int
@@ -400,36 +443,40 @@
     repeat: float
         number of repeats
     traj_file: Path
         path where to save the trajectory
     dump_rate: int, default=1000
         Keep a cache of the last 'dump_rate' atoms and
         write them to the trajectory file every 'dump_rate' steps.
+    wrap: bool
+        Keep the atoms in the cell.
     """
 
     model = zntrack.deps()
 
-    model_outs = zntrack.dvc.outs(zntrack.nwd / "model/")
-    checker_list: list = zntrack.deps(None)
-    constraint_list: list = zntrack.deps(None)
-    modifier: list = zntrack.deps(None)
+    model_outs = zntrack.outs_path(zntrack.nwd / "model/")
+    checks: list = zntrack.deps(None)
+    constraints: list = zntrack.deps(None)
+    modifiers: list = zntrack.deps(None)
     thermostat = zntrack.deps()
 
-    steps: int = zntrack.zn.params()
-    sampling_rate = zntrack.zn.params(1)
-    repeat = zntrack.zn.params((1, 1, 1))
-    dump_rate = zntrack.zn.params(1000)
-    pop_last = zntrack.zn.params(False)
-    use_momenta = zntrack.zn.params(False)
+    steps: int = zntrack.params()
+    sampling_rate = zntrack.params(1)
+    repeat = zntrack.params((1, 1, 1))
+    dump_rate = zntrack.params(1000)
+    pop_last = zntrack.params(False)
+    use_momenta = zntrack.params(False)
+    seed: int = zntrack.params(42)
+    wrap: bool = zntrack.params(False)
 
-    metrics_dict = zntrack.zn.plots()
+    metrics_dict = zntrack.plots()
 
-    steps_before_stopping = zntrack.zn.metrics()
+    steps_before_stopping = zntrack.metrics()
 
-    traj_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "trajectory.h5")
+    traj_file: pathlib.Path = zntrack.outs_path(zntrack.nwd / "structures.h5")
 
     def get_atoms(self) -> ase.Atoms:
         atoms: ase.Atoms = self.get_data()
         return atoms.repeat(self.repeat)
 
     @property
     def atoms(self) -> typing.List[ase.Atoms]:
@@ -442,20 +489,22 @@
             format_handler=functools.partial(
                 znh5md.FormatHandler, file_handle=file_handle
             ),
         ).get_atoms_list()
 
     def run(self):  # noqa: C901
         """Run the simulation."""
-        if self.checker_list is None:
-            self.checker_list = []
-        if self.modifier is None:
-            self.modifier = []
-        if self.constraint_list is None:
-            self.constraint_list = []
+        np.random.seed(self.seed)
+
+        if self.checks is None:
+            self.checks = []
+        if self.modifiers is None:
+            self.modifiers = []
+        if self.constraints is None:
+            self.constraints = []
 
         self.model_outs.mkdir(parents=True, exist_ok=True)
         (self.model_outs / "outs.txt").write_text("Lorem Ipsum")
         atoms = self.get_atoms()
         atoms.calc = self.model.get_calculator(directory=self.model_outs)
 
         if not self.use_momenta:
@@ -464,15 +513,15 @@
 
         # initialize thermostat
         time_step = self.thermostat.time_step
         thermostat = self.thermostat.get_thermostat(atoms=atoms)
 
         # initialize Atoms calculator and metrics_dict
         metrics_dict = {"energy": [], "temperature": []}
-        for checker in self.checker_list:
+        for checker in self.checks:
             checker.initialize(atoms)
             if checker.get_quantity() is not None:
                 metrics_dict[checker.get_quantity()] = []
 
         # Run simulation
         sampling_iterations = self.steps / self.sampling_rate
         if sampling_iterations % 1 != 0:
@@ -481,15 +530,15 @@
             log.warning(
                 "The sampling_rate is not a devisor of steps."
                 f"Steps were adjusted to {self.steps}"
             )
         sampling_iterations = int(sampling_iterations)
         total_fs = self.steps * time_step
 
-        for constraint in self.constraint_list:
+        for constraint in self.constraints:
             atoms.set_constraint(constraint.get_constraint(atoms))
 
         atoms_cache = []
 
         db = znh5md.io.DataWriter(self.traj_file)
         db.initialize_database_groups()
         self.steps_before_stopping = -1
@@ -501,40 +550,39 @@
         ) as pbar:
             for idx_outer in range(sampling_iterations):
                 desc = []
                 stop = []
 
                 # run MD for sampling_rate steps
                 for idx_inner in range(self.sampling_rate):
-                    for modifier in self.modifier:
+                    for modifier in self.modifiers:
                         modifier.modify(
                             thermostat,
                             step=idx_outer * self.sampling_rate + idx_inner,
                             total_steps=self.steps,
                         )
-
+                    if self.wrap:
+                        atoms.wrap()
                     thermostat.run(1)
 
-                    for checker in self.checker_list:
+                    for checker in self.checks:
                         stop.append(checker.check(atoms))
                         if stop[-1]:
                             log.critical(str(checker))
 
                     if any(stop):
                         break
 
                 if any(stop):
                     self.steps_before_stopping = (
                         idx_outer * self.sampling_rate + idx_inner
                     )
                     break
                 else:
-                    metrics_dict = update_metrics_dict(
-                        atoms, metrics_dict, self.checker_list
-                    )
+                    metrics_dict = update_metrics_dict(atoms, metrics_dict, self.checks)
                     atoms_cache.append(freeze_copy_atoms(atoms))
                     if len(atoms_cache) == self.dump_rate:
                         db.add(
                             znh5md.io.AtomsReader(
                                 atoms_cache,
                                 frames_per_chunk=self.dump_rate,
                                 step=1,
@@ -547,15 +595,15 @@
                     temperature = metrics_dict["temperature"][-1]
                     energy = metrics_dict["energy"][-1]
                     desc = get_desc(temperature, energy, time, total_fs)
                     pbar.set_description(desc)
                     pbar.update(self.sampling_rate)
 
         if not self.pop_last and self.steps_before_stopping != -1:
-            metrics_dict = update_metrics_dict(atoms, metrics_dict, self.checker_list)
+            metrics_dict = update_metrics_dict(atoms, metrics_dict, self.checks)
             atoms_cache.append(freeze_copy_atoms(atoms))
 
         db.add(
             znh5md.io.AtomsReader(
                 atoms_cache,
                 frames_per_chunk=self.dump_rate,
                 step=1,
@@ -571,17 +619,17 @@
     """TQDM description."""
     return (
         f"Temp.: {temperature:.3f} K \t Energy {total_energy:.3f} eV \t Time"
         f" {time:.1f}/{total_time:.1f} fs"
     )
 
 
-def update_metrics_dict(atoms, metrics_dict, checker_list):
+def update_metrics_dict(atoms, metrics_dict, checks):
     temperature, energy = get_energy(atoms)
     metrics_dict["energy"].append(energy)
     metrics_dict["temperature"].append(temperature)
-    for checker in checker_list:
+    for checker in checks:
         metric = checker.get_value(atoms)
         if metric is not None:
             metrics_dict[checker.get_quantity()].append(metric)
 
     return metrics_dict
```

### Comparing `ipsuite-0.1.1/ipsuite/calculators/ase_standard.py` & `ipsuite-0.1.2/ipsuite/calculators/ase_standard.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/calculators/cp2k.py` & `ipsuite-0.1.2/ipsuite/calculators/cp2k.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """CP2K interface without ASE calculator.
 
 This interface is less restrictive than CP2K Single Point.
 """
+
 import contextlib
 import functools
 import logging
 import os
 import pathlib
 import shutil
 import subprocess
@@ -185,15 +186,15 @@
 
     cp2k_shell: str = zntrack.meta.Text(None)
     cp2k_params = zntrack.params_path("cp2k.yaml")
     cp2k_files = zntrack.deps_path(None)
 
     wfn_restart_file: str = zntrack.deps_path(None)
     wfn_restart_node = zntrack.deps(None)
-    output_file = zntrack.outs_path(zntrack.nwd / "atoms.h5")
+    output_file = zntrack.outs_path(zntrack.nwd / "structures.h5")
     cp2k_directory = zntrack.outs_path(zntrack.nwd / "cp2k")
 
     def run(self):
         """ZnTrack run method.
 
         Raises
         ------
```

### Comparing `ipsuite-0.1.1/ipsuite/calculators/lammps.py` & `ipsuite-0.1.2/ipsuite/calculators/lammps.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/calculators/orca.py` & `ipsuite-0.1.2/ipsuite/calculators/orca.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import zntrack
 from ase.calculators.orca import ORCA
 
 from ipsuite import base
 
 
 class OrcaSinglePoint(base.ProcessAtoms):
-    orcasimpleinput: str = zntrack.zn.params("B3LYP def2-TZVP")
-    orcablocks: str = zntrack.zn.params("%pal nprocs 16 end")
+    orcasimpleinput: str = zntrack.params("B3LYP def2-TZVP")
+    orcablocks: str = zntrack.params("%pal nprocs 16 end")
     ASE_ORCA_COMMAND: str = zntrack.meta.Environment("orca")
 
-    orca_directory: str = zntrack.dvc.outs(zntrack.nwd / "orca")
-    output_file: str = zntrack.dvc.outs(zntrack.nwd / "atoms.h5")
+    orca_directory: str = zntrack.outs_path(zntrack.nwd / "orca")
+    output_file: str = zntrack.outs_path(zntrack.nwd / "structures.h5")
 
     def run(self):
         db = znh5md.io.DataWriter(self.output_file)
         db.initialize_database_groups()
 
         calc = self.get_calculator()
         for atoms in tqdm.tqdm(self.get_data(), ncols=70):
```

### Comparing `ipsuite-0.1.1/ipsuite/calculators/xtb.py` & `ipsuite-0.1.2/ipsuite/calculators/xtb.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Attributes
     ----------
     method: str
         xTB method to be used. Only "GFN1-xTB" supports PBC.
     """
 
-    method: str = zntrack.zn.params("GFN1-xTB")
+    method: str = zntrack.params("GFN1-xTB")
 
     def run(self):
         self.atoms = []
 
         calculator = self.get_calculator()
 
         for atom in tqdm.tqdm(self.get_data(), ncols=70):
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_comparison/MMKernel.py` & `ipsuite-0.1.2/ipsuite/configuration_comparison/MMKernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Minimum Membership Kernel (MMKernel) module."""
+
 import numpy as np
 import tensorflow as tf
 
 from ipsuite.configuration_comparison import ConfigurationComparison
 
 
 @tf.function(jit_compile=False)
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_comparison/REMatch.py` & `ipsuite-0.1.2/ipsuite/configuration_comparison/REMatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """REMatch kernel Node."""
+
 import numpy as np
 import tensorflow as tf
 import zntrack
 from dscribe.kernels import REMatchKernel
 from sklearn.preprocessing import normalize
 
 from ipsuite.configuration_comparison import ConfigurationComparison
@@ -23,17 +24,17 @@
         Parameter controlling the entropic penalty. Values close to zero approach the
         best-match solution and values towards infinity approach the average kernel.
     threshold: float
         Convergence threshold used in the Sinkhorn-algorithm.
 
     """
 
-    metric: str = zntrack.zn.params("linear")
-    alpha: float = zntrack.zn.params(1.0)
-    threshold: float = zntrack.zn.params(1e-6)
+    metric: str = zntrack.params("linear")
+    alpha: float = zntrack.params(1.0)
+    threshold: float = zntrack.params(1e-6)
 
     def _post_init_(self):
         """Initialise the REMatchKernel instance."""
         self.re = REMatchKernel(
             metric=self.metric, alpha=self.alpha, threshold=self.threshold
         )
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_comparison/base.py` & `ipsuite-0.1.2/ipsuite/configuration_comparison/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import pandas as pd
 import tensorflow as tf
 import znjson
 import zntrack
 from dscribe.descriptors import SOAP
 from tqdm import trange
 
-from ipsuite import base, utils
+from ipsuite import base
 
 
 def convert_to_df(similarities: typing.List) -> pd.DataFrame:
-    """Convert similarities to pd.DataFrame to save as zn.plots.
+    """Convert similarities to pd.DataFrame to save as zntrack.plots.
 
     Parameters
     ----------
     similarities: typing.List
         contains similarities
     Returns
     -------
@@ -121,71 +121,72 @@
     reference: typing.Union[utils.helpers.UNION_ATOMS_OR_ATOMS_LST,
      utils.types.SupportsAtoms]
         reference configurations to compare analyte to
     analyte: typing.Union[
         utils.helpers.UNION_ATOMS_OR_ATOMS_LST, utils.types.SupportsAtoms
     ]
         analyte comparison to compare with reference
-    similarities: zn.plots()
+    similarities: zntrack.plots()
         in the end a csv file to save computed maximal similarities
     soap: typing.Union[dict, SOAPParameter]
         parameter to use for the SOAP descriptor
     result: typing.List[typing.List[float]]
         result of the comparison, all similarity computations
     node_name: str
         name of the node used within the dvc graph
     compile_with_jit: bool
         choose if kernel should be compiled with jit or not.
+    memory: int
+            How far back to look in the MMK vector.
     """
 
     reference: base.protocol.HasOrIsAtoms = zntrack.deps()
     analyte: base.protocol.HasOrIsAtoms = zntrack.deps()
-    similarities = zntrack.zn.plots()
-    soap: typing.Union[dict, SOAPParameter] = zntrack.zn.params(SOAPParameter())
-    result: typing.List[float] = zntrack.zn.outs()
+    memory: int = zntrack.params(1000)
+    similarities = zntrack.plots()
+    soap: typing.Union[dict, SOAPParameter] = zntrack.params(SOAPParameter())
+    result: typing.List[float] = zntrack.outs()
 
     _name_ = "ConfigurationComparison"
     use_jit: bool = zntrack.meta.Text(True)
 
     def __init__(
         self,
         reference=None,
         analyte=None,
         soap: dict = None,
         use_jit: bool = True,
-        **kwargs
+        **kwargs,
     ):
         """Initialize the ConfigurationComparison node.
 
         Parameters
         ----------
         reference: typing.Union[utils.helpers.UNION_ATOMS_OR_ATOMS_LST,
                     utils.types.SupportsAtoms]
             reference configurations to compare analyte to
         analyte: typing.Union[utils.helpers.UNION_ATOMS_OR_ATOMS_LST,
                 utils.types.SupportsAtoms]
             analyte comparison to compare with reference (If reference is None, analyte
              will be compared to itself)
-        similarities: zn.plots()
+        similarities: zntrack.plots()
             In the end a csv file to save computed maximal similarities
         soap: dict
             Parameter to use for the SOAP descriptor.
         use_jit: bool
             use jit compilation.
         kwargs: dict
             additional keyword arguments
         """
         super().__init__(**kwargs)
         if soap is None:
             soap = {}
-        if reference is None:
-            self.reference = None
-        else:
-            self.reference = utils.helpers.get_deps_if_node(reference, "atoms")
-        self.analyte = utils.helpers.get_deps_if_node(analyte, "atoms")
+        self.reference = reference
+        self.analyte = analyte
+
         if not self.state.loaded:
             self.soap = SOAPParameter(**soap)
 
         self.soap_file = self.nwd / "soap_representation.hdf5"
 
         # remove "soap_reference" from HDF5, do not write "soap_analyte"
         self.load_analyte = False
@@ -199,17 +200,17 @@
         It will create SOAP descriptor for each configurations
          and save them ordered in a hdf5 file.
         """
         species = [int(x) for x in set(self.analyte[0].get_atomic_numbers())]
         _soap = SOAP(
             species=species,
             periodic=False,  # any(self.analyte[0].pbc),
-            rcut=self.soap.r_cut,
-            nmax=self.soap.n_max,
-            lmax=self.soap.l_max,
+            r_cut=self.soap.r_cut,
+            n_max=self.soap.n_max,
+            l_max=self.soap.l_max,
             sigma=self.soap.sigma,
             rbf=self.soap.rbf,
             weighting=self.soap.weighting,
         )
         if self.reference is None:
             with h5py.File(self.soap_file, "w") as representation_file:
                 create_dataset(
@@ -287,14 +288,20 @@
                     leave=True,
                     disable=self.disable_tqdm,
                 ) as pbar:
                     for max_index, _atoms in enumerate(self.analyte):
                         if max_index == 0:
                             continue
                         reference_soap = representation_file["soap"][:max_index]
+                        # if max_index <= self.memory:
+                        #     reference_soap = representation_file["soap"][:max_index]
+                        # else:
+                        #     reference_soap = representation_file["soap"][
+                        #         max_index - self.memory : max_index
+                        #     ]
                         analyte_soap = representation_file["soap"][max_index]
                         comparison = self.compare(reference_soap, analyte_soap)
                         self.result.append(float(comparison.numpy()))
                         self._save_plots(max_index)
                         pbar.update(1)
         else:
             with h5py.File(self.soap_file, "r") as representation_file:
@@ -302,14 +309,22 @@
                     (len(self.analyte)),
                     desc="Comparing",
                     leave=True,
                     disable=self.disable_tqdm,
                 ) as pbar:
                     for max_index, _atoms in enumerate(self.analyte):
                         reference_soap = representation_file["soap_reference"]
+                        # if max_index <= self.memory:
+                        #     reference_soap = representation_file["soap_reference"][
+                        #         :max_index
+                        #     ]
+                        # else:
+                        #     reference_soap = representation_file["soap_reference"][
+                        #         max_index - self.memory : max_index
+                        #     ]
                         analyte_soap = representation_file["soap_analyte"][max_index]
                         comparison = self.compare(reference_soap, analyte_soap)
                         self.result.append(float(comparison.numpy()))
                         self._save_plots(max_index)
                         pbar.update(1)
         self.similarities = convert_to_df(self.result)
         with h5py.File(self.soap_file, "a") as representation_file:
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_generation/smiles_to_atoms.py` & `ipsuite-0.1.2/ipsuite/configuration_generation/smiles_to_atoms.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from ipsuite import base, fields
 
 
 class SmilesToAtoms(base.IPSNode):
     atoms = fields.Atoms()
 
-    smiles: str = zntrack.zn.params()
-    cell: float = zntrack.zn.params(None)
-    seed: int = zntrack.zn.params(1234)
-    optimizer: str = zntrack.zn.params("UFF")
-    image: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "molecule.png")
+    smiles: str = zntrack.params()
+    cell: float = zntrack.params(None)
+    seed: int = zntrack.params(1234)
+    optimizer: str = zntrack.params("UFF")
+    image: pathlib.Path = zntrack.outs_path(zntrack.nwd / "molecule.png")
 
     def run(self):
         mol = Chem.MolFromSmiles(self.smiles)
         Draw.MolToFile(mol, self.image)
 
         mol = Chem.AddHs(mol)
         AllChem.EmbedMolecule(mol, randomSeed=self.seed)
@@ -43,19 +43,19 @@
     def view(self) -> view:
         return view(self.atoms[0], viewer="x3d")
 
 
 class SmilesToConformers(base.IPSNode):
     atoms = fields.Atoms()
 
-    smiles: str = zntrack.zn.params()
-    numConfs: int = zntrack.zn.params()
-    seed: int = zntrack.zn.params(42)
-    maxAttempts: int = zntrack.zn.params(1000)
-    cell: float = zntrack.zn.params(100)
+    smiles: str = zntrack.params()
+    numConfs: int = zntrack.params()
+    seed: int = zntrack.params(42)
+    maxAttempts: int = zntrack.params(1000)
+    cell: float = zntrack.params(100)
 
     def run(self):
         mol = Chem.MolFromSmiles(self.smiles)
         mol = Chem.AddHs(mol)
         AllChem.EmbedMultipleConfs(
             mol,
             numConfs=self.numConfs,
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/__init__.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Configuration Selection Nodes."""
+
 from ipsuite.configuration_selection.base import ConfigurationSelection
+from ipsuite.configuration_selection.filter import FilterOutlier
 from ipsuite.configuration_selection.index import IndexSelection
 from ipsuite.configuration_selection.kernel import KernelSelection
 from ipsuite.configuration_selection.random import RandomSelection
 from ipsuite.configuration_selection.split import SplitSelection
 from ipsuite.configuration_selection.threshold import ThresholdSelection
 from ipsuite.configuration_selection.uniform_arange import UniformArangeSelection
 from ipsuite.configuration_selection.uniform_energetic import UniformEnergeticSelection
@@ -15,8 +17,9 @@
     "UniformEnergeticSelection",
     "UniformTemporalSelection",
     "UniformArangeSelection",
     "KernelSelection",
     "IndexSelection",
     "ThresholdSelection",
     "SplitSelection",
+    "FilterOutlier",
 ]
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/index.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Select configurations by item, e.g. slice or list of indices."""
+
 import typing
 
 import ase
 import zntrack
 
 from ipsuite.configuration_selection import ConfigurationSelection
 
@@ -11,14 +12,14 @@
     """Select atoms based on getitems.
 
     Attributes
     ----------
     indices: list[int]|slice|
     """
 
-    indices = zntrack.zn.params()
+    indices = zntrack.params()
 
     def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
         """Select Atoms randomly."""
         if isinstance(self.indices, list):
             return self.indices
         return list(range(len(atoms_lst)))[self.indices]
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/kernel.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/kernel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 """Use a Kernel and some initial configuration to select further configurations."""
+
 from __future__ import annotations
 
+import logging
 import typing
 
 import ase
 import numpy as np
 import tqdm
 import zntrack
 
-from ipsuite import utils
 from ipsuite.configuration_selection.base import ConfigurationSelection
 
 if typing.TYPE_CHECKING:
     import ipsuite
 
 
+log = logging.getLogger(__name__)
+
+
 class KernelSelection(ConfigurationSelection):
     """Use the chosen kernel to selected configurations furthes apart.
 
     Attributes
     ----------
     n_configurations: int
         number of configurations to select
-    kernel: ConfigurationComparison = zn.Nodes()
+    kernel: ConfigurationComparison = zntrack.Nodes()
     points_per_cycle: int
         Number of configurations to add before recomputing the MMK
     correlation_time: int
         Ideally the correlation time of the data to only sample from uncorrelated data.
         This will only sample from configurations that are configuration_time apart.
         The smaller, the slower is the selection but the number of looked at
         configuration is larger giving potentially better results.
     seed: int
         seed selection in case of random picking initial configuration
+    threshold: float
+        threshold to stop the selection. The maximum number of configurations
+        is still n_configurations. If the threshold is reached before, the
+        selection stops. Typical values can be 0.995
     """
 
-    n_configurations: int = zntrack.zn.params()
+    n_configurations: int = zntrack.params()
     kernel: "ipsuite.configuration_comparison.ConfigurationComparison" = zntrack.deps()
-    initial_configurations: typing.List[ase.Atoms] = zntrack.deps()
-    points_per_cycle: int = zntrack.zn.params(1)
-    kernel_results: typing.List[typing.List[float]] = zntrack.zn.outs()
-    seed = zntrack.zn.params(1234)
+    initial_configurations: typing.List[ase.Atoms] = zntrack.deps(None)
+    points_per_cycle: int = zntrack.params(1)
+    kernel_results: typing.List[typing.List[float]] = zntrack.outs()
+    seed = zntrack.params(1234)
+    threshold: float = zntrack.params(None)
 
     # TODO what if the correlation time restricts the number of atoms to
     #  be less than n_configurations?
-    correlation_time: int = zntrack.zn.params(1)
-
-    def _post_init_(self):
-        """Run after the init of the node."""
-        super()._post_init_()
-        self.initial_configurations = utils.helpers.get_deps_if_node(
-            self.initial_configurations, "atoms"
-        )
+    correlation_time: int = zntrack.params(1)
 
     def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
         """Atom Selection method.
 
         Parameters
         ----------
         atoms_lst: typing.List[ase.Atoms]
@@ -63,47 +65,74 @@
         Returns
         -------
         typing.List[int]:
             list containing the taken indices
         """
         if self.initial_configurations is None:
             np.random.seed(self.seed)
-            self.initial_configurations = [atoms_lst[np.random.randint(len(atoms_lst))]]
+            initial_configurations = [atoms_lst[np.random.randint(len(atoms_lst))]]
+            self.n_configurations -= 1
+        else:
+            initial_configurations = self.initial_configurations
         selected_atoms = []
         # we don't change the analyte, so we don't want to recompute the
         # SOAP vector every time.
         self.kernel.analyte = atoms_lst[:: self.correlation_time]
         self.kernel.remove_database = False
         self.kernel.load_analyte = False
         self.kernel.disable_tqdm = True
 
         self.kernel_results = []
+        hist_results = []
+
         # TODO do not use the atoms in atoms_list but store the ids directly
-        for _ in tqdm.trange(self.n_configurations, ncols=70):
-            self.kernel.reference = self.initial_configurations + selected_atoms
-            self.kernel.run()
-
-            minimum_indices = np.argsort(self.kernel.result)[: self.points_per_cycle]
-            selected_atoms += [self.kernel.analyte[x.item()] for x in minimum_indices]
-            # There is currently no check in place to ensure that an atom is only
-            # selected once. This should inherently be ensured by the way the
-            # MMK selects configurations.
-            self.kernel.load_analyte = True
-            self.kernel_results.append(self.kernel.result)
+        try:
+            for idx in tqdm.trange(self.n_configurations, ncols=70):
+                self.kernel.reference = initial_configurations + selected_atoms
+                self.kernel.run()
+
+                minimum_indices = np.argsort(self.kernel.result)[: self.points_per_cycle]
+                selected_atoms += [self.kernel.analyte[x.item()] for x in minimum_indices]
+                # There is currently no check in place to ensure that an atom is only
+                # selected once. This should inherently be ensured by the way the
+                # MMK selects configurations.
+                self.kernel.load_analyte = True
+                self.kernel_results.append(self.kernel.result)
+                if self.threshold is not None:
+                    hist, bins = np.histogram(
+                        self.kernel.result, bins=np.linspace(0, 1, 10000), density=True
+                    )
+                    bins = bins[:-1]
+                    hist[bins > self.threshold] = 0
+                    hist_results.append(np.trapz(hist, bins))
+                    if hist_results[-1] == 0:
+                        log.warning(
+                            f"Threshold {self.threshold} reached before"
+                            f" {self.n_configurations} configurations were selected -"
+                            f" stopping after selecting {idx + 1} configurations."
+                        )
+                        break
+        finally:
+            self.kernel.unlink_database()
 
-        self.kernel.unlink_database()
+        if self.initial_configurations is None:
+            # include the randomly selected configuration
+            selected_atoms += initial_configurations
+            self.n_configurations += 1
 
         selected_ids = [
             idx for idx, atom in enumerate(atoms_lst) if atom in selected_atoms
         ]
-        if len(selected_ids) != self.n_configurations:
-            raise ValueError(
-                f"Unable to select {self.n_configurations}. Could only select"
-                f" {len(selected_ids)}"
-            )
+        if self.threshold is None:
+            if len(selected_ids) != self.n_configurations:
+                print(f"{self.initial_configurations = }")
+                raise ValueError(
+                    f"Unable to select {self.n_configurations}. Could only select"
+                    f" {len(selected_ids)}"
+                )
 
         return selected_ids
 
     def plot_kernel(self, duration: int = 1000, remove: bool = True):
         """Generate an animation of the Kernel change while extending the reference.
 
         Raises
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/random.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/split.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Module for selecting Atoms randomly."""
+
 import typing
 
 import ase
 import numpy as np
 import zntrack
 
 from ipsuite.configuration_selection import ConfigurationSelection
 
 
-class RandomSelection(ConfigurationSelection):
-    """Select atoms randomly."""
+class SplitSelection(ConfigurationSelection):
+    """Select the first n % of the data.
+
+    Attributes
+    ----------
+    split : float
+        The percentage of the data to select.
+    """
 
-    n_configurations = zntrack.zn.params()
-    seed = zntrack.zn.params(1234)
+    split = zntrack.params()
 
     def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
         """Select Atoms randomly."""
-        np.random.seed(self.seed)
-        return np.random.choice(
-            len(atoms_lst), size=self.n_configurations, replace=False
-        ).tolist()
+        return np.arange(len(atoms_lst))[: int(len(atoms_lst) * self.split)].tolist()
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/threshold.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/threshold.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,111 @@
 """Selecting atoms with a given step between them."""
+
 import typing
 
 import ase
 import matplotlib.pyplot as plt
 import numpy as np
 import zntrack
 
-from ipsuite.analysis.ensemble import plot_with_uncertainty
 from ipsuite.configuration_selection import ConfigurationSelection
 
 
+def mean_reduction(values, axis):
+    return np.mean(values, axis=axis)
+
+
+def max_reduction(values, axis):
+    return np.max(values, axis=axis)
+
+
+def check_dimension(values):
+    if values.ndim > 1:
+        raise ValueError(
+            f"Value dimension is {values.ndim} != 1. "
+            "Reduce the dimension by defining dim_reduction, "
+            "use mean or max to get (n_structures,) shape."
+        )
+
+
+REDUCTIONS = {
+    "mean": mean_reduction,
+    "max": max_reduction,
+}
+
+
 class ThresholdSelection(ConfigurationSelection):
     """Select atoms based on a given threshold.
 
     Select atoms above a given threshold or the n_configurations with the
     highest / lowest value. Typically useful for uncertainty based selection.
 
     Attributes
     ----------
     key: str
-        the key in 'calc.results' to select from
+        The key in 'calc.results' to select from
     threshold: float, optional
         All values above (or below if negative) this threshold will be selected.
         If n_configurations is given, 'self.threshold' will be prioritized,
         but a maximum of n_configurations will be selected.
     reference: str, optional
         For visualizing the selection a reference value can be given.
         For 'energy_uncertainty' this would typically be 'energy'.
     n_configurations: int, optional
-        number of configurations to select.
+        Number of configurations to select.
     min_distance: int, optional
-        minimum distance between selected configurations.
+        Minimum distance between selected configurations.
+    dim_reduction: str, optional
+        Reduces the dimensionality of the chosen uncertainty along the specified axis
+        by calculating either the maximum or mean value.
+
+        Choose from ["max", "mean"]
+    reduction_axis: tuple(int), optional
+        Specifies the axis along which the reduction occurs.
     """
 
-    key = zntrack.zn.params("energy_uncertainty")
-    reference = zntrack.zn.params("energy")
-    threshold = zntrack.zn.params(None)
-    n_configurations = zntrack.zn.params(None)
-    min_distance: int = zntrack.zn.params(1)
-    img_selection = zntrack.dvc.outs(zntrack.nwd / "selection.png")
+    key = zntrack.params("energy_uncertainty")
+    reference = zntrack.params("energy")
+    threshold = zntrack.params(None)
+    n_configurations = zntrack.params(None)
+    min_distance: int = zntrack.params(1)
+    dim_reduction: str = zntrack.params(None)
+    reduction_axis = zntrack.params((1, 2))
 
     def _post_init_(self):
         if self.threshold is None and self.n_configurations is None:
             raise ValueError("Either 'threshold' or 'n_configurations' must not be None.")
 
         return super()._post_init_()
 
-    def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
+    def select_atoms(
+        self, atoms_lst: typing.List[ase.Atoms], save_fig: bool = True
+    ) -> typing.List[int]:
         """Take every nth (step) object of a given atoms list.
 
         Parameters
         ----------
         atoms_lst: typing.List[ase.Atoms]
             list of atoms objects to arange
 
         Returns
         -------
         typing.List[int]:
             list containing the taken indices
         """
+
+        self.reduction_axis = tuple(self.reduction_axis)
         values = np.array([atoms.calc.results[self.key] for atoms in atoms_lst])
+
+        if self.dim_reduction is not None:
+            reduction_fn = REDUCTIONS[self.dim_reduction]
+            values = reduction_fn(values, self.reduction_axis)
+
+        check_dimension(values)
+
         if self.threshold is not None:
             if self.threshold < 0:
                 indices = np.where(values < self.threshold)[0]
                 if self.n_configurations is not None:
                     indices = np.argsort(values)[indices]
             else:
                 indices = np.where(values > self.threshold)[0]
@@ -71,39 +113,37 @@
                     indices = np.argsort(values)[::-1][indices]
         else:
             if np.mean(values) > 0:
                 indices = np.argsort(values)[::-1]
             else:
                 indices = np.argsort(values)
 
+        selection = self.get_selection(indices)
+
+        return selection
+
+    def get_selection(self, indices):
         selected = []
         for val in indices:
             # If the value is close to any of the already selected values, skip it.
             if not any(np.abs(val - np.array(selected)) < self.min_distance):
                 selected.append(val)
             if len(selected) == self.n_configurations:
                 break
 
-        self._get_plot(atoms_lst, np.array(selected))
-
         return selected
 
     def _get_plot(self, atoms_lst: typing.List[ase.Atoms], indices: typing.List[int]):
+        indices = np.array(indices)
         values = np.array([atoms.calc.results[self.key] for atoms in atoms_lst])
-        if self.reference is not None:
-            reference = np.array(
-                [atoms.calc.results[self.reference] for atoms in atoms_lst]
-            )
-            fig, ax, _ = plot_with_uncertainty(
-                {"std": values, "mean": reference},
-                ylabel=self.key,
-                xlabel="configuration",
-            )
-            ax.plot(indices, reference[indices], "x", color="red")
-        else:
-            fig, ax = plt.subplots()
-            ax.plot(values, label=self.key)
-            ax.plot(indices, values[indices], "x", color="red")
-            ax.set_ylabel(self.key)
-            ax.set_xlabel("configuration")
+
+        if self.dim_reduction is not None:
+            reduction_fn = REDUCTIONS[self.dim_reduction]
+            values = reduction_fn(values, self.reduction_axis)
+
+        fig, ax = plt.subplots()
+        ax.plot(values, label=self.key)
+        ax.plot(indices, values[indices], "x", color="red")
+        ax.set_ylabel(self.key)
+        ax.set_xlabel("configuration")
 
         fig.savefig(self.img_selection, bbox_inches="tight")
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/uniform_arange.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/uniform_arange.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Selecting atoms with a given step between them."""
+
 import typing
 
 import ase
 import numpy as np
 import zntrack
 
 from ipsuite.configuration_selection import ConfigurationSelection
@@ -13,15 +14,15 @@
 
     Attributes
     ----------
     step: int
         setting the step, every nth (step) object will be taken
     """
 
-    step = zntrack.zn.params()
+    step = zntrack.params()
 
     def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
         """Take every nth (step) object of a given atoms list.
 
         Parameters
         ----------
         atoms_lst: typing.List[ase.Atoms]
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/uniform_energetic.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/uniform_energetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for selecting atoms uniformly in energy space."""
+
 import logging
 import typing
 
 import ase
 import numpy as np
 import zntrack
 
@@ -10,15 +11,15 @@
 
 log = logging.getLogger(__name__)
 
 
 class UniformEnergeticSelection(ConfigurationSelection):
     """A class to perform data selection based on uniform global energy selection."""
 
-    n_configurations = zntrack.zn.params()
+    n_configurations = zntrack.params()
 
     def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
         """Select Atoms uniform in energy space."""
         log.warning(f"Running search for {self.n_configurations} to max {len(atoms_lst)}")
 
         data = np.array([x.get_potential_energy() for x in atoms_lst])
```

### Comparing `ipsuite-0.1.1/ipsuite/configuration_selection/uniform_temporal.py` & `ipsuite-0.1.2/ipsuite/configuration_selection/uniform_temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Module for selecting atoms uniform in time."""
+
 import typing
 
 import ase
 import numpy as np
 import zntrack
 
 from ipsuite.configuration_selection import ConfigurationSelection
 
 
 class UniformTemporalSelection(ConfigurationSelection):
     """Select atoms uniform in time."""
 
-    n_configurations = zntrack.zn.params()
+    n_configurations = zntrack.params()
 
     def select_atoms(self, atoms_lst: typing.List[ase.Atoms]) -> typing.List[int]:
         """Select Atoms uniform in time."""
         return (
             np.round(np.linspace(0, len(atoms_lst) - 1, self.n_configurations))
             .astype(int)
             .tolist()
```

### Comparing `ipsuite-0.1.1/ipsuite/data_loading/add_data_ase.py` & `ipsuite-0.1.2/ipsuite/data_loading/add_data_ase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """ipsuite data loading with ASE."""
+
+import functools
 import logging
 import pathlib
 import typing
 
 import ase.io
 import tqdm
 import zntrack
@@ -36,27 +38,53 @@
     ):
         if lines_to_read is not None and config >= lines_to_read:
             break
         atoms.append(atom)
     return atoms
 
 
+class ReadData(base.IPSNode):
+    """Read data without converting it to H5MD.
+
+    This Node can be used instead of `AddData` to avoid
+    initial conversion to H5MD. Later Nodes might still
+    convert the data to H5MD.
+
+    Attributes
+    ----------
+    file: str|Path
+        path to the file that should be read.
+    lines_to_read: int, optional
+        maximal number of lines/configurations to read, None for read all
+    """
+
+    file: typing.Union[str, pathlib.Path] = zntrack.deps_path()
+    lines_to_read: int = zntrack.params(None)
+
+    def run(self):
+        pass
+
+    @functools.cached_property
+    def atoms(self) -> typing.List[ase.Atoms]:
+        return load_data(self.file, self.lines_to_read)
+
+
 class AddData(base.IPSNode):
     """Add data using ASE.
 
     Attributes
     ----------
     use_dvc: bool
         Don't use the filename as a parameter but rather use dvc add <file>
         to track the file with DVC.
     """
 
     atoms: typing.List[ase.Atoms] = fields.Atoms()
     file: typing.Union[str, pathlib.Path] = zntrack.dvc.deps()
-    lines_to_read: int = zntrack.zn.params(None)
+    lines_to_read: int = zntrack.params(None)
 
     def _post_init_(self):
         if not pathlib.Path(pathlib.Path(self.file).name + ".dvc").exists():
             log.warning(
                 f"Please run 'dvc add {self.file}' to track the file with DVC. Otherwise,"
                 " it might end up being git tracked."
             )
```

### Comparing `ipsuite-0.1.1/ipsuite/data_loading/add_data_h5md.py` & `ipsuite-0.1.2/ipsuite/data_loading/add_data_h5md.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Load Data directly from a H5MD trajectory file."""
+
 import functools
 import typing
 
 import ase
 import h5py
 import znh5md
 import zntrack
```

### Comparing `ipsuite-0.1.1/ipsuite/fields/atoms.py` & `ipsuite-0.1.2/ipsuite/fields/atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Lazy ASE Atoms loading."""
+
 import functools
 import typing
 
 import h5py
 import znh5md
 import zntrack
```

### Comparing `ipsuite-0.1.1/ipsuite/geometry/barycenter_coarse_grain.py` & `ipsuite-0.1.2/ipsuite/geometry/barycenter_coarse_grain.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/geometry/graphs.py` & `ipsuite-0.1.2/ipsuite/geometry/graphs.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/geometry/mapping.py` & `ipsuite-0.1.2/ipsuite/geometry/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Molecule Mapping using networkx"""
+
 import typing
 
 import ase
 
 from ipsuite import base
 from ipsuite.geometry import barycenter_coarse_grain, graphs, unwrap
```

### Comparing `ipsuite-0.1.1/ipsuite/geometry/unwrap.py` & `ipsuite-0.1.2/ipsuite/geometry/unwrap.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/models/base.py` & `ipsuite-0.1.2/ipsuite/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base class for all MLModel Implementations."""
+
 import pathlib
 import typing
 
 import ase.calculators.calculator
 import ase.io
 import tqdm
 import zntrack
@@ -12,17 +13,17 @@
 
 
 class MLModel(base.AnalyseAtoms):
     """Parent class for all MLModel Implementations."""
 
     _name_ = "MLModel"
 
-    use_energy: bool = zntrack.zn.params(True)
-    use_forces: bool = zntrack.zn.params(True)
-    use_stresses: bool = zntrack.zn.params(False)
+    use_energy: bool = zntrack.params(True)
+    use_forces: bool = zntrack.params(True)
+    use_stresses: bool = zntrack.params(False)
 
     def get_calculator(self, **kwargs) -> ase.calculators.calculator.Calculator:
         """Get a model specific ase calculator object.
 
         Returns
         -------
         calc:
```

### Comparing `ipsuite-0.1.1/ipsuite/models/ensemble.py` & `ipsuite-0.1.2/ipsuite/models/ensemble.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing
-from uuid import uuid4
 
 import ase
 import numpy as np
 import zntrack
 from ase.calculators.calculator import Calculator, all_changes
 from tqdm import tqdm
 
@@ -50,18 +49,16 @@
                 [x.get_stress() for x in results], axis=0
             )
 
 
 class EnsembleModel(base.IPSNode):
     models: typing.List[MLModel] = zntrack.deps()
 
-    uuid = zntrack.zn.outs()  # to connect this Node to other Nodes it requires an output.
-
     def run(self) -> None:
-        self.uuid = str(uuid4())
+        pass
 
     def get_calculator(self, **kwargs) -> ase.calculators.calculator.Calculator:
         """Property to return a model specific ase calculator object.
 
         Returns
         -------
         calc:
```

### Comparing `ipsuite-0.1.1/ipsuite/models/gap.py` & `ipsuite-0.1.2/ipsuite/models/gap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Description.
 
 GAP module to perform training using the Gaussian process
 regression from Gabor Csanyi.
 """
+
 import dataclasses
 import importlib.resources as pkg_resources
 import logging
 import subprocess as sp
 import typing
 from collections import OrderedDict
 from pathlib import Path
@@ -16,15 +17,15 @@
 import quippy.potential
 import xmltodict
 import znflow
 import zntrack
 from jinja2 import Template
 from znjson import ConverterBase, config
 
-from ipsuite import static_data, utils
+from ipsuite import static_data
 from ipsuite.models import MLModel
 
 log = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass()
 class SOAP:
@@ -193,24 +194,24 @@
     model_outputs: Path
         Path to save model files
     train_data: List[ase.Atoms]
         atoms object to train the model on
     """
 
     # SOAP
-    soap: typing.Union[dict, SOAP] = zntrack.zn.params(SOAP())
+    soap: typing.Union[dict, SOAP] = zntrack.params(SOAP())
     # DistanceNb
-    distance_nb: typing.Union[dict, DistanceNb] = zntrack.zn.params(DistanceNb())
+    distance_nb: typing.Union[dict, DistanceNb] = zntrack.params(DistanceNb())
     # GAP
-    gap: typing.Union[dict, GapParameter] = zntrack.zn.params(GapParameter())
+    gap: typing.Union[dict, GapParameter] = zntrack.params(GapParameter())
     # #
-    model_directory: Path = zntrack.dvc.outs(zntrack.nwd / "model")
-    train_data_file: Path = zntrack.dvc.outs(zntrack.nwd / "train_atoms.extxyz")
-    gap_input_script: Path = zntrack.dvc.outs(zntrack.nwd / "gap.input")
-    _train_idx_file: Path = zntrack.dvc.outs(zntrack.nwd / "train_atoms.extxyz.idx")
+    model_directory: Path = zntrack.outs_path(zntrack.nwd / "model")
+    train_data_file: Path = zntrack.outs_path(zntrack.nwd / "train_atoms.extxyz")
+    gap_input_script: Path = zntrack.outs_path(zntrack.nwd / "gap.input")
+    _train_idx_file: Path = zntrack.outs_path(zntrack.nwd / "train_atoms.extxyz.idx")
 
     #
     OPENBLAS_NUM_THREADS = zntrack.meta.Environment(None)
 
     #
     def _post_init_(self):
         if not self.state.loaded:
@@ -223,15 +224,14 @@
 
             if isinstance(self.soap, dict):
                 self.soap = SOAP(**self.soap)
             if isinstance(self.gap, dict):
                 self.gap = GapParameter(**self.gap)
             if isinstance(self.distance_nb, dict):
                 self.distance_nb = DistanceNb(**self.distance_nb)
-            self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
 
     def run(self):
         """Create output directory and train the model."""
         self.model_directory.mkdir(exist_ok=True, parents=True)
         self.train_model()
 
     @property
```

### Comparing `ipsuite-0.1.1/ipsuite/models/mace_model.py` & `ipsuite-0.1.2/ipsuite/models/mace_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import pandas as pd
 import torch
 import yaml
 import zntrack
 from mace.calculators import MACECalculator
 
-from ipsuite import utils
 from ipsuite.models import MLModel
 from ipsuite.static_data import STATIC_PATH
 
 log = logging.getLogger(__name__)
 
 
 def execute(cmd, **kwargs):
@@ -31,34 +30,30 @@
     if return_code := popen.wait():  # finally a use for walrus operator
         raise subprocess.CalledProcessError(return_code, cmd)
 
 
 class MACE(MLModel):
     """MACE model."""
 
-    train_data_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "train-data.extxyz")
+    train_data_file: pathlib.Path = zntrack.outs_path(zntrack.nwd / "train-data.extxyz")
 
     test_data = zntrack.deps()
-    test_data_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "test-data.extxyz")
-    model_dir: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "model")
+    test_data_file: pathlib.Path = zntrack.outs_path(zntrack.nwd / "test-data.extxyz")
+    model_dir: pathlib.Path = zntrack.outs_path(zntrack.nwd / "model")
 
-    config: str = zntrack.dvc.params("mace.yaml")
+    config: str = zntrack.params_path("mace.yaml")
     device: str = zntrack.meta.Text(None)
 
-    training: pathlib.Path = zntrack.dvc.plots(
+    training: pathlib.Path = zntrack.plots_path(
         zntrack.nwd / "training.csv",
         template=STATIC_PATH / "y_log.json",
         x="epoch",
         y=["loss", "rmse_e_per_atom", "rmse_f"],
     )
 
-    def _post_init_(self):
-        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
-        self.test_data = utils.helpers.get_deps_if_node(self.test_data, "atoms")
-
     def _post_load_(self) -> None:
         if self.device is None:
             self.device = "cuda" if torch.cuda.is_available() else "cpu"
 
     @classmethod
     def generate_config_file(self, file: str = "mace.yaml"):
         example = {
@@ -78,36 +73,36 @@
             "E0s": "average",
         }
         pathlib.Path(file).write_text(yaml.safe_dump(example))
 
     def run(self):
         """Train a MACE model."""
         self.model_dir.mkdir(parents=True, exist_ok=True)
-        cmd = """curl -sSL https://raw.githubusercontent.com/ACEsuit/mace/main/scripts/run_train.py | python - """  # noqa E501
-        cmd += '--name="MACE_model" '
-        cmd += f'--train_file="{self.train_data_file.resolve().as_posix()}" '
-        cmd += "--valid_fraction=0.05 "
-        cmd += f'--test_file="{self.test_data_file.resolve().as_posix()}" '
-        cmd += f"--device={self.device} "
+        cmd = ["mace_run_train"]
+        cmd.append("--name=MACE_model")
+        cmd.append(f"--train_file={self.train_data_file.resolve().as_posix()}")
+        cmd.append("--valid_fraction=0.05")
+        cmd.append(f"--test_file={self.test_data_file.resolve().as_posix()}")
+        cmd.append(f"--device={self.device}")
 
         config = yaml.safe_load(pathlib.Path(self.config).read_text())
         for key, val in config.items():
             if val is True:
-                cmd += f"--{key} "
+                cmd.append(f"--{key}")
             elif val is False:
                 pass
             else:
-                cmd += f'--{key}="{val}" '
+                cmd.append(f"--{key}={val}")
 
         self.write_data_to_file(file=self.train_data_file, atoms_list=self.data)
         self.write_data_to_file(file=self.test_data_file, atoms_list=self.test_data)
 
         log.debug(f"Running: {cmd}")
 
-        for path in execute(cmd, shell=True, cwd=self.model_dir):
+        for path in execute(cmd, cwd=self.model_dir):
             print(path, end="")
             file = list((self.model_dir / "results").glob("*.*"))
             if len(file) == 1:
                 data = []
 
                 with file[0].open() as f:
                     for line in f.readlines():
@@ -121,15 +116,20 @@
         """Return the ASE calculator."""
         import unittest.mock
 
         with self.state.fs.open(self.config) as f:
             config = yaml.safe_load(f)
             default_dtype = config.get("default_dtype", "float64")
 
+        if self.state.fs.exists(self.model_dir / "MACE_model_swa.model"):
+            model_name = "MACE_model_swa.model"
+        else:
+            model_name = "MACE_model.model"
+
         with unittest.mock.patch(
             "torch.serialization._open_file_like", self.state.fs.open
         ):
             return MACECalculator(
-                model_path=self.model_dir / "MACE_model_swa.model",
+                model_paths=self.model_dir / model_name,
                 device=device or self.device,
                 default_dtype=default_dtype,
             )
```

### Comparing `ipsuite-0.1.1/ipsuite/models/nequip.py` & `ipsuite-0.1.2/ipsuite/models/nequip.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """The Nequip and allegro model module."""
+
 import logging
 import pathlib
 import shutil
 import subprocess
 import typing
 
 import ase.io
 import ase.symbols
 import pandas as pd
 import torch
 import yaml
 import zntrack
 import zntrack.utils
 
-from ipsuite import utils
 from ipsuite.models import MLModel
 from ipsuite.utils.helpers import check_duplicate_keys
 
 log = logging.getLogger(__name__)
 
 
 def _write_xyz_input_files(
@@ -33,40 +33,40 @@
 
     return n_train, chemical_symbols
 
 
 class Nequip(MLModel):
     """The Nequip and allegro model."""
 
-    config: str = zntrack.dvc.params()
+    config: str = zntrack.params_path()
     validation_data = zntrack.deps()
 
-    train_data_file: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "train.extxyz")
-    validation_data_file: pathlib.Path = zntrack.dvc.outs(
+    train_data_file: pathlib.Path = zntrack.outs_path(zntrack.nwd / "train.extxyz")
+    validation_data_file: pathlib.Path = zntrack.outs_path(
         zntrack.nwd / "validation.extxyz"
     )
 
-    deployed_model: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "deployed_model.pth")
-    model_directory: pathlib.Path = zntrack.dvc.outs(zntrack.nwd / "model")
+    deployed_model: pathlib.Path = zntrack.outs_path(zntrack.nwd / "deployed_model.pth")
+    model_directory: pathlib.Path = zntrack.outs_path(zntrack.nwd / "model")
 
-    metrics_batch_train = zntrack.dvc.plots(
+    metrics_batch_train = zntrack.plots_path(
         zntrack.nwd / "metrics_batch_train.csv"  # , y=" loss", y_label="loss"
     )
-    metrics_batch_val = zntrack.dvc.plots(
+    metrics_batch_val = zntrack.plots_path(
         zntrack.nwd / "metrics_batch_val.csv"  # , y=" loss", y_label="loss"
     )
-    metrics_epoch = zntrack.dvc.plots(
+    metrics_epoch = zntrack.plots_path(
         zntrack.nwd / "metrics_epoch.csv",
         # x="epoch",
         # x_label="epochs",
         # y="validation_loss",
         # y_label="validation loss",
     )
 
-    metrics = zntrack.zn.metrics()
+    metrics = zntrack.metrics()
 
     device: str = zntrack.meta.Text("cuda" if torch.cuda.is_available() else "cpu")
     remove_processed_dataset = True
 
     def _post_init_(self):
         """Post init hook."""
         if not self.state.loaded:
@@ -74,19 +74,14 @@
                 raise ValueError("Can not train nequip model without a parameter file")
             else:
                 log.info(
                     "Please keep track of the parameter file with git, just like the"
                     f" params.yaml. Use 'git add {self.config}'."
                 )
 
-        self.data = utils.helpers.get_deps_if_node(self.data, "atoms")
-        self.validation_data = utils.helpers.get_deps_if_node(
-            self.validation_data, "atoms"
-        )
-
     def _handle_parameter_file(self, n_train: int, n_val: int, chemical_symbols: list):
         """Update and rewrite the nequip parameter file."""
         parameter = pathlib.Path(self.config).read_text()
         parameter = yaml.safe_load(parameter)
 
         custom_parameters = {
             "root": self.model_directory.as_posix(),
```

### Comparing `ipsuite-0.1.1/ipsuite/nodes.py` & `ipsuite-0.1.2/ipsuite/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,31 @@
     SplitSelection = "ipsuite.configuration_selection.SplitSelection"
     UniformArangeSelection = "ipsuite.configuration_selection.UniformArangeSelection"
     UniformEnergeticSelection = (
         "ipsuite.configuration_selection.UniformEnergeticSelection"
     )
     UniformTemporalSelection = "ipsuite.configuration_selection.UniformTemporalSelection"
     ThresholdSelection = "ipsuite.configuration_selection.ThresholdSelection"
+    FilterOutlier = "ipsuite.configuration_selection.FilterOutlier"
+    BatchKernelSelection = "ipsuite.models.apax.BatchKernelSelection"
 
     # Configuration Comparison
     REMatch = "ipsuite.configuration_comparison.REMatch"
     MMKernel = "ipsuite.configuration_comparison.MMKernel"
 
     # Configuration Generation
     Packmol = "ipsuite.configuration_generation.Packmol"
+    MultiPackmol = "ipsuite.configuration_generation.MultiPackmol"
     SmilesToAtoms = "ipsuite.configuration_generation.SmilesToAtoms"
     SmilesToConformers = "ipsuite.configuration_generation.SmilesToConformers"
 
     # Data
     AddData = "ipsuite.data_loading.AddData"
     AddDataH5MD = "ipsuite.data_loading.AddDataH5MD"
+    ReadData = "ipsuite.data_loading.ReadData"
 
     # Bootstrap
     RattleAtoms = "ipsuite.bootstrap.RattleAtoms"
     TranslateMolecules = "ipsuite.bootstrap.TranslateMolecules"
     RotateMolecules = "ipsuite.bootstrap.RotateMolecules"
     SurfaceRasterScan = "ipsuite.bootstrap.SurfaceRasterScan"
     SurfaceRasterMetrics = "ipsuite.bootstrap.SurfaceRasterMetrics"
@@ -55,49 +59,54 @@
     ForcesUncertaintyHistogram = "ipsuite.analysis.ForcesUncertaintyHistogram"
     EnergyUncertaintyHistogram = "ipsuite.analysis.EnergyUncertaintyHistogram"
     ModelEnsembleAnalysis = "ipsuite.analysis.ModelEnsembleAnalysis"
     PredictionMetrics = "ipsuite.analysis.PredictionMetrics"
     ForceAngles = "ipsuite.analysis.ForceAngles"
     RattleAnalysis = "ipsuite.analysis.RattleAnalysis"
     Prediction = "ipsuite.analysis.Prediction"
+    CalibrationMetrics = "ipsuite.analysis.CalibrationMetrics"
     BoxScale = "ipsuite.analysis.BoxScale"
     BoxHeatUp = "ipsuite.analysis.BoxHeatUp"
     NaNCheck = "ipsuite.analysis.NaNCheck"
     ConnectivityCheck = "ipsuite.analysis.ConnectivityCheck"
     EnergySpikeCheck = "ipsuite.analysis.EnergySpikeCheck"
     MDStability = "ipsuite.analysis.MDStability"
     MoveSingleParticle = "ipsuite.analysis.MoveSingleParticle"
     AnalyseGlobalForceSensitivity = "ipsuite.analysis.AnalyseGlobalForceSensitivity"
     AnalyseSingleForceSensitivity = "ipsuite.analysis.AnalyseSingleForceSensitivity"
     ForceDecomposition = "ipsuite.analysis.ForceDecomposition"
     ThresholdCheck = "ipsuite.analysis.ThresholdCheck"
     TemperatureCheck = "ipsuite.analysis.TemperatureCheck"
     FixedSphereConstraint = "ipsuite.calculators.FixedSphereConstraint"
+    FixedLayerConstraint = "ipsuite.calculators.FixedLayerConstraint"
+    AnalyseDensity = "ipsuite.analysis.AnalyseDensity"
 
     # calculators
     CP2KSinglePoint = "ipsuite.calculators.CP2KSinglePoint"
     CP2KYaml = "ipsuite.calculators.CP2KYaml"
     ASEGeoOpt = "ipsuite.calculators.ASEGeoOpt"
     ASEMD = "ipsuite.calculators.ASEMD"
     xTBSinglePoint = "ipsuite.calculators.xTBSinglePoint"
     LJSinglePoint = "ipsuite.calculators.LJSinglePoint"
     EMTSinglePoint = "ipsuite.calculators.EMTSinglePoint"
     OrcaSinglePoint = "ipsuite.calculators.OrcaSinglePoint"
     ApaxJaxMD = "ipsuite.calculators.ApaxJaxMD"
     LammpsSimulator = "ipsuite.calculators.LammpsSimulator"
+    MixCalculator = "ipsuite.calculators.MixCalculator"
 
     LangevinThermostat = "ipsuite.calculators.LangevinThermostat"
     NPTThermostat = "ipsuite.calculators.NPTThermostat"
     RescaleBoxModifier = "ipsuite.calculators.RescaleBoxModifier"
     BoxOscillatingRampModifier = "ipsuite.calculators.BoxOscillatingRampModifier"
     TemperatureRampModifier = "ipsuite.calculators.TemperatureRampModifier"
     TemperatureOscillatingRampModifier = (
         "ipsuite.calculators.TemperatureOscillatingRampModifier"
     )
     TemperatureRampModifier = "ipsuite.calculators.TemperatureRampModifier"
+    TorchD3 = "ipsuite.calculators.TorchD3"
 
     # Geometry
     BarycenterMapping = "ipsuite.geometry.BarycenterMapping"
 
 
 def __getattr__(name):
     """Overwrite the default __getattr__ to import the nodes lazily."""
```

### Comparing `ipsuite-0.1.1/ipsuite/static_data/gap.jinja2` & `ipsuite-0.1.2/ipsuite/static_data/gap.jinja2`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/static_data/lammps_npt.jinja2` & `ipsuite-0.1.2/ipsuite/static_data/lammps_npt.jinja2`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/static_data/y_log.json` & `ipsuite-0.1.2/ipsuite/static_data/y_log.json`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/utils/ase_sim.py` & `ipsuite-0.1.2/ipsuite/utils/ase_sim.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utils that help running simulations with ASE."""
+
 import functools
 import typing
 
 import ase
 import numpy as np
 from ase import units
 from ase.calculators.singlepoint import SinglePointCalculator
@@ -45,7 +46,40 @@
     result.calc = SinglePointCalculator(result, **atoms.calc.results)
     return result
 
 
 @freeze_copy_atoms.register
 def _(atoms: list) -> list[ase.Atoms]:
     return [freeze_copy_atoms(x) for x in atoms]
+
+
+def get_box_from_density(
+    data: list[list[ase.Atoms]], count: list[int], density: float
+) -> list[float]:
+    """Get the box size from the molar volume.
+
+    Attributes
+    ----------
+    data: list[list[ase.Atoms]]
+        List of list of atoms objects. The last atoms object is used to compute the
+        molar volume.
+    count: list[int]
+        Number of molecules for each entry in data.
+    density: float
+        Density of the system in kg/m^3.
+    """
+    molar_mass = [sum(atoms[0].get_masses()) * count for atoms, count in zip(data, count)]
+    molar_mass = sum(molar_mass)  #  g / mol
+    molar_volume = molar_mass / density / 1000  # m^3 / mol
+
+    # convert to particles / A^3
+    volume = molar_volume * (ase.units.m**3) / ase.units.mol
+
+    box = [volume ** (1 / 3) for _ in range(3)]
+    return box
+
+
+def get_density_from_atoms(atoms: ase.Atoms) -> float:
+    """Compute the density of the atoms in kg/m3."""
+    volume = atoms.get_volume()
+    molar_volume = volume / (units.m**3 / units.mol)
+    return atoms.get_masses().sum() / 1000 / molar_volume
```

### Comparing `ipsuite-0.1.1/ipsuite/utils/combine.py` & `ipsuite-0.1.2/ipsuite/utils/combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         If True, the function will return the input if it is not a
         dictionary. If False, it will raise a TypeError.
 
     Example
     -------
         >>> data = {'a': [1, 2, 3], 'b': [4, 5, 6]}
         >>> get_flat_data_from_dict(data)
-        >>> # [1, 2, 3, 4, 5, 6]
+        [1, 2, 3, 4, 5, 6]
     """
     if not isinstance(data, dict):
         if silent_ignore:
             return data
         else:
             raise TypeError(f"data must be a dictionary and not {type(data)}")
 
@@ -157,15 +157,15 @@
         If True, the function will return the input if it is not a
         dictionary. If False, it will raise a TypeError.
 
     Example
     -------
         >>> data = {'a': [1, 2, 3], 'b': [4, 5, 6]}
         >>> get_ids_per_key(data, [0, 1, 3, 5])
-        >>> # {'a': [0, 1], 'b': [0, 2]}
+        {'a': [0, 1], 'b': [0, 2]}
     """
     if not isinstance(data, dict):
         if silent_ignore:
             return np.array(ids).tolist()
         else:
             raise TypeError(f"data must be a dictionary and not {type(data)}")
```

### Comparing `ipsuite-0.1.1/ipsuite/utils/helpers.py` & `ipsuite-0.1.2/ipsuite/utils/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 """ipsuite helper modules."""
 
 import contextlib
 from logging import Logger
 
+import typing_extensions as tyex
 import znflow
 from zntrack import Node
 
 
 def setup_ase():
     """Add uncertainty keys to ASE all properties."""
     from ase.calculators.calculator import all_properties
 
-    for val in ["forces_uncertainty", "energy_uncertainty", "stress_uncertainty"]:
+    for val in [
+        "forces_uncertainty",
+        "energy_uncertainty",
+        "stress_uncertainty",
+        "node_energy",
+    ]:
         if val not in all_properties:
             all_properties.append(val)
 
 
+@tyex.deprecated(
+    "It is recommended to pass the attribute directly, instead of giving a 'zntrack.Node'"
+    " instance."
+)
 def get_deps_if_node(obj, attribute: str):
     """Apply getdeps if obj is subclass/instance of a Node.
 
     Parameters
     ----------
     obj: any
         Any object that is either a Node or not.
```

### Comparing `ipsuite-0.1.1/ipsuite/utils/logs.py` & `ipsuite-0.1.2/ipsuite/utils/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logging Setup for the ipsuite package."""
+
 import logging
 import sys
 
 
 def setup_logging(name) -> None:
     """Configure logging for the ipsuite package."""
     logger = logging.getLogger(name)
```

### Comparing `ipsuite-0.1.1/ipsuite/utils/md.py` & `ipsuite-0.1.2/ipsuite/utils/md.py`

 * *Files identical despite different names*

### Comparing `ipsuite-0.1.1/ipsuite/utils/metrics.py` & `ipsuite-0.1.2/ipsuite/utils/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Utils for computing metrics."""
+
 import numpy as np
+from scipy import stats
 
 
 def calculate_l_p_norm(y_true: np.ndarray, y_pred: np.ndarray, p: int = 2):
     r"""Calculate the mean of the l_p_norm of given data.
 
     .. math::
         l_{p} = \frac{1}{N} \sum_{i}^{N} \left| x_{i} - x_{i}^{\text{true}}\right|^{p}.
@@ -64,16 +66,19 @@
     return np.rad2deg(
         np.arccos(np.clip(np.einsum("ix, ix -> i", u_vec1, u_vec2), -1.0, 1.0))
     )
 
 
 def get_full_metrics(true: np.ndarray, prediction: np.ndarray) -> dict:
     """Calculate metrics for a given true and predicted value."""
-    return {
+    metrics = {
         "rmse": root_mean_squared_error(true, prediction),
         "mse": mean_squared_error(true, prediction),
         "mae": mean_absolute_error(true, prediction),
         "max": maximum_error(true, prediction),
         "lp4": calculate_l_p_norm(true, prediction, p=4),
         "rrmse": relative_rmse(true, prediction),
-        # "pearsonr": pearsonr(true, prediction)[0],
     }
+
+    if len(true) > 2:
+        metrics["pearsonr"] = stats.pearsonr(true, prediction)[0]
+    return metrics
```

### Comparing `ipsuite-0.1.1/pyproject.toml` & `ipsuite-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 [tool.poetry]
 name = "ipsuite"
-version = "0.1.1"
+version = "0.1.2"
 description = "A suite of tools for machine learned interatomic potentials."
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 keywords = ["data-version-control", "machine-learning", "reproducibility", "interatomic potentials"]
 license = "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)"
 readme = "README.md"
 
+[tool.poetry.urls]
+documentation = "https://ipsuite.readthedocs.io"
+repository = "https://github.com/zincware/ipsuite"
+
 [tool.poetry.dependencies]
 # tensorflow-io-gcs-filesystem
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.12"
 
 znh5md = "^0.1.6a0"
 ase = "^3.22.1"
 
 seaborn = "^0.12.2"
-# cp2k-input-tools = {git = "https://github.com/cp2k/cp2k-input-tools.git"}
+cp2k-input-tools = "^0.9"
 cp2k-output-tools = "^0.5.0"
 
 
 #[tool.poetry.group.comparison.dependencies]
 h5py = { version = "^3.8.0", optional = true }
 tensorflow = { version = "^2.11.0", optional = true }
-dscribe = { version = "^1.2.2", optional = true }
+dscribe = { version = "^2.1.0", optional = true }
 
 #[tool.poetry.group.GAP.dependencies]
 quippy-ase = { version = "^0.9.12", optional = true }
 xmltodict = "^0.13.0"
 
 nequip = { version = "^0.5.6", optional = true }
-# apax = { git = "https://github.com/apax-hub/apax.git", rev = "dev", optional = true}
 rdkit = "^2023"
 lazy-loader = "^0.2"
 znflow = "^0.1.11"
-zntrack = "^0.7.0"
+zntrack = "^0.7.2"
 
-# [tool.poetry.group.allegro.dependencies]
-# mir-allegro = { git = "https://github.com/mir-group/allegro.git", optional = true}
+[tool.poetry.group.allegro.dependencies]
+mir-allegro = { git = "https://github.com/mir-group/allegro.git", optional = true}
 
 # [tool.poetry.group.mace.dependencies]
-# mace = { git = "https://github.com/ACEsuit/mace.git", optional = true}
+mace-torch = { version = "^0.3.4", optional = true}
+torch-dftd = { version = "^0.4.0", optional = true }
+# [tool.poetry.group.apax.dependencies]
+apax = { version = "^0.4.0", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.4.0"
 pytest = "^7.2.1"
 coverage = "^7.2.1"
 imageio = "^2.28.1"
+dvc-s3 = "^3.0.1"
 
 [tool.poetry.group.notebook.dependencies]
 jupyterlab = "^3.6.1"
 ipywidgets = "^8.0.6"
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.2.6"
+furo = "^2024.1.29"
+sphinx-copybutton = "^0.5.2"
+
 [tool.poetry.extras]
 comparison = ["h5py", "tensorflow", "dscribe"]
 gap = ["quippy-ase", "xmltodict"]
 nequip = ["nequip"]
 apax = ["apax"]
-allegro = ["mir-allegro"]
-mace = ["mace"]
+# allegro = ["mir-allegro"]
+mace = ["mace-torch"]
+d3 = ["torch-dftd"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = 'black'
@@ -110,8 +124,9 @@
 # Same as Black.
 line-length = 90
 
 # Assume Python 3.10.
 target-version = "py310"
 
 [tool.codespell]
-skip = "poetry.lock,ipsuite/static_data/*"
+ignore-words-list = "dscribe"
+skip = "poetry.lock,ipsuite/static_data/*,docs/source/examples/06_Bootstrapping_Datasets.ipynb"
```

