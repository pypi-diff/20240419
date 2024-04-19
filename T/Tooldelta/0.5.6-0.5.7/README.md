# Comparing `tmp/tooldelta-0.5.6.tar.gz` & `tmp/tooldelta-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.6.tar", max compression
+gzip compressed data, was "tooldelta-0.5.7.tar", max compression
```

## Comparing `tooldelta-0.5.6.tar` & `tooldelta-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1497 2024-04-19 13:43:42.401255 tooldelta-0.5.6/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-19 13:43:42.401255 tooldelta-0.5.6/README.md
--rwxr-xr-x   0        0        0      973 2024-04-19 13:43:51.737315 tooldelta-0.5.6/pyproject.toml
--rwxr-xr-x   0        0        0      360 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/auths.py
--rwxr-xr-x   0        0        0    19961 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    12365 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10889 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/color_print.py
--rw-r--r--   0        0        0     1884 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    30100 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/frame.py
--rwxr-xr-x   0        0        0     4644 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    20497 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1276 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/logger.py
--rw-r--r--   0        0        0    29616 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1292 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/packets.py
--rwxr-xr-x   0        0        0    15769 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7341 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      450 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     9975 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9146 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    16934 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16769 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1774 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/starter.py
--rwxr-xr-x   0        0        0      808 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9071 2024-04-19 13:43:42.405254 tooldelta-0.5.6/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-19 14:07:38.946065 tooldelta-0.5.7/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-19 14:07:38.946065 tooldelta-0.5.7/README.md
+-rwxr-xr-x   0        0        0      973 2024-04-19 14:07:46.998008 tooldelta-0.5.7/pyproject.toml
+-rwxr-xr-x   0        0        0      360 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    19961 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    12365 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10889 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1884 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    30100 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     4644 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    20525 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1276 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/logger.py
+-rw-r--r--   0        0        0    30151 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1292 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    15769 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7341 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      450 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     9975 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9146 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    16934 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16769 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1774 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      808 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9071 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.7/PKG-INFO
```

### Comparing `tooldelta-0.5.6/LICENSE` & `tooldelta-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/README.md` & `tooldelta-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/pyproject.toml` & `tooldelta-0.5.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.6" # This field is automatically set to the value in the version file
+version = "0.5.7" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.5.6/tooldelta/auths.py` & `tooldelta-0.5.7/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/builtins.py` & `tooldelta-0.5.7/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/cfg.py` & `tooldelta-0.5.7/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/color_print.py` & `tooldelta-0.5.7/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/constants.py` & `tooldelta-0.5.7/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.7/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/frame.py` & `tooldelta-0.5.7/tooldelta/frame.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/game_texts.py` & `tooldelta-0.5.7/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/launch_cli.py` & `tooldelta-0.5.7/tooldelta/launch_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         Args:
             serverNumber (int): 服务器号
             password (str): 服务器密码
             fbToken (str): 验证服务器Token
             auth_server (str): 验证服务器地址
         """
         super().__init__(serverNumber, password, fbToken, auth_server)
+        neo_conn.load_lib()
         self.status = SysStatus.LOADING
         self.launch_event = threading.Event()
         self.omega: Optional[neo_conn.ThreadOmega] = None
         self.neomg_proc = None
         self.download_libs()
         self.status = SysStatus.LAUNCHING
         self.secret_exit_key = ""
```

### Comparing `tooldelta-0.5.6/tooldelta/launch_options.py` & `tooldelta-0.5.7/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/logger.py` & `tooldelta-0.5.7/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/neo_conn.py` & `tooldelta-0.5.7/tooldelta/neo_conn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import platform
 import ctypes
 import ujson as json
 import os.path
 import traceback
 import threading
 import enum
 from typing import Iterable, Tuple, Optional, Union, Any, Callable, List, Dict
@@ -44,45 +45,15 @@
         "len": l,
         "cap": l,
     }
     return byteCSlice(**kwargs)
 
 
 # define lib path and how to load it
-import platform
 
-sys_machine = platform.machine().lower()
-sys_type = platform.uname().system
-sys_fn = os.path.join(os.getcwd(), "tooldelta")
-if sys_machine == "x86_64":
-    sys_machine = "amd64"
-elif sys_machine == "aarch64":
-    sys_machine = "arm64"
-if sys_type == "Windows":
-    lib_path = f"neomega_windows_{sys_machine}.dll"
-    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
-    LIB = ctypes.cdll.LoadLibrary(lib_path)
-elif "TERMUX_VERSION" in os.environ:
-    lib_path = "neomega_android_arm64.so"
-    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
-    LIB = ctypes.CDLL(lib_path)
-elif sys_type == "Linux":
-    lib_path = f"neomega_linux_{sys_machine}.so"
-    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
-    LIB = ctypes.CDLL(lib_path)
-else:
-    lib_path = f"neomega_macos_{sys_machine}.dylib"
-    lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
-    LIB = ctypes.CDLL(lib_path)
-
-# define lib functions
-
-# lib core functions: connect
-LIB.ConnectOmega.argtypes = [CString]
-LIB.ConnectOmega.restype = CString
 
 
 def ConnectOmega(address):
     r = LIB.ConnectOmega(toCString(address))
     if r is not None:
         raise Exception(toPyString(r))
 
@@ -93,27 +64,24 @@
     UserToken: str = ""
     UserName: str = ""
     UserPassword: str = ""
     ServerCode: str = ""
     ServerPassword: str = ""
 
 
-LIB.StartOmega.argtypes = [CString, CString]
-LIB.StartOmega.restype = CString
 
 
 def StartOmega(address, AccountOptions):
     r = LIB.StartOmega(
         toCString(address), toCString(json.dumps(AccountOptions.__dict__))
     )
     if r is not None:
         raise Exception(toPyString(r))
 
 
-LIB.OmegaAvailable.restype = ctypes.c_uint8
 
 
 def OmegaAvailable():
     if LIB.OmegaAvailable() != 1:
         raise Exception("omega Core disconnected")
 
 
@@ -121,198 +89,127 @@
 
 
 # lib core: event basic
 class Event(ctypes.Structure):
     _fields_ = [("type", CString), ("retriever", CString)]
 
 
-LIB.EventPoll.restype = Event
 
 
 def EventPoll() -> tuple[str, str]:
     event = LIB.EventPoll()
     return toPyString(event.type), toPyString(event.retriever)
 
 
 def OmitEvent():
     LIB.OmitEvent()
 
 
 # end lib core: event
 
 # event retrievers
-LIB.ConsumeOmegaConnError.restype = CString
-LIB.ConsumeCommandResponseCB.restype = CString
 
 
 class MCPacketEvent(ctypes.Structure):
     _fields_ = [("packetDataAsJsonStr", CString), ("convertError", CString)]
 
 
-LIB.ConsumeMCPacket.restype = MCPacketEvent
 
 # Async Actions
 # cmds
 
-LIB.SendWebSocketCommandNeedResponse.argtypes = [CString, CString]
 
 
 def SendWebSocketCommandNeedResponse(cmd: str, retrieverID: str):
     OmegaAvailable()
-    LIB.SendWebSocketCommandNeedResponse(toCString(cmd), toCString(retrieverID))
+    LIB.SendWebSocketCommandNeedResponse(
+        toCString(cmd), toCString(retrieverID))
 
 
-LIB.SendPlayerCommandNeedResponse.argtypes = [CString, CString]
 
 
 def SendPlayerCommandNeedResponse(cmd: str, retrieverID: str):
     OmegaAvailable()
     LIB.SendPlayerCommandNeedResponse(toCString(cmd), toCString(retrieverID))
 
 
 # OneWay Actions
-LIB.SendWOCommand.argtypes = [CString]
 
 
 def SendSettingsCommand(cmd: str):
     OmegaAvailable()
     LIB.SendWOCommand(toCString(cmd))
 
 
-LIB.SendWebSocketCommandOmitResponse.argtypes = [CString]
 
 
 def SendWebSocketCommandOmitResponse(cmd: str):
     OmegaAvailable()
     LIB.SendWebSocketCommandOmitResponse(toCString(cmd))
 
 
-LIB.SendPlayerCommandOmitResponse.argtypes = [CString]
 
 
 def SendPlayerCommandOmitResponse(cmd: str):
     OmegaAvailable()
     LIB.SendPlayerCommandOmitResponse(toCString(cmd))
 
 
 # Instance Actions
-LIB.FreeMem.argtypes = [ctypes.c_void_p]
-LIB.ListenAllPackets.argtypes = None
-LIB.GetPacketNameIDMapping.restype = CString
-LIB.JsonStrAsIsGamePacketBytes.argtypes = [CInt, CString]
 
 
 class JsonStrAsIsGamePacketBytes_return(ctypes.Structure):
     _fields_ = [("pktBytes", CBytes), ("l", CInt), ("err", CString)]
 
 
-LIB.JsonStrAsIsGamePacketBytes.restype = JsonStrAsIsGamePacketBytes_return
 
 
 def JsonStrAsIsGamePacketBytes(packetID: int, jsonStr: str) -> bytes:
     r = LIB.JsonStrAsIsGamePacketBytes(to_GoInt(packetID), toCString(jsonStr))
     if toPyString(r.err) != "":
         raise ValueError(toPyString(r.err))
     bs = r.pktBytes[: r.l]
     LIB.FreeMem(r.pktBytes)
     return bs
 
 
-LIB.SendGamePacket.argtypes = [CInt, CString]
-LIB.SendGamePacket.restype = CString
 
 
 def SendGamePacket(packetID: int, jsonStr: str) -> None:
     r = LIB.SendGamePacket(to_GoInt(packetID), toCString(jsonStr))
     if toPyString(r) != "":
         raise ValueError(toPyString(r))
 
 
-LIB.GetClientMaintainedBotBasicInfo.restype = CString
 
 
 # ClientMaintainedBotBasicInfo will not change
 @dataclass
 class ClientMaintainedBotBasicInfo:
     BotName: str = ""
     BotRuntimeID: int = 0
     BotUniqueID: int = 0
     BotIdentity: str = ""
     BotUUIDStr: str = ""
 
 
-LIB.GetClientMaintainedExtendInfo.restype = CString
 
 
 # any member of ClientMaintainedExtendInfo could be not found(which means related info not currently received from server)
 @dataclass
 class ClientMaintainedExtendInfo:
     CompressThreshold: Optional[int] = None
     WorldGameMode: Optional[int] = None
     WorldDifficulty: Optional[int] = None
     Time: Optional[int] = None
     DayTime: Optional[int] = None
     TimePercent: Optional[float] = None
     GameRules: Optional[Dict[str, Any]] = None
 
 
-LIB.GetAllOnlinePlayers.restype = CString
-LIB.ReleaseBindPlayer.argtypes = [CString]
-LIB.PlayerName.argtypes = [CString]
-LIB.PlayerName.restype = CString
-LIB.PlayerEntityUniqueID.argtypes = [CString]
-LIB.PlayerEntityUniqueID.restype = ctypes.c_int64
-LIB.PlayerLoginTime.argtypes = [CString]
-LIB.PlayerLoginTime.restype = ctypes.c_int64
-LIB.PlayerPlatformChatID.argtypes = [CString]
-LIB.PlayerPlatformChatID.restype = CString
-LIB.PlayerBuildPlatform.argtypes = [CString]
-LIB.PlayerBuildPlatform.restype = ctypes.c_int32
-LIB.PlayerSkinID.argtypes = [CString]
-LIB.PlayerSkinID.restype = CString
-LIB.PlayerPropertiesFlag.argtypes = [CString]
-LIB.PlayerPropertiesFlag.restype = ctypes.c_uint32
-LIB.PlayerCommandPermissionLevel.argtypes = [CString]
-LIB.PlayerCommandPermissionLevel.restype = ctypes.c_uint32
-LIB.PlayerActionPermissions.argtypes = [CString]
-LIB.PlayerActionPermissions.restype = ctypes.c_uint32
-LIB.PlayerGetAbilityString.argtypes = [CString]
-LIB.PlayerGetAbilityString.restype = CString
-LIB.PlayerOPPermissionLevel.argtypes = [CString]
-LIB.PlayerOPPermissionLevel.restype = ctypes.c_uint32
-LIB.PlayerCustomStoredPermissions.argtypes = [CString]
-LIB.PlayerCustomStoredPermissions.restype = ctypes.c_uint32
-LIB.PlayerDeviceID.argtypes = [CString]
-LIB.PlayerDeviceID.restype = CString
-LIB.PlayerEntityRuntimeID.argtypes = [CString]
-LIB.PlayerEntityRuntimeID.restype = ctypes.c_uint64
-LIB.PlayerEntityMetadata.argtypes = [CString]
-LIB.PlayerEntityMetadata.restype = CString
-LIB.PlayerIsOP.argtypes = [CString]
-LIB.PlayerIsOP.restype = ctypes.c_uint8
-LIB.PlayerOnline.argtypes = [CString]
-LIB.PlayerOnline.restype = ctypes.c_uint8
-
-LIB.GetPlayerByUUID.argtypes = [CString]
-LIB.GetPlayerByUUID.restype = CString
-
-LIB.GetPlayerByName.argtypes = [CString]
-LIB.GetPlayerByName.restype = CString
-
-LIB.ConsumePlayerChange.restype = CString
-LIB.InterceptPlayerJustNextInput.argtypes = [CString, CString]
-LIB.ConsumeChat.restype = CString
-
-LIB.PlayerChat.argtypes = [CString, CString]
-LIB.PlayerTitle.argtypes = [CString, CString, CString]
-LIB.PlayerActionBar.argtypes = [CString, CString]
-LIB.SetPlayerAbility.argtypes = [CString, CString]
-
-LIB.ListenCommandBlock.argtypes = [CString]
-LIB.PlaceCommandBlock.argtypes = [CString]
 
 
 def ConsumeChat() -> "Chat":
     chatData = json.loads(toPyString(LIB.ConsumeChat()))
     return Chat(**chatData)
 
 
@@ -618,27 +515,30 @@
         self._omega_disconnected_reason = ""
 
         # cmd events
         self._cmd_callback_retriever_counter = Counter("cmd_callback")
         self._omega_cmd_callback_events: Dict[str, Callable] = {}
 
         # packet listeners
-        self._packet_listeners: Dict[str, List[Callable[[str, any], None]]] = {}
+        self._packet_listeners: Dict[str,
+                                     List[Callable[[str, any], None]]] = {}
 
         # setup actions
-        LIB.ListenAllPackets()  # make LIB listen to all packets and new packets will have eventType="MCPacket"
+        # make LIB listen to all packets and new packets will have eventType="MCPacket"
+        LIB.ListenAllPackets()
         mapping = json.loads(toPyString(LIB.GetPacketNameIDMapping()))
         self._packet_name_to_id_mapping: dict[str, int] = mapping
         self._packet_id_to_name_mapping = {}
         for packet_name, packet_id in self._packet_name_to_id_mapping.items():
             self._packet_id_to_name_mapping[packet_id] = packet_name
             self._packet_listeners[packet_name] = []
 
         LIB.ListenPlayerChange()
-        self._player_change_listeners: List[Callable[[PlayerKit, str], None]] = []
+        self._player_change_listeners: List[Callable[[
+            PlayerKit, str], None]] = []
 
         # get bot basic info (this info will not change so we need to get it only once)
         self._bot_basic_info = ClientMaintainedBotBasicInfo(
             **json.loads(toPyString(LIB.GetClientMaintainedBotBasicInfo()))
         )
 
         # player hooks
@@ -702,15 +602,16 @@
                 playerUUID = retriever
                 if len(self._player_change_listeners) == 0:
                     LIB.OmitEvent()
                 else:
                     action = toPyString(LIB.ConsumePlayerChange())
                     for callback in self._player_change_listeners:
                         self.start_new(
-                            callback, (self._get_bind_player(playerUUID), action)
+                            callback, (self._get_bind_player(
+                                playerUUID), action)
                         )
 
             elif eventType == "PlayerInterceptInput":
                 OmitEvent()
 
             elif eventType == "Chat":
                 OmitEvent()
@@ -894,15 +795,16 @@
 
     def listen_named_command_block(
         self, command_block_name: str, callback: Callable[[Chat], None]
     ):
         if command_block_name not in self._name_command_block_msg_listeners:
             self._name_command_block_msg_listeners[command_block_name] = []
         LIB.ListenCommandBlock(toCString(command_block_name))
-        self._name_command_block_msg_listeners[command_block_name].append(callback)
+        self._name_command_block_msg_listeners[command_block_name].append(
+            callback)
 
     @staticmethod
     def place_command_block(place_option: CommandBlockPlaceOption):
         LIB.PlaceCommandBlock(toCString(json.dumps(place_option.__dict__)))
 
     def __del__(self):
         for t in self._running_threads.values():
@@ -922,7 +824,117 @@
         "SuccessCOunt": c.SuccessCount,
         "DataSet": c.DataSet,
     }
 
 
 def _unpack_output_msgs(c: OutputMessage):
     return {"Success": c.Success, "Message": c.Message, "Parameters": c.Parameters}
+
+
+def load_lib():
+    global LIB
+    sys_machine = platform.machine().lower()
+    sys_type = platform.uname().system
+    sys_fn = os.path.join(os.getcwd(), "tooldelta")
+    if sys_machine == "x86_64":
+        sys_machine = "amd64"
+    elif sys_machine == "aarch64":
+        sys_machine = "arm64"
+    if sys_type == "Windows":
+        lib_path = f"neomega_windows_{sys_machine}.dll"
+        lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+        LIB = ctypes.cdll.LoadLibrary(lib_path)
+    elif "TERMUX_VERSION" in os.environ:
+        lib_path = "neomega_android_arm64.so"
+        lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+        LIB = ctypes.CDLL(lib_path)
+    elif sys_type == "Linux":
+        lib_path = f"neomega_linux_{sys_machine}.so"
+        lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+        LIB = ctypes.CDLL(lib_path)
+    else:
+        lib_path = f"neomega_macos_{sys_machine}.dylib"
+        lib_path = os.path.join(sys_fn, "neo_libs", lib_path)
+        LIB = ctypes.CDLL(lib_path)
+
+    # define lib functions
+
+    # lib core functions: connect
+    LIB.ConnectOmega.argtypes = [CString]
+    LIB.ConnectOmega.restype = CString
+    LIB.StartOmega.argtypes = [CString, CString]
+    LIB.StartOmega.restype = CString
+
+    LIB.OmegaAvailable.restype = ctypes.c_uint8
+
+    LIB.EventPoll.restype = Event
+    LIB.ConsumeOmegaConnError.restype = CString
+    LIB.ConsumeCommandResponseCB.restype = CString
+    LIB.ConsumeMCPacket.restype = MCPacketEvent
+    LIB.SendWebSocketCommandNeedResponse.argtypes = [CString, CString]
+    LIB.SendPlayerCommandNeedResponse.argtypes = [CString, CString]
+    LIB.SendWOCommand.argtypes = [CString]
+    LIB.SendWebSocketCommandOmitResponse.argtypes = [CString]
+    LIB.SendPlayerCommandOmitResponse.argtypes = [CString]
+    LIB.FreeMem.argtypes = [ctypes.c_void_p]
+    LIB.ListenAllPackets.argtypes = None
+    LIB.GetPacketNameIDMapping.restype = CString
+    LIB.JsonStrAsIsGamePacketBytes.argtypes = [CInt, CString]
+    LIB.JsonStrAsIsGamePacketBytes.restype = JsonStrAsIsGamePacketBytes_return
+    LIB.SendGamePacket.argtypes = [CInt, CString]
+    LIB.SendGamePacket.restype = CString
+    LIB.GetClientMaintainedBotBasicInfo.restype = CString
+    LIB.GetClientMaintainedExtendInfo.restype = CString
+    LIB.GetAllOnlinePlayers.restype = CString
+    LIB.ReleaseBindPlayer.argtypes = [CString]
+    LIB.PlayerName.argtypes = [CString]
+    LIB.PlayerName.restype = CString
+    LIB.PlayerEntityUniqueID.argtypes = [CString]
+    LIB.PlayerEntityUniqueID.restype = ctypes.c_int64
+    LIB.PlayerLoginTime.argtypes = [CString]
+    LIB.PlayerLoginTime.restype = ctypes.c_int64
+    LIB.PlayerPlatformChatID.argtypes = [CString]
+    LIB.PlayerPlatformChatID.restype = CString
+    LIB.PlayerBuildPlatform.argtypes = [CString]
+    LIB.PlayerBuildPlatform.restype = ctypes.c_int32
+    LIB.PlayerSkinID.argtypes = [CString]
+    LIB.PlayerSkinID.restype = CString
+    LIB.PlayerPropertiesFlag.argtypes = [CString]
+    LIB.PlayerPropertiesFlag.restype = ctypes.c_uint32
+    LIB.PlayerCommandPermissionLevel.argtypes = [CString]
+    LIB.PlayerCommandPermissionLevel.restype = ctypes.c_uint32
+    LIB.PlayerActionPermissions.argtypes = [CString]
+    LIB.PlayerActionPermissions.restype = ctypes.c_uint32
+    LIB.PlayerGetAbilityString.argtypes = [CString]
+    LIB.PlayerGetAbilityString.restype = CString
+    LIB.PlayerOPPermissionLevel.argtypes = [CString]
+    LIB.PlayerOPPermissionLevel.restype = ctypes.c_uint32
+    LIB.PlayerCustomStoredPermissions.argtypes = [CString]
+    LIB.PlayerCustomStoredPermissions.restype = ctypes.c_uint32
+    LIB.PlayerDeviceID.argtypes = [CString]
+    LIB.PlayerDeviceID.restype = CString
+    LIB.PlayerEntityRuntimeID.argtypes = [CString]
+    LIB.PlayerEntityRuntimeID.restype = ctypes.c_uint64
+    LIB.PlayerEntityMetadata.argtypes = [CString]
+    LIB.PlayerEntityMetadata.restype = CString
+    LIB.PlayerIsOP.argtypes = [CString]
+    LIB.PlayerIsOP.restype = ctypes.c_uint8
+    LIB.PlayerOnline.argtypes = [CString]
+    LIB.PlayerOnline.restype = ctypes.c_uint8
+
+    LIB.GetPlayerByUUID.argtypes = [CString]
+    LIB.GetPlayerByUUID.restype = CString
+
+    LIB.GetPlayerByName.argtypes = [CString]
+    LIB.GetPlayerByName.restype = CString
+
+    LIB.ConsumePlayerChange.restype = CString
+    LIB.InterceptPlayerJustNextInput.argtypes = [CString, CString]
+    LIB.ConsumeChat.restype = CString
+
+    LIB.PlayerChat.argtypes = [CString, CString]
+    LIB.PlayerTitle.argtypes = [CString, CString, CString]
+    LIB.PlayerActionBar.argtypes = [CString, CString]
+    LIB.SetPlayerAbility.argtypes = [CString, CString]
+
+    LIB.ListenCommandBlock.argtypes = [CString]
+    LIB.PlaceCommandBlock.argtypes = [CString]
```

### Comparing `tooldelta-0.5.6/tooldelta/packets.py` & `tooldelta-0.5.7/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.7/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.7/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.7/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_manager.py` & `tooldelta-0.5.7/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/plugin_market.py` & `tooldelta-0.5.7/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/starter.py` & `tooldelta-0.5.7/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/sys_args.py` & `tooldelta-0.5.7/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/tooldelta/urlmethod.py` & `tooldelta-0.5.7/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.6/PKG-INFO` & `tooldelta-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.6
+Version: 0.5.7
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.6 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.7 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
```

