# Comparing `tmp/django_feed_reader-2.0.1b1.tar.gz` & `tmp/django_feed_reader-2.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feed_reader-2.0.1b1.tar", last modified: Sat Apr 20 09:43:37 2024, max compression
+gzip compressed data, was "django_feed_reader-2.0.1b2.tar", last modified: Sat May 11 08:34:35 2024, max compression
```

## Comparing `django_feed_reader-2.0.1b1.tar` & `django_feed_reader-2.0.1b2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.723745 django_feed_reader-2.0.1b1/
--rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django_feed_reader-2.0.1b1/LICENSE
--rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django_feed_reader-2.0.1b1/MANIFEST.in
--rw-r--r--   0 g          (501) staff       (20)     6869 2024-04-20 09:43:37.723680 django_feed_reader-2.0.1b1/PKG-INFO
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.723263 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/
--rw-r--r--   0 g          (501) staff       (20)     6869 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)     1236 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)       90 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        6 2024-04-20 09:43:37.000000 django_feed_reader-2.0.1b1/django_feed_reader.egg-info/top_level.txt
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.720103 django_feed_reader-2.0.1b1/feeds/
--rw-r--r--   0 g          (501) staff       (20)      442 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     1528 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/admin.py
--rw-r--r--   0 g          (501) staff       (20)      139 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/apps.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.720245 django_feed_reader-2.0.1b1/feeds/management/
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/management/__init__.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.720540 django_feed_reader-2.0.1b1/feeds/management/commands/
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/management/commands/__init__.py
--rw-r--r--   0 g          (501) staff       (20)      415 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/management/commands/refreshfeeds.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-20 09:43:37.723119 django_feed_reader-2.0.1b1/feeds/migrations/
--rw-r--r--   0 g          (501) staff       (20)     3384 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0001_initial.py
--rw-r--r--   0 g          (501) staff       (20)      395 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0002_auto_20190604_0845.py
--rw-r--r--   0 g          (501) staff       (20)      407 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0003_post_image_url.py
--rw-r--r--   0 g          (501) staff       (20)      513 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0004_webproxy.py
--rw-r--r--   0 g          (501) staff       (20)      385 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0005_source_description.py
--rw-r--r--   0 g          (501) staff       (20)      921 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0006_auto_20190901_1644.py
--rw-r--r--   0 g          (501) staff       (20)     1098 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0007_auto_20210502_0716.py
--rw-r--r--   0 g          (501) staff       (20)      419 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0008_allow_longer_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)      576 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
--rw-r--r--   0 g          (501) staff       (20)      626 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py
--rw-r--r--   0 g          (501) staff       (20)      439 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0011_alter_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)     1383 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0012_source_last_read_subscription.py
--rw-r--r--   0 g          (501) staff       (20)      474 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
--rw-r--r--   0 g          (501) staff       (20)      561 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0014_post_json_source_json.py
--rw-r--r--   0 g          (501) staff       (20)      393 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/0015_source_alt_url.py
--rw-r--r--   0 g          (501) staff       (20)        0 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/migrations/__init__.py
--rw-r--r--   0 g          (501) staff       (20)    17419 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/models.py
--rw-r--r--   0 g          (501) staff       (20)    34044 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/tests.py
--rw-r--r--   0 g          (501) staff       (20)    14197 2024-04-20 09:41:43.000000 django_feed_reader-2.0.1b1/feeds/utils.py
--rw-r--r--   0 g          (501) staff       (20)    20969 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/utils_internal.py
--rw-r--r--   0 g          (501) staff       (20)       63 2024-04-18 21:35:29.000000 django_feed_reader-2.0.1b1/feeds/views.py
--rw-r--r--   0 g          (501) staff       (20)       38 2024-04-20 09:43:37.723925 django_feed_reader-2.0.1b1/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      903 2024-04-20 09:43:34.000000 django_feed_reader-2.0.1b1/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-05-11 08:34:35.505271 django_feed_reader-2.0.1b2/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django_feed_reader-2.0.1b2/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django_feed_reader-2.0.1b2/MANIFEST.in
+-rw-r--r--   0 g          (501) staff       (20)     6869 2024-05-11 08:34:35.505205 django_feed_reader-2.0.1b2/PKG-INFO
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-05-11 08:34:35.504967 django_feed_reader-2.0.1b2/django_feed_reader.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)     6869 2024-05-11 08:34:35.000000 django_feed_reader-2.0.1b2/django_feed_reader.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     1236 2024-05-11 08:34:35.000000 django_feed_reader-2.0.1b2/django_feed_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-05-11 08:34:35.000000 django_feed_reader-2.0.1b2/django_feed_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)       90 2024-05-11 08:34:35.000000 django_feed_reader-2.0.1b2/django_feed_reader.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        6 2024-05-11 08:34:35.000000 django_feed_reader-2.0.1b2/django_feed_reader.egg-info/top_level.txt
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-05-11 08:34:35.501349 django_feed_reader-2.0.1b2/feeds/
+-rw-r--r--   0 g          (501) staff       (20)      442 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     1528 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/admin.py
+-rw-r--r--   0 g          (501) staff       (20)      139 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/apps.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-05-11 08:34:35.501513 django_feed_reader-2.0.1b2/feeds/management/
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/management/__init__.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-05-11 08:34:35.501845 django_feed_reader-2.0.1b2/feeds/management/commands/
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/management/commands/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)      870 2024-05-11 06:38:11.000000 django_feed_reader-2.0.1b2/feeds/management/commands/refreshfeeds.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-05-11 08:34:35.504821 django_feed_reader-2.0.1b2/feeds/migrations/
+-rw-r--r--   0 g          (501) staff       (20)     3384 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0001_initial.py
+-rw-r--r--   0 g          (501) staff       (20)      395 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0002_auto_20190604_0845.py
+-rw-r--r--   0 g          (501) staff       (20)      407 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0003_post_image_url.py
+-rw-r--r--   0 g          (501) staff       (20)      513 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0004_webproxy.py
+-rw-r--r--   0 g          (501) staff       (20)      385 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0005_source_description.py
+-rw-r--r--   0 g          (501) staff       (20)      921 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0006_auto_20190901_1644.py
+-rw-r--r--   0 g          (501) staff       (20)     1098 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0007_auto_20210502_0716.py
+-rw-r--r--   0 g          (501) staff       (20)      419 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0008_allow_longer_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)      576 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
+-rw-r--r--   0 g          (501) staff       (20)      626 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0010_enclosure_description_enclosure_medium.py
+-rw-r--r--   0 g          (501) staff       (20)      439 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0011_alter_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)     1383 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0012_source_last_read_subscription.py
+-rw-r--r--   0 g          (501) staff       (20)      474 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0013_delete_webproxy_enclosure_is_current.py
+-rw-r--r--   0 g          (501) staff       (20)      561 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0014_post_json_source_json.py
+-rw-r--r--   0 g          (501) staff       (20)      393 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/0015_source_alt_url.py
+-rw-r--r--   0 g          (501) staff       (20)        0 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/migrations/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)    17419 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/models.py
+-rw-r--r--   0 g          (501) staff       (20)    35210 2024-05-11 08:12:53.000000 django_feed_reader-2.0.1b2/feeds/tests.py
+-rw-r--r--   0 g          (501) staff       (20)    14277 2024-05-11 06:25:00.000000 django_feed_reader-2.0.1b2/feeds/utils.py
+-rw-r--r--   0 g          (501) staff       (20)    21076 2024-05-11 08:33:49.000000 django_feed_reader-2.0.1b2/feeds/utils_internal.py
+-rw-r--r--   0 g          (501) staff       (20)       63 2024-04-28 21:10:53.000000 django_feed_reader-2.0.1b2/feeds/views.py
+-rw-r--r--   0 g          (501) staff       (20)       38 2024-05-11 08:34:35.505453 django_feed_reader-2.0.1b2/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      903 2024-05-11 08:33:17.000000 django_feed_reader-2.0.1b2/setup.py
```

### Comparing `django_feed_reader-2.0.1b1/LICENSE` & `django_feed_reader-2.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/PKG-INFO` & `django_feed_reader-2.0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 2.0.1b1
+Version: 2.0.1b2
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django_feed_reader-2.0.1b1/django_feed_reader.egg-info/PKG-INFO` & `django_feed_reader-2.0.1b2/django_feed_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 2.0.1b1
+Version: 2.0.1b2
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django_feed_reader-2.0.1b1/django_feed_reader.egg-info/SOURCES.txt` & `django_feed_reader-2.0.1b2/django_feed_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/admin.py` & `django_feed_reader-2.0.1b2/feeds/admin.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0001_initial.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0004_webproxy.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0004_webproxy.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0006_auto_20190901_1644.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0006_auto_20190901_1644.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0007_auto_20210502_0716.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0007_auto_20210502_0716.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0010_enclosure_description_enclosure_medium.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0010_enclosure_description_enclosure_medium.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0012_source_last_read_subscription.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0012_source_last_read_subscription.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/migrations/0014_post_json_source_json.py` & `django_feed_reader-2.0.1b2/feeds/migrations/0014_post_json_source_json.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/models.py` & `django_feed_reader-2.0.1b2/feeds/models.py`

 * *Files identical despite different names*

### Comparing `django_feed_reader-2.0.1b1/feeds/tests.py` & `django_feed_reader-2.0.1b2/feeds/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,14 +449,29 @@
         read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.description, 'Public posts from @xurble@toot.community')
 
         self.assertEqual(src.posts.all()[0].enclosures.count(), 1)
 
+    def test_youtube_embed(self, mock):
+
+        self._populate_mock(mock, status=200, test_file="youtube.xml", content_type="application/rss+xml")
+
+        src = Source(name="test1", feed_url=BASE_URL, interval=0)
+        src.save()
+
+        read_feed(src, output=NullOutput())
+        src.refresh_from_db()
+
+        post = src.posts.all()[0]
+
+        self.assertTrue("iframe" in post.body)
+
+
     def test_media_content(self, mock):
 
         self._populate_mock(mock, status=200, test_file="media_content.xml", content_type="application/rss+xml")
 
         src = Source(name="test1", feed_url=BASE_URL, interval=0)
         src.save()
 
@@ -575,14 +590,40 @@
         self.assertEqual(src.status_code, 200)
 
         body = src.posts.all()[0].body
 
         self.assertTrue("<img" in body)
         self.assertFalse("align=" in body)
         self.assertFalse("hspace=" in body)
+        self.assertTrue("class=" in body)
+        self.assertFalse("style=" in body)
+
+    def test_sanitize_style(self, mock):
+
+        self._populate_mock(mock, status=200, test_file="sanitizer_style.xml", content_type="application/rss+xml")
+
+        src = Source(name="test1", feed_url=BASE_URL, interval=0)
+        src.save()
+
+        # read the feed to update the name
+        read_feed(src, output=NullOutput())
+        src.refresh_from_db()
+
+        self.assertEqual(src.status_code, 200)
+
+        body = src.posts.all()[0].body
+
+        print (body)
+
+        self.assertTrue("<img" in body)
+        self.assertFalse("align=" in body)
+        self.assertFalse("hspace=" in body)
+        self.assertTrue("class=" in body)
+        self.assertFalse("style=" in body)
+
 
     def create_source(self, mock, test_name, test_fn):
         self._populate_mock(mock, status=200,
                             test_file=test_fn,
                             content_type="application/rss+xml")
         src = Source(name=test_name, feed_url=BASE_URL, interval=0)
         src.save()
@@ -916,15 +957,15 @@
 
     def test_perm_redirect(self, mock):
 
         new_url = "http://new.feed.com/"
         self._populate_mock(mock, status=301, test_file="empty_file.txt", content_type="text/plain", headers={"Location": new_url})
         self._populate_mock(mock, status=200, test_file="rss_xhtml_body.xml", content_type="application/xml+rss",  url=new_url)
 
-        src = Source(name="test1", feed_url=BASE_URL, interval=0)
+        src = Source(name="test1", feed_url=BASE_URL, interval=60)
         src.save()
 
         read_feed(src, output=NullOutput())
         src.refresh_from_db()
 
         self.assertEqual(src.status_code, 301)
         self.assertEqual(src.interval, 60)
```

### Comparing `django_feed_reader-2.0.1b1/feeds/utils.py` & `django_feed_reader-2.0.1b2/feeds/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,18 @@
     :param output: A file-like object where logging messages will be written (default stdout).
     :type output: TextIO
     """
     todo = Source.objects.filter(Q(due_poll__lt=timezone.now()) & Q(live=True))
 
     output.write(f"\nQueue size is {todo.count()}")
 
-    sources = todo.order_by("due_poll")[:max_feeds]
+    if max_feeds > 0:
+        sources = todo.order_by("due_poll")[:max_feeds]
+    else:
+        sources = todo.order_by("due_poll")
 
     output.write("\nProcessing %d" % sources.count())
 
     for src in sources:
         read_feed(src, output)
```

### Comparing `django_feed_reader-2.0.1b1/feeds/utils_internal.py` & `django_feed_reader-2.0.1b2/feeds/utils_internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,19 @@
 def _customize_sanitizer(fp):
 
     bad_attributes = [
         "align",
         "valign",
         "hspace",
         "width",
-        "height"
+        "height",
+        "style",
     ]
 
+    fp.sanitizer._HTMLSanitizer.acceptable_elements.add("iframe")  # youtube
     for item in bad_attributes:
         try:
             if item in fp.sanitizer._HTMLSanitizer.acceptable_attributes:
                 fp.sanitizer._HTMLSanitizer.acceptable_attributes.remove(item)
         except Exception:
             logging.debug("Could not remove {}".format(item))
 
@@ -63,22 +65,22 @@
 
 def fix_relative(html: str, url: str):
 
     """ this is fucking cheesy """
     try:
         base = "/".join(url.split("/")[:3])
 
-        html = html.replace("src='//", "src='http://")
-        html = html.replace('src="//', 'src="http://')
+        html = html.replace("src='//", "src='https://")
+        html = html.replace('src="//', 'src="https://')
 
         html = html.replace("src='/", "src='%s/" % base)
         html = html.replace('src="/', 'src="%s/' % base)
 
-        html = html.replace("href='//", "href='http://")
-        html = html.replace('href="//', 'href="http://')
+        html = html.replace("href='//", "href='https://")
+        html = html.replace('href="//', 'href="https://')
 
         html = html.replace("href='/", "href='%s/" % base)
         html = html.replace('href="/', 'href="%s/' % base)
 
     except Exception:
         pass
 
@@ -419,15 +421,15 @@
         keep_going = True
         while keep_going:
             keep_going = False  # assume were stopping unless we find a next link
             if hasattr(f.feed, 'links'):
                 for link in f.feed.links:
                     if 'rel' in link and link['rel'] == "next":
                         ret = requests.get(link['href'], headers=headers, verify=VERIFY_HTTPS, allow_redirects=True, timeout=20)
-                        (pok, pchanged) = parse_feed_xml(source_feed, ret.content)
+                        (pok, pchanged) = parse_feed_xml(source_feed, ret.content, output)
                         # print(link['href'])
                         # print((pok, pchanged))
                         f = parser.parse(ret.content)  # rebase the loop on this feed version
                         keep_going = True
 
     return (ok, changed)
```

### Comparing `django_feed_reader-2.0.1b1/setup.py` & `django_feed_reader-2.0.1b2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('readme.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='django-feed-reader',
-    version='2.0.1-beta.1',
+    version='2.0.1-beta.2',
     description='An RSS feed reading library for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Gareth Simpson',
     author_email='g@xurble.org',
     url='https://github.com/xurble/django-feed-reader',
     license='MIT',
```

