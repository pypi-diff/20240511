# Comparing `tmp/dash_oflog_components-0.0.8.tar.gz` & `tmp/dash_oflog_components-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_oflog_components-0.0.8.tar", last modified: Mon Feb 26 15:52:40 2024, max compression
+gzip compressed data, was "dash_oflog_components-0.0.9.tar", last modified: Mon Feb 26 16:03:54 2024, max compression
```

## Comparing `dash_oflog_components-0.0.8.tar` & `dash_oflog_components-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 15:52:40.778935 dash_oflog_components-0.0.8/
--rw-rw-rw-   0        0        0        0 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      454 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4185 2024-02-26 15:52:40.778935 dash_oflog_components-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3842 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 15:52:40.769920 dash_oflog_components-0.0.8/dash_oflog_components/
--rw-rw-rw-   0        0        0     1149 2024-02-26 15:47:57.000000 dash_oflog_components-0.0.8/dash_oflog_components/DualInput.py
--rw-rw-rw-   0        0        0      924 2024-02-16 16:02:44.000000 dash_oflog_components-0.0.8/dash_oflog_components/DualInput2.py
--rw-rw-rw-   0        0        0     1541 2024-02-21 15:50:45.000000 dash_oflog_components-0.0.8/dash_oflog_components/Test.py
--rw-rw-rw-   0        0        0      862 2024-02-21 15:50:45.000000 dash_oflog_components-0.0.8/dash_oflog_components/Test2.py
--rw-rw-rw-   0        0        0     2604 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.8/dash_oflog_components/__init__.py
--rw-rw-rw-   0        0        0       67 2024-02-26 15:47:57.000000 dash_oflog_components-0.0.8/dash_oflog_components/_imports_.py
--rw-rw-rw-   0        0        0    13273 2024-02-26 15:47:53.000000 dash_oflog_components-0.0.8/dash_oflog_components/dash_oflog_components.min.js
--rw-rw-rw-   0        0        0    43035 2024-02-26 15:47:53.000000 dash_oflog_components-0.0.8/dash_oflog_components/dash_oflog_components.min.js.map
--rw-rw-rw-   0        0        0     1349 2024-02-26 15:47:57.000000 dash_oflog_components-0.0.8/dash_oflog_components/metadata.json
--rw-rw-rw-   0        0        0     2494 2024-02-26 15:47:56.000000 dash_oflog_components-0.0.8/dash_oflog_components/package-info.json
-drwxrwxrwx   0        0        0        0 2024-02-26 15:52:40.776935 dash_oflog_components-0.0.8/dash_oflog_components.egg-info/
--rw-rw-rw-   0        0        0     4185 2024-02-26 15:52:40.000000 dash_oflog_components-0.0.8/dash_oflog_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-02-26 15:52:40.000000 dash_oflog_components-0.0.8/dash_oflog_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 15:52:40.000000 dash_oflog_components-0.0.8/dash_oflog_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-02-26 15:52:40.000000 dash_oflog_components-0.0.8/dash_oflog_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2494 2024-02-26 15:52:21.000000 dash_oflog_components-0.0.8/package.json
--rw-rw-rw-   0        0        0       42 2024-02-26 15:52:40.778935 dash_oflog_components-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-26 16:03:54.649122 dash_oflog_components-0.0.9/
+-rw-rw-rw-   0        0        0        0 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      454 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4185 2024-02-26 16:03:54.648118 dash_oflog_components-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3842 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-26 16:03:54.641115 dash_oflog_components-0.0.9/dash_oflog_components/
+-rw-rw-rw-   0        0        0     1149 2024-02-26 16:02:12.000000 dash_oflog_components-0.0.9/dash_oflog_components/DualInput.py
+-rw-rw-rw-   0        0        0      924 2024-02-16 16:02:44.000000 dash_oflog_components-0.0.9/dash_oflog_components/DualInput2.py
+-rw-rw-rw-   0        0        0     1541 2024-02-21 15:50:45.000000 dash_oflog_components-0.0.9/dash_oflog_components/Test.py
+-rw-rw-rw-   0        0        0      862 2024-02-21 15:50:45.000000 dash_oflog_components-0.0.9/dash_oflog_components/Test2.py
+-rw-rw-rw-   0        0        0     2604 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.9/dash_oflog_components/__init__.py
+-rw-rw-rw-   0        0        0       67 2024-02-26 16:02:12.000000 dash_oflog_components-0.0.9/dash_oflog_components/_imports_.py
+-rw-rw-rw-   0        0        0    13266 2024-02-26 16:02:09.000000 dash_oflog_components-0.0.9/dash_oflog_components/dash_oflog_components.min.js
+-rw-rw-rw-   0        0        0    42975 2024-02-26 16:02:09.000000 dash_oflog_components-0.0.9/dash_oflog_components/dash_oflog_components.min.js.map
+-rw-rw-rw-   0        0        0     1349 2024-02-26 16:02:12.000000 dash_oflog_components-0.0.9/dash_oflog_components/metadata.json
+-rw-rw-rw-   0        0        0     2494 2024-02-26 16:02:11.000000 dash_oflog_components-0.0.9/dash_oflog_components/package-info.json
+drwxrwxrwx   0        0        0        0 2024-02-26 16:03:54.647125 dash_oflog_components-0.0.9/dash_oflog_components.egg-info/
+-rw-rw-rw-   0        0        0     4185 2024-02-26 16:03:54.000000 dash_oflog_components-0.0.9/dash_oflog_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-02-26 16:03:54.000000 dash_oflog_components-0.0.9/dash_oflog_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-26 16:03:54.000000 dash_oflog_components-0.0.9/dash_oflog_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-02-26 16:03:54.000000 dash_oflog_components-0.0.9/dash_oflog_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2494 2024-02-26 16:03:31.000000 dash_oflog_components-0.0.9/package.json
+-rw-rw-rw-   0        0        0       42 2024-02-26 16:03:54.649122 dash_oflog_components-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-02-15 14:43:22.000000 dash_oflog_components-0.0.9/setup.py
```

### Comparing `dash_oflog_components-0.0.8/PKG-INFO` & `dash_oflog_components-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_oflog_components
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dash react components for use in oflog data products
 Home-page: UNKNOWN
 Author: Haydn Jenkins <haydn.jenkins@levellingup.gov.uk>
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
```

### Comparing `dash_oflog_components-0.0.8/README.md` & `dash_oflog_components-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/DualInput.py` & `dash_oflog_components-0.0.9/dash_oflog_components/DualInput.py`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/DualInput2.py` & `dash_oflog_components-0.0.9/dash_oflog_components/DualInput2.py`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/Test.py` & `dash_oflog_components-0.0.9/dash_oflog_components/Test.py`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/Test2.py` & `dash_oflog_components-0.0.9/dash_oflog_components/Test2.py`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/__init__.py` & `dash_oflog_components-0.0.9/dash_oflog_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/dash_oflog_components.min.js` & `dash_oflog_components-0.0.9/dash_oflog_components/dash_oflog_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -239,15 +239,15 @@
         var a = jsonpScriptSrc;
         jsonpScriptSrc = function(n) {
             var e, t = (e = o(), /\/_dash-component-suites\//.test(e.src)),
                 r = a(n);
             if (!t) return r;
             var i = r.split("/"),
                 s = i.slice(-1)[0].split(".");
-            return s.splice(1, 0, "v0_0_7m1708962473"), i.splice(-1, 1, s.join(".")), i.join("/")
+            return s.splice(1, 0, "v0_0_8m1708963329"), i.splice(-1, 1, s.join(".")), i.join("/")
         }
     }
     t.nc = void 0;
     var i = {};
     (() => {
         t.r(i), t.d(i, {
             DualInput: () => x
@@ -338,16 +338,16 @@
             for (var t = 0, r = new Array(e); t < e; t++) r[t] = n[t];
             return r
         }
 
         function B(t) {
             var r = t.id,
                 o = t.options,
-                i = t.setProps,
-                s = t.initialValue,
+                i = t.value,
+                s = t.setProps,
                 c = (t.label, C((0, n.useState)(""), 2)),
                 l = c[0],
                 u = c[1],
                 p = C((0, n.useState)(0), 2),
                 d = p[0],
                 f = p[1],
                 A = C((0, n.useState)([]), 2),
@@ -358,30 +358,30 @@
                 h = b[1],
                 y = C((0, n.useState)(!1), 2),
                 I = y[0],
                 B = y[1],
                 x = C((0, n.useState)(!1), 2),
                 k = x[0],
                 E = x[1];
-            s.length > 0 && u(s);
+            i.length > 0 && u(i);
             var w = function(n) {
                 n.target.closest(".input-container") || h(!1)
             };
             return e().useEffect((function() {
                 return document.body.addEventListener("click", w),
                     function() {
                         document.body.removeEventListener("click", w)
                     }
             }), []), e().createElement("div", null, e().createElement("div", {
                 className: "input-container"
             }, e().createElement("input", {
                 id: r,
                 className: "dual-input ".concat(k ? "focused" : ""),
                 onKeyDown: function(n) {
-                    if (13 === n.keyCode) u(v[d].label), i({
+                    if (13 === n.keyCode) u(v[d].label), s({
                         value: v[d].value,
                         label: v[d].label
                     }), h(!1), f(0);
                     else if (38 === n.keyCode) {
                         if (0 === d) return;
                         f(d - 1)
                     } else if (40 === n.keyCode) {
@@ -430,15 +430,15 @@
             }, v.map((function(n, t) {
                 var r = "suggestion";
                 return t === d && (r = "".concat(r, " active-suggestion")), t % 2 != 0 && (r = "".concat(r, " odd-suggestion")), e().createElement("li", {
                     key: t,
                     "data-key": t,
                     className: r,
                     onMouseDown: function(n) {
-                        return (e = n).preventDefault(), u(e.currentTarget.dataset.label), i({
+                        return (e = n).preventDefault(), u(e.currentTarget.dataset.label), s({
                             value: e.currentTarget.dataset.value,
                             label: e.currentTarget.dataset.label
                         }), void h(!1);
                         var e
                     },
                     onMouseEnter: function(n) {
                         return e = n.target, t = parseInt(e.getAttribute("data-key")), void f(t);
```

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/dash_oflog_components.min.js.map` & `dash_oflog_components-0.0.9/dash_oflog_components/dash_oflog_components.min.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9163375027430327%*

 * *Differences: {"'mappings'": "'wFAGIA,E,MAA0B,GAA4B,KAE1DA,EAAwBC,KAAK,CAACC,EAAOC,GAAI,qzCAmEtC,GAAG,CAAC,QAAU,EAAE,QAAU,CAAC,6CAA6C,MAAQ,GAAG,SAAW,6iBAA6iB,eAAiB,CAAC,47CAA47C,WAAa,MAEzmE,S,UCpEAD,EAAOE,QAAU,SAAUC,GACzB,IAAIC,EAAO,GA4EX,OAzEAA,EAAKC,SAAW,WACd,OAAOC,KAAKC,KAAI,SAAUC,GACxB,IAAIC,EAAU,GACVC,OAA+B,IAAZF,EAAK,GAoB5B,OAnBIA,EAAK,KACPC,GAAW,cAAcE,OAAOH,EAAK,GAAI,QAEvCA,EAAK,KACPC,GAAW,UAAUE,OAAOH,EAAK,GAAI,OAEnCE,IACFD,GAAW,SAASE,OAAOH,EAAK,GAAGI,OAAS,EAAI,IAAID,OAAOH,EAAK,IAAM,GAAI,OAE5EC,GAAWN,EAAuBK,GAC9BE […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_oflog_components.min.js",
-    "mappings": "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",
+    "mappings": "wFAGIA,E,MAA0B,GAA4B,KAE1DA,EAAwBC,KAAK,CAACC,EAAOC,GAAI,qzCAmEtC,GAAG,CAAC,QAAU,EAAE,QAAU,CAAC,6CAA6C,MAAQ,GAAG,SAAW,6iBAA6iB,eAAiB,CAAC,47CAA47C,WAAa,MAEzmE,S,UCpEAD,EAAOE,QAAU,SAAUC,GACzB,IAAIC,EAAO,GA4EX,OAzEAA,EAAKC,SAAW,WACd,OAAOC,KAAKC,KAAI,SAAUC,GACxB,IAAIC,EAAU,GACVC,OAA+B,IAAZF,EAAK,GAoB5B,OAnBIA,EAAK,KACPC,GAAW,cAAcE,OAAOH,EAAK,GAAI,QAEvCA,EAAK,KACPC,GAAW,UAAUE,OAAOH,EAAK,GAAI,OAEnCE,IACFD,GAAW,SAASE,OAAOH,EAAK,GAAGI,OAAS,EAAI,IAAID,OAAOH,EAAK,IAAM,GAAI,OAE5EC,GAAWN,EAAuBK,GAC9BE,IACFD,GAAW,KAETD,EAAK,KACPC,GAAW,KAETD,EAAK,KACPC,GAAW,KAENA,CACT,IAAGI,KAAK,GACV,EAGAT,EAAKU,EAAI,SAAWC,EAASC,EAAOC,EAAQC,EAAUC,GAC7B,iBAAZJ,IACTA,EAAU,CAAC,CAAC,KAAMA,OAASK,KAE7B,IAAIC,EAAyB,CAAC,EAC9B,GAAIJ,EACF,IAAK,IAAIK,EAAI,EAAGA,EAAIhB,KAAKM,OAAQU,IAAK,CACpC,IAAIrB,EAAKK,KAAKgB,GAAG,GACP,MAANrB,IACFoB,EAAuBpB,IAAM,EAEjC,CAEF,IAAK,IAAIsB,EAAK,EAAGA,EAAKR,EAAQH,OAAQW,IAAM,CAC1C,IAAIf,EAAO,GAAGG,OAAOI,EAAQQ,IACzBN,GAAUI,EAAuBb,EAAK,WAGrB,IAAVW,SACc,IAAZX,EAAK,KAGdA,EAAK,GAAK,SAASG,OAAOH,EAAK,GAAGI,OAAS,EAAI,IAAID,OAAOH,EAAK,IAAM,GAAI,MAAMG,OAAOH,EAAK,GAAI,MAF/FA,EAAK,GAAKW,GAMVH,IACGR,EAAK,IAGRA,EAAK,GAAK,UAAUG,OAAOH,EAAK,GAAI,MAAMG,OAAOH,EAAK,GAAI,KAC1DA,EAAK,GAAKQ,GAHVR,EAAK,GAAKQ,GAMVE,IACGV,EAAK,IAGRA,EAAK,GAAK,cAAcG,OAAOH,EAAK,GAAI,OAAOG,OAAOH,EAAK,GAAI,KAC/DA,EAAK,GAAKU,GAHVV,EAAK,GAAK,GAAGG,OAAOO,IAMxBd,EAAKL,KAAKS,GACZ,CACF,EACOJ,CACT,C,UClFAJ,EAAOE,QAAU,SAAUM,GACzB,IAAIC,EAAUD,EAAK,GACfgB,EAAahB,EAAK,GACtB,IAAKgB,EACH,OAAOf,EAET,GAAoB,mBAATgB,KAAqB,CAC9B,IAAIC,EAASD,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUN,MACzDO,EAAO,+DAA+DpB,OAAOe,GAC7EM,EAAgB,OAAOrB,OAAOoB,EAAM,OACxC,MAAO,CAACtB,GAASE,OAAO,CAACqB,IAAgBnB,KAAK,KAChD,CACA,MAAO,CAACJ,GAASI,KAAK,KACxB,C,SCbA,IAAIoB,EAAc,GAClB,SAASC,EAAqBC,GAE5B,IADA,IAAIC,GAAU,EACLtB,EAAI,EAAGA,EAAImB,EAAYrB,OAAQE,IACtC,GAAImB,EAAYnB,GAAGqB,aAAeA,EAAY,CAC5CC,EAAStB,EACT,KACF,CAEF,OAAOsB,CACT,CACA,SAASC,EAAajC,EAAMkC,GAG1B,IAFA,IAAIC,EAAa,CAAC,EACdC,EAAc,GACT1B,EAAI,EAAGA,EAAIV,EAAKQ,OAAQE,IAAK,CACpC,IAAIN,EAAOJ,EAAKU,GACZb,EAAKqC,EAAQG,KAAOjC,EAAK,GAAK8B,EAAQG,KAAOjC,EAAK,GAClDkC,EAAQH,EAAWtC,IAAO,EAC1BkC,EAAa,GAAGxB,OAAOV,EAAI,KAAKU,OAAO+B,GAC3CH,EAAWtC,GAAMyC,EAAQ,EACzB,IAAIC,EAAoBT,EAAqBC,GACzCS,EAAM,CACRC,IAAKrC,EAAK,GACVQ,MAAOR,EAAK,GACZsC,UAAWtC,EAAK,GAChBU,SAAUV,EAAK,GACfW,MAAOX,EAAK,IAEd,IAA2B,IAAvBmC,EACFV,EAAYU,GAAmBI,aAC/Bd,EAAYU,GAAmBK,QAAQJ,OAClC,CACL,IAAII,EAAUC,EAAgBL,EAAKN,GACnCA,EAAQY,QAAUpC,EAClBmB,EAAYkB,OAAOrC,EAAG,EAAG,CACvBqB,WAAYA,EACZa,QAASA,EACTD,WAAY,GAEhB,CACAP,EAAYzC,KAAKoC,EACnB,CACA,OAAOK,CACT,CACA,SAASS,EAAgBL,EAAKN,GAC5B,IAAIc,EAAMd,EAAQe,OAAOf,GAYzB,OAXAc,EAAIE,OAAOV,GACG,SAAiBW,GAC7B,GAAIA,EAAQ,CACV,GAAIA,EAAOV,MAAQD,EAAIC,KAAOU,EAAOvC,QAAU4B,EAAI5B,OAASuC,EAAOT,YAAcF,EAAIE,WAAaS,EAAOrC,WAAa0B,EAAI1B,UAAYqC,EAAOpC,QAAUyB,EAAIzB,MACzJ,OAEFiC,EAAIE,OAAOV,EAAMW,EACnB,MACEH,EAAII,QAER,CAEF,CACAxD,EAAOE,QAAU,SAAUE,EAAMkC,GAG/B,IAAImB,EAAkBpB,EADtBjC,EAAOA,GAAQ,GADfkC,EAAUA,GAAW,CAAC,GAGtB,OAAO,SAAgBoB,GACrBA,EAAUA,GAAW,GACrB,IAAK,IAAI5C,EAAI,EAAGA,EAAI2C,EAAgB7C,OAAQE,IAAK,CAC/C,IACI6C,EAAQzB,EADKuB,EAAgB3C,IAEjCmB,EAAY0B,GAAOZ,YACrB,CAEA,IADA,IAAIa,EAAqBvB,EAAaqB,EAASpB,GACtCuB,EAAK,EAAGA,EAAKJ,EAAgB7C,OAAQiD,IAAM,CAClD,IACIC,EAAS5B,EADKuB,EAAgBI,IAEK,IAAnC5B,EAAY6B,GAAQf,aACtBd,EAAY6B,GAAQd,UACpBf,EAAYkB,OAAOW,EAAQ,GAE/B,CACAL,EAAkBG,CACpB,CACF,C,UCjFA,IAAIG,EAAO,CAAC,EA+BZ/D,EAAOE,QAPP,SAA0B8D,EAAQC,GAChC,IAAIC,EAtBN,SAAmBA,GACjB,QAA4B,IAAjBH,EAAKG,GAAyB,CACvC,IAAIC,EAAcC,SAASC,cAAcH,GAGzC,GAAII,OAAOC,mBAAqBJ,aAAuBG,OAAOC,kBAC5D,IAGEJ,EAAcA,EAAYK,gBAAgBC,IAC5C,CAAE,MAAOC,GAEPP,EAAc,IAChB,CAEFJ,EAAKG,GAAUC,CACjB,CACA,OAAOJ,EAAKG,EACd,CAIeS,CAAUX,GACvB,IAAKE,EACH,MAAM,IAAIU,MAAM,2GAElBV,EAAOW,YAAYZ,EACrB,C,UCvBAjE,EAAOE,QANP,SAA4BoC,GAC1B,IAAIwC,EAAUV,SAASW,cAAc,SAGrC,OAFAzC,EAAQ0C,cAAcF,EAASxC,EAAQ2C,YACvC3C,EAAQ0B,OAAOc,EAASxC,EAAQA,SACzBwC,CACT,C,eCCA9E,EAAOE,QANP,SAAwCgF,GACtC,IAAIC,EAAmD,KACnDA,GACFD,EAAaE,aAAa,QAASD,EAEvC,C,UCoDAnF,EAAOE,QAjBP,SAAgBoC,GACd,GAAwB,oBAAb8B,SACT,MAAO,CACLd,OAAQ,WAAmB,EAC3BE,OAAQ,WAAmB,GAG/B,IAAI0B,EAAe5C,EAAQ+C,mBAAmB/C,GAC9C,MAAO,CACLgB,OAAQ,SAAgBV,IAjD5B,SAAesC,EAAc5C,EAASM,GACpC,IAAIC,EAAM,GACND,EAAI1B,WACN2B,GAAO,cAAclC,OAAOiC,EAAI1B,SAAU,QAExC0B,EAAI5B,QACN6B,GAAO,UAAUlC,OAAOiC,EAAI5B,MAAO,OAErC,IAAIN,OAAiC,IAAdkC,EAAIzB,MACvBT,IACFmC,GAAO,SAASlC,OAAOiC,EAAIzB,MAAMP,OAAS,EAAI,IAAID,OAAOiC,EAAIzB,OAAS,GAAI,OAE5E0B,GAAOD,EAAIC,IACPnC,IACFmC,GAAO,KAELD,EAAI5B,QACN6B,GAAO,KAELD,EAAI1B,WACN2B,GAAO,KAET,IAAIC,EAAYF,EAAIE,UAChBA,GAA6B,oBAATrB,OACtBoB,GAAO,uDAAuDlC,OAAOc,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUgB,MAAe,QAKtIR,EAAQgD,kBAAkBzC,EAAKqC,EAAc5C,EAAQA,QACvD,CAoBMiD,CAAML,EAAc5C,EAASM,EAC/B,EACAY,OAAQ,YArBZ,SAA4B0B,GAE1B,GAAgC,OAA5BA,EAAaM,WACf,OAAO,EAETN,EAAaM,WAAWC,YAAYP,EACtC,CAgBMQ,CAAmBR,EACrB,EAEJ,C,UC9CAlF,EAAOE,QAVP,SAA2B2C,EAAKqC,GAC9B,GAAIA,EAAaS,WACfT,EAAaS,WAAWC,QAAU/C,MAC7B,CACL,KAAOqC,EAAaW,YAClBX,EAAaO,YAAYP,EAAaW,YAExCX,EAAaL,YAAYT,SAAS0B,eAAejD,GACnD,CACF,C,GCXIkD,EAA2B,CAAC,EAGhC,SAASC,EAAoBC,GAE5B,IAAIC,EAAeH,EAAyBE,GAC5C,QAAqB7E,IAAjB8E,EACH,OAAOA,EAAahG,QAGrB,IAAIF,EAAS+F,EAAyBE,GAAY,CACjDhG,GAAIgG,EAEJ/F,QAAS,CAAC,GAOX,OAHAiG,EAAoBF,GAAUjG,EAAQA,EAAOE,QAAS8F,GAG/ChG,EAAOE,OACf,CCrBA8F,EAAoBI,EAAKpG,IACxB,IAAIqG,EAASrG,GAAUA,EAAOsG,WAC7B,IAAOtG,EAAiB,QACxB,IAAM,EAEP,OADAgG,EAAoBO,EAAEF,EAAQ,CAAEG,EAAGH,IAC5BA,CAAM,ECLdL,EAAoBO,EAAI,CAACrG,EAASuG,KACjC,IAAI,IAAIC,KAAOD,EACXT,EAAoBW,EAAEF,EAAYC,KAASV,EAAoBW,EAAEzG,EAASwG,IAC5EE,OAAOC,eAAe3G,EAASwG,EAAK,CAAEI,YAAY,EAAMC,IAAKN,EAAWC,IAE1E,ECNDV,EAAoBW,EAAI,CAAC/D,EAAKoE,IAAUJ,OAAOK,UAAUC,eAAeC,KAAKvE,EAAKoE,GCClFhB,EAAoBoB,EAAKlH,IACH,oBAAXmH,QAA0BA,OAAOC,aAC1CV,OAAOC,eAAe3G,EAASmH,OAAOC,YAAa,CAAEC,MAAO,WAE7DX,OAAOC,eAAe3G,EAAS,aAAc,CAAEqH,OAAO,GAAO,ECL9D,IA4BYC,EA5BRC,EAAmB,WACnB,IAAIC,EAAStD,SAASuD,cACtB,IAAKD,EAAQ,CAOT,IAHA,IAAIE,EAAcxD,SAASyD,qBAAqB,UAC5CC,EAAU,GAELhH,EAAI,EAAGA,EAAI8G,EAAYhH,OAAQE,IACpCgH,EAAQ/H,KAAK6H,EAAY9G,IAI7B4G,GADAI,EAAUA,EAAQC,QAAO,SAASC,GAAK,OAAQA,EAAEC,QAAUD,EAAEE,OAASF,EAAEG,WAAa,KACpEC,OAAO,GAAG,EAC/B,CAEA,OAAOV,CACX,EAkBA,GAZAd,OAAOC,eAAeb,EAAqB,IAAK,CAC5Ce,KAGQS,EAFSC,IAEIY,IAAIC,MAAM,KAAKF,MAAM,GAAI,GAAGvH,KAAK,KAAO,IAElD,WACH,OAAO2G,CACX,KAIsB,oBAAnBe,eAAgC,CACvC,IAAIC,EAAqBD,eACzBA,eAAiB,SAASE,GACtB,IAnBqBf,EAoBjBgB,GApBiBhB,EAmBRD,IAlBV,6BAA6BkB,KAAKjB,EAAOW,MAqBxCA,EAAMG,EAAmBC,GAE7B,IAAIC,EACA,OAAOL,EAGX,IAAIO,EAAeP,EAAIC,MAAM,KACzBO,EAAgBD,EAAaR,OAAO,GAAG,GAAGE,MAAM,KAKpD,OAHAO,EAAc1F,OAAO,EAAG,EAAG,qBAC3ByF,EAAazF,QAAQ,EAAG,EAAG0F,EAAchI,KAAK,MAEvC+H,EAAa/H,KAAK,IAC7B,CACJ,CCxDAmF,EAAoB8C,QAAK1H,E,+CCAzB,MAAM,EAA+BkD,OAAc,M,aCAnD,MAAM,EAA+BA,OAAkB,U,aCwBvD,MCAA,EAtBA,SAAwBiD,EAAOjF,EAASyG,GAIpC,GAFwB,KAAKJ,KAAKpB,IDJhBS,ECQDT,EDPXyB,EAAS,sCAAHrI,OAAyCqH,EAAC,iBAC/CiB,MAAMD,GACRE,MAAK,SAACC,GAEH,IAAKA,EAASC,GACV,MAAM,IAAIxE,MAAM,+BAGpB,OAAOuE,EAASE,MACpB,IACCH,MAAK,SAACnH,GAEH,OAAOA,EAAKK,MAChB,IAAE,OACK,SAACkH,GAEJC,QAAQD,MACJ,gDACAA,EAER,KCboBJ,MAAK,SAACM,GACtB,IAAIC,EAAsBD,EAAUjJ,KAAI,SAACmJ,GAAQ,MAAM,CACnDC,MAAOD,EACPnC,MAAOmC,EACV,IACDX,EAAeU,EACnB,QACG,CAEH,IAAMG,EAAkBtH,EAAQyF,QAAO,SAAC8B,GAAM,OAC1CA,EAAc,MAAEC,WAAWvC,EAAM,IAErCwB,EAAea,EACnB,CDrBJ,IAAsB5B,EACZgB,CCqBV,E,uHCXI1G,EAAU,CAAC,E,khCCJf,SAASyH,EAASC,GAAwC,IAAtC/J,EAAE+J,EAAF/J,GAAIqC,EAAO0H,EAAP1H,QAASiF,EAAKyC,EAALzC,MAAO0C,EAAQD,EAARC,SAEUC,GAFKF,EAALL,MAEAQ,GAAZC,EAAAA,EAAAA,UAAS,IAAG,IAAvCC,EAASH,EAAA,GAAEI,EAAYJ,EAAA,GAC6BK,EAAAJ,GAAXC,EAAAA,EAAAA,UAAS,GAAE,GAApDI,EAAgBD,EAAA,GAAEE,EAAmBF,EAAA,GACMG,EAAAP,GAAZC,EAAAA,EAAAA,UAAS,IAAG,GAA3CO,EAAWD,EAAA,GAAE3B,EAAc2B,EAAA,GAC2BE,EAAAT,GAAfC,EAAAA,EAAAA,WAAS,GAAM,GAAtDS,EAAeD,EAAA,GAAEE,EAAkBF,EAAA,GACSG,EAAAZ,GAAfC,EAAAA,EAAAA,WAAS,GAAM,GAA5CY,EAAUD,EAAA,GAAEE,EAAaF,EAAA,GACSG,EAAAf,GAAfC,EAAAA,EAAAA,WAAS,GAAM,GAAlCe,EAAKD,EAAA,GAAEE,EAAQF,EAAA,GAGlB3D,EAAM3G,OAAS,GACf0J,EAAa/C,GA4GjB,IAAM8D,EAAqB,SAAC3G,GACnBA,EAAER,OAAOoH,QAAQ,qBAClBR,GAAmB,EAE3B,EAWA,OARAS,IAAAA,WAAgB,WAEZ,OADAnH,SAASoH,KAAKC,iBAAiB,QAASJ,GACjC,WACHjH,SAASoH,KAAKE,oBAAoB,QAASL,EAC/C,CACJ,GAAG,IAICE,IAAAA,cAAA,WACIA,IAAAA,cAAA,OAAKI,UAAU,mBACXJ,IAAAA,cAAA,SACItL,GAAIA,EACJ0L,UAAS,cAAAhL,OAAgBwK,EAAQ,UAAY,IAC7CS,UA1GhB,SAAmBlH,GAEf,GAAkB,KAAdA,EAAEmH,QACFvB,EAAaK,EAAYH,GAAyB,OAClDP,EAAS,CACL1C,MAAOoD,EAAYH,GAAyB,MAC5Cb,MAAOgB,EAAYH,GAAyB,QAEhDM,GAAmB,GACnBL,EAAoB,QAInB,GAAkB,KAAd/F,EAAEmH,QAAgB,CACvB,GAAyB,IAArBrB,EAEA,OAGJC,EAAoBD,EAAmB,EAC3C,MAGK,GAAkB,KAAd9F,EAAEmH,QAAgB,CACvB,GAAIrB,EAAmB,IAAMG,EAAY/J,OAGrC,YADA6J,EAAoB,GAIxBA,EAAoBD,EAAmB,EAC3C,KAGmB,QAAV9F,EAAEgC,KACPoE,GAAmB,EAE3B,EAsEgBgB,aAAa,MACbC,YAAY,yCACZxE,MAAO8C,EACP2B,SAjIhB,SAAkBtH,GACd,IAAM6C,EAAQ7C,EAAER,OAAOqD,MACvB+C,EAAa5F,EAAER,OAAOqD,OAGlBA,EAAM3G,QAAU,GAChBqK,GAAc,GACdH,GAAmB,GACnBmB,EAAe1E,EAAOjF,EAASyG,KAG/BkC,GAAc,GACdlC,EAAe,IACf+B,GAAmB,GACnBL,EAAoB,GAE5B,EAkHgByB,QA5DhB,SAAiBxH,GACbA,EAAEyH,iBACFf,GAAS,GAET,IAAM7D,EAAQ7C,EAAER,OAAOqD,MACnBA,EAAM3G,OAAS,EACfqK,GAAc,IAEdA,GAAc,GACdH,GAAmB,GACnBmB,EAAe1E,EAAOjF,EAASyG,GAEvC,EAiDgBqD,OA9ChB,WACIhB,GAAS,EACb,EA6CgB,gBAAc,UACd,oBAAkB,OAClB,gBAAc,mBACd,gBAAeP,EACf,mBAAiB,2BACjBwB,SAAS,MAEZhC,GACGkB,IAAAA,cAAA,UACII,UAAU,eACVW,QA5CpB,WACIhC,EAAa,IACbQ,GAAmB,EACvB,EA0CoB,aAAW,eACd,MAMRE,GACGO,IAAAA,cAAA,OAAKI,UAAU,qBACXJ,IAAAA,cAAA,MAAII,UAAU,eACVJ,IAAAA,cAAA,MAAII,UAAU,6BAA4B,gDAOrDd,GACGU,IAAAA,cAAA,MACII,UAAU,cACV,aAAW,cACXY,KAAK,UACLtM,GAAG,mBAEF0K,EAAYpK,KAAI,SAACiM,EAAY7I,GAC1B,IAAIgI,EAAY,aAQhB,OANIhI,IAAU6G,IACVmB,EAAY,GAAHhL,OAAMgL,EAAS,uBAExBhI,EAAQ,GAAM,IACdgI,EAAY,GAAHhL,OAAMgL,EAAS,oBAGxBJ,IAAAA,cAAA,MACI7E,IAAK/C,EACL,WAAUA,EACVgI,UAAWA,EACXc,YAAa,SAACC,GAAK,OA1HpBhI,EA2HuBgI,GA1H5CP,iBACF7B,EAAa5F,EAAEiI,cAAcC,QAAQjD,OACrCM,EAAS,CACL1C,MAAO7C,EAAEiI,cAAcC,QAAQrF,MAC/BoC,MAAOjF,EAAEiI,cAAcC,QAAQjD,aAEnCmB,GAAmB,GAPvB,IAA2BpG,CA2H6B,EAE5BmI,aAAc,SAACH,GAAK,OA7FtCI,EA6FwDJ,EA7F1CxI,OACdwC,EAAMqG,SAASD,EAAUE,aAAa,kBAE5CvC,EAAoB/D,GAJxB,IACUoG,EACApG,CA4F8D,EAC5C,gBAAe/C,GAAS6G,EACxB,aAAYgC,EACZD,KAAK,SACL,gBAAe5I,EACf,aAAY6I,EAAkB,MAC9B,aAAYA,EAAkB,MAC9B,eAAcA,EAAkB,MAChCH,SAAS,MAERG,EAAkB,MAG/B,KAGRjB,IAAAA,cAAA,QAAMtL,GAAG,2BAA2BgE,MAAO,CAACgJ,QAAS,SAAS,+CAK1E,CDtNA3K,EAAQgD,kBAAoB,IAC5BhD,EAAQ0C,cAAgB,IAElB1C,EAAQ0B,OAAS,SAAc,KAAM,QAE3C1B,EAAQe,OAAS,IACjBf,EAAQ+C,mBAAqB,IAEhB,IAAI,IAAS/C,GAKJ,KAAW,IAAQ4K,QAAS,IAAQA,OC2M1DnD,EAAUoD,UAAY,CAClBlN,GAAImN,IAAAA,OACJzD,MAAOyD,IAAAA,OACP9K,QAAS8K,IAAAA,MACTnD,SAAUmD,IAAAA,KACV7F,MAAO6F,IAAAA,QAEXrD,EAAUsD,aAAe,CACrBpN,GAAI,aACJqC,QAAS,GACT2H,SAAU,WAAO,EACjB1C,MAAO,GACPoC,MAAO,IAGX,S",
     "names": [
         "___CSS_LOADER_EXPORT___",
         "push",
         "module",
         "id",
         "exports",
         "cssWithMappingToString",
@@ -162,15 +162,14 @@
         "label",
         "filteredOptions",
         "option",
         "startsWith",
         "DualInput",
         "_ref",
         "setProps",
-        "initialValue",
         "_useState2",
         "_slicedToArray",
         "useState",
         "userInput",
         "setUserInput",
         "_useState4",
         "activeSuggestion",
@@ -256,18 +255,18 @@
         "\"use strict\";\n\n/* istanbul ignore next  */\nfunction apply(styleElement, options, obj) {\n  var css = \"\";\n  if (obj.supports) {\n    css += \"@supports (\".concat(obj.supports, \") {\");\n  }\n  if (obj.media) {\n    css += \"@media \".concat(obj.media, \" {\");\n  }\n  var needLayer = typeof obj.layer !== \"undefined\";\n  if (needLayer) {\n    css += \"@layer\".concat(obj.layer.length > 0 ? \" \".concat(obj.layer) : \"\", \" {\");\n  }\n  css += obj.css;\n  if (needLayer) {\n    css += \"}\";\n  }\n  if (obj.media) {\n    css += \"}\";\n  }\n  if (obj.supports) {\n    css += \"}\";\n  }\n  var sourceMap = obj.sourceMap;\n  if (sourceMap && typeof btoa !== \"undefined\") {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  }\n\n  // For old IE\n  /* istanbul ignore if  */\n  options.styleTagTransform(css, styleElement, options.options);\n}\nfunction removeStyleElement(styleElement) {\n  // istanbul ignore if\n  if (styleElement.parentNode === null) {\n    return false;\n  }\n  styleElement.parentNode.removeChild(styleElement);\n}\n\n/* istanbul ignore next  */\nfunction domAPI(options) {\n  if (typeof document === \"undefined\") {\n    return {\n      update: function update() {},\n      remove: function remove() {}\n    };\n  }\n  var styleElement = options.insertStyleElement(options);\n  return {\n    update: function update(obj) {\n      apply(styleElement, options, obj);\n    },\n    remove: function remove() {\n      removeStyleElement(styleElement);\n    }\n  };\n}\nmodule.exports = domAPI;",
         "\"use strict\";\n\n/* istanbul ignore next  */\nfunction styleTagTransform(css, styleElement) {\n  if (styleElement.styleSheet) {\n    styleElement.styleSheet.cssText = css;\n  } else {\n    while (styleElement.firstChild) {\n      styleElement.removeChild(styleElement.firstChild);\n    }\n    styleElement.appendChild(document.createTextNode(css));\n  }\n}\nmodule.exports = styleTagTransform;",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_7m1708962473\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_8m1708963329\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "__webpack_require__.nc = undefined;",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
         "function getPostcodes(s) {\r\n    const apiUrl = `https://api.postcodes.io/postcodes/${s}/autocomplete`;\r\n    return fetch(apiUrl)\r\n        .then((response) => {\r\n            // Check if response is successful\r\n            if (!response.ok) {\r\n                throw new Error('Network response was not ok');\r\n            }\r\n            // Parse response JSON\r\n            return response.json();\r\n        })\r\n        .then((data) => {\r\n            // Do something with the data\r\n            return data.result;\r\n        })\r\n        .catch((error) => {\r\n            // Handle errors\r\n            console.error(\r\n                'There was a problem with the fetch operation:',\r\n                error\r\n            );\r\n        });\r\n}\r\n\r\nexport default getPostcodes;\r\n",
         "import getPostcodes from './getPostcodes';\r\n\r\nfunction getSuggestions(value, options, setSuggestions) {\r\n    // If numeric it is likely a postcode\r\n    const containsNumeric = /\\d/.test(value);\r\n\r\n    if (containsNumeric) {\r\n        // Postcode suggestions\r\n        getPostcodes(value).then((postcodes) => {\r\n            let postcodeSuggestions = postcodes.map((postcode) => ({\r\n                label: postcode,\r\n                value: postcode,\r\n            }));\r\n            setSuggestions(postcodeSuggestions);\r\n        });\r\n    } else {\r\n        // Options suggestions\r\n        const filteredOptions = options.filter((option) =>\r\n            option['label'].startsWith(value)\r\n        );\r\n        setSuggestions(filteredOptions);\r\n    }\r\n}\r\n\r\nexport default getSuggestions;\r\n",
         "\n      import API from \"!../../../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\";\n      import domAPI from \"!../../../node_modules/style-loader/dist/runtime/styleDomAPI.js\";\n      import insertFn from \"!../../../node_modules/style-loader/dist/runtime/insertBySelector.js\";\n      import setAttributes from \"!../../../node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js\";\n      import insertStyleElement from \"!../../../node_modules/style-loader/dist/runtime/insertStyleElement.js\";\n      import styleTagTransformFn from \"!../../../node_modules/style-loader/dist/runtime/styleTagTransform.js\";\n      import content, * as namedExport from \"!!../../../node_modules/css-loader/dist/cjs.js!./styles.css\";\n      \n      \n\nvar options = {};\n\noptions.styleTagTransform = styleTagTransformFn;\noptions.setAttributes = setAttributes;\n\n      options.insert = insertFn.bind(null, \"head\");\n    \noptions.domAPI = domAPI;\noptions.insertStyleElement = insertStyleElement;\n\nvar update = API(content, options);\n\n\n\nexport * from \"!!../../../node_modules/css-loader/dist/cjs.js!./styles.css\";\n       export default content && content.locals ? content.locals : undefined;\n",
-        "import React from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport {useState} from 'react';\r\n\r\nimport getSuggestions from '../getSuggestions';\r\nimport './styles.css';\r\nimport {init} from 'ramda';\r\nfunction DualInput({id, options, setProps, initialValue, label}) {\r\n    // Define the state of the component\r\n    const [userInput, setUserInput] = useState('');\r\n    const [activeSuggestion, setActiveSuggestion] = useState(0);\r\n    const [suggestions, setSuggestions] = useState([]);\r\n    const [showSuggestions, setShowSuggestions] = useState(false);\r\n    const [showPrompt, setShowPrompt] = useState(false);\r\n    const [focus, setFocus] = useState(false);\r\n\r\n    // Initial value popoulated\r\n    if (initialValue.length > 0) {\r\n        setUserInput(initialValue);\r\n    }\r\n\r\n    // When a user types into the input\r\n    function onChange(e) {\r\n        const value = e.target.value;\r\n        setUserInput(e.target.value);\r\n\r\n        // This needs to be extracted into a function and called onFocus too.\r\n        if (value.length >= 3) {\r\n            setShowPrompt(false);\r\n            setShowSuggestions(true);\r\n            getSuggestions(value, options, setSuggestions);\r\n        } else {\r\n            // Reset suggestions when value is less than 3 characters\r\n            setShowPrompt(true);\r\n            setSuggestions([]);\r\n            setShowSuggestions(false);\r\n            setActiveSuggestion(0);\r\n        }\r\n    }\r\n\r\n    // Handle keyboard interactiosn\r\n    function onKeyDown(e) {\r\n        // User pressed the enter key\r\n        if (e.keyCode === 13) {\r\n            setUserInput(suggestions[activeSuggestion]['label']);\r\n            setProps({\r\n                value: suggestions[activeSuggestion]['value'],\r\n                label: suggestions[activeSuggestion]['label'],\r\n            });\r\n            setShowSuggestions(false);\r\n            setActiveSuggestion(0);\r\n        }\r\n\r\n        // User pressed the up arrow\r\n        else if (e.keyCode === 38) {\r\n            if (activeSuggestion === 0) {\r\n                // There is nowhere higher to go\r\n                return;\r\n            }\r\n            // Move active suggestion up one\r\n            setActiveSuggestion(activeSuggestion - 1);\r\n        }\r\n\r\n        // User pressed the down arrow\r\n        else if (e.keyCode === 40) {\r\n            if (activeSuggestion + 1 === suggestions.length) {\r\n                // There is nowhere lower to go, reset to top\r\n                setActiveSuggestion(0);\r\n                return;\r\n            }\r\n            // Move active suggestion down one.\r\n            setActiveSuggestion(activeSuggestion + 1);\r\n        }\r\n\r\n        // User pressed the tab button and wants to move away\r\n        else if (e.key === 'Tab') {\r\n            setShowSuggestions(false);\r\n        }\r\n    }\r\n\r\n    // Handle clicks\r\n    function handleOptionClick(e) {\r\n        e.preventDefault();\r\n        setUserInput(e.currentTarget.dataset.label);\r\n        setProps({\r\n            value: e.currentTarget.dataset.value,\r\n            label: e.currentTarget.dataset.label,\r\n        });\r\n        setShowSuggestions(false);\r\n    }\r\n\r\n    // On focus of the input box\r\n    function onFocus(e) {\r\n        e.preventDefault();\r\n        setFocus(true);\r\n        // This is where we need to call the suggestions code again\r\n        const value = e.target.value;\r\n        if (value.length < 3) {\r\n            setShowPrompt(true);\r\n        } else {\r\n            setShowPrompt(false);\r\n            setShowSuggestions(true);\r\n            getSuggestions(value, options, setSuggestions);\r\n        }\r\n    }\r\n\r\n    // When user blurs from input box\r\n    function onBlur() {\r\n        setFocus(false);\r\n    }\r\n\r\n    // When user hovers over option\r\n    function onMouseEnter(e) {\r\n        const liElement = e.target;\r\n        const key = parseInt(liElement.getAttribute('data-key'));\r\n\r\n        setActiveSuggestion(key);\r\n    }\r\n\r\n    // When user clicks clear button\r\n    function clearInput() {\r\n        setUserInput('');\r\n        setShowSuggestions(false);\r\n    }\r\n\r\n    // Code to allow clicking away from the component\r\n    const handleClickOutside = (e) => {\r\n        if (!e.target.closest('.input-container')) {\r\n            setShowSuggestions(false);\r\n        }\r\n    };\r\n\r\n    // Handles when a user clicks away from the components\r\n    React.useEffect(() => {\r\n        document.body.addEventListener('click', handleClickOutside);\r\n        return () => {\r\n            document.body.removeEventListener('click', handleClickOutside);\r\n        };\r\n    }, []);\r\n\r\n    // Return the component JSX\r\n    return (\r\n        <div>\r\n            <div className=\"input-container\">\r\n                <input\r\n                    id={id}\r\n                    className={`dual-input ${focus ? 'focused' : ''}`} // Toggle focus styling\r\n                    onKeyDown={onKeyDown}\r\n                    autoComplete=\"off\"\r\n                    placeholder=\"Enter a postcode or local authority...\"\r\n                    value={userInput}\r\n                    onChange={onChange}\r\n                    onFocus={onFocus}\r\n                    onBlur={onBlur}\r\n                    aria-haspopup=\"listbox\"\r\n                    aria-autocomplete=\"both\"\r\n                    aria-controls=\"suggestions-list\"\r\n                    aria-expanded={showSuggestions}\r\n                    aria-describedby=\"dualInput__assistiveHint\"\r\n                    tabIndex=\"0\"\r\n                ></input>\r\n                {userInput && (\r\n                    <button\r\n                        className=\"clear-button\"\r\n                        onClick={clearInput}\r\n                        aria-label=\"Clear input\"\r\n                    >\r\n                        x\r\n                    </button>\r\n                )}\r\n            </div>\r\n\r\n            {showPrompt && (\r\n                <div className=\"dual-input-prompt\">\r\n                    <ul className=\"suggestions\">\r\n                        <li className=\"suggestion odd-suggestion\">\r\n                            Enter 3 or more characters for suggestions\r\n                        </li>\r\n                    </ul>\r\n                </div>\r\n            )}\r\n\r\n            {showSuggestions && (\r\n                <ul\r\n                    className=\"suggestions\"\r\n                    aria-label=\"Suggestions\"\r\n                    role=\"listbox\"\r\n                    id=\"suggestion-list\"\r\n                >\r\n                    {suggestions.map((suggestion, index) => {\r\n                        let className = 'suggestion';\r\n\r\n                        if (index === activeSuggestion) {\r\n                            className = `${className} active-suggestion`; // Toggle active suggestion styling\r\n                        }\r\n                        if (index % 2 !== 0) {\r\n                            className = `${className} odd-suggestion`; // Toggle odd stylinh\r\n                        }\r\n                        return (\r\n                            <li\r\n                                key={index}\r\n                                data-key={index}\r\n                                className={className}\r\n                                onMouseDown={(event) =>\r\n                                    handleOptionClick(event)\r\n                                } // Had to use onMouseDown rather than onClick. Wasn't working in dash.\r\n                                onMouseEnter={(event) => onMouseEnter(event)}\r\n                                aria-selected={index == activeSuggestion}\r\n                                aria-label={suggestion}\r\n                                role=\"option\"\r\n                                aria-posinset={index}\r\n                                data-value={suggestion['value']}\r\n                                data-label={suggestion['label']}\r\n                                option-value={suggestion['value']}\r\n                                tabIndex=\"-1\"\r\n                            >\r\n                                {suggestion['label']}\r\n                            </li>\r\n                        );\r\n                    })}\r\n                </ul>\r\n            )}\r\n            <span id=\"dualInput__assistiveHint\" style={{display: 'none'}}>\r\n                Enter 3 or more characters for suggestions.\r\n            </span>\r\n        </div>\r\n    );\r\n}\r\n\r\nDualInput.propTypes = {\r\n    id: PropTypes.string,\r\n    label: PropTypes.string,\r\n    options: PropTypes.array,\r\n    setProps: PropTypes.func,\r\n    value: PropTypes.string,\r\n};\r\nDualInput.defaultProps = {\r\n    id: 'dual_input',\r\n    options: [],\r\n    setProps: () => {},\r\n    value: '',\r\n    label: '',\r\n};\r\n\r\nexport default DualInput;\r\n"
+        "import React from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport {useState} from 'react';\r\n\r\nimport getSuggestions from '../getSuggestions';\r\nimport './styles.css';\r\n\r\nfunction DualInput({id, options, value, setProps, label}) {\r\n    // Define the state of the component\r\n    const [userInput, setUserInput] = useState('');\r\n    const [activeSuggestion, setActiveSuggestion] = useState(0);\r\n    const [suggestions, setSuggestions] = useState([]);\r\n    const [showSuggestions, setShowSuggestions] = useState(false);\r\n    const [showPrompt, setShowPrompt] = useState(false);\r\n    const [focus, setFocus] = useState(false);\r\n\r\n    // Initial value popoulated\r\n    if (value.length > 0) {\r\n        setUserInput(value);\r\n    }\r\n\r\n    // When a user types into the input\r\n    function onChange(e) {\r\n        const value = e.target.value;\r\n        setUserInput(e.target.value);\r\n\r\n        // This needs to be extracted into a function and called onFocus too.\r\n        if (value.length >= 3) {\r\n            setShowPrompt(false);\r\n            setShowSuggestions(true);\r\n            getSuggestions(value, options, setSuggestions);\r\n        } else {\r\n            // Reset suggestions when value is less than 3 characters\r\n            setShowPrompt(true);\r\n            setSuggestions([]);\r\n            setShowSuggestions(false);\r\n            setActiveSuggestion(0);\r\n        }\r\n    }\r\n\r\n    // Handle keyboard interactiosn\r\n    function onKeyDown(e) {\r\n        // User pressed the enter key\r\n        if (e.keyCode === 13) {\r\n            setUserInput(suggestions[activeSuggestion]['label']);\r\n            setProps({\r\n                value: suggestions[activeSuggestion]['value'],\r\n                label: suggestions[activeSuggestion]['label'],\r\n            });\r\n            setShowSuggestions(false);\r\n            setActiveSuggestion(0);\r\n        }\r\n\r\n        // User pressed the up arrow\r\n        else if (e.keyCode === 38) {\r\n            if (activeSuggestion === 0) {\r\n                // There is nowhere higher to go\r\n                return;\r\n            }\r\n            // Move active suggestion up one\r\n            setActiveSuggestion(activeSuggestion - 1);\r\n        }\r\n\r\n        // User pressed the down arrow\r\n        else if (e.keyCode === 40) {\r\n            if (activeSuggestion + 1 === suggestions.length) {\r\n                // There is nowhere lower to go, reset to top\r\n                setActiveSuggestion(0);\r\n                return;\r\n            }\r\n            // Move active suggestion down one.\r\n            setActiveSuggestion(activeSuggestion + 1);\r\n        }\r\n\r\n        // User pressed the tab button and wants to move away\r\n        else if (e.key === 'Tab') {\r\n            setShowSuggestions(false);\r\n        }\r\n    }\r\n\r\n    // Handle clicks\r\n    function handleOptionClick(e) {\r\n        e.preventDefault();\r\n        setUserInput(e.currentTarget.dataset.label);\r\n        setProps({\r\n            value: e.currentTarget.dataset.value,\r\n            label: e.currentTarget.dataset.label,\r\n        });\r\n        setShowSuggestions(false);\r\n    }\r\n\r\n    // On focus of the input box\r\n    function onFocus(e) {\r\n        e.preventDefault();\r\n        setFocus(true);\r\n        // This is where we need to call the suggestions code again\r\n        const value = e.target.value;\r\n        if (value.length < 3) {\r\n            setShowPrompt(true);\r\n        } else {\r\n            setShowPrompt(false);\r\n            setShowSuggestions(true);\r\n            getSuggestions(value, options, setSuggestions);\r\n        }\r\n    }\r\n\r\n    // When user blurs from input box\r\n    function onBlur() {\r\n        setFocus(false);\r\n    }\r\n\r\n    // When user hovers over option\r\n    function onMouseEnter(e) {\r\n        const liElement = e.target;\r\n        const key = parseInt(liElement.getAttribute('data-key'));\r\n\r\n        setActiveSuggestion(key);\r\n    }\r\n\r\n    // When user clicks clear button\r\n    function clearInput() {\r\n        setUserInput('');\r\n        setShowSuggestions(false);\r\n    }\r\n\r\n    // Code to allow clicking away from the component\r\n    const handleClickOutside = (e) => {\r\n        if (!e.target.closest('.input-container')) {\r\n            setShowSuggestions(false);\r\n        }\r\n    };\r\n\r\n    // Handles when a user clicks away from the components\r\n    React.useEffect(() => {\r\n        document.body.addEventListener('click', handleClickOutside);\r\n        return () => {\r\n            document.body.removeEventListener('click', handleClickOutside);\r\n        };\r\n    }, []);\r\n\r\n    // Return the component JSX\r\n    return (\r\n        <div>\r\n            <div className=\"input-container\">\r\n                <input\r\n                    id={id}\r\n                    className={`dual-input ${focus ? 'focused' : ''}`} // Toggle focus styling\r\n                    onKeyDown={onKeyDown}\r\n                    autoComplete=\"off\"\r\n                    placeholder=\"Enter a postcode or local authority...\"\r\n                    value={userInput}\r\n                    onChange={onChange}\r\n                    onFocus={onFocus}\r\n                    onBlur={onBlur}\r\n                    aria-haspopup=\"listbox\"\r\n                    aria-autocomplete=\"both\"\r\n                    aria-controls=\"suggestions-list\"\r\n                    aria-expanded={showSuggestions}\r\n                    aria-describedby=\"dualInput__assistiveHint\"\r\n                    tabIndex=\"0\"\r\n                ></input>\r\n                {userInput && (\r\n                    <button\r\n                        className=\"clear-button\"\r\n                        onClick={clearInput}\r\n                        aria-label=\"Clear input\"\r\n                    >\r\n                        x\r\n                    </button>\r\n                )}\r\n            </div>\r\n\r\n            {showPrompt && (\r\n                <div className=\"dual-input-prompt\">\r\n                    <ul className=\"suggestions\">\r\n                        <li className=\"suggestion odd-suggestion\">\r\n                            Enter 3 or more characters for suggestions\r\n                        </li>\r\n                    </ul>\r\n                </div>\r\n            )}\r\n\r\n            {showSuggestions && (\r\n                <ul\r\n                    className=\"suggestions\"\r\n                    aria-label=\"Suggestions\"\r\n                    role=\"listbox\"\r\n                    id=\"suggestion-list\"\r\n                >\r\n                    {suggestions.map((suggestion, index) => {\r\n                        let className = 'suggestion';\r\n\r\n                        if (index === activeSuggestion) {\r\n                            className = `${className} active-suggestion`; // Toggle active suggestion styling\r\n                        }\r\n                        if (index % 2 !== 0) {\r\n                            className = `${className} odd-suggestion`; // Toggle odd stylinh\r\n                        }\r\n                        return (\r\n                            <li\r\n                                key={index}\r\n                                data-key={index}\r\n                                className={className}\r\n                                onMouseDown={(event) =>\r\n                                    handleOptionClick(event)\r\n                                } // Had to use onMouseDown rather than onClick. Wasn't working in dash.\r\n                                onMouseEnter={(event) => onMouseEnter(event)}\r\n                                aria-selected={index == activeSuggestion}\r\n                                aria-label={suggestion}\r\n                                role=\"option\"\r\n                                aria-posinset={index}\r\n                                data-value={suggestion['value']}\r\n                                data-label={suggestion['label']}\r\n                                option-value={suggestion['value']}\r\n                                tabIndex=\"-1\"\r\n                            >\r\n                                {suggestion['label']}\r\n                            </li>\r\n                        );\r\n                    })}\r\n                </ul>\r\n            )}\r\n            <span id=\"dualInput__assistiveHint\" style={{display: 'none'}}>\r\n                Enter 3 or more characters for suggestions.\r\n            </span>\r\n        </div>\r\n    );\r\n}\r\n\r\nDualInput.propTypes = {\r\n    id: PropTypes.string,\r\n    label: PropTypes.string,\r\n    options: PropTypes.array,\r\n    setProps: PropTypes.func,\r\n    value: PropTypes.string,\r\n};\r\nDualInput.defaultProps = {\r\n    id: 'dual_input',\r\n    options: [],\r\n    setProps: () => {},\r\n    value: '',\r\n    label: '',\r\n};\r\n\r\nexport default DualInput;\r\n"
     ],
     "version": 3
 }
```

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/metadata.json` & `dash_oflog_components-0.0.9/dash_oflog_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components/package-info.json` & `dash_oflog_components-0.0.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -54,9 +54,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_oflog_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.7"
+    "version": "0.0.9"
 }
```

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components.egg-info/PKG-INFO` & `dash_oflog_components-0.0.9/dash_oflog_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-oflog-components
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dash react components for use in oflog data products
 Home-page: UNKNOWN
 Author: Haydn Jenkins <haydn.jenkins@levellingup.gov.uk>
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
```

### Comparing `dash_oflog_components-0.0.8/dash_oflog_components.egg-info/SOURCES.txt` & `dash_oflog_components-0.0.9/dash_oflog_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/package.json` & `dash_oflog_components-0.0.9/dash_oflog_components/package-info.json`

 * *Files identical despite different names*

### Comparing `dash_oflog_components-0.0.8/setup.py` & `dash_oflog_components-0.0.9/setup.py`

 * *Files identical despite different names*

