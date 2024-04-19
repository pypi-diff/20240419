# Comparing `tmp/hnt_nf_jira_library-0.3.8.tar.gz` & `tmp/hnt_nf_jira_library-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.3.8.tar", last modified: Thu Apr 18 13:06:05 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.9.tar", last modified: Thu Apr 18 20:17:40 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.3.8.tar` & `hnt_nf_jira_library-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:06:05.071109 hnt_nf_jira_library-0.3.8/
--rw-rw-rw-   0        0        0      286 2024-04-18 13:06:05.066963 hnt_nf_jira_library-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 13:06:05.064964 hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-18 13:06:04.000000 hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-18 13:06:04.000000 hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:06:04.000000 hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-18 13:06:04.000000 hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 13:06:04.000000 hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 13:06:05.000956 hnt_nf_jira_library-0.3.8/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.8/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:06:05.049836 hnt_nf_jira_library-0.3.8/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:06:05.061993 hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     4336 2024-04-18 12:56:37.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3354 2024-04-18 12:41:15.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.8/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    14826 2024-04-17 17:51:01.000000 hnt_nf_jira_library-0.3.8/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-18 13:06:05.071109 hnt_nf_jira_library-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-18 13:05:59.000000 hnt_nf_jira_library-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 20:17:40.736985 hnt_nf_jira_library-0.3.9/
+-rw-rw-rw-   0        0        0      286 2024-04-18 20:17:40.733982 hnt_nf_jira_library-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 20:17:40.732016 hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-18 20:17:40.000000 hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-04-18 20:17:40.000000 hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 20:17:40.000000 hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-18 20:17:40.000000 hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 20:17:40.000000 hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 20:17:40.642977 hnt_nf_jira_library-0.3.9/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.9/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 20:17:40.711980 hnt_nf_jira_library-0.3.9/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-18 20:17:40.727981 hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     4338 2024-04-18 19:53:59.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     3354 2024-04-18 12:41:15.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.9/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    14829 2024-04-18 20:06:55.000000 hnt_nf_jira_library-0.3.9/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 20:17:40.737984 hnt_nf_jira_library-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-18 20:16:07.000000 hnt_nf_jira_library-0.3.9/setup.py
```

### Comparing `hnt_nf_jira_library-0.3.8/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.9/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 new_fields_data[key] = new_value
 
         return new_fields_data
     
 class GuiandoHelper(BaseHelper):
         
         def __init__(self):
-            self._check_sefaz = lambda form_data: form_data[POSSUI_CHAVE_ACESSO][0] == 1
+            self._check_sefaz = lambda form_data: form_data[POSSUI_CHAVE_ACESSO][0] == "1"
             self._check_document_type = lambda document_type: 'nota_fiscal' if document_type == "2" else 'fatura'
             self.ConsumoService = ConsumoService()
 
         def download_pdf_nexinvoice(self, attachment):
             path = attachment[ARQUIVOS_DA_FATURA][0]
             pdf = self._download_pdf(path)
             return pdf
```

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.3.9/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.9/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.8/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.9/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         sintese_itens = []
         validTotalPercents = 0.0
 
         if not issue["allocation_data"]:
 
             item = {
                 "centro": issue["domain_data"]["centro"]["centro"],
-                "centro_custo": f"{issue['domain_data']['centro']['centro']}210",
+                "centro_custo": f"{issue['domain_data']['centro']['centro_custo']}",
                 "cod_imposto": "C6",
                 "valor_bruto": str(issue["json_data"][VALOR_TOTAL_DA_FATURA]),
             }
 
             sintese_item = {
                 "categoria_cc": "K",
                 "quantidade": 1,
```

