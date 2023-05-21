# Comparing `tmp/vule_magics-1.1.3.tar.gz` & `tmp/vule_magics-1.2.0.tar.gz`

## Comparing `vule_magics-1.1.3.tar` & `vule_magics-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vule_magics-1.1.3/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vule_magics-1.1.3/CHANGELOG.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 vule_magics-1.1.3/RELEASE.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 vule_magics-1.1.3/install.json
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 vule_magics-1.1.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vule_magics-1.1.3/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vule_magics-1.1.3/tsconfig.json
--rw-r--r--   0        0        0   217147 2020-02-02 00:00:00.000000 vule_magics-1.1.3/yarn.lock
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 vule_magics-1.1.3/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vule_magics-1.1.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 vule_magics-1.1.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vule_magics-1.1.3/style/index.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/_version.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/labextension/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/labextension/static/568.86f8cf51e32d5a4a98cb.js
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/labextension/static/remoteEntry.4bf4c81a69b56d83a0c3.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/sparksql/__init__.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/sparksql/sparksql.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 vule_magics-1.1.3/vule_magics/sparksql/widget.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vule_magics-1.1.3/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 vule_magics-1.1.3/LICENSE
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 vule_magics-1.1.3/README.md
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 vule_magics-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 vule_magics-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vule_magics-1.2.0/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vule_magics-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 vule_magics-1.2.0/RELEASE.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 vule_magics-1.2.0/install.json
+-rw-r--r--   0        0        0   538859 2020-02-02 00:00:00.000000 vule_magics-1.2.0/package-lock.json
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 vule_magics-1.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vule_magics-1.2.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vule_magics-1.2.0/tsconfig.json
+-rw-r--r--   0        0        0   190057 2020-02-02 00:00:00.000000 vule_magics-1.2.0/yarn.lock
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 vule_magics-1.2.0/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vule_magics-1.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 vule_magics-1.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vule_magics-1.2.0/style/index.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/_version.py
+-rw-r--r--   0        0        0    15107 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/colab/sparksql/__init__.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/labextension/package.json
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/labextension/static/568.56228813aa0df1f53f88.js
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/labextension/static/remoteEntry.151e76b9ce3f68cc9167.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/sparksql/__init__.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/sparksql/sparksql.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 vule_magics-1.2.0/vule_magics/sparksql/widget.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 vule_magics-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 vule_magics-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 vule_magics-1.2.0/README.md
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 vule_magics-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 vule_magics-1.2.0/PKG-INFO
```

### Comparing `vule_magics-1.1.3/RELEASE.md` & `vule_magics-1.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/package.json` & `vule_magics-1.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.2.0'"}*

```diff
@@ -163,9 +163,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.3"
+    "version": "1.2.0"
 }
```

### Comparing `vule_magics-1.1.3/tsconfig.json` & `vule_magics-1.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/vule_magics/labextension/package.json` & `vule_magics-1.2.0/vule_magics/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.151e76b9ce3f68cc9167.js'}}",*

 * * "'version'": "'1.2.0'"}*

```diff
@@ -96,15 +96,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/vule24/vule-jupyter-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4bf4c81a69b56d83a0c3.js",
+            "load": "static/remoteEntry.151e76b9ce3f68cc9167.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "vule_magics/labextension"
     },
     "keywords": [
         "jupyter",
@@ -168,9 +168,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.3"
+    "version": "1.2.0"
 }
```

### Comparing `vule_magics-1.1.3/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js` & `vule_magics-1.2.0/vule_magics/labextension/static/747.6b9eb3eb7bd07ac8fdef.js`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/vule_magics/labextension/static/remoteEntry.4bf4c81a69b56d83a0c3.js` & `vule_magics-1.2.0/vule_magics/labextension/static/remoteEntry.151e76b9ce3f68cc9167.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, b, g, m, y, w, S = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, g, m, b, y, w, S = {
             348: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,18 +43,18 @@
         }), r
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        568: "86f8cf51e32d5a4a98cb",
+        568: "56228813aa0df1f53f88",
         747: "6b9eb3eb7bd07ac8fdef"
     } [e] + ".js?v=" + {
-        568: "86f8cf51e32d5a4a98cb",
+        568: "56228813aa0df1f53f88",
         747: "6b9eb3eb7bd07ac8fdef"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => k.e(568).then((() => () => k(568))),
                         from: i,
                         eager: !1
                     })
-                })("vule-magics", "1.1.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vule-magics", "1.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -212,38 +212,38 @@
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, c = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, p = (e, r, t, n) => {
         "undefined" != typeof console && console.warn && console.warn(c(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, o) {
+    }, h = e => (e.loaded = 1, e.get()), g = (v = e => function(r, t, n, o) {
         var a = k.I(r);
         return a && a.then ? a.then(e.bind(e, r, k.S[r], t, n, o)) : e(r, k.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || u(r, t))))), g = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = {}, y = {
-        123: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        191: () => b("default", "@jupyterlab/cells", [1, 3, 6, 3])
+    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || u(r, t))))), m = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), b = {}, y = {
+        123: () => m("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        191: () => g("default", "@jupyterlab/cells", [1, 3, 6, 3])
     }, w = {
         568: [123, 191]
     }, k.f.consumes = (e, r) => {
         k.o(w, e) && w[e].forEach((e => {
-            if (k.o(m, e)) return r.push(m[e]);
+            if (k.o(b, e)) return r.push(b[e]);
             var t = r => {
-                    m[e] = 0, k.m[e] = t => {
+                    b[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete m[e], k.m[e] = t => {
+                    delete b[e], k.m[e] = t => {
                         throw delete k.c[e], r
                     }
                 };
             try {
                 var o = y[e]();
-                o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             466: 0
```

### Comparing `vule_magics-1.1.3/vule_magics/labextension/static/third-party-licenses.json` & `vule_magics-1.2.0/vule_magics/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/vule_magics/sparksql/sparksql.py` & `vule_magics-1.2.0/vule_magics/sparksql/sparksql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import print_function
 from IPython.core.magic import Magics, magics_class, cell_magic, line_magic
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
-from IPython import display
 from pyspark.sql import SparkSession
 from pyspark.sql.dataframe import DataFrame
 from string import Formatter
-import numpy as np
+
+import json
 
 from .widget import generate_output_widget, generate_classic_table
 
 
 @magics_class
 class SparkSQL(Magics):
 
@@ -22,42 +21,41 @@
     @argument('-n', '--num-rows', type=int, default=100)
     @argument('-c', '--classic', action='store_true', default=False)
     @cell_magic
     def sql(self, line, cell):
         self.create_temp_view_for_available_dataframe()
         
         args = parse_argstring(self.sql, line)
-        query_str = self.format_fillin_pyvar(cell)
+        query_str = rf'{self.format_fillin_pyvar(cell)}'
         
         sdf = self.spark.sql(query_str)
         if args.dataframe:
             self.shell.user_ns.update({args.dataframe: sdf})
         if not args.classic:
             return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe or None)
         else:
             return generate_classic_table(sdf, num_rows=args.num_rows)
 
 
-
     @magic_arguments()
     @argument('dataframe', metavar='DF', type=str, nargs='?')
     @argument('-n', '--num-rows', type=int, default=20)
     @argument('-c', '--classic', action='store_true', default=False)
     @line_magic
     def show(self, line):
         args = parse_argstring(self.sql, line)
+        if not args.dataframe:
+            raise ValueError('dataframe is required. Eg. `%show <dataframe>`')
         sdf = self.shell.user_ns.get(args.dataframe, None)
-        try:
-            if not args.classic:
-                return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe)
-            else:
-                return generate_classic_table(sdf, num_rows=args.num_rows)
-        except AttributeError as err:
-            display(err)
-            print("Input dataframe is not existed")
+        if not sdf:
+            raise NameError(f"Name '{args.dataframe}' is not defined")
+        if not args.classic:
+            return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe)
+        else:
+            return generate_classic_table(sdf, num_rows=args.num_rows)
 
 
     def create_temp_view_for_available_dataframe(self):
         for k, v in self.shell.user_ns.items():
             v.createOrReplaceTempView(k) if isinstance(v, DataFrame) else None
 
     def format_fillin_pyvar(self, source):
```

### Comparing `vule_magics-1.1.3/vule_magics/sparksql/widget.py` & `vule_magics-1.2.0/vule_magics/sparksql/widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         'display.max_rows', None, 
         'display.max_columns', None, 
         'display.max_colwidth', None
     ):
         return ipd.HTML(
             "<div style='max-height: 650px'>" +
             sdf.limit(num_rows).toPandas().style
-                .format(precision=3, thousands=",", decimal=".")
+                .format(na_rep='null', precision=3, thousands=",", decimal=".")
                 .set_table_styles([
                     {'selector': 'thead th', 'props': 'position: sticky; top: 0; z-index: 1; background-color: var(--jp-layout-color0); border-bottom: var(--jp-border-width) solid var(--jp-border-color1) !important;'},
                     {'selector': 'thead th:first-child', 'props': 'position: sticky; left: 0; z-index: 2; background-color: var(--jp-layout-color0);'},
                     {'selector': 'tbody th', 'props': 'position: sticky; left: 0; z-index: 1; background-color: inherit;'},
                 ])
                 .set_table_attributes(
                     'style="border-collapse:separate"'
@@ -37,15 +37,15 @@
     ):
         dataframe = copy.deepcopy(sdf.limit(num_rows).toPandas())
         return (
             dataframe,
             ipd.HTML(
                 "<div style='max-height: 650px'>" +
                 dataframe.style
-                    .format(precision=3, thousands=",", decimal=".")
+                    .format(na_rep='null', precision=3, thousands=",", decimal=".")
                     .set_table_styles([
                         {'selector': 'thead th', 'props': 'position: sticky; top: 0; z-index: 1; background-color: var(--jp-layout-color0); border-bottom: var(--jp-border-width) solid var(--jp-border-color1) !important;'},
                         {'selector': 'thead th:first-child', 'props': 'position: sticky; left: 0; z-index: 2; background-color: var(--jp-layout-color0);'},
                         {'selector': 'tbody th', 'props': 'position: sticky; left: 0; z-index: 1; background-color: inherit;'},
                     ])
                     .set_table_attributes(
                         'style="border-collapse:separate"'
@@ -116,25 +116,25 @@
         disabled=False,
         button_style='',
         icon='table',
         layout=layout_btn_render_type)
     btn_chart_line = w.Button(
         disabled=False,
         button_style='',
-        icon='line-chart',
+        icon='chart-line',
         layout=layout_btn_render_type)
     btn_chart_bar = w.Button(
         disabled=False,
         button_style='',
-        icon='bar-chart',
+        icon='chart-bar',
         layout=layout_btn_render_type)
     btn_chart_scatter = w.Button(
         disabled=False,
         button_style='',
-        icon='scatter-chart',
+        icon='chart-scatter',
         layout=layout_btn_render_type)
     btn_save_csv = w.Button(
         description='Save as CSV',
         disabled=False,
         button_style='warning',
         icon='save',
         layout=w.Layout(width='auto', margin='1px 2px 2px 2px'))
@@ -218,15 +218,15 @@
         if b.icon == 'table':
             with console:
                 ipd.clear_output()
             with output:
                 ipd.clear_output(wait=True)
                 ipd.display(table_html) 
         else:
-            state['current_render'] = b.icon.split('-')[0]
+            state['current_render'] = b.icon.split('-')[-1]
             with console:
                 ipd.clear_output(wait=True)
                 ipd.display(console_box)
             plot(
                 output, 
                 current_render=state['current_render'],
                 template=state['template'],
```

### Comparing `vule_magics-1.1.3/.gitignore` & `vule_magics-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/LICENSE` & `vule_magics-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/README.md` & `vule_magics-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vule_magics-1.1.3/pyproject.toml` & `vule_magics-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
+    'ipywidgets == 7.7.2',
+    'jupyterlab-widgets == 1.1.4',
+    'pandas >= 2.0.0',
+    'plotly'
+
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
```

### Comparing `vule_magics-1.1.3/PKG-INFO` & `vule_magics-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vule_magics
-Version: 1.1.3
+Version: 1.2.0
 Summary: JupyterLab MagicCommands Extension
 Project-URL: Homepage, https://github.com/vule24/vule-jupyter-extensions
 Project-URL: Bug Tracker, https://github.com/vule24/vule-jupyter-extensions/issues
 Project-URL: Repository, https://github.com/vule24/vule-jupyter-extensions.git
 Author-email: Vu Le <ltnv24@gmail.com>
 License: BSD 3-Clause License
         
@@ -46,14 +46,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Requires-Dist: ipywidgets==7.7.2
+Requires-Dist: jupyterlab-widgets==1.1.4
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: plotly
 Description-Content-Type: text/markdown
 
 # vule-magics
 
 [![Github Actions Status](https://github.com/vule24/vule-jupyter-extensions/actions/workflows/publish-release.vule-magics.yml/badge.svg)](https://github.com/vule24/vule-jupyter-extensions/actions/workflows/publish-release.vule-magics.yml)
 JupyterLab MagicCommands Extension
```

