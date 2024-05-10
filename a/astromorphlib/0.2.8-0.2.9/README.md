# Comparing `tmp/astromorphlib-0.2.8.tar.gz` & `tmp/astromorphlib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromorphlib-0.2.8.tar", last modified: Thu Sep 22 18:59:27 2022, max compression
+gzip compressed data, was "astromorphlib-0.2.9.tar", last modified: Fri Sep 30 20:09:15 2022, max compression
```

## Comparing `astromorphlib-0.2.8.tar` & `astromorphlib-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-22 18:59:27.942105 astromorphlib-0.2.8/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      399 2022-04-05 21:26:30.000000 astromorphlib-0.2.8/LICENSE.txt
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      141 2022-08-10 23:57:37.000000 astromorphlib-0.2.8/MANIFEST.in
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     1994 2022-09-22 18:59:27.942105 astromorphlib-0.2.8/PKG-INFO
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)     1669 2022-09-02 13:44:12.000000 astromorphlib-0.2.8/README.md
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-22 18:59:27.762105 astromorphlib-0.2.8/astromorphlib.egg-info/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)     1994 2022-09-22 18:59:27.000000 astromorphlib-0.2.8/astromorphlib.egg-info/PKG-INFO
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      395 2022-09-22 18:59:27.000000 astromorphlib-0.2.8/astromorphlib.egg-info/SOURCES.txt
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)        1 2022-09-22 18:59:27.000000 astromorphlib-0.2.8/astromorphlib.egg-info/dependency_links.txt
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)        9 2022-09-22 18:59:27.000000 astromorphlib-0.2.8/astromorphlib.egg-info/top_level.txt
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)       38 2022-09-22 18:59:27.942105 astromorphlib-0.2.8/setup.cfg
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      712 2022-09-22 18:24:15.000000 astromorphlib-0.2.8/setup.py
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-22 18:59:27.846105 astromorphlib-0.2.8/stat_lib/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)   294972 2022-05-01 21:05:42.000000 astromorphlib-0.2.8/stat_lib/Table_Arp_Madore_pairs_updated.txt
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)    79583 2022-09-22 18:53:24.000000 astromorphlib-0.2.8/stat_lib/__init__.py
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-22 18:59:27.910105 astromorphlib-0.2.8/stat_lib/__pycache__/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)    46494 2022-09-20 22:54:32.000000 astromorphlib-0.2.8/stat_lib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)    21235 2022-04-12 22:37:01.000000 astromorphlib-0.2.8/stat_lib/__pycache__/stat_lib.cpython-38.pyc
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      312 2022-08-10 21:41:50.000000 astromorphlib-0.2.8/stat_lib/properties.dat
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)   106560 2022-04-05 22:04:36.000000 astromorphlib-0.2.8/stat_lib/zero_points.fits
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-30 20:09:15.553474 astromorphlib-0.2.9/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      399 2022-04-05 21:26:30.000000 astromorphlib-0.2.9/LICENSE.txt
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      141 2022-08-10 23:57:37.000000 astromorphlib-0.2.9/MANIFEST.in
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     1994 2022-09-30 20:09:15.553474 astromorphlib-0.2.9/PKG-INFO
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)     1669 2022-09-02 13:44:12.000000 astromorphlib-0.2.9/README.md
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-30 20:09:15.513474 astromorphlib-0.2.9/astromorphlib.egg-info/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)     1994 2022-09-30 20:09:15.000000 astromorphlib-0.2.9/astromorphlib.egg-info/PKG-INFO
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      395 2022-09-30 20:09:15.000000 astromorphlib-0.2.9/astromorphlib.egg-info/SOURCES.txt
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)        1 2022-09-30 20:09:15.000000 astromorphlib-0.2.9/astromorphlib.egg-info/dependency_links.txt
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)        9 2022-09-30 20:09:15.000000 astromorphlib-0.2.9/astromorphlib.egg-info/top_level.txt
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)       38 2022-09-30 20:09:15.553474 astromorphlib-0.2.9/setup.cfg
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      712 2022-09-30 20:08:16.000000 astromorphlib-0.2.9/setup.py
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-30 20:09:15.513474 astromorphlib-0.2.9/stat_lib/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)   294972 2022-05-01 21:05:42.000000 astromorphlib-0.2.9/stat_lib/Table_Arp_Madore_pairs_updated.txt
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)    80004 2022-09-30 18:29:45.000000 astromorphlib-0.2.9/stat_lib/__init__.py
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2022-09-30 20:09:15.513474 astromorphlib-0.2.9/stat_lib/__pycache__/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)    46770 2022-09-30 18:29:54.000000 astromorphlib-0.2.9/stat_lib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)    21235 2022-04-12 22:37:01.000000 astromorphlib-0.2.9/stat_lib/__pycache__/stat_lib.cpython-38.pyc
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      312 2022-08-10 21:41:50.000000 astromorphlib-0.2.9/stat_lib/properties.dat
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)   106560 2022-04-05 22:04:36.000000 astromorphlib-0.2.9/stat_lib/zero_points.fits
```

### Comparing `astromorphlib-0.2.8/PKG-INFO` & `astromorphlib-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromorphlib
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python scripts to analyze the morphology of isolated/interacting galaxies
 Home-page: https://gitlab.com/joseaher/astromorphlib
 Author: J. A. Hernandez-Jimenez
 Author-email: joseaher@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `astromorphlib-0.2.8/README.md` & `astromorphlib-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `astromorphlib-0.2.8/astromorphlib.egg-info/PKG-INFO` & `astromorphlib-0.2.9/astromorphlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromorphlib
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python scripts to analyze the morphology of isolated/interacting galaxies
 Home-page: https://gitlab.com/joseaher/astromorphlib
 Author: J. A. Hernandez-Jimenez
 Author-email: joseaher@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `astromorphlib-0.2.8/setup.py` & `astromorphlib-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='astromorphlib',
-      version='0.2.8',
+      version='0.2.9',
       description='Python scripts to analyze the morphology of isolated/interacting galaxies',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='J. A. Hernandez-Jimenez',
       author_email='joseaher@gmail.com',
       url = "https://gitlab.com/joseaher/astromorphlib",
       packages=['stat_lib'],
```

### Comparing `astromorphlib-0.2.8/stat_lib/Table_Arp_Madore_pairs_updated.txt` & `astromorphlib-0.2.9/stat_lib/Table_Arp_Madore_pairs_updated.txt`

 * *Files identical despite different names*

### Comparing `astromorphlib-0.2.8/stat_lib/__init__.py` & `astromorphlib-0.2.9/stat_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from astropy.table import Table
 from astroquery import simbad
 from astroquery.ipac.ned import Ned
 from astropy.wcs import wcs
 from astropy.coordinates import SkyCoord
 import astropy.units as u
 
-from photutils import make_source_mask
+from photutils.segmentation import make_source_mask
 from astropy.stats import sigma_clipped_stats
 from photutils.background import Background2D, MedianBackground
 from photutils.segmentation import detect_sources
 from photutils.segmentation import deblend_sources
 
 from astropy.convolution import Gaussian2DKernel
 from astropy.stats import gaussian_fwhm_to_sigma
@@ -407,15 +407,15 @@
     if os.path.exists(outputfile):
         data = ascii.read(outputfile)
     else:
         direcbase = os.path.dirname(os.path.realpath(__file__))
         datat = ascii.read(direcbase + '/properties.dat')
         print (Fore.RED + '\n*It was create the properties.dat to print the out parameters')
 
-        unitst = [str, np.float64, np.float64, np.float64, np.float64, np.float64,
+        unitst = [str, np.float64, np.float64, np.float64, np.float64, str,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
                  np.float64, np.float64, np.float64, np.float64, np.float64,
@@ -431,15 +431,16 @@
         print (data['GAL'][data['GAL']==gal])
         ind=np.where(data['GAL']==gal)[0][0]
 
     else:
         print (Fore.BLACK +'\nRow was created for {}'.format(gal))
         data.add_row()
         ind = -1
-        if len(gal) > len(data['GAL'][0]):
+        len_ar = np.array([len(s) for s in data['GAL']])
+        if len(gal) > np.max(len_ar):
             print ('Change the string format of GAL column')
             #data['GAL'].asdtype = 'str'+str(len(gal))
             new_c = data['GAL'].astype('U'+str(len(gal)))
             data.replace_column('GAL', new_c)
         data['GAL'][ind] = gal
 
     print ('\nsky_mean_statmorph ={:.3f}'.format(morph.sky_mean))
@@ -1206,15 +1207,15 @@
                 bbox_inches='tight')
 
 
 def plot_simbad(gal, tab_gal, conn, size_image_phy, table, user_order=None,
                 user_text=None, xtpos=10, ytpos=20, deltay=10,
                 savefig=None, add_object=True, itsconsider='no', itsgroup='off',
                 Nmembers=0, print_arp='yes', print_scale='yes',
-                usesimbad = 'no', band='R'):
+                usesimbad = 'no', band='R', outputfile='properties.dat'):
 
     idg =np.where(tab_gal['gal']==gal)[0][0]
 
     D = tab_gal['vel'][idg]/H
     arc_kpc = np.tan(np.deg2rad(1./3600.))*D*1e3
     if usesimbad == 'no':
         pix_scima = 0.55
@@ -1269,14 +1270,15 @@
                 ind = -1
                 data['GAL'][ind] = comp
 
             data['ra'][ind] = table['RA_d'][comp_ind]
             data['dec'][ind] = table['DEC_d'][comp_ind]
             data['radvel'][ind] = table['RV_VALUE'][comp_ind]
             data['z'][ind] = table['Z_VALUE'][comp_ind]
+            data['morph_type'] = data['morph_type'].astype(str)
             data['morph_type'][ind] = table['MORPH_TYPE'][comp_ind]
             if itsconsider=='yes':
                 data['Its_considered?'][ind]=1
             if itsconsider=='no':
                 data['Its_considered?'][ind]=0
             if len(user_order) >2:
                 data['Its_group?'][ind]=1
@@ -1485,15 +1487,16 @@
         print ("tab_pro['D_to_main'][ind_g] = sep_kpc")
         print ("tab_pro.write('properties.dat', format='ascii', overwrite=True)")
 
 
 def ex_phot_mod_decals (gal, tab_gal, size_image_phy=50, snr_g = 2.0,
                         areagal=2, band='r', sky_box=[100, 100], deblend='off',
                         psf=1, run_auto='no', show_plot='yes',
-                        nsigma=2, npixels=5, dilate_size=11):
+                        nsigma=2, npixels=5, dilate_size=11,
+                        outputfile='properties.dat'):
 
     idg =np.where(tab_gal['gal']==gal)[0][0]
     D = tab_gal['vel'][idg]/H
     arc_kpc = np.tan(np.deg2rad(1./3600.))*D*1e3
     sc_ima = 0.27
     print (Fore.BLUE +"\nBasic information:")
     print (Fore.BLUE +"-------------------")
@@ -1677,30 +1680,30 @@
         plt.close()
 
     if run_auto == 'no':
 
         part0 = f"\n\nSL.phot_mod_decals('{gal}', tab, size_image_phy={size_image_phy}, "
         part1 = f""" snr_g = {snr_g}, areagal={areagal}, band="{band}", """
         part2 = f"""sky_box = {sky_box},\n deblend ="{deblend}", """
-        part3 = """user_order=[1,2], user_list=["A","B"])"""
+        part3 = """user_order=[1,2], user_list=["A","B"], outputfile={outputfile=})"""
         print(part0 + part1 + part2 + part3)
     else:
 
         maxarea = int(segmc[int(segmc.shape[0]*.5), int(segmc.shape[1]*.5)])-1
 
         part0 = f"\n\nSL.phot_mod_decals('{gal}', tab, size_image_phy={size_image_phy}, "
         part1 = f""" snr_g = {snr_g}, areagal={areagal}, band="{band}", """
         part2 = f"""sky_box = {sky_box},\n deblend ="{deblend}", """
-        part3 = f"""user_order=[{maxarea}], user_list=["{band}"])"""
+        part3 = f"""user_order=[{maxarea}], user_list=["{band}"], outputfile={outputfile=})"""
         print(part0 + part1 + part2 + part3)
 
         phot_mod_decals(gal, tab_gal, size_image_phy=size_image_phy, snr_g = snr_g,
                            areagal=areagal, band=band, sky_box = sky_box,
                            deblend =deblend, user_order=[maxarea], user_list=[band],
-                           show_plot=show_plot)
+                           show_plot=show_plot, outputfile=outputfile)
 
 
 def phot_mod_decals (gal, tab_gal, size_image_phy=50, snr_g = 2.0, areagal=2,
                      band = 'r',
                      user_order=None, user_list=None, sky_box=[100, 100],
                      deblend='off', show_plot='yes',nsigma=2, npixels=5,
                      dilate_size=11, outputfile='properties.dat', eta=0.2):
@@ -1938,14 +1941,16 @@
             size_image_phy)
     if not os.path.exists(path):
         print (f"\nDowloading {path} ...")
         part0 = 'ra={}&dec={}&layer=dr8&pixscale=0.27&bands=g&size={}'.format(
              tab_gal['ra'][idg], tab_gal['dec'][idg], int(size_image))
         targ = home + part0
         print (targ)
+
+        #https://www.legacysurvey.org/viewer/fits-cutout?ra=153.445175&dec=-0.9142411&layer=ls-dr10-early-grz&pixscale=0.27&bands=g&size=420
         #wget.download(targ, out=path)
         request.urlretrieve(targ, path)
     else:
        print (f'\nThe image {path} already exist')
 
     path = 'fits_images/{}_{}_{}kpc.fits'.format(gal[:suf_num], 'r',
            size_image_phy)
```

### Comparing `astromorphlib-0.2.8/stat_lib/__pycache__/__init__.cpython-38.pyc` & `astromorphlib-0.2.9/stat_lib/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Sep 20 22:54:08 2022 UTC, .py size: 83188 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-00000000: 550d 0d0a 0000 0000 9044 2a63 f444 0100  U........D*c.D..
+00000000: 550d 0d0a 0000 0000 9935 3763 8438 0100  U........57c.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0016 0000 0040 0000 0073 ae02 0000 6400  .....@...s....d.
+00000020: 0016 0000 0040 0000 0073 b002 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c05 5a05 6400 6402 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6406 6c0f 6d10 5a10 0100 6400 6407 6c11  d.l.m.Z...d.d.l.
 00000090: 6d12 5a12 0100 6400 6408 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
 000000a0: 0100 6400 6401 6c15 6d16 5a17 0100 6400  ..d.d.l.m.Z...d.
 000000b0: 6409 6c18 6d19 5a19 0100 6400 640a 6c1a  d.l.m.Z...d.d.l.
 000000c0: 6d1b 5a1b 0100 6400 640b 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000d0: 6d1e 5a1e 0100 6400 640c 6c1f 6d20 5a20  m.Z...d.d.l.m Z 
-000000e0: 0100 6400 640d 6c1f 6d21 5a21 0100 6400  ..d.d.l.m!Z!..d.
-000000f0: 640e 6c22 6d23 5a23 0100 6400 640f 6c1a  d.l"m#Z#..d.d.l.
-00000100: 6d24 5a24 0100 6400 6410 6c25 6d26 5a26  m$Z$..d.d.l%m&Z&
-00000110: 0100 6400 6411 6c27 6d28 5a28 0100 6400  ..d.d.l'm(Z(..d.
-00000120: 6412 6c29 6d2a 5a2a 6d2b 5a2b 6d2c 5a2c  d.l)m*Z*m+Z+m,Z,
-00000130: 6d2d 5a2d 6d2e 5a2e 0100 6400 6413 6c2f  m-Z-m.Z...d.d.l/
-00000140: 6d30 5a30 0100 6400 6401 6c31 6d32 5a33  m0Z0..d.d.l1m2Z3
-00000150: 0100 6400 6401 6c18 5a18 6400 6401 6c34  ..d.d.l.Z.d.d.l4
+000000d0: 6d1e 5a1e 0100 6400 640c 6c18 6d1f 5a1f  m.Z...d.d.l.m.Z.
+000000e0: 0100 6400 640d 6c18 6d20 5a20 0100 6400  ..d.d.l.m Z ..d.
+000000f0: 640e 6c21 6d22 5a22 0100 6400 640f 6c1a  d.l!m"Z"..d.d.l.
+00000100: 6d23 5a23 0100 6400 6410 6c24 6d25 5a25  m#Z#..d.d.l$m%Z%
+00000110: 0100 6400 6411 6c26 6d27 5a27 0100 6400  ..d.d.l&m'Z'..d.
+00000120: 6412 6c28 6d29 5a29 6d2a 5a2a 6d2b 5a2b  d.l(m)Z)m*Z*m+Z+
+00000130: 6d2c 5a2c 6d2d 5a2d 0100 6400 6413 6c2e  m,Z,m-Z-..d.d.l.
+00000140: 6d2f 5a2f 0100 6400 6401 6c30 6d31 5a32  m/Z/..d.d.l0m1Z2
+00000150: 0100 6400 6401 6c33 5a33 6400 6401 6c34  ..d.d.l3Z3d.d.l4
 00000160: 5a34 6400 6414 6c35 6d36 5a36 0100 6415  Z4d.d.l5m6Z6..d.
 00000170: 5a37 6416 5a38 6400 6401 6c39 5a39 6400  Z7d.Z8d.d.l9Z9d.
 00000180: 6401 6c3a 5a3a 6400 6401 6c3b 5a3c 6417  d.l:Z:d.d.l;Z<d.
 00000190: 5a3d 6418 5a3e 6419 5a3f 650e 6a40 a041  Z=d.Z>d.Z?e.j@.A
 000001a0: a100 0100 650e 6a40 a042 641a a101 0100  ....e.j@.Bd.....
 000001b0: 650e 6a40 a043 641b 641c 641d 641e 641f  e.j@.Cd.d.d.d.d.
 000001c0: 6420 6421 6422 6423 6424 6425 6426 6427  d d!d"d#d$d%d&d'
@@ -35,600 +35,600 @@
 00000220: 6430 643d 6401 643e 643f 6440 643f 6431  d0d=d.d>d?d@d?d1
 00000230: 6431 6702 6432 6441 6442 6433 6431 6430  d1g.d2dAdBd3d1d0
 00000240: 6434 6435 6437 6438 6442 6436 6616 6443  d4d5d7d8dBd6f.dC
 00000250: 6444 8401 5a48 645a 6446 6447 8401 5a49  dD..ZHdZdFdG..ZI
 00000260: 645b 6449 644a 8401 5a4a 645c 644c 644d  d[dIdJ..ZJd\dLdM
 00000270: 8401 5a4b 645d 644f 6450 8401 5a4c 642e  ..ZKd]dOdP..ZLd.
 00000280: 642f 6430 6451 6431 6431 6702 6432 6441  d/d0dQd1d1g.d2dA
-00000290: 6442 6438 6430 6434 6435 660c 6452 6453  dBd8d0d4d5f.dRdS
-000002a0: 8401 5a4d 642e 642f 6430 6451 6401 6401  ..ZMd.d/d0dQd.d.
-000002b0: 6431 6431 6702 6432 6438 6430 6434 6435  d1d1g.d2d8d0d4d5
-000002c0: 6436 6437 660e 6454 6455 8401 5a4e 645e  d6d7f.dTdU..ZNd^
-000002d0: 6457 6458 8401 5a4f 6401 5300 295f e900  dWdX..ZOd.S.)_..
-000002e0: 0000 004e 2901 da0b 6d61 6b65 5f66 6967  ...N)...make_fig
-000002f0: 7572 6529 02da 0466 6974 73da 0561 7363  ure)...fits..asc
-00000300: 6969 2901 da05 5461 626c 6529 01da 0673  ii)...Table)...s
-00000310: 696d 6261 6429 01da 034e 6564 2901 da03  imbad)...Ned)...
-00000320: 7763 7329 01da 0853 6b79 436f 6f72 6429  wcs)...SkyCoord)
-00000330: 01da 106d 616b 655f 736f 7572 6365 5f6d  ...make_source_m
-00000340: 6173 6b29 01da 1373 6967 6d61 5f63 6c69  ask)...sigma_cli
-00000350: 7070 6564 5f73 7461 7473 2902 da0c 4261  pped_stats)...Ba
-00000360: 636b 6772 6f75 6e64 3244 da10 4d65 6469  ckground2D..Medi
-00000370: 616e 4261 636b 6772 6f75 6e64 2901 da0e  anBackground)...
-00000380: 6465 7465 6374 5f73 6f75 7263 6573 2901  detect_sources).
-00000390: da0f 6465 626c 656e 645f 736f 7572 6365  ..deblend_source
-000003a0: 7329 01da 1047 6175 7373 6961 6e32 444b  s)...Gaussian2DK
-000003b0: 6572 6e65 6c29 01da 1667 6175 7373 6961  ernel)...gaussia
-000003c0: 6e5f 6677 686d 5f74 6f5f 7369 676d 6129  n_fwhm_to_sigma)
-000003d0: 01da 0571 756f 7465 2901 da0b 7572 6c72  ...quote)...urlr
-000003e0: 6574 7269 6576 6529 05da 0e4d 696e 4d61  etrieve)...MinMa
-000003f0: 7849 6e74 6572 7661 6cda 0b53 7172 7453  xInterval..SqrtS
-00000400: 7472 6574 6368 da0c 4173 696e 6853 7472  tretch..AsinhStr
-00000410: 6574 6368 da0e 496d 6167 654e 6f72 6d61  etch..ImageNorma
-00000420: 6c69 7a65 da0f 6d61 6b65 5f6c 7570 746f  lize..make_lupto
-00000430: 6e5f 7267 6229 01da 0446 6f72 6529 01da  n_rgb)...Fore)..
-00000440: 0772 6571 7565 7374 6700 0000 0000 8051  .requestg......Q
-00000450: 4067 0000 0000 804f 1241 da07 7465 7272  @g.....O.A..terr
-00000460: 6169 6e7a 1b68 7474 703a 2f2f 7369 6d62  ainz.http://simb
-00000470: 6164 2e75 2d73 7472 6173 6267 2e66 722f  ad.u-strasbg.fr/
-00000480: 7a1a 6874 7470 3a2f 2f73 696d 6261 642e  z.http://simbad.
-00000490: 6861 7276 6172 642e 6564 752f da0b 636f  harvard.edu/..co
-000004a0: 6f72 6469 6e61 7465 737a 0572 6128 6429  ordinatesz.ra(d)
-000004b0: 7a06 6465 6328 6429 da08 7276 5f76 616c  z.dec(d)..rv_val
-000004c0: 7565 da07 7a5f 7661 6c75 65da 096d 6f72  ue..z_value..mor
-000004d0: 7068 7479 7065 da0b 6469 6d5f 6d61 6a61  phtype..dim_maja
-000004e0: 7869 73da 0b64 696d 5f6d 696e 6178 6973  xis..dim_minaxis
-000004f0: da09 6469 6d5f 616e 676c 657a 0766 6c75  ..dim_anglez.flu
-00000500: 7828 4229 7a07 666c 7578 2856 297a 0766  x(B)z.flux(V)z.f
-00000510: 6c75 7828 5229 7a07 666c 7578 284a 297a  lux(R)z.flux(J)z
-00000520: 0766 6c75 7828 4829 7a07 666c 7578 284b  .flux(H)z.flux(K
-00000530: 29da 056f 7479 7065 6305 0000 0000 0000  )..otypec.......
-00000540: 0000 0000 0006 0000 0006 0000 0043 0000  .............C..
-00000550: 0073 3600 0000 7400 a001 7c00 a101 7d05  .s6...t...|...}.
-00000560: 7400 6a02 7c05 7c05 6401 6b01 3c00 6402  t.j.|.|.d.k.<.d.
-00000570: 7400 a003 7c05 7c01 1800 7c03 7c02 1400  t...|.|...|.|...
-00000580: 1b00 a101 1400 7c04 1700 5300 2903 4e72  ......|...S.).Nr
-00000590: 0100 0000 e700 0000 0000 0004 c029 04da  .............)..
-000005a0: 026e 70da 0463 6f70 79da 036e 616e da05  .np..copy..nan..
-000005b0: 6c6f 6731 3029 06da 066e 616d 6569 6eda  log10)...namein.
-000005c0: 0c6d 6564 6961 6e5f 736b 795f 76da 0461  .median_sky_v..a
-000005d0: 7265 61da 0174 da02 7a70 da03 696d 61a9  rea..t..zp..ima.
-000005e0: 0072 2f00 0000 fa4c 2f68 6f6d 652f 6a6f  .r/....L/home/jo
-000005f0: 7365 6168 6572 2f44 726f 7062 6f78 2f77  seaher/Dropbox/w
-00000600: 6f72 6b2f 7072 6f67 2f70 6163 6b61 6765  ork/prog/package
-00000610: 735f 6173 7472 6f6d 6f72 7068 6c69 622f  s_astromorphlib/
-00000620: 7374 6174 5f6c 6962 2f5f 5f69 6e69 745f  stat_lib/__init_
-00000630: 5f2e 7079 da0a 696d 615f 666c 326d 6167  _.py..ima_fl2mag
-00000640: 4800 0000 7306 0000 0000 020a 010e 0172  H...s..........r
-00000650: 3100 0000 6302 0000 0000 0000 0000 0000  1...c...........
-00000660: 0002 0000 0005 0000 0043 0000 0073 1a00  .........C...s..
-00000670: 0000 6401 7c01 7c00 1b00 1400 6402 7400  ..d.|.|.....d.t.
-00000680: a001 6403 a101 1b00 1400 5300 2904 4e67  ..d.......S.).Ng
-00000690: 0000 0000 0000 0440 e700 0000 0000 00f0  .......@........
-000006a0: 3f67 0000 0000 0000 2440 2902 7225 0000  ?g......$@).r%..
-000006b0: 00da 036c 6f67 2902 da01 49da 0549 5f65  ...log)...I..I_e
-000006c0: 7272 722f 0000 0072 2f00 0000 7230 0000  rrr/...r/...r0..
-000006d0: 00da 0b63 616c 5f65 7272 5f6d 6167 4e00  ...cal_err_magN.
-000006e0: 0000 7302 0000 0000 0172 3600 0000 e932  ..s......r6....2
-000006f0: 0000 00e7 0000 0000 0000 0040 e902 0000  ...........@....
-00000700: 00e9 6400 0000 da03 6f66 66da 0152 e905  ..d.....off..R..
-00000710: 0000 00e9 0b00 0000 fa0e 7072 6f70 6572  ..........proper
-00000720: 7469 6573 2e64 6174 679a 9999 9999 99c9  ties.datg.......
-00000730: 3fda 0379 6573 6311 0000 0000 0000 0000  ?..yesc.........
-00000740: 0000 004b 0000 0012 0000 0043 0000 0073  ...K.......C...s
-00000750: b60c 0000 7400 a001 7c01 6401 1900 7c00  ....t...|.d...|.
-00000760: 6b02 a101 6402 1900 6402 1900 7d11 7c01  k...d...d...}.|.
-00000770: 6403 1900 7c11 1900 7402 1b00 7d12 7400  d...|...t...}.t.
-00000780: a003 7400 a004 6404 a101 a101 7c12 1400  ..t...d.....|...
-00000790: 6405 1400 7d13 7405 7406 6a07 6406 1700  d...}.t.t.j.d...
-000007a0: 8301 0100 7405 7406 6a07 6407 1700 8301  ....t.t.j.d.....
-000007b0: 0100 7405 7406 6a07 6408 a008 7c13 a101  ..t.t.j.d...|...
-000007c0: 1700 8301 0100 7c03 7c13 1b00 6409 1b00  ......|.|...d...
-000007d0: 640a 1400 7d14 7c14 640b 1400 6409 1400  d...}.|.d...d...
-000007e0: 640c 1b00 7d15 7405 7406 6a07 640d a008  d...}.t.t.j.d...
-000007f0: 7c14 a101 1700 8301 0100 7400 a009 7c05  |.........t...|.
-00000800: a101 7400 6a0a 1400 7c13 640a 1300 1b00  ..t.j...|.d.....
-00000810: 640e 1b00 7d16 7405 7406 6a07 640f a008  d...}.t.t.j.d...
-00000820: 7c05 7c16 a102 1700 8301 0100 7c02 a00b  |.|.........|...
-00000830: 7c01 6410 1900 7c11 1900 7c01 6411 1900  |.d...|...|.d...
-00000840: 7c11 1900 a102 7d17 7400 6a0c a00d 7c17  |.....}.t.j...|.
-00000850: 6412 1900 6413 a102 9001 7244 7405 7406  d...d.....rDt.t.
-00000860: 6a0e 6414 1700 8301 0100 7405 7406 6a0e  j.d.......t.t.j.
-00000870: 6415 1700 8301 0100 7405 7406 6a0e 6416  d.......t.t.j.d.
-00000880: 1700 8301 0100 7405 7406 6a0e 6417 1700  ......t.t.j.d...
-00000890: 8301 0100 6400 5300 7400 a00f 7c14 a101  ....d.S.t...|...
-000008a0: 9001 727e 7405 7406 6a0e 6414 1700 8301  ..r~t.t.j.d.....
-000008b0: 0100 7405 7406 6a0e 6418 1700 8301 0100  ..t.t.j.d.......
-000008c0: 7405 7406 6a0e 6419 1700 8301 0100 6400  t.t.j.d.......d.
-000008d0: 5300 7405 7406 6a0e 641a 1700 8301 0100  S.t.t.j.d.......
-000008e0: 7405 641b 8301 0100 641c a008 7c00 7c03  t.d.....d...|.|.
-000008f0: a102 7d18 641d a008 7c00 7c0a 7c03 a103  ..}.d...|.|.|...
-00000900: 7d19 7410 6a11 a012 7c18 a101 9001 73d4  }.t.j...|.....s.
-00000910: 7410 6a11 a012 7c19 a101 9001 72e4 7c0a  t.j...|.....r.|.
-00000920: 641e 6b02 9001 72e4 7405 641f 7c18 9b00  d.k...r.t.d.|...
-00000930: 6420 9d03 8301 0100 7410 6a11 a012 7c18  d ......t.j...|.
-00000940: a101 9002 734a 7410 6a11 a012 7c19 a101  ....sJt.j...|...
-00000950: 9002 734a 7c0a 641e 6b02 9002 724a 7405  ..sJ|.d.k...rJt.
-00000960: 6421 7c18 9b00 6422 9d03 8301 0100 7c02  d!|...d"......|.
-00000970: 6a13 7c01 6410 1900 7c11 1900 7c01 6411  j.|.d...|...|.d.
-00000980: 1900 7c11 1900 7414 7c14 8301 7c0a 7c19  ..|...t.|...|.|.
-00000990: 6402 6423 8502 1900 6424 8d05 0100 7410  d.d#....d$....t.
-000009a0: 6a11 a012 7c19 a101 9002 7268 7405 641f  j...|.....rht.d.
-000009b0: 7c19 9b00 6420 9d03 8301 0100 7410 6a11  |...d ......t.j.
-000009c0: a012 7c19 a101 9002 73c0 7c0a 641e 6b03  ..|.....s.|.d.k.
-000009d0: 9002 72c0 7405 6421 7c19 9b00 6422 9d03  ..r.t.d!|...d"..
-000009e0: 8301 0100 7c02 6a13 7c01 6410 1900 7c11  ....|.j.|.d...|.
-000009f0: 1900 7c01 6411 1900 7c11 1900 7414 7c14  ..|.d...|...t.|.
-00000a00: 8301 7c0a 7c19 6402 6423 8502 1900 6424  ..|.|.d.d#....d$
-00000a10: 8d05 0100 7c17 6412 1900 7d1a 7405 6425  ....|.d...}.t.d%
-00000a20: 8301 0100 7405 7406 6a07 6426 a008 7c1a  ....t.t.j.d&..|.
-00000a30: a101 1700 8301 0100 7405 6425 8301 0100  ........t.d%....
-00000a40: 6427 7c00 9b00 6428 9d03 7d18 6429 a008  d'|...d(..}.d)..
-00000a50: 7c00 6400 642a 8502 1900 a101 7d19 6429  |.d.d*......}.d)
-00000a60: a008 7c1a a101 7d1b 7410 6a11 a012 7c18  ..|...}.t.j...|.
-00000a70: a101 9003 733e 7410 6a11 a012 7c19 a101  ....s>t.j...|...
-00000a80: 9003 733e 7410 6a11 a012 7c1b a101 9003  ..s>t.j...|.....
-00000a90: 72c4 7410 6a11 a012 7c18 a101 9003 726a  r.t.j...|.....rj
-00000aa0: 7415 6a16 7c18 642b 642c 8d02 7d1c 7405  t.j.|.d+d,..}.t.
-00000ab0: 642d 7c18 9b00 6420 9d03 8301 0100 7410  d-|...d ......t.
-00000ac0: 6a11 a012 7c19 a101 9003 7296 7415 6a16  j...|.....r.t.j.
-00000ad0: 7c19 642b 642c 8d02 7d1c 7405 642d 7c19  |.d+d,..}.t.d-|.
-00000ae0: 9b00 6420 9d03 8301 0100 7410 6a11 a012  ..d ......t.j...
-00000af0: 7c1b a101 9004 7202 7415 6a16 7c1b 642b  |.....r.t.j.|.d+
-00000b00: 642c 8d02 7d1c 7405 642d 7c1b 9b00 6420  d,..}.t.d-|...d 
-00000b10: 9d03 8301 0100 6e3e 642e 7417 7c1a 8301  ......n>d.t.|...
-00000b20: 1700 642f 1700 6430 1700 7d1d 7405 6431  ..d/..d0..}.t.d1
-00000b30: 7c1d 8302 0100 7c02 a018 7c1d a101 7d1c  |.....|...|...}.
-00000b40: 7c1c 6a19 6427 7c1a 9b00 6428 9d03 642b  |.j.d'|...d(..d+
-00000b50: 642c 8d02 0100 7405 7406 6a1a 6432 1700  d,....t.t.j.d2..
-00000b60: 8301 0100 7405 6433 8301 0100 7410 6a11  ....t.d3....t.j.
-00000b70: a01b 7410 6a11 a01c 741d a101 a101 7d1e  ..t.j...t.....}.
-00000b80: 7415 a016 7c1e 6434 1700 a101 7d1f 7400  t...|.d4....}.t.
-00000b90: a001 7c1f 6412 1900 7c1c 6435 1900 6402  ..|.d...|.d5..d.
-00000ba0: 1900 6b02 a101 6402 1900 6402 1900 7d20  ..k...d...d...} 
-00000bb0: 7c1f 7c0a 1900 7c20 1900 7d21 7405 6436  |.|...| ..}!t.d6
-00000bc0: 7c20 6437 a008 7c21 a101 6438 7c17 6412  | d7..|!..d8|.d.
-00000bd0: 1900 8305 0100 7400 a01e 7400 a01f 7c1c  ......t...t...|.
-00000be0: 6439 1900 a101 643a a102 7d22 7405 643b  d9....d:..}"t.d;
-00000bf0: a008 7420 7c1c 6439 1900 8301 a101 8301  ..t |.d9........
-00000c00: 0100 7405 643c a008 7c22 a101 8301 0100  ..t.d<..|"......
-00000c10: 6409 7d23 643a 7d24 643d 7d25 7400 a009  d.}#d:}$d=}%t...
-00000c20: 7c23 a101 7d26 643a 7d27 7c01 6401 1900  |#..}&d:}'|.d...
-00000c30: 7c11 1900 643e a008 7c0a 7c03 a102 1700  |...d>..|.|.....
-00000c40: 7d28 7c0a 641e 6b02 9005 7274 7a4a 7421  }(|.d.k...rtzJt!
-00000c50: a022 643f 7c01 6401 1900 7c11 1900 1700  ."d?|.d...|.....
-00000c60: 6440 a008 7c03 a101 1700 a101 7d29 7405  d@..|.......})t.
-00000c70: 7406 6a0e 6441 a008 7c01 6401 1900 7c11  t.j.dA..|.d...|.
-00000c80: 1900 6440 a008 7c03 a101 1700 a101 1700  ..d@..|.........
-00000c90: 8301 0100 5700 6e2e 0100 0100 0100 7421  ....W.n.......t!
-00000ca0: a022 643f 7c28 1700 a101 7d29 7405 7406  ."d?|(....})t.t.
-00000cb0: 6a0e 6441 a008 7c28 a101 1700 8301 0100  j.dA..|(........
-00000cc0: 5900 6e02 5800 6e22 7421 a022 643f 7c28  Y.n.X.n"t!."d?|(
-00000cd0: 1700 a101 7d29 7405 7406 6a0e 6441 a008  ....})t.t.j.dA..
-00000ce0: 7c28 a101 1700 8301 0100 7c29 643a 1900  |(........|)d:..
-00000cf0: 6a23 7d2a 7405 7406 6a07 6442 1700 8301  j#}*t.t.j.dB....
-00000d00: 0100 7405 6443 8301 0100 7405 6444 8301  ..t.dC....t.dD..
-00000d10: 0100 7424 7c2a 7c0b 7c0c 7c0d 6445 8d04  ..t$|*|.|.|.dE..
-00000d20: 7d2b 7425 6a26 6446 6447 8d01 7d2c 7425  }+t%j&dFdG..},t%
-00000d30: 6a27 7c2b 6448 6449 8d02 0100 7425 6a28  j'|+dHdI....t%j(
-00000d40: 644a 7c00 1700 644b a008 7c03 a101 1700  dJ|...dK..|.....
-00000d50: 644c 644d 8d02 0100 7c10 644e 6b02 9006  dLdM....|.dNk...
-00000d60: 7218 7425 a029 a100 0100 6e08 7425 a02a  r.t%.)....n.t%.*
-00000d70: a100 0100 742b 7c2a 644f 7c2b 6450 8d03  ....t+|*dO|+dP..
-00000d80: 5c03 7d2d 7d2e 7d2f 7405 7406 6a07 6451  \.}-}.}/t.t.j.dQ
-00000d90: 1700 8301 0100 7405 6452 8301 0100 7405  ......t.dR....t.
-00000da0: 6453 a008 7c2d a101 8301 0100 7405 6454  dS..|-......t.dT
-00000db0: a008 7c2e a101 8301 0100 7405 6455 a008  ..|.......t.dU..
-00000dc0: 7c2f a101 8301 0100 7405 6456 a008 7c08  |/......t.dV..|.
-00000dd0: 6402 1900 7c08 643a 1900 a102 8301 0100  d...|.d:........
-00000de0: 7405 6457 8301 0100 742c 8300 7d30 742d  t.dW....t,..}0t-
-00000df0: 7c2a 7c08 6458 7c30 7c2b 7c2e 6459 8d06  |*|.dX|0|+|.dY..
-00000e00: 7d31 7c2a 7c31 6a2e 1800 7d2a 7425 6a26  }1|*|1j...}*t%j&
-00000e10: 6446 6447 8d01 7d2c 7425 6a27 7c31 6a2e  dFdG..},t%j'|1j.
-00000e20: 6448 6449 8d02 0100 7425 6a28 644a 7c00  dHdI....t%j(dJ|.
-00000e30: 1700 645a a008 7c03 a101 1700 644c 644d  ..dZ..|.....dLdM
-00000e40: 8d02 0100 7c10 644e 6b02 9007 7204 7425  ....|.dNk...r.t%
-00000e50: a029 a100 0100 6e08 7425 a02a a100 0100  .)....n.t%.*....
-00000e60: 7c01 6401 1900 7c11 1900 645b a008 7c03  |.d...|...d[..|.
-00000e70: a101 1700 7d32 7421 6a2f 643f 7c32 1700  ....}2t!j/d?|2..
-00000e80: 645c 1700 7c31 6a2e 645d 645e 8d03 0100  d\..|1j.d]d^....
-00000e90: 7421 6a2f 643f 7c32 1700 645f 1700 7c2a  t!j/d?|2..d_..|*
-00000ea0: 645d 645e 8d03 0100 7405 6460 7c32 1700  d]d^....t.d`|2..
-00000eb0: 6461 1700 8301 0100 7430 7c2a 7c25 7c26  da......t0|*|%|&
-00000ec0: 7c27 7c21 8305 7d33 7400 a031 7400 a032  |'|!..}3t..1t..2
-00000ed0: 640a a101 640a 1400 a101 640a 1400 7d34  d...d.....d...}4
-00000ee0: 6462 7d35 7c22 7c34 1b00 7d36 7400 6a33  db}5|"|4..}6t.j3
-00000ef0: 7c35 0b00 7c35 643a 1700 8502 7c35 0b00  |5..|5d:....|5..
-00000f00: 7c35 643a 1700 8502 6602 1900 5c02 7d37  |5d:....f...\.}7
-00000f10: 7d38 7400 a034 7c38 640a 1300 7c37 640a  }8t..4|8d...|7d.
-00000f20: 1300 1700 0b00 6463 7c36 640a 1300 1400  ......dc|6d.....
-00000f30: 1b00 a101 7d39 7c39 7400 a035 7c39 a101  ....}9|9t..5|9..
-00000f40: 1d00 7d39 7c22 7436 1400 7d3a 7437 7c3a  ..}9|"t6..}:t7|:
-00000f50: 6464 6464 6465 8d03 7d3b 7c3b a038 a100  ddddde..};|;.8..
-00000f60: 0100 7414 7c16 8301 7d3c 7439 6a3a 7c2a  ..t.|...}<t9j:|*
-00000f70: 7c04 6466 8d02 7d3d 7439 a03b 7c2a 7c3d  |.df..}=t9.;|*|=
-00000f80: 7c3c a103 7d3e 7c09 6467 6b02 9008 729c  |<..}>|.dgk...r.
-00000f90: 7405 6468 8301 0100 7405 6469 8301 0100  t.dh....t.di....
-00000fa0: 7405 646a 8301 0100 7425 6a26 6446 6447  t.dj....t%j&dFdG
-00000fb0: 8d01 0100 7425 6a27 7c3e 6448 6449 8d02  ....t%j'|>dHdI..
-00000fc0: 0100 7c10 644e 6b02 9008 7282 7425 a029  ..|.dNk...r.t%.)
-00000fd0: a100 0100 6e08 7425 a02a a100 0100 743c  ....n.t%.*....t<
-00000fe0: 7c2a 7c3e 7c3c 646b 646c 646d 8d05 7d3e  |*|>|<dkdldm..}>
-00000ff0: 7405 646e 8301 0100 7405 646f 8301 0100  t.dn....t.do....
-00001000: 7425 6a26 6446 6447 8d01 0100 7425 6a27  t%j&dFdG....t%j'
-00001010: 7c3e 6448 6470 6471 8d03 0100 644a 7c01  |>dHdpdq....dJ|.
-00001020: 6401 1900 7c11 1900 1700 6472 a008 7c03  d...|.....dr..|.
-00001030: a101 1700 7d3f 7425 6a28 7c3f 644c 644d  ....}?t%j(|?dLdM
-00001040: 8d02 0100 7c10 644e 6b02 9009 7204 7425  ....|.dNk...r.t%
-00001050: a029 a100 0100 6e08 7425 a02a a100 0100  .)....n.t%.*....
-00001060: 7405 7406 6a0e 6473 1700 8301 0100 7405  t.t.j.ds......t.
-00001070: 6474 8301 0100 743d a03d a100 7d40 743e  dt....t=.=..}@t>
-00001080: 6a3f 7c2a 7c3e 6a23 7c24 7c39 7c0f 6475  j?|*|>j#|$|9|.du
-00001090: 8d05 7d41 7405 6476 743d a03d a100 7c40  ..}At.dvt=.=..|@
-000010a0: 1800 1600 8301 0100 7405 7420 7c41 8301  ........t.t |A..
-000010b0: 8301 0100 6477 6478 6479 647a 647b 647c  ....dwdxdydzd{d|
-000010c0: 647d 647e 647f 6480 6481 6482 6483 6484  d}d~d.d.d.d.d.d.
-000010d0: 670e 7d42 7405 6485 8301 0100 7405 6486  g.}Bt.d.....t.d.
-000010e0: 8301 0100 7c00 6402 640a 8502 1900 6487  ....|.d.d.....d.
-000010f0: 6b02 9009 72bc 7c00 642a 1900 a040 a100  k...r.|.d*...@..
-00001100: 9009 72bc 7c00 6400 642a 8502 1900 7d00  ..r.|.d.d*....}.
-00001110: 7c06 6400 6b08 900b 722a 7400 a041 7c3e  |.d.k...r*t..A|>
-00001120: 6a42 a101 7d43 7443 7c43 6400 6400 642a  jB..}CtC|Cd.d.d*
-00001130: 8503 1900 8301 4400 9001 5d3e 5c02 7d44  ......D...]>\.}D
-00001140: 7d45 7c41 7c45 1900 7d46 7444 7c46 7c00  }E|A|E..}FtD|F|.
-00001150: 7c42 7c44 1900 1700 7c2a 7c33 7c25 7c26  |B|D....|*|3|%|&
-00001160: 7c27 7c21 7c39 7c22 7c23 7c13 7c03 7c0e  |'|!|9|"|#|.|.|.
-00001170: 7c10 6488 8d0f 0100 7445 a016 7c0e a101  |.d.....tE..|...
-00001180: 7d47 7400 a001 7c47 6489 1900 7c00 7c42  }Gt...|Gd...|.|B
-00001190: 7c44 1900 1700 6b02 a101 6402 1900 6402  |D....k...d...d.
-000011a0: 1900 7d48 7400 a001 7c01 6401 1900 7c00  ..}Ht...|.d...|.
-000011b0: 6b02 a101 6402 1900 6402 1900 7d49 7c01  k...d...d...}I|.
-000011c0: 6410 1900 7c49 1900 7c47 6410 1900 7c48  d...|I..|Gd...|H
-000011d0: 3c00 7c01 6411 1900 7c49 1900 7c47 6411  <.|.d...|I..|Gd.
-000011e0: 1900 7c48 3c00 7c01 6403 1900 7c49 1900  ..|H<.|.d...|I..
-000011f0: 7c47 648a 1900 7c48 3c00 7a18 7c01 648b  |Gd...|H<.z.|.d.
-00001200: 1900 7c49 1900 7c47 648c 1900 7c48 3c00  ..|I..|Gd...|H<.
-00001210: 5700 6e24 0100 0100 0100 7c01 6403 1900  W.n$......|.d...
-00001220: 7c49 1900 7446 1b00 7c47 648c 1900 7c48  |I..tF..|Gd...|H
-00001230: 3c00 5900 6e02 5800 7a18 7c01 648d 1900  <.Y.n.X.z.|.d...
-00001240: 7c49 1900 7c47 648d 1900 7c48 3c00 5700  |I..|Gd...|H<.W.
-00001250: 6e14 0100 0100 0100 7405 648e 8301 0100  n.......t.d.....
-00001260: 5900 6e02 5800 7445 6a19 7c47 7c0e 645d  Y.n.X.tEj.|G|.d]
-00001270: 645e 8d03 0100 9009 71e4 9001 6e4a 7443  d^......q...nJtC
-00001280: 7c06 8301 4400 9001 5d3e 5c02 7d44 7d45  |...D...]>\.}D}E
-00001290: 7c41 7c45 1900 7d46 7444 7c46 7c00 7c07  |A|E..}FtD|F|.|.
-000012a0: 7c44 1900 1700 7c2a 7c33 7c25 7c26 7c27  |D....|*|3|%|&|'
-000012b0: 7c21 7c39 7c22 7c23 7c13 7c03 7c0e 7c10  |!|9|"|#|.|.|.|.
-000012c0: 6488 8d0f 0100 7445 a016 7c0e a101 7d47  d.....tE..|...}G
-000012d0: 7400 a001 7c47 6489 1900 7c00 7c07 7c44  t...|Gd...|.|.|D
-000012e0: 1900 1700 6b02 a101 6402 1900 6402 1900  ....k...d...d...
-000012f0: 7d48 7400 a001 7c01 6401 1900 7c00 6b02  }Ht...|.d...|.k.
-00001300: a101 6402 1900 6402 1900 7d49 7c01 6410  ..d...d...}I|.d.
-00001310: 1900 7c49 1900 7c47 6410 1900 7c48 3c00  ..|I..|Gd...|H<.
-00001320: 7c01 6411 1900 7c49 1900 7c47 6411 1900  |.d...|I..|Gd...
-00001330: 7c48 3c00 7c01 6403 1900 7c49 1900 7c47  |H<.|.d...|I..|G
-00001340: 648a 1900 7c48 3c00 7a18 7c01 648b 1900  d...|H<.z.|.d...
-00001350: 7c49 1900 7c47 648c 1900 7c48 3c00 5700  |I..|Gd...|H<.W.
-00001360: 6e24 0100 0100 0100 7c01 6403 1900 7c49  n$......|.d...|I
-00001370: 1900 7446 1b00 7c47 648c 1900 7c48 3c00  ..tF..|Gd...|H<.
-00001380: 5900 6e02 5800 7a18 7c01 648d 1900 7c49  Y.n.X.z.|.d...|I
-00001390: 1900 7c47 648d 1900 7c48 3c00 5700 6e14  ..|Gd...|H<.W.n.
-000013a0: 0100 0100 0100 7405 648e 8301 0100 5900  ......t.d.....Y.
-000013b0: 6e02 5800 7445 6a19 7c47 7c0e 645d 645e  n.X.tEj.|G|.d]d^
-000013c0: 8d03 0100 900b 7132 7425 a029 a100 0100  ......q2t%.)....
-000013d0: 6700 7d4a 7c07 4400 5d14 7d44 7c4a a047  g.}J|.D.].}D|J.G
-000013e0: 7c00 7c44 1700 a101 0100 900c 7184 7405  |.|D........q.t.
-000013f0: 648f a008 7c00 7c06 7c4a 7420 7c06 8301  d...|.|.|Jt |...
-00001400: a104 8301 0100 6400 5300 2990 4eda 0367  ......d.S.).N..g
-00001410: 616c 7201 0000 00da 0376 656c e7df bc9a  alr......vel....
-00001420: 7856 3432 3fe7 0000 0000 0040 8f40 fa13  xV42?......@.@..
-00001430: 0a42 6173 6963 2069 6e66 6f72 6d61 7469  .Basic informati
-00001440: 6f6e 3afa 132d 2d2d 2d2d 2d2d 2d2d 2d2d  on:..-----------
-00001450: 2d2d 2d2d 2d2d 2d2d fa0e 6172 635f 6b70  --------..arc_kp
-00001460: 6320 7b3a 2e34 667d e79a 9999 9999 99e1  c {:.4f}........
-00001470: 3f72 3900 0000 e700 0000 0000 00e0 3fe7  ?r9...........?.
-00001480: 0000 0000 0020 ac40 fa19 696d 6167 6520  ..... .@..image 
-00001490: 7369 7a65 2069 6e20 7069 783a 207b 3a2e  size in pix: {:.
-000014a0: 3166 7de7 5d8f c2f5 285c d33f fa30 4d69  1f}.]...(\.?.0Mi
-000014b0: 6e69 6d75 6d20 6465 7465 6374 696f 6e20  nimum detection 
-000014c0: 6172 6561 207b 3a2e 3166 7d20 6b63 705e  area {:.1f} kcp^
-000014d0: 3220 3d20 7b3a 2e30 667d 2070 6978 da02  2 = {:.0f} pix..
-000014e0: 7261 da03 6465 63da 0566 6965 6c64 da02  ra..dec..field..
-000014f0: 4d43 fa33 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  MC.3.===========
+00000290: 6442 6438 6430 6434 6435 6436 660d 6452  dBd8d0d4d5d6f.dR
+000002a0: 6453 8401 5a4d 642e 642f 6430 6451 6401  dS..ZMd.d/d0dQd.
+000002b0: 6401 6431 6431 6702 6432 6438 6430 6434  d.d1d1g.d2d8d0d4
+000002c0: 6435 6436 6437 660e 6454 6455 8401 5a4e  d5d6d7f.dTdU..ZN
+000002d0: 645e 6457 6458 8401 5a4f 6401 5300 295f  d^dWdX..ZOd.S.)_
+000002e0: e900 0000 004e 2901 da0b 6d61 6b65 5f66  .....N)...make_f
+000002f0: 6967 7572 6529 02da 0466 6974 73da 0561  igure)...fits..a
+00000300: 7363 6969 2901 da05 5461 626c 6529 01da  scii)...Table)..
+00000310: 0673 696d 6261 6429 01da 034e 6564 2901  .simbad)...Ned).
+00000320: da03 7763 7329 01da 0853 6b79 436f 6f72  ..wcs)...SkyCoor
+00000330: 6429 01da 106d 616b 655f 736f 7572 6365  d)...make_source
+00000340: 5f6d 6173 6b29 01da 1373 6967 6d61 5f63  _mask)...sigma_c
+00000350: 6c69 7070 6564 5f73 7461 7473 2902 da0c  lipped_stats)...
+00000360: 4261 636b 6772 6f75 6e64 3244 da10 4d65  Background2D..Me
+00000370: 6469 616e 4261 636b 6772 6f75 6e64 2901  dianBackground).
+00000380: da0e 6465 7465 6374 5f73 6f75 7263 6573  ..detect_sources
+00000390: 2901 da0f 6465 626c 656e 645f 736f 7572  )...deblend_sour
+000003a0: 6365 7329 01da 1047 6175 7373 6961 6e32  ces)...Gaussian2
+000003b0: 444b 6572 6e65 6c29 01da 1667 6175 7373  DKernel)...gauss
+000003c0: 6961 6e5f 6677 686d 5f74 6f5f 7369 676d  ian_fwhm_to_sigm
+000003d0: 6129 01da 0571 756f 7465 2901 da0b 7572  a)...quote)...ur
+000003e0: 6c72 6574 7269 6576 6529 05da 0e4d 696e  lretrieve)...Min
+000003f0: 4d61 7849 6e74 6572 7661 6cda 0b53 7172  MaxInterval..Sqr
+00000400: 7453 7472 6574 6368 da0c 4173 696e 6853  tStretch..AsinhS
+00000410: 7472 6574 6368 da0e 496d 6167 654e 6f72  tretch..ImageNor
+00000420: 6d61 6c69 7a65 da0f 6d61 6b65 5f6c 7570  malize..make_lup
+00000430: 746f 6e5f 7267 6229 01da 0446 6f72 6529  ton_rgb)...Fore)
+00000440: 01da 0772 6571 7565 7374 6700 0000 0000  ...requestg.....
+00000450: 8051 4067 0000 0000 804f 1241 da07 7465  .Q@g.....O.A..te
+00000460: 7272 6169 6e7a 1b68 7474 703a 2f2f 7369  rrainz.http://si
+00000470: 6d62 6164 2e75 2d73 7472 6173 6267 2e66  mbad.u-strasbg.f
+00000480: 722f 7a1a 6874 7470 3a2f 2f73 696d 6261  r/z.http://simba
+00000490: 642e 6861 7276 6172 642e 6564 752f da0b  d.harvard.edu/..
+000004a0: 636f 6f72 6469 6e61 7465 737a 0572 6128  coordinatesz.ra(
+000004b0: 6429 7a06 6465 6328 6429 da08 7276 5f76  d)z.dec(d)..rv_v
+000004c0: 616c 7565 da07 7a5f 7661 6c75 65da 096d  alue..z_value..m
+000004d0: 6f72 7068 7479 7065 da0b 6469 6d5f 6d61  orphtype..dim_ma
+000004e0: 6a61 7869 73da 0b64 696d 5f6d 696e 6178  jaxis..dim_minax
+000004f0: 6973 da09 6469 6d5f 616e 676c 657a 0766  is..dim_anglez.f
+00000500: 6c75 7828 4229 7a07 666c 7578 2856 297a  lux(B)z.flux(V)z
+00000510: 0766 6c75 7828 5229 7a07 666c 7578 284a  .flux(R)z.flux(J
+00000520: 297a 0766 6c75 7828 4829 7a07 666c 7578  )z.flux(H)z.flux
+00000530: 284b 29da 056f 7479 7065 6305 0000 0000  (K)..otypec.....
+00000540: 0000 0000 0000 0006 0000 0006 0000 0043  ...............C
+00000550: 0000 0073 3600 0000 7400 a001 7c00 a101  ...s6...t...|...
+00000560: 7d05 7400 6a02 7c05 7c05 6401 6b01 3c00  }.t.j.|.|.d.k.<.
+00000570: 6402 7400 a003 7c05 7c01 1800 7c03 7c02  d.t...|.|...|.|.
+00000580: 1400 1b00 a101 1400 7c04 1700 5300 2903  ........|...S.).
+00000590: 4e72 0100 0000 e700 0000 0000 0004 c029  Nr.............)
+000005a0: 04da 026e 70da 0463 6f70 79da 036e 616e  ...np..copy..nan
+000005b0: da05 6c6f 6731 3029 06da 066e 616d 6569  ..log10)...namei
+000005c0: 6eda 0c6d 6564 6961 6e5f 736b 795f 76da  n..median_sky_v.
+000005d0: 0461 7265 61da 0174 da02 7a70 da03 696d  .area..t..zp..im
+000005e0: 61a9 0072 2f00 0000 fa4c 2f68 6f6d 652f  a..r/....L/home/
+000005f0: 6a6f 7365 6168 6572 2f44 726f 7062 6f78  joseaher/Dropbox
+00000600: 2f77 6f72 6b2f 7072 6f67 2f70 6163 6b61  /work/prog/packa
+00000610: 6765 735f 6173 7472 6f6d 6f72 7068 6c69  ges_astromorphli
+00000620: 622f 7374 6174 5f6c 6962 2f5f 5f69 6e69  b/stat_lib/__ini
+00000630: 745f 5f2e 7079 da0a 696d 615f 666c 326d  t__.py..ima_fl2m
+00000640: 6167 4800 0000 7306 0000 0000 020a 010e  agH...s.........
+00000650: 0172 3100 0000 6302 0000 0000 0000 0000  .r1...c.........
+00000660: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00000670: 1a00 0000 6401 7c01 7c00 1b00 1400 6402  ....d.|.|.....d.
+00000680: 7400 a001 6403 a101 1b00 1400 5300 2904  t...d.......S.).
+00000690: 4e67 0000 0000 0000 0440 e700 0000 0000  Ng.......@......
+000006a0: 00f0 3f67 0000 0000 0000 2440 2902 7225  ..?g......$@).r%
+000006b0: 0000 00da 036c 6f67 2902 da01 49da 0549  .....log)...I..I
+000006c0: 5f65 7272 722f 0000 0072 2f00 0000 7230  _errr/...r/...r0
+000006d0: 0000 00da 0b63 616c 5f65 7272 5f6d 6167  .....cal_err_mag
+000006e0: 4e00 0000 7302 0000 0000 0172 3600 0000  N...s......r6...
+000006f0: e932 0000 00e7 0000 0000 0000 0040 e902  .2...........@..
+00000700: 0000 00e9 6400 0000 da03 6f66 66da 0152  ....d.....off..R
+00000710: e905 0000 00e9 0b00 0000 fa0e 7072 6f70  ............prop
+00000720: 6572 7469 6573 2e64 6174 679a 9999 9999  erties.datg.....
+00000730: 99c9 3fda 0379 6573 6311 0000 0000 0000  ..?..yesc.......
+00000740: 0000 0000 004b 0000 0012 0000 0043 0000  .....K.......C..
+00000750: 0073 b60c 0000 7400 a001 7c01 6401 1900  .s....t...|.d...
+00000760: 7c00 6b02 a101 6402 1900 6402 1900 7d11  |.k...d...d...}.
+00000770: 7c01 6403 1900 7c11 1900 7402 1b00 7d12  |.d...|...t...}.
+00000780: 7400 a003 7400 a004 6404 a101 a101 7c12  t...t...d.....|.
+00000790: 1400 6405 1400 7d13 7405 7406 6a07 6406  ..d...}.t.t.j.d.
+000007a0: 1700 8301 0100 7405 7406 6a07 6407 1700  ......t.t.j.d...
+000007b0: 8301 0100 7405 7406 6a07 6408 a008 7c13  ....t.t.j.d...|.
+000007c0: a101 1700 8301 0100 7c03 7c13 1b00 6409  ........|.|...d.
+000007d0: 1b00 640a 1400 7d14 7c14 640b 1400 6409  ..d...}.|.d...d.
+000007e0: 1400 640c 1b00 7d15 7405 7406 6a07 640d  ..d...}.t.t.j.d.
+000007f0: a008 7c14 a101 1700 8301 0100 7400 a009  ..|.........t...
+00000800: 7c05 a101 7400 6a0a 1400 7c13 640a 1300  |...t.j...|.d...
+00000810: 1b00 640e 1b00 7d16 7405 7406 6a07 640f  ..d...}.t.t.j.d.
+00000820: a008 7c05 7c16 a102 1700 8301 0100 7c02  ..|.|.........|.
+00000830: a00b 7c01 6410 1900 7c11 1900 7c01 6411  ..|.d...|...|.d.
+00000840: 1900 7c11 1900 a102 7d17 7400 6a0c a00d  ..|.....}.t.j...
+00000850: 7c17 6412 1900 6413 a102 9001 7244 7405  |.d...d.....rDt.
+00000860: 7406 6a0e 6414 1700 8301 0100 7405 7406  t.j.d.......t.t.
+00000870: 6a0e 6415 1700 8301 0100 7405 7406 6a0e  j.d.......t.t.j.
+00000880: 6416 1700 8301 0100 7405 7406 6a0e 6417  d.......t.t.j.d.
+00000890: 1700 8301 0100 6400 5300 7400 a00f 7c14  ......d.S.t...|.
+000008a0: a101 9001 727e 7405 7406 6a0e 6414 1700  ....r~t.t.j.d...
+000008b0: 8301 0100 7405 7406 6a0e 6418 1700 8301  ....t.t.j.d.....
+000008c0: 0100 7405 7406 6a0e 6419 1700 8301 0100  ..t.t.j.d.......
+000008d0: 6400 5300 7405 7406 6a0e 641a 1700 8301  d.S.t.t.j.d.....
+000008e0: 0100 7405 641b 8301 0100 641c a008 7c00  ..t.d.....d...|.
+000008f0: 7c03 a102 7d18 641d a008 7c00 7c0a 7c03  |...}.d...|.|.|.
+00000900: a103 7d19 7410 6a11 a012 7c18 a101 9001  ..}.t.j...|.....
+00000910: 73d4 7410 6a11 a012 7c19 a101 9001 72e4  s.t.j...|.....r.
+00000920: 7c0a 641e 6b02 9001 72e4 7405 641f 7c18  |.d.k...r.t.d.|.
+00000930: 9b00 6420 9d03 8301 0100 7410 6a11 a012  ..d ......t.j...
+00000940: 7c18 a101 9002 734a 7410 6a11 a012 7c19  |.....sJt.j...|.
+00000950: a101 9002 734a 7c0a 641e 6b02 9002 724a  ....sJ|.d.k...rJ
+00000960: 7405 6421 7c18 9b00 6422 9d03 8301 0100  t.d!|...d"......
+00000970: 7c02 6a13 7c01 6410 1900 7c11 1900 7c01  |.j.|.d...|...|.
+00000980: 6411 1900 7c11 1900 7414 7c14 8301 7c0a  d...|...t.|...|.
+00000990: 7c19 6402 6423 8502 1900 6424 8d05 0100  |.d.d#....d$....
+000009a0: 7410 6a11 a012 7c19 a101 9002 7268 7405  t.j...|.....rht.
+000009b0: 641f 7c19 9b00 6420 9d03 8301 0100 7410  d.|...d ......t.
+000009c0: 6a11 a012 7c19 a101 9002 73c0 7c0a 641e  j...|.....s.|.d.
+000009d0: 6b03 9002 72c0 7405 6421 7c19 9b00 6422  k...r.t.d!|...d"
+000009e0: 9d03 8301 0100 7c02 6a13 7c01 6410 1900  ......|.j.|.d...
+000009f0: 7c11 1900 7c01 6411 1900 7c11 1900 7414  |...|.d...|...t.
+00000a00: 7c14 8301 7c0a 7c19 6402 6423 8502 1900  |...|.|.d.d#....
+00000a10: 6424 8d05 0100 7c17 6412 1900 7d1a 7405  d$....|.d...}.t.
+00000a20: 6425 8301 0100 7405 7406 6a07 6426 a008  d%....t.t.j.d&..
+00000a30: 7c1a a101 1700 8301 0100 7405 6425 8301  |.........t.d%..
+00000a40: 0100 6427 7c00 9b00 6428 9d03 7d18 6429  ..d'|...d(..}.d)
+00000a50: a008 7c00 6400 642a 8502 1900 a101 7d19  ..|.d.d*......}.
+00000a60: 6429 a008 7c1a a101 7d1b 7410 6a11 a012  d)..|...}.t.j...
+00000a70: 7c18 a101 9003 733e 7410 6a11 a012 7c19  |.....s>t.j...|.
+00000a80: a101 9003 733e 7410 6a11 a012 7c1b a101  ....s>t.j...|...
+00000a90: 9003 72c4 7410 6a11 a012 7c18 a101 9003  ..r.t.j...|.....
+00000aa0: 726a 7415 6a16 7c18 642b 642c 8d02 7d1c  rjt.j.|.d+d,..}.
+00000ab0: 7405 642d 7c18 9b00 6420 9d03 8301 0100  t.d-|...d ......
+00000ac0: 7410 6a11 a012 7c19 a101 9003 7296 7415  t.j...|.....r.t.
+00000ad0: 6a16 7c19 642b 642c 8d02 7d1c 7405 642d  j.|.d+d,..}.t.d-
+00000ae0: 7c19 9b00 6420 9d03 8301 0100 7410 6a11  |...d ......t.j.
+00000af0: a012 7c1b a101 9004 7202 7415 6a16 7c1b  ..|.....r.t.j.|.
+00000b00: 642b 642c 8d02 7d1c 7405 642d 7c1b 9b00  d+d,..}.t.d-|...
+00000b10: 6420 9d03 8301 0100 6e3e 642e 7417 7c1a  d ......n>d.t.|.
+00000b20: 8301 1700 642f 1700 6430 1700 7d1d 7405  ....d/..d0..}.t.
+00000b30: 6431 7c1d 8302 0100 7c02 a018 7c1d a101  d1|.....|...|...
+00000b40: 7d1c 7c1c 6a19 6427 7c1a 9b00 6428 9d03  }.|.j.d'|...d(..
+00000b50: 642b 642c 8d02 0100 7405 7406 6a1a 6432  d+d,....t.t.j.d2
+00000b60: 1700 8301 0100 7405 6433 8301 0100 7410  ......t.d3....t.
+00000b70: 6a11 a01b 7410 6a11 a01c 741d a101 a101  j...t.j...t.....
+00000b80: 7d1e 7415 a016 7c1e 6434 1700 a101 7d1f  }.t...|.d4....}.
+00000b90: 7400 a001 7c1f 6412 1900 7c1c 6435 1900  t...|.d...|.d5..
+00000ba0: 6402 1900 6b02 a101 6402 1900 6402 1900  d...k...d...d...
+00000bb0: 7d20 7c1f 7c0a 1900 7c20 1900 7d21 7405  } |.|...| ..}!t.
+00000bc0: 6436 7c20 6437 a008 7c21 a101 6438 7c17  d6| d7..|!..d8|.
+00000bd0: 6412 1900 8305 0100 7400 a01e 7400 a01f  d.......t...t...
+00000be0: 7c1c 6439 1900 a101 643a a102 7d22 7405  |.d9....d:..}"t.
+00000bf0: 643b a008 7420 7c1c 6439 1900 8301 a101  d;..t |.d9......
+00000c00: 8301 0100 7405 643c a008 7c22 a101 8301  ....t.d<..|"....
+00000c10: 0100 6409 7d23 643a 7d24 643d 7d25 7400  ..d.}#d:}$d=}%t.
+00000c20: a009 7c23 a101 7d26 643a 7d27 7c01 6401  ..|#..}&d:}'|.d.
+00000c30: 1900 7c11 1900 643e a008 7c0a 7c03 a102  ..|...d>..|.|...
+00000c40: 1700 7d28 7c0a 641e 6b02 9005 7274 7a4a  ..}(|.d.k...rtzJ
+00000c50: 7421 a022 643f 7c01 6401 1900 7c11 1900  t!."d?|.d...|...
+00000c60: 1700 6440 a008 7c03 a101 1700 a101 7d29  ..d@..|.......})
+00000c70: 7405 7406 6a0e 6441 a008 7c01 6401 1900  t.t.j.dA..|.d...
+00000c80: 7c11 1900 6440 a008 7c03 a101 1700 a101  |...d@..|.......
+00000c90: 1700 8301 0100 5700 6e2e 0100 0100 0100  ......W.n.......
+00000ca0: 7421 a022 643f 7c28 1700 a101 7d29 7405  t!."d?|(....})t.
+00000cb0: 7406 6a0e 6441 a008 7c28 a101 1700 8301  t.j.dA..|(......
+00000cc0: 0100 5900 6e02 5800 6e22 7421 a022 643f  ..Y.n.X.n"t!."d?
+00000cd0: 7c28 1700 a101 7d29 7405 7406 6a0e 6441  |(....})t.t.j.dA
+00000ce0: a008 7c28 a101 1700 8301 0100 7c29 643a  ..|(........|)d:
+00000cf0: 1900 6a23 7d2a 7405 7406 6a07 6442 1700  ..j#}*t.t.j.dB..
+00000d00: 8301 0100 7405 6443 8301 0100 7405 6444  ....t.dC....t.dD
+00000d10: 8301 0100 7424 7c2a 7c0b 7c0c 7c0d 6445  ....t$|*|.|.|.dE
+00000d20: 8d04 7d2b 7425 6a26 6446 6447 8d01 7d2c  ..}+t%j&dFdG..},
+00000d30: 7425 6a27 7c2b 6448 6449 8d02 0100 7425  t%j'|+dHdI....t%
+00000d40: 6a28 644a 7c00 1700 644b a008 7c03 a101  j(dJ|...dK..|...
+00000d50: 1700 644c 644d 8d02 0100 7c10 644e 6b02  ..dLdM....|.dNk.
+00000d60: 9006 7218 7425 a029 a100 0100 6e08 7425  ..r.t%.)....n.t%
+00000d70: a02a a100 0100 742b 7c2a 644f 7c2b 6450  .*....t+|*dO|+dP
+00000d80: 8d03 5c03 7d2d 7d2e 7d2f 7405 7406 6a07  ..\.}-}.}/t.t.j.
+00000d90: 6451 1700 8301 0100 7405 6452 8301 0100  dQ......t.dR....
+00000da0: 7405 6453 a008 7c2d a101 8301 0100 7405  t.dS..|-......t.
+00000db0: 6454 a008 7c2e a101 8301 0100 7405 6455  dT..|.......t.dU
+00000dc0: a008 7c2f a101 8301 0100 7405 6456 a008  ..|/......t.dV..
+00000dd0: 7c08 6402 1900 7c08 643a 1900 a102 8301  |.d...|.d:......
+00000de0: 0100 7405 6457 8301 0100 742c 8300 7d30  ..t.dW....t,..}0
+00000df0: 742d 7c2a 7c08 6458 7c30 7c2b 7c2e 6459  t-|*|.dX|0|+|.dY
+00000e00: 8d06 7d31 7c2a 7c31 6a2e 1800 7d2a 7425  ..}1|*|1j...}*t%
+00000e10: 6a26 6446 6447 8d01 7d2c 7425 6a27 7c31  j&dFdG..},t%j'|1
+00000e20: 6a2e 6448 6449 8d02 0100 7425 6a28 644a  j.dHdI....t%j(dJ
+00000e30: 7c00 1700 645a a008 7c03 a101 1700 644c  |...dZ..|.....dL
+00000e40: 644d 8d02 0100 7c10 644e 6b02 9007 7204  dM....|.dNk...r.
+00000e50: 7425 a029 a100 0100 6e08 7425 a02a a100  t%.)....n.t%.*..
+00000e60: 0100 7c01 6401 1900 7c11 1900 645b a008  ..|.d...|...d[..
+00000e70: 7c03 a101 1700 7d32 7421 6a2f 643f 7c32  |.....}2t!j/d?|2
+00000e80: 1700 645c 1700 7c31 6a2e 645d 645e 8d03  ..d\..|1j.d]d^..
+00000e90: 0100 7421 6a2f 643f 7c32 1700 645f 1700  ..t!j/d?|2..d_..
+00000ea0: 7c2a 645d 645e 8d03 0100 7405 6460 7c32  |*d]d^....t.d`|2
+00000eb0: 1700 6461 1700 8301 0100 7430 7c2a 7c25  ..da......t0|*|%
+00000ec0: 7c26 7c27 7c21 8305 7d33 7400 a031 7400  |&|'|!..}3t..1t.
+00000ed0: a032 640a a101 640a 1400 a101 640a 1400  .2d...d.....d...
+00000ee0: 7d34 6462 7d35 7c22 7c34 1b00 7d36 7400  }4db}5|"|4..}6t.
+00000ef0: 6a33 7c35 0b00 7c35 643a 1700 8502 7c35  j3|5..|5d:....|5
+00000f00: 0b00 7c35 643a 1700 8502 6602 1900 5c02  ..|5d:....f...\.
+00000f10: 7d37 7d38 7400 a034 7c38 640a 1300 7c37  }7}8t..4|8d...|7
+00000f20: 640a 1300 1700 0b00 6463 7c36 640a 1300  d.......dc|6d...
+00000f30: 1400 1b00 a101 7d39 7c39 7400 a035 7c39  ......}9|9t..5|9
+00000f40: a101 1d00 7d39 7c22 7436 1400 7d3a 7437  ....}9|"t6..}:t7
+00000f50: 7c3a 6464 6464 6465 8d03 7d3b 7c3b a038  |:ddddde..};|;.8
+00000f60: a100 0100 7414 7c16 8301 7d3c 7439 6a3a  ....t.|...}<t9j:
+00000f70: 7c2a 7c04 6466 8d02 7d3d 7439 a03b 7c2a  |*|.df..}=t9.;|*
+00000f80: 7c3d 7c3c a103 7d3e 7c09 6467 6b02 9008  |=|<..}>|.dgk...
+00000f90: 729c 7405 6468 8301 0100 7405 6469 8301  r.t.dh....t.di..
+00000fa0: 0100 7405 646a 8301 0100 7425 6a26 6446  ..t.dj....t%j&dF
+00000fb0: 6447 8d01 0100 7425 6a27 7c3e 6448 6449  dG....t%j'|>dHdI
+00000fc0: 8d02 0100 7c10 644e 6b02 9008 7282 7425  ....|.dNk...r.t%
+00000fd0: a029 a100 0100 6e08 7425 a02a a100 0100  .)....n.t%.*....
+00000fe0: 743c 7c2a 7c3e 7c3c 646b 646c 646d 8d05  t<|*|>|<dkdldm..
+00000ff0: 7d3e 7405 646e 8301 0100 7405 646f 8301  }>t.dn....t.do..
+00001000: 0100 7425 6a26 6446 6447 8d01 0100 7425  ..t%j&dFdG....t%
+00001010: 6a27 7c3e 6448 6470 6471 8d03 0100 644a  j'|>dHdpdq....dJ
+00001020: 7c01 6401 1900 7c11 1900 1700 6472 a008  |.d...|.....dr..
+00001030: 7c03 a101 1700 7d3f 7425 6a28 7c3f 644c  |.....}?t%j(|?dL
+00001040: 644d 8d02 0100 7c10 644e 6b02 9009 7204  dM....|.dNk...r.
+00001050: 7425 a029 a100 0100 6e08 7425 a02a a100  t%.)....n.t%.*..
+00001060: 0100 7405 7406 6a0e 6473 1700 8301 0100  ..t.t.j.ds......
+00001070: 7405 6474 8301 0100 743d a03d a100 7d40  t.dt....t=.=..}@
+00001080: 743e 6a3f 7c2a 7c3e 6a23 7c24 7c39 7c0f  t>j?|*|>j#|$|9|.
+00001090: 6475 8d05 7d41 7405 6476 743d a03d a100  du..}At.dvt=.=..
+000010a0: 7c40 1800 1600 8301 0100 7405 7420 7c41  |@........t.t |A
+000010b0: 8301 8301 0100 6477 6478 6479 647a 647b  ......dwdxdydzd{
+000010c0: 647c 647d 647e 647f 6480 6481 6482 6483  d|d}d~d.d.d.d.d.
+000010d0: 6484 670e 7d42 7405 6485 8301 0100 7405  d.g.}Bt.d.....t.
+000010e0: 6486 8301 0100 7c00 6402 640a 8502 1900  d.....|.d.d.....
+000010f0: 6487 6b02 9009 72bc 7c00 642a 1900 a040  d.k...r.|.d*...@
+00001100: a100 9009 72bc 7c00 6400 642a 8502 1900  ....r.|.d.d*....
+00001110: 7d00 7c06 6400 6b08 900b 722a 7400 a041  }.|.d.k...r*t..A
+00001120: 7c3e 6a42 a101 7d43 7443 7c43 6400 6400  |>jB..}CtC|Cd.d.
+00001130: 642a 8503 1900 8301 4400 9001 5d3e 5c02  d*......D...]>\.
+00001140: 7d44 7d45 7c41 7c45 1900 7d46 7444 7c46  }D}E|A|E..}FtD|F
+00001150: 7c00 7c42 7c44 1900 1700 7c2a 7c33 7c25  |.|B|D....|*|3|%
+00001160: 7c26 7c27 7c21 7c39 7c22 7c23 7c13 7c03  |&|'|!|9|"|#|.|.
+00001170: 7c0e 7c10 6488 8d0f 0100 7445 a016 7c0e  |.|.d.....tE..|.
+00001180: a101 7d47 7400 a001 7c47 6489 1900 7c00  ..}Gt...|Gd...|.
+00001190: 7c42 7c44 1900 1700 6b02 a101 6402 1900  |B|D....k...d...
+000011a0: 6402 1900 7d48 7400 a001 7c01 6401 1900  d...}Ht...|.d...
+000011b0: 7c00 6b02 a101 6402 1900 6402 1900 7d49  |.k...d...d...}I
+000011c0: 7c01 6410 1900 7c49 1900 7c47 6410 1900  |.d...|I..|Gd...
+000011d0: 7c48 3c00 7c01 6411 1900 7c49 1900 7c47  |H<.|.d...|I..|G
+000011e0: 6411 1900 7c48 3c00 7c01 6403 1900 7c49  d...|H<.|.d...|I
+000011f0: 1900 7c47 648a 1900 7c48 3c00 7a18 7c01  ..|Gd...|H<.z.|.
+00001200: 648b 1900 7c49 1900 7c47 648c 1900 7c48  d...|I..|Gd...|H
+00001210: 3c00 5700 6e24 0100 0100 0100 7c01 6403  <.W.n$......|.d.
+00001220: 1900 7c49 1900 7446 1b00 7c47 648c 1900  ..|I..tF..|Gd...
+00001230: 7c48 3c00 5900 6e02 5800 7a18 7c01 648d  |H<.Y.n.X.z.|.d.
+00001240: 1900 7c49 1900 7c47 648d 1900 7c48 3c00  ..|I..|Gd...|H<.
+00001250: 5700 6e14 0100 0100 0100 7405 648e 8301  W.n.......t.d...
+00001260: 0100 5900 6e02 5800 7445 6a19 7c47 7c0e  ..Y.n.X.tEj.|G|.
+00001270: 645d 645e 8d03 0100 9009 71e4 9001 6e4a  d]d^......q...nJ
+00001280: 7443 7c06 8301 4400 9001 5d3e 5c02 7d44  tC|...D...]>\.}D
+00001290: 7d45 7c41 7c45 1900 7d46 7444 7c46 7c00  }E|A|E..}FtD|F|.
+000012a0: 7c07 7c44 1900 1700 7c2a 7c33 7c25 7c26  |.|D....|*|3|%|&
+000012b0: 7c27 7c21 7c39 7c22 7c23 7c13 7c03 7c0e  |'|!|9|"|#|.|.|.
+000012c0: 7c10 6488 8d0f 0100 7445 a016 7c0e a101  |.d.....tE..|...
+000012d0: 7d47 7400 a001 7c47 6489 1900 7c00 7c07  }Gt...|Gd...|.|.
+000012e0: 7c44 1900 1700 6b02 a101 6402 1900 6402  |D....k...d...d.
+000012f0: 1900 7d48 7400 a001 7c01 6401 1900 7c00  ..}Ht...|.d...|.
+00001300: 6b02 a101 6402 1900 6402 1900 7d49 7c01  k...d...d...}I|.
+00001310: 6410 1900 7c49 1900 7c47 6410 1900 7c48  d...|I..|Gd...|H
+00001320: 3c00 7c01 6411 1900 7c49 1900 7c47 6411  <.|.d...|I..|Gd.
+00001330: 1900 7c48 3c00 7c01 6403 1900 7c49 1900  ..|H<.|.d...|I..
+00001340: 7c47 648a 1900 7c48 3c00 7a18 7c01 648b  |Gd...|H<.z.|.d.
+00001350: 1900 7c49 1900 7c47 648c 1900 7c48 3c00  ..|I..|Gd...|H<.
+00001360: 5700 6e24 0100 0100 0100 7c01 6403 1900  W.n$......|.d...
+00001370: 7c49 1900 7446 1b00 7c47 648c 1900 7c48  |I..tF..|Gd...|H
+00001380: 3c00 5900 6e02 5800 7a18 7c01 648d 1900  <.Y.n.X.z.|.d...
+00001390: 7c49 1900 7c47 648d 1900 7c48 3c00 5700  |I..|Gd...|H<.W.
+000013a0: 6e14 0100 0100 0100 7405 648e 8301 0100  n.......t.d.....
+000013b0: 5900 6e02 5800 7445 6a19 7c47 7c0e 645d  Y.n.X.tEj.|G|.d]
+000013c0: 645e 8d03 0100 900b 7132 7425 a029 a100  d^......q2t%.)..
+000013d0: 0100 6700 7d4a 7c07 4400 5d14 7d44 7c4a  ..g.}J|.D.].}D|J
+000013e0: a047 7c00 7c44 1700 a101 0100 900c 7184  .G|.|D........q.
+000013f0: 7405 648f a008 7c00 7c06 7c4a 7420 7c06  t.d...|.|.|Jt |.
+00001400: 8301 a104 8301 0100 6400 5300 2990 4eda  ........d.S.).N.
+00001410: 0367 616c 7201 0000 00da 0376 656c e7df  .galr......vel..
+00001420: bc9a 7856 3432 3fe7 0000 0000 0040 8f40  ..xV42?......@.@
+00001430: fa13 0a42 6173 6963 2069 6e66 6f72 6d61  ...Basic informa
+00001440: 7469 6f6e 3afa 132d 2d2d 2d2d 2d2d 2d2d  tion:..---------
+00001450: 2d2d 2d2d 2d2d 2d2d 2d2d fa0e 6172 635f  ----------..arc_
+00001460: 6b70 6320 7b3a 2e34 667d e79a 9999 9999  kpc {:.4f}......
+00001470: 99e1 3f72 3900 0000 e700 0000 0000 00e0  ..?r9...........
+00001480: 3fe7 0000 0000 0020 ac40 fa19 696d 6167  ?...... .@..imag
+00001490: 6520 7369 7a65 2069 6e20 7069 783a 207b  e size in pix: {
+000014a0: 3a2e 3166 7de7 5d8f c2f5 285c d33f fa30  :.1f}.]...(\.?.0
+000014b0: 4d69 6e69 6d75 6d20 6465 7465 6374 696f  Minimum detectio
+000014c0: 6e20 6172 6561 207b 3a2e 3166 7d20 6b63  n area {:.1f} kc
+000014d0: 705e 3220 3d20 7b3a 2e30 667d 2070 6978  p^2 = {:.0f} pix
+000014e0: da02 7261 da03 6465 63da 0566 6965 6c64  ..ra..dec..field
+000014f0: da02 4d43 fa33 0a3d 3d3d 3d3d 3d3d 3d3d  ..MC.3.=========
 00001500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001520: 3d3d 3d3d 3d3d 3dfa 3a0a 0a54 6869 7320  =======.:..This 
-00001530: 6761 6c61 7879 2069 7320 696e 2074 6865  galaxy is in the
-00001540: 204d 6167 656c 6c61 6e69 6320 436c 6f75   Magellanic Clou
-00001550: 6473 2054 696c 6573 2c20 7468 6572 6566  ds Tiles, theref
-00001560: 6f72 65fa 3374 6865 7265 2069 7320 6e6f  ore.3there is no
-00001570: 7420 6120 7068 6f74 6f6d 6574 7269 6320  t a photometric 
-00001580: 6361 7461 6c6f 6720 6176 6169 626c 6520  catalog avaible 
-00001590: 666f 7220 6974 2c20 7a28 7468 6520 7068  for it, z(the ph
-000015a0: 6f74 6f6d 6574 7269 6320 616e 616c 7973  otometric analys
-000015b0: 6973 2069 7320 6e6f 7420 706f 7373 6962  is is not possib
-000015c0: 6c65 fa28 0a0a 5468 6973 2067 616c 6178  le.(..This galax
-000015d0: 7920 6861 7320 6e6f 7420 7261 6469 616c  y has not radial
-000015e0: 2066 726f 6d20 5349 4d42 4144 fa29 7468   from SIMBAD.)th
-000015f0: 6520 7068 6f74 6f6d 6574 7269 6320 616e  e photometric an
-00001600: 616c 7973 6973 2069 7320 6e6f 7420 706f  alysis is not po
-00001610: 7373 6962 6c65 21fa 2b0a 0a4c 6f61 6469  ssible!.+..Loadi
-00001620: 6e67 2f44 6f77 6e6c 6f61 6469 6e67 2074  ng/Downloading t
-00001630: 6865 2069 6d61 6765 7320 616e 6420 7461  he images and ta
-00001640: 626c 6573 fa2d 2d2d 2d2d 2d2d 2d2d 2d2d  bles.-----------
+00001520: 3d3d 3d3d 3d3d 3d3d 3dfa 3a0a 0a54 6869  =========.:..Thi
+00001530: 7320 6761 6c61 7879 2069 7320 696e 2074  s galaxy is in t
+00001540: 6865 204d 6167 656c 6c61 6e69 6320 436c  he Magellanic Cl
+00001550: 6f75 6473 2054 696c 6573 2c20 7468 6572  ouds Tiles, ther
+00001560: 6566 6f72 65fa 3374 6865 7265 2069 7320  efore.3there is 
+00001570: 6e6f 7420 6120 7068 6f74 6f6d 6574 7269  not a photometri
+00001580: 6320 6361 7461 6c6f 6720 6176 6169 626c  c catalog avaibl
+00001590: 6520 666f 7220 6974 2c20 7a28 7468 6520  e for it, z(the 
+000015a0: 7068 6f74 6f6d 6574 7269 6320 616e 616c  photometric anal
+000015b0: 7973 6973 2069 7320 6e6f 7420 706f 7373  ysis is not poss
+000015c0: 6962 6c65 fa28 0a0a 5468 6973 2067 616c  ible.(..This gal
+000015d0: 6178 7920 6861 7320 6e6f 7420 7261 6469  axy has not radi
+000015e0: 616c 2066 726f 6d20 5349 4d42 4144 fa29  al from SIMBAD.)
+000015f0: 7468 6520 7068 6f74 6f6d 6574 7269 6320  the photometric 
+00001600: 616e 616c 7973 6973 2069 7320 6e6f 7420  analysis is not 
+00001610: 706f 7373 6962 6c65 21fa 2b0a 0a4c 6f61  possible!.+..Loa
+00001620: 6469 6e67 2f44 6f77 6e6c 6f61 6469 6e67  ding/Downloading
+00001630: 2074 6865 2069 6d61 6765 7320 616e 6420   the images and 
+00001640: 7461 626c 6573 fa2d 2d2d 2d2d 2d2d 2d2d  tables.---------
 00001650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001670: 2d2d 2dfa 1766 6974 735f 696d 6167 6573  ---..fits_images
-00001680: 2f7b 7d5f 7b7d 6b70 632e 667a fa1a 6669  /{}_{}kpc.fz..fi
-00001690: 7473 5f69 6d61 6765 732f 7b7d 5f7b 7d5f  ts_images/{}_{}_
-000016a0: 7b7d 6b70 632e 667a 723c 0000 00fa 0b0a  {}kpc.fzr<......
-000016b0: 5468 6520 696d 6167 6520 fa0e 2061 6c72  The image .. alr
-000016c0: 6561 6479 2065 7869 7374 fa0c 0a44 6f77  eady exist...Dow
-000016d0: 6c6f 6164 696e 6720 fa04 202e 2e2e e9fd  loading .. .....
-000016e0: ffff ffa9 01da 0866 696c 6570 6174 687a  .......filepathz
-000016f0: 1d23 2323 2323 2323 2323 2323 2323 2323  .###############
-00001700: 2323 2323 2323 2323 2323 2323 2323 7a0c  ##############z.
-00001710: 0a0a 2046 6965 6c64 3a20 7b7d 7a07 7461  .. Field: {}z.ta
-00001720: 626c 6573 2f7a 095f 6677 686d 2e74 6162  bles/z._fwhm.tab
-00001730: 7a12 7461 626c 6573 2f7b 7d5f 6677 686d  z.tables/{}_fwhm
-00001740: 2e74 6162 e9ff ffff ff72 0400 0000 a901  .tab.....r......
-00001750: da06 666f 726d 6174 7a0b 0a54 6865 2074  ..formatz..The t
-00001760: 6162 6c65 2061 4c01 0000 5345 4c45 4354  able aL...SELECT
-00001770: 2064 6574 2e49 442c 2064 6574 2e52 412c   det.ID, det.RA,
-00001780: 2064 6574 2e44 4543 2c20 6465 742e 412c   det.DEC, det.A,
-00001790: 2064 6574 2e42 2c20 6465 742e 5468 6574   det.B, det.Thet
-000017a0: 612c 2064 6574 2e4b 524f 4e5f 7241 4449  a, det.KRON_rADI
-000017b0: 5553 2c20 6465 742e 725f 6175 746f 2c20  US, det.r_auto, 
-000017c0: 6465 742e 434c 4153 535f 5354 4152 2c20  det.CLASS_STAR, 
-000017d0: 6465 742e 4649 454c 442c 2064 6574 2e6e  det.FIELD, det.n
-000017e0: 4465 745f 6175 746f 2c20 6465 742e 4657  Det_auto, det.FW
-000017f0: 484d 2c20 2064 6574 2e46 5748 4d5f 6e2c  HM,  det.FWHM_n,
-00001800: 2063 6c61 662e 434c 4153 532c 2063 6c61   claf.CLASS, cla
-00001810: 662e 6d6f 6465 6c5f 666c 6167 2c20 636c  f.model_flag, cl
-00001820: 6166 2e50 524f 425f 4741 4c2c 2063 6c61  af.PROB_GAL, cla
-00001830: 662e 5052 4f42 5f51 534f 2c20 636c 6166  f.PROB_QSO, claf
-00001840: 2e50 524f 425f 5354 4152 2020 4652 4f4d  .PROB_STAR  FROM
-00001850: 2069 6472 332e 616c 6c5f 6964 7233 2061   idr3.all_idr3 a
-00001860: 7320 6465 7420 6a6f 696e 2069 6472 332e  s det join idr3.
-00001870: 7661 635f 7374 6172 5f67 616c 6178 795f  vac_star_galaxy_
-00001880: 7175 6173 6172 2061 7320 636c 6166 206f  quasar as claf o
-00001890: 6e20 636c 6166 2e49 4420 3d20 6465 742e  n claf.ID = det.
-000018a0: 4944 2057 4845 5245 2064 6574 2e46 4945  ID WHERE det.FIE
-000018b0: 4c44 203d 2027 7a1b 2720 616e 6420 636c  LD = 'z.' and cl
-000018c0: 6166 2e50 524f 425f 5354 4152 203e 2030  af.PROB_STAR > 0
-000018d0: 2e38 207a 2561 6e64 2064 6574 2e72 5f61  .8 z%and det.r_a
-000018e0: 7574 6f20 3e31 3320 616e 6420 6465 742e  uto >13 and det.
-000018f0: 725f 6175 746f 3c31 3720 7a1f 0a44 6f69  r_auto<17 z..Doi
-00001900: 6e67 2074 6865 2066 6f6c 6c6f 7769 6e67  ng the following
-00001910: 2071 7565 7279 202e 2e2e 0afa 1e0a 0a5a   query ........Z
-00001920: 5020 616e 6420 6d65 616e 2050 5346 206f  P and mean PSF o
-00001930: 6620 7468 6520 4669 656c 64fa 202d 2d2d  f the Field. ---
+00001670: 2d2d 2d2d 2dfa 1766 6974 735f 696d 6167  -----..fits_imag
+00001680: 6573 2f7b 7d5f 7b7d 6b70 632e 667a fa1a  es/{}_{}kpc.fz..
+00001690: 6669 7473 5f69 6d61 6765 732f 7b7d 5f7b  fits_images/{}_{
+000016a0: 7d5f 7b7d 6b70 632e 667a 723c 0000 00fa  }_{}kpc.fzr<....
+000016b0: 0b0a 5468 6520 696d 6167 6520 fa0e 2061  ..The image .. a
+000016c0: 6c72 6561 6479 2065 7869 7374 fa0c 0a44  lready exist...D
+000016d0: 6f77 6c6f 6164 696e 6720 fa04 202e 2e2e  owloading .. ...
+000016e0: e9fd ffff ffa9 01da 0866 696c 6570 6174  .........filepat
+000016f0: 687a 1d23 2323 2323 2323 2323 2323 2323  hz.#############
+00001700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001710: 7a0c 0a0a 2046 6965 6c64 3a20 7b7d 7a07  z... Field: {}z.
+00001720: 7461 626c 6573 2f7a 095f 6677 686d 2e74  tables/z._fwhm.t
+00001730: 6162 7a12 7461 626c 6573 2f7b 7d5f 6677  abz.tables/{}_fw
+00001740: 686d 2e74 6162 e9ff ffff ff72 0400 0000  hm.tab.....r....
+00001750: a901 da06 666f 726d 6174 7a0b 0a54 6865  ....formatz..The
+00001760: 2074 6162 6c65 2061 4c01 0000 5345 4c45   table aL...SELE
+00001770: 4354 2064 6574 2e49 442c 2064 6574 2e52  CT det.ID, det.R
+00001780: 412c 2064 6574 2e44 4543 2c20 6465 742e  A, det.DEC, det.
+00001790: 412c 2064 6574 2e42 2c20 6465 742e 5468  A, det.B, det.Th
+000017a0: 6574 612c 2064 6574 2e4b 524f 4e5f 7241  eta, det.KRON_rA
+000017b0: 4449 5553 2c20 6465 742e 725f 6175 746f  DIUS, det.r_auto
+000017c0: 2c20 6465 742e 434c 4153 535f 5354 4152  , det.CLASS_STAR
+000017d0: 2c20 6465 742e 4649 454c 442c 2064 6574  , det.FIELD, det
+000017e0: 2e6e 4465 745f 6175 746f 2c20 6465 742e  .nDet_auto, det.
+000017f0: 4657 484d 2c20 2064 6574 2e46 5748 4d5f  FWHM,  det.FWHM_
+00001800: 6e2c 2063 6c61 662e 434c 4153 532c 2063  n, claf.CLASS, c
+00001810: 6c61 662e 6d6f 6465 6c5f 666c 6167 2c20  laf.model_flag, 
+00001820: 636c 6166 2e50 524f 425f 4741 4c2c 2063  claf.PROB_GAL, c
+00001830: 6c61 662e 5052 4f42 5f51 534f 2c20 636c  laf.PROB_QSO, cl
+00001840: 6166 2e50 524f 425f 5354 4152 2020 4652  af.PROB_STAR  FR
+00001850: 4f4d 2069 6472 332e 616c 6c5f 6964 7233  OM idr3.all_idr3
+00001860: 2061 7320 6465 7420 6a6f 696e 2069 6472   as det join idr
+00001870: 332e 7661 635f 7374 6172 5f67 616c 6178  3.vac_star_galax
+00001880: 795f 7175 6173 6172 2061 7320 636c 6166  y_quasar as claf
+00001890: 206f 6e20 636c 6166 2e49 4420 3d20 6465   on claf.ID = de
+000018a0: 742e 4944 2057 4845 5245 2064 6574 2e46  t.ID WHERE det.F
+000018b0: 4945 4c44 203d 2027 7a1b 2720 616e 6420  IELD = 'z.' and 
+000018c0: 636c 6166 2e50 524f 425f 5354 4152 203e  claf.PROB_STAR >
+000018d0: 2030 2e38 207a 2561 6e64 2064 6574 2e72   0.8 z%and det.r
+000018e0: 5f61 7574 6f20 3e31 3320 616e 6420 6465  _auto >13 and de
+000018f0: 742e 725f 6175 746f 3c31 3720 7a1f 0a44  t.r_auto<17 z..D
+00001900: 6f69 6e67 2074 6865 2066 6f6c 6c6f 7769  oing the followi
+00001910: 6e67 2071 7565 7279 202e 2e2e 0afa 1e0a  ng query .......
+00001920: 0a5a 5020 616e 6420 6d65 616e 2050 5346  .ZP and mean PSF
+00001930: 206f 6620 7468 6520 4669 656c 64fa 202d   of the Field. -
 00001940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7a 112f  -------------z./
-00001960: 7a65 726f 5f70 6f69 6e74 732e 6669 7473  zero_points.fits
-00001970: da05 4669 656c 647a 0d0a 6964 5f7a 705f  ..Fieldz..id_zp_
-00001980: 7461 626c 653a 7a09 5a50 3d7b 3a2e 3166  table:z.ZP={:.1f
-00001990: 7d7a 0646 6965 6c64 3ada 0446 5748 4de9  }z.Field:..FWHM.
-000019a0: 0100 0000 7a21 0a4e 756d 6265 7220 6f66  ....z!.Number of
-000019b0: 2073 7461 7220 3133 3c52 5f61 7574 6f3c   star 13<R_auto<
-000019c0: 3137 203a 207b 7dfa 214d 6564 6961 6e20  17 : {}.!Median 
-000019d0: 6677 686d 2069 6e20 7468 6520 6669 656c  fwhm in the fiel
-000019e0: 6420 3a20 7b3a 2e31 667d e700 0000 0000  d : {:.1f}......
-000019f0: 0000 007a 0c5f 7b7d 5f7b 7d6b 7063 2e66  ...z._{}_{}kpc.f
-00001a00: 7afa 0c66 6974 735f 696d 6167 6573 2f7a  z..fits_images/z
-00001a10: 095f 7b7d 6b70 632e 667a 7a20 0a54 6865  ._{}kpc.fzz .The
-00001a20: 2061 6e61 6c79 7369 7320 6973 2070 6572   analysis is per
-00001a30: 666f 726d 6564 206f 6e20 7b7d fa22 0a0a  formed on {}."..
-00001a40: 4361 6c63 756c 6174 696e 6720 7468 6520  Calculating the 
-00001a50: 696d 6167 6520 6261 636b 6772 6f75 6e64  image background
-00001a60: fa2a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .*--------------
+00001950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7a  ---------------z
+00001960: 112f 7a65 726f 5f70 6f69 6e74 732e 6669  ./zero_points.fi
+00001970: 7473 da05 4669 656c 647a 0d0a 6964 5f7a  ts..Fieldz..id_z
+00001980: 705f 7461 626c 653a 7a09 5a50 3d7b 3a2e  p_table:z.ZP={:.
+00001990: 3166 7d7a 0646 6965 6c64 3ada 0446 5748  1f}z.Field:..FWH
+000019a0: 4de9 0100 0000 7a21 0a4e 756d 6265 7220  M.....z!.Number 
+000019b0: 6f66 2073 7461 7220 3133 3c52 5f61 7574  of star 13<R_aut
+000019c0: 6f3c 3137 203a 207b 7dfa 214d 6564 6961  o<17 : {}.!Media
+000019d0: 6e20 6677 686d 2069 6e20 7468 6520 6669  n fwhm in the fi
+000019e0: 656c 6420 3a20 7b3a 2e31 667d e700 0000  eld : {:.1f}....
+000019f0: 0000 0000 007a 0c5f 7b7d 5f7b 7d6b 7063  .....z._{}_{}kpc
+00001a00: 2e66 7afa 0c66 6974 735f 696d 6167 6573  .fz..fits_images
+00001a10: 2f7a 095f 7b7d 6b70 632e 667a 7a20 0a54  /z._{}kpc.fzz .T
+00001a20: 6865 2061 6e61 6c79 7369 7320 6973 2070  he analysis is p
+00001a30: 6572 666f 726d 6564 206f 6e20 7b7d fa22  erformed on {}."
+00001a40: 0a0a 4361 6c63 756c 6174 696e 6720 7468  ..Calculating th
+00001a50: 6520 696d 6167 6520 6261 636b 6772 6f75  e image backgrou
+00001a60: 6e64 fa2a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  nd.*------------
 00001a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d fa25 4d61  ------------.%Ma
-00001a90: 736b 696e 6720 7468 6520 736f 7572 6365  sking the source
-00001aa0: 7320 6f76 6572 2074 6865 2069 6d61 6765  s over the image
-00001ab0: 2e2e 2ea9 03da 066e 7369 676d 61da 076e  .......nsigma..n
-00001ac0: 7069 7865 6c73 da0b 6469 6c61 7465 5f73  pixels..dilate_s
-00001ad0: 697a 65a9 02e7 0000 0000 0000 1a40 7275  ize..........@ru
-00001ae0: 0000 00a9 01da 0766 6967 7369 7a65 da05  .......figsize..
-00001af0: 6c6f 7765 72a9 01da 066f 7269 6769 6efa  lower....origin.
-00001b00: 0b69 6d61 6765 732f 6669 675f 7a13 5f7b  .images/fig_z._{
-00001b10: 7d6b 7063 5f73 6b79 5f6d 6173 6b2e 706e  }kpc_sky_mask.pn
-00001b20: 67da 0574 6967 6874 a901 da0b 6262 6f78  g..tight....bbox
-00001b30: 5f69 6e63 6865 7372 4000 0000 e700 0000  _inchesr@.......
-00001b40: 0000 0026 40a9 02da 0573 6967 6d61 da04  ...&@....sigma..
-00001b50: 6d61 736b fa2d 0a0a 4d65 6469 616e 2053  mask.-..Median S
-00001b60: 6b79 2073 7562 7472 6163 7469 6f6e 2066  ky subtraction f
-00001b70: 6f72 2074 6865 2077 686f 6c65 2063 7574  or the whole cut
-00001b80: 6f75 74fa 2c2d 2d2d 2d2d 2d2d 2d2d 2d2d  out.,-----------
+00001a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d fa25  --------------.%
+00001a90: 4d61 736b 696e 6720 7468 6520 736f 7572  Masking the sour
+00001aa0: 6365 7320 6f76 6572 2074 6865 2069 6d61  ces over the ima
+00001ab0: 6765 2e2e 2ea9 03da 066e 7369 676d 61da  ge.......nsigma.
+00001ac0: 076e 7069 7865 6c73 da0b 6469 6c61 7465  .npixels..dilate
+00001ad0: 5f73 697a 65a9 02e7 0000 0000 0000 1a40  _size..........@
+00001ae0: 7275 0000 00a9 01da 0766 6967 7369 7a65  ru.......figsize
+00001af0: da05 6c6f 7765 72a9 01da 066f 7269 6769  ..lower....origi
+00001b00: 6efa 0b69 6d61 6765 732f 6669 675f 7a13  n..images/fig_z.
+00001b10: 5f7b 7d6b 7063 5f73 6b79 5f6d 6173 6b2e  _{}kpc_sky_mask.
+00001b20: 706e 67da 0574 6967 6874 a901 da0b 6262  png..tight....bb
+00001b30: 6f78 5f69 6e63 6865 7372 4000 0000 e700  ox_inchesr@.....
+00001b40: 0000 0000 0026 40a9 02da 0573 6967 6d61  .....&@....sigma
+00001b50: da04 6d61 736b fa2d 0a0a 4d65 6469 616e  ..mask.-..Median
+00001b60: 2053 6b79 2073 7562 7472 6163 7469 6f6e   Sky subtraction
+00001b70: 2066 6f72 2074 6865 2077 686f 6c65 2063   for the whole c
+00001b80: 7574 6f75 74fa 2c2d 2d2d 2d2d 2d2d 2d2d  utout.,---------
 00001b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001bb0: 2dfa 166d 6561 6e5f 736b 795f 3a73 6567  -..mean_sky_:seg
-00001bc0: 203d 207b 3a2e 3266 7dfa 156d 6564 6961   = {:.2f}..media
-00001bd0: 6e5f 736b 795f 6720 3d20 7b3a 2e32 667d  n_sky_g = {:.2f}
-00001be0: fa12 7374 645f 736b 795f 6720 3d20 7b3a  ..std_sky_g = {:
-00001bf0: 2e32 667d fa45 0a0a 4573 7469 6d61 7469  .2f}.E..Estimati
-00001c00: 6e67 2074 6865 2032 4420 736b 7920 5f62  ng the 2D sky _b
-00001c10: 6163 6b67 726f 756e 6420 6279 2075 7369  ackground by usi
-00001c20: 6e67 2061 2073 6b79 2062 6f78 206f 6620  ng a sky box of 
-00001c30: 7b7d 787b 7d20 7069 7865 6cfa 432d 2d2d  {}x{} pixel.C---
+00001bb0: 2d2d 2dfa 166d 6561 6e5f 736b 795f 3a73  ---..mean_sky_:s
+00001bc0: 6567 203d 207b 3a2e 3266 7dfa 156d 6564  eg = {:.2f}..med
+00001bd0: 6961 6e5f 736b 795f 6720 3d20 7b3a 2e32  ian_sky_g = {:.2
+00001be0: 667d fa12 7374 645f 736b 795f 6720 3d20  f}..std_sky_g = 
+00001bf0: 7b3a 2e32 667d fa45 0a0a 4573 7469 6d61  {:.2f}.E..Estima
+00001c00: 7469 6e67 2074 6865 2032 4420 736b 7920  ting the 2D sky 
+00001c10: 5f62 6163 6b67 726f 756e 6420 6279 2075  _background by u
+00001c20: 7369 6e67 2061 2073 6b79 2062 6f78 206f  sing a sky box o
+00001c30: 6620 7b7d 787b 7d20 7069 7865 6cfa 432d  f {}x{} pixel.C-
 00001c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00001c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001c80: a902 e903 0000 0072 8b00 0000 a904 da0b  .......r........
-00001c90: 6669 6c74 6572 5f73 697a 65da 0d62 6b67  filter_size..bkg
-00001ca0: 5f65 7374 696d 6174 6f72 da0d 636f 7665  _estimator..cove
-00001cb0: 7261 6765 5f6d 6173 6bda 0a66 696c 6c5f  rage_mask..fill_
-00001cc0: 7661 6c75 657a 0e5f 7b7d 6b70 635f 736b  valuez._{}kpc_sk
-00001cd0: 792e 706e 677a 065f 7b7d 6b70 63fa 095f  y.pngz._{}kpc.._
-00001ce0: 736b 792e 6669 7473 54a9 01da 096f 7665  sky.fitsT....ove
-00001cf0: 7277 7269 7465 fa0d 5f73 6b79 5f73 7562  rwrite.._sky_sub
-00001d00: 2e66 6974 73fa 1353 6176 696e 6720 6669  .fits..Saving fi
-00001d10: 7473 5f69 6d61 6765 732f fa11 5f73 6b79  ts_images/.._sky
-00001d20: 5f73 7562 2e66 6974 732e 2e2e 0ae9 1400  _sub.fits.......
-00001d30: 0000 7238 0000 0072 8b00 0000 a902 da06  ..r8...r........
-00001d40: 785f 7369 7a65 da06 795f 7369 7a65 a901  x_size..y_size..
-00001d50: 7271 0000 00da 026f 6efa 160a 5065 7266  rq.....on...Perf
-00001d60: 6f72 6d69 6e67 2064 6562 6c65 6469 6e67  orming debleding
-00001d70: 3afa 172d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :..-------------
-00001d80: 2d2d 2d2d 2d2d 2d2d 2d2d fa22 5365 676d  ----------."Segm
-00001d90: 656e 7461 7469 6f6e 206d 6170 2077 6974  entation map wit
-00001da0: 686f 7574 2064 6562 6c65 6469 6e67 e920  hout debleding. 
-00001db0: 0000 00e7 fca9 f1d2 4d62 503f a903 7272  ........MbP?..rr
-00001dc0: 0000 00da 076e 6c65 7665 6c73 da08 636f  .....nlevels..co
-00001dd0: 6e74 7261 7374 fa18 0a46 696e 616c 2053  ntrast...Final S
-00001de0: 6567 6d65 6e74 6174 696f 6e20 6d61 703a  egmentation map:
-00001df0: fa19 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
-00001e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2dda 0467 7261  -----------..gra
-00001e10: 7929 0272 7a00 0000 da04 636d 6170 7a0f  y).rz.....cmapz.
-00001e20: 5f7b 7d6b 7063 5f73 6567 6d2e 706e 67fa  _{}kpc_segm.png.
-00001e30: 130a 0a52 756e 6e69 6e67 2053 7461 746d  ...Running Statm
-00001e40: 6f72 7068 fa15 2d2d 2d2d 2d2d 2d2d 2d2d  orph..----------
-00001e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2da9 03da 0467  -----------....g
-00001e60: 6169 6eda 0370 7366 da03 6574 61fa 0b54  ain..psf..eta..T
-00001e70: 696d 653a 2025 6720 732e da01 41da 0142  ime: %g s...A..B
-00001e80: da01 43da 0144 da01 45da 0146 da01 47da  ..C..D..E..F..G.
-00001e90: 0148 7234 0000 00da 014a da01 4bda 014c  .Hr4.....J..K..L
-00001ea0: da01 4dda 014e fa09 0a0a 5265 7375 6c74  ..M..N....Result
-00001eb0: 73fa 0c2d 2d2d 2d2d 2d2d 2d2d 2d2d 0ada  s..-----------..
-00001ec0: 0241 4d29 02da 0a6f 7574 7075 7466 696c  .AM)...outputfil
-00001ed0: 65da 0973 686f 775f 706c 6f74 da03 4741  e..show_plot..GA
-00001ee0: 4cda 0672 6164 7665 6cda 015a da01 7ada  L..radvel..Z..z.
-00001ef0: 064a 636c 6173 73da 0061 1901 0000 534c  .Jclass..a....SL
-00001f00: 2e70 6c6f 745f 7369 6d62 6164 2827 7b7d  .plot_simbad('{}
-00001f10: 272c 2074 6162 5f67 616c 2c20 636f 6e6e  ', tab_gal, conn
-00001f20: 2c20 7369 7a65 5f69 6d61 6765 5f70 6879  , size_image_phy
-00001f30: 3d31 3030 2c0a 2020 2020 2020 2020 2020  =100,.          
+00001c80: 2d2d a902 e903 0000 0072 8b00 0000 a904  --.......r......
+00001c90: da0b 6669 6c74 6572 5f73 697a 65da 0d62  ..filter_size..b
+00001ca0: 6b67 5f65 7374 696d 6174 6f72 da0d 636f  kg_estimator..co
+00001cb0: 7665 7261 6765 5f6d 6173 6bda 0a66 696c  verage_mask..fil
+00001cc0: 6c5f 7661 6c75 657a 0e5f 7b7d 6b70 635f  l_valuez._{}kpc_
+00001cd0: 736b 792e 706e 677a 065f 7b7d 6b70 63fa  sky.pngz._{}kpc.
+00001ce0: 095f 736b 792e 6669 7473 54a9 01da 096f  ._sky.fitsT....o
+00001cf0: 7665 7277 7269 7465 fa0d 5f73 6b79 5f73  verwrite.._sky_s
+00001d00: 7562 2e66 6974 73fa 1353 6176 696e 6720  ub.fits..Saving 
+00001d10: 6669 7473 5f69 6d61 6765 732f fa11 5f73  fits_images/.._s
+00001d20: 6b79 5f73 7562 2e66 6974 732e 2e2e 0ae9  ky_sub.fits.....
+00001d30: 1400 0000 7238 0000 0072 8b00 0000 a902  ....r8...r......
+00001d40: da06 785f 7369 7a65 da06 795f 7369 7a65  ..x_size..y_size
+00001d50: a901 7271 0000 00da 026f 6efa 160a 5065  ..rq.....on...Pe
+00001d60: 7266 6f72 6d69 6e67 2064 6562 6c65 6469  rforming debledi
+00001d70: 6e67 3afa 172d 2d2d 2d2d 2d2d 2d2d 2d2d  ng:..-----------
+00001d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d fa22 5365  ------------."Se
+00001d90: 676d 656e 7461 7469 6f6e 206d 6170 2077  gmentation map w
+00001da0: 6974 686f 7574 2064 6562 6c65 6469 6e67  ithout debleding
+00001db0: e920 0000 00e7 fca9 f1d2 4d62 503f a903  . ........MbP?..
+00001dc0: 7272 0000 00da 076e 6c65 7665 6c73 da08  rr.....nlevels..
+00001dd0: 636f 6e74 7261 7374 fa18 0a46 696e 616c  contrast...Final
+00001de0: 2053 6567 6d65 6e74 6174 696f 6e20 6d61   Segmentation ma
+00001df0: 703a fa19 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  p:..------------
+00001e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2dda 0467  -------------..g
+00001e10: 7261 7929 0272 7a00 0000 da04 636d 6170  ray).rz.....cmap
+00001e20: 7a0f 5f7b 7d6b 7063 5f73 6567 6d2e 706e  z._{}kpc_segm.pn
+00001e30: 67fa 130a 0a52 756e 6e69 6e67 2053 7461  g....Running Sta
+00001e40: 746d 6f72 7068 fa15 2d2d 2d2d 2d2d 2d2d  tmorph..--------
+00001e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2da9 03da  -------------...
+00001e60: 0467 6169 6eda 0370 7366 da03 6574 61fa  .gain..psf..eta.
+00001e70: 0b54 696d 653a 2025 6720 732e da01 41da  .Time: %g s...A.
+00001e80: 0142 da01 43da 0144 da01 45da 0146 da01  .B..C..D..E..F..
+00001e90: 47da 0148 7234 0000 00da 014a da01 4bda  G..Hr4.....J..K.
+00001ea0: 014c da01 4dda 014e fa09 0a0a 5265 7375  .L..M..N....Resu
+00001eb0: 6c74 73fa 0c2d 2d2d 2d2d 2d2d 2d2d 2d2d  lts..-----------
+00001ec0: 0ada 0241 4d29 02da 0a6f 7574 7075 7466  ...AM)...outputf
+00001ed0: 696c 65da 0973 686f 775f 706c 6f74 da03  ile..show_plot..
+00001ee0: 4741 4cda 0672 6164 7665 6cda 015a da01  GAL..radvel..Z..
+00001ef0: 7ada 064a 636c 6173 73da 0061 1901 0000  z..Jclass..a....
+00001f00: 534c 2e70 6c6f 745f 7369 6d62 6164 2827  SL.plot_simbad('
+00001f10: 7b7d 272c 2074 6162 5f67 616c 2c20 636f  {}', tab_gal, co
+00001f20: 6e6e 2c20 7369 7a65 5f69 6d61 6765 5f70  nn, size_image_p
+00001f30: 6879 3d31 3030 2c0a 2020 2020 2020 2020  hy=100,.        
 00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 7461 626c 653d 6f75 7470 7574 2c20 2075  table=output,  u
-00001f60: 7365 725f 6f72 6465 723d 7b7d 2c0a 2020  ser_order={},.  
+00001f50: 2020 7461 626c 653d 6f75 7470 7574 2c20    table=output, 
+00001f60: 2075 7365 725f 6f72 6465 723d 7b7d 2c0a   user_order={},.
 00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2020 2020 7573 6572 5f74 6578          user_tex
-00001f90: 743d 7b7d 2c20 7874 706f 733d 3630 2c20  t={}, xtpos=60, 
-00001fa0: 7974 706f 733d 3130 2c0a 2020 2020 2020  ytpos=10,.      
+00001f80: 2020 2020 2020 2020 2020 7573 6572 5f74            user_t
+00001f90: 6578 743d 7b7d 2c20 7874 706f 733d 3630  ext={}, xtpos=60
+00001fa0: 2c20 7974 706f 733d 3130 2c0a 2020 2020  , ytpos=10,.    
 00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 6465 6c74 6179 3d31 302c 2073      deltay=10, s
-00001fd0: 6176 6566 6967 3d27 7965 7327 2c20 6974  avefig='yes', it
-00001fe0: 7363 6f6e 7369 6465 723d 2779 6573 272c  sconsider='yes',
-00001ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002000: 2020 2020 2020 2020 2020 204e 6d65 6d62             Nmemb
-00002010: 6572 733d 7b7d 2929 4872 2500 0000 da05  ers={}))Hr%.....
-00002020: 7768 6572 6572 b700 0000 da03 7461 6eda  wherer......tan.
-00002030: 0764 6567 3272 6164 da05 7072 696e 7472  .deg2rad..printr
-00002040: 1900 0000 da04 424c 5545 7264 0000 00da  ......BLUErd....
-00002050: 0673 7175 6172 65da 0270 69da 0b63 6865  .square..pi..che
-00002060: 636b 636f 6f72 6473 da04 6368 6172 da0a  ckcoords..char..
-00002070: 7374 6172 7473 7769 7468 da03 5245 44da  startswith..RED.
-00002080: 0569 736e 616e da02 6f73 da04 7061 7468  .isnan..os..path
-00002090: da06 6578 6973 7473 da07 6765 745f 6375  ..exists..get_cu
-000020a0: 74da 0369 6e74 7205 0000 00da 0472 6561  t..intr......rea
-000020b0: 64da 0373 7472 da05 7175 6572 79da 0577  d..str..query..w
-000020c0: 7269 7465 da05 424c 4143 4bda 0764 6972  rite..BLACK..dir
-000020d0: 6e61 6d65 da08 7265 616c 7061 7468 da08  name..realpath..
-000020e0: 5f5f 6669 6c65 5f5f da05 726f 756e 64da  __file__..round.
-000020f0: 096e 616e 6d65 6469 616e da03 6c65 6e72  .nanmedian..lenr
-00002100: 0300 0000 da04 6f70 656e da04 6461 7461  ......open..data
-00002110: 720a 0000 00da 0370 6c74 da06 6669 6775  r......plt..figu
-00002120: 7265 da06 696d 7368 6f77 da07 7361 7665  re..imshow..save
-00002130: 6669 67da 0473 686f 77da 0563 6c6f 7365  fig..show..close
-00002140: 720b 0000 0072 0d00 0000 720c 0000 00da  r....r....r.....
-00002150: 0a62 6163 6b67 726f 756e 64da 0777 7269  .background..wri
-00002160: 7465 746f 7231 0000 00da 0473 7172 7472  tetor1.....sqrtr
-00002170: 3300 0000 da05 6d67 7269 64da 0365 7870  3.....mgrid..exp
-00002180: da03 7375 6d72 1100 0000 7210 0000 00da  ..sumr....r.....
-00002190: 096e 6f72 6d61 6c69 7a65 da09 7068 6f74  .normalize..phot
-000021a0: 7574 696c 73da 1064 6574 6563 745f 7468  utils..detect_th
-000021b0: 7265 7368 6f6c 6472 0e00 0000 720f 0000  resholdr....r...
-000021c0: 00da 0474 696d 65da 0973 7461 746d 6f72  ...time..statmor
-000021d0: 7068 da11 736f 7572 6365 5f6d 6f72 7068  ph..source_morph
-000021e0: 6f6c 6f67 79da 0769 7361 6c70 6861 da07  ology..isalpha..
-000021f0: 6172 6773 6f72 74da 0561 7265 6173 da09  argsort..areas..
-00002200: 656e 756d 6572 6174 65da 0970 6c6f 745f  enumerate..plot_
-00002210: 7374 6174 7204 0000 00da 0763 5f73 7065  statr......c_spe
-00002220: 6564 da06 6170 7065 6e64 294b 7241 0000  ed..append)KrA..
-00002230: 00da 0774 6162 5f67 616c da04 636f 6e6e  ...tab_gal..conn
-00002240: da0e 7369 7a65 5f69 6d61 6765 5f70 6879  ..size_image_phy
-00002250: da05 736e 725f 67da 0761 7265 6167 616c  ..snr_g..areagal
-00002260: da0a 7573 6572 5f6f 7264 6572 da09 7573  ..user_order..us
-00002270: 6572 5f6c 6973 74da 0773 6b79 5f62 6f78  er_list..sky_box
-00002280: da07 6465 626c 656e 64da 0462 616e 6472  ..deblend..bandr
-00002290: 7100 0000 7272 0000 0072 7300 0000 72c0  q...rr...rs...r.
-000022a0: 0000 0072 ae00 0000 72c1 0000 00da 0369  ...r....r......i
-000022b0: 6467 72b3 0000 00da 0761 7263 5f6b 7063  dgr......arc_kpc
-000022c0: da0a 7369 7a65 5f69 6d61 6765 da0a 7261  ..size_image..ra
-000022d0: 6469 7573 5f63 6174 da08 6172 6561 5f6d  dius_cat..area_m
-000022e0: 696e da03 6f75 7472 d500 0000 da05 7061  in..outr......pa
-000022f0: 7468 7472 6700 0000 da06 7061 7468 7474  thtrg.....pathtt
-00002300: da08 7461 625f 6677 686d da0a 7175 6572  ..tab_fwhm..quer
-00002310: 795f 7478 7431 da09 6469 7265 6362 6173  y_txt1..direcbas
-00002320: 65da 025a 50da 0569 645f 7a70 722d 0000  e..ZP..id_zpr-..
-00002330: 00da 0570 7366 5f67 da07 7363 5f69 6d61  ...psf_g..sc_ima
-00002340: 6772 ac00 0000 da0c 6d65 6469 616e 5f73  gr......median_s
-00002350: 6b79 5f67 722b 0000 0072 2c00 0000 da06  ky_gr+...r,.....
-00002360: 7061 7468 5f61 da05 696d 6167 6eda 0469  path_a..imagn..i
-00002370: 6d61 67da 066d 6173 6b5f 67da 0366 6967  mag..mask_g..fig
-00002380: da08 6d65 616e 5f73 6b79 da0a 6d65 6469  ..mean_sky..medi
-00002390: 616e 5f73 6b79 da07 7374 645f 736b 7972  an_sky..std_skyr
-000023a0: 8e00 0000 da03 626b 67da 0770 6174 6867  ......bkg..pathg
-000023b0: 616c da05 696d 6167 6dda 0766 6163 5f73  al..imagm..fac_s
-000023c0: 6967 da04 7369 7a65 da09 7369 676d 615f  ig..size..sigma_
-000023d0: 7073 66da 0179 da01 78da 0470 7366 6772  psf..y..x..psfgr
-000023e0: 8100 0000 da06 6b65 726e 656c da09 6e70  ......kernel..np
-000023f0: 6978 656c 735f 67da 0974 6872 6573 686f  ixels_g..thresho
-00002400: 6c64 da04 7365 676d da05 7361 7665 6eda  ld..segm..saven.
-00002410: 0573 7461 7274 da0d 736f 7572 6365 5f6d  .start..source_m
-00002420: 6f72 7068 73da 056c 6973 746c da05 736f  orphs..listl..so
-00002430: 7274 61da 0169 da04 6761 6c69 da05 6d6f  rta..i..gali..mo
-00002440: 7270 6872 e500 0000 da03 696e 64da 0669  rphr......ind..i
-00002450: 6e64 6761 6cda 0a6e 7573 6572 5f6c 6973  ndgal..nuser_lis
-00002460: 7472 2f00 0000 722f 0000 0072 3000 0000  tr/...r/...r0...
-00002470: da08 7068 6f74 5f6d 6f64 5300 0000 731c  ..phot_modS...s.
-00002480: 0200 0000 051a 0110 0118 010e 010e 0114  ................
-00002490: 0110 0110 0114 011c 010c 0102 ff08 031c  ................
-000024a0: 0114 010e 010e 010e 010e 0104 020c 010e  ................
-000024b0: 010e 010e 0104 020e 0108 020c 010e 0126  ...............&
-000024c0: 0110 0126 0110 011e 0102 000a ff06 030e  ...&............
-000024d0: 0110 0218 0110 011e 0102 010a fe06 2408  ..............$.
-000024e0: 0208 0114 0108 020c 0112 010a 012a 050e  .............*..
-000024f0: 010e 0110 010e 010e 0110 010e 010e 0112  ................
-00002500: 0202 0706 f902 0802 f802 0902 f704 0a0a  ................
-00002510: 010a 0316 020e 0108 0214 010e 0122 010c  ............."..
-00002520: 010e 0102 0006 ff04 0416 0116 010e 0204  ................
-00002530: 0104 0104 010a 0104 0218 010a 0102 0106  ................
-00002540: 010a ff02 0108 ff06 020a 0114 ff0c 0206  ................
-00002550: 010e 011c 020e 0114 010a 050e 0108 0108  ................
-00002560: 0108 0102 ff06 020c 010e 0114 0102 ff06  ................
-00002570: 020a 010a 0208 0206 0102 ff0c 020e 0108  ................
-00002580: 010e 010e 010e 0306 0106 0006 ff06 0208  ................
-00002590: 0206 0108 0102 0002 0102 fe06 040a 020c  ................
-000025a0: 0110 0114 0102 ff06 020a 010a 0208 0216  ................
-000025b0: 011a 0118 0110 0310 0718 0104 0108 0126  ...............&
-000025c0: 0124 010e 0508 010e 0108 0308 010e 010e  .$..............
-000025d0: 020a 0108 0108 0208 010c 010e 010a 010a  ................
-000025e0: 0208 0108 0202 0002 fe06 0f08 0108 020c  ................
-000025f0: 0110 021a 010e 020a 010a 0208 040e 0108  ................
-00002600: 0208 0106 0104 0002 0002 0002 ff06 0214  ................
-00002610: 010c 0220 0208 0108 0320 010c 020a 010c  ... ..... ......
-00002620: 011c 0208 011a 0102 0002 0002 0002 0002  ................
-00002630: 0102 0002 fe06 040a 0222 011a 0214 0114  ........."......
-00002640: 0114 0102 0118 0106 011e 0102 0118 0106  ................
-00002650: 010e 0118 0212 0108 0116 0102 0002 0002  ................
-00002660: 0002 0002 0002 0002 0102 0002 fe06 040a  ................
-00002670: 0222 011a 0214 0114 0114 0102 0118 0106  ."..............
-00002680: 011e 0102 0118 0106 010e 0114 0208 0104  ................
-00002690: 0108 0112 0106 0402 0002 0002 0106 fb72  ...............r
-000026a0: 3901 0000 630f 0000 0000 0000 0000 0000  9...c...........
-000026b0: 0029 0000 0032 0000 0043 0000 0073 4e07  .)...2...C...sN.
-000026c0: 0000 7400 6a01 a002 7c0e a101 721a 7403  ..t.j...|...r.t.
-000026d0: a004 7c0e a101 7d0f 9001 6e3a 7400 6a01  ..|...}...n:t.j.
-000026e0: a005 7400 6a01 a006 7407 a101 a101 7d10  ..t.j...t.....}.
-000026f0: 7403 a004 7c10 6401 1700 a101 7d11 7408  t...|.d.....}.t.
-00002700: 7409 6a0a 6402 1700 8301 0100 740b 740c  t.j.d.......t.t.
-00002710: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
-00002720: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
+00001fc0: 2020 2020 2020 6465 6c74 6179 3d31 302c        deltay=10,
+00001fd0: 2073 6176 6566 6967 3d27 7965 7327 2c20   savefig='yes', 
+00001fe0: 6974 7363 6f6e 7369 6465 723d 2779 6573  itsconsider='yes
+00001ff0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00002000: 2020 2020 2020 2020 2020 2020 204e 6d65               Nme
+00002010: 6d62 6572 733d 7b7d 2929 4872 2500 0000  mbers={}))Hr%...
+00002020: da05 7768 6572 6572 b700 0000 da03 7461  ..wherer......ta
+00002030: 6eda 0764 6567 3272 6164 da05 7072 696e  n..deg2rad..prin
+00002040: 7472 1900 0000 da04 424c 5545 7264 0000  tr......BLUErd..
+00002050: 00da 0673 7175 6172 65da 0270 69da 0b63  ...square..pi..c
+00002060: 6865 636b 636f 6f72 6473 da04 6368 6172  heckcoords..char
+00002070: da0a 7374 6172 7473 7769 7468 da03 5245  ..startswith..RE
+00002080: 44da 0569 736e 616e da02 6f73 da04 7061  D..isnan..os..pa
+00002090: 7468 da06 6578 6973 7473 da07 6765 745f  th..exists..get_
+000020a0: 6375 74da 0369 6e74 7205 0000 00da 0472  cut..intr......r
+000020b0: 6561 64da 0373 7472 da05 7175 6572 79da  ead..str..query.
+000020c0: 0577 7269 7465 da05 424c 4143 4bda 0764  .write..BLACK..d
+000020d0: 6972 6e61 6d65 da08 7265 616c 7061 7468  irname..realpath
+000020e0: da08 5f5f 6669 6c65 5f5f da05 726f 756e  ..__file__..roun
+000020f0: 64da 096e 616e 6d65 6469 616e da03 6c65  d..nanmedian..le
+00002100: 6e72 0300 0000 da04 6f70 656e da04 6461  nr......open..da
+00002110: 7461 720a 0000 00da 0370 6c74 da06 6669  tar......plt..fi
+00002120: 6775 7265 da06 696d 7368 6f77 da07 7361  gure..imshow..sa
+00002130: 7665 6669 67da 0473 686f 77da 0563 6c6f  vefig..show..clo
+00002140: 7365 720b 0000 0072 0d00 0000 720c 0000  ser....r....r...
+00002150: 00da 0a62 6163 6b67 726f 756e 64da 0777  ...background..w
+00002160: 7269 7465 746f 7231 0000 00da 0473 7172  ritetor1.....sqr
+00002170: 7472 3300 0000 da05 6d67 7269 64da 0365  tr3.....mgrid..e
+00002180: 7870 da03 7375 6d72 1100 0000 7210 0000  xp..sumr....r...
+00002190: 00da 096e 6f72 6d61 6c69 7a65 da09 7068  ...normalize..ph
+000021a0: 6f74 7574 696c 73da 1064 6574 6563 745f  otutils..detect_
+000021b0: 7468 7265 7368 6f6c 6472 0e00 0000 720f  thresholdr....r.
+000021c0: 0000 00da 0474 696d 65da 0973 7461 746d  .....time..statm
+000021d0: 6f72 7068 da11 736f 7572 6365 5f6d 6f72  orph..source_mor
+000021e0: 7068 6f6c 6f67 79da 0769 7361 6c70 6861  phology..isalpha
+000021f0: da07 6172 6773 6f72 74da 0561 7265 6173  ..argsort..areas
+00002200: da09 656e 756d 6572 6174 65da 0970 6c6f  ..enumerate..plo
+00002210: 745f 7374 6174 7204 0000 00da 0763 5f73  t_statr......c_s
+00002220: 7065 6564 da06 6170 7065 6e64 294b 7241  peed..append)KrA
+00002230: 0000 00da 0774 6162 5f67 616c da04 636f  .....tab_gal..co
+00002240: 6e6e da0e 7369 7a65 5f69 6d61 6765 5f70  nn..size_image_p
+00002250: 6879 da05 736e 725f 67da 0761 7265 6167  hy..snr_g..areag
+00002260: 616c da0a 7573 6572 5f6f 7264 6572 da09  al..user_order..
+00002270: 7573 6572 5f6c 6973 74da 0773 6b79 5f62  user_list..sky_b
+00002280: 6f78 da07 6465 626c 656e 64da 0462 616e  ox..deblend..ban
+00002290: 6472 7100 0000 7272 0000 0072 7300 0000  drq...rr...rs...
+000022a0: 72c0 0000 0072 ae00 0000 72c1 0000 00da  r....r....r.....
+000022b0: 0369 6467 72b3 0000 00da 0761 7263 5f6b  .idgr......arc_k
+000022c0: 7063 da0a 7369 7a65 5f69 6d61 6765 da0a  pc..size_image..
+000022d0: 7261 6469 7573 5f63 6174 da08 6172 6561  radius_cat..area
+000022e0: 5f6d 696e da03 6f75 7472 d500 0000 da05  _min..outr......
+000022f0: 7061 7468 7472 6700 0000 da06 7061 7468  pathtrg.....path
+00002300: 7474 da08 7461 625f 6677 686d da0a 7175  tt..tab_fwhm..qu
+00002310: 6572 795f 7478 7431 da09 6469 7265 6362  ery_txt1..direcb
+00002320: 6173 65da 025a 50da 0569 645f 7a70 722d  ase..ZP..id_zpr-
+00002330: 0000 00da 0570 7366 5f67 da07 7363 5f69  .....psf_g..sc_i
+00002340: 6d61 6772 ac00 0000 da0c 6d65 6469 616e  magr......median
+00002350: 5f73 6b79 5f67 722b 0000 0072 2c00 0000  _sky_gr+...r,...
+00002360: da06 7061 7468 5f61 da05 696d 6167 6eda  ..path_a..imagn.
+00002370: 0469 6d61 67da 066d 6173 6b5f 67da 0366  .imag..mask_g..f
+00002380: 6967 da08 6d65 616e 5f73 6b79 da0a 6d65  ig..mean_sky..me
+00002390: 6469 616e 5f73 6b79 da07 7374 645f 736b  dian_sky..std_sk
+000023a0: 7972 8e00 0000 da03 626b 67da 0770 6174  yr......bkg..pat
+000023b0: 6867 616c da05 696d 6167 6dda 0766 6163  hgal..imagm..fac
+000023c0: 5f73 6967 da04 7369 7a65 da09 7369 676d  _sig..size..sigm
+000023d0: 615f 7073 66da 0179 da01 78da 0470 7366  a_psf..y..x..psf
+000023e0: 6772 8100 0000 da06 6b65 726e 656c da09  gr......kernel..
+000023f0: 6e70 6978 656c 735f 67da 0974 6872 6573  npixels_g..thres
+00002400: 686f 6c64 da04 7365 676d da05 7361 7665  hold..segm..save
+00002410: 6eda 0573 7461 7274 da0d 736f 7572 6365  n..start..source
+00002420: 5f6d 6f72 7068 73da 056c 6973 746c da05  _morphs..listl..
+00002430: 736f 7274 61da 0169 da04 6761 6c69 da05  sorta..i..gali..
+00002440: 6d6f 7270 6872 e500 0000 da03 696e 64da  morphr......ind.
+00002450: 0669 6e64 6761 6cda 0a6e 7573 6572 5f6c  .indgal..nuser_l
+00002460: 6973 7472 2f00 0000 722f 0000 0072 3000  istr/...r/...r0.
+00002470: 0000 da08 7068 6f74 5f6d 6f64 5300 0000  ....phot_modS...
+00002480: 731c 0200 0000 051a 0110 0118 010e 010e  s...............
+00002490: 0114 0110 0110 0114 011c 010c 0102 ff08  ................
+000024a0: 031c 0114 010e 010e 010e 010e 0104 020c  ................
+000024b0: 010e 010e 010e 0104 020e 0108 020c 010e  ................
+000024c0: 0126 0110 0126 0110 011e 0102 000a ff06  .&...&..........
+000024d0: 030e 0110 0218 0110 011e 0102 010a fe06  ................
+000024e0: 0408 0208 0114 0108 020c 0112 010a 012a  ...............*
+000024f0: 050e 010e 0110 010e 010e 0110 010e 010e  ................
+00002500: 0112 0202 0706 f902 0802 f802 0902 f704  ................
+00002510: 0a0a 010a 0316 020e 0108 0214 010e 0122  ..............."
+00002520: 010c 010e 0102 0006 ff04 0416 0116 010e  ................
+00002530: 0204 0104 0104 010a 0104 0218 010a 0102  ................
+00002540: 0106 010a ff02 0108 ff06 020a 0114 ff0c  ................
+00002550: 0206 010e 011c 020e 0114 010a 050e 0108  ................
+00002560: 0108 0108 0102 ff06 020c 010e 0114 0102  ................
+00002570: ff06 020a 010a 0208 0206 0102 ff0c 020e  ................
+00002580: 0108 010e 010e 010e 0306 0106 0006 ff06  ................
+00002590: 0208 0206 0108 0102 0002 0102 fe06 040a  ................
+000025a0: 020c 0110 0114 0102 ff06 020a 010a 0208  ................
+000025b0: 0216 011a 0118 0110 0310 0718 0104 0108  ................
+000025c0: 0126 0124 010e 0508 010e 0108 0308 010e  .&.$............
+000025d0: 010e 020a 0108 0108 0208 010c 010e 010a  ................
+000025e0: 010a 0208 0108 0202 0002 fe06 0608 0108  ................
+000025f0: 020c 0110 021a 010e 020a 010a 0208 040e  ................
+00002600: 0108 0208 0106 0104 0002 0002 0002 ff06  ................
+00002610: 0214 010c 0220 0208 0108 0320 010c 020a  ..... ..... ....
+00002620: 010c 011c 0208 011a 0102 0002 0002 0002  ................
+00002630: 0002 0102 0002 fe06 040a 0222 011a 0214  ..........."....
+00002640: 0114 0114 0102 0118 0106 011e 0102 0118  ................
+00002650: 0106 010e 0118 0212 0108 0116 0102 0002  ................
+00002660: 0002 0002 0002 0002 0002 0102 0002 fe06  ................
+00002670: 040a 0222 011a 0214 0114 0114 0102 0118  ..."............
+00002680: 0106 011e 0102 0118 0106 010e 0114 0208  ................
+00002690: 0104 0108 0112 0106 0402 0002 0002 0106  ................
+000026a0: fb72 3901 0000 630f 0000 0000 0000 0000  .r9...c.........
+000026b0: 0000 002a 0000 0032 0000 0043 0000 0073  ...*...2...C...s
+000026c0: 5e07 0000 7400 6a01 a002 7c0e a101 721a  ^...t.j...|...r.
+000026d0: 7403 a004 7c0e a101 7d0f 9001 6e38 7400  t...|...}...n8t.
+000026e0: 6a01 a005 7400 6a01 a006 7407 a101 a101  j...t.j...t.....
+000026f0: 7d10 7403 a004 7c10 6401 1700 a101 7d11  }.t...|.d.....}.
+00002700: 7408 7409 6a0a 6402 1700 8301 0100 740b  t.t.j.d.......t.
+00002710: 740c 6a0d 740c 6a0d 740c 6a0d 740c 6a0d  t.j.t.j.t.j.t.j.
+00002720: 740b 740c 6a0d 740c 6a0d 740c 6a0d 740c  t.t.j.t.j.t.j.t.
 00002730: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 00002740: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 00002750: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 00002760: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 00002770: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 00002780: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 00002790: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
@@ -636,2271 +636,2289 @@
 000027b0: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 000027c0: 6a0d 740c 6a0d 740c 6a0d 740c 6a0d 740c  j.t.j.t.j.t.j.t.
 000027d0: 6a0d 6732 7d12 740e 7c11 6a0f 7c12 6403  j.g2}.t.|.j.|.d.
 000027e0: 8d02 7d0f 7c0f a010 a100 0100 7c0f 6404  ..}.|.......|.d.
 000027f0: 1900 a011 6405 740b 7412 7c01 8301 8301  ....d.t.t.|.....
 00002800: 1700 a101 7c0f 6404 3c00 7c01 7c0f 6404  ....|.d.<.|.|.d.
 00002810: 1900 6406 3c00 7413 7c0f 6404 1900 7c01  ..d.<.t.|.d...|.
-00002820: 6b02 8301 9001 72a8 7408 7409 6a14 6407  k.....r.t.t.j.d.
+00002820: 6b02 8301 9001 72a6 7408 7409 6a14 6407  k.....r.t.t.j.d.
 00002830: 1700 8301 0100 7408 7c0f 6404 1900 7c0f  ......t.|.d...|.
 00002840: 6404 1900 7c01 6b02 1900 8301 0100 740c  d...|.k.......t.
 00002850: a015 7c0f 6404 1900 7c01 6b02 a101 6406  ..|.d...|.k...d.
-00002860: 1900 6406 1900 7d13 6e74 7408 7409 6a14  ..d...}.ntt.t.j.
+00002860: 1900 6406 1900 7d13 6e86 7408 7409 6a14  ..d...}.n.t.t.j.
 00002870: 6408 a016 7c01 a101 1700 8301 0100 7c0f  d...|.........|.
-00002880: a010 a100 0100 6409 7d13 7412 7c01 8301  ......d.}.t.|...
-00002890: 7412 7c0f 6404 1900 6406 1900 8301 6b04  t.|.d...d.....k.
-000028a0: 9002 7210 7408 640a 8301 0100 7c0f 6404  ..r.t.d.....|.d.
-000028b0: 1900 a011 6405 740b 7412 7c01 8301 8301  ....d.t.t.|.....
-000028c0: 1700 a101 7d14 7c0f a017 6404 7c14 a102  ....}.|...d.|...
-000028d0: 0100 7c01 7c0f 6404 1900 7c13 3c00 7408  ..|.|.d...|.<.t.
-000028e0: 640b a016 7c00 6a18 a101 8301 0100 7408  d...|.j.......t.
-000028f0: 640c a016 7c00 6a19 a101 8301 0100 7408  d...|.j.......t.
-00002900: 640d 7c00 6a1a 8302 0100 7408 640e 7c00  d.|.j.....t.d.|.
-00002910: 6a1b 8302 0100 7408 640f 8301 0100 7c00  j.....t.d.....|.
-00002920: 6a1c 7c0f 6410 1900 7c13 3c00 7c00 6a1d  j.|.d...|.<.|.j.
-00002930: 7c0f 6411 1900 7c13 3c00 7c00 6a1e 7c0f  |.d...|.<.|.j.|.
-00002940: 6412 1900 7c13 3c00 7c00 6a1f 7c0f 6413  d...|.<.|.j.|.d.
-00002950: 1900 7c13 3c00 7c00 6a20 7c0f 6414 1900  ..|.<.|.j |.d...
-00002960: 7c13 3c00 7c00 6a21 7c0f 6415 1900 7c13  |.<.|.j!|.d...|.
-00002970: 3c00 7c00 6a22 7c0f 6416 1900 7c13 3c00  <.|.j"|.d...|.<.
-00002980: 7c00 6a23 7c0f 6417 1900 7c13 3c00 7c00  |.j#|.d...|.<.|.
-00002990: 6a24 7c0f 6418 1900 7c13 3c00 7c00 6a25  j$|.d...|.<.|.j%
-000029a0: 7c0f 6419 1900 7c13 3c00 7c00 6a26 7c0f  |.d...|.<.|.j&|.
-000029b0: 641a 1900 7c13 3c00 7c00 6a27 7c0f 641b  d...|.<.|.j'|.d.
-000029c0: 1900 7c13 3c00 7c00 6a28 7c0f 641c 1900  ..|.<.|.j(|.d...
-000029d0: 7c13 3c00 7c00 6a29 7c0f 641d 1900 7c13  |.<.|.j)|.d...|.
-000029e0: 3c00 7c00 6a2a 7c0f 641e 1900 7c13 3c00  <.|.j*|.d...|.<.
-000029f0: 7c00 6a2b 7c0f 641f 1900 7c13 3c00 7c00  |.j+|.d...|.<.|.
-00002a00: 6a2c 7c0f 6420 1900 7c13 3c00 7408 7409  j,|.d ..|.<.t.t.
-00002a10: 6a0a 6421 a016 7c00 6a29 a101 1700 8301  j.d!..|.j)......
-00002a20: 0100 7c00 6a2d 7c0f 6422 1900 7c13 3c00  ..|.j-|.d"..|.<.
-00002a30: 7c00 6a2e 7c0f 6423 1900 7c13 3c00 7c00  |.j.|.d#..|.<.|.
-00002a40: 6a2f 7c0f 6424 1900 7c13 3c00 7c00 6a30  j/|.d$..|.<.|.j0
-00002a50: 7c0f 6425 1900 7c13 3c00 7c00 6a31 7c0f  |.d%..|.<.|.j1|.
-00002a60: 6426 1900 7c13 3c00 7c00 6a32 7c0f 6427  d&..|.<.|.j2|.d'
-00002a70: 1900 7c13 3c00 7c00 6a33 7c0f 6428 1900  ..|.<.|.j3|.d(..
-00002a80: 7c13 3c00 7c00 6a34 7c0f 6429 1900 7c13  |.<.|.j4|.d)..|.
-00002a90: 3c00 7c00 6a35 7c0f 642a 1900 7c13 3c00  <.|.j5|.d*..|.<.
-00002aa0: 7c00 6a36 7c0f 642b 1900 7c13 3c00 7c00  |.j6|.d+..|.<.|.
-00002ab0: 6a37 7c0f 642c 1900 7c13 3c00 7c00 6a38  j7|.d,..|.<.|.j8
-00002ac0: 7c0f 642d 1900 7c13 3c00 7c00 6a1a 7c0f  |.d-..|.<.|.j.|.
-00002ad0: 642e 1900 7c13 3c00 7c00 6a1b 7c0f 642f  d...|.<.|.j.|.d/
-00002ae0: 1900 7c13 3c00 7c09 7c0f 6430 1900 7c13  ..|.<.|.|.d0..|.
-00002af0: 3c00 7c0c 7c0f 6431 1900 7c13 3c00 7403  <.|.|.d1..|.<.t.
-00002b00: 6a39 7c0f 7c0e 6432 6433 8d03 0100 7c02  j9|.|.d2d3....|.
-00002b10: 6a3a 5c02 7d15 7d16 740c 6a3b 6406 7c15  j:\.}.}.t.j;d.|.
-00002b20: 8502 6406 7c16 8502 6602 1900 5c02 7d17  ..d.|...f...\.}.
-00002b30: 7d18 743c 6a3d 7c00 6a32 7c00 6a33 7c00  }.t<j=|.j2|.j3|.
-00002b40: 6a34 7c00 6a35 7c00 6a36 7c00 6a37 7c00  j4|.j5|.j6|.j7|.
-00002b50: 6a38 6434 8d07 7d19 7c19 a03e 7c08 a101  j8d4..}.|..>|...
-00002b60: 0100 7c19 7c18 7c17 8302 7d1a 743f 6a40  ..|.|.|...}.t?j@
-00002b70: 6435 6436 8d01 7d1b 6406 6437 6c41 6d42  d5d6..}.d.d7lAmB
-00002b80: 7d1c 0100 7c1c 7c1b 6438 6439 643a 643b  }...|.|.d8d9d:d;
-00002b90: 643c 643d 643e 643f 8d08 7d1d 7c1d 6406  d<d=d>d?..}.|.d.
-00002ba0: 1900 7d1e 740c a043 7c03 a101 7d1f 7c1f  ..}.t..C|...}.|.
-00002bb0: 740c a044 7c1f a101 0f00 1900 7d1f 740c  t..D|.......}.t.
-00002bc0: a045 7c1f 6440 a102 7d20 740c a045 7c1f  .E|.d@..} t..E|.
-00002bd0: 6441 a102 7d21 7446 6a47 7c03 6a3a 6440  dA..}!tFjG|.j:d@
-00002be0: 1900 6442 1b00 7c02 6a3a 6406 1900 6442  ..dB..|.j:d...dB
-00002bf0: 1b00 6702 7c0a 6443 7c0b 1b00 6444 6445  ..g.|.dC|...dDdE
-00002c00: 6443 6446 6447 6448 6449 644a 6442 7c1e  dCdFdGdHdIdJdB|.
-00002c10: 644b 644c 8d0e 0100 7446 6a40 7c03 6406  dKdL....tFj@|.d.
-00002c20: 6406 6702 6406 6406 6702 7c20 7c21 6406  d.g.d.d.g.| |!d.
-00002c30: 6703 7448 7c0a 6406 644d 644e 644f 6702  g.tH|.d.dMdNdOg.
-00002c40: 7c1e 6450 8d0a 0100 7c1d 6440 1900 7d22  |.dP....|.d@..}"
-00002c50: 7449 7c1a 7c04 7c05 7c06 7c07 8305 7d23  tI|.|.|.|.|...}#
-00002c60: 743f 6a4a 7c22 a04b a100 6451 6452 8d02  t?jJ|".K..dQdR..
-00002c70: 0100 7446 6a47 7c23 6a3a 6440 1900 6442  ..tFjG|#j:d@..dB
-00002c80: 1b00 7c23 6a3a 6406 1900 6442 1b00 6702  ..|#j:d...dB..g.
-00002c90: 7c0a 6443 7c0b 1b00 6444 6445 6443 6446  |.dC|...dDdEdCdF
-00002ca0: 6447 6448 6449 644a 6442 7c22 644b 644c  dGdHdIdJdB|"dKdL
-00002cb0: 8d0e 0100 7446 6a40 7c23 6406 6406 6702  ....tFj@|#d.d.g.
-00002cc0: 6406 6406 6702 7c20 7c21 6406 6703 7448  d.d.g.| |!d.g.tH
-00002cd0: 7c0a 644d 644e 644f 6702 7c22 6453 8d09  |.dMdNdOg.|"dS..
-00002ce0: 0100 7c1d 6442 1900 7d24 7c02 7c1a 1800  ..|.dB..}$|.|...
-00002cf0: 7d25 7449 7c25 7c04 7c05 7c06 7c07 8305  }%tI|%|.|.|.|...
-00002d00: 7d26 743f 6a4a 7c24 a04b a100 6451 6452  }&t?jJ|$.K..dQdR
-00002d10: 8d02 0100 7446 6a47 7c26 6a3a 6440 1900  ....tFjG|&j:d@..
-00002d20: 6442 1b00 7c26 6a3a 6406 1900 6442 1b00  dB..|&j:d...dB..
-00002d30: 6702 7c0a 6443 7c0b 1b00 6444 6445 6443  g.|.dC|...dDdEdC
-00002d40: 6446 6447 6448 6449 644a 6442 7c24 644b  dFdGdHdIdJdB|$dK
-00002d50: 644c 8d0e 0100 7446 6a40 7c26 6406 6406  dL....tFj@|&d.d.
-00002d60: 6702 6406 6406 6702 7c20 7c21 6406 6703  g.d.d.g.| |!d.g.
-00002d70: 7448 7c0a 6406 644d 644e 644f 6702 7c24  tH|.d.dMdNdOg.|$
-00002d80: 6450 8d0a 7d27 743f 6a4c 7c27 6454 6455  dP..}'t?jL|'dTdU
-00002d90: 7c1d 6a4d 6406 1900 6456 8d04 7d28 7c28  |.jMd...dV..}(|(
-00002da0: 6a4e a04f a100 0100 743f 6a50 6457 7c01  jN.O....t?jPdW|.
-00002db0: 1700 6458 a016 7c0c a101 1700 6459 645a  ..dX..|.....dYdZ
-00002dc0: 8d02 0100 7c0d 645b 6b03 9007 7214 743f  ....|.d[k...r.t?
-00002dd0: a051 a100 0100 7452 7c00 8301 7d1b 743f  .Q....tR|...}.t?
-00002de0: 6a50 6457 7c01 1700 645c a016 7c0c a101  jPdW|...d\..|...
-00002df0: 1700 6459 645a 8d02 0100 7c0d 645b 6b03  ..dYdZ....|.d[k.
-00002e00: 9007 724a 743f a051 a100 0100 6400 5300  ..rJt?.Q....d.S.
-00002e10: 295d 4e7a 0f2f 7072 6f70 6572 7469 6573  )]Nz./properties
-00002e20: 2e64 6174 7a3e 0a2a 4974 2077 6173 2063  .datz>.*It was c
-00002e30: 7265 6174 6520 7468 6520 7072 6f70 6572  reate the proper
-00002e40: 7469 6573 2e64 6174 2074 6f20 7072 696e  ties.dat to prin
-00002e50: 7420 7468 6520 6f75 7420 7061 7261 6d65  t the out parame
-00002e60: 7465 7273 2902 da05 6e61 6d65 73da 0564  ters)...names..d
-00002e70: 7479 7065 72c2 0000 00da 0155 7201 0000  typer......Ur...
-00002e80: 007a 100a 526f 7720 7761 7320 7570 6461  .z..Row was upda
-00002e90: 7465 647a 170a 526f 7720 7761 7320 6372  tedz..Row was cr
-00002ea0: 6561 7465 6420 666f 7220 7b7d 7262 0000  eated for {}rb..
-00002eb0: 007a 2643 6861 6e67 6520 7468 6520 7374  .z&Change the st
-00002ec0: 7269 6e67 2066 6f72 6d61 7420 6f66 2047  ring format of G
-00002ed0: 414c 2063 6f6c 756d 6e7a 1b0a 736b 795f  AL columnz..sky_
-00002ee0: 6d65 616e 5f73 7461 746d 6f72 7068 203d  mean_statmorph =
-00002ef0: 7b3a 2e33 667d 7a1b 736b 795f 7369 676d  {:.3f}z.sky_sigm
-00002f00: 615f 7374 6174 6d6f 7270 6820 3d7b 3a2e  a_statmorph ={:.
-00002f10: 3366 7d7a 0666 6c61 6720 3d7a 0d66 6c61  3f}z.flag =z.fla
-00002f20: 675f 7365 7273 6963 203d 72c7 0000 00da  g_sersic =r.....
-00002f30: 0372 3230 da03 7238 30da 0447 696e 69da  .r20..r80..Gini.
-00002f40: 034d 3230 7a08 4628 475f 4d32 3029 7a08  .M20z.F(G_M20)z.
-00002f50: 5328 475f 4d32 3029 da03 535f 4e72 b200  S(G_M20)..S_Nr..
-00002f60: 0000 72b0 0000 00da 0153 da03 7235 30da  ..r......S..r50.
-00002f70: 0666 6c75 785f 63da 0666 6c75 785f 65da  .flux_c..flux_e.
-00002f80: 0872 7065 7472 6f5f 63da 0872 7065 7472  .rpetro_c..rpetr
-00002f90: 6f5f 65da 0772 6861 6c66 5f63 da07 7268  o_e..rhalf_c..rh
-00002fa0: 616c 665f 657a 190a 2050 6574 726f 7369  alf_ez.. Petrosi
-00002fb0: 616e 2052 6164 6975 7320 7b3a 2e31 667d  an Radius {:.1f}
-00002fc0: 72bb 0000 0072 3400 0000 72b3 0000 00da  r....r4...r.....
-00002fd0: 0241 6fda 0241 73da 0553 6572 5f41 da05  .Ao..As..Ser_A..
-00002fe0: 5365 725f 52da 0553 6572 5f6e da06 5365  Ser_R..Ser_n..Se
-00002ff0: 725f 7863 da06 5365 725f 7963 da09 5365  r_xc..Ser_yc..Se
-00003000: 725f 656c 6c69 70da 0953 6572 5f74 6865  r_ellip..Ser_the
-00003010: 7461 da0a 666c 6167 5f6d 6f72 7068 da0b  ta..flag_morph..
-00003020: 666c 6167 5f73 6572 7369 63da 0570 7366  flag_sersic..psf
-00003030: 5f52 da05 7369 7a65 7054 7292 0000 0029  _R..sizepTr....)
-00003040: 07da 0961 6d70 6c69 7475 6465 da05 725f  ...amplitude..r_
-00003050: 6566 66da 016e da03 785f 30da 0379 5f30  eff..n..x_0..y_0
-00003060: da05 656c 6c69 70da 0574 6865 7461 2902  ..ellip..theta).
-00003070: e90f 0000 0072 3d00 0000 7276 0000 0029  .....r=...rv...)
-00003080: 01da 0949 6d61 6765 4772 6964 e96f 0000  ...ImageGrid.o..
-00003090: 0029 0272 6900 0000 728b 0000 0067 6666  .).ri...r....gff
-000030a0: 6666 6666 d63f da05 7269 6768 74da 0673  ffff.?..right..s
-000030b0: 696e 676c 657a 0235 2567 9a99 9999 9999  inglez.5%g......
-000030c0: a93f 2906 da0b 6e72 6f77 735f 6e63 6f6c  .?)...nrows_ncol
-000030d0: 73da 0861 7865 735f 7061 64da 0d63 6261  s..axes_pad..cba
-000030e0: 725f 6c6f 6361 7469 6f6e da09 6362 6172  r_location..cbar
-000030f0: 5f6d 6f64 65da 0963 6261 725f 7369 7a65  _mode..cbar_size
-00003100: da08 6362 6172 5f70 6164 7269 0000 00e9  ..cbar_padri....
-00003110: 5a00 0000 7239 0000 0072 3d00 0000 7a05  Z...r9...r=...z.
-00003120: 3520 6b70 63da 0131 7232 0000 0072 4900  5 kpc..1r2...rI.
-00003130: 0000 67cd cccc cccc ccf4 3f7a 026b 2dda  ..g.......?z.k-.
-00003140: 016b 7297 0000 0029 0ada 0470 6172 72da  .kr....)...parr.
-00003150: 066c 6172 726f 77da 026e 78da 026e 79da  .larrow..nx..ny.
-00003160: 0670 6f73 7478 74da 0463 6261 72da 0463  .postxt..cbar..c
-00003170: 7465 78da 056c 696e 6577 da02 4158 da07  tex..linew..AX..
-00003180: 6261 7274 6578 73da 046e 6f6e 65fa 1724  bartexs..none..$
-00003190: 5c44 656c 7461 5c64 656c 7461 2420 2861  \Delta\delta$ (a
-000031a0: 7263 7365 6329 fa18 245c 4465 6c74 6120  rcsec)..$\Delta 
-000031b0: 5c61 6c70 6861 2420 2861 7263 7365 6329  \alpha$ (arcsec)
-000031c0: 2909 da04 6365 6e74 da05 6465 6c74 61da  )...cent..delta.
-000031d0: 046c 696d 7472 a800 0000 da05 7363 616c  .limtr......scal
-000031e0: 65da 0763 6261 726f 7074 da06 6f75 7469  e..cbaropt..outi
-000031f0: 6d61 da08 6e61 6d65 6178 6973 7274 0100  ma..nameaxisrt..
-00003200: 0046 2901 da07 7669 7369 626c 6529 0872  .F)...visible).r
-00003210: 7901 0000 727a 0100 0072 7b01 0000 72a8  y...rz...r{...r.
-00003220: 0000 0072 7c01 0000 727e 0100 0072 7f01  ...r|...r~...r..
-00003230: 0000 7274 0100 007a 0425 2e31 667a 1224  ..rt...z.%.1fz.$
-00003240: 6d61 675c 2c61 7263 7365 635e 7b2d 327d  mag\,arcsec^{-2}
-00003250: 2429 0372 6400 0000 da05 6c61 6265 6cda  $).rd.....label.
-00003260: 0363 6178 727b 0000 007a 105f 7b7d 6b70  .caxr{...z._{}kp
-00003270: 635f 6d6f 6465 6c2e 706e 6772 7c00 0000  c_model.pngr|...
-00003280: 727d 0000 0072 4000 0000 7a0f 5f7b 7d6b  r}...r@...z._{}k
-00003290: 7063 5f73 7461 742e 706e 6729 5372 d400  pc_stat.png)Sr..
-000032a0: 0000 72d5 0000 0072 d600 0000 7204 0000  ..r....r....r...
-000032b0: 0072 d900 0000 72de 0000 0072 df00 0000  .r....r....r....
-000032c0: 72e0 0000 0072 cb00 0000 7219 0000 0072  r....r....r....r
-000032d0: d200 0000 72da 0000 0072 2500 0000 da07  ....r....r%.....
-000032e0: 666c 6f61 7436 3472 0500 0000 da08 636f  float64r......co
-000032f0: 6c6e 616d 6573 da07 6164 645f 726f 77da  lnames..add_row.
-00003300: 0661 7374 7970 6572 e300 0000 da03 616e  .astyper......an
-00003310: 7972 dd00 0000 72c8 0000 0072 6400 0000  yr....r....rd...
-00003320: da0e 7265 706c 6163 655f 636f 6c75 6d6e  ..replace_column
-00003330: da08 736b 795f 6d65 616e da09 736b 795f  ..sky_mean..sky_
-00003340: 7369 676d 61da 0466 6c61 6772 5401 0000  sigma..flagrT...
-00003350: 723d 0100 0072 3e01 0000 da04 6769 6e69  r=...r>.....gini
-00003360: da03 6d32 30da 0e67 696e 695f 6d32 305f  ..m20..gini_m20_
-00003370: 6275 6c67 65da 0f67 696e 695f 6d32 305f  bulge..gini_m20_
-00003380: 6d65 7267 6572 da0c 736e 5f70 6572 5f70  merger..sn_per_p
-00003390: 6978 656c da0d 636f 6e63 656e 7472 6174  ixel..concentrat
-000033a0: 696f 6eda 0961 7379 6d6d 6574 7279 da0a  ion..asymmetry..
-000033b0: 736d 6f6f 7468 6e65 7373 7243 0100 00da  smoothnessrC....
-000033c0: 0966 6c75 785f 6369 7263 da0a 666c 7578  .flux_circ..flux
-000033d0: 5f65 6c6c 6970 da0b 7270 6574 726f 5f63  _ellip..rpetro_c
-000033e0: 6972 63da 0c72 7065 7472 6f5f 656c 6c69  irc..rpetro_elli
-000033f0: 70da 0a72 6861 6c66 5f63 6972 63da 0b72  p..rhalf_circ..r
-00003400: 6861 6c66 5f65 6c6c 6970 da09 6d75 6c74  half_ellip..mult
-00003410: 696d 6f64 65da 0969 6e74 656e 7369 7479  imode..intensity
-00003420: da09 6465 7669 6174 696f 6eda 0f6f 7574  ..deviation..out
-00003430: 6572 5f61 7379 6d6d 6574 7279 da0f 7368  er_asymmetry..sh
-00003440: 6170 655f 6173 796d 6d65 7472 79da 1073  ape_asymmetry..s
-00003450: 6572 7369 635f 616d 706c 6974 7564 65da  ersic_amplitude.
-00003460: 0c73 6572 7369 635f 7268 616c 66da 0873  .sersic_rhalf..s
-00003470: 6572 7369 635f 6eda 0973 6572 7369 635f  ersic_n..sersic_
-00003480: 7863 da09 7365 7273 6963 5f79 63da 0c73  xc..sersic_yc..s
-00003490: 6572 7369 635f 656c 6c69 70da 0c73 6572  ersic_ellip..ser
-000034a0: 7369 635f 7468 6574 6172 dc00 0000 da05  sic_thetar......
-000034b0: 7368 6170 6572 ef00 0000 72f6 0000 00da  shaper....r.....
-000034c0: 1143 6f6e 766f 6c76 6564 5365 7273 6963  .ConvolvedSersic
-000034d0: 3244 da07 7365 745f 7073 6672 e600 0000  2D..set_psfr....
-000034e0: 72e7 0000 00da 176d 706c 5f74 6f6f 6c6b  r......mpl_toolk
-000034f0: 6974 732e 6178 6573 5f67 7269 6431 725f  its.axes_grid1r_
-00003500: 0100 0072 2600 0000 72d3 0000 00da 0a70  ...r&...r......p
-00003510: 6572 6365 6e74 696c 65da 0570 6675 6e63  ercentile..pfunc
-00003520: da03 6261 72da 0863 6f6c 6f72 6d61 7072  ..bar..colormapr
-00003530: 3100 0000 da04 7365 7470 da0f 6765 745f  1.....setp..get_
-00003540: 7974 6963 6b6c 6162 656c 73da 0863 6f6c  yticklabels..col
-00003550: 6f72 6261 72da 0963 6261 725f 6178 6573  orbar..cbar_axes
-00003560: da02 6178 da0c 696e 7665 7274 5f79 6178  ..ax..invert_yax
-00003570: 6973 72e9 0000 0072 eb00 0000 7202 0000  isr....r....r...
-00003580: 0029 2972 3501 0000 7241 0000 0072 1b01  .))r5...rA...r..
-00003590: 0000 7223 0100 0072 1801 0000 722b 0000  ..r#...r....r+..
-000035a0: 0072 2c00 0000 722d 0000 0072 2901 0000  .r,...r-...r)...
-000035b0: 7216 0100 00da 0673 635f 696d 6172 0a01  r......sc_imar..
-000035c0: 0000 7201 0100 0072 c100 0000 72c0 0000  ..r....r....r...
-000035d0: 0072 e500 0000 7213 0100 00da 0564 6174  .r....r......dat
-000035e0: 6174 da06 756e 6974 7374 7236 0100 00da  at..unitstr6....
-000035f0: 056e 6577 5f63 726f 0100 0072 6e01 0000  .new_cro...rn...
-00003600: 7227 0100 0072 2801 0000 da0c 6669 7474  r'...r(.....fitt
-00003610: 6564 5f6d 6f64 656c da0c 696d 6167 655f  ed_model..image_
-00003620: 6d6f 6465 6c67 721d 0100 0072 5f01 0000  modelgr....r_...
-00003630: da04 6772 6964 72b2 0100 00da 0669 6d61  ..gridr......ima
-00003640: 675f 63da 0869 6d61 675f 6d69 6eda 0869  g_c..imag_min..i
-00003650: 6d61 675f 6d61 78da 0361 7831 da0d 696d  mag_max..ax1..im
-00003660: 6167 655f 6d6f 6465 6c6d 67da 0361 7832  age_modelmg..ax2
-00003670: da09 7265 7369 6475 616c 67da 0a72 6573  ..residualg..res
-00003680: 6964 7561 6c67 6dda 0269 6dda 0263 6272  idualgm..im..cbr
-00003690: 2f00 0000 722f 0000 0072 3000 0000 72fc  /...r/...r0...r.
-000036a0: 0000 00bc 0100 0073 ba01 0000 0004 0c01  .......s........
-000036b0: 0e02 1401 0e01 0e02 1601 0400 0400 0400  ................
-000036c0: 0400 0401 0400 0400 0400 0400 0401 0400  ................
-000036d0: 0400 0400 0400 0401 0400 0400 0400 0400  ................
-000036e0: 0401 0400 0400 0400 0400 0401 0400 0400  ................
-000036f0: 0400 0400 0401 0400 0400 0400 0400 0401  ................
-00003700: 0400 0400 0400 0400 0401 0400 0400 0400  ................
-00003710: 04f7 040a 0e01 0801 1e01 0c02 1201 0e01  ................
-00003720: 1801 1c03 1401 0801 0401 1a01 0802 1a01  ................
-00003730: 0c01 0c02 1001 1001 0c01 0c01 0802 0e01  ................
-00003740: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
-00003750: 0e02 0e02 0e01 0e01 0e01 0e01 0e01 0e02  ................
-00003760: 1602 0e01 0e01 0e01 0e01 0e02 0e01 0e01  ................
-00003770: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0c01  ................
-00003780: 0c02 1002 0a01 1a01 0401 0401 0401 0401  ................
-00003790: 0401 0401 0401 04f9 0608 0a01 0a02 0c02  ................
-000037a0: 0c01 0601 0201 0201 0201 0201 0201 02fa  ................
-000037b0: 060a 0802 0a01 1002 0c01 0c03 2801 0200  ............(...
-000037c0: 0200 0200 0201 0200 0200 0200 0200 0200  ................
-000037d0: 02fe 0604 1a01 0200 0200 0200 0201 0601  ................
-000037e0: 02fd 0605 0801 1002 1202 2001 0600 0200  .......... .....
-000037f0: 0200 0200 0200 0201 0200 0200 0200 0200  ................
-00003800: 0200 02fe 0604 1201 0800 0200 0201 0201  ................
-00003810: 0601 02fc 0608 0801 0802 1002 1202 2601  ..............&.
-00003820: 0200 0200 0200 0200 0201 0200 0200 0200  ................
-00003830: 0200 0200 02fe 0604 1201 0801 0200 0200  ................
-00003840: 0200 0201 0601 02fc 0606 0a01 08ff 0602  ................
-00003850: 0a02 1401 02ff 0602 0a01 0802 0801 1401  ................
-00003860: 02ff 0602 0a01 72fc 0000 00da 0663 6972  ......r......cir
-00003870: 636c 65e9 f401 0000 e90a 0000 0072 9700  cle..........r..
-00003880: 0000 7269 0000 00da 026e 6f63 1900 0000  ..ri.....noc....
-00003890: 0000 0000 0000 0000 4700 0000 1300 0000  ........G.......
-000038a0: 4300 0000 733a 0e00 0074 00a0 017c 0164  C...s:...t...|.d
-000038b0: 0119 007c 006b 02a1 0164 0219 0064 0219  ...|.k...d...d..
-000038c0: 007d 197c 0164 0319 007c 1919 0074 021b  .}.|.d...|...t..
-000038d0: 007d 1a74 00a0 0374 00a0 0464 04a1 01a1  .}.t...t...d....
-000038e0: 017c 1a14 0064 0514 007d 1b74 0574 066a  .|...d...}.t.t.j
-000038f0: 0764 0617 0083 0101 0074 0564 0783 0101  .d.......t.d....
-00003900: 0074 086a 09a0 0a74 086a 09a0 0b74 0ca1  .t.j...t.j...t..
-00003910: 01a1 017d 1c74 0d6a 0e7c 1c64 0817 0064  ...}.t.j.|.d...d
-00003920: 0964 0a8d 027d 1d74 057c 1d64 0b19 0074  .d...}.t.|.d...t
-00003930: 00a0 017c 1d64 0119 007c 006b 02a1 0164  ...|.d...|.k...d
-00003940: 0219 0019 0083 0101 0074 057c 1d64 0c19  .........t.|.d..
-00003950: 0074 00a0 017c 1d64 0119 007c 006b 02a1  .t...|.d...|.k..
-00003960: 0164 0219 0019 0083 0101 0074 0574 066a  .d.........t.t.j
-00003970: 0f64 0d17 0083 0101 0074 0574 066a 0f64  .d.......t.t.j.d
-00003980: 0e17 0083 0101 0074 0574 066a 0f64 0fa0  .......t.t.j.d..
-00003990: 107c 1aa1 0117 0083 0101 0074 0574 066a  .|.........t.t.j
-000039a0: 0f64 10a0 107c 1ba1 0117 0083 0101 007c  .d...|.........|
-000039b0: 037c 1b1b 0064 111b 0064 1214 007d 1e7c  .|...d...d...}.|
-000039c0: 1e64 1314 0064 1114 0064 141b 007d 1f74  .d...d...d...}.t
-000039d0: 0574 066a 0f64 15a0 107c 1ea1 0117 0083  .t.j.d...|......
-000039e0: 0101 0074 00a0 117c 05a1 0174 006a 1214  ...t...|...t.j..
-000039f0: 007c 1b64 1213 001b 0064 161b 007d 2074  .|.d.....d...} t
-00003a00: 0574 066a 0f64 17a0 107c 057c 20a1 0217  .t.j.d...|.| ...
-00003a10: 0083 0101 007c 02a0 137c 0164 1819 007c  .....|...|.d...|
-00003a20: 1919 007c 0164 1919 007c 1919 00a1 027d  ...|.d...|.....}
-00003a30: 2174 006a 14a0 157c 2164 1a19 0064 1ba1  !t.j...|!d...d..
-00003a40: 0290 0172 d874 0574 066a 0764 1c17 0083  ...r.t.t.j.d....
-00003a50: 0101 0074 0574 066a 0764 1d17 0083 0101  ...t.t.j.d......
-00003a60: 0074 0574 066a 0764 1e17 0083 0101 0074  .t.t.j.d.......t
-00003a70: 0574 066a 0764 1f17 0083 0101 0064 0053  .t.j.d.......d.S
-00003a80: 0074 00a0 167c 1ea1 0190 0272 1274 0574  .t...|.....r.t.t
-00003a90: 066a 0764 1c17 0083 0101 0074 0574 066a  .j.d.......t.t.j
-00003aa0: 0764 2017 0083 0101 0074 0574 066a 0764  .d ......t.t.j.d
-00003ab0: 1f17 0083 0101 0064 0053 007c 1164 216b  .......d.S.|.d!k
-00003ac0: 0290 0272 b464 227c 0164 0119 007c 1919  ...r.d"|.d...|..
-00003ad0: 0017 0064 2317 007d 2264 227c 0164 0119  ...d#..}"d"|.d..
-00003ae0: 007c 1919 0064 0064 2485 0219 0017 0064  .|...d.d$......d
-00003af0: 2317 007d 2374 086a 09a0 177c 22a1 0190  #..}#t.j...|"...
-00003b00: 0273 6874 086a 09a0 177c 23a1 0190 0272  .sht.j...|#....r
-00003b10: 8674 0574 066a 0764 1c17 0083 0101 0074  .t.t.j.d.......t
-00003b20: 0574 066a 0764 2517 0083 0101 006e 2e74  .t.j.d%......n.t
-00003b30: 0574 066a 0764 1c17 0083 0101 0074 0574  .t.j.d.......t.t
-00003b40: 066a 0764 2617 0083 0101 0074 0574 066a  .j.d&......t.t.j
-00003b50: 0764 1f17 0083 0101 0064 0053 0074 086a  .d.......d.S.t.j
-00003b60: 09a0 1764 27a1 0190 0273 da74 08a0 1864  ...d'....s.t...d
-00003b70: 28a1 0101 0074 0574 066a 0764 2917 0083  (....t.t.j.d)...
-00003b80: 0101 0074 086a 09a0 1764 2aa1 0190 0373  ...t.j...d*....s
-00003b90: 0074 08a0 1864 2ba1 0101 0074 0574 066a  .t...d+....t.t.j
-00003ba0: 0764 2c17 0083 0101 0074 0564 2d83 0101  .d,......t.d-...
-00003bb0: 007c 117d 247c 037c 246b 0090 0372 1c64  .|.}$|.|$k...r.d
-00003bc0: 217d 246e 047c 037d 2474 0574 066a 1964  !}$n.|.}$t.t.j.d
-00003bd0: 2d17 0083 0101 007c 1764 2e6b 0290 0372  -......|.d.k...r
-00003be0: 4c74 1a7c 007c 017c 247c 067c 087c 0764  Lt.|.|.|$|.|.|.d
-00003bf0: 2f8d 067d 2574 0574 066a 1964 3017 0083  /..}%t.t.j.d0...
-00003c00: 0101 0074 0564 3183 0101 0064 32a0 107c  ...t.d1....d2..|
-00003c10: 007c 03a1 027d 2264 33a0 107c 007c 107c  .|...}"d3..|.|.|
-00003c20: 03a1 037d 2374 086a 09a0 177c 22a1 0190  ...}#t.j...|"...
-00003c30: 0373 a274 086a 09a0 177c 23a1 0190 0372  .s.t.j...|#....r
-00003c40: b27c 1064 346b 0290 0372 b274 0564 357c  .|.d4k...r.t.d5|
-00003c50: 229b 0064 369d 0383 0101 0074 086a 09a0  "..d6......t.j..
-00003c60: 177c 22a1 0190 0473 1874 086a 09a0 177c  .|"....s.t.j...|
-00003c70: 23a1 0190 0473 187c 1064 346b 0290 0472  #....s.|.d4k...r
-00003c80: 1874 0564 377c 229b 0064 389d 0383 0101  .t.d7|"..d8.....
-00003c90: 007c 026a 1b7c 0164 1819 007c 1919 007c  .|.j.|.d...|...|
-00003ca0: 0164 1919 007c 1919 0074 1c7c 1e83 017c  .d...|...t.|...|
-00003cb0: 107c 2264 0264 3985 0219 0064 3a8d 0501  .|"d.d9....d:...
-00003cc0: 0074 086a 09a0 177c 23a1 0190 0472 3674  .t.j...|#....r6t
-00003cd0: 0564 357c 239b 0064 369d 0383 0101 0074  .d5|#..d6......t
-00003ce0: 086a 09a0 177c 23a1 0190 0473 8e7c 1064  .j...|#....s.|.d
-00003cf0: 346b 0390 0472 8e74 0564 377c 239b 0064  4k...r.t.d7|#..d
-00003d00: 389d 0383 0101 007c 026a 1b7c 0164 1819  8......|.j.|.d..
-00003d10: 007c 1919 007c 0164 1919 007c 1919 0074  .|...|.d...|...t
-00003d20: 1c7c 1e83 017c 107c 2364 0264 3985 0219  .|...|.|#d.d9...
-00003d30: 0064 3a8d 0501 0064 3ba0 107c 007c 03a1  .d:....d;..|.|..
-00003d40: 027d 2274 086a 09a0 177c 22a1 0190 0673  .}"t.j...|"....s
-00003d50: 9074 0564 3c7c 0164 1819 007c 1919 007c  .t.d<|.d...|...|
-00003d60: 0164 1919 007c 1919 0074 1c7c 1e83 0183  .d...|...t.|....
-00003d70: 0401 0074 1c7c 1e83 0164 3d6b 0090 0572  ...t.|...d=k...r
-00003d80: 2274 0564 3e83 0101 0074 0564 3f83 0101  "t.d>....t.d?...
-00003d90: 0074 0564 4083 0101 007c 02a0 1d7c 0164  .t.d@....|...|.d
-00003da0: 1819 007c 1919 007c 0164 1919 007c 1919  ...|...|.d...|..
-00003db0: 0074 1c7c 1e83 01a1 037d 267c 26a0 1e7c  .t.|.....}&|&..|
-00003dc0: 2264 41a1 0201 0090 0671 a074 1c7c 1e83  "dA......q.t.|..
-00003dd0: 0164 426b 0090 0572 8674 0564 4383 0101  .dBk...r.t.dC...
-00003de0: 0074 0564 4483 0101 0074 0564 4583 0101  .t.dD....t.dE...
-00003df0: 007c 026a 1f7c 0164 1819 007c 1919 007c  .|.j.|.d...|...|
-00003e00: 0164 1919 007c 1919 0074 1c7c 1e83 0164  .d...|...t.|...d
-00003e10: 4664 3464 4764 4864 4964 4a8d 087d 267c  Fd4dGdHdIdJ..}&|
-00003e20: 26a0 1e7c 2264 41a1 0201 0090 0671 a074  &..|"dA......q.t
-00003e30: 0564 4383 0101 0074 0564 4b83 0101 0074  .dC....t.dK....t
-00003e40: 0564 4583 0101 0064 4ca0 107c 007c 03a1  .dE....dL..|.|..
-00003e50: 027d 2374 086a 09a0 177c 2364 4d17 00a1  .}#t.j...|#dM...
-00003e60: 0190 0573 e87c 026a 1b7c 0164 1819 007c  ...s.|.j.|.d...|
-00003e70: 1919 007c 0164 1919 007c 1919 0074 1c7c  ...|.d...|...t.|
-00003e80: 1e83 0164 477c 2364 4e17 0064 3a8d 0501  ...dG|#dN..d:...
-00003e90: 0074 086a 09a0 177c 2364 4f17 00a1 0190  .t.j...|#dO.....
-00003ea0: 0673 267c 026a 1b7c 0164 1819 007c 1919  .s&|.j.|.d...|..
-00003eb0: 007c 0164 1919 007c 1919 0074 1c7c 1e83  .|.d...|...t.|..
-00003ec0: 0164 467c 2364 5017 0064 3a8d 0501 0074  .dF|#dP..d:....t
-00003ed0: 20a0 2164 51a0 107c 007c 03a1 02a1 017d   .!dQ..|.|.....}
-00003ee0: 277c 2764 5219 006a 227d 2874 20a0 2164  '|'dR..j"}(t .!d
-00003ef0: 51a0 107c 007c 03a1 02a1 017d 277c 2764  Q..|.|.....}'|'d
-00003f00: 5219 006a 227d 2974 20a0 2164 32a0 107c  R..j"})t .!d2..|
-00003f10: 007c 03a1 02a1 017d 277c 2764 5219 006a  .|.....}'|'dR..j
-00003f20: 227d 2a74 237c 297c 2a7c 2864 1364 497c  "}*t#|)|*|(d.dI|
-00003f30: 2264 538d 0601 006e 1074 0564 357c 229b  "dS....n.t.d5|".
-00003f40: 0064 369d 0383 0101 007c 1764 2e6b 0290  .d6......|.d.k..
-00003f50: 0672 cc74 247c 007c 017c 027c 247c 2564  .r.t$|.|.|.|$|%d
-00003f60: 547c 097c 0a7c 0b64 2e64 2e7c 0f7c 1064  T|.|.|.d.d.|.|.d
-00003f70: 558d 0d01 0064 3ba0 107c 007c 03a1 027d  U....d;..|.|...}
-00003f80: 2b74 25a0 267c 2ba1 017d 2c7c 1064 346b  +t%.&|+..},|.d4k
-00003f90: 0290 0772 247a 1674 20a0 2164 32a0 107c  ...r$z.t .!d2..|
-00003fa0: 007c 03a1 02a1 017d 2757 006e 2001 0001  .|.....}'W.n ...
-00003fb0: 0001 0074 20a0 2164 33a0 107c 007c 107c  ...t .!d3..|.|.|
-00003fc0: 03a1 03a1 017d 2759 006e 0258 007c 1064  .....}'Y.n.X.|.d
-00003fd0: 346b 0390 0772 4274 20a0 2164 33a0 107c  4k...rBt .!d3..|
-00003fe0: 007c 107c 03a1 03a1 017d 277c 2764 5219  .|.|.....}'|'dR.
-00003ff0: 006a 227d 2a74 0564 5683 0101 0074 0574  .j"}*t.dV....t.t
-00004000: 066a 0f64 5717 0083 0101 0074 0564 5883  .j.dW......t.dX.
-00004010: 0101 0074 0564 5683 0101 0074 277c 2a7c  ...t.dV....t'|*|
-00004020: 127c 137c 1464 598d 047d 2d74 256a 2864  .|.|.dY..}-t%j(d
-00004030: 5a64 5b8d 017d 2e74 256a 297c 2d64 5c64  Zd[..}.t%j)|-d\d
-00004040: 5d8d 0201 007c 1664 5e6b 0290 0772 b074  ]....|.d^k...r.t
-00004050: 25a0 2aa1 0001 006e 0874 25a0 2ba1 0001  %.*....n.t%.+...
-00004060: 0074 2c7c 2a64 5f7c 2d64 608d 035c 037d  .t,|*d_|-d`..\.}
-00004070: 2f7d 307d 3174 0574 066a 0f64 6117 0083  /}0}1t.t.j.da...
-00004080: 0101 0074 0564 5883 0101 0074 0564 62a0  ...t.dX....t.db.
-00004090: 107c 2fa1 0183 0101 0074 0564 63a0 107c  .|/......t.dc..|
-000040a0: 30a1 0183 0101 0074 0564 64a0 107c 31a1  0......t.dd..|1.
-000040b0: 0183 0101 0074 0564 65a0 107c 0c64 0219  .....t.de..|.d..
-000040c0: 007c 0c64 5219 00a1 0283 0101 0074 0564  .|.dR........t.d
-000040d0: 5883 0101 007c 0c64 0219 007c 2a6a 2d64  X....|.d...|*j-d
-000040e0: 5219 0064 1314 006b 0590 0872 7474 0574  R..d...k...rtt.t
-000040f0: 066a 0764 6617 0083 0101 0074 0574 066a  .j.df......t.t.j
-00004100: 0764 67a0 107c 2a6a 2d64 5219 0064 1314  .dg..|*j-dR..d..
-00004110: 00a1 0117 0083 0101 0064 0053 0074 2e83  .........d.S.t..
-00004120: 007d 3274 2f7c 2a7c 0c64 687c 327c 2d7c  .}2t/|*|.dh|2|-|
-00004130: 3064 698d 067d 337c 2a7c 336a 3038 007d  0di..}3|*|3j08.}
-00004140: 2a74 0564 6a83 0101 0074 256a 2864 5a64  *t.dj....t%j(dZd
-00004150: 5b8d 017d 2e74 256a 297c 336a 3064 5c64  [..}.t%j)|3j0d\d
-00004160: 5d8d 0201 007c 1664 5e6b 0290 0872 d074  ]....|.d^k...r.t
-00004170: 25a0 2aa1 0001 006e 0874 25a0 2ba1 0001  %.*....n.t%.+...
-00004180: 007c 0e74 3114 007d 3474 327c 3464 4864  .|.t1..}4t2|4dHd
-00004190: 4864 6b8d 037d 357c 35a0 33a1 0001 0074  Hdk..}5|5.3....t
-000041a0: 1c7c 2083 017d 3674 346a 357c 2a7c 0464  .| ..}6t4j5|*|.d
-000041b0: 6c8d 027d 3774 34a0 367c 2a7c 377c 36a1  l..}7t4.6|*|7|6.
-000041c0: 037d 387c 0d64 6d6b 0290 0972 8474 0564  .}8|.dmk...r.t.d
-000041d0: 6e83 0101 0074 0564 6f83 0101 0074 0564  n....t.do....t.d
-000041e0: 7083 0101 0074 256a 2864 5a64 5b8d 017d  p....t%j(dZd[..}
-000041f0: 2e74 256a 297c 3864 5c64 5d8d 0201 007c  .t%j)|8d\d]....|
-00004200: 1664 5e6b 0290 0972 6a74 25a0 2aa1 0001  .d^k...rjt%.*...
-00004210: 006e 0874 25a0 2ba1 0001 0074 377c 2a7c  .n.t%.+....t7|*|
-00004220: 387c 3664 7164 7264 738d 057d 3874 00a0  8|6dqdrds..}8t..
-00004230: 387c 386a 39a1 017d 3974 0564 7483 0101  8|8j9..}9t.dt...
-00004240: 0074 057c 386a 3983 0101 0074 0574 00a0  .t.|8j9....t.t..
-00004250: 3a74 3b7c 386a 3983 01a1 0183 0101 0064  :t;|8j9........d
-00004260: 0264 006c 3c7d 3a64 757c 3a6a 3d64 763c  .d.l<}:du|:j=dv<
-00004270: 0064 777c 3a6a 3d64 783c 0064 797c 3a6a  .dw|:j=dx<.dy|:j
-00004280: 3d64 7a3c 0064 497c 3a6a 3d64 7b3c 0064  =dz<.dI|:j=d{<.d
-00004290: 797c 3a6a 3d64 7c3c 0064 497c 3a6a 3d64  y|:j=d|<.dI|:j=d
-000042a0: 7d3c 0064 797c 3a6a 3d64 7e3c 0064 797c  }<.dy|:j=d~<.dy|
-000042b0: 3a6a 3d64 7f3c 0074 256a 2864 8064 5b8d  :j=d.<.t%j(d.d[.
-000042c0: 017d 2e74 00a0 3e7c 386a 22a1 01a0 3f74  .}.t..>|8j"...?t
-000042d0: 40a1 017d 3b74 006a 417c 3b7c 3b64 816b  @..};t.jA|;|;d.k
-000042e0: 023c 0074 1c7c 1e83 0164 1314 0064 1114  .<.t.|...d...d..
-000042f0: 007c 1b14 007d 3c74 256a 297c 3b64 8264  .|...}<t%j)|;d.d
-00004300: 8364 5c64 848d 047d 3d74 00a0 3a74 00a0  .d\d...}=t..:t..
-00004310: 427c 3ba1 01a1 0144 005d 427d 3e74 00a0  B|;....D.]B}>t..
-00004320: 017c 3b7c 3e64 5217 006b 02a1 017d 3f74  .|;|>dR..k...}?t
-00004330: 256a 437c 3f64 5219 0064 0219 007c 3f64  %jC|?dR..d...|?d
-00004340: 0219 0064 0219 0074 4474 1c7c 3e83 0183  ...d...tDt.|>...
-00004350: 0164 8564 868d 0401 0090 0a71 7074 25a0  .d.d.......qpt%.
-00004360: 457c 3da1 017d 407c 406a 46a0 47a1 0001  E|=..}@|@jF.G...
-00004370: 0074 25a0 47a1 0001 007c 1664 5e6b 0290  .t%.G....|.d^k..
-00004380: 0a72 e474 25a0 2aa1 0001 006e 0874 25a0  .r.t%.*....n.t%.
-00004390: 2ba1 0001 007c 1664 5e6b 0290 0d72 267c  +....|.d^k...r&|
-000043a0: 0f64 2e6b 0290 0b72 1664 227c 0164 0119  .d.k...r.d"|.d..
-000043b0: 007c 1919 0017 0064 2317 007d 226e 0c64  .|.....d#..}"n.d
-000043c0: 87a0 107c 007c 24a1 027d 2274 086a 09a0  ...|.|$..}"t.j..
-000043d0: 177c 22a1 0190 0b73 de74 0564 8883 0101  .|"....s.t.d....
-000043e0: 0074 256a 2864 8964 5b8d 017d 2e74 25a0  .t%j(d.d[..}.t%.
-000043f0: 4864 8aa1 0101 0074 256a 297c 3864 5c64  Hd.....t%j)|8d\d
-00004400: 8b74 00a0 4964 2464 5264 2464 5267 04a1  .t..Id$dRd$dRg..
-00004410: 017c 3c14 0064 8c8d 0401 0074 25a0 4a64  .|<..d.....t%.Jd
-00004420: 8da1 0101 0074 25a0 4b64 8ea1 0101 0074  .....t%.Kd.....t
-00004430: 25a0 47a1 0001 0074 25a0 4864 8fa1 0101  %.G....t%.Hd....
-00004440: 0074 256a 297c 2c74 00a0 4964 2464 5264  .t%j)|,t..Id$dRd
-00004450: 2464 5267 04a1 017c 3c14 0064 908d 0201  $dRg...|<..d....
-00004460: 0074 25a0 4ca1 0001 0074 25a0 4a64 8da1  .t%.L....t%.Jd..
-00004470: 0101 0074 25a0 47a1 0001 0074 25a0 2aa1  ...t%.G....t%.*.
-00004480: 0001 0090 016e 4874 25a0 267c 22a1 017d  .....nHt%.&|"..}
-00004490: 4174 256a 2864 9164 5b8d 017d 2e74 25a0  At%j(d.d[..}.t%.
-000044a0: 4864 92a1 0101 0074 256a 297c 3864 5c64  Hd.....t%j)|8d\d
-000044b0: 8b74 00a0 4964 2464 5264 2464 5267 04a1  .t..Id$dRd$dRg..
-000044c0: 017c 3c14 0064 8c8d 0401 0074 25a0 4a64  .|<..d.....t%.Jd
-000044d0: 8da1 0101 0074 25a0 4b64 8ea1 0101 0074  .....t%.Kd.....t
-000044e0: 25a0 47a1 0001 0074 25a0 4864 93a1 0101  %.G....t%.Hd....
-000044f0: 0074 256a 297c 2c74 00a0 4964 2464 5264  .t%j)|,t..Id$dRd
-00004500: 2464 5267 04a1 017c 3c14 0064 908d 0201  $dRg...|<..d....
-00004510: 0074 25a0 4ca1 0001 0074 25a0 4a64 8da1  .t%.L....t%.Jd..
-00004520: 0101 0074 25a0 47a1 0001 0074 25a0 4864  ...t%.G....t%.Hd
-00004530: 94a1 0101 007c 0f64 2e6b 0290 0c72 bc64  .....|.d.k...r.d
-00004540: 217c 1b1b 0064 111b 0064 1214 007d 1e74  !|...d...d...}.t
-00004550: 1c7c 1e83 0164 1314 0064 1114 007c 1b14  .|...d...d...|..
-00004560: 007d 3c6e 2864 957d 1e7c 2464 1214 007c  .}<n(d.}.|$d...|
-00004570: 1b1b 007c 1e1b 007d 4274 1c7c 1e83 0164  ...|...}Bt.|...d
-00004580: 1314 007c 4214 007c 1b14 007d 3c74 256a  ...|B..|...}<t%j
-00004590: 297c 4174 00a0 4964 2464 5264 2464 5267  )|At..Id$dRd$dRg
-000045a0: 04a1 017c 3c14 0064 908d 0201 0074 25a0  ...|<..d.....t%.
-000045b0: 4ca1 0001 0074 25a0 4a64 8da1 0101 0074  L....t%.Jd.....t
-000045c0: 25a0 47a1 0001 0074 25a0 2aa1 0001 007c  %.G....t%.*....|
-000045d0: 1764 5e6b 0390 0d72 8064 967c 009b 0064  .d^k...r.d.|...d
-000045e0: 977c 039b 0064 989d 057d 4364 997c 049b  .|...d...}Cd.|..
-000045f0: 0064 9a7c 059b 0064 9b7c 0c9b 0064 9c7c  .d.|...d.|...d.|
-00004600: 0d9b 0064 9d9d 097d 4464 9e7c 109b 0064  ...d...}Dd.|...d
-00004610: 9f9d 037d 4574 057c 437c 4417 007c 4517  ...}Et.|C|D..|E.
-00004620: 0083 0101 007c 2553 0074 1c7c 3b74 1c7c  .....|%S.t.|;t.|
-00004630: 3b6a 2d64 0219 0064 1314 0083 0174 1c7c  ;j-d...d.....t.|
-00004640: 3b6a 2d64 5219 0064 1314 0083 0166 0219  ;j-dR..d.....f..
-00004650: 0083 0164 5218 007d 4664 967c 009b 0064  ...dR..}Fd.|...d
-00004660: 977c 039b 0064 989d 057d 4364 997c 049b  .|...d...}Cd.|..
-00004670: 0064 9a7c 059b 0064 9b7c 0c9b 0064 9c7c  .d.|...d.|...d.|
-00004680: 0d9b 0064 9d9d 097d 4464 a07c 469b 0064  ...d...}Dd.|F..d
-00004690: a17c 109b 0064 a27c 109b 0064 9f9d 077d  .|...d.|...d...}
-000046a0: 4574 057c 437c 4417 007c 4517 0083 0101  Et.|C|D..|E.....
-000046b0: 0074 4d7c 007c 017c 027c 037c 047c 057c  .tM|.|.|.|.|.|.|
-000046c0: 4667 017c 1067 017c 0c7c 0d7c 107c 127c  Fg.|.g.|.|.|.|.|
-000046d0: 137c 147c 187c 157c 1664 a38d 1101 0064  .|.|.|.|.d.....d
-000046e0: 0053 0029 a44e 7241 0000 0072 0100 0000  .S.).NrA...r....
-000046f0: 7242 0000 0072 4300 0000 7244 0000 00fa  rB...rC...rD....
-00004700: 170a 4172 7020 2620 4d61 6f64 6f72 6520  ..Arp & Maodore 
-00004710: 4361 7461 6c6f 673a fa18 2d2d 2d2d 2d2d  Catalog:..------
-00004720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004730: 2d2d fa23 2f54 6162 6c65 5f41 7270 5f4d  --.#/Table_Arp_M
-00004740: 6164 6f72 655f 7061 6972 735f 7570 6461  adore_pairs_upda
-00004750: 7465 642e 7478 7472 0400 0000 7263 0000  ted.txtr....rc..
-00004760: 00a9 02da 0363 6174 da08 6372 6f73 735f  .....cat..cross_
-00004770: 4944 a902 da04 6465 7363 da05 636f 6465  ID....desc..code
-00004780: 7372 4500 0000 7246 0000 00fa 1344 6973  srE...rF.....Dis
-00004790: 7461 6e63 6520 7b3a 2e31 667d 204d 7063  tance {:.1f} Mpc
-000047a0: 7247 0000 0072 4800 0000 7239 0000 0072  rG...rH...r9...r
-000047b0: 4900 0000 724a 0000 0072 4b00 0000 724c  I...rJ...rK...rL
-000047c0: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
-000047d0: 0000 7250 0000 0072 5100 0000 7252 0000  ..rP...rQ...rR..
-000047e0: 0072 5300 0000 7254 0000 0072 5600 0000  .rS...rT...rV...
-000047f0: 7255 0000 0072 3a00 0000 fa0c 696d 6167  rU...r:.....imag
-00004800: 6573 5f31 3030 6b2f fa13 5f31 3030 5f6b  es_100k/.._100_k
-00004810: 7063 5f72 6164 6975 732e 706e 6772 6200  pc_radius.pngrb.
-00004820: 0000 7a27 0a0a 5468 6973 2067 616c 6178  ..z'..This galax
-00004830: 7920 6861 7320 3130 3020 6b70 6320 696d  y has 100 kpc im
-00004840: 6167 6520 6176 6169 626c 657a 2b0a 0a54  age avaiblez+..T
-00004850: 6869 7320 6761 6c61 7879 2068 6173 206e  his galaxy has n
-00004860: 6f74 2031 3030 206b 7063 2069 6d61 6765  ot 100 kpc image
-00004870: 2061 7661 6962 6c65 da0b 6669 7473 5f69   avaible..fits_i
-00004880: 6d61 6765 73fa 116d 6b64 6972 2066 6974  mages..mkdir fit
-00004890: 735f 696d 6167 6573 fa23 0a54 6865 2066  s_images.#.The f
-000048a0: 6f6c 6465 7220 6669 7473 5f69 6d61 6765  older fits_image
-000048b0: 7320 7761 7320 6372 6561 7465 64da 0669  s was created..i
-000048c0: 6d61 6765 73fa 0c6d 6b64 6972 2069 6d61  mages..mkdir ima
-000048d0: 6765 73fa 1e0a 5468 6520 666f 6c64 6572  ges...The folder
-000048e0: 2069 6d61 6765 7320 7761 7320 6372 6561   images was crea
-000048f0: 7465 6472 c700 0000 72c8 0100 0029 0472  tedr....r....).r
-00004900: 0101 0000 da06 7265 6769 6f6e da07 6c69  ......region..li
-00004910: 6d74 7665 6cda 0673 6572 7665 727a 200a  mtvel..serverz .
-00004920: 0a4c 6f61 6469 6e67 2f44 6f77 6e6c 6f61  .Loading/Downloa
-00004930: 6469 6e67 2074 6865 2069 6d61 6765 7372  ding the imagesr
-00004940: 5800 0000 7259 0000 0072 5a00 0000 723c  X...rY...rZ...r<
-00004950: 0000 0072 5b00 0000 725c 0000 0072 5d00  ...r[...r\...r].
-00004960: 0000 725e 0000 0072 5f00 0000 7260 0000  ..r^...r_...r`..
-00004970: 00fa 1769 6d61 6765 732f 6669 675f 7b7d  ...images/fig_{}
-00004980: 5f7b 7d6b 7063 2e70 6e67 7a1a 0a44 6f77  _{}kpc.pngz..Dow
-00004990: 6e6c 6f61 6469 6e67 2074 6865 2070 6e67  nloading the png
-000049a0: 2066 696c 653a e9e8 0300 007a 1d0a 2323   file:.....z..##
-000049b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000049c0: 2323 2323 2323 2323 2323 7a1d 446f 776e  ##########z.Down
-000049d0: 6c6f 6164 696e 6720 5247 4220 3132 2062  loading RGB 12 b
-000049e0: 616e 6420 696d 6167 657a 1c23 2323 2323  and imagez.#####
-000049f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004a00: 2323 2323 2323 23da 0350 4e47 69d0 0700  #######..PNGi...
-00004a10: 007a 2e0a 2323 2323 2323 2323 2323 2323  .z..############
-00004a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004a40: 237a 2d44 6f77 6e6f 6164 696e 6720 5247  #z-Downoading RG
-00004a50: 4220 3320 6261 6e64 2069 6d61 6765 2028  B 3 band image (
-00004a60: 696d 6167 653e 3130 3030 2070 6978 2129  image>1000 pix!)
-00004a70: 7a2d 2323 2323 2323 2323 2323 2323 2323  z-##############
-00004a80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004a90: 2323 2323 2323 2323 2323 2323 2323 2372  ###############r
-00004aa0: 3400 0000 72b6 0000 0072 8b00 0000 e908  4...r....r......
-00004ab0: 0000 0029 0572 3c00 0000 72b6 0000 0072  ...).r<...r....r
-00004ac0: b100 0000 da07 7374 7265 7463 68da 0151  ......stretch..Q
-00004ad0: 7a2d 446f 776e 6f61 6469 6e67 2052 4742  z-Downoading RGB
-00004ae0: 2033 2062 616e 6420 696d 6167 6520 2869   3 band image (i
-00004af0: 6d61 6765 3e32 3030 3020 7069 7821 297a  mage>2000 pix!)z
-00004b00: 1466 6974 735f 696d 6167 6573 2f7b 7d5f  .fits_images/{}_
-00004b10: 7b7d 6b70 637a 055f 472e 667a da02 5f47  {}kpcz._G.fz.._G
-00004b20: 7a05 5f49 2e66 7ada 025f 497a 1966 6974  z._I.fz.._Iz.fit
-00004b30: 735f 696d 6167 6573 2f7b 7d5f 7b7d 6b70  s_images/{}_{}kp
-00004b40: 635f 472e 667a 7269 0000 0029 0372 e201  c_G.fzri...).r..
-00004b50: 0000 72e3 0100 00da 0866 696c 656e 616d  ..r......filenam
-00004b60: 6546 290a 7201 0100 00da 0574 6162 6c65  eF).r......table
-00004b70: da0a 6164 645f 6f62 6a65 6374 da05 7874  ..add_object..xt
-00004b80: 706f 73da 0579 7470 6f73 da06 6465 6c74  pos..ytpos..delt
-00004b90: 6179 da09 7072 696e 745f 6172 70da 0b70  ay..print_arp..p
-00004ba0: 7269 6e74 5f73 6361 6c65 da09 7573 6573  rint_scale..uses
-00004bb0: 696d 6261 6472 0801 0000 726f 0000 0072  imbadr....ro...r
-00004bc0: 6d00 0000 726e 0000 0072 7000 0000 7274  m...rn...rp...rt
-00004bd0: 0000 0072 7600 0000 7278 0000 0072 7900  ...rv...rx...ry.
-00004be0: 0000 7240 0000 0072 7f00 0000 7280 0000  ..r@...r....r...
-00004bf0: 0072 8300 0000 7285 0000 0072 8600 0000  .r....r....r....
-00004c00: 7287 0000 0072 8800 0000 7a2b 0a0a 5468  r....r....z+..Th
-00004c10: 6520 736b 7920 626f 7820 6973 2062 6967  e sky box is big
-00004c20: 6765 7220 666f 7220 7468 6520 696d 6167  ger for the imag
-00004c30: 6520 7369 7a65 217a 2b50 6c65 6173 6520  e size!z+Please 
-00004c40: 696e 7472 6f64 7563 6520 6120 736d 616c  introduce a smal
-00004c50: 6c65 7220 626f 7820 7468 616e 207b 7d20  ler box than {} 
-00004c60: 7069 7821 728a 0000 0072 8c00 0000 fa0e  pix!r....r......
-00004c70: 4261 636b 6772 6f75 6e64 206d 6170 7298  Background mapr.
-00004c80: 0000 0072 9b00 0000 729c 0000 0072 9d00  ...r....r....r..
-00004c90: 0000 729e 0000 0072 9f00 0000 72a0 0000  ..r....r....r...
-00004ca0: 0072 a100 0000 72a2 0000 00fa 290a 4172  .r....r.....).Ar
-00004cb0: 6561 2069 6e20 7069 7865 6c20 6f66 2074  ea in pixel of t
-00004cc0: 6865 2064 6574 6563 7469 6f6e 206f 626a  he detection obj
-00004cd0: 6563 7473 3a20 e916 0000 00fa 0e61 7865  ects: .......axe
-00004ce0: 732e 6c61 6265 6c73 697a 6572 5e01 0000  s.labelsizer^...
-00004cf0: fa0f 6c65 6765 6e64 2e66 6f6e 7473 697a  ..legend.fontsiz
-00004d00: 65e9 1000 0000 fa10 7874 6963 6b2e 6d61  e.......xtick.ma
-00004d10: 6a6f 722e 7369 7a65 fa10 7874 6963 6b2e  jor.size..xtick.
-00004d20: 6d69 6e6f 722e 7369 7a65 fa10 7974 6963  minor.size..ytic
-00004d30: 6b2e 6d61 6a6f 722e 7369 7a65 fa10 7974  k.major.size..yt
-00004d40: 6963 6b2e 6d69 6e6f 722e 7369 7a65 fa0f  ick.minor.size..
-00004d50: 7874 6963 6b2e 6c61 6265 6c73 697a 65fa  xtick.labelsize.
-00004d60: 0f79 7469 636b 2e6c 6162 656c 7369 7a65  .ytick.labelsize
-00004d70: a902 72e1 0100 0072 e101 0000 726b 0000  ..r....r....rk..
-00004d80: 00da 0650 6169 7265 64da 076e 6561 7265  ...Paired..neare
-00004d90: 7374 a903 72a8 0000 00da 0d69 6e74 6572  st..r......inter
-00004da0: 706f 6c61 7469 6f6e 727a 0000 00e9 1e00  polationrz......
-00004db0: 0000 a901 da08 666f 6e74 7369 7a65 fa1a  ......fontsize..
-00004dc0: 696d 6167 6573 2f7b 7d5f 7369 6d62 6164  images/{}_simbad
-00004dd0: 5f7b 7d6b 7063 2e70 6e67 7a26 0a54 6865  _{}kpc.pngz&.The
-00004de0: 2069 6d61 6765 206f 6620 3130 3020 6b70   image of 100 kp
-00004df0: 6320 6973 206e 6f74 2061 7661 696c 6162  c is not availab
-00004e00: 6c65 2902 e911 0000 0072 e101 0000 e979  le)......r.....y
-00004e10: 0000 0072 a700 0000 2903 727a 0000 0072  ...r....).rz...r
-00004e20: a800 0000 da06 6578 7465 6e74 fa07 7820  ......extent..x 
-00004e30: 286b 7063 29fa 0779 2028 6b70 6329 e97a  (kpc)..y (kpc).z
-00004e40: 0000 00a9 0172 0602 0000 2902 e915 0000  .....r....).....
-00004e50: 0072 e101 0000 e983 0000 00e9 8400 0000  .r..............
-00004e60: e985 0000 00e9 2c01 0000 7a0f 0a0a 534c  ......,...z...SL
-00004e70: 2e70 686f 745f 6d6f 6428 277a 2127 2c20  .phot_mod('z!', 
-00004e80: 7461 625f 6761 6c2c 2063 6f6e 6e2c 2073  tab_gal, conn, s
-00004e90: 697a 655f 696d 6167 655f 7068 793d fa02  ize_image_phy=..
-00004ea0: 2c20 fa09 2073 6e72 5f67 203d 20fa 0a2c  , .. snr_g = ..,
-00004eb0: 2061 7265 6167 616c 3d7a 0b2c 736b 795f   areagal=z.,sky_
-00004ec0: 626f 7820 3d20 fa0d 2c0a 2064 6562 6c65  box = ..,. deble
-00004ed0: 6e64 203d 22fa 0322 2c20 7a2d 7573 6572  nd ="..", z-user
-00004ee0: 5f6f 7264 6572 3d5b 312c 325d 2c20 7573  _order=[1,2], us
-00004ef0: 6572 5f6c 6973 743d 5b22 4122 2c22 4222  er_list=["A","B"
-00004f00: 5d2c 2062 616e 643d 277a 0227 29fa 0c75  ], band='z.')..u
-00004f10: 7365 725f 6f72 6465 723d 5b7a 0e5d 2c20  ser_order=[z.], 
-00004f20: 7573 6572 5f6c 6973 743d 5b7a 095d 2c20  user_list=[z.], 
-00004f30: 6261 6e64 3d27 290e 7201 0100 0072 0201  band=').r....r..
-00004f40: 0000 7203 0100 0072 0401 0000 7205 0100  ..r....r....r...
-00004f50: 0072 0601 0000 7207 0100 0072 0801 0000  .r....r....r....
-00004f60: 7271 0000 0072 7200 0000 7273 0000 0072  rq...rr...rs...r
-00004f70: c000 0000 72ae 0000 0072 c100 0000 294e  ....r....r....)N
-00004f80: 7225 0000 0072 c800 0000 72b7 0000 0072  r%...r....r....r
-00004f90: c900 0000 72ca 0000 0072 cb00 0000 7219  ....r....r....r.
-00004fa0: 0000 0072 d200 0000 72d4 0000 0072 d500  ...r....r....r..
-00004fb0: 0000 72de 0000 0072 df00 0000 72e0 0000  ..r....r....r...
-00004fc0: 0072 0500 0000 72d9 0000 0072 cc00 0000  .r....r....r....
-00004fd0: 7264 0000 0072 cd00 0000 72ce 0000 0072  rd...r....r....r
-00004fe0: cf00 0000 72d0 0000 0072 d100 0000 72d3  ....r....r....r.
-00004ff0: 0000 0072 d600 0000 da06 7379 7374 656d  ...r......system
-00005000: 72dd 0000 00da 0a63 6174 5f73 696d 6261  r......cat_simba
-00005010: 6472 d700 0000 72d8 0000 00da 0f74 7765  dr....r......twe
-00005020: 6c76 655f 6261 6e64 5f69 6d67 da04 7361  lve_band_img..sa
-00005030: 7665 da07 6765 745f 696d 6772 0300 0000  ve..get_imgr....
-00005040: 72e4 0000 0072 e500 0000 7218 0000 00da  r....r....r.....
-00005050: 0b70 6c6f 745f 7369 6d62 6164 72e6 0000  .plot_simbadr...
-00005060: 00da 0669 6d72 6561 6472 0a00 0000 72e7  ...imreadr....r.
-00005070: 0000 0072 e800 0000 72ea 0000 0072 eb00  ...r....r....r..
-00005080: 0000 720b 0000 0072 a601 0000 720d 0000  ..r....r....r...
-00005090: 0072 0c00 0000 72ec 0000 0072 1100 0000  .r....r....r....
-000050a0: 7210 0000 0072 f200 0000 72f3 0000 0072  r....r....r....r
-000050b0: f400 0000 720e 0000 0072 0f00 0000 da06  ....r....r......
-000050c0: 6172 676d 6178 72fa 0000 00da 0661 7261  argmaxr......ara
-000050d0: 6e67 6572 e300 0000 da0a 6d61 7470 6c6f  nger......matplo
-000050e0: 746c 6962 da08 7263 5061 7261 6d73 7226  tlib..rcParamsr&
-000050f0: 0000 0072 8601 0000 da05 666c 6f61 7472  ...r......floatr
-00005100: 2700 0000 da06 6e61 6e6d 6178 da04 7465  '.....nanmax..te
-00005110: 7874 72da 0000 0072 b001 0000 72b2 0100  xtr....r....r...
-00005120: 00da 0d6d 696e 6f72 7469 636b 735f 6f6e  ...minorticks_on
-00005130: da07 7375 6270 6c6f 74da 0561 7272 6179  ..subplot..array
-00005140: da06 786c 6162 656c da06 796c 6162 656c  ..xlabel..ylabel
-00005150: 72ba 0100 0072 3901 0000 2947 7241 0000  r....r9...)GrA..
-00005160: 0072 ff00 0000 7200 0100 0072 0101 0000  .r....r....r....
-00005170: 7202 0100 0072 0301 0000 72db 0100 0072  r....r....r....r
-00005180: dd01 0000 72dc 0100 0072 e901 0000 72ea  ....r....r....r.
-00005190: 0100 0072 eb01 0000 7206 0100 0072 0701  ...r....r....r..
-000051a0: 0000 72ad 0000 0072 ee01 0000 7208 0100  ..r....r....r...
-000051b0: 00da 0e66 6965 6c64 5f73 697a 655f 7068  ...field_size_ph
-000051c0: 7972 7100 0000 7272 0000 0072 7300 0000  yrq...rr...rs...
-000051d0: 72ae 0000 0072 c100 0000 da08 7275 6e5f  r....r......run_
-000051e0: 6175 746f 72c0 0000 0072 0901 0000 72b3  autor....r....r.
-000051f0: 0000 0072 0a01 0000 7213 0100 0072 bf00  ...r....r....r..
-00005200: 0000 720b 0100 0072 0c01 0000 720d 0100  ..r....r....r...
-00005210: 0072 0e01 0000 72d5 0000 0072 0f01 0000  .r....r....r....
-00005220: da09 7261 6473 696d 6261 64da 096f 7574  ..radsimbad..out
-00005230: 7369 6d62 6164 da04 696d 6163 721a 0100  simbad..imacr...
-00005240: 00da 0669 6d61 675f 47da 0669 6d61 675f  ...imag_G..imag_
-00005250: 4972 1b01 0000 da05 7265 6164 6eda 0569  Ir......readn..i
-00005260: 6d61 3530 721c 0100 0072 1d01 0000 721e  ma50r....r....r.
-00005270: 0100 0072 1f01 0000 7220 0100 0072 8e00  ...r....r ...r..
-00005280: 0000 7221 0100 0072 8100 0000 722a 0100  ..r!...r....r*..
-00005290: 0072 2b01 0000 722c 0100 0072 2d01 0000  .r+...r,...r-...
-000052a0: da08 6761 6c5f 6d61 696e da03 6d70 6cda  ..gal_main..mpl.
-000052b0: 0573 6567 6d63 da0e 7369 7a65 5f69 6d61  .segmc..size_ima
-000052c0: 6765 5f6b 7063 da05 696d 7365 6772 3301  ge_kpc..imsegr3.
-000052d0: 0000 da03 706f 7372 c401 0000 da06 696d  ....posr......im
-000052e0: 6131 3030 da09 7069 785f 7363 696d 61da  a100..pix_scima.
-000052f0: 0570 6172 7430 da05 7061 7274 31da 0570  .part0..part1..p
-00005300: 6172 7432 da07 6d61 7861 7265 6172 2f00  art2..maxarear/.
-00005310: 0000 722f 0000 0072 3000 0000 da0b 6578  ..r/...r0.....ex
-00005320: 5f70 686f 745f 6d6f 6474 0200 0073 8a02  _phot_modt...s..
-00005330: 0000 0007 1a01 1001 1802 0e01 0801 1401  ................
-00005340: 0a01 02ff 0602 2201 2202 0e01 0e02 1401  ......".".......
-00005350: 1401 1002 1001 1401 1c01 0c01 02ff 0803  ................
-00005360: 1c01 1401 0e01 0e01 0e01 0e01 0402 0c01  ................
-00005370: 0e01 0e01 0e01 0402 0a01 1401 1c01 1c01  ................
-00005380: 0e01 1002 0e01 0e01 0e01 0402 0e01 0a01  ................
-00005390: 0e02 0e01 0a01 0e02 0801 0401 0a01 0602  ................
-000053a0: 0402 0e02 0a01 0a01 0200 02ff 060d 0e01  ................
-000053b0: 0803 0c01 0e01 2601 1001 2601 1001 1e01  ......&...&.....
-000053c0: 0200 0aff 0603 0e01 1002 1801 1001 1e01  ................
-000053d0: 0201 0afe 0605 0c01 0e01 0e01 0a00 06ff  ................
-000053e0: 0402 0e01 0801 0801 0801 1801 06ff 0402  ................
-000053f0: 1001 0e01 0801 0801 0801 1801 0601 0200  ................
-00005400: 0200 0200 0200 02fe 0603 1002 0801 0801  ................
-00005410: 0802 0c01 1201 1801 0600 0200 06ff 0602  ................
-00005420: 1201 1801 0600 0200 06ff 0603 0a01 02ff  ................
-00005430: 0602 0a01 0a01 02ff 0602 0a01 0a01 02ff  ................
-00005440: 0602 0a02 0c01 02ff 0806 1003 0a01 0c01  ................
-00005450: 0200 0200 0200 0201 0200 0200 0200 02fe  ................
-00005460: 0604 0c01 0a01 0a01 0201 1601 0601 1a01  ................
-00005470: 0a01 1401 0a06 0801 0e01 0801 0801 0801  ................
-00005480: 02ff 0602 0c01 0e01 0a01 0a02 0802 0601  ................
-00005490: 02ff 0c02 0e01 0801 0e01 0e01 0e04 0601  ................
-000054a0: 0600 06ff 0602 0802 1801 0e01 0a01 0cff  ................
-000054b0: 0802 0402 0601 0801 0200 0201 02fe 0604  ................
-000054c0: 0a02 0801 0c01 1001 0a01 0a02 0803 0801  ................
-000054d0: 0e01 0803 0801 0e01 0e02 0a01 0801 0802  ................
-000054e0: 0801 0c01 0e01 0a01 0a02 0801 0802 0200  ................
-000054f0: 02fe 0607 0c01 0801 0a01 1406 0801 0a01  ................
-00005500: 0a01 0a01 0a01 0a01 0a01 0a01 0a02 0c01  ................
-00005510: 1201 0e01 1409 0a01 02ff 0604 1401 1201  ................
-00005520: 2e02 0a01 0a01 0801 0a01 0a02 0803 0a01  ................
-00005530: 0a01 1602 0c01 0e01 0801 0c01 0a01 0a01  ................
-00005540: 14ff 0602 0a01 0a01 0801 0a01 2001 0801  ............ ...
-00005550: 0a01 0801 0c04 0a01 0c01 0a01 0a01 14ff  ................
-00005560: 0602 0a01 0a01 0801 0a01 2001 0801 0a01  .......... .....
-00005570: 0801 0a01 0a01 1001 1602 0401 1001 1401  ................
-00005580: 2001 0801 0a01 0801 0802 0a01 1201 1e01   ...............
-00005590: 0c01 1002 0402 3002 1201 1e01 1801 1002  ......0.........
-000055a0: 0a01 0200 0201 0400 0400 0201 0200 0200  ................
-000055b0: 0200 0201 0200 0200 0201 02fb 723e 0200  ............r>..
-000055c0: 00da 0362 6f78 6306 0000 0000 0000 0000  ...boxc.........
-000055d0: 0000 000f 0000 0007 0000 0043 0000 0073  ...........C...s
-000055e0: 3601 0000 7400 a001 7c01 6401 1900 7c00  6...t...|.d...|.
-000055f0: 6b02 a101 6402 1900 6402 1900 7d06 7c01  k...d...d...}.|.
-00005600: 6403 1900 7c06 1900 7d07 7c07 7402 1b00  d...|...}.|.t...
-00005610: 7d08 7400 a003 7400 a004 6404 a101 a101  }.t...t...d.....
-00005620: 7c08 1400 6405 1400 7d09 7c02 7c09 1b00  |...d...}.|.|...
-00005630: 7d0a 7c03 6406 6b02 7274 6407 a005 7c01  }.|.d.k.rtd...|.
-00005640: 6408 1900 7c06 1900 7c01 6409 1900 7c06  d...|...|.d...|.
-00005650: 1900 7c0a a103 7d0b 7c03 640a 6b02 72a4  ..|...}.|.d.k.r.
-00005660: 640b a005 7c01 6408 1900 7c06 1900 7c01  d...|.d...|...|.
-00005670: 6409 1900 7c06 1900 7c0a 640c 1400 7c0a  d...|...|.d...|.
-00005680: 640c 1400 a104 7d0b 7c04 640d 6b02 72b2  d.....}.|.d.k.r.
-00005690: 640e 7d0c 6e14 640f a005 7c07 7c04 1700  d.}.n.d...|.|...
-000056a0: 7c07 7c04 1800 a102 7d0c 7c0b 7c0c 1700  |.|.....}.|.|...
-000056b0: 6410 1700 7d0d 7406 6411 8301 0100 7406  d...}.t.d.....t.
-000056c0: 6412 8301 0100 7406 7c0d 8301 0100 7c05  d.....t.|.....|.
-000056d0: 6400 6b09 9001 720e 7c05 6413 1700 7407  d.k...r.|.d...t.
-000056e0: 6a08 5f09 7406 6414 7407 6a08 6a09 8302  j._.t.d.t.j.j...
-000056f0: 0100 7407 6a08 a00a 7c0d a101 7d0e 7406  ..t.j...|...}.t.
-00005700: 6415 8301 0100 7406 6416 8301 0100 7406  d.....t.d.....t.
-00005710: 7c0e 8301 0100 7c0e 5300 2917 4e72 4100  |.....|.S.).NrA.
-00005720: 0000 7201 0000 0072 4200 0000 7243 0000  ..r....rB...rC..
-00005730: 0072 4400 0000 72c5 0100 007a 2a72 6567  .rD...r....z*reg
-00005740: 696f 6e28 6369 7263 6c65 2c20 4943 5253  ion(circle, ICRS
-00005750: 2c20 7b3a 2b66 7d20 7b3a 2b66 7d2c 207b  , {:+f} {:+f}, {
-00005760: 3a2e 3066 7d73 2972 4e00 0000 724f 0000  :.0f}s)rN...rO..
-00005770: 0072 3f02 0000 7a2f 7265 6769 6f6e 2862  .r?...z/region(b
-00005780: 6f78 2c20 4943 5253 2c20 7b3a 2b66 7d20  ox, ICRS, {:+f} 
-00005790: 7b3a 2b66 7d2c 207b 3a2e 3066 7d73 207b  {:+f}, {:.0f}s {
-000057a0: 3a2e 3066 7d73 2972 3900 0000 7262 0000  :.0f}s)r9...rb..
-000057b0: 0072 c700 0000 7a1d 2026 2072 6164 7665  .r....z. & radve
-000057c0: 6c20 203c 207b 7d20 2620 7261 6476 656c  l  < {} & radvel
-000057d0: 203e 207b 7d7a 1120 2620 6f74 7970 6520   > {}z. & otype 
-000057e0: 3d20 4761 6c61 7879 7a0d 5369 6d62 6164  = Galaxyz.Simbad
-000057f0: 2071 7565 7279 207a 0d3d 3d3d 3d3d 3d3d   query z.=======
-00005800: 3d3d 3d3d 3d0a 7a11 7369 6d62 6164 2f73  =====.z.simbad/s
-00005810: 696d 2d73 6372 6970 747a 1a43 6861 6e67  im-scriptz.Chang
-00005820: 696e 6720 5369 6d62 6164 2073 6572 7665  ing Simbad serve
-00005830: 7220 746f 207a 070a 4f75 7470 7574 7a07  r to z..Outputz.
-00005840: 3d3d 3d3d 3d3d 0a29 0b72 2500 0000 72c8  ======.).r%...r.
-00005850: 0000 0072 b700 0000 72c9 0000 0072 ca00  ...r....r....r..
-00005860: 0000 7264 0000 0072 cb00 0000 7206 0000  ..rd...r....r...
-00005870: 00da 0653 696d 6261 64da 0a53 494d 4241  ...Simbad..SIMBA
-00005880: 445f 5552 4cda 0e71 7565 7279 5f63 7269  D_URL..query_cri
-00005890: 7465 7269 6129 0f72 c200 0000 72ff 0000  teria).r....r...
-000058a0: 0072 0101 0000 72db 0100 0072 dc01 0000  .r....r....r....
-000058b0: 72dd 0100 0072 0901 0000 da06 7665 6c67  r....r......velg
-000058c0: 616c 72b3 0000 00da 076b 7063 5f61 7263  alr......kpc_arc
-000058d0: da07 6172 6364 6973 74da 0566 7061 7274  ..arcdist..fpart
-000058e0: da05 7370 6172 74da 0761 6c6c 6372 6974  ..spart..allcrit
-000058f0: da06 7265 7375 6c74 722f 0000 0072 2f00  ..resultr/...r/.
-00005900: 0000 7230 0000 0072 1702 0000 f103 0000  ..r0...r........
-00005910: 7346 0000 0000 031a 010c 0208 0218 0208  sF..............
-00005920: 0308 0104 010a 010a 0002 fe04 0308 0104  ................
-00005930: 010a 010a 0106 0006 fd04 0408 0106 020a  ................
-00005940: 0106 ff04 020c 0208 0108 0108 020a 010c  ................
-00005950: 010e 010c 0208 0108 0108 0272 1702 0000  ...........r....
-00005960: 720f 0200 0063 0500 0000 0000 0000 0000  r....c..........
-00005970: 0000 1200 0000 0600 0000 4300 0000 7302  ..........C...s.
-00005980: 0100 0074 00a0 017c 0164 0119 007c 006b  ...t...|.d...|.k
-00005990: 02a1 0164 0219 0064 0219 007d 057c 0164  ...d...d...}.|.d
-000059a0: 0319 007c 0519 007d 067c 0674 021b 007d  ...|...}.|.t...}
-000059b0: 0774 00a0 0374 00a0 0464 04a1 01a1 017c  .t...t...d.....|
-000059c0: 0714 0064 0514 007d 087c 0264 0614 007c  ...d...}.|.d...|
-000059d0: 081b 007d 097c 0964 071b 007d 0a7c 0164  ...}.|.d...}.|.d
-000059e0: 0819 007c 0519 007d 0b7c 0164 0919 007c  ...|...}.|.d...|
-000059f0: 0519 007d 0c64 0a7d 0d64 0ba0 0574 0664  ...}.d.}.d...t.d
-00005a00: 0c83 017c 037c 047c 0aa1 047d 0e64 0da0  ...|.|.|...}.d..
-00005a10: 057c 0b7c 0ca1 027d 0f74 077c 0d7c 0e17  .|.|...}.t.|.|..
-00005a20: 007c 0f17 0064 0e17 0064 0fa0 057c 007c  .|...d...d...|.|
-00005a30: 02a1 0283 0201 0074 08a0 0964 0fa0 057c  .......t...d...|
-00005a40: 007c 02a1 02a1 017d 1064 0ba0 0574 0664  .|.....}.d...t.d
-00005a50: 1083 017c 037c 047c 0aa1 047d 0e74 0aa0  ...|.|.|...}.t..
-00005a60: 0b7c 0d7c 0e17 007c 0f17 00a1 017d 117c  .|.|...|.....}.|
-00005a70: 11a0 0c64 11a0 057c 007c 02a1 02a1 0101  ...d...|.|......
-00005a80: 0064 0053 0029 124e 7241 0000 0072 0100  .d.S.).NrA...r..
-00005a90: 0000 7242 0000 0072 4300 0000 7244 0000  ..rB...rC...rD..
-00005aa0: 0072 3900 0000 724a 0000 0072 4e00 0000  .r9...rJ...rN...
-00005ab0: 724f 0000 007a 3968 7474 703a 2f2f 616c  rO...z9http://al
-00005ac0: 6173 6b79 2e75 2d73 7472 6173 6267 2e66  asky.u-strasbg.f
-00005ad0: 722f 6869 7073 2d69 6d61 6765 2d73 6572  r/hips-image-ser
-00005ae0: 7669 6365 732f 6869 7073 3266 6974 733f  vices/hips2fits?
-00005af0: 7a21 6869 7073 3d7b 7d26 7769 6474 683d  z!hips={}&width=
-00005b00: 7b7d 2668 6569 6768 743d 7b7d 2666 6f76  {}&height={}&fov
-00005b10: 3d7b 7d7a 0a44 5353 322f 636f 6c6f 727a  ={}z.DSS2/colorz
-00005b20: 2a26 7072 6f6a 6563 7469 6f6e 3d54 414e  *&projection=TAN
-00005b30: 2663 6f6f 7264 7379 733d 6963 7273 2672  &coordsys=icrs&r
-00005b40: 613d 7b7d 2664 6563 3d7b 7d7a 0b26 666f  a={}&dec={}z.&fo
-00005b50: 726d 6174 3d70 6e67 7203 0200 007a 0844  rmat=pngr....z.D
-00005b60: 5353 322f 7265 64fa 2066 6974 735f 696d  SS2/red. fits_im
-00005b70: 6167 6573 2f7b 7d5f 7369 6d62 6164 5f7b  ages/{}_simbad_{
-00005b80: 7d6b 7063 2e66 6974 7329 0d72 2500 0000  }kpc.fits).r%...
-00005b90: 72c8 0000 0072 b700 0000 72c9 0000 0072  r....r....r....r
-00005ba0: ca00 0000 7264 0000 0072 1200 0000 7213  ....rd...r....r.
-00005bb0: 0000 0072 e600 0000 721c 0200 0072 0300  ...r....r....r..
-00005bc0: 0000 72e4 0000 0072 ed00 0000 2912 72c2  ..r....r....).r.
-00005bd0: 0000 0072 ff00 0000 7201 0100 00da 0577  ...r....r......w
-00005be0: 6964 7468 da06 6865 6967 6874 7209 0100  idth..heightr...
-00005bf0: 0072 4302 0000 72b3 0000 0072 4402 0000  .rC...r....rD...
-00005c00: 7245 0200 00da 0366 6f76 724e 0000 0072  rE.....fovrN...r
-00005c10: 4f00 0000 da09 6261 7369 635f 7572 6cda  O.....basic_url.
-00005c20: 0b6f 626a 6563 745f 7572 6c31 da0b 6f62  .object_url1..ob
-00005c30: 6a65 6374 5f75 726c 32da 0a69 6d61 5f73  ject_url2..ima_s
-00005c40: 696d 6261 64da 0368 6475 722f 0000 0072  imbad..hdur/...r
-00005c50: 2f00 0000 7230 0000 00da 0f73 696d 6261  /...r0.....simba
-00005c60: 645f 646f 776e 6c6f 6164 1d04 0000 7338  d_download....s8
-00005c70: 0000 0000 031a 010c 0208 0118 020c 0108  ................
-00005c80: 020c 010c 0204 010a 0102 0002 0002 ff04  ................
-00005c90: 020c 0510 010a ff04 030a 0102 ff06 050a  ................
-00005ca0: 0102 0002 0002 ff04 0212 0172 5302 0000  ...........rS...
-00005cb0: e90c 0000 0063 0c00 0000 0000 0000 0000  .....c..........
-00005cc0: 0000 3100 0000 0c00 0000 4300 0000 7304  ..1.......C...s.
-00005cd0: 0700 0074 00a0 017c 0164 0119 007c 006b  ...t...|.d...|.k
-00005ce0: 02a1 0164 0219 0064 0219 007d 0c7c 0164  ...d...d...}.|.d
-00005cf0: 0319 007c 0c19 007d 0d7c 0d74 021b 007d  ...|...}.|.t...}
-00005d00: 0e74 00a0 0374 00a0 0464 04a1 01a1 017c  .t...t...d.....|
-00005d10: 0e14 0064 0514 007d 0f7c 0264 0614 007c  ...d...}.|.d...|
-00005d20: 0f1b 007d 107c 1064 071b 007d 117c 0164  ...}.|.d...}.|.d
-00005d30: 0819 007c 0c19 007d 127c 0164 0919 007c  ...|...}.|.d...|
-00005d40: 0c19 007d 1364 0aa0 057c 007c 02a1 027d  ...}.d...|.|...}
-00005d50: 1474 066a 07a0 087c 14a1 0173 ae74 0964  .t.j...|...s.t.d
-00005d60: 0b7c 149b 0064 0c9d 0383 0101 0074 0a7c  .|...d.......t.|
-00005d70: 007c 017c 027c 037c 0464 0d8d 0501 006e  .|.|.|.|.d.....n
-00005d80: 1674 0974 0b6a 0c64 0e7c 149b 0064 0f9d  .t.t.j.d.|...d..
-00005d90: 0317 0083 0101 0074 0da0 0e64 0aa0 057c  .......t...d...|
-00005da0: 007c 02a1 02a1 017d 1574 0fa0 1064 10a0  .|.....}.t...d..
-00005db0: 057c 007c 02a1 02a1 017d 1674 0974 0b6a  .|.|.....}.t.t.j
-00005dc0: 1164 1117 0083 0101 0074 127c 007c 017c  .d.......t.|.|.|
-00005dd0: 0264 127c 0964 0064 138d 067d 177c 177c  .d.|.d.d...}.|.|
-00005de0: 1764 1419 0064 026b 0419 007d 1774 0f6a  .d...d.k...}.t.j
-00005df0: 1364 1564 168d 0101 0074 0f6a 147c 1674  .d.d.....t.j.|.t
-00005e00: 00a0 1564 1764 1864 1764 1867 04a1 017c  ...d.d.d.d.g...|
-00005e10: 0214 0064 198d 0201 0074 167c 1274 176a  ...d.....t.|.t.j
-00005e20: 1814 007c 1374 176a 1814 0083 027d 187c  ...|.t.j.....}.|
-00005e30: 0a64 1a6b 0290 0172 8e74 196a 1a7c 1864  .d.k...r.t.j.|.d
-00005e40: 1b7c 1014 0074 176a 1b14 0064 1c8d 027d  .|...t.j...d...}
-00005e50: 197c 197c 1964 1d19 0064 026b 0419 007d  .|.|.d...d.k...}
-00005e60: 1974 167c 1764 1e19 007c 1764 1f19 0083  .t.|.d...|.d....
-00005e70: 027d 1a7c 18a0 1c7c 1aa1 017d 1b7c 1b6a  .}.|...|...}.|.j
-00005e80: 1b7c 0f14 007d 1c74 0964 2083 0101 0074  .|...}.t.d ....t
-00005e90: 0974 0b6a 1d64 2117 0083 0101 0074 0964  .t.j.d!......t.d
-00005ea0: 2283 0101 0074 00a0 1e74 1f7c 1a83 01a1  "....t...t.|....
-00005eb0: 0144 005d 407d 1d64 237d 1e74 097c 1e64  .D.]@}.d#}.t.|.d
-00005ec0: 24a0 057c 007c 1d7c 1764 2519 007c 1d19  $..|.|.|.d%..|..
-00005ed0: 007c 1764 1419 007c 1d19 007c 1c7c 1d19  .|.d...|...|.|..
-00005ee0: 007c 1b6a 1b7c 1d19 00a1 0617 0083 0101  .|.j.|..........
-00005ef0: 0090 0171 e074 20a0 217c 1564 0219 006a  ...q.t .!|.d...j
-00005f00: 22a1 017d 1f7c 1fa0 237c 1764 1e19 007c  "..}.|..#|.d...|
-00005f10: 1764 1f19 0064 02a1 035c 027d 207d 217c  .d...d...\.} }!|
-00005f20: 0264 0614 007c 031b 007d 227c 207c 0364  .d...|...}"| |.d
-00005f30: 1b14 0018 007c 2214 007d 207c 217c 0364  .....|"..} |!|.d
-00005f40: 1b14 0018 007c 2214 007d 217c 1564 0219  .....|"..}!|.d..
-00005f50: 006a 247d 237c 207c 236a 2564 1819 007c  .j$}#| |#j%d...|
-00005f60: 2214 0064 2614 006b 047c 217c 236a 2564  "..d&..k.|!|#j%d
-00005f70: 0219 007c 2214 0064 2614 006b 0440 007c  ...|"..d&..k.@.|
-00005f80: 2064 1b7c 2214 007c 236a 2564 1819 0014   d.|"..|#j%d....
-00005f90: 006b 0040 007c 2164 1b7c 2214 007c 236a  .k.@.|!d.|"..|#j
-00005fa0: 2564 0219 0014 006b 0040 007d 2474 0f6a  %d.....k.@.}$t.j
-00005fb0: 267c 207c 2419 007c 217c 2419 0064 2764  &| |$..|!|$..d'd
-00005fc0: 2864 2964 2a8d 0501 007c 0a64 1a6b 0290  (d)d*....|.d.k..
-00005fd0: 0472 727c 1964 2b19 007d 257c 1964 2c19  .rr|.d+..}%|.d,.
-00005fe0: 007d 267c 1fa0 237c 257c 2664 02a1 035c  .}&|..#|%|&d...\
-00005ff0: 027d 277d 287c 277c 0364 1b14 0018 007c  .}'}(|'|.d.....|
-00006000: 2214 007d 277c 287c 0364 1b14 0018 007c  "..}'|(|.d.....|
-00006010: 2214 007d 287c 277c 236a 2564 1819 007c  "..}(|'|#j%d...|
-00006020: 2214 0064 2614 006b 047c 287c 236a 2564  "..d&..k.|(|#j%d
-00006030: 0219 007c 2214 0064 2614 006b 0440 007c  ...|"..d&..k.@.|
-00006040: 2764 1b7c 2214 007c 236a 2564 1819 0014  'd.|"..|#j%d....
-00006050: 006b 0040 007c 2864 1b7c 2214 007c 236a  .k.@.|(d.|"..|#j
-00006060: 2564 0219 0014 006b 0040 007d 2974 0f6a  %d.....k.@.})t.j
-00006070: 267c 277c 2919 007c 287c 2919 0064 2764  &|'|)..|(|)..d'd
-00006080: 2d64 2e64 2f8d 0501 0074 0964 2083 0101  -d.d/....t.d ...
-00006090: 0074 0974 0b6a 0c64 3017 0083 0101 0074  .t.t.j.d0......t
-000060a0: 0964 3183 0101 0074 097c 1964 3219 0083  .d1....t.|.d2...
-000060b0: 0101 0064 337c 1964 2b19 005f 2764 337c  ...d3|.d+.._'d3|
-000060c0: 1964 2c19 005f 2774 167c 1964 2b19 007c  .d,.._'t.|.d+..|
-000060d0: 1964 2c19 0083 027d 1a7c 18a0 1c7c 1aa1  .d,....}.|...|..
-000060e0: 017d 1b7c 1b6a 1b7c 0f14 007d 1c74 0964  .}.|.j.|...}.t.d
-000060f0: 2083 0101 0074 00a0 1e74 1f7c 1a83 01a1   ....t...t.|....
-00006100: 0144 005d 407d 1d64 237d 1e74 097c 1e64  .D.]@}.d#}.t.|.d
-00006110: 24a0 057c 007c 1d7c 1964 3419 007c 1d19  $..|.|.|.d4..|..
-00006120: 007c 1964 1d19 007c 1d19 007c 1c7c 1d19  .|.d...|...|.|..
-00006130: 007c 1b6a 1b7c 1d19 00a1 0617 0083 0101  .|.j.|..........
-00006140: 0090 0471 3074 00a0 287c 21a1 017d 2a7c  ...q0t..(|!..}*|
-00006150: 247c 2a19 007d 247c 0864 356b 0290 0572  $|*..}$|.d5k...r
-00006160: 9474 297c 2a7c 2419 0083 0144 005d f85c  .t)|*|$....D.].\
-00006170: 027d 1d7d 2b74 2a7c 1764 3619 007c 2b19  .}.}+t*|.d6..|+.
-00006180: 0083 0164 37a0 057c 1764 1419 007c 2b19  ...d7..|.d...|+.
-00006190: 007c 2ba1 0217 007d 2c7c 207c 2a19 007c  .|+....},| |*..|
-000061a0: 2419 007c 1d19 007c 0517 007d 2d7c 217c  $..|...|...}-|!|
-000061b0: 2a19 007c 2419 007c 1d19 007c 0617 007d  *..|$..|...|...}
-000061c0: 2e7c 1d64 026b 0290 0572 0e74 0f6a 2b7c  .|.d.k...r.t.j+|
-000061d0: 2d7c 2e7c 2c64 3864 3964 3a8d 0501 006e  -|.|,d8d9d:....n
-000061e0: 827c 217c 2a19 007c 2419 007c 1d64 1818  .|!|*..|$..|.d..
-000061f0: 0019 007c 0617 007d 2f74 2c7c 2e7c 2f18  ...|...}/t,|.|/.
-00006200: 0083 0164 3b6b 0090 0572 407c 2e7c 0737  ...d;k...r@|.|.7
-00006210: 007d 2e7c 1d64 186b 0490 0572 7c7c 217c  .}.|.d.k...r||!|
-00006220: 2a19 007c 2419 007c 1d64 0618 0019 007c  *..|$..|.d.....|
-00006230: 0617 007d 3074 2c7c 2e7c 3018 0083 0164  ...}0t,|.|0....d
-00006240: 3c6b 0090 0572 7c7c 2e7c 0737 007d 2e74  <k...r||.|.7.}.t
-00006250: 0f6a 2b7c 2d7c 2e7c 2c64 3864 3964 3a8d  .j+|-|.|,d8d9d:.
-00006260: 0501 0090 0471 9a7c 0864 356b 0290 0672  .....q.|.d5k...r
-00006270: ce7c 0a64 1a6b 0290 0672 ce74 00a0 287c  .|.d.k...r.t..(|
-00006280: 28a1 017d 2a7c 297c 2a19 007d 2974 297c  (..}*|)|*..})t)|
-00006290: 2a7c 2919 0083 0144 0090 015d 045c 027d  *|)....D...].\.}
-000062a0: 1d7d 2b74 2a7c 1964 3d19 007c 2b19 0083  .}+t*|.d=..|+...
-000062b0: 0164 37a0 057c 1964 1d19 007c 2b19 007c  .d7..|.d...|+..|
-000062c0: 2ba1 0217 007d 2c7c 277c 2a19 007c 2919  +....},|'|*..|).
-000062d0: 007c 1d19 007c 0517 007d 2d7c 287c 2a19  .|...|...}-|(|*.
-000062e0: 007c 2919 007c 1d19 007c 0617 007c 0b18  .|)..|...|...|..
-000062f0: 007d 2e7c 1d64 026b 0290 0672 4074 0f6a  .}.|.d.k...r@t.j
-00006300: 2b7c 2d7c 2e7c 2c64 3864 2e64 3a8d 0501  +|-|.|,d8d.d:...
-00006310: 006e 8a7c 287c 2a19 007c 2919 007c 1d64  .n.|(|*..|)..|.d
-00006320: 1818 0019 007c 0617 007c 0b18 007d 2f74  .....|...|...}/t
-00006330: 2c7c 2e7c 2f18 0083 0164 3b6b 0090 0672  ,|.|/....d;k...r
-00006340: 767c 2e7c 0737 007d 2e7c 1d64 186b 0490  v|.|.7.}.|.d.k..
-00006350: 0672 b67c 287c 2a19 007c 2919 007c 1d64  .r.|(|*..|)..|.d
-00006360: 0618 0019 007c 0617 007c 0b18 007d 3074  .....|...|...}0t
-00006370: 2c7c 2e7c 3018 0083 0164 3c6b 0090 0672  ,|.|0....d<k...r
-00006380: b67c 2e7c 0737 007d 2e74 0f6a 2b7c 2d7c  .|.|.7.}.t.j+|-|
-00006390: 2e7c 2c64 3864 2e64 3a8d 0501 0090 0571  .|,d8d.d:......q
-000063a0: c674 0fa0 2d64 3ea1 0101 0074 0fa0 2e64  .t..-d>....t...d
-000063b0: 3fa1 0101 0074 0fa0 2fa1 0001 0074 0f6a  ?....t../....t.j
-000063c0: 3064 40a0 057c 007c 02a1 0264 4164 428d  0d@..|.|...dAdB.
-000063d0: 0201 0064 0053 0029 434e 7241 0000 0072  ...d.S.)CNrA...r
-000063e0: 0100 0000 7242 0000 0072 4300 0000 7244  ....rB...rC...rD
-000063f0: 0000 0072 3900 0000 724a 0000 0072 4e00  ...r9...rJ...rN.
-00006400: 0000 724f 0000 0072 4a02 0000 725d 0000  ..rO...rJ...r]..
-00006410: 0072 5e00 0000 a903 7201 0100 0072 4b02  .r^.....r....rK.
-00006420: 0000 724c 0200 00fa 060a 5468 6973 20fa  ..rL......This .
-00006430: 1e20 6669 6c65 2069 7320 616c 7265 6164  . file is alread
-00006440: 7920 646f 776e 6c6f 6164 6564 2e2e 2e72  y downloaded...r
-00006450: 0302 0000 7a1a 0a2d 2d2d 2d2d 2d2d 2d2d  ....z..---------
-00006460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00006470: 72c5 0100 0029 0372 db01 0000 72dc 0100  r....).r....r...
-00006480: 0072 dd01 0000 da08 5256 5f56 414c 5545  .r......RV_VALUE
-00006490: a902 72c7 0100 0072 c701 0000 7276 0000  ..r....r....rv..
-000064a0: 0072 6200 0000 7269 0000 0072 0a02 0000  .rb...ri...r....
-000064b0: 7240 0000 0072 4900 0000 2901 da06 7261  r@...rI...)...ra
-000064c0: 6469 7573 da08 5665 6c6f 6369 7479 da04  dius..Velocity..
-000064d0: 5241 5f64 da05 4445 435f 6472 c700 0000  RA_d..DEC_dr....
-000064e0: 7a14 0a50 726f 6a65 6374 6564 2044 6973  z..Projected Dis
-000064f0: 7461 6e63 6573 72ca 0100 00fa 1b50 726f  tancesr......Pro
-00006500: 7965 6374 6564 2064 6973 7461 6e63 6520  yected distance 
-00006510: 6265 7477 6565 6e20 7a3b 7b7d 2061 6e64  between z;{} and
-00006520: 2028 7b7d 2920 7b7d 2028 7b7d 206b 6d2f   ({}) {} ({} km/
-00006530: 7329 2069 7320 3d20 7b3a 2e31 667d 5c2c  s) is = {:.1f}\,
-00006540: 6b70 6320 287b 3a2e 3166 7d24 5c61 7263  kpc ({:.1f}$\arc
-00006550: 7365 6324 29da 074d 4149 4e5f 4944 e700  sec$)..MAIN_ID..
-00006560: 0000 0000 00e0 bf72 3a00 0000 7276 0100  .......r:...rv..
-00006570: 00da 0167 a903 da01 73da 0a66 6163 6563  ...g....s..facec
-00006580: 6f6c 6f72 73da 0a65 6467 6563 6f6c 6f72  olors..edgecolor
-00006590: 73da 0252 41da 0344 4543 7228 0100 00da  s..RA..DECr(....
-000065a0: 0172 2903 7263 0200 00da 066d 6172 6b65  .r).rc.....marke
-000065b0: 72da 0563 6f6c 6f72 7a23 0a4e 4544 2054  r..colorz#.NED T
-000065c0: 6162 6c65 2028 4e6f 2072 6563 7472 6963  able (No rectric
-000065d0: 7469 6f6e 2069 6e20 5672 6164 297a 253d  tion in Vrad)z%=
-000065e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000065f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006600: 3d3d 3d0a 2906 fa0b 4f62 6a65 6374 204e  ===.)...Object N
-00006610: 616d 6572 6602 0000 7267 0200 00da 0454  amerf...rg.....T
-00006620: 7970 6572 5b02 0000 da08 5265 6473 6869  yper[.....Redshi
-00006630: 6674 da03 6465 6772 6b02 0000 729c 0000  ft..degrk...r...
-00006640: 00da 054f 5459 5045 7a11 2056 7261 643d  ...OTYPEz. Vrad=
-00006650: 7b3a 2e30 667d 2028 7b7d 2972 5402 0000  {:.0f} ({})rT...
-00006660: da01 77a9 0272 0202 0000 726a 0200 0072  ..w..r....rj...r
-00006670: 0002 0000 e93c 0000 0072 6c02 0000 7207  .....<...rl...r.
-00006680: 0200 0072 0802 0000 7a22 696d 6167 6573  ...r....z"images
-00006690: 2f7b 7d5f 7369 6d62 6164 5f7b 7d6b 7063  /{}_simbad_{}kpc
-000066a0: 5f6d 6172 6b65 7273 2e70 6e67 727c 0000  _markers.pngr|..
-000066b0: 0072 7d00 0000 2931 7225 0000 0072 c800  .r}...)1r%...r..
-000066c0: 0000 72b7 0000 0072 c900 0000 72ca 0000  ..r....r....r...
-000066d0: 0072 6400 0000 72d4 0000 0072 d500 0000  .rd...r....r....
-000066e0: 72d6 0000 0072 cb00 0000 7253 0200 0072  r....r....rS...r
-000066f0: 1900 0000 72d2 0000 0072 0300 0000 72e4  ....r....r....r.
-00006700: 0000 0072 e600 0000 721c 0200 0072 dd00  ...r....r....r..
-00006710: 0000 7217 0200 0072 e700 0000 72e8 0000  ..r....r....r...
-00006720: 0072 2602 0000 7209 0000 00da 0175 726e  .r&...r......urn
-00006730: 0200 0072 0700 0000 da0c 7175 6572 795f  ...r......query_
-00006740: 7265 6769 6f6e da06 6172 6373 6563 da0a  region..arcsec..
-00006750: 7365 7061 7261 7469 6f6e 72cc 0000 0072  separationr....r
-00006760: 1e02 0000 72e3 0000 0072 0800 0000 da03  ....r....r......
-00006770: 5743 53da 0668 6561 6465 72da 0d61 6c6c  WCS..header..all
-00006780: 5f77 6f72 6c64 3270 6978 72e5 0000 0072  _world2pixr....r
-00006790: a601 0000 da07 7363 6174 7465 72da 0475  ......scatter..u
-000067a0: 6e69 7472 f900 0000 72fb 0000 0072 da00  nitr....r....r..
-000067b0: 0000 7223 0200 00da 0361 6273 7227 0200  ..r#.....absr'..
-000067c0: 0072 2802 0000 7224 0200 0072 e900 0000  .r(...r$...r....
-000067d0: 2931 72c2 0000 0072 ff00 0000 7201 0100  )1r....r....r...
-000067e0: 0072 4b02 0000 724c 0200 0072 e901 0000  .rK...rL...r....
-000067f0: 72ea 0100 0072 eb01 0000 da08 6c61 6265  r....r......labe
-00006800: 6c74 7874 72dc 0100 00da 086e 6564 5f70  ltxtr......ned_p
-00006810: 6c6f 74da 0a64 656c 7461 795f 6e65 6472  lot..deltay_nedr
-00006820: 0901 0000 7243 0200 0072 b300 0000 7244  ....rC...r....rD
-00006830: 0200 0072 4502 0000 724d 0200 0072 4e00  ...rE...rM...rN.
-00006840: 0000 724f 0000 0072 d500 0000 7252 0200  ..rO...r....rR..
-00006850: 0072 5102 0000 72e7 0100 00da 0867 616c  .rQ...r......gal
-00006860: 636f 6f72 64da 0974 6162 6c65 5f6e 6564  coord..table_ned
-00006870: da04 736b 7963 da03 7365 70da 0773 6570  ..skyc..sep..sep
-00006880: 5f6b 7063 7233 0100 00da 0374 7874 7270  _kpcr3.....txtrp
-00006890: 0200 00da 0358 6763 da03 5967 63da 0573  .....Xgc..Ygc..s
-000068a0: 6369 6d61 722e 0000 00da 0463 6f6e 64da  cimar......cond.
-000068b0: 066e 6564 5f72 61da 076e 6564 5f64 6563  .ned_ra..ned_dec
-000068c0: da07 5867 635f 6e65 64da 0759 6763 5f6e  ..Xgc_ned..Ygc_n
-000068d0: 6564 da08 636f 6e64 5f6e 6564 da05 6f72  ed..cond_ned..or
-000068e0: 6465 6dda 0469 6e64 67da 0574 6578 746c  dem..indg..textl
-000068f0: da04 7870 6f73 da04 7970 6f73 da05 7970  ..xpos..ypos..yp
-00006900: 6f73 62da 0679 706f 7362 6272 2f00 0000  osb..yposbbr/...
-00006910: 722f 0000 0072 3000 0000 da10 7369 6d62  r/...r0.....simb
-00006920: 6164 5f74 6875 6d62 6e61 696c 4204 0000  ad_thumbnailB...
-00006930: 7328 0100 0000 061a 010c 0208 0118 020c  s(..............
-00006940: 0108 020c 010c 020c 010c 0110 0108 0102  ................
-00006950: 0002 ff08 0316 020a 0102 ff06 020a 0102  ................
-00006960: ff06 040e 010a 0102 0002 ff06 0210 040c  ................
-00006970: 0120 0216 030a 0118 0110 0212 010a 020a  . ..............
-00006980: 0208 010e 0108 0112 0204 0108 0102 0002  ................
-00006990: 000a 000a 0006 0108 fe0c 0510 011a 020c  ................
-000069a0: 0210 0110 020a 022a 0114 ff02 0114 ff04  .......*........
-000069b0: 0314 0102 ff06 040a 0208 0108 0212 0210  ................
-000069c0: 0110 0214 0114 ff02 0214 fe02 0314 fd04  ................
-000069d0: 0510 0102 0002 0002 ff06 0208 010e 0108  ................
-000069e0: 010c 020a 010a 0112 020a 020a 0208 0112  ................
-000069f0: 0104 0108 0102 0002 000a 000a 0106 0008  ................
-00006a00: fe0c 040a 0108 030a 0114 0112 010a 0002  ................
-00006a10: ff06 0314 0114 020a 0116 0318 0112 0208  ................
-00006a20: 010a 0118 0112 0108 0218 0214 010a 0108  ................
-00006a30: 0116 0112 010a 0002 ff06 0314 0118 020a  ................
-00006a40: 0116 031c 0112 0208 010a 011c 0112 0108  ................
-00006a50: 0218 020a 010a 0108 010e 0102 ff72 9602  .............r..
-00006a60: 0000 5463 1300 0000 0000 0000 0000 0000  ..Tc............
-00006a70: 3400 0000 1000 0000 4300 0000 73ee 0a00  4.......C...s...
-00006a80: 0074 00a0 017c 0164 0119 007c 006b 02a1  .t...|.d...|.k..
-00006a90: 0164 0219 0064 0219 007d 137c 0164 0319  .d...d...}.|.d..
-00006aa0: 007c 1319 0074 021b 007d 1474 00a0 0374  .|...t...}.t...t
-00006ab0: 00a0 0464 04a1 01a1 017c 1414 0064 0514  ...d.....|...d..
-00006ac0: 007d 157c 1164 066b 0272 5064 077d 166e  .}.|.d.k.rPd.}.n
-00006ad0: 1a7c 0364 0814 007c 151b 0064 091b 007d  .|.d...|...d...}
-00006ae0: 1674 0564 0a7c 1683 0201 007c 037c 151b  .t.d.|.....|.|..
-00006af0: 007c 161b 0064 0814 007d 177c 1064 0b6b  .|...d...}.|.d.k
-00006b00: 0272 9674 0574 066a 0764 0ca0 087c 15a1  .r.t.t.j.d...|..
-00006b10: 0117 0083 0101 007c 0f64 0b6b 0290 0172  .......|.d.k...r
-00006b20: 2074 0574 066a 0964 0d17 0083 0101 0074   t.t.j.d.......t
-00006b30: 0564 0e83 0101 0074 0a6a 0ba0 0c74 0a6a  .d.....t.j...t.j
-00006b40: 0ba0 0d74 0ea1 01a1 017d 1874 0f6a 107c  ...t.....}.t.j.|
-00006b50: 1864 0f17 0064 1064 118d 027d 1974 057c  .d...d.d...}.t.|
-00006b60: 1964 1219 0074 00a0 017c 1964 0119 007c  .d...t...|.d...|
-00006b70: 006b 02a1 0164 0219 0019 0083 0101 0074  .k...d.........t
-00006b80: 057c 1964 1319 0074 00a0 017c 1964 0119  .|.d...t...|.d..
-00006b90: 007c 006b 02a1 0164 0219 0019 0083 0101  .|.k...d........
-00006ba0: 007c 0b90 0372 d274 11a0 1074 12a1 017d  .|...r.t...t...}
-00006bb0: 1a74 137c 0464 1419 007c 0519 007c 0464  .t.|.d...|...|.d
-00006bc0: 1519 007c 0519 0083 027d 1b7c 1b64 0219  ...|.....}.|.d..
-00006bd0: 00a0 147c 1b64 1664 0085 0219 00a1 017d  ...|.d.d.......}
-00006be0: 1c7c 1c6a 157c 1514 007d 1d74 00a0 1674  .|.j.|...}.t...t
-00006bf0: 177c 1b64 1664 0085 0219 0083 01a1 0144  .|.d.d.........D
-00006c00: 005d 3e7d 1e74 066a 1864 1717 007d 1f74  .]>}.t.j.d...}.t
-00006c10: 057c 1f64 18a0 087c 0664 0219 007c 067c  .|.d...|.d...|.|
-00006c20: 1e64 1617 0019 007c 1d7c 1e19 007c 1c6a  .d.....|.|...|.j
-00006c30: 157c 1e19 00a1 0417 0083 0101 0090 0171  .|.............q
-00006c40: 8074 0564 1983 0101 0074 1974 1a7c 057c  .t.d.....t.t.|.|
-00006c50: 0683 0283 0144 0090 015d e85c 027d 1e5c  .....D...].\.}.\
-00006c60: 027d 207d 2174 177c 1a83 0164 026b 0290  .} }!t.|...d.k..
-00006c70: 0172 fa7c 1aa0 1ba1 0001 0074 1c7c 1a64  .r.|.......t.|.d
-00006c80: 1a19 007c 216b 0283 0190 0272 3e74 0574  ...|!k.....r>t.t
-00006c90: 066a 0764 1b7c 219b 0064 1c9d 0317 0083  .j.d.|!..d......
-00006ca0: 0101 0074 00a0 017c 1a64 1a19 007c 216b  ...t...|.d...|!k
-00006cb0: 02a1 0164 0219 0064 0219 007d 226e 2c74  ...d...d...}"n,t
-00006cc0: 0574 066a 0764 1da0 087c 21a1 0117 0083  .t.j.d...|!.....
-00006cd0: 0101 007c 1aa0 1ba1 0001 0064 1e7d 227c  ...|.......d.}"|
-00006ce0: 217c 1a64 1a19 007c 223c 007c 0464 1419  !|.d...|"<.|.d..
-00006cf0: 007c 2019 007c 1a64 1f19 007c 223c 007c  .| ..|.d...|"<.|
-00006d00: 0464 1519 007c 2019 007c 1a64 2019 007c  .d...| ..|.d ..|
-00006d10: 223c 007c 0464 2119 007c 2019 007c 1a64  "<.|.d!..| ..|.d
-00006d20: 2219 007c 223c 007c 0464 2319 007c 2019  "..|"<.|.d#..| .
-00006d30: 007c 1a64 2419 007c 223c 007c 0464 2519  .|.d$..|"<.|.d%.
-00006d40: 007c 2019 007c 1a64 2619 007c 223c 007c  .| ..|.d&..|"<.|
-00006d50: 0c64 0b6b 0290 0272 e464 167c 1a64 2719  .d.k...r.d.|.d'.
-00006d60: 007c 223c 007c 0c64 066b 0290 0272 fa64  .|"<.|.d.k...r.d
-00006d70: 027c 1a64 2719 007c 223c 0074 177c 0583  .|.d'..|"<.t.|..
-00006d80: 0164 086b 0490 0372 1464 167c 1a64 2819  .d.k...r.d.|.d(.
-00006d90: 007c 223c 007c 0d64 0b6b 0290 0372 2a64  .|"<.|.d.k...r*d
-00006da0: 167c 1a64 2819 007c 223c 007c 0d64 066b  .|.d(..|"<.|.d.k
-00006db0: 0290 0372 4064 027c 1a64 2819 007c 223c  ...r@d.|.d(..|"<
-00006dc0: 0074 177c 0583 0164 166b 0490 0372 787c  .t.|...d.k...rx|
-00006dd0: 0e64 026b 0290 0372 6a74 177c 0583 017c  .d.k...rjt.|...|
-00006de0: 1a64 2919 007c 223c 006e 0c7c 0e7c 1a64  .d)..|"<.n.|.|.d
-00006df0: 2919 007c 223c 006e 287c 0e64 026b 0290  )..|"<.n(|.d.k..
-00006e00: 0372 9474 177c 0583 017c 1a64 2919 007c  .r.t.|...|.d)..|
-00006e10: 223c 006e 0c7c 0e7c 1a64 2919 007c 223c  "<.n.|.|.d)..|"<
-00006e20: 007c 1e64 026b 0490 0172 d67c 1d7c 1e64  .|.d.k...r.|.|.d
-00006e30: 1618 0019 007c 1a64 2a19 007c 223c 0090  .....|.d*..|"<..
-00006e40: 0171 d674 116a 1d7c 1a74 1264 2b64 2c8d  .q.t.j.|.t.d+d,.
-00006e50: 0301 0064 0264 006c 1e7d 2364 2d7c 236a  ...d.d.l.}#d-|#j
-00006e60: 1f64 2e3c 0064 2f7c 236a 1f64 303c 0064  .d.<.d/|#j.d0<.d
-00006e70: 317c 236a 1f64 323c 0064 337c 236a 1f64  1|#j.d2<.d3|#j.d
-00006e80: 343c 0064 317c 236a 1f64 353c 0064 337c  4<.d1|#j.d5<.d3|
-00006e90: 236a 1f64 363c 0064 317c 236a 1f64 373c  #j.d6<.d1|#j.d7<
-00006ea0: 0064 317c 236a 1f64 383c 007c 1164 066b  .d1|#j.d8<.|.d.k
-00006eb0: 0290 0572 7e64 39a0 087c 007c 03a1 027d  ...r~d9..|.|...}
-00006ec0: 247c 0364 3a6b 0290 0472 5664 3b7c 0017  $|.d:k...rVd;|..
-00006ed0: 0064 3c17 007d 2474 20a0 217c 24a1 017d  .d<..}$t .!|$..}
-00006ee0: 2564 3da0 087c 007c 03a1 027d 2464 3ea0  %d=..|.|...}$d>.
-00006ef0: 087c 007c 127c 03a1 037d 2674 0a6a 0ba0  .|.|.|...}&t.j..
-00006f00: 227c 24a1 0190 0473 a074 0a6a 0ba0 227c  "|$....s.t.j.."|
-00006f10: 26a1 0190 0472 e47c 1264 3f6b 0290 0472  &....r.|.d?k...r
-00006f20: e474 0574 066a 1864 407c 249b 0064 419d  .t.t.j.d@|$..dA.
-00006f30: 0317 0083 0101 007a 1274 23a0 247c 24a1  .......z.t#.$|$.
-00006f40: 0164 1619 007d 2757 006e 1a01 0001 0001  .d...}'W.n......
-00006f50: 0074 23a0 247c 26a1 0164 1619 007d 2759  .t#.$|&..d...}'Y
-00006f60: 006e 0258 0074 0a6a 0ba0 227c 24a1 0190  .n.X.t.j.."|$...
-00006f70: 0573 5074 0a6a 0ba0 227c 26a1 0190 0573  .sPt.j.."|&....s
-00006f80: 507c 1264 3f6b 0290 0572 5074 0574 066a  P|.d?k...rPt.t.j
-00006f90: 1864 427c 249b 0064 439d 0317 0083 0101  .dB|$..dC.......
-00006fa0: 007c 026a 257c 0164 1f19 007c 1319 007c  .|.j%|.d...|...|
-00006fb0: 0164 2019 007c 1319 0074 267c 1783 017c  .d ..|...t&|...|
-00006fc0: 127c 2664 0264 4485 0219 0064 458d 0501  .|&d.dD....dE...
-00006fd0: 0074 0a6a 0ba0 227c 26a1 0190 0572 fe74  .t.j.."|&....r.t
-00006fe0: 23a0 247c 26a1 0164 1619 007d 2774 0564  #.$|&..d...}'t.d
-00006ff0: 407c 269b 0064 419d 0383 0101 006e 8064  @|&..dA......n.d
-00007000: 46a0 087c 007c 03a1 027d 2474 0a6a 0ba0  F..|.|...}$t.j..
-00007010: 227c 24a1 0190 0573 bc74 0564 427c 249b  "|$....s.t.dB|$.
-00007020: 0064 439d 0383 0101 0074 277c 007c 017c  .dC......t'|.|.|
-00007030: 0364 0964 0964 478d 0501 006e 1674 0574  .d.d.dG....n.t.t
-00007040: 066a 0764 487c 249b 0064 499d 0317 0083  .j.dH|$..dI.....
-00007050: 0101 0074 23a0 2464 46a0 087c 007c 03a1  ...t#.$dF..|.|..
-00007060: 02a1 0164 0219 007d 2774 20a0 2164 4aa0  ...d...}'t .!dJ.
-00007070: 087c 007c 03a1 02a1 017d 2564 097d 177c  .|.|.....}%d.}.|
-00007080: 276a 2864 1619 007d 1774 00a0 2964 1664  'j(d...}.t..)d.d
-00007090: 1e64 1e64 1667 04a1 017c 1714 0064 4b14  .d.d.g...|...dK.
-000070a0: 007c 1614 007d 2874 206a 2a64 4c64 4d8d  .|...}(t j*dLdM.
-000070b0: 0101 0074 206a 2b7c 257c 2864 4e8d 0201  ...t j+|%|(dN...
-000070c0: 0074 2c6a 2d64 4b7c 1714 0064 4b7c 1714  .t,j-dK|...dK|..
-000070d0: 0067 027c 1664 4f7c 151b 0064 5064 5164  .g.|.dO|...dPdQd
-000070e0: 5264 5364 5464 5464 5564 5664 5764 1664  RdSdTdTdUdVdWd.d
-000070f0: 0064 588d 0e01 0074 2ea0 2f7c 276a 30a1  .dX....t../|'j0.
-00007100: 017d 297c 0464 006b 0890 0672 9064 0053  .})|.d.k...r.d.S
-00007110: 007c 29a0 317c 0464 1419 007c 0464 1519  .|).1|.d...|.d..
-00007120: 0064 02a1 035c 027d 2a7d 2b7c 2a7c 1614  .d...\.}*}+|*|..
-00007130: 007c 1764 4b14 007c 1614 0018 0064 1e14  .|.dK..|.....d..
-00007140: 007d 2a7c 2b7c 1614 007c 1764 4b14 007c  .}*|+|...|.dK..|
-00007150: 1614 0018 007d 2b7c 2a7c 276a 2864 1619  .....}+|*|'j(d..
-00007160: 0064 5914 007c 1614 006b 047c 2b7c 276a  .dY..|...k.|+|'j
-00007170: 2864 0219 0064 5914 007c 1614 006b 0440  (d...dY..|...k.@
-00007180: 007c 2a64 4b7c 1614 007c 276a 2864 1619  .|*dK|...|'j(d..
-00007190: 0014 006b 0040 007c 2b64 4b7c 1614 007c  ...k.@.|+dK|...|
-000071a0: 276a 2864 0219 0014 006b 0040 007d 2c74  'j(d.....k.@.},t
-000071b0: 00a0 327c 2ba1 017d 2d7c 0564 006b 0890  ..2|+..}-|.d.k..
-000071c0: 0872 8274 206a 337c 2a7c 2c19 007c 2b7c  .r.t j3|*|,..|+|
-000071d0: 2c19 0064 3a64 5a64 5b64 5c8d 0501 0074  ,..d:dZd[d\....t
-000071e0: 197c 2d7c 2c19 0083 0144 005d ee5c 027d  .|-|,....D.].\.}
-000071f0: 1e7d 2e7c 0464 5d19 007c 2e19 0064 5ea0  .}.|.d]..|...d^.
-00007200: 087c 0464 2119 007c 2e19 007c 2e7c 0464  .|.d!..|...|.|.d
-00007210: 5f19 007c 2e19 00a1 0317 007d 2f7c 2a7c  _..|.......}/|*|
-00007220: 2d19 007c 2c19 007c 1e19 007c 0717 007d  -..|,..|...|...}
-00007230: 307c 2b7c 2d19 007c 2c19 007c 1e19 007c  0|+|-..|,..|...|
-00007240: 0817 007d 317c 1e64 026b 0290 0772 e474  ...}1|.d.k...r.t
-00007250: 206a 347c 307c 317c 2f64 6064 5764 618d   j4|0|1|/d`dWda.
-00007260: 0501 006e 727c 2b7c 2d19 007c 2c19 007c  ...nr|+|-..|,..|
-00007270: 1e64 1618 0019 007d 327c 317c 3218 0064  .d.....}2|1|2..d
-00007280: 626b 0090 0872 0e7c 317c 0937 007d 317c  bk...r.|1|.7.}1|
-00007290: 1e64 166b 0490 0872 427c 2b7c 2d19 007c  .d.k...rB|+|-..|
-000072a0: 2c19 007c 1e64 0818 0019 007d 337c 317c  ,..|.d.....}3|1|
-000072b0: 3318 0064 636b 0090 0872 427c 317c 0937  3..dck...rB|1|.7
-000072c0: 007d 3174 206a 347c 307c 317c 2f64 6064  .}1t j4|0|1|/d`d
-000072d0: 5764 618d 0501 0090 0771 6a74 20a0 35a1  Wda......qjt .5.
-000072e0: 0001 0074 20a0 3664 64a1 0101 0074 20a0  ...t .6dd....t .
-000072f0: 3764 65a1 0101 0074 20a0 38a1 0001 0090  7de....t .8.....
-00007300: 026e 6874 206a 337c 2a7c 0519 007c 2b7c  .nht j3|*|...|+|
-00007310: 0519 0064 3a64 5a64 5b64 5c8d 0501 0074  ...d:dZd[d\....t
-00007320: 197c 0583 0144 005d b45c 027d 1e7d 2e7c  .|...D.].\.}.}.|
-00007330: 067c 1e19 007d 2f7c 2a7c 2e19 007c 0717  .|...}/|*|...|..
-00007340: 007d 307c 2b7c 2e19 007c 0817 007d 317c  .}0|+|...|...}1|
-00007350: 1e64 026b 0290 0872 ee74 206a 347c 307c  .d.k...r.t j4|0|
-00007360: 317c 2f64 6064 5764 618d 0501 006e 6a7c  1|/d`dWda....nj|
-00007370: 2b7c 0519 007c 1e64 1618 0019 007d 327c  +|...|.d.....}2|
-00007380: 317c 3218 0064 626b 0090 0972 147c 317c  1|2..dbk...r.|1|
-00007390: 0937 007d 317c 1e64 166b 0490 0972 447c  .7.}1|.d.k...rD|
-000073a0: 2b7c 0519 007c 1e64 0818 0019 007d 337c  +|...|.d.....}3|
-000073b0: 317c 3318 0064 636b 0090 0972 447c 317c  1|3..dck...rD|1|
-000073c0: 0937 007d 3174 206a 347c 307c 317c 2f64  .7.}1t j4|0|1|/d
-000073d0: 6064 5764 618d 0501 0090 0871 a674 20a0  `dWda......q.t .
-000073e0: 35a1 0001 0074 20a0 3664 64a1 0101 0074  5....t .6dd....t
-000073f0: 20a0 3764 65a1 0101 007c 0a64 006b 0990   .7de....|.d.k..
-00007400: 0972 a474 0564 66a0 087c 00a1 0183 0101  .r.t.df..|......
-00007410: 0074 206a 3964 67a0 087c 00a1 0164 6864  .t j9dg..|...dhd
-00007420: 698d 0201 007c 29a0 317c 0464 1419 0064  i....|).1|.d...d
-00007430: 0219 007c 0464 1519 0064 0219 0064 02a1  ...|.d...d...d..
-00007440: 035c 027d 2a7d 2b7c 1164 0b6b 0290 0972  .\.}*}+|.d.k...r
-00007450: de64 46a0 087c 007c 03a1 027d 246e 0c64  .dF..|.|...}$n.d
-00007460: 3da0 087c 007c 03a1 027d 2474 0574 066a  =..|.|...}$t.t.j
-00007470: 3a64 6a17 0083 0101 0074 0564 0e83 0101  :dj......t.d....
-00007480: 0074 0564 6b83 0101 0074 0564 6c83 0101  .t.dk....t.dl...
-00007490: 0074 0564 6da0 087c 24a1 0183 0101 0074  .t.dm..|$......t
-000074a0: 0564 6e83 0101 0074 0564 6fa0 087c 0464  .dn....t.do..|.d
-000074b0: 1419 0064 0219 007c 0464 1519 0064 0219  ...d...|.d...d..
-000074c0: 00a1 0283 0101 0074 0564 70a0 087c 2a7c  .......t.dp..|*|
-000074d0: 16a1 0283 0101 0074 0564 71a0 087c 2b7c  .......t.dq..|+|
-000074e0: 16a1 0283 0101 0074 0564 7283 0101 0074  .......t.dr....t
-000074f0: 0564 6b83 0101 0074 0564 7383 0101 0074  .dk....t.ds....t
-00007500: 0564 74a0 087c 00a1 0183 0101 0074 0564  .dt..|.......t.d
-00007510: 7583 0101 0074 0564 7683 0101 0074 0564  u....t.dv....t.d
-00007520: 7783 0101 0074 0564 6b83 0101 0074 0564  w....t.dk....t.d
-00007530: 7883 0101 0074 0564 7983 0101 0074 0564  x....t.dy....t.d
-00007540: 0ca0 087c 15a1 0183 0101 0074 0564 7a83  ...|.......t.dz.
-00007550: 0101 0074 0564 7b83 0101 0074 0564 7c83  ...t.d{....t.d|.
-00007560: 0101 0074 0564 7d83 0101 0064 0053 0029  ...t.d}....d.S.)
-00007570: 7e4e 7241 0000 0072 0100 0000 7242 0000  ~NrA...r....rB..
-00007580: 0072 4300 0000 7244 0000 0072 c801 0000  .rC...rD...r....
-00007590: 7248 0000 0072 3900 0000 720f 0200 007a  rH...r9...r....z
-000075a0: 1953 696d 6261 6420 7363 616c 6520 7069  .Simbad scale pi
-000075b0: 782f 6172 6373 6563 203a 7240 0000 007a  x/arcsec :r@...z
-000075c0: 0c61 7263 5f6b 7063 203d 207b 7d72 c901  .arc_kpc = {}r..
-000075d0: 0000 72ca 0100 0072 cb01 0000 7204 0000  ..r....r....r...
-000075e0: 0072 6300 0000 72cc 0100 0072 cf01 0000  .rc...r....r....
-000075f0: 725c 0200 0072 5d02 0000 7269 0000 0072  r\...r]...ri...r
-00007600: 5e02 0000 7a2c 7b7d 2061 6e64 207b 7d20  ^...z,{} and {} 
-00007610: 6973 203d 207b 3a2e 3166 7d5c 2c6b 7063  is = {:.1f}\,kpc
-00007620: 2028 7b3a 2e31 667d 245c 6172 6373 6563   ({:.1f}$\arcsec
-00007630: 2429 72c7 0000 0072 c200 0000 7a08 526f  $)r....r....z.Ro
-00007640: 7720 666f 7220 7a0c 2077 6173 2075 7064  w for z. was upd
-00007650: 6174 6564 7a16 526f 7720 7761 7320 6372  atedz.Row was cr
-00007660: 6561 7465 6420 666f 7220 7b7d 7262 0000  eated for {}rb..
-00007670: 0072 4e00 0000 724f 0000 0072 5802 0000  .rN...rO...rX...
-00007680: 72c3 0000 00da 075a 5f56 414c 5545 72c5  r......Z_VALUEr.
-00007690: 0000 00da 0a4d 4f52 5048 5f54 5950 45da  .....MORPH_TYPE.
-000076a0: 0a6d 6f72 7068 5f74 7970 657a 0f49 7473  .morph_typez.Its
-000076b0: 5f63 6f6e 7369 6465 7265 643f 7a0a 4974  _considered?z.It
-000076c0: 735f 6772 6f75 703f da08 4e6d 656d 6265  s_group?..Nmembe
-000076d0: 7273 da09 445f 746f 5f6d 6169 6e54 7292  rs..D_to_mainTr.
-000076e0: 0000 0072 f101 0000 72f2 0100 0072 5e01  ...r....r....r^.
-000076f0: 0000 72f3 0100 0072 f401 0000 72f5 0100  ..r....r....r...
-00007700: 0072 e101 0000 72f6 0100 0072 f701 0000  .r....r....r....
-00007710: 72f8 0100 0072 f901 0000 72fa 0100 0072  r....r....r....r
-00007720: de01 0000 723a 0000 0072 d301 0000 72d4  ....r:...r....r.
-00007730: 0100 0072 5900 0000 725a 0000 0072 3c00  ...rY...rZ...r<.
-00007740: 0000 725b 0000 0072 5c00 0000 725d 0000  ..r[...r\...r]..
-00007750: 0072 5e00 0000 725f 0000 0072 6000 0000  .r^...r_...r`...
-00007760: 724a 0200 0072 5502 0000 7256 0200 0072  rJ...rU...rV...r
-00007770: 5702 0000 7203 0200 0072 4900 0000 7259  W...r....rI...rY
-00007780: 0200 0072 7600 0000 720a 0200 0072 c701  ...rv...r....r..
-00007790: 0000 7a06 3130 206b 7063 da02 3132 726a  ..z.10 kpc..12rj
-000077a0: 0100 0067 0000 0000 0000 2040 7232 0000  ...g...... @r2..
-000077b0: 0067 3333 3333 3333 f33f 7a02 772d 7270  .g333333.?z.w-rp
-000077c0: 0200 0029 0a72 7501 0000 726c 0100 0072  ...).ru...rl...r
-000077d0: 6d01 0000 726e 0100 0072 6f01 0000 7270  m...rn...ro...rp
-000077e0: 0100 0072 7101 0000 7272 0100 0072 7301  ...rq...rr...rs.
-000077f0: 0000 7274 0100 0072 6002 0000 7276 0100  ..rt...r`...rv..
-00007800: 0072 6102 0000 7262 0200 0072 6f02 0000  .ra...rb...ro...
-00007810: 7a1a 2056 7261 643d 7b3a 2e30 667d 2028  z. Vrad={:.0f} (
-00007820: 7b7d 2920 423d 7b3a 2e31 667d da06 464c  {}) B={:.1f}..FL
-00007830: 5558 5f42 7254 0200 0072 7102 0000 7200  UX_BrT...rq...r.
-00007840: 0200 0072 7202 0000 7277 0100 0072 7801  ...rr...rw...rx.
-00007850: 0000 7a1f 0a53 6176 696e 6720 6669 6775  ..z..Saving figu
-00007860: 7265 2069 6e20 696d 6167 6573 2f7b 7d2e  re in images/{}.
-00007870: 706e 677a 0d69 6d61 6765 732f 7b7d 2e70  pngz.images/{}.p
-00007880: 6e67 727c 0000 0072 7d00 0000 7a2a 0a49  ngr|...r}...z*.I
-00007890: 6e20 6361 7365 2020 746f 2061 6464 206d  n case  to add m
-000078a0: 616e 7561 6c6c 7920 7468 6520 636f 6f72  anually the coor
-000078b0: 6469 6e61 7465 733a da01 0a7a 1b66 726f  dinates:...z.fro
-000078c0: 6d20 6173 7472 6f70 792e 7763 7320 696d  m astropy.wcs im
-000078d0: 706f 7274 2077 6373 7a18 696d 6120 3d20  port wcsz.ima = 
-000078e0: 6669 7473 2e6f 7065 6e28 277b 7d27 295b  fits.open('{}')[
-000078f0: 315d 7a18 7720 3d20 2077 6373 2e57 4353  1]z.w =  wcs.WCS
-00007900: 2869 6d61 2e68 6561 6465 7229 7a27 636f  (ima.header)z'co
-00007910: 6f72 645f 6120 3d20 536b 7943 6f6f 7264  ord_a = SkyCoord
-00007920: 2827 7b7d 207b 7d27 2c20 756e 6974 3d75  ('{} {}', unit=u
-00007930: 2e64 6567 297a 2e63 6f6f 7264 5f62 203d  .deg)z.coord_b =
-00007940: 2077 2e61 6c6c 5f70 6978 3277 6f72 6c64   w.all_pix2world
-00007950: 287b 7d20 2b20 6465 6c74 615f 7261 2f7b  ({} + delta_ra/{
-00007960: 7d2a 2d31 2c7a 2f20 2020 2020 2020 2020  }*-1,z/         
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 207b 7d20 2b20 6465 6c74 615f 6465 632f   {} + delta_dec/
-00007990: 7b7d 2c20 3029 7a36 7072 696e 7420 2822  {}, 0)z6print ("
-000079a0: 7b3a 2e37 667d 207b 3a2e 3766 7d22 2e66  {:.7f} {:.7f}".f
-000079b0: 6f72 6d61 7428 636f 6f72 645f 625b 305d  ormat(coord_b[0]
-000079c0: 2c20 636f 6f72 645f 625b 315d 2929 7a34  , coord_b[1]))z4
-000079d0: 7461 625f 7072 6f3d 5461 626c 652e 7265  tab_pro=Table.re
-000079e0: 6164 2827 7072 6f70 6572 7469 6573 2e64  ad('properties.d
-000079f0: 6174 272c 2066 6f72 6d61 743d 2761 7363  at', format='asc
-00007a00: 6969 2729 7a2d 696e 645f 6720 3d20 6e70  ii')z-ind_g = np
-00007a10: 2e77 6865 7265 2874 6162 5f70 726f 5b27  .where(tab_pro['
-00007a20: 4741 4c27 5d3d 3d27 7b7d 4227 295b 305d  GAL']=='{}B')[0]
-00007a30: 5b30 5d7a 2370 7269 6e74 2028 2769 6e64  [0]z#print ('ind
-00007a40: 6578 206f 6620 6761 6c61 7879 203d 2027  ex of galaxy = '
-00007a50: 2c20 696e 645f 6729 7a21 7461 625f 7072  , ind_g)z!tab_pr
-00007a60: 6f5b 2772 6127 5d5b 696e 645f 675d 203d  o['ra'][ind_g] =
-00007a70: 2063 6f6f 7264 5f62 5b30 5d7a 2274 6162   coord_b[0]z"tab
-00007a80: 5f70 726f 5b27 6465 6327 5d5b 696e 645f  _pro['dec'][ind_
-00007a90: 675d 203d 2063 6f6f 7264 5f62 5b31 5d7a  g] = coord_b[1]z
-00007aa0: 3663 6f6f 7264 5f62 203d 2053 6b79 436f  6coord_b = SkyCo
-00007ab0: 6f72 6428 636f 6f72 645f 625b 305d 2c20  ord(coord_b[0], 
-00007ac0: 636f 6f72 645f 625b 315d 2c20 756e 6974  coord_b[1], unit
-00007ad0: 3d75 2e64 6567 297a 2173 6570 203d 2063  =u.deg)z!sep = c
-00007ae0: 6f6f 7264 5f61 2e73 6570 6172 6174 696f  oord_a.separatio
-00007af0: 6e28 636f 6f72 645f 6229 7a1c 7365 705f  n(coord_b)z.sep_
-00007b00: 6b70 6320 3d20 7365 702e 6172 6373 6563  kpc = sep.arcsec
-00007b10: 2a61 7263 5f6b 7063 7a76 7072 696e 7420  *arc_kpczvprint 
-00007b20: 2827 5365 7061 7261 7469 6f6e 2062 6574  ('Separation bet
-00007b30: 7765 656e 2061 2053 6563 6f6e 6461 7279  ween a Secondary
-00007b40: 2061 6e64 2050 7269 6d61 7279 2024 5c73   and Primary $\s
-00007b50: 696d 2420 7b3a 2e31 667d 5c2c 6b70 6320  im$ {:.1f}\,kpc 
-00007b60: 287b 3a2e 3166 7d24 5c5c 6172 6373 6563  ({:.1f}$\\arcsec
-00007b70: 2429 272e 666f 726d 6174 2873 6570 5f6b  $)'.format(sep_k
-00007b80: 7063 2c20 7365 702e 6172 6373 6563 2929  pc, sep.arcsec))
-00007b90: 7a25 7461 625f 7072 6f5b 2744 5f74 6f5f  z%tab_pro['D_to_
-00007ba0: 6d61 696e 275d 5b69 6e64 5f67 5d20 3d20  main'][ind_g] = 
-00007bb0: 7365 705f 6b70 637a 3f74 6162 5f70 726f  sep_kpcz?tab_pro
-00007bc0: 2e77 7269 7465 2827 7072 6f70 6572 7469  .write('properti
-00007bd0: 6573 2e64 6174 272c 2066 6f72 6d61 743d  es.dat', format=
-00007be0: 2761 7363 6969 272c 206f 7665 7277 7269  'ascii', overwri
-00007bf0: 7465 3d54 7275 6529 293b 7225 0000 0072  te=True));r%...r
-00007c00: c800 0000 72b7 0000 0072 c900 0000 72ca  ....r....r....r.
-00007c10: 0000 0072 cb00 0000 7219 0000 0072 d200  ...r....r....r..
-00007c20: 0000 7264 0000 0072 cc00 0000 72d4 0000  ..rd...r....r...
-00007c30: 0072 d500 0000 72de 0000 0072 df00 0000  .r....r....r....
-00007c40: 72e0 0000 0072 0500 0000 72d9 0000 0072  r....r....r....r
-00007c50: 0400 0000 72c0 0000 0072 0900 0000 7276  ....r....r....rv
-00007c60: 0200 0072 7502 0000 721e 0200 0072 e300  ...ru...r....r..
-00007c70: 0000 72dd 0000 0072 fb00 0000 da03 7a69  ..r....r......zi
-00007c80: 7072 8501 0000 7287 0100 0072 dc00 0000  pr....r....r....
-00007c90: 721f 0200 0072 2002 0000 72e6 0000 0072  r....r ...r....r
-00007ca0: 1c02 0000 72d6 0000 0072 0300 0000 72e4  ....r....r....r.
-00007cb0: 0000 0072 d700 0000 72d8 0000 0072 5302  ...r....r....rS.
-00007cc0: 0000 72a6 0100 0072 2602 0000 72e7 0000  ..r....r&...r...
-00007cd0: 0072 e800 0000 72ab 0100 0072 ac01 0000  .r....r....r....
-00007ce0: 7208 0000 0072 7702 0000 7278 0200 0072  r....rw...rx...r
-00007cf0: 7902 0000 72f9 0000 0072 7a02 0000 7223  y...r....rz...r#
-00007d00: 0200 0072 2402 0000 7228 0200 0072 2702  ...r$...r(...r'.
-00007d10: 0000 72ea 0000 0072 e900 0000 da05 4752  ..r....r......GR
-00007d20: 4545 4e29 3472 4100 0000 72ff 0000 0072  EEN)4rA...r....r
-00007d30: 0001 0000 7201 0100 0072 e701 0000 7204  ....r....r....r.
-00007d40: 0100 00da 0975 7365 725f 7465 7874 72e9  .....user_textr.
-00007d50: 0100 0072 ea01 0000 72eb 0100 0072 e900  ...r....r....r..
-00007d60: 0000 72e8 0100 00da 0b69 7473 636f 6e73  ..r......itscons
-00007d70: 6964 6572 da08 6974 7367 726f 7570 729a  ider..itsgroupr.
-00007d80: 0200 0072 ec01 0000 72ed 0100 0072 ee01  ...r....r....r..
-00007d90: 0000 7208 0100 0072 0901 0000 72b3 0000  ..r....r....r...
-00007da0: 0072 0a01 0000 7239 0200 0072 0b01 0000  .r....r9...r....
-00007db0: 7213 0100 0072 bf00 0000 72e5 0000 0072  r....r....r....r
-00007dc0: 8202 0000 7283 0200 0072 8402 0000 7233  ....r....r....r3
-00007dd0: 0100 0072 8502 0000 da08 636f 6d70 5f69  ...r......comp_i
-00007de0: 6e64 da04 636f 6d70 7236 0100 0072 3302  nd..compr6...r3.
-00007df0: 0000 72d5 0000 00da 0669 6d61 706e 6772  ..r......imapngr
-00007e00: 0f01 0000 722e 0000 0072 0602 0000 7270  ....r....r....rp
-00007e10: 0200 0072 8602 0000 7287 0200 0072 8902  ...r....r....r..
-00007e20: 0000 728f 0200 0072 9002 0000 7291 0200  ..r....r....r...
-00007e30: 0072 9202 0000 7293 0200 0072 9402 0000  .r....r....r....
-00007e40: 7295 0200 0072 2f00 0000 722f 0000 0072  r....r/...r/...r
-00007e50: 3000 0000 721b 0200 00f4 0400 0073 cc01  0...r........s..
-00007e60: 0000 0006 1a02 1001 1801 0801 0602 1001  ................
-00007e70: 0a02 1002 0801 1402 0a01 0e01 0801 1401  ................
-00007e80: 0a01 02ff 0602 2201 2202 0601 0a03 1a01  ......".".......
-00007e90: 1602 0a02 1a01 0a01 0801 0600 0a00 0600  ................
-00007ea0: 08ff 0c04 0801 1c02 0e01 0803 1201 1602  ................
-00007eb0: 1c03 1401 0801 0401 0c02 1401 1401 1401  ................
-00007ec0: 1401 1401 0a01 0c01 0a01 0c01 0e01 0c01  ................
-00007ed0: 0a01 0c01 0a01 0c01 0e01 0a01 1202 0e02  ................
-00007ee0: 0a01 1202 0c01 0a01 1803 1003 0801 0a01  ................
-00007ef0: 0a01 0a01 0a01 0a01 0a01 0a01 0a03 0a03  ................
-00007f00: 0c01 0a01 0c02 0a03 0c01 0e01 2601 1601  ............&...
-00007f10: 0201 1201 0601 1401 2601 1601 1e01 0201  ........&.......
-00007f20: 0afe 0604 0e01 0e01 1203 0c01 0e01 1001  ................
-00007f30: 0801 0200 02ff 0803 1602 0a01 02ff 0401  ................
-00007f40: 02ff 0402 0a01 02ff 0602 0402 0a01 1e02  ................
-00007f50: 0c02 0e01 1401 0600 0200 0200 0200 0200  ................
-00007f60: 0201 0200 0200 0200 0200 0200 02fe 0605  ................
-00007f70: 0c02 0a01 0402 1a02 1801 1402 2a01 14ff  ............*...
-00007f80: 0201 14ff 0403 0a03 0a03 1401 02ff 0604  ................
-00007f90: 1401 0e01 0a00 0200 0aff 0603 1401 1402  ................
-00007fa0: 0a01 1603 1401 0e01 0801 0a01 1401 0e01  ................
-00007fb0: 0802 180a 0801 0a01 0a01 0c04 1401 02ff  ................
-00007fc0: 0604 1001 0803 0c01 0c02 0a01 1603 1001  ................
-00007fd0: 0e01 0801 0a01 1001 0e01 0802 180a 0801  ................
-00007fe0: 0a01 0a01 0a01 0e01 1402 2202 0a01 0e02  ..........".....
-00007ff0: 0c03 0e01 0801 0801 0801 0e01 0801 0601  ................
-00008000: 0a00 0aff 0602 0801 02ff 0602 0801 02ff  ................
-00008010: 0602 0802 0801 0801 0e01 0801 0801 0801  ................
-00008020: 0801 0801 0801 0e01 0801 0802 0801 721b  ..............r.
-00008030: 0200 0072 6802 0000 630e 0000 0000 0000  ...rh...c.......
-00008040: 0000 0000 0035 0000 000d 0000 0043 0000  .....5.......C..
-00008050: 0073 8a07 0000 7400 a001 7c01 6401 1900  .s....t...|.d...
-00008060: 7c00 6b02 a101 6402 1900 6402 1900 7d0e  |.k...d...d...}.
-00008070: 7c01 6403 1900 7c0e 1900 7402 1b00 7d0f  |.d...|...t...}.
-00008080: 7400 a003 7400 a004 6404 a101 a101 7c0f  t...t...d.....|.
-00008090: 1400 6405 1400 7d10 6406 7d11 7405 7406  ..d...}.d.}.t.t.
-000080a0: 6a07 6407 1700 8301 0100 7405 7406 6a07  j.d.......t.t.j.
-000080b0: 6408 1700 8301 0100 7405 7406 6a08 6409  d.......t.t.j.d.
-000080c0: a009 7c01 640a 1900 7c0e 1900 a101 1700  ..|.d...|.......
-000080d0: 8301 0100 7405 7406 6a07 640b a009 7c0f  ....t.t.j.d...|.
-000080e0: a101 1700 8301 0100 7405 7406 6a07 640c  ........t.t.j.d.
-000080f0: a009 7c10 a101 1700 8301 0100 7c02 7c10  ..|.........|.|.
-00008100: 1b00 7c11 1b00 640d 1400 7d12 7c12 640e  ..|...d...}.|.d.
-00008110: 1400 640f 1400 6410 1b00 7d13 7405 7406  ..d...d...}.t.t.
-00008120: 6a07 6411 a009 7c12 a101 1700 8301 0100  j.d...|.........
-00008130: 7400 a00a 7c04 a101 7400 6a0b 1400 7c10  t...|...t.j...|.
-00008140: 640d 1300 1b00 6412 1b00 7d14 7405 7406  d.....d...}.t.t.
-00008150: 6a07 6413 a009 7c04 7c14 a102 1700 8301  j.d...|.|.......
-00008160: 0100 740c 6a0d a00e 6414 a101 9001 7332  ..t.j...d.....s2
-00008170: 740c a00f 6415 a101 0100 7405 7406 6a08  t...d.....t.t.j.
-00008180: 6416 1700 8301 0100 740c 6a0d a00e 6417  d.......t.j...d.
-00008190: a101 9001 7358 740c a00f 6418 a101 0100  ....sXt...d.....
-000081a0: 7405 7406 6a08 6419 1700 8301 0100 7405  t.t.j.d.......t.
-000081b0: 7406 6a10 641a 1700 8301 0100 7405 641b  t.j.d.......t.d.
-000081c0: 8301 0100 641c 7d15 641d a009 7c00 7c05  ....d.}.d...|.|.
-000081d0: 7c02 a103 7d16 740c 6a0d a00e 7c16 a101  |...}.t.j...|...
-000081e0: 9001 73e0 7405 641e 7c16 9b00 641f 9d03  ..s.t.d.|...d...
-000081f0: 8301 0100 6420 a009 7c01 6421 1900 7c0e  ....d ..|.d!..|.
-00008200: 1900 7c01 6422 1900 7c0e 1900 7c05 7411  ..|.d"..|...|.t.
-00008210: 7c12 8301 a104 7d17 7c15 7c17 1700 7d18  |.....}.|.|...}.
-00008220: 7405 7c18 8301 0100 7412 a013 7c18 7c16  t.|.....t...|.|.
-00008230: a102 0100 6e10 7405 6423 7c16 9b00 6424  ....n.t.d#|...d$
-00008240: 9d03 8301 0100 6425 7d15 6426 a009 7c00  ......d%}.d&..|.
-00008250: 7c02 a102 7d16 740c 6a0d a00e 7c16 a101  |...}.t.j...|...
-00008260: 9002 7356 7405 6427 8301 0100 6428 a009  ..sVt.d'....d(..
-00008270: 7c01 6421 1900 7c0e 1900 7c01 6422 1900  |.d!..|...|.d"..
-00008280: 7c0e 1900 7411 7c12 8301 a103 7d17 7c15  |...t.|.....}.|.
-00008290: 7c17 1700 7d18 7405 7c18 8301 0100 7412  |...}.t.|.....t.
-000082a0: a013 7c18 7c16 a102 0100 6e10 7405 6423  ..|.|.....n.t.d#
-000082b0: 7c16 9b00 6424 9d03 8301 0100 6426 a009  |...d$......d&..
-000082c0: 7c00 7c02 a102 7d19 7414 a015 7c19 a101  |.|...}.t...|...
-000082d0: 7d1a 7416 a017 641d a009 7c00 7c05 7c02  }.t...d...|.|.|.
-000082e0: a103 a101 7d1b 7c1b 6402 1900 6a18 7d1c  ....}.|.d...j.}.
-000082f0: 7411 7c12 8301 640e 1400 640f 1400 7c10  t.|...d...d...|.
-00008300: 1400 7d1d 7414 6a19 6429 642a 8d01 7d1e  ..}.t.j.d)d*..}.
-00008310: 7414 6a1a 7c1a 7400 a01b 642b 642c 642b  t.j.|.t...d+d,d+
-00008320: 642c 6704 a101 7c1d 1400 640e 1400 642d  d,g...|...d...d-
-00008330: 8d02 0100 7414 a01c a100 0100 7414 a01d  ....t.......t...
-00008340: 642e a101 0100 7414 a01e 642f a101 0100  d.....t...d/....
-00008350: 7414 a01f a100 0100 7c0a 6430 6b02 9003  t.......|.d0k...
-00008360: 7216 7414 a020 a100 0100 6e08 7414 a021  r.t.. ....n.t..!
-00008370: a100 0100 7405 6431 8301 0100 7405 7406  ....t.d1....t.t.
-00008380: 6a07 6432 1700 8301 0100 7405 6433 8301  j.d2......t.d3..
-00008390: 0100 7405 6431 8301 0100 7422 7c1c 7c0b  ..t.d1....t"|.|.
-000083a0: 7c0c 7c0d 6434 8d04 7d1f 7414 6a19 6429  |.|.d4..}.t.j.d)
-000083b0: 642a 8d01 7d1e 7414 6a1a 7c1f 6435 6436  d*..}.t.j.|.d5d6
-000083c0: 8d02 0100 7c0a 6430 6b02 9003 7282 7414  ....|.d0k...r.t.
-000083d0: a020 a100 0100 6e08 7414 a021 a100 0100  . ....n.t..!....
-000083e0: 7423 7c1c 6437 7c1f 6438 8d03 5c03 7d20  t#|.d7|.d8..\.} 
-000083f0: 7d21 7d22 7405 7406 6a07 6439 1700 8301  }!}"t.t.j.d9....
-00008400: 0100 7405 6433 8301 0100 7405 643a a009  ..t.d3....t.d:..
-00008410: 7c20 a101 8301 0100 7405 643b a009 7c21  | ......t.d;..|!
-00008420: a101 8301 0100 7405 643c a009 7c22 a101  ......t.d<..|"..
-00008430: 8301 0100 7405 643d a009 7c06 6402 1900  ....t.d=..|.d...
-00008440: 7c06 642c 1900 a102 8301 0100 7405 6433  |.d,........t.d3
-00008450: 8301 0100 7424 8300 7d23 7425 7c1c 7c06  ....t$..}#t%|.|.
-00008460: 643e 7c23 7c1f 7c21 643f 8d06 7d24 7c1c  d>|#|.|!d?..}$|.
-00008470: 7c24 6a26 3800 7d1c 7405 6440 8301 0100  |$j&8.}.t.d@....
-00008480: 7414 6a19 6429 642a 8d01 7d1e 7414 6a1a  t.j.d)d*..}.t.j.
-00008490: 7c24 6a26 6435 6436 8d02 0100 7c0a 6430  |$j&d5d6....|.d0
-000084a0: 6b02 9004 725a 7414 a020 a100 0100 6e08  k...rZt.. ....n.
-000084b0: 7414 a021 a100 0100 7c08 7427 1400 7d25  t..!....|.t'..}%
-000084c0: 7428 7c25 6441 6441 6442 8d03 7d26 7c26  t(|%dAdAdB..}&|&
-000084d0: a029 a100 0100 7411 7c14 8301 7d27 742a  .)....t.|...}'t*
-000084e0: 6a2b 7c1c 7c03 6443 8d02 7d28 742a a02c  j+|.|.dC..}(t*.,
-000084f0: 7c1c 7c28 7c27 a103 7d29 7c07 6444 6b02  |.|(|'..})|.dDk.
-00008500: 9005 720e 7405 6445 8301 0100 7405 6446  ..r.t.dE....t.dF
-00008510: 8301 0100 7405 6447 8301 0100 7414 6a19  ....t.dG....t.j.
-00008520: 6429 642a 8d01 7d1e 7414 6a1a 7c29 6435  d)d*..}.t.j.|)d5
-00008530: 6436 8d02 0100 742d 7c1c 7c29 7c27 6448  d6....t-|.|)|'dH
-00008540: 6449 644a 8d05 7d29 7c0a 6430 6b02 9005  dIdJ..})|.d0k...
-00008550: 7206 7414 a020 a100 0100 6e08 7414 a021  r.t.. ....n.t..!
-00008560: a100 0100 7400 a02e 7c29 6a2f a101 7d2a  ....t...|)j/..}*
-00008570: 7405 644b 8301 0100 7405 7c29 6a2f 8301  t.dK....t.|)j/..
-00008580: 0100 7405 7400 a030 7431 7c29 6a2f 8301  ..t.t..0t1|)j/..
-00008590: a101 8301 0100 6402 6400 6c32 7d2b 644c  ......d.d.l2}+dL
-000085a0: 7c2b 6a33 644d 3c00 644e 7c2b 6a33 644f  |+j3dM<.dN|+j3dO
-000085b0: 3c00 6450 7c2b 6a33 6451 3c00 6452 7c2b  <.dP|+j3dQ<.dR|+
-000085c0: 6a33 6453 3c00 6450 7c2b 6a33 6454 3c00  j3dS<.dP|+j3dT<.
-000085d0: 6452 7c2b 6a33 6455 3c00 6450 7c2b 6a33  dR|+j3dU<.dP|+j3
-000085e0: 6456 3c00 6450 7c2b 6a33 6457 3c00 7414  dV<.dP|+j3dW<.t.
-000085f0: 6a19 6458 642a 8d01 7d1e 7400 a034 7c29  j.dXd*..}.t..4|)
-00008600: 6a18 a101 a035 7436 a101 7d2c 7400 6a37  j....5t6..},t.j7
-00008610: 7c2c 7c2c 6459 6b02 3c00 7414 6a1a 7c2c  |,|,dYk.<.t.j.|,
-00008620: 645a 645b 6435 645c 8d04 7d2d 7400 a030  dZd[d5d\..}-t..0
-00008630: 7400 a038 7c2c a101 a101 4400 5d42 7d2e  t..8|,....D.]B}.
-00008640: 7400 a001 7c2c 7c2e 642c 1700 6b02 a101  t...|,|.d,..k...
-00008650: 7d2f 7414 6a39 7c2f 642c 1900 6402 1900  }/t.j9|/d,..d...
-00008660: 7c2f 6402 1900 6402 1900 743a 7411 7c2e  |/d...d...t:t.|.
-00008670: 8301 8301 645d 645e 8d04 0100 9005 71e6  ....d]d^......q.
-00008680: 7414 a03b 7c2d a101 7d30 7c30 6a3c a01f  t..;|-..}0|0j<..
-00008690: a100 0100 7414 a01f a100 0100 7c0a 6430  ....t.......|.d0
-000086a0: 6b02 9006 725a 7414 a020 a100 0100 6e08  k...rZt.. ....n.
-000086b0: 7414 a021 a100 0100 7416 6a3d 645f 7c2c  t..!....t.j=d_|,
-000086c0: 6460 6461 8d03 0100 7c09 6462 6b02 9006  d`da....|.dbk...
-000086d0: 72d2 6463 7c00 9b00 6464 7c02 9b00 6465  r.dc|...dd|...de
-000086e0: 9d05 7d17 6466 7c03 9b00 6467 7c04 9b00  ..}.df|...dg|...
-000086f0: 6468 7c05 9b00 6469 9d07 7d31 646a 7c06  dh|...di..}1dj|.
-00008700: 9b00 646b 7c07 9b00 6469 9d05 7d32 646c  ..dk|...di..}2dl
-00008710: 7d33 7405 7c17 7c31 1700 7c32 1700 7c33  }3t.|.|1..|2..|3
-00008720: 1700 8301 0100 6eb4 7411 7c2c 7411 7c2c  ......n.t.|,t.|,
-00008730: 6a3e 6402 1900 640e 1400 8301 7411 7c2c  j>d...d.....t.|,
-00008740: 6a3e 642c 1900 640e 1400 8301 6602 1900  j>d,..d.....f...
-00008750: 8301 642c 1800 7d34 6463 7c00 9b00 6464  ..d,..}4dc|...dd
-00008760: 7c02 9b00 6465 9d05 7d17 6466 7c03 9b00  |...de..}.df|...
-00008770: 6467 7c04 9b00 6468 7c05 9b00 6469 9d07  dg|...dh|...di..
-00008780: 7d31 646a 7c06 9b00 646b 7c07 9b00 6469  }1dj|...dk|...di
-00008790: 9d05 7d32 646d 7c34 9b00 646e 7c05 9b00  ..}2dm|4..dn|...
-000087a0: 646f 9d05 7d33 7405 7c17 7c31 1700 7c32  do..}3t.|.|1..|2
-000087b0: 1700 7c33 1700 8301 0100 743f 7c00 7c01  ..|3......t?|.|.
-000087c0: 7c02 7c03 7c04 7c05 7c06 7c07 7c34 6701  |.|.|.|.|.|.|4g.
-000087d0: 7c05 6701 7c0a 6470 8d0b 0100 6400 5300  |.g.|.dp....d.S.
-000087e0: 2971 4e72 4100 0000 7201 0000 0072 4200  )qNrA...r....rB.
-000087f0: 0000 7243 0000 0072 4400 0000 e748 e17a  ..rC...rD....H.z
-00008800: 14ae 47d1 3f72 4500 0000 7246 0000 00fa  ..G.?rE...rF....
-00008810: 0a4a 636c 6173 7320 7b7d 2072 c600 0000  .Jclass {} r....
-00008820: 72d2 0100 0072 4700 0000 7239 0000 0072  r....rG...r9...r
-00008830: 4900 0000 7248 0000 0072 4a00 0000 724b  I...rH...rJ...rK
-00008840: 0000 0072 4c00 0000 724d 0000 0072 d501  ...rL...rM...r..
-00008850: 0000 72d6 0100 0072 d701 0000 72d8 0100  ..r....r....r...
-00008860: 0072 d901 0000 72da 0100 0072 5700 0000  .r....r....rW...
-00008870: 7258 0000 00fa 3068 7474 7073 3a2f 2f77  rX....0https://w
-00008880: 7777 2e6c 6567 6163 7973 7572 7665 792e  ww.legacysurvey.
-00008890: 6f72 672f 7669 6577 6572 2f66 6974 732d  org/viewer/fits-
-000088a0: 6375 746f 7574 3ffa 1c66 6974 735f 696d  cutout?..fits_im
-000088b0: 6167 6573 2f7b 7d5f 7b7d 5f7b 7d6b 7063  ages/{}_{}_{}kpc
-000088c0: 2e66 6974 7372 5d00 0000 725e 0000 007a  .fitsr]...r^...z
-000088d0: 3572 613d 7b7d 2664 6563 3d7b 7d26 6c61  5ra={}&dec={}&la
-000088e0: 7965 723d 6472 3826 7069 7873 6361 6c65  yer=dr8&pixscale
-000088f0: 3d30 2e32 3726 6261 6e64 733d 7b7d 2673  =0.27&bands={}&s
-00008900: 697a 653d 7b7d 724e 0000 0072 4f00 0000  ize={}rN...rO...
-00008910: 725b 0000 0072 5c00 0000 7a30 6874 7470  r[...r\...z0http
-00008920: 733a 2f2f 7777 772e 6c65 6761 6379 7375  s://www.legacysu
-00008930: 7276 6579 2e6f 7267 2f76 6965 7765 722f  rvey.org/viewer/
-00008940: 6a70 6567 2d63 7574 6f75 743f 7a18 696d  jpeg-cutout?z.im
-00008950: 6167 6573 2f66 6967 5f7b 7d5f 7b7d 6b70  ages/fig_{}_{}kp
-00008960: 632e 6a70 6567 7a1c 0a44 6f77 6e6c 6f61  c.jpegz..Downloa
-00008970: 6469 6e67 2074 6865 206a 7065 6720 6669  ding the jpeg fi
-00008980: 6c65 2e2e 7a36 7261 3d7b 7d26 6465 633d  le..z6ra={}&dec=
-00008990: 7b7d 266c 6179 6572 3d64 7238 2670 6978  {}&layer=dr8&pix
-000089a0: 7363 616c 653d 302e 3237 2662 616e 6473  scale=0.27&bands
-000089b0: 3d67 727a 2673 697a 653d 7b7d 7274 0000  =grz&size={}rt..
-000089c0: 0072 7600 0000 7262 0000 0072 6900 0000  .rv...rb...ri...
-000089d0: 720a 0200 0072 0702 0000 7208 0200 0072  r....r....r....r
-000089e0: 4000 0000 726f 0000 0072 6d00 0000 726e  @...ro...rm...rn
-000089f0: 0000 0072 7000 0000 7278 0000 0072 7900  ...rp...rx...ry.
-00008a00: 0000 727f 0000 0072 8000 0000 7283 0000  ..r....r....r...
-00008a10: 0072 8500 0000 7286 0000 0072 8700 0000  .r....r....r....
-00008a20: 7288 0000 0072 8a00 0000 728c 0000 0072  r....r....r....r
-00008a30: ef01 0000 728b 0000 0072 9800 0000 729b  ....r....r....r.
-00008a40: 0000 0072 9c00 0000 729d 0000 0072 9e00  ...r....r....r..
-00008a50: 0000 729f 0000 0072 a000 0000 72a1 0000  ..r....r....r...
-00008a60: 0072 a200 0000 72f0 0100 0072 f101 0000  .r....r....r....
-00008a70: 72f2 0100 0072 5e01 0000 72f3 0100 0072  r....r^...r....r
-00008a80: f401 0000 72f5 0100 0072 e101 0000 72f6  ....r....r....r.
-00008a90: 0100 0072 f701 0000 72f8 0100 0072 f901  ...r....r....r..
-00008aa0: 0000 72fa 0100 0072 fb01 0000 726b 0000  ..r....r....rk..
-00008ab0: 0072 fc01 0000 72fd 0100 0072 fe01 0000  .r....r....r....
-00008ac0: 7200 0200 0072 0102 0000 7a09 7465 7374  r....r....z.test
-00008ad0: 2e66 6974 7354 7292 0000 0072 c801 0000  .fitsTr....r....
-00008ae0: 7a16 0a0a 534c 2e70 686f 745f 6d6f 645f  z...SL.phot_mod_
-00008af0: 6465 6361 6c73 2827 7a17 272c 2074 6162  decals('z.', tab
-00008b00: 2c20 7369 7a65 5f69 6d61 6765 5f70 6879  , size_image_phy
-00008b10: 3d72 1002 0000 7211 0200 0072 1202 0000  =r....r....r....
-00008b20: 7a08 2c20 6261 6e64 3d22 7214 0200 007a  z., band="r....z
-00008b30: 0a73 6b79 5f62 6f78 203d 2072 1302 0000  .sky_box = r....
-00008b40: 7a26 7573 6572 5f6f 7264 6572 3d5b 312c  z&user_order=[1,
-00008b50: 325d 2c20 7573 6572 5f6c 6973 743d 5b22  2], user_list=["
-00008b60: 4122 2c22 4222 5d29 7215 0200 007a 0f5d  A","B"])r....z.]
-00008b70: 2c20 7573 6572 5f6c 6973 743d 5b22 7a03  , user_list=["z.
-00008b80: 225d 2929 0972 0101 0000 7202 0100 0072  "])).r....r....r
-00008b90: 0301 0000 7208 0100 0072 0601 0000 7207  ....r....r....r.
-00008ba0: 0100 0072 0401 0000 7205 0100 0072 c100  ...r....r....r..
-00008bb0: 0000 2940 7225 0000 0072 c800 0000 72b7  ..)@r%...r....r.
-00008bc0: 0000 0072 c900 0000 72ca 0000 0072 cb00  ...r....r....r..
-00008bd0: 0000 7219 0000 0072 cc00 0000 72d2 0000  ..r....r....r...
-00008be0: 0072 6400 0000 72cd 0000 0072 ce00 0000  .rd...r....r....
-00008bf0: 72d4 0000 0072 d500 0000 72d6 0000 0072  r....r....r....r
-00008c00: 1602 0000 72dd 0000 0072 d800 0000 721a  ....r....r....r.
-00008c10: 0000 0072 1300 0000 72e6 0000 0072 1c02  ...r....r....r..
-00008c20: 0000 7203 0000 0072 e400 0000 72e5 0000  ..r....r....r...
-00008c30: 0072 e700 0000 72e8 0000 0072 2602 0000  .r....r....r&...
-00008c40: 72ba 0100 0072 2702 0000 7228 0200 0072  r....r'...r(...r
-00008c50: 2402 0000 72ea 0000 0072 eb00 0000 720a  $...r....r....r.
-00008c60: 0000 0072 0b00 0000 720d 0000 0072 0c00  ...r....r....r..
-00008c70: 0000 72ec 0000 0072 1100 0000 7210 0000  ..r....r....r...
-00008c80: 0072 f200 0000 72f3 0000 0072 f400 0000  .r....r....r....
-00008c90: 720e 0000 0072 0f00 0000 721d 0200 0072  r....r....r....r
-00008ca0: fa00 0000 721e 0200 0072 e300 0000 721f  ....r....r....r.
-00008cb0: 0200 0072 2002 0000 7226 0000 0072 8601  ...r ...r&...r..
-00008cc0: 0000 7221 0200 0072 2700 0000 7222 0200  ..r!...r'...r"..
-00008cd0: 0072 2302 0000 72da 0000 0072 b001 0000  .r#...r....r....
-00008ce0: 72b2 0100 0072 ed00 0000 72a6 0100 00da  r....r....r.....
-00008cf0: 0f70 686f 745f 6d6f 645f 6465 6361 6c73  .phot_mod_decals
-00008d00: 2935 7241 0000 0072 ff00 0000 7201 0100  )5rA...r....r...
-00008d10: 0072 0201 0000 7203 0100 0072 0801 0000  .r....r....r....
-00008d20: 7206 0100 0072 0701 0000 72ad 0000 0072  r....r....r....r
-00008d30: 2a02 0000 72c1 0000 0072 7100 0000 7272  *...r....rq...rr
-00008d40: 0000 0072 7300 0000 7209 0100 0072 b300  ...rs...r....r..
-00008d50: 0000 720a 0100 0072 b401 0000 720b 0100  ..r....r....r...
-00008d60: 0072 0c01 0000 720d 0100 00da 0468 6f6d  .r....r......hom
-00008d70: 6572 d500 0000 723a 0200 00da 0474 6172  er....r:.....tar
-00008d80: 6772 3002 0000 7231 0200 0072 1a01 0000  gr0...r1...r....
-00008d90: 721b 0100 0072 3502 0000 721d 0100 0072  r....r5...r....r
-00008da0: 1c01 0000 721e 0100 0072 1f01 0000 7220  ....r....r....r 
-00008db0: 0100 0072 8e00 0000 7221 0100 0072 8100  ...r....r!...r..
-00008dc0: 0000 722a 0100 0072 2b01 0000 722c 0100  ..r*...r+...r,..
-00008dd0: 0072 2d01 0000 7232 0200 0072 3302 0000  .r-...r2...r3...
-00008de0: 7234 0200 0072 3602 0000 7233 0100 0072  r4...r6...r3...r
-00008df0: 3702 0000 72c4 0100 0072 3b02 0000 723c  7...r....r;...r<
-00008e00: 0200 00da 0570 6172 7433 723d 0200 0072  .....part3r=...r
-00008e10: 2f00 0000 722f 0000 0072 3000 0000 da12  /...r/...r0.....
-00008e20: 6578 5f70 686f 745f 6d6f 645f 6465 6361  ex_phot_mod_deca
-00008e30: 6c73 1e06 0000 7358 0100 0000 051a 0110  ls....sX........
-00008e40: 0118 0104 010e 010e 011c 0114 0114 0110  ................
-00008e50: 0210 0114 011c 010c 0102 ff08 030e 010a  ................
-00008e60: 010e 020e 010a 010e 020e 0108 0204 010e  ................
-00008e70: 010e 0110 0104 010a 000a 0002 0006 ff04  ................
-00008e80: 0208 0108 020e 0310 0204 010c 010e 0108  ................
-00008e90: 0104 010a 000a 0006 ff04 0208 0108 020e  ................
-00008ea0: 0310 020c 010a 0114 010a 0214 010c 0124  ...............$
-00008eb0: 0108 010a 010a 0108 020a 010a 0208 0608  ................
-00008ec0: 010e 0108 0108 0108 0102 ff06 020c 010e  ................
-00008ed0: 010a 010a 0208 0106 0102 ff0c 020e 0108  ................
-00008ee0: 010e 010e 010e 0406 0106 0006 ff06 0208  ................
-00008ef0: 0306 0108 0102 0002 0102 fe06 040a 0208  ................
-00008f00: 010c 0110 010a 010a 0208 0308 010e 0108  ................
-00008f10: 0308 010e 010e 020a 0108 0108 0208 010c  ................
-00008f20: 010e 0108 0202 0002 fe06 030a 010a 0208  ................
-00008f30: 040c 0108 010a 0114 0608 010a 010a 010a  ................
-00008f40: 010a 010a 010a 010a 010a 020c 0112 010e  ................
-00008f50: 0a0a 0102 ff06 0414 0112 012e 020a 010a  ................
-00008f60: 0108 010a 010a 0208 0110 020a 0212 0118  ................
-00008f70: 0112 0104 0116 0330 0212 0118 0112 0112  .......0........
-00008f80: 0114 020a 0102 0002 0002 0102 0004 0004  ................
-00008f90: 0102 fd72 af02 0000 6310 0000 0000 0000  ...r....c.......
-00008fa0: 0000 0000 0042 0000 0012 0000 0043 0000  .....B.......C..
-00008fb0: 0073 6408 0000 7400 a001 7c01 6401 1900  .sd...t...|.d...
-00008fc0: 7c00 6b02 a101 6402 1900 6402 1900 7d10  |.k...d...d...}.
-00008fd0: 7c01 6403 1900 7c10 1900 7402 1b00 7d11  |.d...|...t...}.
-00008fe0: 7400 a003 7400 a004 6404 a101 a101 7c11  t...t...d.....|.
-00008ff0: 1400 6405 1400 7d12 7405 7406 6a07 6406  ..d...}.t.t.j.d.
-00009000: 1700 8301 0100 7405 7406 6a07 6407 1700  ......t.t.j.d...
-00009010: 8301 0100 7405 7406 6a08 6408 a009 7c01  ....t.t.j.d...|.
-00009020: 6409 1900 7c10 1900 a101 1700 8301 0100  d...|...........
-00009030: 7405 7406 6a07 640a a009 7c12 a101 1700  t.t.j.d...|.....
-00009040: 8301 0100 7c02 7c12 1b00 640b 1b00 640c  ....|.|...d...d.
-00009050: 1400 7d13 7c13 640d 1400 640b 1400 640e  ..}.|.d...d...d.
-00009060: 1b00 7d14 7405 7406 6a07 640f a009 7c13  ..}.t.t.j.d...|.
-00009070: a101 1700 8301 0100 7400 a00a 7c04 a101  ........t...|...
-00009080: 7400 6a0b 1400 7c12 640c 1300 1b00 6410  t.j...|.d.....d.
-00009090: 1b00 7d15 7405 7406 6a07 6411 a009 7c04  ..}.t.t.j.d...|.
-000090a0: 7c15 a102 1700 8301 0100 7405 7406 6a0c  |.........t.t.j.
-000090b0: 6412 1700 8301 0100 7405 6413 8301 0100  d.......t.d.....
-000090c0: 6414 7d16 7c01 6415 7c05 1700 1900 7c10  d.}.|.d.|.....|.
-000090d0: 1900 7d17 7405 6416 a009 7c16 a101 8301  ..}.t.d...|.....
-000090e0: 0100 7405 6417 a009 7c17 a101 8301 0100  ..t.d...|.......
-000090f0: 6418 7d18 6419 7d19 641a 7d1a 7400 a00a  d.}.d.}.d.}.t...
-00009100: 7c18 a101 7d1b 6419 7d1c 740d a00e 641b  |...}.d.}.t...d.
-00009110: 7c01 6401 1900 7c10 1900 1700 641c a009  |.d...|.....d...
-00009120: 7c05 7c02 a102 1700 a101 7d1d 7c1d 6402  |.|.......}.|.d.
-00009130: 1900 6a0f 7d1e 7405 7406 6a07 641d 1700  ..j.}.t.t.j.d...
-00009140: 8301 0100 7405 641e 8301 0100 7405 641f  ....t.d.....t.d.
-00009150: 8301 0100 7410 7c1e 7c0b 7c0c 7c0d 6420  ....t.|.|.|.|.d 
-00009160: 8d04 7d1f 7411 6a12 6421 6422 8d01 7d20  ..}.t.j.d!d"..} 
-00009170: 7411 6a13 7c1f 6423 6424 8d02 0100 7411  t.j.|.d#d$....t.
-00009180: 6a14 6425 7c00 1700 6426 a009 7c05 7c02  j.d%|...d&..|.|.
-00009190: a102 1700 6427 6428 8d02 0100 7c0a 6429  ....d'd(....|.d)
-000091a0: 6b02 9001 72fa 7411 a015 a100 0100 6e08  k...r.t.......n.
-000091b0: 7411 a016 a100 0100 7417 7c1e 642a 7c1f  t.......t.|.d*|.
-000091c0: 642b 8d03 5c03 7d21 7d22 7d23 7405 7406  d+..\.}!}"}#t.t.
-000091d0: 6a07 642c 1700 8301 0100 7405 642d 8301  j.d,......t.d-..
-000091e0: 0100 7405 642e a009 7c21 a101 8301 0100  ..t.d...|!......
-000091f0: 7405 642f a009 7c22 a101 8301 0100 7405  t.d/..|"......t.
-00009200: 6430 a009 7c23 a101 8301 0100 7405 6431  d0..|#......t.d1
-00009210: a009 7c08 6402 1900 7c08 6419 1900 a102  ..|.d...|.d.....
-00009220: 8301 0100 7405 6432 8301 0100 7418 8300  ....t.d2....t...
-00009230: 7d24 7419 7c1e 7c08 6433 7c24 7c1f 7c22  }$t.|.|.d3|$|.|"
-00009240: 6434 8d06 7d25 7c1e 7c25 6a1a 1800 7d1e  d4..}%|.|%j...}.
-00009250: 7411 6a12 6421 6422 8d01 7d20 7411 6a13  t.j.d!d"..} t.j.
-00009260: 7c25 6a1a 6423 6424 8d02 0100 7411 6a14  |%j.d#d$....t.j.
-00009270: 6425 7c00 1700 6435 a009 7c05 7c02 a102  d%|...d5..|.|...
-00009280: 1700 6427 6428 8d02 0100 7c0a 6429 6b02  ..d'd(....|.d)k.
-00009290: 9002 72e8 7411 a015 a100 0100 6e08 7411  ..r.t.......n.t.
-000092a0: a016 a100 0100 7c01 6401 1900 7c10 1900  ......|.d...|...
-000092b0: 6436 a009 7c05 7c02 a102 1700 7d26 740d  d6..|.|.....}&t.
-000092c0: 6a1b 641b 7c26 1700 6437 1700 7c25 6a1a  j.d.|&..d7..|%j.
-000092d0: 6438 6439 8d03 0100 740d 6a1b 641b 7c26  d8d9....t.j.d.|&
-000092e0: 1700 643a 1700 7c1e 6438 6439 8d03 0100  ..d:..|.d8d9....
-000092f0: 7405 643b 7c26 1700 643c 1700 8301 0100  t.d;|&..d<......
-00009300: 741c 7c1e 7c1a 7c1b 7c1c 7c16 8305 7d27  t.|.|.|.|.|...}'
-00009310: 7400 a01d 7400 a01e 640c a101 640c 1400  t...t...d...d...
-00009320: a101 640c 1400 7d28 643d 7d29 7c17 7c28  ..d...}(d=})|.|(
-00009330: 1b00 7d2a 7400 6a1f 7c29 0b00 7c29 6419  ..}*t.j.|)..|)d.
-00009340: 1700 8502 7c29 0b00 7c29 6419 1700 8502  ....|)..|)d.....
-00009350: 6602 1900 5c02 7d2b 7d2c 7400 a020 7c2c  f...\.}+},t.. |,
-00009360: 640c 1300 7c2b 640c 1300 1700 0b00 643e  d...|+d.......d>
-00009370: 7c2a 640c 1300 1400 1b00 a101 7d2d 7c2d  |*d.........}-|-
-00009380: 7400 a021 7c2d a101 1d00 7d2d 7c17 7422  t..!|-....}-|.t"
-00009390: 1400 7d2e 7423 7c2e 643f 643f 6440 8d03  ..}.t#|.d?d?d@..
-000093a0: 7d2f 7c2f a024 a100 0100 7425 7c15 8301  }/|/.$....t%|...
-000093b0: 7d30 7426 6a27 7c1e 7c03 6441 8d02 7d31  }0t&j'|.|.dA..}1
-000093c0: 7426 a028 7c1e 7c31 7c30 a103 7d32 7c09  t&.(|.|1|0..}2|.
-000093d0: 6442 6b02 9004 7282 7405 6443 8301 0100  dBk...r.t.dC....
-000093e0: 7405 6444 8301 0100 7405 6445 8301 0100  t.dD....t.dE....
-000093f0: 7411 6a12 6421 6422 8d01 0100 7411 6a13  t.j.d!d"....t.j.
-00009400: 7c32 6423 6424 8d02 0100 7c0a 6429 6b02  |2d#d$....|.d)k.
-00009410: 9004 7268 7411 a015 a100 0100 6e08 7411  ..rht.......n.t.
-00009420: a016 a100 0100 7429 7c1e 7c32 7c30 6446  ......t)|.|2|0dF
-00009430: 6447 6448 8d05 7d32 7405 6449 8301 0100  dGdH..}2t.dI....
-00009440: 7405 644a 8301 0100 7411 6a12 644b 6422  t.dJ....t.j.dKd"
-00009450: 8d01 7d20 7400 a02a 7c32 6a0f a101 a02b  ..} t..*|2j....+
-00009460: 742c a101 7d33 7400 6a2d 7c33 7c33 641a  t,..}3t.j-|3|3d.
-00009470: 6b02 3c00 7411 6a13 7c33 644c 644d 6423  k.<.t.j.|3dLdMd#
-00009480: 644e 8d04 7d34 7400 a02e 7400 a02f 7c33  dN..}4t...t../|3
-00009490: a101 a101 4400 5d42 7d35 7400 a001 7c33  ....D.]B}5t...|3
-000094a0: 7c35 6419 1700 6b02 a101 7d36 7411 6a30  |5d...k...}6t.j0
-000094b0: 7c36 6419 1900 6402 1900 7c36 6402 1900  |6d...d...|6d...
-000094c0: 6402 1900 7431 7425 7c35 8301 8301 644f  d...t1t%|5....dO
-000094d0: 6450 8d04 0100 9004 71e0 7411 a032 7c34  dP......q.t..2|4
-000094e0: a101 7d37 7c37 6a33 a034 a100 0100 7411  ..}7|7j3.4....t.
-000094f0: a034 a100 0100 6425 7c01 6401 1900 7c10  .4....d%|.d...|.
-00009500: 1900 1700 6451 a009 7c05 7c02 a102 1700  ....dQ..|.|.....
-00009510: 7d38 7411 6a14 7c38 6427 6428 8d02 0100  }8t.j.|8d'd(....
-00009520: 7c0a 6429 6b02 9005 727e 7411 a015 a100  |.d)k...r~t.....
-00009530: 0100 6e08 7411 a016 a100 0100 7405 7406  ..n.t.......t.t.
-00009540: 6a08 6452 1700 8301 0100 7405 6453 8301  j.dR......t.dS..
-00009550: 0100 7435 a035 a100 7d39 7400 6a2d 7c1e  ..t5.5..}9t.j-|.
-00009560: 7c1e 7400 6a36 6b02 3c00 7400 6a2d 7c1e  |.t.j6k.<.t.j-|.
-00009570: 7c1e 7400 6a36 0b00 6b02 3c00 7437 6a38  |.t.j6..k.<.t7j8
-00009580: 7c1e 7c32 6a0f 7c19 7c2d 7c0f 6454 8d05  |.|2j.|.|-|.dT..
-00009590: 7d3a 7405 6455 7435 a035 a100 7c39 1800  }:t.dUt5.5..|9..
-000095a0: 1600 8301 0100 7405 7439 7c3a 8301 8301  ......t.t9|:....
-000095b0: 0100 6456 6457 6458 6459 645a 645b 645c  ..dVdWdXdYdZd[d\
-000095c0: 645d 645e 645f 6460 6461 6462 6463 670e  d]d^d_d`dadbdcg.
-000095d0: 7d3b 7405 6464 8301 0100 7405 6465 8301  };t.dd....t.de..
-000095e0: 0100 7c06 6400 6b08 9007 7254 7400 a03a  ..|.d.k...rTt..:
-000095f0: 7c32 6a3b a101 7d3c 743c 7c3c 6400 6400  |2j;..}<t<|<d.d.
-00009600: 6466 8503 1900 8301 4400 5dfa 5c02 7d35  df......D.].\.}5
-00009610: 7d3d 7c3a 7c3d 1900 7d3e 743d 7c3e 7c00  }=|:|=..}>t=|>|.
-00009620: 7c3b 7c35 1900 1700 7c1e 7c27 7c1a 7c1b  |;|5....|.|'|.|.
-00009630: 7c1c 7c16 7c2d 7c17 7c18 7c12 7c02 7c0a  |.|.|-|.|.|.|.|.
-00009640: 7c0e 6467 8d0f 0100 743e a03f 7c0e a101  |.dg....t>.?|...
-00009650: 7d3f 7400 a001 7c3f 6468 1900 7c00 7c3b  }?t...|?dh..|.|;
-00009660: 7c35 1900 1700 6b02 a101 6402 1900 6402  |5....k...d...d.
-00009670: 1900 7d40 7400 a001 7c01 6401 1900 7c00  ..}@t...|.d...|.
-00009680: 6b02 a101 6402 1900 6402 1900 7d41 7c01  k...d...d...}A|.
-00009690: 6469 1900 7c41 1900 7c3f 6469 1900 7c40  di..|A..|?di..|@
-000096a0: 3c00 7c01 646a 1900 7c41 1900 7c3f 646a  <.|.dj..|A..|?dj
-000096b0: 1900 7c40 3c00 7c01 6403 1900 7c41 1900  ..|@<.|.d...|A..
-000096c0: 7c3f 646b 1900 7c40 3c00 7c01 646c 1900  |?dk..|@<.|.dl..
-000096d0: 7c41 1900 7c3f 646d 1900 7c40 3c00 7c01  |A..|?dm..|@<.|.
-000096e0: 6409 1900 7c41 1900 7c3f 6409 1900 7c40  d...|A..|?d...|@
-000096f0: 3c00 743e 6a40 7c3f 7c0e 6438 6439 8d03  <.t>j@|?|.d8d9..
-00009700: 0100 9006 7154 9001 6e04 743c 7c06 8301  ....qT..n.t<|...
-00009710: 4400 5dfa 5c02 7d35 7d3d 7c3a 7c3d 1900  D.].\.}5}=|:|=..
-00009720: 7d3e 743d 7c3e 7c00 7c07 7c35 1900 1700  }>t=|>|.|.|5....
-00009730: 7c1e 7c27 7c1a 7c1b 7c1c 7c16 7c2d 7c17  |.|'|.|.|.|.|-|.
-00009740: 7c18 7c12 7c02 7c0a 7c0e 6467 8d0f 0100  |.|.|.|.|.dg....
-00009750: 743e a03f 7c0e a101 7d3f 7400 a001 7c3f  t>.?|...}?t...|?
-00009760: 6468 1900 7c00 7c07 7c35 1900 1700 6b02  dh..|.|.|5....k.
-00009770: a101 6402 1900 6402 1900 7d40 7400 a001  ..d...d...}@t...
-00009780: 7c01 6401 1900 7c00 6b02 a101 6402 1900  |.d...|.k...d...
-00009790: 6402 1900 7d41 7c01 6469 1900 7c41 1900  d...}A|.di..|A..
-000097a0: 7c3f 6469 1900 7c40 3c00 7c01 646a 1900  |?di..|@<.|.dj..
-000097b0: 7c41 1900 7c3f 646a 1900 7c40 3c00 7c01  |A..|?dj..|@<.|.
-000097c0: 6403 1900 7c41 1900 7c3f 646b 1900 7c40  d...|A..|?dk..|@
-000097d0: 3c00 7c01 646c 1900 7c41 1900 7c3f 646d  <.|.dl..|A..|?dm
-000097e0: 1900 7c40 3c00 7c01 6409 1900 7c41 1900  ..|@<.|.d...|A..
-000097f0: 7c3f 6409 1900 7c40 3c00 743e 6a40 7c3f  |?d...|@<.t>j@|?
-00009800: 7c0e 6438 6439 8d03 0100 9007 715c 7411  |.d8d9......q\t.
-00009810: a015 a100 0100 6400 5300 296e 4e72 4100  ......d.S.)nNrA.
-00009820: 0000 7201 0000 0072 4200 0000 7243 0000  ..r....rB...rC..
-00009830: 0072 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
-00009840: 72a8 0200 0072 c600 0000 7247 0000 0072  r....r....rG...r
-00009850: 4800 0000 7239 0000 0072 4900 0000 724a  H...r9...rI...rJ
-00009860: 0000 0072 4b00 0000 724c 0000 0072 4d00  ...rK...rL...rM.
-00009870: 0000 7265 0000 0072 6600 0000 e700 0000  ..re...rf.......
-00009880: 0000 8036 40da 0870 7366 7369 7a65 5f7a  ...6@..psfsize_z
-00009890: 0a0a 5a50 3a7b 3a2e 3166 7d72 6a00 0000  ..ZP:{:.1f}rj...
-000098a0: 72a7 0200 0072 6900 0000 726b 0000 0072  r....ri...rk...r
-000098b0: 6c00 0000 7a0e 5f7b 7d5f 7b7d 6b70 632e  l...z._{}_{}kpc.
-000098c0: 6669 7473 726d 0000 0072 6e00 0000 726f  fitsrm...rn...ro
-000098d0: 0000 0072 7000 0000 7274 0000 0072 7600  ...rp...rt...rv.
-000098e0: 0000 7278 0000 0072 7900 0000 727b 0000  ..rx...ry...r{..
-000098f0: 007a 157b 7d5f 7b7d 6b70 635f 736b 795f  .z.{}_{}kpc_sky_
-00009900: 6d61 736b 2e70 6e67 727c 0000 0072 7d00  mask.pngr|...r}.
-00009910: 0000 7240 0000 0072 7f00 0000 7280 0000  ..r@...r....r...
-00009920: 0072 8300 0000 7284 0000 0072 8500 0000  .r....r....r....
-00009930: 7286 0000 0072 8700 0000 7288 0000 0072  r....r....r....r
-00009940: 8900 0000 728a 0000 0072 8c00 0000 7a11  ....r....r....z.
-00009950: 5f7b 7d5f 7b7d 6b70 635f 736b 792e 706e  _{}_{}kpc_sky.pn
-00009960: 677a 095f 7b7d 5f7b 7d6b 7063 7291 0000  gz._{}_{}kpcr...
-00009970: 0054 7292 0000 0072 9400 0000 7295 0000  .Tr....r....r...
-00009980: 0072 9600 0000 7297 0000 0072 3800 0000  .r....r....r8...
-00009990: 728b 0000 0072 9800 0000 729b 0000 0072  r....r....r....r
-000099a0: 9c00 0000 729d 0000 0072 9e00 0000 729f  ....r....r....r.
-000099b0: 0000 0072 a000 0000 72a1 0000 0072 a200  ...r....r....r..
-000099c0: 0000 72a5 0000 0072 a600 0000 72fb 0100  ..r....r....r...
-000099d0: 0072 fc01 0000 72fd 0100 0072 fe01 0000  .r....r....r....
-000099e0: 7200 0200 0072 0102 0000 7a12 5f7b 7d5f  r....r....z._{}_
-000099f0: 7b7d 6b70 635f 7365 676d 2e70 6e67 72a9  {}kpc_segm.pngr.
-00009a00: 0000 0072 aa00 0000 72ab 0000 0072 af00  ...r....r....r..
-00009a10: 0000 72b0 0000 0072 b100 0000 72b2 0000  ..r....r....r...
-00009a20: 0072 b300 0000 72b4 0000 0072 b500 0000  .r....r....r....
-00009a30: 72b6 0000 0072 b700 0000 7234 0000 0072  r....r....r4...r
-00009a40: b800 0000 72b9 0000 0072 ba00 0000 72bb  ....r....r....r.
-00009a50: 0000 0072 bc00 0000 72bd 0000 0072 be00  ...r....r....r..
-00009a60: 0000 7262 0000 0029 0272 c100 0000 72c0  ..rb...).r....r.
-00009a70: 0000 0072 c200 0000 724e 0000 0072 4f00  ...r....rN...rO.
-00009a80: 0000 72c3 0000 0072 c400 0000 72c5 0000  ..r....r....r...
-00009a90: 0029 4172 2500 0000 72c8 0000 0072 b700  .)Ar%...r....r..
-00009aa0: 0000 72c9 0000 0072 ca00 0000 72cb 0000  ..r....r....r...
-00009ab0: 0072 1900 0000 72cc 0000 0072 d200 0000  .r....r....r....
-00009ac0: 7264 0000 0072 cd00 0000 72ce 0000 0072  rd...r....r....r
-00009ad0: dd00 0000 7203 0000 0072 e400 0000 72e5  ....r....r....r.
-00009ae0: 0000 0072 0a00 0000 72e6 0000 0072 e700  ...r....r....r..
-00009af0: 0000 72e8 0000 0072 e900 0000 72ea 0000  ..r....r....r...
-00009b00: 0072 eb00 0000 720b 0000 0072 0d00 0000  .r....r....r....
-00009b10: 720c 0000 0072 ec00 0000 72ed 0000 0072  r....r....r....r
-00009b20: 3100 0000 72ee 0000 0072 3300 0000 72ef  1...r....r3...r.
-00009b30: 0000 0072 f000 0000 72f1 0000 0072 1100  ...r....r....r..
-00009b40: 0000 7210 0000 0072 f200 0000 72d8 0000  ..r....r....r...
-00009b50: 0072 f300 0000 72f4 0000 0072 0e00 0000  .r....r....r....
-00009b60: 720f 0000 0072 2600 0000 7286 0100 0072  r....r&...r....r
-00009b70: 2102 0000 7227 0000 0072 1e02 0000 7222  !...r'...r....r"
-00009b80: 0200 0072 2302 0000 72da 0000 0072 b001  ...r#...r....r..
-00009b90: 0000 72b2 0100 0072 2402 0000 72f5 0000  ..r....r$...r...
-00009ba0: 00da 0369 6e66 72f6 0000 0072 f700 0000  ...infr....r....
-00009bb0: 72e3 0000 0072 f900 0000 72fa 0000 0072  r....r....r....r
-00009bc0: fb00 0000 72fc 0000 0072 0400 0000 72d9  ....r....r....r.
-00009bd0: 0000 0072 dc00 0000 2942 7241 0000 0072  ...r....)BrA...r
-00009be0: ff00 0000 7201 0100 0072 0201 0000 7203  ....r....r....r.
-00009bf0: 0100 0072 0801 0000 7204 0100 0072 0501  ...r....r....r..
-00009c00: 0000 7206 0100 0072 0701 0000 72c1 0000  ..r....r....r...
-00009c10: 0072 7100 0000 7272 0000 0072 7300 0000  .rq...rr...rs...
-00009c20: 72c0 0000 0072 ae00 0000 7209 0100 0072  r....r....r....r
-00009c30: b300 0000 720a 0100 0072 0b01 0000 720c  ....r....r....r.
-00009c40: 0100 0072 0d01 0000 722d 0000 0072 1601  ...r....r-...r..
-00009c50: 0000 7217 0100 0072 ac00 0000 7218 0100  ..r....r....r...
-00009c60: 0072 2b00 0000 722c 0000 0072 1a01 0000  .r+...r,...r....
-00009c70: 721b 0100 0072 1c01 0000 721d 0100 0072  r....r....r....r
-00009c80: 1e01 0000 721f 0100 0072 2001 0000 728e  ....r....r ...r.
-00009c90: 0000 0072 2101 0000 7222 0100 0072 2301  ...r!...r"...r#.
-00009ca0: 0000 7224 0100 0072 2501 0000 7226 0100  ..r$...r%...r&..
-00009cb0: 0072 2701 0000 7228 0100 0072 2901 0000  .r'...r(...r)...
-00009cc0: 7281 0000 0072 2a01 0000 722b 0100 0072  r....r*...r+...r
-00009cd0: 2c01 0000 722d 0100 0072 3402 0000 7236  ,...r-...r4...r6
-00009ce0: 0200 0072 3301 0000 7237 0200 0072 c401  ...r3...r7...r..
-00009cf0: 0000 722e 0100 0072 2f01 0000 7230 0100  ..r....r/...r0..
-00009d00: 0072 3101 0000 7232 0100 0072 3401 0000  .r1...r2...r4...
-00009d10: 7235 0100 0072 e500 0000 7236 0100 0072  r5...r....r6...r
-00009d20: 3701 0000 722f 0000 0072 2f00 0000 7230  7...r/...r/...r0
-00009d30: 0000 0072 ab02 0000 fd06 0000 737a 0100  ...r........sz..
-00009d40: 0000 061a 0110 0118 010e 010e 011c 0114  ................
-00009d50: 0110 0110 0114 011c 010c 0102 ff08 040e  ................
-00009d60: 0108 0304 0110 020e 010e 0204 0104 0104  ................
-00009d70: 010a 0104 0516 0102 0002 ff08 020a 050e  ................
-00009d80: 0108 0108 0108 0102 ff06 020c 010e 0110  ................
-00009d90: 0102 ff04 0102 ff06 020a 010a 0208 0306  ................
-00009da0: 0102 ff0c 020e 0108 010e 010e 010e 0306  ................
-00009db0: 0106 0006 ff06 0208 0206 0108 0102 0002  ................
-00009dc0: 0102 fe06 040a 020c 0110 0110 0102 ff04  ................
-00009dd0: 0102 ff06 020a 010a 0208 0218 011a 0118  ................
-00009de0: 0110 0310 0718 0104 0108 0126 0124 010e  ...........&.$..
-00009df0: 0508 010e 0108 0308 010e 010e 020a 0108  ................
-00009e00: 0108 0208 010c 010e 010a 010a 0208 0108  ................
-00009e10: 0202 0002 fe06 0f08 0108 050c 0112 010e  ................
-00009e20: 020a 0102 ff06 0214 0112 012e 020a 010a  ................
-00009e30: 0108 0112 0102 0002 ff06 020e 010a 010a  ................
-00009e40: 0208 050e 0108 0208 0110 0112 0106 0104  ................
-00009e50: 0002 0002 0002 ff06 0214 010c 0220 0208  ............. ..
-00009e60: 0108 020a 010c 011a 0208 011a 0102 0002  ................
-00009e70: 0002 0002 0002 0102 0002 fe06 040a 0222  ..............."
-00009e80: 011a 0214 0114 0114 0114 0114 0218 0210  ................
-00009e90: 0108 0116 0102 0002 0002 0002 0002 0002  ................
-00009ea0: 0002 0102 0002 fe06 040a 0222 011a 0214  ..........."....
-00009eb0: 0114 0114 0114 0114 0214 0272 ab02 0000  ...........r....
-00009ec0: 7262 0000 0063 0600 0000 0000 0000 0000  rb...c..........
-00009ed0: 0000 3700 0000 0d00 0000 4300 0000 7326  ..7.......C...s&
-00009ee0: 0900 0064 0164 006c 007d 0674 01a0 027c  ...d.d.l.}.t...|
-00009ef0: 0164 0219 007c 0064 007c 0485 0219 006b  .d...|.d.|.....k
-00009f00: 02a1 0164 0119 0064 0119 007d 077c 0164  ...d...d...}.|.d
-00009f10: 0319 007c 0719 0074 031b 007d 0874 01a0  ...|...t...}.t..
-00009f20: 0474 01a0 0564 04a1 01a1 017c 0814 0064  .t...d.....|...d
-00009f30: 0514 007d 0964 067d 0a7c 027c 091b 007c  ...}.d.}.|.|...|
-00009f40: 0a1b 0064 0714 007d 0b74 0674 076a 0864  ...d...}.t.t.j.d
-00009f50: 0817 0083 0101 0074 0664 0983 0101 0064  .......t.d.....d
-00009f60: 0a7d 0c64 0ba0 097c 0064 007c 0485 0219  .}.d...|.d.|....
-00009f70: 0064 0c7c 02a1 037d 0d74 0a6a 0ba0 0c7c  .d.|...}.t.j...|
-00009f80: 0da1 0173 f274 0664 0d7c 0d9b 0064 0e9d  ...s.t.d.|...d..
-00009f90: 0383 0101 0064 0fa0 097c 0164 1019 007c  .....d...|.d...|
-00009fa0: 0719 007c 0164 1119 007c 0719 0074 0d7c  ...|.d...|...t.|
-00009fb0: 0b83 01a1 037d 0e7c 0c7c 0e17 007d 0f74  .....}.|.|...}.t
-00009fc0: 067c 0f83 0101 0074 0ea0 0f7c 0f7c 0da1  .|.....t...|.|..
-00009fd0: 0201 006e 1074 0664 127c 0d9b 0064 139d  ...n.t.d.|...d..
-00009fe0: 0383 0101 0064 0ba0 097c 0064 007c 0485  .....d...|.d.|..
-00009ff0: 0219 0064 147c 02a1 037d 0d74 0a6a 0ba0  ...d.|...}.t.j..
-0000a000: 0c7c 0da1 0190 0173 7674 0664 0d7c 0d9b  .|.....svt.d.|..
-0000a010: 0064 0e9d 0383 0101 0064 15a0 097c 0164  .d.......d...|.d
-0000a020: 1019 007c 0719 007c 0164 1119 007c 0719  ...|...|.d...|..
-0000a030: 0074 0d7c 0b83 01a1 037d 0e7c 0c7c 0e17  .t.|.....}.|.|..
-0000a040: 007d 0f74 067c 0f83 0101 0074 0ea0 0f7c  .}.t.|.....t...|
-0000a050: 0f7c 0da1 0201 006e 1074 0664 127c 0d9b  .|.....n.t.d.|..
-0000a060: 0064 139d 0383 0101 0074 10a0 1164 0ba0  .d.......t...d..
-0000a070: 097c 0064 007c 0485 0219 0064 0c7c 02a1  .|.d.|.....d.|..
-0000a080: 03a1 017d 107c 1064 0119 006a 127d 1174  ...}.|.d...j.}.t
-0000a090: 13a0 1464 0ba0 097c 0064 007c 0485 0219  ...d...|.d.|....
-0000a0a0: 0064 0c7c 02a1 03a1 0164 0119 007d 1274  .d.|.....d...}.t
-0000a0b0: 10a0 1164 0ba0 097c 0064 007c 0485 0219  ...d...|.d.|....
-0000a0c0: 0064 147c 02a1 03a1 017d 137c 1364 0119  .d.|.....}.|.d..
-0000a0d0: 006a 127d 1474 15a0 167c 03a1 017d 1574  .j.}.t...|...}.t
-0000a0e0: 01a0 027c 1564 1619 007c 006b 02a1 0164  ...|.d...|.k...d
-0000a0f0: 0119 0064 0119 007d 167c 1564 1719 007c  ...d...}.|.d...|
-0000a100: 1619 007d 177c 1564 1819 007c 1619 007d  ...}.|.d...|...}
-0000a110: 187c 1564 1919 007c 1619 007d 1974 01a0  .|.d...|...}.t..
-0000a120: 177c 1564 1a19 007c 1619 00a1 017d 1a7c  .|.d...|.....}.|
-0000a130: 1564 1b19 007c 1619 007d 1b7c 1564 1c19  .d...|...}.|.d..
-0000a140: 007c 1619 007d 1c74 136a 187c 1764 1d18  .|...}.t.j.|.d..
-0000a150: 007c 1864 1d18 007c 1b7c 197c 1a64 1e17  .|.d...|.|.|.d..
-0000a160: 0074 0d7c 06a0 197c 1b7c 1b64 1f7c 1918  .t.|...|.|.d.|..
-0000a170: 0014 00a1 0264 0714 0083 0164 208d 067d  .....d.....d ..}
-0000a180: 1d7c 1b64 0714 007d 1b74 136a 187c 1764  .|.d...}.t.j.|.d
-0000a190: 1d18 007c 1864 1d18 007c 1b7c 197c 1a64  ...|.d...|.|.|.d
-0000a1a0: 1e17 0074 0d7c 06a0 197c 1b7c 1b64 1f7c  ...t.|...|.|.d.|
-0000a1b0: 1918 0014 00a1 0264 0714 0083 0164 208d  .......d.....d .
-0000a1c0: 067d 1e74 13a0 1a7c 1d7c 127c 1174 016a  .}.t...|.|.|.t.j
-0000a1d0: 1b14 00a1 037d 1f74 13a0 1a7c 1e7c 127c  .....}.t...|.|.|
-0000a1e0: 1174 016a 1b14 00a1 037d 2074 1c6a 1d64  .t.j.....} t.j.d
-0000a1f0: 2164 228d 017d 2174 01a0 1e7c 1164 23a1  !d"..}!t...|.d#.
-0000a200: 027d 2274 01a0 1e7c 1164 24a1 027d 2374  .}"t...|.d$..}#t
-0000a210: 1c6a 1f7c 1164 2564 2664 277c 227c 2364  .j.|.d%d&d'|"|#d
-0000a220: 288d 0601 0074 1ca0 207c 1e64 0064 0085  (....t.. |.d.d..
-0000a230: 0264 0166 0219 007c 1e64 0064 0085 0264  .d.f...|.d.d...d
-0000a240: 1f66 0219 0064 29a1 0301 0074 1ca0 21a1  .f...d)....t..!.
-0000a250: 0001 0074 1ca0 2264 2aa1 0101 0074 1ca0  ...t.."d*....t..
-0000a260: 2364 2ba1 0101 0074 1ca0 24a1 0001 0074  #d+....t..$....t
-0000a270: 1c6a 2564 2ca0 097c 0064 007c 0485 0219  .j%d,..|.d.|....
-0000a280: 0064 0c7c 02a1 0364 2d64 2e8d 0201 007c  .d.|...d-d.....|
-0000a290: 0564 2f6b 0290 0372 c074 1ca0 26a1 0001  .d/k...r.t..&...
-0000a2a0: 006e 0874 1ca0 27a1 0001 0074 01a0 287c  .n.t..'....t..(|
-0000a2b0: 117c 2017 00a1 017d 2474 01a0 287c 147c  .| ....}$t..(|.|
-0000a2c0: 2017 00a1 017d 2564 307d 2664 3174 01a0   ....}%d0}&d1t..
-0000a2d0: 297c 24a1 0114 0064 3017 007d 2764 3174  )|$....d0..}'d1t
-0000a2e0: 01a0 297c 25a1 0114 0064 3017 007d 2864  ..)|%....d0..}(d
-0000a2f0: 3264 3364 347c 277c 2818 0014 0017 0013  2d3d4|'|(.......
-0000a300: 007d 2964 3574 01a0 297c 0864 3614 00a1  .})d5t..)|.d6...
-0000a310: 0114 0064 3717 007c 2717 007d 2a64 3574  ...d7..|'..}*d5t
-0000a320: 01a0 297c 0864 3614 00a1 0114 0064 3717  ..)|.d6......d7.
-0000a330: 007c 2817 007d 2b64 3264 3864 397c 2a18  .|(..}+d2d8d9|*.
-0000a340: 0014 0013 007d 2c7c 2c7c 2914 007d 2d7a  .....},|,|)..}-z
-0000a350: c47c 0164 1c19 007c 0719 007d 2e74 2a7c  .|.d...|...}.t*|
-0000a360: 2e14 0074 031b 007d 2f74 2b7c 087c 2f18  ...t...}/t+|.|/.
-0000a370: 0083 0164 3a14 007d 3074 01a0 2c7c 0164  ...d:..}0t..,|.d
-0000a380: 3b19 00a1 017d 317c 317c 0719 0064 3c6b  ;....}1|1|...d<k
-0000a390: 0390 0572 2274 2d7c 0164 1019 007c 0719  ...r"t-|.d...|..
-0000a3a0: 007c 0164 1119 007c 0719 0074 2e6a 2f64  .|.d...|...t.j/d
-0000a3b0: 3d8d 037d 3274 2d7c 0164 3b19 007c 0719  =..}2t-|.d;..|..
-0000a3c0: 007c 0164 3e19 007c 0719 0074 2e6a 2f64  .|.d>..|...t.j/d
-0000a3d0: 3d8d 037d 337c 32a0 307c 33a1 017d 347c  =..}3|2.0|3..}4|
-0000a3e0: 346a 317c 0914 007d 3574 01a0 3274 01a0  4j1|...}5t..2t..
-0000a3f0: 337c 35a1 0174 01a0 337c 30a1 0117 00a1  3|5..t..3|0.....
-0000a400: 017d 366e 0c74 016a 1b7d 3574 016a 1b7d  .}6n.t.j.}5t.j.}
-0000a410: 3657 006e 0c01 0001 0001 0059 006e 0258  6W.n.......Y.n.X
-0000a420: 0074 15a0 167c 03a1 017d 1574 01a0 027c  .t...|...}.t...|
-0000a430: 1564 1619 007c 006b 02a1 0164 0119 0064  .d...|.k...d...d
-0000a440: 0119 007d 1674 0674 076a 3464 3f17 0083  ...}.t.t.j4d?...
-0000a450: 0101 0074 0674 076a 3464 4017 0083 0101  ...t.t.j4d@.....
-0000a460: 007a 3074 01a0 297c 2da1 017c 1564 4119  .z0t..)|-..|.dA.
-0000a470: 007c 163c 0074 0674 076a 3564 42a0 0974  .|.<.t.t.j5dB..t
-0000a480: 01a0 297c 2da1 01a1 0117 0083 0101 0057  ..)|-..........W
-0000a490: 006e 6a01 0001 0001 0074 0674 076a 0864  .nj......t.t.j.d
-0000a4a0: 43a0 097c 03a1 0117 0083 0101 007c 156a  C..|.........|.j
-0000a4b0: 3674 01a0 3774 387c 1583 01a1 0174 016a  6t..7t8|.....t.j
-0000a4c0: 1b14 0064 4164 448d 0201 0074 01a0 297c  ...dAdD....t..)|
-0000a4d0: 2da1 017c 1564 4119 007c 163c 0074 0674  -..|.dA..|.<.t.t
-0000a4e0: 076a 3564 42a0 0974 01a0 297c 2da1 01a1  .j5dB..t..)|-...
-0000a4f0: 0117 0083 0101 0059 006e 0258 007a 247c  .......Y.n.X.z$|
-0000a500: 287c 1564 4519 007c 163c 0074 0674 076a  (|.dE..|.<.t.t.j
-0000a510: 3564 46a0 097c 28a1 0117 0083 0101 0057  5dF..|(........W
-0000a520: 006e 5e01 0001 0001 0074 0674 076a 0864  .n^......t.t.j.d
-0000a530: 47a0 097c 03a1 0117 0083 0101 007c 156a  G..|.........|.j
-0000a540: 3674 01a0 3774 387c 1583 01a1 0174 016a  6t..7t8|.....t.j
-0000a550: 1b14 0064 4564 448d 0201 007c 287c 1564  ...dEdD....|(|.d
-0000a560: 4519 007c 163c 0074 0674 076a 3564 46a0  E..|.<.t.t.j5dF.
-0000a570: 097c 28a1 0117 0083 0101 0059 006e 0258  .|(........Y.n.X
-0000a580: 007a 247c 277c 1564 4819 007c 163c 0074  .z$|'|.dH..|.<.t
-0000a590: 0674 076a 3564 49a0 097c 27a1 0117 0083  .t.j5dI..|'.....
-0000a5a0: 0101 0057 006e 5e01 0001 0001 0074 0674  ...W.n^......t.t
-0000a5b0: 076a 0864 4aa0 097c 03a1 0117 0083 0101  .j.dJ..|........
-0000a5c0: 007c 156a 3674 01a0 3774 387c 1583 01a1  .|.j6t..7t8|....
-0000a5d0: 0174 016a 1b14 0064 4864 448d 0201 007c  .t.j...dHdD....|
-0000a5e0: 277c 1564 4819 007c 163c 0074 0674 076a  '|.dH..|.<.t.t.j
-0000a5f0: 3564 49a0 097c 27a1 0117 0083 0101 0059  5dI..|'........Y
-0000a600: 006e 0258 007a 247c 2b7c 1564 4b19 007c  .n.X.z$|+|.dK..|
-0000a610: 163c 0074 0674 076a 3564 4ca0 097c 2ba1  .<.t.t.j5dL..|+.
-0000a620: 0117 0083 0101 0057 006e 5e01 0001 0001  .......W.n^.....
-0000a630: 0074 0674 076a 0864 4da0 097c 03a1 0117  .t.t.j.dM..|....
-0000a640: 0083 0101 007c 156a 3674 01a0 3774 387c  .....|.j6t..7t8|
-0000a650: 1583 01a1 0174 016a 1b14 0064 4b64 448d  .....t.j...dKdD.
-0000a660: 0201 007c 2b7c 1564 4b19 007c 163c 0074  ...|+|.dK..|.<.t
-0000a670: 0674 076a 3564 4ca0 097c 2ba1 0117 0083  .t.j5dL..|+.....
-0000a680: 0101 0059 006e 0258 007a 247c 2a7c 1564  ...Y.n.X.z$|*|.d
-0000a690: 4e19 007c 163c 0074 0674 076a 3564 4fa0  N..|.<.t.t.j5dO.
-0000a6a0: 097c 2aa1 0117 0083 0101 0057 006e 5e01  .|*........W.n^.
-0000a6b0: 0001 0001 0074 0674 076a 0864 50a0 097c  .....t.t.j.dP..|
-0000a6c0: 03a1 0117 0083 0101 007c 156a 3674 01a0  .........|.j6t..
-0000a6d0: 3774 387c 1583 01a1 0174 016a 1b14 0064  7t8|.....t.j...d
-0000a6e0: 4e64 448d 0201 007c 2a7c 1564 4e19 007c  NdD....|*|.dN..|
-0000a6f0: 163c 0074 0674 076a 3564 4fa0 097c 2aa1  .<.t.t.j5dO..|*.
-0000a700: 0117 0083 0101 0059 006e 0258 007a 347c  .......Y.n.X.z4|
-0000a710: 0164 5119 007c 0719 007c 1564 5219 007c  .dQ..|...|.dR..|
-0000a720: 163c 0074 0674 076a 3464 53a0 097c 0164  .<.t.t.j4dS..|.d
-0000a730: 5419 007c 0719 00a1 0117 0083 0101 0057  T..|...........W
-0000a740: 006e 0c01 0001 0001 0059 006e 0258 007a  .n.......Y.n.X.z
-0000a750: 2c7c 357c 1564 5519 007c 163c 0074 0674  ,|5|.dU..|.<.t.t
-0000a760: 076a 3464 56a0 097c 0164 5119 007c 0719  .j4dV..|.dQ..|..
-0000a770: 00a1 0117 0083 0101 0057 006e 0c01 0001  .........W.n....
-0000a780: 0001 0059 006e 0258 007a 247c 367c 1564  ...Y.n.X.z$|6|.d
-0000a790: 5719 007c 163c 0074 0674 076a 3464 58a0  W..|.<.t.t.j4dX.
-0000a7a0: 097c 35a1 0117 0083 0101 0057 006e 0c01  .|5........W.n..
-0000a7b0: 0001 0001 0059 006e 0258 007a 2c7c 0164  .....Y.n.X.z,|.d
-0000a7c0: 5419 007c 0719 007c 1564 5419 007c 163c  T..|...|.dT..|.<
-0000a7d0: 0074 0674 076a 3464 59a0 097c 36a1 0117  .t.t.j4dY..|6...
-0000a7e0: 0083 0101 0057 006e 0c01 0001 0001 0059  .....W.n.......Y
-0000a7f0: 006e 0258 0074 156a 397c 157c 0364 5a64  .n.X.t.j9|.|.dZd
-0000a800: 5b8d 0301 0064 0053 0029 5c4e 7201 0000  [....d.S.)\Nr...
-0000a810: 0072 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
-0000a820: 7244 0000 0072 a702 0000 7239 0000 007a  rD...r....r9...z
-0000a830: 230a 0a4c 6f61 6469 6e67 2f44 6f77 6e6c  #..Loading/Downl
-0000a840: 6f61 6469 6e67 2044 6563 616c 7320 696d  oading Decals im
-0000a850: 6167 6573 7258 0000 0072 a902 0000 72aa  agesrX...r....r.
-0000a860: 0200 0072 6102 0000 725d 0000 0072 5e00  ...ra...r]...r^.
-0000a870: 0000 7a34 7261 3d7b 7d26 6465 633d 7b7d  ..z4ra={}&dec={}
-0000a880: 266c 6179 6572 3d64 7238 2670 6978 7363  &layer=dr8&pixsc
-0000a890: 616c 653d 302e 3237 2662 616e 6473 3d67  ale=0.27&bands=g
-0000a8a0: 2673 697a 653d 7b7d 724e 0000 0072 4f00  &size={}rN...rO.
-0000a8b0: 0000 725b 0000 0072 5c00 0000 7268 0200  ..r[...r\...rh..
-0000a8c0: 007a 3472 613d 7b7d 2664 6563 3d7b 7d26  .z4ra={}&dec={}&
-0000a8d0: 6c61 7965 723d 6472 3826 7069 7873 6361  layer=dr8&pixsca
-0000a8e0: 6c65 3d30 2e32 3726 6261 6e64 733d 7226  le=0.27&bands=r&
-0000a8f0: 7369 7a65 3d7b 7d72 c200 0000 724f 0100  size={}r....rO..
-0000a900: 0072 5001 0000 7251 0100 0072 5201 0000  .rP...rQ...rR...
-0000a910: 724d 0100 0072 c500 0000 7249 0000 0072  rM...r....rI...r
-0000a920: 6901 0000 7269 0000 0029 06da 0278 30da  i...ri...)...x0.
-0000a930: 0279 30da 0373 6d61 da03 6570 73da 0270  .y0..sma..eps..p
-0000a940: 61da 0473 7465 7072 7400 0000 7276 0000  a..steprt...rv..
-0000a950: 0072 3700 0000 6700 0000 0000 e058 4072  .r7...g......X@r
-0000a960: fd01 0000 da08 5264 596c 4275 5f72 7278  ......RdYlBu_rrx
-0000a970: 0000 0029 0572 ff01 0000 72a8 0000 0072  ...).r....r....r
-0000a980: 7a00 0000 da04 766d 696e da04 766d 6178  z.....vmin..vmax
-0000a990: 7a03 6b2d 2d7a 0778 2028 7069 7829 7a07  z.k--z.x (pix)z.
-0000a9a0: 7920 2870 6978 297a 1d69 6d61 6765 732f  y (pix)z.images/
-0000a9b0: 6669 675f 7b7d 5f67 5f7b 7d6b 7063 5f32  fig_{}_g_{}kpc_2
-0000a9c0: 5265 2e70 6e67 727c 0000 0072 7d00 0000  Re.pngr|...r}...
-0000a9d0: 7240 0000 0072 b002 0000 7224 0000 0072  r@...r....r$...r
-0000a9e0: c701 0000 6756 0e2d b29d efdf bf67 e7fb  ....gV.-.....g..
-0000a9f0: a9f1 d24d f83f 6700 0000 0000 0014 c067  ...M.?g........g
-0000aa00: 0000 0000 8084 2e41 6700 0000 0000 0014  .......Ag.......
-0000aa10: 4067 9a99 9999 9999 d93f 6771 3d0a d7a3  @g.......?gq=...
-0000aa20: 7014 4072 df01 0000 7266 0200 0072 6b00  p.@r....rf...rk.
-0000aa30: 0000 2901 727b 0200 0072 6702 0000 7a15  ..).r{...rg...z.
-0000aa40: 0a47 656e 6572 616c 2069 6e66 6f72 6d61  .General informa
-0000aa50: 7469 6f6e 3a72 4600 0000 da04 6d61 7373  tion:rF.....mass
-0000aa60: 7a14 0a4d 6173 7320 286c 6f67 2920 3d20  z..Mass (log) = 
-0000aa70: 7b3a 2e31 667d 7a27 5468 6520 636f 6c75  {:.1f}z'The colu
-0000aa80: 6d6e 203c 3c6d 6173 733e 3e20 7761 7320  mn <<mass>> was 
-0000aa90: 6164 6465 6420 746f 2074 6865 207b 7d29  added to the {})
-0000aaa0: 01da 046e 616d 65da 096d 6167 5f72 5f32  ...name..mag_r_2
-0000aab0: 5265 7a12 6d61 675f 725f 3252 6520 3d20  Rez.mag_r_2Re = 
-0000aac0: 7b3a 2e31 667d 7a2c 5468 6520 636f 6c75  {:.1f}z,The colu
-0000aad0: 6d6e 203c 3c6d 6167 5f72 5f32 5265 3e3e  mn <<mag_r_2Re>>
-0000aae0: 2077 6173 2061 6464 6564 2074 6f20 7468   was added to th
-0000aaf0: 6520 7b7d da09 6d61 675f 675f 3252 657a  e {}..mag_g_2Rez
-0000ab00: 126d 6167 5f67 5f32 5265 203d 207b 3a2e  .mag_g_2Re = {:.
-0000ab10: 3166 7d7a 2c54 6865 2063 6f6c 756d 6e20  1f}z,The column 
-0000ab20: 3c3c 6d61 675f 675f 3252 653e 3e20 7761  <<mag_g_2Re>> wa
-0000ab30: 7320 6164 6465 6420 746f 2074 6865 207b  s added to the {
-0000ab40: 7dda 064d 725f 3252 657a 0f4d 725f 3252  }..Mr_2Rez.Mr_2R
-0000ab50: 6520 3d20 7b3a 2e31 667d 7a29 5468 6520  e = {:.1f}z)The 
-0000ab60: 636f 6c75 6d6e 203c 3c4d 725f 3252 653e  column <<Mr_2Re>
-0000ab70: 3e20 7761 7320 6164 6465 6420 746f 2074  > was added to t
-0000ab80: 6865 207b 7dda 064d 675f 3252 657a 0f4d  he {}..Mg_2Rez.M
-0000ab90: 675f 3252 6520 3d20 7b3a 2e31 667d 7a29  g_2Re = {:.1f}z)
-0000aba0: 5468 6520 636f 6c75 6d6e 203c 3c4d 675f  The column <<Mg_
-0000abb0: 3252 653e 3e20 7761 7320 6164 6465 6420  2Re>> was added 
-0000abc0: 746f 2074 6865 207b 7dda 0773 6967 6d61  to the {}..sigma
-0000abd0: 5f43 da05 7369 675f 437a 120a 4c78 2028  _C..sig_Cz..Lx (
-0000abe0: 6c6f 6729 203d 207b 3a2e 3166 7dda 024c  log) = {:.1f}..L
-0000abf0: 78da 0644 5f70 726f 6a7a 1373 6967 6d61  x..D_projz.sigma
-0000ac00: 203d 207b 3a2e 3166 7d20 6b6d 2f73 da06   = {:.1f} km/s..
-0000ac10: 445f 696e 7472 7a13 445f 7072 6f6a 203d  D_intrz.D_proj =
-0000ac20: 207b 3a2e 3166 7d20 6b70 637a 1344 5f69   {:.1f} kpcz.D_i
-0000ac30: 6e74 7220 3d20 7b3a 2e31 667d 206b 7063  ntr = {:.1f} kpc
-0000ac40: 5472 9200 0000 293a da09 6675 6e63 7469  Tr....):..functi
-0000ac50: 6f6e 7372 2500 0000 72c8 0000 0072 b700  onsr%...r....r..
-0000ac60: 0000 72c9 0000 0072 ca00 0000 72cb 0000  ..r....r....r...
-0000ac70: 0072 1900 0000 72dd 0000 0072 6400 0000  .r....r....rd...
-0000ac80: 72d4 0000 0072 d500 0000 72d6 0000 0072  r....r....r....r
-0000ac90: d800 0000 721a 0000 0072 1300 0000 7203  ....r....r....r.
-0000aca0: 0000 0072 e400 0000 72e5 0000 0072 ab01  ...r....r....r..
-0000acb0: 0000 da05 6361 6c6c 6672 0400 0000 72d9  ....callfr....r.
-0000acc0: 0000 00da 0772 6164 3264 6567 da07 656c  .....rad2deg..el
-0000acd0: 6c69 7073 65da 1070 6572 695f 656c 6c69  lipse..peri_elli
-0000ace0: 705f 6578 6163 74da 086d 6173 6b70 6f6c  p_exact..maskpol
-0000acf0: 7972 2700 0000 72e6 0000 0072 e700 0000  yr'...r....r....
-0000ad00: da0d 6e61 6e70 6572 6365 6e74 696c 6572  ..nanpercentiler
-0000ad10: e800 0000 da04 706c 6f74 72ba 0100 0072  ......plotr....r
-0000ad20: 2702 0000 7228 0200 0072 2402 0000 72e9  '...r(...r$...r.
-0000ad30: 0000 0072 ea00 0000 72eb 0000 00da 066e  ...r....r......n
-0000ad40: 616e 7375 6d72 2800 0000 72fd 0000 0072  ansumr(...r....r
-0000ad50: 7c02 0000 7226 0200 0072 0900 0000 7273  |...r&...r....rs
-0000ad60: 0200 0072 6e02 0000 7276 0200 0072 7502  ...rn...rv...ru.
-0000ad70: 0000 72ee 0000 0072 cd00 0000 72cc 0000  ..r....r....r...
-0000ad80: 0072 d200 0000 da0a 6164 645f 636f 6c75  .r......add_colu
-0000ad90: 6d6e da05 7a65 726f 7372 e300 0000 72dc  mn..zerosr....r.
-0000ada0: 0000 0029 3772 4100 0000 72ff 0000 0072  ...)7rA...r....r
-0000adb0: 0101 0000 72c0 0000 00da 0773 7566 5f6e  ....r......suf_n
-0000adc0: 756d 72c1 0000 00da 0466 756e 6372 0901  umr......funcr..
-0000add0: 0000 72b3 0000 0072 0a01 0000 72b4 0100  ..r....r....r...
-0000ade0: 0072 0b01 0000 72ac 0200 0072 d500 0000  .r....r....r....
-0000adf0: 723a 0200 0072 ad02 0000 721a 0100 0072  r:...r....r....r
-0000ae00: 1b01 0000 da05 696d 6178 79da 0569 6d61  ......imaxy..ima
-0000ae10: 726e da04 696d 6172 72e5 0000 0072 3601  rn..imarr....r6.
-0000ae20: 0000 da0a 6365 6e74 785f 7068 6f74 da0a  ....centx_phot..
-0000ae30: 6365 6e74 795f 7068 6f74 da04 6570 7330  centy_phot..eps0
-0000ae40: 725d 0100 00da 0873 6d61 656c 6c69 70da  r].....smaellip.
-0000ae50: 057a 5f67 616c da0d 6761 6c5f 706f 6c5f  .z_gal..gal_pol_
-0000ae60: 3152 6566 66da 0d67 616c 5f70 6f6c 5f32  1Reff..gal_pol_2
-0000ae70: 5265 6666 da09 6d61 736b 5f67 616c 31da  Reff..mask_gal1.
-0000ae80: 096d 6173 6b5f 6761 6c32 721d 0100 0072  .mask_gal2r....r
-0000ae90: ba02 0000 72bb 0200 00da 0566 6c75 7867  ....r......fluxg
-0000aea0: da05 666c 7578 7272 2d00 0000 da05 6d61  ..fluxrr-.....ma
-0000aeb0: 675f 67da 056d 6167 5f72 da03 4d4c 67da  g_g..mag_r..MLg.
-0000aec0: 024d 67da 024d 72da 024c 67da 0c6d 6173  .Mg..Mr..Lg..mas
-0000aed0: 735f 7374 656c 6c61 72da 037a 5f43 da05  s_stellar..z_C..
-0000aee0: 445f 6761 6cda 0764 656c 7461 5f44 724e  D_gal..delta_DrN
-0000aef0: 0000 00da 0963 6f6f 7264 5f67 616c da07  .....coord_gal..
-0000af00: 636f 6f72 645f 4372 8302 0000 7284 0200  coord_Cr....r...
-0000af10: 00da 0544 5f69 6e74 722f 0000 0072 2f00  ...D_intr/...r/.
-0000af20: 0000 7230 0000 00da 0b6d 6173 735f 6465  ..r0.....mass_de
-0000af30: 6361 6c73 eb07 0000 737a 0100 0000 0308  cals....sz......
-0000af40: 0222 0110 0118 0104 0110 020e 0108 0204  ."..............
-0000af50: 0116 010c 0110 0104 010a 000a 0006 ff04  ................
-0000af60: 0208 0108 020e 0210 0216 010e 0110 0104  ................
-0000af70: 010a 000a 0006 ff04 0208 0108 020e 0210  ................
-0000af80: 0214 0102 ff06 020a 0214 0102 ff04 0102  ................
-0000af90: ff04 0414 0102 ff06 020a 020a 021a 020c  ................
-0000afa0: 010c 010c 0112 010c 010c 0210 0102 0002  ................
-0000afb0: 0006 011a fe06 0408 0110 0102 0002 0006  ................
-0000afc0: 011a fe06 0414 0114 020c 010c 010c 020c  ................
-0000afd0: 0102 0002 ff06 0226 0108 010a 010a 0108  .......&........
-0000afe0: 0114 0102 ff02 0102 ff06 020a 010a 0208  ................
-0000aff0: 020e 010e 0204 0212 0112 0214 011a 011a  ................
-0000b000: 0110 0108 0302 010c 010c 0110 020e 010e  ................
-0000b010: 0120 0120 010a 020a 011c 0206 010a 0106  . . ............
-0000b020: 0106 020a 011a 020e 010e 0202 0112 011e  ................
-0000b030: 0106 010a 0102 ff08 021e 0112 0120 0102  ............. ..
-0000b040: 010c 0118 0106 010a 0102 ff08 021e 010c  ................
-0000b050: 011a 0102 010c 0118 0106 010a 0102 ff08  ................
-0000b060: 021e 010c 011a 0102 010c 0118 0106 010a  ................
-0000b070: 0102 ff08 021e 010c 011a 0102 010c 0118  ................
-0000b080: 0106 010a 0102 ff08 021e 010c 011a 0102  ................
-0000b090: 0114 0120 0106 0106 0102 010c 0120 0106  ... ......... ..
-0000b0a0: 0106 0102 010c 0118 0106 0106 0102 0114  ................
-0000b0b0: 0118 0106 0106 0272 ef02 0000 2902 7240  .......r....).r@
-0000b0c0: 0000 0072 3f00 0000 2904 723a 0000 0072  ...r?...).r:...r
-0000b0d0: 3f02 0000 72c6 0100 004e 2903 723a 0000  ?...r....N).r:..
-0000b0e0: 0072 0f02 0000 720f 0200 0029 0a72 3a00  .r....r....).r:.
-0000b0f0: 0000 720f 0200 0072 0f02 0000 72c7 0100  ..r....r....r...
-0000b100: 0072 9700 0000 72c7 0100 0072 3b00 0000  .r....r....r;...
-0000b110: 72c6 0100 0072 c801 0000 7254 0200 0029  r....r....rT...)
-0000b120: 0e4e 4e72 c701 0000 7297 0000 0072 c701  .NNr....r....r..
-0000b130: 0000 4e54 72c8 0100 0072 3b00 0000 7201  ..NTr....r;...r.
-0000b140: 0000 0072 4000 0000 7240 0000 0072 c801  ...r@...r@...r..
-0000b150: 0000 723c 0000 0029 0372 3f00 0000 7262  ..r<...).r?...rb
-0000b160: 0000 0072 4000 0000 2950 da05 6e75 6d70  ...r@...)P..nump
-0000b170: 7972 2500 0000 da11 6d61 7470 6c6f 746c  yr%.....matplotl
-0000b180: 6962 2e70 7970 6c6f 74da 0670 7970 6c6f  ib.pyplot..pyplo
-0000b190: 7472 e600 0000 72f6 0000 005a 2173 7461  tr....r....Z!sta
-0000b1a0: 746d 6f72 7068 2e75 7469 6c73 2e69 6d61  tmorph.utils.ima
-0000b1b0: 6765 5f64 6961 676e 6f73 7469 6373 7202  ge_diagnosticsr.
-0000b1c0: 0000 00da 0a61 7374 726f 7079 2e69 6f72  .....astropy.ior
-0000b1d0: 0300 0000 7204 0000 00da 0d61 7374 726f  ....r......astro
-0000b1e0: 7079 2e74 6162 6c65 7205 0000 00da 0a61  py.tabler......a
-0000b1f0: 7374 726f 7175 6572 7972 0600 0000 da13  stroqueryr......
-0000b200: 6173 7472 6f71 7565 7279 2e69 7061 632e  astroquery.ipac.
-0000b210: 6e65 6472 0700 0000 5a0b 6173 7472 6f70  nedr....Z.astrop
-0000b220: 792e 7763 7372 0800 0000 da13 6173 7472  y.wcsr......astr
-0000b230: 6f70 792e 636f 6f72 6469 6e61 7465 7372  opy.coordinatesr
-0000b240: 0900 0000 da0d 6173 7472 6f70 792e 756e  ......astropy.un
-0000b250: 6974 73da 0575 6e69 7473 7273 0200 0072  its..unitsrs...r
-0000b260: f300 0000 720a 0000 00da 0d61 7374 726f  ....r......astro
-0000b270: 7079 2e73 7461 7473 720b 0000 005a 1470  py.statsr....Z.p
-0000b280: 686f 7475 7469 6c73 2e62 6163 6b67 726f  hotutils.backgro
-0000b290: 756e 6472 0c00 0000 720d 0000 005a 1670  undr....r....Z.p
-0000b2a0: 686f 7475 7469 6c73 2e73 6567 6d65 6e74  hotutils.segment
-0000b2b0: 6174 696f 6e72 0e00 0000 720f 0000 00da  ationr....r.....
-0000b2c0: 1361 7374 726f 7079 2e63 6f6e 766f 6c75  .astropy.convolu
-0000b2d0: 7469 6f6e 7210 0000 0072 1100 0000 da0c  tionr....r......
-0000b2e0: 7572 6c6c 6962 2e70 6172 7365 7212 0000  urllib.parser...
-0000b2f0: 00da 0e75 726c 6c69 622e 7265 7175 6573  ...urllib.reques
-0000b300: 7472 1300 0000 da15 6173 7472 6f70 792e  tr......astropy.
-0000b310: 7669 7375 616c 697a 6174 696f 6e72 1400  visualizationr..
-0000b320: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-0000b330: 0072 1800 0000 da08 636f 6c6f 7261 6d61  .r......colorama
-0000b340: 7219 0000 00da 0d73 6369 7079 2e6e 6469  r......scipy.ndi
-0000b350: 6d61 6765 da07 6e64 696d 6167 65da 036e  mage..ndimage..n
-0000b360: 6469 da04 7767 6574 da06 7572 6c6c 6962  di..wget..urllib
-0000b370: 721a 0000 0072 b700 0000 72fd 0000 0072  r....r....r....r
-0000b380: d400 0000 72f5 0000 00da 0e70 6c6f 745f  ....r......plot_
-0000b390: 6675 6e63 7469 6f6e 7372 ab01 0000 72ad  functionsr....r.
-0000b3a0: 0100 00da 0973 6572 7665 725f 6672 da09  .....server_fr..
-0000b3b0: 7365 7276 655f 7573 6172 4002 0000 da14  serve_usar@.....
-0000b3c0: 7265 7365 745f 766f 7461 626c 655f 6669  reset_votable_fi
-0000b3d0: 656c 6473 da15 7265 6d6f 7665 5f76 6f74  elds..remove_vot
-0000b3e0: 6162 6c65 5f66 6965 6c64 73da 1261 6464  able_fields..add
-0000b3f0: 5f76 6f74 6162 6c65 5f66 6965 6c64 7372  _votable_fieldsr
-0000b400: 3100 0000 7236 0000 0072 3901 0000 72fc  1...r6...r9...r.
-0000b410: 0000 0072 3e02 0000 7217 0200 0072 5302  ...r>...r....rS.
-0000b420: 0000 7296 0200 0072 1b02 0000 72af 0200  ..r....r....r...
-0000b430: 0072 ab02 0000 72ef 0200 0072 2f00 0000  .r....r....r/...
-0000b440: 722f 0000 0072 2f00 0000 7230 0000 00da  r/...r/...r0....
-0000b450: 083c 6d6f 6475 6c65 3e01 0000 0073 3c01  .<module>....s<.
-0000b460: 0000 0801 0c02 0801 0c02 1001 0c01 0c01  ................
-0000b470: 0c01 0c01 0c01 0c02 0c01 0c01 1001 0c01  ................
-0000b480: 0c02 0c01 0c02 0c01 0c01 1c03 0c02 0c02  ................
-0000b490: 0802 0801 0c02 0401 0401 0801 0802 0803  ................
-0000b4a0: 0402 0401 0406 0a02 0c09 0e01 0200 0200  ................
-0000b4b0: 0201 0200 0200 0200 0201 0200 0200 0200  ................
-0000b4c0: 02fd 0406 0806 0805 0601 0200 0200 0601  ................
-0000b4d0: 0200 0200 0200 0200 0201 0200 0200 02fd  ................
-0000b4e0: 0a7f 007f 006c 0001 00fe 0a7f 0039 0601  .....l.......9..
-0000b4f0: 0200 0200 0200 0200 0201 0200 0600 0200  ................
-0000b500: 0201 0200 0200 0200 0201 0200 0200 0200  ................
-0000b510: 0200 0201 02fb 0a7f 007f 007f 0000 0001  ................
-0000b520: 00ff 0a2c 0001 00ff 0a25 0001 0000 0000  ...,.....%......
-0000b530: 0000 0001 0000 0000 0001 00fd 0a7f 0033  ...............3
-0000b540: 0001 0000 0000 0000 0001 0000 0000 0000  ................
-0000b550: 0001 0000 0000 0001 0000 00fc 0a7f 007f  ................
-0000b560: 002c 0401 0200 0200 0600 0201 0200 0200  .,..............
-0000b570: 0201 0200 0200 02fd 0a7f 0060 0601 0201  ...........`....
-0000b580: 0200 0200 0601 0200 0200 0200 0201 0200  ................
-0000b590: 0200 02fc 0a7f 006f 0001 0000 00ff       .......o......
+00002880: a010 a100 0100 6409 7d13 740c a017 640a  ......d.}.t...d.
+00002890: 640b 8400 7c0f 6404 1900 4400 8301 a101  d...|.d...D.....
+000028a0: 7d14 7412 7c01 8301 740c a018 7c14 a101  }.t.|...t...|...
+000028b0: 6b04 9002 7220 7408 640c 8301 0100 7c0f  k...r t.d.....|.
+000028c0: 6404 1900 a011 6405 740b 7412 7c01 8301  d.....d.t.t.|...
+000028d0: 8301 1700 a101 7d15 7c0f a019 6404 7c15  ......}.|...d.|.
+000028e0: a102 0100 7c01 7c0f 6404 1900 7c13 3c00  ....|.|.d...|.<.
+000028f0: 7408 640d a016 7c00 6a1a a101 8301 0100  t.d...|.j.......
+00002900: 7408 640e a016 7c00 6a1b a101 8301 0100  t.d...|.j.......
+00002910: 7408 640f 7c00 6a1c 8302 0100 7408 6410  t.d.|.j.....t.d.
+00002920: 7c00 6a1d 8302 0100 7408 6411 8301 0100  |.j.....t.d.....
+00002930: 7c00 6a1e 7c0f 6412 1900 7c13 3c00 7c00  |.j.|.d...|.<.|.
+00002940: 6a1f 7c0f 6413 1900 7c13 3c00 7c00 6a20  j.|.d...|.<.|.j 
+00002950: 7c0f 6414 1900 7c13 3c00 7c00 6a21 7c0f  |.d...|.<.|.j!|.
+00002960: 6415 1900 7c13 3c00 7c00 6a22 7c0f 6416  d...|.<.|.j"|.d.
+00002970: 1900 7c13 3c00 7c00 6a23 7c0f 6417 1900  ..|.<.|.j#|.d...
+00002980: 7c13 3c00 7c00 6a24 7c0f 6418 1900 7c13  |.<.|.j$|.d...|.
+00002990: 3c00 7c00 6a25 7c0f 6419 1900 7c13 3c00  <.|.j%|.d...|.<.
+000029a0: 7c00 6a26 7c0f 641a 1900 7c13 3c00 7c00  |.j&|.d...|.<.|.
+000029b0: 6a27 7c0f 641b 1900 7c13 3c00 7c00 6a28  j'|.d...|.<.|.j(
+000029c0: 7c0f 641c 1900 7c13 3c00 7c00 6a29 7c0f  |.d...|.<.|.j)|.
+000029d0: 641d 1900 7c13 3c00 7c00 6a2a 7c0f 641e  d...|.<.|.j*|.d.
+000029e0: 1900 7c13 3c00 7c00 6a2b 7c0f 641f 1900  ..|.<.|.j+|.d...
+000029f0: 7c13 3c00 7c00 6a2c 7c0f 6420 1900 7c13  |.<.|.j,|.d ..|.
+00002a00: 3c00 7c00 6a2d 7c0f 6421 1900 7c13 3c00  <.|.j-|.d!..|.<.
+00002a10: 7c00 6a2e 7c0f 6422 1900 7c13 3c00 7408  |.j.|.d"..|.<.t.
+00002a20: 7409 6a0a 6423 a016 7c00 6a2b a101 1700  t.j.d#..|.j+....
+00002a30: 8301 0100 7c00 6a2f 7c0f 6424 1900 7c13  ....|.j/|.d$..|.
+00002a40: 3c00 7c00 6a30 7c0f 6425 1900 7c13 3c00  <.|.j0|.d%..|.<.
+00002a50: 7c00 6a31 7c0f 6426 1900 7c13 3c00 7c00  |.j1|.d&..|.<.|.
+00002a60: 6a32 7c0f 6427 1900 7c13 3c00 7c00 6a33  j2|.d'..|.<.|.j3
+00002a70: 7c0f 6428 1900 7c13 3c00 7c00 6a34 7c0f  |.d(..|.<.|.j4|.
+00002a80: 6429 1900 7c13 3c00 7c00 6a35 7c0f 642a  d)..|.<.|.j5|.d*
+00002a90: 1900 7c13 3c00 7c00 6a36 7c0f 642b 1900  ..|.<.|.j6|.d+..
+00002aa0: 7c13 3c00 7c00 6a37 7c0f 642c 1900 7c13  |.<.|.j7|.d,..|.
+00002ab0: 3c00 7c00 6a38 7c0f 642d 1900 7c13 3c00  <.|.j8|.d-..|.<.
+00002ac0: 7c00 6a39 7c0f 642e 1900 7c13 3c00 7c00  |.j9|.d...|.<.|.
+00002ad0: 6a3a 7c0f 642f 1900 7c13 3c00 7c00 6a1c  j:|.d/..|.<.|.j.
+00002ae0: 7c0f 6430 1900 7c13 3c00 7c00 6a1d 7c0f  |.d0..|.<.|.j.|.
+00002af0: 6431 1900 7c13 3c00 7c09 7c0f 6432 1900  d1..|.<.|.|.d2..
+00002b00: 7c13 3c00 7c0c 7c0f 6433 1900 7c13 3c00  |.<.|.|.d3..|.<.
+00002b10: 7403 6a3b 7c0f 7c0e 6434 6435 8d03 0100  t.j;|.|.d4d5....
+00002b20: 7c02 6a3c 5c02 7d16 7d17 740c 6a3d 6406  |.j<\.}.}.t.j=d.
+00002b30: 7c16 8502 6406 7c17 8502 6602 1900 5c02  |...d.|...f...\.
+00002b40: 7d18 7d19 743e 6a3f 7c00 6a34 7c00 6a35  }.}.t>j?|.j4|.j5
+00002b50: 7c00 6a36 7c00 6a37 7c00 6a38 7c00 6a39  |.j6|.j7|.j8|.j9
+00002b60: 7c00 6a3a 6436 8d07 7d1a 7c1a a040 7c08  |.j:d6..}.|..@|.
+00002b70: a101 0100 7c1a 7c19 7c18 8302 7d1b 7441  ....|.|.|...}.tA
+00002b80: 6a42 6437 6438 8d01 7d1c 6406 6439 6c43  jBd7d8..}.d.d9lC
+00002b90: 6d44 7d1d 0100 7c1d 7c1c 643a 643b 643c  mD}...|.|.d:d;d<
+00002ba0: 643d 643e 643f 6440 6441 8d08 7d1e 7c1e  d=d>d?d@dA..}.|.
+00002bb0: 6406 1900 7d1f 740c a045 7c03 a101 7d20  d...}.t..E|...} 
+00002bc0: 7c20 740c a046 7c20 a101 0f00 1900 7d20  | t..F| ......} 
+00002bd0: 740c a047 7c20 6442 a102 7d21 740c a047  t..G| dB..}!t..G
+00002be0: 7c20 6443 a102 7d22 7448 6a49 7c03 6a3c  | dC..}"tHjI|.j<
+00002bf0: 6442 1900 6444 1b00 7c02 6a3c 6406 1900  dB..dD..|.j<d...
+00002c00: 6444 1b00 6702 7c0a 6445 7c0b 1b00 6446  dD..g.|.dE|...dF
+00002c10: 6447 6445 6448 6449 644a 644b 644c 6444  dGdEdHdIdJdKdLdD
+00002c20: 7c1f 644d 644e 8d0e 0100 7448 6a42 7c03  |.dMdN....tHjB|.
+00002c30: 6406 6406 6702 6406 6406 6702 7c21 7c22  d.d.g.d.d.g.|!|"
+00002c40: 6406 6703 744a 7c0a 6406 644f 6450 6451  d.g.tJ|.d.dOdPdQ
+00002c50: 6702 7c1f 6452 8d0a 0100 7c1e 6442 1900  g.|.dR....|.dB..
+00002c60: 7d23 744b 7c1b 7c04 7c05 7c06 7c07 8305  }#tK|.|.|.|.|...
+00002c70: 7d24 7441 6a4c 7c23 a04d a100 6453 6454  }$tAjL|#.M..dSdT
+00002c80: 8d02 0100 7448 6a49 7c24 6a3c 6442 1900  ....tHjI|$j<dB..
+00002c90: 6444 1b00 7c24 6a3c 6406 1900 6444 1b00  dD..|$j<d...dD..
+00002ca0: 6702 7c0a 6445 7c0b 1b00 6446 6447 6445  g.|.dE|...dFdGdE
+00002cb0: 6448 6449 644a 644b 644c 6444 7c23 644d  dHdIdJdKdLdD|#dM
+00002cc0: 644e 8d0e 0100 7448 6a42 7c24 6406 6406  dN....tHjB|$d.d.
+00002cd0: 6702 6406 6406 6702 7c21 7c22 6406 6703  g.d.d.g.|!|"d.g.
+00002ce0: 744a 7c0a 644f 6450 6451 6702 7c23 6455  tJ|.dOdPdQg.|#dU
+00002cf0: 8d09 0100 7c1e 6444 1900 7d25 7c02 7c1b  ....|.dD..}%|.|.
+00002d00: 1800 7d26 744b 7c26 7c04 7c05 7c06 7c07  ..}&tK|&|.|.|.|.
+00002d10: 8305 7d27 7441 6a4c 7c25 a04d a100 6453  ..}'tAjL|%.M..dS
+00002d20: 6454 8d02 0100 7448 6a49 7c27 6a3c 6442  dT....tHjI|'j<dB
+00002d30: 1900 6444 1b00 7c27 6a3c 6406 1900 6444  ..dD..|'j<d...dD
+00002d40: 1b00 6702 7c0a 6445 7c0b 1b00 6446 6447  ..g.|.dE|...dFdG
+00002d50: 6445 6448 6449 644a 644b 644c 6444 7c25  dEdHdIdJdKdLdD|%
+00002d60: 644d 644e 8d0e 0100 7448 6a42 7c27 6406  dMdN....tHjB|'d.
+00002d70: 6406 6702 6406 6406 6702 7c21 7c22 6406  d.g.d.d.g.|!|"d.
+00002d80: 6703 744a 7c0a 6406 644f 6450 6451 6702  g.tJ|.d.dOdPdQg.
+00002d90: 7c25 6452 8d0a 7d28 7441 6a4e 7c28 6456  |%dR..}(tAjN|(dV
+00002da0: 6457 7c1e 6a4f 6406 1900 6458 8d04 7d29  dW|.jOd...dX..})
+00002db0: 7c29 6a50 a051 a100 0100 7441 6a52 6459  |)jP.Q....tAjRdY
+00002dc0: 7c01 1700 645a a016 7c0c a101 1700 645b  |...dZ..|.....d[
+00002dd0: 645c 8d02 0100 7c0d 645d 6b03 9007 7224  d\....|.d]k...r$
+00002de0: 7441 a053 a100 0100 7454 7c00 8301 7d1c  tA.S....tT|...}.
+00002df0: 7441 6a52 6459 7c01 1700 645e a016 7c0c  tAjRdY|...d^..|.
+00002e00: a101 1700 645b 645c 8d02 0100 7c0d 645d  ....d[d\....|.d]
+00002e10: 6b03 9007 725a 7441 a053 a100 0100 6400  k...rZtA.S....d.
+00002e20: 5300 295f 4e7a 0f2f 7072 6f70 6572 7469  S.)_Nz./properti
+00002e30: 6573 2e64 6174 7a3e 0a2a 4974 2077 6173  es.datz>.*It was
+00002e40: 2063 7265 6174 6520 7468 6520 7072 6f70   create the prop
+00002e50: 6572 7469 6573 2e64 6174 2074 6f20 7072  erties.dat to pr
+00002e60: 696e 7420 7468 6520 6f75 7420 7061 7261  int the out para
+00002e70: 6d65 7465 7273 2902 da05 6e61 6d65 73da  meters)...names.
+00002e80: 0564 7479 7065 72c2 0000 00da 0155 7201  .dtyper......Ur.
+00002e90: 0000 007a 100a 526f 7720 7761 7320 7570  ...z..Row was up
+00002ea0: 6461 7465 647a 170a 526f 7720 7761 7320  datedz..Row was 
+00002eb0: 6372 6561 7465 6420 666f 7220 7b7d 7262  created for {}rb
+00002ec0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002ed0: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
+00002ee0: 0067 007c 005d 0c7d 0174 007c 0183 0191  .g.|.].}.t.|....
+00002ef0: 0271 0453 0072 2f00 0000 2901 72e3 0000  .q.S.r/...).r...
+00002f00: 0029 02da 022e 30da 0173 722f 0000 0072  .)....0..sr/...r
+00002f10: 2f00 0000 7230 0000 00da 0a3c 6c69 7374  /...r0.....<list
+00002f20: 636f 6d70 3eb6 0100 0073 0400 0000 0600  comp>....s......
+00002f30: 0200 7a1d 706c 6f74 5f73 7461 742e 3c6c  ..z.plot_stat.<l
+00002f40: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00002f50: 3e7a 2643 6861 6e67 6520 7468 6520 7374  >z&Change the st
+00002f60: 7269 6e67 2066 6f72 6d61 7420 6f66 2047  ring format of G
+00002f70: 414c 2063 6f6c 756d 6e7a 1b0a 736b 795f  AL columnz..sky_
+00002f80: 6d65 616e 5f73 7461 746d 6f72 7068 203d  mean_statmorph =
+00002f90: 7b3a 2e33 667d 7a1b 736b 795f 7369 676d  {:.3f}z.sky_sigm
+00002fa0: 615f 7374 6174 6d6f 7270 6820 3d7b 3a2e  a_statmorph ={:.
+00002fb0: 3366 7d7a 0666 6c61 6720 3d7a 0d66 6c61  3f}z.flag =z.fla
+00002fc0: 675f 7365 7273 6963 203d 72c7 0000 00da  g_sersic =r.....
+00002fd0: 0372 3230 da03 7238 30da 0447 696e 69da  .r20..r80..Gini.
+00002fe0: 034d 3230 7a08 4628 475f 4d32 3029 7a08  .M20z.F(G_M20)z.
+00002ff0: 5328 475f 4d32 3029 da03 535f 4e72 b200  S(G_M20)..S_Nr..
+00003000: 0000 72b0 0000 00da 0153 da03 7235 30da  ..r......S..r50.
+00003010: 0666 6c75 785f 63da 0666 6c75 785f 65da  .flux_c..flux_e.
+00003020: 0872 7065 7472 6f5f 63da 0872 7065 7472  .rpetro_c..rpetr
+00003030: 6f5f 65da 0772 6861 6c66 5f63 da07 7268  o_e..rhalf_c..rh
+00003040: 616c 665f 657a 190a 2050 6574 726f 7369  alf_ez.. Petrosi
+00003050: 616e 2052 6164 6975 7320 7b3a 2e31 667d  an Radius {:.1f}
+00003060: 72bb 0000 0072 3400 0000 72b3 0000 00da  r....r4...r.....
+00003070: 0241 6fda 0241 73da 0553 6572 5f41 da05  .Ao..As..Ser_A..
+00003080: 5365 725f 52da 0553 6572 5f6e da06 5365  Ser_R..Ser_n..Se
+00003090: 725f 7863 da06 5365 725f 7963 da09 5365  r_xc..Ser_yc..Se
+000030a0: 725f 656c 6c69 70da 0953 6572 5f74 6865  r_ellip..Ser_the
+000030b0: 7461 da0a 666c 6167 5f6d 6f72 7068 da0b  ta..flag_morph..
+000030c0: 666c 6167 5f73 6572 7369 63da 0570 7366  flag_sersic..psf
+000030d0: 5f52 da05 7369 7a65 7054 7292 0000 0029  _R..sizepTr....)
+000030e0: 07da 0961 6d70 6c69 7475 6465 da05 725f  ...amplitude..r_
+000030f0: 6566 66da 016e da03 785f 30da 0379 5f30  eff..n..x_0..y_0
+00003100: da05 656c 6c69 70da 0574 6865 7461 2902  ..ellip..theta).
+00003110: e90f 0000 0072 3d00 0000 7276 0000 0029  .....r=...rv...)
+00003120: 01da 0949 6d61 6765 4772 6964 e96f 0000  ...ImageGrid.o..
+00003130: 0029 0272 6900 0000 728b 0000 0067 6666  .).ri...r....gff
+00003140: 6666 6666 d63f da05 7269 6768 74da 0673  ffff.?..right..s
+00003150: 696e 676c 657a 0235 2567 9a99 9999 9999  inglez.5%g......
+00003160: a93f 2906 da0b 6e72 6f77 735f 6e63 6f6c  .?)...nrows_ncol
+00003170: 73da 0861 7865 735f 7061 64da 0d63 6261  s..axes_pad..cba
+00003180: 725f 6c6f 6361 7469 6f6e da09 6362 6172  r_location..cbar
+00003190: 5f6d 6f64 65da 0963 6261 725f 7369 7a65  _mode..cbar_size
+000031a0: da08 6362 6172 5f70 6164 7269 0000 00e9  ..cbar_padri....
+000031b0: 5a00 0000 7239 0000 0072 3d00 0000 7a05  Z...r9...r=...z.
+000031c0: 3520 6b70 63da 0131 7232 0000 0072 4900  5 kpc..1r2...rI.
+000031d0: 0000 67cd cccc cccc ccf4 3f7a 026b 2dda  ..g.......?z.k-.
+000031e0: 016b 7297 0000 0029 0ada 0470 6172 72da  .kr....)...parr.
+000031f0: 066c 6172 726f 77da 026e 78da 026e 79da  .larrow..nx..ny.
+00003200: 0670 6f73 7478 74da 0463 6261 72da 0463  .postxt..cbar..c
+00003210: 7465 78da 056c 696e 6577 da02 4158 da07  tex..linew..AX..
+00003220: 6261 7274 6578 73da 046e 6f6e 65fa 1724  bartexs..none..$
+00003230: 5c44 656c 7461 5c64 656c 7461 2420 2861  \Delta\delta$ (a
+00003240: 7263 7365 6329 fa18 245c 4465 6c74 6120  rcsec)..$\Delta 
+00003250: 5c61 6c70 6861 2420 2861 7263 7365 6329  \alpha$ (arcsec)
+00003260: 2909 da04 6365 6e74 da05 6465 6c74 61da  )...cent..delta.
+00003270: 046c 696d 7472 a800 0000 da05 7363 616c  .limtr......scal
+00003280: 65da 0763 6261 726f 7074 da06 6f75 7469  e..cbaropt..outi
+00003290: 6d61 da08 6e61 6d65 6178 6973 7277 0100  ma..nameaxisrw..
+000032a0: 0046 2901 da07 7669 7369 626c 6529 0872  .F)...visible).r
+000032b0: 7c01 0000 727d 0100 0072 7e01 0000 72a8  |...r}...r~...r.
+000032c0: 0000 0072 7f01 0000 7281 0100 0072 8201  ...r....r....r..
+000032d0: 0000 7277 0100 007a 0425 2e31 667a 1224  ..rw...z.%.1fz.$
+000032e0: 6d61 675c 2c61 7263 7365 635e 7b2d 327d  mag\,arcsec^{-2}
+000032f0: 2429 0372 6400 0000 da05 6c61 6265 6cda  $).rd.....label.
+00003300: 0363 6178 727b 0000 007a 105f 7b7d 6b70  .caxr{...z._{}kp
+00003310: 635f 6d6f 6465 6c2e 706e 6772 7c00 0000  c_model.pngr|...
+00003320: 727d 0000 0072 4000 0000 7a0f 5f7b 7d6b  r}...r@...z._{}k
+00003330: 7063 5f73 7461 742e 706e 6729 5572 d400  pc_stat.png)Ur..
+00003340: 0000 72d5 0000 0072 d600 0000 7204 0000  ..r....r....r...
+00003350: 0072 d900 0000 72de 0000 0072 df00 0000  .r....r....r....
+00003360: 72e0 0000 0072 cb00 0000 7219 0000 0072  r....r....r....r
+00003370: d200 0000 72da 0000 0072 2500 0000 da07  ....r....r%.....
+00003380: 666c 6f61 7436 3472 0500 0000 da08 636f  float64r......co
+00003390: 6c6e 616d 6573 da07 6164 645f 726f 77da  lnames..add_row.
+000033a0: 0661 7374 7970 6572 e300 0000 da03 616e  .astyper......an
+000033b0: 7972 dd00 0000 72c8 0000 0072 6400 0000  yr....r....rd...
+000033c0: da05 6172 7261 79da 036d 6178 da0e 7265  ..array..max..re
+000033d0: 706c 6163 655f 636f 6c75 6d6e da08 736b  place_column..sk
+000033e0: 795f 6d65 616e da09 736b 795f 7369 676d  y_mean..sky_sigm
+000033f0: 61da 0466 6c61 6772 5701 0000 7240 0100  a..flagrW...r@..
+00003400: 0072 4101 0000 da04 6769 6e69 da03 6d32  .rA.....gini..m2
+00003410: 30da 0e67 696e 695f 6d32 305f 6275 6c67  0..gini_m20_bulg
+00003420: 65da 0f67 696e 695f 6d32 305f 6d65 7267  e..gini_m20_merg
+00003430: 6572 da0c 736e 5f70 6572 5f70 6978 656c  er..sn_per_pixel
+00003440: da0d 636f 6e63 656e 7472 6174 696f 6eda  ..concentration.
+00003450: 0961 7379 6d6d 6574 7279 da0a 736d 6f6f  .asymmetry..smoo
+00003460: 7468 6e65 7373 7246 0100 00da 0966 6c75  thnessrF.....flu
+00003470: 785f 6369 7263 da0a 666c 7578 5f65 6c6c  x_circ..flux_ell
+00003480: 6970 da0b 7270 6574 726f 5f63 6972 63da  ip..rpetro_circ.
+00003490: 0c72 7065 7472 6f5f 656c 6c69 70da 0a72  .rpetro_ellip..r
+000034a0: 6861 6c66 5f63 6972 63da 0b72 6861 6c66  half_circ..rhalf
+000034b0: 5f65 6c6c 6970 da09 6d75 6c74 696d 6f64  _ellip..multimod
+000034c0: 65da 0969 6e74 656e 7369 7479 da09 6465  e..intensity..de
+000034d0: 7669 6174 696f 6eda 0f6f 7574 6572 5f61  viation..outer_a
+000034e0: 7379 6d6d 6574 7279 da0f 7368 6170 655f  symmetry..shape_
+000034f0: 6173 796d 6d65 7472 79da 1073 6572 7369  asymmetry..sersi
+00003500: 635f 616d 706c 6974 7564 65da 0c73 6572  c_amplitude..ser
+00003510: 7369 635f 7268 616c 66da 0873 6572 7369  sic_rhalf..sersi
+00003520: 635f 6eda 0973 6572 7369 635f 7863 da09  c_n..sersic_xc..
+00003530: 7365 7273 6963 5f79 63da 0c73 6572 7369  sersic_yc..sersi
+00003540: 635f 656c 6c69 70da 0c73 6572 7369 635f  c_ellip..sersic_
+00003550: 7468 6574 6172 dc00 0000 da05 7368 6170  thetar......shap
+00003560: 6572 ef00 0000 72f6 0000 00da 1143 6f6e  er....r......Con
+00003570: 766f 6c76 6564 5365 7273 6963 3244 da07  volvedSersic2D..
+00003580: 7365 745f 7073 6672 e600 0000 72e7 0000  set_psfr....r...
+00003590: 00da 176d 706c 5f74 6f6f 6c6b 6974 732e  ...mpl_toolkits.
+000035a0: 6178 6573 5f67 7269 6431 7262 0100 0072  axes_grid1rb...r
+000035b0: 2600 0000 72d3 0000 00da 0a70 6572 6365  &...r......perce
+000035c0: 6e74 696c 65da 0570 6675 6e63 da03 6261  ntile..pfunc..ba
+000035d0: 72da 0863 6f6c 6f72 6d61 7072 3100 0000  r..colormapr1...
+000035e0: da04 7365 7470 da0f 6765 745f 7974 6963  ..setp..get_ytic
+000035f0: 6b6c 6162 656c 73da 0863 6f6c 6f72 6261  klabels..colorba
+00003600: 72da 0963 6261 725f 6178 6573 da02 6178  r..cbar_axes..ax
+00003610: da0c 696e 7665 7274 5f79 6178 6973 72e9  ..invert_yaxisr.
+00003620: 0000 0072 eb00 0000 7202 0000 0029 2a72  ...r....r....)*r
+00003630: 3501 0000 7241 0000 0072 1b01 0000 7223  5...rA...r....r#
+00003640: 0100 0072 1801 0000 722b 0000 0072 2c00  ...r....r+...r,.
+00003650: 0000 722d 0000 0072 2901 0000 7216 0100  ..r-...r)...r...
+00003660: 00da 0673 635f 696d 6172 0a01 0000 7201  ...sc_imar....r.
+00003670: 0100 0072 c100 0000 72c0 0000 0072 e500  ...r....r....r..
+00003680: 0000 7213 0100 00da 0564 6174 6174 da06  ..r......datat..
+00003690: 756e 6974 7374 7236 0100 00da 066c 656e  unitstr6.....len
+000036a0: 5f61 72da 056e 6577 5f63 7272 0100 0072  _ar..new_crr...r
+000036b0: 7101 0000 7227 0100 0072 2801 0000 da0c  q...r'...r(.....
+000036c0: 6669 7474 6564 5f6d 6f64 656c da0c 696d  fitted_model..im
+000036d0: 6167 655f 6d6f 6465 6c67 721d 0100 0072  age_modelgr....r
+000036e0: 6201 0000 da04 6772 6964 72b7 0100 00da  b.....gridr.....
+000036f0: 0669 6d61 675f 63da 0869 6d61 675f 6d69  .imag_c..imag_mi
+00003700: 6eda 0869 6d61 675f 6d61 78da 0361 7831  n..imag_max..ax1
+00003710: da0d 696d 6167 655f 6d6f 6465 6c6d 67da  ..image_modelmg.
+00003720: 0361 7832 da09 7265 7369 6475 616c 67da  .ax2..residualg.
+00003730: 0a72 6573 6964 7561 6c67 6dda 0269 6dda  .residualgm..im.
+00003740: 0263 6272 2f00 0000 722f 0000 0072 3000  .cbr/...r/...r0.
+00003750: 0000 72fc 0000 0093 0100 0073 bc01 0000  ..r........s....
+00003760: 0004 0c01 0e02 1401 0e01 0e02 1401 0400  ................
+00003770: 0400 0400 0400 0401 0400 0400 0400 0400  ................
+00003780: 0401 0400 0400 0400 0400 0401 0400 0400  ................
+00003790: 0400 0400 0401 0400 0400 0400 0400 0401  ................
+000037a0: 0400 0400 0400 0400 0401 0400 0400 0400  ................
+000037b0: 0400 0401 0400 0400 0400 0400 0401 0400  ................
+000037c0: 0400 0400 04f7 040a 0e01 0801 1e01 0c02  ................
+000037d0: 1201 0e01 1801 1c03 1401 0801 0401 1801  ................
+000037e0: 1401 0802 1a01 0c01 0c02 1001 1001 0c01  ................
+000037f0: 0c01 0802 0e01 0e01 0e01 0e01 0e01 0e01  ................
+00003800: 0e01 0e01 0e01 0e02 0e02 0e01 0e01 0e01  ................
+00003810: 0e01 0e01 0e02 1602 0e01 0e01 0e01 0e01  ................
+00003820: 0e02 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
+00003830: 0e01 0e01 0c01 0c02 1002 0a01 1a01 0401  ................
+00003840: 0401 0401 0401 0401 0401 0401 04f9 0608  ................
+00003850: 0a01 0a02 0c02 0c01 0601 0201 0201 0201  ................
+00003860: 0201 0201 02fa 060a 0802 0a01 1002 0c01  ................
+00003870: 0c03 2801 0200 0200 0200 0201 0200 0200  ..(.............
+00003880: 0200 0200 0200 02fe 0604 1a01 0200 0200  ................
+00003890: 0200 0201 0601 02fd 0605 0801 1002 1202  ................
+000038a0: 2001 0600 0200 0200 0200 0200 0201 0200   ...............
+000038b0: 0200 0200 0200 0200 02fe 0604 1201 0800  ................
+000038c0: 0200 0201 0201 0601 02fc 0608 0801 0802  ................
+000038d0: 1002 1202 2601 0200 0200 0200 0200 0201  ....&...........
+000038e0: 0200 0200 0200 0200 0200 02fe 0604 1201  ................
+000038f0: 0801 0200 0200 0200 0201 0601 02fc 0606  ................
+00003900: 0a01 08ff 0602 0a02 1401 02ff 0602 0a01  ................
+00003910: 0802 0801 1401 02ff 0602 0a01 72fc 0000  ............r...
+00003920: 00da 0663 6972 636c 65e9 f401 0000 e90a  ...circle.......
+00003930: 0000 0072 9700 0000 7269 0000 00da 026e  ...r....ri.....n
+00003940: 6f63 1900 0000 0000 0000 0000 0000 4700  oc............G.
+00003950: 0000 1300 0000 4300 0000 733a 0e00 0074  ......C...s:...t
+00003960: 00a0 017c 0164 0119 007c 006b 02a1 0164  ...|.d...|.k...d
+00003970: 0219 0064 0219 007d 197c 0164 0319 007c  ...d...}.|.d...|
+00003980: 1919 0074 021b 007d 1a74 00a0 0374 00a0  ...t...}.t...t..
+00003990: 0464 04a1 01a1 017c 1a14 0064 0514 007d  .d.....|...d...}
+000039a0: 1b74 0574 066a 0764 0617 0083 0101 0074  .t.t.j.d.......t
+000039b0: 0564 0783 0101 0074 086a 09a0 0a74 086a  .d.....t.j...t.j
+000039c0: 09a0 0b74 0ca1 01a1 017d 1c74 0d6a 0e7c  ...t.....}.t.j.|
+000039d0: 1c64 0817 0064 0964 0a8d 027d 1d74 057c  .d...d.d...}.t.|
+000039e0: 1d64 0b19 0074 00a0 017c 1d64 0119 007c  .d...t...|.d...|
+000039f0: 006b 02a1 0164 0219 0019 0083 0101 0074  .k...d.........t
+00003a00: 057c 1d64 0c19 0074 00a0 017c 1d64 0119  .|.d...t...|.d..
+00003a10: 007c 006b 02a1 0164 0219 0019 0083 0101  .|.k...d........
+00003a20: 0074 0574 066a 0f64 0d17 0083 0101 0074  .t.t.j.d.......t
+00003a30: 0574 066a 0f64 0e17 0083 0101 0074 0574  .t.j.d.......t.t
+00003a40: 066a 0f64 0fa0 107c 1aa1 0117 0083 0101  .j.d...|........
+00003a50: 0074 0574 066a 0f64 10a0 107c 1ba1 0117  .t.t.j.d...|....
+00003a60: 0083 0101 007c 037c 1b1b 0064 111b 0064  .....|.|...d...d
+00003a70: 1214 007d 1e7c 1e64 1314 0064 1114 0064  ...}.|.d...d...d
+00003a80: 141b 007d 1f74 0574 066a 0f64 15a0 107c  ...}.t.t.j.d...|
+00003a90: 1ea1 0117 0083 0101 0074 00a0 117c 05a1  .........t...|..
+00003aa0: 0174 006a 1214 007c 1b64 1213 001b 0064  .t.j...|.d.....d
+00003ab0: 161b 007d 2074 0574 066a 0f64 17a0 107c  ...} t.t.j.d...|
+00003ac0: 057c 20a1 0217 0083 0101 007c 02a0 137c  .| ........|...|
+00003ad0: 0164 1819 007c 1919 007c 0164 1919 007c  .d...|...|.d...|
+00003ae0: 1919 00a1 027d 2174 006a 14a0 157c 2164  .....}!t.j...|!d
+00003af0: 1a19 0064 1ba1 0290 0172 d874 0574 066a  ...d.....r.t.t.j
+00003b00: 0764 1c17 0083 0101 0074 0574 066a 0764  .d.......t.t.j.d
+00003b10: 1d17 0083 0101 0074 0574 066a 0764 1e17  .......t.t.j.d..
+00003b20: 0083 0101 0074 0574 066a 0764 1f17 0083  .....t.t.j.d....
+00003b30: 0101 0064 0053 0074 00a0 167c 1ea1 0190  ...d.S.t...|....
+00003b40: 0272 1274 0574 066a 0764 1c17 0083 0101  .r.t.t.j.d......
+00003b50: 0074 0574 066a 0764 2017 0083 0101 0074  .t.t.j.d ......t
+00003b60: 0574 066a 0764 1f17 0083 0101 0064 0053  .t.j.d.......d.S
+00003b70: 007c 1164 216b 0290 0272 b464 227c 0164  .|.d!k...r.d"|.d
+00003b80: 0119 007c 1919 0017 0064 2317 007d 2264  ...|.....d#..}"d
+00003b90: 227c 0164 0119 007c 1919 0064 0064 2485  "|.d...|...d.d$.
+00003ba0: 0219 0017 0064 2317 007d 2374 086a 09a0  .....d#..}#t.j..
+00003bb0: 177c 22a1 0190 0273 6874 086a 09a0 177c  .|"....sht.j...|
+00003bc0: 23a1 0190 0272 8674 0574 066a 0764 1c17  #....r.t.t.j.d..
+00003bd0: 0083 0101 0074 0574 066a 0764 2517 0083  .....t.t.j.d%...
+00003be0: 0101 006e 2e74 0574 066a 0764 1c17 0083  ...n.t.t.j.d....
+00003bf0: 0101 0074 0574 066a 0764 2617 0083 0101  ...t.t.j.d&.....
+00003c00: 0074 0574 066a 0764 1f17 0083 0101 0064  .t.t.j.d.......d
+00003c10: 0053 0074 086a 09a0 1764 27a1 0190 0273  .S.t.j...d'....s
+00003c20: da74 08a0 1864 28a1 0101 0074 0574 066a  .t...d(....t.t.j
+00003c30: 0764 2917 0083 0101 0074 086a 09a0 1764  .d)......t.j...d
+00003c40: 2aa1 0190 0373 0074 08a0 1864 2ba1 0101  *....s.t...d+...
+00003c50: 0074 0574 066a 0764 2c17 0083 0101 0074  .t.t.j.d,......t
+00003c60: 0564 2d83 0101 007c 117d 247c 037c 246b  .d-....|.}$|.|$k
+00003c70: 0090 0372 1c64 217d 246e 047c 037d 2474  ...r.d!}$n.|.}$t
+00003c80: 0574 066a 1964 2d17 0083 0101 007c 1764  .t.j.d-......|.d
+00003c90: 2e6b 0290 0372 4c74 1a7c 007c 017c 247c  .k...rLt.|.|.|$|
+00003ca0: 067c 087c 0764 2f8d 067d 2574 0574 066a  .|.|.d/..}%t.t.j
+00003cb0: 1964 3017 0083 0101 0074 0564 3183 0101  .d0......t.d1...
+00003cc0: 0064 32a0 107c 007c 03a1 027d 2264 33a0  .d2..|.|...}"d3.
+00003cd0: 107c 007c 107c 03a1 037d 2374 086a 09a0  .|.|.|...}#t.j..
+00003ce0: 177c 22a1 0190 0373 a274 086a 09a0 177c  .|"....s.t.j...|
+00003cf0: 23a1 0190 0372 b27c 1064 346b 0290 0372  #....r.|.d4k...r
+00003d00: b274 0564 357c 229b 0064 369d 0383 0101  .t.d5|"..d6.....
+00003d10: 0074 086a 09a0 177c 22a1 0190 0473 1874  .t.j...|"....s.t
+00003d20: 086a 09a0 177c 23a1 0190 0473 187c 1064  .j...|#....s.|.d
+00003d30: 346b 0290 0472 1874 0564 377c 229b 0064  4k...r.t.d7|"..d
+00003d40: 389d 0383 0101 007c 026a 1b7c 0164 1819  8......|.j.|.d..
+00003d50: 007c 1919 007c 0164 1919 007c 1919 0074  .|...|.d...|...t
+00003d60: 1c7c 1e83 017c 107c 2264 0264 3985 0219  .|...|.|"d.d9...
+00003d70: 0064 3a8d 0501 0074 086a 09a0 177c 23a1  .d:....t.j...|#.
+00003d80: 0190 0472 3674 0564 357c 239b 0064 369d  ...r6t.d5|#..d6.
+00003d90: 0383 0101 0074 086a 09a0 177c 23a1 0190  .....t.j...|#...
+00003da0: 0473 8e7c 1064 346b 0390 0472 8e74 0564  .s.|.d4k...r.t.d
+00003db0: 377c 239b 0064 389d 0383 0101 007c 026a  7|#..d8......|.j
+00003dc0: 1b7c 0164 1819 007c 1919 007c 0164 1919  .|.d...|...|.d..
+00003dd0: 007c 1919 0074 1c7c 1e83 017c 107c 2364  .|...t.|...|.|#d
+00003de0: 0264 3985 0219 0064 3a8d 0501 0064 3ba0  .d9....d:....d;.
+00003df0: 107c 007c 03a1 027d 2274 086a 09a0 177c  .|.|...}"t.j...|
+00003e00: 22a1 0190 0673 9074 0564 3c7c 0164 1819  "....s.t.d<|.d..
+00003e10: 007c 1919 007c 0164 1919 007c 1919 0074  .|...|.d...|...t
+00003e20: 1c7c 1e83 0183 0401 0074 1c7c 1e83 0164  .|.......t.|...d
+00003e30: 3d6b 0090 0572 2274 0564 3e83 0101 0074  =k...r"t.d>....t
+00003e40: 0564 3f83 0101 0074 0564 4083 0101 007c  .d?....t.d@....|
+00003e50: 02a0 1d7c 0164 1819 007c 1919 007c 0164  ...|.d...|...|.d
+00003e60: 1919 007c 1919 0074 1c7c 1e83 01a1 037d  ...|...t.|.....}
+00003e70: 267c 26a0 1e7c 2264 41a1 0201 0090 0671  &|&..|"dA......q
+00003e80: a074 1c7c 1e83 0164 426b 0090 0572 8674  .t.|...dBk...r.t
+00003e90: 0564 4383 0101 0074 0564 4483 0101 0074  .dC....t.dD....t
+00003ea0: 0564 4583 0101 007c 026a 1f7c 0164 1819  .dE....|.j.|.d..
+00003eb0: 007c 1919 007c 0164 1919 007c 1919 0074  .|...|.d...|...t
+00003ec0: 1c7c 1e83 0164 4664 3464 4764 4864 4964  .|...dFd4dGdHdId
+00003ed0: 4a8d 087d 267c 26a0 1e7c 2264 41a1 0201  J..}&|&..|"dA...
+00003ee0: 0090 0671 a074 0564 4383 0101 0074 0564  ...q.t.dC....t.d
+00003ef0: 4b83 0101 0074 0564 4583 0101 0064 4ca0  K....t.dE....dL.
+00003f00: 107c 007c 03a1 027d 2374 086a 09a0 177c  .|.|...}#t.j...|
+00003f10: 2364 4d17 00a1 0190 0573 e87c 026a 1b7c  #dM......s.|.j.|
+00003f20: 0164 1819 007c 1919 007c 0164 1919 007c  .d...|...|.d...|
+00003f30: 1919 0074 1c7c 1e83 0164 477c 2364 4e17  ...t.|...dG|#dN.
+00003f40: 0064 3a8d 0501 0074 086a 09a0 177c 2364  .d:....t.j...|#d
+00003f50: 4f17 00a1 0190 0673 267c 026a 1b7c 0164  O......s&|.j.|.d
+00003f60: 1819 007c 1919 007c 0164 1919 007c 1919  ...|...|.d...|..
+00003f70: 0074 1c7c 1e83 0164 467c 2364 5017 0064  .t.|...dF|#dP..d
+00003f80: 3a8d 0501 0074 20a0 2164 51a0 107c 007c  :....t .!dQ..|.|
+00003f90: 03a1 02a1 017d 277c 2764 5219 006a 227d  .....}'|'dR..j"}
+00003fa0: 2874 20a0 2164 51a0 107c 007c 03a1 02a1  (t .!dQ..|.|....
+00003fb0: 017d 277c 2764 5219 006a 227d 2974 20a0  .}'|'dR..j"})t .
+00003fc0: 2164 32a0 107c 007c 03a1 02a1 017d 277c  !d2..|.|.....}'|
+00003fd0: 2764 5219 006a 227d 2a74 237c 297c 2a7c  'dR..j"}*t#|)|*|
+00003fe0: 2864 1364 497c 2264 538d 0601 006e 1074  (d.dI|"dS....n.t
+00003ff0: 0564 357c 229b 0064 369d 0383 0101 007c  .d5|"..d6......|
+00004000: 1764 2e6b 0290 0672 cc74 247c 007c 017c  .d.k...r.t$|.|.|
+00004010: 027c 247c 2564 547c 097c 0a7c 0b64 2e64  .|$|%dT|.|.|.d.d
+00004020: 2e7c 0f7c 1064 558d 0d01 0064 3ba0 107c  .|.|.dU....d;..|
+00004030: 007c 03a1 027d 2b74 25a0 267c 2ba1 017d  .|...}+t%.&|+..}
+00004040: 2c7c 1064 346b 0290 0772 247a 1674 20a0  ,|.d4k...r$z.t .
+00004050: 2164 32a0 107c 007c 03a1 02a1 017d 2757  !d2..|.|.....}'W
+00004060: 006e 2001 0001 0001 0074 20a0 2164 33a0  .n ......t .!d3.
+00004070: 107c 007c 107c 03a1 03a1 017d 2759 006e  .|.|.|.....}'Y.n
+00004080: 0258 007c 1064 346b 0390 0772 4274 20a0  .X.|.d4k...rBt .
+00004090: 2164 33a0 107c 007c 107c 03a1 03a1 017d  !d3..|.|.|.....}
+000040a0: 277c 2764 5219 006a 227d 2a74 0564 5683  '|'dR..j"}*t.dV.
+000040b0: 0101 0074 0574 066a 0f64 5717 0083 0101  ...t.t.j.dW.....
+000040c0: 0074 0564 5883 0101 0074 0564 5683 0101  .t.dX....t.dV...
+000040d0: 0074 277c 2a7c 127c 137c 1464 598d 047d  .t'|*|.|.|.dY..}
+000040e0: 2d74 256a 2864 5a64 5b8d 017d 2e74 256a  -t%j(dZd[..}.t%j
+000040f0: 297c 2d64 5c64 5d8d 0201 007c 1664 5e6b  )|-d\d]....|.d^k
+00004100: 0290 0772 b074 25a0 2aa1 0001 006e 0874  ...r.t%.*....n.t
+00004110: 25a0 2ba1 0001 0074 2c7c 2a64 5f7c 2d64  %.+....t,|*d_|-d
+00004120: 608d 035c 037d 2f7d 307d 3174 0574 066a  `..\.}/}0}1t.t.j
+00004130: 0f64 6117 0083 0101 0074 0564 5883 0101  .da......t.dX...
+00004140: 0074 0564 62a0 107c 2fa1 0183 0101 0074  .t.db..|/......t
+00004150: 0564 63a0 107c 30a1 0183 0101 0074 0564  .dc..|0......t.d
+00004160: 64a0 107c 31a1 0183 0101 0074 0564 65a0  d..|1......t.de.
+00004170: 107c 0c64 0219 007c 0c64 5219 00a1 0283  .|.d...|.dR.....
+00004180: 0101 0074 0564 5883 0101 007c 0c64 0219  ...t.dX....|.d..
+00004190: 007c 2a6a 2d64 5219 0064 1314 006b 0590  .|*j-dR..d...k..
+000041a0: 0872 7474 0574 066a 0764 6617 0083 0101  .rtt.t.j.df.....
+000041b0: 0074 0574 066a 0764 67a0 107c 2a6a 2d64  .t.t.j.dg..|*j-d
+000041c0: 5219 0064 1314 00a1 0117 0083 0101 0064  R..d...........d
+000041d0: 0053 0074 2e83 007d 3274 2f7c 2a7c 0c64  .S.t...}2t/|*|.d
+000041e0: 687c 327c 2d7c 3064 698d 067d 337c 2a7c  h|2|-|0di..}3|*|
+000041f0: 336a 3038 007d 2a74 0564 6a83 0101 0074  3j08.}*t.dj....t
+00004200: 256a 2864 5a64 5b8d 017d 2e74 256a 297c  %j(dZd[..}.t%j)|
+00004210: 336a 3064 5c64 5d8d 0201 007c 1664 5e6b  3j0d\d]....|.d^k
+00004220: 0290 0872 d074 25a0 2aa1 0001 006e 0874  ...r.t%.*....n.t
+00004230: 25a0 2ba1 0001 007c 0e74 3114 007d 3474  %.+....|.t1..}4t
+00004240: 327c 3464 4864 4864 6b8d 037d 357c 35a0  2|4dHdHdk..}5|5.
+00004250: 33a1 0001 0074 1c7c 2083 017d 3674 346a  3....t.| ..}6t4j
+00004260: 357c 2a7c 0464 6c8d 027d 3774 34a0 367c  5|*|.dl..}7t4.6|
+00004270: 2a7c 377c 36a1 037d 387c 0d64 6d6b 0290  *|7|6..}8|.dmk..
+00004280: 0972 8474 0564 6e83 0101 0074 0564 6f83  .r.t.dn....t.do.
+00004290: 0101 0074 0564 7083 0101 0074 256a 2864  ...t.dp....t%j(d
+000042a0: 5a64 5b8d 017d 2e74 256a 297c 3864 5c64  Zd[..}.t%j)|8d\d
+000042b0: 5d8d 0201 007c 1664 5e6b 0290 0972 6a74  ]....|.d^k...rjt
+000042c0: 25a0 2aa1 0001 006e 0874 25a0 2ba1 0001  %.*....n.t%.+...
+000042d0: 0074 377c 2a7c 387c 3664 7164 7264 738d  .t7|*|8|6dqdrds.
+000042e0: 057d 3874 00a0 387c 386a 39a1 017d 3974  .}8t..8|8j9..}9t
+000042f0: 0564 7483 0101 0074 057c 386a 3983 0101  .dt....t.|8j9...
+00004300: 0074 0574 00a0 3a74 3b7c 386a 3983 01a1  .t.t..:t;|8j9...
+00004310: 0183 0101 0064 0264 006c 3c7d 3a64 757c  .....d.d.l<}:du|
+00004320: 3a6a 3d64 763c 0064 777c 3a6a 3d64 783c  :j=dv<.dw|:j=dx<
+00004330: 0064 797c 3a6a 3d64 7a3c 0064 497c 3a6a  .dy|:j=dz<.dI|:j
+00004340: 3d64 7b3c 0064 797c 3a6a 3d64 7c3c 0064  =d{<.dy|:j=d|<.d
+00004350: 497c 3a6a 3d64 7d3c 0064 797c 3a6a 3d64  I|:j=d}<.dy|:j=d
+00004360: 7e3c 0064 797c 3a6a 3d64 7f3c 0074 256a  ~<.dy|:j=d.<.t%j
+00004370: 2864 8064 5b8d 017d 2e74 00a0 3e7c 386a  (d.d[..}.t..>|8j
+00004380: 22a1 01a0 3f74 40a1 017d 3b74 006a 417c  "...?t@..};t.jA|
+00004390: 3b7c 3b64 816b 023c 0074 1c7c 1e83 0164  ;|;d.k.<.t.|...d
+000043a0: 1314 0064 1114 007c 1b14 007d 3c74 256a  ...d...|...}<t%j
+000043b0: 297c 3b64 8264 8364 5c64 848d 047d 3d74  )|;d.d.d\d...}=t
+000043c0: 00a0 3a74 00a0 427c 3ba1 01a1 0144 005d  ..:t..B|;....D.]
+000043d0: 427d 3e74 00a0 017c 3b7c 3e64 5217 006b  B}>t...|;|>dR..k
+000043e0: 02a1 017d 3f74 256a 437c 3f64 5219 0064  ...}?t%jC|?dR..d
+000043f0: 0219 007c 3f64 0219 0064 0219 0074 4474  ...|?d...d...tDt
+00004400: 1c7c 3e83 0183 0164 8564 868d 0401 0090  .|>....d.d......
+00004410: 0a71 7074 25a0 457c 3da1 017d 407c 406a  .qpt%.E|=..}@|@j
+00004420: 46a0 47a1 0001 0074 25a0 47a1 0001 007c  F.G....t%.G....|
+00004430: 1664 5e6b 0290 0a72 e474 25a0 2aa1 0001  .d^k...r.t%.*...
+00004440: 006e 0874 25a0 2ba1 0001 007c 1664 5e6b  .n.t%.+....|.d^k
+00004450: 0290 0d72 267c 0f64 2e6b 0290 0b72 1664  ...r&|.d.k...r.d
+00004460: 227c 0164 0119 007c 1919 0017 0064 2317  "|.d...|.....d#.
+00004470: 007d 226e 0c64 87a0 107c 007c 24a1 027d  .}"n.d...|.|$..}
+00004480: 2274 086a 09a0 177c 22a1 0190 0b73 de74  "t.j...|"....s.t
+00004490: 0564 8883 0101 0074 256a 2864 8964 5b8d  .d.....t%j(d.d[.
+000044a0: 017d 2e74 25a0 4864 8aa1 0101 0074 256a  .}.t%.Hd.....t%j
+000044b0: 297c 3864 5c64 8b74 00a0 4964 2464 5264  )|8d\d.t..Id$dRd
+000044c0: 2464 5267 04a1 017c 3c14 0064 8c8d 0401  $dRg...|<..d....
+000044d0: 0074 25a0 4a64 8da1 0101 0074 25a0 4b64  .t%.Jd.....t%.Kd
+000044e0: 8ea1 0101 0074 25a0 47a1 0001 0074 25a0  .....t%.G....t%.
+000044f0: 4864 8fa1 0101 0074 256a 297c 2c74 00a0  Hd.....t%j)|,t..
+00004500: 4964 2464 5264 2464 5267 04a1 017c 3c14  Id$dRd$dRg...|<.
+00004510: 0064 908d 0201 0074 25a0 4ca1 0001 0074  .d.....t%.L....t
+00004520: 25a0 4a64 8da1 0101 0074 25a0 47a1 0001  %.Jd.....t%.G...
+00004530: 0074 25a0 2aa1 0001 0090 016e 4874 25a0  .t%.*......nHt%.
+00004540: 267c 22a1 017d 4174 256a 2864 9164 5b8d  &|"..}At%j(d.d[.
+00004550: 017d 2e74 25a0 4864 92a1 0101 0074 256a  .}.t%.Hd.....t%j
+00004560: 297c 3864 5c64 8b74 00a0 4964 2464 5264  )|8d\d.t..Id$dRd
+00004570: 2464 5267 04a1 017c 3c14 0064 8c8d 0401  $dRg...|<..d....
+00004580: 0074 25a0 4a64 8da1 0101 0074 25a0 4b64  .t%.Jd.....t%.Kd
+00004590: 8ea1 0101 0074 25a0 47a1 0001 0074 25a0  .....t%.G....t%.
+000045a0: 4864 93a1 0101 0074 256a 297c 2c74 00a0  Hd.....t%j)|,t..
+000045b0: 4964 2464 5264 2464 5267 04a1 017c 3c14  Id$dRd$dRg...|<.
+000045c0: 0064 908d 0201 0074 25a0 4ca1 0001 0074  .d.....t%.L....t
+000045d0: 25a0 4a64 8da1 0101 0074 25a0 47a1 0001  %.Jd.....t%.G...
+000045e0: 0074 25a0 4864 94a1 0101 007c 0f64 2e6b  .t%.Hd.....|.d.k
+000045f0: 0290 0c72 bc64 217c 1b1b 0064 111b 0064  ...r.d!|...d...d
+00004600: 1214 007d 1e74 1c7c 1e83 0164 1314 0064  ...}.t.|...d...d
+00004610: 1114 007c 1b14 007d 3c6e 2864 957d 1e7c  ...|...}<n(d.}.|
+00004620: 2464 1214 007c 1b1b 007c 1e1b 007d 4274  $d...|...|...}Bt
+00004630: 1c7c 1e83 0164 1314 007c 4214 007c 1b14  .|...d...|B..|..
+00004640: 007d 3c74 256a 297c 4174 00a0 4964 2464  .}<t%j)|At..Id$d
+00004650: 5264 2464 5267 04a1 017c 3c14 0064 908d  Rd$dRg...|<..d..
+00004660: 0201 0074 25a0 4ca1 0001 0074 25a0 4a64  ...t%.L....t%.Jd
+00004670: 8da1 0101 0074 25a0 47a1 0001 0074 25a0  .....t%.G....t%.
+00004680: 2aa1 0001 007c 1764 5e6b 0390 0d72 8064  *....|.d^k...r.d
+00004690: 967c 009b 0064 977c 039b 0064 989d 057d  .|...d.|...d...}
+000046a0: 4364 997c 049b 0064 9a7c 059b 0064 9b7c  Cd.|...d.|...d.|
+000046b0: 0c9b 0064 9c7c 0d9b 0064 9d9d 097d 4464  ...d.|...d...}Dd
+000046c0: 9e7c 109b 0064 9f9d 037d 4574 057c 437c  .|...d...}Et.|C|
+000046d0: 4417 007c 4517 0083 0101 007c 2553 0074  D..|E......|%S.t
+000046e0: 1c7c 3b74 1c7c 3b6a 2d64 0219 0064 1314  .|;t.|;j-d...d..
+000046f0: 0083 0174 1c7c 3b6a 2d64 5219 0064 1314  ...t.|;j-dR..d..
+00004700: 0083 0166 0219 0083 0164 5218 007d 4664  ...f.....dR..}Fd
+00004710: 967c 009b 0064 977c 039b 0064 989d 057d  .|...d.|...d...}
+00004720: 4364 997c 049b 0064 9a7c 059b 0064 9b7c  Cd.|...d.|...d.|
+00004730: 0c9b 0064 9c7c 0d9b 0064 9d9d 097d 4464  ...d.|...d...}Dd
+00004740: a07c 469b 0064 a17c 109b 0064 a27c 109b  .|F..d.|...d.|..
+00004750: 0064 9f9d 077d 4574 057c 437c 4417 007c  .d...}Et.|C|D..|
+00004760: 4517 0083 0101 0074 4d7c 007c 017c 027c  E......tM|.|.|.|
+00004770: 037c 047c 057c 4667 017c 1067 017c 0c7c  .|.|.|Fg.|.g.|.|
+00004780: 0d7c 107c 127c 137c 147c 187c 157c 1664  .|.|.|.|.|.|.|.d
+00004790: a38d 1101 0064 0053 0029 a44e 7241 0000  .....d.S.).NrA..
+000047a0: 0072 0100 0000 7242 0000 0072 4300 0000  .r....rB...rC...
+000047b0: 7244 0000 00fa 170a 4172 7020 2620 4d61  rD......Arp & Ma
+000047c0: 6f64 6f72 6520 4361 7461 6c6f 673a fa18  odore Catalog:..
+000047d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047e0: 2d2d 2d2d 2d2d 2d2d fa23 2f54 6162 6c65  --------.#/Table
+000047f0: 5f41 7270 5f4d 6164 6f72 655f 7061 6972  _Arp_Madore_pair
+00004800: 735f 7570 6461 7465 642e 7478 7472 0400  s_updated.txtr..
+00004810: 0000 7263 0000 00a9 02da 0363 6174 da08  ..rc.......cat..
+00004820: 6372 6f73 735f 4944 a902 da04 6465 7363  cross_ID....desc
+00004830: da05 636f 6465 7372 4500 0000 7246 0000  ..codesrE...rF..
+00004840: 00fa 1344 6973 7461 6e63 6520 7b3a 2e31  ...Distance {:.1
+00004850: 667d 204d 7063 7247 0000 0072 4800 0000  f} MpcrG...rH...
+00004860: 7239 0000 0072 4900 0000 724a 0000 0072  r9...rI...rJ...r
+00004870: 4b00 0000 724c 0000 0072 4d00 0000 724e  K...rL...rM...rN
+00004880: 0000 0072 4f00 0000 7250 0000 0072 5100  ...rO...rP...rQ.
+00004890: 0000 7252 0000 0072 5300 0000 7254 0000  ..rR...rS...rT..
+000048a0: 0072 5600 0000 7255 0000 0072 3a00 0000  .rV...rU...r:...
+000048b0: fa0c 696d 6167 6573 5f31 3030 6b2f fa13  ..images_100k/..
+000048c0: 5f31 3030 5f6b 7063 5f72 6164 6975 732e  _100_kpc_radius.
+000048d0: 706e 6772 6200 0000 7a27 0a0a 5468 6973  pngrb...z'..This
+000048e0: 2067 616c 6178 7920 6861 7320 3130 3020   galaxy has 100 
+000048f0: 6b70 6320 696d 6167 6520 6176 6169 626c  kpc image avaibl
+00004900: 657a 2b0a 0a54 6869 7320 6761 6c61 7879  ez+..This galaxy
+00004910: 2068 6173 206e 6f74 2031 3030 206b 7063   has not 100 kpc
+00004920: 2069 6d61 6765 2061 7661 6962 6c65 da0b   image avaible..
+00004930: 6669 7473 5f69 6d61 6765 73fa 116d 6b64  fits_images..mkd
+00004940: 6972 2066 6974 735f 696d 6167 6573 fa23  ir fits_images.#
+00004950: 0a54 6865 2066 6f6c 6465 7220 6669 7473  .The folder fits
+00004960: 5f69 6d61 6765 7320 7761 7320 6372 6561  _images was crea
+00004970: 7465 64da 0669 6d61 6765 73fa 0c6d 6b64  ted..images..mkd
+00004980: 6972 2069 6d61 6765 73fa 1e0a 5468 6520  ir images...The 
+00004990: 666f 6c64 6572 2069 6d61 6765 7320 7761  folder images wa
+000049a0: 7320 6372 6561 7465 6472 c700 0000 72ce  s createdr....r.
+000049b0: 0100 0029 0472 0101 0000 da06 7265 6769  ...).r......regi
+000049c0: 6f6e da07 6c69 6d74 7665 6cda 0673 6572  on..limtvel..ser
+000049d0: 7665 727a 200a 0a4c 6f61 6469 6e67 2f44  verz ..Loading/D
+000049e0: 6f77 6e6c 6f61 6469 6e67 2074 6865 2069  ownloading the i
+000049f0: 6d61 6765 7372 5800 0000 7259 0000 0072  magesrX...rY...r
+00004a00: 5a00 0000 723c 0000 0072 5b00 0000 725c  Z...r<...r[...r\
+00004a10: 0000 0072 5d00 0000 725e 0000 0072 5f00  ...r]...r^...r_.
+00004a20: 0000 7260 0000 00fa 1769 6d61 6765 732f  ..r`.....images/
+00004a30: 6669 675f 7b7d 5f7b 7d6b 7063 2e70 6e67  fig_{}_{}kpc.png
+00004a40: 7a1a 0a44 6f77 6e6c 6f61 6469 6e67 2074  z..Downloading t
+00004a50: 6865 2070 6e67 2066 696c 653a e9e8 0300  he png file:....
+00004a60: 007a 1d0a 2323 2323 2323 2323 2323 2323  .z..############
+00004a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004a80: 7a1d 446f 776e 6c6f 6164 696e 6720 5247  z.Downloading RG
+00004a90: 4220 3132 2062 616e 6420 696d 6167 657a  B 12 band imagez
+00004aa0: 1c23 2323 2323 2323 2323 2323 2323 2323  .###############
+00004ab0: 2323 2323 2323 2323 2323 2323 23da 0350  #############..P
+00004ac0: 4e47 69d0 0700 007a 2e0a 2323 2323 2323  NGi....z..######
+00004ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004af0: 2323 2323 2323 237a 2d44 6f77 6e6f 6164  #######z-Downoad
+00004b00: 696e 6720 5247 4220 3320 6261 6e64 2069  ing RGB 3 band i
+00004b10: 6d61 6765 2028 696d 6167 653e 3130 3030  mage (image>1000
+00004b20: 2070 6978 2129 7a2d 2323 2323 2323 2323   pix!)z-########
+00004b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004b50: 2323 2323 2372 3400 0000 72b6 0000 0072  #####r4...r....r
+00004b60: 8b00 0000 e908 0000 0029 0572 3c00 0000  .........).r<...
+00004b70: 72b6 0000 0072 b100 0000 da07 7374 7265  r....r......stre
+00004b80: 7463 68da 0151 7a2d 446f 776e 6f61 6469  tch..Qz-Downoadi
+00004b90: 6e67 2052 4742 2033 2062 616e 6420 696d  ng RGB 3 band im
+00004ba0: 6167 6520 2869 6d61 6765 3e32 3030 3020  age (image>2000 
+00004bb0: 7069 7821 297a 1466 6974 735f 696d 6167  pix!)z.fits_imag
+00004bc0: 6573 2f7b 7d5f 7b7d 6b70 637a 055f 472e  es/{}_{}kpcz._G.
+00004bd0: 667a da02 5f47 7a05 5f49 2e66 7ada 025f  fz.._Gz._I.fz.._
+00004be0: 497a 1966 6974 735f 696d 6167 6573 2f7b  Iz.fits_images/{
+00004bf0: 7d5f 7b7d 6b70 635f 472e 667a 7269 0000  }_{}kpc_G.fzri..
+00004c00: 0029 0372 e801 0000 72e9 0100 00da 0866  .).r....r......f
+00004c10: 696c 656e 616d 6546 290a 7201 0100 00da  ilenameF).r.....
+00004c20: 0574 6162 6c65 da0a 6164 645f 6f62 6a65  .table..add_obje
+00004c30: 6374 da05 7874 706f 73da 0579 7470 6f73  ct..xtpos..ytpos
+00004c40: da06 6465 6c74 6179 da09 7072 696e 745f  ..deltay..print_
+00004c50: 6172 70da 0b70 7269 6e74 5f73 6361 6c65  arp..print_scale
+00004c60: da09 7573 6573 696d 6261 6472 0801 0000  ..usesimbadr....
+00004c70: 726f 0000 0072 6d00 0000 726e 0000 0072  ro...rm...rn...r
+00004c80: 7000 0000 7274 0000 0072 7600 0000 7278  p...rt...rv...rx
+00004c90: 0000 0072 7900 0000 7240 0000 0072 7f00  ...ry...r@...r..
+00004ca0: 0000 7280 0000 0072 8300 0000 7285 0000  ..r....r....r...
+00004cb0: 0072 8600 0000 7287 0000 0072 8800 0000  .r....r....r....
+00004cc0: 7a2b 0a0a 5468 6520 736b 7920 626f 7820  z+..The sky box 
+00004cd0: 6973 2062 6967 6765 7220 666f 7220 7468  is bigger for th
+00004ce0: 6520 696d 6167 6520 7369 7a65 217a 2b50  e image size!z+P
+00004cf0: 6c65 6173 6520 696e 7472 6f64 7563 6520  lease introduce 
+00004d00: 6120 736d 616c 6c65 7220 626f 7820 7468  a smaller box th
+00004d10: 616e 207b 7d20 7069 7821 728a 0000 0072  an {} pix!r....r
+00004d20: 8c00 0000 fa0e 4261 636b 6772 6f75 6e64  ......Background
+00004d30: 206d 6170 7298 0000 0072 9b00 0000 729c   mapr....r....r.
+00004d40: 0000 0072 9d00 0000 729e 0000 0072 9f00  ...r....r....r..
+00004d50: 0000 72a0 0000 0072 a100 0000 72a2 0000  ..r....r....r...
+00004d60: 00fa 290a 4172 6561 2069 6e20 7069 7865  ..).Area in pixe
+00004d70: 6c20 6f66 2074 6865 2064 6574 6563 7469  l of the detecti
+00004d80: 6f6e 206f 626a 6563 7473 3a20 e916 0000  on objects: ....
+00004d90: 00fa 0e61 7865 732e 6c61 6265 6c73 697a  ...axes.labelsiz
+00004da0: 6572 6101 0000 fa0f 6c65 6765 6e64 2e66  era.....legend.f
+00004db0: 6f6e 7473 697a 65e9 1000 0000 fa10 7874  ontsize.......xt
+00004dc0: 6963 6b2e 6d61 6a6f 722e 7369 7a65 fa10  ick.major.size..
+00004dd0: 7874 6963 6b2e 6d69 6e6f 722e 7369 7a65  xtick.minor.size
+00004de0: fa10 7974 6963 6b2e 6d61 6a6f 722e 7369  ..ytick.major.si
+00004df0: 7a65 fa10 7974 6963 6b2e 6d69 6e6f 722e  ze..ytick.minor.
+00004e00: 7369 7a65 fa0f 7874 6963 6b2e 6c61 6265  size..xtick.labe
+00004e10: 6c73 697a 65fa 0f79 7469 636b 2e6c 6162  lsize..ytick.lab
+00004e20: 656c 7369 7a65 a902 72e7 0100 0072 e701  elsize..r....r..
+00004e30: 0000 726b 0000 00da 0650 6169 7265 64da  ..rk.....Paired.
+00004e40: 076e 6561 7265 7374 a903 72a8 0000 00da  .nearest..r.....
+00004e50: 0d69 6e74 6572 706f 6c61 7469 6f6e 727a  .interpolationrz
+00004e60: 0000 00e9 1e00 0000 a901 da08 666f 6e74  ............font
+00004e70: 7369 7a65 fa1a 696d 6167 6573 2f7b 7d5f  size..images/{}_
+00004e80: 7369 6d62 6164 5f7b 7d6b 7063 2e70 6e67  simbad_{}kpc.png
+00004e90: 7a26 0a54 6865 2069 6d61 6765 206f 6620  z&.The image of 
+00004ea0: 3130 3020 6b70 6320 6973 206e 6f74 2061  100 kpc is not a
+00004eb0: 7661 696c 6162 6c65 2902 e911 0000 0072  vailable)......r
+00004ec0: e701 0000 e979 0000 0072 a700 0000 2903  .....y...r....).
+00004ed0: 727a 0000 0072 a800 0000 da06 6578 7465  rz...r......exte
+00004ee0: 6e74 fa07 7820 286b 7063 29fa 0779 2028  nt..x (kpc)..y (
+00004ef0: 6b70 6329 e97a 0000 00a9 0172 0c02 0000  kpc).z.....r....
+00004f00: 2902 e915 0000 0072 e701 0000 e983 0000  )......r........
+00004f10: 00e9 8400 0000 e985 0000 00e9 2c01 0000  ............,...
+00004f20: 7a0f 0a0a 534c 2e70 686f 745f 6d6f 6428  z...SL.phot_mod(
+00004f30: 277a 2127 2c20 7461 625f 6761 6c2c 2063  'z!', tab_gal, c
+00004f40: 6f6e 6e2c 2073 697a 655f 696d 6167 655f  onn, size_image_
+00004f50: 7068 793d fa02 2c20 fa09 2073 6e72 5f67  phy=.., .. snr_g
+00004f60: 203d 20fa 0a2c 2061 7265 6167 616c 3d7a   = .., areagal=z
+00004f70: 0b2c 736b 795f 626f 7820 3d20 fa0d 2c0a  .,sky_box = ..,.
+00004f80: 2064 6562 6c65 6e64 203d 22fa 0322 2c20   deblend ="..", 
+00004f90: 7a2d 7573 6572 5f6f 7264 6572 3d5b 312c  z-user_order=[1,
+00004fa0: 325d 2c20 7573 6572 5f6c 6973 743d 5b22  2], user_list=["
+00004fb0: 4122 2c22 4222 5d2c 2062 616e 643d 277a  A","B"], band='z
+00004fc0: 0227 29fa 0c75 7365 725f 6f72 6465 723d  .')..user_order=
+00004fd0: 5b7a 0e5d 2c20 7573 6572 5f6c 6973 743d  [z.], user_list=
+00004fe0: 5b7a 095d 2c20 6261 6e64 3d27 290e 7201  [z.], band=').r.
+00004ff0: 0100 0072 0201 0000 7203 0100 0072 0401  ...r....r....r..
+00005000: 0000 7205 0100 0072 0601 0000 7207 0100  ..r....r....r...
+00005010: 0072 0801 0000 7271 0000 0072 7200 0000  .r....rq...rr...
+00005020: 7273 0000 0072 c000 0000 72ae 0000 0072  rs...r....r....r
+00005030: c100 0000 294e 7225 0000 0072 c800 0000  ....)Nr%...r....
+00005040: 72b7 0000 0072 c900 0000 72ca 0000 0072  r....r....r....r
+00005050: cb00 0000 7219 0000 0072 d200 0000 72d4  ....r....r....r.
+00005060: 0000 0072 d500 0000 72de 0000 0072 df00  ...r....r....r..
+00005070: 0000 72e0 0000 0072 0500 0000 72d9 0000  ..r....r....r...
+00005080: 0072 cc00 0000 7264 0000 0072 cd00 0000  .r....rd...r....
+00005090: 72ce 0000 0072 cf00 0000 72d0 0000 0072  r....r....r....r
+000050a0: d100 0000 72d3 0000 0072 d600 0000 da06  ....r....r......
+000050b0: 7379 7374 656d 72dd 0000 00da 0a63 6174  systemr......cat
+000050c0: 5f73 696d 6261 6472 d700 0000 72d8 0000  _simbadr....r...
+000050d0: 00da 0f74 7765 6c76 655f 6261 6e64 5f69  ...twelve_band_i
+000050e0: 6d67 da04 7361 7665 da07 6765 745f 696d  mg..save..get_im
+000050f0: 6772 0300 0000 72e4 0000 0072 e500 0000  gr....r....r....
+00005100: 7218 0000 00da 0b70 6c6f 745f 7369 6d62  r......plot_simb
+00005110: 6164 72e6 0000 00da 0669 6d72 6561 6472  adr......imreadr
+00005120: 0a00 0000 72e7 0000 0072 e800 0000 72ea  ....r....r....r.
+00005130: 0000 0072 eb00 0000 720b 0000 0072 ab01  ...r....r....r..
+00005140: 0000 720d 0000 0072 0c00 0000 72ec 0000  ..r....r....r...
+00005150: 0072 1100 0000 7210 0000 0072 f200 0000  .r....r....r....
+00005160: 72f3 0000 0072 f400 0000 720e 0000 0072  r....r....r....r
+00005170: 0f00 0000 da06 6172 676d 6178 72fa 0000  ......argmaxr...
+00005180: 00da 0661 7261 6e67 6572 e300 0000 da0a  ...aranger......
+00005190: 6d61 7470 6c6f 746c 6962 da08 7263 5061  matplotlib..rcPa
+000051a0: 7261 6d73 7226 0000 0072 8901 0000 da05  ramsr&...r......
+000051b0: 666c 6f61 7472 2700 0000 da06 6e61 6e6d  floatr'.....nanm
+000051c0: 6178 da04 7465 7874 72da 0000 0072 b501  ax..textr....r..
+000051d0: 0000 72b7 0100 00da 0d6d 696e 6f72 7469  ..r......minorti
+000051e0: 636b 735f 6f6e da07 7375 6270 6c6f 7472  cks_on..subplotr
+000051f0: 8b01 0000 da06 786c 6162 656c da06 796c  ......xlabel..yl
+00005200: 6162 656c 72c0 0100 0072 3901 0000 2947  abelr....r9...)G
+00005210: 7241 0000 0072 ff00 0000 7200 0100 0072  rA...r....r....r
+00005220: 0101 0000 7202 0100 0072 0301 0000 72e1  ....r....r....r.
+00005230: 0100 0072 e301 0000 72e2 0100 0072 ef01  ...r....r....r..
+00005240: 0000 72f0 0100 0072 f101 0000 7206 0100  ..r....r....r...
+00005250: 0072 0701 0000 72ad 0000 0072 f401 0000  .r....r....r....
+00005260: 7208 0100 00da 0e66 6965 6c64 5f73 697a  r......field_siz
+00005270: 655f 7068 7972 7100 0000 7272 0000 0072  e_phyrq...rr...r
+00005280: 7300 0000 72ae 0000 0072 c100 0000 da08  s...r....r......
+00005290: 7275 6e5f 6175 746f 72c0 0000 0072 0901  run_autor....r..
+000052a0: 0000 72b3 0000 0072 0a01 0000 7213 0100  ..r....r....r...
+000052b0: 0072 bf00 0000 720b 0100 0072 0c01 0000  .r....r....r....
+000052c0: 720d 0100 0072 0e01 0000 72d5 0000 0072  r....r....r....r
+000052d0: 0f01 0000 da09 7261 6473 696d 6261 64da  ......radsimbad.
+000052e0: 096f 7574 7369 6d62 6164 da04 696d 6163  .outsimbad..imac
+000052f0: 721a 0100 00da 0669 6d61 675f 47da 0669  r......imag_G..i
+00005300: 6d61 675f 4972 1b01 0000 da05 7265 6164  mag_Ir......read
+00005310: 6eda 0569 6d61 3530 721c 0100 0072 1d01  n..ima50r....r..
+00005320: 0000 721e 0100 0072 1f01 0000 7220 0100  ..r....r....r ..
+00005330: 0072 8e00 0000 7221 0100 0072 8100 0000  .r....r!...r....
+00005340: 722a 0100 0072 2b01 0000 722c 0100 0072  r*...r+...r,...r
+00005350: 2d01 0000 da08 6761 6c5f 6d61 696e da03  -.....gal_main..
+00005360: 6d70 6cda 0573 6567 6d63 da0e 7369 7a65  mpl..segmc..size
+00005370: 5f69 6d61 6765 5f6b 7063 da05 696d 7365  _image_kpc..imse
+00005380: 6772 3301 0000 da03 706f 7372 ca01 0000  gr3.....posr....
+00005390: da06 696d 6131 3030 da09 7069 785f 7363  ..ima100..pix_sc
+000053a0: 696d 61da 0570 6172 7430 da05 7061 7274  ima..part0..part
+000053b0: 31da 0570 6172 7432 da07 6d61 7861 7265  1..part2..maxare
+000053c0: 6172 2f00 0000 722f 0000 0072 3000 0000  ar/...r/...r0...
+000053d0: da0b 6578 5f70 686f 745f 6d6f 644c 0200  ..ex_phot_modL..
+000053e0: 0073 8a02 0000 0007 1a01 1001 1802 0e01  .s..............
+000053f0: 0801 1401 0a01 02ff 0602 2201 2202 0e01  .........."."...
+00005400: 0e02 1401 1401 1002 1001 1401 1c01 0c01  ................
+00005410: 02ff 0803 1c01 1401 0e01 0e01 0e01 0e01  ................
+00005420: 0402 0c01 0e01 0e01 0e01 0402 0a01 1401  ................
+00005430: 1c01 1c01 0e01 1002 0e01 0e01 0e01 0402  ................
+00005440: 0e01 0a01 0e02 0e01 0a01 0e02 0801 0401  ................
+00005450: 0a01 0602 0402 0e04 0a01 0a01 0200 02ff  ................
+00005460: 0603 0e01 0803 0c01 0e01 2601 1001 2601  ..........&...&.
+00005470: 1001 1e01 0200 0aff 0603 0e01 1002 1801  ................
+00005480: 1001 1e01 0201 0afe 0605 0c01 0e01 0e01  ................
+00005490: 0a00 06ff 0402 0e01 0801 0801 0801 1801  ................
+000054a0: 06ff 0402 1001 0e01 0801 0801 0801 1801  ................
+000054b0: 0601 0200 0200 0200 0200 02fe 0603 1002  ................
+000054c0: 0801 0801 0802 0c01 1201 1801 0600 0200  ................
+000054d0: 06ff 0602 1201 1801 0600 0200 06ff 0603  ................
+000054e0: 0a01 02ff 0602 0a01 0a01 02ff 0602 0a01  ................
+000054f0: 0a01 02ff 0602 0a02 0c01 02ff 0804 1003  ................
+00005500: 0a01 0c01 0200 0200 0200 0201 0200 0200  ................
+00005510: 0200 02fe 0604 0c01 0a01 0a01 0201 1601  ................
+00005520: 0601 1a01 0a01 1401 0a06 0801 0e01 0801  ................
+00005530: 0801 0801 02ff 0602 0c01 0e01 0a01 0a02  ................
+00005540: 0802 0601 02ff 0c02 0e01 0801 0e01 0e01  ................
+00005550: 0e04 0601 0600 06ff 0602 0802 1801 0e01  ................
+00005560: 0a01 0cff 0802 0402 0601 0801 0200 0201  ................
+00005570: 02fe 0604 0a02 0801 0c01 1001 0a01 0a02  ................
+00005580: 0803 0801 0e01 0803 0801 0e01 0e02 0a01  ................
+00005590: 0801 0802 0801 0c01 0e01 0a01 0a02 0801  ................
+000055a0: 0802 0200 02fe 0604 0c01 0801 0a01 1406  ................
+000055b0: 0801 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000055c0: 0a05 0c01 1201 0e01 1402 0a01 02ff 0604  ................
+000055d0: 1401 1201 2e02 0a01 0a01 0801 0a01 0a02  ................
+000055e0: 0802 0a01 0a01 1602 0c01 0e01 0801 0c01  ................
+000055f0: 0a01 0a01 14ff 0602 0a01 0a01 0801 0a01  ................
+00005600: 2001 0801 0a01 0801 0c04 0a01 0c01 0a01   ...............
+00005610: 0a01 14ff 0602 0a01 0a01 0801 0a01 2001  .............. .
+00005620: 0801 0a01 0801 0a01 0a01 1001 1602 0401  ................
+00005630: 1001 1401 2001 0801 0a01 0801 0802 0a01  .... ...........
+00005640: 1201 1e01 0c01 1002 0402 3002 1201 1e01  ..........0.....
+00005650: 1801 1002 0a01 0200 0201 0400 0400 0201  ................
+00005660: 0200 0200 0200 0201 0200 0200 0201 02fb  ................
+00005670: 7243 0200 00da 0362 6f78 6306 0000 0000  rC.....boxc.....
+00005680: 0000 0000 0000 000f 0000 0007 0000 0043  ...............C
+00005690: 0000 0073 3601 0000 7400 a001 7c01 6401  ...s6...t...|.d.
+000056a0: 1900 7c00 6b02 a101 6402 1900 6402 1900  ..|.k...d...d...
+000056b0: 7d06 7c01 6403 1900 7c06 1900 7d07 7c07  }.|.d...|...}.|.
+000056c0: 7402 1b00 7d08 7400 a003 7400 a004 6404  t...}.t...t...d.
+000056d0: a101 a101 7c08 1400 6405 1400 7d09 7c02  ....|...d...}.|.
+000056e0: 7c09 1b00 7d0a 7c03 6406 6b02 7274 6407  |...}.|.d.k.rtd.
+000056f0: a005 7c01 6408 1900 7c06 1900 7c01 6409  ..|.d...|...|.d.
+00005700: 1900 7c06 1900 7c0a a103 7d0b 7c03 640a  ..|...|...}.|.d.
+00005710: 6b02 72a4 640b a005 7c01 6408 1900 7c06  k.r.d...|.d...|.
+00005720: 1900 7c01 6409 1900 7c06 1900 7c0a 640c  ..|.d...|...|.d.
+00005730: 1400 7c0a 640c 1400 a104 7d0b 7c04 640d  ..|.d.....}.|.d.
+00005740: 6b02 72b2 640e 7d0c 6e14 640f a005 7c07  k.r.d.}.n.d...|.
+00005750: 7c04 1700 7c07 7c04 1800 a102 7d0c 7c0b  |...|.|.....}.|.
+00005760: 7c0c 1700 6410 1700 7d0d 7406 6411 8301  |...d...}.t.d...
+00005770: 0100 7406 6412 8301 0100 7406 7c0d 8301  ..t.d.....t.|...
+00005780: 0100 7c05 6400 6b09 9001 720e 7c05 6413  ..|.d.k...r.|.d.
+00005790: 1700 7407 6a08 5f09 7406 6414 7407 6a08  ..t.j._.t.d.t.j.
+000057a0: 6a09 8302 0100 7407 6a08 a00a 7c0d a101  j.....t.j...|...
+000057b0: 7d0e 7406 6415 8301 0100 7406 6416 8301  }.t.d.....t.d...
+000057c0: 0100 7406 7c0e 8301 0100 7c0e 5300 2917  ..t.|.....|.S.).
+000057d0: 4e72 4100 0000 7201 0000 0072 4200 0000  NrA...r....rB...
+000057e0: 7243 0000 0072 4400 0000 72cb 0100 007a  rC...rD...r....z
+000057f0: 2a72 6567 696f 6e28 6369 7263 6c65 2c20  *region(circle, 
+00005800: 4943 5253 2c20 7b3a 2b66 7d20 7b3a 2b66  ICRS, {:+f} {:+f
+00005810: 7d2c 207b 3a2e 3066 7d73 2972 4e00 0000  }, {:.0f}s)rN...
+00005820: 724f 0000 0072 4402 0000 7a2f 7265 6769  rO...rD...z/regi
+00005830: 6f6e 2862 6f78 2c20 4943 5253 2c20 7b3a  on(box, ICRS, {:
+00005840: 2b66 7d20 7b3a 2b66 7d2c 207b 3a2e 3066  +f} {:+f}, {:.0f
+00005850: 7d73 207b 3a2e 3066 7d73 2972 3900 0000  }s {:.0f}s)r9...
+00005860: 7262 0000 0072 c700 0000 7a1d 2026 2072  rb...r....z. & r
+00005870: 6164 7665 6c20 203c 207b 7d20 2620 7261  advel  < {} & ra
+00005880: 6476 656c 203e 207b 7d7a 1120 2620 6f74  dvel > {}z. & ot
+00005890: 7970 6520 3d20 4761 6c61 7879 7a0d 5369  ype = Galaxyz.Si
+000058a0: 6d62 6164 2071 7565 7279 207a 0d3d 3d3d  mbad query z.===
+000058b0: 3d3d 3d3d 3d3d 3d3d 3d0a 7a11 7369 6d62  =========.z.simb
+000058c0: 6164 2f73 696d 2d73 6372 6970 747a 1a43  ad/sim-scriptz.C
+000058d0: 6861 6e67 696e 6720 5369 6d62 6164 2073  hanging Simbad s
+000058e0: 6572 7665 7220 746f 207a 070a 4f75 7470  erver to z..Outp
+000058f0: 7574 7a07 3d3d 3d3d 3d3d 0a29 0b72 2500  utz.======.).r%.
+00005900: 0000 72c8 0000 0072 b700 0000 72c9 0000  ..r....r....r...
+00005910: 0072 ca00 0000 7264 0000 0072 cb00 0000  .r....rd...r....
+00005920: 7206 0000 00da 0653 696d 6261 64da 0a53  r......Simbad..S
+00005930: 494d 4241 445f 5552 4cda 0e71 7565 7279  IMBAD_URL..query
+00005940: 5f63 7269 7465 7269 6129 0f72 c200 0000  _criteria).r....
+00005950: 72ff 0000 0072 0101 0000 72e1 0100 0072  r....r....r....r
+00005960: e201 0000 72e3 0100 0072 0901 0000 da06  ....r....r......
+00005970: 7665 6c67 616c 72b3 0000 00da 076b 7063  velgalr......kpc
+00005980: 5f61 7263 da07 6172 6364 6973 74da 0566  _arc..arcdist..f
+00005990: 7061 7274 da05 7370 6172 74da 0761 6c6c  part..spart..all
+000059a0: 6372 6974 da06 7265 7375 6c74 722f 0000  crit..resultr/..
+000059b0: 0072 2f00 0000 7230 0000 0072 1d02 0000  .r/...r0...r....
+000059c0: b703 0000 7346 0000 0000 031a 010c 0208  ....sF..........
+000059d0: 0218 0208 0308 0104 010a 010a 0002 fe04  ................
+000059e0: 0308 0104 010a 010a 0106 0006 fd04 0408  ................
+000059f0: 0106 020a 0106 ff04 020c 0208 0108 0108  ................
+00005a00: 020a 010c 010e 010c 0208 0108 0108 0272  ...............r
+00005a10: 1d02 0000 7215 0200 0063 0500 0000 0000  ....r....c......
+00005a20: 0000 0000 0000 1200 0000 0600 0000 4300  ..............C.
+00005a30: 0000 7302 0100 0074 00a0 017c 0164 0119  ..s....t...|.d..
+00005a40: 007c 006b 02a1 0164 0219 0064 0219 007d  .|.k...d...d...}
+00005a50: 057c 0164 0319 007c 0519 007d 067c 0674  .|.d...|...}.|.t
+00005a60: 021b 007d 0774 00a0 0374 00a0 0464 04a1  ...}.t...t...d..
+00005a70: 01a1 017c 0714 0064 0514 007d 087c 0264  ...|...d...}.|.d
+00005a80: 0614 007c 081b 007d 097c 0964 071b 007d  ...|...}.|.d...}
+00005a90: 0a7c 0164 0819 007c 0519 007d 0b7c 0164  .|.d...|...}.|.d
+00005aa0: 0919 007c 0519 007d 0c64 0a7d 0d64 0ba0  ...|...}.d.}.d..
+00005ab0: 0574 0664 0c83 017c 037c 047c 0aa1 047d  .t.d...|.|.|...}
+00005ac0: 0e64 0da0 057c 0b7c 0ca1 027d 0f74 077c  .d...|.|...}.t.|
+00005ad0: 0d7c 0e17 007c 0f17 0064 0e17 0064 0fa0  .|...|...d...d..
+00005ae0: 057c 007c 02a1 0283 0201 0074 08a0 0964  .|.|.......t...d
+00005af0: 0fa0 057c 007c 02a1 02a1 017d 1064 0ba0  ...|.|.....}.d..
+00005b00: 0574 0664 1083 017c 037c 047c 0aa1 047d  .t.d...|.|.|...}
+00005b10: 0e74 0aa0 0b7c 0d7c 0e17 007c 0f17 00a1  .t...|.|...|....
+00005b20: 017d 117c 11a0 0c64 11a0 057c 007c 02a1  .}.|...d...|.|..
+00005b30: 02a1 0101 0064 0053 0029 124e 7241 0000  .....d.S.).NrA..
+00005b40: 0072 0100 0000 7242 0000 0072 4300 0000  .r....rB...rC...
+00005b50: 7244 0000 0072 3900 0000 724a 0000 0072  rD...r9...rJ...r
+00005b60: 4e00 0000 724f 0000 007a 3968 7474 703a  N...rO...z9http:
+00005b70: 2f2f 616c 6173 6b79 2e75 2d73 7472 6173  //alasky.u-stras
+00005b80: 6267 2e66 722f 6869 7073 2d69 6d61 6765  bg.fr/hips-image
+00005b90: 2d73 6572 7669 6365 732f 6869 7073 3266  -services/hips2f
+00005ba0: 6974 733f 7a21 6869 7073 3d7b 7d26 7769  its?z!hips={}&wi
+00005bb0: 6474 683d 7b7d 2668 6569 6768 743d 7b7d  dth={}&height={}
+00005bc0: 2666 6f76 3d7b 7d7a 0a44 5353 322f 636f  &fov={}z.DSS2/co
+00005bd0: 6c6f 727a 2a26 7072 6f6a 6563 7469 6f6e  lorz*&projection
+00005be0: 3d54 414e 2663 6f6f 7264 7379 733d 6963  =TAN&coordsys=ic
+00005bf0: 7273 2672 613d 7b7d 2664 6563 3d7b 7d7a  rs&ra={}&dec={}z
+00005c00: 0b26 666f 726d 6174 3d70 6e67 7209 0200  .&format=pngr...
+00005c10: 007a 0844 5353 322f 7265 64fa 2066 6974  .z.DSS2/red. fit
+00005c20: 735f 696d 6167 6573 2f7b 7d5f 7369 6d62  s_images/{}_simb
+00005c30: 6164 5f7b 7d6b 7063 2e66 6974 7329 0d72  ad_{}kpc.fits).r
+00005c40: 2500 0000 72c8 0000 0072 b700 0000 72c9  %...r....r....r.
+00005c50: 0000 0072 ca00 0000 7264 0000 0072 1200  ...r....rd...r..
+00005c60: 0000 7213 0000 0072 e600 0000 7222 0200  ..r....r....r"..
+00005c70: 0072 0300 0000 72e4 0000 0072 ed00 0000  .r....r....r....
+00005c80: 2912 72c2 0000 0072 ff00 0000 7201 0100  ).r....r....r...
+00005c90: 00da 0577 6964 7468 da06 6865 6967 6874  ...width..height
+00005ca0: 7209 0100 0072 4802 0000 72b3 0000 0072  r....rH...r....r
+00005cb0: 4902 0000 724a 0200 00da 0366 6f76 724e  I...rJ.....fovrN
+00005cc0: 0000 0072 4f00 0000 da09 6261 7369 635f  ...rO.....basic_
+00005cd0: 7572 6cda 0b6f 626a 6563 745f 7572 6c31  url..object_url1
+00005ce0: da0b 6f62 6a65 6374 5f75 726c 32da 0a69  ..object_url2..i
+00005cf0: 6d61 5f73 696d 6261 64da 0368 6475 722f  ma_simbad..hdur/
+00005d00: 0000 0072 2f00 0000 7230 0000 00da 0f73  ...r/...r0.....s
+00005d10: 696d 6261 645f 646f 776e 6c6f 6164 e303  imbad_download..
+00005d20: 0000 7338 0000 0000 031a 010c 0208 0118  ..s8............
+00005d30: 020c 0108 020c 010c 0204 010a 0102 0002  ................
+00005d40: 0002 ff04 020c 0510 010a ff04 030a 0102  ................
+00005d50: ff06 050a 0102 0002 0002 ff04 0212 0172  ...............r
+00005d60: 5802 0000 e90c 0000 0063 0c00 0000 0000  X........c......
+00005d70: 0000 0000 0000 3100 0000 0c00 0000 4300  ......1.......C.
+00005d80: 0000 7304 0700 0074 00a0 017c 0164 0119  ..s....t...|.d..
+00005d90: 007c 006b 02a1 0164 0219 0064 0219 007d  .|.k...d...d...}
+00005da0: 0c7c 0164 0319 007c 0c19 007d 0d7c 0d74  .|.d...|...}.|.t
+00005db0: 021b 007d 0e74 00a0 0374 00a0 0464 04a1  ...}.t...t...d..
+00005dc0: 01a1 017c 0e14 0064 0514 007d 0f7c 0264  ...|...d...}.|.d
+00005dd0: 0614 007c 0f1b 007d 107c 1064 071b 007d  ...|...}.|.d...}
+00005de0: 117c 0164 0819 007c 0c19 007d 127c 0164  .|.d...|...}.|.d
+00005df0: 0919 007c 0c19 007d 1364 0aa0 057c 007c  ...|...}.d...|.|
+00005e00: 02a1 027d 1474 066a 07a0 087c 14a1 0173  ...}.t.j...|...s
+00005e10: ae74 0964 0b7c 149b 0064 0c9d 0383 0101  .t.d.|...d......
+00005e20: 0074 0a7c 007c 017c 027c 037c 0464 0d8d  .t.|.|.|.|.|.d..
+00005e30: 0501 006e 1674 0974 0b6a 0c64 0e7c 149b  ...n.t.t.j.d.|..
+00005e40: 0064 0f9d 0317 0083 0101 0074 0da0 0e64  .d.........t...d
+00005e50: 0aa0 057c 007c 02a1 02a1 017d 1574 0fa0  ...|.|.....}.t..
+00005e60: 1064 10a0 057c 007c 02a1 02a1 017d 1674  .d...|.|.....}.t
+00005e70: 0974 0b6a 1164 1117 0083 0101 0074 127c  .t.j.d.......t.|
+00005e80: 007c 017c 0264 127c 0964 0064 138d 067d  .|.|.d.|.d.d...}
+00005e90: 177c 177c 1764 1419 0064 026b 0419 007d  .|.|.d...d.k...}
+00005ea0: 1774 0f6a 1364 1564 168d 0101 0074 0f6a  .t.j.d.d.....t.j
+00005eb0: 147c 1674 00a0 1564 1764 1864 1764 1867  .|.t...d.d.d.d.g
+00005ec0: 04a1 017c 0214 0064 198d 0201 0074 167c  ...|...d.....t.|
+00005ed0: 1274 176a 1814 007c 1374 176a 1814 0083  .t.j...|.t.j....
+00005ee0: 027d 187c 0a64 1a6b 0290 0172 8e74 196a  .}.|.d.k...r.t.j
+00005ef0: 1a7c 1864 1b7c 1014 0074 176a 1b14 0064  .|.d.|...t.j...d
+00005f00: 1c8d 027d 197c 197c 1964 1d19 0064 026b  ...}.|.|.d...d.k
+00005f10: 0419 007d 1974 167c 1764 1e19 007c 1764  ...}.t.|.d...|.d
+00005f20: 1f19 0083 027d 1a7c 18a0 1c7c 1aa1 017d  .....}.|...|...}
+00005f30: 1b7c 1b6a 1b7c 0f14 007d 1c74 0964 2083  .|.j.|...}.t.d .
+00005f40: 0101 0074 0974 0b6a 1d64 2117 0083 0101  ...t.t.j.d!.....
+00005f50: 0074 0964 2283 0101 0074 00a0 1e74 1f7c  .t.d"....t...t.|
+00005f60: 1a83 01a1 0144 005d 407d 1d64 237d 1e74  .....D.]@}.d#}.t
+00005f70: 097c 1e64 24a0 057c 007c 1d7c 1764 2519  .|.d$..|.|.|.d%.
+00005f80: 007c 1d19 007c 1764 1419 007c 1d19 007c  .|...|.d...|...|
+00005f90: 1c7c 1d19 007c 1b6a 1b7c 1d19 00a1 0617  .|...|.j.|......
+00005fa0: 0083 0101 0090 0171 e074 20a0 217c 1564  .......q.t .!|.d
+00005fb0: 0219 006a 22a1 017d 1f7c 1fa0 237c 1764  ...j"..}.|..#|.d
+00005fc0: 1e19 007c 1764 1f19 0064 02a1 035c 027d  ...|.d...d...\.}
+00005fd0: 207d 217c 0264 0614 007c 031b 007d 227c   }!|.d...|...}"|
+00005fe0: 207c 0364 1b14 0018 007c 2214 007d 207c   |.d.....|"..} |
+00005ff0: 217c 0364 1b14 0018 007c 2214 007d 217c  !|.d.....|"..}!|
+00006000: 1564 0219 006a 247d 237c 207c 236a 2564  .d...j$}#| |#j%d
+00006010: 1819 007c 2214 0064 2614 006b 047c 217c  ...|"..d&..k.|!|
+00006020: 236a 2564 0219 007c 2214 0064 2614 006b  #j%d...|"..d&..k
+00006030: 0440 007c 2064 1b7c 2214 007c 236a 2564  .@.| d.|"..|#j%d
+00006040: 1819 0014 006b 0040 007c 2164 1b7c 2214  .....k.@.|!d.|".
+00006050: 007c 236a 2564 0219 0014 006b 0040 007d  .|#j%d.....k.@.}
+00006060: 2474 0f6a 267c 207c 2419 007c 217c 2419  $t.j&| |$..|!|$.
+00006070: 0064 2764 2864 2964 2a8d 0501 007c 0a64  .d'd(d)d*....|.d
+00006080: 1a6b 0290 0472 727c 1964 2b19 007d 257c  .k...rr|.d+..}%|
+00006090: 1964 2c19 007d 267c 1fa0 237c 257c 2664  .d,..}&|..#|%|&d
+000060a0: 02a1 035c 027d 277d 287c 277c 0364 1b14  ...\.}'}(|'|.d..
+000060b0: 0018 007c 2214 007d 277c 287c 0364 1b14  ...|"..}'|(|.d..
+000060c0: 0018 007c 2214 007d 287c 277c 236a 2564  ...|"..}(|'|#j%d
+000060d0: 1819 007c 2214 0064 2614 006b 047c 287c  ...|"..d&..k.|(|
+000060e0: 236a 2564 0219 007c 2214 0064 2614 006b  #j%d...|"..d&..k
+000060f0: 0440 007c 2764 1b7c 2214 007c 236a 2564  .@.|'d.|"..|#j%d
+00006100: 1819 0014 006b 0040 007c 2864 1b7c 2214  .....k.@.|(d.|".
+00006110: 007c 236a 2564 0219 0014 006b 0040 007d  .|#j%d.....k.@.}
+00006120: 2974 0f6a 267c 277c 2919 007c 287c 2919  )t.j&|'|)..|(|).
+00006130: 0064 2764 2d64 2e64 2f8d 0501 0074 0964  .d'd-d.d/....t.d
+00006140: 2083 0101 0074 0974 0b6a 0c64 3017 0083   ....t.t.j.d0...
+00006150: 0101 0074 0964 3183 0101 0074 097c 1964  ...t.d1....t.|.d
+00006160: 3219 0083 0101 0064 337c 1964 2b19 005f  2......d3|.d+.._
+00006170: 2764 337c 1964 2c19 005f 2774 167c 1964  'd3|.d,.._'t.|.d
+00006180: 2b19 007c 1964 2c19 0083 027d 1a7c 18a0  +..|.d,....}.|..
+00006190: 1c7c 1aa1 017d 1b7c 1b6a 1b7c 0f14 007d  .|...}.|.j.|...}
+000061a0: 1c74 0964 2083 0101 0074 00a0 1e74 1f7c  .t.d ....t...t.|
+000061b0: 1a83 01a1 0144 005d 407d 1d64 237d 1e74  .....D.]@}.d#}.t
+000061c0: 097c 1e64 24a0 057c 007c 1d7c 1964 3419  .|.d$..|.|.|.d4.
+000061d0: 007c 1d19 007c 1964 1d19 007c 1d19 007c  .|...|.d...|...|
+000061e0: 1c7c 1d19 007c 1b6a 1b7c 1d19 00a1 0617  .|...|.j.|......
+000061f0: 0083 0101 0090 0471 3074 00a0 287c 21a1  .......q0t..(|!.
+00006200: 017d 2a7c 247c 2a19 007d 247c 0864 356b  .}*|$|*..}$|.d5k
+00006210: 0290 0572 9474 297c 2a7c 2419 0083 0144  ...r.t)|*|$....D
+00006220: 005d f85c 027d 1d7d 2b74 2a7c 1764 3619  .].\.}.}+t*|.d6.
+00006230: 007c 2b19 0083 0164 37a0 057c 1764 1419  .|+....d7..|.d..
+00006240: 007c 2b19 007c 2ba1 0217 007d 2c7c 207c  .|+..|+....},| |
+00006250: 2a19 007c 2419 007c 1d19 007c 0517 007d  *..|$..|...|...}
+00006260: 2d7c 217c 2a19 007c 2419 007c 1d19 007c  -|!|*..|$..|...|
+00006270: 0617 007d 2e7c 1d64 026b 0290 0572 0e74  ...}.|.d.k...r.t
+00006280: 0f6a 2b7c 2d7c 2e7c 2c64 3864 3964 3a8d  .j+|-|.|,d8d9d:.
+00006290: 0501 006e 827c 217c 2a19 007c 2419 007c  ...n.|!|*..|$..|
+000062a0: 1d64 1818 0019 007c 0617 007d 2f74 2c7c  .d.....|...}/t,|
+000062b0: 2e7c 2f18 0083 0164 3b6b 0090 0572 407c  .|/....d;k...r@|
+000062c0: 2e7c 0737 007d 2e7c 1d64 186b 0490 0572  .|.7.}.|.d.k...r
+000062d0: 7c7c 217c 2a19 007c 2419 007c 1d64 0618  ||!|*..|$..|.d..
+000062e0: 0019 007c 0617 007d 3074 2c7c 2e7c 3018  ...|...}0t,|.|0.
+000062f0: 0083 0164 3c6b 0090 0572 7c7c 2e7c 0737  ...d<k...r||.|.7
+00006300: 007d 2e74 0f6a 2b7c 2d7c 2e7c 2c64 3864  .}.t.j+|-|.|,d8d
+00006310: 3964 3a8d 0501 0090 0471 9a7c 0864 356b  9d:......q.|.d5k
+00006320: 0290 0672 ce7c 0a64 1a6b 0290 0672 ce74  ...r.|.d.k...r.t
+00006330: 00a0 287c 28a1 017d 2a7c 297c 2a19 007d  ..(|(..}*|)|*..}
+00006340: 2974 297c 2a7c 2919 0083 0144 0090 015d  )t)|*|)....D...]
+00006350: 045c 027d 1d7d 2b74 2a7c 1964 3d19 007c  .\.}.}+t*|.d=..|
+00006360: 2b19 0083 0164 37a0 057c 1964 1d19 007c  +....d7..|.d...|
+00006370: 2b19 007c 2ba1 0217 007d 2c7c 277c 2a19  +..|+....},|'|*.
+00006380: 007c 2919 007c 1d19 007c 0517 007d 2d7c  .|)..|...|...}-|
+00006390: 287c 2a19 007c 2919 007c 1d19 007c 0617  (|*..|)..|...|..
+000063a0: 007c 0b18 007d 2e7c 1d64 026b 0290 0672  .|...}.|.d.k...r
+000063b0: 4074 0f6a 2b7c 2d7c 2e7c 2c64 3864 2e64  @t.j+|-|.|,d8d.d
+000063c0: 3a8d 0501 006e 8a7c 287c 2a19 007c 2919  :....n.|(|*..|).
+000063d0: 007c 1d64 1818 0019 007c 0617 007c 0b18  .|.d.....|...|..
+000063e0: 007d 2f74 2c7c 2e7c 2f18 0083 0164 3b6b  .}/t,|.|/....d;k
+000063f0: 0090 0672 767c 2e7c 0737 007d 2e7c 1d64  ...rv|.|.7.}.|.d
+00006400: 186b 0490 0672 b67c 287c 2a19 007c 2919  .k...r.|(|*..|).
+00006410: 007c 1d64 0618 0019 007c 0617 007c 0b18  .|.d.....|...|..
+00006420: 007d 3074 2c7c 2e7c 3018 0083 0164 3c6b  .}0t,|.|0....d<k
+00006430: 0090 0672 b67c 2e7c 0737 007d 2e74 0f6a  ...r.|.|.7.}.t.j
+00006440: 2b7c 2d7c 2e7c 2c64 3864 2e64 3a8d 0501  +|-|.|,d8d.d:...
+00006450: 0090 0571 c674 0fa0 2d64 3ea1 0101 0074  ...q.t..-d>....t
+00006460: 0fa0 2e64 3fa1 0101 0074 0fa0 2fa1 0001  ...d?....t../...
+00006470: 0074 0f6a 3064 40a0 057c 007c 02a1 0264  .t.j0d@..|.|...d
+00006480: 4164 428d 0201 0064 0053 0029 434e 7241  AdB....d.S.)CNrA
+00006490: 0000 0072 0100 0000 7242 0000 0072 4300  ...r....rB...rC.
+000064a0: 0000 7244 0000 0072 3900 0000 724a 0000  ..rD...r9...rJ..
+000064b0: 0072 4e00 0000 724f 0000 0072 4f02 0000  .rN...rO...rO...
+000064c0: 725d 0000 0072 5e00 0000 a903 7201 0100  r]...r^.....r...
+000064d0: 0072 5002 0000 7251 0200 00fa 060a 5468  .rP...rQ......Th
+000064e0: 6973 20fa 1e20 6669 6c65 2069 7320 616c  is .. file is al
+000064f0: 7265 6164 7920 646f 776e 6c6f 6164 6564  ready downloaded
+00006500: 2e2e 2e72 0902 0000 7a1a 0a2d 2d2d 2d2d  ...r....z..-----
+00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006520: 2d2d 2d0a 72cb 0100 0029 0372 e101 0000  ---.r....).r....
+00006530: 72e2 0100 0072 e301 0000 da08 5256 5f56  r....r......RV_V
+00006540: 414c 5545 a902 72cd 0100 0072 cd01 0000  ALUE..r....r....
+00006550: 7276 0000 0072 6200 0000 7269 0000 0072  rv...rb...ri...r
+00006560: 1002 0000 7240 0000 0072 4900 0000 2901  ....r@...rI...).
+00006570: da06 7261 6469 7573 da08 5665 6c6f 6369  ..radius..Veloci
+00006580: 7479 da04 5241 5f64 da05 4445 435f 6472  ty..RA_d..DEC_dr
+00006590: c700 0000 7a14 0a50 726f 6a65 6374 6564  ....z..Projected
+000065a0: 2044 6973 7461 6e63 6573 72d0 0100 00fa   Distancesr.....
+000065b0: 1b50 726f 7965 6374 6564 2064 6973 7461  .Proyected dista
+000065c0: 6e63 6520 6265 7477 6565 6e20 7a3b 7b7d  nce between z;{}
+000065d0: 2061 6e64 2028 7b7d 2920 7b7d 2028 7b7d   and ({}) {} ({}
+000065e0: 206b 6d2f 7329 2069 7320 3d20 7b3a 2e31   km/s) is = {:.1
+000065f0: 667d 5c2c 6b70 6320 287b 3a2e 3166 7d24  f}\,kpc ({:.1f}$
+00006600: 5c61 7263 7365 6324 29da 074d 4149 4e5f  \arcsec$)..MAIN_
+00006610: 4944 e700 0000 0000 00e0 bf72 3a00 0000  ID.........r:...
+00006620: 7279 0100 00da 0167 a903 723e 0100 00da  ry.....g..r>....
+00006630: 0a66 6163 6563 6f6c 6f72 73da 0a65 6467  .facecolors..edg
+00006640: 6563 6f6c 6f72 73da 0252 41da 0344 4543  ecolors..RA..DEC
+00006650: 7228 0100 00da 0172 2903 723e 0100 00da  r(.....r).r>....
+00006660: 066d 6172 6b65 72da 0563 6f6c 6f72 7a23  .marker..colorz#
+00006670: 0a4e 4544 2054 6162 6c65 2028 4e6f 2072  .NED Table (No r
+00006680: 6563 7472 6963 7469 6f6e 2069 6e20 5672  ectriction in Vr
+00006690: 6164 297a 253d 3d3d 3d3d 3d3d 3d3d 3d3d  ad)z%===========
+000066a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000066b0: 3d3d 3d3d 3d3d 3d3d 3d0a 2906 fa0b 4f62  =========.)...Ob
+000066c0: 6a65 6374 204e 616d 6572 6a02 0000 726b  ject Namerj...rk
+000066d0: 0200 00da 0454 7970 6572 6002 0000 da08  .....Typer`.....
+000066e0: 5265 6473 6869 6674 da03 6465 6772 6f02  Redshift..degro.
+000066f0: 0000 729c 0000 00da 054f 5459 5045 7a11  ..r......OTYPEz.
+00006700: 2056 7261 643d 7b3a 2e30 667d 2028 7b7d   Vrad={:.0f} ({}
+00006710: 2972 5902 0000 da01 77a9 0272 0802 0000  )rY.....w..r....
+00006720: 726e 0200 0072 0602 0000 e93c 0000 0072  rn...r.....<...r
+00006730: 7002 0000 720d 0200 0072 0e02 0000 7a22  p...r....r....z"
+00006740: 696d 6167 6573 2f7b 7d5f 7369 6d62 6164  images/{}_simbad
+00006750: 5f7b 7d6b 7063 5f6d 6172 6b65 7273 2e70  _{}kpc_markers.p
+00006760: 6e67 727c 0000 0072 7d00 0000 2931 7225  ngr|...r}...)1r%
+00006770: 0000 0072 c800 0000 72b7 0000 0072 c900  ...r....r....r..
+00006780: 0000 72ca 0000 0072 6400 0000 72d4 0000  ..r....rd...r...
+00006790: 0072 d500 0000 72d6 0000 0072 cb00 0000  .r....r....r....
+000067a0: 7258 0200 0072 1900 0000 72d2 0000 0072  rX...r....r....r
+000067b0: 0300 0000 72e4 0000 0072 e600 0000 7222  ....r....r....r"
+000067c0: 0200 0072 dd00 0000 721d 0200 0072 e700  ...r....r....r..
+000067d0: 0000 72e8 0000 0072 8b01 0000 7209 0000  ..r....r....r...
+000067e0: 00da 0175 7272 0200 0072 0700 0000 da0c  ...urr...r......
+000067f0: 7175 6572 795f 7265 6769 6f6e da06 6172  query_region..ar
+00006800: 6373 6563 da0a 7365 7061 7261 7469 6f6e  csec..separation
+00006810: 72cc 0000 0072 2402 0000 72e3 0000 0072  r....r$...r....r
+00006820: 0800 0000 da03 5743 53da 0668 6561 6465  ......WCS..heade
+00006830: 72da 0d61 6c6c 5f77 6f72 6c64 3270 6978  r..all_world2pix
+00006840: 72e5 0000 0072 ab01 0000 da07 7363 6174  r....r......scat
+00006850: 7465 72da 0475 6e69 7472 f900 0000 72fb  ter..unitr....r.
+00006860: 0000 0072 da00 0000 7229 0200 00da 0361  ...r....r).....a
+00006870: 6273 722c 0200 0072 2d02 0000 722a 0200  bsr,...r-...r*..
+00006880: 0072 e900 0000 2931 72c2 0000 0072 ff00  .r....)1r....r..
+00006890: 0000 7201 0100 0072 5002 0000 7251 0200  ..r....rP...rQ..
+000068a0: 0072 ef01 0000 72f0 0100 0072 f101 0000  .r....r....r....
+000068b0: da08 6c61 6265 6c74 7874 72e2 0100 00da  ..labeltxtr.....
+000068c0: 086e 6564 5f70 6c6f 74da 0a64 656c 7461  .ned_plot..delta
+000068d0: 795f 6e65 6472 0901 0000 7248 0200 0072  y_nedr....rH...r
+000068e0: b300 0000 7249 0200 0072 4a02 0000 7252  ....rI...rJ...rR
+000068f0: 0200 0072 4e00 0000 724f 0000 0072 d500  ...rN...rO...r..
+00006900: 0000 7257 0200 0072 5602 0000 72ed 0100  ..rW...rV...r...
+00006910: 00da 0867 616c 636f 6f72 64da 0974 6162  ...galcoord..tab
+00006920: 6c65 5f6e 6564 da04 736b 7963 da03 7365  le_ned..skyc..se
+00006930: 70da 0773 6570 5f6b 7063 7233 0100 00da  p..sep_kpcr3....
+00006940: 0374 7874 7274 0200 00da 0358 6763 da03  .txtrt.....Xgc..
+00006950: 5967 63da 0573 6369 6d61 722e 0000 00da  Ygc..scimar.....
+00006960: 0463 6f6e 64da 066e 6564 5f72 61da 076e  .cond..ned_ra..n
+00006970: 6564 5f64 6563 da07 5867 635f 6e65 64da  ed_dec..Xgc_ned.
+00006980: 0759 6763 5f6e 6564 da08 636f 6e64 5f6e  .Ygc_ned..cond_n
+00006990: 6564 da05 6f72 6465 6dda 0469 6e64 67da  ed..ordem..indg.
+000069a0: 0574 6578 746c da04 7870 6f73 da04 7970  .textl..xpos..yp
+000069b0: 6f73 da05 7970 6f73 62da 0679 706f 7362  os..yposb..yposb
+000069c0: 6272 2f00 0000 722f 0000 0072 3000 0000  br/...r/...r0...
+000069d0: da10 7369 6d62 6164 5f74 6875 6d62 6e61  ..simbad_thumbna
+000069e0: 696c 0804 0000 7328 0100 0000 061a 010c  il....s(........
+000069f0: 0208 0118 020c 0108 020c 010c 020c 010c  ................
+00006a00: 0110 0108 0102 0002 ff08 0316 020a 0102  ................
+00006a10: ff06 020a 0102 ff06 040e 010a 0102 0002  ................
+00006a20: ff06 0210 040c 0120 0216 030a 0118 0110  ....... ........
+00006a30: 0212 010a 020a 0208 010e 0108 0112 0204  ................
+00006a40: 0108 0102 0002 000a 000a 0006 0108 fe0c  ................
+00006a50: 0510 011a 020c 0210 0110 020a 022a 0114  .............*..
+00006a60: ff02 0114 ff04 0314 0102 ff06 040a 0208  ................
+00006a70: 0108 0212 0210 0110 0214 0114 ff02 0214  ................
+00006a80: fe02 0314 fd04 0510 0102 0002 0002 ff06  ................
+00006a90: 0208 010e 0108 010c 020a 010a 0112 020a  ................
+00006aa0: 020a 0208 0112 0104 0108 0102 0002 000a  ................
+00006ab0: 000a 0106 0008 fe0c 040a 0108 030a 0114  ................
+00006ac0: 0112 010a 0002 ff06 0314 0114 020a 0116  ................
+00006ad0: 0318 0112 0208 010a 0118 0112 0108 0218  ................
+00006ae0: 0214 010a 0108 0116 0112 010a 0002 ff06  ................
+00006af0: 0314 0118 020a 0116 031c 0112 0208 010a  ................
+00006b00: 011c 0112 0108 0218 020a 010a 0108 010e  ................
+00006b10: 0102 ff72 9a02 0000 5463 1400 0000 0000  ...r....Tc......
+00006b20: 0000 0000 0000 3500 0000 1000 0000 4300  ......5.......C.
+00006b30: 0000 7300 0b00 0074 00a0 017c 0164 0119  ..s....t...|.d..
+00006b40: 007c 006b 02a1 0164 0219 0064 0219 007d  .|.k...d...d...}
+00006b50: 147c 0164 0319 007c 1419 0074 021b 007d  .|.d...|...t...}
+00006b60: 1574 00a0 0374 00a0 0464 04a1 01a1 017c  .t...t...d.....|
+00006b70: 1514 0064 0514 007d 167c 1164 066b 0272  ...d...}.|.d.k.r
+00006b80: 5064 077d 176e 1a7c 0364 0814 007c 161b  Pd.}.n.|.d...|..
+00006b90: 0064 091b 007d 1774 0564 0a7c 1783 0201  .d...}.t.d.|....
+00006ba0: 007c 037c 161b 007c 171b 0064 0814 007d  .|.|...|...d...}
+00006bb0: 187c 1064 0b6b 0272 9674 0574 066a 0764  .|.d.k.r.t.t.j.d
+00006bc0: 0ca0 087c 16a1 0117 0083 0101 007c 0f64  ...|.........|.d
+00006bd0: 0b6b 0290 0172 2074 0574 066a 0964 0d17  .k...r t.t.j.d..
+00006be0: 0083 0101 0074 0564 0e83 0101 0074 0a6a  .....t.d.....t.j
+00006bf0: 0ba0 0c74 0a6a 0ba0 0d74 0ea1 01a1 017d  ...t.j...t.....}
+00006c00: 1974 0f6a 107c 1964 0f17 0064 1064 118d  .t.j.|.d...d.d..
+00006c10: 027d 1a74 057c 1a64 1219 0074 00a0 017c  .}.t.|.d...t...|
+00006c20: 1a64 0119 007c 006b 02a1 0164 0219 0019  .d...|.k...d....
+00006c30: 0083 0101 0074 057c 1a64 1319 0074 00a0  .....t.|.d...t..
+00006c40: 017c 1a64 0119 007c 006b 02a1 0164 0219  .|.d...|.k...d..
+00006c50: 0019 0083 0101 007c 0b90 0372 e474 11a0  .......|...r.t..
+00006c60: 107c 13a1 017d 1b74 127c 0464 1419 007c  .|...}.t.|.d...|
+00006c70: 0519 007c 0464 1519 007c 0519 0083 027d  ...|.d...|.....}
+00006c80: 1c7c 1c64 0219 00a0 137c 1c64 1664 0085  .|.d.....|.d.d..
+00006c90: 0219 00a1 017d 1d7c 1d6a 147c 1614 007d  .....}.|.j.|...}
+00006ca0: 1e74 00a0 1574 167c 1c64 1664 0085 0219  .t...t.|.d.d....
+00006cb0: 0083 01a1 0144 005d 3e7d 1f74 066a 1764  .....D.]>}.t.j.d
+00006cc0: 1717 007d 2074 057c 2064 18a0 087c 0664  ...} t.| d...|.d
+00006cd0: 0219 007c 067c 1f64 1617 0019 007c 1e7c  ...|.|.d.....|.|
+00006ce0: 1f19 007c 1d6a 147c 1f19 00a1 0417 0083  ...|.j.|........
+00006cf0: 0101 0090 0171 8074 0564 1983 0101 0074  .....q.t.d.....t
+00006d00: 1874 197c 057c 0683 0283 0144 0090 015d  .t.|.|.....D...]
+00006d10: fa5c 027d 1f5c 027d 217d 2274 167c 1b83  .\.}.\.}!}"t.|..
+00006d20: 0164 026b 0290 0172 fa7c 1ba0 1aa1 0001  .d.k...r.|......
+00006d30: 0074 1b7c 1b64 1a19 007c 226b 0283 0190  .t.|.d...|"k....
+00006d40: 0272 3e74 0574 066a 0764 1b7c 229b 0064  .r>t.t.j.d.|"..d
+00006d50: 1c9d 0317 0083 0101 0074 00a0 017c 1b64  .........t...|.d
+00006d60: 1a19 007c 226b 02a1 0164 0219 0064 0219  ...|"k...d...d..
+00006d70: 007d 236e 2c74 0574 066a 0764 1da0 087c  .}#n,t.t.j.d...|
+00006d80: 22a1 0117 0083 0101 007c 1ba0 1aa1 0001  "........|......
+00006d90: 0064 1e7d 237c 227c 1b64 1a19 007c 233c  .d.}#|"|.d...|#<
+00006da0: 007c 0464 1419 007c 2119 007c 1b64 1f19  .|.d...|!..|.d..
+00006db0: 007c 233c 007c 0464 1519 007c 2119 007c  .|#<.|.d...|!..|
+00006dc0: 1b64 2019 007c 233c 007c 0464 2119 007c  .d ..|#<.|.d!..|
+00006dd0: 2119 007c 1b64 2219 007c 233c 007c 0464  !..|.d"..|#<.|.d
+00006de0: 2319 007c 2119 007c 1b64 2419 007c 233c  #..|!..|.d$..|#<
+00006df0: 007c 1b64 2519 00a0 1c74 1da1 017c 1b64  .|.d%....t...|.d
+00006e00: 253c 007c 0464 2619 007c 2119 007c 1b64  %<.|.d&..|!..|.d
+00006e10: 2519 007c 233c 007c 0c64 0b6b 0290 0272  %..|#<.|.d.k...r
+00006e20: f664 167c 1b64 2719 007c 233c 007c 0c64  .d.|.d'..|#<.|.d
+00006e30: 066b 0290 0372 0c64 027c 1b64 2719 007c  .k...r.d.|.d'..|
+00006e40: 233c 0074 167c 0583 0164 086b 0490 0372  #<.t.|...d.k...r
+00006e50: 2664 167c 1b64 2819 007c 233c 007c 0d64  &d.|.d(..|#<.|.d
+00006e60: 0b6b 0290 0372 3c64 167c 1b64 2819 007c  .k...r<d.|.d(..|
+00006e70: 233c 007c 0d64 066b 0290 0372 5264 027c  #<.|.d.k...rRd.|
+00006e80: 1b64 2819 007c 233c 0074 167c 0583 0164  .d(..|#<.t.|...d
+00006e90: 166b 0490 0372 8a7c 0e64 026b 0290 0372  .k...r.|.d.k...r
+00006ea0: 7c74 167c 0583 017c 1b64 2919 007c 233c  |t.|...|.d)..|#<
+00006eb0: 006e 0c7c 0e7c 1b64 2919 007c 233c 006e  .n.|.|.d)..|#<.n
+00006ec0: 287c 0e64 026b 0290 0372 a674 167c 0583  (|.d.k...r.t.|..
+00006ed0: 017c 1b64 2919 007c 233c 006e 0c7c 0e7c  .|.d)..|#<.n.|.|
+00006ee0: 1b64 2919 007c 233c 007c 1f64 026b 0490  .d)..|#<.|.d.k..
+00006ef0: 0172 d67c 1e7c 1f64 1618 0019 007c 1b64  .r.|.|.d.....|.d
+00006f00: 2a19 007c 233c 0090 0171 d674 116a 1e7c  *..|#<...q.t.j.|
+00006f10: 1b7c 1364 2b64 2c8d 0301 0064 0264 006c  .|.d+d,....d.d.l
+00006f20: 1f7d 2464 2d7c 246a 2064 2e3c 0064 2f7c  .}$d-|$j d.<.d/|
+00006f30: 246a 2064 303c 0064 317c 246a 2064 323c  $j d0<.d1|$j d2<
+00006f40: 0064 337c 246a 2064 343c 0064 317c 246a  .d3|$j d4<.d1|$j
+00006f50: 2064 353c 0064 337c 246a 2064 363c 0064   d5<.d3|$j d6<.d
+00006f60: 317c 246a 2064 373c 0064 317c 246a 2064  1|$j d7<.d1|$j d
+00006f70: 383c 007c 1164 066b 0290 0572 9064 39a0  8<.|.d.k...r.d9.
+00006f80: 087c 007c 03a1 027d 257c 0364 3a6b 0290  .|.|...}%|.d:k..
+00006f90: 0472 6864 3b7c 0017 0064 3c17 007d 2574  .rhd;|...d<..}%t
+00006fa0: 21a0 227c 25a1 017d 2664 3da0 087c 007c  !."|%..}&d=..|.|
+00006fb0: 03a1 027d 2564 3ea0 087c 007c 127c 03a1  ...}%d>..|.|.|..
+00006fc0: 037d 2774 0a6a 0ba0 237c 25a1 0190 0473  .}'t.j..#|%....s
+00006fd0: b274 0a6a 0ba0 237c 27a1 0190 0472 f67c  .t.j..#|'....r.|
+00006fe0: 1264 3f6b 0290 0472 f674 0574 066a 1764  .d?k...r.t.t.j.d
+00006ff0: 407c 259b 0064 419d 0317 0083 0101 007a  @|%..dA........z
+00007000: 1274 24a0 257c 25a1 0164 1619 007d 2857  .t$.%|%..d...}(W
+00007010: 006e 1a01 0001 0001 0074 24a0 257c 27a1  .n.......t$.%|'.
+00007020: 0164 1619 007d 2859 006e 0258 0074 0a6a  .d...}(Y.n.X.t.j
+00007030: 0ba0 237c 25a1 0190 0573 6274 0a6a 0ba0  ..#|%....sbt.j..
+00007040: 237c 27a1 0190 0573 627c 1264 3f6b 0290  #|'....sb|.d?k..
+00007050: 0572 6274 0574 066a 1764 427c 259b 0064  .rbt.t.j.dB|%..d
+00007060: 439d 0317 0083 0101 007c 026a 267c 0164  C........|.j&|.d
+00007070: 1f19 007c 1419 007c 0164 2019 007c 1419  ...|...|.d ..|..
+00007080: 0074 277c 1883 017c 127c 2764 0264 4485  .t'|...|.|'d.dD.
+00007090: 0219 0064 458d 0501 0074 0a6a 0ba0 237c  ...dE....t.j..#|
+000070a0: 27a1 0190 0672 1074 24a0 257c 27a1 0164  '....r.t$.%|'..d
+000070b0: 1619 007d 2874 0564 407c 279b 0064 419d  ...}(t.d@|'..dA.
+000070c0: 0383 0101 006e 8064 46a0 087c 007c 03a1  .....n.dF..|.|..
+000070d0: 027d 2574 0a6a 0ba0 237c 25a1 0190 0573  .}%t.j..#|%....s
+000070e0: ce74 0564 427c 259b 0064 439d 0383 0101  .t.dB|%..dC.....
+000070f0: 0074 287c 007c 017c 0364 0964 0964 478d  .t(|.|.|.d.d.dG.
+00007100: 0501 006e 1674 0574 066a 0764 487c 259b  ...n.t.t.j.dH|%.
+00007110: 0064 499d 0317 0083 0101 0074 24a0 2564  .dI........t$.%d
+00007120: 46a0 087c 007c 03a1 02a1 0164 0219 007d  F..|.|.....d...}
+00007130: 2874 21a0 2264 4aa0 087c 007c 03a1 02a1  (t!."dJ..|.|....
+00007140: 017d 2664 097d 187c 286a 2964 1619 007d  .}&d.}.|(j)d...}
+00007150: 1874 00a0 2a64 1664 1e64 1e64 1667 04a1  .t..*d.d.d.d.g..
+00007160: 017c 1814 0064 4b14 007c 1714 007d 2974  .|...dK..|...})t
+00007170: 216a 2b64 4c64 4d8d 0101 0074 216a 2c7c  !j+dLdM....t!j,|
+00007180: 267c 2964 4e8d 0201 0074 2d6a 2e64 4b7c  &|)dN....t-j.dK|
+00007190: 1814 0064 4b7c 1814 0067 027c 1764 4f7c  ...dK|...g.|.dO|
+000071a0: 161b 0064 5064 5164 5264 5364 5464 5464  ...dPdQdRdSdTdTd
+000071b0: 5564 5664 5764 1664 0064 588d 0e01 0074  UdVdWd.d.dX....t
+000071c0: 2fa0 307c 286a 31a1 017d 2a7c 0464 006b  /.0|(j1..}*|.d.k
+000071d0: 0890 0672 a264 0053 007c 2aa0 327c 0464  ...r.d.S.|*.2|.d
+000071e0: 1419 007c 0464 1519 0064 02a1 035c 027d  ...|.d...d...\.}
+000071f0: 2b7d 2c7c 2b7c 1714 007c 1864 4b14 007c  +},|+|...|.dK..|
+00007200: 1714 0018 0064 1e14 007d 2b7c 2c7c 1714  .....d...}+|,|..
+00007210: 007c 1864 4b14 007c 1714 0018 007d 2c7c  .|.dK..|.....},|
+00007220: 2b7c 286a 2964 1619 0064 5914 007c 1714  +|(j)d...dY..|..
+00007230: 006b 047c 2c7c 286a 2964 0219 0064 5914  .k.|,|(j)d...dY.
+00007240: 007c 1714 006b 0440 007c 2b64 4b7c 1714  .|...k.@.|+dK|..
+00007250: 007c 286a 2964 1619 0014 006b 0040 007c  .|(j)d.....k.@.|
+00007260: 2c64 4b7c 1714 007c 286a 2964 0219 0014  ,dK|...|(j)d....
+00007270: 006b 0040 007d 2d74 00a0 337c 2ca1 017d  .k.@.}-t..3|,..}
+00007280: 2e7c 0564 006b 0890 0872 9474 216a 347c  .|.d.k...r.t!j4|
+00007290: 2b7c 2d19 007c 2c7c 2d19 0064 3a64 5a64  +|-..|,|-..d:dZd
+000072a0: 5b64 5c8d 0501 0074 187c 2e7c 2d19 0083  [d\....t.|.|-...
+000072b0: 0144 005d ee5c 027d 1f7d 2f7c 0464 5d19  .D.].\.}.}/|.d].
+000072c0: 007c 2f19 0064 5ea0 087c 0464 2119 007c  .|/..d^..|.d!..|
+000072d0: 2f19 007c 2f7c 0464 5f19 007c 2f19 00a1  /..|/|.d_..|/...
+000072e0: 0317 007d 307c 2b7c 2e19 007c 2d19 007c  ...}0|+|...|-..|
+000072f0: 1f19 007c 0717 007d 317c 2c7c 2e19 007c  ...|...}1|,|...|
+00007300: 2d19 007c 1f19 007c 0817 007d 327c 1f64  -..|...|...}2|.d
+00007310: 026b 0290 0772 f674 216a 357c 317c 327c  .k...r.t!j5|1|2|
+00007320: 3064 6064 5764 618d 0501 006e 727c 2c7c  0d`dWda....nr|,|
+00007330: 2e19 007c 2d19 007c 1f64 1618 0019 007d  ...|-..|.d.....}
+00007340: 337c 327c 3318 0064 626b 0090 0872 207c  3|2|3..dbk...r |
+00007350: 327c 0937 007d 327c 1f64 166b 0490 0872  2|.7.}2|.d.k...r
+00007360: 547c 2c7c 2e19 007c 2d19 007c 1f64 0818  T|,|...|-..|.d..
+00007370: 0019 007d 347c 327c 3418 0064 636b 0090  ...}4|2|4..dck..
+00007380: 0872 547c 327c 0937 007d 3274 216a 357c  .rT|2|.7.}2t!j5|
+00007390: 317c 327c 3064 6064 5764 618d 0501 0090  1|2|0d`dWda.....
+000073a0: 0771 7c74 21a0 36a1 0001 0074 21a0 3764  .q|t!.6....t!.7d
+000073b0: 64a1 0101 0074 21a0 3864 65a1 0101 0074  d....t!.8de....t
+000073c0: 21a0 39a1 0001 0090 026e 6874 216a 347c  !.9......nht!j4|
+000073d0: 2b7c 0519 007c 2c7c 0519 0064 3a64 5a64  +|...|,|...d:dZd
+000073e0: 5b64 5c8d 0501 0074 187c 0583 0144 005d  [d\....t.|...D.]
+000073f0: b45c 027d 1f7d 2f7c 067c 1f19 007d 307c  .\.}.}/|.|...}0|
+00007400: 2b7c 2f19 007c 0717 007d 317c 2c7c 2f19  +|/..|...}1|,|/.
+00007410: 007c 0817 007d 327c 1f64 026b 0290 0972  .|...}2|.d.k...r
+00007420: 0074 216a 357c 317c 327c 3064 6064 5764  .t!j5|1|2|0d`dWd
+00007430: 618d 0501 006e 6a7c 2c7c 0519 007c 1f64  a....nj|,|...|.d
+00007440: 1618 0019 007d 337c 327c 3318 0064 626b  .....}3|2|3..dbk
+00007450: 0090 0972 267c 327c 0937 007d 327c 1f64  ...r&|2|.7.}2|.d
+00007460: 166b 0490 0972 567c 2c7c 0519 007c 1f64  .k...rV|,|...|.d
+00007470: 0818 0019 007d 347c 327c 3418 0064 636b  .....}4|2|4..dck
+00007480: 0090 0972 567c 327c 0937 007d 3274 216a  ...rV|2|.7.}2t!j
+00007490: 357c 317c 327c 3064 6064 5764 618d 0501  5|1|2|0d`dWda...
+000074a0: 0090 0871 b874 21a0 36a1 0001 0074 21a0  ...q.t!.6....t!.
+000074b0: 3764 64a1 0101 0074 21a0 3864 65a1 0101  7dd....t!.8de...
+000074c0: 007c 0a64 006b 0990 0972 b674 0564 66a0  .|.d.k...r.t.df.
+000074d0: 087c 00a1 0183 0101 0074 216a 3a64 67a0  .|.......t!j:dg.
+000074e0: 087c 00a1 0164 6864 698d 0201 007c 2aa0  .|...dhdi....|*.
+000074f0: 327c 0464 1419 0064 0219 007c 0464 1519  2|.d...d...|.d..
+00007500: 0064 0219 0064 02a1 035c 027d 2b7d 2c7c  .d...d...\.}+},|
+00007510: 1164 0b6b 0290 0972 f064 46a0 087c 007c  .d.k...r.dF..|.|
+00007520: 03a1 027d 256e 0c64 3da0 087c 007c 03a1  ...}%n.d=..|.|..
+00007530: 027d 2574 0574 066a 3b64 6a17 0083 0101  .}%t.t.j;dj.....
+00007540: 0074 0564 0e83 0101 0074 0564 6b83 0101  .t.d.....t.dk...
+00007550: 0074 0564 6c83 0101 0074 0564 6da0 087c  .t.dl....t.dm..|
+00007560: 25a1 0183 0101 0074 0564 6e83 0101 0074  %......t.dn....t
+00007570: 0564 6fa0 087c 0464 1419 0064 0219 007c  .do..|.d...d...|
+00007580: 0464 1519 0064 0219 00a1 0283 0101 0074  .d...d.........t
+00007590: 0564 70a0 087c 2b7c 17a1 0283 0101 0074  .dp..|+|.......t
+000075a0: 0564 71a0 087c 2c7c 17a1 0283 0101 0074  .dq..|,|.......t
+000075b0: 0564 7283 0101 0074 0564 6b83 0101 0074  .dr....t.dk....t
+000075c0: 0564 7383 0101 0074 0564 74a0 087c 00a1  .ds....t.dt..|..
+000075d0: 0183 0101 0074 0564 7583 0101 0074 0564  .....t.du....t.d
+000075e0: 7683 0101 0074 0564 7783 0101 0074 0564  v....t.dw....t.d
+000075f0: 6b83 0101 0074 0564 7883 0101 0074 0564  k....t.dx....t.d
+00007600: 7983 0101 0074 0564 0ca0 087c 16a1 0183  y....t.d...|....
+00007610: 0101 0074 0564 7a83 0101 0074 0564 7b83  ...t.dz....t.d{.
+00007620: 0101 0074 0564 7c83 0101 0074 0564 7d83  ...t.d|....t.d}.
+00007630: 0101 0064 0053 0029 7e4e 7241 0000 0072  ...d.S.)~NrA...r
+00007640: 0100 0000 7242 0000 0072 4300 0000 7244  ....rB...rC...rD
+00007650: 0000 0072 ce01 0000 7248 0000 0072 3900  ...r....rH...r9.
+00007660: 0000 7215 0200 007a 1953 696d 6261 6420  ..r....z.Simbad 
+00007670: 7363 616c 6520 7069 782f 6172 6373 6563  scale pix/arcsec
+00007680: 203a 7240 0000 007a 0c61 7263 5f6b 7063   :r@...z.arc_kpc
+00007690: 203d 207b 7d72 cf01 0000 72d0 0100 0072   = {}r....r....r
+000076a0: d101 0000 7204 0000 0072 6300 0000 72d2  ....r....rc...r.
+000076b0: 0100 0072 d501 0000 7261 0200 0072 6202  ...r....ra...rb.
+000076c0: 0000 7269 0000 0072 6302 0000 7a2c 7b7d  ..ri...rc...z,{}
+000076d0: 2061 6e64 207b 7d20 6973 203d 207b 3a2e   and {} is = {:.
+000076e0: 3166 7d5c 2c6b 7063 2028 7b3a 2e31 667d  1f}\,kpc ({:.1f}
+000076f0: 245c 6172 6373 6563 2429 72c7 0000 0072  $\arcsec$)r....r
+00007700: c200 0000 7a08 526f 7720 666f 7220 7a0c  ....z.Row for z.
+00007710: 2077 6173 2075 7064 6174 6564 7a16 526f   was updatedz.Ro
+00007720: 7720 7761 7320 6372 6561 7465 6420 666f  w was created fo
+00007730: 7220 7b7d 7262 0000 0072 4e00 0000 724f  r {}rb...rN...rO
+00007740: 0000 0072 5d02 0000 72c3 0000 00da 075a  ...r]...r......Z
+00007750: 5f56 414c 5545 72c5 0000 00da 0a6d 6f72  _VALUEr......mor
+00007760: 7068 5f74 7970 65da 0a4d 4f52 5048 5f54  ph_type..MORPH_T
+00007770: 5950 457a 0f49 7473 5f63 6f6e 7369 6465  YPEz.Its_conside
+00007780: 7265 643f 7a0a 4974 735f 6772 6f75 703f  red?z.Its_group?
+00007790: da08 4e6d 656d 6265 7273 da09 445f 746f  ..Nmembers..D_to
+000077a0: 5f6d 6169 6e54 7292 0000 0072 f701 0000  _mainTr....r....
+000077b0: 72f8 0100 0072 6101 0000 72f9 0100 0072  r....ra...r....r
+000077c0: fa01 0000 72fb 0100 0072 e701 0000 72fc  ....r....r....r.
+000077d0: 0100 0072 fd01 0000 72fe 0100 0072 ff01  ...r....r....r..
+000077e0: 0000 7200 0200 0072 e401 0000 723a 0000  ..r....r....r:..
+000077f0: 0072 d901 0000 72da 0100 0072 5900 0000  .r....r....rY...
+00007800: 725a 0000 0072 3c00 0000 725b 0000 0072  rZ...r<...r[...r
+00007810: 5c00 0000 725d 0000 0072 5e00 0000 725f  \...r]...r^...r_
+00007820: 0000 0072 6000 0000 724f 0200 0072 5a02  ...r`...rO...rZ.
+00007830: 0000 725b 0200 0072 5c02 0000 7209 0200  ..r[...r\...r...
+00007840: 0072 4900 0000 725e 0200 0072 7600 0000  .rI...r^...rv...
+00007850: 7210 0200 0072 cd01 0000 7a06 3130 206b  r....r....z.10 k
+00007860: 7063 da02 3132 726d 0100 0067 0000 0000  pc..12rm...g....
+00007870: 0000 2040 7232 0000 0067 3333 3333 3333  .. @r2...g333333
+00007880: f33f 7a02 772d 7274 0200 0029 0a72 7801  .?z.w-rt...).rx.
+00007890: 0000 726f 0100 0072 7001 0000 7271 0100  ..ro...rp...rq..
+000078a0: 0072 7201 0000 7273 0100 0072 7401 0000  .rr...rs...rt...
+000078b0: 7275 0100 0072 7601 0000 7277 0100 0072  ru...rv...rw...r
+000078c0: 6502 0000 7279 0100 0072 6602 0000 7267  e...ry...rf...rg
+000078d0: 0200 0072 7302 0000 7a1a 2056 7261 643d  ...rs...z. Vrad=
+000078e0: 7b3a 2e30 667d 2028 7b7d 2920 423d 7b3a  {:.0f} ({}) B={:
+000078f0: 2e31 667d da06 464c 5558 5f42 7259 0200  .1f}..FLUX_BrY..
+00007900: 0072 7502 0000 7206 0200 0072 7602 0000  .ru...r....rv...
+00007910: 727a 0100 0072 7b01 0000 7a1f 0a53 6176  rz...r{...z..Sav
+00007920: 696e 6720 6669 6775 7265 2069 6e20 696d  ing figure in im
+00007930: 6167 6573 2f7b 7d2e 706e 677a 0d69 6d61  ages/{}.pngz.ima
+00007940: 6765 732f 7b7d 2e70 6e67 727c 0000 0072  ges/{}.pngr|...r
+00007950: 7d00 0000 7a2a 0a49 6e20 6361 7365 2020  }...z*.In case  
+00007960: 746f 2061 6464 206d 616e 7561 6c6c 7920  to add manually 
+00007970: 7468 6520 636f 6f72 6469 6e61 7465 733a  the coordinates:
+00007980: da01 0a7a 1b66 726f 6d20 6173 7472 6f70  ...z.from astrop
+00007990: 792e 7763 7320 696d 706f 7274 2077 6373  y.wcs import wcs
+000079a0: 7a18 696d 6120 3d20 6669 7473 2e6f 7065  z.ima = fits.ope
+000079b0: 6e28 277b 7d27 295b 315d 7a18 7720 3d20  n('{}')[1]z.w = 
+000079c0: 2077 6373 2e57 4353 2869 6d61 2e68 6561   wcs.WCS(ima.hea
+000079d0: 6465 7229 7a27 636f 6f72 645f 6120 3d20  der)z'coord_a = 
+000079e0: 536b 7943 6f6f 7264 2827 7b7d 207b 7d27  SkyCoord('{} {}'
+000079f0: 2c20 756e 6974 3d75 2e64 6567 297a 2e63  , unit=u.deg)z.c
+00007a00: 6f6f 7264 5f62 203d 2077 2e61 6c6c 5f70  oord_b = w.all_p
+00007a10: 6978 3277 6f72 6c64 287b 7d20 2b20 6465  ix2world({} + de
+00007a20: 6c74 615f 7261 2f7b 7d2a 2d31 2c7a 2f20  lta_ra/{}*-1,z/ 
+00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a40: 2020 2020 2020 2020 207b 7d20 2b20 6465           {} + de
+00007a50: 6c74 615f 6465 632f 7b7d 2c20 3029 7a36  lta_dec/{}, 0)z6
+00007a60: 7072 696e 7420 2822 7b3a 2e37 667d 207b  print ("{:.7f} {
+00007a70: 3a2e 3766 7d22 2e66 6f72 6d61 7428 636f  :.7f}".format(co
+00007a80: 6f72 645f 625b 305d 2c20 636f 6f72 645f  ord_b[0], coord_
+00007a90: 625b 315d 2929 7a34 7461 625f 7072 6f3d  b[1]))z4tab_pro=
+00007aa0: 5461 626c 652e 7265 6164 2827 7072 6f70  Table.read('prop
+00007ab0: 6572 7469 6573 2e64 6174 272c 2066 6f72  erties.dat', for
+00007ac0: 6d61 743d 2761 7363 6969 2729 7a2d 696e  mat='ascii')z-in
+00007ad0: 645f 6720 3d20 6e70 2e77 6865 7265 2874  d_g = np.where(t
+00007ae0: 6162 5f70 726f 5b27 4741 4c27 5d3d 3d27  ab_pro['GAL']=='
+00007af0: 7b7d 4227 295b 305d 5b30 5d7a 2370 7269  {}B')[0][0]z#pri
+00007b00: 6e74 2028 2769 6e64 6578 206f 6620 6761  nt ('index of ga
+00007b10: 6c61 7879 203d 2027 2c20 696e 645f 6729  laxy = ', ind_g)
+00007b20: 7a21 7461 625f 7072 6f5b 2772 6127 5d5b  z!tab_pro['ra'][
+00007b30: 696e 645f 675d 203d 2063 6f6f 7264 5f62  ind_g] = coord_b
+00007b40: 5b30 5d7a 2274 6162 5f70 726f 5b27 6465  [0]z"tab_pro['de
+00007b50: 6327 5d5b 696e 645f 675d 203d 2063 6f6f  c'][ind_g] = coo
+00007b60: 7264 5f62 5b31 5d7a 3663 6f6f 7264 5f62  rd_b[1]z6coord_b
+00007b70: 203d 2053 6b79 436f 6f72 6428 636f 6f72   = SkyCoord(coor
+00007b80: 645f 625b 305d 2c20 636f 6f72 645f 625b  d_b[0], coord_b[
+00007b90: 315d 2c20 756e 6974 3d75 2e64 6567 297a  1], unit=u.deg)z
+00007ba0: 2173 6570 203d 2063 6f6f 7264 5f61 2e73  !sep = coord_a.s
+00007bb0: 6570 6172 6174 696f 6e28 636f 6f72 645f  eparation(coord_
+00007bc0: 6229 7a1c 7365 705f 6b70 6320 3d20 7365  b)z.sep_kpc = se
+00007bd0: 702e 6172 6373 6563 2a61 7263 5f6b 7063  p.arcsec*arc_kpc
+00007be0: 7a76 7072 696e 7420 2827 5365 7061 7261  zvprint ('Separa
+00007bf0: 7469 6f6e 2062 6574 7765 656e 2061 2053  tion between a S
+00007c00: 6563 6f6e 6461 7279 2061 6e64 2050 7269  econdary and Pri
+00007c10: 6d61 7279 2024 5c73 696d 2420 7b3a 2e31  mary $\sim$ {:.1
+00007c20: 667d 5c2c 6b70 6320 287b 3a2e 3166 7d24  f}\,kpc ({:.1f}$
+00007c30: 5c5c 6172 6373 6563 2429 272e 666f 726d  \\arcsec$)'.form
+00007c40: 6174 2873 6570 5f6b 7063 2c20 7365 702e  at(sep_kpc, sep.
+00007c50: 6172 6373 6563 2929 7a25 7461 625f 7072  arcsec))z%tab_pr
+00007c60: 6f5b 2744 5f74 6f5f 6d61 696e 275d 5b69  o['D_to_main'][i
+00007c70: 6e64 5f67 5d20 3d20 7365 705f 6b70 637a  nd_g] = sep_kpcz
+00007c80: 3f74 6162 5f70 726f 2e77 7269 7465 2827  ?tab_pro.write('
+00007c90: 7072 6f70 6572 7469 6573 2e64 6174 272c  properties.dat',
+00007ca0: 2066 6f72 6d61 743d 2761 7363 6969 272c   format='ascii',
+00007cb0: 206f 7665 7277 7269 7465 3d54 7275 6529   overwrite=True)
+00007cc0: 293c 7225 0000 0072 c800 0000 72b7 0000  )<r%...r....r...
+00007cd0: 0072 c900 0000 72ca 0000 0072 cb00 0000  .r....r....r....
+00007ce0: 7219 0000 0072 d200 0000 7264 0000 0072  r....r....rd...r
+00007cf0: cc00 0000 72d4 0000 0072 d500 0000 72de  ....r....r....r.
+00007d00: 0000 0072 df00 0000 72e0 0000 0072 0500  ...r....r....r..
+00007d10: 0000 72d9 0000 0072 0400 0000 7209 0000  ..r....r....r...
+00007d20: 0072 7a02 0000 7279 0200 0072 2402 0000  .rz...ry...r$...
+00007d30: 72e3 0000 0072 dd00 0000 72fb 0000 00da  r....r....r.....
+00007d40: 037a 6970 7288 0100 0072 8a01 0000 7289  .zipr....r....r.
+00007d50: 0100 0072 da00 0000 72dc 0000 0072 2502  ...r....r....r%.
+00007d60: 0000 7226 0200 0072 e600 0000 7222 0200  ..r&...r....r"..
+00007d70: 0072 d600 0000 7203 0000 0072 e400 0000  .r....r....r....
+00007d80: 72d7 0000 0072 d800 0000 7258 0200 0072  r....r....rX...r
+00007d90: ab01 0000 728b 0100 0072 e700 0000 72e8  ....r....r....r.
+00007da0: 0000 0072 b001 0000 72b1 0100 0072 0800  ...r....r....r..
+00007db0: 0000 727b 0200 0072 7c02 0000 727d 0200  ..r{...r|...r}..
+00007dc0: 0072 f900 0000 727e 0200 0072 2902 0000  .r....r~...r)...
+00007dd0: 722a 0200 0072 2d02 0000 722c 0200 0072  r*...r-...r,...r
+00007de0: ea00 0000 72e9 0000 00da 0547 5245 454e  ....r......GREEN
+00007df0: 2935 7241 0000 0072 ff00 0000 7200 0100  )5rA...r....r...
+00007e00: 0072 0101 0000 72ed 0100 0072 0401 0000  .r....r....r....
+00007e10: da09 7573 6572 5f74 6578 7472 ef01 0000  ..user_textr....
+00007e20: 72f0 0100 0072 f101 0000 72e9 0000 0072  r....r....r....r
+00007e30: ee01 0000 da0b 6974 7363 6f6e 7369 6465  ......itsconside
+00007e40: 72da 0869 7473 6772 6f75 7072 9e02 0000  r..itsgroupr....
+00007e50: 72f2 0100 0072 f301 0000 72f4 0100 0072  r....r....r....r
+00007e60: 0801 0000 72c0 0000 0072 0901 0000 72b3  ....r....r....r.
+00007e70: 0000 0072 0a01 0000 723e 0200 0072 0b01  ...r....r>...r..
+00007e80: 0000 7213 0100 0072 bf00 0000 72e5 0000  ..r....r....r...
+00007e90: 0072 8602 0000 7287 0200 0072 8802 0000  .r....r....r....
+00007ea0: 7233 0100 0072 8902 0000 da08 636f 6d70  r3...r......comp
+00007eb0: 5f69 6e64 da04 636f 6d70 7236 0100 0072  _ind..compr6...r
+00007ec0: 3802 0000 72d5 0000 00da 0669 6d61 706e  8...r......imapn
+00007ed0: 6772 0f01 0000 722e 0000 0072 0c02 0000  gr....r....r....
+00007ee0: 7274 0200 0072 8a02 0000 728b 0200 0072  rt...r....r....r
+00007ef0: 8d02 0000 7293 0200 0072 9402 0000 7295  ....r....r....r.
+00007f00: 0200 0072 9602 0000 7297 0200 0072 9802  ...r....r....r..
+00007f10: 0000 7299 0200 0072 2f00 0000 722f 0000  ..r....r/...r/..
+00007f20: 0072 3000 0000 7221 0200 00ba 0400 0073  .r0...r!.......s
+00007f30: ce01 0000 0006 1a02 1001 1801 0801 0602  ................
+00007f40: 1001 0a02 1002 0801 1402 0a01 0e01 0801  ................
+00007f50: 1401 0a01 02ff 0602 2201 2202 0601 0a03  ........".".....
+00007f60: 1a01 1602 0a02 1a01 0a01 0801 0600 0a00  ................
+00007f70: 0600 08ff 0c04 0801 1c02 0e01 0803 1201  ................
+00007f80: 1602 1c03 1401 0801 0401 0c02 1401 1401  ................
+00007f90: 1401 1401 1201 1401 0a01 0c01 0a01 0c01  ................
+00007fa0: 0e01 0c01 0a01 0c01 0a01 0c01 0e01 0a01  ................
+00007fb0: 1202 0e02 0a01 1202 0c01 0a01 1803 1003  ................
+00007fc0: 0801 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00007fd0: 0a03 0a03 0c01 0a01 0c02 0a03 0c01 0e01  ................
+00007fe0: 2601 1601 0201 1201 0601 1401 2601 1601  &...........&...
+00007ff0: 1e01 0201 0afe 0604 0e01 0e01 1203 0c01  ................
+00008000: 0e01 1001 0801 0200 02ff 0803 1602 0a01  ................
+00008010: 02ff 0401 02ff 0402 0a01 02ff 0602 0402  ................
+00008020: 0a01 1e02 0c02 0e01 1401 0600 0200 0200  ................
+00008030: 0200 0200 0201 0200 0200 0200 0200 0200  ................
+00008040: 02fe 0605 0c02 0a01 0402 1a02 1801 1402  ................
+00008050: 2a01 14ff 0201 14ff 0403 0a03 0a03 1401  *...............
+00008060: 02ff 0603 1401 0e01 0a00 0200 0aff 0603  ................
+00008070: 1401 1402 0a01 1603 1401 0e01 0801 0a01  ................
+00008080: 1401 0e01 0802 1802 0801 0a01 0a01 0c04  ................
+00008090: 1401 02ff 0604 1001 0802 0c01 0c02 0a01  ................
+000080a0: 1603 1001 0e01 0801 0a01 1001 0e01 0802  ................
+000080b0: 1802 0801 0a01 0a01 0a01 0e01 1402 2202  ..............".
+000080c0: 0a01 0e02 0c03 0e01 0801 0801 0801 0e01  ................
+000080d0: 0801 0601 0a00 0aff 0602 0801 02ff 0602  ................
+000080e0: 0801 02ff 0602 0802 0801 0801 0e01 0801  ................
+000080f0: 0801 0801 0801 0801 0801 0e01 0801 0802  ................
+00008100: 0801 7221 0200 0072 6c02 0000 630f 0000  ..r!...rl...c...
+00008110: 0000 0000 0000 0000 0036 0000 000e 0000  .........6......
+00008120: 0043 0000 0073 8207 0000 7400 a001 7c01  .C...s....t...|.
+00008130: 6401 1900 7c00 6b02 a101 6402 1900 6402  d...|.k...d...d.
+00008140: 1900 7d0f 7c01 6403 1900 7c0f 1900 7402  ..}.|.d...|...t.
+00008150: 1b00 7d10 7400 a003 7400 a004 6404 a101  ..}.t...t...d...
+00008160: a101 7c10 1400 6405 1400 7d11 6406 7d12  ..|...d...}.d.}.
+00008170: 7405 7406 6a07 6407 1700 8301 0100 7405  t.t.j.d.......t.
+00008180: 7406 6a07 6408 1700 8301 0100 7405 7406  t.j.d.......t.t.
+00008190: 6a08 6409 a009 7c01 640a 1900 7c0f 1900  j.d...|.d...|...
+000081a0: a101 1700 8301 0100 7405 7406 6a07 640b  ........t.t.j.d.
+000081b0: a009 7c10 a101 1700 8301 0100 7405 7406  ..|.........t.t.
+000081c0: 6a07 640c a009 7c11 a101 1700 8301 0100  j.d...|.........
+000081d0: 7c02 7c11 1b00 7c12 1b00 640d 1400 7d13  |.|...|...d...}.
+000081e0: 7c13 640e 1400 640f 1400 6410 1b00 7d14  |.d...d...d...}.
+000081f0: 7405 7406 6a07 6411 a009 7c13 a101 1700  t.t.j.d...|.....
+00008200: 8301 0100 7400 a00a 7c04 a101 7400 6a0b  ....t...|...t.j.
+00008210: 1400 7c11 640d 1300 1b00 6412 1b00 7d15  ..|.d.....d...}.
+00008220: 7405 7406 6a07 6413 a009 7c04 7c15 a102  t.t.j.d...|.|...
+00008230: 1700 8301 0100 740c 6a0d a00e 6414 a101  ......t.j...d...
+00008240: 9001 7332 740c a00f 6415 a101 0100 7405  ..s2t...d.....t.
+00008250: 7406 6a08 6416 1700 8301 0100 740c 6a0d  t.j.d.......t.j.
+00008260: a00e 6417 a101 9001 7358 740c a00f 6418  ..d.....sXt...d.
+00008270: a101 0100 7405 7406 6a08 6419 1700 8301  ....t.t.j.d.....
+00008280: 0100 7405 7406 6a10 641a 1700 8301 0100  ..t.t.j.d.......
+00008290: 7405 641b 8301 0100 641c 7d16 641d a009  t.d.....d.}.d...
+000082a0: 7c00 7c05 7c02 a103 7d17 740c 6a0d a00e  |.|.|...}.t.j...
+000082b0: 7c17 a101 9001 73e0 7405 641e 7c17 9b00  |.....s.t.d.|...
+000082c0: 641f 9d03 8301 0100 6420 a009 7c01 6421  d.......d ..|.d!
+000082d0: 1900 7c0f 1900 7c01 6422 1900 7c0f 1900  ..|...|.d"..|...
+000082e0: 7c05 7411 7c13 8301 a104 7d18 7c16 7c18  |.t.|.....}.|.|.
+000082f0: 1700 7d19 7405 7c19 8301 0100 7412 a013  ..}.t.|.....t...
+00008300: 7c19 7c17 a102 0100 6e10 7405 6423 7c17  |.|.....n.t.d#|.
+00008310: 9b00 6424 9d03 8301 0100 6425 7d16 6426  ..d$......d%}.d&
+00008320: a009 7c00 7c02 a102 7d17 740c 6a0d a00e  ..|.|...}.t.j...
+00008330: 7c17 a101 9002 7356 7405 6427 8301 0100  |.....sVt.d'....
+00008340: 6428 a009 7c01 6421 1900 7c0f 1900 7c01  d(..|.d!..|...|.
+00008350: 6422 1900 7c0f 1900 7411 7c13 8301 a103  d"..|...t.|.....
+00008360: 7d18 7c16 7c18 1700 7d19 7405 7c19 8301  }.|.|...}.t.|...
+00008370: 0100 7412 a013 7c19 7c17 a102 0100 6e10  ..t...|.|.....n.
+00008380: 7405 6423 7c17 9b00 6424 9d03 8301 0100  t.d#|...d$......
+00008390: 6426 a009 7c00 7c02 a102 7d1a 7414 a015  d&..|.|...}.t...
+000083a0: 7c1a a101 7d1b 7416 a017 641d a009 7c00  |...}.t...d...|.
+000083b0: 7c05 7c02 a103 a101 7d1c 7c1c 6402 1900  |.|.....}.|.d...
+000083c0: 6a18 7d1d 7411 7c13 8301 640e 1400 640f  j.}.t.|...d...d.
+000083d0: 1400 7c11 1400 7d1e 7414 6a19 6429 642a  ..|...}.t.j.d)d*
+000083e0: 8d01 7d1f 7414 6a1a 7c1b 7400 a01b 642b  ..}.t.j.|.t...d+
+000083f0: 642c 642b 642c 6704 a101 7c1e 1400 640e  d,d+d,g...|...d.
+00008400: 1400 642d 8d02 0100 7414 a01c a100 0100  ..d-....t.......
+00008410: 7414 a01d 642e a101 0100 7414 a01e 642f  t...d.....t...d/
+00008420: a101 0100 7414 a01f a100 0100 7c0a 6430  ....t.......|.d0
+00008430: 6b02 9003 7216 7414 a020 a100 0100 6e08  k...r.t.. ....n.
+00008440: 7414 a021 a100 0100 7405 6431 8301 0100  t..!....t.d1....
+00008450: 7405 7406 6a07 6432 1700 8301 0100 7405  t.t.j.d2......t.
+00008460: 6433 8301 0100 7405 6431 8301 0100 7422  d3....t.d1....t"
+00008470: 7c1d 7c0b 7c0c 7c0d 6434 8d04 7d20 7414  |.|.|.|.d4..} t.
+00008480: 6a19 6429 642a 8d01 7d1f 7414 6a1a 7c20  j.d)d*..}.t.j.| 
+00008490: 6435 6436 8d02 0100 7c0a 6430 6b02 9003  d5d6....|.d0k...
+000084a0: 7282 7414 a020 a100 0100 6e08 7414 a021  r.t.. ....n.t..!
+000084b0: a100 0100 7423 7c1d 6437 7c20 6438 8d03  ....t#|.d7| d8..
+000084c0: 5c03 7d21 7d22 7d23 7405 7406 6a07 6439  \.}!}"}#t.t.j.d9
+000084d0: 1700 8301 0100 7405 6433 8301 0100 7405  ......t.d3....t.
+000084e0: 643a a009 7c21 a101 8301 0100 7405 643b  d:..|!......t.d;
+000084f0: a009 7c22 a101 8301 0100 7405 643c a009  ..|"......t.d<..
+00008500: 7c23 a101 8301 0100 7405 643d a009 7c06  |#......t.d=..|.
+00008510: 6402 1900 7c06 642c 1900 a102 8301 0100  d...|.d,........
+00008520: 7405 6433 8301 0100 7424 8300 7d24 7425  t.d3....t$..}$t%
+00008530: 7c1d 7c06 643e 7c24 7c20 7c22 643f 8d06  |.|.d>|$| |"d?..
+00008540: 7d25 7c1d 7c25 6a26 3800 7d1d 7405 6440  }%|.|%j&8.}.t.d@
+00008550: 8301 0100 7414 6a19 6429 642a 8d01 7d1f  ....t.j.d)d*..}.
+00008560: 7414 6a1a 7c25 6a26 6435 6436 8d02 0100  t.j.|%j&d5d6....
+00008570: 7c0a 6430 6b02 9004 725a 7414 a020 a100  |.d0k...rZt.. ..
+00008580: 0100 6e08 7414 a021 a100 0100 7c08 7427  ..n.t..!....|.t'
+00008590: 1400 7d26 7428 7c26 6441 6441 6442 8d03  ..}&t(|&dAdAdB..
+000085a0: 7d27 7c27 a029 a100 0100 7411 7c15 8301  }'|'.)....t.|...
+000085b0: 7d28 742a 6a2b 7c1d 7c03 6443 8d02 7d29  }(t*j+|.|.dC..})
+000085c0: 742a a02c 7c1d 7c29 7c28 a103 7d2a 7c07  t*.,|.|)|(..}*|.
+000085d0: 6444 6b02 9005 720e 7405 6445 8301 0100  dDk...r.t.dE....
+000085e0: 7405 6446 8301 0100 7405 6447 8301 0100  t.dF....t.dG....
+000085f0: 7414 6a19 6429 642a 8d01 7d1f 7414 6a1a  t.j.d)d*..}.t.j.
+00008600: 7c2a 6435 6436 8d02 0100 742d 7c1d 7c2a  |*d5d6....t-|.|*
+00008610: 7c28 6448 6449 644a 8d05 7d2a 7c0a 6430  |(dHdIdJ..}*|.d0
+00008620: 6b02 9005 7206 7414 a020 a100 0100 6e08  k...r.t.. ....n.
+00008630: 7414 a021 a100 0100 7400 a02e 7c2a 6a2f  t..!....t...|*j/
+00008640: a101 7d2b 7405 644b 8301 0100 7405 7c2a  ..}+t.dK....t.|*
+00008650: 6a2f 8301 0100 7405 7400 a030 7431 7c2a  j/....t.t..0t1|*
+00008660: 6a2f 8301 a101 8301 0100 6402 6400 6c32  j/........d.d.l2
+00008670: 7d2c 644c 7c2c 6a33 644d 3c00 644e 7c2c  },dL|,j3dM<.dN|,
+00008680: 6a33 644f 3c00 6450 7c2c 6a33 6451 3c00  j3dO<.dP|,j3dQ<.
+00008690: 6452 7c2c 6a33 6453 3c00 6450 7c2c 6a33  dR|,j3dS<.dP|,j3
+000086a0: 6454 3c00 6452 7c2c 6a33 6455 3c00 6450  dT<.dR|,j3dU<.dP
+000086b0: 7c2c 6a33 6456 3c00 6450 7c2c 6a33 6457  |,j3dV<.dP|,j3dW
+000086c0: 3c00 7414 6a19 6458 642a 8d01 7d1f 7400  <.t.j.dXd*..}.t.
+000086d0: a034 7c2a 6a18 a101 a035 7436 a101 7d2d  .4|*j....5t6..}-
+000086e0: 7400 6a37 7c2d 7c2d 6459 6b02 3c00 7414  t.j7|-|-dYk.<.t.
+000086f0: 6a1a 7c2d 645a 645b 6435 645c 8d04 7d2e  j.|-dZd[d5d\..}.
+00008700: 7400 a030 7400 a038 7c2d a101 a101 4400  t..0t..8|-....D.
+00008710: 5d42 7d2f 7400 a001 7c2d 7c2f 642c 1700  ]B}/t...|-|/d,..
+00008720: 6b02 a101 7d30 7414 6a39 7c30 642c 1900  k...}0t.j9|0d,..
+00008730: 6402 1900 7c30 6402 1900 6402 1900 743a  d...|0d...d...t:
+00008740: 7411 7c2f 8301 8301 645d 645e 8d04 0100  t.|/....d]d^....
+00008750: 9005 71e6 7414 a03b 7c2e a101 7d31 7c31  ..q.t..;|...}1|1
+00008760: 6a3c a01f a100 0100 7414 a01f a100 0100  j<......t.......
+00008770: 7c0a 6430 6b02 9006 725a 7414 a020 a100  |.d0k...rZt.. ..
+00008780: 0100 6e08 7414 a021 a100 0100 7c09 645f  ..n.t..!....|.d_
+00008790: 6b02 9006 72c2 6460 7c00 9b00 6461 7c02  k...r.d`|...da|.
+000087a0: 9b00 6462 9d05 7d18 6463 7c03 9b00 6464  ..db..}.dc|...dd
+000087b0: 7c04 9b00 6465 7c05 9b00 6466 9d07 7d32  |...de|...df..}2
+000087c0: 6467 7c06 9b00 6468 7c07 9b00 6466 9d05  dg|...dh|...df..
+000087d0: 7d33 6469 7d34 7405 7c18 7c32 1700 7c33  }3di}4t.|.|2..|3
+000087e0: 1700 7c34 1700 8301 0100 6ebc 7411 7c2d  ..|4......n.t.|-
+000087f0: 7411 7c2d 6a3d 6402 1900 640e 1400 8301  t.|-j=d...d.....
+00008800: 7411 7c2d 6a3d 642c 1900 640e 1400 8301  t.|-j=d,..d.....
+00008810: 6602 1900 8301 642c 1800 7d35 6460 7c00  f.....d,..}5d`|.
+00008820: 9b00 6461 7c02 9b00 6462 9d05 7d18 6463  ..da|...db..}.dc
+00008830: 7c03 9b00 6464 7c04 9b00 6465 7c05 9b00  |...dd|...de|...
+00008840: 6466 9d07 7d32 6467 7c06 9b00 6468 7c07  df..}2dg|...dh|.
+00008850: 9b00 6466 9d05 7d33 646a 7c35 9b00 646b  ..df..}3dj|5..dk
+00008860: 7c05 9b00 646c 7c0e 9b02 646d 9d07 7d34  |...dl|...dm..}4
+00008870: 7405 7c18 7c32 1700 7c33 1700 7c34 1700  t.|.|2..|3..|4..
+00008880: 8301 0100 743e 7c00 7c01 7c02 7c03 7c04  ....t>|.|.|.|.|.
+00008890: 7c05 7c06 7c07 7c35 6701 7c05 6701 7c0a  |.|.|.|5g.|.g.|.
+000088a0: 7c0e 646e 8d0c 0100 6400 5300 296f 4e72  |.dn....d.S.)oNr
+000088b0: 4100 0000 7201 0000 0072 4200 0000 7243  A...r....rB...rC
+000088c0: 0000 0072 4400 0000 e748 e17a 14ae 47d1  ...rD....H.z..G.
+000088d0: 3f72 4500 0000 7246 0000 00fa 0a4a 636c  ?rE...rF.....Jcl
+000088e0: 6173 7320 7b7d 2072 c600 0000 72d8 0100  ass {} r....r...
+000088f0: 0072 4700 0000 7239 0000 0072 4900 0000  .rG...r9...rI...
+00008900: 7248 0000 0072 4a00 0000 724b 0000 0072  rH...rJ...rK...r
+00008910: 4c00 0000 724d 0000 0072 db01 0000 72dc  L...rM...r....r.
+00008920: 0100 0072 dd01 0000 72de 0100 0072 df01  ...r....r....r..
+00008930: 0000 72e0 0100 0072 5700 0000 7258 0000  ..r....rW...rX..
+00008940: 00fa 3068 7474 7073 3a2f 2f77 7777 2e6c  ..0https://www.l
+00008950: 6567 6163 7973 7572 7665 792e 6f72 672f  egacysurvey.org/
+00008960: 7669 6577 6572 2f66 6974 732d 6375 746f  viewer/fits-cuto
+00008970: 7574 3ffa 1c66 6974 735f 696d 6167 6573  ut?..fits_images
+00008980: 2f7b 7d5f 7b7d 5f7b 7d6b 7063 2e66 6974  /{}_{}_{}kpc.fit
+00008990: 7372 5d00 0000 725e 0000 007a 3572 613d  sr]...r^...z5ra=
+000089a0: 7b7d 2664 6563 3d7b 7d26 6c61 7965 723d  {}&dec={}&layer=
+000089b0: 6472 3826 7069 7873 6361 6c65 3d30 2e32  dr8&pixscale=0.2
+000089c0: 3726 6261 6e64 733d 7b7d 2673 697a 653d  7&bands={}&size=
+000089d0: 7b7d 724e 0000 0072 4f00 0000 725b 0000  {}rN...rO...r[..
+000089e0: 0072 5c00 0000 7a30 6874 7470 733a 2f2f  .r\...z0https://
+000089f0: 7777 772e 6c65 6761 6379 7375 7276 6579  www.legacysurvey
+00008a00: 2e6f 7267 2f76 6965 7765 722f 6a70 6567  .org/viewer/jpeg
+00008a10: 2d63 7574 6f75 743f 7a18 696d 6167 6573  -cutout?z.images
+00008a20: 2f66 6967 5f7b 7d5f 7b7d 6b70 632e 6a70  /fig_{}_{}kpc.jp
+00008a30: 6567 7a1c 0a44 6f77 6e6c 6f61 6469 6e67  egz..Downloading
+00008a40: 2074 6865 206a 7065 6720 6669 6c65 2e2e   the jpeg file..
+00008a50: 7a36 7261 3d7b 7d26 6465 633d 7b7d 266c  z6ra={}&dec={}&l
+00008a60: 6179 6572 3d64 7238 2670 6978 7363 616c  ayer=dr8&pixscal
+00008a70: 653d 302e 3237 2662 616e 6473 3d67 727a  e=0.27&bands=grz
+00008a80: 2673 697a 653d 7b7d 7274 0000 0072 7600  &size={}rt...rv.
+00008a90: 0000 7262 0000 0072 6900 0000 7210 0200  ..rb...ri...r...
+00008aa0: 0072 0d02 0000 720e 0200 0072 4000 0000  .r....r....r@...
+00008ab0: 726f 0000 0072 6d00 0000 726e 0000 0072  ro...rm...rn...r
+00008ac0: 7000 0000 7278 0000 0072 7900 0000 727f  p...rx...ry...r.
+00008ad0: 0000 0072 8000 0000 7283 0000 0072 8500  ...r....r....r..
+00008ae0: 0000 7286 0000 0072 8700 0000 7288 0000  ..r....r....r...
+00008af0: 0072 8a00 0000 728c 0000 0072 f501 0000  .r....r....r....
+00008b00: 728b 0000 0072 9800 0000 729b 0000 0072  r....r....r....r
+00008b10: 9c00 0000 729d 0000 0072 9e00 0000 729f  ....r....r....r.
+00008b20: 0000 0072 a000 0000 72a1 0000 0072 a200  ...r....r....r..
+00008b30: 0000 72f6 0100 0072 f701 0000 72f8 0100  ..r....r....r...
+00008b40: 0072 6101 0000 72f9 0100 0072 fa01 0000  .ra...r....r....
+00008b50: 72fb 0100 0072 e701 0000 72fc 0100 0072  r....r....r....r
+00008b60: fd01 0000 72fe 0100 0072 ff01 0000 7200  ....r....r....r.
+00008b70: 0200 0072 0102 0000 726b 0000 0072 0202  ...r....rk...r..
+00008b80: 0000 7203 0200 0072 0402 0000 7206 0200  ..r....r....r...
+00008b90: 0072 0702 0000 72ce 0100 007a 160a 0a53  .r....r....z...S
+00008ba0: 4c2e 7068 6f74 5f6d 6f64 5f64 6563 616c  L.phot_mod_decal
+00008bb0: 7328 277a 1727 2c20 7461 622c 2073 697a  s('z.', tab, siz
+00008bc0: 655f 696d 6167 655f 7068 793d 7216 0200  e_image_phy=r...
+00008bd0: 0072 1702 0000 7218 0200 007a 082c 2062  .r....r....z., b
+00008be0: 616e 643d 2272 1a02 0000 7a0a 736b 795f  and="r....z.sky_
+00008bf0: 626f 7820 3d20 7219 0200 007a 4075 7365  box = r....z@use
+00008c00: 725f 6f72 6465 723d 5b31 2c32 5d2c 2075  r_order=[1,2], u
+00008c10: 7365 725f 6c69 7374 3d5b 2241 222c 2242  ser_list=["A","B
+00008c20: 225d 2c20 6f75 7470 7574 6669 6c65 3d7b  "], outputfile={
+00008c30: 6f75 7470 7574 6669 6c65 3d7d 2972 1b02  outputfile=})r..
+00008c40: 0000 7a0f 5d2c 2075 7365 725f 6c69 7374  ..z.], user_list
+00008c50: 3d5b 227a 1a22 5d2c 206f 7574 7075 7466  =["z."], outputf
+00008c60: 696c 653d 6f75 7470 7574 6669 6c65 3dfa  ile=outputfile=.
+00008c70: 0129 290a 7201 0100 0072 0201 0000 7203  .)).r....r....r.
+00008c80: 0100 0072 0801 0000 7206 0100 0072 0701  ...r....r....r..
+00008c90: 0000 7204 0100 0072 0501 0000 72c1 0000  ..r....r....r...
+00008ca0: 0072 c000 0000 293f 7225 0000 0072 c800  .r....)?r%...r..
+00008cb0: 0000 72b7 0000 0072 c900 0000 72ca 0000  ..r....r....r...
+00008cc0: 0072 cb00 0000 7219 0000 0072 cc00 0000  .r....r....r....
+00008cd0: 72d2 0000 0072 6400 0000 72cd 0000 0072  r....rd...r....r
+00008ce0: ce00 0000 72d4 0000 0072 d500 0000 72d6  ....r....r....r.
+00008cf0: 0000 0072 1c02 0000 72dd 0000 0072 d800  ...r....r....r..
+00008d00: 0000 721a 0000 0072 1300 0000 72e6 0000  ..r....r....r...
+00008d10: 0072 2202 0000 7203 0000 0072 e400 0000  .r"...r....r....
+00008d20: 72e5 0000 0072 e700 0000 72e8 0000 0072  r....r....r....r
+00008d30: 8b01 0000 72c0 0100 0072 2c02 0000 722d  ....r....r,...r-
+00008d40: 0200 0072 2a02 0000 72ea 0000 0072 eb00  ...r*...r....r..
+00008d50: 0000 720a 0000 0072 0b00 0000 720d 0000  ..r....r....r...
+00008d60: 0072 0c00 0000 72ec 0000 0072 1100 0000  .r....r....r....
+00008d70: 7210 0000 0072 f200 0000 72f3 0000 0072  r....r....r....r
+00008d80: f400 0000 720e 0000 0072 0f00 0000 7223  ....r....r....r#
+00008d90: 0200 0072 fa00 0000 7224 0200 0072 e300  ...r....r$...r..
+00008da0: 0000 7225 0200 0072 2602 0000 7226 0000  ..r%...r&...r&..
+00008db0: 0072 8901 0000 7227 0200 0072 2700 0000  .r....r'...r'...
+00008dc0: 7228 0200 0072 2902 0000 72da 0000 0072  r(...r)...r....r
+00008dd0: b501 0000 72b7 0100 0072 ab01 0000 da0f  ....r....r......
+00008de0: 7068 6f74 5f6d 6f64 5f64 6563 616c 7329  phot_mod_decals)
+00008df0: 3672 4100 0000 72ff 0000 0072 0101 0000  6rA...r....r....
+00008e00: 7202 0100 0072 0301 0000 7208 0100 0072  r....r....r....r
+00008e10: 0601 0000 7207 0100 0072 ad00 0000 722f  ....r....r....r/
+00008e20: 0200 0072 c100 0000 7271 0000 0072 7200  ...r....rq...rr.
+00008e30: 0000 7273 0000 0072 c000 0000 7209 0100  ..rs...r....r...
+00008e40: 0072 b300 0000 720a 0100 0072 b901 0000  .r....r....r....
+00008e50: 720b 0100 0072 0c01 0000 720d 0100 00da  r....r....r.....
+00008e60: 0468 6f6d 6572 d500 0000 723f 0200 00da  .homer....r?....
+00008e70: 0474 6172 6772 3502 0000 7236 0200 0072  .targr5...r6...r
+00008e80: 1a01 0000 721b 0100 0072 3a02 0000 721d  ....r....r:...r.
+00008e90: 0100 0072 1c01 0000 721e 0100 0072 1f01  ...r....r....r..
+00008ea0: 0000 7220 0100 0072 8e00 0000 7221 0100  ..r ...r....r!..
+00008eb0: 0072 8100 0000 722a 0100 0072 2b01 0000  .r....r*...r+...
+00008ec0: 722c 0100 0072 2d01 0000 7237 0200 0072  r,...r-...r7...r
+00008ed0: 3802 0000 7239 0200 0072 3b02 0000 7233  8...r9...r;...r3
+00008ee0: 0100 0072 3c02 0000 72ca 0100 0072 4002  ...r<...r....r@.
+00008ef0: 0000 7241 0200 00da 0570 6172 7433 7242  ..rA.....part3rB
+00008f00: 0200 0072 2f00 0000 722f 0000 0072 3000  ...r/...r/...r0.
+00008f10: 0000 da12 6578 5f70 686f 745f 6d6f 645f  ....ex_phot_mod_
+00008f20: 6465 6361 6c73 d305 0000 735c 0100 0000  decals....s\....
+00008f30: 061a 0110 0118 0104 010e 010e 011c 0114  ................
+00008f40: 0114 0110 0210 0114 011c 010c 0102 ff08  ................
+00008f50: 030e 010a 010e 020e 010a 010e 020e 0108  ................
+00008f60: 0204 010e 010e 0110 0104 010a 000a 0002  ................
+00008f70: 0006 ff04 0208 0108 020e 0310 0204 010c  ................
+00008f80: 010e 0108 0104 010a 000a 0006 ff04 0208  ................
+00008f90: 0108 020e 0310 020c 010a 010c 0102 ff06  ................
+00008fa0: 020a 0214 010c 0124 0108 010a 010a 0108  .......$........
+00008fb0: 020a 010a 0208 0608 010e 0108 0108 0108  ................
+00008fc0: 0102 ff06 020c 010e 010a 010a 0208 0106  ................
+00008fd0: 0102 ff0c 020e 0108 010e 010e 010e 0206  ................
+00008fe0: 0106 0006 ff06 0208 0306 0108 0102 0002  ................
+00008ff0: 0102 fe06 040a 0208 010c 0110 010a 010a  ................
+00009000: 0208 0308 010e 0108 0308 010e 010e 020a  ................
+00009010: 0108 0108 0208 010c 010e 0108 0202 0002  ................
+00009020: fe06 030a 010a 0208 020c 0108 010a 0114  ................
+00009030: 0608 010a 010a 010a 010a 010a 010a 010a  ................
+00009040: 010a 050c 0112 010e 020a 0102 ff06 0314  ................
+00009050: 0112 012e 020a 010a 0108 010a 010a 0208  ................
+00009060: 020a 0212 0118 0112 0104 0116 0330 0212  .............0..
+00009070: 0118 0112 0118 0114 020a 0102 0002 0002  ................
+00009080: 0102 0004 0004 0102 0002 fd72 b402 0000  ...........r....
+00009090: 6310 0000 0000 0000 0000 0000 0044 0000  c............D..
+000090a0: 0012 0000 0043 0000 0073 4a08 0000 7400  .....C...sJ...t.
+000090b0: a001 7c01 6401 1900 7c00 6b02 a101 6402  ..|.d...|.k...d.
+000090c0: 1900 6402 1900 7d10 7c01 6403 1900 7c10  ..d...}.|.d...|.
+000090d0: 1900 7402 1b00 7d11 7400 a003 7400 a004  ..t...}.t...t...
+000090e0: 6404 a101 a101 7c11 1400 6405 1400 7d12  d.....|...d...}.
+000090f0: 7405 7406 6a07 6406 1700 8301 0100 7405  t.t.j.d.......t.
+00009100: 7406 6a07 6407 1700 8301 0100 7405 7406  t.j.d.......t.t.
+00009110: 6a08 6408 a009 7c01 6409 1900 7c10 1900  j.d...|.d...|...
+00009120: a101 1700 8301 0100 7405 7406 6a07 640a  ........t.t.j.d.
+00009130: a009 7c12 a101 1700 8301 0100 7c02 7c12  ..|.........|.|.
+00009140: 1b00 640b 1b00 640c 1400 7d13 7c13 640d  ..d...d...}.|.d.
+00009150: 1400 640b 1400 640e 1b00 7d14 7405 7406  ..d...d...}.t.t.
+00009160: 6a07 640f a009 7c13 a101 1700 8301 0100  j.d...|.........
+00009170: 7400 a00a 7c04 a101 7400 6a0b 1400 7c12  t...|...t.j...|.
+00009180: 640c 1300 1b00 6410 1b00 7d15 6411 a009  d.....d...}.d...
+00009190: 7c04 7c15 a102 7d16 7405 7406 6a07 7c16  |.|...}.t.t.j.|.
+000091a0: 1700 8301 0100 7405 7406 6a0c 6412 1700  ......t.t.j.d...
+000091b0: 8301 0100 7405 6413 8301 0100 6414 7d17  ....t.d.....d.}.
+000091c0: 7c01 6415 7c05 1700 1900 7c10 1900 7d18  |.d.|.....|...}.
+000091d0: 7405 6416 a009 7c17 a101 8301 0100 7405  t.d...|.......t.
+000091e0: 6417 a009 7c18 a101 8301 0100 6418 7d19  d...|.......d.}.
+000091f0: 6419 7d1a 641a 7d1b 7400 a00a 7c19 a101  d.}.d.}.t...|...
+00009200: 7d1c 6419 7d1d 641b 7c01 6401 1900 7c10  }.d.}.d.|.d...|.
+00009210: 1900 1700 641c a009 7c05 7c02 a102 1700  ....d...|.|.....
+00009220: 7d1e 740d a00e 7c1e a101 7d1f 7c1f 6402  }.t...|...}.|.d.
+00009230: 1900 6a0f 7d20 7405 7406 6a07 641d 1700  ..j.} t.t.j.d...
+00009240: 8301 0100 7405 641e 8301 0100 7405 641f  ....t.d.....t.d.
+00009250: 8301 0100 7410 7c20 7c0b 7c0c 7c0d 6420  ....t.| |.|.|.d 
+00009260: 8d04 7d21 7411 6a12 6421 6422 8d01 7d22  ..}!t.j.d!d"..}"
+00009270: 7411 6a13 7c21 6423 6424 8d02 0100 7411  t.j.|!d#d$....t.
+00009280: 6a14 6425 7c00 1700 6426 a009 7c05 7c02  j.d%|...d&..|.|.
+00009290: a102 1700 6427 6428 8d02 0100 7c0a 6429  ....d'd(....|.d)
+000092a0: 6b02 9002 7202 7411 a015 a100 0100 6e08  k...r.t.......n.
+000092b0: 7411 a016 a100 0100 7417 7c20 642a 7c21  t.......t.| d*|!
+000092c0: 642b 8d03 5c03 7d23 7d24 7d25 7405 7406  d+..\.}#}$}%t.t.
+000092d0: 6a07 642c 1700 8301 0100 7405 642d 8301  j.d,......t.d-..
+000092e0: 0100 7405 642e a009 7c23 a101 8301 0100  ..t.d...|#......
+000092f0: 7405 642f a009 7c24 a101 8301 0100 7405  t.d/..|$......t.
+00009300: 6430 a009 7c25 a101 8301 0100 7405 6431  d0..|%......t.d1
+00009310: a009 7c08 6402 1900 7c08 6419 1900 a102  ..|.d...|.d.....
+00009320: 8301 0100 7405 6432 8301 0100 7418 8300  ....t.d2....t...
+00009330: 7d26 7419 7c20 7c08 6433 7c26 7c21 7c24  }&t.| |.d3|&|!|$
+00009340: 6434 8d06 7d27 7c20 7c27 6a1a 1800 7d20  d4..}'| |'j...} 
+00009350: 7411 6a12 6421 6422 8d01 7d22 7411 6a13  t.j.d!d"..}"t.j.
+00009360: 7c27 6a1a 6423 6424 8d02 0100 7411 6a14  |'j.d#d$....t.j.
+00009370: 6425 7c00 1700 6435 a009 7c05 7c02 a102  d%|...d5..|.|...
+00009380: 1700 6427 6428 8d02 0100 7c0a 6429 6b02  ..d'd(....|.d)k.
+00009390: 9002 72f0 7411 a015 a100 0100 6e08 7411  ..r.t.......n.t.
+000093a0: a016 a100 0100 7c01 6401 1900 7c10 1900  ......|.d...|...
+000093b0: 6436 a009 7c05 7c02 a102 1700 7d28 740d  d6..|.|.....}(t.
+000093c0: 6a1b 641b 7c28 1700 6437 1700 7c27 6a1a  j.d.|(..d7..|'j.
+000093d0: 6438 6439 8d03 0100 740d 6a1b 641b 7c28  d8d9....t.j.d.|(
+000093e0: 1700 643a 1700 7c20 6438 6439 8d03 0100  ..d:..| d8d9....
+000093f0: 7405 643b 7c28 1700 643c 1700 8301 0100  t.d;|(..d<......
+00009400: 741c 7c20 7c1b 7c1c 7c1d 7c17 8305 7d29  t.| |.|.|.|...})
+00009410: 7400 a01d 7400 a01e 640c a101 640c 1400  t...t...d...d...
+00009420: a101 640c 1400 7d2a 643d 7d2b 7c18 7c2a  ..d...}*d=}+|.|*
+00009430: 1b00 7d2c 7400 6a1f 7c2b 0b00 7c2b 6419  ..},t.j.|+..|+d.
+00009440: 1700 8502 7c2b 0b00 7c2b 6419 1700 8502  ....|+..|+d.....
+00009450: 6602 1900 5c02 7d2d 7d2e 7400 a020 7c2e  f...\.}-}.t.. |.
+00009460: 640c 1300 7c2d 640c 1300 1700 0b00 643e  d...|-d.......d>
+00009470: 7c2c 640c 1300 1400 1b00 a101 7d2f 7c2f  |,d.........}/|/
+00009480: 7400 a021 7c2f a101 1d00 7d2f 7c18 7422  t..!|/....}/|.t"
+00009490: 1400 7d30 7423 7c30 643f 643f 6440 8d03  ..}0t#|0d?d?d@..
+000094a0: 7d31 7c31 a024 a100 0100 7425 7c15 8301  }1|1.$....t%|...
+000094b0: 7d32 7426 6a27 7c20 7c03 6441 8d02 7d33  }2t&j'| |.dA..}3
+000094c0: 7426 a028 7c20 7c33 7c32 a103 7d34 7c09  t&.(| |3|2..}4|.
+000094d0: 6442 6b02 9004 728a 7405 6443 8301 0100  dBk...r.t.dC....
+000094e0: 7405 6444 8301 0100 7405 6445 8301 0100  t.dD....t.dE....
+000094f0: 7411 6a12 6421 6422 8d01 0100 7411 6a13  t.j.d!d"....t.j.
+00009500: 7c34 6423 6424 8d02 0100 7c0a 6429 6b02  |4d#d$....|.d)k.
+00009510: 9004 7270 7411 a015 a100 0100 6e08 7411  ..rpt.......n.t.
+00009520: a016 a100 0100 7429 7c20 7c34 7c32 6446  ......t)| |4|2dF
+00009530: 6447 6448 8d05 7d34 7405 6449 8301 0100  dGdH..}4t.dI....
+00009540: 7405 644a 8301 0100 7411 6a12 644b 6422  t.dJ....t.j.dKd"
+00009550: 8d01 7d22 7400 a02a 7c34 6a0f a101 a02b  ..}"t..*|4j....+
+00009560: 742c a101 7d35 7400 6a2d 7c35 7c35 641a  t,..}5t.j-|5|5d.
+00009570: 6b02 3c00 7411 6a13 7c35 644c 644d 6423  k.<.t.j.|5dLdMd#
+00009580: 644e 8d04 7d36 7400 a02e 7400 a02f 7c35  dN..}6t...t../|5
+00009590: a101 a101 4400 5d42 7d37 7400 a001 7c35  ....D.]B}7t...|5
+000095a0: 7c37 6419 1700 6b02 a101 7d38 7411 6a30  |7d...k...}8t.j0
+000095b0: 7c38 6419 1900 6402 1900 7c38 6402 1900  |8d...d...|8d...
+000095c0: 6402 1900 7431 7425 7c37 8301 8301 644f  d...t1t%|7....dO
+000095d0: 6450 8d04 0100 9004 71e8 7411 a032 7c36  dP......q.t..2|6
+000095e0: a101 7d39 7c39 6a33 a034 a100 0100 7411  ..}9|9j3.4....t.
+000095f0: a034 a100 0100 6425 7c01 6401 1900 7c10  .4....d%|.d...|.
+00009600: 1900 1700 6451 a009 7c05 7c02 a102 1700  ....dQ..|.|.....
+00009610: 7d3a 7411 6a14 7c3a 6427 6428 8d02 0100  }:t.j.|:d'd(....
+00009620: 7c0a 6429 6b02 9005 7286 7411 a015 a100  |.d)k...r.t.....
+00009630: 0100 6e08 7411 a016 a100 0100 7405 7406  ..n.t.......t.t.
+00009640: 6a08 6452 1700 8301 0100 7405 6453 8301  j.dR......t.dS..
+00009650: 0100 7435 a035 a100 7d3b 7436 6a37 7c20  ..t5.5..};t6j7| 
+00009660: 7c34 6a0f 7c1a 7c2f 7c0f 6454 8d05 7d3c  |4j.|.|/|.dT..}<
+00009670: 7405 6455 7435 a035 a100 7c3b 1800 1600  t.dUt5.5..|;....
+00009680: 8301 0100 7405 7438 7c3c 8301 8301 0100  ....t.t8|<......
+00009690: 6456 6457 6458 6459 645a 645b 645c 645d  dVdWdXdYdZd[d\d]
+000096a0: 645e 645f 6460 6461 6462 6463 670e 7d3d  d^d_d`dadbdcg.}=
+000096b0: 7405 6464 8301 0100 7405 6465 8301 0100  t.dd....t.de....
+000096c0: 7c06 6400 6b08 9007 723a 7400 a039 7c34  |.d.k...r:t..9|4
+000096d0: 6a3a a101 7d3e 743b 7c3e 6400 6400 6466  j:..}>t;|>d.d.df
+000096e0: 8503 1900 8301 4400 5dfa 5c02 7d37 7d3f  ......D.].\.}7}?
+000096f0: 7c3c 7c3f 1900 7d40 743c 7c40 7c00 7c3d  |<|?..}@t<|@|.|=
+00009700: 7c37 1900 1700 7c20 7c29 7c1b 7c1c 7c1d  |7....| |)|.|.|.
+00009710: 7c17 7c2f 7c18 7c19 7c12 7c02 7c0a 7c0e  |.|/|.|.|.|.|.|.
+00009720: 6467 8d0f 0100 743d a03e 7c0e a101 7d41  dg....t=.>|...}A
+00009730: 7400 a001 7c41 6468 1900 7c00 7c3d 7c37  t...|Adh..|.|=|7
+00009740: 1900 1700 6b02 a101 6402 1900 6402 1900  ....k...d...d...
+00009750: 7d42 7400 a001 7c01 6401 1900 7c00 6b02  }Bt...|.d...|.k.
+00009760: a101 6402 1900 6402 1900 7d43 7c01 6469  ..d...d...}C|.di
+00009770: 1900 7c43 1900 7c41 6469 1900 7c42 3c00  ..|C..|Adi..|B<.
+00009780: 7c01 646a 1900 7c43 1900 7c41 646a 1900  |.dj..|C..|Adj..
+00009790: 7c42 3c00 7c01 6403 1900 7c43 1900 7c41  |B<.|.d...|C..|A
+000097a0: 646b 1900 7c42 3c00 7c01 646c 1900 7c43  dk..|B<.|.dl..|C
+000097b0: 1900 7c41 646c 1900 7c42 3c00 7c01 6409  ..|Adl..|B<.|.d.
+000097c0: 1900 7c43 1900 7c41 6409 1900 7c42 3c00  ..|C..|Ad...|B<.
+000097d0: 743d 6a3f 7c41 7c0e 6438 6439 8d03 0100  t=j?|A|.d8d9....
+000097e0: 9006 713a 9001 6e04 743b 7c06 8301 4400  ..q:..n.t;|...D.
+000097f0: 5dfa 5c02 7d37 7d3f 7c3c 7c3f 1900 7d40  ].\.}7}?|<|?..}@
+00009800: 743c 7c40 7c00 7c07 7c37 1900 1700 7c20  t<|@|.|.|7....| 
+00009810: 7c29 7c1b 7c1c 7c1d 7c17 7c2f 7c18 7c19  |)|.|.|.|.|/|.|.
+00009820: 7c12 7c02 7c0a 7c0e 6467 8d0f 0100 743d  |.|.|.|.dg....t=
+00009830: a03e 7c0e a101 7d41 7400 a001 7c41 6468  .>|...}At...|Adh
+00009840: 1900 7c00 7c07 7c37 1900 1700 6b02 a101  ..|.|.|7....k...
+00009850: 6402 1900 6402 1900 7d42 7400 a001 7c01  d...d...}Bt...|.
+00009860: 6401 1900 7c00 6b02 a101 6402 1900 6402  d...|.k...d...d.
+00009870: 1900 7d43 7c01 6469 1900 7c43 1900 7c41  ..}C|.di..|C..|A
+00009880: 6469 1900 7c42 3c00 7c01 646a 1900 7c43  di..|B<.|.dj..|C
+00009890: 1900 7c41 646a 1900 7c42 3c00 7c01 6403  ..|Adj..|B<.|.d.
+000098a0: 1900 7c43 1900 7c41 646b 1900 7c42 3c00  ..|C..|Adk..|B<.
+000098b0: 7c01 646c 1900 7c43 1900 7c41 646c 1900  |.dl..|C..|Adl..
+000098c0: 7c42 3c00 7c01 6409 1900 7c43 1900 7c41  |B<.|.d...|C..|A
+000098d0: 6409 1900 7c42 3c00 743d 6a3f 7c41 7c0e  d...|B<.t=j?|A|.
+000098e0: 6438 6439 8d03 0100 9007 7142 7411 a015  d8d9......qBt...
+000098f0: a100 0100 6400 5300 296d 4e72 4100 0000  ....d.S.)mNrA...
+00009900: 7201 0000 0072 4200 0000 7243 0000 0072  r....rB...rC...r
+00009910: 4400 0000 7245 0000 0072 4600 0000 72ac  D...rE...rF...r.
+00009920: 0200 0072 c600 0000 7247 0000 0072 4800  ...r....rG...rH.
+00009930: 0000 7239 0000 0072 4900 0000 724a 0000  ..r9...rI...rJ..
+00009940: 0072 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
+00009950: 7265 0000 0072 6600 0000 e700 0000 0000  re...rf.........
+00009960: 8036 40da 0870 7366 7369 7a65 5f7a 0a0a  .6@..psfsize_z..
+00009970: 5a50 3a7b 3a2e 3166 7d72 6a00 0000 72ab  ZP:{:.1f}rj...r.
+00009980: 0200 0072 6900 0000 726b 0000 0072 6c00  ...ri...rk...rl.
+00009990: 0000 7a0e 5f7b 7d5f 7b7d 6b70 632e 6669  ..z._{}_{}kpc.fi
+000099a0: 7473 726d 0000 0072 6e00 0000 726f 0000  tsrm...rn...ro..
+000099b0: 0072 7000 0000 7274 0000 0072 7600 0000  .rp...rt...rv...
+000099c0: 7278 0000 0072 7900 0000 727b 0000 007a  rx...ry...r{...z
+000099d0: 157b 7d5f 7b7d 6b70 635f 736b 795f 6d61  .{}_{}kpc_sky_ma
+000099e0: 736b 2e70 6e67 727c 0000 0072 7d00 0000  sk.pngr|...r}...
+000099f0: 7240 0000 0072 7f00 0000 7280 0000 0072  r@...r....r....r
+00009a00: 8300 0000 7284 0000 0072 8500 0000 7286  ....r....r....r.
+00009a10: 0000 0072 8700 0000 7288 0000 0072 8900  ...r....r....r..
+00009a20: 0000 728a 0000 0072 8c00 0000 7a11 5f7b  ..r....r....z._{
+00009a30: 7d5f 7b7d 6b70 635f 736b 792e 706e 677a  }_{}kpc_sky.pngz
+00009a40: 095f 7b7d 5f7b 7d6b 7063 7291 0000 0054  ._{}_{}kpcr....T
+00009a50: 7292 0000 0072 9400 0000 7295 0000 0072  r....r....r....r
+00009a60: 9600 0000 7297 0000 0072 3800 0000 728b  ....r....r8...r.
+00009a70: 0000 0072 9800 0000 729b 0000 0072 9c00  ...r....r....r..
+00009a80: 0000 729d 0000 0072 9e00 0000 729f 0000  ..r....r....r...
+00009a90: 0072 a000 0000 72a1 0000 0072 a200 0000  .r....r....r....
+00009aa0: 72a5 0000 0072 a600 0000 7201 0200 0072  r....r....r....r
+00009ab0: 0202 0000 7203 0200 0072 0402 0000 7206  ....r....r....r.
+00009ac0: 0200 0072 0702 0000 7a12 5f7b 7d5f 7b7d  ...r....z._{}_{}
+00009ad0: 6b70 635f 7365 676d 2e70 6e67 72a9 0000  kpc_segm.pngr...
+00009ae0: 0072 aa00 0000 72ab 0000 0072 af00 0000  .r....r....r....
+00009af0: 72b0 0000 0072 b100 0000 72b2 0000 0072  r....r....r....r
+00009b00: b300 0000 72b4 0000 0072 b500 0000 72b6  ....r....r....r.
+00009b10: 0000 0072 b700 0000 7234 0000 0072 b800  ...r....r4...r..
+00009b20: 0000 72b9 0000 0072 ba00 0000 72bb 0000  ..r....r....r...
+00009b30: 0072 bc00 0000 72bd 0000 0072 be00 0000  .r....r....r....
+00009b40: 7262 0000 0029 0272 c100 0000 72c0 0000  rb...).r....r...
+00009b50: 0072 c200 0000 724e 0000 0072 4f00 0000  .r....rN...rO...
+00009b60: 72c3 0000 0072 c500 0000 2940 7225 0000  r....r....)@r%..
+00009b70: 0072 c800 0000 72b7 0000 0072 c900 0000  .r....r....r....
+00009b80: 72ca 0000 0072 cb00 0000 7219 0000 0072  r....r....r....r
+00009b90: cc00 0000 72d2 0000 0072 6400 0000 72cd  ....r....rd...r.
+00009ba0: 0000 0072 ce00 0000 72dd 0000 0072 0300  ...r....r....r..
+00009bb0: 0000 72e4 0000 0072 e500 0000 720a 0000  ..r....r....r...
+00009bc0: 0072 e600 0000 72e7 0000 0072 e800 0000  .r....r....r....
+00009bd0: 72e9 0000 0072 ea00 0000 72eb 0000 0072  r....r....r....r
+00009be0: 0b00 0000 720d 0000 0072 0c00 0000 72ec  ....r....r....r.
+00009bf0: 0000 0072 ed00 0000 7231 0000 0072 ee00  ...r....r1...r..
+00009c00: 0000 7233 0000 0072 ef00 0000 72f0 0000  ..r3...r....r...
+00009c10: 0072 f100 0000 7211 0000 0072 1000 0000  .r....r....r....
+00009c20: 72f2 0000 0072 d800 0000 72f3 0000 0072  r....r....r....r
+00009c30: f400 0000 720e 0000 0072 0f00 0000 7226  ....r....r....r&
+00009c40: 0000 0072 8901 0000 7227 0200 0072 2700  ...r....r'...r'.
+00009c50: 0000 7224 0200 0072 2802 0000 7229 0200  ..r$...r(...r)..
+00009c60: 0072 da00 0000 72b5 0100 0072 b701 0000  .r....r....r....
+00009c70: 722a 0200 0072 f500 0000 72f6 0000 0072  r*...r....r....r
+00009c80: f700 0000 72e3 0000 0072 f900 0000 72fa  ....r....r....r.
+00009c90: 0000 0072 fb00 0000 72fc 0000 0072 0400  ...r....r....r..
+00009ca0: 0000 72d9 0000 0072 dc00 0000 2944 7241  ..r....r....)DrA
+00009cb0: 0000 0072 ff00 0000 7201 0100 0072 0201  ...r....r....r..
+00009cc0: 0000 7203 0100 0072 0801 0000 7204 0100  ..r....r....r...
+00009cd0: 0072 0501 0000 7206 0100 0072 0701 0000  .r....r....r....
+00009ce0: 72c1 0000 0072 7100 0000 7272 0000 0072  r....rq...rr...r
+00009cf0: 7300 0000 72c0 0000 0072 ae00 0000 7209  s...r....r....r.
+00009d00: 0100 0072 b300 0000 720a 0100 0072 0b01  ...r....r....r..
+00009d10: 0000 720c 0100 0072 0d01 0000 da05 7465  ..r....r......te
+00009d20: 7874 7472 2d00 0000 7216 0100 0072 1701  xttr-...r....r..
+00009d30: 0000 72ac 0000 0072 1801 0000 722b 0000  ..r....r....r+..
+00009d40: 0072 2c00 0000 720f 0100 0072 1a01 0000  .r,...r....r....
+00009d50: 721b 0100 0072 1c01 0000 721d 0100 0072  r....r....r....r
+00009d60: 1e01 0000 721f 0100 0072 2001 0000 728e  ....r....r ...r.
+00009d70: 0000 0072 2101 0000 7222 0100 0072 2301  ...r!...r"...r#.
+00009d80: 0000 7224 0100 0072 2501 0000 7226 0100  ..r$...r%...r&..
+00009d90: 0072 2701 0000 7228 0100 0072 2901 0000  .r'...r(...r)...
+00009da0: 7281 0000 0072 2a01 0000 722b 0100 0072  r....r*...r+...r
+00009db0: 2c01 0000 722d 0100 0072 3902 0000 723b  ,...r-...r9...r;
+00009dc0: 0200 0072 3301 0000 723c 0200 0072 ca01  ...r3...r<...r..
+00009dd0: 0000 722e 0100 0072 2f01 0000 7230 0100  ..r....r/...r0..
+00009de0: 0072 3101 0000 7232 0100 0072 3401 0000  .r1...r2...r4...
+00009df0: 7235 0100 0072 e500 0000 7236 0100 0072  r5...r....r6...r
+00009e00: 3701 0000 722f 0000 0072 2f00 0000 7230  7...r/...r/...r0
+00009e10: 0000 0072 b002 0000 a906 0000 7382 0100  ...r........s...
+00009e20: 0000 061a 0110 0118 010e 010e 011c 0114  ................
+00009e30: 0110 0110 0114 011c 0106 0102 ff04 020e  ................
+00009e40: 020e 0108 0304 0110 020e 010e 0204 0104  ................
+00009e50: 0104 010a 0104 0512 0102 0002 ff06 020a  ................
+00009e60: 010a 050e 0108 0108 0108 0102 ff06 020c  ................
+00009e70: 010e 0110 0102 ff04 0102 ff06 020a 010a  ................
+00009e80: 0208 0306 0102 ff0c 020e 0108 010e 010e  ................
+00009e90: 010e 0306 0106 0006 ff06 0208 0206 0108  ................
+00009ea0: 0102 0002 0102 fe06 040a 020c 0110 0110  ................
+00009eb0: 0102 ff04 0102 ff06 020a 010a 0208 0218  ................
+00009ec0: 0112 0102 ff06 0210 0102 ff06 0210 0310  ................
+00009ed0: 0618 0104 0108 0126 0124 010e 0508 010e  .......&.$......
+00009ee0: 0108 0208 010e 010e 020a 0108 0108 0208  ................
+00009ef0: 010c 010e 010a 010a 0208 0108 0202 0002  ................
+00009f00: fe06 0408 0108 020c 0112 010e 020a 0102  ................
+00009f10: ff06 0214 0112 012e 020a 010a 0108 0112  ................
+00009f20: 0102 0002 ff06 020e 010a 010a 0208 020e  ................
+00009f30: 0108 0208 0106 0104 0002 0002 0002 ff06  ................
+00009f40: 0214 010c 0220 0208 0108 020a 010c 011a  ..... ..........
+00009f50: 0208 011a 0102 0002 0002 0002 0002 0102  ................
+00009f60: 0002 fe06 040a 0222 011a 0214 0114 0114  ......."........
+00009f70: 0114 0114 0218 0210 0108 0116 0102 0002  ................
+00009f80: 0002 0002 0002 0002 0002 0102 0002 fe06  ................
+00009f90: 040a 0222 011a 0214 0114 0114 0114 0114  ..."............
+00009fa0: 0214 0272 b002 0000 7262 0000 0063 0600  ...r....rb...c..
+00009fb0: 0000 0000 0000 0000 0000 3700 0000 0d00  ..........7.....
+00009fc0: 0000 4300 0000 7326 0900 0064 0164 006c  ..C...s&...d.d.l
+00009fd0: 007d 0674 01a0 027c 0164 0219 007c 0064  .}.t...|.d...|.d
+00009fe0: 007c 0485 0219 006b 02a1 0164 0119 0064  .|.....k...d...d
+00009ff0: 0119 007d 077c 0164 0319 007c 0719 0074  ...}.|.d...|...t
+0000a000: 031b 007d 0874 01a0 0474 01a0 0564 04a1  ...}.t...t...d..
+0000a010: 01a1 017c 0814 0064 0514 007d 0964 067d  ...|...d...}.d.}
+0000a020: 0a7c 027c 091b 007c 0a1b 0064 0714 007d  .|.|...|...d...}
+0000a030: 0b74 0674 076a 0864 0817 0083 0101 0074  .t.t.j.d.......t
+0000a040: 0664 0983 0101 0064 0a7d 0c64 0ba0 097c  .d.....d.}.d...|
+0000a050: 0064 007c 0485 0219 0064 0c7c 02a1 037d  .d.|.....d.|...}
+0000a060: 0d74 0a6a 0ba0 0c7c 0da1 0173 f274 0664  .t.j...|...s.t.d
+0000a070: 0d7c 0d9b 0064 0e9d 0383 0101 0064 0fa0  .|...d.......d..
+0000a080: 097c 0164 1019 007c 0719 007c 0164 1119  .|.d...|...|.d..
+0000a090: 007c 0719 0074 0d7c 0b83 01a1 037d 0e7c  .|...t.|.....}.|
+0000a0a0: 0c7c 0e17 007d 0f74 067c 0f83 0101 0074  .|...}.t.|.....t
+0000a0b0: 0ea0 0f7c 0f7c 0da1 0201 006e 1074 0664  ...|.|.....n.t.d
+0000a0c0: 127c 0d9b 0064 139d 0383 0101 0064 0ba0  .|...d.......d..
+0000a0d0: 097c 0064 007c 0485 0219 0064 147c 02a1  .|.d.|.....d.|..
+0000a0e0: 037d 0d74 0a6a 0ba0 0c7c 0da1 0190 0173  .}.t.j...|.....s
+0000a0f0: 7674 0664 0d7c 0d9b 0064 0e9d 0383 0101  vt.d.|...d......
+0000a100: 0064 15a0 097c 0164 1019 007c 0719 007c  .d...|.d...|...|
+0000a110: 0164 1119 007c 0719 0074 0d7c 0b83 01a1  .d...|...t.|....
+0000a120: 037d 0e7c 0c7c 0e17 007d 0f74 067c 0f83  .}.|.|...}.t.|..
+0000a130: 0101 0074 0ea0 0f7c 0f7c 0da1 0201 006e  ...t...|.|.....n
+0000a140: 1074 0664 127c 0d9b 0064 139d 0383 0101  .t.d.|...d......
+0000a150: 0074 10a0 1164 0ba0 097c 0064 007c 0485  .t...d...|.d.|..
+0000a160: 0219 0064 0c7c 02a1 03a1 017d 107c 1064  ...d.|.....}.|.d
+0000a170: 0119 006a 127d 1174 13a0 1464 0ba0 097c  ...j.}.t...d...|
+0000a180: 0064 007c 0485 0219 0064 0c7c 02a1 03a1  .d.|.....d.|....
+0000a190: 0164 0119 007d 1274 10a0 1164 0ba0 097c  .d...}.t...d...|
+0000a1a0: 0064 007c 0485 0219 0064 147c 02a1 03a1  .d.|.....d.|....
+0000a1b0: 017d 137c 1364 0119 006a 127d 1474 15a0  .}.|.d...j.}.t..
+0000a1c0: 167c 03a1 017d 1574 01a0 027c 1564 1619  .|...}.t...|.d..
+0000a1d0: 007c 006b 02a1 0164 0119 0064 0119 007d  .|.k...d...d...}
+0000a1e0: 167c 1564 1719 007c 1619 007d 177c 1564  .|.d...|...}.|.d
+0000a1f0: 1819 007c 1619 007d 187c 1564 1919 007c  ...|...}.|.d...|
+0000a200: 1619 007d 1974 01a0 177c 1564 1a19 007c  ...}.t...|.d...|
+0000a210: 1619 00a1 017d 1a7c 1564 1b19 007c 1619  .....}.|.d...|..
+0000a220: 007d 1b7c 1564 1c19 007c 1619 007d 1c74  .}.|.d...|...}.t
+0000a230: 136a 187c 1764 1d18 007c 1864 1d18 007c  .j.|.d...|.d...|
+0000a240: 1b7c 197c 1a64 1e17 0074 0d7c 06a0 197c  .|.|.d...t.|...|
+0000a250: 1b7c 1b64 1f7c 1918 0014 00a1 0264 0714  .|.d.|.......d..
+0000a260: 0083 0164 208d 067d 1d7c 1b64 0714 007d  ...d ..}.|.d...}
+0000a270: 1b74 136a 187c 1764 1d18 007c 1864 1d18  .t.j.|.d...|.d..
+0000a280: 007c 1b7c 197c 1a64 1e17 0074 0d7c 06a0  .|.|.|.d...t.|..
+0000a290: 197c 1b7c 1b64 1f7c 1918 0014 00a1 0264  .|.|.d.|.......d
+0000a2a0: 0714 0083 0164 208d 067d 1e74 13a0 1a7c  .....d ..}.t...|
+0000a2b0: 1d7c 127c 1174 016a 1b14 00a1 037d 1f74  .|.|.t.j.....}.t
+0000a2c0: 13a0 1a7c 1e7c 127c 1174 016a 1b14 00a1  ...|.|.|.t.j....
+0000a2d0: 037d 2074 1c6a 1d64 2164 228d 017d 2174  .} t.j.d!d"..}!t
+0000a2e0: 01a0 1e7c 1164 23a1 027d 2274 01a0 1e7c  ...|.d#..}"t...|
+0000a2f0: 1164 24a1 027d 2374 1c6a 1f7c 1164 2564  .d$..}#t.j.|.d%d
+0000a300: 2664 277c 227c 2364 288d 0601 0074 1ca0  &d'|"|#d(....t..
+0000a310: 207c 1e64 0064 0085 0264 0166 0219 007c   |.d.d...d.f...|
+0000a320: 1e64 0064 0085 0264 1f66 0219 0064 29a1  .d.d...d.f...d).
+0000a330: 0301 0074 1ca0 21a1 0001 0074 1ca0 2264  ...t..!....t.."d
+0000a340: 2aa1 0101 0074 1ca0 2364 2ba1 0101 0074  *....t..#d+....t
+0000a350: 1ca0 24a1 0001 0074 1c6a 2564 2ca0 097c  ..$....t.j%d,..|
+0000a360: 0064 007c 0485 0219 0064 0c7c 02a1 0364  .d.|.....d.|...d
+0000a370: 2d64 2e8d 0201 007c 0564 2f6b 0290 0372  -d.....|.d/k...r
+0000a380: c074 1ca0 26a1 0001 006e 0874 1ca0 27a1  .t..&....n.t..'.
+0000a390: 0001 0074 01a0 287c 117c 2017 00a1 017d  ...t..(|.| ....}
+0000a3a0: 2474 01a0 287c 147c 2017 00a1 017d 2564  $t..(|.| ....}%d
+0000a3b0: 307d 2664 3174 01a0 297c 24a1 0114 0064  0}&d1t..)|$....d
+0000a3c0: 3017 007d 2764 3174 01a0 297c 25a1 0114  0..}'d1t..)|%...
+0000a3d0: 0064 3017 007d 2864 3264 3364 347c 277c  .d0..}(d2d3d4|'|
+0000a3e0: 2818 0014 0017 0013 007d 2964 3574 01a0  (........})d5t..
+0000a3f0: 297c 0864 3614 00a1 0114 0064 3717 007c  )|.d6......d7..|
+0000a400: 2717 007d 2a64 3574 01a0 297c 0864 3614  '..}*d5t..)|.d6.
+0000a410: 00a1 0114 0064 3717 007c 2817 007d 2b64  .....d7..|(..}+d
+0000a420: 3264 3864 397c 2a18 0014 0013 007d 2c7c  2d8d9|*......},|
+0000a430: 2c7c 2914 007d 2d7a c47c 0164 3a19 007c  ,|)..}-z.|.d:..|
+0000a440: 0719 007d 2e74 2a7c 2e14 0074 031b 007d  ...}.t*|...t...}
+0000a450: 2f74 2b7c 087c 2f18 0083 0164 3b14 007d  /t+|.|/....d;..}
+0000a460: 3074 01a0 2c7c 0164 3c19 00a1 017d 317c  0t..,|.d<....}1|
+0000a470: 317c 0719 0064 3d6b 0390 0572 2274 2d7c  1|...d=k...r"t-|
+0000a480: 0164 1019 007c 0719 007c 0164 1119 007c  .d...|...|.d...|
+0000a490: 0719 0074 2e6a 2f64 3e8d 037d 3274 2d7c  ...t.j/d>..}2t-|
+0000a4a0: 0164 3c19 007c 0719 007c 0164 3f19 007c  .d<..|...|.d?..|
+0000a4b0: 0719 0074 2e6a 2f64 3e8d 037d 337c 32a0  ...t.j/d>..}3|2.
+0000a4c0: 307c 33a1 017d 347c 346a 317c 0914 007d  0|3..}4|4j1|...}
+0000a4d0: 3574 01a0 3274 01a0 337c 35a1 0174 01a0  5t..2t..3|5..t..
+0000a4e0: 337c 30a1 0117 00a1 017d 366e 0c74 016a  3|0......}6n.t.j
+0000a4f0: 1b7d 3574 016a 1b7d 3657 006e 0c01 0001  .}5t.j.}6W.n....
+0000a500: 0001 0059 006e 0258 0074 15a0 167c 03a1  ...Y.n.X.t...|..
+0000a510: 017d 1574 01a0 027c 1564 1619 007c 006b  .}.t...|.d...|.k
+0000a520: 02a1 0164 0119 0064 0119 007d 1674 0674  ...d...d...}.t.t
+0000a530: 076a 3464 4017 0083 0101 0074 0674 076a  .j4d@......t.t.j
+0000a540: 3464 4117 0083 0101 007a 3074 01a0 297c  4dA......z0t..)|
+0000a550: 2da1 017c 1564 4219 007c 163c 0074 0674  -..|.dB..|.<.t.t
+0000a560: 076a 3564 43a0 0974 01a0 297c 2da1 01a1  .j5dC..t..)|-...
+0000a570: 0117 0083 0101 0057 006e 6a01 0001 0001  .......W.nj.....
+0000a580: 0074 0674 076a 0864 44a0 097c 03a1 0117  .t.t.j.dD..|....
+0000a590: 0083 0101 007c 156a 3674 01a0 3774 387c  .....|.j6t..7t8|
+0000a5a0: 1583 01a1 0174 016a 1b14 0064 4264 458d  .....t.j...dBdE.
+0000a5b0: 0201 0074 01a0 297c 2da1 017c 1564 4219  ...t..)|-..|.dB.
+0000a5c0: 007c 163c 0074 0674 076a 3564 43a0 0974  .|.<.t.t.j5dC..t
+0000a5d0: 01a0 297c 2da1 01a1 0117 0083 0101 0059  ..)|-..........Y
+0000a5e0: 006e 0258 007a 247c 287c 1564 4619 007c  .n.X.z$|(|.dF..|
+0000a5f0: 163c 0074 0674 076a 3564 47a0 097c 28a1  .<.t.t.j5dG..|(.
+0000a600: 0117 0083 0101 0057 006e 5e01 0001 0001  .......W.n^.....
+0000a610: 0074 0674 076a 0864 48a0 097c 03a1 0117  .t.t.j.dH..|....
+0000a620: 0083 0101 007c 156a 3674 01a0 3774 387c  .....|.j6t..7t8|
+0000a630: 1583 01a1 0174 016a 1b14 0064 4664 458d  .....t.j...dFdE.
+0000a640: 0201 007c 287c 1564 4619 007c 163c 0074  ...|(|.dF..|.<.t
+0000a650: 0674 076a 3564 47a0 097c 28a1 0117 0083  .t.j5dG..|(.....
+0000a660: 0101 0059 006e 0258 007a 247c 277c 1564  ...Y.n.X.z$|'|.d
+0000a670: 4919 007c 163c 0074 0674 076a 3564 4aa0  I..|.<.t.t.j5dJ.
+0000a680: 097c 27a1 0117 0083 0101 0057 006e 5e01  .|'........W.n^.
+0000a690: 0001 0001 0074 0674 076a 0864 4ba0 097c  .....t.t.j.dK..|
+0000a6a0: 03a1 0117 0083 0101 007c 156a 3674 01a0  .........|.j6t..
+0000a6b0: 3774 387c 1583 01a1 0174 016a 1b14 0064  7t8|.....t.j...d
+0000a6c0: 4964 458d 0201 007c 277c 1564 4919 007c  IdE....|'|.dI..|
+0000a6d0: 163c 0074 0674 076a 3564 4aa0 097c 27a1  .<.t.t.j5dJ..|'.
+0000a6e0: 0117 0083 0101 0059 006e 0258 007a 247c  .......Y.n.X.z$|
+0000a6f0: 2b7c 1564 4c19 007c 163c 0074 0674 076a  +|.dL..|.<.t.t.j
+0000a700: 3564 4da0 097c 2ba1 0117 0083 0101 0057  5dM..|+........W
+0000a710: 006e 5e01 0001 0001 0074 0674 076a 0864  .n^......t.t.j.d
+0000a720: 4ea0 097c 03a1 0117 0083 0101 007c 156a  N..|.........|.j
+0000a730: 3674 01a0 3774 387c 1583 01a1 0174 016a  6t..7t8|.....t.j
+0000a740: 1b14 0064 4c64 458d 0201 007c 2b7c 1564  ...dLdE....|+|.d
+0000a750: 4c19 007c 163c 0074 0674 076a 3564 4da0  L..|.<.t.t.j5dM.
+0000a760: 097c 2ba1 0117 0083 0101 0059 006e 0258  .|+........Y.n.X
+0000a770: 007a 247c 2a7c 1564 4f19 007c 163c 0074  .z$|*|.dO..|.<.t
+0000a780: 0674 076a 3564 50a0 097c 2aa1 0117 0083  .t.j5dP..|*.....
+0000a790: 0101 0057 006e 5e01 0001 0001 0074 0674  ...W.n^......t.t
+0000a7a0: 076a 0864 51a0 097c 03a1 0117 0083 0101  .j.dQ..|........
+0000a7b0: 007c 156a 3674 01a0 3774 387c 1583 01a1  .|.j6t..7t8|....
+0000a7c0: 0174 016a 1b14 0064 4f64 458d 0201 007c  .t.j...dOdE....|
+0000a7d0: 2a7c 1564 4f19 007c 163c 0074 0674 076a  *|.dO..|.<.t.t.j
+0000a7e0: 3564 50a0 097c 2aa1 0117 0083 0101 0059  5dP..|*........Y
+0000a7f0: 006e 0258 007a 347c 0164 5219 007c 0719  .n.X.z4|.dR..|..
+0000a800: 007c 1564 5319 007c 163c 0074 0674 076a  .|.dS..|.<.t.t.j
+0000a810: 3464 54a0 097c 0164 5519 007c 0719 00a1  4dT..|.dU..|....
+0000a820: 0117 0083 0101 0057 006e 0c01 0001 0001  .......W.n......
+0000a830: 0059 006e 0258 007a 2c7c 357c 1564 5619  .Y.n.X.z,|5|.dV.
+0000a840: 007c 163c 0074 0674 076a 3464 57a0 097c  .|.<.t.t.j4dW..|
+0000a850: 0164 5219 007c 0719 00a1 0117 0083 0101  .dR..|..........
+0000a860: 0057 006e 0c01 0001 0001 0059 006e 0258  .W.n.......Y.n.X
+0000a870: 007a 247c 367c 1564 5819 007c 163c 0074  .z$|6|.dX..|.<.t
+0000a880: 0674 076a 3464 59a0 097c 35a1 0117 0083  .t.j4dY..|5.....
+0000a890: 0101 0057 006e 0c01 0001 0001 0059 006e  ...W.n.......Y.n
+0000a8a0: 0258 007a 2c7c 0164 5519 007c 0719 007c  .X.z,|.dU..|...|
+0000a8b0: 1564 5519 007c 163c 0074 0674 076a 3464  .dU..|.<.t.t.j4d
+0000a8c0: 5aa0 097c 36a1 0117 0083 0101 0057 006e  Z..|6........W.n
+0000a8d0: 0c01 0001 0001 0059 006e 0258 0074 156a  .......Y.n.X.t.j
+0000a8e0: 397c 157c 0364 5b64 5c8d 0301 0064 0053  9|.|.d[d\....d.S
+0000a8f0: 0029 5d4e 7201 0000 0072 4100 0000 7242  .)]Nr....rA...rB
+0000a900: 0000 0072 4300 0000 7244 0000 0072 ab02  ...rC...rD...r..
+0000a910: 0000 7239 0000 007a 230a 0a4c 6f61 6469  ..r9...z#..Loadi
+0000a920: 6e67 2f44 6f77 6e6c 6f61 6469 6e67 2044  ng/Downloading D
+0000a930: 6563 616c 7320 696d 6167 6573 7258 0000  ecals imagesrX..
+0000a940: 0072 ad02 0000 72ae 0200 0072 6602 0000  .r....r....rf...
+0000a950: 725d 0000 0072 5e00 0000 7a34 7261 3d7b  r]...r^...z4ra={
+0000a960: 7d26 6465 633d 7b7d 266c 6179 6572 3d64  }&dec={}&layer=d
+0000a970: 7238 2670 6978 7363 616c 653d 302e 3237  r8&pixscale=0.27
+0000a980: 2662 616e 6473 3d67 2673 697a 653d 7b7d  &bands=g&size={}
+0000a990: 724e 0000 0072 4f00 0000 725b 0000 0072  rN...rO...r[...r
+0000a9a0: 5c00 0000 726c 0200 007a 3472 613d 7b7d  \...rl...z4ra={}
+0000a9b0: 2664 6563 3d7b 7d26 6c61 7965 723d 6472  &dec={}&layer=dr
+0000a9c0: 3826 7069 7873 6361 6c65 3d30 2e32 3726  8&pixscale=0.27&
+0000a9d0: 6261 6e64 733d 7226 7369 7a65 3d7b 7d72  bands=r&size={}r
+0000a9e0: c200 0000 7252 0100 0072 5301 0000 7254  ....rR...rS...rT
+0000a9f0: 0100 0072 5501 0000 7250 0100 0072 c500  ...rU...rP...r..
+0000aa00: 0000 7249 0000 0072 6c01 0000 7269 0000  ..rI...rl...ri..
+0000aa10: 0029 06da 0278 30da 0279 30da 0373 6d61  .)...x0..y0..sma
+0000aa20: da03 6570 73da 0270 61da 0473 7465 7072  ..eps..pa..stepr
+0000aa30: 7400 0000 7276 0000 0072 3700 0000 6700  t...rv...r7...g.
+0000aa40: 0000 0000 e058 4072 0302 0000 da08 5264  .....X@r......Rd
+0000aa50: 596c 4275 5f72 7278 0000 0029 0572 0502  YlBu_rrx...).r..
+0000aa60: 0000 72a8 0000 0072 7a00 0000 da04 766d  ..r....rz.....vm
+0000aa70: 696e da04 766d 6178 7a03 6b2d 2d7a 0778  in..vmaxz.k--z.x
+0000aa80: 2028 7069 7829 7a07 7920 2870 6978 297a   (pix)z.y (pix)z
+0000aa90: 1d69 6d61 6765 732f 6669 675f 7b7d 5f67  .images/fig_{}_g
+0000aaa0: 5f7b 7d6b 7063 5f32 5265 2e70 6e67 727c  _{}kpc_2Re.pngr|
+0000aab0: 0000 0072 7d00 0000 7240 0000 0072 b502  ...r}...r@...r..
+0000aac0: 0000 7224 0000 0072 cd01 0000 6756 0e2d  ..r$...r....gV.-
+0000aad0: b29d efdf bf67 e7fb a9f1 d24d f83f 6700  .....g.....M.?g.
+0000aae0: 0000 0000 0014 c067 0000 0000 8084 2e41  .......g.......A
+0000aaf0: 6700 0000 0000 0014 4067 9a99 9999 9999  g.......@g......
+0000ab00: d93f 6771 3d0a d7a3 7014 4072 c400 0000  .?gq=...p.@r....
+0000ab10: 72e5 0100 0072 6a02 0000 726b 0000 0029  r....rj...rk...)
+0000ab20: 0172 7f02 0000 726b 0200 007a 150a 4765  .r....rk...z..Ge
+0000ab30: 6e65 7261 6c20 696e 666f 726d 6174 696f  neral informatio
+0000ab40: 6e3a 7246 0000 00da 046d 6173 737a 140a  n:rF.....massz..
+0000ab50: 4d61 7373 2028 6c6f 6729 203d 207b 3a2e  Mass (log) = {:.
+0000ab60: 3166 7d7a 2754 6865 2063 6f6c 756d 6e20  1f}z'The column 
+0000ab70: 3c3c 6d61 7373 3e3e 2077 6173 2061 6464  <<mass>> was add
+0000ab80: 6564 2074 6f20 7468 6520 7b7d 2901 da04  ed to the {})...
+0000ab90: 6e61 6d65 da09 6d61 675f 725f 3252 657a  name..mag_r_2Rez
+0000aba0: 126d 6167 5f72 5f32 5265 203d 207b 3a2e  .mag_r_2Re = {:.
+0000abb0: 3166 7d7a 2c54 6865 2063 6f6c 756d 6e20  1f}z,The column 
+0000abc0: 3c3c 6d61 675f 725f 3252 653e 3e20 7761  <<mag_r_2Re>> wa
+0000abd0: 7320 6164 6465 6420 746f 2074 6865 207b  s added to the {
+0000abe0: 7dda 096d 6167 5f67 5f32 5265 7a12 6d61  }..mag_g_2Rez.ma
+0000abf0: 675f 675f 3252 6520 3d20 7b3a 2e31 667d  g_g_2Re = {:.1f}
+0000ac00: 7a2c 5468 6520 636f 6c75 6d6e 203c 3c6d  z,The column <<m
+0000ac10: 6167 5f67 5f32 5265 3e3e 2077 6173 2061  ag_g_2Re>> was a
+0000ac20: 6464 6564 2074 6f20 7468 6520 7b7d da06  dded to the {}..
+0000ac30: 4d72 5f32 5265 7a0f 4d72 5f32 5265 203d  Mr_2Rez.Mr_2Re =
+0000ac40: 207b 3a2e 3166 7d7a 2954 6865 2063 6f6c   {:.1f}z)The col
+0000ac50: 756d 6e20 3c3c 4d72 5f32 5265 3e3e 2077  umn <<Mr_2Re>> w
+0000ac60: 6173 2061 6464 6564 2074 6f20 7468 6520  as added to the 
+0000ac70: 7b7d da06 4d67 5f32 5265 7a0f 4d67 5f32  {}..Mg_2Rez.Mg_2
+0000ac80: 5265 203d 207b 3a2e 3166 7d7a 2954 6865  Re = {:.1f}z)The
+0000ac90: 2063 6f6c 756d 6e20 3c3c 4d67 5f32 5265   column <<Mg_2Re
+0000aca0: 3e3e 2077 6173 2061 6464 6564 2074 6f20  >> was added to 
+0000acb0: 7468 6520 7b7d da07 7369 676d 615f 43da  the {}..sigma_C.
+0000acc0: 0573 6967 5f43 7a12 0a4c 7820 286c 6f67  .sig_Cz..Lx (log
+0000acd0: 2920 3d20 7b3a 2e31 667d da02 4c78 da06  ) = {:.1f}..Lx..
+0000ace0: 445f 7072 6f6a 7a13 7369 676d 6120 3d20  D_projz.sigma = 
+0000acf0: 7b3a 2e31 667d 206b 6d2f 73da 0644 5f69  {:.1f} km/s..D_i
+0000ad00: 6e74 727a 1344 5f70 726f 6a20 3d20 7b3a  ntrz.D_proj = {:
+0000ad10: 2e31 667d 206b 7063 7a13 445f 696e 7472  .1f} kpcz.D_intr
+0000ad20: 203d 207b 3a2e 3166 7d20 6b70 6354 7292   = {:.1f} kpcTr.
+0000ad30: 0000 0029 3ada 0966 756e 6374 696f 6e73  ...):..functions
+0000ad40: 7225 0000 0072 c800 0000 72b7 0000 0072  r%...r....r....r
+0000ad50: c900 0000 72ca 0000 0072 cb00 0000 7219  ....r....r....r.
+0000ad60: 0000 0072 dd00 0000 7264 0000 0072 d400  ...r....rd...r..
+0000ad70: 0000 72d5 0000 0072 d600 0000 72d8 0000  ..r....r....r...
+0000ad80: 0072 1a00 0000 7213 0000 0072 0300 0000  .r....r....r....
+0000ad90: 72e4 0000 0072 e500 0000 72b0 0100 00da  r....r....r.....
+0000ada0: 0563 616c 6c66 7204 0000 0072 d900 0000  .callfr....r....
+0000adb0: da07 7261 6432 6465 67da 0765 6c6c 6970  ..rad2deg..ellip
+0000adc0: 7365 da10 7065 7269 5f65 6c6c 6970 5f65  se..peri_ellip_e
+0000add0: 7861 6374 da08 6d61 736b 706f 6c79 7227  xact..maskpolyr'
+0000ade0: 0000 0072 e600 0000 72e7 0000 00da 0d6e  ...r....r......n
+0000adf0: 616e 7065 7263 656e 7469 6c65 72e8 0000  anpercentiler...
+0000ae00: 00da 0470 6c6f 7472 c001 0000 722c 0200  ...plotr....r,..
+0000ae10: 0072 2d02 0000 722a 0200 0072 e900 0000  .r-...r*...r....
+0000ae20: 72ea 0000 0072 eb00 0000 da06 6e61 6e73  r....r......nans
+0000ae30: 756d 7228 0000 0072 fd00 0000 7280 0200  umr(...r....r...
+0000ae40: 0072 8b01 0000 7209 0000 0072 7702 0000  .r....r....rw...
+0000ae50: 7272 0200 0072 7a02 0000 7279 0200 0072  rr...rz...ry...r
+0000ae60: ee00 0000 72cd 0000 0072 cc00 0000 72d2  ....r....r....r.
+0000ae70: 0000 00da 0a61 6464 5f63 6f6c 756d 6eda  .....add_column.
+0000ae80: 057a 6572 6f73 72e3 0000 0072 dc00 0000  .zerosr....r....
+0000ae90: 2937 7241 0000 0072 ff00 0000 7201 0100  )7rA...r....r...
+0000aea0: 0072 c000 0000 da07 7375 665f 6e75 6d72  .r......suf_numr
+0000aeb0: c100 0000 da04 6675 6e63 7209 0100 0072  ......funcr....r
+0000aec0: b300 0000 720a 0100 0072 b901 0000 720b  ....r....r....r.
+0000aed0: 0100 0072 b102 0000 72d5 0000 0072 3f02  ...r....r....r?.
+0000aee0: 0000 72b2 0200 0072 1a01 0000 721b 0100  ..r....r....r...
+0000aef0: 00da 0569 6d61 7879 da05 696d 6172 6eda  ...imaxy..imarn.
+0000af00: 0469 6d61 7272 e500 0000 7236 0100 00da  .imarr....r6....
+0000af10: 0a63 656e 7478 5f70 686f 74da 0a63 656e  .centx_phot..cen
+0000af20: 7479 5f70 686f 74da 0465 7073 3072 6001  ty_phot..eps0r`.
+0000af30: 0000 da08 736d 6165 6c6c 6970 da05 7a5f  ....smaellip..z_
+0000af40: 6761 6cda 0d67 616c 5f70 6f6c 5f31 5265  gal..gal_pol_1Re
+0000af50: 6666 da0d 6761 6c5f 706f 6c5f 3252 6566  ff..gal_pol_2Ref
+0000af60: 66da 096d 6173 6b5f 6761 6c31 da09 6d61  f..mask_gal1..ma
+0000af70: 736b 5f67 616c 3272 1d01 0000 72bf 0200  sk_gal2r....r...
+0000af80: 0072 c002 0000 da05 666c 7578 67da 0566  .r......fluxg..f
+0000af90: 6c75 7872 722d 0000 00da 056d 6167 5f67  luxrr-.....mag_g
+0000afa0: da05 6d61 675f 72da 034d 4c67 da02 4d67  ..mag_r..MLg..Mg
+0000afb0: da02 4d72 da02 4c67 da0c 6d61 7373 5f73  ..Mr..Lg..mass_s
+0000afc0: 7465 6c6c 6172 da03 7a5f 43da 0544 5f67  tellar..z_C..D_g
+0000afd0: 616c da07 6465 6c74 615f 4472 4e00 0000  al..delta_DrN...
+0000afe0: da09 636f 6f72 645f 6761 6cda 0763 6f6f  ..coord_gal..coo
+0000aff0: 7264 5f43 7287 0200 0072 8802 0000 da05  rd_Cr....r......
+0000b000: 445f 696e 7472 2f00 0000 722f 0000 0072  D_intr/...r/...r
+0000b010: 3000 0000 da0b 6d61 7373 5f64 6563 616c  0.....mass_decal
+0000b020: 7385 0700 0073 9a01 0000 0003 0802 2201  s....s........".
+0000b030: 1001 1801 0401 1002 0e01 0802 0401 1001  ................
+0000b040: 02ff 0402 0c01 1001 0401 0a00 0a00 06ff  ................
+0000b050: 0402 0801 0804 0e02 1002 1001 02ff 0402  ................
+0000b060: 0e01 1001 0401 0a00 0a00 06ff 0402 0801  ................
+0000b070: 0802 0e02 1002 1401 02ff 0602 0a02 1401  ................
+0000b080: 02ff 0401 02ff 0404 1401 02ff 0602 0a02  ................
+0000b090: 0a02 1a02 0c01 0c01 0c01 1201 0c01 0c02  ................
+0000b0a0: 1001 0200 0200 0601 0801 0aff 0201 02ff  ................
+0000b0b0: 04fe 0605 0801 1001 0200 0200 0601 0801  ................
+0000b0c0: 0aff 0201 02ff 04fe 0605 1401 1402 0c01  ................
+0000b0d0: 0c01 0c02 0c01 0200 02ff 0602 2601 0801  ............&...
+0000b0e0: 0a01 0a01 0801 1401 02ff 0201 02ff 0602  ................
+0000b0f0: 0a01 0a02 0802 0e01 0e02 0402 1201 1202  ................
+0000b100: 1401 1a01 1a01 1001 0803 0201 0c01 0c01  ................
+0000b110: 1002 0e01 0e01 1601 04ff 0602 1601 04ff  ................
+0000b120: 0602 0a02 0a01 1c02 0601 0a01 0601 0602  ................
+0000b130: 0a01 1a02 0e01 0e02 0201 1201 1e01 0601  ................
+0000b140: 0a01 02ff 0802 1e01 1201 2001 0201 0c01  .......... .....
+0000b150: 1801 0601 0a01 02ff 0802 1e01 0c01 1a01  ................
+0000b160: 0201 0c01 1801 0601 0a01 02ff 0802 1e01  ................
+0000b170: 0c01 1a01 0201 0c01 1801 0601 0a01 02ff  ................
+0000b180: 0802 1e01 0c01 1a01 0201 0c01 1801 0601  ................
+0000b190: 0a01 02ff 0802 1e01 0c01 1a01 0201 1401  ................
+0000b1a0: 2001 0601 0601 0201 0c01 2001 0601 0601   ......... .....
+0000b1b0: 0201 0c01 1801 0601 0601 0201 1401 1801  ................
+0000b1c0: 0601 0602 72f4 0200 0029 0272 4000 0000  ....r....).r@...
+0000b1d0: 723f 0000 0029 0472 3a00 0000 7244 0200  r?...).r:...rD..
+0000b1e0: 0072 cc01 0000 4e29 0372 3a00 0000 7215  .r....N).r:...r.
+0000b1f0: 0200 0072 1502 0000 290a 723a 0000 0072  ...r....).r:...r
+0000b200: 1502 0000 7215 0200 0072 cd01 0000 7297  ....r....r....r.
+0000b210: 0000 0072 cd01 0000 723b 0000 0072 cc01  ...r....r;...r..
+0000b220: 0000 72ce 0100 0072 5902 0000 290f 4e4e  ..r....rY...).NN
+0000b230: 72cd 0100 0072 9700 0000 72cd 0100 004e  r....r....r....N
+0000b240: 5472 ce01 0000 723b 0000 0072 0100 0000  Tr....r;...r....
+0000b250: 7240 0000 0072 4000 0000 72ce 0100 0072  r@...r@...r....r
+0000b260: 3c00 0000 723f 0000 0029 0372 3f00 0000  <...r?...).r?...
+0000b270: 7262 0000 0072 4000 0000 2950 da05 6e75  rb...r@...)P..nu
+0000b280: 6d70 7972 2500 0000 da11 6d61 7470 6c6f  mpyr%.....matplo
+0000b290: 746c 6962 2e70 7970 6c6f 74da 0670 7970  tlib.pyplot..pyp
+0000b2a0: 6c6f 7472 e600 0000 72f6 0000 005a 2173  lotr....r....Z!s
+0000b2b0: 7461 746d 6f72 7068 2e75 7469 6c73 2e69  tatmorph.utils.i
+0000b2c0: 6d61 6765 5f64 6961 676e 6f73 7469 6373  mage_diagnostics
+0000b2d0: 7202 0000 00da 0a61 7374 726f 7079 2e69  r......astropy.i
+0000b2e0: 6f72 0300 0000 7204 0000 00da 0d61 7374  or....r......ast
+0000b2f0: 726f 7079 2e74 6162 6c65 7205 0000 00da  ropy.tabler.....
+0000b300: 0a61 7374 726f 7175 6572 7972 0600 0000  .astroqueryr....
+0000b310: da13 6173 7472 6f71 7565 7279 2e69 7061  ..astroquery.ipa
+0000b320: 632e 6e65 6472 0700 0000 da0b 6173 7472  c.nedr......astr
+0000b330: 6f70 792e 7763 7372 0800 0000 da13 6173  opy.wcsr......as
+0000b340: 7472 6f70 792e 636f 6f72 6469 6e61 7465  tropy.coordinate
+0000b350: 7372 0900 0000 da0d 6173 7472 6f70 792e  sr......astropy.
+0000b360: 756e 6974 73da 0575 6e69 7473 7277 0200  units..unitsrw..
+0000b370: 005a 1670 686f 7475 7469 6c73 2e73 6567  .Z.photutils.seg
+0000b380: 6d65 6e74 6174 696f 6e72 0a00 0000 da0d  mentationr......
+0000b390: 6173 7472 6f70 792e 7374 6174 7372 0b00  astropy.statsr..
+0000b3a0: 0000 5a14 7068 6f74 7574 696c 732e 6261  ..Z.photutils.ba
+0000b3b0: 636b 6772 6f75 6e64 720c 0000 0072 0d00  ckgroundr....r..
+0000b3c0: 0000 720e 0000 0072 0f00 0000 da13 6173  ..r....r......as
+0000b3d0: 7472 6f70 792e 636f 6e76 6f6c 7574 696f  tropy.convolutio
+0000b3e0: 6e72 1000 0000 7211 0000 00da 0c75 726c  nr....r......url
+0000b3f0: 6c69 622e 7061 7273 6572 1200 0000 da0e  lib.parser......
+0000b400: 7572 6c6c 6962 2e72 6571 7565 7374 7213  urllib.requestr.
+0000b410: 0000 00da 1561 7374 726f 7079 2e76 6973  .....astropy.vis
+0000b420: 7561 6c69 7a61 7469 6f6e 7214 0000 0072  ualizationr....r
+0000b430: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+0000b440: 0000 00da 0863 6f6c 6f72 616d 6172 1900  .....coloramar..
+0000b450: 0000 da0d 7363 6970 792e 6e64 696d 6167  ....scipy.ndimag
+0000b460: 65da 076e 6469 6d61 6765 da03 6e64 6972  e..ndimage..ndir
+0000b470: f300 0000 da04 7767 6574 da06 7572 6c6c  ......wget..urll
+0000b480: 6962 721a 0000 0072 b700 0000 72fd 0000  ibr....r....r...
+0000b490: 0072 d400 0000 72f5 0000 00da 0e70 6c6f  .r....r......plo
+0000b4a0: 745f 6675 6e63 7469 6f6e 7372 b001 0000  t_functionsr....
+0000b4b0: 72b2 0100 00da 0973 6572 7665 725f 6672  r......server_fr
+0000b4c0: da09 7365 7276 655f 7573 6172 4502 0000  ..serve_usarE...
+0000b4d0: da14 7265 7365 745f 766f 7461 626c 655f  ..reset_votable_
+0000b4e0: 6669 656c 6473 da15 7265 6d6f 7665 5f76  fields..remove_v
+0000b4f0: 6f74 6162 6c65 5f66 6965 6c64 73da 1261  otable_fields..a
+0000b500: 6464 5f76 6f74 6162 6c65 5f66 6965 6c64  dd_votable_field
+0000b510: 7372 3100 0000 7236 0000 0072 3901 0000  sr1...r6...r9...
+0000b520: 72fc 0000 0072 4302 0000 721d 0200 0072  r....rC...r....r
+0000b530: 5802 0000 729a 0200 0072 2102 0000 72b4  X...r....r!...r.
+0000b540: 0200 0072 b002 0000 72f4 0200 0072 2f00  ...r....r....r/.
+0000b550: 0000 722f 0000 0072 2f00 0000 7230 0000  ..r/...r/...r0..
+0000b560: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+0000b570: 3e01 0000 0801 0c02 0801 0c02 1001 0c01  >...............
+0000b580: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 1001  ................
+0000b590: 0c01 0c02 0c01 0c02 0c01 0c01 1c03 0c02  ................
+0000b5a0: 0c02 0802 0801 0c02 0401 0401 0801 0802  ................
+0000b5b0: 0803 0402 0401 0406 0a02 0c09 0e01 0200  ................
+0000b5c0: 0200 0201 0200 0200 0200 0201 0200 0200  ................
+0000b5d0: 0200 02fd 0406 0806 0805 0601 0200 0200  ................
+0000b5e0: 0601 0200 0200 0200 0200 0201 0200 0200  ................
+0000b5f0: 02fd 0a7f 007f 0043 0001 00fe 0a7f 003a  .......C.......:
+0000b600: 0601 0200 0200 0200 0200 0201 0200 0600  ................
+0000b610: 0200 0201 0200 0200 0200 0201 0200 0200  ................
+0000b620: 0200 0200 0201 02fb 0a7f 007f 006d 0001  .............m..
+0000b630: 00ff 0a2c 0001 00ff 0a25 0001 0000 0000  ...,.....%......
+0000b640: 0000 0001 0000 0000 0001 00fd 0a7f 0033  ...............3
+0000b650: 0001 0000 0000 0000 0001 0000 0000 0000  ................
+0000b660: 0001 0000 0000 0001 0000 0000 00fc 0a7f  ................
+0000b670: 007f 001b 0401 0200 0200 0600 0201 0200  ................
+0000b680: 0200 0201 0200 0200 0201 02fc 0a7f 0057  ...............W
+0000b690: 0601 0201 0200 0200 0601 0200 0200 0200  ................
+0000b6a0: 0201 0200 0200 02fc 0a7f 005d 0001 0000  ...........]....
+0000b6b0: 00ff                                     ..
```

### Comparing `astromorphlib-0.2.8/stat_lib/__pycache__/stat_lib.cpython-38.pyc` & `astromorphlib-0.2.9/stat_lib/__pycache__/stat_lib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `astromorphlib-0.2.8/stat_lib/zero_points.fits` & `astromorphlib-0.2.9/stat_lib/zero_points.fits`

 * *Files identical despite different names*

