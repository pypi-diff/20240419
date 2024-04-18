# Comparing `tmp/ipiranga-inovai-project-lib-0.3.tar.gz` & `tmp/ipiranga-inovai-project-lib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-0.3.tar", last modified: Fri Apr  5 20:34:21 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-0.4.tar", last modified: Thu Apr 18 22:25:52 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-0.3.tar` & `ipiranga-inovai-project-lib-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:34:21.396206 ipiranga-inovai-project-lib-0.3/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.3/LICENSE
--rw-rw-rw-   0        0        0      516 2024-04-05 20:34:21.396206 ipiranga-inovai-project-lib-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 20:34:21.382005 ipiranga-inovai-project-lib-0.3/inovai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.3/inovai/__init__.py
--rw-rw-rw-   0        0        0    12475 2024-02-28 20:27:08.000000 ipiranga-inovai-project-lib-0.3/inovai/entities.py
--rw-rw-rw-   0        0        0      255 2024-04-05 20:24:43.000000 ipiranga-inovai-project-lib-0.3/inovai/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:34:21.391489 ipiranga-inovai-project-lib-0.3/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-04-05 20:34:21.000000 ipiranga-inovai-project-lib-0.3/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-05 20:34:21.000000 ipiranga-inovai-project-lib-0.3/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:34:21.000000 ipiranga-inovai-project-lib-0.3/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 20:34:21.000000 ipiranga-inovai-project-lib-0.3/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 20:34:21.396206 ipiranga-inovai-project-lib-0.3/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-04-05 20:34:17.000000 ipiranga-inovai-project-lib-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:25:52.168255 ipiranga-inovai-project-lib-0.4/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.4/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-04-18 22:25:52.165640 ipiranga-inovai-project-lib-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 22:25:52.145122 ipiranga-inovai-project-lib-0.4/inovai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.4/inovai/__init__.py
+-rw-rw-rw-   0        0        0    12752 2024-04-18 22:22:29.000000 ipiranga-inovai-project-lib-0.4/inovai/entities.py
+-rw-rw-rw-   0        0        0      305 2024-04-18 22:23:03.000000 ipiranga-inovai-project-lib-0.4/inovai/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:25:52.161063 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-04-18 22:25:51.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-18 22:25:52.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 22:25:52.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 22:25:52.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 22:25:52.169496 ipiranga-inovai-project-lib-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-04-18 22:25:31.000000 ipiranga-inovai-project-lib-0.4/setup.py
```

### Comparing `ipiranga-inovai-project-lib-0.3/PKG-INFO` & `ipiranga-inovai-project-lib-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.3
+Version: 0.4
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.3/inovai/entities.py` & `ipiranga-inovai-project-lib-0.4/inovai/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     issuer_cnpj = Column('cd_cnpj_emit', String(14), nullable=False)
     issuance_date = Column('dt_emis_doc_integr', Date, nullable=False)
     fiscal_date = Column('dt_fisc', Date, nullable=False)
     created_at = Column('dt_hora_criacao', DateTime, nullable=False)
     updated_at = Column('dt_incl', DateTime, nullable=False, server_default='NOW()')
     request_id = Column('id_req_doc_fisc', String(40), nullable=True)
     origin = Column('nm_sist_orig', String(50), nullable=True)
+    responsible_movement = Column('id_cnpj_mov', String(), nullable=True)
 
     integration_batch = relationship('IntegrationDocumentBatch', back_populates='integration_document')
     kit_integration_document_status = relationship("KitIntegrationDocumentStatus", back_populates="integration_document")
 
     def to_dict(self):
         return {
             "no_seq_doc_integr": self.document_id,
@@ -44,15 +45,17 @@
             "cd_filial": self.branch_code,
             "cd_cnpj_dest": self.recipient_cnpj,
             "cd_cnpj_emit": self.issuer_cnpj,
             "dt_emis_doc_integr": self.issuance_date.strftime("%Y-%m-%d") if self.issuance_date is not None else None,
             "dt_fisc": self.fiscal_date.strftime("%Y-%m-%d") if self.fiscal_date is not None else None,
             "dt_hora_criacao": self.created_at.strftime("%Y-%m-%d %H:%M:%S") if self.created_at is not None else None,
             "dt_incl": self.updated_at.strftime("%Y-%m-%d %H:%M:%S") if self.updated_at is not None else None,
-            "request_id": self.request_id
+            "request_id": self.request_id,
+            "nm_sist_orig": self.origin,
+            "id_cnpj_mov": self.responsible_movement
         }
 
     def __str__(self):
         return str(self.to_dict())
 
 
 class ObiOrganizationUnit(Base):
@@ -88,24 +91,26 @@
     first_date_document = Column('dt_ini_doc_integr', Date)
     last_date_document = Column('dt_fim_doc_integr', Date)
     error_reason = Column('ds_mot_erro', String)
     batch_code = Column('cd_lote_obi', String)
     start_integration_date = Column('dt_hora_ini_lote_integr', DateTime)
     end_integration_date = Column('dt_hora_fim_lote_integr', DateTime)
     created_at = Column('dt_incl', DateTime, nullable=False)
+    status = Column('ds_status_integr', String(), nullable=False)
 
     batch_files = relationship('BatchFileIntegration', back_populates='integration_batch')
     integration_processing = relationship('IntegrationProcessing', back_populates='integration_batch')
 
-    def __init__(self, integration_batch_id, employer_number, first_date_document, last_date_document):
+    def __init__(self, integration_batch_id, employer_number, first_date_document, last_date_document, status):
         super().__init__()
         self.integration_batch_id = integration_batch_id
         self.employer_number = employer_number
         self.first_date_document = first_date_document
         self.last_date_document = last_date_document
+        self.status = status
         self.start_integration_date = datetime.now()
         self.created_at = self.start_integration_date
 
 
 class IntegrationFile(Base):
     __tablename__ = 'arquivo_integracao'
     __table_args__ = {'schema': 'fiscal'}
```

### Comparing `ipiranga-inovai-project-lib-0.3/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.3
+Version: 0.4
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.3/setup.py` & `ipiranga-inovai-project-lib-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

