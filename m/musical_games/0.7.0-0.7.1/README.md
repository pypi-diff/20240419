# Comparing `tmp/musical_games-0.7.0.tar.gz` & `tmp/musical_games-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.7.0.tar` & `musical_games-0.7.1.tar`

### file list

```diff
@@ -1,99 +1,105 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.7.0/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.7.0/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.7.0/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.7.0/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.7.0/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.7.0/.travis.yml
--rw-r--r--   0        0        0     1032 2024-04-16 05:06:34.950851 musical_games-0.7.0/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.7.0/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.7.0/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.7.0/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.7.0/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.7.0/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.7.0/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.7.0/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.7.0/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.7.0/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.7.0/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.7.0/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.7.0/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1830 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2798 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3767 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.7.0/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    34442 2024-04-13 18:22:02.752740 musical_games-0.7.0/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.7.0/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    15391 2024-04-16 05:05:56.478852 musical_games-0.7.0/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.7.0/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.7.0/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.7.0/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.7.0/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4695 2024-04-09 10:54:53.546529 musical_games-0.7.0/musical_games/utils.py
--rw-r--r--   0        0        0     1114 2024-04-16 05:06:24.374851 musical_games-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.7.0/scripts/__init__.py
--rw-r--r--   0        0        0     9431 2024-04-16 05:05:56.478852 musical_games-0.7.0/scripts/copy_bars.py
--rw-r--r--   0        0        0     1649 2024-04-13 13:01:09.427755 musical_games-0.7.0/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     1652 2024-04-13 13:54:11.547670 musical_games-0.7.0/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1761 2024-04-13 14:21:32.579626 musical_games-0.7.0/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1556 2024-04-16 05:05:56.478852 musical_games-0.7.0/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1519 2024-04-13 14:35:38.727603 musical_games-0.7.0/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     1664 2024-04-13 13:01:48.155754 musical_games-0.7.0/scripts/demo_stadler_meneut_trio.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.7.0/tox.ini
--rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 musical_games-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.7.1/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.7.1/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.7.1/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.7.1/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.7.1/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.7.1/.travis.yml
+-rw-r--r--   0        0        0     1225 2024-04-19 09:45:47.861062 musical_games-0.7.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.7.1/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.7.1/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.7.1/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.7.1/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.7.1/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.7.1/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.7.1/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.7.1/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.7.1/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      624 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2047 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1830 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2796 2024-04-18 10:49:11.595361 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3765 2024-04-18 10:49:11.583361 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-16 05:05:56.478852 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.7.1/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    44061 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.7.1/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    15379 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.7.1/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.7.1/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.7.1/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.7.1/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.7.1/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-04-19 09:45:26.253062 musical_games-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.7.1/scripts/__init__.py
+-rw-r--r--   0        0        0     9431 2024-04-16 05:05:56.478852 musical_games-0.7.1/scripts/copy_bars.py
+-rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.7.1/scripts/demo_stadler_meneut_trio.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.7.1/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.7.1/PKG-INFO
```

### Comparing `musical_games-0.7.0/.gitchangelog.rc` & `musical_games-0.7.1/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/.gitignore` & `musical_games-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/CHANGELOG.rst` & `musical_games-0.7.1/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 *********
 Changelog
 *********
 
+v0.7.1 (2024-04-19)
+===================
+
+Added
+-----
+- Adds functionality for rendering a single dice table element.
+- Adds support for dice games selecting multiple measures per dice throw.
+
+
 v0.7.0 (2024-04-16)
 ===================
 
 Added
 -----
 - Adds the contredanse from Mozart.
```

### Comparing `musical_games-0.7.0/LICENSE` & `musical_games-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/Makefile` & `musical_games-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/README.rst` & `musical_games-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/Makefile` & `musical_games-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/conf.py` & `musical_games-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/contributing.rst` & `musical_games-0.7.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/index.rst` & `musical_games-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/make.bat` & `musical_games-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/musical_games.converters.rst` & `musical_games-0.7.1/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.7.1/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/musical_games.dice_games.rst` & `musical_games-0.7.1/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/docs/musical_games.rst` & `musical_games-0.7.1/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/__version__.py` & `musical_games-0.7.1/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.7.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('contredanse', 'piano_right_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('contredanse', 'piano_right_hand')}"
             }
         <<
             {
                 \key c\major
                 \time 2/4
-                \tempo 8 = 120
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
@@ -42,15 +42,15 @@
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('contredanse', 'piano_left_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('contredanse', 'piano_left_hand')}"
             }
         <<
             {
                 \key c\major
                 \time 2/4
-                \tempo 8 = 120
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
```

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
                 \time 2/4
-                \tempo 8 = 120
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
@@ -78,15 +78,15 @@
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
                 \time 2/4
-                \tempo 8 = 120
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
```

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.7.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/dice_games/base.py` & `musical_games-0.7.1/musical_games/dice_games/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 __author__ = 'Robbert Harms'
 __date__ = '2024-04-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
+import math
+import random
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from functools import reduce
 from operator import mul
 from pathlib import Path
 from typing import Self, TypeAlias, Any
 
+from frozendict import frozendict
 import jinja2
-import numpy as np
-from numpy.random import RandomState
 
 
 int_bar_index: TypeAlias = int
 int_voice_index: TypeAlias = int
 str_dice_table_name: TypeAlias = str
 str_staff_name: TypeAlias = str
 
@@ -53,53 +54,49 @@
         :meth:`compile_single_bar`.
 
         Returns:
             The available dice tables in this game.
         """
 
     @abstractmethod
-    def get_all_duplicate_bars(self) -> dict[str_dice_table_name, list[set[int_bar_index]]]:
-        """Get a list of all the duplicate bars for each dice table.
+    def get_bar_collections(self) -> dict[str_dice_table_name, BarCollection]:
+        """Get the collection of bars for each dice table.
 
-        For each dice table, this should scan the bars belonging to that dice table for duplicates. We return each
-        set of duplicates as a set containing all the bar indices having duplicates.
+        Args:
+            dice_table_name: the name of the dice table
 
         Returns:
-            A list of duplicate bar sets by bar index for each dice table
+            The collection of bars for each dice table as a bar collection object.
         """
 
     @abstractmethod
-    def get_duplicate_bars(self, table_name: str_dice_table_name, bar_index: int_bar_index) -> set[int_bar_index]:
-        """Get the set of duplicates of the given bar in the indicated table.
+    def get_duplicate_dice_table_elements(self, dice_table_name: str_dice_table_name) -> list[set[DiceTableElement]]:
+        """Get a list of all the duplicate bars for a specific dice table.
+
+        For a given dice table, this should scan for duplicate measures in the musical entries corresponding to each
+        element in the dice table. We return each set of duplicates as a tuple containing all the dice table elements
+        having duplicates.
 
         Returns:
-            The set of duplicates for the indicated bar
+            A list of duplicate dice table elements.
         """
 
     @abstractmethod
     def count_unique_compositions(self, count_duplicates=False) -> int:
         """Count the number of unique compositions possible by this dice game.
 
         Args:
             count_duplicates (boolean): if set to False, we exclude all identical bars in a column of the dice matrix.
 
         Returns:
             The number of unique compositions
         """
 
     @abstractmethod
-    def get_nmr_staffs_per_table(self) -> dict[str_dice_table_name, int]:
-        """Get the number of staffs available per dice table.
-
-        Returns:
-            Per dice table, the number of staffs available in the measures table.
-        """
-
-    @abstractmethod
-    def get_random_bar_selection(self, shuffle_staffs: bool = False, seed: int = None) -> BarSelection:
+    def get_random_bar_selection(self, seed: int = None, shuffle_staffs: bool = False) -> BarSelection:
         """Get a random bar selection we may use to create a composition.
 
         Args:
             shuffle_staffs: if we want to shuffle the staffs within a dice table independently.
             seed: a seed for the random number generator.
 
         Returns:
@@ -149,14 +146,34 @@
             bar_ind: the specific bar to lookup in the set of all bars. Should be an element of the referred table.
 
         Returns:
             A lilypond score for the single bar
         """
 
     @abstractmethod
+    def compile_single_dice_table_element(self,
+                                          table_name: str_dice_table_name,
+                                          dice_table_element: DiceTableElement) -> LilypondScore:
+        """Get a lilypond score with only the bar or bars selected by the given dice table element.
+
+        Since some dice tables have select more than one bar per element, we have this method in addition to
+        :meth:`compile_single_bar`. The latter only selects one specific bar, this selects all the bars selected
+        by the dice table element.
+
+        Args:
+            table_name: the specific dice table to use. Names should match those of the method :meth:`get_dice_tables`.
+            dice_table_element: the specific dice table element for which to look up the bars.
+                Should be an element of the referred table.
+
+        Returns:
+            A lilypond score for the dice table element.
+        """
+
+
+    @abstractmethod
     def compile_composition_score(self,
                                   bar_selection: BarSelection,
                                   comment: str | None = None,
                                   single_page: bool = False) -> LilypondScore:
         """Compile a visual composition of this dice game using the selected bars.
 
         Args:
@@ -215,83 +232,84 @@
     @property
     def title(self) -> str:
         return self._title
 
     def get_dice_tables(self) -> dict[str_dice_table_name, DiceTable]:
         return self._dice_tables
 
-    def get_all_duplicate_bars(self) -> dict[str_dice_table_name, list[set[int_bar_index]]]:
-        table_duplicates = {}
-        for table_name, dice_table in self._dice_tables.items():
-            bars = self._bar_collections[table_name].get_synchronous_bars()
-
-            bars_by_lilypond = {}
-            for bar_ind, bar in bars.items():
-                bar_data = tuple(b.lilypond_str for b in bar.get_staffs().values())
-                bar_indices = bars_by_lilypond.setdefault(bar_data, set())
-                bar_indices.add(bar_ind)
-
-            table_duplicates[table_name] = [v for k, v in bars_by_lilypond.items() if len(v) > 1]
-        return table_duplicates
-
-    def get_duplicate_bars(self, table_name: str_dice_table_name, bar_index: int_bar_index) -> list[int_bar_index]:
-        bars = self._bar_collections[table_name].get_synchronous_bars()
-        current_bar = bars[bar_index]
-
-        indices = set()
-        for bar_ind, bar in bars.items():
-            if bar == current_bar:
-                indices.add(bar_ind)
-        return indices
+    def get_bar_collections(self) -> dict[str_dice_table_name, BarCollection]:
+        return self._bar_collections
+
+    def get_duplicate_dice_table_elements(self, dice_table_name: str_dice_table_name) -> list[set[DiceTableElement]]:
+        flat_dice_table = self._dice_tables[dice_table_name].get_elements()
+        bars = self._bar_collections[dice_table_name].get_synchronous_selection(flat_dice_table)
+
+        bars_grouped = {}
+        for dice_table_element, bar in zip(flat_dice_table, bars):
+            bar_elements = bars_grouped.setdefault(bar, set())
+            bar_elements.add(dice_table_element)
+
+        return [v for k, v in bars_grouped.items() if len(v) > 1]
 
     def count_unique_compositions(self, count_duplicates=False) -> int:
-        def count_unique_bars(table_name: str, bar_indexes: list[int]):
-            """Count the number of unique bars in the provided list of bar numbers."""
-            bars_of_table = self._bar_collections[table_name]
-            bars = [tuple(el.lilypond_str for el in bars_of_table.get_synchronous_bar(bar_index).get_bars())
-                    for bar_index in bar_indexes]
-            return len(set(bars))
+        def count_unique_bars(table_name: str, throw_ind: int):
+            """Count the number of unique bars for the indicated throw index (column)."""
+            dice_table_column = self._dice_tables[table_name].get_column(throw_ind)
+            bars_in_column = self._bar_collections[table_name].get_synchronous_selection(dice_table_column)
+            return len(set(bars_in_column))
 
         table_counts = []
         for table_name, table in self._dice_tables.items():
             if count_duplicates:
                 table_counts.append(table.max_dice_value ** table.nmr_throws)
             else:
-                table_counts.append(reduce(mul, [count_unique_bars(table_name, column)
-                                                 for column in table.list_columns()]))
+                table_counts.append(reduce(mul, [count_unique_bars(table_name, throw_ind)
+                                                 for throw_ind in range(table.nmr_throws)]))
         return reduce(mul, table_counts)
 
-    def get_nmr_staffs_per_table(self) -> dict[str_dice_table_name, int]:
-        return {table_name: len(bar_collection.get_staff_names())
-                for table_name, bar_collection in self._bar_collections.items()}
-
-    def get_random_bar_selection(self, shuffle_staffs: bool = False, seed: int = None) -> BarSelection:
+    def get_random_bar_selection(self, seed: int = None, shuffle_staffs: bool = False) -> BarSelection:
         if shuffle_staffs:
             choices = {}
             for table_name, dice_table in self._dice_tables.items():
                 choices[table_name] = {}
                 for staff_ind, staff_name in enumerate(self._bar_collections[table_name].get_staff_names()):
                     choices[table_name][staff_name] = dice_table.get_random_selection(seed + staff_ind)
             return PerStaffsBarSelection(choices)
         else:
             choices = {}
             for table_name, dice_table in self._dice_tables.items():
                 choices[table_name] = dice_table.get_random_selection(seed)
             return GroupedStaffsBarSelection(choices)
 
-    def bar_selection_to_bars(self, bar_selection: BarSelection) -> dict[str_dice_table_name, list[SynchronousBar]]:
+    def bar_selection_to_bars(self,
+                              bar_selection: BarSelection) -> dict[str_dice_table_name, list[tuple[SynchronousBar]]]:
         composition_bars = {table_name: [] for table_name in self._dice_tables.keys()}
 
         for table_name in self._dice_tables.keys():
-            for throw_ind in range(self._dice_tables[table_name].nmr_throws):
-                bars_per_index = {}
-                for staff_name in self._bar_collections[table_name].get_staff_names():
-                    bar_ind = bar_selection.get_bar_index(table_name, throw_ind, staff_name)
-                    bars_per_index[staff_name] = self._bar_collections[table_name].get_bar(staff_name, bar_ind)
-                composition_bars[table_name].append(SimpleSynchronousBar(bars_per_index))
+            staff_names = self._bar_collections[table_name].get_staff_names()
+
+            bars_per_staff = {}
+            for staff_name in staff_names:
+                staff_selection = bar_selection.get_dice_table_elements(table_name, staff_name)
+                selected_bar_tuplets = self._bar_collections[table_name].get_bar_selection(staff_name, staff_selection)
+
+                staff_bars = []
+                for bar_tuplet in selected_bar_tuplets:
+                    for bar in bar_tuplet:
+                        staff_bars.append(bar)
+                bars_per_staff[staff_name] = staff_bars
+
+            complete_bars = []
+            for composition_ind in range(len(bars_per_staff[staff_names[0]])):
+                sync_bars = {}
+                for staff_name in staff_names:
+                    sync_bars[staff_name] = bars_per_staff[staff_name][composition_ind]
+                complete_bars.append(SimpleSynchronousBar(frozendict(sync_bars)))
+
+            composition_bars[table_name] = complete_bars
         return composition_bars
 
     def get_default_midi_settings(self) -> MidiSettings:
         return self._default_midi_settings
 
     def compile_bars_overview(self, single_page: bool = False) -> LilypondScore:
         template = self._jinja2_environment.get_template('bar_overview.ly')
@@ -299,14 +317,21 @@
                                                    render_settings={'single_page': single_page}))
 
     def compile_single_bar(self, table_name: str_dice_table_name, bar_ind: int_bar_index) -> LilypondScore:
         template = self._jinja2_environment.get_template('single_bar.ly')
         synchronous_bar = self._bar_collections[table_name].get_synchronous_bar(bar_ind)
         return SimpleLilypondScore(template.render(table_name=table_name, synchronous_bar=synchronous_bar))
 
+    def compile_single_dice_table_element(self,
+                                          table_name: str_dice_table_name,
+                                          dice_table_element: DiceTableElement) -> LilypondScore:
+        template = self._jinja2_environment.get_template('single_dice_table_element.ly')
+        synchronous_bars = self._bar_collections[table_name].get_synchronous_selection([dice_table_element])[0]
+        return SimpleLilypondScore(template.render(table_name=table_name, synchronous_bars=synchronous_bars))
+
     def compile_composition_score(self,
                                   bar_selection: BarSelection,
                                   comment: str | None = None,
                                   single_page: bool = False) -> LilypondScore:
         template = self._jinja2_environment.get_template('composition_pdf.ly')
         composition_bars = self.bar_selection_to_bars(bar_selection)
         return SimpleLilypondScore(template.render(composition_bars=composition_bars,
@@ -347,20 +372,21 @@
 
         Returns:
             A lilypond string of a single bar.
         """
 
 
 class SynchronousBar(metaclass=ABCMeta):
-    """Representation of a list of bars played synchronously across staves.
+    """Representation of a list of bars played synchronously across staffs.
 
     Suppose that a piece has a piano and a violin, then at each time point there are three bars being played, left and
     right hand piano and the violin. These synchronous bars are connected in this class. For clarity, the different
     bars should be stored in a dictionary with their staff name as key.
     """
+
     @abstractmethod
     def get_staff_names(self) -> list[str_staff_name]:
         """Get the names of the staffs stored in this synchronous bar.
 
         Returns:
             The names of the staffs
         """
@@ -390,19 +416,37 @@
 
         Returns:
             The list of bars, in the order defined by the dictionary.
         """
 
 
 class BarCollection(metaclass=ABCMeta):
-    """Collection of synchronous bars for a single compositional piece.
+    """Collection of synchronous bars.
 
     The bars are expected to be stored in a dictionary mapping bar indices to bars.
     """
 
+    @property
+    @abstractmethod
+    def nmr_bars(self) -> int:
+        """The number of bars in this bar collection.
+
+        Returns:
+            The number of bars in this bar collection (0-indiced).
+        """
+
+    @property
+    @abstractmethod
+    def maximum_bar_ind(self) -> int:
+        """The maximum bar index, 1 + number of bars.
+
+        Returns:
+            The maximum bar index. Since the bars start counting at 1, this is one more than the number of bars.
+        """
+
     @abstractmethod
     def get_synchronous_bars(self) -> dict[int_bar_index, SynchronousBar]:
         """Get the collection of all synchronous bars.
 
         Returns:
             All synchronous bars indexed by their bar index.
         """
@@ -445,14 +489,46 @@
             staff_name: the name of the staff
             bar_index: the index of the bar
 
         Returns:
             The specific bar in the given staff and bar index locations.
         """
 
+    @abstractmethod
+    def get_synchronous_selection(self,
+                                  dice_table_elements: list[DiceTableElement]) -> list[tuple[SynchronousBar, ...]]:
+        """Convert a selection of dice table elements into a list of synchronous bar tuplets.
+
+        Since each dice table element may point to multiple consecutive synchronous bars, we need to return a tuple of
+        synchronous bars per listed dice table element.
+
+        Args:
+            dice_table_elements: the dice table elements we wish to lookup
+
+        Returns:
+            The synchronous bars for each dice table element in the list
+        """
+
+    @abstractmethod
+    def get_bar_selection(self,
+                          staff_name: str_staff_name,
+                          dice_table_elements: list[DiceTableElement]) -> list[tuple[Bar, ...]]:
+        """Convert a selection of dice table elements into a list of bar tuplets.
+
+        Since each dice table element may point to multiple consecutive bars, we need to return a tuple of
+        bars per listed dice table element.
+
+        Args:
+            dice_table_elements: the dice table elements we wish to lookup
+            staff_name: only return the values of this specific staff.
+
+        Returns:
+            The selection of bars for each dice table element and the specific staff
+        """
+
 
 @dataclass(frozen=True, slots=True)
 class SimpleBar(Bar):
     """Dataclass representation of a single bar, of a single staff.
 
     Args:
         lilypond_str: the lilypond string representation of this bar
@@ -463,21 +539,25 @@
 @dataclass(frozen=True, slots=True)
 class SimpleSynchronousBar(SynchronousBar):
     """Representation of a bar across staffs.
 
     Args:
         bars: the bars per staff.
     """
-    bars: dict[str_staff_name, Bar]
+    bars: frozendict[str_staff_name, Bar]
+
+    def __post_init__(self):
+        if not isinstance(self.bars, frozendict):
+            raise ValueError('Expects bars to be of type frozendict.')
 
     def get_staff_names(self) -> list[str_staff_name]:
         return list(self.bars.keys())
 
     def get_staffs(self) -> dict[str_staff_name, Bar]:
-        return self.bars
+        return dict(self.bars)
 
     def get_bar(self, staff_name: str_staff_name) -> Bar:
         return self.bars[staff_name]
 
     def get_bars(self) -> list[Bar]:
         return list(self.bars.values())
 
@@ -490,120 +570,313 @@
     are stored in a dictionary such that we can store the bars with their dice table label instead of a numerical index.
 
     Args:
         bar_collection: the collection of synchronous bars indexed by their bar index and staff name.
     """
     bar_collection: dict[int_bar_index, dict[str_staff_name, Bar]]
 
+    @property
+    def nmr_bars(self) -> int:
+        return len(self.bar_collection)
+
+    @property
+    def maximum_bar_ind(self) -> int:
+        return self.nmr_bars + 1
+
     def get_synchronous_bars(self) -> dict[int_bar_index, SynchronousBar]:
-        return {bar_index: SimpleSynchronousBar(bars) for bar_index, bars in self.bar_collection.items()}
+        return {bar_index: SimpleSynchronousBar(frozendict(bars)) for bar_index, bars in self.bar_collection.items()}
 
     def get_synchronous_bar(self, bar_index: int_bar_index) -> SynchronousBar:
-        return SimpleSynchronousBar(self.bar_collection[bar_index])
+        return SimpleSynchronousBar(frozendict(self.bar_collection[bar_index]))
 
     def get_staff_names(self) -> list[str_staff_name]:
         return list(self.bar_collection[1].keys())
 
     def get_bars(self, staff_name: str_staff_name) -> dict[int_bar_index, Bar]:
         return {bar_index: bars[staff_name] for bar_index, bars in self.bar_collection.items()}
 
     def get_bar(self, staff_name: str_staff_name, bar_index: int_bar_index) -> Bar:
         return self.bar_collection[bar_index][staff_name]
 
+    def get_synchronous_selection(self,
+                                  dice_table_elements: list[DiceTableElement]) -> list[tuple[SynchronousBar, ...]]:
+        bars = []
+        for element in dice_table_elements:
+            bar_tuplets = []
+            for bar_index in element.get_bar_indices():
+                bar_tuplets.append(self.get_synchronous_bar(bar_index))
+            bars.append(tuple(bar_tuplets))
+        return bars
+
+    def get_bar_selection(self,
+                          staff_name: str_staff_name,
+                          dice_table_elements: list[DiceTableElement]) -> list[tuple[Bar, ...]]:
+        bars = []
+        for element in dice_table_elements:
+            bar_tuplets = []
+            for bar_index in element.get_bar_indices():
+                bar_tuplets.append(self.get_bar(staff_name, bar_index))
+            bars.append(tuple(bar_tuplets))
+        return bars
+
 
 class DiceTable(metaclass=ABCMeta):
     """Representation of a dice table used in playing the dice games.
 
-    This assumes all entries in the dice game tables are integers mapping to a bars in the bar table.
+    This assumes all entries in the dice game tables are one or more bar indices mapping to a bars in the bar table.
+
+    Dice tables may select multiple bars per dice throw. This is used in some of the games, for instance Gerlach.
     """
 
     @property
     @abstractmethod
     def nmr_dices(self) -> int:
         """Get the number of dices this table needs."""
 
     @property
     @abstractmethod
+    def max_measures_per_throw(self) -> int:
+        """Get the maximum of measures selected per dice throw."""
+
+    @property
+    @abstractmethod
     def max_dice_value(self) -> int:
         """Get the maximum dice value needed to select row from this dice table."""
 
     @property
     @abstractmethod
     def nmr_throws(self) -> int:
         """Get the maximum number of throws needed to select all the columns from this dice table."""
 
     @abstractmethod
-    def list_rows(self) -> list[list[int]]:
-        """Get a list with the list of row values"""
+    def get_element(self, row: int, column: int) -> DiceTableElement:
+        """Get the dice table element at the specified location.
+
+        Args:
+            row: the row index
+            column: the column index
+
+        Returns:
+            The dice table element
+        """
+
+    @abstractmethod
+    def get_elements(self) -> list[DiceTableElement]:
+        """Get a list of all the dice table elements.
+
+        Returns:
+            A list of all the dice table elements
+        """
+
+    @abstractmethod
+    def list_rows(self) -> list[list[DiceTableElement]]:
+        """Get a list with the list of row values.
+
+        This returns a row view of the dice table, with for each row a list of dice table elements in the row.
+
+        Returns:
+            A row view of the dice table.
+        """
 
     @abstractmethod
-    def list_columns(self) -> list[list[int]]:
-        """Get a list with the list of column values"""
+    def list_columns(self) -> list[list[DiceTableElement]]:
+        """Get a list with the list of column values
+
+        This returns a column view of the dice table, with for each column a list of dice table elements in the column.
+
+        Returns:
+            A column view of the dice table.
+        """
 
     @abstractmethod
-    def get_column(self, column_ind: int) -> list[int]:
+    def get_column(self, column_ind: int) -> list[DiceTableElement]:
         """Get the column of the dice table at the indicated index.
 
         Args:
             column_ind: the index of the column (0 based)
 
         Returns:
-            The dice game labels in the indicated column
+            The dice game elements in the indicated column
         """
 
     @abstractmethod
-    def get_row(self, row_ind: int) -> list[int]:
+    def get_row(self, row_ind: int) -> list[DiceTableElement]:
         """Get the row of the dice table at the indicated index.
 
         Args:
             row_ind: the index of the row (0 based)
 
         Returns:
-            The dice game labels in the indicated row
+            The dice game elements in the indicated row
         """
 
+    @abstractmethod
+    def get_random_selection(self, seed: int = None) -> list[DiceTableElement]:
+        """Get a random selection of bar numbers
+
+        Returns:
+            A list of random bar numbers from the table
+        """
 
-@dataclass(slots=True, frozen=True)
-class SimpleDiceTable(DiceTable):
-    """Implementation of a dice table using a numpy array."""
-    table: np.ndarray
+
+class DiceTableElement(metaclass=ABCMeta):
+    """Representation of an element in a dice table."""
 
     @property
-    def nmr_dices(self) -> int:
-        return self.max_dice_value % 2
+    @abstractmethod
+    def row_ind(self) -> int:
+        """Get the row index of this selection.
+
+        Returns:
+            The row from which this bar selection was made.
+        """
 
     @property
-    def max_dice_value(self) -> int:
-        return self.table.shape[0]
+    @abstractmethod
+    def column_ind(self) -> int:
+        """Get the column index of this selection.
+
+        Returns:
+            The column from which this bar selection was made.
+        """
 
     @property
-    def nmr_throws(self) -> int:
-        return self.table.shape[1]
+    @abstractmethod
+    def nmr_bars_selected(self) -> int:
+        """Get the number of bars selected by this selection.
 
-    def list_rows(self) -> list[list[int]]:
-        return self.table.tolist()
+        Returns:
+            The number of bars selected by this measure.
+        """
 
-    def list_columns(self) -> list[list[int]]:
-        return self.table.T.tolist()
+    @abstractmethod
+    def get_bar_indices(self) -> tuple[int_bar_index, ...]:
+        """Get the bar indices.
 
-    def get_column(self, column_ind: int) -> list[int]:
-        return self.table[:, column_ind].tolist()
+        Returns:
+            The tuple of bars. This may contain only one element in the case of single selection.
+        """
 
-    def get_row(self, row_ind: int) -> list[int]:
-        return self.table[row_ind, :].tolist()
 
-    def get_random_selection(self, seed: int = None) -> list[int]:
-        """Get a random selection of bar numbers
+@dataclass(frozen=True, slots=True)
+class SimpleDiceTableElement(DiceTableElement):
+    """Dataclass implementation of the dice table element selection.
+
+    Args:
+        row: the row from which this element was selected
+        column: the column from which this element was selected
+        bar_indices: the selected bar indices
+    """
+    row: int
+    column: int
+    bar_indices: tuple[int_bar_index, ...]
+
+    @property
+    def row_ind(self) -> int:
+        return self.row
+
+    @property
+    def column_ind(self) -> int:
+        return self.column
+
+    @property
+    def nmr_bars_selected(self) -> int:
+        return len(self.bar_indices)
+
+    def get_bar_indices(self) -> tuple[int_bar_index, ...]:
+        return self.bar_indices
+
+
+@dataclass(slots=True, frozen=True)
+class SimpleDiceTable(DiceTable):
+    """Implementation of a dice table.
+
+    Args:
+        table: the dice table as a list of rows, with for each row the dice table elements
+        max_measures_per_throw: the maximum selected measures in the dice table.
+    """
+    table: list[list[DiceTableElement]]
+    max_measures_per_throw: int
+
+    @classmethod
+    def from_lists(cls, array: list[list[int_bar_index | tuple[int_bar_index, ...]]]) -> Self:
+        """Load this dice table from a simple list table of indices.
+
+        Args:
+            array: array with for each element one or more bar indices.
 
         Returns:
-            A list of random bar numbers from the table
+            An instance of this class.
         """
-        prng = RandomState(seed)
-        dice_throws = prng.randint(0, self.table.shape[0], self.table.shape[1])
-        return self.table[dice_throws, range(self.table.shape[1])].tolist()
+        table = []
+        max_measures_per_throw = 1
+
+        for row_ind, row in enumerate(array):
+            table_column = []
+            for column_ind, value in enumerate(row):
+                value_tuple = value
+                if isinstance(value, int_bar_index):
+                    value_tuple = (value,)
+                table_column.append(SimpleDiceTableElement(row_ind, column_ind, value_tuple))
+
+                if len(value_tuple) > max_measures_per_throw:
+                    max_measures_per_throw = len(value_tuple)
+
+            table.append(table_column)
+
+        return cls(table, max_measures_per_throw)
+
+    @property
+    def nmr_dices(self) -> int:
+        return math.ceil(self.max_dice_value / 6)
+
+    @property
+    def max_dice_value(self) -> int:
+        return len(self.table)
+
+    @property
+    def nmr_throws(self) -> int:
+        return len(self.table[0])
+
+    def get_element(self, row: int, column: int) -> DiceTableElement:
+        return self.table[row][column]
+
+    def get_elements(self) -> list[DiceTableElement]:
+        elements = []
+        for row in self.table:
+            for element in row:
+                elements.append(element)
+        return elements
+
+    def list_rows(self) -> list[list[DiceTableElement]]:
+        return self.table
+
+    def list_columns(self) -> list[list[DiceTableElement]]:
+        columns = []
+        for column_ind in range(len(self.table[0])):
+            column = []
+            for row in self.table:
+                column.append(row[column_ind])
+            columns.append(column)
+        return columns
+
+    def get_column(self, column_ind: int) -> list[DiceTableElement]:
+        return self.list_columns()[column_ind]
+
+    def get_row(self, row_ind: int) -> list[DiceTableElement]:
+        return self.list_rows()[row_ind]
+
+    def get_random_selection(self, seed: int = None) -> list[DiceTableElement]:
+        random.seed(seed)
+        max_val = self.max_dice_value - 1
+        selected_elements = []
+        for throw_ind in range(self.nmr_throws):
+            dice_throw = random.randint(0, max_val)
+            selected_elements.append(self.get_element(dice_throw, throw_ind))
+        return selected_elements
 
 
 class LilypondScore(metaclass=ABCMeta):
     """Representation of a lilypond score."""
 
     @abstractmethod
     def get_score(self) -> str:
@@ -645,86 +918,87 @@
     """Representation of a selection of bars chosen to compile into a dice game composition.
 
     This abstracts the notion of throwing the dice for a musical composition. We allow shuffling staffs within a dice
     table by selecting bar indices by table key and staff name.
     """
 
     @abstractmethod
-    def get_bar_index(self,
-                      table_name: str_dice_table_name,
-                      throw_ind: int,
-                      staff_name: str_staff_name | None = None) -> int_bar_index:
-        """Get the bar index for a specific dice table, a specified throw index and optionally a specific staff.
+    def get_dice_table_element(self,
+                               table_name: str_dice_table_name,
+                               throw_ind: int,
+                               staff_name: str_staff_name | None = None) -> DiceTableElement:
+        """Get the dice table element for a specific dice table, throw index and optionally a specific staff.
 
         Args:
             table_name: the name of the dice table we have indices for
             throw_ind: the index of the dice throw
             staff_name: optionally, within the table, the staff for which we are selecting bar indices.
 
         Returns:
-            The selected bar for this dice table, dice throw and staff.
+            The dice table elements for this dice table, dice throw and staff.
         """
 
     @abstractmethod
-    def get_bar_indices(self,
-                        table_name: str_dice_table_name,
-                        staff_name: str_staff_name | None = None) -> list[int_bar_index]:
-        """Get the bar indices chosen for the specific dice table and staff (within that dice table).
+    def get_dice_table_elements(self,
+                                table_name: str_dice_table_name,
+                                staff_name: str_staff_name | None = None) -> list[DiceTableElement]:
+        """Get the dice table elements chosen for the specific dice table and staff (within that dice table).
 
         For a given table, this may either return the same bar indices for each staff, or a different list per staff.
 
         Args:
             table_name: the name of the dice table we have indices for
             staff_name: optionally, within the table, the staff for which we are selecting bar indices.
 
         Returns:
-            The selected bar for this dice table, dice throw and staff.
+            The selected dice table elements for this dice table, dice throw and staff.
         """
 
 
 @dataclass(slots=True, frozen=True)
 class GroupedStaffsBarSelection(BarSelection):
     """Bar selection where we select the same bar indices for each staff of a dice table.
 
     Args:
-        bar_indices: for each table key, the list of bars we want to select in the composition.
+        dice_table_elements: for each table key, the list of dice table elements we want to select in the composition.
     """
-    bar_indices: dict[str_dice_table_name, list[int_bar_index]]
+    dice_table_elements: dict[str_dice_table_name, list[DiceTableElement]]
 
-    def get_bar_index(self,
-                      table_name: str_dice_table_name,
-                      throw_ind: int,
-                      staff_name: str_staff_name | None = None) -> int_bar_index:
-        return self.bar_indices[table_name][throw_ind]
-
-    def get_bar_indices(self,
-                        table_name: str_dice_table_name,
-                        staff_name: str_staff_name | None = None) -> list[int_bar_index]:
-        return self.bar_indices[table_name]
+    def get_dice_table_element(self,
+                               table_name: str_dice_table_name,
+                               throw_ind: int,
+                               staff_name: str_staff_name | None = None) -> DiceTableElement:
+       return self.dice_table_elements[table_name][throw_ind]
+
+    def get_dice_table_elements(self,
+                                table_name: str_dice_table_name,
+                                staff_name: str_staff_name | None = None) -> list[DiceTableElement]:
+        return self.dice_table_elements[table_name]
 
 
 @dataclass(slots=True, frozen=True)
 class PerStaffsBarSelection(BarSelection):
     """Bar selection where we may select different bar indices for each staff of a dice table.
 
     Args:
-        bar_indices: for each table key, and for each staff, the list of bars we want to select in the composition.
+        dice_table_elements: for each table key, and for each staff, the list of bars we want to
+            select in the composition.
     """
-    bar_indices: dict[str_dice_table_name, dict[str_staff_name, list[int_bar_index]]]
+    dice_table_elements: dict[str_dice_table_name, dict[str_staff_name, list[DiceTableElement]]]
 
-    def get_bar_index(self,
-                      table_name: str_dice_table_name,
-                      throw_ind: int,
-                      staff_name: str_staff_name | None = None) -> int_bar_index:
-        return self.bar_indices[table_name][staff_name][throw_ind]
-
-    def get_bar_indices(self,
-                        table_name: str_dice_table_name,
-                        staff_name: str_staff_name | None = None) -> list[int_bar_index]:
-        return self.bar_indices[table_name][staff_name]
+    def get_dice_table_element(self,
+                               table_name: str_dice_table_name,
+                               throw_ind: int,
+                               staff_name: str_staff_name | None = None) -> DiceTableElement:
+        return self.dice_table_elements[table_name][staff_name][throw_ind]
+
+    def get_dice_table_elements(self,
+                                table_name: str_dice_table_name,
+                                staff_name: str_staff_name | None = None) -> list[DiceTableElement]:
+        return self.dice_table_elements[table_name][staff_name]
 
 
 class MidiSettings(metaclass=ABCMeta):
 
     @abstractmethod
     def get_midi_instrument(self, table_name: str_dice_table_name, staff_name: str_staff_name) -> str:
         """Get the midi instrument to use for rendering the specific table and specific staff.
```

### Comparing `musical_games-0.7.0/musical_games/dice_games/data_csv.py` & `musical_games-0.7.1/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/dice_games/dice_games.py` & `musical_games-0.7.1/musical_games/dice_games/dice_games.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,49 +3,48 @@
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from importlib import resources
 
 import jinja2
-import numpy as np
 
 from musical_games.dice_games.base import (SimpleDiceTable, SimpleMidiSettings, SimpleDiceGame)
 from musical_games.dice_games.data_csv import SimpleBarCollectionCSVReader
 
 
 class CPEBachCounterpoint(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Counterpoint dice by C.P.E. Bach.
 
         In this dice game, the right hand and left hand of the piano piece are shuffled independently by two
         dice tables.
         """
         dice_tables = {
-            'treble': SimpleDiceTable(np.array([
+            'treble': SimpleDiceTable.from_lists([
                 [1, 10, 19, 28, 37, 46],
                 [2, 11, 20, 29, 38, 47],
                 [3, 12, 21, 30, 39, 48],
                 [4, 13, 22, 31, 40, 49],
                 [5, 14, 23, 32, 41, 50],
                 [6, 15, 24, 33, 42, 51],
                 [7, 16, 25, 34, 43, 52],
                 [8, 17, 26, 35, 44, 53],
-                [9, 18, 27, 36, 45, 54]])),
-            'bass': SimpleDiceTable(np.array([
+                [9, 18, 27, 36, 45, 54]]),
+            'bass': SimpleDiceTable.from_lists([
                 [1, 10, 19, 28, 37, 46],
                 [2, 11, 20, 29, 38, 47],
                 [3, 12, 21, 30, 39, 48],
                 [4, 13, 22, 31, 40, 49],
                 [5, 14, 23, 32, 41, 50],
                 [6, 15, 24, 33, 42, 51],
                 [7, 16, 25, 34, 43, 52],
                 [8, 17, 26, 35, 44, 53],
-                [9, 18, 27, 36, 45, 54]])),
+                [9, 18, 27, 36, 45, 54]]),
         }
 
         csv_reader = SimpleBarCollectionCSVReader()
         treble_bars = csv_reader.read_csv(resources.files('musical_games')
                                           / 'data/dice_games/cpe_bach_counterpoint/bars_treble.csv')
         bass_bars = csv_reader.read_csv(resources.files('musical_games')
                                         / 'data/dice_games/cpe_bach_counterpoint/bars_bass.csv')
@@ -59,37 +58,36 @@
             {'treble': {'piano_right_hand': 0}, 'bass': {'piano_left_hand': 0}},
             {'treble': {'piano_right_hand': 1}, 'bass': {'piano_left_hand': 0.75}})
 
         super().__init__('C.P.E. Bach', 'Counterpoint', dice_tables, {'treble': treble_bars, 'bass': bass_bars},
                          jinja2_environment, midi_settings)
 
 
-
 class KirnbergerMenuetTrio(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Menuet and Trio dice game by Kirnberger.
 
         In this dice game, there is a dice table for the menuet and one for the trio.
         """
         dice_tables = {
-            'menuet': SimpleDiceTable(np.array([
+            'menuet': SimpleDiceTable.from_lists([
                 [23, 77, 62, 70, 29, 83, 59, 36, 33, 60, 21, 14, 45, 68, 26, 40],
                 [63, 54, 2, 53, 41, 37, 71, 90, 55, 46, 88, 39, 65, 6, 91, 81],
                 [79, 75, 42, 5, 50, 69, 52, 8, 4, 12, 94, 9, 25, 35, 66, 24],
                 [13, 57, 64, 74, 11, 3, 67, 73, 95, 78, 80, 30, 1, 51, 82, 16],
                 [43, 7, 86, 31, 18, 89, 87, 58, 38, 93, 15, 92, 28, 61, 72, 85],
-                [32, 47, 84, 20, 22, 49, 56, 48, 44, 76, 34, 19, 17, 10, 27, 96]])),
-            'trio': SimpleDiceTable(np.array([
+                [32, 47, 84, 20, 22, 49, 56, 48, 44, 76, 34, 19, 17, 10, 27, 96]]),
+            'trio': SimpleDiceTable.from_lists([
                 [81, 57, 67, 2, 90, 41, 24, 56, 94, 47, 62, 72, 25, 64, 48, 87],
                 [78, 45, 30, 65, 14, 33, 10, 73, 40, 55, 46, 17, 31, 85, 11, 76],
                 [8, 69, 26, 53, 43, 95, 88, 63, 79, 5, 3, 60, 54, 21, 42, 82],
                 [84, 6, 4, 22, 51, 12, 83, 92, 58, 93, 66, 23, 15, 13, 27, 32],
                 [39, 28, 18, 35, 89, 75, 61, 96, 7, 91, 70, 1, 74, 44, 52, 50],
-                [59, 71, 37, 16, 86, 49, 77, 20, 38, 68, 19, 29, 80, 36, 34, 9]])),
+                [59, 71, 37, 16, 86, 49, 77, 20, 38, 68, 19, 29, 80, 36, 34, 9]]),
         }
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'menuet': csv_reader.read_csv(resources.files('musical_games') /
                                                          'data/dice_games/kirnberger_menuet_trio/menuet_bars.csv'),
                            'trio': csv_reader.read_csv(resources.files('musical_games') /
                                                        'data/dice_games/kirnberger_menuet_trio/trio_bars.csv')}
@@ -114,26 +112,26 @@
 
     def __init__(self):
         """Implementation of a Polonaise dice game by Kirnberger.
 
         This dice game has measures for a piano part and two violin parts.
         """
         dice_tables = {
-            'polonaise': SimpleDiceTable(np.array([
+            'polonaise': SimpleDiceTable.from_lists([
                 [70, 34, 68, 18, 32, 58, 80, 11, 59, 35, 74, 13, 21, 33],
                 [10, 24, 50, 46, 14, 26, 22, 77, 65, 5, 27, 71, 15, 39],
                 [42, 6, 60, 2, 52, 66, 82, 3, 9, 83, 67, 1, 53, 25],
                 [62, 8, 36, 12, 16, 38, 43, 41, 45, 17, 37, 49, 73, 23],
                 [44, 56, 40, 79, 48, 54, 78, 84, 29, 76, 61, 57, 51, 75],
                 [72, 30, 4, 28, 22, 64, 69, 63, 7, 47, 19, 31, 81, 55],
                 [114, 112, 126, 87, 89, 88, 90, 93, 86, 94, 96, 85, 95, 104],
                 [123, 116, 137, 110, 91, 98, 129, 99, 107, 122, 105, 93, 106, 121],
                 [131, 147, 143, 113, 101, 115, 103, 140, 111, 145, 133, 109, 117, 125],
                 [138, 151, 118, 124, 141, 127, 142, 149, 97, 134, 120, 100, 119, 132],
-                [144, 153, 146, 128, 150, 154, 152, 102, 135, 148, 136, 108, 130, 139]]))
+                [144, 153, 146, 128, 150, 154, 152, 102, 135, 148, 136, 108, 130, 139]])
         }
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'polonaise': csv_reader.read_csv(resources.files('musical_games') /
                                                             'data/dice_games/kirnberger_polonaise/polonaise_bars.csv')}
 
         template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/kirnberger_polonaise/lilypond')
@@ -148,67 +146,31 @@
             {'polonaise': {'piano_right_hand': 0.75, 'piano_left_hand': 0.6,
                            'violin_1': 0.8625, 'violin_2': 0.8625}})
 
         super().__init__('Kirnberger', 'Polonaise', dice_tables, bar_collections,
                          jinja2_environment, midi_settings)
 
 
-class MozartWaltz(SimpleDiceGame):
-
-    def __init__(self):
-        """Implementation of a Waltz dice game by Mozart."""
-        dice_tables = {
-            'waltz': SimpleDiceTable(np.array([
-                [96, 22, 141, 41, 105, 122, 11, 30, 70, 121, 26, 9, 112, 49, 109, 14],
-                [32, 6, 128, 63, 146, 46, 134, 81, 117, 39, 126, 56, 174, 18, 116, 83],
-                [69, 95, 158, 13, 153, 55, 110, 24, 66, 139, 15, 132, 73, 58, 145, 79],
-                [40, 17, 113, 85, 161, 2, 159, 100, 90, 176, 7, 34, 67, 160, 52, 170],
-                [148, 74, 163, 45, 80, 97, 36, 107, 25, 143, 64, 125, 76, 136, 1, 93],
-                [104, 157, 27, 167, 154, 68, 118, 91, 138, 71, 150, 29, 101, 162, 23, 151],
-                [152, 60, 171, 53, 99, 133, 21, 127, 16, 155, 57, 175, 43, 168, 89, 172],
-                [119, 84, 114, 50, 140, 86, 169, 94, 120, 88, 48, 166, 51, 115, 72, 111],
-                [98, 142, 42, 156, 75, 129, 62, 123, 65, 77, 19, 82, 137, 38, 149, 8],
-                [3, 87, 165, 61, 135, 47, 147, 33, 102, 4, 31, 164, 144, 59, 173, 78],
-                [54, 130, 10, 103, 28, 37, 106, 5, 35, 20, 108, 92, 12, 124, 44, 131]]))
-        }
-
-        csv_reader = SimpleBarCollectionCSVReader()
-        bar_collections = {'waltz': csv_reader.read_csv(resources.files('musical_games') /
-                                                        'data/dice_games/mozart_waltz/waltz_bars.csv')}
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/mozart_waltz/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
-
-        midi_settings = SimpleMidiSettings(
-            {'waltz': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
-            {'waltz': {'piano_right_hand': 0, 'piano_left_hand': 0}},
-            {'waltz': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
-
-        super().__init__('Mozart', 'Waltz', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
-
-
 class MozartContredanse(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Contredanse dice game by Mozart."""
         dice_tables = {
-            'contredanse': SimpleDiceTable(np.array([
+            'contredanse': SimpleDiceTable.from_lists([
                 [70, 14, 164, 122, 25, 153, 18, 167, 155, 3, 162, 170, 13, 166, 95, 5],
                 [10, 64, 100, 12, 149, 30, 161, 11, 148, 28, 135, 173, 169, 174, 2, 20],
                 [33, 1, 160, 163, 77, 156, 168, 172, 22, 176, 62, 126, 31, 24, 159, 41],
                 [36, 114, 8, 35, 111, 39, 137, 44, 4, 157, 38, 9, 151, 32, 17, 171],
                 [105, 150, 57, 71, 117, 52, 132, 130, 136, 91, 138, 19, 134, 101, 154, 146],
                 [165, 152, 112, 15, 147, 27, 73, 102, 144, 104, 87, 107, 128, 48, 109, 74],
                 [7, 81, 131, 37, 21, 125, 49, 115, 116, 133, 72, 141, 94, 80, 129, 65],
                 [142, 106, 40, 69, 43, 140, 23, 89, 66, 124, 26, 84, 75, 103, 96, 127],
                 [99, 68, 86, 139, 120, 92, 143, 83, 93, 55, 29, 51, 42, 110, 108, 98],
                 [85, 45, 90, 158, 82, 123, 78, 58, 61, 34, 119, 46, 59, 54, 60, 47],
-                [145, 97, 6, 121, 56, 67, 63, 16, 50, 79, 175, 76, 113, 88, 53, 118]]))
+                [145, 97, 6, 121, 56, 67, 63, 16, 50, 79, 175, 76, 113, 88, 53, 118]])
         }
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'contredanse': csv_reader.read_csv(resources.files('musical_games') /
                                                         'data/dice_games/mozart_contredanse/contredanse_bars.csv')}
 
         template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/mozart_contredanse/lilypond')
@@ -219,44 +181,79 @@
             {'contredanse': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'contredanse': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'contredanse': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Mozart', 'Contredanse', dice_tables, bar_collections,
                          jinja2_environment, midi_settings)
 
+class MozartWaltz(SimpleDiceGame):
+
+    def __init__(self):
+        """Implementation of a Waltz dice game by Mozart."""
+        dice_tables = {
+            'waltz': SimpleDiceTable.from_lists([
+                [96, 22, 141, 41, 105, 122, 11, 30, 70, 121, 26, 9, 112, 49, 109, 14],
+                [32, 6, 128, 63, 146, 46, 134, 81, 117, 39, 126, 56, 174, 18, 116, 83],
+                [69, 95, 158, 13, 153, 55, 110, 24, 66, 139, 15, 132, 73, 58, 145, 79],
+                [40, 17, 113, 85, 161, 2, 159, 100, 90, 176, 7, 34, 67, 160, 52, 170],
+                [148, 74, 163, 45, 80, 97, 36, 107, 25, 143, 64, 125, 76, 136, 1, 93],
+                [104, 157, 27, 167, 154, 68, 118, 91, 138, 71, 150, 29, 101, 162, 23, 151],
+                [152, 60, 171, 53, 99, 133, 21, 127, 16, 155, 57, 175, 43, 168, 89, 172],
+                [119, 84, 114, 50, 140, 86, 169, 94, 120, 88, 48, 166, 51, 115, 72, 111],
+                [98, 142, 42, 156, 75, 129, 62, 123, 65, 77, 19, 82, 137, 38, 149, 8],
+                [3, 87, 165, 61, 135, 47, 147, 33, 102, 4, 31, 164, 144, 59, 173, 78],
+                [54, 130, 10, 103, 28, 37, 106, 5, 35, 20, 108, 92, 12, 124, 44, 131]])
+        }
+
+        csv_reader = SimpleBarCollectionCSVReader()
+        bar_collections = {'waltz': csv_reader.read_csv(resources.files('musical_games') /
+                                                        'data/dice_games/mozart_waltz/waltz_bars.csv')}
+
+        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/mozart_waltz/lilypond')
+        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
+        jinja2_environment = jinja2.Environment(**env_options)
+
+        midi_settings = SimpleMidiSettings(
+            {'waltz': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
+            {'waltz': {'piano_right_hand': 0, 'piano_left_hand': 0}},
+            {'waltz': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
+
+        super().__init__('Mozart', 'Waltz', dice_tables, bar_collections,
+                         jinja2_environment, midi_settings)
+
 
 class StadlerMenuetTrio(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Menuet and Trio dice game by Stadler.
 
         A similar dice game has been made by Haydn.
 
         In this dice game, there is a dice table for the menuet and one for the trio.
         """
         dice_tables = {
-            'menuet': SimpleDiceTable(np.array([
+            'menuet': SimpleDiceTable.from_lists([
                 [96, 22, 141, 41, 105, 122, 11, 30, 70, 121, 26, 9, 112, 49, 109, 14],
                 [32, 6, 128, 63, 146, 46, 134, 81, 117, 39, 126, 56, 174, 18, 116, 83],
                 [69, 95, 158, 13, 153, 55, 110, 24, 66, 139, 15, 132, 73, 58, 145, 79],
                 [40, 17, 113, 85, 161, 2, 159, 100, 90, 176, 7, 34, 67, 160, 52, 170],
                 [148, 74, 163, 45, 80, 97, 36, 107, 25, 143, 64, 125, 76, 136, 1, 93],
                 [104, 157, 27, 167, 154, 68, 118, 91, 138, 71, 150, 29, 101, 162, 23, 151],
                 [152, 60, 171, 53, 99, 133, 21, 127, 16, 155, 57, 175, 43, 168, 89, 172],
                 [119, 84, 114, 50, 140, 86, 169, 94, 120, 88, 48, 166, 51, 115, 72, 111],
                 [98, 142, 42, 156, 75, 129, 62, 123, 65, 77, 19, 82, 137, 38, 149, 8],
                 [3, 87, 165, 61, 135, 47, 147, 33, 102, 4, 31, 164, 144, 59, 173, 78],
-                [54, 130, 10, 103, 28, 37, 106, 5, 35, 20, 108, 92, 12, 124, 44, 131]])),
-            'trio': SimpleDiceTable(np.array([
+                [54, 130, 10, 103, 28, 37, 106, 5, 35, 20, 108, 92, 12, 124, 44, 131]]),
+            'trio': SimpleDiceTable.from_lists([
                 [72, 6, 59, 25, 81, 41, 89, 13, 36, 5, 46, 79, 30, 95, 19, 66],
                 [56, 82, 42, 74, 14, 7, 26, 71, 76, 20, 64, 84, 8, 35, 47, 88],
                 [75, 39, 54, 1, 65, 43, 15, 80, 9, 34, 93, 48, 69, 58, 90, 21],
                 [40, 73, 16, 68, 29, 55, 2, 61, 22, 67, 49, 77, 57, 87, 33, 10],
                 [83, 3, 28, 53, 37, 17, 44, 70, 63, 85, 32, 96, 12, 23, 50, 91],
-                [18, 45, 62, 38, 4, 27, 52, 94, 11, 92, 24, 86, 51, 60, 78, 31]])),
+                [18, 45, 62, 38, 4, 27, 52, 94, 11, 92, 24, 86, 51, 60, 78, 31]]),
         }
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'menuet': csv_reader.read_csv(resources.files('musical_games') /
                                                          'data/dice_games/stadler_menuet_trio/menuet_bars.csv'),
                            'trio': csv_reader.read_csv(resources.files('musical_games') /
                                                        'data/dice_games/stadler_menuet_trio/trio_bars.csv')}
```

### Comparing `musical_games-0.7.0/musical_games/external/base.py` & `musical_games-0.7.1/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/external/images.py` & `musical_games-0.7.1/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/external/lilypond.py` & `musical_games-0.7.1/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/external/midi_converters.py` & `musical_games-0.7.1/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/external/utils.py` & `musical_games-0.7.1/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/external/wav_converters.py` & `musical_games-0.7.1/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/musical_games/utils.py` & `musical_games-0.7.1/musical_games/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,37 +12,39 @@
 from musical_games.external.wav_converters import wav_to_mp3, wav_to_ogg
 from musical_games.external.midi_converters import midi_to_wav
 from musical_games.external.lilypond import typeset_lilypond, LilypondTypesetResults
 
 
 def auto_convert_lilypond_file(lilypond_in: Path, soundfont: Path | None = None, output_basename: Path | None = None,
                                pdf: bool = True, png: bool = True, ps: bool = False, mp3: bool = True,
-                               ogg: bool = True, midi_gain: float | None = None) -> AutoConvertLilypondResults:
+                               ogg: bool = True, midi_gain: float | None = None,
+                               trim_png: bool = True) -> AutoConvertLilypondResults:
     """Converts a lilypond file to pdf, png, midi, wav, mp3 and ogg.
 
     Given a lilypond file we create some common output files you are typically interested in.
 
     Args:
         lilypond_in: the lilypond file name
         soundfont: the path to the soundfont to use. If not given we will not convert to wav, mp3 and ogg.
         output_basename: path + file prefix. If None we use the dir and basename of the lilypond file.
         pdf: if we want pdf output
         png: if we want png output
         ps: if we want postscript output
         mp3: if we want mp3 output, only applicable if the lilypond has midi output defined
         ogg: if we want ogg output, only applicable if the lilypond has midi output defined
         midi_gain: the gain for use during the midi to wav conversion
+        trim_png: if we want to automatically trim the png outputs
 
     Returns:
         Information about the file names that were outputted
     """
     if not output_basename:
         output_basename = lilypond_in.parent / lilypond_in.stem
 
-    typeset_results = typeset_lilypond(lilypond_in, output_basename, pdf=pdf, png=png, ps=ps)
+    typeset_results = typeset_lilypond(lilypond_in, output_basename, pdf=pdf, png=png, ps=ps, trim_png=trim_png)
 
     wav_list = []
     mp3_list = []
     ogg_list = []
 
     with ThreadPoolExecutor() as executor:
         for midi_conversion_result in executor.map(lambda midi_file: _convert_midi(midi_file, soundfont=soundfont,
```

### Comparing `musical_games-0.7.0/scripts/copy_bars.py` & `musical_games-0.7.1/scripts/copy_bars.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/scripts/demo_cpe_bach.py` & `musical_games-0.7.1/scripts/demo_cpe_bach.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 __author__ = 'Robbert Harms'
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
+from pprint import pprint
+
 from musical_games.dice_games.dice_games import CPEBachCounterpoint
 from musical_games.utils import auto_convert_lilypond_file
 
-out_dir = Path('/tmp/test2')
+out_dir = Path('/tmp/test')
 
 dice_game = CPEBachCounterpoint()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
 dice_game.compile_single_bar('treble', 1).to_file(out_dir / 'bar_treble_1.ly')
 auto_convert_lilypond_file(out_dir / 'bar_treble_1.ly')
 dice_game.compile_single_bar('bass', 1).to_file(out_dir / 'bar_bass_1.ly')
 auto_convert_lilypond_file(out_dir / 'bar_bass_1.ly')
 
-print(dice_game.get_all_duplicate_bars())
+dice_game.compile_single_dice_table_element('treble', dice_game.get_dice_tables()['treble'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_0.ly')
+
+pprint(dice_game.get_duplicate_dice_table_elements('treble'))
+pprint(dice_game.get_duplicate_dice_table_elements('bass'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
 dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
                                     comment='Test').to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
```

### Comparing `musical_games-0.7.0/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.7.1/scripts/demo_kirnberger_meneut_trio.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,27 +5,35 @@
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
 
 from musical_games.dice_games.dice_games import KirnbergerMenuetTrio
 from musical_games.utils import auto_convert_lilypond_file
 
-out_dir = Path('/tmp/test2')
+out_dir = Path('/tmp/test')
 
 dice_game = KirnbergerMenuetTrio()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
 dice_game.compile_single_bar('menuet', 1).to_file(out_dir / 'bar_menuet_1.ly')
 auto_convert_lilypond_file(out_dir / 'bar_menuet_1.ly')
 dice_game.compile_single_bar('trio', 1).to_file(out_dir / 'bar_trio_1.ly')
 auto_convert_lilypond_file(out_dir / 'bar_trio_1.ly')
 
-print(dice_game.get_all_duplicate_bars())
+dice_game.compile_single_dice_table_element('menuet', dice_game.get_dice_tables()['menuet'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_menuet_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_menuet_0.ly')
+dice_game.compile_single_dice_table_element('trio', dice_game.get_dice_tables()['trio'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_trio_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_0.ly')
+
+print(dice_game.get_duplicate_dice_table_elements('menuet'))
+print(dice_game.get_duplicate_dice_table_elements('trio'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
 dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
                                     comment='Test').to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
```

### Comparing `musical_games-0.7.0/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.7.1/scripts/demo_mozart_contredanse.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,41 +2,42 @@
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
 
-from musical_games.dice_games.dice_games import KirnbergerPolonaise
+from musical_games.dice_games.dice_games import MozartContredanse
 from musical_games.utils import auto_convert_lilypond_file
 
-out_dir = Path('/tmp/test2')
+out_dir = Path('/tmp/test')
 
-dice_game = KirnbergerPolonaise()
+dice_game = MozartContredanse()
 
-dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
+dice_game.compile_bars_overview(single_page=False).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-dice_game.compile_single_bar('polonaise', 1).to_file(out_dir / 'bar_polonaise_1.ly')
-auto_convert_lilypond_file(out_dir / 'bar_polonaise_1.ly')
+dice_game.compile_single_bar('contredanse', 11).to_file(out_dir / 'bar_contredanse_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_contredanse_1.ly')
 
-print(dice_game.get_all_duplicate_bars())
-print(dice_game.get_duplicate_bars('polonaise', 88))
+dice_game.compile_single_dice_table_element('contredanse',
+                                            dice_game.get_dice_tables()['contredanse'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_contredanse_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_contredanse_0.ly')
+
+print(dice_game.get_duplicate_dice_table_elements('contredanse'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
-print(dice_game.get_random_bar_selection(shuffle_staffs=False, seed=0))
-print(dice_game.get_random_bar_selection(shuffle_staffs=True, seed=0))
-
-dice_game.compile_composition_score(dice_game.get_random_bar_selection(shuffle_staffs=True, seed=0),
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
 midi_settings = dice_game.get_default_midi_settings()
-my_midi_settings = midi_settings.with_updated_instrument('flute', 'polonaise', 'violin_1')
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'contredanse', 'piano_right_hand')
 
 dice_game.compile_composition_audio(
     dice_game.get_random_bar_selection(seed=0),
     midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
 
 auto_convert_lilypond_file(
     out_dir / 'composition_midi.ly',
```

### Comparing `musical_games-0.7.0/scripts/demo_mozart_contredanse.py` & `musical_games-0.7.1/scripts/demo_mozart_waltz.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,42 @@
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
 
-from musical_games.dice_games.dice_games import MozartContredanse
+from musical_games.dice_games.dice_games import MozartWaltz
 from musical_games.utils import auto_convert_lilypond_file
 
-out_dir = Path('/tmp/test2')
+out_dir = Path('/tmp/test')
 
-dice_game = MozartContredanse()
+dice_game = MozartWaltz()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-dice_game.compile_single_bar('contredanse', 11).to_file(out_dir / 'bar_contredanse_1.ly')
-auto_convert_lilypond_file(out_dir / 'bar_contredanse_1.ly')
+dice_game.compile_single_bar('waltz', 5).to_file(out_dir / 'bar_waltz_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_waltz_1.ly')
 
-print(dice_game.get_all_duplicate_bars())
+dice_game.compile_single_dice_table_element('waltz',
+                                            dice_game.get_dice_tables()['waltz'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_waltz_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_waltz_0.ly')
+
+print(dice_game.get_duplicate_dice_table_elements('waltz'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
-dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=1, shuffle_staffs=False),
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
 midi_settings = dice_game.get_default_midi_settings()
-my_midi_settings = midi_settings.with_updated_instrument('flute', 'contredanse', 'piano_right_hand')
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'waltz', 'piano_right_hand')
 
 dice_game.compile_composition_audio(
     dice_game.get_random_bar_selection(seed=0),
     midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
 
 auto_convert_lilypond_file(
     out_dir / 'composition_midi.ly',
```

### Comparing `musical_games-0.7.0/scripts/demo_mozart_waltz.py` & `musical_games-0.7.1/scripts/demo_kirnberger_polonaise.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
 
-from musical_games.dice_games.dice_games import MozartWaltz
+from musical_games.dice_games.dice_games import KirnbergerPolonaise
 from musical_games.utils import auto_convert_lilypond_file
 
-out_dir = Path('/tmp/test2')
+out_dir = Path('/tmp/test')
 
-dice_game = MozartWaltz()
+dice_game = KirnbergerPolonaise()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-dice_game.compile_single_bar('waltz', 5).to_file(out_dir / 'bar_waltz_1.ly')
-auto_convert_lilypond_file(out_dir / 'bar_waltz_1.ly')
+dice_game.compile_single_bar('polonaise', 1).to_file(out_dir / 'bar_polonaise_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_polonaise_1.ly')
 
-print(dice_game.get_all_duplicate_bars())
+dice_game.compile_single_dice_table_element('polonaise',
+                                            dice_game.get_dice_tables()['polonaise'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_polonaise_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_polonaise_0.ly')
+
+print(dice_game.get_duplicate_dice_table_elements('polonaise'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
-dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0, shuffle_staffs=True),
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
 midi_settings = dice_game.get_default_midi_settings()
-my_midi_settings = midi_settings.with_updated_instrument('flute', 'waltz', 'piano_right_hand')
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'polonaise', 'violin_1')
 
 dice_game.compile_composition_audio(
     dice_game.get_random_bar_selection(seed=0),
     midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
 
 auto_convert_lilypond_file(
     out_dir / 'composition_midi.ly',
     soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
-
+#
```

### Comparing `musical_games-0.7.0/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.7.1/scripts/demo_stadler_meneut_trio.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,27 +5,38 @@
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
 
 from musical_games.dice_games.dice_games import StadlerMenuetTrio
 from musical_games.utils import auto_convert_lilypond_file
 
-out_dir = Path('/tmp/test2')
+out_dir = Path('/tmp/test')
 
 dice_game = StadlerMenuetTrio()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
 dice_game.compile_single_bar('menuet', 1).to_file(out_dir / 'bar_menuet_1.ly')
 auto_convert_lilypond_file(out_dir / 'bar_menuet_1.ly')
 dice_game.compile_single_bar('trio', 1).to_file(out_dir / 'bar_trio_1.ly')
 auto_convert_lilypond_file(out_dir / 'bar_trio_1.ly')
 
-print(dice_game.get_all_duplicate_bars())
+dice_game.compile_single_dice_table_element('menuet',
+                                            dice_game.get_dice_tables()['menuet'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_menuet_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_menuet_0.ly')
+
+dice_game.compile_single_dice_table_element('trio',
+                                            dice_game.get_dice_tables()['trio'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_trio_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_0.ly')
+
+print(dice_game.get_duplicate_dice_table_elements('menuet'))
+print(dice_game.get_duplicate_dice_table_elements('trio'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
 dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
```

### Comparing `musical_games-0.7.0/tox.ini` & `musical_games-0.7.1/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.7.0/PKG-INFO` & `musical_games-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.7.0
+Version: 0.7.1
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: numpy~=1.26.4
 Requires-Dist: Jinja2~=3.1.3
+Requires-Dist: frozendict~=2.4.1
 Requires-Dist: sphinx~=7.2.6 ; extra == "doc"
 Requires-Dist: pytest~=8.0.2 ; extra == "test"
 Requires-Dist: pytest-check~=2.3.1 ; extra == "test"
 Requires-Dist: pytest-cov~=4.1.0 ; extra == "test"
 Requires-Dist: pytest-html~=4.1.1 ; extra == "test"
 Requires-Dist: tox~=4.14.1 ; extra == "test"
 Provides-Extra: doc
```

