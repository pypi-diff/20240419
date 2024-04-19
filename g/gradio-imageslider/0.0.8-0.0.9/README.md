# Comparing `tmp/gradio_imageslider-0.0.8.tar.gz` & `tmp/gradio_imageslider-0.0.9.tar.gz`

## Comparing `gradio_imageslider-0.0.8.tar` & `gradio_imageslider-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/.DS_Store
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/.prettierrc.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/__init__.py
--rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/imageslider.py
--rw-r--r--   0        0        0    32760 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/imageslider.pyi
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/example/index.js
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/example/style.css
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/__vite-browser-external-2447137e.mjs
--rw-r--r--   0        0        0   173424 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/index.js
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/style.css
--rw-r--r--   0        0        0    78110 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/wrapper-6f348d45-492a1cb9.mjs
--rw-r--r--   0        0        0   138779 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/static/index.js
--rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/static/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/demo/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/demo/app.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/package.json
--rw-r--r--   0        0        0    23990 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/example/Image.svelte
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/example/index.ts
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/interactive/Image.svelte
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/interactive/InteractiveImage.svelte
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/interactive/index.ts
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/shared/Slider.svelte
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/shared/utils.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/src/Image.svelte
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/static/ImagePreview.svelte
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/static/StaticImage.svelte
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/frontend/static/index.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/.gitignore
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/.DS_Store
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/.prettierrc.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/__init__.py
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/imageslider.py
+-rw-r--r--   0        0        0    32760 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/imageslider.pyi
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/example/index.js
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/example/style.css
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/__vite-browser-external-2447137e.mjs
+-rw-r--r--   0        0        0   173439 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/index.js
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/style.css
+-rw-r--r--   0        0        0    78110 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/wrapper-6f348d45-492a1cb9.mjs
+-rw-r--r--   0        0        0   138839 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/static/index.js
+-rw-r--r--   0        0        0    12150 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/static/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/demo/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/demo/app.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/package.json
+-rw-r--r--   0        0        0    23990 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/example/Image.svelte
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/example/index.ts
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/interactive/Image.svelte
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/interactive/InteractiveImage.svelte
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/interactive/index.ts
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/shared/Slider.svelte
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/shared/utils.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/src/Image.svelte
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/static/ImagePreview.svelte
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/static/StaticImage.svelte
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/frontend/static/index.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gradio_imageslider-0.0.9/PKG-INFO
```

### Comparing `gradio_imageslider-0.0.8/.DS_Store` & `gradio_imageslider-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/imageslider.py` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/imageslider.py`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/imageslider.pyi` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/imageslider.pyi`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/example/index.js` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/index.js` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6500,15 +6500,15 @@
     }
     const S = (p) => c(p, 1);
     return e.$$set = (p) => {
         "value" in p && n(0, s = p.value), "label" in p && n(1, o = p.label), "show_label" in p && n(2, a = p.show_label), "pending" in p && n(6, u = p.pending), "root" in p && n(3, l = p.root), "i18n" in p && n(7, f = p.i18n), "$$scope" in p && n(13, i = p.$$scope);
     }, e.$$.update = () => {
         e.$$.dirty & /*dragging*/
             16 && h("drag", _), e.$$.dirty & /*value*/
-            1 && console.log(s);
+            1 && console.log("interactive", s);
     }, [
         s,
         o,
         a,
         l,
         _,
         c,
```

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/style.css` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/style.css`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/interactive/wrapper-6f348d45-492a1cb9.mjs` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/interactive/wrapper-6f348d45-492a1cb9.mjs`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/static/index.js` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/static/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5035,15 +5035,16 @@
     function f(h) {
         u = h, n(4, u);
     }
     return e.$$set = (h) => {
         "value" in h && n(5, i = h.value), "label" in h && n(0, s = h.label), "show_label" in h && n(1, o = h.show_label), "root" in h && n(6, l = h.root), "i18n" in h && n(2, a = h.i18n);
     }, e.$$.update = () => {
         e.$$.dirty & /*value, value_, root*/
-            104 && i !== r && (n(3, r = i), Kn(r, l, null));
+            104 && i !== r && (n(3, r = i), Kn(r, l, null)), e.$$.dirty & /*value_*/
+            8 && console.log("static:", r);
     }, [
         s,
         o,
         a,
         r,
         u,
         i,
```

### Comparing `gradio_imageslider-0.0.8/backend/gradio_imageslider/templates/static/style.css` & `gradio_imageslider-0.0.9/backend/gradio_imageslider/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/package.json` & `gradio_imageslider-0.0.9/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/pnpm-lock.yaml` & `gradio_imageslider-0.0.9/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/example/Image.svelte` & `gradio_imageslider-0.0.9/frontend/example/Image.svelte`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/interactive/Image.svelte` & `gradio_imageslider-0.0.9/frontend/interactive/Image.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 		select: SelectData;
 	}>();
 
 	let dragging = false;
 
 	$: dispatch("drag", dragging);
 
-	$: console.log(value);
+	$: console.log("interactive", value);
 </script>
 
 <BlockLabel {show_label} Icon={Image} label={label || "Image"} />
 
 <div data-testid="image" class="image-container">
 	<Slider position={0.5} disabled>
 		<div class="upload-wrap">
```

### Comparing `gradio_imageslider-0.0.8/frontend/interactive/InteractiveImage.svelte` & `gradio_imageslider-0.0.9/frontend/interactive/InteractiveImage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/shared/Slider.svelte` & `gradio_imageslider-0.0.9/frontend/shared/Slider.svelte`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/shared/utils.ts` & `gradio_imageslider-0.0.9/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/frontend/static/ImagePreview.svelte` & `gradio_imageslider-0.0.9/frontend/static/ImagePreview.svelte`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 		let coordinates = get_coordinates_of_clicked_image(evt);
 		if (coordinates) {
 			dispatch("select", { index: coordinates, value: null });
 		}
 	};
 
 	let position = 0.5;
+
+	$: console.log("static:", value_);
 </script>
 
 <BlockLabel {show_label} Icon={Image} label={label || i18n("image.image")} />
 {#if value_ === null}
 	<Empty unpadded_box={true} size="large"><Image /></Empty>
 {:else}
 	<!-- <div class="icon-buttons">
```

### Comparing `gradio_imageslider-0.0.8/frontend/static/StaticImage.svelte` & `gradio_imageslider-0.0.9/frontend/static/StaticImage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_imageslider-0.0.8/pyproject.toml` & `gradio_imageslider-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_imageslider"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python library for easily interacting with trained machine learning models"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = [
   "machine learning",
   "reproducibility",
```

### Comparing `gradio_imageslider-0.0.8/PKG-INFO` & `gradio_imageslider-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_imageslider
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: gradio,gradio custom component,machine learning,reproducibility,visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

