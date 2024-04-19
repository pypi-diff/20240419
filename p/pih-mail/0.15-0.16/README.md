# Comparing `tmp/pih-mail-0.15.tar.gz` & `tmp/pih-mail-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mail-0.15.tar", last modified: Wed Apr 10 01:44:33 2024, max compression
+gzip compressed data, was "pih-mail-0.16.tar", last modified: Fri Apr 19 02:30:10 2024, max compression
```

## Comparing `pih-mail-0.15.tar` & `pih-mail-0.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:44:33.927933 pih-mail-0.15/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:44:33.521534 pih-mail-0.15/MailService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mail-0.15/MailService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-15 01:08:42.000000 pih-mail-0.15/MailService/__main__.py
--rw-rw-rw-   0        0        0        2 2023-07-09 01:12:40.000000 pih-mail-0.15/MailService/api.py
--rw-rw-rw-   0        0        0     1203 2024-04-10 00:27:27.000000 pih-mail-0.15/MailService/const.py
--rw-rw-rw-   0        0        0    10167 2024-04-09 23:26:12.000000 pih-mail-0.15/MailService/service.py
--rw-rw-rw-   0        0        0      318 2024-04-10 01:44:33.865411 pih-mail-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:44:33.844767 pih-mail-0.15/pih_mail.egg-info/
--rw-rw-rw-   0        0        0      318 2024-04-10 01:44:32.000000 pih-mail-0.15/pih_mail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:44:33.927933 pih-mail-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 02:30:10.982240 pih-mail-0.16/
+drwxrwxrwx   0        0        0        0 2024-04-19 02:30:10.182738 pih-mail-0.16/MailService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mail-0.16/MailService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-15 01:08:42.000000 pih-mail-0.16/MailService/__main__.py
+-rw-rw-rw-   0        0        0        2 2023-07-09 01:12:40.000000 pih-mail-0.16/MailService/api.py
+-rw-rw-rw-   0        0        0     1178 2024-04-19 02:26:40.000000 pih-mail-0.16/MailService/const.py
+-rw-rw-rw-   0        0        0    11073 2024-04-18 06:12:00.000000 pih-mail-0.16/MailService/service.py
+-rw-rw-rw-   0        0        0      318 2024-04-19 02:30:10.935373 pih-mail-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 02:30:10.904116 pih-mail-0.16/pih_mail.egg-info/
+-rw-rw-rw-   0        0        0      318 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 02:30:09.000000 pih-mail-0.16/pih_mail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 02:30:10.982240 pih-mail-0.16/setup.cfg
```

### Comparing `pih-mail-0.15/MailService/const.py` & `pih-mail-0.16/MailService/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import ipih
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
-from enum import Enum
-
 NAME: str = "Mail"
 SECTION: str = "MailboxInfo"
 
 HOST = Hosts.WS255
 
 # 0.1 - Persistance caching for email address deliverability checking status and  recall for email deliverability checking if status == UNKNOWN
 # 0.12 - using new method for checking mail deliverity
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 TIMEOUT: int = 10
 TRY_AGAIN_COUNT: int = 5
 TRY_AGAIN_SLEEP_TIME: int = 1
 PACKAGES: tuple[str, ...] = (
     "imap_tools",
     "dnspython",
```

### Comparing `pih-mail-0.15/MailService/service.py` & `pih-mail-0.16/MailService/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 SC = A.CT_SC
 EVM = A.CT_EVM
 
 ISOLATED: bool = False
 
 
 class DH:
-    
+
     EMAIL_IT_USER_PASSWORD: str | None = None
+    EMAIL_RECEPTION_USER_PASSWORD: str | None = None
+    EMAIL_CALL_CENTER_USER_PASSWORD: str | None = None
     EXTERNAL_EMAIL_USER_PASSWORD: str | None = None
     EMAIL_ADD_EMAIL_USER_PASSWORD: str | None = None
     ABSTRACT_API_KEY: str | None = None
 
 
 def start(as_standalone: bool = False) -> None:
 
@@ -44,14 +46,24 @@
                     (
                         A.CT_ADDR.EMAIL_SERVER_ADDRESS,
                         A.CT_EML.IT,
                         DH.EMAIL_IT_USER_PASSWORD,
                     ),
                     (
                         A.CT_ADDR.EMAIL_SERVER_ADDRESS,
+                        A.CT_EML.RECEPTION,
+                        DH.EMAIL_RECEPTION_USER_PASSWORD,
+                    ),
+                    (
+                        A.CT_ADDR.EMAIL_SERVER_ADDRESS,
+                        A.CT_EML.CALL_CENTRE,
+                        DH.EMAIL_CALL_CENTER_USER_PASSWORD,
+                    ),
+                    (
+                        A.CT_ADDR.EMAIL_SERVER_ADDRESS,
                         A.CT_EML.ADD_EMAIL,
                         DH.EMAIL_ADD_EMAIL_USER_PASSWORD,
                     ),
                     (
                         A.CT_EML.EXTERNAL_SERVER,
                         A.CT_EML.EXTERNAL,
                         DH.EXTERNAL_EMAIL_USER_PASSWORD,
@@ -101,28 +113,32 @@
                                         mail_message.text,
                                         mail_message.from_,
                                     )
                                     new_mail_messages.append(new_mail_message)
                                     A.E.new_mail_message_was_received(new_mail_message)
                                 mail_message = mail_message_list[-1]
                                 A.A_DS.value(
-                                    MailboxInfo(mail_message.date, int(mail_message.uid)),
+                                    MailboxInfo(
+                                        mail_message.date, int(mail_message.uid)
+                                    ),
                                     mailbox_address,
                                     SECTION,
                                 )
                     except Exception as _:
                         pass
                 return True
             check_email_accessibility: bool = sc == SC.check_email_accessibility
             if check_email_accessibility or sc == SC.get_email_information:
                 email_address: str = lw(pl.next())
                 method: str = pl.next()
                 cached: bool = pl.next()
                 result: bool | None = (
-                    one(A.R_DS.value(email_address, None, SECTION_DELIVERITY)) if cached else None
+                    one(A.R_DS.value(email_address, None, SECTION_DELIVERITY))
+                    if cached
+                    else None
                 )
                 if nn(result):
                     return result
                 domain: str = email_address.split(A.CT.EMAIL_SPLITTER)[1]
                 if check_email_accessibility and method == A.D.get(
                     EmailVerificationMethods.NORMAL
                 ):
@@ -209,14 +225,20 @@
                 finally:
                     server.quit()
 
             return False
 
         def service_starts_handler() -> None:
             DH.EMAIL_IT_USER_PASSWORD = A.D_V_E.value("EMAIL_IT_USER_PASSWORD")
+            DH.EMAIL_RECEPTION_USER_PASSWORD = A.D_V_E.value(
+                "EMAIL_RECEPTION_USER_PASSWORD"
+            )
+            DH.EMAIL_CALL_CENTER_USER_PASSWORD = A.D_V_E.value(
+                "EMAIL_CALL_CENTER_USER_PASSWORD"
+            )
             DH.EXTERNAL_EMAIL_USER_PASSWORD = A.D_V_E.value(
                 "EXTERNAL_EMAIL_USER_PASSWORD"
             )
             DH.EMAIL_ADD_EMAIL_USER_PASSWORD = A.D_V_E.value(
                 "EMAIL_ADD_EMAIL_USER_PASSWORD"
             )
             DH.ABSTRACT_API_KEY = A.D_V_E.value("ABSTRACT_API_KEY")
```

