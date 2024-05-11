# Comparing `tmp/eyegestures-1.3.4.tar.gz` & `tmp/eyegestures-1.4.4.tar.gz`

## Comparing `eyegestures-1.3.4.tar` & `eyegestures-1.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/Fixation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/__init__.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/calibration.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/eye.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/eyegestures.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/face.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/gazeContexter.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/gazeEstimator.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/gevent.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/processing.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/scalling_test.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker_test.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/utils.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/clusters.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/dataPoints.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/heatmap.py
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/screenTracker.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 eyegestures-1.3.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-1.3.4/LICENSE
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 eyegestures-1.3.4/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-1.3.4/pyproject.toml
--rw-r--r--   0        0        0    51549 2020-02-02 00:00:00.000000 eyegestures-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/Fixation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/__init__.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/calibration.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/eye.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/eyegestures.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/face.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/gazeContexter.py
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/gazeEstimator.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/gevent.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/processing.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/scalling_test.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/screenTracker_test.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/utils.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/screenTracker/clusters.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/screenTracker/dataPoints.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/screenTracker/heatmap.py
+-rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 eyegestures-1.4.4/eyeGestures/screenTracker/screenTracker.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eyegestures-1.4.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-1.4.4/LICENSE
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 eyegestures-1.4.4/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0    51749 2020-02-02 00:00:00.000000 eyegestures-1.4.4/PKG-INFO
```

### Comparing `eyegestures-1.3.4/eyeGestures/Fixation.py` & `eyegestures-1.4.4/eyeGestures/Fixation.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/calibration.py` & `eyegestures-1.4.4/eyeGestures/calibration.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/eye.py` & `eyegestures-1.4.4/eyeGestures/eye.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,17 @@
 
         return self.height/2
 
     def getLandmarks(self):
         """function returning eye landmarks"""
 
         return self.region
+    
+    def getBoundingBox(self):
+        return (self.x,self.y,self.width,self.height)
 
     def _process(self, image, region):
         h, w, _ = image.shape
 
         mask = np.full((h, w), 0, dtype=np.uint8)
         background = np.zeros((h, w), dtype=np.uint8)
         cv2.fillPoly(mask, [region], 0)
```

### Comparing `eyegestures-1.3.4/eyeGestures/eyegestures.py` & `eyegestures-1.4.4/eyeGestures/eyegestures.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/face.py` & `eyegestures-1.4.4/eyeGestures/face.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/gazeContexter.py` & `eyegestures-1.4.4/eyeGestures/gazeContexter.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,28 @@
 
 
 class Gcontext:
     """Helper class for Gcontext"""
 
     def __init__(self,
                  display,
+                 face,
                  roi,
                  edges,
                  cluster_boundaries,
                  gazeBuffor,
                  l_pupil,
                  r_pupil,
                  l_eye_buff,
                  r_eye_buff,
                  fixation,
                  calibration):
 
         self.roi = roi
+        self.face = face
         self.edges = edges
         self.cluster_boundaries = cluster_boundaries
         self.gazeBuffor = gazeBuffor
         self.l_pupil = l_pupil
         self.r_pupil = r_pupil
         self.l_eye_buff = l_eye_buff
         self.r_eye_buff = r_eye_buff
@@ -83,37 +85,39 @@
 
     def __init__(self):
         self.contexter = Contexter()
 
     def get(self,
             id,
             display,
+            face=None,
             roi=dp.ScreenROI(285, 105, 80, 15),
             edges=dp.ScreenROI(285, 105, 80, 15),
             cluster_boundaries=dp.ScreenROI(225, 125, 20, 20),
             buffor=Buffor(200),
             l_pupil=Buffor(20),
             r_pupil=Buffor(20),
             l_eye_buff=Buffor(20),
             r_eye_buff=Buffor(20),
             fixation=Fixation(0, 0, 100),
             calibration=False):
         """Function creating new context or returning if id already exists"""
 
-        context = Gcontext(display,
-                           roi,
-                           edges,
-                           cluster_boundaries,
-                           buffor,
-                           l_pupil,
-                           r_pupil,
-                           l_eye_buff,
-                           r_eye_buff,
-                           fixation,
-                           calibration)
+        context = Gcontext(display=display,
+                           face=face,
+                           roi=roi,
+                           edges=edges,
+                           cluster_boundaries=cluster_boundaries,
+                           gazeBuffor=buffor,
+                           l_pupil=l_pupil,
+                           r_pupil=r_pupil,
+                           l_eye_buff=l_eye_buff,
+                           r_eye_buff=r_eye_buff,
+                           fixation=fixation,
+                           calibration=calibration)
 
         if self.contexter.addContext(id, context):
             return context
         else:
             return self.contexter.getContext(id)
 
     def update(self,
```

### Comparing `eyegestures-1.3.4/eyeGestures/gazeEstimator.py` & `eyegestures-1.4.4/eyeGestures/gazeEstimator.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,14 +33,17 @@
                  roi_x, roi_y,
                  roi_width, roi_height,
                  monitor_offset_x=0,
                  monitor_offset_y=0):
 
         self.screen = dp.Screen(screen_width, screen_heigth)
 
+        self.offset_x = 0
+        self.offset_y = 0
+
         self.roi_x = roi_x
         self.roi_y = roi_y
         self.roi_width = roi_width
         self.roi_height = roi_height
 
         self.eye_screen_w = eye_screen_w
         self.eye_screen_h = eye_screen_h
@@ -105,31 +108,40 @@
         event = None
         face_mesh = self.getFeatures(image)
         if not face_mesh:
             return None
 
         self.face.process(image, face_mesh)
 
-        context = self.GContext.get(context_id, display, roi=dp.ScreenROI(
-            self.roi_x,
-            self.roi_y,
-            self.roi_width,
-            self.roi_height),
+        context = self.GContext.get(context_id, display,
+            face = None,
+            roi =dp.ScreenROI(
+                self.roi_x,
+                self.roi_y,
+                self.roi_width,
+                self.roi_height),
             edges=dp.ScreenROI(285, 105, 80, 15),
             cluster_boundaries=dp.ScreenROI(225, 125, 20, 20),
             buffor=Buffor(200),
             l_pupil=Buffor(20),
             r_pupil=Buffor(20),
             l_eye_buff=Buffor(20),
             r_eye_buff=Buffor(20),
             fixation=Fixation(0, 0, 100))
         context.calibration = calibration
 
         if not self.face is None:
 
+            if context.face == None:
+                x,y,w,h=self.face.getBoundingBox()
+                i_w = self.face.image_w
+                i_h = self.face.image_h
+                context.face = (x,y,w,h,i_w,i_h)
+
+
             l_eye = self.face.getLeftEye()
             r_eye = self.face.getRightEye()
 
             # TODO: check what happens here before with l_pupil
             intersection_x, _ = self.__gaze_intersection(
                 l_eye, r_eye, context.l_eye_buff, context.r_eye_buff)
             l_point, l_buffor = self.__pupil(
@@ -142,14 +154,50 @@
 
             compound_point = np.array(((l_point + r_point)/2), dtype=np.uint32)
 
             blink = l_eye.getBlink() or r_eye.getBlink()
             if blink != True:
                 context.gazeBuffor.add(compound_point)
 
+            print("adjusting roi")
+            if blink != True:
+                # current face radius
+                face_x,face_y,face_w,face_h = self.face.getBoundingBox()
+                image_w = self.face.image_w
+                image_h = self.face.image_h
+
+                face_w_perc = face_w/image_w
+                face_h_perc = face_h/image_h
+
+                # # prev current face radius
+                c_face_x,c_face_y,c_face_w,c_face_h,c_image_w,c_image_h = context.face
+
+                c_face_w_perc = c_face_w/c_image_w
+                c_face_h_perc = c_face_h/c_image_h
+
+                x,y,w,h=self.face.getBoundingBox()
+                i_w = self.face.image_w
+                i_h = self.face.image_h
+                context.face = (x,y,w,h,i_w,i_h)
+
+                # roi update
+
+                # context.roi.x -= diff_face_x * 500 # current size of virtual display
+                # context.roi.y -= diff_face_y * 500 # current size of virtual display
+                if abs(face_w_perc/c_face_w_perc - 1.0) > 0.02:
+                    context.roi.width  = context.roi.width * abs(face_w_perc/c_face_w_perc)
+                    # context.edges.width= context.edges.width * abs(face_w_perc/c_face_w_perc)
+                    context.gazeBuffor.flush()
+                    # context.calibration = True
+                if abs(face_h_perc/c_face_h_perc - 1.0) > 0.02:
+                    context.roi.height = context.roi.height* abs(face_h_perc/c_face_h_perc)
+                    # context.edges.height= context.edges.height * abs(face_w_perc/c_face_w_perc)
+                    context.gazeBuffor.flush()
+                    # context.calibration = True
+
             self.point_screen, roi, cluster = self.screen_man.process(context.gazeBuffor,
                                                                       context.roi,
                                                                       context.edges,
                                                                       self.screen,
                                                                       context.display,
                                                                       context.calibration,
                                                                       (offset_x,
@@ -180,24 +228,30 @@
                 event = Gevent(compound_point,
                                self.freezed_point,
                                blink,
                                fix,
                                l_eye,
                                r_eye,
                                display,
+                               context.roi,
+                               context.edges,
+                               context.cluster_boundaries,
                                context_id)
             else:
                 self.freezed_point = self.point_screen
                 event = Gevent(compound_point,
                                self.point_screen,
                                blink,
                                fix,
                                l_eye,
                                r_eye,
                                display,
+                               context.roi,
+                               context.edges,
+                               context.cluster_boundaries,
                                context_id)
 
         return event
 
     # def get_contextes(self):
     #     """Function returning contextes"""
```

### Comparing `eyegestures-1.3.4/eyeGestures/processing.py` & `eyegestures-1.4.4/eyeGestures/processing.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/scalling_test.py` & `eyegestures-1.4.4/eyeGestures/scalling_test.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/screenTracker_test.py` & `eyegestures-1.4.4/eyeGestures/screenTracker_test.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/utils.py` & `eyegestures-1.4.4/eyeGestures/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,22 @@
         return self.__buffor[0]
 
     def getFirst(self):
         return self.__buffor[len(self.__buffor) - 1]
 
     def getLen(self):
         return len(self.__buffor)
+    
+    def flush(self):
+        tmp = self.__buffor[-1]
+        self.__buffor = []
+        self.__buffor.append(tmp)
+
+    def clear(self):
+        self.__buffor = []
 
 # Bufforless
 
 
 class VideoCapture:
     """Wrapper on openCV2 stream making it bufforless and adding camera search"""
```

### Comparing `eyegestures-1.3.4/eyeGestures/screenTracker/clusters.py` & `eyegestures-1.4.4/eyeGestures/screenTracker/clusters.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/screenTracker/dataPoints.py` & `eyegestures-1.4.4/eyeGestures/screenTracker/dataPoints.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/screenTracker/heatmap.py` & `eyegestures-1.4.4/eyeGestures/screenTracker/heatmap.py`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/eyeGestures/screenTracker/screenTracker.py` & `eyegestures-1.4.4/eyeGestures/screenTracker/screenTracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 
 import eyeGestures.screenTracker.dataPoints as dp
 from eyeGestures.screenTracker.clusters import Clusters
 from eyeGestures.screenTracker.heatmap import Heatmap
 
 # THIS FILE IS SLOWLY BECOMING BLACK MAGIC
 
+def detect_if_inside(point,rect):
+    px = point[0]
+    py = point[1]
+    x,y,width,height = rect.getBoundaries() 
+
+    x_in = x < px and px < x + width
+    y_in = y < py and py < y + height
+    
+    return x_in and y_in
+
 def detect_edges(roi, display, point_on_screen, point_on_display):
     """Function performing edge detection based on point, screen and display sizes"""
     (s_x,s_y) = point_on_screen 
     (d_x,d_y) = point_on_display
 
     x,y,width,height = roi.getBoundaries() 
     new_roi = dp.ScreenROI(x,y,width,height)
@@ -132,14 +142,15 @@
         """Function to update screen processor with new clusters and heatmaps"""
 
         (x,y) = heatmap.getCenter()
         # =====================================
         # ---------histogram obtained----------
         # =====================================
         new_roi = dp.ScreenROI(roi.x,roi.y,roi.width,roi.height)
+        print(f"setting new center: {x,y}")
         new_roi.setCenter(x,y)
         edges.setCenter(x,y)
         # self.eyeScreen.setCenter(x,y) 
         new_roi = scaleUp(new_roi, edges, scale = 0.1)
 
         # =====================================
         # if screen is bigger than edges make it smaller
@@ -184,15 +195,16 @@
     def process(self, buffor, roi, edges, screen, display, calibration, offset):
         """Function doing processing and tracking and calibration of tracker"""
 
         heatmap = Heatmap(screen.width,screen.height,buffor.getBuffor())
         cluster = Clusters(buffor.getBuffor()).getMainCluster()
 
         if cluster is not None:
-   
+
+
             if calibration:
                 roi = self.screen_processor.update(roi, edges, cluster, heatmap)
 
             p, percentage = self.screen_processor.process(
                 buffor.getAvg(20),
                 (offset[0],offset[1]),
                 len(buffor.getBuffor()),
```

### Comparing `eyegestures-1.3.4/LICENSE` & `eyegestures-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.4/README.md` & `eyegestures-1.4.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,63 +3,63 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
 
 ```
 For enterprise avoiding GPL3 licensing there is commercial license!
 ```
 We offer custom integration and managed services. For businesses requiring invoices message us `contact@eyegestures.com`.
 
+### 💜 Sponsors: 
+
+```
+Sponsor us and we can add your link, banner or other promo materials!
+```
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+
+<!-- POLAR-END id=eizdelwu -->
+
 ## 👁️ EyeGestures
 
 EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
 
 <p align="center">
   <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-47d4-b25f-c47ba7f0f4f3" width="300" height="150">
 <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/f3132843-063a-439a-8e1c-2385ddfdccda" width="300
 " height="150">
 </p>
 <p align="center">
 <img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/84aa7436-6153-49bc-b8e6-ccda535f25e6)" width="600
 " height="300">
 </p>
 
-### ⭐ Mission 
+### ⭐ Mission
+
+There is no one-size-fits-all solution, and we believe that diversifying interfaces brings accessibility to digital spaces. Designing eye-driven interfaces provides greater control over computers for those unable to fully utilize their capabilities due to various disabilities, while also offering an additional means of computer control for all users.
 
-There is no one size-fits all solution, and we believe that differentiating interfaces brings accessibility to digital spaces. Designing eye-driven interfaces gives more control over computers to those who cannot fully enjoy their capabilities due to different disabilities, as well as an additional way to control computer to rests. 
+Such technology should not be hindered by expensive eye-tracking hardware, particularly when it is essential for individuals to navigate the digital realm and operate their computers. Many current consumer electronics devices feature built-in native cameras, and ongoing research suggests that achieving eye tracking with reasonable accuracy using these native cameras is feasible.
 
-Such technology should not be paywalled by expensive eye-tracking hardware, especially in case when it is needed to exist in the digital world and operate your computer. Most of the current consumer electronics devices have built-in native cameras, and the current state of research indicates that it is achievable to have eye tracking at reasonable accuracy based on those native cameras. 
+Our mission is to democratize eye-tracking technology, making it accessible to as many people as possible.
 
-Our mission is to bring eye-tracking technology to as many people as possible. 
+While our technology is not flawless, we are committed to continuous improvement and strive for excellence.
 
-Our technology is not perfect, but we strive to be.
+### 📢 Announcements:
+
+<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
 
 ### 📇 Find us:
 - [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
 - [discord](https://discord.gg/FV3RYTuV)
 - [twitter](https://twitter.com/PW4ltz)
 - email: contact@eyegestures.com
 
 Follow us on polar (it costs nothing but you help project!):
 
 <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
 
-### 💜 Sponsors: 
-
-```
-Sponsor us and we can add your link, banner or other promo materials!
-```
-<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
-
-
-
-<!-- POLAR-END id=eizdelwu -->
-
-### 📢 Announcements:
-
-<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
-
 ### 🔥 Web Demos:
 
 - [Main page](https://eyegestures.com/)
 - [Game demo](https://eyegestures.com/game)
 - [Cinema demo](https://eyegestures.com/cinema)
 - [Restaurant](https://eyegestures.com/restaurant)
 
@@ -76,14 +76,16 @@
 ```
 
 ### 🪟 Run Windows App 
 ```
 python3 apps/win_app.py
 ```
 
+Or download it from [`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3)
+
 ### 🔧 Develop 
 
 To begin, you instantiate an EyeGestures object with initial Region of Interest (RoI) parameters. These parameters define a preliminary focus area for the tracker within a virtual 500x500 screen space, which helps in locating the user's gaze more efficiently.
 
 Main `EyeGesture` object provides general configuration initial conditions: 
 
 ```python
```

#### html2text {}

```diff
@@ -1,57 +1,59 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures) ``` For
 enterprise avoiding GPL3 licensing there is commercial license! ``` We offer
 custom integration and managed services. For businesses requiring invoices
-message us `contact@eyegestures.com`. ## ðï¸ EyeGestures EyeGestures is
-open source eyetracking software/library using native webcams and phone camers
-for achieving its goal. The aim of library is to bring accessibility of
-eyetracking and eyedriven interfaces without requirement of obtaining expensive
-hardware.
+message us `contact@eyegestures.com`. ### ð Sponsors: ``` Sponsor us and we
+can add your link, banner or other promo materials! ``` ## ðï¸ EyeGestures
+EyeGestures is open source eyetracking software/library using native webcams
+and phone camers for achieving its goal. The aim of library is to bring
+accessibility of eyetracking and eyedriven interfaces without requirement of
+obtaining expensive hardware.
  [https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-
  47d4-b25f-c47ba7f0f4f3][https://github.com/PeterWaIIace/PeterWaIIace/assets/
                 40773550/f3132843-063a-439a-8e1c-2385ddfdccda]
  [https://github.com/NativeSensors/EyeGestures/assets/40773550/84aa7436-6153-
                            49bc-b8e6-ccda535f25e6)]
-### â­ Mission There is no one size-fits all solution, and we believe that
-differentiating interfaces brings accessibility to digital spaces. Designing
-eye-driven interfaces gives more control over computers to those who cannot
-fully enjoy their capabilities due to different disabilities, as well as an
-additional way to control computer to rests. Such technology should not be
-paywalled by expensive eye-tracking hardware, especially in case when it is
-needed to exist in the digital world and operate your computer. Most of the
-current consumer electronics devices have built-in native cameras, and the
-current state of research indicates that it is achievable to have eye tracking
-at reasonable accuracy based on those native cameras. Our mission is to bring
-eye-tracking technology to as many people as possible. Our technology is not
-perfect, but we strive to be. ### ð Find us: - [RSS](https://polar.sh/
-NativeSensors/
+### â­ Mission There is no one-size-fits-all solution, and we believe that
+diversifying interfaces brings accessibility to digital spaces. Designing eye-
+driven interfaces provides greater control over computers for those unable to
+fully utilize their capabilities due to various disabilities, while also
+offering an additional means of computer control for all users. Such technology
+should not be hindered by expensive eye-tracking hardware, particularly when it
+is essential for individuals to navigate the digital realm and operate their
+computers. Many current consumer electronics devices feature built-in native
+cameras, and ongoing research suggests that achieving eye tracking with
+reasonable accuracy using these native cameras is feasible. Our mission is to
+democratize eye-tracking technology, making it accessible to as many people as
+possible. While our technology is not flawless, we are committed to continuous
+improvement and strive for excellence. ### ð¢ Announcements: _[_P_o_s_t_s_ _o_n
+_P_o_l_a_r_]### ð Find us: - [RSS](https://polar.sh/NativeSensors/
 rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-
 xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U) - [discord](https://discord.gg/FV3RYTuV) -
 [twitter](https://twitter.com/PW4ltz) - email: contact@eyegestures.com Follow
 us on polar (it costs nothing but you help project!): _[_S_u_b_s_c_r_i_b_e_ _o_n_ _P_o_l_a_r_]###
-ð Sponsors: ``` Sponsor us and we can add your link, banner or other promo
-materials! ``` ### ð¢ Announcements: _[_P_o_s_t_s_ _o_n_ _P_o_l_a_r_]### ð¥ Web Demos: -
-[Main page](https://eyegestures.com/) - [Game demo](https://eyegestures.com/
-game) - [Cinema demo](https://eyegestures.com/cinema) - [Restaurant](https://
-eyegestures.com/restaurant) ### ð» Install ``` python3 -m pip install
-eyeGestures ``` Note: you may need to change version of package `eyegestures-
-X.X.X`. ### âï¸ Run ``` python3 examples/simple_example.py ``` ### ðª Run
-Windows App ``` python3 apps/win_app.py ``` ### ð§ Develop To begin, you
-instantiate an EyeGestures object with initial Region of Interest (RoI)
-parameters. These parameters define a preliminary focus area for the tracker
-within a virtual 500x500 screen space, which helps in locating the user's gaze
-more efficiently. Main `EyeGesture` object provides general configuration
-initial conditions: ```python EyeGestures( roi_x = 285 roi_y = 115 roi_width =
-80 roi_height = 15 ) ``` The tracker operates within a virtual screen measuring
-500x500, where it maps the positions of the pupils and other critical facial
-features to deduce the user's gaze direction. Within this space, the Region of
-Interest (RoI) serves as a representation of the user's display, inferred
-through a combination of eye movement and edge detection during calibration.
-After locating the RoI within the 500x500 space, its dimensions are adjusted to
-fit the resolution used in the estimate function, typically described as
+ð¥ Web Demos: - [Main page](https://eyegestures.com/) - [Game demo](https://
+eyegestures.com/game) - [Cinema demo](https://eyegestures.com/cinema) -
+[Restaurant](https://eyegestures.com/restaurant) ### ð» Install ``` python3 -
+m pip install eyeGestures ``` Note: you may need to change version of package
+`eyegestures-X.X.X`. ### âï¸ Run ``` python3 examples/simple_example.py ```
+### ðª Run Windows App ``` python3 apps/win_app.py ``` Or download it from
+[`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/
+1.3.4_App_0.0.3) ### ð§ Develop To begin, you instantiate an EyeGestures
+object with initial Region of Interest (RoI) parameters. These parameters
+define a preliminary focus area for the tracker within a virtual 500x500 screen
+space, which helps in locating the user's gaze more efficiently. Main
+`EyeGesture` object provides general configuration initial conditions:
+```python EyeGestures( roi_x = 285 roi_y = 115 roi_width = 80 roi_height = 15 )
+``` The tracker operates within a virtual screen measuring 500x500, where it
+maps the positions of the pupils and other critical facial features to deduce
+the user's gaze direction. Within this space, the Region of Interest (RoI)
+serves as a representation of the user's display, inferred through a
+combination of eye movement and edge detection during calibration. After
+locating the RoI within the 500x500 space, its dimensions are adjusted to fit
+the resolution used in the estimate function, typically described as
 `display_width` by `display_height`. Calibration aims to precisely determine
 the RoI's dimensions. Prior to calibration, the tracker relies on initial
 optional parameters, including: - `roi_x`: The initial x-coordinate of the RoI
 (ranging from 0 to 500). - `roi_y`: The initial y-coordinate of the RoI
 (ranging from 0 to 500). - `roi_width`: The initial width of the RoI before
 calibration (ranging from 0 to 500 - x). - `roi_height`: The initial height of
 the RoI before calibration (ranging from 0 to 500 - x). Next part is obtaining
```

### Comparing `eyegestures-1.3.4/pyproject.toml` & `eyegestures-1.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "test_app.py",
   "test.py",
   "tools/*"
 ]
 
 [project]
 name = "eyeGestures"
-version = "1.3.4"
+version = "1.4.4"
 authors = [
   { name="Piotr Walas", email="piotr.walas@eyegestures.com" },
 ]
 maintainers = [
   { name="Piotr Walas", email="piotr.walas@eyegestures.com" }
 ]
 description = "Package for eye tracking algorithm allowing for development of gaze controlled computer interface"
```

### Comparing `eyegestures-1.3.4/PKG-INFO` & `eyegestures-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eyeGestures
-Version: 1.3.4
+Version: 1.4.4
 Summary: Package for eye tracking algorithm allowing for development of gaze controlled computer interface
 Project-URL: Homepage, https://github.com/NativeSensors/EyeGestures
 Project-URL: Issues, https://github.com/NativeSensors/EyeGestures/Issues
 Author-email: Piotr Walas <piotr.walas@eyegestures.com>
 Maintainer-email: Piotr Walas <piotr.walas@eyegestures.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -693,63 +693,63 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
 
 ```
 For enterprise avoiding GPL3 licensing there is commercial license!
 ```
 We offer custom integration and managed services. For businesses requiring invoices message us `contact@eyegestures.com`.
 
+### 💜 Sponsors: 
+
+```
+Sponsor us and we can add your link, banner or other promo materials!
+```
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+
+<!-- POLAR-END id=eizdelwu -->
+
 ## 👁️ EyeGestures
 
 EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
 
 <p align="center">
   <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-47d4-b25f-c47ba7f0f4f3" width="300" height="150">
 <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/f3132843-063a-439a-8e1c-2385ddfdccda" width="300
 " height="150">
 </p>
 <p align="center">
 <img src="https://github.com/NativeSensors/EyeGestures/assets/40773550/84aa7436-6153-49bc-b8e6-ccda535f25e6)" width="600
 " height="300">
 </p>
 
-### ⭐ Mission 
+### ⭐ Mission
+
+There is no one-size-fits-all solution, and we believe that diversifying interfaces brings accessibility to digital spaces. Designing eye-driven interfaces provides greater control over computers for those unable to fully utilize their capabilities due to various disabilities, while also offering an additional means of computer control for all users.
 
-There is no one size-fits all solution, and we believe that differentiating interfaces brings accessibility to digital spaces. Designing eye-driven interfaces gives more control over computers to those who cannot fully enjoy their capabilities due to different disabilities, as well as an additional way to control computer to rests. 
+Such technology should not be hindered by expensive eye-tracking hardware, particularly when it is essential for individuals to navigate the digital realm and operate their computers. Many current consumer electronics devices feature built-in native cameras, and ongoing research suggests that achieving eye tracking with reasonable accuracy using these native cameras is feasible.
 
-Such technology should not be paywalled by expensive eye-tracking hardware, especially in case when it is needed to exist in the digital world and operate your computer. Most of the current consumer electronics devices have built-in native cameras, and the current state of research indicates that it is achievable to have eye tracking at reasonable accuracy based on those native cameras. 
+Our mission is to democratize eye-tracking technology, making it accessible to as many people as possible.
 
-Our mission is to bring eye-tracking technology to as many people as possible. 
+While our technology is not flawless, we are committed to continuous improvement and strive for excellence.
 
-Our technology is not perfect, but we strive to be.
+### 📢 Announcements:
+
+<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
 
 ### 📇 Find us:
 - [RSS](https://polar.sh/NativeSensors/rss?auth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwYXRfaWQiOiJkMDYxMDFiOC0xYzYyLTQ1MTYtYjg3YS03NTFhOTM3OTIxZmUiLCJzY29wZXMiOiJhcnRpY2xlczpyZWFkIiwidHlwZSI6ImF1dGgiLCJleHAiOjE3NDMxNjg3ODh9.djoi5ARWHr-xFW_XJ6Fwal3JUT1fAbvx4Npl-daBC5U)
 - [discord](https://discord.gg/FV3RYTuV)
 - [twitter](https://twitter.com/PW4ltz)
 - email: contact@eyegestures.com
 
 Follow us on polar (it costs nothing but you help project!):
 
 <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
 
-### 💜 Sponsors: 
-
-```
-Sponsor us and we can add your link, banner or other promo materials!
-```
-<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
-
-
-
-<!-- POLAR-END id=eizdelwu -->
-
-### 📢 Announcements:
-
-<a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
-
 ### 🔥 Web Demos:
 
 - [Main page](https://eyegestures.com/)
 - [Game demo](https://eyegestures.com/game)
 - [Cinema demo](https://eyegestures.com/cinema)
 - [Restaurant](https://eyegestures.com/restaurant)
 
@@ -766,14 +766,16 @@
 ```
 
 ### 🪟 Run Windows App 
 ```
 python3 apps/win_app.py
 ```
 
+Or download it from [`releases`](https://github.com/NativeSensors/EyeGestures/releases/tag/1.3.4_App_0.0.3)
+
 ### 🔧 Develop 
 
 To begin, you instantiate an EyeGestures object with initial Region of Interest (RoI) parameters. These parameters define a preliminary focus area for the tracker within a virtual 500x500 screen space, which helps in locating the user's gaze more efficiently.
 
 Main `EyeGesture` object provides general configuration initial conditions: 
 
 ```python
```

