# Comparing `tmp/odoo14_addon_ssi_decorator-14.0.1.5.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_decorator-14.0.1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 53913 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1179 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/README.rst
--rw-r--r--  2.0 unx      180 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/__init__.py
--rw-r--r--  2.0 unx      414 b- defN 24-Apr-08 04:44 odoo/addons/ssi_decorator/__manifest__.py
--rw-r--r--  2.0 unx     4197 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/ssi_decorator.py
--rw-r--r--  2.0 unx      193 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/models/__init__.py
--rw-r--r--  2.0 unx     3917 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py
--rw-r--r--  2.0 unx    48333 b- defN 24-Apr-08 04:43 odoo/addons/ssi_decorator/static/description/icon.png
--rw-r--r--  2.0 unx     1662 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1098 b- defN 24-Apr-08 04:45 odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD
-11 files, 61270 bytes uncompressed, 51991 bytes compressed:  15.1%
+Zip file size: 53968 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1179 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/README.rst
+-rw-r--r--  2.0 unx      180 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/__init__.py
+-rw-r--r--  2.0 unx      414 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/__manifest__.py
+-rw-r--r--  2.0 unx     4967 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/ssi_decorator.py
+-rw-r--r--  2.0 unx      193 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/models/__init__.py
+-rw-r--r--  2.0 unx     3917 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py
+-rw-r--r--  2.0 unx    48333 b- defN 24-May-11 00:54 odoo/addons/ssi_decorator/static/description/icon.png
+-rw-r--r--  2.0 unx     1662 b- defN 24-May-11 00:54 odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 00:54 odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-11 00:54 odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1098 b- defN 24-May-11 00:54 odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/RECORD
+11 files, 62040 bytes uncompressed, 52046 bytes compressed:  16.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py
 Comment: 
 
 Filename: odoo/addons/ssi_decorator/static/description/icon.png
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_decorator/__manifest__.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
 {
     "name": "SSI - Decorator",
-    "version": "14.0.1.5.0",
+    "version": "14.0.1.5.1",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [],
     "data": [],
 }
```

## odoo/addons/ssi_decorator/ssi_decorator.py

```diff
@@ -88,14 +88,31 @@
     return attrsetter("_pre_ready_action", args)
 
 
 def post_ready_action(*args):
     return attrsetter("_post_ready_action", args)
 
 
+# QUEUE TO DONE
+def pre_queue_done_check(*args):
+    return attrsetter("_pre_queue_done_check", args)
+
+
+def post_queue_done_check(*args):
+    return attrsetter("_post_queue_done_check", args)
+
+
+def pre_queue_done_action(*args):
+    return attrsetter("_pre_queue_done_action", args)
+
+
+def post_queue_done_action(*args):
+    return attrsetter("_post_queue_done_action", args)
+
+
 # DONE
 def pre_done_check(*args):
     return attrsetter("_pre_done_check", args)
 
 
 def post_done_check(*args):
     return attrsetter("_post_done_check", args)
@@ -105,14 +122,31 @@
     return attrsetter("_pre_done_action", args)
 
 
 def post_done_action(*args):
     return attrsetter("_post_done_action", args)
 
 
+# QUEUE TO CANCEL
+def pre_queue_cancel_check(*args):
+    return attrsetter("_pre_queue_cancel_check", args)
+
+
+def post_queue_cancel_check(*args):
+    return attrsetter("_post_queue_cancel_check", args)
+
+
+def pre_queue_cancel_action(*args):
+    return attrsetter("_pre_queue_cancel_action", args)
+
+
+def post_queue_cancel_action(*args):
+    return attrsetter("_post_queue_cancel_action", args)
+
+
 # CANCEL
 def pre_cancel_check(*args):
     return attrsetter("_pre_cancel_check", args)
 
 
 def post_cancel_check(*args):
     return attrsetter("_post_cancel_check", args)
```

## Comparing `odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA` & `odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-decorator
-Version: 14.0.1.5.0
+Version: 14.0.1.5.1
 Summary: SSI - Decorator
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD` & `odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/ssi_decorator/README.rst,sha256=x3j1DGfpwl-LURwTV8POFMvtSKYhEvN23dbLS_6xV_c,1179
 odoo/addons/ssi_decorator/__init__.py,sha256=tzITx23QOcikJV4zQ1mAV0fGGi0rhMaF3ksZb9m8FVQ,180
-odoo/addons/ssi_decorator/__manifest__.py,sha256=E2AQQNA59DYvNRFEsQrLOshZ_9tqfSR3XMx6zA-X9Fo,414
-odoo/addons/ssi_decorator/ssi_decorator.py,sha256=Z8FpIXGKZNKX9SOedUDpelZ39dofpTQ8PUPv1jxFEU4,4197
+odoo/addons/ssi_decorator/__manifest__.py,sha256=d1_GY-x9mVNk7mCN6CA6ppxAu8E1FYHie6DZ9dOGkog,414
+odoo/addons/ssi_decorator/ssi_decorator.py,sha256=JRYpdKSt_l1yG5xUP81UYShV1dxdW5dsiyPFwznrdQk,4967
 odoo/addons/ssi_decorator/models/__init__.py,sha256=YbUtBI9pRkCEdMYdeZg_cyMUx23l346q6-paMBMWF-U,193
 odoo/addons/ssi_decorator/models/ssi_decorator_mixin.py,sha256=9lmUHQAJIEFcEXicPvArGdOISPQ0RU8klm4mPGucWuA,3917
 odoo/addons/ssi_decorator/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/METADATA,sha256=wqfHuHX5V8fQ-zvCKR-yb-NPcsDMzrOM0YKdDrUYPv8,1662
-odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_decorator-14.0.1.5.0.dist-info/RECORD,,
+odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/METADATA,sha256=Qi2PyakrfWl2C3MVnnZXbTnCIja2_ZV8qkS0JT9ShqI,1662
+odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_decorator-14.0.1.5.1.dist-info/RECORD,,
```

