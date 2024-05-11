# Comparing `tmp/Notion2Pelican-0.0.2-py3-none-any.whl.zip` & `tmp/Notion2Pelican-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8763 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     8640 b- defN 24-Apr-13 12:56 Notion2Pelican/Notion2Pelican.py
--rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-13 13:07 Notion2Pelican/__init__.py
+Zip file size: 9388 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat    10191 b- defN 24-May-10 14:51 Notion2Pelican/Notion2Pelican.py
+-rw-rw-rw-  2.0 fat       23 b- defN 24-May-10 11:43 Notion2Pelican/__init__.py
 -rw-rw-rw-  2.0 fat     7242 b- defN 24-Mar-26 18:59 Notion2Pelican/notion2md.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4279 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      675 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/RECORD
-8 files, 22051 bytes uncompressed, 7575 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-May-10 15:36 Notion2Pelican-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4452 b- defN 24-May-10 15:36 Notion2Pelican-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 15:36 Notion2Pelican-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-10 15:36 Notion2Pelican-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      676 b- defN 24-May-10 15:36 Notion2Pelican-0.0.3.dist-info/RECORD
+8 files, 23776 bytes uncompressed, 8200 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: Notion2Pelican/__init__.py
 Comment: 
 
 Filename: Notion2Pelican/notion2md.py
 Comment: 
 
-Filename: Notion2Pelican-0.0.2.dist-info/LICENSE
+Filename: Notion2Pelican-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: Notion2Pelican-0.0.2.dist-info/METADATA
+Filename: Notion2Pelican-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: Notion2Pelican-0.0.2.dist-info/WHEEL
+Filename: Notion2Pelican-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: Notion2Pelican-0.0.2.dist-info/top_level.txt
+Filename: Notion2Pelican-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Notion2Pelican-0.0.2.dist-info/RECORD
+Filename: Notion2Pelican-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Notion2Pelican/Notion2Pelican.py

```diff
@@ -41,33 +41,37 @@
     Returns
     -------
     data: json
         Data structure returned by the Notion API
 
     Documentation:
     --------------
-    curl https://api.notion.com/v1/blocks/16d8004e-5f6a-42a6-9811-51c22ddada12/children?page_size=100 \  # noqa E501
+    curl https://api.notion.com/v1/blocks/16d8004e-5f6a-42a6-9811-51c22ddada12/children?page_size=100  # noqa E501
     -H 'Authorization: Bearer '"$NOTION_API_KEY"'' \
     -H "Notion-Version: 2022-06-28"
     """
     read_url = f"https://api.notion.com/v1/blocks/{databaseId}/children?page_size=100"  # noqa E501
+
     if fp is None:
         fp = abspath(join(__file__, pardir, "db.json"))
 
     res = requests.request("GET", read_url, headers=notion_header)
     data = res.json()
     html_response = res.status_code
 
     if html_response == 200:  # res.status_code
         with open(fp, 'w', encoding='utf8') as f:
             f.write(json.dumps(data, indent=4))
         if print_res:
             print("print res >>>>>>>>>>>>>")
             print(json.dumps(data, indent=4))
             print("print res <<<<<<<<<<<<<<")
+    else:
+        print("failed to download db: html_response={html_response}")
+        print(res)
     return data
 
 
 def page_tree_ids(res, headers, fp=None):
     """ parses the Notion DB json into a tree
 
     Parameters
@@ -83,17 +87,17 @@
     children_ids : list of dict
         each dict is a page title, page id and list of children
     """
 
     children_ids = []
     for b in res["results"]:
         page_title = ""
-
         if "child_page" in b:
             if b["has_children"]:
+                print(98)
                 id1 = b["id"]
                 page_title = b["child_page"]["title"]
                 res1 = readDatabase(id1, headers, print_res=False)
                 children = page_tree_ids(res1, headers)
                 children_page = {"title": page_title, "id": id1,
                                  "children": children}
                 children_ids.append(children_page)
@@ -146,33 +150,83 @@
                     plain_text = para_block["plain_text"]
                     url = para_block["href"]
                     md += f"[{plain_text}]({url})"
     # md += "\n"
     return md
 
 
-def pageid_2_md(front_matter, res, debug=False):
+def get_img(url, dpo):
+    """ attempts to download the image locally, upon success returns the path
+    if failed returns None
+
+    Parameters
+    ----------
+    url: str
+        the url path on AWS with temp token used by Notion
+    dpo: str
+        the path where the image should be serialized if download successful
+
+    Returns
+    -------
+    fpo: str
+        if None indicates failed download, else the path where the image is
+    """
+    import os
+    from urllib.parse import urlparse
+    from requests import get
+
+    a = urlparse(url)
+    # Output:
+    # /7f35e08f-716e-4cce-94e2-2f47dac447ed/890539ef-92c9-4fa8-9422-1e0c589cdab5/
+    # New_York_Stock_Exchange_-_panoramio.jpg
+    fn = os.path.basename(a.path)
+    # Output: 09-09-201315-47-571378756077.jpg
+    # > New_York_Stock_Exchange_-_panoramio.jpg
+    fp = abspath(join(dpo, fn))
+    fpo = None
+    res = get(url)
+    if res.ok:
+        with open(fp, mode="wb") as fo:
+            fo.write(res.content)
+        fpo = fn
+    return fpo
+
+
+def pageid_2_md(front_matter, res,
+                dp_img=None, rsc_folder="",
+                debug=False):
     """ generates markdown with front matter from notion json
 
     Parameters
     ----------
     front_matter: json
         the page title as the title is not in the json object
     res: json
         json returned by the NOTION API
+    dp_img: str
+        the path where images should be stored once downloaded
+    rsc_folder: str
+        the path prefix to be added to the filename for pelican to generate
+        appropriate hmtl
+    debug: bool
+        if True outputs more info
 
     Returns
     --------
     md: str
         Markdown formatted page
     """
 
-    known_btype = ["heading_1", "heading_2", "paragraph", "bulleted_list_item", "numbered_list_item", "image"]
-
-    # FIXME: 56c2ac88fa7c49d8859c44ce68eca68b
+    img_local = False
+    if dp_img is not None:
+        img_local = True
+
+    known_btype = ["bulleted_list_item",
+                   "heading_1", "heading_2", "heading_3", "image",
+                   "numbered_list_item", "paragraph", "quote"]
 
     if "status" not in front_matter:
         front_matter["status"] = "published"
 
     md = f"""---
 title: {front_matter['title']}
 id: {res["results"][0]['id']}
@@ -185,61 +239,67 @@
 """
 
     md += f"# {front_matter['title']}\n\n"
     prev_btype = ""
 
     for block in res["results"]:
         btype = block["type"]
+        if btype not in known_btype:
+            print(f"unknown btype: {btype}")
         if debug:
             print("btype", btype)
         md_txt = para_2_md(block[btype])
 
         if btype != "numbered_list_item":
             bullet_index = 0
-        
+
         if btype == "paragraph":  # in block:
             md += f"\n{md_txt}\n"
         elif btype == "heading_1":
             md += f"\n# {md_txt}\n\n"
         elif btype == "heading_2":  # in block:
             """ "heading_2": {
                     "rich_text": [
                         {
                             "type": "text",
                             "text": {
                                 "content": """
-            head2 = md_txt # block["heading_2"]["rich_text"][0]["text"]["content"]
+            head2 = md_txt
             # print("head2",head2)
             md += f"\n## {head2}\n\n"
         elif btype == "heading_3":  # in block:
-            head3 = md_txt # block["heading_3"]["rich_text"][0]["text"]["content"]
+            head3 = md_txt
             # print("head2",head2)
             md += f"\n### {head3}\n\n"
         elif btype == "bulleted_list_item":
             # bull = block[btype]["rich_text"]
-            bulletpoint = md_txt #block[btype]["rich_text"][0]["text"]["content"]
+            bulletpoint = md_txt
             md += f"* {bulletpoint}\n"
         elif btype == "numbered_list_item":
-            bulletpoint = md_txt #block[btype]["rich_text"][0]["text"]["content"]
+            bulletpoint = md_txt
             # print("!!!!!!!!!!!!!", prev_btype, btype, bullet_index)
             if prev_btype == btype:
                 bullet_index += 1
                 md += f"{bullet_index}. {bulletpoint}\n"
             else:
                 bullet_index = 1
                 md += f"\n{bullet_index}. {bulletpoint}\n"
         elif btype == "quote":
-            quote_text = md_txt  # block[btype]["rich_text"][0]["text"]["content"]
+            quote_text = md_txt
             md += f"\n> {quote_text}\n"
         elif btype == "image":
             caption = ""
             for c in block["image"]["caption"]:
                 caption += c["plain_text"]
             url = block["image"][block["image"]["type"]]["url"]
-            img = f"![{caption}]({url})\n\n"
+            if img_local:
+                fn = get_img(url, dp_img)
+                img = f"![{caption}]({rsc_folder}{fn})\n\n"
+            else:
+                img = f"![{caption}]({url})\n\n"
             md += img
         prev_btype = btype
     return md
 
 
 def replace_invalid_characters(filename):
     # Define a regular expression pattern to match invalid characters
```

## Notion2Pelican/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## Comparing `Notion2Pelican-0.0.2.dist-info/LICENSE` & `Notion2Pelican-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Notion2Pelican-0.0.2.dist-info/METADATA` & `Notion2Pelican-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Notion2Pelican
-Version: 0.0.2
+Version: 0.0.3
 Summary: Import notion pages in pelican blogging format
 Home-page: https://github.com/oberron/Notion2Pelican
 Author: oberron
 Author-email: one.annum@gmail.com
 License: LICENSE
 Project-URL: Bug Tracker, https://github.com/oberron/Notion2Pelican/issues
 Keywords: Notion Pelican
@@ -62,20 +62,28 @@
 See the ./docs folder for minimalist code which imports a Notion DB into a pelican blogging and generates the static site.
 
 > [!IMPORTANT]  
 > The below example relies on the secrets to be in a local .env file (which containing secrets has to be created for each machine)
 > with the following keys: `FT_dbid` the ID of your database `NOTIONKEY` which usually starts with `secret_` and is available from your 
 > Notion dashboard
 
+> [!IMPORTANT]  
+> Integrations have a scope of the workspace they are created for
+
 > cd docs
 > python example.py
 
 
 ## Release Notes and Roadmap
 
+v0.0.3 - adding support for:
+
+* download images locally
+* download DB into .csv
+
 v0.0.2 - adding support for
 
 * add support for H1 (which was not present)
 * numbered list (which was not working)
 * italic and bold (which was not available)
 * non regression for images (though it was working)
 * add support for quotes
```

## Comparing `Notion2Pelican-0.0.2.dist-info/RECORD` & `Notion2Pelican-0.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Notion2Pelican/Notion2Pelican.py,sha256=WZKB0M1mggAdLYq6S5mPscQJw-YeOF_TNB-h-QaeMKo,8640
-Notion2Pelican/__init__.py,sha256=j7895T8JfsWQAOvxm8SAdESs5iFmIuAqKpyfjSAfKZ4,23
+Notion2Pelican/Notion2Pelican.py,sha256=2axOZx68bS4KugPE5VTsfS0gSeTJrj2GXcyCJu-UCdg,10191
+Notion2Pelican/__init__.py,sha256=4dCrvStS1OgE3Vlcv-qx5-TAo377yOMEToEqCi-PwY4,23
 Notion2Pelican/notion2md.py,sha256=0doPGW6-qflmBNoemZ-wjL0r4ZsJqjQY21BN50dUwUM,7242
-Notion2Pelican-0.0.2.dist-info/LICENSE,sha256=Fn3cwvKKiiE3szx4MfhsP3Onsx25i8Fr2a7iJ7yMZBg,1085
-Notion2Pelican-0.0.2.dist-info/METADATA,sha256=8uA_NEYN-xkdC2EkIzZjsbl9DygyL9DxXtzGowWu0dw,4279
-Notion2Pelican-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Notion2Pelican-0.0.2.dist-info/top_level.txt,sha256=ajK76CzagnB5dN-ombUkwmeUPuH0dRY9LlTmMzaTqlY,15
-Notion2Pelican-0.0.2.dist-info/RECORD,,
+Notion2Pelican-0.0.3.dist-info/LICENSE,sha256=Fn3cwvKKiiE3szx4MfhsP3Onsx25i8Fr2a7iJ7yMZBg,1085
+Notion2Pelican-0.0.3.dist-info/METADATA,sha256=6fYkm3FKWW1I2TvSbaiAJAAGlsH9xdvNPVrQ4Lncyk8,4452
+Notion2Pelican-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Notion2Pelican-0.0.3.dist-info/top_level.txt,sha256=ajK76CzagnB5dN-ombUkwmeUPuH0dRY9LlTmMzaTqlY,15
+Notion2Pelican-0.0.3.dist-info/RECORD,,
```

