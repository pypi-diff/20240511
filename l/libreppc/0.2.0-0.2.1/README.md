# Comparing `tmp/libreppc-0.2.0.tar.gz` & `tmp/libreppc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.2.0.tar", last modified: Mon Apr 15 09:53:36 2024, max compression
+gzip compressed data, was "libreppc-0.2.1.tar", last modified: Sat May 11 08:32:40 2024, max compression
```

## Comparing `libreppc-0.2.0.tar` & `libreppc-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 09:53:36.021946 libreppc-0.2.0/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.2.0/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.2.0/MANIFEST.in
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2232 2024-04-15 09:53:36.021946 libreppc-0.2.0/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1499 2024-04-15 07:05:51.000000 libreppc-0.2.0/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 09:53:36.018612 libreppc-0.2.0/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-15 09:52:49.000000 libreppc-0.2.0/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      786 2024-04-15 04:47:48.000000 libreppc-0.2.0/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7428 2024-04-15 09:42:45.000000 libreppc-0.2.0/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 09:53:36.018612 libreppc-0.2.0/libreppc/static/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     8204 2024-04-15 09:49:10.000000 libreppc-0.2.0/libreppc/static/bloger.css
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7798 2024-04-15 09:52:10.000000 libreppc-0.2.0/libreppc/static/mastodon.css
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 09:53:36.021946 libreppc-0.2.0/libreppc/templates/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2987 2024-04-15 05:04:21.000000 libreppc-0.2.0/libreppc/templates/index.html
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2869 2024-04-15 05:04:41.000000 libreppc-0.2.0/libreppc/templates/post.html
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 09:53:36.021946 libreppc-0.2.0/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2232 2024-04-15 09:53:35.000000 libreppc-0.2.0/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      375 2024-04-15 09:53:35.000000 libreppc-0.2.0/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-15 09:53:35.000000 libreppc-0.2.0/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       37 2024-04-15 09:53:35.000000 libreppc-0.2.0/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-15 09:53:35.000000 libreppc-0.2.0/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-15 09:53:36.021946 libreppc-0.2.0/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1113 2024-04-15 09:52:40.000000 libreppc-0.2.0/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-11 08:32:40.738238 libreppc-0.2.1/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.2.1/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.2.1/MANIFEST.in
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2349 2024-05-11 08:32:40.738238 libreppc-0.2.1/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1616 2024-05-11 08:31:48.000000 libreppc-0.2.1/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-11 08:32:40.738238 libreppc-0.2.1/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       73 2024-05-11 08:32:10.000000 libreppc-0.2.1/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1057 2024-05-11 08:27:53.000000 libreppc-0.2.1/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1290 2024-05-11 08:18:20.000000 libreppc-0.2.1/libreppc/constants.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     9862 2024-05-11 08:26:16.000000 libreppc-0.2.1/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-11 08:32:40.738238 libreppc-0.2.1/libreppc/static/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     8276 2024-04-15 11:41:40.000000 libreppc-0.2.1/libreppc/static/bloger.css
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7834 2024-04-15 11:41:55.000000 libreppc-0.2.1/libreppc/static/mastodon.css
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-11 08:32:40.738238 libreppc-0.2.1/libreppc/templates/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2995 2024-05-11 08:25:32.000000 libreppc-0.2.1/libreppc/templates/index.html
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3703 2024-05-11 08:29:42.000000 libreppc-0.2.1/libreppc/templates/post.html
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-11 08:32:40.738238 libreppc-0.2.1/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2349 2024-05-11 08:32:40.000000 libreppc-0.2.1/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      397 2024-05-11 08:32:40.000000 libreppc-0.2.1/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-05-11 08:32:40.000000 libreppc-0.2.1/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       37 2024-05-11 08:32:40.000000 libreppc-0.2.1/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-05-11 08:32:40.000000 libreppc-0.2.1/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-05-11 08:32:40.738238 libreppc-0.2.1/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1113 2024-04-15 09:52:40.000000 libreppc-0.2.1/setup.py
```

### Comparing `libreppc-0.2.0/LICENSE` & `libreppc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.2.0/PKG-INFO` & `libreppc-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -39,45 +39,54 @@
 ```json
 {
     "theme" : "CSS_FILE_NAME_WITHOUT_.css",
     "avatar" : "https://avatar-url.com",
     "username" : "yourusername",
     "description" : "yourdescription",
     "base_url" : "yourpageurl",
-    "blog_dir" : "blog",
-    "blog_title" : "Blog",
-    "links" : [
+    "static_dir" : "static",
+    "blog" : {
+        "dir" : "blog",
+        "title" : "Blog"
+    },
+    "icons" : [
         {
             "title" : "linktitle",
             "icon" : "iconurl",
             "url" : "linkurl"
         },
     ],
-    "support" : [
+    "fields" : [
         {
             "title" : "Monero/XMR",
             "type" : "text",
             "target" : "yourcryptoaddress"
         },
         {
             "title" : "Patreon",
             "type" : "url",
             "target" : "https://patreon.com/"
         },
     ],
-    "projects" : [
+    "pages" : [
         {
             "title" : "projectname",
             "description" : "projectdescription",
-            "url" : "projecturl"
+            "filename" : "page"
         }
     ]
 }
 ```
 
+You also can generate config via:
+
+```sh
+$ python -m libreppc --init
+```
+
 Then you need to build site with:
 
 ```sh
 $ python -m libreppc --build
 ```
 
 ## Contacts
```

### Comparing `libreppc-0.2.0/README.md` & `libreppc-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,45 +17,54 @@
 ```json
 {
     "theme" : "CSS_FILE_NAME_WITHOUT_.css",
     "avatar" : "https://avatar-url.com",
     "username" : "yourusername",
     "description" : "yourdescription",
     "base_url" : "yourpageurl",
-    "blog_dir" : "blog",
-    "blog_title" : "Blog",
-    "links" : [
+    "static_dir" : "static",
+    "blog" : {
+        "dir" : "blog",
+        "title" : "Blog"
+    },
+    "icons" : [
         {
             "title" : "linktitle",
             "icon" : "iconurl",
             "url" : "linkurl"
         },
     ],
-    "support" : [
+    "fields" : [
         {
             "title" : "Monero/XMR",
             "type" : "text",
             "target" : "yourcryptoaddress"
         },
         {
             "title" : "Patreon",
             "type" : "url",
             "target" : "https://patreon.com/"
         },
     ],
-    "projects" : [
+    "pages" : [
         {
             "title" : "projectname",
             "description" : "projectdescription",
-            "url" : "projecturl"
+            "filename" : "page"
         }
     ]
 }
 ```
 
+You also can generate config via:
+
+```sh
+$ python -m libreppc --init
+```
+
 Then you need to build site with:
 
 ```sh
 $ python -m libreppc --build
 ```
 
 ## Contacts
```

### Comparing `libreppc-0.2.0/libreppc/libreppc.py` & `libreppc-0.2.1/libreppc/libreppc.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 import argparse
 import shutil
 import json
 import pytz
 import os
 import re
 
+from .constants import DEFAULT_BLOG_POST, DEFAULT_CONFIG, DEFAULT_PAGE
+
 class LibrePPC:
 
     current_dir = os.path.dirname(__file__)
 
     def __init__(self, app) -> None:
         self.app = app
-        self.data = json.load(open("config.json"))
-        self.load_blog_previews()
+        self.data = dict()
 
+    def load_config(self) -> None:
+        self.data = json.load(open("config.json"))
         if not 'theme' in self.data.keys():
             self.data['theme'] = 'mastodon'
+        self.load_blog_previews()
 
     def table_to_json(self, text: str) -> dict:
         lines = text.split('\n')
         ret, keys = list(), list()
         for index, line in enumerate(lines):
             if index == 0:
                 keys = [_index.strip() for _index in line.split('|')]
@@ -32,26 +36,31 @@
                 ret.append({keys[_index]:value.strip() for _index, value in enumerate(line.split('|')) if  _index > 0 and _index < len(keys) - 1})
         return ret[0]
 
     def parse_post_metadata(self, postId: str) -> dict:
         file = self.get_post_file(
             self.find_post_file_id(postId.removesuffix('.md'))
         )
-        blog_dir = self.data['blog_dir']
+        blog_dir = self.data['blog']['dir']
         with open(f'{blog_dir}/{file}.md', 'r') as fl:
             table = '\n'.join(fl.read().split('\n')[:3])
             return self.table_to_json(table)
 
     def remove_post_metadata(self, text: str) -> str:
         return '\n'.join(text.split('\n')[3:])
 
     def get_post_files(self) -> list:
-        files = os.listdir(self.data['blog_dir'])
+        blog_dir = self.data['blog']['dir']
+        files = os.listdir(blog_dir)
         files.sort()
         files.reverse()
+        for file in files:
+            if os.path.isdir(f"{blog_dir}/{file}"):
+                files.remove(file)
+
         return files
 
     def get_post_file(self, index: int) -> str | None:
         if index < 0: return None
         files = self.get_post_files()
         if index >= len(files): return None
         return self.get_post_files()[index].removesuffix('.md')
@@ -69,14 +78,23 @@
             **data,
             'id' : postId.removesuffix('.md'),
             'plain_title' : re.sub(cleaner, '', data['title']),
             'plain_description' : re.sub(cleaner, '', data['description']),
             'text' : html
         }
 
+    def make_project_dict(self, data: dict, page_data: dict, html: str) -> dict:
+        cleaner = re.compile('<.*?>')
+        return {
+            **data,
+            'plain_title' : re.sub(cleaner, '', page_data['title']),
+            'plain_description' : re.sub(cleaner, '', page_data['description']),
+            'text' : html
+        } 
+
     def render_template(self, name: str, data: dict) -> str:
         render = render_template(name, **data)
         render = render.replace("&lt;", "<")
         render = render.replace("&gt;", ">")
         render = render.replace("&#34;", '"')
         render = render.replace("amp;", "")
         render = render.replace("amp;", "")
@@ -92,40 +110,56 @@
         return self.render_template('index.html', data)
 
     def render_post(self, index: int, postId: str) -> str:
         previous_post = self.get_post_file(index+1)
         next_post = self.get_post_file(index-1)
 
         text = ""
-        blog_dir = self.data['blog_dir']
+        blog_dir = self.data['blog']['dir']
         postId = postId.replace('.html', '')
         with open(f'{blog_dir}/{postId}.md') as file:
             text = file.read()
 
         text = self.remove_post_metadata(text)
         html = markdown.markdown(text, extensions=['fenced_code', 'nl2br', 'tables', 'codehilite'])
         data = self.data.copy()
         data['post'] = self.make_post_dict(postId, html)
         data['previous_post'] = previous_post
         data['next_post'] = next_post
 
         return self.render_template('post.html', data)
 
+    def render_project_page(self, filename: str) -> str:
+        page = dict()
+        for p in self.data['pages']:
+            if p['filename'] == filename:
+                page = p.copy()
+
+        text = ""
+        with open(f'pages/{filename}.md') as file:
+            text = file.read()
+
+        html = markdown.markdown(text, extensions=['fenced_code', 'nl2br', 'tables', 'codehilite'])
+        data = self.data.copy()
+        data['page'] = self.make_project_dict(data, page, html)
+
+        return self.render_template('post.html', data)
+
     def generate_rss(self) -> FeedGenerator:
         fg = FeedGenerator()
         fg.id(self.data['base_url'])
         fg.title(f"{self.data['username']}'s blog")
         fg.author(name=self.data['username'], email='')
         fg.link(href=self.data['base_url'], rel='alternate')
         fg.logo(self.data['avatar'])
         fg.subtitle(self.data['description'])
         fg.link(href=f"{self.data['base_url']}/feed.atom", rel='self')
         fg.language('en')
 
-        blog_dir = self.data['blog_dir']
+        blog_dir = self.data['blog']['dir']
         files = self.get_post_files()
         files.sort()
 
         for filename in files:
             postId = filename.replace('.md', '')
             with self.app.app_context():
                 path = f'{blog_dir}/{postId}.md'
@@ -148,56 +182,92 @@
                 updated = datetime.fromtimestamp(os.path.getmtime(path))
                 updated = utc.localize(updated)
                 fe.updated(updated)
 
         return fg
 
     def load_blog_previews(self) -> None:
-        blog_dir = self.data['blog_dir']
-        self.data['blog'] = list()
+        blog_dir = self.data['blog']['dir']
+        self.data['blog']['pages'] = list()
         for filename in self.get_post_files():
             with open(f"{blog_dir}/{filename}", 'r', encoding="utf-8") as file:
                 text = file.read()
                 html = markdown.markdown(
                     text, 
                     extensions=['fenced_code', 'nl2br', 'tables', 'codehilite']
                 )
-                self.data['blog'].append(
+                self.data['blog']['pages'].append(
                     self.make_post_dict(filename, html)
                 )
 
     def parse_args(self):
         parser = argparse.ArgumentParser(
             prog='LibrePPC',
             description='A simple profile page creator',
         )
         parser.add_argument('-b', '--build', action='store_true')
         parser.add_argument('-s', '--serve', action='store_true')
+        parser.add_argument('-i', '--init', action='store_true')
         args = parser.parse_args()
         return args
 
+    def init(self) -> None:
+        print("Make default dirs...")
+        os.makedirs("blog", exist_ok=True)
+        os.makedirs("pages", exist_ok=True)
+        os.makedirs("static", exist_ok=True)
+
+        print("Write default blog post...")
+        with open("blog/000-intro.md", "w") as file:
+            file.write(DEFAULT_BLOG_POST)
+
+        print("Write default page...")
+        with open("pages/page.md", "w") as file:
+            file.write(DEFAULT_PAGE)
+
+        print("Write default config...")
+        with open("config.json", "w") as file:
+            json.dump(DEFAULT_CONFIG, file, indent=4)
+
+        print("Complete initialization!")
+
     def build(self) -> None:
         print("Building the site...")
         print("Make build dir...")
         os.makedirs("build/static", exist_ok=True)
         os.makedirs("build/post", exist_ok=True)
+        os.makedirs("build/pages", exist_ok=True)
 
         with open("build/index.html", "w") as file:
             print("Render index.html...")
             with self.app.app_context():
                 file.write(self.render_main(True))
 
         for index, postname in enumerate(self.get_post_files()):
             print(f"Render {postname}...")
             postId = postname.replace('.md', '')
             with open(f"build/post/{postId}.html", "w") as file:
                 with self.app.app_context():
                     file.write(self.render_post(index, postId))
 
+        for page in self.data['pages']:
+            filename = page['filename']
+            print(f"Render {filename}...")
+            with open(f"build/pages/{filename}.html", "w") as file:
+                with self.app.app_context():
+                    file.write(self.render_project_page(filename))
+
         print("Generate rss...")
         fg = self.generate_rss()
         fg.atom_file("build/static/feed.atom")
 
         print("Copy styles...")
         theme = self.data['theme']
+        static_dir = self.data['static_dir']
         shutil.copy(f"{self.current_dir}/static/{theme}.css", f"build/static/{theme}.css")
+        for file in os.listdir(static_dir):
+            shutil.copy(f"{static_dir}/{file}", f"build/static/{file}")
         print("Complete building!")
+
+
+
+
```

### Comparing `libreppc-0.2.0/libreppc/static/bloger.css` & `libreppc-0.2.1/libreppc/static/bloger.css`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     width: 30%;
     margin-left: 3%;
     position: sticky;
     top: 10px;
 }
 
 .avatar {
+    margin-top: 12px;
     height: 96px;
     border-radius: 50%;
     overflow: hidden;
     display: inline-block;
     vertical-align: middle;
 }
 
@@ -110,15 +111,14 @@
 .project:hover {
 }
 
 .blog {
     padding: 1%;
     display: grid;
     grid-template-columns: repeat(1, 1fr);
-    gap: 10px;
     grid-auto-rows: minmax(auto, auto);
 }
 
 .blog a {
     color: #ffffff;
     text-decoration: none;
 }
@@ -165,14 +165,18 @@
     text-align: left;
     padding: 12px;
     margin: 4px;
     border: 0px;
     width: 65%;
 }
 
+.postbody img {
+    width: 100%;
+}
+
 .navigation {
     display: grid;
     grid-template-columns: repeat(2, 1fr);
     gap: 10px;
     grid-auto-rows: minmax(auto, auto);
 }
 
@@ -195,20 +199,21 @@
         grid-template-columns: repeat(3, 1fr);
     }
 }
 
 @media (max-width: 720px) {
     .content {
         width: 90%;
-        margin-left: 5%;
-        margin-right: 5%;
+        margin-left: 2.5%;
+        margin-right: 2.5%;
     }
 
     .profile {
-        width: 95%;
+        margin-left: 0;
+        width: 100%;
         float: none;
         clear: all;
         position: relative;
     }
 
     .projects {
         grid-template-columns: repeat(4, 1fr);
```

### Comparing `libreppc-0.2.0/libreppc/static/mastodon.css` & `libreppc-0.2.1/libreppc/static/mastodon.css`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,18 @@
     background: #1f232b;
     text-align: left;
     padding: 12px;
     margin: 4px;
     border: 0px;
 }
 
+.postbody img {
+    width: 100%;
+}
+
 .navigation {
     display: grid;
     grid-template-columns: repeat(2, 1fr);
     gap: 10px;
     grid-auto-rows: minmax(auto, auto);
 }
```

### Comparing `libreppc-0.2.0/libreppc/templates/index.html` & `libreppc-0.2.1/libreppc/templates/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
         <div class="profile">
             <img class="avatar" src="{{ avatar }}">
 
             <h1 class="username">{{ username }}</h1>
             <p class="description">{{ description }}</p>
 
             <div class="links">
-                {% for link in links %}
+                {% for link in icons %}
                 <div class="link">
                     <a href="{{ link["url"] }}" target="_blank">
                         <img src="{{ link["icon"] }}" alt="{{ link["title"] }}" style="height: 32px">
                     </a>
                 </div>
                 {% endfor %}
             </div>
 
             <div class="support">
-                {% for supporter in support %}
+                {% for supporter in fields %}
                 <div class="supporter">
                     {% if supporter["type"] == "text" %}
                         <p class="title">{{ supporter["title"] }}</p> 
                         <code class="target">{{ supporter["target"] }}</code>
                     {% else %}
                         <p class="title">{{ supporter["title"] }}</p>
                         <a href="{{ supporter["target"] }}" target="_blank">{{ supporter["target"] }}</a>
@@ -48,29 +48,29 @@
                 </div>
                 {% endfor %}
             </div>
 
         </div>
 
         <div class="projects">
-            {% for project in projects %}
-            <a href="{{ project["url"] }}" target="_blank">
+            {% for project in pages %}
+            <a href="pages/{{ project["filename"] }}.html">
                 <div class="project">
                     <h3 class="title">{{ project["title"] }}</h3>
                     <p class="description">{{ project["description"] }}</p>
                 </div>
             </a>
             {% endfor %}
         </div>
 
         <div class="blog">
 
-            <h1>{{ blog_title }}</h1>
+            <h1>{{ blog["title"] }}</h1>
             
-            {% for post in blog %}
+            {% for post in blog["pages"] %}
             <a href="post/{{ post["id"] }}.html">
                 <div class="post">
                     <h1 class="title">{{ post["title"] }}</h1>
                     <p class="description">
                         {{ post["description"] }}
                     </p>
                     <div class="metadata">
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
 [{{ avatar }}]
 ************ {{{{ uusseerrnnaammee }}}} ************
 {{ description }}
-{% for link in links %}
+{% for link in icons %}
 }" target="_blank">
 }" alt="{{ link["title"] }}" style="height: 32px">
 {% endfor %}
-{% for supporter in support %}
+{% for supporter in fields %}
 {% if supporter["type"] == "text" %}
 {{ supporter["title"] }}
 {{ supporter["target"] }} {% else %}
 {{ supporter["title"] }}
 }" target="_blank">{{ supporter["target"] }}
  {% endif %}
 {% endfor %}
-{% for project in projects %}
-}" target="_blank">
+{% for project in pages %}
+}.html">
 ******** {{{{ pprroojjeecctt[[""ttiittllee""]] }}}} ********
 {{ project["description"] }}
 {% endfor %}
-************ {{{{ bblloogg__ttiittllee }}}} ************
-{% for post in blog %}
+************ {{{{ bblloogg[[""ttiittllee""]] }}}} ************
+{% for post in blog["pages"] %}
 }.html">
 ************ {{{{ ppoosstt[[""ttiittllee""]] }}}} ************
 {{ post["description"] }}
 {{ post["date"] }} • {{ post["author"] }}
 {% endfor %}
```

### Comparing `libreppc-0.2.0/libreppc/templates/post.html` & `libreppc-0.2.1/libreppc/templates/post.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="stylesheet" href="../static/{{ theme }}.css">
-    <title>{{ username }} - {{ post["plain_title"] }}</title>
-    <link rel="icon" href="{{ avatar }}">
-
-    <meta property="og:title" content="{{ username }} - {{ post["plain_title"] }}"/>
-    <meta property="og:image" content="{{ avatar }}"/>
-    <meta property="og:description" content="{{ post["plain_description"] }}"/>
-    <meta property="og:url" content="{{ base_url }}/post/{{ post["id"] }}.html"/>
+    {% if post is defined %}
+        <title>{{ username }} - {{ post["plain_title"] }}</title>
+        <link rel="icon" href="{{ avatar }}">
+
+        <meta property="og:title" content="{{ username }} - {{ post["plain_title"] }}"/>
+        <meta property="og:image" content="{{ avatar }}"/>
+        <meta property="og:description" content="{{ post["plain_description"] }}"/>
+        <meta property="og:url" content="{{ base_url }}/post/{{ post["id"] }}.html"/>
+    {% else %}
+        <title>{{ username }} - {{ page["plain_title"] }}</title>
+        <link rel="icon" href="{{ avatar }}">
+
+        <meta property="og:title" content="{{ username }} - {{ page["plain_title"] }}"/>
+        <meta property="og:image" content="{{ avatar }}"/>
+        <meta property="og:description" content="{{ page["plain_description"] }}"/>
+        <meta property="og:url" content="{{ base_url }}/pages/{{ page["id"] }}.html"/>
+    {% endif %}
     <meta property="og:image:width" content="512" />
     <meta property="og:image:height" content="512"/>
     <meta property="og:type" content="website"/> 
 </head>
 <body>
 
     <div class="content">
@@ -46,39 +56,46 @@
                         <a href="{{ supporter["target"] }}" target="_blank">{{ supporter["target"] }}</a>
                     {% endif %}
                 </div>
                 {% endfor %}
             </div>
         </div>
 
-        <div class="postbody">
-            <h1 class="title">{{ post["title"] }}</h1>
-            <div class="metadata">
-                <p>{{ post["date"] }} • {{ post["author"] }}</p>
-            </div>
-            {{ post["text"] }}
-        </div>
-
-        <div class="navigation">
-            {% if previous_post %}
-                <div class="previous-post">
-                    <a href="{{ previous_post }}.html">
-                        <p>Previous post</p>
-                    </a>
+        {% if post is defined %}
+            <div class="postbody">
+                <h1 class="title">{{ post["title"] }}</h1>
+                <div class="metadata">
+                    <p>{{ post["date"] }} • {{ post["author"] }}</p>
                 </div>
-            {% endif %}
+                {{ post["text"] }}
+            </div>
 
-            {% if next_post %}
-                <div class="next-post">
-                    <a href="{{ next_post }}.html">
-                        <p>Next post</p>
-                    </a>
-                </div>
-            {% endif %}
-        </div>
+            <div class="navigation">
+                {% if previous_post %}
+                    <div class="previous-post">
+                        <a href="{{ previous_post }}.html">
+                            <p>Previous post</p>
+                        </a>
+                    </div>
+                {% endif %}
+
+                {% if next_post %}
+                    <div class="next-post">
+                        <a href="{{ next_post }}.html">
+                            <p>Next post</p>
+                        </a>
+                    </div>
+                {% endif %}
+            </div>
+        {% else %}
+            <div class="postbody">
+                <h1 class="title">{{ page["plain_title"] }}</h1>
+                {{ page["text"] }}
+            </div>
+        {% endif %}
 
     </div>
     
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
+{% if post is defined %}
 }"/>
 }"/>
-}.html"/>
+}.html"/> {% else %}
+}"/>
+}"/>
+}.html"/> {% endif %}
 [{{ avatar }}]
 _**_**_**_**_**_**_ _{{_{{_ _uu_ss_ee_rr_nn_aa_mm_ee_ _}}_}}_ _**_**_**_**_**_**
 {{ description }}
 {% for link in links %}
 }" target="_blank">
 }" alt="{{ link["title"] }}" style="height: 32px">
 {% endfor %}
@@ -12,15 +16,20 @@
 {% if supporter["type"] == "text" %}
 {{ supporter["title"] }}
 {{ supporter["target"] }} {% else %}
 {{ supporter["title"] }}
 }" target="_blank">{{ supporter["target"] }}
  {% endif %}
 {% endfor %}
+{% if post is defined %}
 ************ {{{{ ppoosstt[[""ttiittllee""]] }}}} ************
 {{ post["date"] }} • {{ post["author"] }}
 {{ post["text"] }}
 {% if previous_post %}
 _P_r_e_v_i_o_u_s_ _p_o_s_t
 {% endif %} {% if next_post %}
 _N_e_x_t_ _p_o_s_t
 {% endif %}
+{% else %}
+************ {{{{ ppaaggee[[""ppllaaiinn__ttiittllee""]] }}}} ************
+{{ page["text"] }}
+{% endif %}
```

### Comparing `libreppc-0.2.0/libreppc.egg-info/PKG-INFO` & `libreppc-0.2.1/libreppc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -39,45 +39,54 @@
 ```json
 {
     "theme" : "CSS_FILE_NAME_WITHOUT_.css",
     "avatar" : "https://avatar-url.com",
     "username" : "yourusername",
     "description" : "yourdescription",
     "base_url" : "yourpageurl",
-    "blog_dir" : "blog",
-    "blog_title" : "Blog",
-    "links" : [
+    "static_dir" : "static",
+    "blog" : {
+        "dir" : "blog",
+        "title" : "Blog"
+    },
+    "icons" : [
         {
             "title" : "linktitle",
             "icon" : "iconurl",
             "url" : "linkurl"
         },
     ],
-    "support" : [
+    "fields" : [
         {
             "title" : "Monero/XMR",
             "type" : "text",
             "target" : "yourcryptoaddress"
         },
         {
             "title" : "Patreon",
             "type" : "url",
             "target" : "https://patreon.com/"
         },
     ],
-    "projects" : [
+    "pages" : [
         {
             "title" : "projectname",
             "description" : "projectdescription",
-            "url" : "projecturl"
+            "filename" : "page"
         }
     ]
 }
 ```
 
+You also can generate config via:
+
+```sh
+$ python -m libreppc --init
+```
+
 Then you need to build site with:
 
 ```sh
 $ python -m libreppc --build
 ```
 
 ## Contacts
```

### Comparing `libreppc-0.2.0/setup.py` & `libreppc-0.2.1/setup.py`

 * *Files identical despite different names*

