# Comparing `tmp/srslib-0.1.4.tar.gz` & `tmp/srslib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/srslib-0.1.4.tar", last modified: Fri May 25 02:41:20 2018, max compression
+gzip compressed data, was "srslib-0.1.5.tar", last modified: Fri May 10 21:25:32 2024, max compression
```

## Comparing `srslib-0.1.4.tar` & `srslib-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0 chuan     (1000) chuan     (1000)        0 2018-05-25 02:41:20.000000 srslib-0.1.4/
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)     3567 2018-05-25 02:41:20.000000 srslib-0.1.4/PKG-INFO
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)     1838 2017-08-18 01:35:37.000000 srslib-0.1.4/README.rst
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)       63 2018-05-25 02:41:20.000000 srslib-0.1.4/setup.cfg
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)     2818 2018-05-25 02:35:41.000000 srslib-0.1.4/setup.py
-drwxrwxrwx   0 chuan     (1000) chuan     (1000)        0 2018-05-25 02:41:20.000000 srslib-0.1.4/srslib.egg-info/
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)     3567 2018-05-25 02:41:20.000000 srslib-0.1.4/srslib.egg-info/PKG-INFO
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)      188 2018-05-25 02:41:20.000000 srslib-0.1.4/srslib.egg-info/SOURCES.txt
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)        1 2018-05-25 02:41:20.000000 srslib-0.1.4/srslib.egg-info/dependency_links.txt
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)       34 2018-05-25 02:41:20.000000 srslib-0.1.4/srslib.egg-info/requires.txt
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)        7 2018-05-25 02:41:20.000000 srslib-0.1.4/srslib.egg-info/top_level.txt
--rw-rw-rw-   0 chuan     (1000) chuan     (1000)    14041 2018-05-25 02:30:45.000000 srslib-0.1.4/srslib.py
+drwxr-xr-x   0 chuan     (1000) chuan     (1000)        0 2024-05-10 21:25:32.604339 srslib-0.1.5/
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)    11357 2017-07-28 06:44:27.000000 srslib-0.1.5/LICENSE
+-rw-r--r--   0 chuan     (1000) chuan     (1000)     3004 2024-05-10 21:25:32.604339 srslib-0.1.5/PKG-INFO
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)     1790 2024-05-10 21:20:36.000000 srslib-0.1.5/README.rst
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)       63 2024-05-10 21:25:32.604339 srslib-0.1.5/setup.cfg
+-rw-r--r--   0 chuan     (1000) chuan     (1000)     2818 2024-05-10 21:24:55.000000 srslib-0.1.5/setup.py
+drwxr-xr-x   0 chuan     (1000) chuan     (1000)        0 2024-05-10 21:25:32.604339 srslib-0.1.5/srslib.egg-info/
+-rw-r--r--   0 chuan     (1000) chuan     (1000)     3004 2024-05-10 21:25:32.000000 srslib-0.1.5/srslib.egg-info/PKG-INFO
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)      196 2024-05-10 21:25:32.000000 srslib-0.1.5/srslib.egg-info/SOURCES.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        1 2024-05-10 21:25:32.000000 srslib-0.1.5/srslib.egg-info/dependency_links.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)       34 2024-05-10 21:25:32.000000 srslib-0.1.5/srslib.egg-info/requires.txt
+-rw-rw-r--   0 chuan     (1000) chuan     (1000)        7 2024-05-10 21:25:32.000000 srslib-0.1.5/srslib.egg-info/top_level.txt
+-rw-r--r--   0 chuan     (1000) chuan     (1000)    14045 2024-05-10 21:19:57.000000 srslib-0.1.5/srslib.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `srslib-0.1.4/PKG-INFO` & `srslib-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: srslib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sender Rewriting Scheme (SRS) library for Python
 Home-page: https://github.com/jichu4n/srslib
+Download-URL: https://github.com/jichu4n/srslib/archive/0.1.5.tar.gz
 Author: Chuan Ji
 Author-email: jichu4n@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/jichu4n/srslib/archive/0.1.4.tar.gz
-Description: srslib - Sender Rewriting Scheme (SRS) library for Python
-        =========================================================
-        
-        **srslib** is a modern Python implementation of the `Sender Rewriting
-        Scheme (SRS) <https://en.wikipedia.org/wiki/Sender_Rewriting_Scheme>`__.
-        
-        Highlights:
-        
-        -  Compatible with Python 2.7 and 3.x;
-        -  Implements the standard "Guarded" SRS scheme as described in the
-           `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__;
-        -  Simple to use and understand.
-        
-        Installation
-        ------------
-        
-        .. code:: sh
-        
-            pip install srslib
-        
-        Example Usage
-        -------------
-        
-        .. code:: py
-        
-            import srslib
-        
-            srs = srslib.SRS('my_secret_key')
-        
-            # Rewrites an email from alice@A.com to B.com
-            rewritten_addr = srs.forward('alice@A.com', 'B.com')
-            # => 'SRS0=ZPM1=67=A.com=alice@B.com'
-        
-            # Reverse it to get the address to bounce to.
-            try:
-              bounce_addr = srs.reverse(rewritten_addr)
-              # => 'alice@A.com'
-            except srslib.Error as e:
-              ...  # Handle errors
-        
-        Documentation
-        -------------
-        
-        The full documentation for **srslib** lives at
-        https://srslib.readthedocs.io/.
-        
-        Implementation
-        --------------
-        
-        This library is a clean re-implementation of SRS in modern Python based
-        on the `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__, and
-        taking inspiration from the canonical
-        `libsrs2 <https://github.com/shevek/libsrs2>`__ C implementation and the
-        older `pysrs <http://www.bmsi.com/python/pysrs.html>`__ library (which
-        itself is based on the
-        `Mail::SRS <http://search.cpan.org/~shevek/Mail-SRS-0.31/lib/Mail/SRS.pm>`__
-        Perl package).
-        
-        Compared to these two libraries, **srslib**
-        
-        -  ... is a clean, modern, pure-Python implementation and supports
-           Python 3.x;
-        -  ... discards baggage from Mail::SRS around legacy schemes and
-           settings.
-        
-        License
-        -------
-        
-        Licensed under the Apache License, Version 2.0.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
@@ -91,7 +20,76 @@
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Security
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+Requires-Dist: typing; python_version < "3.5"
+
+srslib - Sender Rewriting Scheme (SRS) library for Python
+=========================================================
+
+**srslib** is a modern Python implementation of the `Sender Rewriting
+Scheme (SRS) <https://en.wikipedia.org/wiki/Sender_Rewriting_Scheme>`__.
+
+-  Compatible with Python 2.7 and 3.x
+-  Implements the standard "Guarded" SRS scheme as described in the
+   `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__
+
+Installation
+------------
+
+.. code:: sh
+
+    pip install srslib
+
+Example Usage
+-------------
+
+.. code:: py
+
+    import srslib
+
+    srs = srslib.SRS('my_secret_key')
+
+    # Rewrites an email from alice@A.com to B.com
+    rewritten_addr = srs.forward('alice@A.com', 'B.com')
+    # => 'SRS0=ZPM1=67=A.com=alice@B.com'
+
+    # Reverse it to get the address to bounce to.
+    try:
+      bounce_addr = srs.reverse(rewritten_addr)
+      # => 'alice@A.com'
+    except srslib.Error as e:
+      ...  # Handle errors
+
+Documentation
+-------------
+
+The full documentation for **srslib** lives at
+https://srslib.readthedocs.io/.
+
+Implementation
+--------------
+
+This library is a clean re-implementation of SRS in modern Python based
+on the `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__, and
+taking inspiration from the canonical
+`libsrs2 <https://github.com/shevek/libsrs2>`__ C implementation and the
+older `pysrs <http://www.bmsi.com/python/pysrs.html>`__ library (which
+itself is based on the
+`Mail::SRS <http://search.cpan.org/~shevek/Mail-SRS-0.31/lib/Mail/SRS.pm>`__
+Perl package).
+
+Compared to these two libraries, **srslib**
+
+-  ... is a clean, modern, pure-Python implementation and supports
+   Python 3.x;
+-  ... discards baggage from Mail::SRS around legacy schemes and
+   settings.
+
+License
+-------
+
+Licensed under the Apache License, Version 2.0.
```

### Comparing `srslib-0.1.4/README.rst` & `srslib-0.1.5/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 srslib - Sender Rewriting Scheme (SRS) library for Python
 =========================================================
 
 **srslib** is a modern Python implementation of the `Sender Rewriting
 Scheme (SRS) <https://en.wikipedia.org/wiki/Sender_Rewriting_Scheme>`__.
 
-Highlights:
-
--  Compatible with Python 2.7 and 3.x;
+-  Compatible with Python 2.7 and 3.x
 -  Implements the standard "Guarded" SRS scheme as described in the
-   `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__;
--  Simple to use and understand.
+   `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__
 
 Installation
 ------------
 
 .. code:: sh
 
     pip install srslib
```

### Comparing `srslib-0.1.4/setup.py` & `srslib-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    See the License for the specific language governing permissions and      #
 #    limitations under the License.                                           #
 #                                                                             #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 from setuptools import setup
 
-_version = '0.1.4'
+_version = '0.1.5'
 
 setup(
     name='srslib',
     version=_version,
     download_url=(
         'https://github.com/jichu4n/srslib/archive/%s.tar.gz' % _version),
     description='Sender Rewriting Scheme (SRS) library for Python',
```

### Comparing `srslib-0.1.4/srslib.egg-info/PKG-INFO` & `srslib-0.1.5/srslib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: srslib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sender Rewriting Scheme (SRS) library for Python
 Home-page: https://github.com/jichu4n/srslib
+Download-URL: https://github.com/jichu4n/srslib/archive/0.1.5.tar.gz
 Author: Chuan Ji
 Author-email: jichu4n@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/jichu4n/srslib/archive/0.1.4.tar.gz
-Description: srslib - Sender Rewriting Scheme (SRS) library for Python
-        =========================================================
-        
-        **srslib** is a modern Python implementation of the `Sender Rewriting
-        Scheme (SRS) <https://en.wikipedia.org/wiki/Sender_Rewriting_Scheme>`__.
-        
-        Highlights:
-        
-        -  Compatible with Python 2.7 and 3.x;
-        -  Implements the standard "Guarded" SRS scheme as described in the
-           `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__;
-        -  Simple to use and understand.
-        
-        Installation
-        ------------
-        
-        .. code:: sh
-        
-            pip install srslib
-        
-        Example Usage
-        -------------
-        
-        .. code:: py
-        
-            import srslib
-        
-            srs = srslib.SRS('my_secret_key')
-        
-            # Rewrites an email from alice@A.com to B.com
-            rewritten_addr = srs.forward('alice@A.com', 'B.com')
-            # => 'SRS0=ZPM1=67=A.com=alice@B.com'
-        
-            # Reverse it to get the address to bounce to.
-            try:
-              bounce_addr = srs.reverse(rewritten_addr)
-              # => 'alice@A.com'
-            except srslib.Error as e:
-              ...  # Handle errors
-        
-        Documentation
-        -------------
-        
-        The full documentation for **srslib** lives at
-        https://srslib.readthedocs.io/.
-        
-        Implementation
-        --------------
-        
-        This library is a clean re-implementation of SRS in modern Python based
-        on the `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__, and
-        taking inspiration from the canonical
-        `libsrs2 <https://github.com/shevek/libsrs2>`__ C implementation and the
-        older `pysrs <http://www.bmsi.com/python/pysrs.html>`__ library (which
-        itself is based on the
-        `Mail::SRS <http://search.cpan.org/~shevek/Mail-SRS-0.31/lib/Mail/SRS.pm>`__
-        Perl package).
-        
-        Compared to these two libraries, **srslib**
-        
-        -  ... is a clean, modern, pure-Python implementation and supports
-           Python 3.x;
-        -  ... discards baggage from Mail::SRS around legacy schemes and
-           settings.
-        
-        License
-        -------
-        
-        Licensed under the Apache License, Version 2.0.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
@@ -91,7 +20,76 @@
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Security
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+Requires-Dist: typing; python_version < "3.5"
+
+srslib - Sender Rewriting Scheme (SRS) library for Python
+=========================================================
+
+**srslib** is a modern Python implementation of the `Sender Rewriting
+Scheme (SRS) <https://en.wikipedia.org/wiki/Sender_Rewriting_Scheme>`__.
+
+-  Compatible with Python 2.7 and 3.x
+-  Implements the standard "Guarded" SRS scheme as described in the
+   `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__
+
+Installation
+------------
+
+.. code:: sh
+
+    pip install srslib
+
+Example Usage
+-------------
+
+.. code:: py
+
+    import srslib
+
+    srs = srslib.SRS('my_secret_key')
+
+    # Rewrites an email from alice@A.com to B.com
+    rewritten_addr = srs.forward('alice@A.com', 'B.com')
+    # => 'SRS0=ZPM1=67=A.com=alice@B.com'
+
+    # Reverse it to get the address to bounce to.
+    try:
+      bounce_addr = srs.reverse(rewritten_addr)
+      # => 'alice@A.com'
+    except srslib.Error as e:
+      ...  # Handle errors
+
+Documentation
+-------------
+
+The full documentation for **srslib** lives at
+https://srslib.readthedocs.io/.
+
+Implementation
+--------------
+
+This library is a clean re-implementation of SRS in modern Python based
+on the `original SRS paper <http://www.libsrs2.org/srs/srs.pdf>`__, and
+taking inspiration from the canonical
+`libsrs2 <https://github.com/shevek/libsrs2>`__ C implementation and the
+older `pysrs <http://www.bmsi.com/python/pysrs.html>`__ library (which
+itself is based on the
+`Mail::SRS <http://search.cpan.org/~shevek/Mail-SRS-0.31/lib/Mail/SRS.pm>`__
+Perl package).
+
+Compared to these two libraries, **srslib**
+
+-  ... is a clean, modern, pure-Python implementation and supports
+   Python 3.x;
+-  ... discards baggage from Mail::SRS around legacy schemes and
+   settings.
+
+License
+-------
+
+Licensed under the Apache License, Version 2.0.
```

### Comparing `srslib-0.1.4/srslib.py` & `srslib-0.1.5/srslib.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         alias_host)
 
   @classmethod
   def _split_addr(cls, addr):
     # type: (str) -> Tuple[str, str]
     """Splits an email address to (local_part, host)."""
     try:
-      local_part, host = addr.split('@')
+      local_part, host = addr.rsplit('@', 1)
     except ValueError:
       raise InvalidAddressError('Invalid from_addr address: "%s"' % addr)
     else:
       return (local_part, host)
 
   def generate_hash(self, s, secret, hash_length):
     # type: (str, bytes, int) -> str
```

