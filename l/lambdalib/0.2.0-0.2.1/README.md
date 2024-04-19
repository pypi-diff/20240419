# Comparing `tmp/lambdalib-0.2.0.tar.gz` & `tmp/lambdalib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdalib-0.2.0.tar", last modified: Mon Mar  4 16:32:21 2024, max compression
+gzip compressed data, was "lambdalib-0.2.1.tar", last modified: Fri Apr 19 18:25:09 2024, max compression
```

## Comparing `lambdalib-0.2.0.tar` & `lambdalib-0.2.1.tar`

### file list

```diff
@@ -1,209 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.155475 lambdalib-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.127475 lambdalib-0.2.0/.github/workflows/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.github/workflows/bin/format_verilog.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.github/workflows/ci.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.127475 lambdalib-0.2.0/.github/workflows/config/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.github/workflows/config/verible.rules
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-04 16:32:03.000000 lambdalib-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-04 16:32:03.000000 lambdalib-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-04 16:32:21.155475 lambdalib-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-04 16:32:03.000000 lambdalib-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.127475 lambdalib-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 16:32:03.000000 lambdalib-0.2.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.127475 lambdalib-0.2.0/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-04 16:32:03.000000 lambdalib-0.2.0/docs/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.127475 lambdalib-0.2.0/lambdalib/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/lambdalib/iolib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.131475 lambdalib-0.2.0/lambdalib/iolib/rtl/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioanalog.v
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iobidir.v
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioclamp.v
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iocorner.v
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iocut.v
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioinput.v
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iopoc.v
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioshort.v
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovdd.v
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovdda.v
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovddio.v
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovss.v
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovssa.v
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovssio.v
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioxtal.v
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/iolib/rtl/la_pt.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/lambdalib/padring/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.131475 lambdalib-0.2.0/lambdalib/padring/rtl/
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/padring/rtl/la_iopadring.v
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/padring/rtl/la_iopadring.vh
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/padring/rtl/la_ioside.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.131475 lambdalib-0.2.0/lambdalib/padring/testbench/
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/padring/testbench/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/padring/testbench/tb_la_iopadring.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/lambdalib/ramlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.131475 lambdalib-0.2.0/lambdalib/ramlib/rtl/
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/ramlib/rtl/la_asyncfifo.v
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/ramlib/rtl/la_dpram.v
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/ramlib/rtl/la_spram.v
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/ramlib/rtl/la_spregfile.v
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/ramlib/rtl/la_syncfifo.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/lambdalib/stdlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.151475 lambdalib-0.2.0/lambdalib/stdlib/rtl/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_and2.v
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_and3.v
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_and4.v
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_antenna.v
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao21.v
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao211.v
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao22.v
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao221.v
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao222.v
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao31.v
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao311.v
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao32.v
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao33.v
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi21.v
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi211.v
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi22.v
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi221.v
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi222.v
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi31.v
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi311.v
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi32.v
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi33.v
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_buf.v
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkand2.v
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkbuf.v
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkicgand.v
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkicgor.v
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkinv.v
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkmux2.v
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkmux4.v
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clknand2.v
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clknor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkor4.v
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkxor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_csa32.v
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_csa42.v
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_decap.v
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_delay.v
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffnq.v
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffq.v
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffqn.v
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffrq.v
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffrqn.v
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffsq.v
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffsqn.v
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux2.v
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux3.v
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux4.v
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux5.v
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux6.v
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux7.v
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux8.v
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_drsync.v
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dsync.v
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_footer.v
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_header.v
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_iddr.v
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_inv.v
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_isohi.v
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_isolo.v
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_keeper.v
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_latnq.v
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_latq.v
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_mux2.v
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_mux3.v
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_mux4.v
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_muxi2.v
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_muxi3.v
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_muxi4.v
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nand2.v
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nand3.v
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nand4.v
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nor3.v
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nor4.v
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa21.v
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa211.v
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa22.v
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa221.v
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa222.v
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa31.v
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa311.v
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa32.v
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa33.v
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai21.v
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai22.v
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai221.v
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai222.v
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai31.v
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai311.v
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai32.v
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai33.v
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oddr.v
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_or2.v
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_or3.v
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_or4.v
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_pwrbuf.v
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_rsync.v
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffq.v
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffqn.v
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffrq.v
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffrqn.v
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffsq.v
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffsqn.v
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_tbuf.v
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_tiehi.v
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_tielo.v
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xnor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xnor3.v
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xnor4.v
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xor3.v
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xor4.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/lambdalib/syslib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.151475 lambdalib-0.2.0/lambdalib/syslib/rtl/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_eth.v
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_gpio.v
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_i2c.v
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_jtag.v
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_qspi.v
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_sd.v
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_spi.v
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_uart.v
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/syslib/rtl/la_usb.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.123475 lambdalib-0.2.0/lambdalib/vectorlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.155475 lambdalib-0.2.0/lambdalib/vectorlib/rtl/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vbuf.v
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vinv.v
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_visohi.v
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_visolo.v
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux.v
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux2.v
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux3.v
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux4.v
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux5.v
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux6.v
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux7.v
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-04 16:32:03.000000 lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux8.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.155475 lambdalib-0.2.0/lambdalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-04 16:32:21.000000 lambdalib-0.2.0/lambdalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-03-04 16:32:21.000000 lambdalib-0.2.0/lambdalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 16:32:21.000000 lambdalib-0.2.0/lambdalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-04 16:32:21.000000 lambdalib-0.2.0/lambdalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 16:32:21.000000 lambdalib-0.2.0/lambdalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-04 16:32:03.000000 lambdalib-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 16:32:21.155475 lambdalib-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 16:32:21.155475 lambdalib-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-04 16:32:03.000000 lambdalib-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-04 16:32:03.000000 lambdalib-0.2.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-04 16:32:03.000000 lambdalib-0.2.0/tests/test_local_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-04 16:32:03.000000 lambdalib-0.2.0/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-04 16:32:03.000000 lambdalib-0.2.0/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.161861 lambdalib-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/.github/workflows/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      675 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.github/workflows/bin/format_verilog.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.github/workflows/ci.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/.github/workflows/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.github/workflows/config/verible.rules
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 18:25:05.000000 lambdalib-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-19 18:25:05.000000 lambdalib-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-19 18:25:09.161861 lambdalib-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-19 18:25:05.000000 lambdalib-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 18:25:05.000000 lambdalib-0.2.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 18:25:05.000000 lambdalib-0.2.1/docs/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.133861 lambdalib-0.2.1/lambdalib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.129861 lambdalib-0.2.1/lambdalib/iolib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.137861 lambdalib-0.2.1/lambdalib/iolib/rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioanalog.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iobidir.v
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioclamp.v
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iocorner.v
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iocut.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioinput.v
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iopoc.v
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioshort.v
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovdd.v
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovdda.v
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovddio.v
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovss.v
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovssa.v
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovssio.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioxtal.v
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/iolib/rtl/la_pt.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.129861 lambdalib-0.2.1/lambdalib/padring/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.137861 lambdalib-0.2.1/lambdalib/padring/rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/padring/rtl/la_iopadring.v
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/padring/rtl/la_iopadring.vh
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/padring/rtl/la_ioside.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.137861 lambdalib-0.2.1/lambdalib/padring/testbench/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/padring/testbench/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/padring/testbench/tb_la_iopadring.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.129861 lambdalib-0.2.1/lambdalib/ramlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.137861 lambdalib-0.2.1/lambdalib/ramlib/rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/ramlib/rtl/la_asyncfifo.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/ramlib/rtl/la_dpram.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/ramlib/rtl/la_spram.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/ramlib/rtl/la_spregfile.v
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/ramlib/rtl/la_syncfifo.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.129861 lambdalib-0.2.1/lambdalib/stdlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.157861 lambdalib-0.2.1/lambdalib/stdlib/rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_and2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_and3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_and4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_antenna.v
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao211.v
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao22.v
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao221.v
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao222.v
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao31.v
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao311.v
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao32.v
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao33.v
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi211.v
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi22.v
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi221.v
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi222.v
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi31.v
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi311.v
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi32.v
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi33.v
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_buf.v
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkand2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkbuf.v
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkicgand.v
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkicgor.v
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkinv.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkmux2.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkmux4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clknand2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clknor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkor4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkxor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_csa32.v
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_csa42.v
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_decap.v
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_delay.v
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffnq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffqn.v
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffrq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffrqn.v
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffsq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffsqn.v
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux5.v
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux6.v
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux7.v
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux8.v
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_drsync.v
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dsync.v
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_footer.v
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_header.v
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_iddr.v
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_inv.v
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_isohi.v
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_isolo.v
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_keeper.v
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_latnq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_latq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_mux2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_mux3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_mux4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_muxi2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_muxi3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_muxi4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nand2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nand3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nand4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nor3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nor4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa211.v
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa22.v
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa221.v
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa222.v
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa31.v
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa311.v
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa32.v
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa33.v
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai22.v
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai221.v
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai222.v
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai31.v
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai311.v
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai32.v
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai33.v
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oddr.v
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_or2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_or3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_or4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_pwrbuf.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_rsync.v
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffqn.v
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffrq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffrqn.v
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffsq.v
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffsqn.v
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_tbuf.v
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_tiehi.v
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_tielo.v
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xnor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xnor3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xnor4.v
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xor3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xor4.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.129861 lambdalib-0.2.1/lambdalib/syslib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.157861 lambdalib-0.2.1/lambdalib/syslib/rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_eth.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_gpio.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_i2c.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_jtag.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_qspi.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_sd.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_spi.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_uart.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/syslib/rtl/la_usb.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.157861 lambdalib-0.2.1/lambdalib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.157861 lambdalib-0.2.1/lambdalib/utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/utils/templates/la_spmemory.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.129861 lambdalib-0.2.1/lambdalib/vectorlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.161861 lambdalib-0.2.1/lambdalib/vectorlib/rtl/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vbuf.v
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vinv.v
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_visohi.v
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_visolo.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux.v
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux3.v
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux4.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux5.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux6.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux7.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-19 18:25:05.000000 lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux8.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.161861 lambdalib-0.2.1/lambdalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-19 18:25:09.000000 lambdalib-0.2.1/lambdalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-19 18:25:09.000000 lambdalib-0.2.1/lambdalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:25:09.000000 lambdalib-0.2.1/lambdalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 18:25:09.000000 lambdalib-0.2.1/lambdalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 18:25:09.000000 lambdalib-0.2.1/lambdalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 18:25:05.000000 lambdalib-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:25:09.161861 lambdalib-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:25:09.161861 lambdalib-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 18:25:05.000000 lambdalib-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 18:25:05.000000 lambdalib-0.2.1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 18:25:05.000000 lambdalib-0.2.1/tests/test_local_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 18:25:05.000000 lambdalib-0.2.1/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-19 18:25:05.000000 lambdalib-0.2.1/tests/test_setup.py
```

### Comparing `lambdalib-0.2.0/.github/workflows/bin/format_verilog.sh` & `lambdalib-0.2.1/.github/workflows/bin/format_verilog.sh`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # sources.
 # tests/flows/data/bad.v is ours, but intentionally contains invalid syntax
 find . \( \
     -name "*.v" \
     -or -name "*.vh" \
 \)  -not \( \
     -path "./siliconcompiler/*" \
+    -or -path "./lambdalib/utils/templates/*" \
 \) >> $FILES
 
 verible-verilog-format \
     --failsafe_success=false \
     --indentation_spaces 4 \
     --inplace `cat $FILES`
```

### Comparing `lambdalib-0.2.0/.github/workflows/ci.yml` & `lambdalib-0.2.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         uses: actions/checkout@v4
         with:
           repository: siliconcompiler/siliconcompiler
           path: siliconcompiler
 
       - name: Set up Verible
         run: |
-          ./siliconcompiler/setup/install-verible.sh
+          ./siliconcompiler/setup/ubuntu22/install-verible.sh
           echo /opt/verible/bin >> $GITHUB_PATH
 
       - name: Check format
         id: check-format
         run: |
           ./.github/workflows/bin/format_verilog.sh > files.txt
           cat files.txt
```

### Comparing `lambdalib-0.2.0/.github/workflows/config/verible.rules` & `lambdalib-0.2.1/.github/workflows/config/verible.rules`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/.github/workflows/wheels.yml` & `lambdalib-0.2.1/.github/workflows/wheels.yml`

 * *Files 11% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     steps:
     - uses: actions/download-artifact@v4
       with:
         name: Packages
         path: dist
 
     - name: Publish
-      uses: pypa/gh-action-pypi-publish@v1.8.11
+      uses: pypa/gh-action-pypi-publish@v1.8.14
 
   save:
     needs: [publish]
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/download-artifact@v4
       with:
         name: Packages
         path: dist
 
     - name: Add wheels to GitHub release artifacts
-      uses: softprops/action-gh-release@v1
+      uses: softprops/action-gh-release@v2
       with:
         files: dist/*.whl
```

### Comparing `lambdalib-0.2.0/LICENSE` & `lambdalib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/PKG-INFO` & `lambdalib-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdalib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Standardized ASIC design libraries
 Author: Zero ASIC
 License: MIT License
         
         Copyright (c) 2023 Zero ASIC Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -13,14 +13,15 @@
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/siliconcompiler/lambdalib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: siliconcompiler>=0.20.2
+Requires-Dist: Jinja2>=3.1.3
 Provides-Extra: dev
 Requires-Dist: flake8>=5.0.0; extra == "dev"
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: pytest-timeout>=2.1.0; extra == "dev"
 
 # Lambdalib Introduction
```

### Comparing `lambdalib-0.2.0/README.md` & `lambdalib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/__init__.py` & `lambdalib-0.2.1/lambdalib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from siliconcompiler import Chip, Library
 import siliconcompiler.package as sc_package
 import glob
 import os
 import shutil
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 _libraries = (
     'iolib',
     'stdlib',
     'ramlib',
     'padring',
     'syslib',
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioanalog.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioanalog.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO analog pass-through cell
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * aio[0] = pass through from pad (with esd clamp)
  * aio[1] = small series resistance
  * aio[2] = big series resistance
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iobidir.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iobidir.v`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO bi-directional buffer
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a generic cell that defines the standard interface of the lambda
  * bidrectional buffer cell. It is only suitable for FPGA synthesis.
  *
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioclamp.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioclamp.v`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO ESD clamp cell
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
 module la_ioclamp #(
     parameter TYPE  = "DEFAULT",  // cell type
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iocorner.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iocorner.v`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO corner cell
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iocorner #(
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iocut.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovssa.v`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 /*****************************************************************************
- * Function: IO cut cell
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Function: IO supply cell (vssa)
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
-module la_iocut #(
+module la_iovssa #(
     parameter TYPE  = "DEFAULT",  // cell type
     parameter SIDE  = "NO",       // "NO", "SO", "EA", "WE"
     parameter RINGW = 8           // width of io ring
 ) (
-    // ground never cut
-    inout vss
+    inout             vdd,    // core supply
+    inout             vss,    // core ground
+    inout             vddio,  // io supply
+    inout             vssio,  // io ground
+    inout [RINGW-1:0] ioring  // generic io-ring interface
 );
 
 endmodule
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioinput.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioinput.v`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO bi-directional buffer
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a generic cell that defines the standard interface of the lambda
  * bidrectional buffer cell. It is only suitable for FPGA synthesis.
  *
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iopoc.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iopoc.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO power-on-control cell
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iopoc #(
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_ioshort.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioshort.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovdd.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovdd.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO supply cell (vdd)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iovdd #(
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovdda.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovdda.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO supply cell (vdda)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iovdda #(
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovddio.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovddio.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO supply cell (vddio)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iovddio #(
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovss.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovss.v`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO supply cell (vss)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iovss #(
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovssa.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_ioxtal.v`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 /*****************************************************************************
- * Function: IO supply cell (vssa)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Function: IO xtal oscillator cell
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
- *
  ****************************************************************************/
-module la_iovssa #(
+module la_ioxtal #(
     parameter TYPE  = "DEFAULT",  // cell type
     parameter SIDE  = "NO",       // "NO", "SO", "EA", "WE"
+    parameter CFGW  = 16,         // width of core config bus
     parameter RINGW = 8           // width of io ring
-) (
-    inout             vdd,    // core supply
-    inout             vss,    // core ground
-    inout             vddio,  // io supply
-    inout             vssio,  // io ground
-    inout [RINGW-1:0] ioring  // generic io-ring interface
+) (  // io pad signals
+    inout              padi,    // xtal input pad
+    inout              pado,    // xtal output pad
+    inout              vdd,     // core supply
+    inout              vss,     // core ground
+    inout              vddio,   // io supply
+    inout              vssio,   // io ground
+    inout  [RINGW-1:0] ioring,  // generic io-ring interface
+    input  [ CFGW-1:0] cfg,     // generic config interface
+    // core interface
+    output             z        // clock output to core
 );
 
 endmodule
```

### Comparing `lambdalib-0.2.0/lambdalib/iolib/rtl/la_iovssio.v` & `lambdalib-0.2.1/lambdalib/iolib/rtl/la_iovssio.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO supply cell (vssio)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  *
  ****************************************************************************/
 module la_iovssio #(
```

### Comparing `lambdalib-0.2.0/lambdalib/padring/rtl/la_iopadring.v` & `lambdalib-0.2.1/lambdalib/padring/rtl/la_iopadring.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Padring Generator
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * - Cround (vss) is continuous around the while chip.
  *
  * - Default is for ioring to be cut at corners, user must short rings
```

### Comparing `lambdalib-0.2.0/lambdalib/padring/rtl/la_iopadring.vh` & `lambdalib-0.2.1/lambdalib/padring/rtl/la_iopadring.vh`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Padframe Bitfield Definitions
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  ****************************************************************************/
 
 localparam LA_BIDIR = 8'h00;
 localparam LA_INPUT = 8'h01;
 localparam LA_ANALOG = 8'h02;
 localparam LA_XTAL = 8'h03;
```

### Comparing `lambdalib-0.2.0/lambdalib/padring/rtl/la_ioside.v` & `lambdalib-0.2.1/lambdalib/padring/rtl/la_ioside.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: IO padring side
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Doc:
  *
  * See repo ./README.md and ./la_iopadring.v
  *
  ****************************************************************************/
```

### Comparing `lambdalib-0.2.0/lambdalib/padring/testbench/tb_la_iopadring.v` & `lambdalib-0.2.1/lambdalib/padring/testbench/tb_la_iopadring.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/ramlib/rtl/la_asyncfifo.v` & `lambdalib-0.2.1/lambdalib/ramlib/rtl/la_asyncfifo.v`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Dual Clock Asynchronous FIFO
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a wrapper for selecting from a set of hardened memory macros.
  *
  * A synthesizable reference model is used when the TYPE is DEFAULT. The
```

### Comparing `lambdalib-0.2.0/lambdalib/ramlib/rtl/la_dpram.v` & `lambdalib-0.2.1/lambdalib/ramlib/rtl/la_dpram.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Dual Port RAM (One write port + One read port)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a wrapper for selecting from a set of hardened memory macros.
  *
  * A synthesizable reference model is used when the TYPE is DEFAULT. The
```

### Comparing `lambdalib-0.2.0/lambdalib/ramlib/rtl/la_spram.v` & `lambdalib-0.2.1/lambdalib/ramlib/rtl/la_spram.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Single Port RAM
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a wrapper for selecting from a set of hardened memory macros.
  *
  * A synthesizable reference model is used when the TYPE is DEFAULT. The
```

### Comparing `lambdalib-0.2.0/lambdalib/ramlib/rtl/la_spregfile.v` & `lambdalib-0.2.1/lambdalib/ramlib/rtl/la_spregfile.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Single Port Register File
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a wrapper for selecting from a set of hardened register file macros.
  *
  * A synthesizable reference model is used when the TYPE is DEFAULT. The
```

### Comparing `lambdalib-0.2.0/lambdalib/ramlib/rtl/la_syncfifo.v` & `lambdalib-0.2.1/lambdalib/ramlib/rtl/la_syncfifo.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Synchronous FIFO
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * This is a wrapper for selecting from a set of hardened memory macros.
  *
  ****************************************************************************/
```

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_and2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_and2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_and3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_and3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_and4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_and4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao21.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao21.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao211.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao211.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao22.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao22.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao221.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao221.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao222.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao222.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao31.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao31.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao311.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao311.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao32.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao32.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_ao33.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_ao33.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi21.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi21.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi211.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi211.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi22.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi22.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi221.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi221.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi222.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi222.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi31.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi31.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi311.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi311.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi32.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi32.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_aoi33.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_aoi33.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_buf.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_buf.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkand2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkand2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkbuf.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkbuf.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkicgand.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkicgand.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkicgor.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkicgor.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkinv.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkinv.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkmux2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkmux2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkmux4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkmux4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clknand2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clknand2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clknor2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clknor2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkor2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkor2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkor4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkor4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_clkxor2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_clkxor2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_csa32.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_csa32.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_csa42.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_csa42.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_delay.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_delay.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffnq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffnq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffqn.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffqn.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffrq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffrq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffrqn.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffrqn.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffsq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffsq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dffsqn.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dffsqn.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux5.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux5.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux6.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux6.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux7.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux7.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dmux8.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dmux8.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_drsync.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_drsync.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_dsync.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_dsync.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_footer.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_footer.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_header.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_header.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_iddr.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_iddr.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_inv.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_inv.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_isohi.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_isohi.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_isolo.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_isolo.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_latnq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_latnq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_latq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_latq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_mux2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_mux2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_mux3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_mux3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_mux4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_mux4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_muxi2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_muxi2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_muxi3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_muxi3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_muxi4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_muxi4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nand2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nand2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nand3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nand3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nand4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nand4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nor2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nor2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nor3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nor3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_nor4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_nor4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa21.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa21.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa211.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa211.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa22.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa22.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa221.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa221.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa222.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa222.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa31.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa31.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa311.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa311.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa32.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa32.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oa33.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oa33.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai21.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai21.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai22.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai22.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai221.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai221.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai222.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai222.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai31.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai31.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai311.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai311.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai32.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai32.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oai33.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oai33.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_oddr.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_oddr.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_or2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_or2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_or3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_or3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_or4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_or4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_pwrbuf.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_pwrbuf.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_rsync.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_rsync.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffqn.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffqn.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffrq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffrq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffrqn.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffrqn.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffsq.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffsq.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_sdffsqn.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_sdffsqn.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_tbuf.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_tbuf.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xnor2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xnor2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xnor3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xnor3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xnor4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xnor4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xor2.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xor2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xor3.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xor3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/stdlib/rtl/la_xor4.v` & `lambdalib-0.2.1/lambdalib/stdlib/rtl/la_xor4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_eth.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_eth.v`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: Ethernet Interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
 
 module la_eth #(
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_gpio.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_gpio.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: GPIO Interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
 
 module la_gpio #(
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_i2c.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_i2c.v`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: I2C interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * Firmware configurable as host or device.
  *
  ****************************************************************************/
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_jtag.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_jtag.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: JTAG debug interface (device)
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_qspi.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_qspi.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: QSPI Interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  * 1. Statically configurable as host/device by TYPE.
 
  ****************************************************************************/
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_sd.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_sd.v`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: SD/SDIO/MMC Controller
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_spi.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_spi.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: SPI Interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
 
 module la_spi #(
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_uart.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_uart.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: UART interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
 
 module la_uart #(
```

### Comparing `lambdalib-0.2.0/lambdalib/syslib/rtl/la_usb.v` & `lambdalib-0.2.1/lambdalib/syslib/rtl/la_usb.v`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*****************************************************************************
  * Function: USB Interface
- * Copyright: Lambda Project Authors. ALl rights Reserved.
+ * Copyright: Lambda Project Authors. All rights Reserved.
  * License:  MIT (see LICENSE file in Lambda repository)
  *
  * Docs:
  *
  ****************************************************************************/
 module la_usb #(
     parameter TARGET = "DEFAULT",  // technology target
```

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vbuf.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vbuf.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vinv.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vinv.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_visohi.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_visohi.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_visolo.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_visolo.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux2.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux2.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux3.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux3.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux4.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux4.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux5.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux5.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux6.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux6.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux7.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux7.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib/vectorlib/rtl/la_vmux8.v` & `lambdalib-0.2.1/lambdalib/vectorlib/rtl/la_vmux8.v`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/lambdalib.egg-info/PKG-INFO` & `lambdalib-0.2.1/lambdalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdalib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Standardized ASIC design libraries
 Author: Zero ASIC
 License: MIT License
         
         Copyright (c) 2023 Zero ASIC Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -13,14 +13,15 @@
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/siliconcompiler/lambdalib
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: siliconcompiler>=0.20.2
+Requires-Dist: Jinja2>=3.1.3
 Provides-Extra: dev
 Requires-Dist: flake8>=5.0.0; extra == "dev"
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: pytest-timeout>=2.1.0; extra == "dev"
 
 # Lambdalib Introduction
```

### Comparing `lambdalib-0.2.0/lambdalib.egg-info/SOURCES.txt` & `lambdalib-0.2.1/lambdalib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,16 @@
 lambdalib/syslib/rtl/la_i2c.v
 lambdalib/syslib/rtl/la_jtag.v
 lambdalib/syslib/rtl/la_qspi.v
 lambdalib/syslib/rtl/la_sd.v
 lambdalib/syslib/rtl/la_spi.v
 lambdalib/syslib/rtl/la_uart.v
 lambdalib/syslib/rtl/la_usb.v
+lambdalib/utils/__init__.py
+lambdalib/utils/templates/la_spmemory.v
 lambdalib/vectorlib/rtl/la_vbuf.v
 lambdalib/vectorlib/rtl/la_vinv.v
 lambdalib/vectorlib/rtl/la_visohi.v
 lambdalib/vectorlib/rtl/la_visolo.v
 lambdalib/vectorlib/rtl/la_vmux.v
 lambdalib/vectorlib/rtl/la_vmux2.v
 lambdalib/vectorlib/rtl/la_vmux3.v
```

### Comparing `lambdalib-0.2.0/pyproject.toml` & `lambdalib-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 authors = [{name = "Zero ASIC"}]
 description = "Standardized ASIC design libraries"
 readme = "README.md"
 urls = {Homepage = "https://github.com/siliconcompiler/lambdalib"}
 requires-python = ">= 3.8"
 license = {file = "LICENSE"}
 dependencies = [
-    "siliconcompiler >= 0.20.2"
+    "siliconcompiler >= 0.20.2",
+    "Jinja2 >= 3.1.3"
 ]
 dynamic = ['version']
 
 [tool.setuptools.dynamic]
 version = {attr = "lambdalib.__version__"}
 
 [tool.pytest.ini_options]
```

### Comparing `lambdalib-0.2.0/tests/test_generate.py` & `lambdalib-0.2.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `lambdalib-0.2.0/tests/test_setup.py` & `lambdalib-0.2.1/tests/test_setup.py`

 * *Files identical despite different names*

