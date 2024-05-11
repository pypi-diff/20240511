# Comparing `tmp/ygoutil-0.2.0.tar.gz` & `tmp/ygoutil-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygoutil-0.2.0.tar", last modified: Wed May  1 20:08:21 2024, max compression
+gzip compressed data, was "ygoutil-0.2.1.tar", last modified: Fri May 10 20:03:51 2024, max compression
```

## Comparing `ygoutil-0.2.0.tar` & `ygoutil-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1064 2024-05-01 20:08:06.550142 ygoutil-0.2.0/LICENSE
--rw-r--r--   0        0        0     1156 2024-05-01 20:08:06.550142 ygoutil-0.2.0/README.md
--rw-r--r--   0        0        0      760 2024-05-01 20:08:21.654206 ygoutil-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       51 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/__init__.py
--rw-r--r--   0        0        0       22 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/__version__.py
--rw-r--r--   0        0        0      314 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/__init__.py
--rw-r--r--   0        0        0     5167 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/card.py
--rw-r--r--   0        0        0     8321 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/constant.py
--rw-r--r--   0        0        0      420 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/ids.py
--rw-r--r--   0        0        0      277 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/misc.py
--rw-r--r--   0        0        0    10640 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/unit.py
--rw-r--r--   0        0        0     7128 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/dataloader.py
--rw-r--r--   0        0        0        0 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/legacy/__init__.py
--rw-r--r--   0        0        0     8786 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/legacy/card.py
--rw-r--r--   0        0        0      138 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/__init__.py
--rw-r--r--   0        0        0      259 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/__init__.py
--rw-r--r--   0        0        0     2856 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/api.py
--rw-r--r--   0        0        0     3607 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/misc.py
--rw-r--r--   0        0        0    12674 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/page.py
--rw-r--r--   0        0        0     1953 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/base.py
--rw-r--r--   0        0        0        0 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/cdb/__init__.py
--rw-r--r--   0        0        0     3556 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/cdb/misc.py
--rw-r--r--   0        0        0     1370 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/misc.py
--rw-r--r--   0        0        0    17833 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/ourocg.py
--rw-r--r--   0        0        0    13403 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/sqlbuilder.py
--rw-r--r--   0        0        0     6377 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/ygoRoom.py
--rw-r--r--   0        0        0        0 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      162 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_card.py
--rw-r--r--   0        0        0     1929 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_cdb.py
--rw-r--r--   0        0        0     2447 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_source/test_baige.py
--rw-r--r--   0        0        0     1687 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_source/test_ourocg.py
--rw-r--r--   0        0        0     1054 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_sql.py
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 ygoutil-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-10 20:03:36.329721 ygoutil-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1156 2024-05-10 20:03:36.329721 ygoutil-0.2.1/README.md
+-rw-r--r--   0        0        0      782 2024-05-10 20:03:51.437867 ygoutil-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/__version__.py
+-rw-r--r--   0        0        0      314 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/card/__init__.py
+-rw-r--r--   0        0        0     5417 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/card/card.py
+-rw-r--r--   0        0        0     8321 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/card/constant.py
+-rw-r--r--   0        0        0      420 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/card/ids.py
+-rw-r--r--   0        0        0      277 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/card/misc.py
+-rw-r--r--   0        0        0    10650 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/card/unit.py
+-rw-r--r--   0        0        0     7128 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/dataloader.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/legacy/__init__.py
+-rw-r--r--   0        0        0     8786 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/legacy/card.py
+-rw-r--r--   0        0        0      138 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/__init__.py
+-rw-r--r--   0        0        0      259 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/baige/__init__.py
+-rw-r--r--   0        0        0     2921 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/baige/api.py
+-rw-r--r--   0        0        0     3607 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/baige/misc.py
+-rw-r--r--   0        0        0    13039 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/baige/page.py
+-rw-r--r--   0        0        0     1953 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/base.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/cdb/__init__.py
+-rw-r--r--   0        0        0     3571 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/cdb/misc.py
+-rw-r--r--   0        0        0     1370 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/misc.py
+-rw-r--r--   0        0        0    18268 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/source/ourocg.py
+-rw-r--r--   0        0        0    13403 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/sqlbuilder.py
+-rw-r--r--   0        0        0     6518 2024-05-10 20:03:36.333721 ygoutil-0.2.1/src/ygoutil/ygoRoom.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:03:36.333721 ygoutil-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-10 20:03:36.333721 ygoutil-0.2.1/tests/test_card.py
+-rw-r--r--   0        0        0     1929 2024-05-10 20:03:36.333721 ygoutil-0.2.1/tests/test_cdb.py
+-rw-r--r--   0        0        0     2802 2024-05-10 20:03:36.333721 ygoutil-0.2.1/tests/test_source/test_baige.py
+-rw-r--r--   0        0        0     1705 2024-05-10 20:03:36.333721 ygoutil-0.2.1/tests/test_source/test_ourocg.py
+-rw-r--r--   0        0        0     1054 2024-05-10 20:03:36.333721 ygoutil-0.2.1/tests/test_sql.py
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 ygoutil-0.2.1/PKG-INFO
```

### Comparing `ygoutil-0.2.0/LICENSE` & `ygoutil-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/README.md` & `ygoutil-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/pyproject.toml` & `ygoutil-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "ygoutil"
 dynamic = []
-description = "一个 ygo 工具集"
+description = "一个 ygo 工具集 | Handy tools for ygo"
 authors = [
     { name = "liggest" },
 ]
 dependencies = [
     "typing-extensions>=4.11.0",
     "httpx>=0.27.0",
     "beautifulsoup4>=4.12.3",
     "lxml>=5.2.1",
     "tomli>=2.0.1",
     "tomli-w>=1.0.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `ygoutil-0.2.0/src/ygoutil/card/card.py` & `ygoutil-0.2.1/src/ygoutil/card/card.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
                                SetUnit, TypeUnit, CategoryUnit, MonsterUnit, URLUnit, CardUnit)
 from ygoutil.card.misc import line_or_not
 
 class Card:
     """ YGO 卡片 """
 
     @cached_property
-    def ids(self):
+    def _id_unit(self):
         return IDUnit(self)
 
     @cached_property
-    def names(self):
+    def _name_unit(self):
         return NameUnit(self)
 
     @cached_property
-    def texts(self):
+    def _text_unit(self):
         return TextUnit(self)
 
     @cached_property
     def _limit_unit(self) -> LimitUnit | None:
         return None
 
     @cached_property
@@ -44,38 +44,50 @@
     @cached_property
     def _url_unit(self) -> URLUnit | None:
         return None
 
     @cached_property
     def _extra_unit(self) -> CardUnit | None:
         return None
-
+    
+    @property
+    def ids(self):
+        return self._id_unit
+    
     @property
     def id(self):
-        return self.ids.id
+        return self._id_unit.id
     
     @id.setter
     def id(self, value: int | str):
-        self.ids.id = value
+        self._id_unit.id = value
+
+    @property
+    def names(self):
+        return self._name_unit
 
     @property
     def name(self):
-        return self.names.name
+        return self._name_unit.name
     
     @name.setter
     def name(self, value: str):
-        self.names.name = value
+        self._name_unit.name = value
     
     @property
+    def texts(self):
+        return self._text_unit
+
+    @property
     def text(self):
-        return self.texts.text
+        return self._text_unit.text
     
     @text.setter
     def text(self, value: str):
-        self.texts.text = value
+        self._text_unit.text = value
 
     @property
     def limits(self):
         if self._limit_unit:
             return self._limit_unit
         raise AttributeError("Card does not have limitation data")
 
@@ -170,25 +182,25 @@
                 self.types.add(t)
 
     def _init_monster(self):
         if self.is_monster:
             self._monster_unit = MonsterUnit(self)
 
     def _info_gen(self):
-        yield line_or_not(self.names.info())             # 卡名
+        yield line_or_not(self._name_unit.info())        # 卡名
         yield line_or_not(self._type_unit.info())        # 类型
-        line = f"{self.ids.info()}"                      # 卡号、禁限、OT
+        line = f"{self._id_unit.info()}"                 # 卡号、禁限、OT
         if self._limit_unit:
             line = f"{line}  {self._limit_unit.info()}"
         yield line_or_not(line)
         if self._set_unit:
             yield line_or_not(self._set_unit.info())     # 字段
         if self._monster_unit:
             yield line_or_not(self._monster_unit.info()) # 怪兽
-        yield self.texts.info()                          # 卡片文本，不用再换行
+        yield self._text_unit.info()                     # 卡片文本，不用再换行
         
     def info(self):
         """ 卡片信息 """
         return "".join(self._info_gen())
         
     def __str__(self):
         return self.info()
```

### Comparing `ygoutil-0.2.0/src/ygoutil/card/constant.py` & `ygoutil-0.2.1/src/ygoutil/card/constant.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/card/unit.py` & `ygoutil-0.2.1/src/ygoutil/card/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,17 +372,17 @@
 
     @mark.setter
     def mark(self, value: tuple[int, int]):
         self.left, self.right = value
 
     def _init_p_text(self):
         if base_unit := check_cached_property(self._owner, "texts"):
-            self._owner.texts = PTextUnit.from_base(base_unit)
+            self._owner._text_unit = PTextUnit.from_base(base_unit)
         else:
-            self._owner.texts = PTextUnit(self._owner)
+            self._owner._text_unit = PTextUnit(self._owner)
 
     def info(self):
         return f"←{self.left} 【灵摆】 {self.right}→" if self.left and self.right else ""
 
 class URLUnit(CardUnit):
     """ 相关链接 """
```

### Comparing `ygoutil-0.2.0/src/ygoutil/dataloader.py` & `ygoutil-0.2.1/src/ygoutil/dataloader.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/legacy/card.py` & `ygoutil-0.2.1/src/ygoutil/legacy/card.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/source/baige/api.py` & `ygoutil-0.2.1/src/ygoutil/source/baige/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 from ygoutil.source.baige.misc import Site, BaiGeResult, BaiGeCard, BaiGeNameUnit, BaiGeExtraUnit
 from ygoutil.source.misc import get_json, USE_CLIENT_DEFAULT, deal_web_text
 from ygoutil.source.cdb.misc import card_from_types, card_from_cdb_data
 
 class BaiGe(CardSource):
     """ 查百鸽 """
 
-    api_url = f"{Site.base_url}api/v0/"
+    _api_url = f"{Site.base_url}api/v0/"
     timeout = USE_CLIENT_DEFAULT
+    """ HTTP 请求的超时时间 """
 
-    def json2card(self, json: BaiGeCard) -> Card:
+    def _json2card(self, json: BaiGeCard) -> Card:
         data = json["data"]
         types = data["type"]
         card = card_from_types(types)
         card = card_from_cdb_data(card, json["id"], data["ot"], 0, data["setcode"], types, 
                                   data["atk"], data["def"], data["level"], data["race"], data["attribute"], 0)
-        card.names = BaiGeNameUnit(card).update_from(json)
-        if isinstance(card.texts, PTextUnit):
-            card.texts.p_text = deal_web_text(json["text"]["pdesc"])
-        card.texts._text = deal_web_text(json["text"]["desc"])
+        card._name_unit = BaiGeNameUnit(card).update_from(json)
+        if isinstance(card._text_unit, PTextUnit):
+            card._text_unit.p_text = deal_web_text(json["text"]["pdesc"])
+        card._text_unit._text = deal_web_text(json["text"]["desc"])
         card._extra_unit = BaiGeExtraUnit(card).update_from(json)
         return card
 
-    def json2ids(self, json: BaiGeCard) -> CnJpEnIDCard:
+    def _json2ids(self, json: BaiGeCard) -> CnJpEnIDCard:
         return CnJpEnIDCard(json["id"], json.get("cn_name", ""), json.get("jp_name", ""), json.get("en_name", ""))
 
     async def from_id(self, card_id: int) -> Card | None:
         return await self.from_query(str(card_id))
     
     async def from_name(self, card_name: str) -> Card | None:
         return await self.from_query(card_name)
@@ -43,22 +44,22 @@
             ...
 
         @overload
         async def _gen_from_query(self, query: str, ids_only: Literal[True] = True) -> AsyncGenerator[CnJpEnIDCard, None]:
             ...
 
     async def _gen_from_query(self, query: str, ids_only = False):
-        result: BaiGeResult = await get_json(self.api_url, params=Site.query_params(query), timeout=self.timeout)
+        result: BaiGeResult = await get_json(self._api_url, params=Site.query_params(query), timeout=self.timeout)
         self.current_query = QueryInfo(query, len(result["result"]))
         for card in result["result"]:
             self.current_query.current += 1
             if ids_only:
-                yield self.json2ids(card)
+                yield self._json2ids(card)
             else:
-                yield self.json2card(card)
+                yield self._json2card(card)
 
     async def gen_from_query(self, query: str) -> AsyncGenerator[Card, None]:
         async for card in self._gen_from_query(query):
             yield card
 
     async def gen_ids_from_query(self, query: str) -> AsyncGenerator[CnJpEnIDCard, None]:
         async for card in self._gen_from_query(query, ids_only=True):
```

### Comparing `ygoutil-0.2.0/src/ygoutil/source/baige/misc.py` & `ygoutil-0.2.1/src/ygoutil/source/baige/misc.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/source/baige/page.py` & `ygoutil-0.2.1/src/ygoutil/source/baige/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,45 +19,47 @@
 
 
 class BaiGePage(CardSource):
     """ 查百鸽网页 """
 
     @property
     def link(self):
+        """ 网页链接 """
         return Site.base_url
 
-    link_mark = {
+    _link_mark = {
         "↙": LinkMark.BottomLeft,
         "↓": LinkMark.Bottom,
         "↘": LinkMark.BottomRight,
         "←": LinkMark.Left,
         "→": LinkMark.Right,
         "↖": LinkMark.TopLeft,
         "↑": LinkMark.Top,
         "↗": LinkMark.TopRight,
     }
 
-    link_name = {"数据库": "database", "db": "database", 
+    _link_name = {"数据库": "database", "db": "database", 
                 "日文": "database_jp", "英文": "database_en", "简中": "database_cn",
                 "q&a": "QA", "脚本": "script", "裁定": "ocg_rule"}
 
     @staticmethod
-    def img_link(card_id):
+    def img_link(card_id: int | str):
+        """ 卡图链接 """
         return Site.card_page_url(card_id)
 
-    def get_html(self, url):
-        res = httpx.get(url, timeout=20)
+    def _get_html(self, url, params=None):
+        res = httpx.get(url, params=params, timeout=20)
         return res.text
 
     # async def asyncGetHTML(self, url):
     #     async with httpx.AsyncClient(timeout=20) as client:
     #         res = await client.get(url)
     #         return res.text
 
-    def html2Card(self, html, card_page=False) -> Generator[Card, None, None]:
+    def _html2Card(self, html, card_page=False) -> Generator[Card, None, None]:
         html = BeautifulSoup(html, "lxml")
         divs = self._html2divs(html, card_page)
         if not divs:
             return None
         # cards = []
         self.current_query.total = len(divs)
         for div in divs:
@@ -103,30 +105,30 @@
                         desc += child
             if not types:
                 return None
             
             c = Card.from_types(*types)
             if TYPE_CHECKING:
                 assert info[1].h2
-            names = c.names = BaiGeNameUnit(c)
+            names = c._name_unit = BaiGeNameUnit(c)
             c._extra_unit = BaiGeExtraUnit(c)
             (c.id, c._extra_unit.c_id, names.cn_name, names.jp_name, names.en_name, names.jp_ruby) = self._div_id_names(info)
             # c.database,c.QA,c.wiki,c.yugipedia,c.ygorg,c.ourocg,c.script,c.ocgRule=[
             #     a.get("href") for a in info[1].find_all("a")]
             # links={ a.text.strip().lower() : a.get("href") for a in info[1].find_all("a")}
             c._url_unit = BaiGeURLUnit(c)
             for atag in info[1].find_all("a"):
                 atag: Tag
                 aname: str = atag.text.strip().lower()  # 链接对应的名称都变成小写了
                 alink = atag.get("href")
                 if TYPE_CHECKING:
                     assert isinstance(alink, str)
-                if aname in self.link_name:
-                    setattr(c._url_unit, self.link_name[aname], alink)
-                elif hasattr(c, aname):
+                if aname in self._link_name:
+                    setattr(c._url_unit, self._link_name[aname], alink)
+                elif hasattr(c._url_unit, aname):
                     setattr(c._url_unit, aname, alink)
                 elif aname.startswith("详情"):
                     if alink.endswith("#faq"):  # /card/xxxx#faq
                         alink = alink[:-4]
                     c.urls.url = f"{self.link[:-1]}{alink}"  # https://ygocdb.com/card/xxxx
 
             # c.database=links.get("数据库")
@@ -178,15 +180,15 @@
                 if isinstance(c.monster.levels, LinkUnit):
                     # c.monster.levels.link = lv
                     c.monster.defence = None
                     marks = data.pop(0).split("]")  # [↑][←][→][↙][↓][↘]
                     for m in marks:
                         m = m.strip("[")
                         if m:
-                            c.monster.levels.marks |= self.link_mark[m]
+                            c.monster.levels.marks |= self._link_mark[m]
                 if c.monster._pmark_unit:
                     if data:
                         marks = data.pop(0).split("/")  # 4/4
                     else:
                         # 刻度是 0/0 时好像不会展示在网页上
                         marks = ("0", "0")
                     marks = tuple(deal_int(m) for m in marks)
@@ -194,62 +196,68 @@
                         marks = int(marks[0]), int(marks[1])
                     c.monster._pmark_unit.mark = marks
                     # pdesc = f"←{marks[0]} 【灵摆】 {marks[1]}→" + pdesc
                     # if c.is_effect:
                     #     desc = desc.format(p="【怪兽效果】")
                     # else:
                     #     desc = desc.format(p="【怪兽描述】")
-                    c.texts = PTextUnit(c)
-                    c.texts.p_text = pdesc.strip()
-            c.texts._text = desc.strip()
+                    c._text_unit = PTextUnit(c)
+                    c._text_unit.p_text = pdesc.strip()
+            c._text_unit._text = desc.strip()
             # cards.append(c)
             yield c
 
             # return c  # 先只找一张卡
 
-    def search(self, text: str | int, by_id=False):
-        if by_id:
-            url = f"{self.link}card/{text}"  # text是卡号
-        else:
-            url = f"{self.link}?search={text}"
-        html = self.get_html(url)
-        return next(self.html2Card(html, card_page=by_id), None)
+    def _search(self, text: str | int, by_id=False):
+        text = str(text)
+        url, params = self._request_url_params(text, by_id)
+        html = self._get_html(url, params)
+        self.current_query = QueryInfo(text)
+        if card := next(self._html2Card(html, card_page=by_id), None):
+            self.current_query.current += 1
+        return card
 
     if TYPE_CHECKING:
         @overload
         async def async_search_gen(self, text: str | int, by_id=False, ids_only : Literal[False] = False) -> AsyncGenerator[Card, None]:
             ...
 
         @overload
         async def async_search_gen(self, text: str | int, by_id=False, ids_only : Literal[True] = True) -> AsyncGenerator[CnJpEnIDCard, None]:
             ...
 
     async def async_search_gen(self, text: str | int, by_id=False, ids_only=False):
         text = str(text)
-        if by_id:
-            url = Site.card_page_url(text)  # text是卡号
-            params = None
-        else:
-            url = f"{self.link}"
-            params = Site.query_params(text)
+        url, params = self._request_url_params(text, by_id)
         html = await get_html(url, params=params, timeout=20)
         self.current_query = QueryInfo(text)   # 在这里初始化 QueryInfo，这样能覆盖所有 CardSource 要求的方法
-        gen = self.html2Card(html, card_page=by_id) if not ids_only else self.html2IDCard(html)
+        gen = self._html2Card(html, card_page=by_id) if not ids_only else self._html2IDCard(html)
         for card in gen:
             self.current_query.current += 1
             yield card
 
     async def async_search(self, text: str | int, by_id=False):
         return await anext(self.async_search_gen(text, by_id), None)
 
     asyncSearch = async_search
 
     # ↑ 之前的老代码 ↑
 
     @staticmethod
+    def _request_url_params(text: str, by_id=False):
+        if by_id:
+            url = Site.card_page_url(text)  # text是卡号
+            params = None
+        else:
+            url = Site.base_url
+            params = Site.query_params(text)
+        return url, params
+
+    @staticmethod
     def _html2divs(html: BeautifulSoup, card_page=False) -> ResultSet[Tag]:
         if card_page:
             return html.find_all("div", {"class": "row card detail"})
         else:
             return html.find_all("div", {"class": "row card result"})
 
     @staticmethod
@@ -285,15 +293,15 @@
     async def from_name(self, card_name: str):
         return await self.async_search(card_name)
 
     async def gen_from_query(self, query: str) -> AsyncGenerator[Card, None]:
         async for card in self.async_search_gen(query):
             yield card
 
-    def html2IDCard(self, html) -> Generator[CnJpEnIDCard, None, None]:
+    def _html2IDCard(self, html) -> Generator[CnJpEnIDCard, None, None]:
         html = BeautifulSoup(html, "lxml")
         divs = self._html2divs(html)
         if not divs:
             return None
         self.current_query.total = len(divs)
         for div in divs:
             info = self._div_card_info(div)
```

### Comparing `ygoutil-0.2.0/src/ygoutil/source/base.py` & `ygoutil-0.2.1/src/ygoutil/source/base.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/source/cdb/misc.py` & `ygoutil-0.2.1/src/ygoutil/source/cdb/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     return card
 
 def card_from_cdb_data(card: Card, id: int, ot: int, alias: int, sets: int, types: int, 
                       attack: int, defence: int, level: int, race: int, attribute: int, category: int,
                       set_map: dict[int, str] = None, lf_map: dict[int, int] = None) -> Card:
     if alias:
         id, alias = alias, id  # alias 里面才是真的卡号，id 里面是替身卡号
-        card.ids = AliasIDUnit(card)
-        card.ids.alias_id = alias
+        card._id_unit = AliasIDUnit(card)
+        card._id_unit.alias_id = alias
     card.id = id
     card._limit_unit = LimitUnit(card)  # 有 LimitUnit
     card.limits.ot = CardOT(ot)
     if lf_map:
         card.limits.limit = CardLF(lf_map.get(card.id, CardLF.无限制))
     if set_map:
         card._set_unit = SetUnit(card)  # 传入 set_map 的话，即使没有字段，也保证 SetUnit 存在
@@ -65,15 +65,15 @@
         monster.level = deal_level(level)
         if isinstance(monster.levels, LinkUnit):
             monster.levels.marks = LinkMark(defence)  # 连接怪用防御记录连接标记
         else:
             monster.defence = deal_atk_def(defence)
         if monster._pmark_unit:
             monster._pmark_unit.mark = deal_p_mark(level)
-            card.texts = PTextUnit(card)  # 灵摆怪兽试用 PTextUnit
+            card._text_unit = PTextUnit(card)  # 灵摆怪兽试用 PTextUnit
         monster.race = CardRace(race)
         monster.attribute = CardAttribute(attribute)
     card._category_unit = CategoryUnit(card)  # 有 CategoryUnit
     card.categories = CardCategory(category)
     return card
 
 def card_from_cdb(name: str, text: str,
```

### Comparing `ygoutil-0.2.0/src/ygoutil/source/misc.py` & `ygoutil-0.2.1/src/ygoutil/source/misc.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/source/ourocg.py` & `ygoutil-0.2.1/src/ygoutil/source/ourocg.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,34 +47,39 @@
     CN = 0
     NW = 1
     DEFAULT = 2
 
 class OurOcg(CardSource):
     """ 查 OurOcg 网页 """
     def __init__(self):
-        self.edition = Translate.DEFAULT
+        self._edition = Translate.DEFAULT
         self.name_search_limit = 10
         """ 
-            from_name 中比对卡名时，最多比对卡片数量\n
+            from_name 中精确比对卡名时，最多比对卡片数量\n
             默认最多 10 张（即 1 页），为 0 时表示无限制
         """
 
-    def SetTranslateEdition(self, ed: str):
-        for trans in Translate:
-            if trans.name == ed.upper():
-                self.edition = trans
-                break
+    def set_translate_edition(self, ed: str):
+        """ 设置译文偏好为 'NW' 或 'CN' """
+        trans = Translate.DEFAULT
+        if any(trans := t for t in Translate if t.name == ed.upper()):
+            self._edition = trans
+
+    SetTranslateEdition = set_translate_edition  # 兼容
+
+    @property
+    def link(self):
+        """ 网页链接 """
+        return Site.base_url
 
-    ourocgLink = Site.base_url
-
-    def GetHTML(self, url):
-        res = httpx.get(url)
+    def _getHTML(self, url):
+        res = httpx.get(url, follow_redirects=True)
         return res.text
 
-    def GetCardHTMLWithJ(self, searchtext: str, url: str, searchHTML: str):
+    def _getCardHTMLWithJ(self, searchtext: str, url: str, searchHTML: str):
         targeturl: str = ""
         cardJson = None
         # Pmark=[None,None]
         html = BeautifulSoup(searchHTML, "lxml")
         if html.find_all("title")[0].string.startswith("搜索"):  # 搜索结果页
             scripts = html.find_all("script")
             for s in scripts:
@@ -100,15 +105,15 @@
                         # Pmark=[tar.get("pend_l",None),tar.get("pend_r",None)]
                     # print(targeturl)
                     break
         else:
             targeturl = url  # 直接是卡片详情页
         return targeturl, cardJson
 
-    def GetCardFromHTML(self, cardHTML, cardJson) -> Card:
+    def _getCardFromHTML(self, cardHTML, cardJson) -> Card:
         if cardJson is None:
             cardJson = {}
         # print(cardJson)
         html = BeautifulSoup(cardHTML, "lxml")
         is_RD = self._is_RD(html)
         # div = html.find_all("div", {"class": "val"})
         # divr=[[y for y in x.stripped_strings] for x in div]
@@ -121,20 +126,20 @@
             linkmark = html.find("div", {"class": "linkMark"})
             if TYPE_CHECKING:
                 assert isinstance(linkmark, Tag)
             for mark in linkmark.find_all("i"):
                 temp = mark["class"][1].split("_")
                 if temp[2] == "on":
                     c.monster.link.marks |= LinkMark.from_number(int(temp[1]), with_mid=True)
-        c.names = CnJpEnNameUnit(c)
-        cn_name, nw_name, c.names.jp_name, c.names.en_name = self._names_from_div(divr)
-        c.names.name = cn_name if self.edition is Translate.CN else nw_name  # 默认是 nw
+        c._name_unit = CnJpEnNameUnit(c)
+        cn_name, nw_name, c._name_unit.jp_name, c._name_unit.en_name = self._names_from_div(divr)
+        c._name_unit.name = cn_name if self._edition is Translate.CN else nw_name  # 默认是 nw
         # c.isRD = isRD
         if is_RD:
-            c.ids = RushDuelIDUnit(c)
+            c._id_unit = RushDuelIDUnit(c)
         else:
             id = divr[4][0]
             id = int(id) if id and id != "-" else 0  # id 可能为 -
             c.id = id
         c._url_unit = URLUnit(c)
         c._url_unit.url = cardJson.get("href", "")    # 如果直接是卡片详情页，就没有
         c._url_unit.pic = cardJson.get("img_url", "")
@@ -196,27 +201,29 @@
         for x in range(-2, -1 * (L + 1), -1):
             if divr[effectnum][x] == tempString:
                 tempnum = -1 - x
                 effectlist.append(L - 2 * tempnum)
                 effectlist.append(effectlist[1] + tempnum)
                 effectlist.append(effectlist[2] + tempnum)
         effects = divr[effectnum][
-            effectlist[self.edition.value] : effectlist[self.edition.value + 1]
+            effectlist[self._edition.value] : effectlist[self._edition.value + 1]
         ]
         effectText = "\n".join(effects)
-        c.text = OurOcg.beautifyText(effectText)
+        c.text = self._beautifyText(effectText)
         return c
 
-    def FindCardByName(self, searchtext):
+    def _findCardByName(self, searchtext):
         url = Site.search_url(searchtext)
-        searchHTML = self.GetHTML(url)
-        targeturl, cardJson = self.GetCardHTMLWithJ(searchtext, url, searchHTML)
+        searchHTML = self._getHTML(url)
+        targeturl, cardJson = self._getCardHTMLWithJ(searchtext, url, searchHTML)
         if targeturl:
-            cardHTML = self.GetHTML(targeturl)
-            return self.GetCardFromHTML(cardHTML, cardJson)
+            self.current_query = OurOcgQueryInfo(searchtext)
+            cardHTML = self._getHTML(targeturl)
+            self.current_query.current += 1
+            return self._getCardFromHTML(cardHTML, cardJson)
         return None
 
     # async def AsyncGetHTML(self, url):
     #     async with httpx.AsyncClient() as client:
     #         res = await client.get(url)
     #         return res.text
 
@@ -225,31 +232,32 @@
     #     searchHTML = await get_html(url)
     #     targeturl, cardJson = self.GetCardHTMLWithJ(searchtext, url, searchHTML)
     #     if targeturl:
     #         cardHTML = await get_html(targeturl)
     #         return self.GetCardFromHTML(cardHTML, cardJson)
     #     return None
 
-    wikiLink = Site.wiki_url
+    _wiki_link = Site.wiki_url
 
-    def getWikiLink(self, card: Card):
+    def _get_wiki_link(self, card: Card):
+        """ 试着从 card 的卡名中得出 wiki 链接 """
         if TYPE_CHECKING:
             assert isinstance(card.names, CnJpEnNameUnit)
         if card.names.jp_name:
-            pageword = f"《{OurOcg.towikistr(card.names.jp_name)}》"
+            pageword = f"《{self._to_wiki_str(card.names.jp_name)}》"
         elif card.names.en_name:
             pageword = f"《{card.names.en_name}》"
         else:
             return None
         pageword = parse.quote(pageword, encoding="euc-jp")
-        return f"{self.wikiLink}index.php?cmd=read&page={pageword}"
+        return f"{self._wiki_link}index.php?cmd=read&page={pageword}"
 
     @staticmethod
-    def towikistr(text: str):
-        """半角转全角，以及一些特殊符号的转换"""
+    def _to_wiki_str(text: str):
+        """ 半角转全角，以及一些特殊符号的转换 """
         transDict = {
             #' ':chr(12288), #半角空格直接转化
             "·": "・",
             "－": "−",
             "Ⅰ": "Ｉ",
             "Ⅱ": "ＩＩ",
             "Ⅲ": "ＩＩＩ",
@@ -272,17 +280,17 @@
                 oc = ord(c)
                 if oc > 32 and oc <= 126:  # 半角字符（除空格）根据关系转化
                     c = chr(oc + 65248)
             r += c
         return r
 
     @staticmethod
-    def beautifyText(text):
-        """试着给效果文本加换行，好看一点"""
-        nums = set(list("①②③④⑤⑥⑦⑧⑨⑩●"))
+    def _beautifyText(text: str):
+        """ 试着给效果文本加换行，好看一点 """
+        nums = set("①②③④⑤⑥⑦⑧⑨⑩●")
         transDict = {"・": "·"}
         r = ""
         length = len(text)
         for i, c in enumerate(text):
             trans = transDict.get(c, None)
             if trans:
                 c = trans
@@ -314,15 +322,15 @@
         if TYPE_CHECKING:
             assert isinstance(cn_name, str) and isinstance(nw_name, str) and isinstance(jp_name, str) and isinstance(en_name, str)
         jp_name = jp_name if jp_name != "-" else ""
         en_name = en_name if en_name != "-" else ""
         jp_name = jp_name.replace("・", "·")
         return cn_name, nw_name, jp_name, en_name
 
-    def card_url_json_gen(self, url: str, html: str):
+    def _card_url_json_gen(self, url: str, html: str):
         root = BeautifulSoup(html, "lxml")
         if TYPE_CHECKING:
             assert root.head
             assert root.body
         title = root.head.find("title")
         if TYPE_CHECKING:
             assert isinstance(title, Tag)
@@ -345,24 +353,24 @@
             self.current_query.current_page = meta.get("cur_page", self.current_query.current_page)
         for one in card_data["cards"]:
             if TYPE_CHECKING:
                 assert isinstance(one, dict)
             target_url = str(one["href"]).replace("\\", "")
             yield target_url, one
 
-    def ids_from_json(self, card_json: dict | None) -> OurOcgIDCard | None:
+    def _ids_from_json(self, card_json: dict | None) -> OurOcgIDCard | None:
         if card_json:
             id = int(card_json.get("password") or 0)
             cn_name = card_json.get("name") or ""
             nw_name = card_json.get("name_nw") or ""
             jp_name = card_json.get("name_ja") or ""
             en_name = card_json.get("name_en") or ""  # 名称可能为 None
             return OurOcgIDCard(id, cn_name, jp_name, en_name, nw_name)
 
-    def ids_from_html(self, card_html) -> OurOcgIDCard:
+    def _ids_from_html(self, card_html) -> OurOcgIDCard:
         html = BeautifulSoup(card_html, "lxml")
         is_RD = self._is_RD(html)
         divr = self._div_data(html)
         cn_name, nw_name, jp_name, en_name = self._names_from_div(divr)
         id = 0 if is_RD else int(divr[4][0])
         return OurOcgIDCard(id, cn_name, jp_name, en_name, nw_name)
 
@@ -380,26 +388,26 @@
             ...
 
     async def search_gen(self, query: str, ids_only = False):
         self.current_query = query_info = OurOcgQueryInfo(query)
         while query_info.current_page <= query_info.total_page:
             url = Site.search_url(query, query_info.current_page)  # 默认最初 current_page = 0
             html = await get_html(url, follow_redirects=True)      # OurOcg 有页面重定向
-            for card_url, card_json in self.card_url_json_gen(url, html):
-                if ids_only and (ids := self.ids_from_json(card_json)):
+            for card_url, card_json in self._card_url_json_gen(url, html):
+                if ids_only and (ids := self._ids_from_json(card_json)):
                     query_info.current += 1
                     yield ids
                     continue
                 if card_url:
                     card_html = await get_html(card_url, follow_redirects=True)
                     query_info.current += 1
                     if ids_only:
-                        yield self.ids_from_html(card_html)
+                        yield self._ids_from_html(card_html)
                     else:
-                        yield self.GetCardFromHTML(card_html, card_json)
+                        yield self._getCardFromHTML(card_html, card_json)
             query_info.current_page += 1
 
     async def from_id(self, card_id: int) -> Card | None:
         return await self.from_query(str(card_id))
 
     async def from_name(self, card_name: str) -> Card | None:
         result = None
```

### Comparing `ygoutil-0.2.0/src/ygoutil/sqlbuilder.py` & `ygoutil-0.2.1/src/ygoutil/sqlbuilder.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/src/ygoutil/ygoRoom.py` & `ygoutil-0.2.1/src/ygoutil/ygoRoom.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,14 +166,16 @@
         if self.serverName.startswith("233"):
             host, port = self.servers.get("233", noserver)
             port = int(f"2{'3'*self.serverName.count('3')}")
         elif self.serverName.endswith("编年史") or self.serverName.lower() == "dc":
             host, port = self.servers.get("编年史", noserver)
         elif self.serverName == "2pick" or self.serverName == "轮抽":
             host, port = self.servers.get("2pick", noserver)
+        elif self.serverName.lower() == "mygo" or self.serverName == "888":
+            host, port = self.servers.get("超先行", noserver)
         elif self.serverName.startswith("复读") or self.serverName.lower() == "repiko":
             host, port = self.servers.get("repiko", noserver)
         else:
             if self.serverName:
                 host, port = self.servers.get(self.serverName, noserver)
             else:
                 host, port = noserver
```

### Comparing `ygoutil-0.2.0/tests/test_cdb.py` & `ygoutil-0.2.1/tests/test_cdb.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/tests/test_source/test_baige.py` & `ygoutil-0.2.1/tests/test_source/test_baige.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import pytest
 
 from ygoutil.card import CardType, LinkMark
 from ygoutil.card.ids import CnJpEnIDCard
 from ygoutil.source import BaiGe
-from ygoutil.source.baige import BaiGePage, BaiGeNameUnit, BaiGeExtraUnit
+from ygoutil.source.baige import BaiGePage, BaiGeNameUnit, BaiGeExtraUnit, BaiGeURLUnit
 
 @pytest.fixture(scope="module")
 def baige():
     return BaiGe()
 
 @pytest.fixture(scope="module")
 def baige_page():
@@ -18,14 +18,15 @@
 async def test_baige(baige: BaiGe):
     card = await baige.from_id(84536654)
     assert card
     assert isinstance(card.names, BaiGeNameUnit)
     assert card.name == "形态变化" and card.names.jp_name == "フォーム・チェンジ"
     assert isinstance(card.extras, BaiGeExtraUnit)
     assert card.extras.c_id == 9068
+    assert card.extras.faqs
 
 @pytest.mark.asyncio
 async def test_baige_multiple(baige: BaiGe):
     cards = await baige.list_from_query("被封印者的", limit=3)
     assert cards
     assert len(cards) == 3
     assert all("被封印者的" in card.name for card in cards)
@@ -44,14 +45,24 @@
 async def test_baige_page(baige_page: BaiGePage):
     card = await baige_page.from_name("解码语者")
     assert card
     assert card.name == "解码语者"
     assert card.monster
     assert card.monster.link.link == 3
     assert card.monster.link.marks == LinkMark.BottomLeft | LinkMark.BottomRight | LinkMark.Top
+    assert isinstance(card.urls, BaiGeURLUnit)
+    assert card.urls.database_cn
+    assert card.urls.database_en
+    assert card.urls.database_jp
+    assert card.urls.QA
+    assert card.urls.wiki
+    assert card.urls.yugipedia
+    assert card.urls.ourocg
+    assert card.urls.script
+    assert card.urls.ocg_rule
 
 @pytest.mark.asyncio
 async def test_baige_page_multiple(baige_page: BaiGePage):
     cards = await baige_page.list_from_query("竹光", limit=6)
     assert cards
     assert len(cards) == 6
     assert all(CardType.Spell in card.types for card in cards)
```

### Comparing `ygoutil-0.2.0/tests/test_source/test_ourocg.py` & `ygoutil-0.2.1/tests/test_source/test_ourocg.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     assert isinstance(card.ids, RushDuelIDUnit)
     assert card.id == "RUSH DUEL"
     assert ourocg.current_query.total_page > 1
 
 @pytest.mark.asyncio
 async def test_ourocg_from_name(ourocg: OurOcg):
     ourocg.name_search_limit = 0
-    ourocg.edition = Translate.CN
+    ourocg.set_translate_edition(Translate.CN.name)
     card = await ourocg.from_name("元素英雄 新宇侠")
     assert card
     assert card.name == "E·HERO 新生人"
 
 @pytest.mark.asyncio
 async def test_ourocg_multiple(ourocg: OurOcg):
     cards = await ourocg.list_from_query("宝札", limit=6)
```

### Comparing `ygoutil-0.2.0/tests/test_sql.py` & `ygoutil-0.2.1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.2.0/PKG-INFO` & `ygoutil-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ygoutil
-Version: 0.2.0
-Summary: 一个 ygo 工具集
+Version: 0.2.1
+Summary: 一个 ygo 工具集 | Handy tools for ygo
 Author: liggest
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: typing-extensions>=4.11.0
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: lxml>=5.2.1
```

