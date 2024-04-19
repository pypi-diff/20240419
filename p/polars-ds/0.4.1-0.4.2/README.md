# Comparing `tmp/polars_ds-0.4.1.tar.gz` & `tmp/polars_ds-0.4.2.tar.gz`

## Comparing `polars_ds-0.4.1.tar` & `polars_ds-0.4.2.tar`

### file list

```diff
@@ -1,96 +1,98 @@
--rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 polars_ds-0.4.1/Cargo.toml
--rw-r--r--   0     1001      127     4744 2024-04-11 15:31:28.000000 polars_ds-0.4.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      897 2024-04-11 15:31:28.000000 polars_ds-0.4.1/.gitignore
--rw-r--r--   0     1001      127      268 2024-04-11 15:31:28.000000 polars_ds-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      442 2024-04-11 15:31:28.000000 polars_ds-0.4.1/.readthedocs.yaml
--rw-r--r--   0     1001      127     2312 2024-04-11 15:31:28.000000 polars_ds-0.4.1/CONTRIBUTING.md
--rw-r--r--   0     1001      127     1063 2024-04-11 15:31:28.000000 polars_ds-0.4.1/LICENSE.txt
--rw-r--r--   0     1001      127      715 2024-04-11 15:31:28.000000 polars_ds-0.4.1/Makefile
--rw-r--r--   0     1001      127     8927 2024-04-11 15:31:28.000000 polars_ds-0.4.1/README.md
--rw-r--r--   0     1001      127       55 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/complex.md
--rw-r--r--   0     1001      127       58 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/graph.md
--rw-r--r--   0     1001      127     8531 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/index.md
--rw-r--r--   0     1001      127       57 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/metrics.md
--rw-r--r--   0     1001      127       81 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/num.md
--rw-r--r--   0     1001      127      144 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/polars_ds.md
--rw-r--r--   0     1001      127      123 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/requirements-docs.txt
--rw-r--r--   0     1001      127       67 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/stats.md
--rw-r--r--   0     1001      127       68 2024-04-11 15:31:28.000000 polars_ds-0.4.1/docs/str2.md
--rw-r--r--   0     1001      127   122506 2024-04-11 15:31:28.000000 polars_ds-0.4.1/examples/basics.ipynb
--rw-r--r--   0     1001      127  1764254 2024-04-11 15:31:28.000000 polars_ds-0.4.1/examples/dependency.parquet
--rw-r--r--   0     1001      127   323011 2024-04-11 15:31:28.000000 polars_ds-0.4.1/examples/diagnosis.ipynb
--rw-r--r--   0     1001      127    31063 2024-04-11 15:31:28.000000 polars_ds-0.4.1/examples/sample_and_split.ipynb
--rw-r--r--   0     1001      127      609 2024-04-11 15:31:28.000000 polars_ds-0.4.1/mkdocs.yml
--rw-r--r--   0     1001      127     3230 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/__init__.py
--rw-r--r--   0     1001      127     1243 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/_utils.py
--rw-r--r--   0     1001      127     7324 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/complex.py
--rw-r--r--   0     1001      127    17498 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/diagnosis.py
--rw-r--r--   0     1001      127     7188 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/graph.py
--rw-r--r--   0     1001      127    13270 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/metrics.py
--rw-r--r--   0     1001      127    46127 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/num.py
--rw-r--r--   0     1001      127     6080 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/sample.py
--rw-r--r--   0     1001      127    29669 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/stats.py
--rw-r--r--   0     1001      127    31957 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/str2.py
--rw-r--r--   0     1001      127     1133 2024-04-11 15:31:28.000000 polars_ds-0.4.1/python/polars_ds/type_alias.py
--rw-r--r--   0     1001      127       83 2024-04-11 15:31:28.000000 polars_ds-0.4.1/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-11 15:31:28.000000 polars_ds-0.4.1/rust-toolchain.toml
--rw-r--r--   0     1001      127     2089 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/graph/degree.rs
--rw-r--r--   0     1001      127     4158 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/graph/eigen_centrality.rs
--rw-r--r--   0     1001      127     3146 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/graph/mod.rs
--rw-r--r--   0     1001      127     8711 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/graph/shortest_path.rs
--rw-r--r--   0     1001      127      412 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/lib.rs
--rw-r--r--   0     1001      127      967 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/cond_entropy.rs
--rw-r--r--   0     1001      127     4186 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/convolve.rs
--rw-r--r--   0     1001      127     7150 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/entrophies.rs
--rw-r--r--   0     1001      127     2536 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/fft.rs
--rw-r--r--   0     1001      127     9462 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/float_extras.rs
--rw-r--r--   0     1001      127     1383 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/gcd_lcm.rs
--rw-r--r--   0     1001      127     2734 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/haversine.rs
--rw-r--r--   0     1001      127     8843 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/jaccard.rs
--rw-r--r--   0     1001      127    18850 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/knn.rs
--rw-r--r--   0     1001      127      808 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/lempel_ziv.rs
--rw-r--r--   0     1001      127     3102 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/mod.rs
--rw-r--r--   0     1001      127     9638 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/ols.rs
--rw-r--r--   0     1001      127     3707 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/psi.rs
--rw-r--r--   0     1001      127     2064 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/target_encode.rs
--rw-r--r--   0     1001      127     5762 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/tp_fp.rs
--rw-r--r--   0     1001      127     1422 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/trapz.rs
--rw-r--r--   0     1001      127     2659 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/num/woe_iv.rs
--rw-r--r--   0     1001      127     2251 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/chi2.rs
--rw-r--r--   0     1001      127     3630 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/fstats.rs
--rw-r--r--   0     1001      127     2816 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/ks.rs
--rw-r--r--   0     1001      127     1098 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/mod.rs
--rw-r--r--   0     1001      127     3383 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/normal_test.rs
--rw-r--r--   0     1001      127    15501 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/sample.rs
--rw-r--r--   0     1001      127     6054 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats/t_test.rs
--rw-r--r--   0     1001      127     4235 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats_utils/beta.rs
--rw-r--r--   0     1001      127     6734 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats_utils/gamma.rs
--rw-r--r--   0     1001      127      895 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats_utils/mod.rs
--rw-r--r--   0     1001      127    18992 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/stats_utils/normal.rs
--rw-r--r--   0     1001      127     2221 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/consts.rs
--rw-r--r--   0     1001      127     3082 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/fuzz.rs
--rw-r--r--   0     1001      127    11287 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/hamming.rs
--rw-r--r--   0     1001      127     1066 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/inflections.rs
--rw-r--r--   0     1001      127      483 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/is_stopword.rs
--rw-r--r--   0     1001      127     5723 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/jaro.rs
--rw-r--r--   0     1001      127     7937 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/knn_strs.rs
--rw-r--r--   0     1001      127    13628 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/levenshtein.rs
--rw-r--r--   0     1001      127     1159 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/mod.rs
--rw-r--r--   0     1001      127     5731 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/osa.rs
--rw-r--r--   0     1001      127     3051 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/overlap.rs
--rw-r--r--   0     1001      127    24197 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/snowball/algorithms/english_stemmer.rs
--rw-r--r--   0     1001      127      110 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/snowball/algorithms/mod.rs
--rw-r--r--   0     1001      127      198 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/snowball/among.rs
--rw-r--r--   0     1001      127     1371 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/snowball/mod.rs
--rw-r--r--   0     1001      127    12885 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/snowball/snowball_env.rs
--rw-r--r--   0     1001      127      870 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/snowball_stem.rs
--rw-r--r--   0     1001      127     3059 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/sorensen_dice.rs
--rw-r--r--   0     1001      127     3050 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/str_jaccard.rs
--rw-r--r--   0     1001      127     3461 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/str2/tversky.rs
--rw-r--r--   0     1001      127     2447 2024-04-11 15:31:28.000000 polars_ds-0.4.1/src/utils/mod.rs
--rw-r--r--   0     1001      127      126 2024-04-11 15:31:28.000000 polars_ds-0.4.1/tests/requirements-test.txt
--rw-r--r--   0     1001      127     3490 2024-04-11 15:31:28.000000 polars_ds-0.4.1/tests/test.ipynb
--rw-r--r--   0     1001      127    37617 2024-04-11 15:31:28.000000 polars_ds-0.4.1/tests/test_correctness.py
--rw-r--r--   0     1001      127    72334 2024-04-11 15:31:28.000000 polars_ds-0.4.1/Cargo.lock
--rw-r--r--   0     1001      127      961 2024-04-11 15:31:28.000000 polars_ds-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9645 1970-01-01 00:00:00.000000 polars_ds-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 polars_ds-0.4.2/Cargo.toml
+-rw-r--r--   0     1001      127     4742 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      897 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.gitignore
+-rw-r--r--   0     1001      127      268 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      442 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.readthedocs.yaml
+-rw-r--r--   0     1001      127     2312 2024-04-19 02:51:18.000000 polars_ds-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     1063 2024-04-19 02:51:18.000000 polars_ds-0.4.2/LICENSE.txt
+-rw-r--r--   0     1001      127      715 2024-04-19 02:51:18.000000 polars_ds-0.4.2/Makefile
+-rw-r--r--   0     1001      127     8927 2024-04-19 02:51:18.000000 polars_ds-0.4.2/README.md
+-rw-r--r--   0     1001      127       55 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/complex.md
+-rw-r--r--   0     1001      127       58 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/graph.md
+-rw-r--r--   0     1001      127     8531 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/index.md
+-rw-r--r--   0     1001      127       57 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/metrics.md
+-rw-r--r--   0     1001      127       81 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/num.md
+-rw-r--r--   0     1001      127      144 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/polars_ds.md
+-rw-r--r--   0     1001      127      123 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/requirements-docs.txt
+-rw-r--r--   0     1001      127       67 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/stats.md
+-rw-r--r--   0     1001      127       68 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/str2.md
+-rw-r--r--   0     1001      127   125731 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/basics.ipynb
+-rw-r--r--   0     1001      127  1764254 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/dependency.parquet
+-rw-r--r--   0     1001      127   386350 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/diagnosis.ipynb
+-rw-r--r--   0     1001      127    31063 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/sample_and_split.ipynb
+-rw-r--r--   0     1001      127      609 2024-04-19 02:51:18.000000 polars_ds-0.4.2/mkdocs.yml
+-rw-r--r--   0     1001      127     3230 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/__init__.py
+-rw-r--r--   0     1001      127     1243 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/_utils.py
+-rw-r--r--   0     1001      127     7324 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/complex.py
+-rw-r--r--   0     1001      127    20305 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/diagnosis.py
+-rw-r--r--   0     1001      127     7188 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/graph.py
+-rw-r--r--   0     1001      127    13270 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/metrics.py
+-rw-r--r--   0     1001      127    49302 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/num.py
+-rw-r--r--   0     1001      127     6080 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/sample.py
+-rw-r--r--   0     1001      127    30893 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/stats.py
+-rw-r--r--   0     1001      127    31957 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/str2.py
+-rw-r--r--   0     1001      127     1133 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/type_alias.py
+-rw-r--r--   0     1001      127       83 2024-04-19 02:51:18.000000 polars_ds-0.4.2/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-19 02:51:18.000000 polars_ds-0.4.2/rust-toolchain.toml
+-rw-r--r--   0     1001      127     2089 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/degree.rs
+-rw-r--r--   0     1001      127     4158 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/eigen_centrality.rs
+-rw-r--r--   0     1001      127     3146 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/mod.rs
+-rw-r--r--   0     1001      127     8711 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/shortest_path.rs
+-rw-r--r--   0     1001      127      430 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/lib.rs
+-rw-r--r--   0     1001      127      967 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/cond_entropy.rs
+-rw-r--r--   0     1001      127     4186 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/convolve.rs
+-rw-r--r--   0     1001      127     7150 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/entrophies.rs
+-rw-r--r--   0     1001      127     2536 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/fft.rs
+-rw-r--r--   0     1001      127     9462 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/float_extras.rs
+-rw-r--r--   0     1001      127     1383 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/gcd_lcm.rs
+-rw-r--r--   0     1001      127     2734 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/haversine.rs
+-rw-r--r--   0     1001      127     8843 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/jaccard.rs
+-rw-r--r--   0     1001      127    18850 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/knn.rs
+-rw-r--r--   0     1001      127      808 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/lempel_ziv.rs
+-rw-r--r--   0     1001      127     3126 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/mod.rs
+-rw-r--r--   0     1001      127     9656 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/ols.rs
+-rw-r--r--   0     1001      127     5714 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/pca.rs
+-rw-r--r--   0     1001      127     3707 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/psi.rs
+-rw-r--r--   0     1001      127     2064 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/target_encode.rs
+-rw-r--r--   0     1001      127     5764 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/tp_fp.rs
+-rw-r--r--   0     1001      127     1422 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/trapz.rs
+-rw-r--r--   0     1001      127     2659 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/woe_iv.rs
+-rw-r--r--   0     1001      127     2251 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/chi2.rs
+-rw-r--r--   0     1001      127     3630 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/fstats.rs
+-rw-r--r--   0     1001      127     2817 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/ks.rs
+-rw-r--r--   0     1001      127     1111 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/mod.rs
+-rw-r--r--   0     1001      127     3383 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/normal_test.rs
+-rw-r--r--   0     1001      127    15502 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/sample.rs
+-rw-r--r--   0     1001      127     6054 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/t_test.rs
+-rw-r--r--   0     1001      127     1594 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/xi_corr.rs
+-rw-r--r--   0     1001      127     4235 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/beta.rs
+-rw-r--r--   0     1001      127     6734 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/gamma.rs
+-rw-r--r--   0     1001      127      895 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/mod.rs
+-rw-r--r--   0     1001      127    18992 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/normal.rs
+-rw-r--r--   0     1001      127     2221 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/consts.rs
+-rw-r--r--   0     1001      127     3082 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/fuzz.rs
+-rw-r--r--   0     1001      127    11287 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/hamming.rs
+-rw-r--r--   0     1001      127     1066 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/inflections.rs
+-rw-r--r--   0     1001      127      483 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/is_stopword.rs
+-rw-r--r--   0     1001      127     5723 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/jaro.rs
+-rw-r--r--   0     1001      127     7937 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/knn_strs.rs
+-rw-r--r--   0     1001      127    13628 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/levenshtein.rs
+-rw-r--r--   0     1001      127     1159 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/mod.rs
+-rw-r--r--   0     1001      127     5731 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/osa.rs
+-rw-r--r--   0     1001      127     3051 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/overlap.rs
+-rw-r--r--   0     1001      127    24197 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/algorithms/english_stemmer.rs
+-rw-r--r--   0     1001      127      110 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/algorithms/mod.rs
+-rw-r--r--   0     1001      127      198 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/among.rs
+-rw-r--r--   0     1001      127     1371 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/mod.rs
+-rw-r--r--   0     1001      127    12885 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/snowball_env.rs
+-rw-r--r--   0     1001      127      870 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball_stem.rs
+-rw-r--r--   0     1001      127     3059 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/sorensen_dice.rs
+-rw-r--r--   0     1001      127     3050 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/str_jaccard.rs
+-rw-r--r--   0     1001      127     3461 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/tversky.rs
+-rw-r--r--   0     1001      127     2447 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/utils/mod.rs
+-rw-r--r--   0     1001      127      121 2024-04-19 02:51:18.000000 polars_ds-0.4.2/tests/requirements-test.txt
+-rw-r--r--   0     1001      127     2685 2024-04-19 02:51:18.000000 polars_ds-0.4.2/tests/test.ipynb
+-rw-r--r--   0     1001      127    39271 2024-04-19 02:51:18.000000 polars_ds-0.4.2/tests/test_correctness.py
+-rw-r--r--   0     1001      127    73361 2024-04-19 02:51:18.000000 polars_ds-0.4.2/Cargo.lock
+-rw-r--r--   0     1001      127     1050 2024-04-19 02:51:18.000000 polars_ds-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9693 1970-01-01 00:00:00.000000 polars_ds-0.4.2/PKG-INFO
```

### Comparing `polars_ds-0.4.1/Cargo.toml` & `polars_ds-0.4.2/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "polars_ds"
-version = "0.4.1"
+version = "0.4.2"
 edition = "2021"
 
 [lib]
 name = "_polars_ds"
 crate-type = ["cdylib"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 pyo3 = {version = "*", features = ["abi3-py38", "extension-module"]}
-pyo3-polars = {version = "0.12", features = ["derive"]}
-polars = {version = "0.38.3", features = ["performant", "lazy", "parquet", "dtype-array", "array_count", "cross_join", "ndarray", "log", "cum_agg", "nightly"]}
+pyo3-polars = {version = "0.13", features = ["derive"]}
+polars = {version = "0.39", features = ["performant", "lazy", "parquet", "dtype-array", "diff", "array_count", "abs", "cross_join", "rank", "ndarray", "log", "cum_agg", "nightly"]}
 num = "0.4.1"
 faer = {version = "0.18.2", features = ["nightly"]}
 faer-ext = {version = "0.1.0", features = ["ndarray"]}
 pulp = {version="0.18.9", features=["nightly"]} # One of Fear's dependency
 serde = {version = "*", features=["derive"]}
 ndarray = {version="0.15.6"}
 hashbrown = {version = "0.14.2", features=["nightly"]}
```

### Comparing `polars_ds-0.4.1/.github/workflows/CI.yml` & `polars_ds-0.4.2/.github/workflows/CI.yml`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         with:
           name: wheel-${{ matrix.package }}-${{ matrix.os }}-${{ matrix.architecture }}
           path: dist/*.whl
 
   release:
     name: Test Release
     runs-on: ubuntu-latest
-    # if: "startsWith(github.ref, 'refs/tags/')"
+    if: "startsWith(github.ref, 'refs/tags/')"
     needs: [build-wheels, create-sdist]
     permissions:
         id-token: write
     steps:
       - uses: actions/download-artifact@v4
         with:
           pattern: wheel-*
```

### Comparing `polars_ds-0.4.1/.gitignore` & `polars_ds-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/CONTRIBUTING.md` & `polars_ds-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/LICENSE.txt` & `polars_ds-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/Makefile` & `polars_ds-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/README.md` & `polars_ds-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/docs/index.md` & `polars_ds-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/examples/basics.ipynb` & `polars_ds-0.4.2/examples/basics.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888941590730141%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'data': {'text/html': {insert: [(7, '<small>shape: (5, "*

 * *            '11)</small><table border="1" '*

 * *            'class="dataframe"><thead><tr><th>f</th><th>time_idx</th><th>dummy</th><th>a</th><th>b</th><th>x1</th><th>x2</th><th>y</th><th>actual</th><th>predicted</th><th>dummy_groups</th></tr><tr><td>f64</td><td>i64</td><td>str</td><td>f64</td><td>f64</td><td>i64</td><td>i64</td><td>i64</td><td>i32</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>0.0</td><td>0</td>< […]*

```diff
@@ -42,28 +42,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 11)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>time_idx</th><th>dummy</th><th>a</th><th>b</th><th>x1</th><th>x2</th><th>y</th><th>actual</th><th>predicted</th><th>dummy_groups</th></tr><tr><td>f64</td><td>i64</td><td>str</td><td>f64</td><td>f64</td><td>i64</td><td>i64</td><td>i64</td><td>i32</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>0.0</td><td>0</td><td>&quot;a&quot;</td><td>0.124983</td><td>0.201402</td><td>0</td><td>10000</td><td>-10000</td><td>1</td><td>0.195702</td><td>&quot;a&quot;</td></tr><tr><td>0.841471</td><td>1</td><td>&quot;a&quot;</td><td>0.894659</td><td>0.702391</td><td>1</td><td>10001</td><td>-9999</td><td>1</td><td>0.017836</td><td>&quot;a&quot;</td></tr><tr><td>0.909297</td><td>2</td><td>&quot;a&quot;</td><td>0.074929</td><td>0.793873</td><td>2</td><td>10002</td><td>-9998</td><td>1</td><td>0.716564</td><td>&quot;a&quot;</td></tr><tr><td>0.14112</td><td>3</td><td>&quot;a&quot;</td><td>0.390507</td><td>0.615867</td><td>3</td><td>10003</td><td>-9997</td><td>0</td><td>0.292772</td><td>&quot;a&quot;</td></tr><tr><td>-0.756802</td><td>4</td><td>&quot;a&quot;</td><td>0.799011</td><td>0.232684</td><td>4</td><td>10004</td><td>-9996</td><td>1</td><td>0.8936</td><td>&quot;a&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 11)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>time_idx</th><th>dummy</th><th>a</th><th>b</th><th>x1</th><th>x2</th><th>y</th><th>actual</th><th>predicted</th><th>dummy_groups</th></tr><tr><td>f64</td><td>i64</td><td>str</td><td>f64</td><td>f64</td><td>i64</td><td>i64</td><td>i64</td><td>i32</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>0.0</td><td>0</td><td>&quot;a&quot;</td><td>0.682803</td><td>0.415153</td><td>0</td><td>10000</td><td>-10000</td><td>1</td><td>0.873578</td><td>&quot;a&quot;</td></tr><tr><td>0.841471</td><td>1</td><td>&quot;a&quot;</td><td>0.687497</td><td>0.591041</td><td>1</td><td>10001</td><td>-9999</td><td>0</td><td>0.816631</td><td>&quot;a&quot;</td></tr><tr><td>0.909297</td><td>2</td><td>&quot;a&quot;</td><td>0.671245</td><td>0.565974</td><td>2</td><td>10002</td><td>-9998</td><td>1</td><td>0.806592</td><td>&quot;a&quot;</td></tr><tr><td>0.14112</td><td>3</td><td>&quot;a&quot;</td><td>0.446571</td><td>0.501598</td><td>3</td><td>10003</td><td>-9997</td><td>1</td><td>0.848589</td><td>&quot;a&quot;</td></tr><tr><td>-0.756802</td><td>4</td><td>&quot;a&quot;</td><td>0.836808</td><td>0.782067</td><td>4</td><td>10004</td><td>-9996</td><td>0</td><td>0.746404</td><td>&quot;a&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 11)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 f         \u2506 time_idx \u2506 dummy \u2506 a        \u2506 \u2026 \u2506 y      \u2506 actual \u2506 predicted \u2506 dummy_groups \u2502\n",
                             "\u2502 ---       \u2506 ---      \u2506 ---   \u2506 ---      \u2506   \u2506 ---    \u2506 ---    \u2506 ---       \u2506 ---          \u2502\n",
                             "\u2502 f64       \u2506 i64      \u2506 str   \u2506 f64      \u2506   \u2506 i64    \u2506 i32    \u2506 f64       \u2506 str          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0.0       \u2506 0        \u2506 a     \u2506 0.124983 \u2506 \u2026 \u2506 -10000 \u2506 1      \u2506 0.195702  \u2506 a            \u2502\n",
-                            "\u2502 0.841471  \u2506 1        \u2506 a     \u2506 0.894659 \u2506 \u2026 \u2506 -9999  \u2506 1      \u2506 0.017836  \u2506 a            \u2502\n",
-                            "\u2502 0.909297  \u2506 2        \u2506 a     \u2506 0.074929 \u2506 \u2026 \u2506 -9998  \u2506 1      \u2506 0.716564  \u2506 a            \u2502\n",
-                            "\u2502 0.14112   \u2506 3        \u2506 a     \u2506 0.390507 \u2506 \u2026 \u2506 -9997  \u2506 0      \u2506 0.292772  \u2506 a            \u2502\n",
-                            "\u2502 -0.756802 \u2506 4        \u2506 a     \u2506 0.799011 \u2506 \u2026 \u2506 -9996  \u2506 1      \u2506 0.8936    \u2506 a            \u2502\n",
+                            "\u2502 0.0       \u2506 0        \u2506 a     \u2506 0.682803 \u2506 \u2026 \u2506 -10000 \u2506 1      \u2506 0.873578  \u2506 a            \u2502\n",
+                            "\u2502 0.841471  \u2506 1        \u2506 a     \u2506 0.687497 \u2506 \u2026 \u2506 -9999  \u2506 0      \u2506 0.816631  \u2506 a            \u2502\n",
+                            "\u2502 0.909297  \u2506 2        \u2506 a     \u2506 0.671245 \u2506 \u2026 \u2506 -9998  \u2506 1      \u2506 0.806592  \u2506 a            \u2502\n",
+                            "\u2502 0.14112   \u2506 3        \u2506 a     \u2506 0.446571 \u2506 \u2026 \u2506 -9997  \u2506 1      \u2506 0.848589  \u2506 a            \u2502\n",
+                            "\u2502 -0.756802 \u2506 4        \u2506 a     \u2506 0.836808 \u2506 \u2026 \u2506 -9996  \u2506 0      \u2506 0.746404  \u2506 a            \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -210,28 +210,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>a</th><th>b</th></tr><tr><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1.3944e-15</td><td>-0.124983</td><td>-0.201402</td></tr><tr><td>-0.841471</td><td>-0.894659</td><td>-0.702391</td></tr><tr><td>-0.909297</td><td>-0.074929</td><td>-0.793873</td></tr><tr><td>-0.14112</td><td>-0.390507</td><td>-0.615867</td></tr><tr><td>0.756802</td><td>-0.674028</td><td>-0.031282</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>a</th><th>b</th></tr><tr><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1.3944e-15</td><td>-0.682803</td><td>-0.415153</td></tr><tr><td>-0.841471</td><td>-0.687497</td><td>-0.591041</td></tr><tr><td>-0.909297</td><td>-0.671245</td><td>-0.565974</td></tr><tr><td>-0.14112</td><td>-0.446571</td><td>-0.501598</td></tr><tr><td>0.756802</td><td>-0.154005</td><td>-0.366915</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 f          \u2506 a         \u2506 b         \u2502\n",
                             "\u2502 ---        \u2506 ---       \u2506 ---       \u2502\n",
                             "\u2502 f64        \u2506 f64       \u2506 f64       \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1.3944e-15 \u2506 -0.124983 \u2506 -0.201402 \u2502\n",
-                            "\u2502 -0.841471  \u2506 -0.894659 \u2506 -0.702391 \u2502\n",
-                            "\u2502 -0.909297  \u2506 -0.074929 \u2506 -0.793873 \u2502\n",
-                            "\u2502 -0.14112   \u2506 -0.390507 \u2506 -0.615867 \u2502\n",
-                            "\u2502 0.756802   \u2506 -0.674028 \u2506 -0.031282 \u2502\n",
+                            "\u2502 1.3944e-15 \u2506 -0.682803 \u2506 -0.415153 \u2502\n",
+                            "\u2502 -0.841471  \u2506 -0.687497 \u2506 -0.591041 \u2502\n",
+                            "\u2502 -0.909297  \u2506 -0.671245 \u2506 -0.565974 \u2502\n",
+                            "\u2502 -0.14112   \u2506 -0.446571 \u2506 -0.501598 \u2502\n",
+                            "\u2502 0.756802   \u2506 -0.154005 \u2506 -0.366915 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -495,25 +495,25 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>dummy</th><th>coeffs</th></tr><tr><td>str</td><td>list[f64]</td></tr></thead><tbody><tr><td>&quot;a&quot;</td><td>[2.0, -1.0]</td></tr><tr><td>&quot;b&quot;</td><td>[2.0, -1.0]</td></tr></tbody></table></div>"
+                            "<small>shape: (2, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>dummy</th><th>coeffs</th></tr><tr><td>str</td><td>list[f64]</td></tr></thead><tbody><tr><td>&quot;b&quot;</td><td>[2.0, -1.0]</td></tr><tr><td>&quot;a&quot;</td><td>[2.0, -1.0]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 dummy \u2506 coeffs      \u2502\n",
                             "\u2502 ---   \u2506 ---         \u2502\n",
                             "\u2502 str   \u2506 list[f64]   \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 a     \u2506 [2.0, -1.0] \u2502\n",
                             "\u2502 b     \u2506 [2.0, -1.0] \u2502\n",
+                            "\u2502 a     \u2506 [2.0, -1.0] \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -623,53 +623,136 @@
                 "# Conditional Entropy, should be 0 because x1 is an ID\n",
                 "df.select(\n",
                 "    pds.query_cond_entropy(\"y\", \"x1\")\n",
                 ")"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "81def1cf",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (1, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>list[f64]</td></tr></thead><tbody><tr><td>[288675.133152, 28.94286, 28.709543]</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (1, 1)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a                                 \u2502\n",
+                            "\u2502 ---                               \u2502\n",
+                            "\u2502 list[f64]                         \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 [288675.133152, 28.94286, 28.709\u2026 \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 15,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Only want singular values (principal values?)\n",
+                "df.select(\n",
+                "    pds.query_singular_values(\"a\", \"b\", \"x1\")\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "id": "cc497383",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (2, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>singular_value</th><th>principal_vectors</th></tr><tr><td>f64</td><td>list[f64]</td></tr></thead><tbody><tr><td>28.945769</td><td>[0.698117, 0.715984]</td></tr><tr><td>28.710273</td><td>[0.715984, -0.698117]</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (2, 2)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 singular_value \u2506 principal_vectors     \u2502\n",
+                            "\u2502 ---            \u2506 ---                   \u2502\n",
+                            "\u2502 f64            \u2506 list[f64]             \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 28.945769      \u2506 [0.698117, 0.715984]  \u2502\n",
+                            "\u2502 28.710273      \u2506 [0.715984, -0.698117] \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 16,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Singular values + The principal components\n",
+                "df.select(\n",
+                "    pds.query_pca(\"a\", \"b\")\n",
+                ").unnest(\"a\")"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "1b2e036f",
             "metadata": {},
             "source": [
                 "# ML Metrics"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 17,
             "id": "85d0d094-3c4c-4230-a589-1027c5690162",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>dummy_groups</th><th>l2</th><th>log loss</th><th>precision</th><th>recall</th><th>f</th><th>average_precision</th><th>roc_auc</th></tr><tr><td>str</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>&quot;b&quot;</td><td>0.328426</td><td>0.989413</td><td>0.497244</td><td>0.515721</td><td>0.253157</td><td>0.500238</td><td>0.510534</td></tr><tr><td>&quot;a&quot;</td><td>0.338122</td><td>1.019</td><td>0.493995</td><td>0.496579</td><td>0.247642</td><td>0.493921</td><td>0.492103</td></tr></tbody></table></div>"
+                            "<small>shape: (2, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>dummy_groups</th><th>l2</th><th>log loss</th><th>precision</th><th>recall</th><th>f</th><th>average_precision</th><th>roc_auc</th></tr><tr><td>str</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>&quot;b&quot;</td><td>0.329581</td><td>0.985112</td><td>0.499601</td><td>0.5012</td><td>0.2502</td><td>0.502613</td><td>0.502348</td></tr><tr><td>&quot;a&quot;</td><td>0.33594</td><td>1.003373</td><td>0.48839</td><td>0.503244</td><td>0.247853</td><td>0.490244</td><td>0.494221</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2, 8)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 dummy_groups \u2506 l2       \u2506 log loss \u2506 precision \u2506 recall   \u2506 f        \u2506 average_precis \u2506 roc_auc  \u2502\n",
                             "\u2502 ---          \u2506 ---      \u2506 ---      \u2506 ---       \u2506 ---      \u2506 ---      \u2506 ion            \u2506 ---      \u2502\n",
                             "\u2502 str          \u2506 f64      \u2506 f64      \u2506 f64       \u2506 f64      \u2506 f64      \u2506 ---            \u2506 f64      \u2502\n",
                             "\u2502              \u2506          \u2506          \u2506           \u2506          \u2506          \u2506 f64            \u2506          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 b            \u2506 0.328426 \u2506 0.989413 \u2506 0.497244  \u2506 0.515721 \u2506 0.253157 \u2506 0.500238       \u2506 0.510534 \u2502\n",
-                            "\u2502 a            \u2506 0.338122 \u2506 1.019    \u2506 0.493995  \u2506 0.496579 \u2506 0.247642 \u2506 0.493921       \u2506 0.492103 \u2502\n",
+                            "\u2502 b            \u2506 0.329581 \u2506 0.985112 \u2506 0.499601  \u2506 0.5012   \u2506 0.2502   \u2506 0.502613       \u2506 0.502348 \u2502\n",
+                            "\u2502 a            \u2506 0.33594  \u2506 1.003373 \u2506 0.48839   \u2506 0.503244 \u2506 0.247853 \u2506 0.490244       \u2506 0.494221 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.group_by(\"dummy_groups\").agg(\n",
                 "    pds.query_l2(\"actual\", \"predicted\").alias(\"l2\"),\n",
@@ -684,15 +767,15 @@
             "metadata": {},
             "source": [
                 "# Str Extension"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 18,
             "id": "54ad36f9-264e-4a49-bf36-936639440edf",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -715,15 +798,15 @@
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 word  \u2502\n",
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 words \u2502\n",
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 word  \u2502\n",
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 words \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "size = 100_000\n",
                 "df2 = pl.DataFrame({\n",
@@ -731,104 +814,104 @@
                 "    \"word\":[\"words\", \"word\"] * (size //2)\n",
                 "})\n",
                 "df2.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 19,
             "id": "ee123a7e-7f9b-4f48-a5d5-6354799201ab",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;world&quot;</td></tr><tr><td>&quot;going&quot;</td></tr><tr><td>&quot;to&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;world&quot;</td></tr><tr><td>&quot;to&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr><tr><td>&quot;going&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 1)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 sen    \u2502\n",
                             "\u2502 ---    \u2502\n",
                             "\u2502 str    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 world  \u2502\n",
-                            "\u2502 going  \u2502\n",
                             "\u2502 to     \u2502\n",
                             "\u2502 church \u2502\n",
                             "\u2502 hello  \u2502\n",
+                            "\u2502 going  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Tokenize\n",
                 "df2.select(\n",
                 "    pds.str_tokenize(pl.col(\"sen\").str.to_lowercase()).explode().unique()\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 20,
             "id": "f33017e3-17df-498b-93d9-1d656a344388",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr><tr><td>&quot;go&quot;</td></tr><tr><td>&quot;world&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;go&quot;</td></tr><tr><td>&quot;world&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 1)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 sen    \u2502\n",
                             "\u2502 ---    \u2502\n",
                             "\u2502 str    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 church \u2502\n",
                             "\u2502        \u2502\n",
                             "\u2502 hello  \u2502\n",
+                            "\u2502 church \u2502\n",
                             "\u2502 go     \u2502\n",
                             "\u2502 world  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df2.select(\n",
                 "    pds.str_tokenize(pl.col(\"sen\").str.to_lowercase(), stem=True).explode().unique()\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 21,
             "id": "69237c02-5f9f-4e92-b68d-6ac43aad1a79",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -851,28 +934,28 @@
                             "\u2502 1    \u2502\n",
                             "\u2502 2    \u2502\n",
                             "\u2502 1    \u2502\n",
                             "\u2502 2    \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df2.select(\n",
                 "    pds.str_leven(\"word\", \"world\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 22,
             "id": "2eba320c",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -895,29 +978,29 @@
                             "\u2502 1    \u2502\n",
                             "\u2502 2    \u2502\n",
                             "\u2502 1    \u2502\n",
                             "\u2502 2    \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Damerau-Levenshtein\n",
                 "df2.select(\n",
                 "    pds.str_d_leven(\"word\", \"world\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 23,
             "id": "795396dc",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -940,28 +1023,28 @@
                             "\u2502 0.8  \u2502\n",
                             "\u2502 0.6  \u2502\n",
                             "\u2502 0.8  \u2502\n",
                             "\u2502 0.6  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df2.select( # column \"word\" vs. the word \"world\"\n",
                 "    pds.str_leven(\"word\", \"world\", return_sim = True)\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 24,
             "id": "2dad7633-67fa-47f3-b86a-9f4cd097a650",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -984,43 +1067,43 @@
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 word \u2502\n",
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 word \u2502\n",
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 word \u2502\n",
                             "\u2502 Hello, world! I'm going to churc\u2026 \u2506 word \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df2.filter(\n",
                 "    # This is way faster than computing ditance and then doing a filter\n",
                 "    pds.filter_by_levenshtein(pl.col(\"word\"), \"world\", 1) # <= 1. \n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 25,
             "id": "dc9477c1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = pl.DataFrame({\n",
                 "    \"word\":[\"apple\", \"banana\", \"pineapple\", \"asasasas\", \"sasasass\"],\n",
                 "    \"other_data\": [1,2,3,4,5]\n",
                 "})\n",
                 "gibberish = [\"asasasa\", \"sasaaasss\", \"asdasadadfa\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 26,
             "id": "c50591e0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -1040,15 +1123,15 @@
                             "\u2502 str      \u2506 i64        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 asasasas \u2506 4          \u2502\n",
                             "\u2502 sasasass \u2506 5          \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.filter(\n",
                 "    pds.similar_to_vocab(\n",
@@ -1059,15 +1142,15 @@
                 "        strategy = \"any\" # True if the word is similar to any word in vocab. Other options: \"all\", \"avg\"\n",
                 "    )\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 27,
             "id": "7ece3794",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -1091,15 +1174,15 @@
                             "\u2502 0.428571 \u2506 0.333333  \u2506 0.272727    \u2506 0.166667       \u2506 0.0                       \u2506 0.444444       \u2502\n",
                             "\u2502 0.111111 \u2506 0.111111  \u2506 0.090909    \u2506 0.555556       \u2506 0.444444                  \u2506 0.5            \u2502\n",
                             "\u2502 0.875    \u2506 0.666667  \u2506 0.545455    \u2506 0.25           \u2506 0.25                      \u2506 0.527778       \u2502\n",
                             "\u2502 0.75     \u2506 0.777778  \u2506 0.454545    \u2506 0.25           \u2506 0.25                      \u2506 0.527778       \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.select(\n",
                 "    pds.str_leven(\"word\", \"asasasa\", return_sim=True).alias(\"asasasa\"),\n",
@@ -1117,46 +1200,46 @@
             "metadata": {},
             "source": [
                 "# Stats Extension"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 28,
             "id": "2c6171b0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>f64</td></tr></thead><tbody><tr><td>null</td></tr><tr><td>null</td></tr><tr><td>0.117766</td></tr><tr><td>0.125886</td></tr><tr><td>0.615244</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>f64</td></tr></thead><tbody><tr><td>null</td></tr><tr><td>null</td></tr><tr><td>0.066091</td></tr><tr><td>-0.35634</td></tr><tr><td>1.17341</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 1)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 a        \u2502\n",
                             "\u2502 ---      \u2502\n",
                             "\u2502 f64      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 null     \u2502\n",
                             "\u2502 null     \u2502\n",
-                            "\u2502 0.117766 \u2502\n",
-                            "\u2502 0.125886 \u2502\n",
-                            "\u2502 0.615244 \u2502\n",
+                            "\u2502 0.066091 \u2502\n",
+                            "\u2502 -0.35634 \u2502\n",
+                            "\u2502 1.17341  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "\n",
@@ -1164,181 +1247,181 @@
                 "    \"a\": [None, None] + list(np.random.normal(size = 998))\n",
                 "})\n",
                 "df.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 29,
             "id": "2f6e7445",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random</th></tr><tr><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.117766</td><td>0.562741</td></tr><tr><td>0.125886</td><td>-1.003873</td></tr><tr><td>0.615244</td><td>-0.354483</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random</th></tr><tr><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.066091</td><td>1.838582</td></tr><tr><td>-0.35634</td><td>1.149611</td></tr><tr><td>1.17341</td><td>0.960881</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2506 random    \u2502\n",
-                            "\u2502 ---      \u2506 ---       \u2502\n",
-                            "\u2502 f64      \u2506 f64       \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 null      \u2502\n",
-                            "\u2502 null     \u2506 null      \u2502\n",
-                            "\u2502 0.117766 \u2506 0.562741  \u2502\n",
-                            "\u2502 0.125886 \u2506 -1.003873 \u2502\n",
-                            "\u2502 0.615244 \u2506 -0.354483 \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a        \u2506 random   \u2502\n",
+                            "\u2502 ---      \u2506 ---      \u2502\n",
+                            "\u2502 f64      \u2506 f64      \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null     \u2506 null     \u2502\n",
+                            "\u2502 null     \u2506 null     \u2502\n",
+                            "\u2502 0.066091 \u2506 1.838582 \u2502\n",
+                            "\u2502 -0.35634 \u2506 1.149611 \u2502\n",
+                            "\u2502 1.17341  \u2506 0.960881 \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Genenrate random numbers, respecting null positions in reference column (pl.col(\"a\"))\n",
                 "df.with_columns(\n",
                 "    pl.col(\"a\").stats.rand_normal(mean = 0.5, std = 1., respect_null=True).alias(\"random\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 30,
             "id": "11e13f55",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.117766</td><td>&quot;jbUU&quot;</td></tr><tr><td>0.125886</td><td>&quot;e&quot;</td></tr><tr><td>0.615244</td><td>&quot;p6&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.066091</td><td>&quot;DIu2G&quot;</td></tr><tr><td>-0.35634</td><td>&quot;9eNwx&quot;</td></tr><tr><td>1.17341</td><td>&quot;W&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 a        \u2506 random_str \u2502\n",
                             "\u2502 ---      \u2506 ---        \u2502\n",
                             "\u2502 f64      \u2506 str        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 null     \u2506 null       \u2502\n",
                             "\u2502 null     \u2506 null       \u2502\n",
-                            "\u2502 0.117766 \u2506 jbUU       \u2502\n",
-                            "\u2502 0.125886 \u2506 e          \u2502\n",
-                            "\u2502 0.615244 \u2506 p6         \u2502\n",
+                            "\u2502 0.066091 \u2506 DIu2G      \u2502\n",
+                            "\u2502 -0.35634 \u2506 9eNwx      \u2502\n",
+                            "\u2502 1.17341  \u2506 W          \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Genenrate random string\n",
                 "df.with_columns(\n",
                 "    pl.col(\"a\").stats.rand_str(min_size = 1, max_size = 5, respect_null=True).alias(\"random_str\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 31,
             "id": "43c37394",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.117766</td><td>&quot;qu7bb&quot;</td></tr><tr><td>0.125886</td><td>&quot;UnNuQ&quot;</td></tr><tr><td>0.615244</td><td>&quot;KePfw&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.066091</td><td>&quot;kLzzH&quot;</td></tr><tr><td>-0.35634</td><td>&quot;Kjqg2&quot;</td></tr><tr><td>1.17341</td><td>&quot;dtleS&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 a        \u2506 random_str \u2502\n",
                             "\u2502 ---      \u2506 ---        \u2502\n",
                             "\u2502 f64      \u2506 str        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 null     \u2506 null       \u2502\n",
                             "\u2502 null     \u2506 null       \u2502\n",
-                            "\u2502 0.117766 \u2506 qu7bb      \u2502\n",
-                            "\u2502 0.125886 \u2506 UnNuQ      \u2502\n",
-                            "\u2502 0.615244 \u2506 KePfw      \u2502\n",
+                            "\u2502 0.066091 \u2506 kLzzH      \u2502\n",
+                            "\u2502 -0.35634 \u2506 Kjqg2      \u2502\n",
+                            "\u2502 1.17341  \u2506 dtleS      \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Genenrate fixed size random string, while respecting column a's nulls\n",
                 "df.with_columns(\n",
                 "    pl.col(\"a\").stats.rand_str(min_size = 5, max_size = 5, respect_null=True).alias(\"random_str\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 32,
             "id": "3d0c06a4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>test1</th><th>test2</th><th>test1_perturbed</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>0.034606</td><td>null</td><td>0.034845</td></tr><tr><td>null</td><td>-0.127219</td><td>null</td><td>-0.127212</td></tr><tr><td>0.117766</td><td>-0.89684</td><td>1.772437</td><td>-0.896623</td></tr><tr><td>0.125886</td><td>-0.785084</td><td>1.003134</td><td>-0.785312</td></tr><tr><td>0.615244</td><td>1.312247</td><td>2.792097</td><td>1.312396</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>test1</th><th>test2</th><th>test1_perturbed</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>-0.352337</td><td>null</td><td>-0.352074</td></tr><tr><td>null</td><td>-0.987273</td><td>null</td><td>-0.986941</td></tr><tr><td>0.066091</td><td>-1.252643</td><td>1.691665</td><td>-1.25276</td></tr><tr><td>-0.35634</td><td>-0.180388</td><td>1.093283</td><td>-0.180884</td></tr><tr><td>1.17341</td><td>-0.649039</td><td>0.139838</td><td>-0.648904</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 4)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 a        \u2506 test1     \u2506 test2    \u2506 test1_perturbed \u2502\n",
                             "\u2502 ---      \u2506 ---       \u2506 ---      \u2506 ---             \u2502\n",
                             "\u2502 f64      \u2506 f64       \u2506 f64      \u2506 f64             \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 0.034606  \u2506 null     \u2506 0.034845        \u2502\n",
-                            "\u2502 null     \u2506 -0.127219 \u2506 null     \u2506 -0.127212       \u2502\n",
-                            "\u2502 0.117766 \u2506 -0.89684  \u2506 1.772437 \u2506 -0.896623       \u2502\n",
-                            "\u2502 0.125886 \u2506 -0.785084 \u2506 1.003134 \u2506 -0.785312       \u2502\n",
-                            "\u2502 0.615244 \u2506 1.312247  \u2506 2.792097 \u2506 1.312396        \u2502\n",
+                            "\u2502 null     \u2506 -0.352337 \u2506 null     \u2506 -0.352074       \u2502\n",
+                            "\u2502 null     \u2506 -0.987273 \u2506 null     \u2506 -0.986941       \u2502\n",
+                            "\u2502 0.066091 \u2506 -1.252643 \u2506 1.691665 \u2506 -1.25276        \u2502\n",
+                            "\u2502 -0.35634 \u2506 -0.180388 \u2506 1.093283 \u2506 -0.180884       \u2502\n",
+                            "\u2502 1.17341  \u2506 -0.649039 \u2506 0.139838 \u2506 -0.648904       \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 30,
+                    "execution_count": 32,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.with_columns(\n",
                 "    # Sample from a normal distribution, using reference column \"a\" 's mean and std\n",
@@ -1349,46 +1432,46 @@
                 "    # Add a random pertubation to test1\n",
                 "    pds.perturb(\"test1\", epsilon=0.001).alias(\"test1_perturbed\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 33,
             "id": "67dc6583",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>[0, 1)</th><th>Normal</th><th>Int from [0, 10)</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>i32</td></tr></thead><tbody><tr><td>null</td><td>0.362846</td><td>0.131183</td><td>8</td></tr><tr><td>null</td><td>0.094497</td><td>-0.024039</td><td>8</td></tr><tr><td>0.117766</td><td>0.730207</td><td>0.27907</td><td>5</td></tr><tr><td>0.125886</td><td>0.242051</td><td>-0.229687</td><td>7</td></tr><tr><td>0.615244</td><td>0.166926</td><td>0.430802</td><td>5</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>[0, 1)</th><th>Normal</th><th>Int from [0, 10)</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>i32</td></tr></thead><tbody><tr><td>null</td><td>0.205474</td><td>-1.056756</td><td>5</td></tr><tr><td>null</td><td>0.015194</td><td>0.056542</td><td>4</td></tr><tr><td>0.066091</td><td>0.659457</td><td>-0.101667</td><td>8</td></tr><tr><td>-0.35634</td><td>0.639568</td><td>-2.193398</td><td>7</td></tr><tr><td>1.17341</td><td>0.315957</td><td>-0.790355</td><td>5</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 4)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 a        \u2506 [0, 1)   \u2506 Normal    \u2506 Int from [0, 10) \u2502\n",
                             "\u2502 ---      \u2506 ---      \u2506 ---       \u2506 ---              \u2502\n",
                             "\u2502 f64      \u2506 f64      \u2506 f64       \u2506 i32              \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 0.362846 \u2506 0.131183  \u2506 8                \u2502\n",
-                            "\u2502 null     \u2506 0.094497 \u2506 -0.024039 \u2506 8                \u2502\n",
-                            "\u2502 0.117766 \u2506 0.730207 \u2506 0.27907   \u2506 5                \u2502\n",
-                            "\u2502 0.125886 \u2506 0.242051 \u2506 -0.229687 \u2506 7                \u2502\n",
-                            "\u2502 0.615244 \u2506 0.166926 \u2506 0.430802  \u2506 5                \u2502\n",
+                            "\u2502 null     \u2506 0.205474 \u2506 -1.056756 \u2506 5                \u2502\n",
+                            "\u2502 null     \u2506 0.015194 \u2506 0.056542  \u2506 4                \u2502\n",
+                            "\u2502 0.066091 \u2506 0.659457 \u2506 -0.101667 \u2506 8                \u2502\n",
+                            "\u2502 -0.35634 \u2506 0.639568 \u2506 -2.193398 \u2506 7                \u2502\n",
+                            "\u2502 1.17341  \u2506 0.315957 \u2506 -0.790355 \u2506 5                \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 33,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# New in v0.3.5\n",
                 "# This way, we don't have a reference column, so we cannot respect nulls, but is more convenient to use.\n",
@@ -1397,42 +1480,42 @@
                 "    pds.random_normal(pl.col(\"a\").mean(), pl.col(\"a\").std()).alias(\"Normal\"),\n",
                 "    pds.random_int(0, 10).alias(\"Int from [0, 10)\"),\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 34,
             "id": "7b63f636",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-tests: statistics</th><th>t-tests: pvalue</th><th>normality_test: statistics</th><th>normality_test: pvalue</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>-0.841039</td><td>0.400467</td><td>0.09456</td><td>0.95382</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-tests: statistics</th><th>t-tests: pvalue</th><th>normality_test: statistics</th><th>normality_test: pvalue</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>-0.261893</td><td>0.793441</td><td>1.747484</td><td>0.417387</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 4)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 t-tests: statistics \u2506 t-tests: pvalue \u2506 normality_test: statistics \u2506 normality_test: pvalue \u2502\n",
                             "\u2502 ---                 \u2506 ---             \u2506 ---                        \u2506 ---                    \u2502\n",
                             "\u2502 f64                 \u2506 f64             \u2506 f64                        \u2506 f64                    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 -0.841039           \u2506 0.400467        \u2506 0.09456                    \u2506 0.95382                \u2502\n",
+                            "\u2502 -0.261893           \u2506 0.793441        \u2506 1.747484                   \u2506 0.417387               \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 34,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Genenrate 2 random sample, both normally distributed\n",
                 "# Run Welch's t test on them, p value should be big since they have equal mean\n",
@@ -1450,46 +1533,46 @@
                 "    , pl.col(\"normality_test\").struct.field(\"statistic\").alias(\"normality_test: statistics\")\n",
                 "    , pl.col(\"normality_test\").struct.field(\"pvalue\").alias(\"normality_test: pvalue\")\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 35,
             "id": "b46a72a5",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 5)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>var1</th><th>var2</th><th>category_1</th><th>category_2</th></tr><tr><td>i64</td><td>f64</td><td>f64</td><td>i32</td><td>i32</td></tr></thead><tbody><tr><td>0</td><td>0.665027</td><td>0.048813</td><td>2</td><td>3</td></tr><tr><td>1</td><td>0.259249</td><td>0.646963</td><td>2</td><td>3</td></tr><tr><td>2</td><td>0.689757</td><td>0.38092</td><td>2</td><td>1</td></tr><tr><td>0</td><td>0.238486</td><td>0.188781</td><td>1</td><td>3</td></tr><tr><td>1</td><td>0.717848</td><td>0.149475</td><td>1</td><td>3</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 5)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>var1</th><th>var2</th><th>category_1</th><th>category_2</th></tr><tr><td>i64</td><td>f64</td><td>f64</td><td>i32</td><td>i32</td></tr></thead><tbody><tr><td>0</td><td>0.498654</td><td>0.281769</td><td>3</td><td>5</td></tr><tr><td>1</td><td>0.242465</td><td>0.652056</td><td>3</td><td>4</td></tr><tr><td>2</td><td>0.538076</td><td>0.841711</td><td>1</td><td>9</td></tr><tr><td>0</td><td>0.79132</td><td>0.491</td><td>0</td><td>3</td></tr><tr><td>1</td><td>0.827066</td><td>0.551273</td><td>4</td><td>8</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 5)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 market_id \u2506 var1     \u2506 var2     \u2506 category_1 \u2506 category_2 \u2502\n",
                             "\u2502 ---       \u2506 ---      \u2506 ---      \u2506 ---        \u2506 ---        \u2502\n",
                             "\u2502 i64       \u2506 f64      \u2506 f64      \u2506 i32        \u2506 i32        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0         \u2506 0.665027 \u2506 0.048813 \u2506 2          \u2506 3          \u2502\n",
-                            "\u2502 1         \u2506 0.259249 \u2506 0.646963 \u2506 2          \u2506 3          \u2502\n",
-                            "\u2502 2         \u2506 0.689757 \u2506 0.38092  \u2506 2          \u2506 1          \u2502\n",
-                            "\u2502 0         \u2506 0.238486 \u2506 0.188781 \u2506 1          \u2506 3          \u2502\n",
-                            "\u2502 1         \u2506 0.717848 \u2506 0.149475 \u2506 1          \u2506 3          \u2502\n",
+                            "\u2502 0         \u2506 0.498654 \u2506 0.281769 \u2506 3          \u2506 5          \u2502\n",
+                            "\u2502 1         \u2506 0.242465 \u2506 0.652056 \u2506 3          \u2506 4          \u2502\n",
+                            "\u2502 2         \u2506 0.538076 \u2506 0.841711 \u2506 1          \u2506 9          \u2502\n",
+                            "\u2502 0         \u2506 0.79132  \u2506 0.491    \u2506 0          \u2506 3          \u2502\n",
+                            "\u2502 1         \u2506 0.827066 \u2506 0.551273 \u2506 4          \u2506 8          \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 33,
+                    "execution_count": 35,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "size = 5_000\n",
                 "df = pl.DataFrame({\n",
@@ -1503,42 +1586,42 @@
                 ")\n",
                 "\n",
                 "df.head(5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 36,
             "id": "adc4f66f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>{-0.373137,0.709055}</td><td>{31.422266,0.686052}</td><td>{1.055805,0.376758}</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>{-2.204845,0.027488}</td><td>{28.786602,0.798015}</td><td>{1.520127,0.193397}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 t-test               \u2506 chi2-test            \u2506 f-test              \u2502\n",
                             "\u2502 ---                  \u2506 ---                  \u2506 ---                 \u2502\n",
                             "\u2502 struct[2]            \u2506 struct[2]            \u2506 struct[2]           \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 {-0.373137,0.709055} \u2506 {31.422266,0.686052} \u2506 {1.055805,0.376758} \u2502\n",
+                            "\u2502 {-2.204845,0.027488} \u2506 {28.786602,0.798015} \u2506 {1.520127,0.193397} \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 34,
+                    "execution_count": 36,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# In dataframe statistical tests!\n",
                 "df.select(\n",
@@ -1546,44 +1629,44 @@
                 "    pds.query_chi2(\"category_1\", \"category_2\").alias(\"chi2-test\"),\n",
                 "    pds.query_f_test(\"var1\", group = \"category_1\").alias(\"f-test\")\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 37,
             "id": "65dbb6bd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (3, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>i64</td><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>0</td><td>{1.00574,0.314614}</td><td>{25.167451,0.911882}</td><td>{0.550084,0.698992}</td></tr><tr><td>1</td><td>{0.252718,0.800502}</td><td>{40.441577,0.280539}</td><td>{1.480297,0.205647}</td></tr><tr><td>2</td><td>{-1.922205,0.054665}</td><td>{36.131151,0.462521}</td><td>{0.680857,0.605225}</td></tr></tbody></table></div>"
+                            "<small>shape: (3, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>i64</td><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>0</td><td>{-1.118248,0.263541}</td><td>{38.128166,0.372848}</td><td>{0.758698,0.552177}</td></tr><tr><td>1</td><td>{-1.29356,0.195907}</td><td>{31.584237,0.678621}</td><td>{0.67456,0.609622}</td></tr><tr><td>2</td><td>{-1.405805,0.159875}</td><td>{36.244973,0.457224}</td><td>{2.309402,0.055886}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (3, 4)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 market_id \u2506 t-test               \u2506 chi2-test            \u2506 f-test              \u2502\n",
                             "\u2502 ---       \u2506 ---                  \u2506 ---                  \u2506 ---                 \u2502\n",
                             "\u2502 i64       \u2506 struct[2]            \u2506 struct[2]            \u2506 struct[2]           \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0         \u2506 {1.00574,0.314614}   \u2506 {25.167451,0.911882} \u2506 {0.550084,0.698992} \u2502\n",
-                            "\u2502 1         \u2506 {0.252718,0.800502}  \u2506 {40.441577,0.280539} \u2506 {1.480297,0.205647} \u2502\n",
-                            "\u2502 2         \u2506 {-1.922205,0.054665} \u2506 {36.131151,0.462521} \u2506 {0.680857,0.605225} \u2502\n",
+                            "\u2502 0         \u2506 {-1.118248,0.263541} \u2506 {38.128166,0.372848} \u2506 {0.758698,0.552177} \u2502\n",
+                            "\u2502 1         \u2506 {-1.29356,0.195907}  \u2506 {31.584237,0.678621} \u2506 {0.67456,0.609622}  \u2502\n",
+                            "\u2502 2         \u2506 {-1.405805,0.159875} \u2506 {36.244973,0.457224} \u2506 {2.309402,0.055886} \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 35,
+                    "execution_count": 37,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Can also be done in group by context\n",
                 "df.group_by(\"market_id\").agg(\n",
@@ -1601,15 +1684,15 @@
                 "# Nearest Neighbors Related Tasks\n",
                 "\n",
                 "These queries can be very slow when data/dimension gets huge, even when processed in parallel."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 38,
             "id": "87aff1ef",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import polars_ds as pds\n",
                 "size = 2000\n",
                 "df = pl.DataFrame({\n",
@@ -1622,46 +1705,46 @@
                 "    (pds.random() * 10).alias(\"rh\"),\n",
                 "    pl.col(\"id\").cast(pl.UInt32)\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 39,
             "id": "2fae4b5e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l_inf_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.344033</td><td>0.329014</td><td>0.58807</td><td>0.620571</td><td>9.086603</td><td>15</td></tr><tr><td>1</td><td>0.478353</td><td>0.639429</td><td>0.112137</td><td>0.889891</td><td>6.60086</td><td>18</td></tr><tr><td>2</td><td>0.597618</td><td>0.064757</td><td>0.989752</td><td>0.873602</td><td>4.603702</td><td>7</td></tr><tr><td>3</td><td>0.69054</td><td>0.128104</td><td>0.67956</td><td>0.417295</td><td>7.269824</td><td>22</td></tr><tr><td>4</td><td>0.970639</td><td>0.49373</td><td>0.811869</td><td>0.345611</td><td>1.671346</td><td>10</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l_inf_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>9</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>11</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>13</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>27</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>14</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 7)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 nb_l_inf_cnt \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---          \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 u32          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.344033 \u2506 0.329014 \u2506 0.58807  \u2506 0.620571 \u2506 9.086603 \u2506 15           \u2502\n",
-                            "\u2502 1   \u2506 0.478353 \u2506 0.639429 \u2506 0.112137 \u2506 0.889891 \u2506 6.60086  \u2506 18           \u2502\n",
-                            "\u2502 2   \u2506 0.597618 \u2506 0.064757 \u2506 0.989752 \u2506 0.873602 \u2506 4.603702 \u2506 7            \u2502\n",
-                            "\u2502 3   \u2506 0.69054  \u2506 0.128104 \u2506 0.67956  \u2506 0.417295 \u2506 7.269824 \u2506 22           \u2502\n",
-                            "\u2502 4   \u2506 0.970639 \u2506 0.49373  \u2506 0.811869 \u2506 0.345611 \u2506 1.671346 \u2506 10           \u2502\n",
+                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 9            \u2502\n",
+                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 11           \u2502\n",
+                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 13           \u2502\n",
+                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 27           \u2502\n",
+                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 14           \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 37,
+                    "execution_count": 39,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Get neighbor count. The point itself is always considered a neighbor to itself.\n",
                 "df.with_columns(\n",
@@ -1672,46 +1755,46 @@
                 "        parallel = True \n",
                 "    ).alias(\"nb_l_inf_cnt\")\n",
                 ").head() "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 40,
             "id": "69ad83d1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l1_r_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.344033</td><td>0.329014</td><td>0.58807</td><td>0.620571</td><td>9.086603</td><td>608</td></tr><tr><td>1</td><td>0.478353</td><td>0.639429</td><td>0.112137</td><td>0.889891</td><td>6.60086</td><td>961</td></tr><tr><td>2</td><td>0.597618</td><td>0.064757</td><td>0.989752</td><td>0.873602</td><td>4.603702</td><td>499</td></tr><tr><td>3</td><td>0.69054</td><td>0.128104</td><td>0.67956</td><td>0.417295</td><td>7.269824</td><td>168</td></tr><tr><td>4</td><td>0.970639</td><td>0.49373</td><td>0.811869</td><td>0.345611</td><td>1.671346</td><td>82</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l1_r_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>352</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>71</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>99</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>199</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>523</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 7)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 nb_l1_r_cnt \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---         \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 u32         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.344033 \u2506 0.329014 \u2506 0.58807  \u2506 0.620571 \u2506 9.086603 \u2506 608         \u2502\n",
-                            "\u2502 1   \u2506 0.478353 \u2506 0.639429 \u2506 0.112137 \u2506 0.889891 \u2506 6.60086  \u2506 961         \u2502\n",
-                            "\u2502 2   \u2506 0.597618 \u2506 0.064757 \u2506 0.989752 \u2506 0.873602 \u2506 4.603702 \u2506 499         \u2502\n",
-                            "\u2502 3   \u2506 0.69054  \u2506 0.128104 \u2506 0.67956  \u2506 0.417295 \u2506 7.269824 \u2506 168         \u2502\n",
-                            "\u2502 4   \u2506 0.970639 \u2506 0.49373  \u2506 0.811869 \u2506 0.345611 \u2506 1.671346 \u2506 82          \u2502\n",
+                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 352         \u2502\n",
+                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 71          \u2502\n",
+                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 99          \u2502\n",
+                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 199         \u2502\n",
+                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 523         \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 38,
+                    "execution_count": 40,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.with_columns(\n",
                 "    pds.query_nb_cnt(\n",
@@ -1721,46 +1804,46 @@
                 "        parallel = True \n",
                 "    ).alias(\"nb_l1_r_cnt\")\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 41,
             "id": "ce1a2c7a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>best friends</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>0.344033</td><td>0.329014</td><td>0.58807</td><td>0.620571</td><td>9.086603</td><td>[0, 1723, \u2026 498]</td></tr><tr><td>1</td><td>0.478353</td><td>0.639429</td><td>0.112137</td><td>0.889891</td><td>6.60086</td><td>[1, 100, \u2026 1663]</td></tr><tr><td>2</td><td>0.597618</td><td>0.064757</td><td>0.989752</td><td>0.873602</td><td>4.603702</td><td>[2, 1388, \u2026 316]</td></tr><tr><td>3</td><td>0.69054</td><td>0.128104</td><td>0.67956</td><td>0.417295</td><td>7.269824</td><td>[3, 1696, \u2026 1630]</td></tr><tr><td>4</td><td>0.970639</td><td>0.49373</td><td>0.811869</td><td>0.345611</td><td>1.671346</td><td>[4, 739, \u2026 1854]</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>best friends</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>[0, 1537, \u2026 1065]</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>[1, 729, \u2026 377]</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>[2, 1246, \u2026 1666]</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>[3, 898, \u2026 631]</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>[4, 1096, \u2026 165]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 7)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 best friends      \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---               \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 list[u32]         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.344033 \u2506 0.329014 \u2506 0.58807  \u2506 0.620571 \u2506 9.086603 \u2506 [0, 1723, \u2026 498]  \u2502\n",
-                            "\u2502 1   \u2506 0.478353 \u2506 0.639429 \u2506 0.112137 \u2506 0.889891 \u2506 6.60086  \u2506 [1, 100, \u2026 1663]  \u2502\n",
-                            "\u2502 2   \u2506 0.597618 \u2506 0.064757 \u2506 0.989752 \u2506 0.873602 \u2506 4.603702 \u2506 [2, 1388, \u2026 316]  \u2502\n",
-                            "\u2502 3   \u2506 0.69054  \u2506 0.128104 \u2506 0.67956  \u2506 0.417295 \u2506 7.269824 \u2506 [3, 1696, \u2026 1630] \u2502\n",
-                            "\u2502 4   \u2506 0.970639 \u2506 0.49373  \u2506 0.811869 \u2506 0.345611 \u2506 1.671346 \u2506 [4, 739, \u2026 1854]  \u2502\n",
+                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 [0, 1537, \u2026 1065] \u2502\n",
+                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 [1, 729, \u2026 377]   \u2502\n",
+                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 [2, 1246, \u2026 1666] \u2502\n",
+                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 [3, 898, \u2026 631]   \u2502\n",
+                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 [4, 1096, \u2026 165]  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 39,
+                    "execution_count": 41,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Get ids of the k nearest neighbors. \n",
                 "# The point itself is always considered a neighbor to itself, so k + 1 elements will be returned.\n",
@@ -1773,33 +1856,33 @@
                 "        parallel = True\n",
                 "    ).alias(\"best friends\")\n",
                 ").head() "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": 42,
             "id": "67a769f3",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "shape: (5, 3)\n",
                         "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                         "\u2502 id  \u2506 best friends      \u2506 best friends count \u2502\n",
                         "\u2502 --- \u2506 ---               \u2506 ---                \u2502\n",
                         "\u2502 u32 \u2506 list[u32]         \u2506 u32                \u2502\n",
                         "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                        "\u2502 0   \u2506 [0, 1723, \u2026 654]  \u2506 274                \u2502\n",
-                        "\u2502 1   \u2506 [1, 100, \u2026 1950]  \u2506 191                \u2502\n",
-                        "\u2502 2   \u2506 [2, 1388, \u2026 1696] \u2506 88                 \u2502\n",
-                        "\u2502 3   \u2506 [3, 1696, \u2026 1897] \u2506 220                \u2502\n",
-                        "\u2502 4   \u2506 [4, 739, \u2026 968]   \u2506 159                \u2502\n",
+                        "\u2502 0   \u2506 [0, 1537, \u2026 298]  \u2506 140                \u2502\n",
+                        "\u2502 1   \u2506 [1, 729, \u2026 1477]  \u2506 266                \u2502\n",
+                        "\u2502 2   \u2506 [2, 1246, \u2026 1619] \u2506 172                \u2502\n",
+                        "\u2502 3   \u2506 [3, 898, \u2026 811]   \u2506 172                \u2502\n",
+                        "\u2502 4   \u2506 [4, 1096, \u2026 461]  \u2506 160                \u2502\n",
                         "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n"
                     ]
                 }
             ],
             "source": [
                 "# Get all neighbors within radius r\n",
                 "# The point itself is always considered a neighbor to itself.\n",
@@ -1815,51 +1898,51 @@
                 ").with_columns( # -1 to remove the point itself\n",
                 "    (pl.col(\"best friends\").list.len() - 1).alias(\"best friends count\")\n",
                 ").head())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 43,
             "id": "06cd7fb2",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>idx</th><th>dist</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td><td>list[f64]</td></tr></thead><tbody><tr><td>0</td><td>0.344033</td><td>0.329014</td><td>0.58807</td><td>0.620571</td><td>9.086603</td><td>[0, 1723, \u2026 498]</td><td>[0.0, 0.001033, \u2026 0.006188]</td></tr><tr><td>1</td><td>0.478353</td><td>0.639429</td><td>0.112137</td><td>0.889891</td><td>6.60086</td><td>[1, 100, \u2026 1663]</td><td>[0.0, 0.00246, \u2026 0.004004]</td></tr><tr><td>2</td><td>0.597618</td><td>0.064757</td><td>0.989752</td><td>0.873602</td><td>4.603702</td><td>[2, 1388, \u2026 316]</td><td>[0.0, 0.004788, \u2026 0.008095]</td></tr><tr><td>3</td><td>0.69054</td><td>0.128104</td><td>0.67956</td><td>0.417295</td><td>7.269824</td><td>[3, 1696, \u2026 1630]</td><td>[0.0, 0.000318, \u2026 0.003333]</td></tr><tr><td>4</td><td>0.970639</td><td>0.49373</td><td>0.811869</td><td>0.345611</td><td>1.671346</td><td>[4, 739, \u2026 1854]</td><td>[0.0, 0.005646, \u2026 0.00948]</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>idx</th><th>dist</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td><td>list[f64]</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>[0, 1537, \u2026 1065]</td><td>[0.0, 0.0013, \u2026 0.006013]</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>[1, 729, \u2026 377]</td><td>[0.0, 0.003972, \u2026 0.006201]</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>[2, 1246, \u2026 1666]</td><td>[0.0, 0.001598, \u2026 0.003286]</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>[3, 898, \u2026 631]</td><td>[0.0, 0.001056, \u2026 0.003583]</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>[4, 1096, \u2026 165]</td><td>[0.0, 0.001941, \u2026 0.007024]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 8)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 idx              \u2506 dist             \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---              \u2506 ---              \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 list[u32]        \u2506 list[f64]        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.344033 \u2506 0.329014 \u2506 0.58807  \u2506 0.620571 \u2506 9.086603 \u2506 [0, 1723, \u2026 498] \u2506 [0.0, 0.001033,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.006188]      \u2502\n",
-                            "\u2502 1   \u2506 0.478353 \u2506 0.639429 \u2506 0.112137 \u2506 0.889891 \u2506 6.60086  \u2506 [1, 100, \u2026 1663] \u2506 [0.0, 0.00246, \u2026 \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 0.004004]        \u2502\n",
-                            "\u2502 2   \u2506 0.597618 \u2506 0.064757 \u2506 0.989752 \u2506 0.873602 \u2506 4.603702 \u2506 [2, 1388, \u2026 316] \u2506 [0.0, 0.004788,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.008095]      \u2502\n",
-                            "\u2502 3   \u2506 0.69054  \u2506 0.128104 \u2506 0.67956  \u2506 0.417295 \u2506 7.269824 \u2506 [3, 1696, \u2026      \u2506 [0.0, 0.000318,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1630]            \u2506 \u2026 0.003333]      \u2502\n",
-                            "\u2502 4   \u2506 0.970639 \u2506 0.49373  \u2506 0.811869 \u2506 0.345611 \u2506 1.671346 \u2506 [4, 739, \u2026 1854] \u2506 [0.0, 0.005646,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.00948]       \u2502\n",
+                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 [0, 1537, \u2026      \u2506 [0.0, 0.0013, \u2026  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1065]            \u2506 0.006013]        \u2502\n",
+                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 [1, 729, \u2026 377]  \u2506 [0.0, 0.003972,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.006201]      \u2502\n",
+                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 [2, 1246, \u2026      \u2506 [0.0, 0.001598,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1666]            \u2506 \u2026 0.003286]      \u2502\n",
+                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 [3, 898, \u2026 631]  \u2506 [0.0, 0.001056,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.003583]      \u2502\n",
+                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 [4, 1096, \u2026 165] \u2506 [0.0, 0.001941,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.007024]      \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 41,
+                    "execution_count": 43,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Get ids of the k nearest neighbors and distances\n",
                 "# The point itself is always considered a neighbor to itself, so k + 1 elements will be returned.\n",
@@ -1873,46 +1956,46 @@
                 "        return_dist = True\n",
                 "    ).alias(\"best_friends_w_dist\")\n",
                 ").unnest(\"best_friends_w_dist\").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": 44,
             "id": "b5c69ae4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>0</td><td>0.344033</td><td>0.329014</td><td>0.58807</td><td>0.620571</td><td>9.086603</td></tr><tr><td>1</td><td>0.478353</td><td>0.639429</td><td>0.112137</td><td>0.889891</td><td>6.60086</td></tr><tr><td>6</td><td>0.208114</td><td>0.309071</td><td>0.705663</td><td>0.108659</td><td>5.790588</td></tr><tr><td>8</td><td>0.15995</td><td>0.528839</td><td>0.520647</td><td>0.830624</td><td>3.777744</td></tr><tr><td>9</td><td>0.842498</td><td>0.493781</td><td>0.374203</td><td>0.080603</td><td>5.046259</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td></tr><tr><td>6</td><td>0.356637</td><td>0.916926</td><td>0.509538</td><td>0.344282</td><td>5.110688</td></tr><tr><td>7</td><td>0.489873</td><td>0.351803</td><td>0.861379</td><td>0.985876</td><td>3.487034</td></tr><tr><td>8</td><td>0.485547</td><td>0.796377</td><td>0.776287</td><td>0.102771</td><td>9.366586</td></tr><tr><td>11</td><td>0.548642</td><td>0.621415</td><td>0.179476</td><td>0.942682</td><td>9.447275</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 6)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.344033 \u2506 0.329014 \u2506 0.58807  \u2506 0.620571 \u2506 9.086603 \u2502\n",
-                            "\u2502 1   \u2506 0.478353 \u2506 0.639429 \u2506 0.112137 \u2506 0.889891 \u2506 6.60086  \u2502\n",
-                            "\u2502 6   \u2506 0.208114 \u2506 0.309071 \u2506 0.705663 \u2506 0.108659 \u2506 5.790588 \u2502\n",
-                            "\u2502 8   \u2506 0.15995  \u2506 0.528839 \u2506 0.520647 \u2506 0.830624 \u2506 3.777744 \u2502\n",
-                            "\u2502 9   \u2506 0.842498 \u2506 0.493781 \u2506 0.374203 \u2506 0.080603 \u2506 5.046259 \u2502\n",
+                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2502\n",
+                            "\u2502 6   \u2506 0.356637 \u2506 0.916926 \u2506 0.509538 \u2506 0.344282 \u2506 5.110688 \u2502\n",
+                            "\u2502 7   \u2506 0.489873 \u2506 0.351803 \u2506 0.861379 \u2506 0.985876 \u2506 3.487034 \u2502\n",
+                            "\u2502 8   \u2506 0.485547 \u2506 0.796377 \u2506 0.776287 \u2506 0.102771 \u2506 9.366586 \u2502\n",
+                            "\u2502 11  \u2506 0.548642 \u2506 0.621415 \u2506 0.179476 \u2506 0.942682 \u2506 9.447275 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 42,
+                    "execution_count": 44,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Filter to only points near the given point\n",
                 "df.filter(\n",
@@ -1923,46 +2006,46 @@
                 "        dist = \"l2\" # actually this is squared l2, so this is asking for squared l2 <= 0.2\n",
                 "    )\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 45,
             "id": "4ab9e8f8",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>26</td><td>0.511227</td><td>0.576175</td><td>0.746274</td><td>0.411243</td><td>5.15106</td></tr><tr><td>43</td><td>0.536511</td><td>0.444647</td><td>0.769464</td><td>0.697085</td><td>7.34396</td></tr><tr><td>59</td><td>0.546228</td><td>0.426638</td><td>0.939578</td><td>0.198419</td><td>4.084241</td></tr><tr><td>68</td><td>0.584769</td><td>0.481015</td><td>0.933041</td><td>0.098676</td><td>5.526402</td></tr><tr><td>105</td><td>0.533976</td><td>0.540488</td><td>0.997894</td><td>0.348852</td><td>7.652499</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>50</td><td>0.521872</td><td>0.520009</td><td>0.089207</td><td>0.446793</td><td>2.756932</td></tr><tr><td>138</td><td>0.476258</td><td>0.457252</td><td>0.578248</td><td>0.696907</td><td>4.576948</td></tr><tr><td>174</td><td>0.466104</td><td>0.489402</td><td>0.703968</td><td>0.308085</td><td>7.681611</td></tr><tr><td>178</td><td>0.478427</td><td>0.490086</td><td>0.903002</td><td>0.287589</td><td>5.352698</td></tr><tr><td>319</td><td>0.413976</td><td>0.488702</td><td>0.666915</td><td>0.328137</td><td>5.147284</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 6)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 26  \u2506 0.511227 \u2506 0.576175 \u2506 0.746274 \u2506 0.411243 \u2506 5.15106  \u2502\n",
-                            "\u2502 43  \u2506 0.536511 \u2506 0.444647 \u2506 0.769464 \u2506 0.697085 \u2506 7.34396  \u2502\n",
-                            "\u2502 59  \u2506 0.546228 \u2506 0.426638 \u2506 0.939578 \u2506 0.198419 \u2506 4.084241 \u2502\n",
-                            "\u2502 68  \u2506 0.584769 \u2506 0.481015 \u2506 0.933041 \u2506 0.098676 \u2506 5.526402 \u2502\n",
-                            "\u2502 105 \u2506 0.533976 \u2506 0.540488 \u2506 0.997894 \u2506 0.348852 \u2506 7.652499 \u2502\n",
+                            "\u2502 50  \u2506 0.521872 \u2506 0.520009 \u2506 0.089207 \u2506 0.446793 \u2506 2.756932 \u2502\n",
+                            "\u2502 138 \u2506 0.476258 \u2506 0.457252 \u2506 0.578248 \u2506 0.696907 \u2506 4.576948 \u2502\n",
+                            "\u2502 174 \u2506 0.466104 \u2506 0.489402 \u2506 0.703968 \u2506 0.308085 \u2506 7.681611 \u2502\n",
+                            "\u2502 178 \u2506 0.478427 \u2506 0.490086 \u2506 0.903002 \u2506 0.287589 \u2506 5.352698 \u2502\n",
+                            "\u2502 319 \u2506 0.413976 \u2506 0.488702 \u2506 0.666915 \u2506 0.328137 \u2506 5.147284 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 43,
+                    "execution_count": 45,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Haversine distance is available when dimension is 2\n",
                 "df.filter(\n",
@@ -1973,46 +2056,46 @@
                 "        dist = \"h\" \n",
                 "    )\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 46,
             "id": "7d3f5ae4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>105</td><td>0.533976</td><td>0.540488</td><td>0.997894</td><td>0.348852</td><td>7.652499</td></tr><tr><td>108</td><td>0.479439</td><td>0.467258</td><td>0.354607</td><td>0.05688</td><td>9.206828</td></tr><tr><td>378</td><td>0.466436</td><td>0.561065</td><td>0.593606</td><td>0.98562</td><td>8.152283</td></tr><tr><td>381</td><td>0.487925</td><td>0.556872</td><td>0.417955</td><td>0.309115</td><td>9.76867</td></tr><tr><td>545</td><td>0.456857</td><td>0.559035</td><td>0.431411</td><td>0.195722</td><td>9.912245</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>174</td><td>0.466104</td><td>0.489402</td><td>0.703968</td><td>0.308085</td><td>7.681611</td></tr><tr><td>178</td><td>0.478427</td><td>0.490086</td><td>0.903002</td><td>0.287589</td><td>5.352698</td></tr><tr><td>331</td><td>0.46378</td><td>0.470691</td><td>0.504769</td><td>0.565669</td><td>8.41936</td></tr><tr><td>388</td><td>0.469873</td><td>0.490685</td><td>0.51908</td><td>0.135412</td><td>9.419304</td></tr><tr><td>482</td><td>0.499758</td><td>0.505641</td><td>0.436567</td><td>0.83411</td><td>0.849715</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 6)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 105 \u2506 0.533976 \u2506 0.540488 \u2506 0.997894 \u2506 0.348852 \u2506 7.652499 \u2502\n",
-                            "\u2502 108 \u2506 0.479439 \u2506 0.467258 \u2506 0.354607 \u2506 0.05688  \u2506 9.206828 \u2502\n",
-                            "\u2502 378 \u2506 0.466436 \u2506 0.561065 \u2506 0.593606 \u2506 0.98562  \u2506 8.152283 \u2502\n",
-                            "\u2502 381 \u2506 0.487925 \u2506 0.556872 \u2506 0.417955 \u2506 0.309115 \u2506 9.76867  \u2502\n",
-                            "\u2502 545 \u2506 0.456857 \u2506 0.559035 \u2506 0.431411 \u2506 0.195722 \u2506 9.912245 \u2502\n",
+                            "\u2502 174 \u2506 0.466104 \u2506 0.489402 \u2506 0.703968 \u2506 0.308085 \u2506 7.681611 \u2502\n",
+                            "\u2502 178 \u2506 0.478427 \u2506 0.490086 \u2506 0.903002 \u2506 0.287589 \u2506 5.352698 \u2502\n",
+                            "\u2502 331 \u2506 0.46378  \u2506 0.470691 \u2506 0.504769 \u2506 0.565669 \u2506 8.41936  \u2502\n",
+                            "\u2502 388 \u2506 0.469873 \u2506 0.490685 \u2506 0.51908  \u2506 0.135412 \u2506 9.419304 \u2502\n",
+                            "\u2502 482 \u2506 0.499758 \u2506 0.505641 \u2506 0.436567 \u2506 0.83411  \u2506 0.849715 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 44,
+                    "execution_count": 46,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.filter(\n",
                 "    pds.query_within_dist_from(\n",
@@ -2023,46 +2106,46 @@
                 "        dist = \"h\" \n",
                 "    )\n",
                 ").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 47,
             "id": "f14627bc",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th><th>count</th></tr><tr><td>u64</td><td>list[u32]</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>[0, 857, \u2026 1529]</td><td>126</td></tr><tr><td>1</td><td>[1, 914, \u2026 1971]</td><td>130</td></tr><tr><td>2</td><td>[2, 246, \u2026 484]</td><td>85</td></tr><tr><td>3</td><td>[3, 98, \u2026 1706]</td><td>99</td></tr><tr><td>4</td><td>[4, 1849, \u2026 1743]</td><td>84</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th><th>count</th></tr><tr><td>u64</td><td>list[u32]</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>[0, 1675, \u2026 1305]</td><td>79</td></tr><tr><td>1</td><td>[1, 128, \u2026 322]</td><td>112</td></tr><tr><td>2</td><td>[2, 54, \u2026 1633]</td><td>94</td></tr><tr><td>3</td><td>[3, 963, \u2026 978]</td><td>122</td></tr><tr><td>4</td><td>[4, 61, \u2026 1899]</td><td>120</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 friends           \u2506 count \u2502\n",
                             "\u2502 --- \u2506 ---               \u2506 ---   \u2502\n",
                             "\u2502 u64 \u2506 list[u32]         \u2506 u32   \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 [0, 857, \u2026 1529]  \u2506 126   \u2502\n",
-                            "\u2502 1   \u2506 [1, 914, \u2026 1971]  \u2506 130   \u2502\n",
-                            "\u2502 2   \u2506 [2, 246, \u2026 484]   \u2506 85    \u2502\n",
-                            "\u2502 3   \u2506 [3, 98, \u2026 1706]   \u2506 99    \u2502\n",
-                            "\u2502 4   \u2506 [4, 1849, \u2026 1743] \u2506 84    \u2502\n",
+                            "\u2502 0   \u2506 [0, 1675, \u2026 1305] \u2506 79    \u2502\n",
+                            "\u2502 1   \u2506 [1, 128, \u2026 322]   \u2506 112   \u2502\n",
+                            "\u2502 2   \u2506 [2, 54, \u2026 1633]   \u2506 94    \u2502\n",
+                            "\u2502 3   \u2506 [3, 963, \u2026 978]   \u2506 122   \u2502\n",
+                            "\u2502 4   \u2506 [4, 61, \u2026 1899]   \u2506 120   \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 45,
+                    "execution_count": 47,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "friends = df.select(\n",
                 "    pl.col(\"id\").cast(pl.UInt64),\n",
@@ -2089,58 +2172,58 @@
                 "There is limited functionality in the Graph module currently. E.g. Only constant cost per edge.\n",
                 "\n",
                 "Graph queries are very expensive."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": 48,
             "id": "fba0149e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# friends.select(\n",
                 "#     pl.col(\"friends\").graph.eigen_centrality() # .arg_max()\n",
                 "# ).head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 49,
             "id": "9d2b70d7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0</td></tr><tr><td>0</td><td>857</td></tr><tr><td>0</td><td>92</td></tr><tr><td>0</td><td>692</td></tr><tr><td>0</td><td>1975</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0</td></tr><tr><td>0</td><td>1675</td></tr><tr><td>0</td><td>33</td></tr><tr><td>0</td><td>905</td></tr><tr><td>0</td><td>806</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 friends \u2502\n",
                             "\u2502 --- \u2506 ---     \u2502\n",
                             "\u2502 u32 \u2506 u32     \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 0   \u2506 0       \u2502\n",
-                            "\u2502 0   \u2506 857     \u2502\n",
-                            "\u2502 0   \u2506 92      \u2502\n",
-                            "\u2502 0   \u2506 692     \u2502\n",
-                            "\u2502 0   \u2506 1975    \u2502\n",
+                            "\u2502 0   \u2506 1675    \u2502\n",
+                            "\u2502 0   \u2506 33      \u2502\n",
+                            "\u2502 0   \u2506 905     \u2502\n",
+                            "\u2502 0   \u2506 806     \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 47,
+                    "execution_count": 49,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Turn friends to a table suitable for graph analytics\n",
                 "df_graph = friends.select(\n",
@@ -2151,119 +2234,119 @@
                 "    pl.col(\"friends\").cast(pl.UInt32),\n",
                 ")\n",
                 "df_graph.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": 50,
             "id": "8ff9aa74",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th></tr><tr><td>u32</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>[1207, 171, \u2026 3]</td></tr><tr><td>1</td><td>[1085, 1603, \u2026 3]</td></tr><tr><td>2</td><td>[3]</td></tr><tr><td>3</td><td>[]</td></tr><tr><td>4</td><td>[1743, 822, \u2026 3]</td></tr><tr><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1995</td><td>[558, 54, \u2026 3]</td></tr><tr><td>1996</td><td>[1879, 859, \u2026 3]</td></tr><tr><td>1997</td><td>[1081, 1769, \u2026 3]</td></tr><tr><td>1998</td><td>[203, 760, 3]</td></tr><tr><td>1999</td><td>[119, 1580, \u2026 3]</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th></tr><tr><td>u32</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>[3]</td></tr><tr><td>1</td><td>[1594, 1975, 3]</td></tr><tr><td>2</td><td>[1673, 1707, 3]</td></tr><tr><td>3</td><td>[]</td></tr><tr><td>4</td><td>[1070, 1200, \u2026 3]</td></tr><tr><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1995</td><td>[94, 1397, \u2026 3]</td></tr><tr><td>1996</td><td>[469, 1739, \u2026 3]</td></tr><tr><td>1997</td><td>[797, 1853, \u2026 3]</td></tr><tr><td>1998</td><td>[1994, 197, \u2026 3]</td></tr><tr><td>1999</td><td>[409, 1278, 3]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id   \u2506 path              \u2502\n",
                             "\u2502 ---  \u2506 ---               \u2502\n",
                             "\u2502 u32  \u2506 list[u32]         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0    \u2506 [1207, 171, \u2026 3]  \u2502\n",
-                            "\u2502 1    \u2506 [1085, 1603, \u2026 3] \u2502\n",
-                            "\u2502 2    \u2506 [3]               \u2502\n",
+                            "\u2502 0    \u2506 [3]               \u2502\n",
+                            "\u2502 1    \u2506 [1594, 1975, 3]   \u2502\n",
+                            "\u2502 2    \u2506 [1673, 1707, 3]   \u2502\n",
                             "\u2502 3    \u2506 []                \u2502\n",
-                            "\u2502 4    \u2506 [1743, 822, \u2026 3]  \u2502\n",
+                            "\u2502 4    \u2506 [1070, 1200, \u2026 3] \u2502\n",
                             "\u2502 \u2026    \u2506 \u2026                 \u2502\n",
-                            "\u2502 1995 \u2506 [558, 54, \u2026 3]    \u2502\n",
-                            "\u2502 1996 \u2506 [1879, 859, \u2026 3]  \u2502\n",
-                            "\u2502 1997 \u2506 [1081, 1769, \u2026 3] \u2502\n",
-                            "\u2502 1998 \u2506 [203, 760, 3]     \u2502\n",
-                            "\u2502 1999 \u2506 [119, 1580, \u2026 3]  \u2502\n",
+                            "\u2502 1995 \u2506 [94, 1397, \u2026 3]   \u2502\n",
+                            "\u2502 1996 \u2506 [469, 1739, \u2026 3]  \u2502\n",
+                            "\u2502 1997 \u2506 [797, 1853, \u2026 3]  \u2502\n",
+                            "\u2502 1998 \u2506 [1994, 197, \u2026 3]  \u2502\n",
+                            "\u2502 1999 \u2506 [409, 1278, 3]    \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 48,
+                    "execution_count": 50,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df_graph.select(\n",
                 "    # Shortest path to the node with id = 3\n",
                 "    # Node and link can be str | pl.Expr\n",
                 "    pds.query_shortest_path(node = \"id\", link = pl.col(\"friends\"), target = 3, cost = None, parallel=True).alias(\"shortest_path\")\n",
                 ").unnest(\"shortest_path\").sort(\"id\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 49,
+            "execution_count": 51,
             "id": "76d43fd5",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>reachable</th><th>steps</th></tr><tr><td>u32</td><td>bool</td><td>u32</td></tr></thead><tbody><tr><td>1871</td><td>true</td><td>6</td></tr><tr><td>865</td><td>true</td><td>7</td></tr><tr><td>431</td><td>true</td><td>5</td></tr><tr><td>1557</td><td>true</td><td>2</td></tr><tr><td>191</td><td>true</td><td>6</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>637</td><td>true</td><td>5</td></tr><tr><td>190</td><td>true</td><td>2</td></tr><tr><td>768</td><td>true</td><td>8</td></tr><tr><td>340</td><td>true</td><td>6</td></tr><tr><td>1318</td><td>true</td><td>6</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>reachable</th><th>steps</th></tr><tr><td>u32</td><td>bool</td><td>u32</td></tr></thead><tbody><tr><td>958</td><td>true</td><td>4</td></tr><tr><td>1420</td><td>true</td><td>3</td></tr><tr><td>1505</td><td>true</td><td>1</td></tr><tr><td>1027</td><td>true</td><td>7</td></tr><tr><td>1577</td><td>true</td><td>3</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1791</td><td>true</td><td>7</td></tr><tr><td>1777</td><td>true</td><td>8</td></tr><tr><td>1113</td><td>true</td><td>3</td></tr><tr><td>550</td><td>true</td><td>6</td></tr><tr><td>1653</td><td>true</td><td>1</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id   \u2506 reachable \u2506 steps \u2502\n",
                             "\u2502 ---  \u2506 ---       \u2506 ---   \u2502\n",
                             "\u2502 u32  \u2506 bool      \u2506 u32   \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1871 \u2506 true      \u2506 6     \u2502\n",
-                            "\u2502 865  \u2506 true      \u2506 7     \u2502\n",
-                            "\u2502 431  \u2506 true      \u2506 5     \u2502\n",
-                            "\u2502 1557 \u2506 true      \u2506 2     \u2502\n",
-                            "\u2502 191  \u2506 true      \u2506 6     \u2502\n",
+                            "\u2502 958  \u2506 true      \u2506 4     \u2502\n",
+                            "\u2502 1420 \u2506 true      \u2506 3     \u2502\n",
+                            "\u2502 1505 \u2506 true      \u2506 1     \u2502\n",
+                            "\u2502 1027 \u2506 true      \u2506 7     \u2502\n",
+                            "\u2502 1577 \u2506 true      \u2506 3     \u2502\n",
                             "\u2502 \u2026    \u2506 \u2026         \u2506 \u2026     \u2502\n",
-                            "\u2502 637  \u2506 true      \u2506 5     \u2502\n",
-                            "\u2502 190  \u2506 true      \u2506 2     \u2502\n",
-                            "\u2502 768  \u2506 true      \u2506 8     \u2502\n",
-                            "\u2502 340  \u2506 true      \u2506 6     \u2502\n",
-                            "\u2502 1318 \u2506 true      \u2506 6     \u2502\n",
+                            "\u2502 1791 \u2506 true      \u2506 7     \u2502\n",
+                            "\u2502 1777 \u2506 true      \u2506 8     \u2502\n",
+                            "\u2502 1113 \u2506 true      \u2506 3     \u2502\n",
+                            "\u2502 550  \u2506 true      \u2506 6     \u2502\n",
+                            "\u2502 1653 \u2506 true      \u2506 1     \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 49,
+                    "execution_count": 51,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df_graph.select(\n",
                 "    # Almost every node can reach node 3, and the number is the number steps to reach it\n",
                 "    # This is a way faster way to filter results if you don't need the actual path\n",
                 "    pds.query_node_reachable(\"id\", \"friends\", target = 3).alias(\"reach\")\n",
                 ").unnest(\"reach\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 50,
+            "execution_count": 52,
             "id": "4af6e6b7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -2292,15 +2375,15 @@
                             "\u2502 3   \u2506 0           \u2506 0.1        \u2502\n",
                             "\u2502 3   \u2506 1           \u2506 0.1        \u2502\n",
                             "\u2502 3   \u2506 2           \u2506 0.1        \u2502\n",
                             "\u2502 4   \u2506 1           \u2506 0.1        \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 50,
+                    "execution_count": 52,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "relationships = pl.DataFrame({\n",
                 "    \"id\": range(5),\n",
@@ -2315,91 +2398,91 @@
                 ")\n",
                 "\n",
                 "relationships.head(50)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 51,
+            "execution_count": 53,
             "id": "239f4e85",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th><th>cost</th></tr><tr><td>u32</td><td>list[u32]</td><td>f64</td></tr></thead><tbody><tr><td>1</td><td>[]</td><td>0.0</td></tr><tr><td>0</td><td>[4, 1]</td><td>0.2</td></tr><tr><td>2</td><td>[4, 1]</td><td>0.6</td></tr><tr><td>3</td><td>[1]</td><td>0.1</td></tr><tr><td>4</td><td>[1]</td><td>0.1</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th><th>cost</th></tr><tr><td>u32</td><td>list[u32]</td><td>f64</td></tr></thead><tbody><tr><td>3</td><td>[1]</td><td>0.1</td></tr><tr><td>2</td><td>[4, 1]</td><td>0.6</td></tr><tr><td>0</td><td>[4, 1]</td><td>0.2</td></tr><tr><td>1</td><td>[]</td><td>0.0</td></tr><tr><td>4</td><td>[1]</td><td>0.1</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 path      \u2506 cost \u2502\n",
                             "\u2502 --- \u2506 ---       \u2506 ---  \u2502\n",
                             "\u2502 u32 \u2506 list[u32] \u2506 f64  \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1   \u2506 []        \u2506 0.0  \u2502\n",
-                            "\u2502 0   \u2506 [4, 1]    \u2506 0.2  \u2502\n",
-                            "\u2502 2   \u2506 [4, 1]    \u2506 0.6  \u2502\n",
                             "\u2502 3   \u2506 [1]       \u2506 0.1  \u2502\n",
+                            "\u2502 2   \u2506 [4, 1]    \u2506 0.6  \u2502\n",
+                            "\u2502 0   \u2506 [4, 1]    \u2506 0.2  \u2502\n",
+                            "\u2502 1   \u2506 []        \u2506 0.0  \u2502\n",
                             "\u2502 4   \u2506 [1]       \u2506 0.1  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 51,
+                    "execution_count": 53,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# To go to node at id = 1, node 0 would rather go to 4 first and then 1.\n",
                 "relationships.select(\n",
                 "    pds.query_shortest_path(\"id\", \"connections\", target = 1, cost = \"close-ness\").alias(\"path\")\n",
                 ").unnest(\"path\").head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": 54,
             "id": "df458bdd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>node</th><th>deg</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>1</td><td>2</td></tr><tr><td>0</td><td>4</td></tr><tr><td>2</td><td>1</td></tr><tr><td>3</td><td>3</td></tr><tr><td>4</td><td>1</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>node</th><th>deg</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>3</td><td>3</td></tr><tr><td>2</td><td>1</td></tr><tr><td>0</td><td>4</td></tr><tr><td>1</td><td>2</td></tr><tr><td>4</td><td>1</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 node \u2506 deg \u2502\n",
                             "\u2502 ---  \u2506 --- \u2502\n",
                             "\u2502 u32  \u2506 u32 \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1    \u2506 2   \u2502\n",
-                            "\u2502 0    \u2506 4   \u2502\n",
-                            "\u2502 2    \u2506 1   \u2502\n",
                             "\u2502 3    \u2506 3   \u2502\n",
+                            "\u2502 2    \u2506 1   \u2502\n",
+                            "\u2502 0    \u2506 4   \u2502\n",
+                            "\u2502 1    \u2506 2   \u2502\n",
                             "\u2502 4    \u2506 1   \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 52,
+                    "execution_count": 54,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# In and out deg\n",
                 "relationships.select(\n",
@@ -2415,28 +2498,28 @@
                 "# String Nearest Neighbors\n",
                 "\n",
                 "This might be very slow for very large vocab / column."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 53,
+            "execution_count": 55,
             "id": "f2c9ed80",
             "metadata": {},
             "outputs": [],
             "source": [
                 "df = pl.DataFrame({\n",
                 "    \"a\":[\"AAAAA\", \"ABCABC\", \"AAAADDD\", \"ADSDSDS\", \"WORD\"],\n",
                 "    \"b\":[\"AAAAT\", \"ABCACD\", \"ADSSD\", \"APPLES\", \"WORLD\"] \n",
                 "})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 54,
+            "execution_count": 56,
             "id": "062fd694",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -2459,15 +2542,15 @@
                             "\u2502 ABCACD                   \u2502\n",
                             "\u2502 AAAAT                    \u2502\n",
                             "\u2502 ADSSD                    \u2502\n",
                             "\u2502 WORLD                    \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 54,
+                    "execution_count": 56,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Use Levenshtein to find the nearest neighbor in vocab to word in column a\n",
                 "df.select(\n",
@@ -2478,15 +2561,15 @@
                 "        metric = \"lv\"\n",
                 "    ).alias(\"similar_words_from_vocab\"),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 55,
+            "execution_count": 57,
             "id": "29437b8b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -2509,15 +2592,15 @@
                             "\u2502 [\"ABCACD\", \"AAAAT\"]      \u2502\n",
                             "\u2502 [\"AAAAT\", \"ABCACD\"]      \u2502\n",
                             "\u2502 [\"ADSSD\", \"APPLES\"]      \u2502\n",
                             "\u2502 [\"WORLD\", \"ADSSD\"]       \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 55,
+                    "execution_count": 57,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Use Levenshtein to find 2 nearest neighbors\n",
                 "df.select(\n",
@@ -2528,15 +2611,15 @@
                 "        metric = \"lv\"\n",
                 "    ).alias(\"similar_words_from_vocab\"),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 56,
+            "execution_count": 58,
             "id": "9150bece",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -2559,15 +2642,15 @@
                             "\u2502 [\"ABCACD\"]               \u2502\n",
                             "\u2502 []                       \u2502\n",
                             "\u2502 []                       \u2502\n",
                             "\u2502 []                       \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 56,
+                    "execution_count": 58,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Currently only Levenshtein and hamming are implemented for this\n",
                 "# Empty means nothing in vocab can be compared in the hamming sense with the corresponding word in a\n",
@@ -2580,15 +2663,15 @@
                 "        metric = \"hamming\"\n",
                 "    ).alias(\"similar_words_from_vocab\"),\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 57,
+            "execution_count": 59,
             "id": "b35776a1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
@@ -2611,15 +2694,15 @@
                             "\u2502 ABCABC  \u2506 [\"ABCDEFG\", \"AAAAA\", \"ZIV\"]   \u2502\n",
                             "\u2502 AAAADDD \u2506 [\"AAAAA\", \"WORLD\", \"ABCDEFG\"] \u2502\n",
                             "\u2502 ADSDSDS \u2506 [\"ABCDEFG\", \"WORLD\", \"AAAAA\"] \u2502\n",
                             "\u2502 WORD    \u2506 [\"WORLD\", \"ZIV\", \"TQQQ\"]      \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 57,
+                    "execution_count": 59,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# You may provide a vocab like this\n",
                 "df.select(\n",
```

### Comparing `polars_ds-0.4.1/examples/dependency.parquet` & `polars_ds-0.4.2/examples/dependency.parquet`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/examples/diagnosis.ipynb` & `polars_ds-0.4.2/examples/diagnosis.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96711026690573%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'data': {'text/html': {insert: [(7, '<small>shape: (5, "*

 * *            '6)</small><table border="1" '*

 * *            'class="dataframe"><thead><tr><th>uniform_1</th><th>uniform_2</th><th>exp</th><th>normal</th><th>fat_normal</th><th>list_prob</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[f64]</td></tr></thead><tbody><tr><td>3.867326</td><td>0.03482</td><td>1.00831</td><td>-0.62235</td><td>373.692025</td><td>[0.03482, '*

 * *            '0.96518]</t […]*

```diff
@@ -32,43 +32,45 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 5)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>uniform_1</th><th>uniform_2</th><th>exp</th><th>normal</th><th>fat_normal</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>8.848739</td><td>0.674563</td><td>6.468318</td><td>-0.441383</td><td>-365.360162</td></tr><tr><td>10.753657</td><td>0.465546</td><td>0.211793</td><td>-0.460255</td><td>1186.918797</td></tr><tr><td>5.312738</td><td>0.340861</td><td>0.189075</td><td>1.703051</td><td>1154.9914</td></tr><tr><td>5.691811</td><td>0.538038</td><td>2.03916</td><td>-0.259023</td><td>312.649592</td></tr><tr><td>6.511997</td><td>0.645332</td><td>3.130591</td><td>-0.9498</td><td>-954.291002</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>uniform_1</th><th>uniform_2</th><th>exp</th><th>normal</th><th>fat_normal</th><th>list_prob</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[f64]</td></tr></thead><tbody><tr><td>3.867326</td><td>0.03482</td><td>1.00831</td><td>-0.62235</td><td>373.692025</td><td>[0.03482, 0.96518]</td></tr><tr><td>3.172853</td><td>0.259646</td><td>2.071108</td><td>-0.69498</td><td>57.152982</td><td>[0.259646, 0.740354]</td></tr><tr><td>7.274324</td><td>0.96818</td><td>2.65899</td><td>0.545511</td><td>648.0624</td><td>[0.96818, 0.03182]</td></tr><tr><td>7.203889</td><td>0.829088</td><td>9.922334</td><td>1.327169</td><td>-1395.185035</td><td>[0.829088, 0.170912]</td></tr><tr><td>3.21813</td><td>0.250897</td><td>2.77609</td><td>0.47411</td><td>519.104254</td><td>[0.250897, 0.749103]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
-                            "shape: (5, 5)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 uniform_1 \u2506 uniform_2 \u2506 exp      \u2506 normal    \u2506 fat_normal  \u2502\n",
-                            "\u2502 ---       \u2506 ---       \u2506 ---      \u2506 ---       \u2506 ---         \u2502\n",
-                            "\u2502 f64       \u2506 f64       \u2506 f64      \u2506 f64       \u2506 f64         \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 8.848739  \u2506 0.674563  \u2506 6.468318 \u2506 -0.441383 \u2506 -365.360162 \u2502\n",
-                            "\u2502 10.753657 \u2506 0.465546  \u2506 0.211793 \u2506 -0.460255 \u2506 1186.918797 \u2502\n",
-                            "\u2502 5.312738  \u2506 0.340861  \u2506 0.189075 \u2506 1.703051  \u2506 1154.9914   \u2502\n",
-                            "\u2502 5.691811  \u2506 0.538038  \u2506 2.03916  \u2506 -0.259023 \u2506 312.649592  \u2502\n",
-                            "\u2502 6.511997  \u2506 0.645332  \u2506 3.130591 \u2506 -0.9498   \u2506 -954.291002 \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "shape: (5, 6)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 uniform_1 \u2506 uniform_2 \u2506 exp      \u2506 normal   \u2506 fat_normal   \u2506 list_prob            \u2502\n",
+                            "\u2502 ---       \u2506 ---       \u2506 ---      \u2506 ---      \u2506 ---          \u2506 ---                  \u2502\n",
+                            "\u2502 f64       \u2506 f64       \u2506 f64      \u2506 f64      \u2506 f64          \u2506 list[f64]            \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 3.867326  \u2506 0.03482   \u2506 1.00831  \u2506 -0.62235 \u2506 373.692025   \u2506 [0.03482, 0.96518]   \u2502\n",
+                            "\u2502 3.172853  \u2506 0.259646  \u2506 2.071108 \u2506 -0.69498 \u2506 57.152982    \u2506 [0.259646, 0.740354] \u2502\n",
+                            "\u2502 7.274324  \u2506 0.96818   \u2506 2.65899  \u2506 0.545511 \u2506 648.0624     \u2506 [0.96818, 0.03182]   \u2502\n",
+                            "\u2502 7.203889  \u2506 0.829088  \u2506 9.922334 \u2506 1.327169 \u2506 -1395.185035 \u2506 [0.829088, 0.170912] \u2502\n",
+                            "\u2502 3.21813   \u2506 0.250897  \u2506 2.77609  \u2506 0.47411  \u2506 519.104254   \u2506 [0.250897, 0.749103] \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = pds.random_data(size=100_000, n_cols = 0).select(\n",
                 "    pds.random(0.0, 12.0).alias(\"uniform_1\"),\n",
                 "    pds.random(0.0, 1.0).alias(\"uniform_2\"),\n",
                 "    pds.random_exp(0.5).alias(\"exp\"),\n",
                 "    pds.random_normal(0.0, 1.0).alias(\"normal\"),\n",
                 "    pds.random_normal(0.0, 1000.0).alias(\"fat_normal\"),\n",
+                ").with_columns(\n",
+                "    pl.concat_list(\"uniform_2\", 1 - pl.col(\"uniform_2\")).alias(\"list_prob\")\n",
                 ")\n",
                 "df.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
@@ -83,59 +85,59 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"noguwlnnhj\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
+                            "<div id=\"tzkgjbujru\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
                             "<style>\n",
-                            "#noguwlnnhj table {\n",
+                            "#tzkgjbujru table {\n",
                             "          font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;\n",
                             "          -webkit-font-smoothing: antialiased;\n",
                             "          -moz-osx-font-smoothing: grayscale;\n",
                             "        }\n",
                             "\n",
-                            "#noguwlnnhj thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
+                            "#tzkgjbujru thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
                             " tr { background-color: transparent !important; }\n",
-                            "#noguwlnnhj p { margin: 0 !important; padding: 0 !important; }\n",
-                            " #noguwlnnhj .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
-                            " #noguwlnnhj .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
-                            " #noguwlnnhj .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
-                            " #noguwlnnhj .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
-                            " #noguwlnnhj .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #noguwlnnhj .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #noguwlnnhj .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #noguwlnnhj .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
-                            " #noguwlnnhj .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
-                            " #noguwlnnhj .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
-                            " #noguwlnnhj .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
-                            " #noguwlnnhj .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
-                            " #noguwlnnhj .gt_spanner_row { border-bottom-style: hidden !important; }\n",
-                            " #noguwlnnhj .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
-                            " #noguwlnnhj .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
-                            " #noguwlnnhj .gt_from_md> :first-child { margin-top: 0 !important; }\n",
-                            " #noguwlnnhj .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
-                            " #noguwlnnhj .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
-                            " #noguwlnnhj .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
-                            " #noguwlnnhj .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
-                            " #noguwlnnhj .gt_row_group_first td { border-top-width: 2px !important; }\n",
-                            " #noguwlnnhj .gt_row_group_first th { border-top-width: 2px !important; }\n",
-                            " #noguwlnnhj .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #noguwlnnhj .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #noguwlnnhj .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
-                            " #noguwlnnhj .gt_left { text-align: left !important; }\n",
-                            " #noguwlnnhj .gt_center { text-align: center !important; }\n",
-                            " #noguwlnnhj .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
-                            " #noguwlnnhj .gt_font_normal { font-weight: normal !important; }\n",
-                            " #noguwlnnhj .gt_font_bold { font-weight: bold !important; }\n",
-                            " #noguwlnnhj .gt_font_italic { font-style: italic !important; }\n",
-                            " #noguwlnnhj .gt_super { font-size: 65% !important; }\n",
-                            " #noguwlnnhj .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
-                            " #noguwlnnhj .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
+                            "#tzkgjbujru p { margin: 0 !important; padding: 0 !important; }\n",
+                            " #tzkgjbujru .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
+                            " #tzkgjbujru .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
+                            " #tzkgjbujru .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
+                            " #tzkgjbujru .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
+                            " #tzkgjbujru .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #tzkgjbujru .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #tzkgjbujru .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #tzkgjbujru .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
+                            " #tzkgjbujru .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
+                            " #tzkgjbujru .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
+                            " #tzkgjbujru .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
+                            " #tzkgjbujru .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
+                            " #tzkgjbujru .gt_spanner_row { border-bottom-style: hidden !important; }\n",
+                            " #tzkgjbujru .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
+                            " #tzkgjbujru .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
+                            " #tzkgjbujru .gt_from_md> :first-child { margin-top: 0 !important; }\n",
+                            " #tzkgjbujru .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
+                            " #tzkgjbujru .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
+                            " #tzkgjbujru .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
+                            " #tzkgjbujru .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
+                            " #tzkgjbujru .gt_row_group_first td { border-top-width: 2px !important; }\n",
+                            " #tzkgjbujru .gt_row_group_first th { border-top-width: 2px !important; }\n",
+                            " #tzkgjbujru .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #tzkgjbujru .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #tzkgjbujru .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
+                            " #tzkgjbujru .gt_left { text-align: left !important; }\n",
+                            " #tzkgjbujru .gt_center { text-align: center !important; }\n",
+                            " #tzkgjbujru .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
+                            " #tzkgjbujru .gt_font_normal { font-weight: normal !important; }\n",
+                            " #tzkgjbujru .gt_font_bold { font-weight: bold !important; }\n",
+                            " #tzkgjbujru .gt_font_italic { font-style: italic !important; }\n",
+                            " #tzkgjbujru .gt_super { font-size: 65% !important; }\n",
+                            " #tzkgjbujru .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
+                            " #tzkgjbujru .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
                             " \n",
                             "</style>\n",
                             "<table class=\"gt_table\" data-quarto-disable-processing=\"false\" data-quarto-bootstrap=\"false\">\n",
                             "\n",
                             "<tr class=\"gt_col_headings\">\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_left\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"column\">column</th>\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_center\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"non_null_cnt\">non_null_cnt</th>\n",
@@ -152,124 +154,125 @@
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_center\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"histogram\">histogram</th>\n",
                             "</tr>\n",
                             "<tbody class=\"gt_table_body\">\n",
                             "<tr>\n",
                             "  <th class=\"gt_row gt_left gt_stub\">uniform_1</th>\n",
                             "  <td class=\"gt_row gt_center\">100000</td>\n",
                             "  <td class=\"gt_row gt_right\">0.00%</td>\n",
-                            "  <td class=\"gt_row gt_right\">5.990</td>\n",
+                            "  <td class=\"gt_row gt_right\">6.016</td>\n",
                             "  <td class=\"gt_row gt_right\">3.465</td>\n",
                             "  <td class=\"gt_row gt_right\">0.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">2.998</td>\n",
-                            "  <td class=\"gt_row gt_right\">5.980</td>\n",
-                            "  <td class=\"gt_row gt_right\">8.983</td>\n",
+                            "  <td class=\"gt_row gt_right\">3.024</td>\n",
+                            "  <td class=\"gt_row gt_right\">6.030</td>\n",
+                            "  <td class=\"gt_row gt_right\">9.028</td>\n",
                             "  <td class=\"gt_row gt_right\">12.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">5.985</td>\n",
+                            "  <td class=\"gt_row gt_right\">6.004</td>\n",
                             "  <td class=\"gt_row gt_center\">0</td>\n",
-                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"17.412474257134456\" width=\"40\" height=\"97.58752574286555\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"17.736098852603707\" width=\"40\" height=\"97.2639011473963\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"17.118270079435124\" width=\"40\" height=\"97.88172992056488\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"15.191232715504563\" width=\"40\" height=\"99.80876728449543\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"17.01529861724037\" width=\"40\" height=\"97.98470138275962\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"16.117975875257425\" width=\"40\" height=\"98.88202412474257\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"16.059135039717564\" width=\"40\" height=\"98.94086496028244\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"19.574874963224474\" width=\"40\" height=\"95.42512503677553\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"15.823771697558106\" width=\"40\" height=\"99.1762283024419\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"17.14769049720506\" width=\"40\" height=\"97.85230950279494\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"18.19211532803766\" width=\"40\" height=\"96.80788467196234\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"18.92762577228597\" width=\"40\" height=\"96.07237422771402\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"15.456016475433952\" width=\"40\" height=\"99.54398352456604\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"17.20653133274492\" width=\"40\" height=\"97.79346866725508\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">6.80K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.63K</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.80K</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.61K</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.65K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.78K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.66K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.72K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.73K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.49K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.74K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.65K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.58K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.53K</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.77K</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.65K</text></g></svg></div></td>\n",
+                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"19.027533684827176\" width=\"40\" height=\"95.97246631517282\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"16.098418277680135\" width=\"40\" height=\"98.90158172231986\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"18.09021675454013\" width=\"40\" height=\"96.90978324545986\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"20.653192735793787\" width=\"40\" height=\"94.3468072642062\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"17.460456942003518\" width=\"40\" height=\"97.53954305799648\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"18.13415348564734\" width=\"40\" height=\"96.86584651435265\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"17.094317516110134\" width=\"40\" height=\"97.90568248388986\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"17.489748096074983\" width=\"40\" height=\"97.51025190392502\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"18.80785002929115\" width=\"40\" height=\"96.19214997070885\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"17.343292325717638\" width=\"40\" height=\"97.65670767428236\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"16.11306385471588\" width=\"40\" height=\"98.88693614528412\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"15.849443468072641\" width=\"40\" height=\"99.15055653192736\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"15.263620386643238\" width=\"40\" height=\"99.73637961335676\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"18.016988869361448\" width=\"40\" height=\"96.98301113063854\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">6.83K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.55K</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.75K</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.62K</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.44K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.83K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.66K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.61K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.68K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.66K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.57K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.67K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.75K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.77K</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.81K</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.62K</text></g></svg></div></td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th class=\"gt_row gt_left gt_stub\">uniform_2</th>\n",
                             "  <td class=\"gt_row gt_center\">100000</td>\n",
                             "  <td class=\"gt_row gt_right\">0.00%</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.501</td>\n",
+                            "  <td class=\"gt_row gt_right\">0.502</td>\n",
                             "  <td class=\"gt_row gt_right\">0.289</td>\n",
                             "  <td class=\"gt_row gt_right\">0.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.250</td>\n",
+                            "  <td class=\"gt_row gt_right\">0.253</td>\n",
                             "  <td class=\"gt_row gt_right\">0.500</td>\n",
                             "  <td class=\"gt_row gt_right\">0.752</td>\n",
                             "  <td class=\"gt_row gt_right\">1.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.501</td>\n",
+                            "  <td class=\"gt_row gt_right\">0.500</td>\n",
                             "  <td class=\"gt_row gt_center\">0</td>\n",
-                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"17.51256281407035\" width=\"40\" height=\"97.48743718592965\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"16.078924031924323\" width=\"40\" height=\"98.92107596807568\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"16.788353532367726\" width=\"40\" height=\"98.21164646763228\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"15.857227313035768\" width=\"40\" height=\"99.14277268696424\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"17.37954478273722\" width=\"40\" height=\"97.62045521726279\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"16.241501625775943\" width=\"40\" height=\"98.75849837422406\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"17.14306828258942\" width=\"40\" height=\"97.85693171741057\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"16.655335501034582\" width=\"40\" height=\"98.34466449896541\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"18.029855158143658\" width=\"40\" height=\"96.97014484185634\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"16.714454626071536\" width=\"40\" height=\"98.28554537392847\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"16.448418563405262\" width=\"40\" height=\"98.55158143659474\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"15.325155187703219\" width=\"40\" height=\"99.67484481229678\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"15.73898906296187\" width=\"40\" height=\"99.26101093703812\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"16.1084835944428\" width=\"40\" height=\"98.8915164055572\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">6.77K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.60K</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.69K</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.64K</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.71K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.60K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.68K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.62K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.77K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.65K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.56K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.65K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.67K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.74K</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.72K</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.69K</text></g></svg></div></td>\n",
+                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"18.096830473974986\" width=\"40\" height=\"96.90316952602501\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"20.946496074440244\" width=\"40\" height=\"94.05350392555975\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"17.71881360860715\" width=\"40\" height=\"97.28118639139285\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"20.030532131433553\" width=\"40\" height=\"94.96946786856645\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"18.111369584181446\" width=\"40\" height=\"96.88863041581855\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"18.44576911892992\" width=\"40\" height=\"96.55423088107008\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"19.347193951730155\" width=\"40\" height=\"95.65280604826984\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"17.77697004943297\" width=\"40\" height=\"97.22302995056702\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"17.47164873509741\" width=\"40\" height=\"97.5283512649026\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"17.544344286129686\" width=\"40\" height=\"97.45565571387031\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"16.817388775806915\" width=\"40\" height=\"98.18261122419308\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"17.00639720849084\" width=\"40\" height=\"97.99360279150916\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"17.558883396336142\" width=\"40\" height=\"97.44111660366386\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"19.21634195987206\" width=\"40\" height=\"95.78365804012793\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">6.88K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.66K</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.47K</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.69K</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.53K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.66K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.64K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.58K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.69K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.71K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.70K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.75K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.74K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.70K</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.88K</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.59K</text></g></svg></div></td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th class=\"gt_row gt_left gt_stub\">exp</th>\n",
                             "  <td class=\"gt_row gt_center\">100000</td>\n",
                             "  <td class=\"gt_row gt_right\">0.00%</td>\n",
-                            "  <td class=\"gt_row gt_right\">1.990</td>\n",
-                            "  <td class=\"gt_row gt_right\">1.985</td>\n",
+                            "  <td class=\"gt_row gt_right\">2.007</td>\n",
+                            "  <td class=\"gt_row gt_right\">2.004</td>\n",
                             "  <td class=\"gt_row gt_right\">0.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.576</td>\n",
-                            "  <td class=\"gt_row gt_right\">1.380</td>\n",
-                            "  <td class=\"gt_row gt_right\">2.757</td>\n",
-                            "  <td class=\"gt_row gt_right\">22.454</td>\n",
-                            "  <td class=\"gt_row gt_right\">2.181</td>\n",
-                            "  <td class=\"gt_row gt_center\">4786</td>\n",
-                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"67.60534147127396\" width=\"40\" height=\"47.39465852872604\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"92.68826885531777\" width=\"40\" height=\"22.311731144682227\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"104.42699546979547\" width=\"40\" height=\"10.573004530204528\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"110.0925943476695\" width=\"40\" height=\"4.907405652330496\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"112.71025645885854\" width=\"40\" height=\"2.289743541141462\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"113.90820175521732\" width=\"40\" height=\"1.0917982447826802\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"114.48632408969425\" width=\"40\" height=\"0.51367591030575\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"114.74031882025133\" width=\"40\" height=\"0.259681179748668\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"114.89195746536005\" width=\"40\" height=\"0.1080425346399494\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"114.94124002502038\" width=\"40\" height=\"0.0587599749796226\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"114.98104516936141\" width=\"40\" height=\"0.018954830638591602\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"114.9905225846807\" width=\"40\" height=\"0.009477415319295801\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"114.99431355080843\" width=\"40\" height=\"0.005686449191571796\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"114.99431355080843\" width=\"40\" height=\"0.005686449191571796\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">52.8K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">52.8K</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">25.0K</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">11.8K</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5.58K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2.59K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">1.21K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">576</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">271</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">137</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">57</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">31</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">10</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">3</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">3</text></g></svg></div></td>\n",
+                            "  <td class=\"gt_row gt_right\">0.578</td>\n",
+                            "  <td class=\"gt_row gt_right\">1.390</td>\n",
+                            "  <td class=\"gt_row gt_right\">2.787</td>\n",
+                            "  <td class=\"gt_row gt_right\">23.544</td>\n",
+                            "  <td class=\"gt_row gt_right\">2.209</td>\n",
+                            "  <td class=\"gt_row gt_center\">4825</td>\n",
+                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"69.68272944638588\" width=\"40\" height=\"45.31727055361412\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"94.06014346146773\" width=\"40\" height=\"20.93985653853227\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"105.42670590399116\" width=\"40\" height=\"9.573294096008837\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"110.55637299981608\" width=\"40\" height=\"4.443627000183923\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"112.96211145852493\" width=\"40\" height=\"2.03788854147507\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"114.11899944822513\" width=\"40\" height=\"0.8810005517748749\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"114.60823983814603\" width=\"40\" height=\"0.39176016185396634\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"114.81239654221078\" width=\"40\" height=\"0.18760345778922272\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"114.91723376862241\" width=\"40\" height=\"0.08276623137759032\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"114.96137575869045\" width=\"40\" height=\"0.03862424130954878\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"114.98160750413831\" width=\"40\" height=\"0.018392495861689895\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"114.9944822512415\" width=\"40\" height=\"0.0055177487585069684\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"114.99632150082766\" width=\"40\" height=\"0.003678499172337979\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"114.99632150082766\" width=\"40\" height=\"0.003678499172337979\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">54.4K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">54.4K</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">24.6K</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">11.4K</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5.20K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2.42K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">1.11K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">479</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">213</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">102</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">45</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">21</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">10</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">3</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2</text></g></svg></div></td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th class=\"gt_row gt_left gt_stub\">normal</th>\n",
                             "  <td class=\"gt_row gt_center\">100000</td>\n",
                             "  <td class=\"gt_row gt_right\">0.00%</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">1.001</td>\n",
-                            "  <td class=\"gt_row gt_right\">\u22124.519</td>\n",
-                            "  <td class=\"gt_row gt_right\">\u22120.676</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.000</td>\n",
-                            "  <td class=\"gt_row gt_right\">0.673</td>\n",
-                            "  <td class=\"gt_row gt_right\">4.451</td>\n",
-                            "  <td class=\"gt_row gt_right\">1.349</td>\n",
-                            "  <td class=\"gt_row gt_center\">711</td>\n",
-                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"114.97453634936129\" width=\"40\" height=\"0.02546365063871292\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"114.83448627084837\" width=\"40\" height=\"0.16551372915162688\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"113.87111148835038\" width=\"40\" height=\"1.1288885116496203\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"109.20701947969275\" width=\"40\" height=\"5.792980520307253\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"95.56274667911556\" width=\"40\" height=\"19.437253320884437\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"66.99253066247931\" width=\"40\" height=\"48.00746933752069\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"32.70572507745194\" width=\"40\" height=\"82.29427492254806\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"29.751941603361207\" width=\"40\" height=\"85.2480583966388\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"63.21966642617663\" width=\"40\" height=\"51.78033357382337\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"93.12672410134533\" width=\"40\" height=\"21.87327589865467\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"108.13330221109366\" width=\"40\" height=\"6.866697788906336\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"113.44247336926537\" width=\"40\" height=\"1.5575266307346283\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"114.80477867843653\" width=\"40\" height=\"0.19522132156346572\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"114.9787802911344\" width=\"40\" height=\"0.021219708865601206\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">23.6K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">39</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">266</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">1.36K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">4.58K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">11.3K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">19.4K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">23.6K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">20.1K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">12.2K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5.15K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">1.62K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">367</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">46</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5</text></g></svg></div></td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22120.004</td>\n",
+                            "  <td class=\"gt_row gt_right\">1.000</td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22123.991</td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22120.681</td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22120.010</td>\n",
+                            "  <td class=\"gt_row gt_right\">0.674</td>\n",
+                            "  <td class=\"gt_row gt_right\">4.671</td>\n",
+                            "  <td class=\"gt_row gt_right\">1.355</td>\n",
+                            "  <td class=\"gt_row gt_center\">710</td>\n",
+                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"114.86943406420242\" width=\"40\" height=\"0.13056593579757703\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"114.03651343928685\" width=\"40\" height=\"0.9634865607131502\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"110.73634685516186\" width=\"40\" height=\"4.263653144838145\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"99.63374003871955\" width=\"40\" height=\"15.366259961280448\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"74.72265994327135\" width=\"40\" height=\"40.27734005672865\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"40.622439331862594\" width=\"40\" height=\"74.3775606681374\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"19.14659402998514\" width=\"40\" height=\"95.85340597001486\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"46.835576966368016\" width=\"40\" height=\"68.16442303363198\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"80.67466570618163\" width=\"40\" height=\"34.32533429381837\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"102.55571563639639\" width=\"40\" height=\"12.444284363603614\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"111.6593129530413\" width=\"40\" height=\"3.340687046958706\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"114.39219305749404\" width=\"40\" height=\"0.6078069425059596\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"114.89644770609158\" width=\"40\" height=\"0.10355229390842169\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"114.99099545270361\" width=\"40\" height=\"0.009004547296385113\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">22.2K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">29</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">214</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">947</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">3.41K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">8.95K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">16.5K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">22.2K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">21.3K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">15.1K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">7.62K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2.76K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">742</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">135</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">23</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2</text></g></svg></div></td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th class=\"gt_row gt_left gt_stub\">fat_normal</th>\n",
                             "  <td class=\"gt_row gt_center\">100000</td>\n",
                             "  <td class=\"gt_row gt_right\">0.00%</td>\n",
-                            "  <td class=\"gt_row gt_right\">1.056</td>\n",
-                            "  <td class=\"gt_row gt_right\">1,000.689</td>\n",
-                            "  <td class=\"gt_row gt_right\">\u22124,102.369</td>\n",
-                            "  <td class=\"gt_row gt_right\">\u2212674.466</td>\n",
-                            "  <td class=\"gt_row gt_right\">2.550</td>\n",
-                            "  <td class=\"gt_row gt_right\">675.878</td>\n",
-                            "  <td class=\"gt_row gt_right\">4,061.315</td>\n",
-                            "  <td class=\"gt_row gt_right\">1,350.344</td>\n",
-                            "  <td class=\"gt_row gt_center\">711</td>\n",
-                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"114.92009025101062\" width=\"40\" height=\"0.07990974898937964\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"114.3983265958447\" width=\"40\" height=\"0.6016734041553065\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"112.43348688540003\" width=\"40\" height=\"2.566513114599971\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"105.73516969070226\" width=\"40\" height=\"9.264830309297736\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"88.43235874776724\" width=\"40\" height=\"26.56764125223276\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"59.25119864623485\" width=\"40\" height=\"55.74880135376515\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"28.537651593494402\" width=\"40\" height=\"86.4623484065056\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"26.49290213406036\" width=\"40\" height=\"88.50709786593964\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"57.15004230516123\" width=\"40\" height=\"57.84995769483877\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"86.58033280060168\" width=\"40\" height=\"28.41966719939832\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"104.68224123343049\" width=\"40\" height=\"10.317758766569511\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"112.04803986086303\" width=\"40\" height=\"2.951960139136972\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"114.43123061013443\" width=\"40\" height=\"0.5687693898655652\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"114.84958164896118\" width=\"40\" height=\"0.15041835103882306\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">21.3K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">17</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">128</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">546</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">1.97K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5.65K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">11.9K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">18.4K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">21.3K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">18.8K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">12.3K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">6.05K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2.19K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">628</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">121</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">32</text></g></svg></div></td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22122.638</td>\n",
+                            "  <td class=\"gt_row gt_right\">1,000.913</td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22124,180.218</td>\n",
+                            "  <td class=\"gt_row gt_right\">\u2212679.219</td>\n",
+                            "  <td class=\"gt_row gt_right\">\u22121.040</td>\n",
+                            "  <td class=\"gt_row gt_right\">675.313</td>\n",
+                            "  <td class=\"gt_row gt_right\">4,250.217</td>\n",
+                            "  <td class=\"gt_row gt_right\">1,354.532</td>\n",
+                            "  <td class=\"gt_row gt_center\">661</td>\n",
+                            "  <td class=\"gt_row gt_center\"><div><svg role=\"img\" viewBox=\"0 0 850 130\" style=\"height: 2em; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;\"><defs><pattern id=\"area_pattern\" width=\"8\" height=\"8\" patternUnits=\"userSpaceOnUse\"><path class=\"pattern-line\" d=\"M 0,8 l 8,-8 M -1,1 l 4,-4 M 6,10 l 4,-4\" stroke=\"#FF0000\" stroke-width=\"1.5\" stroke-linecap=\"round\" shape-rendering=\"geometricPrecision\"></path></pattern></defs><style> text { font-family: ui-monospace, 'Cascadia Code', 'Source Code Pro', Menlo, Consolas, 'DejaVu Sans Mono', monospace; stroke-width: 0.15em; paint-order: stroke; stroke-linejoin: round; cursor: default; } .vert-line:hover rect { fill: #911EB4; fill-opacity: 40%; stroke: #FFFFFF60; color: red; } .vert-line:hover text { stroke: white; fill: #212427; } .horizontal-line:hover text {stroke: white; fill: #212427; } .ref-line:hover rect { stroke: #FFFFFF60; } .ref-line:hover line { stroke: #FF0000; } .ref-line:hover text { stroke: white; fill: #212427; } .y-axis-line:hover rect { fill: #EDEDED; fill-opacity: 60%; stroke: #FFFFFF60; color: red; } .y-axis-line:hover text { stroke: white; stroke-width: 0.20em; fill: #1A1C1F; } </style><line x1=\"22.5\" y1=\"115.0\" x2=\"827.5\" y2=\"115.0\" stroke=\"#BFBFBF\" stroke-width=\"4\"></line><rect x=\"30.0\" y=\"114.92277290691864\" width=\"40\" height=\"0.07722709308136189\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"83.57142857142857\" y=\"114.57297960296188\" width=\"40\" height=\"0.42702039703812034\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"137.14285714285714\" y=\"112.65593058647163\" width=\"40\" height=\"2.3440694135283735\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"190.7142857142857\" y=\"105.6782355880616\" width=\"40\" height=\"9.321764411938403\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"244.28571428571428\" y=\"88.2794257938491\" width=\"40\" height=\"26.7205742061509\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"297.85714285714283\" y=\"58.065461318311904\" width=\"40\" height=\"56.934538681688096\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"351.4285714285714\" y=\"26.81120247126698\" width=\"40\" height=\"88.18879752873302\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"405.0\" y=\"15.0\" width=\"40\" height=\"100.0\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"458.57142857142856\" y=\"31.090491982010636\" width=\"40\" height=\"83.90950801798937\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"512.1428571428571\" y=\"62.44923454322446\" width=\"40\" height=\"52.55076545677554\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"565.7142857142857\" y=\"91.518420933085\" width=\"40\" height=\"23.481579066915003\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"619.2857142857142\" y=\"107.06378049334484\" width=\"40\" height=\"7.9362195066551635\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"672.8571428571428\" y=\"113.01480943079089\" width=\"40\" height=\"1.9851905692091094\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"726.4285714285713\" y=\"114.645663925862\" width=\"40\" height=\"0.35433607413800416\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><rect x=\"780.0\" y=\"114.95457229818744\" width=\"40\" height=\"0.04542770181255662\" stroke=\"#3290CC\" stroke-width=\"4\" fill=\"#3FB5FF\"></rect><g class=\"y-axis-line\"><rect x=\"0\" y=\"0\" width=\"65\" height=\"130\" stroke=\"transparent\" stroke-width=\"0\" fill=\"transparent\"></rect><text x=\"0\" y=\"19.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">22.0K</text><text x=\"0\" y=\"126.0\" fill=\"transparent\" stroke=\"transparent\" font-size=\"25\">0</text></g><g class=\"vert-line\"><rect x=\"40.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"60.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">17</text></g><g class=\"vert-line\"><rect x=\"93.57142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"113.57142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">94</text></g><g class=\"vert-line\"><rect x=\"147.14285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"167.14285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">516</text></g><g class=\"vert-line\"><rect x=\"200.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"220.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">2.05K</text></g><g class=\"vert-line\"><rect x=\"254.28571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"274.2857142857143\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5.88K</text></g><g class=\"vert-line\"><rect x=\"307.85714285714283\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"327.85714285714283\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">12.5K</text></g><g class=\"vert-line\"><rect x=\"361.4285714285714\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"381.4285714285714\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">19.4K</text></g><g class=\"vert-line\"><rect x=\"415.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"435.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">22.0K</text></g><g class=\"vert-line\"><rect x=\"468.57142857142856\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"488.57142857142856\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">18.5K</text></g><g class=\"vert-line\"><rect x=\"522.1428571428571\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"542.1428571428571\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">11.6K</text></g><g class=\"vert-line\"><rect x=\"575.7142857142857\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"595.7142857142857\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">5.17K</text></g><g class=\"vert-line\"><rect x=\"629.2857142857142\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"649.2857142857142\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">1.75K</text></g><g class=\"vert-line\"><rect x=\"682.8571428571428\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"702.8571428571428\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">437</text></g><g class=\"vert-line\"><rect x=\"736.4285714285713\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"756.4285714285713\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">78</text></g><g class=\"vert-line\"><rect x=\"790.0\" y=\"0\" width=\"20\" height=\"130\" stroke=\"transparent\" stroke-width=\"12\" fill=\"transparent\"></rect><text x=\"810.0\" y=\"20\" fill=\"transparent\" stroke=\"transparent\" font-size=\"30px\">10</text></g></svg></div></td>\n",
                             "</tr>\n",
                             "</tbody>\n",
                             "\n",
                             "\n",
                             "</table>\n",
                             "\n",
                             "</div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "GT(_tbl_data=shape: (5, 13)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 column     \u2506 non_null_c \u2506 null% \u2506 mean     \u2506 \u2026 \u2506 max        \u2506 IQR        \u2506 outlier_c \u2506 histogram \u2502\n",
-                            "\u2502 ---        \u2506 nt         \u2506 ---   \u2506 ---      \u2506   \u2506 ---        \u2506 ---        \u2506 nt        \u2506 ---       \u2502\n",
-                            "\u2502 str        \u2506 ---        \u2506 f64   \u2506 f64      \u2506   \u2506 f64        \u2506 f64        \u2506 ---       \u2506 struct[1] \u2502\n",
-                            "\u2502            \u2506 u32        \u2506       \u2506          \u2506   \u2506            \u2506            \u2506 u32       \u2506           \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 uniform_1  \u2506 100000     \u2506 0.0   \u2506 5.990448 \u2506 \u2026 \u2506 11.999961  \u2506 5.985282   \u2506 0         \u2506 {[6634,   \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 6798, \u2026   \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 6648]}    \u2502\n",
-                            "\u2502 uniform_2  \u2506 100000     \u2506 0.0   \u2506 0.50083  \u2506 \u2026 \u2506 1.0        \u2506 0.501454   \u2506 0         \u2506 {[6596,   \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 6693, \u2026   \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 6691]}    \u2502\n",
-                            "\u2502 exp        \u2506 100000     \u2506 0.0   \u2506 1.98982  \u2506 \u2026 \u2506 22.454359  \u2506 2.180683   \u2506 4786      \u2506 {[52757,  \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 25004, \u2026  \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 3]}       \u2502\n",
-                            "\u2502 normal     \u2506 100000     \u2506 0.0   \u2506 0.000112 \u2506 \u2026 \u2506 4.451234   \u2506 1.349317   \u2506 711       \u2506 {[6, 39,  \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 \u2026 5]}     \u2502\n",
-                            "\u2502 fat_normal \u2506 100000     \u2506 0.0   \u2506 1.055753 \u2506 \u2026 \u2506 4061.31530 \u2506 1350.34389 \u2506 711       \u2506 {[17,     \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506 1          \u2506            \u2506           \u2506 128, \u2026    \u2502\n",
-                            "\u2502            \u2506            \u2506       \u2506          \u2506   \u2506            \u2506            \u2506           \u2506 32]}      \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7ebd4f51f290>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.stub: 2>, column_label='column', column_align='left', column_width=None), ColInfo(var='non_null_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='non_null_cnt', column_align='center', column_width=None), ColInfo(var='null%', type=<ColInfoTypeEnum.default: 1>, column_label='null%', column_align='right', column_width=None), ColInfo(var='mean', type=<ColInfoTypeEnum.default: 1>, column_label='mean', column_align='right', column_width=None), ColInfo(var='std', type=<ColInfoTypeEnum.default: 1>, column_label='std', column_align='right', column_width=None), ColInfo(var='min', type=<ColInfoTypeEnum.default: 1>, column_label='min', column_align='right', column_width=None), ColInfo(var='q1', type=<ColInfoTypeEnum.default: 1>, column_label='q1', column_align='right', column_width=None), ColInfo(var='median', type=<ColInfoTypeEnum.default: 1>, column_label='median', column_align='right', column_width=None), ColInfo(var='q3', type=<ColInfoTypeEnum.default: 1>, column_label='q3', column_align='right', column_width=None), ColInfo(var='max', type=<ColInfoTypeEnum.default: 1>, column_label='max', column_align='right', column_width=None), ColInfo(var='IQR', type=<ColInfoTypeEnum.default: 1>, column_label='IQR', column_align='right', column_width=None), ColInfo(var='outlier_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='outlier_cnt', column_align='center', column_width=None), ColInfo(var='histogram', type=<ColInfoTypeEnum.default: 1>, column_label='histogram', column_align='center', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname='uniform_1', group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname='uniform_2', group_label=None, built=False), RowInfo(rownum_i=2, group_id=None, rowname='exp', group_label=None, built=False), RowInfo(rownum_i=3, group_id=None, rowname='normal', group_label=None, built=False), RowInfo(rownum_i=4, group_id=None, rowname='fat_normal', group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead='column', _source_notes=[], _footnotes=[], _styles=[], _locale=<great_tables._gt_data.Locale object at 0x7ebd177cdf50>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7ebd2f355810>, <great_tables._gt_data.FormatInfo object at 0x7ebd17784290>, <great_tables._gt_data.FormatInfo object at 0x7ebd1e7d90d0>], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 column     \u2506 non_null_c \u2506 null% \u2506 mean      \u2506 \u2026 \u2506 max        \u2506 IQR       \u2506 outlier_c \u2506 histogram \u2502\n",
+                            "\u2502 ---        \u2506 nt         \u2506 ---   \u2506 ---       \u2506   \u2506 ---        \u2506 ---       \u2506 nt        \u2506 ---       \u2502\n",
+                            "\u2502 str        \u2506 ---        \u2506 f64   \u2506 f64       \u2506   \u2506 f64        \u2506 f64       \u2506 ---       \u2506 struct[1] \u2502\n",
+                            "\u2502            \u2506 u32        \u2506       \u2506           \u2506   \u2506            \u2506           \u2506 u32       \u2506           \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 uniform_1  \u2506 100000     \u2506 0.0   \u2506 6.016376  \u2506 \u2026 \u2506 11.999955  \u2506 6.003771  \u2506 0         \u2506 {[6553,   \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 6753, \u2026   \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 6622]}    \u2502\n",
+                            "\u2502 uniform_2  \u2506 100000     \u2506 0.0   \u2506 0.502327  \u2506 \u2026 \u2506 0.999982   \u2506 0.49965   \u2506 0         \u2506 {[6665,   \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 6469, \u2026   \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 6588]}    \u2502\n",
+                            "\u2502 exp        \u2506 100000     \u2506 0.0   \u2506 2.007269  \u2506 \u2026 \u2506 23.544025  \u2506 2.208975  \u2506 4825      \u2506 {[54370,  \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 24639, \u2026  \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 2]}       \u2502\n",
+                            "\u2502 normal     \u2506 100000     \u2506 0.0   \u2506 -0.00395  \u2506 \u2026 \u2506 4.67116    \u2506 1.355211  \u2506 710       \u2506 {[29,     \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 214, \u2026    \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506            \u2506           \u2506           \u2506 2]}       \u2502\n",
+                            "\u2502 fat_normal \u2506 100000     \u2506 0.0   \u2506 -2.638463 \u2506 \u2026 \u2506 4250.21731 \u2506 1354.5317 \u2506 661       \u2506 {[17, 94, \u2502\n",
+                            "\u2502            \u2506            \u2506       \u2506           \u2506   \u2506 1          \u2506 23        \u2506           \u2506 \u2026 10]}    \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7839f002e7d0>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.stub: 2>, column_label='column', column_align='left', column_width=None), ColInfo(var='non_null_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='non_null_cnt', column_align='center', column_width=None), ColInfo(var='null%', type=<ColInfoTypeEnum.default: 1>, column_label='null%', column_align='right', column_width=None), ColInfo(var='mean', type=<ColInfoTypeEnum.default: 1>, column_label='mean', column_align='right', column_width=None), ColInfo(var='std', type=<ColInfoTypeEnum.default: 1>, column_label='std', column_align='right', column_width=None), ColInfo(var='min', type=<ColInfoTypeEnum.default: 1>, column_label='min', column_align='right', column_width=None), ColInfo(var='q1', type=<ColInfoTypeEnum.default: 1>, column_label='q1', column_align='right', column_width=None), ColInfo(var='median', type=<ColInfoTypeEnum.default: 1>, column_label='median', column_align='right', column_width=None), ColInfo(var='q3', type=<ColInfoTypeEnum.default: 1>, column_label='q3', column_align='right', column_width=None), ColInfo(var='max', type=<ColInfoTypeEnum.default: 1>, column_label='max', column_align='right', column_width=None), ColInfo(var='IQR', type=<ColInfoTypeEnum.default: 1>, column_label='IQR', column_align='right', column_width=None), ColInfo(var='outlier_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='outlier_cnt', column_align='center', column_width=None), ColInfo(var='histogram', type=<ColInfoTypeEnum.default: 1>, column_label='histogram', column_align='center', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname='uniform_1', group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname='uniform_2', group_label=None, built=False), RowInfo(rownum_i=2, group_id=None, rowname='exp', group_label=None, built=False), RowInfo(rownum_i=3, group_id=None, rowname='normal', group_label=None, built=False), RowInfo(rownum_i=4, group_id=None, rowname='fat_normal', group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead='column', _source_notes=[], _footnotes=[], _styles=[], _locale=<great_tables._gt_data.Locale object at 0x7839eabf2c10>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7839e8d15950>, <great_tables._gt_data.FormatInfo object at 0x7839e806ec10>, <great_tables._gt_data.FormatInfo object at 0x7839e806fe90>], _substitutions=[], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "# Only shows for numerical columns \n",
                 "dia.numeric_profile(n_bins=15)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
@@ -280,57 +283,115 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (10, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x</th><th>y</th><th>corr</th></tr><tr><td>str</td><td>str</td><td>f64</td></tr></thead><tbody><tr><td>&quot;exp&quot;</td><td>&quot;fat_normal&quot;</td><td>0.007474</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;exp&quot;</td><td>0.007295</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;normal&quot;</td><td>-0.007233</td></tr><tr><td>&quot;exp&quot;</td><td>&quot;normal&quot;</td><td>-0.00411</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;uniform_2&quot;</td><td>-0.001841</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;fat_normal&quot;</td><td>0.001837</td></tr><tr><td>&quot;uniform_2&quot;</td><td>&quot;fat_normal&quot;</td><td>-0.00146</td></tr><tr><td>&quot;uniform_2&quot;</td><td>&quot;normal&quot;</td><td>0.001047</td></tr><tr><td>&quot;uniform_2&quot;</td><td>&quot;exp&quot;</td><td>-0.000907</td></tr><tr><td>&quot;normal&quot;</td><td>&quot;fat_normal&quot;</td><td>0.00077</td></tr></tbody></table></div>"
+                            "<small>shape: (10, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>x</th><th>y</th><th>corr</th></tr><tr><td>str</td><td>str</td><td>f64</td></tr></thead><tbody><tr><td>&quot;exp&quot;</td><td>&quot;fat_normal&quot;</td><td>0.006503</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;fat_normal&quot;</td><td>0.005486</td></tr><tr><td>&quot;normal&quot;</td><td>&quot;fat_normal&quot;</td><td>-0.002918</td></tr><tr><td>&quot;uniform_2&quot;</td><td>&quot;fat_normal&quot;</td><td>0.002199</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;uniform_2&quot;</td><td>-0.001753</td></tr><tr><td>&quot;uniform_2&quot;</td><td>&quot;exp&quot;</td><td>-0.001631</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;normal&quot;</td><td>0.001608</td></tr><tr><td>&quot;exp&quot;</td><td>&quot;normal&quot;</td><td>-0.001274</td></tr><tr><td>&quot;uniform_2&quot;</td><td>&quot;normal&quot;</td><td>-0.001158</td></tr><tr><td>&quot;uniform_1&quot;</td><td>&quot;exp&quot;</td><td>0.000366</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (10, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 x         \u2506 y          \u2506 corr      \u2502\n",
                             "\u2502 ---       \u2506 ---        \u2506 ---       \u2502\n",
                             "\u2502 str       \u2506 str        \u2506 f64       \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 exp       \u2506 fat_normal \u2506 0.007474  \u2502\n",
-                            "\u2502 uniform_1 \u2506 exp        \u2506 0.007295  \u2502\n",
-                            "\u2502 uniform_1 \u2506 normal     \u2506 -0.007233 \u2502\n",
-                            "\u2502 exp       \u2506 normal     \u2506 -0.00411  \u2502\n",
-                            "\u2502 uniform_1 \u2506 uniform_2  \u2506 -0.001841 \u2502\n",
-                            "\u2502 uniform_1 \u2506 fat_normal \u2506 0.001837  \u2502\n",
-                            "\u2502 uniform_2 \u2506 fat_normal \u2506 -0.00146  \u2502\n",
-                            "\u2502 uniform_2 \u2506 normal     \u2506 0.001047  \u2502\n",
-                            "\u2502 uniform_2 \u2506 exp        \u2506 -0.000907 \u2502\n",
-                            "\u2502 normal    \u2506 fat_normal \u2506 0.00077   \u2502\n",
+                            "\u2502 exp       \u2506 fat_normal \u2506 0.006503  \u2502\n",
+                            "\u2502 uniform_1 \u2506 fat_normal \u2506 0.005486  \u2502\n",
+                            "\u2502 normal    \u2506 fat_normal \u2506 -0.002918 \u2502\n",
+                            "\u2502 uniform_2 \u2506 fat_normal \u2506 0.002199  \u2502\n",
+                            "\u2502 uniform_1 \u2506 uniform_2  \u2506 -0.001753 \u2502\n",
+                            "\u2502 uniform_2 \u2506 exp        \u2506 -0.001631 \u2502\n",
+                            "\u2502 uniform_1 \u2506 normal     \u2506 0.001608  \u2502\n",
+                            "\u2502 exp       \u2506 normal     \u2506 -0.001274 \u2502\n",
+                            "\u2502 uniform_2 \u2506 normal     \u2506 -0.001158 \u2502\n",
+                            "\u2502 uniform_1 \u2506 exp        \u2506 0.000366  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.infer_corr()"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'numerics': ['uniform_1', 'uniform_2', 'exp', 'normal', 'fat_normal'],\n",
+                            " 'ints': [],\n",
+                            " 'floats': ['uniform_1', 'uniform_2', 'exp', 'normal', 'fat_normal'],\n",
+                            " 'strs': [],\n",
+                            " 'bools': [],\n",
+                            " 'cats': [],\n",
+                            " 'list_floats': ['list_prob'],\n",
+                            " 'list_ints': [],\n",
+                            " 'list_bool': [],\n",
+                            " 'list_str': [],\n",
+                            " 'simple_types': ['uniform_1',\n",
+                            "  'uniform_2',\n",
+                            "  'exp',\n",
+                            "  'normal',\n",
+                            "  'fat_normal',\n",
+                            "  'list_prob'],\n",
+                            " 'other_types': []}"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "dia.meta()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "['uniform_2', 'list_prob']"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Uniform_2 can potentially be a probability score column (e.g. output of predict_proba, but taking values only for class =1)\n",
+                "# list_prob can potentially be a 2-class probability column (e.g. output of predict_proba)\n",
+                "dia.infer_prob()"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Dependency Detection\n",
                 "\n",
                 "Does knowing values in column A tell us values in column B?"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
@@ -358,36 +419,36 @@
                             "\u2502 APPF8027386553 \u2506 Male   \u2506 30/01/89 \u2506 09/07/16       \u2506 \u2026 \u2506 null          \u2506 null \u2506 7    \u2506 0        \u2502\n",
                             "\u2502 7              \u2506        \u2506          \u2506                \u2506   \u2506               \u2506      \u2506      \u2506          \u2502\n",
                             "\u2502 APPG6099443664 \u2506 Male   \u2506 19/04/85 \u2506 20/07/16       \u2506 \u2026 \u2506 null          \u2506 null \u2506 10   \u2506 0        \u2502\n",
                             "\u2502 1              \u2506        \u2506          \u2506                \u2506   \u2506               \u2506      \u2506      \u2506          \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = pl.read_parquet(\"dependency.parquet\")\n",
                 "df.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dia = DIA(df)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "INFO:polars_ds.diagnosis:Running dependency for columns: ['Approved', 'Gender', 'Contacted', 'Primary_Bank_Type', 'City_Category', 'Employer_Category1', 'Employer_Category2', 'Var1', 'Loan_Period', 'Source_Category', 'Source', 'Customer_Existing_Primary_Bank_Code', 'Lead_Creation_Date', 'Loan_Amount', 'City_Code', 'EMI', 'DOB', 'Employer_Code', 'ID'].\n"
@@ -422,386 +483,386 @@
                             "\u2502 City_Code          \u2506 EMI                               \u2506 3.147327     \u2502\n",
                             "\u2502 Lead_Creation_Date \u2506 EMI                               \u2506 3.92818      \u2502\n",
                             "\u2502 Lead_Creation_Date \u2506 City_Code                         \u2506 4.204907     \u2502\n",
                             "\u2502 Lead_Creation_Date \u2506 Loan_Amount                       \u2506 4.336805     \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.infer_dependency()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/svg+xml": [
                             "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
                             "<!-- Generated by graphviz version 10.0.1 (0)\n",
                             " -->\n",
                             "<!-- Title: Dependency Plot Pages: 1 -->\n",
-                            "<svg width=\"2056pt\" height=\"188pt\"\n",
-                            " viewBox=\"0.00 0.00 2056.28 188.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<svg width=\"2022pt\" height=\"188pt\"\n",
+                            " viewBox=\"0.00 0.00 2021.93 188.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
                             "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 184)\">\n",
                             "<title>Dependency Plot</title>\n",
-                            "<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-184 2052.28,-184 2052.28,4 -4,4\"/>\n",
-                            "<!-- Employer_Category2 -->\n",
+                            "<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-184 2017.93,-184 2017.93,4 -4,4\"/>\n",
+                            "<!-- Var1 -->\n",
                             "<g id=\"node1\" class=\"node\">\n",
-                            "<title>Employer_Category2</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"90.76\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"90.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category2</text>\n",
+                            "<title>Var1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"143.76\" cy=\"-90\" rx=\"28.32\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"143.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Var1</text>\n",
                             "</g>\n",
-                            "<!-- Employer_Code -->\n",
+                            "<!-- ID -->\n",
                             "<g id=\"node2\" class=\"node\">\n",
-                            "<title>Employer_Code</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"221.76\" cy=\"-90\" rx=\"71.82\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"221.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Code</text>\n",
+                            "<title>ID</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1129.76\" cy=\"-162\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1129.76\" y=\"-156.95\" font-family=\"Times,serif\" font-size=\"14.00\">ID</text>\n",
                             "</g>\n",
-                            "<!-- Employer_Code&#45;&gt;Employer_Category2 -->\n",
+                            "<!-- ID&#45;&gt;Var1 -->\n",
                             "<g id=\"edge1\" class=\"edge\">\n",
-                            "<title>Employer_Code&#45;&gt;Employer_Category2</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M192.36,-73.29C174.37,-63.68 151.11,-51.25 131.38,-40.7\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"133.23,-37.73 122.76,-36.1 129.93,-43.9 133.23,-37.73\"/>\n",
-                            "</g>\n",
-                            "<!-- Employer_Category1 -->\n",
-                            "<g id=\"node9\" class=\"node\">\n",
-                            "<title>Employer_Category1</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"290.76\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"290.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category1</text>\n",
-                            "</g>\n",
-                            "<!-- Employer_Code&#45;&gt;Employer_Category1 -->\n",
-                            "<g id=\"edge8\" class=\"edge\">\n",
-                            "<title>Employer_Code&#45;&gt;Employer_Category1</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M238.46,-72.05C246.77,-63.63 256.97,-53.28 266.15,-43.97\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"268.62,-46.45 273.15,-36.87 263.64,-41.53 268.62,-46.45\"/>\n",
-                            "</g>\n",
-                            "<!-- DOB -->\n",
-                            "<g id=\"node3\" class=\"node\">\n",
-                            "<title>DOB</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"341.76\" cy=\"-90\" rx=\"30.37\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"341.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">DOB</text>\n",
+                            "<title>ID&#45;&gt;Var1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1102.54,-160.85C966.78,-159.88 362.34,-153.06 180.76,-108 179,-107.56 177.23,-107.05 175.46,-106.47\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"176.79,-103.23 166.2,-102.85 174.24,-109.75 176.79,-103.23\"/>\n",
                             "</g>\n",
-                            "<!-- ID -->\n",
+                            "<!-- Employer_Code -->\n",
                             "<g id=\"node4\" class=\"node\">\n",
-                            "<title>ID</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1124.76\" cy=\"-162\" rx=\"27\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1124.76\" y=\"-156.95\" font-family=\"Times,serif\" font-size=\"14.00\">ID</text>\n",
+                            "<title>Employer_Code</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"261.76\" cy=\"-90\" rx=\"71.82\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"261.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Code</text>\n",
                             "</g>\n",
                             "<!-- ID&#45;&gt;Employer_Code -->\n",
-                            "<g id=\"edge6\" class=\"edge\">\n",
+                            "<g id=\"edge17\" class=\"edge\">\n",
                             "<title>ID&#45;&gt;Employer_Code</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1097.66,-160.65C994.02,-159.03 613.06,-150.35 302.76,-108 296.71,-107.17 290.44,-106.15 284.18,-105.03\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"284.95,-101.61 274.48,-103.18 283.65,-108.49 284.95,-101.61\"/>\n",
-                            "</g>\n",
-                            "<!-- ID&#45;&gt;DOB -->\n",
-                            "<g id=\"edge2\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;DOB</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1097.5,-160.26C980.66,-156.89 521.78,-141.75 381.76,-108 379.62,-107.48 377.44,-106.86 375.26,-106.17\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"376.6,-102.93 366,-102.75 374.17,-109.5 376.6,-102.93\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1102.44,-160.54C1001.26,-158.54 638.49,-148.79 342.76,-108 336.71,-107.17 330.44,-106.14 324.18,-105.01\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"324.96,-101.59 314.48,-103.16 323.65,-108.47 324.96,-101.59\"/>\n",
                             "</g>\n",
                             "<!-- Customer_Existing_Primary_Bank_Code -->\n",
                             "<g id=\"node5\" class=\"node\">\n",
                             "<title>Customer_Existing_Primary_Bank_Code</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"555.76\" cy=\"-90\" rx=\"165.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"555.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Customer_Existing_Primary_Bank_Code</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"516.76\" cy=\"-90\" rx=\"165.48\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"516.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Customer_Existing_Primary_Bank_Code</text>\n",
                             "</g>\n",
                             "<!-- ID&#45;&gt;Customer_Existing_Primary_Bank_Code -->\n",
                             "<g id=\"edge3\" class=\"edge\">\n",
                             "<title>ID&#45;&gt;Customer_Existing_Primary_Bank_Code</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1098.08,-157.72C1023.55,-148.55 809.73,-122.24 673.9,-105.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"674.49,-102.08 664.14,-104.33 673.63,-109.03 674.49,-102.08\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1103.03,-157.95C1023.8,-148.9 786.64,-121.82 639.36,-105\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"639.87,-101.54 629.54,-103.88 639.08,-108.49 639.87,-101.54\"/>\n",
                             "</g>\n",
-                            "<!-- Var1 -->\n",
+                            "<!-- Contacted -->\n",
                             "<g id=\"node6\" class=\"node\">\n",
-                            "<title>Var1</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"767.76\" cy=\"-90\" rx=\"28.32\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"767.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Var1</text>\n",
+                            "<title>Contacted</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"748.76\" cy=\"-90\" rx=\"48.28\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"748.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Contacted</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;Var1 -->\n",
+                            "<!-- ID&#45;&gt;Contacted -->\n",
                             "<g id=\"edge4\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;Var1</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1097.66,-158.96C1041.8,-154.23 910.29,-140.34 804.76,-108 803.16,-107.51 801.53,-106.96 799.9,-106.37\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"801.28,-103.16 790.7,-102.63 798.64,-109.64 801.28,-103.16\"/>\n",
+                            "<title>ID&#45;&gt;Contacted</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1103.08,-157.81C1047.39,-150.89 914.91,-133.1 805.76,-108 802.4,-107.23 798.94,-106.37 795.47,-105.45\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"796.48,-102.1 785.91,-102.81 794.62,-108.85 796.48,-102.1\"/>\n",
+                            "</g>\n",
+                            "<!-- City_Code -->\n",
+                            "<g id=\"node9\" class=\"node\">\n",
+                            "<title>City_Code</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"865.76\" cy=\"-90\" rx=\"50.84\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"865.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Code</text>\n",
+                            "</g>\n",
+                            "<!-- ID&#45;&gt;City_Code -->\n",
+                            "<g id=\"edge11\" class=\"edge\">\n",
+                            "<title>ID&#45;&gt;City_Code</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1104.59,-154.65C1066.03,-144.88 990.03,-125.45 925.76,-108 922.42,-107.09 918.98,-106.15 915.51,-105.19\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"916.49,-101.83 905.91,-102.51 914.6,-108.57 916.49,-101.83\"/>\n",
                             "</g>\n",
                             "<!-- Approved -->\n",
-                            "<g id=\"node8\" class=\"node\">\n",
+                            "<g id=\"node11\" class=\"node\">\n",
                             "<title>Approved</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"861.76\" cy=\"-90\" rx=\"47.77\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"861.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Approved</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"982.76\" cy=\"-90\" rx=\"47.77\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"982.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Approved</text>\n",
                             "</g>\n",
                             "<!-- ID&#45;&gt;Approved -->\n",
-                            "<g id=\"edge7\" class=\"edge\">\n",
+                            "<g id=\"edge8\" class=\"edge\">\n",
                             "<title>ID&#45;&gt;Approved</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1099.63,-154.86C1060.74,-145.29 983.7,-126.03 918.76,-108 915.64,-107.13 912.42,-106.22 909.18,-105.29\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"910.22,-101.95 899.64,-102.51 908.27,-108.67 910.22,-101.95\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1108.07,-150.67C1085.41,-139.88 1049.38,-122.72 1021.76,-109.57\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1023.53,-106.54 1012.99,-105.4 1020.52,-112.86 1023.53,-106.54\"/>\n",
                             "</g>\n",
-                            "<!-- Contacted -->\n",
-                            "<g id=\"node10\" class=\"node\">\n",
-                            "<title>Contacted</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"975.76\" cy=\"-90\" rx=\"48.28\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"975.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Contacted</text>\n",
+                            "<!-- Gender -->\n",
+                            "<g id=\"node12\" class=\"node\">\n",
+                            "<title>Gender</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1086.76\" cy=\"-90\" rx=\"38.04\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1086.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Gender</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;Contacted -->\n",
+                            "<!-- ID&#45;&gt;Gender -->\n",
                             "<g id=\"edge9\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;Contacted</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1103.09,-150.82C1080.12,-140.03 1043.34,-122.75 1015.2,-109.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1016.79,-106.41 1006.25,-105.33 1013.82,-112.75 1016.79,-106.41\"/>\n",
+                            "<title>ID&#45;&gt;Gender</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1119.79,-144.76C1114.76,-136.58 1108.54,-126.45 1102.85,-117.2\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1105.99,-115.61 1097.77,-108.92 1100.02,-119.28 1105.99,-115.61\"/>\n",
+                            "</g>\n",
+                            "<!-- DOB -->\n",
+                            "<g id=\"node13\" class=\"node\">\n",
+                            "<title>DOB</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1172.76\" cy=\"-90\" rx=\"30.37\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1172.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">DOB</text>\n",
+                            "</g>\n",
+                            "<!-- ID&#45;&gt;DOB -->\n",
+                            "<g id=\"edge10\" class=\"edge\">\n",
+                            "<title>ID&#45;&gt;DOB</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1139.73,-144.76C1144.84,-136.46 1151.17,-126.15 1156.92,-116.79\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1159.8,-118.79 1162.05,-108.44 1153.83,-115.13 1159.8,-118.79\"/>\n",
                             "</g>\n",
                             "<!-- Source -->\n",
-                            "<g id=\"node11\" class=\"node\">\n",
+                            "<g id=\"node14\" class=\"node\">\n",
                             "<title>Source</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1078.76\" cy=\"-90\" rx=\"36.51\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1078.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Source</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1257.76\" cy=\"-90\" rx=\"36.51\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1257.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Source</text>\n",
                             "</g>\n",
                             "<!-- ID&#45;&gt;Source -->\n",
-                            "<g id=\"edge10\" class=\"edge\">\n",
+                            "<g id=\"edge12\" class=\"edge\">\n",
                             "<title>ID&#45;&gt;Source</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1114.32,-145.12C1108.81,-136.73 1101.92,-126.24 1095.67,-116.73\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1098.72,-115.01 1090.31,-108.57 1092.87,-118.85 1098.72,-115.01\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1150.33,-149.75C1170.27,-138.85 1200.87,-122.11 1224.32,-109.29\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1225.78,-112.48 1232.88,-104.61 1222.42,-106.34 1225.78,-112.48\"/>\n",
                             "</g>\n",
-                            "<!-- Gender -->\n",
-                            "<g id=\"node12\" class=\"node\">\n",
-                            "<title>Gender</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1171.76\" cy=\"-90\" rx=\"38.04\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1171.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Gender</text>\n",
+                            "<!-- Loan_Period -->\n",
+                            "<g id=\"node15\" class=\"node\">\n",
+                            "<title>Loan_Period</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1370.76\" cy=\"-90\" rx=\"58.52\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1370.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Loan_Period</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;Gender -->\n",
-                            "<g id=\"edge11\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;Gender</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1135.43,-145.12C1141.05,-136.73 1148.1,-126.24 1154.48,-116.73\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1157.3,-118.82 1159.97,-108.56 1151.49,-114.91 1157.3,-118.82\"/>\n",
+                            "<!-- ID&#45;&gt;Loan_Period -->\n",
+                            "<g id=\"edge13\" class=\"edge\">\n",
+                            "<title>ID&#45;&gt;Loan_Period</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1154.2,-153.9C1192.55,-142.76 1267.74,-120.92 1318.62,-106.14\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1319.33,-109.58 1327.95,-103.43 1317.38,-102.86 1319.33,-109.58\"/>\n",
                             "</g>\n",
-                            "<!-- Loan_Amount -->\n",
-                            "<g id=\"node13\" class=\"node\">\n",
-                            "<title>Loan_Amount</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1292.76\" cy=\"-90\" rx=\"65.17\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1292.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Loan_Amount</text>\n",
+                            "<!-- EMI -->\n",
+                            "<g id=\"node16\" class=\"node\">\n",
+                            "<title>EMI</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1475.76\" cy=\"-90\" rx=\"28.32\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1475.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">EMI</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;Loan_Amount -->\n",
-                            "<g id=\"edge12\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;Loan_Amount</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1147.42,-151.56C1172.93,-140.93 1215.03,-123.39 1247.37,-109.91\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1248.65,-113.17 1256.53,-106.1 1245.95,-106.71 1248.65,-113.17\"/>\n",
+                            "<!-- ID&#45;&gt;EMI -->\n",
+                            "<g id=\"edge14\" class=\"edge\">\n",
+                            "<title>ID&#45;&gt;EMI</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1156.76,-158.75C1211.16,-153.71 1337.37,-139.39 1438.76,-108 1440.36,-107.5 1441.99,-106.95 1443.62,-106.36\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1444.88,-109.63 1452.82,-102.61 1442.24,-103.15 1444.88,-109.63\"/>\n",
                             "</g>\n",
                             "<!-- Source_Category -->\n",
-                            "<g id=\"node14\" class=\"node\">\n",
+                            "<g id=\"node17\" class=\"node\">\n",
                             "<title>Source_Category</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1450.76\" cy=\"-90\" rx=\"74.89\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1450.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Source_Category</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1596.76\" cy=\"-90\" rx=\"74.89\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1596.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Source_Category</text>\n",
                             "</g>\n",
                             "<!-- ID&#45;&gt;Source_Category -->\n",
-                            "<g id=\"edge13\" class=\"edge\">\n",
+                            "<g id=\"edge15\" class=\"edge\">\n",
                             "<title>ID&#45;&gt;Source_Category</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1150.34,-155.51C1200.42,-144.75 1312.81,-120.62 1385.03,-105.11\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1385.74,-108.54 1394.78,-103.02 1384.27,-101.7 1385.74,-108.54\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1156.31,-157.9C1218.7,-150.5 1379.42,-130.7 1512.76,-108 1518.72,-106.99 1524.9,-105.87 1531.09,-104.7\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1531.54,-108.18 1540.69,-102.85 1530.21,-101.3 1531.54,-108.18\"/>\n",
                             "</g>\n",
                             "<!-- Lead_Creation_Date -->\n",
-                            "<g id=\"node15\" class=\"node\">\n",
+                            "<g id=\"node18\" class=\"node\">\n",
                             "<title>Lead_Creation_Date</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1631.76\" cy=\"-90\" rx=\"87.69\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1631.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Lead_Creation_Date</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1777.76\" cy=\"-90\" rx=\"87.69\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1777.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Lead_Creation_Date</text>\n",
                             "</g>\n",
                             "<!-- ID&#45;&gt;Lead_Creation_Date -->\n",
-                            "<g id=\"edge14\" class=\"edge\">\n",
+                            "<g id=\"edge16\" class=\"edge\">\n",
                             "<title>ID&#45;&gt;Lead_Creation_Date</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1151.2,-158C1216.46,-150.5 1390.37,-129.97 1534.76,-108 1541.83,-106.92 1549.18,-105.75 1556.53,-104.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1556.88,-108.02 1566.16,-102.91 1555.71,-101.12 1556.88,-108.02\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1156.79,-159.15C1236.96,-153.49 1480.3,-135.17 1680.76,-108 1688.1,-107.01 1695.74,-105.86 1703.36,-104.64\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1703.68,-108.14 1712.98,-103.07 1702.55,-101.23 1703.68,-108.14\"/>\n",
                             "</g>\n",
-                            "<!-- EMI -->\n",
-                            "<g id=\"node16\" class=\"node\">\n",
-                            "<title>EMI</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1765.76\" cy=\"-90\" rx=\"28.32\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1765.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">EMI</text>\n",
+                            "<!-- Loan_Amount -->\n",
+                            "<g id=\"node19\" class=\"node\">\n",
+                            "<title>Loan_Amount</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1948.76\" cy=\"-90\" rx=\"65.17\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"1948.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Loan_Amount</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;EMI -->\n",
-                            "<g id=\"edge15\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;EMI</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1151.98,-159.85C1254.53,-155.32 1617.34,-137.53 1728.76,-108 1730.38,-107.57 1732.02,-107.07 1733.66,-106.53\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1734.87,-109.81 1742.9,-102.91 1732.31,-103.3 1734.87,-109.81\"/>\n",
+                            "<!-- ID&#45;&gt;Loan_Amount -->\n",
+                            "<g id=\"edge18\" class=\"edge\">\n",
+                            "<title>ID&#45;&gt;Loan_Amount</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M1156.99,-160.58C1254.67,-158.76 1596.48,-149.61 1874.76,-108 1880.02,-107.21 1885.47,-106.25 1890.9,-105.19\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"1891.43,-108.66 1900.51,-103.2 1890.01,-101.8 1891.43,-108.66\"/>\n",
                             "</g>\n",
-                            "<!-- City_Code -->\n",
-                            "<g id=\"node17\" class=\"node\">\n",
-                            "<title>City_Code</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1862.76\" cy=\"-90\" rx=\"50.84\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1862.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Code</text>\n",
+                            "<!-- Employer_Category1 -->\n",
+                            "<g id=\"node3\" class=\"node\">\n",
+                            "<title>Employer_Category1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"90.76\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"90.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category1</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;City_Code -->\n",
-                            "<g id=\"edge16\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;City_Code</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1152.13,-160.8C1244.5,-159.7 1552.88,-152.71 1802.76,-108 1806.78,-107.28 1810.92,-106.4 1815.05,-105.43\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1815.6,-108.9 1824.43,-103.05 1813.88,-102.12 1815.6,-108.9\"/>\n",
+                            "<!-- Employer_Code&#45;&gt;Employer_Category1 -->\n",
+                            "<g id=\"edge2\" class=\"edge\">\n",
+                            "<title>Employer_Code&#45;&gt;Employer_Category1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M225.5,-74.15C200.48,-63.92 166.94,-50.19 139.58,-38.99\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"141.03,-35.8 130.45,-35.25 138.38,-42.27 141.03,-35.8\"/>\n",
                             "</g>\n",
-                            "<!-- Loan_Period -->\n",
-                            "<g id=\"node18\" class=\"node\">\n",
-                            "<title>Loan_Period</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1989.76\" cy=\"-90\" rx=\"58.52\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1989.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Loan_Period</text>\n",
+                            "<!-- Employer_Category2 -->\n",
+                            "<g id=\"node7\" class=\"node\">\n",
+                            "<title>Employer_Category2</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"290.76\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"290.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category2</text>\n",
                             "</g>\n",
-                            "<!-- ID&#45;&gt;Loan_Period -->\n",
-                            "<g id=\"edge17\" class=\"edge\">\n",
-                            "<title>ID&#45;&gt;Loan_Period</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1152.18,-160.98C1254.49,-160.53 1623.47,-155.5 1922.76,-108 1927.36,-107.27 1932.11,-106.37 1936.85,-105.37\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1937.37,-108.84 1946.35,-103.22 1935.83,-102.01 1937.37,-108.84\"/>\n",
+                            "<!-- Employer_Code&#45;&gt;Employer_Category2 -->\n",
+                            "<g id=\"edge5\" class=\"edge\">\n",
+                            "<title>Employer_Code&#45;&gt;Employer_Category2</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M268.93,-71.7C272.05,-64.15 275.8,-55.12 279.29,-46.68\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"282.5,-48.08 283.1,-37.5 276.03,-45.4 282.5,-48.08\"/>\n",
                             "</g>\n",
                             "<!-- Primary_Bank_Type -->\n",
-                            "<g id=\"node7\" class=\"node\">\n",
+                            "<g id=\"node10\" class=\"node\">\n",
                             "<title>Primary_Bank_Type</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"555.76\" cy=\"-18\" rx=\"88.71\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"555.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Primary_Bank_Type</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"516.76\" cy=\"-18\" rx=\"88.71\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"516.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Primary_Bank_Type</text>\n",
                             "</g>\n",
                             "<!-- Customer_Existing_Primary_Bank_Code&#45;&gt;Primary_Bank_Type -->\n",
-                            "<g id=\"edge5\" class=\"edge\">\n",
+                            "<g id=\"edge7\" class=\"edge\">\n",
                             "<title>Customer_Existing_Primary_Bank_Code&#45;&gt;Primary_Bank_Type</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M555.76,-71.7C555.76,-64.41 555.76,-55.73 555.76,-47.54\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"559.26,-47.62 555.76,-37.62 552.26,-47.62 559.26,-47.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M516.76,-71.7C516.76,-64.41 516.76,-55.73 516.76,-47.54\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"520.26,-47.62 516.76,-37.62 513.26,-47.62 520.26,-47.62\"/>\n",
                             "</g>\n",
                             "<!-- City_Category -->\n",
-                            "<g id=\"node19\" class=\"node\">\n",
+                            "<g id=\"node8\" class=\"node\">\n",
                             "<title>City_Category</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"1862.76\" cy=\"-18\" rx=\"65.17\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"1862.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Category</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"865.76\" cy=\"-18\" rx=\"65.17\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"865.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Category</text>\n",
                             "</g>\n",
                             "<!-- City_Code&#45;&gt;City_Category -->\n",
-                            "<g id=\"edge18\" class=\"edge\">\n",
+                            "<g id=\"edge6\" class=\"edge\">\n",
                             "<title>City_Code&#45;&gt;City_Category</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M1862.76,-71.7C1862.76,-64.41 1862.76,-55.73 1862.76,-47.54\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"1866.26,-47.62 1862.76,-37.62 1859.26,-47.62 1866.26,-47.62\"/>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M865.76,-71.7C865.76,-64.41 865.76,-55.73 865.76,-47.54\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"869.26,-47.62 865.76,-37.62 862.26,-47.62 869.26,-47.62\"/>\n",
                             "</g>\n",
                             "</g>\n",
                             "</svg>\n"
                         ],
                         "text/plain": [
-                            "<graphviz.graphs.Digraph at 0x7ebd1e7dac90>"
+                            "<graphviz.graphs.Digraph at 0x7839d2145310>"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.plot_dependency()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/svg+xml": [
                             "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
                             "<!-- Generated by graphviz version 10.0.1 (0)\n",
                             " -->\n",
                             "<!-- Title: Dependency Plot Pages: 1 -->\n",
-                            "<svg width=\"859pt\" height=\"116pt\"\n",
-                            " viewBox=\"0.00 0.00 858.93 116.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<svg width=\"824pt\" height=\"116pt\"\n",
+                            " viewBox=\"0.00 0.00 823.93 116.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
                             "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 112)\">\n",
                             "<title>Dependency Plot</title>\n",
-                            "<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-112 854.93,-112 854.93,4 -4,4\"/>\n",
-                            "<!-- City_Category -->\n",
+                            "<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-112 819.93,-112 819.93,4 -4,4\"/>\n",
+                            "<!-- Employer_Category1 -->\n",
                             "<g id=\"node1\" class=\"node\">\n",
-                            "<title>City_Category</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"65.17\" cy=\"-18\" rx=\"65.17\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"65.17\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Category</text>\n",
+                            "<title>Employer_Category1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"90.76\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"90.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category1</text>\n",
                             "</g>\n",
-                            "<!-- City_Code -->\n",
+                            "<!-- Employer_Code -->\n",
                             "<g id=\"node2\" class=\"node\">\n",
-                            "<title>City_Code</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"65.17\" cy=\"-90\" rx=\"50.84\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"65.17\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Code</text>\n",
+                            "<title>Employer_Code</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"176.76\" cy=\"-90\" rx=\"71.82\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"176.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Code</text>\n",
                             "</g>\n",
-                            "<!-- City_Code&#45;&gt;City_Category -->\n",
+                            "<!-- Employer_Code&#45;&gt;Employer_Category1 -->\n",
                             "<g id=\"edge1\" class=\"edge\">\n",
-                            "<title>City_Code&#45;&gt;City_Category</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M65.17,-71.7C65.17,-64.41 65.17,-55.73 65.17,-47.54\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"68.67,-47.62 65.17,-37.62 61.67,-47.62 68.67,-47.62\"/>\n",
+                            "<title>Employer_Code&#45;&gt;Employer_Category1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M156.38,-72.41C145.61,-63.65 132.2,-52.73 120.32,-43.06\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"122.73,-40.51 112.77,-36.91 118.31,-45.94 122.73,-40.51\"/>\n",
+                            "</g>\n",
+                            "<!-- Employer_Category2 -->\n",
+                            "<g id=\"node5\" class=\"node\">\n",
+                            "<title>Employer_Category2</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"290.76\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"290.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category2</text>\n",
+                            "</g>\n",
+                            "<!-- Employer_Code&#45;&gt;Employer_Category2 -->\n",
+                            "<g id=\"edge3\" class=\"edge\">\n",
+                            "<title>Employer_Code&#45;&gt;Employer_Category2</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M202.91,-72.94C218.19,-63.56 237.7,-51.58 254.45,-41.3\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"255.96,-44.48 262.65,-36.26 252.29,-38.51 255.96,-44.48\"/>\n",
                             "</g>\n",
                             "<!-- Primary_Bank_Type -->\n",
                             "<g id=\"node3\" class=\"node\">\n",
                             "<title>Primary_Bank_Type</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"299.17\" cy=\"-18\" rx=\"88.71\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"299.17\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Primary_Bank_Type</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"516.76\" cy=\"-18\" rx=\"88.71\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"516.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Primary_Bank_Type</text>\n",
                             "</g>\n",
                             "<!-- Customer_Existing_Primary_Bank_Code -->\n",
                             "<g id=\"node4\" class=\"node\">\n",
                             "<title>Customer_Existing_Primary_Bank_Code</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"299.17\" cy=\"-90\" rx=\"165.48\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"299.17\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Customer_Existing_Primary_Bank_Code</text>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"516.76\" cy=\"-90\" rx=\"165.48\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"516.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Customer_Existing_Primary_Bank_Code</text>\n",
                             "</g>\n",
                             "<!-- Customer_Existing_Primary_Bank_Code&#45;&gt;Primary_Bank_Type -->\n",
                             "<g id=\"edge2\" class=\"edge\">\n",
                             "<title>Customer_Existing_Primary_Bank_Code&#45;&gt;Primary_Bank_Type</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M299.17,-71.7C299.17,-64.41 299.17,-55.73 299.17,-47.54\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"302.67,-47.62 299.17,-37.62 295.67,-47.62 302.67,-47.62\"/>\n",
-                            "</g>\n",
-                            "<!-- Employer_Category2 -->\n",
-                            "<g id=\"node5\" class=\"node\">\n",
-                            "<title>Employer_Category2</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"560.17\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"560.17\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category2</text>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M516.76,-71.7C516.76,-64.41 516.76,-55.73 516.76,-47.54\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"520.26,-47.62 516.76,-37.62 513.26,-47.62 520.26,-47.62\"/>\n",
                             "</g>\n",
-                            "<!-- Employer_Code -->\n",
+                            "<!-- City_Category -->\n",
                             "<g id=\"node6\" class=\"node\">\n",
-                            "<title>Employer_Code</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"625.17\" cy=\"-90\" rx=\"71.82\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"625.17\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Code</text>\n",
-                            "</g>\n",
-                            "<!-- Employer_Code&#45;&gt;Employer_Category2 -->\n",
-                            "<g id=\"edge3\" class=\"edge\">\n",
-                            "<title>Employer_Code&#45;&gt;Employer_Category2</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M609.44,-72.05C601.61,-63.63 592,-53.28 583.35,-43.97\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"586.16,-41.84 576.79,-36.9 581.03,-46.61 586.16,-41.84\"/>\n",
+                            "<title>City_Category</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"750.76\" cy=\"-18\" rx=\"65.17\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"750.76\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Category</text>\n",
                             "</g>\n",
-                            "<!-- Employer_Category1 -->\n",
+                            "<!-- City_Code -->\n",
                             "<g id=\"node7\" class=\"node\">\n",
-                            "<title>Employer_Category1</title>\n",
-                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"760.17\" cy=\"-18\" rx=\"90.76\" ry=\"18\"/>\n",
-                            "<text text-anchor=\"middle\" x=\"760.17\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">Employer_Category1</text>\n",
+                            "<title>City_Code</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"750.76\" cy=\"-90\" rx=\"50.84\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"750.76\" y=\"-84.95\" font-family=\"Times,serif\" font-size=\"14.00\">City_Code</text>\n",
                             "</g>\n",
-                            "<!-- Employer_Code&#45;&gt;Employer_Category1 -->\n",
+                            "<!-- City_Code&#45;&gt;City_Category -->\n",
                             "<g id=\"edge4\" class=\"edge\">\n",
-                            "<title>Employer_Code&#45;&gt;Employer_Category1</title>\n",
-                            "<path fill=\"none\" stroke=\"black\" d=\"M655.47,-73.29C674.22,-63.57 698.55,-50.95 719.03,-40.33\"/>\n",
-                            "<polygon fill=\"black\" stroke=\"black\" points=\"720.43,-43.55 727.69,-35.84 717.21,-37.34 720.43,-43.55\"/>\n",
+                            "<title>City_Code&#45;&gt;City_Category</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M750.76,-71.7C750.76,-64.41 750.76,-55.73 750.76,-47.54\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"754.26,-47.62 750.76,-37.62 747.26,-47.62 754.26,-47.62\"/>\n",
                             "</g>\n",
                             "</g>\n",
                             "</svg>\n"
                         ],
                         "text/plain": [
-                            "<graphviz.graphs.Digraph at 0x7ebd1e7d9b10>"
+                            "<graphviz.graphs.Digraph at 0x7839c45af050>"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# ID implies everything, of course, because ID is unique.\n",
                 "# So let's not plot it\n",
                 "dia.plot_dependency(exclude=[\"ID\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
@@ -837,76 +898,76 @@
                             "\u2502 Contacted \u2506 0         \u2506 2        \u2506 Y         \u2506 \u2026 \u2506 1         \u2506 1         \u2506 1.0       \u2506 1.0       \u2502\n",
                             "\u2502 Source    \u2506 0         \u2506 29       \u2506 S122      \u2506 \u2026 \u2506 4         \u2506 4         \u2506 4.0       \u2506 4.0       \u2502\n",
                             "\u2502 Source_Ca \u2506 0         \u2506 7        \u2506 B         \u2506 \u2026 \u2506 1         \u2506 1         \u2506 1.0       \u2506 1.0       \u2502\n",
                             "\u2502 tegory    \u2506           \u2506          \u2506           \u2506   \u2506           \u2506           \u2506           \u2506           \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.str_stats()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"dxqfhhzdbj\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
+                            "<div id=\"dtaeddvjbm\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
                             "<style>\n",
-                            "#dxqfhhzdbj table {\n",
+                            "#dtaeddvjbm table {\n",
                             "          font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;\n",
                             "          -webkit-font-smoothing: antialiased;\n",
                             "          -moz-osx-font-smoothing: grayscale;\n",
                             "        }\n",
                             "\n",
-                            "#dxqfhhzdbj thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
+                            "#dtaeddvjbm thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
                             " tr { background-color: transparent !important; }\n",
-                            "#dxqfhhzdbj p { margin: 0 !important; padding: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
-                            " #dxqfhhzdbj .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
-                            " #dxqfhhzdbj .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #dxqfhhzdbj .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #dxqfhhzdbj .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #dxqfhhzdbj .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
-                            " #dxqfhhzdbj .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
-                            " #dxqfhhzdbj .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
-                            " #dxqfhhzdbj .gt_spanner_row { border-bottom-style: hidden !important; }\n",
-                            " #dxqfhhzdbj .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
-                            " #dxqfhhzdbj .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
-                            " #dxqfhhzdbj .gt_from_md> :first-child { margin-top: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
-                            " #dxqfhhzdbj .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
-                            " #dxqfhhzdbj .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
-                            " #dxqfhhzdbj .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
-                            " #dxqfhhzdbj .gt_row_group_first td { border-top-width: 2px !important; }\n",
-                            " #dxqfhhzdbj .gt_row_group_first th { border-top-width: 2px !important; }\n",
-                            " #dxqfhhzdbj .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #dxqfhhzdbj .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #dxqfhhzdbj .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
-                            " #dxqfhhzdbj .gt_left { text-align: left !important; }\n",
-                            " #dxqfhhzdbj .gt_center { text-align: center !important; }\n",
-                            " #dxqfhhzdbj .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
-                            " #dxqfhhzdbj .gt_font_normal { font-weight: normal !important; }\n",
-                            " #dxqfhhzdbj .gt_font_bold { font-weight: bold !important; }\n",
-                            " #dxqfhhzdbj .gt_font_italic { font-style: italic !important; }\n",
-                            " #dxqfhhzdbj .gt_super { font-size: 65% !important; }\n",
-                            " #dxqfhhzdbj .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
-                            " #dxqfhhzdbj .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
+                            "#dtaeddvjbm p { margin: 0 !important; padding: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
+                            " #dtaeddvjbm .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
+                            " #dtaeddvjbm .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #dtaeddvjbm .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #dtaeddvjbm .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #dtaeddvjbm .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
+                            " #dtaeddvjbm .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
+                            " #dtaeddvjbm .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
+                            " #dtaeddvjbm .gt_spanner_row { border-bottom-style: hidden !important; }\n",
+                            " #dtaeddvjbm .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
+                            " #dtaeddvjbm .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
+                            " #dtaeddvjbm .gt_from_md> :first-child { margin-top: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
+                            " #dtaeddvjbm .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
+                            " #dtaeddvjbm .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
+                            " #dtaeddvjbm .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
+                            " #dtaeddvjbm .gt_row_group_first td { border-top-width: 2px !important; }\n",
+                            " #dtaeddvjbm .gt_row_group_first th { border-top-width: 2px !important; }\n",
+                            " #dtaeddvjbm .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #dtaeddvjbm .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #dtaeddvjbm .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
+                            " #dtaeddvjbm .gt_left { text-align: left !important; }\n",
+                            " #dtaeddvjbm .gt_center { text-align: center !important; }\n",
+                            " #dtaeddvjbm .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
+                            " #dtaeddvjbm .gt_font_normal { font-weight: normal !important; }\n",
+                            " #dtaeddvjbm .gt_font_bold { font-weight: bold !important; }\n",
+                            " #dtaeddvjbm .gt_font_italic { font-style: italic !important; }\n",
+                            " #dtaeddvjbm .gt_super { font-size: 65% !important; }\n",
+                            " #dtaeddvjbm .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
+                            " #dtaeddvjbm .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
                             " \n",
                             "</style>\n",
                             "<table class=\"gt_table\" data-quarto-disable-processing=\"false\" data-quarto-bootstrap=\"false\">\n",
                             "\n",
                             "<tr class=\"gt_col_headings\">\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_left\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"column\">column</th>\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_center\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"non_null_cnt\">non_null_cnt</th>\n",
@@ -1094,29 +1155,29 @@
                             "\u2502            \u2506            \u2506          \u2506 2          \u2506   \u2506          \u2506         \u2506           \u2506 8179, \u2026   \u2502\n",
                             "\u2502            \u2506            \u2506          \u2506            \u2506   \u2506          \u2506         \u2506           \u2506 2]}       \u2502\n",
                             "\u2502 Var1       \u2506 69713      \u2506 0.0      \u2506 3.948446   \u2506 \u2026 \u2506 10.0     \u2506 7.0     \u2506 0         \u2506 {[23308,  \u2502\n",
                             "\u2502            \u2506            \u2506          \u2506            \u2506   \u2506          \u2506         \u2506           \u2506 13363, \u2026  \u2502\n",
                             "\u2502            \u2506            \u2506          \u2506            \u2506   \u2506          \u2506         \u2506           \u2506 13420]}   \u2502\n",
                             "\u2502 Approved   \u2506 69713      \u2506 0.0      \u2506 0.014631   \u2506 \u2026 \u2506 1.0      \u2506 0.0     \u2506 1020      \u2506 {[68693,  \u2502\n",
                             "\u2502            \u2506            \u2506          \u2506            \u2506   \u2506          \u2506         \u2506           \u2506 1020]}    \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7ebd1752c650>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.stub: 2>, column_label='column', column_align='left', column_width=None), ColInfo(var='non_null_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='non_null_cnt', column_align='center', column_width=None), ColInfo(var='null%', type=<ColInfoTypeEnum.default: 1>, column_label='null%', column_align='right', column_width=None), ColInfo(var='mean', type=<ColInfoTypeEnum.default: 1>, column_label='mean', column_align='right', column_width=None), ColInfo(var='std', type=<ColInfoTypeEnum.default: 1>, column_label='std', column_align='right', column_width=None), ColInfo(var='min', type=<ColInfoTypeEnum.default: 1>, column_label='min', column_align='right', column_width=None), ColInfo(var='q1', type=<ColInfoTypeEnum.default: 1>, column_label='q1', column_align='right', column_width=None), ColInfo(var='median', type=<ColInfoTypeEnum.default: 1>, column_label='median', column_align='right', column_width=None), ColInfo(var='q3', type=<ColInfoTypeEnum.default: 1>, column_label='q3', column_align='right', column_width=None), ColInfo(var='max', type=<ColInfoTypeEnum.default: 1>, column_label='max', column_align='right', column_width=None), ColInfo(var='IQR', type=<ColInfoTypeEnum.default: 1>, column_label='IQR', column_align='right', column_width=None), ColInfo(var='outlier_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='outlier_cnt', column_align='center', column_width=None), ColInfo(var='histogram', type=<ColInfoTypeEnum.default: 1>, column_label='histogram', column_align='center', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname='Employer_Category2', group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname='Monthly_Income', group_label=None, built=False), RowInfo(rownum_i=2, group_id=None, rowname='Existing_EMI', group_label=None, built=False), RowInfo(rownum_i=3, group_id=None, rowname='Loan_Amount', group_label=None, built=False), RowInfo(rownum_i=4, group_id=None, rowname='Loan_Period', group_label=None, built=False), RowInfo(rownum_i=5, group_id=None, rowname='Interest_Rate', group_label=None, built=False), RowInfo(rownum_i=6, group_id=None, rowname='EMI', group_label=None, built=False), RowInfo(rownum_i=7, group_id=None, rowname='Var1', group_label=None, built=False), RowInfo(rownum_i=8, group_id=None, rowname='Approved', group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead='column', _source_notes=[], _footnotes=[], _styles=[], _locale=<great_tables._gt_data.Locale object at 0x7ebd17787610>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7ebd1e7afd50>, <great_tables._gt_data.FormatInfo object at 0x7ebd17543ad0>, <great_tables._gt_data.FormatInfo object at 0x7ebd17543c50>], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7839c57dad10>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.stub: 2>, column_label='column', column_align='left', column_width=None), ColInfo(var='non_null_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='non_null_cnt', column_align='center', column_width=None), ColInfo(var='null%', type=<ColInfoTypeEnum.default: 1>, column_label='null%', column_align='right', column_width=None), ColInfo(var='mean', type=<ColInfoTypeEnum.default: 1>, column_label='mean', column_align='right', column_width=None), ColInfo(var='std', type=<ColInfoTypeEnum.default: 1>, column_label='std', column_align='right', column_width=None), ColInfo(var='min', type=<ColInfoTypeEnum.default: 1>, column_label='min', column_align='right', column_width=None), ColInfo(var='q1', type=<ColInfoTypeEnum.default: 1>, column_label='q1', column_align='right', column_width=None), ColInfo(var='median', type=<ColInfoTypeEnum.default: 1>, column_label='median', column_align='right', column_width=None), ColInfo(var='q3', type=<ColInfoTypeEnum.default: 1>, column_label='q3', column_align='right', column_width=None), ColInfo(var='max', type=<ColInfoTypeEnum.default: 1>, column_label='max', column_align='right', column_width=None), ColInfo(var='IQR', type=<ColInfoTypeEnum.default: 1>, column_label='IQR', column_align='right', column_width=None), ColInfo(var='outlier_cnt', type=<ColInfoTypeEnum.default: 1>, column_label='outlier_cnt', column_align='center', column_width=None), ColInfo(var='histogram', type=<ColInfoTypeEnum.default: 1>, column_label='histogram', column_align='center', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname='Employer_Category2', group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname='Monthly_Income', group_label=None, built=False), RowInfo(rownum_i=2, group_id=None, rowname='Existing_EMI', group_label=None, built=False), RowInfo(rownum_i=3, group_id=None, rowname='Loan_Amount', group_label=None, built=False), RowInfo(rownum_i=4, group_id=None, rowname='Loan_Period', group_label=None, built=False), RowInfo(rownum_i=5, group_id=None, rowname='Interest_Rate', group_label=None, built=False), RowInfo(rownum_i=6, group_id=None, rowname='EMI', group_label=None, built=False), RowInfo(rownum_i=7, group_id=None, rowname='Var1', group_label=None, built=False), RowInfo(rownum_i=8, group_id=None, rowname='Approved', group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead='column', _source_notes=[], _footnotes=[], _styles=[], _locale=<great_tables._gt_data.Locale object at 0x7839c45a3c50>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7839d1922d50>, <great_tables._gt_data.FormatInfo object at 0x7839c45a27d0>, <great_tables._gt_data.FormatInfo object at 0x7839c45b7e90>], _substitutions=[], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.numeric_profile(iqr_multiplier=2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
@@ -1138,36 +1199,36 @@
                             "\u2502 Monthly_In \u2506 0.001546   \u2506 1.0       \u2506 0.245826  \u2506 \u2026 \u2506 -0.014789 \u2506 0.035163 \u2506 0.024854 \u2506 0.000472 \u2502\n",
                             "\u2502 come       \u2506            \u2506           \u2506           \u2506   \u2506           \u2506          \u2506          \u2506          \u2502\n",
                             "\u2502 Existing_E \u2506 -0.017074  \u2506 0.245826  \u2506 1.0       \u2506 \u2026 \u2506 -0.023001 \u2506 0.000813 \u2506 0.00662  \u2506 0.027821 \u2502\n",
                             "\u2502 MI         \u2506            \u2506           \u2506           \u2506   \u2506           \u2506          \u2506          \u2506          \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import polars.selectors as cs\n",
                 "\n",
                 "dia.corr(subset=[\"Monthly_Income\", \"Existing_EMI\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "INFO:polars_ds.diagnosis:The following columns are not numeric/not in the dataframe, skipped: \n",
-                        "['Gender', 'Employer_Code', 'Customer_Existing_Primary_Bank_Code', 'Source', 'Contacted', 'ID', 'DOB', 'Lead_Creation_Date', 'City_Code', 'Employer_Category1', 'City_Category', 'Source_Category', 'Primary_Bank_Type']\n"
+                        "['DOB', 'Lead_Creation_Date', 'Gender', 'Source', 'Primary_Bank_Type', 'Employer_Category1', 'Customer_Existing_Primary_Bank_Code', 'Contacted', 'City_Code', 'City_Category', 'ID', 'Source_Category', 'Employer_Code']\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
@@ -1200,76 +1261,76 @@
                             "\u2502 Rate      \u2506           \u2506           \u2506           \u2506   \u2506           \u2506           \u2506           \u2506 7        \u2502\n",
                             "\u2502 EMI       \u2506 -0.051729 \u2506 0.035163  \u2506 0.000813  \u2506 \u2026 \u2506 -0.241648 \u2506 1.0       \u2506 0.293474  \u2506 0.050129 \u2502\n",
                             "\u2502 Var1      \u2506 -0.124415 \u2506 0.024854  \u2506 0.00662   \u2506 \u2026 \u2506 -0.554138 \u2506 0.293474  \u2506 1.0       \u2506 0.11244  \u2502\n",
                             "\u2502 Approved  \u2506 -0.019413 \u2506 0.000472  \u2506 0.027821  \u2506 \u2026 \u2506 -0.094387 \u2506 0.050129  \u2506 0.11244   \u2506 1.0      \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.corr(subset=cs.all())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"lcfkyyepht\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
+                            "<div id=\"wgssvaaomh\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
                             "<style>\n",
-                            "#lcfkyyepht table {\n",
+                            "#wgssvaaomh table {\n",
                             "          font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;\n",
                             "          -webkit-font-smoothing: antialiased;\n",
                             "          -moz-osx-font-smoothing: grayscale;\n",
                             "        }\n",
                             "\n",
-                            "#lcfkyyepht thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
+                            "#wgssvaaomh thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
                             " tr { background-color: transparent !important; }\n",
-                            "#lcfkyyepht p { margin: 0 !important; padding: 0 !important; }\n",
-                            " #lcfkyyepht .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
-                            " #lcfkyyepht .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
-                            " #lcfkyyepht .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
-                            " #lcfkyyepht .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
-                            " #lcfkyyepht .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #lcfkyyepht .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #lcfkyyepht .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #lcfkyyepht .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
-                            " #lcfkyyepht .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
-                            " #lcfkyyepht .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
-                            " #lcfkyyepht .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
-                            " #lcfkyyepht .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
-                            " #lcfkyyepht .gt_spanner_row { border-bottom-style: hidden !important; }\n",
-                            " #lcfkyyepht .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
-                            " #lcfkyyepht .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
-                            " #lcfkyyepht .gt_from_md> :first-child { margin-top: 0 !important; }\n",
-                            " #lcfkyyepht .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
-                            " #lcfkyyepht .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
-                            " #lcfkyyepht .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
-                            " #lcfkyyepht .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
-                            " #lcfkyyepht .gt_row_group_first td { border-top-width: 2px !important; }\n",
-                            " #lcfkyyepht .gt_row_group_first th { border-top-width: 2px !important; }\n",
-                            " #lcfkyyepht .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #lcfkyyepht .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #lcfkyyepht .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
-                            " #lcfkyyepht .gt_left { text-align: left !important; }\n",
-                            " #lcfkyyepht .gt_center { text-align: center !important; }\n",
-                            " #lcfkyyepht .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
-                            " #lcfkyyepht .gt_font_normal { font-weight: normal !important; }\n",
-                            " #lcfkyyepht .gt_font_bold { font-weight: bold !important; }\n",
-                            " #lcfkyyepht .gt_font_italic { font-style: italic !important; }\n",
-                            " #lcfkyyepht .gt_super { font-size: 65% !important; }\n",
-                            " #lcfkyyepht .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
-                            " #lcfkyyepht .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
+                            "#wgssvaaomh p { margin: 0 !important; padding: 0 !important; }\n",
+                            " #wgssvaaomh .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
+                            " #wgssvaaomh .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
+                            " #wgssvaaomh .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
+                            " #wgssvaaomh .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
+                            " #wgssvaaomh .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #wgssvaaomh .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #wgssvaaomh .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #wgssvaaomh .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
+                            " #wgssvaaomh .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
+                            " #wgssvaaomh .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
+                            " #wgssvaaomh .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
+                            " #wgssvaaomh .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
+                            " #wgssvaaomh .gt_spanner_row { border-bottom-style: hidden !important; }\n",
+                            " #wgssvaaomh .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
+                            " #wgssvaaomh .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
+                            " #wgssvaaomh .gt_from_md> :first-child { margin-top: 0 !important; }\n",
+                            " #wgssvaaomh .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
+                            " #wgssvaaomh .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
+                            " #wgssvaaomh .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
+                            " #wgssvaaomh .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
+                            " #wgssvaaomh .gt_row_group_first td { border-top-width: 2px !important; }\n",
+                            " #wgssvaaomh .gt_row_group_first th { border-top-width: 2px !important; }\n",
+                            " #wgssvaaomh .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #wgssvaaomh .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #wgssvaaomh .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
+                            " #wgssvaaomh .gt_left { text-align: left !important; }\n",
+                            " #wgssvaaomh .gt_center { text-align: center !important; }\n",
+                            " #wgssvaaomh .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
+                            " #wgssvaaomh .gt_font_normal { font-weight: normal !important; }\n",
+                            " #wgssvaaomh .gt_font_bold { font-weight: bold !important; }\n",
+                            " #wgssvaaomh .gt_font_italic { font-style: italic !important; }\n",
+                            " #wgssvaaomh .gt_super { font-size: 65% !important; }\n",
+                            " #wgssvaaomh .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
+                            " #wgssvaaomh .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
                             " \n",
                             "</style>\n",
                             "<table class=\"gt_table\" data-quarto-disable-processing=\"false\" data-quarto-bootstrap=\"false\">\n",
                             "\n",
                             "<tr class=\"gt_col_headings\">\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_left\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"column\">column</th>\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_right\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"Employer_Category2\">Employer_Category2</th>\n",
@@ -1283,30 +1344,30 @@
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_right\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"Approved\">Approved</th>\n",
                             "</tr>\n",
                             "<tbody class=\"gt_table_body\">\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Monthly_Income</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.002</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #770269;\" class=\"gt_row gt_right\">0.246</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #640277;\" class=\"gt_row gt_right\">0.040</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #76026a;\" class=\"gt_row gt_right\">0.246</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #630277;\" class=\"gt_row gt_right\">0.040</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.004</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.015</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #630278;\" class=\"gt_row gt_right\">0.035</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #620278;\" class=\"gt_row gt_right\">0.025</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.000</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Existing_EMI</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.017</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #770269;\" class=\"gt_row gt_right\">0.246</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #76026a;\" class=\"gt_row gt_right\">0.246</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #610279;\" class=\"gt_row gt_right\">0.009</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #600279;\" class=\"gt_row gt_right\">0.009</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.005</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.023</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #5d027c;\" class=\"gt_row gt_right\">\u22120.023</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.001</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.007</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #620278;\" class=\"gt_row gt_right\">0.028</td>\n",
                             "</tr>\n",
                             "</tbody>\n",
                             "\n",
                             "\n",
@@ -1323,87 +1384,87 @@
                             "\u2502 str        \u2506 ---        \u2506 ---       \u2506 ---       \u2506   \u2506 ---       \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
                             "\u2502            \u2506 f64        \u2506 f64       \u2506 f64       \u2506   \u2506 f64       \u2506          \u2506          \u2506          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 Monthly_In \u2506 0.001546   \u2506 1.0       \u2506 0.245826  \u2506 \u2026 \u2506 -0.014789 \u2506 0.035163 \u2506 0.024854 \u2506 0.000472 \u2502\n",
                             "\u2502 come       \u2506            \u2506           \u2506           \u2506   \u2506           \u2506          \u2506          \u2506          \u2502\n",
                             "\u2502 Existing_E \u2506 -0.017074  \u2506 0.245826  \u2506 1.0       \u2506 \u2026 \u2506 -0.023001 \u2506 0.000813 \u2506 0.00662  \u2506 0.027821 \u2502\n",
                             "\u2502 MI         \u2506            \u2506           \u2506           \u2506   \u2506           \u2506          \u2506          \u2506          \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7ebd17542910>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.default: 1>, column_label='column', column_align='left', column_width=None), ColInfo(var='Employer_Category2', type=<ColInfoTypeEnum.default: 1>, column_label='Employer_Category2', column_align='right', column_width=None), ColInfo(var='Monthly_Income', type=<ColInfoTypeEnum.default: 1>, column_label='Monthly_Income', column_align='right', column_width=None), ColInfo(var='Existing_EMI', type=<ColInfoTypeEnum.default: 1>, column_label='Existing_EMI', column_align='right', column_width=None), ColInfo(var='Loan_Amount', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Amount', column_align='right', column_width=None), ColInfo(var='Loan_Period', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Period', column_align='right', column_width=None), ColInfo(var='Interest_Rate', type=<ColInfoTypeEnum.default: 1>, column_label='Interest_Rate', column_align='right', column_width=None), ColInfo(var='EMI', type=<ColInfoTypeEnum.default: 1>, column_label='EMI', column_align='right', column_width=None), ColInfo(var='Var1', type=<ColInfoTypeEnum.default: 1>, column_label='Var1', column_align='right', column_width=None), ColInfo(var='Approved', type=<ColInfoTypeEnum.default: 1>, column_label='Approved', column_align='right', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname=None, group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead=None, _source_notes=[], _footnotes=[], _styles=[StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#770269')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#770269')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#610279')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')])], _locale=<great_tables._gt_data.Locale object at 0x7ebd175568d0>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7ebd17555cd0>], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7839c45ad110>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.default: 1>, column_label='column', column_align='left', column_width=None), ColInfo(var='Employer_Category2', type=<ColInfoTypeEnum.default: 1>, column_label='Employer_Category2', column_align='right', column_width=None), ColInfo(var='Monthly_Income', type=<ColInfoTypeEnum.default: 1>, column_label='Monthly_Income', column_align='right', column_width=None), ColInfo(var='Existing_EMI', type=<ColInfoTypeEnum.default: 1>, column_label='Existing_EMI', column_align='right', column_width=None), ColInfo(var='Loan_Amount', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Amount', column_align='right', column_width=None), ColInfo(var='Loan_Period', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Period', column_align='right', column_width=None), ColInfo(var='Interest_Rate', type=<ColInfoTypeEnum.default: 1>, column_label='Interest_Rate', column_align='right', column_width=None), ColInfo(var='EMI', type=<ColInfoTypeEnum.default: 1>, column_label='EMI', column_align='right', column_width=None), ColInfo(var='Var1', type=<ColInfoTypeEnum.default: 1>, column_label='Var1', column_align='right', column_width=None), ColInfo(var='Approved', type=<ColInfoTypeEnum.default: 1>, column_label='Approved', column_align='right', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname=None, group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead=None, _source_notes=[], _footnotes=[], _styles=[StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#76026a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#76026a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#600279')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5d027c')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')])], _locale=<great_tables._gt_data.Locale object at 0x7839c45d5d90>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7839c45d5e10>], _substitutions=[], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.plot_corr(subset=[\"Monthly_Income\", \"Existing_EMI\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "INFO:polars_ds.diagnosis:The following columns are not numeric/not in the dataframe, skipped: \n",
-                        "['Gender', 'Employer_Code', 'Customer_Existing_Primary_Bank_Code', 'Source', 'Contacted', 'ID', 'DOB', 'Lead_Creation_Date', 'City_Code', 'Employer_Category1', 'City_Category', 'Source_Category', 'Primary_Bank_Type']\n"
+                        "['DOB', 'Lead_Creation_Date', 'Gender', 'Source', 'Primary_Bank_Type', 'Employer_Category1', 'Customer_Existing_Primary_Bank_Code', 'Contacted', 'City_Code', 'City_Category', 'ID', 'Source_Category', 'Employer_Code']\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"jcrmxfwsvn\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
+                            "<div id=\"zcnbgdizqy\" style=\"padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;\">\n",
                             "<style>\n",
-                            "#jcrmxfwsvn table {\n",
+                            "#zcnbgdizqy table {\n",
                             "          font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;\n",
                             "          -webkit-font-smoothing: antialiased;\n",
                             "          -moz-osx-font-smoothing: grayscale;\n",
                             "        }\n",
                             "\n",
-                            "#jcrmxfwsvn thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
+                            "#zcnbgdizqy thead, tbody, tfoot, tr, td, th { border-style: none !important; }\n",
                             " tr { background-color: transparent !important; }\n",
-                            "#jcrmxfwsvn p { margin: 0 !important; padding: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
-                            " #jcrmxfwsvn .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
-                            " #jcrmxfwsvn .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #jcrmxfwsvn .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #jcrmxfwsvn .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #jcrmxfwsvn .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
-                            " #jcrmxfwsvn .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
-                            " #jcrmxfwsvn .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
-                            " #jcrmxfwsvn .gt_spanner_row { border-bottom-style: hidden !important; }\n",
-                            " #jcrmxfwsvn .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
-                            " #jcrmxfwsvn .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
-                            " #jcrmxfwsvn .gt_from_md> :first-child { margin-top: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
-                            " #jcrmxfwsvn .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
-                            " #jcrmxfwsvn .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
-                            " #jcrmxfwsvn .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
-                            " #jcrmxfwsvn .gt_row_group_first td { border-top-width: 2px !important; }\n",
-                            " #jcrmxfwsvn .gt_row_group_first th { border-top-width: 2px !important; }\n",
-                            " #jcrmxfwsvn .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
-                            " #jcrmxfwsvn .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
-                            " #jcrmxfwsvn .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
-                            " #jcrmxfwsvn .gt_left { text-align: left !important; }\n",
-                            " #jcrmxfwsvn .gt_center { text-align: center !important; }\n",
-                            " #jcrmxfwsvn .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
-                            " #jcrmxfwsvn .gt_font_normal { font-weight: normal !important; }\n",
-                            " #jcrmxfwsvn .gt_font_bold { font-weight: bold !important; }\n",
-                            " #jcrmxfwsvn .gt_font_italic { font-style: italic !important; }\n",
-                            " #jcrmxfwsvn .gt_super { font-size: 65% !important; }\n",
-                            " #jcrmxfwsvn .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
-                            " #jcrmxfwsvn .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
+                            "#zcnbgdizqy p { margin: 0 !important; padding: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_table { display: table !important; border-collapse: collapse !important; line-height: normal !important; margin-left: auto !important; margin-right: auto !important; color: #333333 !important; font-size: 16px !important; font-weight: normal !important; font-style: normal !important; background-color: #FFFFFF !important; width: auto !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #A8A8A8 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #A8A8A8 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; }\n",
+                            " #zcnbgdizqy .gt_caption { padding-top: 4px !important; padding-bottom: 4px !important; }\n",
+                            " #zcnbgdizqy .gt_title { color: #333333 !important; font-size: 125% !important; font-weight: initial !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; border-bottom-color: #FFFFFF !important; border-bottom-width: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_subtitle { color: #333333 !important; font-size: 85% !important; font-weight: initial !important; padding-top: 3px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; border-top-color: #FFFFFF !important; border-top-width: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_heading { background-color: #FFFFFF !important; text-align: center !important; border-bottom-color: #FFFFFF !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #zcnbgdizqy .gt_bottom_border { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #zcnbgdizqy .gt_col_headings { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #zcnbgdizqy .gt_col_heading { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; padding-left: 5px !important; padding-right: 5px !important; overflow-x: hidden !important; }\n",
+                            " #zcnbgdizqy .gt_column_spanner_outer { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: normal !important; text-transform: inherit !important; padding-top: 0 !important; padding-bottom: 0 !important; padding-left: 4px !important; padding-right: 4px !important; }\n",
+                            " #zcnbgdizqy .gt_column_spanner_outer:first-child { padding-left: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_column_spanner_outer:last-child { padding-right: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_column_spanner { border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: bottom !important; padding-top: 5px !important; padding-bottom: 5px !important; overflow-x: hidden !important; display: inline-block !important; width: 100% !important; }\n",
+                            " #zcnbgdizqy .gt_spanner_row { border-bottom-style: hidden !important; }\n",
+                            " #zcnbgdizqy .gt_group_heading { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; text-align: left !important; }\n",
+                            " #zcnbgdizqy .gt_empty_group_heading { padding: 0.5px !important; color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; vertical-align: middle !important; }\n",
+                            " #zcnbgdizqy .gt_from_md> :first-child { margin-top: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_from_md> :last-child { margin-bottom: 0 !important; }\n",
+                            " #zcnbgdizqy .gt_row { padding-top: 8px !important; padding-bottom: 8px !important; padding-left: 5px !important; padding-right: 5px !important; margin: 10px !important; border-top-style: solid !important; border-top-width: 1px !important; border-top-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 1px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 1px !important; border-right-color: #D3D3D3 !important; vertical-align: middle !important; overflow-x: hidden !important; }\n",
+                            " #zcnbgdizqy .gt_stub { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; }\n",
+                            " #zcnbgdizqy .gt_stub_row_group { color: #333333 !important; background-color: #FFFFFF !important; font-size: 100% !important; font-weight: initial !important; text-transform: inherit !important; border-right-style: solid !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; padding-left: 5px !important; padding-right: 5px !important; vertical-align: top !important; }\n",
+                            " #zcnbgdizqy .gt_row_group_first td { border-top-width: 2px !important; }\n",
+                            " #zcnbgdizqy .gt_row_group_first th { border-top-width: 2px !important; }\n",
+                            " #zcnbgdizqy .gt_table_body { border-top-style: solid !important; border-top-width: 2px !important; border-top-color: #D3D3D3 !important; border-bottom-style: solid !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; }\n",
+                            " #zcnbgdizqy .gt_sourcenotes { color: #333333 !important; background-color: #FFFFFF !important; border-bottom-style: none !important; border-bottom-width: 2px !important; border-bottom-color: #D3D3D3 !important; border-left-style: none !important; border-left-width: 2px !important; border-left-color: #D3D3D3 !important; border-right-style: none !important; border-right-width: 2px !important; border-right-color: #D3D3D3 !important; }\n",
+                            " #zcnbgdizqy .gt_sourcenote { font-size: 90% !important; padding-top: 4px !important; padding-bottom: 4px !important; padding-left: 5px !important; padding-right: 5px !important; text-align: left !important; }\n",
+                            " #zcnbgdizqy .gt_left { text-align: left !important; }\n",
+                            " #zcnbgdizqy .gt_center { text-align: center !important; }\n",
+                            " #zcnbgdizqy .gt_right { text-align: right !important; font-variant-numeric: tabular-nums !important; }\n",
+                            " #zcnbgdizqy .gt_font_normal { font-weight: normal !important; }\n",
+                            " #zcnbgdizqy .gt_font_bold { font-weight: bold !important; }\n",
+                            " #zcnbgdizqy .gt_font_italic { font-style: italic !important; }\n",
+                            " #zcnbgdizqy .gt_super { font-size: 65% !important; }\n",
+                            " #zcnbgdizqy .gt_footnote_marks { font-size: 75% !important; vertical-align: 0.4em !important; position: initial !important; }\n",
+                            " #zcnbgdizqy .gt_asterisk { font-size: 100% !important; vertical-align: 0 !important; }\n",
                             " \n",
                             "</style>\n",
                             "<table class=\"gt_table\" data-quarto-disable-processing=\"false\" data-quarto-bootstrap=\"false\">\n",
                             "\n",
                             "<tr class=\"gt_col_headings\">\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_left\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"column\">column</th>\n",
                             "  <th class=\"gt_col_heading gt_columns_bottom_border gt_right\" rowspan=\"1\" colspan=\"1\" scope=\"col\" id=\"Employer_Category2\">Employer_Category2</th>\n",
@@ -1429,69 +1490,69 @@
                             "  <td style=\"color: #FFFFFF; background-color: #540282;\" class=\"gt_row gt_right\">\u22120.124</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.019</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Monthly_Income</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.002</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #770269;\" class=\"gt_row gt_right\">0.246</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #640277;\" class=\"gt_row gt_right\">0.040</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #76026a;\" class=\"gt_row gt_right\">0.246</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #630277;\" class=\"gt_row gt_right\">0.040</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.004</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.015</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #630278;\" class=\"gt_row gt_right\">0.035</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #620278;\" class=\"gt_row gt_right\">0.025</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.000</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Existing_EMI</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.017</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #770269;\" class=\"gt_row gt_right\">0.246</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #76026a;\" class=\"gt_row gt_right\">0.246</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #610279;\" class=\"gt_row gt_right\">0.009</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #600279;\" class=\"gt_row gt_right\">0.009</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.005</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.023</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #5d027c;\" class=\"gt_row gt_right\">\u22120.023</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.001</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.007</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #620278;\" class=\"gt_row gt_right\">0.028</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Loan_Amount</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5a027e;\" class=\"gt_row gt_right\">\u22120.061</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #640277;\" class=\"gt_row gt_right\">0.040</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #610279;\" class=\"gt_row gt_right\">0.009</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #630277;\" class=\"gt_row gt_right\">0.040</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #600279;\" class=\"gt_row gt_right\">0.009</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #830261;\" class=\"gt_row gt_right\">0.380</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #42028f;\" class=\"gt_row gt_right\">\u22120.321</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #410290;\" class=\"gt_row gt_right\">\u22120.321</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #b5023d;\" class=\"gt_row gt_right\">0.917</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #7c0265;\" class=\"gt_row gt_right\">0.308</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #640277;\" class=\"gt_row gt_right\">0.047</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Loan_Period</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.007</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.004</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.005</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #830261;\" class=\"gt_row gt_right\">0.380</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #560281;\" class=\"gt_row gt_right\">\u22120.097</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #560280;\" class=\"gt_row gt_right\">\u22120.097</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #670274;\" class=\"gt_row gt_right\">0.084</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #59027e;\" class=\"gt_row gt_right\">\u22120.066</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.000</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Interest_Rate</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #70026e;\" class=\"gt_row gt_right\">0.178</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.015</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.023</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #42028f;\" class=\"gt_row gt_right\">\u22120.321</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #560281;\" class=\"gt_row gt_right\">\u22120.097</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #5d027c;\" class=\"gt_row gt_right\">\u22120.023</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #410290;\" class=\"gt_row gt_right\">\u22120.321</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #560280;\" class=\"gt_row gt_right\">\u22120.097</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #49028a;\" class=\"gt_row gt_right\">\u22120.242</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #2c029f;\" class=\"gt_row gt_right\">\u22120.554</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #560281;\" class=\"gt_row gt_right\">\u22120.094</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #570280;\" class=\"gt_row gt_right\">\u22120.094</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">EMI</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5b027d;\" class=\"gt_row gt_right\">\u22120.052</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #630278;\" class=\"gt_row gt_right\">0.035</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.001</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #b5023d;\" class=\"gt_row gt_right\">0.917</td>\n",
@@ -1516,15 +1577,15 @@
                             "<tr>\n",
                             "  <td class=\"gt_row gt_left\">Approved</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5e027b;\" class=\"gt_row gt_right\">\u22120.019</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #60027a;\" class=\"gt_row gt_right\">0.000</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #620278;\" class=\"gt_row gt_right\">0.028</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #640277;\" class=\"gt_row gt_right\">0.047</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #5f027a;\" class=\"gt_row gt_right\">\u22120.000</td>\n",
-                            "  <td style=\"color: #FFFFFF; background-color: #560281;\" class=\"gt_row gt_right\">\u22120.094</td>\n",
+                            "  <td style=\"color: #FFFFFF; background-color: #570280;\" class=\"gt_row gt_right\">\u22120.094</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #640277;\" class=\"gt_row gt_right\">0.050</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #6a0272;\" class=\"gt_row gt_right\">0.112</td>\n",
                             "  <td style=\"color: #FFFFFF; background-color: #bd0237;\" class=\"gt_row gt_right\">1.000</td>\n",
                             "</tr>\n",
                             "</tbody>\n",
                             "\n",
                             "\n",
@@ -1552,27 +1613,309 @@
                             "\u2502 Loan_Peri \u2506 -0.007449 \u2506 -0.003671 \u2506 -0.004603 \u2506 \u2026 \u2506 -0.096629 \u2506 0.083965  \u2506 -0.065702 \u2506 -0.00037 \u2502\n",
                             "\u2502 od        \u2506           \u2506           \u2506           \u2506   \u2506           \u2506           \u2506           \u2506 5        \u2502\n",
                             "\u2502 Interest_ \u2506 0.177605  \u2506 -0.014789 \u2506 -0.023001 \u2506 \u2026 \u2506 1.0       \u2506 -0.241648 \u2506 -0.554138 \u2506 -0.09438 \u2502\n",
                             "\u2502 Rate      \u2506           \u2506           \u2506           \u2506   \u2506           \u2506           \u2506           \u2506 7        \u2502\n",
                             "\u2502 EMI       \u2506 -0.051729 \u2506 0.035163  \u2506 0.000813  \u2506 \u2026 \u2506 -0.241648 \u2506 1.0       \u2506 0.293474  \u2506 0.050129 \u2502\n",
                             "\u2502 Var1      \u2506 -0.124415 \u2506 0.024854  \u2506 0.00662   \u2506 \u2026 \u2506 -0.554138 \u2506 0.293474  \u2506 1.0       \u2506 0.11244  \u2502\n",
                             "\u2502 Approved  \u2506 -0.019413 \u2506 0.000472  \u2506 0.027821  \u2506 \u2026 \u2506 -0.094387 \u2506 0.050129  \u2506 0.11244   \u2506 1.0      \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7ebd17555950>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.default: 1>, column_label='column', column_align='left', column_width=None), ColInfo(var='Employer_Category2', type=<ColInfoTypeEnum.default: 1>, column_label='Employer_Category2', column_align='right', column_width=None), ColInfo(var='Monthly_Income', type=<ColInfoTypeEnum.default: 1>, column_label='Monthly_Income', column_align='right', column_width=None), ColInfo(var='Existing_EMI', type=<ColInfoTypeEnum.default: 1>, column_label='Existing_EMI', column_align='right', column_width=None), ColInfo(var='Loan_Amount', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Amount', column_align='right', column_width=None), ColInfo(var='Loan_Period', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Period', column_align='right', column_width=None), ColInfo(var='Interest_Rate', type=<ColInfoTypeEnum.default: 1>, column_label='Interest_Rate', column_align='right', column_width=None), ColInfo(var='EMI', type=<ColInfoTypeEnum.default: 1>, column_label='EMI', column_align='right', column_width=None), ColInfo(var='Var1', type=<ColInfoTypeEnum.default: 1>, column_label='Var1', column_align='right', column_width=None), ColInfo(var='Approved', type=<ColInfoTypeEnum.default: 1>, column_label='Approved', column_align='right', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=2, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=3, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=4, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=5, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=6, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=7, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=8, group_id=None, rowname=None, group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead=None, _source_notes=[], _footnotes=[], _styles=[StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5a027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#70026e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5b027d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#540282')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#770269')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#770269')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#610279')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5a027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#610279')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#830261')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#42028f')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#b5023d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7c0265')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#830261')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#560281')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#670274')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#59027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#70026e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#42028f')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#560281')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#49028a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#2c029f')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#560281')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5b027d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#b5023d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#670274')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#49028a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7b0266')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#540282')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7c0265')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#59027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#2c029f')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7b0266')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#6a0272')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#560281')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#6a0272')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')])], _locale=<great_tables._gt_data.Locale object at 0x7ebd1755afd0>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7ebd1755ae50>], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518, _body=<great_tables._gt_data.Body object at 0x7839c45d3910>, _boxhead=Boxhead([ColInfo(var='column', type=<ColInfoTypeEnum.default: 1>, column_label='column', column_align='left', column_width=None), ColInfo(var='Employer_Category2', type=<ColInfoTypeEnum.default: 1>, column_label='Employer_Category2', column_align='right', column_width=None), ColInfo(var='Monthly_Income', type=<ColInfoTypeEnum.default: 1>, column_label='Monthly_Income', column_align='right', column_width=None), ColInfo(var='Existing_EMI', type=<ColInfoTypeEnum.default: 1>, column_label='Existing_EMI', column_align='right', column_width=None), ColInfo(var='Loan_Amount', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Amount', column_align='right', column_width=None), ColInfo(var='Loan_Period', type=<ColInfoTypeEnum.default: 1>, column_label='Loan_Period', column_align='right', column_width=None), ColInfo(var='Interest_Rate', type=<ColInfoTypeEnum.default: 1>, column_label='Interest_Rate', column_align='right', column_width=None), ColInfo(var='EMI', type=<ColInfoTypeEnum.default: 1>, column_label='EMI', column_align='right', column_width=None), ColInfo(var='Var1', type=<ColInfoTypeEnum.default: 1>, column_label='Var1', column_align='right', column_width=None), ColInfo(var='Approved', type=<ColInfoTypeEnum.default: 1>, column_label='Approved', column_align='right', column_width=None)]), _stub=Stub([RowInfo(rownum_i=0, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=1, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=2, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=3, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=4, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=5, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=6, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=7, group_id=None, rowname=None, group_label=None, built=False), RowInfo(rownum_i=8, group_id=None, rowname=None, group_label=None, built=False)]), _row_groups=[], _group_rows=GroupRows([]), _spanners=Spanners([]), _heading=Heading(title=None, subtitle=None, preheader=None), _stubhead=None, _source_notes=[], _footnotes=[], _styles=[StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5a027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#70026e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5b027d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#540282')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Employer_Category2', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#76026a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Monthly_Income', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#76026a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#600279')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5d027c')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Existing_EMI', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5a027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#600279')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#830261')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#410290')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#b5023d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7c0265')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Amount', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#830261')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#560280')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#670274')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#59027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Loan_Period', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#70026e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5d027c')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#410290')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#560280')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#49028a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#2c029f')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Interest_Rate', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#570280')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5b027d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#630278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#b5023d')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#670274')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#49028a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7b0266')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='EMI', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#540282')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7c0265')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#59027e')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#2c029f')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#7b0266')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Var1', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#6a0272')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=0, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5e027b')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=1, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#60027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=2, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#620278')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=3, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=4, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#5f027a')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=5, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#570280')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=6, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#640277')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=7, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#6a0272')]), StyleInfo(locname='data', locnum=5, grpname=None, colname='Approved', rownum=8, colnum=None, styles=[CellStyleText(color='#FFFFFF', font=None, size=None, align=None, v_align=None, style=None, weight=None, stretch=None, decorate=None, transform=None, whitespace=None), CellStyleFill(color='#bd0237')])], _locale=<great_tables._gt_data.Locale object at 0x7839c45d3d50>, _formats=[<great_tables._gt_data.FormatInfo object at 0x7839c45d3850>], _substitutions=[], _options=Options(table_id=OptionsInfo(scss=False, category='table', type='value', value=None), table_caption=OptionsInfo(scss=False, category='table', type='value', value=None), table_width=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_layout=OptionsInfo(scss=True, category='table', type='value', value='fixed'), table_margin_left=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_margin_right=OptionsInfo(scss=True, category='table', type='px', value='auto'), table_background_color=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_font_names=OptionsInfo(scss=False, category='table', type='values', value=['-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Helvetica Neue', 'Fira Sans', 'Droid Sans', 'Arial', 'sans-serif']), table_font_size=OptionsInfo(scss=True, category='table', type='px', value='16px'), table_font_weight=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_style=OptionsInfo(scss=True, category='table', type='value', value='normal'), table_font_color=OptionsInfo(scss=True, category='table', type='value', value='#333333'), table_font_color_light=OptionsInfo(scss=True, category='table', type='value', value='#FFFFFF'), table_border_top_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_top_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_top_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_top_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_right_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_right_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_right_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), table_border_bottom_include=OptionsInfo(scss=False, category='table', type='boolean', value=True), table_border_bottom_style=OptionsInfo(scss=True, category='table', type='value', value='solid'), table_border_bottom_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_bottom_color=OptionsInfo(scss=True, category='table', type='value', value='#A8A8A8'), table_border_left_style=OptionsInfo(scss=True, category='table', type='value', value='none'), table_border_left_width=OptionsInfo(scss=True, category='table', type='px', value='2px'), table_border_left_color=OptionsInfo(scss=True, category='table', type='value', value='#D3D3D3'), heading_background_color=OptionsInfo(scss=True, category='heading', type='value', value=None), heading_align=OptionsInfo(scss=True, category='heading', type='value', value='center'), heading_title_font_size=OptionsInfo(scss=True, category='heading', type='px', value='125%'), heading_title_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_subtitle_font_size=OptionsInfo(scss=True, category='heading', type='px', value='85%'), heading_subtitle_font_weight=OptionsInfo(scss=True, category='heading', type='value', value='initial'), heading_padding=OptionsInfo(scss=True, category='heading', type='px', value='4px'), heading_padding_horizontal=OptionsInfo(scss=True, category='heading', type='px', value='5px'), heading_border_bottom_style=OptionsInfo(scss=True, category='heading', type='value', value='solid'), heading_border_bottom_width=OptionsInfo(scss=True, category='heading', type='px', value='2px'), heading_border_bottom_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), heading_border_lr_style=OptionsInfo(scss=True, category='heading', type='value', value='none'), heading_border_lr_width=OptionsInfo(scss=True, category='heading', type='px', value='1px'), heading_border_lr_color=OptionsInfo(scss=True, category='heading', type='value', value='#D3D3D3'), column_labels_background_color=OptionsInfo(scss=True, category='column_labels', type='value', value=None), column_labels_font_size=OptionsInfo(scss=True, category='column_labels', type='px', value='100%'), column_labels_font_weight=OptionsInfo(scss=True, category='column_labels', type='value', value='normal'), column_labels_text_transform=OptionsInfo(scss=True, category='column_labels', type='value', value='inherit'), column_labels_padding=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_padding_horizontal=OptionsInfo(scss=True, category='column_labels', type='px', value='5px'), column_labels_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), column_labels_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), column_labels_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), column_labels_border_top_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_top_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_top_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_bottom_style=OptionsInfo(scss=True, category='column_labels', type='value', value='solid'), column_labels_border_bottom_width=OptionsInfo(scss=True, category='column_labels', type='px', value='2px'), column_labels_border_bottom_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_border_lr_style=OptionsInfo(scss=True, category='column_labels', type='value', value='none'), column_labels_border_lr_width=OptionsInfo(scss=True, category='column_labels', type='px', value='1px'), column_labels_border_lr_color=OptionsInfo(scss=True, category='column_labels', type='value', value='#D3D3D3'), column_labels_hidden=OptionsInfo(scss=False, category='column_labels', type='boolean', value=False), row_group_background_color=OptionsInfo(scss=True, category='row_group', type='value', value=None), row_group_font_size=OptionsInfo(scss=True, category='row_group', type='px', value='100%'), row_group_font_weight=OptionsInfo(scss=True, category='row_group', type='value', value='initial'), row_group_text_transform=OptionsInfo(scss=True, category='row_group', type='value', value='inherit'), row_group_padding=OptionsInfo(scss=True, category='row_group', type='px', value='8px'), row_group_padding_horizontal=OptionsInfo(scss=True, category='row_group', type='px', value='5px'), row_group_border_top_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_top_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_top_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_right_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_right_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_right_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_bottom_style=OptionsInfo(scss=True, category='row_group', type='value', value='solid'), row_group_border_bottom_width=OptionsInfo(scss=True, category='row_group', type='px', value='2px'), row_group_border_bottom_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_border_left_style=OptionsInfo(scss=True, category='row_group', type='value', value='none'), row_group_border_left_width=OptionsInfo(scss=True, category='row_group', type='px', value='1px'), row_group_border_left_color=OptionsInfo(scss=True, category='row_group', type='value', value='#D3D3D3'), row_group_as_column=OptionsInfo(scss=False, category='row_group', type='boolean', value=False), table_body_hlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_hlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_hlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_vlines_style=OptionsInfo(scss=True, category='table_body', type='value', value='none'), table_body_vlines_width=OptionsInfo(scss=True, category='table_body', type='px', value='1px'), table_body_vlines_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_top_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_top_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_top_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), table_body_border_bottom_style=OptionsInfo(scss=True, category='table_body', type='value', value='solid'), table_body_border_bottom_width=OptionsInfo(scss=True, category='table_body', type='px', value='2px'), table_body_border_bottom_color=OptionsInfo(scss=True, category='table_body', type='value', value='#D3D3D3'), data_row_padding=OptionsInfo(scss=True, category='data_row', type='px', value='8px'), data_row_padding_horizontal=OptionsInfo(scss=True, category='data_row', type='px', value='5px'), stub_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), stub_row_group_background_color=OptionsInfo(scss=True, category='stub', type='value', value=None), stub_row_group_font_size=OptionsInfo(scss=True, category='stub', type='px', value='100%'), stub_row_group_font_weight=OptionsInfo(scss=True, category='stub', type='value', value='initial'), stub_row_group_text_transform=OptionsInfo(scss=True, category='stub', type='value', value='inherit'), stub_row_group_border_style=OptionsInfo(scss=True, category='stub', type='value', value='solid'), stub_row_group_border_width=OptionsInfo(scss=True, category='stub', type='px', value='2px'), stub_row_group_border_color=OptionsInfo(scss=True, category='stub', type='value', value='#D3D3D3'), source_notes_padding=OptionsInfo(scss=True, category='source_notes', type='px', value='4px'), source_notes_padding_horizontal=OptionsInfo(scss=True, category='source_notes', type='px', value='5px'), source_notes_background_color=OptionsInfo(scss=True, category='source_notes', type='value', value=None), source_notes_font_size=OptionsInfo(scss=True, category='source_notes', type='px', value='90%'), source_notes_border_bottom_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_bottom_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_bottom_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_border_lr_style=OptionsInfo(scss=True, category='source_notes', type='value', value='none'), source_notes_border_lr_width=OptionsInfo(scss=True, category='source_notes', type='px', value='2px'), source_notes_border_lr_color=OptionsInfo(scss=True, category='source_notes', type='value', value='#D3D3D3'), source_notes_multiline=OptionsInfo(scss=False, category='source_notes', type='boolean', value=True), source_notes_sep=OptionsInfo(scss=False, category='source_notes', type='value', value=' '), container_width=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_height=OptionsInfo(scss=False, category='container', type='px', value='auto'), container_padding_x=OptionsInfo(scss=False, category='container', type='px', value='0px'), container_padding_y=OptionsInfo(scss=False, category='container', type='px', value='10px'), container_overflow_x=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), container_overflow_y=OptionsInfo(scss=False, category='container', type='overflow', value='auto'), quarto_disable_processing=OptionsInfo(scss=False, category='quarto', type='logical', value=False), quarto_use_bootstrap=OptionsInfo(scss=False, category='quarto', type='logical', value=False)), _has_built=False)"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dia.plot_corr(subset=cs.all())"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Classic Iris Dataset\n",
+                "\n",
+                "Need sklearn to download the dataset and that's it."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div><style>\n",
+                            ".dataframe > thead > tr,\n",
+                            ".dataframe > tbody > tr {\n",
+                            "  text-align: right;\n",
+                            "  white-space: pre-wrap;\n",
+                            "}\n",
+                            "</style>\n",
+                            "<small>shape: (5, 5)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sepal length (cm)</th><th>sepal width (cm)</th><th>petal length (cm)</th><th>petal width (cm)</th><th>species</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>5.1</td><td>3.5</td><td>1.4</td><td>0.2</td><td>&quot;setosa&quot;</td></tr><tr><td>4.9</td><td>3.0</td><td>1.4</td><td>0.2</td><td>&quot;setosa&quot;</td></tr><tr><td>4.7</td><td>3.2</td><td>1.3</td><td>0.2</td><td>&quot;setosa&quot;</td></tr><tr><td>4.6</td><td>3.1</td><td>1.5</td><td>0.2</td><td>&quot;setosa&quot;</td></tr><tr><td>5.0</td><td>3.6</td><td>1.4</td><td>0.2</td><td>&quot;setosa&quot;</td></tr></tbody></table></div>"
+                        ],
+                        "text/plain": [
+                            "shape: (5, 5)\n",
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 sepal length (cm) \u2506 sepal width (cm) \u2506 petal length (cm) \u2506 petal width (cm) \u2506 species \u2502\n",
+                            "\u2502 ---               \u2506 ---              \u2506 ---               \u2506 ---              \u2506 ---     \u2502\n",
+                            "\u2502 f64               \u2506 f64              \u2506 f64               \u2506 f64              \u2506 str     \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 5.1               \u2506 3.5              \u2506 1.4               \u2506 0.2              \u2506 setosa  \u2502\n",
+                            "\u2502 4.9               \u2506 3.0              \u2506 1.4               \u2506 0.2              \u2506 setosa  \u2502\n",
+                            "\u2502 4.7               \u2506 3.2              \u2506 1.3               \u2506 0.2              \u2506 setosa  \u2502\n",
+                            "\u2502 4.6               \u2506 3.1              \u2506 1.5               \u2506 0.2              \u2506 setosa  \u2502\n",
+                            "\u2502 5.0               \u2506 3.6              \u2506 1.4               \u2506 0.2              \u2506 setosa  \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                        ]
+                    },
+                    "execution_count": 19,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from sklearn import datasets\n",
+                "dataset = datasets.load_iris()\n",
+                "df = pl.from_numpy(dataset.data, schema = dataset.feature_names).with_columns(\n",
+                "    pl.Series(values=dataset.target).alias(\"species\")\n",
+                ").with_columns(\n",
+                "    pl.col(\"species\").replace(old=[0,1,2], new=dataset.target_names)\n",
+                ")\n",
+                "df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 20,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "%opts magic unavailable (pyparsing cannot be imported)\n",
+                        "%compositor magic unavailable (pyparsing cannot be imported)\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "application/javascript": "(function(root) {\n  function now() {\n    return new Date();\n  }\n\n  var force = true;\n  var py_version = '3.4.1'.replace('rc', '-rc.').replace('.dev', '-dev.');\n  var reloading = false;\n  var Bokeh = root.Bokeh;\n\n  if (typeof (root._bokeh_timeout) === \"undefined\" || force) {\n    root._bokeh_timeout = Date.now() + 5000;\n    root._bokeh_failed_load = false;\n  }\n\n  function run_callbacks() {\n    try {\n      root._bokeh_onload_callbacks.forEach(function(callback) {\n        if (callback != null)\n          callback();\n      });\n    } finally {\n      delete root._bokeh_onload_callbacks;\n    }\n    console.debug(\"Bokeh: all callbacks have finished\");\n  }\n\n  function load_libs(css_urls, js_urls, js_modules, js_exports, callback) {\n    if (css_urls == null) css_urls = [];\n    if (js_urls == null) js_urls = [];\n    if (js_modules == null) js_modules = [];\n    if (js_exports == null) js_exports = {};\n\n    root._bokeh_onload_callbacks.push(callback);\n\n    if (root._bokeh_is_loading > 0) {\n      console.debug(\"Bokeh: BokehJS is being loaded, scheduling callback at\", now());\n      return null;\n    }\n    if (js_urls.length === 0 && js_modules.length === 0 && Object.keys(js_exports).length === 0) {\n      run_callbacks();\n      return null;\n    }\n    if (!reloading) {\n      console.debug(\"Bokeh: BokehJS not loaded, scheduling load and callback at\", now());\n    }\n\n    function on_load() {\n      root._bokeh_is_loading--;\n      if (root._bokeh_is_loading === 0) {\n        console.debug(\"Bokeh: all BokehJS libraries/stylesheets loaded\");\n        run_callbacks()\n      }\n    }\n    window._bokeh_on_load = on_load\n\n    function on_error() {\n      console.error(\"failed to load \" + url);\n    }\n\n    var skip = [];\n    if (window.requirejs) {\n      window.requirejs.config({'packages': {}, 'paths': {}, 'shim': {}});\n      root._bokeh_is_loading = css_urls.length + 0;\n    } else {\n      root._bokeh_is_loading = css_urls.length + js_urls.length + js_modules.length + Object.keys(js_exports).length;\n    }\n\n    var existing_stylesheets = []\n    var links = document.getElementsByTagName('link')\n    for (var i = 0; i < links.length; i++) {\n      var link = links[i]\n      if (link.href != null) {\n\texisting_stylesheets.push(link.href)\n      }\n    }\n    for (var i = 0; i < css_urls.length; i++) {\n      var url = css_urls[i];\n      if (existing_stylesheets.indexOf(url) !== -1) {\n\ton_load()\n\tcontinue;\n      }\n      const element = document.createElement(\"link\");\n      element.onload = on_load;\n      element.onerror = on_error;\n      element.rel = \"stylesheet\";\n      element.type = \"text/css\";\n      element.href = url;\n      console.debug(\"Bokeh: injecting link tag for BokehJS stylesheet: \", url);\n      document.body.appendChild(element);\n    }    var existing_scripts = []\n    var scripts = document.getElementsByTagName('script')\n    for (var i = 0; i < scripts.length; i++) {\n      var script = scripts[i]\n      if (script.src != null) {\n\texisting_scripts.push(script.src)\n      }\n    }\n    for (var i = 0; i < js_urls.length; i++) {\n      var url = js_urls[i];\n      if (skip.indexOf(url) !== -1 || existing_scripts.indexOf(url) !== -1) {\n\tif (!window.requirejs) {\n\t  on_load();\n\t}\n\tcontinue;\n      }\n      var element = document.createElement('script');\n      element.onload = on_load;\n      element.onerror = on_error;\n      element.async = false;\n      element.src = url;\n      console.debug(\"Bokeh: injecting script tag for BokehJS library: \", url);\n      document.head.appendChild(element);\n    }\n    for (var i = 0; i < js_modules.length; i++) {\n      var url = js_modules[i];\n      if (skip.indexOf(url) !== -1 || existing_scripts.indexOf(url) !== -1) {\n\tif (!window.requirejs) {\n\t  on_load();\n\t}\n\tcontinue;\n      }\n      var element = document.createElement('script');\n      element.onload = on_load;\n      element.onerror = on_error;\n      element.async = false;\n      element.src = url;\n      element.type = \"module\";\n      console.debug(\"Bokeh: injecting script tag for BokehJS library: \", url);\n      document.head.appendChild(element);\n    }\n    for (const name in js_exports) {\n      var url = js_exports[name];\n      if (skip.indexOf(url) >= 0 || root[name] != null) {\n\tif (!window.requirejs) {\n\t  on_load();\n\t}\n\tcontinue;\n      }\n      var element = document.createElement('script');\n      element.onerror = on_error;\n      element.async = false;\n      element.type = \"module\";\n      console.debug(\"Bokeh: injecting script tag for BokehJS library: \", url);\n      element.textContent = `\n      import ${name} from \"${url}\"\n      window.${name} = ${name}\n      window._bokeh_on_load()\n      `\n      document.head.appendChild(element);\n    }\n    if (!js_urls.length && !js_modules.length) {\n      on_load()\n    }\n  };\n\n  function inject_raw_css(css) {\n    const element = document.createElement(\"style\");\n    element.appendChild(document.createTextNode(css));\n    document.body.appendChild(element);\n  }\n\n  var js_urls = [\"https://cdn.bokeh.org/bokeh/release/bokeh-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-gl-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-widgets-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-tables-3.4.1.min.js\", \"https://cdn.holoviz.org/panel/1.4.1/dist/panel.min.js\"];\n  var js_modules = [];\n  var js_exports = {};\n  var css_urls = [];\n  var inline_js = [    function(Bokeh) {\n      Bokeh.set_log_level(\"info\");\n    },\nfunction(Bokeh) {} // ensure no trailing comma for IE\n  ];\n\n  function run_inline_js() {\n    if ((root.Bokeh !== undefined) || (force === true)) {\n      for (var i = 0; i < inline_js.length; i++) {\n\ttry {\n          inline_js[i].call(root, root.Bokeh);\n\t} catch(e) {\n\t  if (!reloading) {\n\t    throw e;\n\t  }\n\t}\n      }\n      // Cache old bokeh versions\n      if (Bokeh != undefined && !reloading) {\n\tvar NewBokeh = root.Bokeh;\n\tif (Bokeh.versions === undefined) {\n\t  Bokeh.versions = new Map();\n\t}\n\tif (NewBokeh.version !== Bokeh.version) {\n\t  Bokeh.versions.set(NewBokeh.version, NewBokeh)\n\t}\n\troot.Bokeh = Bokeh;\n      }} else if (Date.now() < root._bokeh_timeout) {\n      setTimeout(run_inline_js, 100);\n    } else if (!root._bokeh_failed_load) {\n      console.log(\"Bokeh: BokehJS failed to load within specified timeout.\");\n      root._bokeh_failed_load = true;\n    }\n    root._bokeh_is_initializing = false\n  }\n\n  function load_or_wait() {\n    // Implement a backoff loop that tries to ensure we do not load multiple\n    // versions of Bokeh and its dependencies at the same time.\n    // In recent versions we use the root._bokeh_is_initializing flag\n    // to determine whether there is an ongoing attempt to initialize\n    // bokeh, however for backward compatibility we also try to ensure\n    // that we do not start loading a newer (Panel>=1.0 and Bokeh>3) version\n    // before older versions are fully initialized.\n    if (root._bokeh_is_initializing && Date.now() > root._bokeh_timeout) {\n      root._bokeh_is_initializing = false;\n      root._bokeh_onload_callbacks = undefined;\n      console.log(\"Bokeh: BokehJS was loaded multiple times but one version failed to initialize.\");\n      load_or_wait();\n    } else if (root._bokeh_is_initializing || (typeof root._bokeh_is_initializing === \"undefined\" && root._bokeh_onload_callbacks !== undefined)) {\n      setTimeout(load_or_wait, 100);\n    } else {\n      root._bokeh_is_initializing = true\n      root._bokeh_onload_callbacks = []\n      var bokeh_loaded = Bokeh != null && (Bokeh.version === py_version || (Bokeh.versions !== undefined && Bokeh.versions.has(py_version)));\n      if (!reloading && !bokeh_loaded) {\n\troot.Bokeh = undefined;\n      }\n      load_libs(css_urls, js_urls, js_modules, js_exports, function() {\n\tconsole.debug(\"Bokeh: BokehJS plotting callback run at\", now());\n\trun_inline_js();\n      });\n    }\n  }\n  // Give older versions of the autoload script a head-start to ensure\n  // they initialize before we start loading newer version.\n  setTimeout(load_or_wait, 100)\n}(window));",
+                        "application/vnd.holoviews_load.v0+json": ""
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "application/javascript": "\nif ((window.PyViz === undefined) || (window.PyViz instanceof HTMLElement)) {\n  window.PyViz = {comms: {}, comm_status:{}, kernels:{}, receivers: {}, plot_index: []}\n}\n\n\n    function JupyterCommManager() {\n    }\n\n    JupyterCommManager.prototype.register_target = function(plot_id, comm_id, msg_handler) {\n      if (window.comm_manager || ((window.Jupyter !== undefined) && (Jupyter.notebook.kernel != null))) {\n        var comm_manager = window.comm_manager || Jupyter.notebook.kernel.comm_manager;\n        comm_manager.register_target(comm_id, function(comm) {\n          comm.on_msg(msg_handler);\n        });\n      } else if ((plot_id in window.PyViz.kernels) && (window.PyViz.kernels[plot_id])) {\n        window.PyViz.kernels[plot_id].registerCommTarget(comm_id, function(comm) {\n          comm.onMsg = msg_handler;\n        });\n      } else if (typeof google != 'undefined' && google.colab.kernel != null) {\n        google.colab.kernel.comms.registerTarget(comm_id, (comm) => {\n          var messages = comm.messages[Symbol.asyncIterator]();\n          function processIteratorResult(result) {\n            var message = result.value;\n            console.log(message)\n            var content = {data: message.data, comm_id};\n            var buffers = []\n            for (var buffer of message.buffers || []) {\n              buffers.push(new DataView(buffer))\n            }\n            var metadata = message.metadata || {};\n            var msg = {content, buffers, metadata}\n            msg_handler(msg);\n            return messages.next().then(processIteratorResult);\n          }\n          return messages.next().then(processIteratorResult);\n        })\n      }\n    }\n\n    JupyterCommManager.prototype.get_client_comm = function(plot_id, comm_id, msg_handler) {\n      if (comm_id in window.PyViz.comms) {\n        return window.PyViz.comms[comm_id];\n      } else if (window.comm_manager || ((window.Jupyter !== undefined) && (Jupyter.notebook.kernel != null))) {\n        var comm_manager = window.comm_manager || Jupyter.notebook.kernel.comm_manager;\n        var comm = comm_manager.new_comm(comm_id, {}, {}, {}, comm_id);\n        if (msg_handler) {\n          comm.on_msg(msg_handler);\n        }\n      } else if ((plot_id in window.PyViz.kernels) && (window.PyViz.kernels[plot_id])) {\n        var comm = window.PyViz.kernels[plot_id].connectToComm(comm_id);\n        comm.open();\n        if (msg_handler) {\n          comm.onMsg = msg_handler;\n        }\n      } else if (typeof google != 'undefined' && google.colab.kernel != null) {\n        var comm_promise = google.colab.kernel.comms.open(comm_id)\n        comm_promise.then((comm) => {\n          window.PyViz.comms[comm_id] = comm;\n          if (msg_handler) {\n            var messages = comm.messages[Symbol.asyncIterator]();\n            function processIteratorResult(result) {\n              var message = result.value;\n              var content = {data: message.data};\n              var metadata = message.metadata || {comm_id};\n              var msg = {content, metadata}\n              msg_handler(msg);\n              return messages.next().then(processIteratorResult);\n            }\n            return messages.next().then(processIteratorResult);\n          }\n        }) \n        var sendClosure = (data, metadata, buffers, disposeOnDone) => {\n          return comm_promise.then((comm) => {\n            comm.send(data, metadata, buffers, disposeOnDone);\n          });\n        };\n        var comm = {\n          send: sendClosure\n        };\n      }\n      window.PyViz.comms[comm_id] = comm;\n      return comm;\n    }\n    window.PyViz.comm_manager = new JupyterCommManager();\n    \n\n\nvar JS_MIME_TYPE = 'application/javascript';\nvar HTML_MIME_TYPE = 'text/html';\nvar EXEC_MIME_TYPE = 'application/vnd.holoviews_exec.v0+json';\nvar CLASS_NAME = 'output';\n\n/**\n * Render data to the DOM node\n */\nfunction render(props, node) {\n  var div = document.createElement(\"div\");\n  var script = document.createElement(\"script\");\n  node.appendChild(div);\n  node.appendChild(script);\n}\n\n/**\n * Handle when a new output is added\n */\nfunction handle_add_output(event, handle) {\n  var output_area = handle.output_area;\n  var output = handle.output;\n  if ((output.data == undefined) || (!output.data.hasOwnProperty(EXEC_MIME_TYPE))) {\n    return\n  }\n  var id = output.metadata[EXEC_MIME_TYPE][\"id\"];\n  var toinsert = output_area.element.find(\".\" + CLASS_NAME.split(' ')[0]);\n  if (id !== undefined) {\n    var nchildren = toinsert.length;\n    var html_node = toinsert[nchildren-1].children[0];\n    html_node.innerHTML = output.data[HTML_MIME_TYPE];\n    var scripts = [];\n    var nodelist = html_node.querySelectorAll(\"script\");\n    for (var i in nodelist) {\n      if (nodelist.hasOwnProperty(i)) {\n        scripts.push(nodelist[i])\n      }\n    }\n\n    scripts.forEach( function (oldScript) {\n      var newScript = document.createElement(\"script\");\n      var attrs = [];\n      var nodemap = oldScript.attributes;\n      for (var j in nodemap) {\n        if (nodemap.hasOwnProperty(j)) {\n          attrs.push(nodemap[j])\n        }\n      }\n      attrs.forEach(function(attr) { newScript.setAttribute(attr.name, attr.value) });\n      newScript.appendChild(document.createTextNode(oldScript.innerHTML));\n      oldScript.parentNode.replaceChild(newScript, oldScript);\n    });\n    if (JS_MIME_TYPE in output.data) {\n      toinsert[nchildren-1].children[1].textContent = output.data[JS_MIME_TYPE];\n    }\n    output_area._hv_plot_id = id;\n    if ((window.Bokeh !== undefined) && (id in Bokeh.index)) {\n      window.PyViz.plot_index[id] = Bokeh.index[id];\n    } else {\n      window.PyViz.plot_index[id] = null;\n    }\n  } else if (output.metadata[EXEC_MIME_TYPE][\"server_id\"] !== undefined) {\n    var bk_div = document.createElement(\"div\");\n    bk_div.innerHTML = output.data[HTML_MIME_TYPE];\n    var script_attrs = bk_div.children[0].attributes;\n    for (var i = 0; i < script_attrs.length; i++) {\n      toinsert[toinsert.length - 1].childNodes[1].setAttribute(script_attrs[i].name, script_attrs[i].value);\n    }\n    // store reference to server id on output_area\n    output_area._bokeh_server_id = output.metadata[EXEC_MIME_TYPE][\"server_id\"];\n  }\n}\n\n/**\n * Handle when an output is cleared or removed\n */\nfunction handle_clear_output(event, handle) {\n  var id = handle.cell.output_area._hv_plot_id;\n  var server_id = handle.cell.output_area._bokeh_server_id;\n  if (((id === undefined) || !(id in PyViz.plot_index)) && (server_id !== undefined)) { return; }\n  var comm = window.PyViz.comm_manager.get_client_comm(\"hv-extension-comm\", \"hv-extension-comm\", function () {});\n  if (server_id !== null) {\n    comm.send({event_type: 'server_delete', 'id': server_id});\n    return;\n  } else if (comm !== null) {\n    comm.send({event_type: 'delete', 'id': id});\n  }\n  delete PyViz.plot_index[id];\n  if ((window.Bokeh !== undefined) & (id in window.Bokeh.index)) {\n    var doc = window.Bokeh.index[id].model.document\n    doc.clear();\n    const i = window.Bokeh.documents.indexOf(doc);\n    if (i > -1) {\n      window.Bokeh.documents.splice(i, 1);\n    }\n  }\n}\n\n/**\n * Handle kernel restart event\n */\nfunction handle_kernel_cleanup(event, handle) {\n  delete PyViz.comms[\"hv-extension-comm\"];\n  window.PyViz.plot_index = {}\n}\n\n/**\n * Handle update_display_data messages\n */\nfunction handle_update_output(event, handle) {\n  handle_clear_output(event, {cell: {output_area: handle.output_area}})\n  handle_add_output(event, handle)\n}\n\nfunction register_renderer(events, OutputArea) {\n  function append_mime(data, metadata, element) {\n    // create a DOM node to render to\n    var toinsert = this.create_output_subarea(\n    metadata,\n    CLASS_NAME,\n    EXEC_MIME_TYPE\n    );\n    this.keyboard_manager.register_events(toinsert);\n    // Render to node\n    var props = {data: data, metadata: metadata[EXEC_MIME_TYPE]};\n    render(props, toinsert[0]);\n    element.append(toinsert);\n    return toinsert\n  }\n\n  events.on('output_added.OutputArea', handle_add_output);\n  events.on('output_updated.OutputArea', handle_update_output);\n  events.on('clear_output.CodeCell', handle_clear_output);\n  events.on('delete.Cell', handle_clear_output);\n  events.on('kernel_ready.Kernel', handle_kernel_cleanup);\n\n  OutputArea.prototype.register_mime_type(EXEC_MIME_TYPE, append_mime, {\n    safe: true,\n    index: 0\n  });\n}\n\nif (window.Jupyter !== undefined) {\n  try {\n    var events = require('base/js/events');\n    var OutputArea = require('notebook/js/outputarea').OutputArea;\n    if (OutputArea.prototype.mime_types().indexOf(EXEC_MIME_TYPE) == -1) {\n      register_renderer(events, OutputArea);\n    }\n  } catch(err) {\n  }\n}\n",
+                        "application/vnd.holoviews_load.v0+json": ""
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<style>*[data-root-id],\n",
+                            "*[data-root-id] > * {\n",
+                            "  box-sizing: border-box;\n",
+                            "  font-family: var(--jp-ui-font-family);\n",
+                            "  font-size: var(--jp-ui-font-size1);\n",
+                            "  color: var(--vscode-editor-foreground, var(--jp-ui-font-color1));\n",
+                            "}\n",
+                            "\n",
+                            "/* Override VSCode background color */\n",
+                            ".cell-output-ipywidget-background:has(\n",
+                            "    > .cell-output-ipywidget-background > .lm-Widget > *[data-root-id]\n",
+                            "  ),\n",
+                            ".cell-output-ipywidget-background:has(> .lm-Widget > *[data-root-id]) {\n",
+                            "  background-color: transparent !important;\n",
+                            "}\n",
+                            "</style>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "application/vnd.holoviews_exec.v0+json": "",
+                        "text/html": [
+                            "<div id='p1002'>\n",
+                            "  <div id=\"d1c42be5-7857-4628-9451-30ad5e3d1ba2\" data-root-id=\"p1002\" style=\"display: contents;\"></div>\n",
+                            "</div>\n",
+                            "<script type=\"application/javascript\">(function(root) {\n",
+                            "  var docs_json = {\"88ffc8b6-069d-4041-ac36-6f195d03af78\":{\"version\":\"3.4.1\",\"title\":\"Bokeh Application\",\"roots\":[{\"type\":\"object\",\"name\":\"panel.models.browser.BrowserInfo\",\"id\":\"p1002\"},{\"type\":\"object\",\"name\":\"panel.models.comm_manager.CommManager\",\"id\":\"p1003\",\"attributes\":{\"plot_id\":\"p1002\",\"comm_id\":\"3b41d43c08254c24abae5ef46be825ed\",\"client_comm_id\":\"b91d6a9d22ca47c18589690a8291424c\"}}],\"defs\":[{\"type\":\"model\",\"name\":\"ReactiveHTML1\"},{\"type\":\"model\",\"name\":\"FlexBox1\",\"properties\":[{\"name\":\"align_content\",\"kind\":\"Any\",\"default\":\"flex-start\"},{\"name\":\"align_items\",\"kind\":\"Any\",\"default\":\"flex-start\"},{\"name\":\"flex_direction\",\"kind\":\"Any\",\"default\":\"row\"},{\"name\":\"flex_wrap\",\"kind\":\"Any\",\"default\":\"wrap\"},{\"name\":\"gap\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"justify_content\",\"kind\":\"Any\",\"default\":\"flex-start\"}]},{\"type\":\"model\",\"name\":\"FloatPanel1\",\"properties\":[{\"name\":\"config\",\"kind\":\"Any\",\"default\":{\"type\":\"map\"}},{\"name\":\"contained\",\"kind\":\"Any\",\"default\":true},{\"name\":\"position\",\"kind\":\"Any\",\"default\":\"right-top\"},{\"name\":\"offsetx\",\"kind\":\"Any\",\"default\":null},{\"name\":\"offsety\",\"kind\":\"Any\",\"default\":null},{\"name\":\"theme\",\"kind\":\"Any\",\"default\":\"primary\"},{\"name\":\"status\",\"kind\":\"Any\",\"default\":\"normalized\"}]},{\"type\":\"model\",\"name\":\"GridStack1\",\"properties\":[{\"name\":\"mode\",\"kind\":\"Any\",\"default\":\"warn\"},{\"name\":\"ncols\",\"kind\":\"Any\",\"default\":null},{\"name\":\"nrows\",\"kind\":\"Any\",\"default\":null},{\"name\":\"allow_resize\",\"kind\":\"Any\",\"default\":true},{\"name\":\"allow_drag\",\"kind\":\"Any\",\"default\":true},{\"name\":\"state\",\"kind\":\"Any\",\"default\":[]}]},{\"type\":\"model\",\"name\":\"drag1\",\"properties\":[{\"name\":\"slider_width\",\"kind\":\"Any\",\"default\":5},{\"name\":\"slider_color\",\"kind\":\"Any\",\"default\":\"black\"},{\"name\":\"value\",\"kind\":\"Any\",\"default\":50}]},{\"type\":\"model\",\"name\":\"click1\",\"properties\":[{\"name\":\"terminal_output\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"debug_name\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"clears\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"FastWrapper1\",\"properties\":[{\"name\":\"object\",\"kind\":\"Any\",\"default\":null},{\"name\":\"style\",\"kind\":\"Any\",\"default\":null}]},{\"type\":\"model\",\"name\":\"NotificationAreaBase1\",\"properties\":[{\"name\":\"js_events\",\"kind\":\"Any\",\"default\":{\"type\":\"map\"}},{\"name\":\"position\",\"kind\":\"Any\",\"default\":\"bottom-right\"},{\"name\":\"_clear\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"NotificationArea1\",\"properties\":[{\"name\":\"js_events\",\"kind\":\"Any\",\"default\":{\"type\":\"map\"}},{\"name\":\"notifications\",\"kind\":\"Any\",\"default\":[]},{\"name\":\"position\",\"kind\":\"Any\",\"default\":\"bottom-right\"},{\"name\":\"_clear\",\"kind\":\"Any\",\"default\":0},{\"name\":\"types\",\"kind\":\"Any\",\"default\":[{\"type\":\"map\",\"entries\":[[\"type\",\"warning\"],[\"background\",\"#ffc107\"],[\"icon\",{\"type\":\"map\",\"entries\":[[\"className\",\"fas fa-exclamation-triangle\"],[\"tagName\",\"i\"],[\"color\",\"white\"]]}]]},{\"type\":\"map\",\"entries\":[[\"type\",\"info\"],[\"background\",\"#007bff\"],[\"icon\",{\"type\":\"map\",\"entries\":[[\"className\",\"fas fa-info-circle\"],[\"tagName\",\"i\"],[\"color\",\"white\"]]}]]}]}]},{\"type\":\"model\",\"name\":\"Notification\",\"properties\":[{\"name\":\"background\",\"kind\":\"Any\",\"default\":null},{\"name\":\"duration\",\"kind\":\"Any\",\"default\":3000},{\"name\":\"icon\",\"kind\":\"Any\",\"default\":null},{\"name\":\"message\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"notification_type\",\"kind\":\"Any\",\"default\":null},{\"name\":\"_destroyed\",\"kind\":\"Any\",\"default\":false}]},{\"type\":\"model\",\"name\":\"TemplateActions1\",\"properties\":[{\"name\":\"open_modal\",\"kind\":\"Any\",\"default\":0},{\"name\":\"close_modal\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"BootstrapTemplateActions1\",\"properties\":[{\"name\":\"open_modal\",\"kind\":\"Any\",\"default\":0},{\"name\":\"close_modal\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"TemplateEditor1\",\"properties\":[{\"name\":\"layout\",\"kind\":\"Any\",\"default\":[]}]},{\"type\":\"model\",\"name\":\"MaterialTemplateActions1\",\"properties\":[{\"name\":\"open_modal\",\"kind\":\"Any\",\"default\":0},{\"name\":\"close_modal\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"copy_to_clipboard1\",\"properties\":[{\"name\":\"fill\",\"kind\":\"Any\",\"default\":\"none\"},{\"name\":\"value\",\"kind\":\"Any\",\"default\":null}]}]}};\n",
+                            "  var render_items = [{\"docid\":\"88ffc8b6-069d-4041-ac36-6f195d03af78\",\"roots\":{\"p1002\":\"d1c42be5-7857-4628-9451-30ad5e3d1ba2\"},\"root_ids\":[\"p1002\"]}];\n",
+                            "  var docs = Object.values(docs_json)\n",
+                            "  if (!docs) {\n",
+                            "    return\n",
+                            "  }\n",
+                            "  const py_version = docs[0].version.replace('rc', '-rc.').replace('.dev', '-dev.')\n",
+                            "  function embed_document(root) {\n",
+                            "    var Bokeh = get_bokeh(root)\n",
+                            "    Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
+                            "    for (const render_item of render_items) {\n",
+                            "      for (const root_id of render_item.root_ids) {\n",
+                            "\tconst id_el = document.getElementById(root_id)\n",
+                            "\tif (id_el.children.length && (id_el.children[0].className === 'bk-root')) {\n",
+                            "\t  const root_el = id_el.children[0]\n",
+                            "\t  root_el.id = root_el.id + '-rendered'\n",
+                            "\t}\n",
+                            "      }\n",
+                            "    }\n",
+                            "  }\n",
+                            "  function get_bokeh(root) {\n",
+                            "    if (root.Bokeh === undefined) {\n",
+                            "      return null\n",
+                            "    } else if (root.Bokeh.version !== py_version) {\n",
+                            "      if (root.Bokeh.versions === undefined || !root.Bokeh.versions.has(py_version)) {\n",
+                            "\treturn null\n",
+                            "      }\n",
+                            "      return root.Bokeh.versions.get(py_version);\n",
+                            "    } else if (root.Bokeh.version === py_version) {\n",
+                            "      return root.Bokeh\n",
+                            "    }\n",
+                            "    return null\n",
+                            "  }\n",
+                            "  function is_loaded(root) {\n",
+                            "    var Bokeh = get_bokeh(root)\n",
+                            "    return (Bokeh != null && Bokeh.Panel !== undefined)\n",
+                            "  }\n",
+                            "  if (is_loaded(root)) {\n",
+                            "    embed_document(root);\n",
+                            "  } else {\n",
+                            "    var attempts = 0;\n",
+                            "    var timer = setInterval(function(root) {\n",
+                            "      if (is_loaded(root)) {\n",
+                            "        clearInterval(timer);\n",
+                            "        embed_document(root);\n",
+                            "      } else if (document.readyState == \"complete\") {\n",
+                            "        attempts++;\n",
+                            "        if (attempts > 200) {\n",
+                            "          clearInterval(timer);\n",
+                            "\t  var Bokeh = get_bokeh(root)\n",
+                            "\t  if (Bokeh == null || Bokeh.Panel == null) {\n",
+                            "            console.warn(\"Panel: ERROR: Unable to run Panel code because Bokeh or Panel library is missing\");\n",
+                            "\t  } else {\n",
+                            "\t    console.warn(\"Panel: WARNING: Attempting to render but not all required libraries could be resolved.\")\n",
+                            "\t    embed_document(root)\n",
+                            "\t  }\n",
+                            "        }\n",
+                            "      }\n",
+                            "    }, 25, root)\n",
+                            "  }\n",
+                            "})(window);</script>"
+                        ]
+                    },
+                    "metadata": {
+                        "application/vnd.holoviews_exec.v0+json": {
+                            "id": "p1002"
+                        }
+                    },
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {},
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "data": {
+                        "application/vnd.holoviews_exec.v0+json": "",
+                        "text/html": [
+                            "<div id='p1004'>\n",
+                            "  <div id=\"afabadf6-435b-4591-8fba-afec772ea19b\" data-root-id=\"p1004\" style=\"display: contents;\"></div>\n",
+                            "</div>\n",
+                            "<script type=\"application/javascript\">(function(root) {\n",
+                            "  var docs_json = {\"6b147e8d-4e4d-44d8-824d-9e8d46002ccb\":{\"version\":\"3.4.1\",\"title\":\"Bokeh Application\",\"roots\":[{\"type\":\"object\",\"name\":\"Row\",\"id\":\"p1004\",\"attributes\":{\"name\":\"Row00985\",\"tags\":[\"embedded\"],\"stylesheets\":[\"\\n:host(.pn-loading):before, .pn-loading:before {\\n  background-color: #c3c3c3;\\n  mask-size: auto calc(min(50%, 400px));\\n  -webkit-mask-size: auto calc(min(50%, 400px));\\n}\",{\"type\":\"object\",\"name\":\"ImportedStyleSheet\",\"id\":\"p1007\",\"attributes\":{\"url\":\"https://cdn.holoviz.org/panel/1.4.1/dist/css/loading.css\"}},{\"type\":\"object\",\"name\":\"ImportedStyleSheet\",\"id\":\"p1099\",\"attributes\":{\"url\":\"https://cdn.holoviz.org/panel/1.4.1/dist/css/listpanel.css\"}},{\"type\":\"object\",\"name\":\"ImportedStyleSheet\",\"id\":\"p1005\",\"attributes\":{\"url\":\"https://cdn.holoviz.org/panel/1.4.1/dist/bundled/theme/default.css\"}},{\"type\":\"object\",\"name\":\"ImportedStyleSheet\",\"id\":\"p1006\",\"attributes\":{\"url\":\"https://cdn.holoviz.org/panel/1.4.1/dist/bundled/theme/native.css\"}}],\"min_width\":700,\"margin\":0,\"sizing_mode\":\"stretch_width\",\"align\":\"start\",\"children\":[{\"type\":\"object\",\"name\":\"Spacer\",\"id\":\"p1008\",\"attributes\":{\"name\":\"HSpacer00992\",\"stylesheets\":[\"\\n:host(.pn-loading):before, .pn-loading:before {\\n  background-color: #c3c3c3;\\n  mask-size: auto calc(min(50%, 400px));\\n  -webkit-mask-size: auto calc(min(50%, 400px));\\n}\",{\"id\":\"p1007\"},{\"id\":\"p1005\"},{\"id\":\"p1006\"}],\"margin\":0,\"sizing_mode\":\"stretch_width\",\"align\":\"start\"}},{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1022\",\"attributes\":{\"width\":700,\"height\":300,\"margin\":[5,10],\"sizing_mode\":\"fixed\",\"align\":\"start\",\"x_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1009\",\"attributes\":{\"tags\":[[[\"pc1\",\"pc1\",null]],[]],\"start\":-3.5246372795487297,\"end\":4.096478957755966,\"reset_start\":-3.5246372795487297,\"reset_end\":4.096478957755966}},\"y_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1010\",\"attributes\":{\"tags\":[[[\"pc2\",\"pc2\",null]],{\"type\":\"map\",\"entries\":[[\"invert_yaxis\",false],[\"autorange\",false]]}],\"start\":-1.5299848182583364,\"end\":1.6381787145249902,\"reset_start\":-1.5299848182583364,\"reset_end\":1.6381787145249902}},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1032\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1033\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1025\",\"attributes\":{\"text_color\":\"black\",\"text_font_size\":\"12pt\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1062\",\"attributes\":{\"name\":\"setosa\",\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1053\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1054\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1055\"},\"data\":{\"type\":\"map\",\"entries\":[[\"pc1\",{\"type\":\"ndarray\",\"array\":{\"type\":\"bytes\",\"data\":\"TCgv2xZ5BcBxHb3qj7YFwCx/ZBanHAfA90uqUHb2BcDccuRVadQFwFGrzlUzPwLAsYOkGHaQBsCwwbFLWAIFwJHkZdRPFwfA2a6uys1hBcBpN7lGOg4EwKal6Tbs5gTAdOGqp/NJBsCrAAWeWcoJwPMSd+RyKAXAGPf/oZsWA8C73cEu/PwEwJK8+y62LwXA6xvYZTuZAcDQxq82MrQEwFvHTpxnewLAzmiBIIJZBMBnBsFxProJwL6a6F//awLA1j8zlJXYAsD0K4ltqA0EwKEdDr0kwAPAaQM4lKF/BMC73XlgxB0FwFwZrnNQDgXAzM74+P2yBMAciWGwikcDwNUcTbzeMAXAJ2cifjbKBMAfQ3sebRgFwPBCchoQ7gbAxZOCznwABcDeNtISzWcGwHOjnXQR2AfAaGn3OlW4BMB04fJ1KykGwHY/09GBywbABIiTSLD6B8B3OKLOsj4DwKwoibEIrQHAAApETzK3BcDvZaasIE4EwNsK4vA3twbAso9zVz1YBMADnPMXe6AFwA==\"},\"shape\":[50],\"dtype\":\"float64\",\"order\":\"little\"}],[\"pc2\",{\"type\":\"ndarray\",\"array\":{\"type\":\"bytes\",\"data\":\"V/0gJgFx1D8ZqYDk+afGv3BDTuqzjcK/kS2PrgJf1L+tDrjCi+nUP48iSKL6uOc/jxnO+PDmtr91A0hhzOnEPxb646aHgeK/GAkoGU8gvb+GmOuHZ6TkP1jtwve6Ko4/ArvhZyYYzr8QZ1EuWF3gvzzksk443PI/IUnRC7Ro9T/5Qh4qFvHpPzkZVB1W9dM/AXngIkzu6z8MQlMHFm/gP4iVw9LPC9k/oyHFHjW22z+YNt1QexXBP4eOQMf7RLk/pskYoJsWo7/fDzJfrrDCv5NSPrYEw8A/NVqzrLSI1z8M7ImJdvjTP6+k0IEGNsm/V8f+uhsnyr+27f9IlUzaPz6a/Y8TB+o/h4lpaIZ98T+OmVs8+w6/v5DW8LjewbE/4eAACgou4z/ChQeBdTHRP5hlyKK1Ot+/h91C9k5RzT9kvMGWot3QP52oU1lZHO6/22if1B3i1b/YvjNh8CzIPyZfLfZJ8ts/vKWKRWkD0L8BLMSp5B7gP/09HwdSLc2//eGs4oaK4j9ETuo1oJK7Pw==\"},\"shape\":[50],\"dtype\":\"float64\",\"order\":\"little\"}],[\"species\",[\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\",\"setosa\"]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1063\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1064\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1059\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"fill_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"hatch_color\":{\"type\":\"value\",\"value\":\"#30a2da\"}}},\"selection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1067\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"angle\":{\"type\":\"value\",\"value\":0.0},\"line_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"line_alpha\":{\"type\":\"value\",\"value\":1.0},\"line_width\":{\"type\":\"value\",\"value\":1},\"line_join\":{\"type\":\"value\",\"value\":\"bevel\"},\"line_cap\":{\"type\":\"value\",\"value\":\"butt\"},\"line_dash\":{\"type\":\"value\",\"value\":[]},\"line_dash_offset\":{\"type\":\"value\",\"value\":0},\"fill_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"fill_alpha\":{\"type\":\"value\",\"value\":1.0},\"hatch_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":1.0},\"hatch_scale\":{\"type\":\"value\",\"value\":12.0},\"hatch_pattern\":{\"type\":\"value\",\"value\":null},\"hatch_weight\":{\"type\":\"value\",\"value\":1.0},\"marker\":{\"type\":\"value\",\"value\":\"circle\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1060\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1061\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_color\":{\"type\":\"value\",\"value\":\"#30a2da\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1077\",\"attributes\":{\"name\":\"versicolor\",\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1068\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1069\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1070\"},\"data\":{\"type\":\"map\",\"entries\":[[\"pc1\",{\"type\":\"ndarray\",\"array\":{\"type\":\"bytes\",\"data\":\"HVGrYaWO9D+KpcUw8tbtP/6OhkXIbfc/zc7/ffR2xz/Mrij23mjxP2HEd5qNiOQ/g0dSVF6F8T/RifMa0Pjnv+PL2ZLDtPA/Au41RBzpgb9Vn3SGO0Dgv+66NKfVX+A/fSsjB2D10D98k+VglYTvP4yuqMMvQ8a/vLCsFwmx7T/LLlJpCyHlP/RgXDywOM4/m74oOkI77j9EJTOA/SenP/CxvL9L3PE/lJm60qTn1j8Cx410XMX0P9D+NafNfu0/ST4HFRTg5j+7GK98Os7sP3QbE9v4T/U/iVra88Hs+D9ufOMcegbqP3xcM0OvjtO/o8Bs37xwsb+R5bmWjEXIv+JEMPt+dsE/DPadmZYU9j+NbH/j8tDiP609FobI0ek/cvupKfOH8z9hxpeaQhXqPzcdqI+Ke88/v4WhPgdNxT8oZne1Sb/dP+uXBuCOgew/FzOs/piCzT+RXx4whovmv0QqQenI2NY/7tfxHWo+1T8ByGTP6hPYPwl8NI/7j+Q/DXkYF80B7b9n9VVt1CLTPw==\"},\"shape\":[50],\"dtype\":\"float64\",\"order\":\"little\"}],[\"pc2\",{\"type\":\"ndarray\",\"array\":{\"type\":\"bytes\",\"data\":\"+GilptXs5T/5f2MNlF/UPwHxisXrIuA/wlbG5aN+6r9LjY/eXxizP6CswoaOxNq/tYxXGVgk0j/nJ2WLCBTwv+stn3X2Os0/i2fKqXwj578d088Ba0H0v5C13aWDnrq/Iq/jEeaZ4b97+m0ZEPS/v3YJ6AaIT9C/Dj1/0kTm3T8y5bAUDpfWv8HQRvngWdW/5CQyx3Jh4b+ntbBuxa7iv/v43TRzqbW/qJ3WJBKlsb9/olWed/rUv4RprLfzY8e/CNsr40MUwz+eUe2gNwbVP1PcJbDWSc8/GbGBOaUe0T+zXp+jqejEv+laVpObkde/PyOEJcWQ5r8WKSi/6MTlv5J4CoMbGdS/bfFHQOrw2r9Cv6upkP7ev7bIk1H32sg/UijxfXAW2j/3hU2HdM/XvyDcavOAL9G/Y9ix/lfS5b+QR5cOeHblv0yA39pSpaG/JgcKLnXh2b897IoyKzLwv7ezSTY5KOC/TTYXyEQ4y7+i/exTGcTSv4A2scn1KZI/Vn1It+ox6L/KaxZ3V1TWvw==\"},\"shape\":[50],\"dtype\":\"float64\",\"order\":\"little\"}],[\"species\",[\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\",\"versicolor\"]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1078\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1079\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1074\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"fill_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"hatch_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"}}},\"selection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1081\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"angle\":{\"type\":\"value\",\"value\":0.0},\"line_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"line_alpha\":{\"type\":\"value\",\"value\":1.0},\"line_width\":{\"type\":\"value\",\"value\":1},\"line_join\":{\"type\":\"value\",\"value\":\"bevel\"},\"line_cap\":{\"type\":\"value\",\"value\":\"butt\"},\"line_dash\":{\"type\":\"value\",\"value\":[]},\"line_dash_offset\":{\"type\":\"value\",\"value\":0},\"fill_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"fill_alpha\":{\"type\":\"value\",\"value\":1.0},\"hatch_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":1.0},\"hatch_scale\":{\"type\":\"value\",\"value\":12.0},\"hatch_pattern\":{\"type\":\"value\",\"value\":null},\"hatch_weight\":{\"type\":\"value\",\"value\":1.0},\"marker\":{\"type\":\"value\",\"value\":\"circle\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1075\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1076\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_color\":{\"type\":\"value\",\"value\":\"#fc4f30\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1091\",\"attributes\":{\"name\":\"virginica\",\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1082\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1083\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1084\"},\"data\":{\"type\":\"map\",\"entries\":[[\"pc1\",{\"type\":\"ndarray\",\"array\":{\"type\":\"bytes\",\"data\":\"JVEO+eE/BEBHG+lfzqT2P71ux9Xz7gRAjOs9JWSL/z8r/F/nz8wCQF/AFKUiLQtAZNImPu+t4D/SAJA18HUHQD657WngkQJAbmHnh4FVB0DXT7N+oJb6PxNxmAG82vw/eTOlyiFTAUAZck3S4on1P/hr9UX2X/k/DlhmP6d4/j/ozrcn7TH/P7q+Z0h95QtADh/YWHtdDkA4/Ir4CtD0P9oXSswrbANAoXp9yBsv8z8aXs4T1v8LQDuE1tViOPY/jp1z6BQ0AkDhay5EqOkEQONV8nPZIvQ/aHULF3qo9D+Fg+6RJv0AQMjfQ1OhGgNA5x3/7767BkAGMr9ua9gJQD/vIT6HRgFAt0uf0Ugb9z9P2pr8LoD8PxXxBf+rnAhAt8DsCWknAUDHOU0ySHv+P6ErHYmPtfI/4MwnO2PcAECx+MaKY4MCQAR9sOGbwf4/RxvpX86k9j/HWAkoDYEEQHZMQZmXWQNArJk23xIb/z8FvqJCRm/4PzCyGJPCOvw/A8cKwUFq/j+xRhWtNj72Pw==\"},\"shape\":[50],\"dtype\":\"float64\",\"order\":\"little\"}],[\"pc2\",{\"type\":\"ndarray\",\"array\":{\"type\":\"bytes\",\"data\":\"Q2GJGcUrhL/wu9T3tmXiv+1CAF2CAtY/r42v71IBx78C+pA2FZ2kv135Ajt0oOE/I8jHLIoV878xCqEVg8DWPwFZFOTeNc+/qXp3s6EM6T9bLrwoVwHPP/MTHnEDmsu/RHloGuuuyz/I2pgmstvovw63Spq8ROG/iHWPnjaHvj+sDhVBlnmlP5jXGwvUz/I/e23Wxvp30D92Ont7Vlvov8q9agxdNNg/rUtDDxpl47/1Njw3r3vdPzekJtXBKcq/QyoecHxw1T9xJBFm5/LhPylhIhSRAMe/icRCKf/dvb/4CKtdatjKv8w0aZeovN0/MjUT+GgE2D9VTLGHlPz1PzTRRG/Az8u/po/c4V5bwr+Si9yeY/7fv090QEHMBOY/krCCrZ/twT9kmc0l6z2pP+YbxqFmHsW/RjixgpDT1z/TIvOW4oHHP62g2LxjMNo/8LvU97Zl4r9MMBc6gMjRP82Z6kzQgdM/+G+8+Q4ByD8qQ3SFMQXYv+coKAkYMLQ/GL+bc1TbvT+bqyHnHRfSvw==\"},\"shape\":[50],\"dtype\":\"float64\",\"order\":\"little\"}],[\"species\",[\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\",\"virginica\"]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1092\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1093\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1088\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"fill_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"hatch_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"}}},\"selection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1095\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"angle\":{\"type\":\"value\",\"value\":0.0},\"line_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"line_alpha\":{\"type\":\"value\",\"value\":1.0},\"line_width\":{\"type\":\"value\",\"value\":1},\"line_join\":{\"type\":\"value\",\"value\":\"bevel\"},\"line_cap\":{\"type\":\"value\",\"value\":\"butt\"},\"line_dash\":{\"type\":\"value\",\"value\":[]},\"line_dash_offset\":{\"type\":\"value\",\"value\":0},\"fill_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"fill_alpha\":{\"type\":\"value\",\"value\":1.0},\"hatch_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":1.0},\"hatch_scale\":{\"type\":\"value\",\"value\":12.0},\"hatch_pattern\":{\"type\":\"value\",\"value\":null},\"hatch_weight\":{\"type\":\"value\",\"value\":1.0},\"marker\":{\"type\":\"value\",\"value\":\"circle\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1089\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1090\",\"attributes\":{\"tags\":[\"apply_ranges\"],\"x\":{\"type\":\"field\",\"field\":\"pc1\"},\"y\":{\"type\":\"field\",\"field\":\"pc2\"},\"size\":{\"type\":\"value\",\"value\":5.477225575051661},\"line_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_color\":{\"type\":\"value\",\"value\":\"#e5ae38\"},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1031\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1014\",\"attributes\":{\"tags\":[\"hv_created\"],\"renderers\":\"auto\",\"zoom_together\":\"none\"}},{\"type\":\"object\",\"name\":\"HoverTool\",\"id\":\"p1015\",\"attributes\":{\"tags\":[\"hv_created\"],\"renderers\":[{\"id\":\"p1062\"},{\"id\":\"p1077\"},{\"id\":\"p1091\"}],\"tooltips\":[[\"species\",\"@{species}\"],[\"pc1\",\"@{pc1}\"],[\"pc2\",\"@{pc2}\"]]}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1044\"},{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1045\"},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1046\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1047\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1052\"}],\"active_drag\":{\"id\":\"p1045\"},\"active_scroll\":{\"id\":\"p1014\"}}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1039\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1040\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1041\"},\"axis_label\":\"pc2\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1042\"}}}],\"right\":[{\"type\":\"object\",\"name\":\"Legend\",\"id\":\"p1065\",\"attributes\":{\"location\":[0,0],\"title\":\"species\",\"click_policy\":\"mute\",\"items\":[{\"type\":\"object\",\"name\":\"LegendItem\",\"id\":\"p1066\",\"attributes\":{\"label\":{\"type\":\"value\",\"value\":\"setosa\"},\"renderers\":[{\"id\":\"p1062\"}]}},{\"type\":\"object\",\"name\":\"LegendItem\",\"id\":\"p1080\",\"attributes\":{\"label\":{\"type\":\"value\",\"value\":\"versicolor\"},\"renderers\":[{\"id\":\"p1077\"}]}},{\"type\":\"object\",\"name\":\"LegendItem\",\"id\":\"p1094\",\"attributes\":{\"label\":{\"type\":\"value\",\"value\":\"virginica\"},\"renderers\":[{\"id\":\"p1091\"}]}}]}}],\"below\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1034\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1035\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1036\"},\"axis_label\":\"pc1\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1037\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1038\",\"attributes\":{\"axis\":{\"id\":\"p1034\"},\"grid_line_color\":null}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1043\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1039\"},\"grid_line_color\":null}}],\"min_border_top\":10,\"min_border_bottom\":10,\"min_border_left\":10,\"min_border_right\":10,\"output_backend\":\"webgl\"}},{\"type\":\"object\",\"name\":\"Spacer\",\"id\":\"p1097\",\"attributes\":{\"name\":\"HSpacer00993\",\"stylesheets\":[\"\\n:host(.pn-loading):before, .pn-loading:before {\\n  background-color: #c3c3c3;\\n  mask-size: auto calc(min(50%, 400px));\\n  -webkit-mask-size: auto calc(min(50%, 400px));\\n}\",{\"id\":\"p1007\"},{\"id\":\"p1005\"},{\"id\":\"p1006\"}],\"margin\":0,\"sizing_mode\":\"stretch_width\",\"align\":\"start\"}}]}}],\"defs\":[{\"type\":\"model\",\"name\":\"ReactiveHTML1\"},{\"type\":\"model\",\"name\":\"FlexBox1\",\"properties\":[{\"name\":\"align_content\",\"kind\":\"Any\",\"default\":\"flex-start\"},{\"name\":\"align_items\",\"kind\":\"Any\",\"default\":\"flex-start\"},{\"name\":\"flex_direction\",\"kind\":\"Any\",\"default\":\"row\"},{\"name\":\"flex_wrap\",\"kind\":\"Any\",\"default\":\"wrap\"},{\"name\":\"gap\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"justify_content\",\"kind\":\"Any\",\"default\":\"flex-start\"}]},{\"type\":\"model\",\"name\":\"FloatPanel1\",\"properties\":[{\"name\":\"config\",\"kind\":\"Any\",\"default\":{\"type\":\"map\"}},{\"name\":\"contained\",\"kind\":\"Any\",\"default\":true},{\"name\":\"position\",\"kind\":\"Any\",\"default\":\"right-top\"},{\"name\":\"offsetx\",\"kind\":\"Any\",\"default\":null},{\"name\":\"offsety\",\"kind\":\"Any\",\"default\":null},{\"name\":\"theme\",\"kind\":\"Any\",\"default\":\"primary\"},{\"name\":\"status\",\"kind\":\"Any\",\"default\":\"normalized\"}]},{\"type\":\"model\",\"name\":\"GridStack1\",\"properties\":[{\"name\":\"mode\",\"kind\":\"Any\",\"default\":\"warn\"},{\"name\":\"ncols\",\"kind\":\"Any\",\"default\":null},{\"name\":\"nrows\",\"kind\":\"Any\",\"default\":null},{\"name\":\"allow_resize\",\"kind\":\"Any\",\"default\":true},{\"name\":\"allow_drag\",\"kind\":\"Any\",\"default\":true},{\"name\":\"state\",\"kind\":\"Any\",\"default\":[]}]},{\"type\":\"model\",\"name\":\"drag1\",\"properties\":[{\"name\":\"slider_width\",\"kind\":\"Any\",\"default\":5},{\"name\":\"slider_color\",\"kind\":\"Any\",\"default\":\"black\"},{\"name\":\"value\",\"kind\":\"Any\",\"default\":50}]},{\"type\":\"model\",\"name\":\"click1\",\"properties\":[{\"name\":\"terminal_output\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"debug_name\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"clears\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"FastWrapper1\",\"properties\":[{\"name\":\"object\",\"kind\":\"Any\",\"default\":null},{\"name\":\"style\",\"kind\":\"Any\",\"default\":null}]},{\"type\":\"model\",\"name\":\"NotificationAreaBase1\",\"properties\":[{\"name\":\"js_events\",\"kind\":\"Any\",\"default\":{\"type\":\"map\"}},{\"name\":\"position\",\"kind\":\"Any\",\"default\":\"bottom-right\"},{\"name\":\"_clear\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"NotificationArea1\",\"properties\":[{\"name\":\"js_events\",\"kind\":\"Any\",\"default\":{\"type\":\"map\"}},{\"name\":\"notifications\",\"kind\":\"Any\",\"default\":[]},{\"name\":\"position\",\"kind\":\"Any\",\"default\":\"bottom-right\"},{\"name\":\"_clear\",\"kind\":\"Any\",\"default\":0},{\"name\":\"types\",\"kind\":\"Any\",\"default\":[{\"type\":\"map\",\"entries\":[[\"type\",\"warning\"],[\"background\",\"#ffc107\"],[\"icon\",{\"type\":\"map\",\"entries\":[[\"className\",\"fas fa-exclamation-triangle\"],[\"tagName\",\"i\"],[\"color\",\"white\"]]}]]},{\"type\":\"map\",\"entries\":[[\"type\",\"info\"],[\"background\",\"#007bff\"],[\"icon\",{\"type\":\"map\",\"entries\":[[\"className\",\"fas fa-info-circle\"],[\"tagName\",\"i\"],[\"color\",\"white\"]]}]]}]}]},{\"type\":\"model\",\"name\":\"Notification\",\"properties\":[{\"name\":\"background\",\"kind\":\"Any\",\"default\":null},{\"name\":\"duration\",\"kind\":\"Any\",\"default\":3000},{\"name\":\"icon\",\"kind\":\"Any\",\"default\":null},{\"name\":\"message\",\"kind\":\"Any\",\"default\":\"\"},{\"name\":\"notification_type\",\"kind\":\"Any\",\"default\":null},{\"name\":\"_destroyed\",\"kind\":\"Any\",\"default\":false}]},{\"type\":\"model\",\"name\":\"TemplateActions1\",\"properties\":[{\"name\":\"open_modal\",\"kind\":\"Any\",\"default\":0},{\"name\":\"close_modal\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"BootstrapTemplateActions1\",\"properties\":[{\"name\":\"open_modal\",\"kind\":\"Any\",\"default\":0},{\"name\":\"close_modal\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"TemplateEditor1\",\"properties\":[{\"name\":\"layout\",\"kind\":\"Any\",\"default\":[]}]},{\"type\":\"model\",\"name\":\"MaterialTemplateActions1\",\"properties\":[{\"name\":\"open_modal\",\"kind\":\"Any\",\"default\":0},{\"name\":\"close_modal\",\"kind\":\"Any\",\"default\":0}]},{\"type\":\"model\",\"name\":\"copy_to_clipboard1\",\"properties\":[{\"name\":\"fill\",\"kind\":\"Any\",\"default\":\"none\"},{\"name\":\"value\",\"kind\":\"Any\",\"default\":null}]}]}};\n",
+                            "  var render_items = [{\"docid\":\"6b147e8d-4e4d-44d8-824d-9e8d46002ccb\",\"roots\":{\"p1004\":\"afabadf6-435b-4591-8fba-afec772ea19b\"},\"root_ids\":[\"p1004\"]}];\n",
+                            "  var docs = Object.values(docs_json)\n",
+                            "  if (!docs) {\n",
+                            "    return\n",
+                            "  }\n",
+                            "  const py_version = docs[0].version.replace('rc', '-rc.').replace('.dev', '-dev.')\n",
+                            "  function embed_document(root) {\n",
+                            "    var Bokeh = get_bokeh(root)\n",
+                            "    Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
+                            "    for (const render_item of render_items) {\n",
+                            "      for (const root_id of render_item.root_ids) {\n",
+                            "\tconst id_el = document.getElementById(root_id)\n",
+                            "\tif (id_el.children.length && (id_el.children[0].className === 'bk-root')) {\n",
+                            "\t  const root_el = id_el.children[0]\n",
+                            "\t  root_el.id = root_el.id + '-rendered'\n",
+                            "\t}\n",
+                            "      }\n",
+                            "    }\n",
+                            "  }\n",
+                            "  function get_bokeh(root) {\n",
+                            "    if (root.Bokeh === undefined) {\n",
+                            "      return null\n",
+                            "    } else if (root.Bokeh.version !== py_version) {\n",
+                            "      if (root.Bokeh.versions === undefined || !root.Bokeh.versions.has(py_version)) {\n",
+                            "\treturn null\n",
+                            "      }\n",
+                            "      return root.Bokeh.versions.get(py_version);\n",
+                            "    } else if (root.Bokeh.version === py_version) {\n",
+                            "      return root.Bokeh\n",
+                            "    }\n",
+                            "    return null\n",
+                            "  }\n",
+                            "  function is_loaded(root) {\n",
+                            "    var Bokeh = get_bokeh(root)\n",
+                            "    return (Bokeh != null && Bokeh.Panel !== undefined)\n",
+                            "  }\n",
+                            "  if (is_loaded(root)) {\n",
+                            "    embed_document(root);\n",
+                            "  } else {\n",
+                            "    var attempts = 0;\n",
+                            "    var timer = setInterval(function(root) {\n",
+                            "      if (is_loaded(root)) {\n",
+                            "        clearInterval(timer);\n",
+                            "        embed_document(root);\n",
+                            "      } else if (document.readyState == \"complete\") {\n",
+                            "        attempts++;\n",
+                            "        if (attempts > 200) {\n",
+                            "          clearInterval(timer);\n",
+                            "\t  var Bokeh = get_bokeh(root)\n",
+                            "\t  if (Bokeh == null || Bokeh.Panel == null) {\n",
+                            "            console.warn(\"Panel: ERROR: Unable to run Panel code because Bokeh or Panel library is missing\");\n",
+                            "\t  } else {\n",
+                            "\t    console.warn(\"Panel: WARNING: Attempting to render but not all required libraries could be resolved.\")\n",
+                            "\t    embed_document(root)\n",
+                            "\t  }\n",
+                            "        }\n",
+                            "      }\n",
+                            "    }, 25, root)\n",
+                            "  }\n",
+                            "})(window);</script>"
+                        ],
+                        "text/plain": [
+                            ":NdOverlay   [species]\n",
+                            "   :Scatter   [pc1]   (pc2)"
+                        ]
+                    },
+                    "execution_count": 20,
+                    "metadata": {
+                        "application/vnd.holoviews_exec.v0+json": {
+                            "id": "p1004"
+                        }
+                    },
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "dia = DIA(df)\n",
+                "dia.plot_pc2(pl.all().exclude(\"species\"), by = \"species\")"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
```

### Comparing `polars_ds-0.4.1/examples/sample_and_split.ipynb` & `polars_ds-0.4.2/examples/sample_and_split.ipynb`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/mkdocs.yml` & `polars_ds-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/__init__.py` & `polars_ds-0.4.2/python/polars_ds/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from polars_ds.metrics import *  # noqa: F403
 from polars_ds.stats import *  # noqa: F403
 from polars_ds.complex import ComplexExt  # noqa: E402, F401
 from polars_ds.str2 import *  # noqa: F403
 
 logging.basicConfig(level=logging.INFO)
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 def l_inf_horizontal(*v: Union[str, pl.Expr], normalize: bool = False) -> pl.Expr:
     """
     Horizontally L inf norm. Shorthand for pl.max_horizontal(pl.col(x).abs() for x in exprs).
 
     Parameters
```

### Comparing `polars_ds-0.4.1/python/polars_ds/_utils.py` & `polars_ds-0.4.2/python/polars_ds/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/complex.py` & `polars_ds-0.4.2/python/polars_ds/complex.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/diagnosis.py` & `polars_ds-0.4.2/python/polars_ds/diagnosis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import polars.selectors as cs
 import polars as pl
 import logging
-from typing import Union, List, Optional
+from typing import Union, List, Optional, Iterable
 from functools import lru_cache
-from .num import query_cond_entropy
+from .num import query_cond_entropy, query_principal_components
 from itertools import combinations
 import graphviz
 from great_tables import GT
+from polars.type_aliases import IntoExpr
 
 logger = logging.getLogger(__name__)
 
 
 # DIA = Data Inspection Assistant / DIAgonsis
 class DIA:
 
@@ -24,15 +25,44 @@
         self._frame: pl.LazyFrame = df.lazy()
         self.numerics: List[str] = df.select(cs.numeric()).columns
         self.ints: List[str] = df.select(cs.integer()).columns
         self.floats: List[str] = df.select(cs.float()).columns
         self.strs: List[str] = df.select(cs.string()).columns
         self.bools: List[str] = df.select(cs.boolean()).columns
         self.cats: List[str] = df.select(cs.categorical()).columns
-        self.simple_types: List[str] = self.numerics + self.strs + self.bools + self.cats
+        self.list_floats: List[str] = [
+            c
+            for c, t in df.schema.items()
+            if (t.is_(pl.List(pl.Float32)) or (t.is_(pl.List(pl.Float64))))
+        ]
+        self.list_ints: List[str] = [
+            c
+            for c, t in df.schema.items()
+            if t.is_(pl.List(pl.UInt8))
+            or t.is_(pl.List(pl.UInt16))
+            or t.is_(pl.List(pl.UInt32))
+            or t.is_(pl.List(pl.UInt64))
+            or t.is_(pl.List(pl.Int8))
+            or t.is_(pl.List(pl.Int16))
+            or t.is_(pl.List(pl.Int32))
+            or t.is_(pl.List(pl.Int64))
+        ]
+        self.list_bool: List[str] = [c for c, t in df.schema.items() if t.is_(pl.List(pl.Boolean))]
+        self.list_str: List[str] = [c for c, t in df.schema.items() if t.is_(pl.List(pl.String))]
+
+        self.simple_types: List[str] = (
+            self.numerics
+            + self.strs
+            + self.bools
+            + self.cats
+            + self.list_floats
+            + self.list_ints
+            + self.list_bool
+            + self.list_str
+        )
         self.other_types: List[str] = [c for c in self._frame.columns if c not in self.simple_types]
 
     def numeric_profile(self, n_bins: int = 20, iqr_multiplier: float = 1.5):
         """
         Creates a numerical profile with a histogram plot. Notice that the histograms may have
         completely different scales on the x-axis.
 
@@ -131,33 +161,24 @@
                 pl.col(c).str.len_bytes().quantile(0.05).alias("5p_byte_len"),
                 pl.col(c).str.len_bytes().quantile(0.95).alias("95p_byte_len"),
             )
             for c in to_check
         ]
         return pl.concat(pl.collect_all(frames))
 
-    def corr(self, subset: Union[str, List[str], pl.Expr]) -> pl.DataFrame:
+    def corr(self, subset: Union[IntoExpr, Iterable[IntoExpr]]) -> pl.DataFrame:
         """
         Returns a dataframe containing correlation information between the subset and all numeric columns.
 
         Parameters
         ----------
         subset
-            Either a str representing a column name or a list of strings representing column names, or a Polars
-            selector/expression which select columns
+            Anything that can be put into a Polars .select statement.
         """
-        if isinstance(subset, str):
-            temp = [subset]
-        elif isinstance(subset, list):
-            temp = [s for s in subset if isinstance(s, str)]
-        elif isinstance(subset, pl.Expr):
-            temp = self._frame.select(subset).columns
-        else:
-            raise ValueError("Unknown subset type.")
-
+        temp = self._frame.select(subset).columns
         to_check = [c for c in temp if c in self.numerics]
         if len(to_check) != len(temp):
             removed = list(set(temp).difference(to_check))
             logger.info(
                 f"The following columns are not numeric/not in the dataframe, skipped: \n{removed}"
             )
 
@@ -166,23 +187,22 @@
                 pl.lit(x).alias("column"), *(pl.corr(x, y).alias(y) for y in self.numerics)
             )
             for x in to_check
         ]
 
         return pl.concat(pl.collect_all(corrs))
 
-    def plot_corr(self, subset: Union[str, List[str], pl.Expr]):
+    def plot_corr(self, subset: Union[IntoExpr, Iterable[IntoExpr]]):
         """
         Plots the correlations using classic heat maps.
 
         Parameters
         ----------
         subset
-            Either a str representing a column name or a list of strings representing column names, or a Polars
-            selector/expression which select columns
+            Anything that can be put into a Polars .select statement.
         """
         corr = self.corr(subset)
         cols = [c for c in corr.columns if c != "column"]
         return (
             GT(corr)
             .fmt_number(columns=cols, decimals=3)
             .data_color(
@@ -190,14 +210,42 @@
                 palette=["#0202bd", "#bd0237"],
                 domain=[-1, 1],
                 alpha=0.5,
                 na_color="#000000",
             )
         )
 
+    def infer_prob(self) -> List[str]:
+        """
+        Infers columns that can potentially be probabilities. For f32/f64 columns, this checks if all values are
+        between 0 and 1. For List[f32] or List[f64] columns, this checks whether the column can potentially be
+        multi-class probabilities.
+        """
+        is_ok = (
+            self._frame.select(
+                *((pl.col(c).is_between(0.0, 1.0).all()).alias(c) for c in self.floats),
+                *(
+                    (
+                        (
+                            pl.col(c).list.eval((pl.element() >= 0.0).all()).list.first()
+                        )  # every number must be positive
+                        & (pl.col(c).list.sum() == 1.0)  # class prob must sum to 1
+                        & (
+                            pl.col(c).list.len().min() == pl.col(c).list.len().max()
+                        )  # class prob column must have the same length
+                    ).alias(c)
+                    for c in self.list_floats
+                ),
+            )
+            .collect()
+            .row(0)
+        )
+
+        return [c for c, ok in zip(self.floats + self.list_floats, is_ok) if ok is True]
+
     @lru_cache
     def infer_high_null(self, threshold: float = 0.75) -> List[str]:
         """
         Infers columns with more than threshold percentage nulls.
 
         Parameters
         ----------
@@ -482,7 +530,37 @@
 
             dot.node(c)
             for p in parents_of_c:
                 dot.node(p)
                 dot.edge(p, c)
 
         return dot
+
+    def plot_pc2(
+        self, *features: Union[IntoExpr, Iterable[IntoExpr]], by: str, center: bool = True, **kwargs
+    ):
+        """
+        Creates a 2D scatter plot based on the reduced dimensions via PCA, and color it by `by`.
+
+        Paramters
+        ---------
+        features
+            Any selection expression for Polars
+        by
+            Color the 2-D PCA plot by the values in the column
+        center
+            Whether to automatically center the features
+        kwargs
+            Anything else that will be passed to hvplot's scatter function
+        """
+        feats = self._frame.select(features).columns
+        if len(feats) < 2:
+            raise ValueError("You must pass >= 2 features.")
+
+        temp = (
+            self._frame.select(
+                query_principal_components(*feats, center=center, k=2).alias("pc"), by
+            )
+            .collect()
+            .unnest("pc")
+        )
+        return temp.plot.scatter("pc1", "pc2", by=by, **kwargs)
```

### Comparing `polars_ds-0.4.1/python/polars_ds/graph.py` & `polars_ds-0.4.2/python/polars_ds/graph.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/metrics.py` & `polars_ds-0.4.2/python/polars_ds/metrics.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/num.py` & `polars_ds-0.4.2/python/polars_ds/num.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,28 @@
             changes_length=True,
         )
 
 
 # ----------------------------------------------------------------------------------
 
 
+def softmax(x: StrOrExpr) -> pl.Expr:
+    """
+    Applies the softmax function to the column, which turns any real valued column into valid probability
+    values. This is simply a shorthand for x.exp() / x.exp().sum() for expressions x.
+
+    Paramters
+    ---------
+    x
+        Either a str represeting a column name or a Polars expression
+    """
+    xx = str_to_expr(x)
+    return xx.exp() / (xx.exp().sum())
+
+
 def query_gcd(x: StrOrExpr, y: Union[int, str, pl.Expr]) -> pl.Expr:
     """
     Computes GCD of two integer columns. This will try to cast everything to int32.
 
     Parameters
     ----------
     x
@@ -299,14 +313,108 @@
         symbol="pl_haversine",
         args=[xlat, xlong, ylat, ylong],
         is_elementwise=True,
         cast_to_supertype=True,
     )
 
 
+def query_singular_values(
+    *features: StrOrExpr,
+    center: bool = True,
+    as_explained_var: bool = False,
+    as_ratio: bool = False,
+) -> pl.Expr:
+    """
+    Finds all principal values (singular values) for the data matrix formed by the given features
+    and returns them in descending order.
+
+    Note: if a row has null values, it will be dropped.
+
+    Paramters
+    ---------
+    features
+        Feature columns
+    center
+        Whether to center the data or not. If you want to standard-normalize, set this to False,
+        and do it for input features by hand.
+    as_explained_var
+        If true, return the explained variance, which is singular_value ^ 2 / (n_samples - 1)
+    as_ratio
+        If true, normalize output to between 0 and 1.
+    """
+    feats = [str_to_expr(f) for f in features]
+    if center:
+        actual_inputs = [f - f.mean() for f in feats]
+    else:
+        actual_inputs = feats
+
+    out = pl_plugin(lib=_lib, symbol="pl_singular_values", args=actual_inputs, returns_scalar=True)
+    if as_explained_var:
+        out = out.list.eval(pl.element().pow(2) / (pl.count() - 1))
+    if as_ratio:
+        out = out.list.eval(pl.element() / pl.element().sum())
+
+    return out
+
+
+def query_pca(
+    *features: StrOrExpr,
+    center: bool = True,
+) -> pl.Expr:
+    """
+    Finds all singular values as well as the principle vectors.
+
+    Paramters
+    ---------
+    features
+        Feature columns
+    center
+        Whether to center the data or not. If you want to standard normalize, set this to False,
+        and do it for input features by hand.
+    """
+    feats = [str_to_expr(f) for f in features]
+    if center:
+        actual_inputs = [f - f.mean() for f in feats]
+    else:
+        actual_inputs = feats
+
+    return pl_plugin(lib=_lib, symbol="pl_pca", args=actual_inputs, changes_length=True)
+
+
+def query_principal_components(
+    *features: StrOrExpr,
+    k: int = 2,
+    center: bool = True,
+) -> pl.Expr:
+    """
+    Transforms the features to get the first k principal components.
+
+    Paramters
+    ---------
+    features
+        Feature columns
+    center
+        Whether to center the data or not. If you want to standard normalize, set this to False,
+        and do it for input features by hand.
+    """
+    feats = [str_to_expr(f) for f in features]
+    if k > len(feats) or k < 0:
+        raise ValueError("Input `k` should be between 1 and the number of features inclusive.")
+
+    if center:
+        actual_inputs = [f - f.mean() for f in feats]
+    else:
+        actual_inputs = feats
+
+    actual_inputs.insert(0, pl.lit(k, dtype=pl.UInt32).alias("principal_components"))
+    return pl_plugin(
+        lib=_lib, symbol="pl_principal_components", args=actual_inputs, changes_length=True
+    )
+
+
 def query_knn_ptwise(
     *features: StrOrExpr,
     index: StrOrExpr,
     k: int = 5,
     leaf_size: int = 32,
     dist: Distance = "l2",
     parallel: bool = False,
```

### Comparing `polars_ds-0.4.1/python/polars_ds/sample.py` & `polars_ds-0.4.2/python/polars_ds/sample.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/stats.py` & `polars_ds-0.4.2/python/polars_ds/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,16 +283,16 @@
     equal_var: bool = False,
 ) -> pl.Expr:
     """
     Performs 2 sample student's t test or Welch's t test. Functionality-wise this is desgined
     to be equivalent to SciPy's ttest_ind, with fewer options. The result is not exact but
     within 1e-10 precision from SciPy's.
 
-    In the case of student's t test, the data is assumed to have no nulls, and n = self._expr.count()
-    is used. Note self._expr.count() only counts non-null elements after polars 0.20.
+    In the case of student's t test, the data is assumed to have no nulls, and n = expr.count()
+    is used. Note expr.count() only counts non-null elements after polars 0.20.
     The degree of freedom will be 2n - 2. As a result, nulls might cause problems.
 
     In the case of Welch's t test, data will be sanitized (nulls, NaNs, Infs will be dropped
     before the test), and df will be counted based on the length of sanitized data.
 
     Parameters
     ----------
@@ -322,16 +322,16 @@
     else:
         s1 = y1.filter(y1.is_finite())
         s2 = y2.filter(y2.is_finite())
         m1 = s1.mean()
         m2 = s2.mean()
         v1 = s1.var()
         v2 = s2.var()
-        n1 = s1.count().cast(pl.UInt64)
-        n2 = s2.count().cast(pl.UInt64)
+        n1 = s1.len().cast(pl.UInt64)
+        n2 = s2.len().cast(pl.UInt64)
         return pl_plugin(
             lib=_lib,
             symbol="pl_welch_t",
             args=[m1, m2, v1, v2, n1, n2, pl.lit(alternative, dtype=pl.String)],
             returns_scalar=True,
         )
 
@@ -353,15 +353,15 @@
         Alternative of the hypothesis test
     """
     y = str_to_expr(var1)
     s1 = y.filter(y.is_finite())
     sm = s1.mean()
     pm = pl.lit(pop_mean, dtype=pl.Float64)
     var = s1.var()
-    cnt = s1.count().cast(pl.UInt64)
+    cnt = s1.len().cast(pl.UInt64)
     alt = pl.lit(alternative, dtype=pl.String)
     return pl_plugin(
         lib=_lib,
         symbol="pl_ttest_1samp",
         args=[sm, pm, var, cnt, alt],
         returns_scalar=True,
     )
@@ -411,15 +411,15 @@
         )
     else:
         s1 = y.filter(y.is_finite())
         m1 = s1.mean()
         m2 = pl.lit(mean, pl.Float64)
         v1 = s1.var()
         v2 = pl.lit(var, pl.Float64)
-        n1 = s1.count().cast(pl.UInt64)
+        n1 = s1.len().cast(pl.UInt64)
         n2 = pl.lit(cnt, pl.UInt64)
         return pl_plugin(
             lib=_lib,
             symbol="pl_welch_t",
             args=[m1, m2, v1, v2, n1, n2, pl.lit(alternative, dtype=pl.String)],
             returns_scalar=True,
         )
@@ -496,15 +496,15 @@
         raise ValueError("No input feature column to run F-test on.")
     elif len(vars_) == 2:
         return pl_plugin(lib=_lib, symbol="pl_f_test", args=vars_, returns_scalar=True)
     else:
         return pl_plugin(lib=_lib, symbol="pl_f_test", args=vars_, changes_length=True)
 
 
-def query_chi2(var1: Union[pl.Expr, float], var2: Union[pl.Expr, float]) -> pl.Expr:
+def query_chi2(var1: StrOrExpr, var2: StrOrExpr) -> pl.Expr:
     """
     Computes the Chi Squared statistic and p value between two categorical values.
 
     Note that it is up to the user to make sure that the two columns contain categorical
     values. This method is equivalent to SciPy's chi2_contingency, except that it also
     computes the contingency table internally for the user.
 
@@ -519,15 +519,15 @@
         lib=_lib,
         symbol="pl_chi2",
         args=[str_to_expr(var1), str_to_expr(var2)],
         returns_scalar=True,
     )
 
 
-def perturb(var: Union[pl.Expr, float], epsilon: float, positive: bool = False):
+def perturb(var: StrOrExpr, epsilon: float, positive: bool = False):
     """
     Perturb the var by a small amount. This only applies to float columns.
 
     Parameters
     ----------
     var
         Either the name of the column or a Polars expression
@@ -553,15 +553,15 @@
         lib=_lib,
         symbol="pl_perturb",
         args=[str_to_expr(var), lo, hi],
         is_elementwise=True,
     )
 
 
-def normal_test(var: Union[pl.Expr, float]) -> pl.Expr:
+def normal_test(var: StrOrExpr) -> pl.Expr:
     """
     Perform a normality test which is based on D'Agostino and Pearson's test
     that combines skew and kurtosis to produce an omnibus test of normality.
     Null values, NaN and inf are dropped when running this computation.
 
     Parameters
     ----------
@@ -611,15 +611,15 @@
         lib=_lib,
         symbol="pl_random",
         args=[pl.len(), lo, up, pl.lit(seed, pl.UInt64)],
         is_elementwise=True,
     )
 
 
-def random_null(var: Union[pl.Expr, float], pct: float, seed: Optional[int] = None) -> pl.Expr:
+def random_null(var: StrOrExpr, pct: float, seed: Optional[int] = None) -> pl.Expr:
     """
     Creates random null values in var. If var contains nulls originally, they
     will stay null.
 
     Parameters
     ----------
     var
@@ -892,15 +892,15 @@
     https://en.wikipedia.org/wiki/Pearson_correlation_coefficient#Weighted_correlation_coefficient
     """
     xx, yy, w = str_to_expr(x), str_to_expr(y), str_to_expr(weights)
     wx, wy = weighted_mean(xx, w, False), weighted_mean(yy, w, False)
     return w.dot((xx - wx) * (yy - wy)) / w.sum()
 
 
-def weighted_corr(x: StrOrExpr, y: StrOrExpr, weights: Union[pl.Expr, float]) -> pl.Expr:
+def weighted_corr(x: StrOrExpr, y: StrOrExpr, weights: StrOrExpr) -> pl.Expr:
     """
     Computes the weighted correlation between x and y. The weights column must have the same
     length as both x an y.
 
     All weights are assumed to be > 0. This will not check if weights are valid.
 
     Parameters
@@ -937,15 +937,15 @@
     """
     xx, yy = str_to_expr(x), str_to_expr(y)
     x2 = xx.dot(xx).sqrt()
     y2 = yy.dot(yy).sqrt()
     return xx.dot(yy) / (x2 * y2).sqrt()
 
 
-def weighted_cosine_sim(x: StrOrExpr, y: StrOrExpr, weights: Union[pl.Expr, str]) -> pl.Expr:
+def weighted_cosine_sim(x: StrOrExpr, y: StrOrExpr, weights: StrOrExpr) -> pl.Expr:
     """
     Computes the weighted cosine similarity between x and y (column-wise). The weights column
     must have the same length as both x an y.
 
     All weights are assumed to be > 0. This will not check if weights are valid.
 
     Parameters
@@ -962,7 +962,53 @@
     https://en.wikipedia.org/wiki/Pearson_correlation_coefficient#Weighted_correlation_coefficient
     """
     xx, yy = str_to_expr(x), str_to_expr(y)
     w = str_to_expr(weights)
     wx2 = xx.pow(2).dot(w)
     wy2 = yy.pow(2).dot(w)
     return (w * xx).dot(yy) / (wx2 * wy2).sqrt()
+
+
+def xi_corr(
+    x: StrOrExpr, y: StrOrExpr, seed: Optional[int] = None, return_p: bool = False
+) -> pl.Expr:
+    """
+    Computes the ξ(xi) correlation developed by SOURAV CHATTERJEE in the paper in the reference.
+    This will return both the correlation (the statistic) and the p-value. Note that if sample size
+    is smaller than 30, p-value will always be NaN. The ξ correlation is not symmetric, and this only
+    tries to explain whether y is a function of x.
+
+    Parameters
+    ----------
+    x
+        The first variable
+    y
+        The second variable
+    seed
+        Whether to have a seed when we break ties at random
+    return_p
+        Whether to return a two-sided p value for the statistic
+
+    Reference
+    ---------
+    https://arxiv.org/pdf/1909.10140.pdf
+    """
+    xx, yy = str_to_expr(x), str_to_expr(y)
+    args = [
+        xx.rank(method="random", seed=seed),
+        yy.rank(method="max").cast(pl.Float64),
+        (-yy).rank(method="max").cast(pl.Float64),
+    ]
+    if return_p:
+        return pl_plugin(
+            lib=_lib,
+            symbol="pl_xi_corr_w_p",
+            args=args,
+            returns_scalar=True,
+        )
+    else:
+        return pl_plugin(
+            lib=_lib,
+            symbol="pl_xi_corr",
+            args=args,
+            returns_scalar=True,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polars_ds-0.4.1/python/polars_ds/str2.py` & `polars_ds-0.4.2/python/polars_ds/str2.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/python/polars_ds/type_alias.py` & `polars_ds-0.4.2/python/polars_ds/type_alias.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/graph/degree.rs` & `polars_ds-0.4.2/src/graph/degree.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/graph/eigen_centrality.rs` & `polars_ds-0.4.2/src/graph/eigen_centrality.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/graph/mod.rs` & `polars_ds-0.4.2/src/graph/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/graph/shortest_path.rs` & `polars_ds-0.4.2/src/graph/shortest_path.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/cond_entropy.rs` & `polars_ds-0.4.2/src/num/cond_entropy.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/convolve.rs` & `polars_ds-0.4.2/src/num/convolve.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/entrophies.rs` & `polars_ds-0.4.2/src/num/entrophies.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/fft.rs` & `polars_ds-0.4.2/src/num/fft.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/float_extras.rs` & `polars_ds-0.4.2/src/num/float_extras.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/gcd_lcm.rs` & `polars_ds-0.4.2/src/num/gcd_lcm.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/haversine.rs` & `polars_ds-0.4.2/src/num/haversine.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/jaccard.rs` & `polars_ds-0.4.2/src/num/jaccard.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/knn.rs` & `polars_ds-0.4.2/src/num/knn.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/lempel_ziv.rs` & `polars_ds-0.4.2/src/num/lempel_ziv.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/mod.rs` & `polars_ds-0.4.2/src/num/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 mod float_extras;
 mod gcd_lcm;
 mod haversine;
 mod jaccard;
 mod knn;
 mod lempel_ziv;
 mod ols;
+mod pca;
 mod psi;
 mod target_encode;
 mod tp_fp;
 mod trapz;
 mod woe_iv;
 
 // Collection of distances, most will be used as function pointers in kd tree related queries,
 // which may be bad for perf.
 
-// Are these fast?
+// Are these fast? Try with PULP?
 
 #[inline]
 pub fn l_inf_dist<T: Float>(a: &[T], b: &[T]) -> T {
     debug_assert_eq!(a.len(), b.len());
     a.iter()
         .zip(b.iter())
         .fold(T::zero(), |acc, (x, y)| acc.max((*x - *y).abs()))
```

### Comparing `polars_ds-0.4.1/src/num/ols.rs` & `polars_ds-0.4.2/src/num/ols.rs`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,22 @@
     Ok(Field::new(
         "coeffs",
         DataType::List(Box::new(DataType::Float64)),
     ))
 }
 
 /// Returns the coefficients for lstsq as a nrows x 1 matrix
-/// The uses Cholesky decomposition as default method to compute inverse, 
+/// The uses Cholesky decomposition as default method to compute inverse,
 /// and falls back to LU decomposition
 fn faer_cholesky_lstsq(x: MatRef<f64>, xt: MatRef<f64>, y: MatRef<f64>) -> Mat<f64> {
     let xtx = xt * x;
     let inv = match xtx.cholesky(Side::Lower) {
         Ok(cho) => cho.inverse(),
         // Fall back to LU decomp
-        Err(_) => xtx.partial_piv_lu().inverse()
+        Err(_) => xtx.partial_piv_lu().inverse(),
     };
     let coeffs = inv * xt * y;
     coeffs
 }
 
 /// Returns a Array2 ready for linear regression, and a mask, indicates valid rows
 #[inline(always)]
@@ -196,15 +196,15 @@
             let x = mat.slice(s![0..nrows, 1..]);
             let xt = x.t().into_faer();
             let x = x.view().into_faer();
             // Solving Least Square
             let xtx = xt * &x;
             let xtx_inv = match xtx.cholesky(Side::Lower) {
                 Ok(cho) => cho.inverse(),
-                Err(_) => xtx.partial_piv_lu().inverse()
+                Err(_) => xtx.partial_piv_lu().inverse(),
             };
             let coeffs = &xtx_inv * xt * y;
             let betas = coeffs.col_as_slice(0);
             // Degree of Freedom
             let dof = nrows as f64 - ncols as f64;
             // Residue
             let res = y - x * &coeffs;
@@ -224,15 +224,16 @@
             let p_values = t_values
                 .iter()
                 .map(
                     |t| match crate::stats_utils::beta::student_t_sf(t.abs(), dof) {
                         Ok(p) => 2.0 * p,
                         Err(_) => f64::NAN,
                     },
-                ).collect_vec();
+                )
+                .collect_vec();
             // Finalize
             let idx_series = UInt16Chunked::from_iter((0..ncols).map(|i| Some(i as u16)));
             let idx_series = idx_series.with_name("idx").into_series();
             let coeffs_series = Float64Chunked::from_slice("coeff", betas);
             let coeffs_series = coeffs_series.into_series();
             let stderr_series = Float64Chunked::from_vec("std_err", std_err);
             let stderr_series = stderr_series.into_series();
```

### Comparing `polars_ds-0.4.1/src/num/psi.rs` & `polars_ds-0.4.2/src/num/psi.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/target_encode.rs` & `polars_ds-0.4.2/src/num/target_encode.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/tp_fp.rs` & `polars_ds-0.4.2/src/num/tp_fp.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     let temp = df
         .lazy()
         .group_by([col("threshold")])
         .agg([
             len().alias("cnt"),
             col("actual").sum().alias("pos_cnt_at_threshold"),
         ])
-        .sort("threshold", Default::default())
+        .sort(["threshold"], Default::default())
         .with_columns([
             (lit(n) - col("cnt").cum_sum(false) + col("cnt")).alias("predicted_positive"),
             (lit(positive_counts) - col("pos_cnt_at_threshold").cum_sum(false))
                 .shift_and_fill(1, positive_counts)
                 .alias("tp"),
         ])
         .select([
```

### Comparing `polars_ds-0.4.1/src/num/trapz.rs` & `polars_ds-0.4.2/src/num/trapz.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/num/woe_iv.rs` & `polars_ds-0.4.2/src/num/woe_iv.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats/chi2.rs` & `polars_ds-0.4.2/src/stats/chi2.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats/fstats.rs` & `polars_ds-0.4.2/src/stats/fstats.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats/ks.rs` & `polars_ds-0.4.2/src/stats/ks.rs`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     let alpha = inputs[2].f64()?;
     let alpha = alpha.get(0).unwrap();
 
     if (s1.len() <= 30) || (s2.len() <= 30) {
         let s = Series::from_vec("statistic", vec![f64::INFINITY]);
         let p = Series::from_vec("threshold", vec![f64::NAN]);
         let out = StructChunked::new("ks", &[s, p])?;
-        return Ok(out.into_series())
+        return Ok(out.into_series());
     }
 
     let v1 = s1.cont_slice().unwrap();
     let v2 = s2.cont_slice().unwrap();
 
     let res = ks_2samp(v1, v2, alpha);
```

### Comparing `polars_ds-0.4.1/src/stats/mod.rs` & `polars_ds-0.4.2/src/stats/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 mod chi2;
 mod fstats;
 mod ks;
 mod normal_test;
 mod sample;
 mod t_test;
+mod xi_corr;
 
 use polars::prelude::*;
 
 pub fn simple_stats_output(_: &[Field]) -> PolarsResult<Field> {
     let s = Field::new("statistic", DataType::Float64);
     let p = Field::new("pvalue", DataType::Float64);
     let v: Vec<Field> = vec![s, p];
```

### Comparing `polars_ds-0.4.1/src/stats/normal_test.rs` & `polars_ds-0.4.2/src/stats/normal_test.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats/sample.rs` & `polars_ds-0.4.2/src/stats/sample.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     let n = n.get(0).unwrap() as usize;
     let low = inputs[1].i32()?;
     let mut low = low.get(0).unwrap();
     let high = inputs[2].i32()?;
     let mut high = high.get(0).unwrap();
     if low == high {
         let out = Int32Chunked::from_vec("", vec![low; n]);
-        return Ok(out.into_series())
+        return Ok(out.into_series());
     } else if high < low {
         std::mem::swap(&mut low, &mut high);
     }
     let seed = inputs[3].u64()?;
     let seed = seed.get(0);
     let dist = Uniform::new(low, high);
     let mut rng = if let Some(s) = seed {
```

### Comparing `polars_ds-0.4.1/src/stats/t_test.rs` & `polars_ds-0.4.2/src/stats/t_test.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats_utils/beta.rs` & `polars_ds-0.4.2/src/stats_utils/beta.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats_utils/gamma.rs` & `polars_ds-0.4.2/src/stats_utils/gamma.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats_utils/mod.rs` & `polars_ds-0.4.2/src/stats_utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/stats_utils/normal.rs` & `polars_ds-0.4.2/src/stats_utils/normal.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/consts.rs` & `polars_ds-0.4.2/src/str2/consts.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/fuzz.rs` & `polars_ds-0.4.2/src/str2/fuzz.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/hamming.rs` & `polars_ds-0.4.2/src/str2/hamming.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/inflections.rs` & `polars_ds-0.4.2/src/str2/inflections.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/jaro.rs` & `polars_ds-0.4.2/src/str2/jaro.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/knn_strs.rs` & `polars_ds-0.4.2/src/str2/knn_strs.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/levenshtein.rs` & `polars_ds-0.4.2/src/str2/levenshtein.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/mod.rs` & `polars_ds-0.4.2/src/str2/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/osa.rs` & `polars_ds-0.4.2/src/str2/osa.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/overlap.rs` & `polars_ds-0.4.2/src/str2/overlap.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/snowball/algorithms/english_stemmer.rs` & `polars_ds-0.4.2/src/str2/snowball/algorithms/english_stemmer.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/snowball/mod.rs` & `polars_ds-0.4.2/src/str2/snowball/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/snowball/snowball_env.rs` & `polars_ds-0.4.2/src/str2/snowball/snowball_env.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/snowball_stem.rs` & `polars_ds-0.4.2/src/str2/snowball_stem.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/sorensen_dice.rs` & `polars_ds-0.4.2/src/str2/sorensen_dice.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/str_jaccard.rs` & `polars_ds-0.4.2/src/str2/str_jaccard.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/str2/tversky.rs` & `polars_ds-0.4.2/src/str2/tversky.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/src/utils/mod.rs` & `polars_ds-0.4.2/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.1/tests/test.ipynb` & `polars_ds-0.4.2/tests/test.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9459731934731934%*

 * *Differences: {"'cells'": "{0: {'source': ['import polars as pl\\n', 'import polars_ds as pds']}, 1: {'source': "*

 * *            "{insert: [(0, 'df = pds.random_data(size=5_000, n_cols = 0).select(\\n'), (1, '    "*

 * *            'pds.random(0.0, 12.0).alias("x"),\\n\'), (2, \'    pds.random(0.0, '*

 * *            '1.0).alias("y"),\\n\'), (4, \'df.head()\')], delete: [6, 4, 3, 2, 1, 0]}}, 2: '*

 * *            "{'source': {insert: [(0, "*

 * *            '\'df.sort(pl.col("x").rank(method="random")).select(\\n\'), (1, \'    "x",\\n\'), (2,  […]*

```diff
@@ -1,129 +1,78 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import polars as pl\n",
-                "import polars_ds as pds\n",
-                "import numpy as np\n",
-                "import time "
+                "import polars_ds as pds"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
-                "df = pds.random_data(size=10_000, n_cols = 0).select(\n",
-                "    pds.random(0.0, 1.0).alias(\"x1\"),\n",
-                "    pds.random(0.0, 1.0).alias(\"x2\"),\n",
-                "    pds.random(0.0, 1.0).alias(\"w\"),\n",
-                "    pds.random_int(0,2).alias(\"y\")\n",
+                "df = pds.random_data(size=5_000, n_cols = 0).select(\n",
+                "    pds.random(0.0, 12.0).alias(\"x\"),\n",
+                "    pds.random(0.0, 1.0).alias(\"y\"),\n",
                 ")\n",
-                "df"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "df.select(\n",
-                "    pds.weighted_corr(pl.col(\"x1\"), pl.col(\"x2\"), pl.col(\"w\"))\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import polars_ds.sample as sa"
+                "df.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df.filter(\n",
-                "    (pl.int_range(0, pl.len()).shuffle(42) < (pl.len() // 2)).over(pl.col(\"y\")==1)\n",
+                "df.sort(pl.col(\"x\").rank(method=\"random\")).select(\n",
+                "    \"x\",\n",
+                "    \"y\",\n",
+                "    pl.col(\"y\").rank(method=\"max\").cast(pl.Float64).alias(\"r\"),\n",
+                "    (-pl.col(\"y\")).rank(method=\"max\").cast(pl.Float64).alias(\"l\"),\n",
+                ").with_columns(\n",
+                "    pl.col(\"r\").diff().abs().alias(\"r_abs_diff\"),\n",
+                "    (pl.col(\"l\") * (pl.len() - pl.col(\"l\"))).alias(\"l(n-l)\"),\n",
+                ").select(\n",
+                "    1 - (pl.len() / 2) * (pl.col(\"r_abs_diff\").sum() / pl.col(\"l(n-l)\").sum())\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "vn = sa.volume_neutral(df, pl.col(\"y\") == 1, target_volume=30_000)\n",
-                "vn.group_by(\"y\").len()"
+                "from xicor.xicor import Xi\n",
+                "x = df[\"x\"].to_numpy()\n",
+                "y = df[\"y\"].to_numpy()\n",
+                "xi_obj = Xi(x, y)\n",
+                "xi_obj.correlation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "downsampled = sa.down_sample(\n",
-                "    df, \n",
-                "    [(pl.col(\"y\") == 1, 100), (pl.col(\"y\") == 2, 50)]\n",
-                ")"
+                "xi_obj.correlation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": [
-                "downsampled = sa.down_sample(\n",
-                "    df, \n",
-                "    [(pl.col(\"y\").is_between(1, 2, closed=\"both\"), 0.5)]\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "print(downsampled.group_by(\"y\").len().sort(\"y\"))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `polars_ds-0.4.1/tests/test_correctness.py` & `polars_ds-0.4.2/tests/test_correctness.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,68 @@
 import pytest
 import polars as pl
 import numpy as np
 import polars_ds as pds
 from polars.testing import assert_frame_equal
 
 
+def test_pca():
+    from sklearn.decomposition import PCA
+
+    df = pds.random_data(size=2000, n_cols=0).select(
+        pds.random(0.0, 1.0).alias("x1"),
+        pds.random(0.0, 1.0).alias("x2"),
+        pds.random(0.0, 1.0).alias("x3"),
+    )
+
+    singular_values = df.select(pds.query_singular_values("x1", "x2", "x3").alias("res"))["res"][
+        0
+    ].to_numpy()
+
+    pca = PCA()
+    data_matrix = df.select("x1", "x2", "x3").to_numpy().astype(np.float64)
+    pca.fit(data_matrix)
+    ans_singular_values = pca.singular_values_
+
+    assert np.isclose(singular_values, ans_singular_values).all()
+
+    singular_values = df.select(pds.query_singular_values("x1", "x2", "x3").alias("res"))["res"][
+        0
+    ].to_numpy()
+
+    vectors = df.select(pds.query_pca("x1", "x2", "x3").alias("vectors")).unnest("vectors")[
+        "weight_vector"
+    ]
+
+    ans_vectors = pca.components_
+    for i in range(len(vectors)):
+        vi = vectors[i].to_numpy()
+        ans_vi = ans_vectors[i, :]
+        # The principal vector can be either v or -v. It doesn't matter and depends on backend algo's choice.
+        # Have a more relaxed rtol
+        assert np.isclose(np.abs(vi), np.abs(ans_vi), rtol=1e-5).all()
+
+
+def test_xi_corr():
+    df = pds.random_data(size=2_000, n_cols=0).select(
+        pds.random(0.0, 12.0).alias("x"),
+        pds.random(0.0, 1.0).alias("y"),
+    )
+
+    from xicor.xicor import Xi
+
+    x = df["x"].to_numpy()
+    y = df["y"].to_numpy()
+    xi_obj = Xi(x, y)
+    ans_statistic = xi_obj.correlation
+    test_statistic = df.select(pds.xi_corr("x", "y")).item(0, 0)
+
+    assert np.isclose(ans_statistic, test_statistic, rtol=1e-4)
+
+
 @pytest.mark.parametrize(
     "df, ft, res_full, res_valid, res_same",
     [
         (
             pl.DataFrame({"a": [5, 6, 7, 8, 9]}),
             [1, 0, -1],
             pl.DataFrame({"a": pl.Series([5, 6, 2, 2, 2, -8, -9], dtype=pl.Float64)}),
```

### Comparing `polars_ds-0.4.1/Cargo.lock` & `polars_ds-0.4.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1503,17 +1503,17 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f01006048a264047d6cba081fed8e11adbd69c15956f9e53185a9ac4a541853c"
+checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-io",
  "polars-lazy",
@@ -1523,17 +1523,17 @@
  "polars-time",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25197f40d71f82b2f79bb394f03e555d3cc1ce4db1dd052c28318721c71e96ad"
+checksum = "725b09f2b5ef31279b66e27bbab63c58d49d8f6696b66b1f46c7eaab95e80f75"
 dependencies = [
  "ahash",
  "atoi",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -1569,33 +1569,33 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c354515f73cdbbad03c2bf723fcd68e6825943b3ec503055abc8a8cb08ce46bb"
+checksum = "a796945b14b14fbb79b91ef0406e6fddca2be636e889f81ea5d6ee7d36efb4fe"
 dependencies = [
  "bytemuck",
  "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
  "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f20d3c227186f74aa3c228c64ef72f5a15617322fed30b4323eaf53b25f8e7b"
+checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "comfy-table",
@@ -1618,39 +1618,39 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d66dd0ce51f8bd620eb8bd376502fe68a2b1a446d5433ecd2e75270b0755ce76"
+checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
 dependencies = [
  "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-ffi"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6c93ea335ccca3dc7fd8ca4a8d129178afc9634c8caf2237500a3390e4aa60b"
+checksum = "dcdd5a0b45dea8df72db9dfca694a1acc753bd868f3a751903b83cacdb896d2b"
 dependencies = [
  "polars-arrow",
  "polars-core",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b40bef2edcdc58394792c4d779465144283a09ff1836324e7b72df7978a6e992"
+checksum = "b2c8589e418cbe4a48228d64b2a8a40284a82ec3c98817c0c2bcc0267701338b"
 dependencies = [
  "ahash",
  "async-trait",
  "atoi_simd",
  "bytes",
  "chrono",
  "fast-float",
@@ -1675,17 +1675,17 @@
  "smartstring",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c27df26a19d3092298d31d47614ad84dc330c106e38aa8cd53727cd91c07cf56"
+checksum = "89b2632b1af668e2058d5f8f916d8fbde3cac63d03ae29a705f598e41dcfeb7f"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
@@ -1698,17 +1698,17 @@
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f8a51c3bdc9e7c34196ff6f5c3cb17da134e5aafb1756aaf24b76c7118e63dc"
+checksum = "efdbdb4d9a92109bc2e0ce8e17af5ae8ab643bb5b7ee9d1d74f0aeffd1fbc95f"
 dependencies = [
  "ahash",
  "argminmax",
  "base64",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -1719,26 +1719,27 @@
  "memchr",
  "num-traits",
  "polars-arrow",
  "polars-compute",
  "polars-core",
  "polars-error",
  "polars-utils",
+ "rand",
  "rayon",
  "regex",
  "smartstring",
  "unicode-reverse",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8824ee00fbbe83d69553f2711014c50361238d210ed81a7a297695b7db97d42"
+checksum = "b421d2196f786fdfe162db614c8485f8308fe41575d4de634a39bbe460d1eb6a"
 dependencies = [
  "ahash",
  "async-stream",
  "base64",
  "brotli",
  "ethnum",
  "flate2",
@@ -1754,17 +1755,17 @@
  "snap",
  "streaming-decompression",
  "zstd",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c5e2c1f14e81d60cfa9afe4e611a9bad9631a2cb7cd19b7c0094d0dc32f0231"
+checksum = "48700f1d5bd56a15451e581f465c09541492750360f18637b196f995470a015c"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown",
  "num-traits",
  "polars-arrow",
@@ -1779,54 +1780,56 @@
  "smartstring",
  "uuid",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff48362bd1b078bbbec7e7ba9ec01fea58fee2887db22a8e3deaf78f322fa3c4"
+checksum = "2fb8e2302e20c44defd5be8cad9c96e75face63c3a5f609aced8c4ec3b3ac97d"
 dependencies = [
  "ahash",
  "bytemuck",
  "chrono-tz",
+ "hashbrown",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-parquet",
  "polars-time",
  "polars-utils",
  "rayon",
+ "recursive",
  "regex",
  "smartstring",
  "strum_macros 0.25.3",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63029da56ff6a720b190490bbc7b6263f9b72d1134311b1f381fc8d306d37770"
+checksum = "a515bdc68c2ae3702e3de70d89601f3b71ca8137e282a226dddb53ee4bacfa2e"
 dependencies = [
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-sql"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3652c362959f608d1297196b973d1e3acb508a9562b886ac39bf7606b841052b"
+checksum = "7b4bb7cc1c04c3023d1953b2f1dec50515e8fd8169a5a2bf4967b3b082232db7"
 dependencies = [
  "hex",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-lazy",
  "polars-plan",
@@ -1834,17 +1837,17 @@
  "serde",
  "serde_json",
  "sqlparser",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86eb74ea6ddfe675aa5c3f33c00dadbe2b85f0e8e3887b85db1fd5a3397267fd"
+checksum = "efc18e3ad92eec55db89d88f16c22d436559ba7030cf76f86f6ed7a754b673f1"
 dependencies = [
  "atoi",
  "chrono",
  "chrono-tz",
  "now",
  "once_cell",
  "polars-arrow",
@@ -1854,35 +1857,36 @@
  "polars-utils",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "694656a7d2b0cd8f07660dbc8d0fb7a81066ff57a452264907531d805c1e58c4"
+checksum = "c760b6c698cfe2fbbbd93d6cfb408db14ececfe1d92445dae2229ce1b5b21ae8"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-error",
  "raw-cpuid 11.0.1",
  "rayon",
  "smartstring",
+ "stacker",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ds"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "ahash",
  "approx",
  "faer",
  "faer-ext",
  "hashbrown",
  "inflections",
@@ -1932,14 +1936,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "pulp"
 version = "0.18.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03457ac216146f43f921500bac4e892d5cd32b0479b929cbfc90f95cd6c599c2"
 dependencies = [
  "bytemuck",
  "libm",
@@ -1958,17 +1971,17 @@
  "num-traits",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -1976,79 +1989,79 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-polars"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6ab8ad08494161085fb0d2d9de82c7fde7398da1778ee7e7a5a596ff4201f5b"
+checksum = "469bd1d378fb3a34c1b182383e84741d9e7c5451a5d29a3f9c557aac161876cd"
 dependencies = [
  "polars",
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "pyo3",
  "pyo3-polars-derive",
  "serde",
  "serde-pickle",
  "thiserror",
 ]
 
 [[package]]
 name = "pyo3-polars-derive"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c67d6b47b05d3827ef8e5f4449ae1a1861f5d7086ee18c5429e347b0d03c19"
+checksum = "3ba3d428667917efd2c233534db5779f55b398e123aea75243da8491856e1131"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
  "syn 2.0.58",
@@ -2165,14 +2178,34 @@
 [[package]]
 name = "reborrow"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03251193000f4bd3b042892be858ee50e8b3719f2b08e5833ac4353724632430"
 
 [[package]]
+name = "recursive"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0786a43debb760f491b1bc0269fe5e84155353c67482b9e60d0cfb596054b43e"
+dependencies = [
+ "recursive-proc-macro-impl",
+ "stacker",
+]
+
+[[package]]
+name = "recursive-proc-macro-impl"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76009fbe0614077fc1a2ce255e3a1881a2e3a3527097d5dc6d8212c585e7e38b"
+dependencies = [
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -2375,14 +2408,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "743b4dc2cbde11890ccb254a8fc9d537fa41b36da00de2a1c5e9848c9bc42bd7"
 dependencies = [
  "log",
 ]
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "streaming-decompression"
```

### Comparing `polars_ds-0.4.1/pyproject.toml` & `polars_ds-0.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.3.2"]
 build-backend = "maturin"
 
 [project]
 name = "polars_ds"
 requires-python = ">=3.8"
-version = "0.4.1"
+version = "0.4.2"
 
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -22,16 +22,17 @@
     "polars >= 0.20.6, !=0.20.12",
 ] 
 
 keywords = ["polars-extension", "scientific-computing", "data-science"]
 
 [project.optional-dependencies]
 plot = [
-    "great-tables >= 0.4",
-    "graphviz >= 0.20"
+    "great-tables >= 0.5",
+    "graphviz >= 0.20",
+    "hvplot >= 0.9.1" # Polars's plot backend for now, which in term is backed by Bokeh
 ]
 
 [tool.maturin]
 strip = true
 python-source = "python"
 features = ["pyo3/extension-module"]
 module-name = "polars_ds._polars_ds"
```

### Comparing `polars_ds-0.4.1/PKG-INFO` & `polars_ds-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: polars_ds
-Version: 0.4.1
+Version: 0.4.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: polars >=0.20.6, !=0.20.12
-Requires-Dist: great-tables >=0.4 ; extra == 'plot'
+Requires-Dist: great-tables >=0.5 ; extra == 'plot'
 Requires-Dist: graphviz >=0.20 ; extra == 'plot'
+Requires-Dist: hvplot >=0.9.1 ; extra == 'plot'
 Provides-Extra: plot
 License-File: LICENSE.txt
 Keywords: polars-extension,scientific-computing,data-science
 Author-email: Tianren Qin <tq9695@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.3 Name: polars_ds Version: 0.4.1 Classifier: Development
+Metadata-Version: 2.3 Name: polars_ds Version: 0.4.2 Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Rust Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: License ::
 OSI Approved :: MIT License Requires-Dist: polars >=0.20.6, !=0.20.12 Requires-
-Dist: great-tables >=0.4 ; extra == 'plot' Requires-Dist: graphviz >=0.20 ;
-extra == 'plot' Provides-Extra: plot License-File: LICENSE.txt Keywords:
-polars-extension,scientific-computing,data-science Author-email: Tianren Qin
+Dist: great-tables >=0.5 ; extra == 'plot' Requires-Dist: graphviz >=0.20 ;
+extra == 'plot' Requires-Dist: hvplot >=0.9.1 ; extra == 'plot' Provides-Extra:
+plot License-File: LICENSE.txt Keywords: polars-extension,scientific-
+computing,data-science Author-email: Tianren Qin
 gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM
                         ************ PPoollaarrss ffoorr DDaattaa SScciieennccee
                                      ************
                _D_o_c_u_m_e_n_t_a_t_i_o_n | _U_s_e_r_ _G_u_i_d_e | _W_a_n_t_ _t_o_ _C_o_n_t_r_i_b_u_t_e_?
                              ppiipp iinnssttaallll ppoollaarrss--ddss
 # The Project The goal of the project is to **reduce dependencies**, **improve
```

