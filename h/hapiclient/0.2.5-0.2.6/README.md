# Comparing `tmp/hapiclient-0.2.5.tar.gz` & `tmp/hapiclient-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hapiclient-0.2.5.tar", last modified: Mon Jul 25 18:38:11 2022, max compression
+gzip compressed data, was "hapiclient-0.2.6.tar", last modified: Sat May 11 19:05:49 2024, max compression
```

## Comparing `hapiclient-0.2.5.tar` & `hapiclient-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 weigel     (501) staff       (20)        0 2022-07-25 18:38:11.000000 hapiclient-0.2.5/
--rw-r--r--   0 weigel     (501) staff       (20)     3516 2022-07-25 18:37:40.000000 hapiclient-0.2.5/CHANGES.txt
--rw-r--r--   0 weigel     (501) staff       (20)     1456 2022-06-28 14:47:56.000000 hapiclient-0.2.5/LICENSE.txt
--rw-r--r--   0 weigel     (501) staff       (20)       48 2022-06-28 14:47:56.000000 hapiclient-0.2.5/MANIFEST.in
--rw-r--r--   0 weigel     (501) staff       (20)     6419 2022-07-25 18:38:11.000000 hapiclient-0.2.5/PKG-INFO
--rw-r--r--   0 weigel     (501) staff       (20)     6106 2022-07-25 18:38:02.000000 hapiclient-0.2.5/README.md
-drwxr-xr-x   0 weigel     (501) staff       (20)        0 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient/
--rw-r--r--   0 weigel     (501) staff       (20)      387 2022-07-25 18:37:54.000000 hapiclient-0.2.5/hapiclient/__init__.py
--rw-r--r--   0 weigel     (501) staff       (20)    42822 2022-07-25 18:37:54.000000 hapiclient-0.2.5/hapiclient/hapi.py
--rw-r--r--   0 weigel     (501) staff       (20)    11019 2022-07-25 18:38:02.000000 hapiclient-0.2.5/hapiclient/hapitime.py
-drwxr-xr-x   0 weigel     (501) staff       (20)        0 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient/test/
--rw-r--r--   0 weigel     (501) staff       (20)        0 2022-06-28 14:47:56.000000 hapiclient-0.2.5/hapiclient/test/__init__.py
--rw-r--r--   0 weigel     (501) staff       (20)     8541 2022-07-12 21:33:13.000000 hapiclient-0.2.5/hapiclient/test/compare.py
--rw-r--r--   0 weigel     (501) staff       (20)     8399 2022-07-12 21:33:04.000000 hapiclient-0.2.5/hapiclient/test/test_chunking.py
--rw-r--r--   0 weigel     (501) staff       (20)     9989 2022-07-12 21:38:59.000000 hapiclient-0.2.5/hapiclient/test/test_hapi.py
--rw-r--r--   0 weigel     (501) staff       (20)     3180 2022-07-12 21:33:04.000000 hapiclient-0.2.5/hapiclient/test/test_hapitime2datetime.py
--rw-r--r--   0 weigel     (501) staff       (20)     2013 2022-07-12 21:33:04.000000 hapiclient-0.2.5/hapiclient/test/test_hapitime_reformat.py
--rw-r--r--   0 weigel     (501) staff       (20)    13582 2022-07-12 21:33:13.000000 hapiclient-0.2.5/hapiclient/util.py
-drwxr-xr-x   0 weigel     (501) staff       (20)        0 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient.egg-info/
--rw-r--r--   0 weigel     (501) staff       (20)     6419 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient.egg-info/PKG-INFO
--rw-r--r--   0 weigel     (501) staff       (20)      508 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient.egg-info/SOURCES.txt
--rw-r--r--   0 weigel     (501) staff       (20)        1 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient.egg-info/dependency_links.txt
--rw-r--r--   0 weigel     (501) staff       (20)       57 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient.egg-info/requires.txt
--rw-r--r--   0 weigel     (501) staff       (20)       11 2022-07-25 18:38:11.000000 hapiclient-0.2.5/hapiclient.egg-info/top_level.txt
--rw-r--r--   0 weigel     (501) staff       (20)       38 2022-07-25 18:38:11.000000 hapiclient-0.2.5/setup.cfg
--rw-r--r--   0 weigel     (501) staff       (20)     1484 2022-07-25 18:37:54.000000 hapiclient-0.2.5/setup.py
+drwxr-xr-x   0 weigel     (501) staff       (20)        0 2024-05-11 19:05:49.732020 hapiclient-0.2.6/
+-rw-r--r--   0 weigel     (501) staff       (20)     3947 2024-05-11 19:04:13.000000 hapiclient-0.2.6/CHANGES.txt
+-rw-r--r--   0 weigel     (501) staff       (20)     1456 2022-06-28 14:47:56.000000 hapiclient-0.2.6/LICENSE.txt
+-rw-r--r--   0 weigel     (501) staff       (20)       48 2022-06-28 14:47:56.000000 hapiclient-0.2.6/MANIFEST.in
+-rw-r--r--   0 weigel     (501) staff       (20)     5705 2024-05-11 19:05:49.731778 hapiclient-0.2.6/PKG-INFO
+-rw-r--r--   0 weigel     (501) staff       (20)     5412 2023-02-04 20:16:02.000000 hapiclient-0.2.6/README.md
+drwxr-xr-x   0 weigel     (501) staff       (20)        0 2024-05-11 19:05:49.727891 hapiclient-0.2.6/hapiclient/
+-rw-r--r--   0 weigel     (501) staff       (20)      489 2024-05-11 19:04:33.000000 hapiclient-0.2.6/hapiclient/__init__.py
+-rw-r--r--   0 weigel     (501) staff       (20)    44278 2024-05-11 19:04:33.000000 hapiclient-0.2.6/hapiclient/hapi.py
+-rw-r--r--   0 weigel     (501) staff       (20)    11866 2022-08-08 16:22:59.000000 hapiclient-0.2.6/hapiclient/hapitime.py
+drwxr-xr-x   0 weigel     (501) staff       (20)        0 2024-05-11 19:05:49.731461 hapiclient-0.2.6/hapiclient/test/
+-rw-r--r--   0 weigel     (501) staff       (20)        0 2022-06-28 14:47:56.000000 hapiclient-0.2.6/hapiclient/test/__init__.py
+-rw-r--r--   0 weigel     (501) staff       (20)     8541 2022-08-08 15:05:00.000000 hapiclient-0.2.6/hapiclient/test/compare.py
+-rw-r--r--   0 weigel     (501) staff       (20)     8415 2022-09-22 02:31:48.000000 hapiclient-0.2.6/hapiclient/test/test_chunking.py
+-rw-r--r--   0 weigel     (501) staff       (20)      510 2022-08-08 15:05:17.000000 hapiclient-0.2.6/hapiclient/test/test_datetime2hapitime.py
+-rw-r--r--   0 weigel     (501) staff       (20)    10794 2024-01-28 00:22:57.000000 hapiclient-0.2.6/hapiclient/test/test_hapi.py
+-rw-r--r--   0 weigel     (501) staff       (20)     3164 2022-08-08 16:24:08.000000 hapiclient-0.2.6/hapiclient/test/test_hapitime2datetime.py
+-rw-r--r--   0 weigel     (501) staff       (20)     2013 2022-08-08 15:05:00.000000 hapiclient-0.2.6/hapiclient/test/test_hapitime_reformat.py
+-rw-r--r--   0 weigel     (501) staff       (20)    13576 2023-01-07 10:23:53.000000 hapiclient-0.2.6/hapiclient/util.py
+drwxr-xr-x   0 weigel     (501) staff       (20)        0 2024-05-11 19:05:49.729482 hapiclient-0.2.6/hapiclient.egg-info/
+-rw-r--r--   0 weigel     (501) staff       (20)     5705 2024-05-11 19:05:49.000000 hapiclient-0.2.6/hapiclient.egg-info/PKG-INFO
+-rw-r--r--   0 weigel     (501) staff       (20)      550 2024-05-11 19:05:49.000000 hapiclient-0.2.6/hapiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 weigel     (501) staff       (20)        1 2024-05-11 19:05:49.000000 hapiclient-0.2.6/hapiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 weigel     (501) staff       (20)       57 2024-05-11 19:05:49.000000 hapiclient-0.2.6/hapiclient.egg-info/requires.txt
+-rw-r--r--   0 weigel     (501) staff       (20)       11 2024-05-11 19:05:49.000000 hapiclient-0.2.6/hapiclient.egg-info/top_level.txt
+-rw-r--r--   0 weigel     (501) staff       (20)       38 2024-05-11 19:05:49.732096 hapiclient-0.2.6/setup.cfg
+-rw-r--r--   0 weigel     (501) staff       (20)     1484 2024-05-11 19:04:33.000000 hapiclient-0.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hapiclient-0.2.5/CHANGES.txt` & `hapiclient-0.2.6/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -90,7 +90,17 @@
 	2022-03-01 -- bf0cc88 Add allow_missing_Z in hapitime2datetime.
 v0.2.4:
 	2022-03-07 -- 88b0eb2 try/except on file read
 	2022-03-29 -- 0042abb Fix for method=''. Closes #47.
 v0.2.5:
 	2022-06-30 -- 10df388 Update docstring for hapi()
 	2022-07-12 -- 460c30b Final Unicode/Windows fixes
+v0.2.6b:
+	2022-08-08 -- 508fb20-3f1168c Add datetime2hapitime
+	2022-08-08 -- 8bfef2f Allow start and stop to be None; https://github.com/hapi-server/client-python/issues/10
+	2022-09-21 -- bc70f3c CSV read failure; https://github.com/hapi-server/client-python/issues/62
+	2022-09-22 -- 373fdca Catch other CSV read failures
+v0.2.6b1:
+	2023-02-04 -- 2ef7cff Unicode fix; Log string fix
+	2024-05-11 -- fba4ad3 Testing Updates
+v0.2.6:
+
```

### Comparing `hapiclient-0.2.5/LICENSE.txt` & `hapiclient-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hapiclient-0.2.5/PKG-INFO` & `hapiclient-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hapiclient
-Version: 0.2.5
+Version: 0.2.6
 Summary: Interface to Heliophysics data server API
 Home-page: http://pypi.python.org/pypi/hapiclient/
 Author: Bob Weigel
 Author-email: rweigel@gmu.edu
 License: LICENSE.txt
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![DOI](https://zenodo.org/badge/93170857.svg)](https://zenodo.org/badge/latestdoi/93170857)
 [![Build Status](https://app.travis-ci.com/hapi-server/client-python.svg?branch=master)](https://app.travis-ci.com/hapi-server/client-python)
 
 **HAPI Client for Python**
@@ -26,17 +25,17 @@
 ```
 
 The optional [hapiplot package](https://github.com/hapi-server/plot-python) provides basic preview plotting capabilities of data from a HAPI server. The [Plotting section](https://colab.research.google.com/github/hapi-server/client-python-notebooks/blob/master/hapi_demo.ipynb#plotting) of the `hapiclient` Jupyter Notebook shows how to plot the output of `hapiclient` using many other plotting libraries.
 
 To install `hapiplot`, use
 
 ```bash
-pip install hapiplot --upgrade
+python -m pip install hapiplot --upgrade
 # or
-pip install 'git+https://github.com/hapi-server/plot-python' --upgrade
+python -m pip install 'git+https://github.com/hapi-server/plot-python' --upgrade
 ```
 
 See the [Appendix](#appendix) for a fail-safe installation method.
 
 # Basic Example
 
 ```python
@@ -93,26 +92,26 @@
 
 The HAPI client data model is intentionally basic. There is an ongoing discussion of a data model for Heliophysics data among the [PyHC community](https://heliopython.org/). When this data model is complete, a function that converts `data` and `meta` to that data model will be included in the `hapiclient` package.
 
 # Development
 
 ```bash
 git clone https://github.com/hapi-server/client-python
-cd client-python; pip install -e .
+cd client-python; python -m pip install -e .
 ```
 
 or, create an isolated Anaconda installation (downloads and installs latest Miniconda3) using
 
 ``` bash
 make install PYTHON=python3.6
 # Execute command displayed to activate isolated environment
 ```
 
 The command `pip install -e .` creates symlinks so that the local package is
-used instead of an installed package. You may need to execute `pip uninstall hapiclient` to ensure the local package is used. To check the version installed, use `pip list | grep hapiclient`.
+used instead of an installed package. You may need to execute `python -m pip uninstall hapiclient` to ensure the local package is used. To check the version installed, use `python -m pip list | grep hapiclient`.
 
 To run tests before a commit, execute
 
 ```bash
 make repository-test
 ```
 
@@ -123,32 +122,7 @@
 test_reader_short()
 ```
 
 # Contact
 
 Submit bug reports and feature requests on the [repository issue
 tracker](https://github.com/hapi-server/client-python/issues>).
-
-# Appendix
-
-Fail-safe installation
-
-Python command line:
-
-```python
-import os
-print(os.popen("pip install hapiclient").read())
-```
-
-The above executes and displays the output of the operating system
-command `pip install hapiclient` using the shell environment
-associated with that installation of Python.
-
-This method addresses a problem that is sometimes encountered when
-attempting to use `pip` packages in Anaconda. To use a `pip` package
-in Anaconda, one must use the version of `pip` installed with Anaconda
-(it is usually under a subdirectory with the name `anaconda/`) as
-opposed to the one installed with the operating system. To see the
-location of ``pip`` used in a given Python session, enter
-`print(os.popen("which pip").read())`.
-
-
```

### Comparing `hapiclient-0.2.5/README.md` & `hapiclient-0.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ```
 
 The optional [hapiplot package](https://github.com/hapi-server/plot-python) provides basic preview plotting capabilities of data from a HAPI server. The [Plotting section](https://colab.research.google.com/github/hapi-server/client-python-notebooks/blob/master/hapi_demo.ipynb#plotting) of the `hapiclient` Jupyter Notebook shows how to plot the output of `hapiclient` using many other plotting libraries.
 
 To install `hapiplot`, use
 
 ```bash
-pip install hapiplot --upgrade
+python -m pip install hapiplot --upgrade
 # or
-pip install 'git+https://github.com/hapi-server/plot-python' --upgrade
+python -m pip install 'git+https://github.com/hapi-server/plot-python' --upgrade
 ```
 
 See the [Appendix](#appendix) for a fail-safe installation method.
 
 # Basic Example
 
 ```python
@@ -81,26 +81,26 @@
 
 The HAPI client data model is intentionally basic. There is an ongoing discussion of a data model for Heliophysics data among the [PyHC community](https://heliopython.org/). When this data model is complete, a function that converts `data` and `meta` to that data model will be included in the `hapiclient` package.
 
 # Development
 
 ```bash
 git clone https://github.com/hapi-server/client-python
-cd client-python; pip install -e .
+cd client-python; python -m pip install -e .
 ```
 
 or, create an isolated Anaconda installation (downloads and installs latest Miniconda3) using
 
 ``` bash
 make install PYTHON=python3.6
 # Execute command displayed to activate isolated environment
 ```
 
 The command `pip install -e .` creates symlinks so that the local package is
-used instead of an installed package. You may need to execute `pip uninstall hapiclient` to ensure the local package is used. To check the version installed, use `pip list | grep hapiclient`.
+used instead of an installed package. You may need to execute `python -m pip uninstall hapiclient` to ensure the local package is used. To check the version installed, use `python -m pip list | grep hapiclient`.
 
 To run tests before a commit, execute
 
 ```bash
 make repository-test
 ```
 
@@ -111,30 +111,7 @@
 test_reader_short()
 ```
 
 # Contact
 
 Submit bug reports and feature requests on the [repository issue
 tracker](https://github.com/hapi-server/client-python/issues>).
-
-# Appendix
-
-Fail-safe installation
-
-Python command line:
-
-```python
-import os
-print(os.popen("pip install hapiclient").read())
-```
-
-The above executes and displays the output of the operating system
-command `pip install hapiclient` using the shell environment
-associated with that installation of Python.
-
-This method addresses a problem that is sometimes encountered when
-attempting to use `pip` packages in Anaconda. To use a `pip` package
-in Anaconda, one must use the version of `pip` installed with Anaconda
-(it is usually under a subdirectory with the name `anaconda/`) as
-opposed to the one installed with the operating system. To see the
-location of ``pip`` used in a given Python session, enter
-`print(os.popen("which pip").read())`.
```

### Comparing `hapiclient-0.2.5/hapiclient/hapi.py` & `hapiclient-0.2.6/hapiclient/hapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     return opts
 
 
 def hapi(*args, **kwargs):
     """Request data from a HAPI server.
 
-    Version: 0.2.5
+    Version: 0.2.6
 
 
     Examples
     ----------
     `Jupyter Notebook <https://colab.research.google.com/drive/11Zy99koiE90JKJ4u_KPTaEBMQFzbfU3P?usp=sharing>`_
 
     Parameters
@@ -190,18 +190,18 @@
         always ends with ``/hapi``).
     dataset: str
         A string specifying a dataset from a `server`
     parameters: str
         A comma-separated list of parameters in `dataset`
     start: str
         The start time of the requested data
-    stop: str
+    stop: str or None
         The end time of the requested data; end times are exclusive - the
         last data record returned by a HAPI server should have a timestamp
-        before `start`.
+        before `start`. If `None`, `stopDate` is used.
     options: dict
             `logging` (``False``) - Log to console
 
             `cache` (``True``) - Save responses and processed responses in cachedir
 
             `cachedir` (``'./hapi-data'``)
 
@@ -333,15 +333,15 @@
     if nin > 3:
         START = args[3]
         if START[-1] != 'Z':
             # TODO: Consider warning.
             START = START + 'Z'
     if nin > 4:
         STOP = args[4]
-        if STOP[-1] != 'Z':
+        if STOP is not None and STOP[-1] != 'Z':
             # TODO: Consider warning.
             STOP = STOP + 'Z'
 
     # Override defaults
     opts = setopts(hapiopts(), kwargs)
 
     assert (opts['logging'] in [True, False]), "logging keyword must be True of False"
@@ -418,14 +418,20 @@
         # is returned.
         fname_root = request2path(SERVER, DATASET, '', '', '', opts['cachedir'])
         fnamejson = fname_root + '.json'
         fnamepkl = fname_root + '.pkl'
 
         if nin == 5:  # Data requested
 
+            if STOP is None:
+                log('STOP was given as None. Getting stopDate for dataset.', opts)
+                meta = hapi(SERVER, DATASET)
+                STOP = meta['stopDate']
+                log('Using STOP = {STOP}', opts)
+
             tic_totalTime = time.time()
 
             # URL to get CSV (will be used if binary response is not available)
             urlcsv = SERVER + '/data?id=' + DATASET + '&parameters=' + \
                      PARAMETERS + '&time.min=' + START + '&time.max=' + STOP
             # URL for binary request
             urlbin = urlcsv + '&format=binary'
@@ -724,88 +730,112 @@
                 urlretrieve(urlbin, fnamebin)
                 toc0 = time.time() - tic0
                 log('Reading and parsing %s' % fnamebin.replace(urld + '/', ''), opts)
                 tic = time.time()
                 try:
                     data = np.fromfile(fnamebin, dtype=dt)
                 except:
-                    error('Could not read response from {}'.format(urlbin))
+                    error('Malformed response? Could not read: {}'.format(urlbin))
             else:
                 from io import BytesIO
                 log('Writing %s to buffer' % urlbin.replace(urld + '/', ''), opts)
                 tic0 = time.time()
                 buff = BytesIO(urlopen(urlbin).read())
                 toc0 = time.time() - tic0
                 log('Parsing BytesIO buffer.', opts)
                 tic = time.time()
                 try:
                     data = np.frombuffer(buff.read(), dtype=dt)
                 except:
-                    error('Could not read response from {}'.format(urlbin))
+                    error('Malformed response? Could not read: {}'.format(urlbin))
+
 
             # Handle Unicode
             time_name = meta['parameters'][0]['name']
             datanew = np.ndarray(shape=data[time_name].shape, dtype=dto)
             for i in range(0, len(dto)):
                 name = meta['parameters'][i]['name']
                 if sys.version_info[0] < 3:
                     # str() here is needed for Python 2.7. Numpy does not allow
                     # Unicode names in this version and if a dt is created
                     # with Unicode, it automatically converts Unicode chars to
                     # slash encoded ASCII.
                     name = str(name)
-                if isinstance(dt[i][1], str) and 'U' in dto[i][1]:
+                if data[name].size > 0 and isinstance(dt[i][1], str) and 'U' in dto[i][1]:
                     # Decode data.
                     datanew[name] = np.char.decode(data[name])
                 else:
                     datanew[name] = data[name]
             data = datanew
 
         else:
             # HAPI CSV
 
+            file_empty = False
+
             if opts["cache"]:
                 log('Writing %s to %s' % (urlcsv, fnamecsv.replace(urld + '/', '')), opts)
                 tic0 = time.time()
                 urlretrieve(urlcsv, fnamecsv)
                 toc0 = time.time() - tic0
                 log('Reading and parsing %s' % fnamecsv.replace(urld + '/', ''), opts)
                 tic = time.time()
+                if os.path.getsize(fnamecsv) == 0:
+                    file_empty = True
+                    data = np.array([], dtype=dt)
             else:
                 from io import StringIO
-                #log('Writing %s to buffer' % urlcsv.replace(urld + '/', ''), opts)
+                log('Writing %s to buffer' % urlcsv.replace(urld + '/', ''), opts)
                 tic0 = time.time()
                 fnamecsv = StringIO(urlopen(urlcsv).read().decode())
+                fnamecsv.seek(0, os.SEEK_END)
+                if fnamecsv.tell() == 0:
+                    file_empty = True
+                    data = np.array([], dtype=dt)
+                else:
+                    fnamecsv.seek(0)
                 toc0 = time.time() - tic0
                 log('Parsing StringIO buffer.', opts)
                 tic = time.time()
 
-            if not missing_length:
-                # All string and isotime parameters have a length in metadata.
-                if opts['method'] == 'numpy':
-                    data = np.genfromtxt(fnamecsv, dtype=dt, delimiter=',',
-                                            replace_space=' ',
-                                            deletechars='', encoding='utf-8')
-                if opts['method'] == '' or opts['method'] == 'pandas':
-                    # Read file into Pandas DataFrame
-                    df = pandas.read_csv(fnamecsv, sep=',', header=None,
-                                            encoding='utf-8')
-                    # Allocate output N-D array (It is not possible to pass dtype=dt
-                    # as computed to pandas.read_csv; pandas dtype is different
-                    # from numpy's dtype.)
-                    data = np.ndarray(shape=(len(df)), dtype=dt)
-                    # Insert data from dataframe 'df' columns into N-D array 'data'
-                    for i in range(0, len(pnames)):
-                        shape = np.append(len(data), psizes[i])
-                        # In numpy 1.8.2 and Python 2.7, this throws an error
-                        # for no apparent reason. Works as expected in numpy 1.10.4
-                        data[pnames[i]] = np.squeeze(
-                            np.reshape(df.values[:, np.arange(cols[i][0], cols[i][1] + 1)], shape))
-            else:
-                data = parse_missing_length(fnamecsv, dt, cols, psizes, pnames, ptypes, opts)
+            if file_empty == False:
+                if not missing_length:
+                    # All string and isotime parameters have a length in metadata.
+                    if opts['method'] == 'numpy':
+                        try:
+                            data = np.genfromtxt(fnamecsv,
+                                                 dtype=dt,
+                                                 delimiter=',',
+                                                 replace_space=' ',
+                                                 deletechars='',
+                                                 encoding='utf-8')
+                        except:
+                            error('Malformed response? Could not read response: {}'.format(urlcsv))
+                    if opts['method'] == '' or opts['method'] == 'pandas':
+                        # Read file into Pandas DataFrame
+                        try:
+                            df = pandas.read_csv(fnamecsv,
+                                                 sep=',',
+                                                 header=None,
+                                                 encoding='utf-8')
+                        except:
+                            error('Malformed response? Could not read response: {}'.format(urlcsv))
+                        # Allocate output N-D array (It is not possible to pass dtype=dt
+                        # as computed to pandas.read_csv; pandas dtype is different
+                        # from numpy's dtype.)
+                        data = np.ndarray(shape=(len(df)), dtype=dt)
+                        # Insert data from dataframe 'df' columns into N-D array 'data'
+                        for i in range(0, len(pnames)):
+                            shape = np.append(len(data), psizes[i])
+                            # In numpy 1.8.2 and Python 2.7, this throws an error
+                            # for no apparent reason. Works as expected in numpy 1.10.4
+                            data[pnames[i]] = np.squeeze(
+                                np.reshape(df.values[:, np.arange(cols[i][0], cols[i][1] + 1)], shape))
+                else:
+                    data = parse_missing_length(fnamecsv, dt, cols, psizes, pnames, ptypes, opts)
 
         toc = time.time() - tic
 
         # Extra metadata associated with request will be saved in
         # a pkl file with same base name as npy data file.
         meta.update({"x_server": SERVER})
         meta.update({"x_dataset": DATASET})
```

### Comparing `hapiclient-0.2.5/hapiclient/hapitime.py` & `hapiclient-0.2.6/hapiclient/hapitime.py`

 * *Files 7% similar despite different names*

```diff
@@ -238,20 +238,17 @@
     if 'allow_missing_Z' in kwargs and kwargs['allow_missing_Z'] == True:
         allow_missing_Z = True
 
     opts = kwargs.copy()
 
     if type(Time) == list:
         Time = np.asarray(Time)
-    if type(Time) == str or type(Time) == bytes:
-        Time = np.asarray([Time])
 
     if type(Time) != np.ndarray:
-        error('Problem with time data.' + '\n')
-        return
+        Time = np.asarray([Time])
 
     if Time.size == 0:
         error('Time array is empty.' + '\n')
         return
 
     reshape = False
     if Time.shape[0] != Time.size:
@@ -325,7 +322,45 @@
     log("Manual processing time = %.4fs, Input = %s, fmt = %s" % \
         (toc, Time[0], fmt), opts)
 
     if reshape:
         pythonDateTime = np.reshape(pythonDateTime, shape)
 
     return pythonDateTime
+
+
+def datetime2hapitime(dts):
+    """Convert Python datetime object(s) to ISO 8601 string(s)
+
+    Typical usage:
+    ::
+
+        from hapiclient import datetime2hapitime
+        import datetime
+        dts = [datetime.datetime(2000, 1, 1), datetime.datetime(2000, 1, 2)]
+        hapi_times = datetime2hapitime(dts)
+        print(hapi_times) 
+        # ['2000-01-01T00:00:00.000000Z', '2000-01-02T00:00:00.000000Z']
+
+    Parameter
+    ---------
+    dts:
+    - A Python datetime object
+    - A list of Python datetime object(s)
+
+    Returns
+    -------
+    - A ISO 8601 string (if input is Python datetime object)
+    - A list of ISO 8601 strings (if input is list of Python datetime object)
+    """
+
+    single = False
+    if isinstance(dts, list) == False:
+        single = True
+        dts = [dts]
+
+    hapi_times = [dt.strftime('%Y-%m-%dT%H:%M:%S.%fZ') for dt in dts]
+
+    if single == True:
+        return hapi_times[0]
+    else:
+        return hapi_times
```

### Comparing `hapiclient-0.2.5/hapiclient/test/compare.py` & `hapiclient-0.2.6/hapiclient/test/compare.py`

 * *Files identical despite different names*

### Comparing `hapiclient-0.2.5/hapiclient/test/test_chunking.py` & `hapiclient-0.2.6/hapiclient/test/test_chunking.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # Python 2-compatable dict concatenation.
     # https://treyhunner.com/2016/02/how-to-merge-dictionaries-in-python/
     d12 = d1.copy()
     d12.update(d2)
     return d12
 
 
-opts0 = {'logging': hapi_logging, 'usecache': False, 'cache': False}
+opts0 = {'logging': hapi_logging, 'usecache': False, 'cache': True, 'format': 'csv'}
 
 # Test dict.
 # Key indicates chunk size to use for chunk test
 td = {
         "P1Y": {
                 "__comment": "dataset3 has cadence of P1D",
                 "server": server,
```

### Comparing `hapiclient-0.2.5/hapiclient/test/test_hapi.py` & `hapiclient-0.2.6/hapiclient/test/test_hapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 @pytest.mark.short
 def test_unicode():
 
     from hapiclient.util import warning, unicode_error_message
 
     server     = 'http://hapi-server.org/servers/TestData3.1/hapi';
     #datasets   = ["dataset1", "dataset1-Zα☃"]
-    datasets   = ["dataset1-Zα☃"]
+    datasets   = ["dataset1-Aα☃"]
     #datasets = ["dataset1"]
 
     run = 'short'
 
     opts = {
                 'logging': True,
                 'cachedir': '/tmp/hapi-data',
@@ -286,14 +286,43 @@
     opts = {'logging': logging, 'cachedir': '/tmp/hapi-data', 'cache': True, 'usecache': False}
     assert compare.read(server, dataset, 'scalar,vector,spectra', run, opts)
 
     opts = {'logging': logging, 'cachedir': '/tmp/hapi-data', 'cache': False, 'usecache': True}
     assert compare.read(server, dataset, 'scalar,vector,spectra', run, opts)
 
 
+@pytest.mark.short
+def test_none_stop():
+    import numpy as np
+
+    from hapiclient import hapi
+    from hapiclient import hapitime2datetime
+    from hapiclient import datetime2hapitime
+    from datetime import timedelta
+
+    server     = 'http://hapi-server.org/servers/TestData2.0/hapi'
+    dataset    = 'dataset1'
+    parameters = 'scalar'
+
+    meta = hapi(server, dataset)
+    stop = meta['stopDate']
+    stop_dt = hapitime2datetime(stop)[0]
+
+    start_dt = stop_dt - timedelta(minutes=1)
+    start = datetime2hapitime(start_dt)
+
+    data1, meta1 = hapi(server, dataset, parameters, start, None)
+
+    data2, meta2 = hapi(server, dataset, parameters, start, stop)
+
+    allequal = True
+    for name in data1.dtype.names:
+        assert np.array_equal(data1[name], data2[name])
+
+
 def runall():
     from hapiclient.test import test_hapi
     for i in dir(test_hapi):
         item = getattr(test_hapi,i)
         if callable(item) and item.__name__.startswith("test_"):
             if item.__name__ == 'test_reader_long':
                 continue
@@ -301,10 +330,11 @@
             item()
 
 
 if __name__ == '__main__':
     #runall()
     #test_dataset()
     #test_reader_short()
-    test_unicode()
+    #test_unicode()
     #test_request2path()
-    #test_reader_long()
+    test_reader_short()
+    #test_none_stop()
```

### Comparing `hapiclient-0.2.5/hapiclient/test/test_hapitime2datetime.py` & `hapiclient-0.2.6/hapiclient/test/test_hapitime2datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import os
 import numpy as np
 
 from hapiclient import hapitime2datetime
 from hapiclient.util import log
 
 # Create empty file
-logfile = os.path.splitext(__file__)[0] + "log"
-with open(logfile + ".log", "w") as f: pass
-logging = open(logfile + "log", "a")
+logfile = os.path.splitext(__file__)[0] + ".log"
+with open(logfile, "w") as f: pass
+logging = open(logfile, "a")
 
 expected = '1970-01-01T00:00:00.000000Z'
 
 def test_api():
 
 	log("API test.", {'logging': logging})
```

### Comparing `hapiclient-0.2.5/hapiclient/test/test_hapitime_reformat.py` & `hapiclient-0.2.6/hapiclient/test/test_hapitime_reformat.py`

 * *Files identical despite different names*

### Comparing `hapiclient-0.2.5/hapiclient/util.py` & `hapiclient-0.2.6/hapiclient/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     #line = stack()[1][2]
 
     fname = path.basename(fname)
 
     def prefix():
         import platform
-        prefix = "\x1b[31m[0;31mHAPIWarning:\x1b[0m "
+        prefix = "\x1b[31mHAPIWarning:\x1b[0m "
         if platform.system() == 'Windows' and pythonshell() == 'shell':
             prefix = "HAPIWarning: "        
 
         return prefix
 
     # Custom warning format function
     def _warning(message, category=UserWarning, filename='', lineno=-1, file=None, line=''):
```

### Comparing `hapiclient-0.2.5/hapiclient.egg-info/PKG-INFO` & `hapiclient-0.2.6/hapiclient.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: hapiclient
-Version: 0.2.5
+Version: 0.2.6
 Summary: Interface to Heliophysics data server API
 Home-page: http://pypi.python.org/pypi/hapiclient/
 Author: Bob Weigel
 Author-email: rweigel@gmu.edu
 License: LICENSE.txt
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![DOI](https://zenodo.org/badge/93170857.svg)](https://zenodo.org/badge/latestdoi/93170857)
 [![Build Status](https://app.travis-ci.com/hapi-server/client-python.svg?branch=master)](https://app.travis-ci.com/hapi-server/client-python)
 
 **HAPI Client for Python**
@@ -26,17 +25,17 @@
 ```
 
 The optional [hapiplot package](https://github.com/hapi-server/plot-python) provides basic preview plotting capabilities of data from a HAPI server. The [Plotting section](https://colab.research.google.com/github/hapi-server/client-python-notebooks/blob/master/hapi_demo.ipynb#plotting) of the `hapiclient` Jupyter Notebook shows how to plot the output of `hapiclient` using many other plotting libraries.
 
 To install `hapiplot`, use
 
 ```bash
-pip install hapiplot --upgrade
+python -m pip install hapiplot --upgrade
 # or
-pip install 'git+https://github.com/hapi-server/plot-python' --upgrade
+python -m pip install 'git+https://github.com/hapi-server/plot-python' --upgrade
 ```
 
 See the [Appendix](#appendix) for a fail-safe installation method.
 
 # Basic Example
 
 ```python
@@ -93,26 +92,26 @@
 
 The HAPI client data model is intentionally basic. There is an ongoing discussion of a data model for Heliophysics data among the [PyHC community](https://heliopython.org/). When this data model is complete, a function that converts `data` and `meta` to that data model will be included in the `hapiclient` package.
 
 # Development
 
 ```bash
 git clone https://github.com/hapi-server/client-python
-cd client-python; pip install -e .
+cd client-python; python -m pip install -e .
 ```
 
 or, create an isolated Anaconda installation (downloads and installs latest Miniconda3) using
 
 ``` bash
 make install PYTHON=python3.6
 # Execute command displayed to activate isolated environment
 ```
 
 The command `pip install -e .` creates symlinks so that the local package is
-used instead of an installed package. You may need to execute `pip uninstall hapiclient` to ensure the local package is used. To check the version installed, use `pip list | grep hapiclient`.
+used instead of an installed package. You may need to execute `python -m pip uninstall hapiclient` to ensure the local package is used. To check the version installed, use `python -m pip list | grep hapiclient`.
 
 To run tests before a commit, execute
 
 ```bash
 make repository-test
 ```
 
@@ -123,32 +122,7 @@
 test_reader_short()
 ```
 
 # Contact
 
 Submit bug reports and feature requests on the [repository issue
 tracker](https://github.com/hapi-server/client-python/issues>).
-
-# Appendix
-
-Fail-safe installation
-
-Python command line:
-
-```python
-import os
-print(os.popen("pip install hapiclient").read())
-```
-
-The above executes and displays the output of the operating system
-command `pip install hapiclient` using the shell environment
-associated with that installation of Python.
-
-This method addresses a problem that is sometimes encountered when
-attempting to use `pip` packages in Anaconda. To use a `pip` package
-in Anaconda, one must use the version of `pip` installed with Anaconda
-(it is usually under a subdirectory with the name `anaconda/`) as
-opposed to the one installed with the operating system. To see the
-location of ``pip`` used in a given Python session, enter
-`print(os.popen("which pip").read())`.
-
-
```

### Comparing `hapiclient-0.2.5/setup.py` & `hapiclient-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         # https://docs.pytest.org/en/stable/py27-py34-deprecation.html
         # Perhaps old version of pip causes this?
         install_requires.append("pytest")
 
 # version is modified by misc/version.py (executed from Makefile). Do not edit.
 setup(
     name='hapiclient',
-    version='0.2.5',
+    version='0.2.6',
     author='Bob Weigel',
     author_email='rweigel@gmu.edu',
     packages=find_packages(),
     url='http://pypi.python.org/pypi/hapiclient/',
     license='LICENSE.txt',
     description='Interface to Heliophysics data server API',
     long_description=open('README.md').read(),
```

