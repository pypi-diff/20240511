# Comparing `tmp/STAIR-tools-1.2.7.tar.gz` & `tmp/STAIR-tools-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STAIR-tools-1.2.7.tar", last modified: Tue May  7 05:18:39 2024, max compression
+gzip compressed data, was "STAIR-tools-1.2.8.tar", last modified: Sat May 11 08:21:29 2024, max compression
```

## Comparing `STAIR-tools-1.2.7.tar` & `STAIR-tools-1.2.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-07 05:18:39.831523 STAIR-tools-1.2.7/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-07 05:18:39.831266 STAIR-tools-1.2.7/PKG-INFO
--rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.7/README.md
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-07 05:18:39.828732 STAIR-tools-1.2.7/STAIR/
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.7/STAIR/ABA_annotation.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-07 05:18:39.828851 STAIR-tools-1.2.7/STAIR/ABAanno/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.7/STAIR/ABAanno/__init__.py
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.7/STAIR/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.7/STAIR/emb_alignment.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-07 05:18:39.829707 STAIR-tools-1.2.7/STAIR/embedding/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.7/STAIR/embedding/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.7/STAIR/embedding/dataset_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6047 2024-05-07 05:16:40.000000 STAIR-tools-1.2.7/STAIR/embedding/dataset_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.7/STAIR/embedding/loss.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.7/STAIR/embedding/module_ae.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.7/STAIR/embedding/module_hgat.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.7/STAIR/embedding/module_hgat1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12320 2024-04-29 06:21:03.000000 STAIR-tools-1.2.7/STAIR/loc_alignment.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14364 2024-04-28 11:59:13.000000 STAIR-tools-1.2.7/STAIR/loc_prediction.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-07 05:18:39.830496 STAIR-tools-1.2.7/STAIR/location/
--rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.7/STAIR/location/__init__.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.7/STAIR/location/align_fine.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)    11236 2023-12-23 11:23:13.000000 STAIR-tools-1.2.7/STAIR/location/align_init.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.7/STAIR/location/edge_detection.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.7/STAIR/location/edge_detection1.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.7/STAIR/location/transformation.py
--rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.7/STAIR/utils.py
-drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-07 05:18:39.831078 STAIR-tools-1.2.7/STAIR_tools.egg-info/
--rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-07 05:18:39.000000 STAIR-tools-1.2.7/STAIR_tools.egg-info/PKG-INFO
--rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-07 05:18:39.000000 STAIR-tools-1.2.7/STAIR_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-07 05:18:39.000000 STAIR-tools-1.2.7/STAIR_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-07 05:18:39.000000 STAIR-tools-1.2.7/STAIR_tools.egg-info/top_level.txt
--rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-07 05:18:39.831575 STAIR-tools-1.2.7/setup.cfg
--rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-07 05:18:31.000000 STAIR-tools-1.2.7/setup.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.076707 STAIR-tools-1.2.8/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-11 08:21:29.076477 STAIR-tools-1.2.8/PKG-INFO
+-rwxr-xr-x   0 yuanyuan   (501) staff       (20)     1320 2023-12-25 02:00:08.000000 STAIR-tools-1.2.8/README.md
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.072338 STAIR-tools-1.2.8/STAIR/
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8661 2023-12-23 11:23:09.000000 STAIR-tools-1.2.8/STAIR/ABA_annotation.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.072565 STAIR-tools-1.2.8/STAIR/ABAanno/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.8/STAIR/ABAanno/__init__.py
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.8/STAIR/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    18514 2024-05-06 15:17:54.000000 STAIR-tools-1.2.8/STAIR/emb_alignment.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.074397 STAIR-tools-1.2.8/STAIR/embedding/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2024-04-25 02:41:10.000000 STAIR-tools-1.2.8/STAIR/embedding/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     3804 2024-05-04 11:27:47.000000 STAIR-tools-1.2.8/STAIR/embedding/dataset_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6047 2024-05-07 05:16:40.000000 STAIR-tools-1.2.8/STAIR/embedding/dataset_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)      988 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/loss.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     5493 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/module_ae.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8658 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/module_hgat.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     6954 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/embedding/module_hgat1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12477 2024-05-11 08:20:36.000000 STAIR-tools-1.2.8/STAIR/loc_alignment.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    14363 2024-05-11 08:19:13.000000 STAIR-tools-1.2.8/STAIR/loc_prediction.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.075744 STAIR-tools-1.2.8/STAIR/location/
+-rw-------   0 yuanyuan   (501) staff       (20)      120 2023-08-11 07:05:03.000000 STAIR-tools-1.2.8/STAIR/location/__init__.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     7819 2023-12-23 11:23:12.000000 STAIR-tools-1.2.8/STAIR/location/align_fine.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)    12278 2024-05-11 08:16:53.000000 STAIR-tools-1.2.8/STAIR/location/align_init.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     8534 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/location/edge_detection.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     9354 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/location/edge_detection1.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2298 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/location/transformation.py
+-rwxrwxrwx   0 yuanyuan   (501) staff       (20)     2821 2023-12-23 11:23:13.000000 STAIR-tools-1.2.8/STAIR/utils.py
+drwxr-xr-x   0 yuanyuan   (501) staff       (20)        0 2024-05-11 08:21:29.076293 STAIR-tools-1.2.8/STAIR_tools.egg-info/
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      253 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yuanyuan   (501) staff       (20)      702 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        1 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)        6 2024-05-11 08:21:29.000000 STAIR-tools-1.2.8/STAIR_tools.egg-info/top_level.txt
+-rw-r--r--   0 yuanyuan   (501) staff       (20)       38 2024-05-11 08:21:29.076754 STAIR-tools-1.2.8/setup.cfg
+-rw-------   0 yuanyuan   (501) staff       (20)      489 2024-05-11 08:21:05.000000 STAIR-tools-1.2.8/setup.py
```

### Comparing `STAIR-tools-1.2.7/README.md` & `STAIR-tools-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/ABA_annotation.py` & `STAIR-tools-1.2.8/STAIR/ABA_annotation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/emb_alignment.py` & `STAIR-tools-1.2.8/STAIR/emb_alignment.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/embedding/dataset_ae.py` & `STAIR-tools-1.2.8/STAIR/embedding/dataset_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/embedding/dataset_hgat.py` & `STAIR-tools-1.2.8/STAIR/embedding/dataset_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/embedding/loss.py` & `STAIR-tools-1.2.8/STAIR/embedding/loss.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/embedding/module_ae.py` & `STAIR-tools-1.2.8/STAIR/embedding/module_ae.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/embedding/module_hgat.py` & `STAIR-tools-1.2.8/STAIR/embedding/module_hgat.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/embedding/module_hgat1.py` & `STAIR-tools-1.2.8/STAIR/embedding/module_hgat1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/loc_alignment.py` & `STAIR-tools-1.2.8/STAIR/loc_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             
     
     def init_align(self, 
                    emb_key,
                    spatial_key = 'spatial',
                    num_mnn = 1, 
                    init_align_key = 'transform_init',
+                   use_scale = False,
                    return_result = False
                    ):
         '''
         Initial alignment of spatial location.
         
         Parameters
         ----------
@@ -80,30 +81,31 @@
         num_mnn
             The number of mutual nearest neighbors calculated according to emb_key
         init_align_key
             Key of initial transformed coordinates added in .obsm
         
         '''
         self.init_align_key = init_align_key
-        self.init_adatas, anchors, self.Ts_init = initial_alignment(self.adata_list, 
-                                                                    spatial_key = spatial_key,
-                                                                    emb_key = emb_key,
-                                                                    num_mnn = num_mnn,
-                                                                    key_added = init_align_key
-                                                                )
+        self.init_adatas, anchors, self.Ts_init, scales = initial_alignment(self.adata_list, 
+		                                                                    spatial_key = spatial_key,
+		                                                                    emb_key = emb_key,
+		                                                                    num_mnn = num_mnn,
+		                                                                    key_added = init_align_key,
+		                                                                    use_scale = use_scale
+		                                                                )
         # self.boundary = [(anchor[:,0].tolist(), anchor[:,1].tolist()) for anchor in anchors]
         
         if self.make_log:
             self.makeLog(f"Parameter set for initial alignment")
             self.makeLog(f"  Starting coordinates: {spatial_key}")
             self.makeLog(f"  K of MNN: {num_mnn}")
             self.makeLog(f"  Aligned coordinates: {init_align_key}")
         
         if return_result:
-            return anchors, self.Ts_init
+            return anchors, self.Ts_init, scales
 
 
     def detect_fine_points( self,
                             slice_boundary = True, 
                             domain_boundary = True, 
                             domain_key = 'layer_cluster',
                             num_domains = 1,
```

### Comparing `STAIR-tools-1.2.7/STAIR/loc_prediction.py` & `STAIR-tools-1.2.8/STAIR/loc_prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     nearest_slices = [loc_knowns.index[abs(loc_knowns - preds[i]).argmin()] for i in range(len(preds))]
     return preds, nearest_slices
 
 
 
 def init_align_with_scale(  adata_ref,
                             adata_query, 
-                            emb_key = 'HAN_SE',
+                            emb_key = 'STAIR',
                             num_mnn = 1,
                             spatial_key1 = 'spatial',
                             spatial_key2 = None,
                             use_scale = True, 
                             key_added = 'init_scale',
                             return_scale = False
                         ):
```

### Comparing `STAIR-tools-1.2.7/STAIR/location/align_fine.py` & `STAIR-tools-1.2.8/STAIR/location/align_fine.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/location/align_init.py` & `STAIR-tools-1.2.8/STAIR/location/align_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 
 def align_init_pair(adata1, 
                     adata2, 
                     spatial_key1,
                     spatial_key2 = None,
                     num_mnn = 1,
-                    emb_key = 'HAN_SE',
-                    key_added = 'transform_init'
+                    emb_key = 'STAIR',
+                    key_added = 'transform_init',
+                    use_scale = False
                     ):
     '''
     Align spatial coordinates of adata2 to match adata1 according to the similarity of emb_key.
     Input:
       adata1
       adata2
       spatial_key1: Key of spatial coordinates in .obsm 
@@ -54,24 +55,115 @@
     # Extract the coordinates of the nearest neighbors
     if spatial_key2 is None:
         spatial_key2 = spatial_key1
     
     B = adata1[pair[:,0],:].obsm[spatial_key1]
     A = adata2[pair[:,1],:].obsm[spatial_key2]
     
+    if use_scale:
+        scales_ = np.array([np.sqrt(((B[i] - B[j])**2).sum()) / np.sqrt(((A[i] - A[j])**2).sum()) for i in range(B.shape[0]) for j in range(B.shape[0]) if i!=j])
+        scale_use = np.median(scales_)
+        A = A * scale_use
+    else:
+        scale_use=None
+
     # search for best transformation
     T,_,_ = best_fit_transform(A, B)
     
     # transform the coordinates of adata2
-    adata2.obsm[key_added] = transform(adata2.obsm[spatial_key2], T)    
+    if use_scale:
+        adata2.obsm[key_added] = transform(adata2.obsm[spatial_key2] * scale_use, T)    
+    else:
+        adata2.obsm[key_added] = transform(adata2.obsm[spatial_key2], T)    
     
     if key_added!=spatial_key1:
         adata1.obsm[key_added] = adata1.obsm[spatial_key1]
     
-    return adata1, adata2, pair, T
+    return adata1, adata2, pair, T, scale_use
+
+
+
+
+
+def initial_alignment(  adatas, 
+                        spatial_key = 'spatial',
+                        emb_key = 'HAN_SE',
+                        num_mnn = 1, 
+                        key_added = 'transform_init',
+                        use_scale = False
+                      ):
+    
+    '''
+    Perform initial alignment for adatas according to the similarity of emb_key.
+    Input:
+      adatas:       Adata list to be aligned
+      spatial_key:  Key of spatial coordinates in .obsm 
+      emb_key:      The key used to calculate spot similarity in .obsm
+      num_mnn:      The number of mutual nearest neighbors calculated according to emb_key
+      key_added:    Key of transformed coordinates added in .obsm
+    Returns:
+      adatas:       Aligned adata list with 'transformed' in .obsm
+      anchors:      np.array of indices of nearest neighbor pairs
+    '''
+    
+    aligned_init = []
+    anchors = []
+    Ts = []
+    scales = []
+    
+
+    print('Performing initial alignment of the 1 pair of data...')
+    
+    # initial alignment of the first two adatas
+    adata1, adata2 = adatas[0], adatas[1]
+    
+    adata1, adata2, anchor_tmp, T_tmp, scale_tmp = align_init_pair( adata1, 
+                                                                    adata2, 
+                                                                    spatial_key1 = spatial_key,
+                                                                    spatial_key2 = None,
+                                                                    num_mnn = num_mnn, 
+                                                                    emb_key = emb_key,
+                                                                    key_added = key_added,
+                                                                    use_scale = use_scale
+                                                                    )
+    
+    aligned_init.append(adata1)
+    aligned_init.append(adata2)
+    anchors.append(anchor_tmp)
+    Ts.append(T_tmp)
+    scales.append(scale_tmp)
+    
+    # initial alignment of the rest adatas
+    if len(aligned_init)!=len(adatas):
+        for i in range(1, len(adatas)-1):
+            
+            print(f'Performing initial alignment of the {i+1} pair of data...')
+            
+            adata1_tmp = aligned_init[-1]
+            adata2_tmp = adatas[i+1]
+            
+            for T_ in Ts:
+                adata2_tmp.obsm[spatial_key] = transform(adata2_tmp.obsm[spatial_key], T_)
+            
+            _, adata2_tmp, anchor_tmp, T_tmp, scale_tmp = align_init_pair( adata1_tmp, 
+                                                                            adata2_tmp, 
+                                                                            spatial_key1 = key_added, 
+                                                                            spatial_key2 = spatial_key, 
+                                                                            num_mnn = num_mnn, 
+                                                                            emb_key = emb_key,
+                                                                            key_added = key_added,
+                                                                            use_scale = use_scale
+                                                                           )
+                    
+            aligned_init.append(adata2_tmp)
+            anchors.append(anchor_tmp)
+            Ts.append(T_tmp)
+            scales.append(scale_tmp)
+    
+    return aligned_init, anchors, Ts, scales
 
 
 # def align_init_pair(adata1, 
 #                     adata2, 
 #                     spatial_key1,
 #                     spatial_key2 = None,
 #                     num_mnn = 1,
@@ -168,124 +260,52 @@
 #         adata1.obsm[key_added] = adata1.obsm[spatial_key1]
     
 #     adata2.obsm[key_added] = transform(adata2.obsm[spatial_key2], T)
     
 #     return adata1, adata2, pair, T
 
 
-def initial_alignment(  adatas, 
-                        spatial_key = 'spatial',
-                        emb_key = 'HAN_SE',
-                        num_mnn = 1, 
-                        key_added = 'transform_init'
-                        ):
-    
-    '''
-    Perform initial alignment for adatas according to the similarity of emb_key.
-    Input:
-      adatas:       Adata list to be aligned
-      spatial_key:  Key of spatial coordinates in .obsm 
-      emb_key:      The key used to calculate spot similarity in .obsm
-      num_mnn:      The number of mutual nearest neighbors calculated according to emb_key
-      key_added:    Key of transformed coordinates added in .obsm
-    Returns:
-      adatas:       Aligned adata list with 'transformed' in .obsm
-      anchors:      np.array of indices of nearest neighbor pairs
-    '''
-    
-    aligned_init = []
-    anchors = []
-    Ts = []
-    
-    print('Performing initial alignment of the 1 pair of data...')
-    
-    # initial alignment of the first two adatas
-    adata1, adata2 = adatas[0], adatas[1]
-    
-    adata1, adata2, anchor_tmp, T_tmp = align_init_pair(adata1, 
-                                                        adata2, 
-                                                        spatial_key1 = spatial_key,
-                                                        spatial_key2 = None,
-                                                        num_mnn = num_mnn, 
-                                                        emb_key = emb_key,
-                                                        key_added = key_added
-                                                        )
-    
-    aligned_init.append(adata1)
-    aligned_init.append(adata2)
-    anchors.append(anchor_tmp)
-    Ts.append(T_tmp)
-    
-    # initial alignment of the rest adatas
-    if len(aligned_init)!=len(adatas):
-        for i in range(1, len(adatas)-1):
-            
-            print(f'Performing initial alignment of the {i+1} pair of data...')
-            
-            adata1_tmp = aligned_init[-1]
-            adata2_tmp = adatas[i+1]
-            
-            for T_ in Ts:
-                adata2_tmp.obsm[spatial_key] = transform(adata2_tmp.obsm[spatial_key], T_)
-            
-            _, adata2_tmp, anchor_tmp, T_tmp = align_init_pair( adata1_tmp, 
-                                                                adata2_tmp, 
-                                                                spatial_key1 = key_added, 
-                                                                spatial_key2 = spatial_key, 
-                                                                num_mnn = num_mnn, 
-                                                                emb_key = emb_key,
-                                                                key_added = key_added
-                                                               )
-                    
-            aligned_init.append(adata2_tmp)
-            anchors.append(anchor_tmp)
-            Ts.append(T_tmp)
-    
-    return aligned_init, anchors, Ts
-
-
-
 
-def initial_alignment_( adatas, 
-                        spatial_key = 'spatial',
-                        emb_key = 'HAN_SE',
-                        num_mnn = 1, 
-                        key_added = 'transform_init'
-                        ):
-    '''
-    Perform initial alignment for adatas according to the similarity of emb_key.
-    Input:
-      adatas:       Adata list to be aligned
-      spatial_key:  Key of spatial coordinates in .obsm 
-      emb_key:      The key used to calculate spot similarity in .obsm
-      num_mnn:      The number of mutual nearest neighbors calculated according to emb_key
-      key_added:    Key of transformed coordinates added in .obsm
-    Returns:
-      adatas:       Aligned adata list with 'transformed' in .obsm
-      anchors:      np.array of indices of nearest neighbor pairs
-    '''
+# def initial_alignment_( adatas, 
+#                         spatial_key = 'spatial',
+#                         emb_key = 'HAN_SE',
+#                         num_mnn = 1, 
+#                         key_added = 'transform_init'
+#                         ):
+#     '''
+#     Perform initial alignment for adatas according to the similarity of emb_key.
+#     Input:
+#       adatas:       Adata list to be aligned
+#       spatial_key:  Key of spatial coordinates in .obsm 
+#       emb_key:      The key used to calculate spot similarity in .obsm
+#       num_mnn:      The number of mutual nearest neighbors calculated according to emb_key
+#       key_added:    Key of transformed coordinates added in .obsm
+#     Returns:
+#       adatas:       Aligned adata list with 'transformed' in .obsm
+#       anchors:      np.array of indices of nearest neighbor pairs
+#     '''
     
-    Ts_init = []
-    for i in range(len(adatas)-1):
-        adata1 = adatas[i]
-        adata2 = adatas[i+1]
-        _, _, _, T_ = align_init_pair(  adata1, 
-                                        adata2, 
-                                        spatial_key1 = spatial_key,
-                                        spatial_key2 = None,
-                                        num_mnn = num_mnn,
-                                        emb_key = emb_key,
-                                        key_added = key_added
-                                        )
-        Ts_init.append(T_)
-    # Compute initial transformed coordinates
-    for i in range(len(adatas)):          
-        adatas[i].obsm[key_added] = adatas[i].obsm[spatial_key]
-        if i != 0:
-            T_tmp = Ts_init[:i]
-            for T_ in T_tmp:
-                adatas[i].obsm[key_added] = transform(adatas[i].obsm[key_added], T_)
-    return adatas, Ts_init
+#     Ts_init = []
+#     for i in range(len(adatas)-1):
+#         adata1 = adatas[i]
+#         adata2 = adatas[i+1]
+#         _, _, _, T_ = align_init_pair(  adata1, 
+#                                         adata2, 
+#                                         spatial_key1 = spatial_key,
+#                                         spatial_key2 = None,
+#                                         num_mnn = num_mnn,
+#                                         emb_key = emb_key,
+#                                         key_added = key_added
+#                                         )
+#         Ts_init.append(T_)
+#     # Compute initial transformed coordinates
+#     for i in range(len(adatas)):          
+#         adatas[i].obsm[key_added] = adatas[i].obsm[spatial_key]
+#         if i != 0:
+#             T_tmp = Ts_init[:i]
+#             for T_ in T_tmp:
+#                 adatas[i].obsm[key_added] = transform(adatas[i].obsm[key_added], T_)
+#     return adatas, Ts_init
```

### Comparing `STAIR-tools-1.2.7/STAIR/location/edge_detection.py` & `STAIR-tools-1.2.8/STAIR/location/edge_detection.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/location/edge_detection1.py` & `STAIR-tools-1.2.8/STAIR/location/edge_detection1.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/location/transformation.py` & `STAIR-tools-1.2.8/STAIR/location/transformation.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR/utils.py` & `STAIR-tools-1.2.8/STAIR/utils.py`

 * *Files identical despite different names*

### Comparing `STAIR-tools-1.2.7/STAIR_tools.egg-info/SOURCES.txt` & `STAIR-tools-1.2.8/STAIR_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

