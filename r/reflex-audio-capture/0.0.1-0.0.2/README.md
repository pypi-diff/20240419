# Comparing `tmp/reflex-audio-capture-0.0.1.tar.gz` & `tmp/reflex_audio_capture-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-audio-capture-0.0.1.tar", last modified: Fri Apr 12 01:33:35 2024, max compression
+gzip compressed data, was "reflex_audio_capture-0.0.2.tar", last modified: Thu Apr 18 22:10:33 2024, max compression
```

## Comparing `reflex-audio-capture-0.0.1.tar` & `reflex_audio_capture-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-12 01:33:35.434561 reflex-audio-capture-0.0.1/
--rw-r--r--   0 masenf     (501) staff       (20)      768 2024-04-12 01:33:35.434276 reflex-audio-capture-0.0.1/PKG-INFO
--rw-r--r--   0 masenf     (501) staff       (20)      238 2024-04-12 01:30:54.000000 reflex-audio-capture-0.0.1/README.md
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-12 01:33:35.432460 reflex-audio-capture-0.0.1/custom_components/
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-12 01:33:35.432920 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture/
--rw-r--r--   0 masenf     (501) staff       (20)       29 2024-04-12 01:22:50.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture/__init__.py
--rw-r--r--   0 masenf     (501) staff       (20)     8185 2024-04-12 01:30:07.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture/audio_capture.py
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-12 01:33:35.433879 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/
--rw-r--r--   0 masenf     (501) staff       (20)      768 2024-04-12 01:33:35.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/PKG-INFO
--rw-r--r--   0 masenf     (501) staff       (20)      440 2024-04-12 01:33:35.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/SOURCES.txt
--rw-r--r--   0 masenf     (501) staff       (20)        1 2024-04-12 01:33:35.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/dependency_links.txt
--rw-r--r--   0 masenf     (501) staff       (20)       34 2024-04-12 01:33:35.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/requires.txt
--rw-r--r--   0 masenf     (501) staff       (20)       21 2024-04-12 01:33:35.000000 reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/top_level.txt
--rw-r--r--   0 masenf     (501) staff       (20)      689 2024-04-12 01:29:42.000000 reflex-audio-capture-0.0.1/pyproject.toml
--rw-r--r--   0 masenf     (501) staff       (20)       38 2024-04-12 01:33:35.434614 reflex-audio-capture-0.0.1/setup.cfg
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-18 22:10:33.433983 reflex_audio_capture-0.0.2/
+-rw-r--r--   0 masenf     (501) staff       (20)      767 2024-04-18 22:10:33.433778 reflex_audio_capture-0.0.2/PKG-INFO
+-rw-r--r--   0 masenf     (501) staff       (20)      238 2024-04-12 01:30:54.000000 reflex_audio_capture-0.0.2/README.md
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-18 22:10:33.432003 reflex_audio_capture-0.0.2/custom_components/
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-18 22:10:33.432570 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture/
+-rw-r--r--   0 masenf     (501) staff       (20)       29 2024-04-12 01:22:50.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture/__init__.py
+-rw-r--r--   0 masenf     (501) staff       (20)     9580 2024-04-18 22:04:21.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture/audio_capture.py
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-18 22:10:33.433491 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/
+-rw-r--r--   0 masenf     (501) staff       (20)      767 2024-04-18 22:10:33.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/PKG-INFO
+-rw-r--r--   0 masenf     (501) staff       (20)      440 2024-04-18 22:10:33.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/SOURCES.txt
+-rw-r--r--   0 masenf     (501) staff       (20)        1 2024-04-18 22:10:33.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/dependency_links.txt
+-rw-r--r--   0 masenf     (501) staff       (20)       33 2024-04-18 22:10:33.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/requires.txt
+-rw-r--r--   0 masenf     (501) staff       (20)       21 2024-04-18 22:10:33.000000 reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/top_level.txt
+-rw-r--r--   0 masenf     (501) staff       (20)      689 2024-04-18 21:47:51.000000 reflex_audio_capture-0.0.2/pyproject.toml
+-rw-r--r--   0 masenf     (501) staff       (20)       38 2024-04-18 22:10:33.434026 reflex_audio_capture-0.0.2/setup.cfg
```

### Comparing `reflex-audio-capture-0.0.1/PKG-INFO` & `reflex_audio_capture-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-audio-capture
-Version: 0.0.1
+Version: 0.0.2
 Summary: Experimental audio-recorder-polyfill component
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/masenf/reflex-audio-capture
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.8a
+Requires-Dist: reflex>=0.4.8
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # reflex-audio-capture
 
 Cross-browser audio capture using audio-recorder-polyfill.
```

### Comparing `reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture/audio_capture.py` & `reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture/audio_capture.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,48 +5,77 @@
 from typing import List
 
 from jinja2 import Environment
 
 import reflex as rx
 
 
+class MediaDeviceInfo(rx.Base):
+    """A media device info object."""
+
+    kind: str
+    label: str
+    deviceId: str
+    groupId: str
+
+
 START_RECORDING_JS_TEMPLATE = """
 const [mediaRecorderState, setMediaRecorderState] = useState('unknown')
 refs['mediarecorder_state_{{ ref }}'] = mediaRecorderState
+const [mediaDevices, setMediaDevices] = useState([])
+refs['mediadevices_{{ ref }}'] = mediaDevices
+const updateMediaDevices = () => {
+  if (!navigator.mediaDevices?.enumerateDevices) {
+    const _error = "enumerateDevices() not supported on your browser!"
+    {{ on_error }}
+  } else {
+    navigator.mediaDevices
+      .enumerateDevices()
+      .then((devices) => {
+        setMediaDevices(devices.filter((device) => device.deviceId && device.kind === "audioinput"))
+      })
+      .catch((err) => {
+        const _error = err.name + ": " + err.message;
+        {{ on_error }}
+      });
+  }
+}
 refs['mediarecorder_start_{{ ref }}'] = useCallback(() => {
     const mediaRecorderRef = refs['mediarecorder_{{ ref }}']
     if (mediaRecorderRef !== undefined) {
-        console.log(mediaRecorderRef)
         mediaRecorderRef.stop()
     }
     if (navigator.mediaDevices && navigator.mediaDevices.getUserMedia) {
-        navigator.mediaDevices.getUserMedia({audio: true})
+        const device_id = ({{ device_id }} ? {deviceId: {{ device_id }}} : true)
+        navigator.mediaDevices.getUserMedia({audio: device_id})
         // Success callback
         .then(async (stream) => {
+            if (mediaDevices.length === 0) {
+                // update device list after permission is granted
+                updateMediaDevices()
+            }
             const AudioRecorder = (await import('audio-recorder-polyfill')).default
             if ({{ use_mp3 }}) {
                 const mpegEncoder = (await import('audio-recorder-polyfill/mpeg-encoder')).default
                 AudioRecorder.encoder = mpegEncoder
                 AudioRecorder.prototype.mimeType = 'audio/mpeg'
             }
             refs['mediarecorder_{{ ref }}'] = new AudioRecorder(stream)
             const mediaRecorderRef = refs['mediarecorder_{{ ref }}']
             const updateState = () => {
-                console.log(mediaRecorderRef.state)
                 setMediaRecorderState(mediaRecorderRef.state)
             }
             mediaRecorderRef.addEventListener('stop', updateState)
             mediaRecorderRef.addEventListener('start', updateState)
             mediaRecorderRef.addEventListener('pause', updateState)
             mediaRecorderRef.addEventListener('resume', updateState)
             mediaRecorderRef.addEventListener('error', updateState)
             mediaRecorderRef.addEventListener(
                 "dataavailable",
                 (e) => {
-                    console.log("data available", e.data.size)
                     if (e.data.size > 0) {
                         var a = new FileReader();
                         a.onload = (e) => {
                             const _data = e.target.result
                             {{ on_data_available }}
                         }
                         a.readAsDataURL(e.data);
@@ -54,26 +83,29 @@
                 }
             );
             {{ on_start_callback }}
             {{ on_stop_callback }}
             {{ on_error_callback }}
             addEventListener('beforeunload', () => {mediaRecorderRef.stop()})
             mediaRecorderRef.start({{ timeslice }})
-            console.log(mediaRecorderRef)
+            console.log(mediaRecorderRef, device_id)
         })
         // Error callback
         .catch((err) => {
             const _error = "The following getUserMedia error occurred: " + err
             {{ on_error }}
         });
     } else {
         const _error = "getUserMedia not supported on your browser!"
         {{ on_error }}
     }
-})"""
+})
+// Enumerate devices and set the state
+useEffect(updateMediaDevices, [])
+"""
 
 
 def get_codec(data_uri) -> str | None:
     if not data_uri.startswith("data:"):
         return None
     colon_index = data_uri.find(":")
     end_index = data_uri.find(";base64,")
@@ -124,14 +156,15 @@
     lib_dependencies: List[str] = ["audio-recorder-polyfill"]
 
     on_data_available: rx.EventHandler[lambda data: [data]]
     on_start: rx.EventHandler
     on_stop: rx.EventHandler
     on_error: rx.EventHandler[lambda error: [error]]
     timeslice: rx.Var[int]
+    device_id: rx.Var[str]
     use_mp3: rx.Var[bool] = True
 
     @classmethod
     def create(cls, *children, **props) -> rx.Component:
         props.setdefault("id", rx.vars.get_unique_variable_name())
         return super().create(*children, **props)
 
@@ -140,14 +173,15 @@
 
     def _get_imports(self):
         return rx.utils.imports.merge_imports(
             super()._get_imports(),
             {
                 "react": [
                     rx.utils.imports.ImportVar(tag="useCallback"),
+                    rx.utils.imports.ImportVar(tag="useEffect"),
                     rx.utils.imports.ImportVar(tag="useState"),
                 ],
             },
         )
 
     def _get_hooks(self) -> str:
         on_data_available = self.event_triggers.get("on_data_available")
@@ -199,15 +233,18 @@
                 ref=self.get_ref(),
                 on_data_available=on_data_available,
                 on_start_callback=on_start_callback,
                 on_stop_callback=on_stop_callback,
                 on_error_callback=on_error_callback,
                 on_error=on_error,
                 timeslice=str(rx.cond(self.timeslice, self.timeslice, "")).strip("{}"),
-                use_mp3=self.use_mp3,
+                device_id=self.device_id._var_name_unwrapped
+                if self.device_id is not None
+                else "undefined",
+                use_mp3=self.use_mp3._var_name_unwrapped,
             )
         )
 
     def start(self):
         return rx.call_script(f"refs['mediarecorder_start_{self.get_ref()}']()")
 
     def stop(self):
@@ -222,7 +259,14 @@
 
     @property
     def recorder_state(self) -> rx.Var[str]:
         return rx.Var.create(
             f"(refs['mediarecorder_state_{self.get_ref()}'])",
             _var_is_local=False,
         ).to(str)
+
+    @property
+    def media_devices(self) -> rx.Var[List[MediaDeviceInfo]]:
+        return rx.Var.create(
+            f"(refs['mediadevices_{self.get_ref()}'])",
+            _var_is_local=False,
+        ).to(List[MediaDeviceInfo])
```

### Comparing `reflex-audio-capture-0.0.1/custom_components/reflex_audio_capture.egg-info/PKG-INFO` & `reflex_audio_capture-0.0.2/custom_components/reflex_audio_capture.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-audio-capture
-Version: 0.0.1
+Version: 0.0.2
 Summary: Experimental audio-recorder-polyfill component
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/masenf/reflex-audio-capture
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.8a
+Requires-Dist: reflex>=0.4.8
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # reflex-audio-capture
 
 Cross-browser audio capture using audio-recorder-polyfill.
```

### Comparing `reflex-audio-capture-0.0.1/pyproject.toml` & `reflex_audio_capture-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-audio-capture"
-version = "0.0.1"
+version = "0.0.2"
 description = "Experimental audio-recorder-polyfill component"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = ["reflex","reflex-custom-components"]
 
-dependencies = ["reflex>=0.4.8a"]
+dependencies = ["reflex>=0.4.8"]
 
 classifiers = ["Development Status :: 4 - Beta"]
 
 [project.urls]
 homepage = "https://github.com/masenf/reflex-audio-capture"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.setuptools.packages.find]
-where = ["custom_components"]
+where = ["custom_components"]
```

