# Comparing `tmp/jupyter_bokeh-4.0.3.tar.gz` & `tmp/jupyter_bokeh-4.0.4.tar.gz`

## Comparing `jupyter_bokeh-4.0.3.tar` & `jupyter_bokeh-4.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/.eslintignore
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/.eslintrc.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/.yarnrc.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/DEVGUIDE.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/MANIFEST.in
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/install.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh.json
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/package.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/setup.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/tsconfig.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/webpack.config.js
--rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/yarn.lock
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/conda.recipe/meta.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/examples/jupyter_interactors.ipynb
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/examples/jupyter_sliders.ipynb
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/examples/jupyter_widgets.ipynb
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/examples/notebook_comms.ipynb
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/examples/server_embed.ipynb
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/examples/static_plot.ipynb
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/_version.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/widgets.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/package.json
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
--rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js.LICENSE.txt
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/824.0516a74f23af97c034d1.js
--rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/remoteEntry.dcb3d6b182afad5c4f51.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/style.js
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/nbextension/extension.js
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/jupyter_bokeh/nbextension/index.js.LICENSE.txt
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/scripts/deploy.sh
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/extension.ts
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/index.ts
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/manager.ts
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/metadata.d.ts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/plugin.ts
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/renderer.ts
--rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/src/widgets.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/style/index.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/README.md
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.eslintignore
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.eslintrc.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.yarnrc.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/DEVGUIDE.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/MANIFEST.in
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/install.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh.json
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/package.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/setup.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/tsconfig.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/webpack.config.js
+-rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/yarn.lock
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/jupyter_interactors.ipynb
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/jupyter_sliders.ipynb
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/jupyter_widgets.ipynb
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/notebook_comms.ipynb
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/server_embed.ipynb
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/examples/static_plot.ipynb
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/_version.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/widgets.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/package.json
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
+-rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js.LICENSE.txt
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/824.a3a1e45ab4137dbaadb5.js
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/remoteEntry.352adabd3ad00a55dce4.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/style.js
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/nbextension/extension.js
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/jupyter_bokeh/nbextension/index.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/scripts/deploy.sh
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/extension.ts
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/index.ts
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/manager.ts
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/metadata.d.ts
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/plugin.ts
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/renderer.ts
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/src/widgets.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/style/index.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/README.md
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.4/PKG-INFO
```

### Comparing `jupyter_bokeh-4.0.3/.eslintrc.js` & `jupyter_bokeh-4.0.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/package.json` & `jupyter_bokeh-4.0.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'4.0.4'"}*

```diff
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.3"
+    "version": "4.0.4"
 }
```

### Comparing `jupyter_bokeh-4.0.3/tsconfig.json` & `jupyter_bokeh-4.0.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/webpack.config.js` & `jupyter_bokeh-4.0.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/yarn.lock` & `jupyter_bokeh-4.0.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/conda.recipe/meta.yaml` & `jupyter_bokeh-4.0.4/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/examples/jupyter_interactors.ipynb` & `jupyter_bokeh-4.0.4/examples/jupyter_interactors.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/examples/jupyter_sliders.ipynb` & `jupyter_bokeh-4.0.4/examples/jupyter_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/examples/jupyter_widgets.ipynb` & `jupyter_bokeh-4.0.4/examples/jupyter_widgets.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/examples/notebook_comms.ipynb` & `jupyter_bokeh-4.0.4/examples/notebook_comms.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/examples/server_embed.ipynb` & `jupyter_bokeh-4.0.4/examples/server_embed.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/examples/static_plot.ipynb` & `jupyter_bokeh-4.0.4/examples/static_plot.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/__init__.py` & `jupyter_bokeh-4.0.4/jupyter_bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/widgets.py` & `jupyter_bokeh-4.0.4/jupyter_bokeh/widgets.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/package.json` & `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9755291005291005%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.352adabd3ad00a55dce4.js'}}",*

 * * "'version'": "'4.0.4'"}*

```diff
@@ -36,15 +36,15 @@
         "{dist,lib}/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/bokeh/jupyter_bokeh",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.dcb3d6b182afad5c4f51.js",
+            "load": "static/remoteEntry.352adabd3ad00a55dce4.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_bokeh/labextension"
     },
     "keywords": [
         "jupyter",
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.3"
+    "version": "4.0.4"
 }
```

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js` & `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js` & `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/824.0516a74f23af97c034d1.js` & `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/824.a3a1e45ab4137dbaadb5.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -157,15 +157,15 @@
                         for (const s in e.roots) t[s] = i;
                         d(this._document, i, t)
                     }
                     this._document.on_change((e => this._change_event(e)))
                 }
                 _combine_events(e) {
                     const t = [];
-                    for (const s of this._msgs) e.kind != s.kind ? t.push(s) : "ModelChanged" == s.kind && "ModelChanged" == e.kind ? s.id == e.id && s.attr == e.attr || t.push(s) : "MessageSent" == s.kind && "MessageSent" == e.kind && (null != s.msg_data.event_values.model && s.msg_data.event_values.model.id == e.msg_data.event_values.model.id && s.msg_data.event_name == e.msg_data.event_name || t.push(s));
+                    for (const s of this._msgs) e.kind != s.kind ? t.push(s) : "ModelChanged" == s.kind && "ModelChanged" == e.kind ? s.model.id == e.model.id && s.attr == e.attr || t.push(s) : "MessageSent" == s.kind && "MessageSent" == e.kind && (null != s.msg_data.event_values.model && s.msg_data.event_values.model.id == e.msg_data.event_values.model.id && s.msg_data.event_name == e.msg_data.event_name || t.push(s));
                     return t.push(e), t
                 }
                 _send(e) {
                     !this._idle && this._combine && this.model.get("combine_events") ? this._msgs = this._combine_events(e) : (this._idle = !1, this.send(e))
                 }
                 _change_event(e) {
                     if (this._blocked) return void this._events.push(e);
@@ -230,12 +230,12 @@
                 },
                 autoStart: !0
             }
         },
         2288: (e, t) => {
             Object.assign(t, {
                 name: "@bokeh/jupyter_bokeh",
-                version: "4.0.3"
+                version: "4.0.4"
             })
         }
     }
 ]);
```

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/remoteEntry.dcb3d6b182afad5c4f51.js` & `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/remoteEntry.352adabd3ad00a55dce4.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -48,21 +48,21 @@
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         7: "2d4b977066efef2921dc",
         25: "a1f00326924633b92ed3",
         256: "3673b9e8accbe04f1c8a",
         805: "5070eeb32117fc99ba19",
-        824: "0516a74f23af97c034d1"
+        824: "a3a1e45ab4137dbaadb5"
     } [e] + ".js?v=" + {
         7: "2d4b977066efef2921dc",
         25: "a1f00326924633b92ed3",
         256: "3673b9e8accbe04f1c8a",
         805: "5070eeb32117fc99ba19",
-        824: "0516a74f23af97c034d1"
+        824: "a3a1e45ab4137dbaadb5"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -114,15 +114,15 @@
                         (!u || !u.loaded && (!o != !u.eager ? o : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     l = [];
-                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.3", (() => Promise.all([j.e(256), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(256)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.4", (() => Promise.all([j.e(256), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(256)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/labextension/static/third-party-licenses.json` & `jupyter_bokeh-4.0.4/jupyter_bokeh/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/jupyter_bokeh/nbextension/index.js.LICENSE.txt` & `jupyter_bokeh-4.0.4/jupyter_bokeh/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/src/manager.ts` & `jupyter_bokeh-4.0.4/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/src/plugin.ts` & `jupyter_bokeh-4.0.4/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/src/renderer.ts` & `jupyter_bokeh-4.0.4/src/renderer.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/src/widgets.ts` & `jupyter_bokeh-4.0.4/src/widgets.ts`

 * *Files 2% similar despite different names*

```diff
@@ -13,35 +13,38 @@
 type DocsJson = any
 type RenderItem = any
 type Document = any
 type DocumentChangedEvent = any
 type Receiver = any
 type Fragment = any
 type HasProps = any
-type Ref = any
 
 const { keys, values } = Object
 
 const version_range = `^${version}`
 
 export type RenderBundle = {
   docs_json: DocsJson
   render_items: RenderItem[]
   div: string
 }
 
+export interface Ref {
+  id: string
+}
+
 export interface DocumentChanged {
   event: 'jsevent'
   kind: string
 }
 
 export interface ModelChanged extends DocumentChanged {
   event: 'jsevent'
   kind: 'ModelChanged'
-  id: string
+  model: Ref
   new: unknown
   attr: string
 }
 
 export interface MessageSent extends DocumentChanged {
   event: 'jsevent'
   kind: 'MessageSent'
@@ -165,15 +168,15 @@
     new_msg: ModelChanged | MessageSent
   ): (ModelChanged | MessageSent)[] {
     const new_msgs = []
     for (const msg of this._msgs) {
       if (new_msg.kind != msg.kind) {
         new_msgs.push(msg)
       } else if (msg.kind == 'ModelChanged' && new_msg.kind == 'ModelChanged') {
-        if (msg.id != new_msg.id || msg.attr != new_msg.attr) {
+        if (msg.model.id != new_msg.model.id || msg.attr != new_msg.attr) {
           new_msgs.push(msg)
         }
       } else if (msg.kind == 'MessageSent' && new_msg.kind == 'MessageSent') {
         if (
           msg.msg_data.event_values.model == null ||
           msg.msg_data.event_values.model.id !=
           new_msg.msg_data.event_values.model.id ||
```

### Comparing `jupyter_bokeh-4.0.3/LICENSE.txt` & `jupyter_bokeh-4.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/README.md` & `jupyter_bokeh-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/pyproject.toml` & `jupyter_bokeh-4.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.3/PKG-INFO` & `jupyter_bokeh-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_bokeh
-Version: 4.0.3
+Version: 4.0.4
 Summary: A Jupyter extension for rendering Bokeh content.
 Project-URL: Homepage, https://github.com/bokeh/jupyter_bokeh
 Project-URL: Bug Tracker, https://github.com/bokeh/jupyter_bokeh/issues
 Project-URL: Repository, https://github.com/bokeh/jupyter_bokeh.git
 Author-email: Bokeh team <info@bokeh.org>
 License: Copyright (c) 2012 - 2020, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
```

