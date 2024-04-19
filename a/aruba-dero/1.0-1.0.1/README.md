# Comparing `tmp/aruba_dero-1.0.tar.gz` & `tmp/aruba_dero-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruba_dero-1.0.tar", last modified: Wed Apr 17 07:57:45 2024, max compression
+gzip compressed data, was "aruba_dero-1.0.1.tar", last modified: Fri Apr 19 09:33:15 2024, max compression
```

## Comparing `aruba_dero-1.0.tar` & `aruba_dero-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 07:57:45.636183 aruba_dero-1.0/
--rw-rw-rw-   0        0        0     1352 2024-04-17 07:57:45.633177 aruba_dero-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      905 2024-04-17 07:35:17.000000 aruba_dero-1.0/README.md
--rw-rw-rw-   0        0        0      556 2024-04-17 07:57:26.000000 aruba_dero-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 07:57:45.636183 aruba_dero-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 07:57:45.583976 aruba_dero-1.0/src/
--rw-rw-rw-   0        0        0     3043 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/Module.py
--rw-rw-rw-   0        0        0        0 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:57:45.630175 aruba_dero-1.0/src/aruba_dero.egg-info/
--rw-rw-rw-   0        0        0     1352 2024-04-17 07:57:45.000000 aruba_dero-1.0/src/aruba_dero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2024-04-17 07:57:45.000000 aruba_dero-1.0/src/aruba_dero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 07:57:45.000000 aruba_dero-1.0/src/aruba_dero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-17 07:57:45.000000 aruba_dero-1.0/src/aruba_dero.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2024-04-17 07:57:45.000000 aruba_dero-1.0/src/aruba_dero.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2024-04-17 07:57:45.000000 aruba_dero-1.0/src/aruba_dero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2735 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:57:45.615420 aruba_dero-1.0/src/modules/
--rw-rw-rw-   0        0        0        0 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:57:45.625177 aruba_dero-1.0/src/modules/clearpass/
--rw-rw-rw-   0        0        0        0 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/modules/clearpass/__init__.py
--rw-rw-rw-   0        0        0    15624 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/modules/clearpass/clearpass.py
--rw-rw-rw-   0        0        0     1552 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/modules/clearpass/temp_webserver.py
--rw-rw-rw-   0        0        0     4802 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/modules/clearpass/utils.py
--rw-rw-rw-   0        0        0     1362 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/modules/clearpass/webserver-process.py
--rw-rw-rw-   0        0        0     2160 2024-04-17 07:35:17.000000 aruba_dero-1.0/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:33:15.233260 aruba_dero-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:33:15.233260 aruba_dero-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:33:15.233260 aruba_dero-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:33:15.229261 aruba_dero-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:33:15.229261 aruba_dero-1.0.1/src/dero-modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:33:15.233260 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:33:15.000000 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-19 09:33:15.000000 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:33:15.000000 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 09:33:15.000000 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 09:33:15.000000 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 09:33:15.000000 aruba_dero-1.0.1/src/dero-modules/aruba_dero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:33:15.233260 aruba_dero-1.0.1/src/dero-modules/clearpass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/src/dero-modules/clearpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/src/dero-modules/clearpass/clearpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/src/dero-modules/clearpass/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/src/dero-modules/clearpass/temp_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/src/dero-modules/clearpass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 09:33:08.000000 aruba_dero-1.0.1/src/dero-modules/clearpass/webserver-process.py
```

### Comparing `aruba_dero-1.0/PKG-INFO` & `aruba_dero-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,40 @@
-Metadata-Version: 2.1
-Name: aruba-dero
-Version: 1.0
-Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
-Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-Requires-Dist: pyclearpass>=1.0.4
-Requires-Dist: psutil~=5.9.8
-Requires-Dist: pyyaml~=6.0.1
-Requires-Dist: cryptography~=42.0.5
-Requires-Dist: winBullet~=1.1
-Requires-Dist: setuptools~=69.2.0
-
-# DemoRolloutHelper - Dero
-
-![Static Badge](https://img.shields.io/badge/3.12-3572a5?logo=python&logoColor=3572a5&label=Python)
-
-This repository contains the code for the DemoRolloutHelper project and its respective modules.
-The project aims to enable the automation of the rollout processes for demo environments.
-
-## Installation
-
-```shell
-pip install . --user
-dero
-```
-
-or with **Docker-Compose**:
-
-```shell
-docker compose run dero
-```
-
-> [!TIP]
-> Please refer to the docker-compose guide in the example [docker-compose.yml](example/docker-compose.yml) file.
-
-or with **Docker**:
-
-```shell
-docker build -t dero .
-docker run --rm -it likqez/aruba-dero <args>
-```
-
-> [!IMPORTANT]
-> Always refer to the respective module documentation for additional installation instructions.
-
-## Available Modules
-
-- [ClearPass Certificate Rollout](src/modules/clearpass/README.md)
-- 
+# DemoRolloutHelper - Dero
+
+![Static Badge](https://img.shields.io/badge/3.12-3572a5?logo=python&logoColor=3572a5&label=Python)
+
+This repository contains the code for the DemoRolloutHelper project and its respective modules.
+The project aims to enable the automation of the rollout processes for demo environments.
+
+## Installation
+
+```shell
+pip install aruba-dero --user
+dero
+```
+
+> [!TIP]
+> It is likely that when installed with the `--user` flag, the `dero` command is not available in your PATH.
+> In this case, add it to your PATH or use the full path to the executable.
+> Àfter opening a **NEW** terminal windows, the helper can be accessed by typing `dero`
+
+or with **Docker-Compose**:
+
+```shell
+docker compose run dero
+```
+
+> [!TIP]
+> Please refer to the docker-compose guide in the example [docker-compose.yml](example/docker-compose.yml) file.
+
+or with **Docker**:
+
+```shell
+docker run --rm -it likqez/aruba-dero <args>
+```
+
+> [!IMPORTANT]
+> Always refer to the respective module documentation for additional installation instructions.
+
+## Available Modules
+
+- [ClearPass Certificate Rollout](src/dero-modules/clearpass/README.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aruba_dero-1.0/src/aruba_dero.egg-info/PKG-INFO` & `aruba_dero-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-Metadata-Version: 2.1
-Name: aruba-dero
-Version: 1.0
-Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
-Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-Requires-Dist: pyclearpass>=1.0.4
-Requires-Dist: psutil~=5.9.8
-Requires-Dist: pyyaml~=6.0.1
-Requires-Dist: cryptography~=42.0.5
-Requires-Dist: winBullet~=1.1
-Requires-Dist: setuptools~=69.2.0
-
-# DemoRolloutHelper - Dero
-
-![Static Badge](https://img.shields.io/badge/3.12-3572a5?logo=python&logoColor=3572a5&label=Python)
-
-This repository contains the code for the DemoRolloutHelper project and its respective modules.
-The project aims to enable the automation of the rollout processes for demo environments.
-
-## Installation
-
-```shell
-pip install . --user
-dero
-```
-
-or with **Docker-Compose**:
-
-```shell
-docker compose run dero
-```
-
-> [!TIP]
-> Please refer to the docker-compose guide in the example [docker-compose.yml](example/docker-compose.yml) file.
-
-or with **Docker**:
-
-```shell
-docker build -t dero .
-docker run --rm -it likqez/aruba-dero <args>
-```
-
-> [!IMPORTANT]
-> Always refer to the respective module documentation for additional installation instructions.
-
-## Available Modules
-
-- [ClearPass Certificate Rollout](src/modules/clearpass/README.md)
-- 
+Metadata-Version: 2.1
+Name: aruba-dero
+Version: 1.0.1
+Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
+Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+Requires-Dist: pyclearpass>=1.0.4
+Requires-Dist: psutil~=5.9.8
+Requires-Dist: pyyaml~=6.0.1
+Requires-Dist: cryptography~=42.0.5
+Requires-Dist: winBullet~=1.1
+Requires-Dist: setuptools~=69.2.0
+
+# DemoRolloutHelper - Dero
+
+![Static Badge](https://img.shields.io/badge/3.12-3572a5?logo=python&logoColor=3572a5&label=Python)
+
+This repository contains the code for the DemoRolloutHelper project and its respective modules.
+The project aims to enable the automation of the rollout processes for demo environments.
+
+## Installation
+
+```shell
+pip install aruba-dero --user
+dero
+```
+
+> [!TIP]
+> It is likely that when installed with the `--user` flag, the `dero` command is not available in your PATH.
+> In this case, add it to your PATH or use the full path to the executable.
+> Àfter opening a **NEW** terminal windows, the helper can be accessed by typing `dero`
+
+or with **Docker-Compose**:
+
+```shell
+docker compose run dero
+```
+
+> [!TIP]
+> Please refer to the docker-compose guide in the example [docker-compose.yml](example/docker-compose.yml) file.
+
+or with **Docker**:
+
+```shell
+docker run --rm -it likqez/aruba-dero <args>
+```
+
+> [!IMPORTANT]
+> Always refer to the respective module documentation for additional installation instructions.
+
+## Available Modules
+
+- [ClearPass Certificate Rollout](src/dero-modules/clearpass/README.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aruba_dero-1.0/src/modules/clearpass/clearpass.py` & `aruba_dero-1.0.1/src/dero-modules/clearpass/clearpass.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-import os
-import pathlib
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
-from getpass import getpass
-
-from bullet import Check, colors, Input, Bullet
-from pyclearpass import *
-
-import utils as utils
-from Module import Module
-from .utils import *
-from .temp_webserver import TemporaryWebServer
-
-
-class ClearPassModule(Module):
-    def __init__(self):
-        # Api
-        super().__init__()
-        self.api_host: str | None = None  # E.g. https://clearpass.example.com:8080
-        self.client_id: str | None = None
-        self.client_access_token: str | None = None
-        self.verify_ssl: bool = True
-        self.client_secret: str | None = None
-        self.login = None
-        # Webserver
-        self.bind_addr: str = "127.0.0.1"
-        self.bind_port: int = 8080
-        self.serve_dir: str = "cppmCerts"
-        # Preparation & Execution
-        self.supported_server_certificates: list[str] = ["HTTPS(ECC)", "HTTPS(RSA)", "RADIUS"]
-        self.servers: list[any] | None = None
-        self.certificate: Certificate | None = None
-        self.cert_is_pkcs12 = False  # Indicating that a pkcs12 file was loaded, so no additional key file is needed
-        self.passphrase: str | None = None
-        self.server_certificate_type: str | None = None  # One of supported_server_certificates
-        # Other
-        self.run_retries: int = 0
-
-    def setup(self):
-        parser = ArgumentParser(description="Update certificate on ClearPass server",
-                                formatter_class=ArgumentDefaultsHelpFormatter)
-        parser.add_argument("--insecure", help="Ignore SSL Verification", action="store_true")
-        args = parser.parse_args()
-        config = vars(args)
-
-        self.api_host = os.environ.get("CPPM_CERT_API_HOST") or self.ask_api_host()
-        self.verify_ssl = os.environ.get("CPPM_CERT_VERIFY_SSL") or not config.get('insecure')
-        self.client_id = os.environ.get("CPPM_CERT_CLIENT_ID")
-        self.client_secret = os.environ.get("CPPM_CERT_CLIENT_SECRET")
-        self.client_access_token = os.environ.get("CPPM_CERT_API_TOKEN")
-
-        self.serve_dir = os.environ.get("CPPM_CERT_SERVE_DIR") or self.serve_dir
-        return True
-
-    def ask_api_host(self) -> str:
-        if not self.api_host:
-            print("No API host provided.")
-            return Input("Enter Api Host: ", default="https://127.0.0.1:443", word_color=colors.foreground["yellow"]).launch()
-        return self.api_host
-
-    def has_credentials(self) -> bool:
-        return bool(self.client_id and self.client_secret) or bool(self.client_access_token)
-
-    def ask_credentials(self):
-        if self.client_id:
-            print(f"Client ID found: {self.client_id}")
-            self.client_secret = getpass(prompt="Please enter client secret: ", stream=None)
-        else:
-            self.client_access_token = getpass(prompt="Enter client access token: ", stream=None)
-        return self.client_access_token or self.client_secret
-
-    def pre_run(self):
-        if self.client_access_token:
-            self.login = ClearPassAPILogin(server=f"{self.api_host}/api",
-                                           api_token=f"{self.client_access_token}",
-                                           verify_ssl=self.verify_ssl)
-        else:
-            self.login = ClearPassAPILogin(server=f"{self.api_host}/api",
-                                           granttype="client_credentials",
-                                           clientsecret=f"{self.client_secret}", clientid=f"{self.client_id}",
-                                           verify_ssl=self.verify_ssl)
-        if not self.test_login():
-            return False
-
-        print("Retrieving cluster servers...")
-        servers = self.collect_cluster_servers()
-        self.select_servers(servers)
-        if len(self.servers) == 0:
-            print("No servers selected. Exiting...")
-            return False
-
-        # Check if the certificate is already installed
-        self.check_current_certificates()
-
-        # Prompt user to select network interface to bind webserver to
-        self.select_bind_address()
-
-        # Make sure the root directory exists and is not empty
-        return self.prepare_srv_directory()
-
-    def run(self):
-        certificate_file = utils.cli_file_picker("Select the certificate: ", root_path=self.serve_dir,
-                                                 current_path=self.serve_dir)
-        if certificate_file is None:
-            print("Cannot select file. Exiting...")
-            return False
-
-        # Check if the selected file is a valid certificate file / PEM/DER
-        _, certificate = check_cert_and_convert_to_pem(certificate_file)
-        if not certificate:
-            # Check for PKCS12 file
-            print("Selected file might be a PKCS12 file. Please provide the passphrase. Press Enter to skip.")
-            self.passphrase = getpass(prompt="Enter passphrase: ", stream=None)
-            _, certificate = pkcs12_to_pem(certificate_file, self.passphrase)
-
-            if not certificate:
-                print("\nInvalid certificate file or wrong passphrase. Try again.")
-                self.retry()
-            else:
-                print("PKCS12 file loaded successfully.")
-                #todo grab key format
-                self.cert_is_pkcs12 = True
-
-        self.reset_retries()
-        self.certificate = certificate
-
-        if not self.cert_is_pkcs12:
-            key_file = utils.cli_file_picker("Select the certificate key: ", root_path=self.serve_dir,
-                                             current_path=self.serve_dir)
-            _, private_key = check_key_and_convert_to_pem(key_file)
-
-            if not private_key:
-                print("Invalid key file. Try again.")
-                self.retry()
-
-            if not private_key.public_key() == self.certificate.public_key():
-                print("Certificate and key do not match. Try again.")
-                self.retry()
-
-            print("Certificate and key match.")
-            print("Bundling into PKCS12 file...")
-
-            if not self.passphrase:
-                print("Creating PKCS12 file. Please provide the passphrase.")
-                self.passphrase = getpass(prompt="Enter passphrase: ", stream=None)
-
-            _, p12_data = bundle_pkcs12(self.certificate, private_key, self.passphrase)
-
-            p12_file = f"{os.path.splitext(certificate_file)[0]}.p12"
-            with open(p12_file, "wb") as file:
-                file.write(p12_data)
-            key_file = p12_file
-
-            if isinstance(private_key, RSAPrivateKey):
-                self.supported_server_certificates.remove("HTTPS(ECC)")
-            elif isinstance(private_key, EllipticCurvePrivateKey):
-                self.supported_server_certificates.remove("HTTPS(RSA)")
-
-        else:
-            key_file = certificate_file
-
-        self.select_certificate_type()
-
-        if not self.servers:
-            print("No servers selected. Aborting...")
-            return False
-
-        with TemporaryWebServer(self.bind_port, self.bind_addr, self.serve_dir) as webserver:
-
-            if not webserver.process:
-                print("Failed to start webserver. Exiting...")
-                return False
-
-            if webserver.host == "0.0.0.0":
-
-                webhost = os.environ.get("CPPM_CERT_SERVE_HOST") or Input("Enter host ip: ", default=f"{utils.get_net_ifaces()[-1].get("ip4")}", word_color=colors.foreground["yellow"]).launch()
-                webhost += f":{webserver.port}"
-            else:
-                webhost = f"https://{webserver.host}:{webserver.port}"
-
-            print(f"Serving on http://{webserver.host}:{webserver.port}...")
-
-            body = {
-                "certificate_url": f"http://{webhost}/{pathlib.PurePath(os.path.relpath(certificate_file, start=self.serve_dir)).as_posix()}",
-                "pkcs12_file_url": f"http://{webhost}/{pathlib.PurePath(os.path.relpath(key_file, start=self.serve_dir)).as_posix()}",
-                "pkcs12_passphrase": f"{self.passphrase}",
-            }
-
-            if not self.server_certificate_type:
-                print("No certificate type selected. Aborting...")
-                return False
-
-            for server in self.servers:
-                res = ApiPlatformCertificates.replace_server_cert_name_by_server_uuid_service_name(self.login,
-                                                                                                   server_uuid=server[
-                                                                                                       'server_uuid'],
-                                                                                                   service_name=self.server_certificate_type,
-                                                                                                   body=body)
-                if res.get("status") and res["status"] != 200:
-                    print(
-                        f"Failed to update certificate on {server.get("name")}: {res.get("status")} {res.get("title")}: {res.get("validation_messages")}")
-                    print("\n!!This module is not performing a rollback. Please check the server manually!!")
-                    print("!!This module is not performing a rollback. Please check the server manually!!")
-                    print("!!This module is not performing a rollback. Please check the server manually!!\n")
-                    return False
-                else:
-                    print(f"Updated certificate on {server.get("name")} successfully. Expiring at {res.get("expiry_date")}")
-                    # Todo. maybe add link to download ics to renew in time?
-        return True
-
-    def post_run(self):
-        return True
-
-    def test_login(self) -> bool:
-        print("\nTrying to login...")
-        try:
-            res = ApiApiOperations.get_oauth_me(self.login)
-            if res.get('status') or not res.get('info'):
-                print(f"Failed to login: {res.get("status")}: {res.get("detail")}")
-                return False
-            print(f"Logged in as {res.get("info")}")
-            return True
-        except Exception as e:
-            print(f"Failed to login: {e}")
-            return False
-
-    def collect_cluster_servers(self):
-        # Collect all instances managed on api host
-        cluster_res = ApiLocalServerConfiguration.get_cluster_server(self.login)
-        # TODO: Response Validation, maybe json schema?
-        servers = []
-        for item in cluster_res['_embedded']['items']:
-            servers.append({"server_uuid": item.get("server_uuid"), "name": item.get("name"), "fqdn": item.ger("fqdn")})
-        return servers
-
-    def select_certificate_type(self) -> str:
-        choices = self.supported_server_certificates
-        if len(choices) == 1:
-            return choices[0]
-
-        cli = Bullet(
-            prompt="Select certificate type to update:",
-            choices=choices,
-            indent=0,
-            align=5,
-            margin=2,
-            bullet="*",
-            bullet_color=colors.bright(colors.foreground["cyan"]),
-            word_color=colors.bright(colors.foreground["yellow"]),
-            word_on_switch=colors.bright(colors.foreground["yellow"]),
-            background_color=colors.background["black"],
-            background_on_switch=colors.background["black"],
-            pad_right=5,
-            return_index=True
-        )
-        cert_type = cli.launch()
-        self.server_certificate_type = choices[cert_type[1]]
-
-    def select_servers(self, all_servers: list) -> None:
-        choices = [f"{server.get("name")}-{server.get("fqdn")}" for server in all_servers]
-        cli = Check(
-            prompt="Select servers to update certificates:",
-            choices=choices,
-            check="*",
-            margin=2,
-            check_color=colors.bright(colors.foreground["yellow"]),
-            check_on_switch=colors.bright(colors.foreground["yellow"]),
-            background_color=colors.background["black"],
-            background_on_switch=colors.background["white"],
-            word_color=colors.foreground["white"],
-            word_on_switch=colors.foreground["black"],
-            return_index=True
-        )
-        servers = cli.launch()
-        self.servers = [all_servers[i] for i in servers[1]]
-
-    def select_bind_address(self) -> None:
-        # Get available network interfaces
-        available_ifaces = utils.get_net_ifaces()
-        available_ifaces.append({"name": "‼ All interfaces ‼", "ip4": "0.0.0.0", "ip6": "::"})
-
-        # Select network interface to bind webserver to
-        cli = Bullet(
-            prompt="Select network interface to bind the webserver to:",
-            choices=[f"{iface.get('name') or 'Unknown'} : {iface.get('ip4')} - {iface.get('ip6')}" for iface in
-                     available_ifaces],
-            indent=0,
-            align=5,
-            margin=2,
-            bullet="*",
-            bullet_color=colors.bright(colors.foreground["cyan"]),
-            word_color=colors.bright(colors.foreground["yellow"]),
-            word_on_switch=colors.bright(colors.foreground["yellow"]),
-            background_color=colors.background["black"],
-            background_on_switch=colors.background["black"],
-            pad_right=5,
-            return_index=True
-        )
-        selected_iface = cli.launch()
-
-        selected_iface = available_ifaces[selected_iface[1]]
-        bind_addr = selected_iface.get('ip4') or "0.0.0.0"
-
-        bind_port = Input("Enter bind port: ", default="8080", word_color=colors.foreground["yellow"]).launch()
-        self.bind_addr = bind_addr
-        self.bind_port = bind_port
-
-    def prepare_srv_directory(self) -> bool:
-        print("\n")
-        if not os.path.exists(self.serve_dir):
-            os.mkdir(self.serve_dir)
-            print(f"Created directory: {self.serve_dir}")
-        if len(os.listdir(self.serve_dir)) == 0:
-            print(f"Directory {self.serve_dir} is empty.")
-            print("Please place the certificate and key files in the directory and press Enter to continue.")
-            try:
-                input("Press Enter to continue...")
-            except EOFError:
-                pass
-            if len(os.listdir(self.serve_dir)) == 0:
-                print("Still no files found.")
-                return False
-        return True
-
-    def check_current_certificates(self) -> None:
-        print("\nChecking current certificates...")
-        for server in self.servers:
-            server_uuid = server.get("server_uuid")
-            for cert_type in self.supported_server_certificates:
-                res = ApiPlatformCertificates.get_server_cert_name_by_server_uuid_service_name(self.login,
-                                                                                               server_uuid=server_uuid,
-                                                                                               service_name=cert_type)
-                pass  # todo check current certificate
-
-    def retry(self):
-        allowed = self.run_retries < 3
-        if allowed:
-            self.run_retries += 1
-            return self.run()
-        return False
-
-    def reset_retries(self):
-        self.run_retries = 0
+import os
+import pathlib
+from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
+from getpass import getpass
+
+from bullet import Check, colors, Input, Bullet
+from pyclearpass import *
+
+import utils as utils
+from Module import Module
+from .utils import *
+from .temp_webserver import TemporaryWebServer
+
+
+class ClearPassModule(Module):
+    def __init__(self):
+        # Api
+        super().__init__()
+        self.api_host: str | None = None  # E.g. https://clearpass.example.com:8080
+        self.client_id: str | None = None
+        self.client_access_token: str | None = None
+        self.verify_ssl: bool = True
+        self.client_secret: str | None = None
+        self.login = None
+        # Webserver
+        self.bind_addr: str = "127.0.0.1"
+        self.bind_port: int = 8080
+        self.serve_dir: str = "cppmCerts"
+        # Preparation & Execution
+        self.supported_server_certificates: list[str] = ["HTTPS(ECC)", "HTTPS(RSA)", "RADIUS"]
+        self.servers: list[any] | None = None
+        self.certificate: Certificate | None = None
+        self.cert_is_pkcs12 = False  # Indicating that a pkcs12 file was loaded, so no additional key file is needed
+        self.passphrase: str | None = None
+        self.server_certificate_type: str | None = None  # One of supported_server_certificates
+        # Other
+        self.run_retries: int = 0
+
+    def setup(self):
+        parser = ArgumentParser(description="Update certificate on ClearPass server",
+                                formatter_class=ArgumentDefaultsHelpFormatter)
+        parser.add_argument("--insecure", help="Ignore SSL Verification", action="store_true")
+        args = parser.parse_args()
+        config = vars(args)
+
+        self.api_host = os.environ.get("CPPM_CERT_API_HOST") or self.ask_api_host()
+        self.verify_ssl = os.environ.get("CPPM_CERT_VERIFY_SSL") or not config.get('insecure')
+        self.client_id = os.environ.get("CPPM_CERT_CLIENT_ID")
+        self.client_secret = os.environ.get("CPPM_CERT_CLIENT_SECRET")
+        self.client_access_token = os.environ.get("CPPM_CERT_API_TOKEN")
+
+        self.serve_dir = os.environ.get("CPPM_CERT_SERVE_DIR") or self.serve_dir
+        return True
+
+    def ask_api_host(self) -> str:
+        if not self.api_host:
+            print("No API host provided.")
+            return Input("Enter Api Host: ", default="https://127.0.0.1:443", word_color=colors.foreground["yellow"]).launch()
+        return self.api_host
+
+    def has_credentials(self) -> bool:
+        return bool(self.client_id and self.client_secret) or bool(self.client_access_token)
+
+    def ask_credentials(self):
+        if self.client_id:
+            print(f"Client ID found: {self.client_id}")
+            self.client_secret = getpass(prompt="Please enter client secret: ", stream=None)
+        else:
+            self.client_access_token = getpass(prompt="Enter client access token: ", stream=None)
+        return self.client_access_token or self.client_secret
+
+    def pre_run(self):
+        if self.client_access_token:
+            self.login = ClearPassAPILogin(server=f"{self.api_host}/api",
+                                           api_token=f"{self.client_access_token}",
+                                           verify_ssl=self.verify_ssl)
+        else:
+            self.login = ClearPassAPILogin(server=f"{self.api_host}/api",
+                                           granttype="client_credentials",
+                                           clientsecret=f"{self.client_secret}", clientid=f"{self.client_id}",
+                                           verify_ssl=self.verify_ssl)
+        if not self.test_login():
+            return False
+
+        print("Retrieving cluster servers...")
+        servers = self.collect_cluster_servers()
+        self.select_servers(servers)
+        if len(self.servers) == 0:
+            print("No servers selected. Exiting...")
+            return False
+
+        # Check if the certificate is already installed
+        self.check_current_certificates()
+
+        # Prompt user to select network interface to bind webserver to
+        self.select_bind_address()
+
+        # Make sure the root directory exists and is not empty
+        return self.prepare_srv_directory()
+
+    def run(self):
+        certificate_file = utils.cli_file_picker("Select the certificate: ", root_path=self.serve_dir,
+                                                 current_path=self.serve_dir)
+        if certificate_file is None:
+            print("Cannot select file. Exiting...")
+            return False
+
+        # Check if the selected file is a valid certificate file / PEM/DER
+        _, certificate = check_cert_and_convert_to_pem(certificate_file)
+        if not certificate:
+            # Check for PKCS12 file
+            print("Selected file might be a PKCS12 file. Please provide the passphrase. Press Enter to skip.")
+            self.passphrase = getpass(prompt="Enter passphrase: ", stream=None)
+            _, certificate = pkcs12_to_pem(certificate_file, self.passphrase)
+
+            if not certificate:
+                print("\nInvalid certificate file or wrong passphrase. Try again.")
+                self.retry()
+            else:
+                print("PKCS12 file loaded successfully.")
+                #todo grab key format
+                self.cert_is_pkcs12 = True
+
+        self.reset_retries()
+        self.certificate = certificate
+
+        if not self.cert_is_pkcs12:
+            key_file = utils.cli_file_picker("Select the certificate key: ", root_path=self.serve_dir,
+                                             current_path=self.serve_dir)
+            _, private_key = check_key_and_convert_to_pem(key_file)
+
+            if not private_key:
+                print("Invalid key file. Try again.")
+                self.retry()
+
+            if not private_key.public_key() == self.certificate.public_key():
+                print("Certificate and key do not match. Try again.")
+                self.retry()
+
+            print("Certificate and key match.")
+            print("Bundling into PKCS12 file...")
+
+            if not self.passphrase:
+                print("Creating PKCS12 file. Please provide the passphrase.")
+                self.passphrase = getpass(prompt="Enter passphrase: ", stream=None)
+
+            _, p12_data = bundle_pkcs12(self.certificate, private_key, self.passphrase)
+
+            p12_file = f"{os.path.splitext(certificate_file)[0]}.p12"
+            with open(p12_file, "wb") as file:
+                file.write(p12_data)
+            key_file = p12_file
+
+            if isinstance(private_key, RSAPrivateKey):
+                self.supported_server_certificates.remove("HTTPS(ECC)")
+            elif isinstance(private_key, EllipticCurvePrivateKey):
+                self.supported_server_certificates.remove("HTTPS(RSA)")
+
+        else:
+            key_file = certificate_file
+
+        self.select_certificate_type()
+
+        if not self.servers:
+            print("No servers selected. Aborting...")
+            return False
+
+        with TemporaryWebServer(self.bind_port, self.bind_addr, self.serve_dir) as webserver:
+
+            if not webserver.process:
+                print("Failed to start webserver. Exiting...")
+                return False
+
+            if webserver.host == "0.0.0.0":
+
+                webhost = os.environ.get("CPPM_CERT_SERVE_HOST") or Input("Enter host ip: ", default=f"{utils.get_net_ifaces()[-1].get("ip4")}", word_color=colors.foreground["yellow"]).launch()
+                webhost += f":{webserver.port}"
+            else:
+                webhost = f"https://{webserver.host}:{webserver.port}"
+
+            print(f"Serving on http://{webserver.host}:{webserver.port}...")
+
+            body = {
+                "certificate_url": f"http://{webhost}/{pathlib.PurePath(os.path.relpath(certificate_file, start=self.serve_dir)).as_posix()}",
+                "pkcs12_file_url": f"http://{webhost}/{pathlib.PurePath(os.path.relpath(key_file, start=self.serve_dir)).as_posix()}",
+                "pkcs12_passphrase": f"{self.passphrase}",
+            }
+
+            if not self.server_certificate_type:
+                print("No certificate type selected. Aborting...")
+                return False
+
+            for server in self.servers:
+                res = ApiPlatformCertificates.replace_server_cert_name_by_server_uuid_service_name(self.login,
+                                                                                                   server_uuid=server[
+                                                                                                       'server_uuid'],
+                                                                                                   service_name=self.server_certificate_type,
+                                                                                                   body=body)
+                if res.get("status") and res["status"] != 200:
+                    print(
+                        f"Failed to update certificate on {server.get("name")}: {res.get("status")} {res.get("title")}: {res.get("validation_messages")}")
+                    print("\n!!This module is not performing a rollback. Please check the server manually!!")
+                    print("!!This module is not performing a rollback. Please check the server manually!!")
+                    print("!!This module is not performing a rollback. Please check the server manually!!\n")
+                    return False
+                else:
+                    print(f"Updated certificate on {server.get("name")} successfully. Expiring at {res.get("expiry_date")}")
+                    # Todo. maybe add link to download ics to renew in time?
+        return True
+
+    def post_run(self):
+        return True
+
+    def test_login(self) -> bool:
+        print("\nTrying to login...")
+        try:
+            res = ApiApiOperations.get_oauth_me(self.login)
+            if res.get('status') or not res.get('info'):
+                print(f"Failed to login: {res.get("status")}: {res.get("detail")}")
+                return False
+            print(f"Logged in as {res.get("info")}")
+            return True
+        except Exception as e:
+            print(f"Failed to login: {e}")
+            return False
+
+    def collect_cluster_servers(self):
+        # Collect all instances managed on api host
+        cluster_res = ApiLocalServerConfiguration.get_cluster_server(self.login)
+        # TODO: Response Validation, maybe json schema?
+        servers = []
+        for item in cluster_res['_embedded']['items']:
+            servers.append({"server_uuid": item.get("server_uuid"), "name": item.get("name"), "fqdn": item.ger("fqdn")})
+        return servers
+
+    def select_certificate_type(self) -> str:
+        choices = self.supported_server_certificates
+        if len(choices) == 1:
+            return choices[0]
+
+        cli = Bullet(
+            prompt="Select certificate type to update:",
+            choices=choices,
+            indent=0,
+            align=5,
+            margin=2,
+            bullet="*",
+            bullet_color=colors.bright(colors.foreground["cyan"]),
+            word_color=colors.bright(colors.foreground["yellow"]),
+            word_on_switch=colors.bright(colors.foreground["yellow"]),
+            background_color=colors.background["black"],
+            background_on_switch=colors.background["black"],
+            pad_right=5,
+            return_index=True
+        )
+        cert_type = cli.launch()
+        self.server_certificate_type = choices[cert_type[1]]
+
+    def select_servers(self, all_servers: list) -> None:
+        choices = [f"{server.get("name")}-{server.get("fqdn")}" for server in all_servers]
+        cli = Check(
+            prompt="Select servers to update certificates:",
+            choices=choices,
+            check="*",
+            margin=2,
+            check_color=colors.bright(colors.foreground["yellow"]),
+            check_on_switch=colors.bright(colors.foreground["yellow"]),
+            background_color=colors.background["black"],
+            background_on_switch=colors.background["white"],
+            word_color=colors.foreground["white"],
+            word_on_switch=colors.foreground["black"],
+            return_index=True
+        )
+        servers = cli.launch()
+        self.servers = [all_servers[i] for i in servers[1]]
+
+    def select_bind_address(self) -> None:
+        # Get available network interfaces
+        available_ifaces = utils.get_net_ifaces()
+        available_ifaces.append({"name": "‼ All interfaces ‼", "ip4": "0.0.0.0", "ip6": "::"})
+
+        # Select network interface to bind webserver to
+        cli = Bullet(
+            prompt="Select network interface to bind the webserver to:",
+            choices=[f"{iface.get('name') or 'Unknown'} : {iface.get('ip4')} - {iface.get('ip6')}" for iface in
+                     available_ifaces],
+            indent=0,
+            align=5,
+            margin=2,
+            bullet="*",
+            bullet_color=colors.bright(colors.foreground["cyan"]),
+            word_color=colors.bright(colors.foreground["yellow"]),
+            word_on_switch=colors.bright(colors.foreground["yellow"]),
+            background_color=colors.background["black"],
+            background_on_switch=colors.background["black"],
+            pad_right=5,
+            return_index=True
+        )
+        selected_iface = cli.launch()
+
+        selected_iface = available_ifaces[selected_iface[1]]
+        bind_addr = selected_iface.get('ip4') or "0.0.0.0"
+
+        bind_port = Input("Enter bind port: ", default="8080", word_color=colors.foreground["yellow"]).launch()
+        self.bind_addr = bind_addr
+        self.bind_port = bind_port
+
+    def prepare_srv_directory(self) -> bool:
+        print("\n")
+        if not os.path.exists(self.serve_dir):
+            os.mkdir(self.serve_dir)
+            print(f"Created directory: {self.serve_dir}")
+        if len(os.listdir(self.serve_dir)) == 0:
+            print(f"Directory {self.serve_dir} is empty.")
+            print("Please place the certificate and key files in the directory and press Enter to continue.")
+            try:
+                input("Press Enter to continue...")
+            except EOFError:
+                pass
+            if len(os.listdir(self.serve_dir)) == 0:
+                print("Still no files found.")
+                return False
+        return True
+
+    def check_current_certificates(self) -> None:
+        print("\nChecking current certificates...")
+        for server in self.servers:
+            server_uuid = server.get("server_uuid")
+            for cert_type in self.supported_server_certificates:
+                res = ApiPlatformCertificates.get_server_cert_name_by_server_uuid_service_name(self.login,
+                                                                                               server_uuid=server_uuid,
+                                                                                               service_name=cert_type)
+                pass  # todo check current certificate
+
+    def retry(self):
+        allowed = self.run_retries < 3
+        if allowed:
+            self.run_retries += 1
+            return self.run()
+        return False
+
+    def reset_retries(self):
+        self.run_retries = 0
```

### Comparing `aruba_dero-1.0/src/modules/clearpass/temp_webserver.py` & `aruba_dero-1.0.1/src/dero-modules/clearpass/temp_webserver.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import errno
-import os
-import subprocess
-
-
-class TemporaryWebServer:
-    def __init__(self, port: int = 8080, host: str = "127.0.0.1", serv_dir: str = ""):
-        self.port = port
-        self.host = host
-        self.serv_dir = serv_dir
-        self.process: subprocess.Popen[bytes] | None = None
-        pass
-
-    def __enter__(self):
-        self.process = self.start_webserver()
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.stop_webserver()
-
-    def start_webserver(self) -> subprocess.Popen[bytes] | None:
-        if self.serv_dir is None:
-            return None
-        try:
-            webserver_exec_path = os.path.join(os.path.dirname(__file__), "webserver-process.py")
-            process = subprocess.Popen(["python", f"{webserver_exec_path}", f"{self.host}", f"{self.port}", "-D", f"{self.serv_dir}"],
-                                       stdout=subprocess.DEVNULL,
-                                       stderr=subprocess.DEVNULL)
-            return process
-        except OSError as e:
-            if e.errno == errno.EADDRINUSE:
-                print(f"Port {self.port} already in use. Incrementing..")
-                self.port += 1
-                self.start_webserver()
-            else:
-                print(f"Failed to start webserver: {e}")
-        return None
-
-    def stop_webserver(self):
-        if self.process:
-            try:
-                self.process.kill()
-            except ProcessLookupError as e:
-                return
+import errno
+import os
+import subprocess
+
+
+class TemporaryWebServer:
+    def __init__(self, port: int = 8080, host: str = "127.0.0.1", serv_dir: str = ""):
+        self.port = port
+        self.host = host
+        self.serv_dir = serv_dir
+        self.process: subprocess.Popen[bytes] | None = None
+        pass
+
+    def __enter__(self):
+        self.process = self.start_webserver()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.stop_webserver()
+
+    def start_webserver(self) -> subprocess.Popen[bytes] | None:
+        if self.serv_dir is None:
+            return None
+        try:
+            webserver_exec_path = os.path.join(os.path.dirname(__file__), "webserver-process.py")
+            process = subprocess.Popen(["python", f"{webserver_exec_path}", f"{self.host}", f"{self.port}", "-D", f"{self.serv_dir}"],
+                                       stdout=subprocess.DEVNULL,
+                                       stderr=subprocess.DEVNULL)
+            return process
+        except OSError as e:
+            if e.errno == errno.EADDRINUSE:
+                print(f"Port {self.port} already in use. Incrementing..")
+                self.port += 1
+                self.start_webserver()
+            else:
+                print(f"Failed to start webserver: {e}")
+        return None
+
+    def stop_webserver(self):
+        if self.process:
+            try:
+                self.process.kill()
+            except ProcessLookupError as e:
+                return
```

### Comparing `aruba_dero-1.0/src/modules/clearpass/utils.py` & `aruba_dero-1.0.1/src/dero-modules/clearpass/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import tempfile
-
-from cryptography import x509
-from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.asymmetric.dh import DHPrivateKey
-from cryptography.hazmat.primitives.asymmetric.dsa import DSAPrivateKey
-from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePrivateKey
-from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
-from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PrivateKey
-from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
-from cryptography.hazmat.primitives.asymmetric.x25519 import X25519PrivateKey
-from cryptography.hazmat.primitives.asymmetric.x448 import X448PrivateKey
-from cryptography.hazmat.primitives.serialization import BestAvailableEncryption
-from cryptography.hazmat.primitives.serialization import pkcs12, load_pem_private_key, load_der_private_key
-from cryptography.x509 import Certificate
-
-
-def check_cert_and_convert_to_pem(filename: str) -> tuple[str | None, Certificate | None]:
-    with open(filename, 'rb') as file:
-        cert_data = file.read()
-        if not cert_data:
-            return None, None
-
-    try:
-        # Try to load as PEM
-        cert = x509.load_pem_x509_certificate(cert_data)
-    except ValueError:
-        try:
-            # If loading as PEM fails, try to load as DER
-            cert = x509.load_der_x509_certificate(cert_data)
-        except ValueError:
-            # If both checks fail, return None
-            return None, None
-
-    # Output as PEM
-    return write_public_to_pem(cert)
-
-
-def check_key_and_convert_to_pem(filename: str, passphrase=None) -> tuple[
-    str | None, DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None]:
-    with open(filename, 'rb') as file:
-        key_data = file.read()
-        if not key_data:
-            return None, None
-
-        passphrase = passphrase.encode() if passphrase else None
-
-        try:
-            # Try to load as PEM
-            key = load_pem_private_key(key_data, passphrase)
-        except ValueError:
-            try:
-                # If loading as PEM fails, try to load as DER
-                key = load_der_private_key(key_data, passphrase)
-            except ValueError:
-                # If both checks fail, return None
-                return None, None
-        return write_private_to_pem(key, passphrase)
-
-
-def pkcs12_to_pem(filename: str, passphrase: str) -> tuple[str | None, object | None]:
-    with open(filename, 'rb') as file:
-        cert_data = file.read()
-        if not cert_data:
-            return None, None
-    try:
-        p12 = pkcs12.load_key_and_certificates(data=cert_data, password=passphrase.encode())
-        cert = p12[1]
-
-        if cert is None:
-            return None, None
-        return write_public_to_pem(cert)
-    except ValueError:
-        return None, None
-
-
-def write_public_to_pem(cert) -> tuple[str, Certificate]:
-    pem_data = cert.public_bytes(serialization.Encoding.PEM)
-
-    # Write the PEM data to a temporary file
-    temp_file = tempfile.NamedTemporaryFile(delete=False)
-    temp_file.write(pem_data)
-    temp_file.close()
-
-    return temp_file.name, cert
-
-
-def write_private_to_pem(
-        key: DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None,
-        passphrase: str | None) -> tuple[
-    str, DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None]:
-    pem_data = key.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.PKCS8,
-        encryption_algorithm=serialization.NoEncryption() if passphrase is None else BestAvailableEncryption(passphrase.encode())
-    )
-
-    # Write the PEM data to a temporary file
-    temp_file = tempfile.NamedTemporaryFile(delete=False)
-    temp_file.write(pem_data)
-    temp_file.close()
-
-    return temp_file.name, key
-
-
-def bundle_pkcs12(cert: Certificate,
-                  key: DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None,
-                  passphrase=None) -> tuple[str | None, bytes | None]:
-    p12 = pkcs12.serialize_key_and_certificates(
-        f"{cert.subject}".encode(), key, cert, None, BestAvailableEncryption(f"{passphrase}".encode())
-    )
-
-    temp_file = tempfile.NamedTemporaryFile(delete=False)
-    temp_file.write(p12)
-    temp_file.close()
-    return temp_file.name, p12
+import tempfile
+
+from cryptography import x509
+from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric.dh import DHPrivateKey
+from cryptography.hazmat.primitives.asymmetric.dsa import DSAPrivateKey
+from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePrivateKey
+from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
+from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PrivateKey
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+from cryptography.hazmat.primitives.asymmetric.x25519 import X25519PrivateKey
+from cryptography.hazmat.primitives.asymmetric.x448 import X448PrivateKey
+from cryptography.hazmat.primitives.serialization import BestAvailableEncryption
+from cryptography.hazmat.primitives.serialization import pkcs12, load_pem_private_key, load_der_private_key
+from cryptography.x509 import Certificate
+
+
+def check_cert_and_convert_to_pem(filename: str) -> tuple[str | None, Certificate | None]:
+    with open(filename, 'rb') as file:
+        cert_data = file.read()
+        if not cert_data:
+            return None, None
+
+    try:
+        # Try to load as PEM
+        cert = x509.load_pem_x509_certificate(cert_data)
+    except ValueError:
+        try:
+            # If loading as PEM fails, try to load as DER
+            cert = x509.load_der_x509_certificate(cert_data)
+        except ValueError:
+            # If both checks fail, return None
+            return None, None
+
+    # Output as PEM
+    return write_public_to_pem(cert)
+
+
+def check_key_and_convert_to_pem(filename: str, passphrase=None) -> tuple[
+    str | None, DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None]:
+    with open(filename, 'rb') as file:
+        key_data = file.read()
+        if not key_data:
+            return None, None
+
+        passphrase = passphrase.encode() if passphrase else None
+
+        try:
+            # Try to load as PEM
+            key = load_pem_private_key(key_data, passphrase)
+        except ValueError:
+            try:
+                # If loading as PEM fails, try to load as DER
+                key = load_der_private_key(key_data, passphrase)
+            except ValueError:
+                # If both checks fail, return None
+                return None, None
+        return write_private_to_pem(key, passphrase)
+
+
+def pkcs12_to_pem(filename: str, passphrase: str) -> tuple[str | None, object | None]:
+    with open(filename, 'rb') as file:
+        cert_data = file.read()
+        if not cert_data:
+            return None, None
+    try:
+        p12 = pkcs12.load_key_and_certificates(data=cert_data, password=passphrase.encode())
+        cert = p12[1]
+
+        if cert is None:
+            return None, None
+        return write_public_to_pem(cert)
+    except ValueError:
+        return None, None
+
+
+def write_public_to_pem(cert) -> tuple[str, Certificate]:
+    pem_data = cert.public_bytes(serialization.Encoding.PEM)
+
+    # Write the PEM data to a temporary file
+    temp_file = tempfile.NamedTemporaryFile(delete=False)
+    temp_file.write(pem_data)
+    temp_file.close()
+
+    return temp_file.name, cert
+
+
+def write_private_to_pem(
+        key: DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None,
+        passphrase: str | None) -> tuple[
+    str, DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None]:
+    pem_data = key.private_bytes(
+        encoding=serialization.Encoding.PEM,
+        format=serialization.PrivateFormat.PKCS8,
+        encryption_algorithm=serialization.NoEncryption() if passphrase is None else BestAvailableEncryption(passphrase.encode())
+    )
+
+    # Write the PEM data to a temporary file
+    temp_file = tempfile.NamedTemporaryFile(delete=False)
+    temp_file.write(pem_data)
+    temp_file.close()
+
+    return temp_file.name, key
+
+
+def bundle_pkcs12(cert: Certificate,
+                  key: DHPrivateKey | Ed25519PrivateKey | Ed448PrivateKey | RSAPrivateKey | DSAPrivateKey | EllipticCurvePrivateKey | X25519PrivateKey | X448PrivateKey | None,
+                  passphrase=None) -> tuple[str | None, bytes | None]:
+    p12 = pkcs12.serialize_key_and_certificates(
+        f"{cert.subject}".encode(), key, cert, None, BestAvailableEncryption(f"{passphrase}".encode())
+    )
+
+    temp_file = tempfile.NamedTemporaryFile(delete=False)
+    temp_file.write(p12)
+    temp_file.close()
+    return temp_file.name, p12
```

### Comparing `aruba_dero-1.0/src/modules/clearpass/webserver-process.py` & `aruba_dero-1.0.1/src/dero-modules/clearpass/webserver-process.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import http.server
-import os
-import socketserver
-import argparse
-
-parser = argparse.ArgumentParser(description="Temporary Webserver for CPPM",
-                                 formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-parser.add_argument("addr", help="Webserver Bind Address", type=str)
-parser.add_argument("port", help="Webserver Port", type=int)
-parser.add_argument("-D", "--root-dir", help="Webserver Root Dir", type=str)
-args = parser.parse_args()
-config = vars(args)
-
-root_dir = os.path.abspath(config.get("root_dir"))
-server_hostname, server_address = 'localhost', config.get("addr")
-server_port = config.get("port")
-
-
-def dir_exists_non_empty(path):
-    if not os.path.exists(path):
-        raise argparse.ArgumentTypeError(f"Directory {path} does not exist")
-    if not os.path.isdir(path):
-        raise argparse.ArgumentTypeError(f"{path} is not a directory")
-    if not os.listdir(path):
-        raise argparse.ArgumentTypeError(f"{path} is empty")
-    return path
-
-
-def start_server():
-    handler = http.server.SimpleHTTPRequestHandler
-    os.chdir(root_dir)
-
-    with socketserver.TCPServer((server_address, server_port), handler) as httpd:
-        print(f"Serving {root_dir}: http://{server_address}:{server_port}")
-        httpd.serve_forever()
-
-
-dir_exists_non_empty(root_dir)
-start_server()
+import http.server
+import os
+import socketserver
+import argparse
+
+parser = argparse.ArgumentParser(description="Temporary Webserver for CPPM",
+                                 formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+parser.add_argument("addr", help="Webserver Bind Address", type=str)
+parser.add_argument("port", help="Webserver Port", type=int)
+parser.add_argument("-D", "--root-dir", help="Webserver Root Dir", type=str)
+args = parser.parse_args()
+config = vars(args)
+
+root_dir = os.path.abspath(config.get("root_dir"))
+server_hostname, server_address = 'localhost', config.get("addr")
+server_port = config.get("port")
+
+
+def dir_exists_non_empty(path):
+    if not os.path.exists(path):
+        raise argparse.ArgumentTypeError(f"Directory {path} does not exist")
+    if not os.path.isdir(path):
+        raise argparse.ArgumentTypeError(f"{path} is not a directory")
+    if not os.listdir(path):
+        raise argparse.ArgumentTypeError(f"{path} is empty")
+    return path
+
+
+def start_server():
+    handler = http.server.SimpleHTTPRequestHandler
+    os.chdir(root_dir)
+
+    with socketserver.TCPServer((server_address, server_port), handler) as httpd:
+        print(f"Serving {root_dir}: http://{server_address}:{server_port}")
+        httpd.serve_forever()
+
+
+dir_exists_non_empty(root_dir)
+start_server()
```

