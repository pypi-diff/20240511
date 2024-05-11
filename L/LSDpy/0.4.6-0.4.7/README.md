# Comparing `tmp/LSDpy-0.4.6.tar.gz` & `tmp/lsdpy-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LSDpy-0.4.6.tar", last modified: Fri Mar 15 02:58:08 2024, max compression
+gzip compressed data, was "lsdpy-0.4.7.tar", last modified: Sat May 11 04:21:17 2024, max compression
```

## Comparing `LSDpy-0.4.6.tar` & `lsdpy-0.4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-03-15 02:58:08.860475 LSDpy-0.4.6/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1072 2022-03-04 03:34:07.000000 LSDpy-0.4.6/LICENSE
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-03-15 02:58:08.856475 LSDpy-0.4.6/LSDpy/
--rw-rw-r--   0 colin     (1000) colin     (1000)       36 2024-03-11 19:49:23.000000 LSDpy-0.4.6/LSDpy/__init__.py
--rw-r--r--   0 colin     (1000) colin     (1000)    33662 2024-03-11 19:49:15.000000 LSDpy-0.4.6/LSDpy/lsdpFunc.py
--rwxr--r--   0 colin     (1000) colin     (1000)    13507 2024-03-11 20:01:25.000000 LSDpy-0.4.6/LSDpy/lsdpy.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-03-15 02:58:08.860475 LSDpy-0.4.6/LSDpy.egg-info/
--rw-r--r--   0 colin     (1000) colin     (1000)    15129 2024-03-15 02:58:08.000000 LSDpy-0.4.6/LSDpy.egg-info/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)      259 2024-03-15 02:58:08.000000 LSDpy-0.4.6/LSDpy.egg-info/SOURCES.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2024-03-15 02:58:08.000000 LSDpy-0.4.6/LSDpy.egg-info/dependency_links.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       46 2024-03-15 02:58:08.000000 LSDpy-0.4.6/LSDpy.egg-info/entry_points.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       23 2024-03-15 02:58:08.000000 LSDpy-0.4.6/LSDpy.egg-info/requires.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        6 2024-03-15 02:58:08.000000 LSDpy-0.4.6/LSDpy.egg-info/top_level.txt
--rw-r--r--   0 colin     (1000) colin     (1000)    15129 2024-03-15 02:58:08.860475 LSDpy-0.4.6/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)    14431 2024-03-11 19:49:38.000000 LSDpy-0.4.6/README.md
--rw-rw-r--   0 colin     (1000) colin     (1000)      947 2024-03-15 02:54:39.000000 LSDpy-0.4.6/pyproject.toml
--rw-rw-r--   0 colin     (1000) colin     (1000)       38 2024-03-15 02:58:08.860475 LSDpy-0.4.6/setup.cfg
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-11 04:21:17.587981 lsdpy-0.4.7/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1072 2022-03-04 03:34:07.000000 lsdpy-0.4.7/LICENSE
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-11 04:21:17.587981 lsdpy-0.4.7/LSDpy/
+-rw-rw-r--   0 colin     (1000) colin     (1000)       36 2024-03-15 03:01:36.000000 lsdpy-0.4.7/LSDpy/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)    33896 2024-05-10 03:53:20.000000 lsdpy-0.4.7/LSDpy/lsdpFunc.py
+-rwxrwxr-x   0 colin     (1000) colin     (1000)    13559 2024-05-10 03:53:16.000000 lsdpy-0.4.7/LSDpy/lsdpy.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2024-05-11 04:21:17.587981 lsdpy-0.4.7/LSDpy.egg-info/
+-rw-r--r--   0 colin     (1000) colin     (1000)    15138 2024-05-11 04:21:17.000000 lsdpy-0.4.7/LSDpy.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)      259 2024-05-11 04:21:17.000000 lsdpy-0.4.7/LSDpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2024-05-11 04:21:17.000000 lsdpy-0.4.7/LSDpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       46 2024-05-11 04:21:17.000000 lsdpy-0.4.7/LSDpy.egg-info/entry_points.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       23 2024-05-11 04:21:17.000000 lsdpy-0.4.7/LSDpy.egg-info/requires.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        6 2024-05-11 04:21:17.000000 lsdpy-0.4.7/LSDpy.egg-info/top_level.txt
+-rw-r--r--   0 colin     (1000) colin     (1000)    15138 2024-05-11 04:21:17.587981 lsdpy-0.4.7/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)    14440 2024-05-10 03:55:33.000000 lsdpy-0.4.7/README.md
+-rw-rw-r--   0 colin     (1000) colin     (1000)      947 2024-05-10 03:51:59.000000 lsdpy-0.4.7/pyproject.toml
+-rw-rw-r--   0 colin     (1000) colin     (1000)       38 2024-05-11 04:21:17.587981 lsdpy-0.4.7/setup.cfg
```

### Comparing `LSDpy-0.4.6/LICENSE` & `lsdpy-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LSDpy-0.4.6/LSDpy/lsdpFunc.py` & `lsdpy-0.4.7/LSDpy/lsdpFunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,45 +321,51 @@
         self.specSigI = np.zeros(self.npix)
         self.specV = np.zeros(self.npix)
         self.specSigV = np.zeros(self.npix)
         self.specN1 = np.zeros(self.npix)
         self.specSigN1 = np.zeros(self.npix)
         self.specN2 = np.zeros(self.npix)
         self.specSigN2 = np.zeros(self.npix)
+        self.header = None
 
-    def save(self, fname, header=None, params=None):
-        #Save the LSD profile to a file.
-        #finally convert I from 1-I to full I/Ic units at output
-        oFile = open(fname, 'w')
-
-        #Add the mask normalizing parameters to the header
+    def makeHeader(self, headerObs=None, params=None):
+        #Generate the header line for the LSD profile file
+        #Use the input observation header if it exists
+        #Then add the mask normalizing parameters to the header
         if params == None:
-            headerAdd = ''
+            headerAdd = '\n'
         else:
             sFormat = ' normalizing: d={:5.3f} lande={:5.3f} wl={:6.1f} (I norm weight {:5.3f}, V norm weight {:7.3f})\n'
             headerAdd = sFormat.format(params.normDepth, params.normLande,
                                        params.normWave, params.normDepth,
                                        params.normDepth*params.normLande
                                        *params.normWave)
         
-        if header == None:
+        if headerObs == None:
             #The observation reading function will usually provide a placeholder
             #header of '#\n' if the file had no header, so this may be unused. 
-            headerTxt = '***LSD profile' + headerAdd
+            self.header = '***LSD profile' + headerAdd
         else:
-            headerTxt = header.strip() + headerAdd
-        oFile.write(headerTxt)
+            self.header = headerObs.strip() + headerAdd
+        return
+
+    def save(self, fname):
+        #Save the LSD profile to a file.
+        #finally convert I from 1-I to full I/Ic units at output
+        oFile = open(fname, 'w')
+        if self.header is not None:
+            oFile.write(self.header)
         
         oFile.write(' {:d} 6\n'.format(self.npix))
         for i in range(self.npix):
             oFile.write('{:>12.6f} {:>13.6e} {:>13.6e} {:>13.6e} {:>13.6e} {:>13.6e} {:>13.6e}\n'.format(
                 self.vel[i], 1.-self.specI[i], self.specSigI[i], self.specV[i],
                 self.specSigV[i], self.specN1[i], self.specSigN1[i]))
         oFile.close()
-        return headerTxt
+        return
 
     def lsdplot(self,fname):
         import matplotlib.pyplot as plt
         
         # Set up axes and put y-axis labels on the right
         fig, (ax1, ax2, ax3) = plt.subplots(3, sharex=True, gridspec_kw = {'height_ratios':[1, 1, 3]})
         ax1.yaxis.set_label_position("right")
```

### Comparing `LSDpy-0.4.6/LSDpy/lsdpy.py` & `lsdpy-0.4.7/LSDpy/lsdpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 #
 # Main LSD code
 
-__version__ = "0.4.6"
+__version__ = "0.4.7"
 
 import numpy as np
 try:
     from . import lsdpFunc
 except ImportError:
     import lsdpFunc as lsdpFunc
 
@@ -79,17 +79,17 @@
              Optionally also returns output model spectrum as a tuple of arrays.
     """
     
     #Read input data
     params = lsdpFunc.paramsLSD('inlsd.dat')
     
     #Use passed parameters, if they exist
+    outputProfName = outName
     if(observation != None):    params.inObs = observation
     if(mask != None):           params.inMask = mask
-    if(outName != None):        outputProfName = outName
     if(velStart != None):       params.velStart = velStart
     if(velEnd != None):         params.velEnd = velEnd
     if(velPixel != None):       params.pixVel = velPixel
     if(normDepth != None):      params.normDepth = normDepth
     if(normLande != None):      params.normLande = normLande
     if(normWave != None):       params.normWave = normWave
     if(removeContPol != None):  params.removeContPol = removeContPol
@@ -128,15 +128,15 @@
     prof = lsdpFunc.prof(params)
     
     #trim the observation's wavelength range
     obs.setInRange(mask, prof)
     
     #Get average observed wavelength spacing (spending a bit of memory for speed)
     wlStep = obs.wlOrig[1:] - obs.wlOrig[:-1]
-    indWlSteps = np.where( (wlStep > 0.) & (wlStep < 0.01))[0]
+    indWlSteps = np.where( (wlStep > 0.) & (wlStep < 0.1))[0]
     obsAvgVel = np.average( wlStep[indWlSteps]/obs.wlOrig[indWlSteps]*c )
     print('Average observed spec velocity spacing: {:.6f} km/s'.format(
         obsAvgVel))
     
     
     #Print some information about the LSD profile to be calculated
     #And output some basic error checking
@@ -186,24 +186,27 @@
     lsdpFunc.scaleErr(prof.specSigN1, chi2N1, obs.wl.shape[0], prof.npix)
     lsdpFunc.zeroProf(prof.specN1, prof.specSigN1, params.removeContPol)
     
     #check for detections
     lsdpFunc.nullTest(prof)
     
     #Save and return the results
-    headerTxt = prof.save(outputProfName, obs.header, params)
+    prof.makeHeader(obs.header, params)
+    if (outputProfName is not None) and (outputProfName != ''):
+        prof.save(outputProfName)
+    
     if(params.fLSDPlotImg != 0):
         prof.lsdplot(params.outPlotImgName)
-        
+    
     if(params.fSaveModelSpec != 0):
             return (prof.vel, 1.-prof.specI, prof.specSigI, prof.specV, 
-                    prof.specSigV, prof.specN1, prof.specSigN1, headerTxt, modelSpec)
+                    prof.specSigV, prof.specN1, prof.specSigN1, prof.header, modelSpec)
 
     return (prof.vel, 1.-prof.specI, prof.specSigI, prof.specV, prof.specSigV,
-            prof.specN1, prof.specSigN1, headerTxt)
+            prof.specN1, prof.specSigN1, prof.header)
 
 
 def make_inlsd_file(inFname):
     """Generate a default inlsd.dat file
 
     This won't be suitable for all cases,
     but provides some resonable default values."""
```

### Comparing `LSDpy-0.4.6/LSDpy.egg-info/PKG-INFO` & `lsdpy-0.4.7/LSDpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LSDpy
-Version: 0.4.6
+Version: 0.4.7
 Summary: Least Squares Deconvolution for spectropolarimetric analysis
 Author-email: Colin Folsom <fosomcp+dev@gmail.com>
 Project-URL: Homepage, https://github.com/folsomcp/LSDpy
 Project-URL: Documentation, https://folsomcp.github.io/specpolFlow/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
@@ -144,15 +144,15 @@
 An estimate of the velocity range that the line spans is printed "line range estimate".  It is based on Stokes I, if the line shape or continuum are particularly strange then the estimate may be wrong.  The line range is taken to be where the profile drops 4 sigma below the continuum level.  The continuum level is estimated from the first and last 20 points in the profile.  The line range is used to compute detections statistics.
 
 The detections statistics are printed for Stokes V, and then N.  The chi^2 of the null model (a flat line) fit to the observation, for the portion inside the line, is printed.  The code also prints the detection probability, and false alarm probability, for that chi^2.  The detection probability is the probability that the null model disagrees with the observation.  Then the code prints the same information calculated outside the line, as a diagnostic test.  This is then repeated for the null.  When operating well, there would be a detection inside the line for Stokes V, but no detection outside the line in V, inside the line in N or outside the line in N.  Currently the code uses detection probabilities of 0.0-0.99 as "non-detection", 0.99-0.9999 as "marginal detections", and > 0.9999 as "definite detections". 
 
 
 ## Change Log
 
-0.4.6 Reogranized the files to work more conveinetly with SetupTools and the PyPI server, for eventual distribution with pip.  Renamed the lsdpy.main function to lsdpy.lsd.  Added a feature to generate a template inlsd.dat file if one does not exist, when LSDpy is ran from the command line.
+0.4.6 & 0.4.7 Reorganized the files to work more conveniently with SetupTools and the PyPI server, for eventual distribution with pip.  Renamed the lsdpy.main function to lsdpy.lsd.  Added a feature to generate a template inlsd.dat file if one does not exist, when LSDpy is ran from the command line.
 
 0.4.5 Added an \_\_init\_\_.py file, for more convenient importing LSDpy as a package.  Added the LSD file header as another return value to the lsdpy.main function.
 
 0.4.4 Added an option to save the LSD model 'spectrum' with a command line argument.  Also fixed a bug where the model spectrum wasn't saved even though the flag in inlsd.dat was set.
 
 0.4.3 When calling LSDpy as function inside another Python script, added an option to return the model 'spectrum' (convolution of the LSD profile and line mask).
```

### Comparing `LSDpy-0.4.6/PKG-INFO` & `lsdpy-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LSDpy
-Version: 0.4.6
+Version: 0.4.7
 Summary: Least Squares Deconvolution for spectropolarimetric analysis
 Author-email: Colin Folsom <fosomcp+dev@gmail.com>
 Project-URL: Homepage, https://github.com/folsomcp/LSDpy
 Project-URL: Documentation, https://folsomcp.github.io/specpolFlow/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
@@ -144,15 +144,15 @@
 An estimate of the velocity range that the line spans is printed "line range estimate".  It is based on Stokes I, if the line shape or continuum are particularly strange then the estimate may be wrong.  The line range is taken to be where the profile drops 4 sigma below the continuum level.  The continuum level is estimated from the first and last 20 points in the profile.  The line range is used to compute detections statistics.
 
 The detections statistics are printed for Stokes V, and then N.  The chi^2 of the null model (a flat line) fit to the observation, for the portion inside the line, is printed.  The code also prints the detection probability, and false alarm probability, for that chi^2.  The detection probability is the probability that the null model disagrees with the observation.  Then the code prints the same information calculated outside the line, as a diagnostic test.  This is then repeated for the null.  When operating well, there would be a detection inside the line for Stokes V, but no detection outside the line in V, inside the line in N or outside the line in N.  Currently the code uses detection probabilities of 0.0-0.99 as "non-detection", 0.99-0.9999 as "marginal detections", and > 0.9999 as "definite detections". 
 
 
 ## Change Log
 
-0.4.6 Reogranized the files to work more conveinetly with SetupTools and the PyPI server, for eventual distribution with pip.  Renamed the lsdpy.main function to lsdpy.lsd.  Added a feature to generate a template inlsd.dat file if one does not exist, when LSDpy is ran from the command line.
+0.4.6 & 0.4.7 Reorganized the files to work more conveniently with SetupTools and the PyPI server, for eventual distribution with pip.  Renamed the lsdpy.main function to lsdpy.lsd.  Added a feature to generate a template inlsd.dat file if one does not exist, when LSDpy is ran from the command line.
 
 0.4.5 Added an \_\_init\_\_.py file, for more convenient importing LSDpy as a package.  Added the LSD file header as another return value to the lsdpy.main function.
 
 0.4.4 Added an option to save the LSD model 'spectrum' with a command line argument.  Also fixed a bug where the model spectrum wasn't saved even though the flag in inlsd.dat was set.
 
 0.4.3 When calling LSDpy as function inside another Python script, added an option to return the model 'spectrum' (convolution of the LSD profile and line mask).
```

### Comparing `LSDpy-0.4.6/README.md` & `lsdpy-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 An estimate of the velocity range that the line spans is printed "line range estimate".  It is based on Stokes I, if the line shape or continuum are particularly strange then the estimate may be wrong.  The line range is taken to be where the profile drops 4 sigma below the continuum level.  The continuum level is estimated from the first and last 20 points in the profile.  The line range is used to compute detections statistics.
 
 The detections statistics are printed for Stokes V, and then N.  The chi^2 of the null model (a flat line) fit to the observation, for the portion inside the line, is printed.  The code also prints the detection probability, and false alarm probability, for that chi^2.  The detection probability is the probability that the null model disagrees with the observation.  Then the code prints the same information calculated outside the line, as a diagnostic test.  This is then repeated for the null.  When operating well, there would be a detection inside the line for Stokes V, but no detection outside the line in V, inside the line in N or outside the line in N.  Currently the code uses detection probabilities of 0.0-0.99 as "non-detection", 0.99-0.9999 as "marginal detections", and > 0.9999 as "definite detections". 
 
 
 ## Change Log
 
-0.4.6 Reogranized the files to work more conveinetly with SetupTools and the PyPI server, for eventual distribution with pip.  Renamed the lsdpy.main function to lsdpy.lsd.  Added a feature to generate a template inlsd.dat file if one does not exist, when LSDpy is ran from the command line.
+0.4.6 & 0.4.7 Reorganized the files to work more conveniently with SetupTools and the PyPI server, for eventual distribution with pip.  Renamed the lsdpy.main function to lsdpy.lsd.  Added a feature to generate a template inlsd.dat file if one does not exist, when LSDpy is ran from the command line.
 
 0.4.5 Added an \_\_init\_\_.py file, for more convenient importing LSDpy as a package.  Added the LSD file header as another return value to the lsdpy.main function.
 
 0.4.4 Added an option to save the LSD model 'spectrum' with a command line argument.  Also fixed a bug where the model spectrum wasn't saved even though the flag in inlsd.dat was set.
 
 0.4.3 When calling LSDpy as function inside another Python script, added an option to return the model 'spectrum' (convolution of the LSD profile and line mask).
```

### Comparing `LSDpy-0.4.6/pyproject.toml` & `lsdpy-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LSDpy"
-version = "0.4.6"
+version = "0.4.7"
 authors = [ { name="Colin Folsom", email="fosomcp+dev@gmail.com" },
 ]
 description = "Least Squares Deconvolution for spectropolarimetric analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
```

