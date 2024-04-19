# Comparing `tmp/aioipfs-0.7.0.tar.gz` & `tmp/aioipfs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioipfs-0.7.0.tar", last modified: Wed Apr 17 18:00:57 2024, max compression
+gzip compressed data, was "aioipfs-0.7.1.tar", last modified: Fri Apr 19 08:44:13 2024, max compression
```

## Comparing `aioipfs-0.7.0.tar` & `aioipfs-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.984653 aioipfs-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-17 18:00:25.000000 aioipfs-0.7.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-17 18:00:25.000000 aioipfs-0.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7663 2024-04-17 18:00:57.984653 aioipfs-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-17 18:00:25.000000 aioipfs-0.7.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.978653 aioipfs-0.7.0/aioipfs/
--rw-rw-rw-   0 root         (0) root         (0)    11032 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    59427 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.981653 aioipfs-0.7.0/aioipfs/apis/
--rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/multibase.py
--rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/p2p.py
--rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/pin.py
--rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/pubsub.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/swarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5464 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/multi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.981653 aioipfs-0.7.0/aioipfs/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.981653 aioipfs-0.7.0/aioipfs/scripts/bohort/
--rw-rw-rw-   0 root         (0) root         (0)     7860 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/scripts/bohort/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/scripts/bohort/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.982653 aioipfs-0.7.0/aioipfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7663 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-17 18:00:25.000000 aioipfs-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 18:00:57.984653 aioipfs-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.982653 aioipfs-0.7.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)    33964 2024-04-17 18:00:25.000000 aioipfs-0.7.0/tests/test_client.py
--rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-17 18:00:25.000000 aioipfs-0.7.0/tests/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.312601 aioipfs-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-19 08:43:43.000000 aioipfs-0.7.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-19 08:43:43.000000 aioipfs-0.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7715 2024-04-19 08:44:13.312601 aioipfs-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-19 08:43:43.000000 aioipfs-0.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.306601 aioipfs-0.7.1/aioipfs/
+-rw-rw-rw-   0 root         (0) root         (0)    11032 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    59427 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.309601 aioipfs-0.7.1/aioipfs/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/multibase.py
+-rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/p2p.py
+-rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/pin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/pubsub.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/apis/swarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5464 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/multi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.309601 aioipfs-0.7.1/aioipfs/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.309601 aioipfs-0.7.1/aioipfs/scripts/bohort/
+-rw-rw-rw-   0 root         (0) root         (0)     8644 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/scripts/bohort/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/scripts/bohort/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/scripts/bohort/default_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-19 08:43:43.000000 aioipfs-0.7.1/aioipfs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.310601 aioipfs-0.7.1/aioipfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7715 2024-04-19 08:44:13.000000 aioipfs-0.7.1/aioipfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-19 08:44:13.000000 aioipfs-0.7.1/aioipfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 08:44:13.000000 aioipfs-0.7.1/aioipfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-19 08:44:13.000000 aioipfs-0.7.1/aioipfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      439 2024-04-19 08:44:13.000000 aioipfs-0.7.1/aioipfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 08:44:13.000000 aioipfs-0.7.1/aioipfs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2024-04-19 08:43:43.000000 aioipfs-0.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 08:44:13.312601 aioipfs-0.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:44:13.310601 aioipfs-0.7.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    33964 2024-04-19 08:43:43.000000 aioipfs-0.7.1/tests/test_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-19 08:43:43.000000 aioipfs-0.7.1/tests/test_helpers.py
```

### Comparing `aioipfs-0.7.0/LICENSE` & `aioipfs-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/PKG-INFO` & `aioipfs-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.7.0
+Version: 0.7.1
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -43,14 +43,15 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-asyncio; extra == "docs"
+Requires-Dist: sphinxcontrib-video; extra == "docs"
 Requires-Dist: guzzle_sphinx_theme; extra == "docs"
 Provides-Extra: bohort
 Requires-Dist: appdirs>=1.4.4; extra == "bohort"
 Requires-Dist: omegaconf==2.3.0; extra == "bohort"
 Requires-Dist: ptpython-aioipfs>=3.0.27; extra == "bohort"
 
 =======
```

### Comparing `aioipfs-0.7.0/README.rst` & `aioipfs-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/__init__.py` & `aioipfs-0.7.1/aioipfs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 from yarl import URL
 from distutils.version import StrictVersion  # type: ignore
 from typing import Union
 
 import async_timeout
 import asyncio
```

### Comparing `aioipfs-0.7.0/aioipfs/api.py` & `aioipfs-0.7.1/aioipfs/api.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/__init__.py` & `aioipfs-0.7.1/aioipfs/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/dag.py` & `aioipfs-0.7.1/aioipfs/apis/dag.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/multibase.py` & `aioipfs-0.7.1/aioipfs/apis/multibase.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/p2p.py` & `aioipfs-0.7.1/aioipfs/apis/p2p.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/pin.py` & `aioipfs-0.7.1/aioipfs/apis/pin.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/pubsub.py` & `aioipfs-0.7.1/aioipfs/apis/pubsub.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/apis/swarm.py` & `aioipfs-0.7.1/aioipfs/apis/swarm.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/exceptions.py` & `aioipfs-0.7.1/aioipfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/helpers.py` & `aioipfs-0.7.1/aioipfs/helpers.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/multi.py` & `aioipfs-0.7.1/aioipfs/multi.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs/scripts/bohort/__init__.py` & `aioipfs-0.7.1/aioipfs/scripts/bohort/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,79 +2,95 @@
 import asyncio
 import functools
 import re
 import operator
 import inspect
 
 from dataclasses import dataclass
+from importlib import resources
 from pathlib import Path
 from typing import Union, List, Dict
 from ptpython import embed
 from prompt_toolkit import print_formatted_text, HTML
 
 import aioipfs
 from aioipfs.apis import SubAPI
 import appdirs  # type: ignore
 
 from omegaconf import OmegaConf
-from omegaconf import DictConfig
+from omegaconf import DictConfig, ListConfig
 
 from .cli import configure
+from .cli import pf_text
 
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 
 @dataclass
 class Context:
     client: aioipfs.AsyncIPFS
     interactive: bool = False
 
 
-def rpc_method_config(config: DictConfig, method: str) -> Union[DictConfig,
-                                                                None]:
+def rpc_method_config(config: DictConfig,
+                      method: str) -> Union[DictConfig, None]:
     rpc = config.get('rpc_methods')
 
     if isinstance(rpc, DictConfig):
         return rpc.get(method)
 
     return None
 
 
 async def _cmd_wrapper(config: DictConfig,
                        ctx: Context, method: str, *args, **kwargs):
+    timeout: float = 0
     try:
         meth = operator.attrgetter(method)(ctx.client)
         assert meth
 
         rpc_cfg = rpc_method_config(config, method)
-        if rpc_cfg and 'defaults' in rpc_cfg:
-            defaults = OmegaConf.to_container(rpc_cfg.defaults)  # type: ignore
+        if rpc_cfg:
+            timeout = rpc_cfg.get('timeout', 0)
+            assert isinstance(timeout, (int, float)), \
+                f"Invalid timeout config for method: {method}"
+
+            if 'defaults' in rpc_cfg:
+                defaults = OmegaConf.to_container(
+                    rpc_cfg.defaults)  # type: ignore
+
+                if isinstance(defaults, dict):
+                    for key, value in defaults.items():
+                        if key not in kwargs and isinstance(value,
+                                                            (int, float, str)):
+                            kwargs[key] = value  # type: ignore
+
+        async with ctx.client.timeout(
+                timeout if timeout > 0 else None):  # type: ignore
+            if inspect.isasyncgenfunction(meth):
+                # async generator
+                _entries: List = []
+
+                async for entry in meth(*args, **kwargs):
+                    _entries.append(entry)
+
+                return _entries
+            else:
+                # coroutine
 
-            if isinstance(defaults, dict):
-                for key, value in defaults.items():
-                    if key not in kwargs and isinstance(value,
-                                                        (int, float, str)):
-                        kwargs[key] = value  # type: ignore
-
-        if inspect.isasyncgenfunction(meth):
-            # async generator
-            _entries: List = []
-
-            async for entry in meth(*args, **kwargs):
-                _entries.append(entry)
-
-            return _entries
-        else:
-            # coroutine
-            return await meth(*args, **kwargs)
+                return await meth(*args, **kwargs)
     except aioipfs.RPCAccessDenied:
         print('Access denied for this RPC endpoint! Check your credentials.')
     except (aioipfs.APIError, aioipfs.UnknownAPIError) as aerr:
         print(f'API error {aerr.code}: {aerr.message}')
+    except asyncio.TimeoutError:
+        pf_text(f'Timeout for method: {method} ({timeout} secs)')
+    except asyncio.CancelledError as err:
+        pf_text(f'Method {method} cancelled: {err}')
     except AttributeError:
         print(f'No such client method: {method}')
     except BaseException:
         raise
 
 
 def get_auth_helper(creds: str) -> Union[aioipfs.BasicAuth,
@@ -86,27 +102,34 @@
     ma = re.match(r'^bearer:(.*?)$', creds)
     if ma:
         return aioipfs.BearerAuth(ma.group(1))
 
     raise ValueError(f'Invalid RPC credentials value: {creds}')
 
 
+def save_config(cfg_path: Path, config: Union[DictConfig, ListConfig]):
+    with open(cfg_path, 'wt') as f:
+        OmegaConf.save(config, f)
+
+
 async def start(args, cfg_dir: Path, data_dir: Path) -> None:
     cfg_path = cfg_dir.joinpath('bohort.yaml')
 
     if not cfg_path.exists():
-        with open(cfg_path, 'wt') as f:
-            OmegaConf.save(OmegaConf.create({
-                'nodes': {},
-                'rpc_methods': {}
-            }), f)
+        cfg_path.touch()
 
     with open(cfg_path, 'rt') as f:
         cfg = OmegaConf.load(f)
 
+    with resources.files(__name__).joinpath(
+            'default_config.yaml').open('r') as f:
+        cfg = OmegaConf.merge(OmegaConf.load(f), cfg)
+
+        save_config(cfg_path, cfg)
+
     if args.save_node:
         assert re.match(r'^[\w_-]+$', args.save_node), \
             "Invalid node name format"
 
         if args.save_node in cfg.nodes:
             del cfg.nodes[args.save_node]
 
@@ -118,16 +141,15 @@
                         'default': args.creds
                     }
                 }
             }
         })
         cfg = OmegaConf.merge(ncfg, cfg)
 
-        with open(cfg_path, 'wt') as f:
-            OmegaConf.save(cfg, f)
+        save_config(cfg_path, cfg)
 
     if args.node:
         node, credid = tuple(args.node.split(
             ':')) if ':' in args.node else (args.node, None)
 
         ncfg = cfg.nodes.get(node)
         assert ncfg, 'Node configuration does not exist!'
@@ -197,15 +219,15 @@
                     )
 
             await embed(
                 globals={},
                 locals=clocals,
                 return_asyncio_coroutine=True,
                 patch_stdout=True,
-                configure=configure,
+                configure=functools.partial(configure, cfg),
                 history_filename=args.history_path if
                 not args.no_history else None
             )  # type: ignore
     except aioipfs.RPCAccessDenied:
         print('RPC access denied!')
     except EOFError:
         pass
```

### Comparing `aioipfs-0.7.0/aioipfs/util.py` & `aioipfs-0.7.1/aioipfs/util.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/aioipfs.egg-info/PKG-INFO` & `aioipfs-0.7.1/aioipfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.7.0
+Version: 0.7.1
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -43,14 +43,15 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.3.0; extra == "docs"
 Requires-Dist: sphinxcontrib-asyncio; extra == "docs"
+Requires-Dist: sphinxcontrib-video; extra == "docs"
 Requires-Dist: guzzle_sphinx_theme; extra == "docs"
 Provides-Extra: bohort
 Requires-Dist: appdirs>=1.4.4; extra == "bohort"
 Requires-Dist: omegaconf==2.3.0; extra == "bohort"
 Requires-Dist: ptpython-aioipfs>=3.0.27; extra == "bohort"
 
 =======
```

### Comparing `aioipfs-0.7.0/aioipfs.egg-info/SOURCES.txt` & `aioipfs-0.7.1/aioipfs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 aioipfs/apis/p2p.py
 aioipfs/apis/pin.py
 aioipfs/apis/pubsub.py
 aioipfs/apis/swarm.py
 aioipfs/scripts/__init__.py
 aioipfs/scripts/bohort/__init__.py
 aioipfs/scripts/bohort/cli.py
+aioipfs/scripts/bohort/default_config.yaml
 tests/test_client.py
 tests/test_helpers.py
```

### Comparing `aioipfs-0.7.0/pyproject.toml` & `aioipfs-0.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "tox",
     "flake8",
     "wheel",
 ]
 docs = [
     "sphinx==5.3.0",
     "sphinxcontrib-asyncio",
+    "sphinxcontrib-video",
     "guzzle_sphinx_theme"
 ]
 bohort = [
     "appdirs>=1.4.4",
     "omegaconf==2.3.0",
     "ptpython-aioipfs>=3.0.27"
 ]
@@ -72,9 +73,12 @@
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
 namespaces = false
 
+[tool.setuptools.package-data]
+"aioipfs.scripts.bohort" = ["*.yaml"]
+
 [project.scripts]
 bohort = "aioipfs.scripts.bohort:run_bohort"
```

### Comparing `aioipfs-0.7.0/tests/test_client.py` & `aioipfs-0.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.7.0/tests/test_helpers.py` & `aioipfs-0.7.1/tests/test_helpers.py`

 * *Files identical despite different names*

