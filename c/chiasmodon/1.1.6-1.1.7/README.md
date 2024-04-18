# Comparing `tmp/chiasmodon-1.1.6.tar.gz` & `tmp/chiasmodon-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.6.tar", last modified: Thu Apr 18 03:07:36 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.7.tar", last modified: Thu Apr 18 03:14:42 2024, max compression
```

## Comparing `chiasmodon-1.1.6.tar` & `chiasmodon-1.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.6/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13130 2024-04-17 23:12:00.000000 chiasmodon-1.1.6/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21184 2024-04-18 03:07:32.000000 chiasmodon-1.1.6/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 03:07:30.000000 chiasmodon-1.1.6/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 03:07:35.000000 chiasmodon-1.1.6/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:14:42.900490 chiasmodon-1.1.7/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.7/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 03:14:42.900490 chiasmodon-1.1.7/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13873 2024-04-18 03:14:25.000000 chiasmodon-1.1.7/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:14:42.900490 chiasmodon-1.1.7/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 03:14:42.000000 chiasmodon-1.1.7/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 03:14:42.000000 chiasmodon-1.1.7/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 03:14:42.000000 chiasmodon-1.1.7/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 03:14:42.000000 chiasmodon-1.1.7/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 03:14:42.000000 chiasmodon-1.1.7/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:14:42.900490 chiasmodon-1.1.7/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21175 2024-04-18 03:12:56.000000 chiasmodon-1.1.7/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 03:13:47.000000 chiasmodon-1.1.7/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 03:14:42.900490 chiasmodon-1.1.7/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 03:13:58.000000 chiasmodon-1.1.7/setup.py
```

### Comparing `chiasmodon-1.1.6/LICENSE.txt` & `chiasmodon-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.6/PKG-INFO` & `chiasmodon-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.6
+Version: 1.1.7
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -52,66 +52,78 @@
 pip install chiasmodon
 ```
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
 
 
 ```
-usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-C COUNTRY]
-                         [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT]
-                         [-L LIMIT] [-v]
+usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-n ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-s] [-sc SCAN_CLIENTS]
+                         [-se SCAN_EMPLOYEES] [-C COUNTRY] [-A] [-de] [-r] [-o OUTPUT] [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}]
+                         [-ot {text,json,csv}] [--init INIT] [-T TIMEOUT] [-L LIMIT] [-v]
 
 Chiasmodon CLI
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Search by domain.
   -a APP, --app APP     Search by google play applciton id.
   -c CIDR, --cidr CIDR  Search by CIDR.
-  -s ASN, --asn ASN     Search by ASN.
+  -n ASN, --asn ASN     Search by ASN.
   -e EMAIL, --email EMAIL
                         Search by email, only pro, only pro account.
   -u USERNAME, --username USERNAME
                         Search by username, only pro account.
   -p PASSWORD, --password PASSWORD
                         Search by password, only pro account.
   -ep ENDPOINT, --endpoint ENDPOINT
                         Search by url endpoint.
+  -s, --scan            scan the company domain (Related company, Clients, Employees, Company ASNs, Company Apps).
+  -sc SCAN_CLIENTS, --scan-clients SCAN_CLIENTS
+                        Run clients scan, default is yes, Ex: -sc no
+  -se SCAN_EMPLOYEES, --scan-employees SCAN_EMPLOYEES
+                        Run employees scan, default is yes, Ex: -se no
   -C COUNTRY, --country COUNTRY
                         sort result by country code default is all
-  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
-                        type view the result default is "cred".
+  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
+  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
+  -r, --related         Get related company domains,this option work only with (-d or --domain), default False
   -o OUTPUT, --output OUTPUT
                         filename to save the result
+  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
+                        type view the result default is "cred".
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
-  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
-  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
   -T TIMEOUT, --timeout TIMEOUT
                         request timeout default is 60.
   -L LIMIT, --limit LIMIT
                         limit results default is 10000.
   -v, --version         version.
 
 Examples:
 
-    # Search for target domain, you will see the result for only this "example.com"
-    chiasmodon_cli.py --domain example.com
+    # Scan company by domain
+    chiasmodon_cli.py --domain example.com --scan
 
+    # Search for target domain, you will see the result for only this "example.com" 
+    chiasmodon_cli.py --domain example.com 
+    
     # Search for target subdomains
-    chiasmodon_cli.py --domain example.com --all
-
-    # Search for target domain, you will see the result for only this "example.com" on United States
-    chiasmodon_cli.py --domain example.com --country US
-
-    # search for target app id
-    chiasmodon_cli.py --app com.example
-
+    chiasmodon_cli.py --domain example.com --all 
+    
+    # Search for target domain, you will see the result for only this "example.com" on United States 
+    chiasmodon_cli.py --domain example.com --country US 
+
+    # Search for related companies by domain
+    chiasmodon_cli.py --domain example.com --related
+
+    # search for target app id 
+    chiasmodon_cli.py --app com.example 
+    
     # Search for target asn
     chiasmodon_cli.py --asn AS123 --type-view cred
 
     # Search for target username
     chiasmodon_cli.py --username someone --country CA
 
     # Search for target password
@@ -120,28 +132,28 @@
     # Search for target endpoint
     chiasmodon_cli.py --endpoint /wp-login.php
 
     # Search for target cidr
     chiasmodon_cli.py --cidr x.x.x.x/24
 
     # Search for target creds by domain emsils
-    chiasmodon_cli.py --domain example.com --domain-emails
+    chiasmodon_cli.py --domain example.com --domain-emails 
     chiasmodon_cli.py --domain example.com --domain-emails --output example-creds.json --output-type json
     chiasmodon_cli.py --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
-
+    
     # Search for target subdomain
     chiasmodon_cli.py --domain company.com --view-type subdomain
-
+    
     # Search for target email
-    chiasmodon_cli.py --email someone@example.com
-    chiasmodon_cli.py --email someone@example.com --view-type url
+    chiasmodon_cli.py --email someone@example.com  
+    chiasmodon_cli.py --email someone@example.com --view-type url 
 
-    # search for multiple targets:
-    chiasmodon_cli.py --domain targets.txt --output example-creds.txt
-    chiasmodon_cli.py --domain targets.txt --view-type url --output example-urls.txt
+    # search for multiple targets: 
+    chiasmodon_cli.py --domain targets.txt --output example-creds.txt 
+    chiasmodon_cli.py --domain targets.txt --view-type url --output example-urls.txt 
 ```
 
 ***How to use pychiasmodon library***:
 ```python
 from pychiasmodon import Chiasmodon as ch 
 token = "PUT_HERE_YOUR_API_KEY"
 obj = ch(token)
```

### Comparing `chiasmodon-1.1.6/README.md` & `chiasmodon-1.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,66 +40,78 @@
 pip install chiasmodon
 ```
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
 
 
 ```
-usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-C COUNTRY]
-                         [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT]
-                         [-L LIMIT] [-v]
+usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-n ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-s] [-sc SCAN_CLIENTS]
+                         [-se SCAN_EMPLOYEES] [-C COUNTRY] [-A] [-de] [-r] [-o OUTPUT] [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}]
+                         [-ot {text,json,csv}] [--init INIT] [-T TIMEOUT] [-L LIMIT] [-v]
 
 Chiasmodon CLI
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Search by domain.
   -a APP, --app APP     Search by google play applciton id.
   -c CIDR, --cidr CIDR  Search by CIDR.
-  -s ASN, --asn ASN     Search by ASN.
+  -n ASN, --asn ASN     Search by ASN.
   -e EMAIL, --email EMAIL
                         Search by email, only pro, only pro account.
   -u USERNAME, --username USERNAME
                         Search by username, only pro account.
   -p PASSWORD, --password PASSWORD
                         Search by password, only pro account.
   -ep ENDPOINT, --endpoint ENDPOINT
                         Search by url endpoint.
+  -s, --scan            scan the company domain (Related company, Clients, Employees, Company ASNs, Company Apps).
+  -sc SCAN_CLIENTS, --scan-clients SCAN_CLIENTS
+                        Run clients scan, default is yes, Ex: -sc no
+  -se SCAN_EMPLOYEES, --scan-employees SCAN_EMPLOYEES
+                        Run employees scan, default is yes, Ex: -se no
   -C COUNTRY, --country COUNTRY
                         sort result by country code default is all
-  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
-                        type view the result default is "cred".
+  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
+  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
+  -r, --related         Get related company domains,this option work only with (-d or --domain), default False
   -o OUTPUT, --output OUTPUT
                         filename to save the result
+  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
+                        type view the result default is "cred".
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
-  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
-  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
   -T TIMEOUT, --timeout TIMEOUT
                         request timeout default is 60.
   -L LIMIT, --limit LIMIT
                         limit results default is 10000.
   -v, --version         version.
 
 Examples:
 
-    # Search for target domain, you will see the result for only this "example.com"
-    chiasmodon_cli.py --domain example.com
+    # Scan company by domain
+    chiasmodon_cli.py --domain example.com --scan
 
+    # Search for target domain, you will see the result for only this "example.com" 
+    chiasmodon_cli.py --domain example.com 
+    
     # Search for target subdomains
-    chiasmodon_cli.py --domain example.com --all
-
-    # Search for target domain, you will see the result for only this "example.com" on United States
-    chiasmodon_cli.py --domain example.com --country US
-
-    # search for target app id
-    chiasmodon_cli.py --app com.example
-
+    chiasmodon_cli.py --domain example.com --all 
+    
+    # Search for target domain, you will see the result for only this "example.com" on United States 
+    chiasmodon_cli.py --domain example.com --country US 
+
+    # Search for related companies by domain
+    chiasmodon_cli.py --domain example.com --related
+
+    # search for target app id 
+    chiasmodon_cli.py --app com.example 
+    
     # Search for target asn
     chiasmodon_cli.py --asn AS123 --type-view cred
 
     # Search for target username
     chiasmodon_cli.py --username someone --country CA
 
     # Search for target password
@@ -108,28 +120,28 @@
     # Search for target endpoint
     chiasmodon_cli.py --endpoint /wp-login.php
 
     # Search for target cidr
     chiasmodon_cli.py --cidr x.x.x.x/24
 
     # Search for target creds by domain emsils
-    chiasmodon_cli.py --domain example.com --domain-emails
+    chiasmodon_cli.py --domain example.com --domain-emails 
     chiasmodon_cli.py --domain example.com --domain-emails --output example-creds.json --output-type json
     chiasmodon_cli.py --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
-
+    
     # Search for target subdomain
     chiasmodon_cli.py --domain company.com --view-type subdomain
-
+    
     # Search for target email
-    chiasmodon_cli.py --email someone@example.com
-    chiasmodon_cli.py --email someone@example.com --view-type url
+    chiasmodon_cli.py --email someone@example.com  
+    chiasmodon_cli.py --email someone@example.com --view-type url 
 
-    # search for multiple targets:
-    chiasmodon_cli.py --domain targets.txt --output example-creds.txt
-    chiasmodon_cli.py --domain targets.txt --view-type url --output example-urls.txt
+    # search for multiple targets: 
+    chiasmodon_cli.py --domain targets.txt --output example-creds.txt 
+    chiasmodon_cli.py --domain targets.txt --view-type url --output example-urls.txt 
 ```
 
 ***How to use pychiasmodon library***:
 ```python
 from pychiasmodon import Chiasmodon as ch 
 token = "PUT_HERE_YOUR_API_KEY"
 obj = ch(token)
```

### Comparing `chiasmodon-1.1.6/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.7/chiasmodon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.6
+Version: 1.1.7
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -52,66 +52,78 @@
 pip install chiasmodon
 ```
 ## 💻Usage
 Chiasmodon provides a flexible and user-friendly command-line interface and python library. Here are some examples to demonstrate its usage:
 
 
 ```
-usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-s ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-C COUNTRY]
-                         [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}] [-o OUTPUT] [-ot {text,json,csv}] [--init INIT] [-A] [-de] [-T TIMEOUT]
-                         [-L LIMIT] [-v]
+usage: chiasmodon_cli.py [-h] [-d DOMAIN] [-a APP] [-c CIDR] [-n ASN] [-e EMAIL] [-u USERNAME] [-p PASSWORD] [-ep ENDPOINT] [-s] [-sc SCAN_CLIENTS]
+                         [-se SCAN_EMPLOYEES] [-C COUNTRY] [-A] [-de] [-r] [-o OUTPUT] [-vt {cred,url,subdomain,email,password,username,app,endpoint,port}]
+                         [-ot {text,json,csv}] [--init INIT] [-T TIMEOUT] [-L LIMIT] [-v]
 
 Chiasmodon CLI
 
 options:
   -h, --help            show this help message and exit
   -d DOMAIN, --domain DOMAIN
                         Search by domain.
   -a APP, --app APP     Search by google play applciton id.
   -c CIDR, --cidr CIDR  Search by CIDR.
-  -s ASN, --asn ASN     Search by ASN.
+  -n ASN, --asn ASN     Search by ASN.
   -e EMAIL, --email EMAIL
                         Search by email, only pro, only pro account.
   -u USERNAME, --username USERNAME
                         Search by username, only pro account.
   -p PASSWORD, --password PASSWORD
                         Search by password, only pro account.
   -ep ENDPOINT, --endpoint ENDPOINT
                         Search by url endpoint.
+  -s, --scan            scan the company domain (Related company, Clients, Employees, Company ASNs, Company Apps).
+  -sc SCAN_CLIENTS, --scan-clients SCAN_CLIENTS
+                        Run clients scan, default is yes, Ex: -sc no
+  -se SCAN_EMPLOYEES, --scan-employees SCAN_EMPLOYEES
+                        Run employees scan, default is yes, Ex: -se no
   -C COUNTRY, --country COUNTRY
                         sort result by country code default is all
-  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
-                        type view the result default is "cred".
+  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
+  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
+  -r, --related         Get related company domains,this option work only with (-d or --domain), default False
   -o OUTPUT, --output OUTPUT
                         filename to save the result
+  -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
+                        type view the result default is "cred".
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
-  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
-  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
   -T TIMEOUT, --timeout TIMEOUT
                         request timeout default is 60.
   -L LIMIT, --limit LIMIT
                         limit results default is 10000.
   -v, --version         version.
 
 Examples:
 
-    # Search for target domain, you will see the result for only this "example.com"
-    chiasmodon_cli.py --domain example.com
+    # Scan company by domain
+    chiasmodon_cli.py --domain example.com --scan
 
+    # Search for target domain, you will see the result for only this "example.com" 
+    chiasmodon_cli.py --domain example.com 
+    
     # Search for target subdomains
-    chiasmodon_cli.py --domain example.com --all
-
-    # Search for target domain, you will see the result for only this "example.com" on United States
-    chiasmodon_cli.py --domain example.com --country US
-
-    # search for target app id
-    chiasmodon_cli.py --app com.example
-
+    chiasmodon_cli.py --domain example.com --all 
+    
+    # Search for target domain, you will see the result for only this "example.com" on United States 
+    chiasmodon_cli.py --domain example.com --country US 
+
+    # Search for related companies by domain
+    chiasmodon_cli.py --domain example.com --related
+
+    # search for target app id 
+    chiasmodon_cli.py --app com.example 
+    
     # Search for target asn
     chiasmodon_cli.py --asn AS123 --type-view cred
 
     # Search for target username
     chiasmodon_cli.py --username someone --country CA
 
     # Search for target password
@@ -120,28 +132,28 @@
     # Search for target endpoint
     chiasmodon_cli.py --endpoint /wp-login.php
 
     # Search for target cidr
     chiasmodon_cli.py --cidr x.x.x.x/24
 
     # Search for target creds by domain emsils
-    chiasmodon_cli.py --domain example.com --domain-emails
+    chiasmodon_cli.py --domain example.com --domain-emails 
     chiasmodon_cli.py --domain example.com --domain-emails --output example-creds.json --output-type json
     chiasmodon_cli.py --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
-
+    
     # Search for target subdomain
     chiasmodon_cli.py --domain company.com --view-type subdomain
-
+    
     # Search for target email
-    chiasmodon_cli.py --email someone@example.com
-    chiasmodon_cli.py --email someone@example.com --view-type url
+    chiasmodon_cli.py --email someone@example.com  
+    chiasmodon_cli.py --email someone@example.com --view-type url 
 
-    # search for multiple targets:
-    chiasmodon_cli.py --domain targets.txt --output example-creds.txt
-    chiasmodon_cli.py --domain targets.txt --view-type url --output example-urls.txt
+    # search for multiple targets: 
+    chiasmodon_cli.py --domain targets.txt --output example-creds.txt 
+    chiasmodon_cli.py --domain targets.txt --view-type url --output example-urls.txt 
 ```
 
 ***How to use pychiasmodon library***:
 ```python
 from pychiasmodon import Chiasmodon as ch 
 token = "PUT_HERE_YOUR_API_KEY"
 obj = ch(token)
```

### Comparing `chiasmodon-1.1.6/cli/chiasmodon_cli.py` & `chiasmodon-1.1.7/cli/chiasmodon_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
     parser.add_argument('-a','--app',           help='Search by google play applciton id.',type=str)
     parser.add_argument('-c','--cidr',          help='Search by CIDR.',type=str)
     parser.add_argument('-n','--asn',          help='Search by ASN.',type=str)
     parser.add_argument('-e','--email',         help='Search by email, only pro, only pro account.',type=str)
     parser.add_argument('-u','--username',      help='Search by username, only pro account.',type=str)
     parser.add_argument('-p','--password',      help='Search by password, only pro account.',type=str)
     parser.add_argument('-ep','--endpoint',     help='Search by url endpoint.',type=str)    
-    parser.add_argument('-s','--scan',          help='scan the company domain (Related company, Client creds, Empolye creds, Company ASNs, Company Apps).',action='store_true', default=False)
+    parser.add_argument('-s','--scan',          help='scan the company domain (Related company, Clients, Employees, Company ASNs, Company Apps).',action='store_true', default=False)
     parser.add_argument('-sc','--scan-clients', help='Run clients scan, default is yes, Ex: -sc no',type=str, default='yes')
     parser.add_argument('-se','--scan-employees',help='Run employees scan, default is yes, Ex: -se no',type=str, default='yes')
     #parser.add_argument('-fs','--full-scan',    help='',action='store_true', default=False) # "soon" 
     parser.add_argument('-C','--country',       help='sort result by country code default is all', type=str, default='all')
     parser.add_argument('-A','--all',           help='view all result using "like",this option work only with (-d or --domain),default is False', action='store_true', default=False)
     parser.add_argument('-de','--domain-emails',help='only result for company "root" domain, this option work only with (-d or --domain), default is False',action='store_true', default=False)
     parser.add_argument('-r','--related',       help='Get related company domains,this option work only with (-d or --domain), default False',action='store_true', default=False)
```

### Comparing `chiasmodon-1.1.6/pychiasmodon.py` & `chiasmodon-1.1.7/pychiasmodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner 
 
-VERSION = "1.1.6"
+VERSION = "1.1.7"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
     'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
     'subdomain':['domain'],
     'email':['domain', 'cidr', 'asn', 'app' ,'endpoint', 'phone', 'password'],
```

### Comparing `chiasmodon-1.1.6/setup.py` & `chiasmodon-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.6',
+      version='1.1.7',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

