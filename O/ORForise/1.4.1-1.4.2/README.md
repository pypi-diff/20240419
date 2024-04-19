# Comparing `tmp/ORForise-1.4.1.tar.gz` & `tmp/orforise-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ORForise-1.4.1.tar", last modified: Thu May 25 23:05:55 2023, max compression
+gzip compressed data, was "orforise-1.4.2.tar", last modified: Fri Apr 19 20:05:31 2024, max compression
```

## Comparing `ORForise-1.4.1.tar` & `orforise-1.4.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/
--rw-r--r--   0 nick      (1000) nick      (1000)    32476 2022-12-23 17:30:27.000000 ORForise-1.4.1/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    36436 2023-05-25 23:05:55.897059 ORForise-1.4.1/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    35840 2023-05-25 23:03:14.000000 ORForise-1.4.1/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      112 2023-03-22 17:27:03.000000 ORForise-1.4.1/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1036 2023-05-25 23:05:55.901059 ORForise-1.4.1/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.861058 ORForise-1.4.1/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.877059 ORForise-1.4.1/src/ORForise/
--rw-r--r--   0 nick      (1000) nick      (1000)    10648 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/Aggregate_Compare.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10223 2023-03-23 16:23:21.000000 ORForise-1.4.1/src/ORForise/Annotation_Compare.py
--rw-r--r--   0 nick      (1000) nick      (1000)    44200 2023-05-25 22:49:25.000000 ORForise-1.4.1/src/ORForise/Comparator.py
--rw-r--r--   0 nick      (1000) nick      (1000)    14057 2023-05-25 22:18:26.000000 ORForise-1.4.1/src/ORForise/GFF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9900 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/GFF_Intersector.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/ORForise_Analysis/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2643 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/cds_checker.py
--rw-r--r--   0 nick      (1000) nick      (1000)      939 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/gene_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10085 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/genome_Metrics.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3479 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10890 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9515 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9886 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/result_File_Analysis.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6114 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5431 2023-04-22 15:00:10.000000 ORForise-1.4.1/src/ORForise/StORForise.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/Augustus/
--rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-12-23 17:30:27.000000 ORForise-1.4.1/src/ORForise/Tools/Augustus/Augustus.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/Augustus/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/Balrog/
--rw-r--r--   0 nick      (1000) nick      (1000)     1387 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/Balrog/Balrog.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/Balrog/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/EasyGene/
--rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/EasyGene/EasyGene.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/EasyGene/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/FGENESB/
--rw-r--r--   0 nick      (1000) nick      (1000)     1480 2022-12-23 17:30:29.000000 ORForise-1.4.1/src/ORForise/Tools/FGENESB/FGENESB.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/FGENESB/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/
--rw-r--r--   0 nick      (1000) nick      (1000)     1376 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/FragGeneScan.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GFF/
--rw-r--r--   0 nick      (1000) nick      (1000)     1894 2023-05-25 22:21:03.000000 ORForise-1.4.1/src/ORForise/Tools/GFF/GFF.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GFF/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/
--rw-r--r--   0 nick      (1000) nick      (1000)     1723 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark/
--rw-r--r--   0 nick      (1000) nick      (1000)     5374 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark/GeneMark.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/
--rw-r--r--   0 nick      (1000) nick      (1000)     1346 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/
--rw-r--r--   0 nick      (1000) nick      (1000)     1359 2022-12-23 17:30:30.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/
--rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/GeneMark_S.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/
--rw-r--r--   0 nick      (1000) nick      (1000)     1468 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.893059 ORForise-1.4.1/src/ORForise/Tools/MetaGene/
--rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGene/MetaGene.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGene/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/
--rw-r--r--   0 nick      (1000) nick      (1000)     1469 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/
--rw-r--r--   0 nick      (1000) nick      (1000)     1452 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/Prodigal/
--rw-r--r--   0 nick      (1000) nick      (1000)     1427 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/Prodigal/Prodigal.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/Prodigal/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/Prokka/
--rw-r--r--   0 nick      (1000) nick      (1000)     1537 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/Prokka/Prokka.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-22 17:27:07.000000 ORForise-1.4.1/src/ORForise/Tools/Prokka/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)     1609 2023-04-22 15:00:10.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:31.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/
--rw-r--r--   0 nick      (1000) nick      (1000)     1860 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1318 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1863 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.897059 ORForise-1.4.1/src/ORForise/Tools/TransDecoder/
--rw-r--r--   0 nick      (1000) nick      (1000)     1384 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/TransDecoder/TransDecoder.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/TransDecoder/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/Tools/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:30:32.000000 ORForise-1.4.1/src/ORForise/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1099 2023-05-25 23:03:14.000000 ORForise-1.4.1/src/ORForise/utils.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-25 23:05:55.877059 ORForise-1.4.1/src/ORForise.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)    36436 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     3007 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)      246 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        6 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/requires.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        9 2023-05-25 23:05:55.000000 ORForise-1.4.1/src/ORForise.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/
+-rw-r--r--   0 nick      (1000) nick      (1000)    32476 2022-12-19 15:31:48.000000 orforise-1.4.2/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)    36457 2024-04-19 20:05:31.597392 orforise-1.4.2/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    35840 2024-04-19 20:04:22.000000 orforise-1.4.2/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      112 2022-12-19 15:31:48.000000 orforise-1.4.2/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1036 2024-04-19 20:05:31.597392 orforise-1.4.2/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.589393 orforise-1.4.2/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.589393 orforise-1.4.2/src/ORForise/
+-rw-r--r--   0 nick      (1000) nick      (1000)    10648 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/Aggregate_Compare.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10228 2024-04-19 18:32:40.000000 orforise-1.4.2/src/ORForise/Annotation_Compare.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    45041 2024-04-19 19:29:11.000000 orforise-1.4.2/src/ORForise/Comparator.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    14057 2023-05-26 15:57:44.000000 orforise-1.4.2/src/ORForise/GFF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9900 2023-03-27 18:58:48.000000 orforise-1.4.2/src/ORForise/GFF_Intersector.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/ORForise_Analysis/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2643 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/cds_checker.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      939 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/gene_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10085 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/genome_Metrics.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3479 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10890 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9515 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9886 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/result_File_Analysis.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6114 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5431 2023-03-28 19:57:59.000000 orforise-1.4.2/src/ORForise/StORForise.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/Augustus/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-12-19 15:31:48.000000 orforise-1.4.2/src/ORForise/Tools/Augustus/Augustus.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/Augustus/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/Balrog/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1387 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/Balrog/Balrog.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/Balrog/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/EasyGene/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1323 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/EasyGene/EasyGene.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/EasyGene/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/FGENESB/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1480 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/FGENESB/FGENESB.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/FGENESB/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/FragGeneScan/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1376 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/FragGeneScan/FragGeneScan.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/FragGeneScan/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/GFF/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2806 2024-04-19 19:29:50.000000 orforise-1.4.2/src/ORForise/Tools/GFF/GFF.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:49.000000 orforise-1.4.2/src/ORForise/Tools/GFF/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/GLIMMER_3/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1723 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GLIMMER_3/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/GeneMark/
+-rw-r--r--   0 nick      (1000) nick      (1000)     5374 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark/GeneMark.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/GeneMark_HA/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1346 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_HA/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.593392 orforise-1.4.2/src/ORForise/Tools/GeneMark_HMM/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1359 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_HMM/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/GeneMark_S/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_S/GeneMark_S.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_S/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/GeneMark_S_2/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1468 2023-03-27 18:58:48.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/GeneMark_S_2/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/MetaGene/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1334 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/MetaGene/MetaGene.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/MetaGene/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/MetaGeneAnnotator/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1469 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:50.000000 orforise-1.4.2/src/ORForise/Tools/MetaGeneAnnotator/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/MetaGeneMark/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1452 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/MetaGeneMark/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/Prodigal/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1427 2023-03-27 18:58:48.000000 orforise-1.4.2/src/ORForise/Tools/Prodigal/Prodigal.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/Prodigal/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/Prokka/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1537 2023-03-27 18:58:48.000000 orforise-1.4.2/src/ORForise/Tools/Prokka/Prokka.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-03-27 18:58:48.000000 orforise-1.4.2/src/ORForise/Tools/Prokka/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1609 2023-03-31 18:24:22.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1860 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1318 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1863 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise/Tools/TransDecoder/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1384 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/TransDecoder/TransDecoder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/TransDecoder/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/Tools/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:51.000000 orforise-1.4.2/src/ORForise/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1099 2024-04-19 20:04:22.000000 orforise-1.4.2/src/ORForise/utils.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-19 20:05:31.597392 orforise-1.4.2/src/ORForise.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)    36457 2024-04-19 20:05:31.000000 orforise-1.4.2/src/ORForise.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)     3007 2024-04-19 20:05:31.000000 orforise-1.4.2/src/ORForise.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-04-19 20:05:31.000000 orforise-1.4.2/src/ORForise.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)      246 2024-04-19 20:05:31.000000 orforise-1.4.2/src/ORForise.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        6 2024-04-19 20:05:31.000000 orforise-1.4.2/src/ORForise.egg-info/requires.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        9 2024-04-19 20:05:31.000000 orforise-1.4.2/src/ORForise.egg-info/top_level.txt
```

### Comparing `ORForise-1.4.1/LICENSE` & `orforise-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/PKG-INFO` & `orforise-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ORForise
-Version: 1.4.1
+Version: 1.4.2
 Summary: ORForise - Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions.
 Home-page: https://github.com/NickJD/ORForise
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/ORForise/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # ORForise - Prokaryote Genome Annotation Analysis and Comparison Platform
 ## Published in Bioinformatics :   https://academic.oup.com/bioinformatics/article/38/5/1198/6454948
 ### Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions. 
 ### Novel genome annotations can be compared to a provided reference annotation from Ensembl and predictions from other tools (or any given GFF annotation) .
 
 # Requirements and Installation:
@@ -57,15 +58,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Annotation_Compare.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -t TOOL -tp TOOL_PREDICTION
                              [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.1: Annotatione-Compare Run Parameters.
+ORForise v1.4.2: Annotatione-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -t TOOL               Which tool to analyse? (Prodigal)
   -tp TOOL_PREDICTION   Tool genome prediction file (.gff) - Different Tool Parameters are compared individually via
@@ -107,15 +108,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Aggregate_Compare.py [-h] -dna GENOME_DNA -t TOOLS -tp TOOL_PREDICTIONS -ref REFERENCE_ANNOTATION
                             [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.1: Aggregate-Compare Run Parameters.
+ORForise v1.4.2: Aggregate-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -t TOOLS              Which tools to analyse? (Prodigal,GeneMarkS)
   -tp TOOL_PREDICTIONS  Tool genome prediction file (.gff) - Providefile locations for each tool comma separated
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
@@ -261,15 +262,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Adder.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add ADDITIONAL_ANNOTATION -o
                     OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-gene_ident GENE_IDENT] [-olap OVERLAP]
 
-ORForise v1.4.1: GFF-Adder Run Parameters.
+ORForise v1.4.2: GFF-Adder Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
@@ -323,15 +324,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Intersector.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add
                           ADDITIONAL_ANNOTATION -o OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-cov COVERAGE]
 
-ORForise v1.4.1: GFF-Intersector Run Parameters.
+ORForise v1.4.2: GFF-Intersector Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
```

### Comparing `ORForise-1.4.1/README.md` & `orforise-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Annotation_Compare.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -t TOOL -tp TOOL_PREDICTION
                              [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.1: Annotatione-Compare Run Parameters.
+ORForise v1.4.2: Annotatione-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -t TOOL               Which tool to analyse? (Prodigal)
   -tp TOOL_PREDICTION   Tool genome prediction file (.gff) - Different Tool Parameters are compared individually via
@@ -92,15 +92,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Aggregate_Compare.py [-h] -dna GENOME_DNA -t TOOLS -tp TOOL_PREDICTIONS -ref REFERENCE_ANNOTATION
                             [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.1: Aggregate-Compare Run Parameters.
+ORForise v1.4.2: Aggregate-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -t TOOLS              Which tools to analyse? (Prodigal,GeneMarkS)
   -tp TOOL_PREDICTIONS  Tool genome prediction file (.gff) - Providefile locations for each tool comma separated
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
@@ -246,15 +246,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Adder.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add ADDITIONAL_ANNOTATION -o
                     OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-gene_ident GENE_IDENT] [-olap OVERLAP]
 
-ORForise v1.4.1: GFF-Adder Run Parameters.
+ORForise v1.4.2: GFF-Adder Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
@@ -308,15 +308,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Intersector.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add
                           ADDITIONAL_ANNOTATION -o OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-cov COVERAGE]
 
-ORForise v1.4.1: GFF-Intersector Run Parameters.
+ORForise v1.4.2: GFF-Intersector Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
```

### Comparing `ORForise-1.4.1/setup.cfg` & `orforise-1.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ORForise
-version = 1.4.1
+version = 1.4.2
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = ORForise - Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/ORForise
 project_urls =
```

### Comparing `ORForise-1.4.1/src/ORForise/Aggregate_Compare.py` & `orforise-1.4.2/src/ORForise/Aggregate_Compare.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Annotation_Compare.py` & `orforise-1.4.2/src/ORForise/Annotation_Compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,19 @@
     ############################################# To get default output filename from input file details
     genome_name = options.reference_annotation.split('/')[-1].split('.')[0]
     metric_description = list(all_Metrics.keys())
     metrics = list(all_Metrics.values())
     rep_metric_description = list(all_rep_Metrics.keys())
     rep_metrics = list(all_rep_Metrics.values())
     ############## Printing to std-out and optional csv file
-    print('Genome Used: ' + str(options.reference_annotation.split('/')[-1]))
+    print('Genome Used: ' + str(options.genome_DNA.split('/')[-1]))
     if options.reference_tool:
         print('Reference Tool Used: '+str(options.reference_tool))
     else:
-        print('Reference Used: ' + str(options.reference_annotation))
+        print('Reference Used: ' + str(options.reference_annotation.split('/')[-1]))
     print('Tool Compared: '+str(options.tool))
     print('Perfect Matches: ' + str(len(perfect_Matches)) + ' [' + str(len(ref_genes))+ '] - '+ format(100 * len(perfect_Matches)/len(ref_genes),'.2f')+'%')
     print('Partial Matches: ' + str(len(partial_Hits)) + ' [' + str(len(ref_genes))+ '] - '+ format(100 * len(partial_Hits)/len(ref_genes),'.2f')+'%')
     print('Missed Genes: ' + str(len(missed_genes)) + ' [' + str(len(ref_genes))+ '] - '+ format(100 * len(missed_genes)/len(ref_genes),'.2f')+'%')
     if options.outname:
         with open(options.outname, 'w', newline='\n', encoding='utf-8') as out_file:  # Clear write out of report
             tool_out = csv.writer(out_file, quoting=csv.QUOTE_NONE, escapechar=" ")
```

### Comparing `ORForise-1.4.1/src/ORForise/Comparator.py` & `orforise-1.4.2/src/ORForise/Comparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,38 @@
 #             to_return = to_return[0]+'_'+to_return[1]+'_'+to_return[2]
 #             return to_return
 #     else:
 #         print ('Key not found')
 
 def is_double_range(range1, range2):
     return len(range1) >= 2 * len(range2)
-def nuc_Count(start, stop, strand):  # Gets correct seq then returns GC
-    if strand == '-':
-        r_Start = comp.genome_Size - stop
-        r_Stop = comp.genome_Size - start
-        seq = (comp.genome_Seq_Rev[r_Start:r_Stop + 1])
-    elif strand == '+':
-        seq = (comp.genome_Seq[start - 1:stop])
+def nuc_Count(verbose, start, stop, strand):  # Gets correct seq then returns GC
+    if stop >= comp.genome_Size:
+        if verbose == True:
+            print("There is a wrap around gene and I am dealing with it the best I can - Start: " + str(start) + " Stop: " + str(stop))
+        extra_stop = stop - comp.genome_Size
+        stop = comp.genome_Size
+        if strand == '-':
+            r_Start = comp.genome_Size - stop
+            r_Stop = comp.genome_Size - start
+            seq = (comp.genome_Seq_Rev[r_Start:r_Stop + 1])
+            extra_seq = (comp.genome_Seq_Rev[-extra_stop-1:])
+            seq = extra_seq+seq
+        elif strand == '+':
+            seq = comp.genome_Seq[start - 1:stop]
+            extra_seq = comp.genome_Seq[:extra_stop +1]
+            seq = seq+extra_seq
+            #seq = (comp.genome_Seq[start - 1:stop])
+    else:
+        if strand == '-':
+            r_Start = comp.genome_Size - stop
+            r_Stop = comp.genome_Size - start
+            seq = (comp.genome_Seq_Rev[r_Start:r_Stop + 1])
+        elif strand == '+':
+            seq = (comp.genome_Seq[start - 1:stop])
     c = 0
     a = 0
     g = 0
     t = 0
     n = 0
     for i in seq:
         if "C" in i:
@@ -319,16 +336,16 @@
                 previously_Covered_Gene = comp.matched_ORFs[g_pos][-1]
                 comp.multi_Matched_ORFs[g_pos] += [g_pos.replace(',', '-'), previously_Covered_Gene.replace(',',
                                                                                                             '-')]  # ORF is same as gene so can use g_pos
             comp.matched_ORFs.update({g_pos: m_ORF_Details})
             comp.genes_Detected.update({str(gene_details): g_pos})
             match_Statistics(o_Start, o_Stop, g_Start, g_Stop, g_Strand)
             perfect_Matched_Genes(g_Start, g_Stop, g_Strand)
-            if verbose == True:
-                print('Perfect Match')
+            #if verbose == True:
+            #    print('Perfect Match')
         elif perfect_Match == False and len(
                 overlapping_ORFs) == 1:  # If we do not have a perfect match but 1 ORF which has passed the filtering
             orf_Pos = list(overlapping_ORFs.keys())[0]
             o_Start = int(orf_Pos.split(',')[0])
             o_Stop = int(orf_Pos.split(',')[1])
             orf_Details = overlapping_ORFs[orf_Pos]
             m_ORF_Details = orf_Details[:]
@@ -340,16 +357,16 @@
                     last_key = [*comp.matched_ORFs.keys()][-1]
                     previously_Covered_Gene = comp.matched_ORFs[last_key][-1]
                 comp.multi_Matched_ORFs[orf_Pos] += [g_pos.replace(',', '-'), previously_Covered_Gene.replace(',',
                                                                                                    '-')]  # ORF collects multiple gene pos'
             comp.matched_ORFs.update({orf_Pos: m_ORF_Details})
             comp.genes_Detected.update({str(gene_details): orf_Pos})
             match_Statistics(o_Start, o_Stop, g_Start, g_Stop, g_Strand)
-            if verbose == True:
-                print('Partial Match')
+            #if verbose == True:
+            #    print('Partial Match')
             partial_Hit_Calc(g_Start, g_Stop, g_Strand, o_Start, o_Stop)
         elif perfect_Match == False and len(
                 overlapping_ORFs) >= 1:  # If we have more than 1 potential ORF match, we check to see which is the 'best' hit
             orf_Pos, orf_Details = candidate_ORF_Selection(gene_Set, overlapping_ORFs)  # Return best match
             o_Start = int(orf_Pos.split(',')[0])
             o_Stop = int(orf_Pos.split(',')[1])
             m_ORF_Details = orf_Details[:]
@@ -370,16 +387,16 @@
             partial_Hit_Calc(g_Start, g_Stop, g_Strand, o_Start, o_Stop)
         elif out_Frame:  # Keep record of ORFs which overlap a gene but in the wrong frame
             if verbose == True:
                 print("Out of Frame Predicted CDS")
             genes_Unmatched(g_Start, g_Stop, g_Strand)  #
         else:
             genes_Unmatched(g_Start, g_Stop, g_Strand)  # No hit
-            if verbose == True:
-                print("No Hit")
+            #if verbose == True:
+            #    print("No Hit")
     for orf_Key in comp.matched_ORFs:  # Remove ORFs from out of frame if ORF was correctly matched to another Gene
         if orf_Key in comp.out_Of_Frame_ORFs:
             del comp.out_Of_Frame_ORFs[orf_Key]
     ######################################## ORF Lengths and Precision
     start_Difference = [x for x in comp.start_Difference if x != 0]  # Remove 0s (Perfect hits)
     stop_Difference = [x for x in comp.stop_Difference if x != 0]
     if len(start_Difference) >= 1:
@@ -405,15 +422,15 @@
         g_Start = int(gene_details[0])
         g_Stop = int(gene_details[1])
         g_Strand = gene_details[2]
         gene_Length = (g_Stop - g_Start) +1
         if gene_Length == 0: print(g_Start, g_Stop, "!!!!!!!!!!!!!!!!!!!!!!!!")
         comp.gene_Lengths.append(gene_Length)
         gene_Nuc_Array[g_Start - 1:g_Stop] = True  # Changing all between the two positions to 1's
-        comp.gene_GC.append(nuc_Count(g_Start, g_Stop, g_Strand))
+        comp.gene_GC.append(nuc_Count(verbose, g_Start, g_Stop, g_Strand))
         if gene_Length <= SHORT_ORF_LENGTH:  # .utils
             comp.gene_Short.append(gene_Length)
         ### Calculate overlapping Genes -
         if prev_Gene_Stop > g_Start:
             if '+' in g_Strand:
                 comp.gene_Pos_Olap.append(prev_Gene_Stop - g_Start)
             elif '-' in g_Strand:
@@ -449,15 +466,15 @@
         if o_Strand == "+":  # Get number of Positive and Negative strand ORFs
             comp.pos_Strand += 1
         elif o_Strand == "-":
             comp.neg_Strand += 1
         orf_Length = (o_Stop - o_Start) +1
         comp.orf_Lengths.append(orf_Length)
         orf_Nuc_Array[o_Start - 1:o_Stop] = True  # Changing all between the two positions to 1's
-        comp.orf_GC.append(nuc_Count(o_Start, o_Stop, o_Strand))
+        comp.orf_GC.append(nuc_Count(verbose, o_Start, o_Stop, o_Strand))
         if orf_Length <= SHORT_ORF_LENGTH:  # .utils
             comp.orf_Short.append(orf_Length)
         ### Calculate overlapping ORFs -
         if prev_ORF_Stop > o_Start:
             if '+' in o_Strand:
                 comp.orf_Pos_Olap.append(prev_ORF_Stop - o_Start)
             elif '-' in o_Strand:
@@ -483,15 +500,15 @@
     for mo_Positions, m_ORF_Details in comp.matched_ORFs.items():
         mo_Start = int(mo_Positions.split(',')[0])
         mo_Stop = int(mo_Positions.split(',')[1])
         mo_Strand = m_ORF_Details[0]
         mo_Length = (mo_Stop - mo_Start)
         matched_ORF_Nuc_Array[mo_Start - 1:mo_Stop] = True  # This is the complete matched orf not the matched orf bits
 
-        comp.m_ORF_GC.append(nuc_Count(mo_Start, mo_Stop, mo_Strand))
+        comp.m_ORF_GC.append(nuc_Count(verbose, mo_Start, mo_Stop, mo_Strand))
         if mo_Length <= SHORT_ORF_LENGTH:  # .utils
             comp.m_ORF_Short.append(mo_Length)
         ### Calculate overlapping Matched ORFs -
         if matched_Prev_ORF_Stop > mo_Start:
             if '+' in mo_Strand:
                 comp.m_ORF_Pos_Olap.append(matched_Prev_ORF_Stop - mo_Start)
             elif '-' in mo_Strand:
```

### Comparing `ORForise-1.4.1/src/ORForise/GFF_Adder.py` & `orforise-1.4.2/src/ORForise/GFF_Adder.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/GFF_Intersector.py` & `orforise-1.4.2/src/ORForise/GFF_Intersector.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/cds_checker.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/cds_checker.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/gene_Lenghts.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/gene_Lenghts.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/genome_Metrics.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/genome_Metrics.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/hypothetical_gene_predictions.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/missed_Gene_Metrics.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/parital_Match_Analysis.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/result_File_Analysis.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/result_File_Analysis.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py` & `orforise-1.4.2/src/ORForise/ORForise_Analysis/start_Codon_Substitution.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/StORForise.py` & `orforise-1.4.2/src/ORForise/StORForise.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/Augustus/Augustus.py` & `orforise-1.4.2/src/ORForise/Tools/Augustus/Augustus.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/Balrog/Balrog.py` & `orforise-1.4.2/src/ORForise/Tools/Balrog/Balrog.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/EasyGene/EasyGene.py` & `orforise-1.4.2/src/ORForise/Tools/EasyGene/EasyGene.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/FGENESB/FGENESB.py` & `orforise-1.4.2/src/ORForise/Tools/FGENESB/FGENESB.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/FragGeneScan/FragGeneScan.py` & `orforise-1.4.2/src/ORForise/Tools/FragGeneScan/FragGeneScan.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GFF/GFF.py` & `orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 import collections
-import sys
+
 try:
     from utils import revCompIterative
     from utils import sortORFs
 except ImportError:
     from ORForise.utils import revCompIterative
     from ORForise.utils import sortORFs
 
 
-def GFF(*args):
-    tool_pred = args[0]
-    genome = args[1]
-    #types = args[2]
-    GFF_ORFs = collections.OrderedDict()
+def StORF_Undetected(tool_pred, genome):
+    storf_orfs = collections.OrderedDict()
     genome_size = len(genome)
-    genome_rev = revCompIterative(genome)
-    with open(tool_pred, 'r') as gff_input:
-        for line in gff_input:
-            if '#' not in line:
-                line = line.split('\t')
-                #gene_types = types.split(',') - Temporary fix
-                #if any(gene_type == line[2] for gene_type in gene_types) and len(line) == 9:  # line[2] for normalrun
-                if 'CDS' in line[2] and len(line) == 9:
-                    start = int(line[3])
-                    stop = int(line[4])
-                    strand = line[6]
-                    info = line[8]
-                    #name = line[8].split('Name=')[1].split(';')[0] # Issue with multiple records for each gene.
-                    if '-' in strand:  # Reverse Compliment starts and stops adjusted
-                        r_start = genome_size - stop
-                        r_stop = genome_size - start
-                        startCodon = genome_rev[r_start:r_start + 3]
-                        stopCodon = genome_rev[r_stop - 2:r_stop + 1]
-                    elif '+' in strand:
-                        startCodon = genome[start - 1:start + 2]
-                        stopCodon = genome[stop - 3:stop]
-                    po = str(start) + ',' + str(stop)
-                    orf = [strand, startCodon, stopCodon, line[2],info] # This needs to detect the type
-                    GFF_ORFs.update({po: orf})
-                # elif "CDS" in line[2]:
-                #     sys.exit("SAS")
+    genome_Rev = revCompIterative(genome)
+    with open(tool_pred, 'r') as storf_input:
+        for line in storf_input:
+            line = line.split()
+            if "StORF" in line[1] and "ORF" in line[2]:
+                start = int(line[3])
+                stop = int(line[4])
+                strand = line[6]
+                if '-' in strand:  # Reverse Compliment starts and stops adjusted
+                    r_start = genome_size - stop
+                    r_stop = genome_size - start
+                    startCodon = genome_Rev[r_start:r_start + 3]
+                    stopCodon = genome_Rev[r_stop - 2:r_stop + 1]
+                elif '+' in strand:
+                    startCodon = genome[start - 1:start - 1 + 3]
+                    stopCodon = genome[stop - 3:stop - 1 + 1]
+                po = str(start) + ',' + str(stop)
+                orf = [strand, startCodon, stopCodon]
+                storf_orfs.update({po: orf})
 
-    GFF_ORFs = sortORFs(GFF_ORFs)
-    return GFF_ORFs
+    storf_orfs = sortORFs(storf_orfs)
+    return storf_orfs
```

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py` & `orforise-1.4.2/src/ORForise/Tools/GLIMMER_3/GLIMMER_3.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GeneMark/GeneMark.py` & `orforise-1.4.2/src/ORForise/Tools/GeneMark/GeneMark.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py` & `orforise-1.4.2/src/ORForise/Tools/GeneMark_HA/GeneMark_HA.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py` & `orforise-1.4.2/src/ORForise/Tools/GeneMark_HMM/GeneMark_HMM.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GeneMark_S/GeneMark_S.py` & `orforise-1.4.2/src/ORForise/Tools/GeneMark_S/GeneMark_S.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py` & `orforise-1.4.2/src/ORForise/Tools/GeneMark_S_2/GeneMark_S_2.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/MetaGene/MetaGene.py` & `orforise-1.4.2/src/ORForise/Tools/MetaGene/MetaGene.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py` & `orforise-1.4.2/src/ORForise/Tools/MetaGeneAnnotator/MetaGeneAnnotator.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py` & `orforise-1.4.2/src/ORForise/Tools/MetaGeneMark/MetaGeneMark.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/Prodigal/Prodigal.py` & `orforise-1.4.2/src/ORForise/Tools/Prodigal/Prodigal.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/Prokka/Prokka.py` & `orforise-1.4.2/src/ORForise/Tools/Prokka/Prokka.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py` & `orforise-1.4.2/src/ORForise/Tools/StORF_Reporter/StORF_Reporter.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py` & `orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/Completely_Undetected/Completey_Undetected.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/StORF_Undetected.py` & `orforise-1.4.2/src/ORForise/Tools/TransDecoder/TransDecoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,32 +4,32 @@
     from utils import revCompIterative
     from utils import sortORFs
 except ImportError:
     from ORForise.utils import revCompIterative
     from ORForise.utils import sortORFs
 
 
-def StORF_Undetected(tool_pred, genome):
-    storf_orfs = collections.OrderedDict()
+def TransDecoder(tool_pred, genome):
+    transDecoder_ORFs = collections.OrderedDict()
     genome_size = len(genome)
-    genome_Rev = revCompIterative(genome)
-    with open(tool_pred, 'r') as storf_input:
-        for line in storf_input:
+    genome_rev = revCompIterative(genome)
+    with open(tool_pred, 'r') as transDecoder_Input:
+        for line in transDecoder_Input:
             line = line.split()
-            if "StORF" in line[1] and "ORF" in line[2]:
+            if len(line) == 9 and "transdecoder" in line[1] and "CDS" in line[2]:
                 start = int(line[3])
                 stop = int(line[4])
                 strand = line[6]
                 if '-' in strand:  # Reverse Compliment starts and stops adjusted
                     r_start = genome_size - stop
                     r_stop = genome_size - start
-                    startCodon = genome_Rev[r_start:r_start + 3]
-                    stopCodon = genome_Rev[r_stop - 2:r_stop + 1]
+                    startCodon = genome_rev[r_start:r_start + 3]
+                    stopCodon = genome_rev[r_stop - 2:r_stop + 1]
                 elif '+' in strand:
-                    startCodon = genome[start - 1:start - 1 + 3]
-                    stopCodon = genome[stop - 3:stop - 1 + 1]
+                    startCodon = genome[start - 1:start + 2]
+                    stopCodon = genome[stop - 3:stop]
                 po = str(start) + ',' + str(stop)
-                orf = [strand, startCodon, stopCodon]
-                storf_orfs.update({po: orf})
+                orf = [strand, startCodon, stopCodon, 'CDS']
+                transDecoder_ORFs.update({po: orf})
 
-    storf_orfs = sortORFs(storf_orfs)
-    return storf_orfs
+    transDecoder_ORFs = sortORFs(transDecoder_ORFs)
+    return transDecoder_ORFs
```

### Comparing `ORForise-1.4.1/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py` & `orforise-1.4.2/src/ORForise/Tools/StORF_Undetected/unvitiated_Genes/unvitiated_Missed_Genes.py`

 * *Files identical despite different names*

### Comparing `ORForise-1.4.1/src/ORForise/utils.py` & `orforise-1.4.2/src/ORForise/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import collections
 
 # Constants
 SHORT_ORF_LENGTH = 300
 MIN_COVERAGE = 75
-ORForise_Version = 'v1.4.1'
+ORForise_Version = 'v1.4.2'
 
 
 def revCompIterative(watson):  # Gets Reverse Complement
     return watson.upper()[::-1].translate(str.maketrans("ATCGRYKMVBHD","TAGCYRMKBVDH"))
 
 
 def sortORFs(tool_ORFs):  # Will only sort by given start position
```

### Comparing `ORForise-1.4.1/src/ORForise.egg-info/PKG-INFO` & `orforise-1.4.2/src/ORForise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ORForise
-Version: 1.4.1
+Version: 1.4.2
 Summary: ORForise - Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions.
 Home-page: https://github.com/NickJD/ORForise
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/ORForise/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # ORForise - Prokaryote Genome Annotation Analysis and Comparison Platform
 ## Published in Bioinformatics :   https://academic.oup.com/bioinformatics/article/38/5/1198/6454948
 ### Platform for analysing and comparing Prokaryote CoDing Sequence (CDS) Gene Predictions. 
 ### Novel genome annotations can be compared to a provided reference annotation from Ensembl and predictions from other tools (or any given GFF annotation) .
 
 # Requirements and Installation:
@@ -57,15 +58,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Annotation_Compare.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -t TOOL -tp TOOL_PREDICTION
                              [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.1: Annotatione-Compare Run Parameters.
+ORForise v1.4.2: Annotatione-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -t TOOL               Which tool to analyse? (Prodigal)
   -tp TOOL_PREDICTION   Tool genome prediction file (.gff) - Different Tool Parameters are compared individually via
@@ -107,15 +108,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: Aggregate_Compare.py [-h] -dna GENOME_DNA -t TOOLS -tp TOOL_PREDICTIONS -ref REFERENCE_ANNOTATION
                             [-rt REFERENCE_TOOL] [-o OUTNAME] [-v {True,False}]
 
-ORForise v1.4.1: Aggregate-Compare Run Parameters.
+ORForise v1.4.2: Aggregate-Compare Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -t TOOLS              Which tools to analyse? (Prodigal,GeneMarkS)
   -tp TOOL_PREDICTIONS  Tool genome prediction file (.gff) - Providefile locations for each tool comma separated
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
@@ -261,15 +262,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Adder.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add ADDITIONAL_ANNOTATION -o
                     OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-gene_ident GENE_IDENT] [-olap OVERLAP]
 
-ORForise v1.4.1: GFF-Adder Run Parameters.
+ORForise v1.4.2: GFF-Adder Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
@@ -323,15 +324,15 @@
 ```python
 Thank you for using ORForise
 Please report any issues to: https://github.com/NickJD/ORForise/issues
 #####
 usage: GFF_Intersector.py [-h] -dna GENOME_DNA -ref REFERENCE_ANNOTATION -at ADDITIONAL_TOOL -add
                           ADDITIONAL_ANNOTATION -o OUTPUT_FILE [-rt REFERENCE_TOOL] [-gi GENE_IDENT] [-cov COVERAGE]
 
-ORForise v1.4.1: GFF-Intersector Run Parameters.
+ORForise v1.4.2: GFF-Intersector Run Parameters.
 
 Required Arguments:
   -dna GENOME_DNA       Genome DNA file (.fa) which both annotations are based on
   -ref REFERENCE_ANNOTATION
                         Which reference annotation file to use as reference?
   -at ADDITIONAL_TOOL   Which format to use for additional annotation?
   -add ADDITIONAL_ANNOTATION
```

### Comparing `ORForise-1.4.1/src/ORForise.egg-info/SOURCES.txt` & `orforise-1.4.2/src/ORForise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

