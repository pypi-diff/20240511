# Comparing `tmp/xyz_util-0.9.7-py3-none-any.whl.zip` & `tmp/xyz_util-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 51906 bytes, number of entries: 25
+Zip file size: 52224 bytes, number of entries: 25
 -rw-r--r--  2.0 unx       88 b- defN 20-Jan-17 14:46 xyz_util/__init__.py
 -rw-r--r--  2.0 unx      975 b- defN 23-Aug-16 03:45 xyz_util/cmdutils.py
--rw-r--r--  2.0 unx    11021 b- defN 23-Dec-21 16:40 xyz_util/crawlutils.py
+-rw-r--r--  2.0 unx    11659 b- defN 24-May-11 03:54 xyz_util/crawlutils.py
 -rw-r--r--  2.0 unx      903 b- defN 18-Oct-15 06:43 xyz_util/cryptutils.py
--rw-r--r--  2.0 unx    14928 b- defN 23-Nov-30 07:39 xyz_util/datautils.py
+-rw-r--r--  2.0 unx    15119 b- defN 24-Apr-17 23:37 xyz_util/datautils.py
 -rw-r--r--  2.0 unx     6400 b- defN 21-Aug-09 10:21 xyz_util/dateutils.py
 -rw-r--r--  2.0 unx    13185 b- defN 21-Jul-04 23:24 xyz_util/dbutils.py
 -rw-r--r--  2.0 unx    17205 b- defN 21-Jul-26 09:02 xyz_util/excelutils.py
 -rw-r--r--  2.0 unx     2667 b- defN 21-Jul-04 23:24 xyz_util/formutils.py
 -rw-r--r--  2.0 unx     4619 b- defN 23-Nov-30 17:19 xyz_util/importutils.py
 -rw-r--r--  2.0 unx     3561 b- defN 23-Jun-16 10:38 xyz_util/mediautils.py
 -rw-r--r--  2.0 unx    15767 b- defN 23-Dec-13 23:31 xyz_util/modelutils.py
--rw-r--r--  2.0 unx    16893 b- defN 23-Mar-23 07:06 xyz_util/mongoutils.py
+-rw-r--r--  2.0 unx    17113 b- defN 24-Feb-04 01:04 xyz_util/mongoutils.py
 -rw-r--r--  2.0 unx    14661 b- defN 21-Jul-13 11:57 xyz_util/pandasutils.py
 -rw-r--r--  2.0 unx      507 b- defN 21-Jun-01 00:29 xyz_util/pdfutils.py
 -rw-r--r--  2.0 unx    15457 b- defN 23-Jul-02 06:27 xyz_util/statutils.py
 -rw-r--r--  2.0 unx     1997 b- defN 23-Mar-06 16:57 xyz_util/textutils.py
 -rw-r--r--  2.0 unx     1675 b- defN 20-Aug-01 15:19 xyz_util/transferutils.py
 -rw-r--r--  2.0 unx     5316 b- defN 21-Jun-05 23:16 xyz_util/validators.py
 -rw-r--r--  2.0 unx     7817 b- defN 23-Nov-30 00:35 xyz_util/views.py
 -rw-r--r--  2.0 unx     3957 b- defN 23-Nov-30 00:35 xyz_util/widgetutils.py
--rw-r--r--  2.0 unx     1028 b- defN 23-Dec-22 02:23 xyz_util-0.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-22 02:23 xyz_util-0.9.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Dec-22 02:23 xyz_util-0.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1950 b- defN 23-Dec-22 02:23 xyz_util-0.9.7.dist-info/RECORD
-25 files, 162678 bytes uncompressed, 48822 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx     1028 b- defN 24-May-11 07:32 xyz_util-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 07:32 xyz_util-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-11 07:32 xyz_util-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1950 b- defN 24-May-11 07:32 xyz_util-0.9.9.dist-info/RECORD
+25 files, 163727 bytes uncompressed, 49140 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: xyz_util/views.py
 Comment: 
 
 Filename: xyz_util/widgetutils.py
 Comment: 
 
-Filename: xyz_util-0.9.7.dist-info/METADATA
+Filename: xyz_util-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: xyz_util-0.9.7.dist-info/WHEEL
+Filename: xyz_util-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_util-0.9.7.dist-info/top_level.txt
+Filename: xyz_util-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_util-0.9.7.dist-info/RECORD
+Filename: xyz_util-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_util/crawlutils.py

```diff
@@ -52,19 +52,22 @@
 
 
 def http_post(url, **kwargs):
     return http_request(url, **kwargs)
 
 
 def http_request(url, data=None, mobile_mode=True, cookies='', referer=None, extra_headers={}, timeout=(20, 20),
-                 proxy=True, allow_redirects=True):
+                 proxy=True, allow_redirects=True, requests=requests.session(), no_agent=False):
     headers = {
         "User-Agent": UA_MOBILE if mobile_mode else UA_PC,
         "Accept-Encoding": "gzip"
     }
+    if no_agent:
+        del headers['User-Agent']
+
     headers.update(extra_headers)
     if referer:
         headers['Referer'] = referer
     if proxy is True:
         proxy = PROXY
     from inspect import isgeneratorfunction
     if isgeneratorfunction(proxy):
@@ -322,18 +325,37 @@
 
 
 def html_get_text(html):
     import bs4
     return bs4.BeautifulSoup(html, 'html.parser').get_text().strip()
 
 
+def clean_html(html):
+    if not html:
+        return ''
+    from bs4 import BeautifulSoup
+    soup = BeautifulSoup(html, 'html.parser')
+
+    for tag in soup.find_all(True):
+        fs = list(tag.attrs.keys())
+        for f in fs:
+            if f == 'href' and tag.name == 'a' and 'javascript:' not in tag.attrs[f]:
+                continue
+            if f == 'src' and tag.name == 'img':
+                continue
+            del tag[f]
+        if tag.name == 'a':
+            tag.attrs['target'] = '_blank'
+    return str(soup)
+
+
 class Reader:
 
     def __init__(self, main_css=None):
-        self.main_css=main_css
+        self.main_css = main_css
 
     def read_images(self, r):
         for e in r.css('img'):
             yield dict(
                 src=e.css('::attr("src")').get(),
                 alt=e.css('::attr("alt")').get()
             )
@@ -349,13 +371,14 @@
         else:
             h = readability_summary(r.text)
         from scrapy.http import HtmlResponse
         pr = HtmlResponse(url=r.url, encoding='utf8', body=h)
         d = self.read_meta(r)
         d.update(
             url=r.url,
-            title=r.css('title::text').get().strip(),
+            title=r.css('head title::text').get().strip(),
             text=html_get_text(h),
             html=h,
             images=list(self.read_images(pr))
         )
         return d
+
```

## xyz_util/datautils.py

```diff
@@ -496,14 +496,25 @@
 
 A = Accessor  # alias
 
 
 def access(obj, path, quiet=True):
     return Accessor(path).resolve(obj, quiet=quiet)
 
+def access_list(obj, path):
+    ps = path.split('.*.')
+    a = obj
+    rs = []
+    ns = [obj]
+    for p in ps:
+        a = access(obj, p)
+        if a is not None:
+            rs.append(a)
+
+
 
 def import_function(s):
     import importlib
     ps = s.split(':')
     m = importlib.import_module(ps[0])
     func = getattr(m, ps[1])
     return func
```

## xyz_util/mongoutils.py

```diff
@@ -93,15 +93,18 @@
         if fields:
             fs.append({'$project': fields})
         return self.collection.aggregate(fs)
 
     def find(self, *args, **kwargs):
         if self.ordering and 'sort' not in kwargs:
             kwargs['sort'] = [django_order_field_to_mongo_sort(s) for s in self.ordering]
-        return self.collection.find(*args, **kwargs)
+        rs = self.collection.find(*args, **kwargs)
+        if not hasattr(rs, 'count'):
+            setattr(rs, 'count', lambda: self.count(args[0]))
+        return rs
 
     def upsert(self, cond, value, **kwargs):
         d = {'$set': value}
         for k, v in kwargs.items():
             d['$%s' % k] = v
         return self.collection.update_one(cond, d, upsert=True)
 
@@ -120,30 +123,32 @@
         if value:
             d['$set'] = value
         for k, v in kwargs.items():
             d['$%s' % k] = v
         return self.collection.update_many(cond, d)
 
     def inc(self, cond, value):
-        self.collection.update(cond, {'$inc': value}, upsert=True)
+        self.collection.update_many(cond, {'$inc': value}, upsert=True)
 
     def add_to_set(self, cond, value):
-        self.collection.update(cond, {'$addToSet': value}, upsert=True)
+        self.collection.update_many(cond, {'$addToSet': value}, upsert=True)
 
     def count(self, filter=None, distinct=False):
         if distinct:
             gs = []
             if filter:
                 gs.append({'$match': filter})
             gs.append({'$group': {'_id': '$%s' % distinct}}),
             gs.append({'$group': {'_id': 0, 'count': {'$sum': 1}}})
             for a in self.collection.aggregate(gs):
                 return a['count']
             return 0
-        return self.collection.count(filter)
+        if not filter:
+            return self.collection.estimated_document_count()
+        return self.collection.count_documents(filter)
 
     def sum(self, field, filter=None):
         gs = []
         if filter:
             gs.append({'$match': filter})
         gs.append({'$group': {'_id': 0, 'result': {'$sum': '$%s' % field}}})
         for a in self.collection.aggregate(gs):
```

## Comparing `xyz_util-0.9.7.dist-info/METADATA` & `xyz_util-0.9.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-util
-Version: 0.9.7
+Version: 0.9.9
 Summary: common utils
 Home-page: https://github.com/szuprefix/py-xyz-util
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

## Comparing `xyz_util-0.9.7.dist-info/RECORD` & `xyz_util-0.9.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 xyz_util/__init__.py,sha256=WEJvfVJ_HXMJKRpMfXP0srWexMdmSlu_Nq5AIb9Ciio,88
 xyz_util/cmdutils.py,sha256=9osBEeDSdOxjzT5RVp5cSNCcNxX4WUGkDBQm4Xzo9-I,975
-xyz_util/crawlutils.py,sha256=jszrf5el5BifCtMqWWoDU59KXXa37LVcKuXqMEKvIuI,11021
+xyz_util/crawlutils.py,sha256=Gn0d3b6lFopHptmRS-5DUBfMKM3m7B-yfYjwpEDewT4,11659
 xyz_util/cryptutils.py,sha256=UVNZlZ-7d-X7rWjUxMPv8EpvtXIyI6YKPZNgb6MCx_Q,903
-xyz_util/datautils.py,sha256=Wv_eDPakPdtFOLJWkaNY1UmL0IaI-qGo9a-pXwtPej8,14928
+xyz_util/datautils.py,sha256=0slkjBlsybjRFLxsWazzgib8S7kxCJuFqvXutZJ8eV0,15119
 xyz_util/dateutils.py,sha256=doPQh86iJNIWhA1EsZy1ar3Vgw3RSFAxUkTgPX_RU3s,6400
 xyz_util/dbutils.py,sha256=Wj4Bf7tJg2UzwTP5-p4rCACXTaIvH5J6milAOpAGHUk,13185
 xyz_util/excelutils.py,sha256=FuK1RnGPG1XFRNDyYbKPK7urc9tvgNXFtR9-NLlamkE,17205
 xyz_util/formutils.py,sha256=bM5pEShw-gmUm5RMVyQ9xPO7RAHZ4TNTwaFXlzebvmU,2667
 xyz_util/importutils.py,sha256=sj3P7eZW83fqgD26eI_zJJUtfpvn2orCwg9_diSSM04,4619
 xyz_util/mediautils.py,sha256=nu_L_qZN3PGZc6d7F-fVv75I1-ZXExp6fSjlCmPmaMs,3561
 xyz_util/modelutils.py,sha256=SO8g0QkeDYHJQmDtQp50RPyNarof8MYAT6Fvl3zHvgc,15767
-xyz_util/mongoutils.py,sha256=vilihwLZ7g6n89a02nOhXvcIxu8UTTzdf4t3qywZWDM,16893
+xyz_util/mongoutils.py,sha256=4PCG9hoRukWOTuLQmHo1cOpP1IjpeyXKcujICmM5t7k,17113
 xyz_util/pandasutils.py,sha256=gOuey7Vf6E62WFYVM4T2EwER9WQ_4Tmk4Ays0h6bCTQ,14661
 xyz_util/pdfutils.py,sha256=EFWIB4j74NHaCmGuVTZGSRbvoB-spl0Vj1_BKFjZl2I,507
 xyz_util/statutils.py,sha256=qkJ1icvRkoq2lQPzS5IZ4sShiKTxLUFxEN-EZrMDHqA,15457
 xyz_util/textutils.py,sha256=AYJm8SQrq-CxyLA4G9bzJyiFFcNW57NckRU0X2CItLI,1997
 xyz_util/transferutils.py,sha256=76VLi9Fjt3whO42oDvBJ0R2_CFzCkxeVxcfIB7VWtrc,1675
 xyz_util/validators.py,sha256=8qulZP-yPyal_GJWzmQzkm8yCHiMuGJ_hVPmK8bW-Ww,5316
 xyz_util/views.py,sha256=DYyW-sD4NL64T2uf9VUhlDLGl2U-Y6NI_WnTtjvh43w,7817
 xyz_util/widgetutils.py,sha256=7T7ns7yJs6beAZlnh_3yqAS0PJsxY4LmUqv1bCI1-94,3957
-xyz_util-0.9.7.dist-info/METADATA,sha256=USJxbQzH_2K2JWkaNNTNfHG66h5rFP0EvgINxeqgXp4,1028
-xyz_util-0.9.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-xyz_util-0.9.7.dist-info/top_level.txt,sha256=0uGpvx0NID3M2oMuWv7LYVDnUpUIIOwIWp8Br1tItgM,9
-xyz_util-0.9.7.dist-info/RECORD,,
+xyz_util-0.9.9.dist-info/METADATA,sha256=SYo_ZIqEvRVdsDKQRbYruxySxhflNqXNqXVvaayNUuk,1028
+xyz_util-0.9.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xyz_util-0.9.9.dist-info/top_level.txt,sha256=0uGpvx0NID3M2oMuWv7LYVDnUpUIIOwIWp8Br1tItgM,9
+xyz_util-0.9.9.dist-info/RECORD,,
```

