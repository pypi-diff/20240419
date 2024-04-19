# Comparing `tmp/civicpy-3.0.0.tar.gz` & `tmp/civicpy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civicpy-3.0.0.tar", last modified: Mon Jan  9 22:25:26 2023, max compression
+gzip compressed data, was "civicpy-3.1.0.tar", last modified: Fri Apr 19 15:18:29 2024, max compression
```

## Comparing `civicpy-3.0.0.tar` & `civicpy-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:25:26.026200 civicpy-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-09 22:25:17.000000 civicpy-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-09 22:25:26.026200 civicpy-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-09 22:25:17.000000 civicpy-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:25:26.026200 civicpy-3.0.0/civicpy/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-09 22:25:17.000000 civicpy-3.0.0/civicpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-09 22:25:17.000000 civicpy-3.0.0/civicpy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89093 2023-01-09 22:25:17.000000 civicpy-3.0.0/civicpy/civic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-01-09 22:25:17.000000 civicpy-3.0.0/civicpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-01-09 22:25:17.000000 civicpy-3.0.0/civicpy/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 22:25:26.026200 civicpy-3.0.0/civicpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-09 22:25:25.000000 civicpy-3.0.0/civicpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-09 22:25:25.000000 civicpy-3.0.0/civicpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 22:25:25.000000 civicpy-3.0.0/civicpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-09 22:25:25.000000 civicpy-3.0.0/civicpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-09 22:25:25.000000 civicpy-3.0.0/civicpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-09 22:25:25.000000 civicpy-3.0.0/civicpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 22:25:26.026200 civicpy-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-09 22:25:17.000000 civicpy-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:18:29.114943 civicpy-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 15:18:25.000000 civicpy-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-19 15:18:29.114943 civicpy-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 15:18:25.000000 civicpy-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:18:29.110943 civicpy-3.1.0/civicpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-19 15:18:25.000000 civicpy-3.1.0/civicpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 15:18:25.000000 civicpy-3.1.0/civicpy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91291 2024-04-19 15:18:25.000000 civicpy-3.1.0/civicpy/civic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-19 15:18:25.000000 civicpy-3.1.0/civicpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-19 15:18:25.000000 civicpy-3.1.0/civicpy/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:18:29.114943 civicpy-3.1.0/civicpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-19 15:18:29.000000 civicpy-3.1.0/civicpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 15:18:29.000000 civicpy-3.1.0/civicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:18:29.000000 civicpy-3.1.0/civicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 15:18:29.000000 civicpy-3.1.0/civicpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 15:18:29.000000 civicpy-3.1.0/civicpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 15:18:29.000000 civicpy-3.1.0/civicpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 15:18:29.114943 civicpy-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-19 15:18:25.000000 civicpy-3.1.0/setup.py
```

### Comparing `civicpy-3.0.0/LICENSE` & `civicpy-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `civicpy-3.0.0/README.md` & `civicpy-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `civicpy-3.0.0/civicpy/__init__.py` & `civicpy-3.1.0/civicpy/__init__.py`

 * *Files identical despite different names*

### Comparing `civicpy-3.0.0/civicpy/__version__.py` & `civicpy-3.1.0/civicpy/__version__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __title__ = 'civicpy'
 __description__ = 'CIViC variant knowledgebase analysis toolkit.'
 __url__ = 'http://civicpy.org'
 __major__ = '3'
-__minor__ = '0'
+__minor__ = '1'
 __patch__ = '0'
 __meta_label__ = ''
 __short_version__ = "{}.{}".format(__major__, __minor__)
 __version__ = "{}.{}".format(__short_version__, __patch__)
 if __meta_label__:
     __version__ += "-{}".format(__meta_label__)
-__authors__ = ['Alex H. Wagner', 'Susanna Kiwala']
+__authors__ = ['Alex H. Wagner', 'Susanna Kiwala', 'Adam Coffman']
 __author_email__ = 'help@civicpy.org'
 __license__ = 'MIT'
-__copyright__ = 'Copyright 2018-2023 The Griffith Lab'
+__copyright__ = 'Copyright 2018-2024 The Griffith Lab'
```

### Comparing `civicpy-3.0.0/civicpy/civic.py` & `civicpy-3.1.0/civicpy/civic.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,20 +442,28 @@
     })
     _COMPLEX_FIELDS = CivicRecord._COMPLEX_FIELDS.union({
         'aliases',
         'assertions',
         'evidence_items',
         'sources',
         'variants',
+        'parsed_name'
     })
 
     def __init__(self, **kwargs):
         self._evidence_items = []
         self._assertions = []
         self._variants = []
+
+        # Convert parsed name types from camel to snake case
+        parsed_name = kwargs.get('parsed_name')
+        if parsed_name:
+            for pn in parsed_name:
+                pn['type'] = ''.join(['_' + c.lower() if c.isupper() else c for c in pn['type']]).lstrip('_')
+
         super().__init__(**kwargs)
 
     @property
     def evidence_sources(self):
         sources = set()
         for evidence in self.evidence_items:
             if evidence.source is not None:
@@ -1211,27 +1219,32 @@
     elements = [cls(**x, partial=True) for x in response_elements]
     cache = [x['id'] for x in response_elements]
     CACHE['{}_all_ids'.format(pluralize(element))] = cache
     return elements
 
 
 def _postprocess_response_element(e, element):
+    if e is None:
+        raise Exception("{} not found".format(element.title()))
     e['type'] = element
     if element == 'assertion':
         e['molecular_profile_id'] = e['molecular_profile']['id']
         e['evidence_ids'] = [evidence['id'] for evidence in e['evidenceItems']]
         e['status'] = e['status'].lower()
     elif element == 'evidence':
         e['molecular_profile_id'] = e['molecular_profile']['id']
         e['assertion_ids'] = [a['id'] for a in e['assertions']]
         e['status'] = e['status'].lower()
     elif element == 'variant':
         e['gene_id'] = e['gene']['id']
         e['entrez_name'] = e['gene']['name']
-        e['entrez_id'] = e['gene']['entrezId']
+        #TODO: handle other types of Variants
+        if e['__typename'] != 'GeneVariant':
+            raise Exception("Variant type {} not supported yet".format(e['__typename']))
+        e['entrez_id'] = e['gene']['featureInstance']['entrezId']
         build = e['referenceBuild']
         if build == 'GRCH37':
             build = 'GRCh37'
         elif build == 'GRCH38':
             build = 'GRCh38'
         e['coordinates'] = {
             'ensembl_version': e['ensemblVersion'],
@@ -1321,15 +1334,15 @@
     return """
         query gene($id: Int!) {
             gene(id: $id) {
                 id
                 name
                 description
                 entrez_id: entrezId
-                aliases: geneAliases
+                aliases: featureAliases
                 sources {
                     id
                     name
                     title
                     citation
                     citation_id: citationId
                     source_type: sourceType
@@ -1363,15 +1376,15 @@
                 endCursor
               }
               nodes {
                 id
                 name
                 description
                 entrez_id: entrezId
-                aliases: geneAliases
+                aliases: featureAliases
                 sources {
                     id
                     name
                     title
                     citation
                     citation_id: citationId
                     source_type: sourceType
@@ -1404,14 +1417,29 @@
                 description
                 molecular_profile_score: molecularProfileScore
                 name
                 variants {
                   id
                 }
                 aliases: molecularProfileAliases
+                parsed_name: parsedName {
+                    type: __typename
+                    ... on MolecularProfileTextSegment {
+                        text
+                    }
+                    ... on Feature {
+                        id
+                        name
+                    }
+                    ... on Variant {
+                        id
+                        name
+                        deprecated
+                    }
+                }
                 sources {
                     id
                     name
                     title
                     citation
                     citation_id: citationId
                     source_type: sourceType
@@ -1450,14 +1478,29 @@
                 description
                 molecular_profile_score: molecularProfileScore
                 name
                 variants {
                   id
                 }
                 aliases: molecularProfileAliases
+                parsed_name: parsedName {
+                    type: __typename
+                    ... on MolecularProfileTextSegment {
+                        text
+                    }
+                    ... on Feature {
+                        id
+                        name
+                    }
+                    ... on Variant {
+                        id
+                        name
+                        deprecated
+                    }
+                }
                 sources {
                     id
                     name
                     title
                     citation
                     citation_id: citationId
                     source_type: sourceType
@@ -1481,98 +1524,112 @@
             }
         }"""
 
 def _construct_get_variant_payload():
     return """
         query variant($id: Int!) {
             variant(id: $id) {
+                __typename
                 id
                 name
-                allele_registry_id: alleleRegistryId
-                gene {
+                ... on GeneVariant {
+                    allele_registry_id: alleleRegistryId
+                    clinvar_entries: clinvarIds
+                    hgvs_expressions: hgvsDescriptions
+                    variantBases
+                    referenceBases
+                    referenceBuild
+                    primaryCoordinates {
+                        chromosome
+                        representativeTranscript
+                        start
+                        stop
+                    }
+                    secondaryCoordinates {
+                        chromosome
+                        representativeTranscript
+                        start
+                        stop
+                    }
+                    ensemblVersion
+                }
+                gene: feature {
                     id
                     name
-                    entrezId
+                    featureInstance {
+                        ... on Gene {
+                            entrezId
+                        }
+                    }
                 }
                 single_variant_molecular_profile_id: singleVariantMolecularProfileId
-                clinvar_entries: clinvarIds
-                hgvs_expressions: hgvsDescriptions
                 variant_aliases: variantAliases
                 variant_types: variantTypes {
                     id
                     name
                     so_id: soid
                     description
                     url
                 }
-                variantBases
-                referenceBases
-                referenceBuild
-                primaryCoordinates {
-                    chromosome
-                    representativeTranscript
-                    start
-                    stop
-                }
-                secondaryCoordinates {
-                    chromosome
-                    representativeTranscript
-                    start
-                    stop
-                }
-                ensemblVersion
             }
         }"""
 
 
 def _construct_get_all_variants_payload():
     return """
         query variants($after: String) {
-            variants(after: $after) {
+            variants(after: $after, category: GENE) {
                 totalCount
                 pageInfo {
                   hasNextPage
                   endCursor
                 }
                 nodes {
+                    __typename
                     id
                     name
-                    allele_registry_id: alleleRegistryId
-                    gene {
-                      id
-                      name
-                      entrezId
+                    ... on GeneVariant {
+                        allele_registry_id: alleleRegistryId
+                        clinvar_entries: clinvarIds
+                        hgvs_expressions: hgvsDescriptions
+                        variantBases
+                        referenceBases
+                        referenceBuild
+                        primaryCoordinates {
+                            chromosome
+                            representativeTranscript
+                            start
+                            stop
+                        }
+                        secondaryCoordinates {
+                            chromosome
+                            representativeTranscript
+                            start
+                            stop
+                        }
+                        ensemblVersion
+                    }
+                    gene: feature {
+                        id
+                        name
+                        featureInstance {
+                            ... on Gene {
+                                entrezId
+                            }
+                        }
                     }
                     single_variant_molecular_profile_id: singleVariantMolecularProfileId
-                    clinvar_entries: clinvarIds
-                    hgvs_expressions: hgvsDescriptions
                     variant_aliases: variantAliases
                     variant_types: variantTypes {
                         id
                         name
                         so_id: soid
                         description
                         url
                     }
-                    variantBases
-                    referenceBases
-                    referenceBuild
-                    primaryCoordinates {
-                        chromosome
-                        representativeTranscript
-                        start
-                        stop
-                    }
-                    secondaryCoordinates {
-                        chromosome
-                        representativeTranscript
-                        start
-                        stop
-                    }
-                    ensemblVersion
                 }
             }
         }"""
 
 def _construct_get_evidence_payload():
     return """
         query evidenceItem($id: Int!) {
@@ -2158,15 +2215,15 @@
         left_idx = chr_idx.searchsorted(chromosome)
         right_idx = chr_idx.searchsorted(chromosome, side='right')
         chr_ct_idx = chr_idx[left_idx:right_idx].index
         right_idx = start_idx.searchsorted(stop, side='right')
         start_ct_idx = start_idx[:right_idx].index
         left_idx = stop_idx.searchsorted(start)
         stop_ct_idx = stop_idx[left_idx:].index
-        match_idx = chr_ct_idx & start_ct_idx & stop_ct_idx
+        match_idx = list(set(chr_ct_idx) & set(start_ct_idx) & set(stop_ct_idx))
         m_df = ct.loc[match_idx, ]
         if search_mode == 'any':
             var_digests = m_df.v_hash.to_list()
             return [CACHE[v] for v in var_digests]
         elif search_mode == 'query_encompassing':
             match_idx = (start <= m_df.start) & (stop >= m_df.stop)
         elif search_mode == 'variant_encompassing':
```

### Comparing `civicpy-3.0.0/civicpy/cli.py` & `civicpy-3.1.0/civicpy/cli.py`

 * *Files identical despite different names*

### Comparing `civicpy-3.0.0/civicpy/exports.py` & `civicpy-3.1.0/civicpy/exports.py`

 * *Files identical despite different names*

### Comparing `civicpy-3.0.0/setup.py` & `civicpy-3.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup
 from civicpy.__version__ import __version__, __authors__, __author_email__, __description__, __url__
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='civicpy',
     version=__version__,
     packages=['civicpy'],
     url=__url__,
     license='MIT',
     author=', '.join(__authors__),
     author_email=__author_email__,
     description=__description__,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
@@ -27,19 +33,19 @@
         'vcfpy',
         'pysam',
         'backports-datetime-fromisoformat',
         'deprecation',
     ],
     extras_require={
         'test': [
-            'pytest==4.1.0',
-            'pytest-cov==2.9.0',
-            'attrs==18.2.0',
-            'python-coveralls',
-            'coverage<5.0',
+            'pytest==6.2.5',
+            'pytest-cov==5.0.0',
+            'attrs==22.1.0',
+            'coveralls',
+            'coverage<7.4.4',
         ],
         'docs': [
             'sphinx',
             'sphinxjp.themes.basicstrap',
             'sphinxcontrib.programoutput'
         ]
     },
```

