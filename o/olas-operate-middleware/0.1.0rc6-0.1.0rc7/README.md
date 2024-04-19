# Comparing `tmp/olas_operate_middleware-0.1.0rc6.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc6.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc7.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc6.tar` & `olas_operate_middleware-0.1.0rc7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc6/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc6/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc6/operate/__init__.py
--rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc6/operate/account/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc6/operate/account/user.py
--rw-r--r--   0        0        0    18550 2024-04-17 09:26:07.366152 olas_operate_middleware-0.1.0rc6/operate/cli.py
--rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc6/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc6/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc6/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc6/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc6/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc6/operate/keys.py
--rw-r--r--   0        0        0     3301 2024-04-17 09:26:07.366847 olas_operate_middleware-0.1.0rc6/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc6/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc6/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc6/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc6/operate/ledger/solana.py
--rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc6/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc6/operate/services/__init__.py
--rw-r--r--   0        0        0    17808 2024-04-17 11:42:50.723943 olas_operate_middleware-0.1.0rc6/operate/services/manage.py
--rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc6/operate/services/protocol.py
--rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc6/operate/services/service.py
--rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc6/operate/types.py
--rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc6/operate/utils/__init__.py
--rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc6/operate/utils/gnosis.py
--rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc6/operate/wallet/__init__.py
--rw-r--r--   0        0        0     8662 2024-04-16 14:21:46.519007 olas_operate_middleware-0.1.0rc6/operate/wallet/master.py
--rw-r--r--   0        0        0     1171 2024-04-18 10:17:15.241211 olas_operate_middleware-0.1.0rc6/pyproject.toml
--rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc7/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc7/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc7/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc7/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc7/operate/account/user.py
+-rw-r--r--   0        0        0    18602 2024-04-19 07:11:29.338570 olas_operate_middleware-0.1.0rc7/operate/cli.py
+-rw-r--r--   0        0        0     1189 2024-04-19 07:11:29.339849 olas_operate_middleware-0.1.0rc7/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc7/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc7/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc7/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc7/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc7/operate/keys.py
+-rw-r--r--   0        0        0     3301 2024-04-17 09:26:07.366847 olas_operate_middleware-0.1.0rc7/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc7/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc7/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc7/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc7/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc7/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc7/operate/services/__init__.py
+-rw-r--r--   0        0        0    18001 2024-04-19 07:11:29.340649 olas_operate_middleware-0.1.0rc7/operate/services/manage.py
+-rw-r--r--   0        0        0    22899 2024-04-19 07:11:29.341358 olas_operate_middleware-0.1.0rc7/operate/services/protocol.py
+-rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc7/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc7/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc7/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6333 2024-04-19 07:11:29.341902 olas_operate_middleware-0.1.0rc7/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc7/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8924 2024-04-19 07:11:29.342488 olas_operate_middleware-0.1.0rc7/operate/wallet/master.py
+-rw-r--r--   0        0        0     1171 2024-04-19 07:11:51.128399 olas_operate_middleware-0.1.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc7/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc6/LICENSE` & `olas_operate_middleware-0.1.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/README.md` & `olas_operate_middleware-0.1.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/account/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/account/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/account/user.py` & `olas_operate_middleware-0.1.0rc7/operate/account/user.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/cli.py` & `olas_operate_middleware-0.1.0rc7/operate/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,18 +485,19 @@
     @with_retries
     async def _stop_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
         service = request.path_params["service"]
         deployment = operate.service_manager().create_or_load(service).deployment
         deployment.stop()
 
-        logger.info(f"Cancelling funding job for {service}")
-        status = funding_jobs[service].cancel()
-        if not status:
-            logger.info(f"Funding job cancellation for {service} failed")
+        if service in funding_jobs:
+            logger.info(f"Cancelling funding job for {service}")
+            status = funding_jobs[service].cancel()
+            if not status:
+                logger.info(f"Funding job cancellation for {service} failed")
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/delete")
     @with_retries
     async def _delete_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
         # TODO: Drain safe before deleting service
```

### Comparing `olas_operate_middleware-0.1.0rc6/operate/constants.py` & `olas_operate_middleware-0.1.0rc7/operate/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 DEPLOYMENT_JSON = "deployment.json"
 CONFIG = "config.json"
 KEY = "key"
 KEYS = "keys"
 KEYS_JSON = "keys.json"
 DOCKER_COMPOSE_YAML = "docker-compose.yaml"
 SERVICE_YAML = "service.yaml"
+
+ON_CHAIN_INTERACT_TIMEOUT = 120.0
+ON_CHAIN_INTERACT_RETRIES = 40.0
+ON_CHAIN_INTERACT_SLEEP = 3.0
```

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc7/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc7/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/keys.py` & `olas_operate_middleware-0.1.0rc7/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc7/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc7/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc7/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc7/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/resource.py` & `olas_operate_middleware-0.1.0rc7/operate/resource.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc7/operate/services/manage.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,14 +172,24 @@
 
             if balance < required_olas:
                 raise ValueError(
                     "You don't have enough olas to stake, "
                     f"required olas: {required_olas}; your balance {balance}"
                 )
 
+        if service.chain_data.token > -1:
+            self.logger.info("Syncing service state")
+            info = ocm.info(token_id=service.chain_data.token)
+            service.chain_data.on_chain_state = OnChainState(info["service_state"])
+            service.chain_data.instances = info["instances"]
+            service.chain_data.multisig = info["multisig"]
+
+            service.store()
+        self.logger.info(f"Service state: {service.chain_data.on_chain_state.name}")
+
         if service.chain_data.on_chain_state == OnChainState.NOTMINTED:
             self.logger.info("Minting service")
             service.chain_data.token = t.cast(
                 int,
                 ocm.mint(
                     package_path=service.service_path,
                     agent_id=user_params.agent_id,
@@ -197,60 +207,52 @@
                         if user_params.use_staking
                         else None
                     ),
                 ).get("token"),
             )
             service.chain_data.on_chain_state = OnChainState.MINTED
             service.store()
-        else:
-            self.logger.info("Service already minted")
 
         if service.chain_data.on_chain_state == OnChainState.MINTED:
             self.logger.info("Activating service")
             ocm.activate(
                 service_id=service.chain_data.token,
                 token=(
                     OLAS[service.ledger_config.chain]
                     if user_params.use_staking
                     else None
                 ),
             )
             service.chain_data.on_chain_state = OnChainState.ACTIVATED
             service.store()
-        else:
-            self.logger.info("Service already activated")
 
         if service.chain_data.on_chain_state == OnChainState.ACTIVATED:
             self.logger.info("Registering service")
             ocm.register(
                 service_id=service.chain_data.token,
                 instances=instances,
                 agents=[user_params.agent_id for _ in instances],
             )
             service.chain_data.on_chain_state = OnChainState.REGISTERED
             service.keys = keys
             service.store()
-        else:
-            self.logger.info("Service already registered")
 
         if service.chain_data.on_chain_state == OnChainState.REGISTERED:
             self.logger.info("Deploying service")
             ocm.deploy(
                 service_id=service.chain_data.token,
                 reuse_multisig=update,
                 token=(
                     OLAS[service.ledger_config.chain]
                     if user_params.use_staking
                     else None
                 ),
             )
             service.chain_data.on_chain_state = OnChainState.DEPLOYED
             service.store()
-        else:
-            self.logger.info("Service already deployed")
 
         info = ocm.info(token_id=service.chain_data.token)
         service.keys = keys
         service.chain_data = OnChainData(
             token=service.chain_data.token,
             instances=info["instances"],
             multisig=info["multisig"],
```

### Comparing `olas_operate_middleware-0.1.0rc6/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc7/operate/services/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 from autonomy.chain.service import get_agent_instances, get_service_info
 from autonomy.chain.tx import TxSettler
 from autonomy.cli.helpers.chain import MintHelper as MintManager
 from autonomy.cli.helpers.chain import OnChainHelper
 from autonomy.cli.helpers.chain import ServiceHelper as ServiceManager
 from hexbytes import HexBytes
 
+from operate.constants import (
+    ON_CHAIN_INTERACT_RETRIES,
+    ON_CHAIN_INTERACT_SLEEP,
+    ON_CHAIN_INTERACT_TIMEOUT,
+)
 from operate.data import DATA_DIR
 from operate.data.contracts.service_staking_token.contract import (
     ServiceStakingTokenContract,
 )
 from operate.types import ContractAddresses
 from operate.utils.gnosis import (
     MultiSendOperation,
@@ -131,17 +136,17 @@
         if not self.slots_available(staking_contract):
             raise ValueError("No sataking slots available.")
 
         tx_settler = TxSettler(
             ledger_api=self.ledger_api,
             crypto=self.crypto,
             chain_type=self.chain_type,
-            timeout=self.timeout,
-            retries=self.retries,
-            sleep=self.sleep,
+            timeout=ON_CHAIN_INTERACT_TIMEOUT,
+            retries=ON_CHAIN_INTERACT_RETRIES,
+            sleep=ON_CHAIN_INTERACT_SLEEP,
         )
 
         # we make use of the ERC20 contract to build the approval transaction
         # since it has the same interface as ERC721 we might want to create
         # a ERC721 contract package
 
         def _build_approval_tx(  # pylint: disable=unused-argument
@@ -222,17 +227,17 @@
         if not self._can_unstake_service(service_id, staking_contract):
             raise ValueError("Service cannot be unstaked yet.")
 
         tx_settler = TxSettler(
             ledger_api=self.ledger_api,
             crypto=self.crypto,
             chain_type=self.chain_type,
-            timeout=self.timeout,
-            retries=self.retries,
-            sleep=self.sleep,
+            timeout=ON_CHAIN_INTERACT_TIMEOUT,
+            retries=ON_CHAIN_INTERACT_RETRIES,
+            sleep=ON_CHAIN_INTERACT_SLEEP,
         )
 
         def _build_unstaking_tx(  # pylint: disable=unused-argument
             *args: t.Any, **kargs: t.Any
         ) -> t.Dict:
             return self.ledger_api.build_transaction(
                 contract_instance=self.staking_ctr.get_instance(
@@ -355,14 +360,17 @@
         # TODO: Support for update
         self._patch()
         manager = MintManager(
             chain_type=self.chain_type,
             key=self.wallet.key_path,
             password=self.wallet.password,
             update_token=update_token,
+            timeout=ON_CHAIN_INTERACT_TIMEOUT,
+            retries=ON_CHAIN_INTERACT_RETRIES,
+            sleep=ON_CHAIN_INTERACT_SLEEP,
         )
 
         # Prepare for minting
         (
             manager.load_package_configuration(
                 package_path=package_path, package_type=PackageType.SERVICE
             )
@@ -409,14 +417,17 @@
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
                 key=self.wallet.key_path,
                 password=self.wallet.password,
+                timeout=ON_CHAIN_INTERACT_TIMEOUT,
+                retries=ON_CHAIN_INTERACT_RETRIES,
+                sleep=ON_CHAIN_INTERACT_SLEEP,
             ).check_is_service_token_secured(
                 token=token,
             ).activate_service()
 
     def register(
         self,
         service_id: int,
@@ -428,14 +439,17 @@
         logging.info(f"Registering service {service_id}...")
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
                 key=self.wallet.key_path,
                 password=self.wallet.password,
+                timeout=ON_CHAIN_INTERACT_TIMEOUT,
+                retries=ON_CHAIN_INTERACT_RETRIES,
+                sleep=ON_CHAIN_INTERACT_SLEEP,
             ).check_is_service_token_secured(
                 token=token,
             ).register_instance(
                 instances=instances,
                 agent_ids=agents,
             )
 
@@ -450,14 +464,17 @@
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
                 key=self.wallet.key_path,
                 password=self.wallet.password,
+                timeout=ON_CHAIN_INTERACT_TIMEOUT,
+                retries=ON_CHAIN_INTERACT_RETRIES,
+                sleep=ON_CHAIN_INTERACT_SLEEP,
             ).check_is_service_token_secured(
                 token=token,
             ).deploy_service(
                 reuse_multisig=reuse_multisig,
             )
 
     def swap(  # pylint: disable=too-many-arguments,too-many-locals
@@ -470,14 +487,17 @@
         logging.info(f"Swapping safe for service {service_id} [{multisig}]...")
         self._patch()
         manager = ServiceManager(
             service_id=service_id,
             chain_type=self.chain_type,
             key=self.wallet.key_path,
             password=self.wallet.password,
+            timeout=ON_CHAIN_INTERACT_TIMEOUT,
+            retries=ON_CHAIN_INTERACT_RETRIES,
+            sleep=ON_CHAIN_INTERACT_SLEEP,
         )
         with tempfile.TemporaryDirectory() as temp_dir:
             key_file = Path(temp_dir, "key.txt")
             key_file.write_text(owner_key, encoding="utf-8")
             owner_crypto = EthereumCrypto(private_key_path=str(key_file))
         owner_cryptos: list[EthereumCrypto] = [owner_crypto]
         owners = [
@@ -559,28 +579,34 @@
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
                 key=self.wallet.key_path,
                 password=self.wallet.password,
+                timeout=ON_CHAIN_INTERACT_TIMEOUT,
+                retries=ON_CHAIN_INTERACT_RETRIES,
+                sleep=ON_CHAIN_INTERACT_SLEEP,
             ).check_is_service_token_secured(
                 token=token,
             ).terminate_service()
 
     def unbond(self, service_id: int, token: t.Optional[str] = None) -> None:
         """Unbond service."""
         logging.info(f"Unbonding service {service_id}...")
         self._patch()
         with contextlib.redirect_stdout(io.StringIO()):
             ServiceManager(
                 service_id=service_id,
                 chain_type=self.chain_type,
                 key=self.wallet.key_path,
                 password=self.wallet.password,
+                timeout=ON_CHAIN_INTERACT_TIMEOUT,
+                retries=ON_CHAIN_INTERACT_RETRIES,
+                sleep=ON_CHAIN_INTERACT_SLEEP,
             ).check_is_service_token_secured(
                 token=token,
             ).unbond_service()
 
     def staking_slots_available(self, staking_contract: str) -> bool:
         """Stake service."""
         self._patch()
```

### Comparing `olas_operate_middleware-0.1.0rc6/operate/services/service.py` & `olas_operate_middleware-0.1.0rc7/operate/services/service.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/types.py` & `olas_operate_middleware-0.1.0rc7/operate/types.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/utils/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/utils/gnosis.py` & `olas_operate_middleware-0.1.0rc7/operate/utils/gnosis.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 from enum import Enum
 
 from aea.crypto.base import Crypto, LedgerApi
 from autonomy.chain.base import registry_contracts
 from autonomy.chain.config import ChainType as ChainProfile
 from autonomy.chain.tx import TxSettler
 
+from operate.constants import (
+    ON_CHAIN_INTERACT_RETRIES,
+    ON_CHAIN_INTERACT_SLEEP,
+    ON_CHAIN_INTERACT_TIMEOUT,
+)
+
 
 NULL_ADDRESS: str = "0x" + "0" * 40
 MAX_UINT256 = 2**256 - 1
 ZERO_ETH = 0
 
 
 class SafeOperation(Enum):
@@ -176,14 +182,17 @@
         del tx["contract_address"]
         return tx
 
     tx_settler = TxSettler(
         ledger_api=ledger_api,
         crypto=crypto,
         chain_type=ChainProfile.CUSTOM,
+        timeout=ON_CHAIN_INTERACT_TIMEOUT,
+        retries=ON_CHAIN_INTERACT_RETRIES,
+        sleep=ON_CHAIN_INTERACT_SLEEP,
     )
     setattr(  # noqa: B010
         tx_settler,
         "build",
         _build,
     )
     tx_settler.transact(
```

### Comparing `olas_operate_middleware-0.1.0rc6/operate/wallet/__init__.py` & `olas_operate_middleware-0.1.0rc7/operate/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc6/operate/wallet/master.py` & `olas_operate_middleware-0.1.0rc7/operate/wallet/master.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 from aea.crypto.base import Crypto, LedgerApi
 from aea.crypto.registries import make_ledger_api
 from aea_ledger_ethereum.ethereum import EthereumApi, EthereumCrypto
 from autonomy.chain.config import ChainType as ChainProfile
 from autonomy.chain.tx import TxSettler
 from web3 import Account
 
+from operate.constants import (
+    ON_CHAIN_INTERACT_RETRIES,
+    ON_CHAIN_INTERACT_SLEEP,
+    ON_CHAIN_INTERACT_TIMEOUT,
+)
 from operate.ledger import get_default_rpc
 from operate.resource import LocalResource
 from operate.types import ChainType, LedgerType
 from operate.utils.gnosis import create_safe as create_gnosis_safe
 
 
 class MasterWallet(LocalResource):
@@ -123,14 +128,17 @@
     def transfer(self, to: str, amount: int, chain_type: ChainType) -> None:
         """Transfer funds to the given account."""
         ledger_api = t.cast(EthereumApi, self.ledger_api(chain_type=chain_type))
         tx_helper = TxSettler(
             ledger_api=ledger_api,
             crypto=self.crypto,
             chain_type=ChainProfile.CUSTOM,
+            timeout=ON_CHAIN_INTERACT_TIMEOUT,
+            retries=ON_CHAIN_INTERACT_RETRIES,
+            sleep=ON_CHAIN_INTERACT_SLEEP,
         )
 
         def _build_tx(  # pylint: disable=unused-argument
             *args: t.Any, **kwargs: t.Any
         ) -> t.Dict:
             """Build transaction"""
             tx = ledger_api.get_transfer_transaction(
```

### Comparing `olas_operate_middleware-0.1.0rc6/pyproject.toml` & `olas_operate_middleware-0.1.0rc7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olas-operate-middleware"
-version = "0.1.0-rc6"
+version = "0.1.0-rc7"
 description = ""
 authors = ["David Vilela <dvilelaf@gmail.com>", "Viraj Patel <vptl185@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "operate" }
 ]
 include = [
```

### Comparing `olas_operate_middleware-0.1.0rc6/PKG-INFO` & `olas_operate_middleware-0.1.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

