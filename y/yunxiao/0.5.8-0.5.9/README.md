# Comparing `tmp/yunxiao-0.5.8.tar.gz` & `tmp/yunxiao-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.5.8.tar", last modified: Tue Apr 30 16:39:14 2024, max compression
+gzip compressed data, was "yunxiao-0.5.9.tar", last modified: Tue Apr 30 19:52:51 2024, max compression
```

## Comparing `yunxiao-0.5.8.tar` & `yunxiao-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.055216 yunxiao-0.5.8/
--rw-rw-rw-   0        0        0      509 2024-04-30 16:39:14.054214 yunxiao-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.8/README.md
--rw-rw-rw-   0        0        0     2504 2024-04-30 16:39:03.000000 yunxiao-0.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 16:39:14.055216 yunxiao-0.5.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.040215 yunxiao-0.5.8/yunxiao/
--rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.8/yunxiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.052218 yunxiao-0.5.8/yunxiao/schemas/
--rw-rw-rw-   0        0        0      403 2024-04-30 15:15:40.000000 yunxiao-0.5.8/yunxiao/schemas/__init__.py
--rw-rw-rw-   0        0        0     2406 2024-04-30 13:07:02.000000 yunxiao-0.5.8/yunxiao/schemas/achievements.py
--rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.8/yunxiao/schemas/page.py
--rw-rw-rw-   0        0        0     4157 2024-04-30 15:41:58.000000 yunxiao-0.5.8/yunxiao/schemas/payments.py
--rw-rw-rw-   0        0        0     2383 2024-04-30 12:00:14.000000 yunxiao-0.5.8/yunxiao/schemas/teachers.py
--rw-rw-rw-   0        0        0    33724 2024-04-30 16:28:56.000000 yunxiao-0.5.8/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.053216 yunxiao-0.5.8/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 19:52:51.488111 yunxiao-0.5.9/
+-rw-rw-rw-   0        0        0      509 2024-04-30 19:52:51.487110 yunxiao-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.9/README.md
+-rw-rw-rw-   0        0        0     2575 2024-04-30 19:52:40.000000 yunxiao-0.5.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 19:52:51.488111 yunxiao-0.5.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 19:52:51.474110 yunxiao-0.5.9/yunxiao/
+-rw-rw-rw-   0        0        0       85 2024-04-30 19:52:31.000000 yunxiao-0.5.9/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0     2710 2024-04-30 19:52:31.000000 yunxiao-0.5.9/yunxiao/achievements.py
+-rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.9/yunxiao/page.py
+-rw-rw-rw-   0        0        0     2637 2024-04-30 19:52:31.000000 yunxiao-0.5.9/yunxiao/teachers.py
+-rw-rw-rw-   0        0        0    10736 2024-04-30 19:52:31.000000 yunxiao-0.5.9/yunxiao/tradeRecords.py
+-rw-rw-rw-   0        0        0    31714 2024-04-30 19:52:31.000000 yunxiao-0.5.9/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:52:51.486111 yunxiao-0.5.9/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-30 19:52:51.000000 yunxiao-0.5.9/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-30 19:52:51.000000 yunxiao-0.5.9/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 19:52:51.000000 yunxiao-0.5.9/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 19:52:51.000000 yunxiao-0.5.9/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 19:52:51.000000 yunxiao-0.5.9/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.5.8/pyproject.toml` & `yunxiao-0.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.5.8"
+version = "0.5.9"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "sqkkyzx", email = "admin@sqkkyzx.com"},
 ]
 
 dependencies = ["requests"]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.5.9" = "分离各对象，将查询函数迁移为对象方法。"
 "0.5.8" = "新增: 对翻页的日志输出启用色彩。"
 "0.5.7" = "新增: 对 payments 引入 pydantic 做数据验证。"
 "0.5.6" = "新增: 对 achievements 引入 pydantic 做数据验证。"
 "0.5.5" = "新增: 对 teacher 引入 pydantic 做数据验证。"
 "0.5.4" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.3" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.2" = "新增（测试）: 引入pydantic做数据验证。"
```

### Comparing `yunxiao-0.5.8/yunxiao/schemas/achievements.py` & `yunxiao-0.5.9/yunxiao/achievements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pydantic import BaseModel, field_validator, computed_field
 from typing import List, Optional
 from datetime import datetime
 from decimal import Decimal
 import uuid
 import time
-from .page import Page
+from yunxiao import YunXiao, Page
 
 
 class Achievement(BaseModel):
     processDate: datetime
     campusName: str
     orderNo: str
     studentId: int
@@ -78,7 +78,13 @@
     orderFlagIds: List[int] = []
     productName: str = ""
     productTypes: List[int] = []
     studentId: str = ""
     teacherIds: List[int] = []
     _t_: int = int(time.time() * 1000)
     page: Page = Page()
+
+
+def query_achievements(auth: YunXiao, payload: AchievementsQueryPayload) -> Achievements:
+    endpoint = f"https://{auth.host}/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail"
+    result_type = Achievements
+    return auth.pages_looper(endpoint, payload, result_type)
```

### Comparing `yunxiao-0.5.8/yunxiao/schemas/teachers.py` & `yunxiao-0.5.9/yunxiao/teachers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 
 from pydantic import BaseModel, field_validator
 from typing import List, Optional
-from .page import Page
+from yunxiao import YunXiao, Page
 
 
 class _CampusDto(BaseModel):
     id: int
     companyId: int
     teacherId: int
     campusId: int
@@ -95,7 +95,13 @@
     """
     campusIds: List[int] = []
     queryKey: str = ""
     roleIds: List[int] = []
     statusIds: List[int] = []
     _t_: int = int(time.time() * 1000)
     page: Page = Page()
+
+
+def query_teachers(auth: YunXiao, payload: TeschersQueryPayload) -> Teschers:
+    endpoint = f"https://{auth.host}/api/cs-pc-crm/teacher/pageList"
+    result_type = Teschers
+    return auth.pages_looper(endpoint, payload, result_type)
```

### Comparing `yunxiao-0.5.8/yunxiao/yunxiao.py` & `yunxiao-0.5.9/yunxiao/yunxiao.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import time
 import requests
-from .schemas import *
 
 
 def timestamp():
     return int(time.time() * 1000)
 
 
 class YunXiao:
@@ -107,15 +106,15 @@
                     page += 1  # 翻页
                 return data_list
 
             return wrapper
 
         return wrapper_func
 
-    def _loop_pages(self, endpoint, payload, schemas):
+    def pages_looper(self, endpoint, payload, schemas):
         response = schemas()  # 结果列表
         response.page.pageSize = payload.page.pageSize
         while payload.page.pageNum <= response.page.totalPage:
             res = self.request(method="post", url=endpoint, json=payload.model_dump())
             try:
                 new = schemas(**res)
                 response.data.extend(new.data)
@@ -199,20 +198,14 @@
                 "refundMoney": data['totalRefundMoney'],
                 "refundStudentSize": 0,
                 "walletMoney": data['totalWalletMoney']
             }
         )
         return data_list
 
-    def teachers_query(self, payload: TeschersQueryPayload) -> Teschers:
-        """
-        查询老师。
-        """
-        return self._loop_pages(f"https://{self.host}/api/cs-pc-crm/teacher/pageList", payload, Teschers)
-
     # 查询意向（APP接口）
     @loop_pages()
     def intentions_query(self, page, size, distributeStatus: int = 1, keyWord: str = "", level: int = "",
                          nonFollowUpDays: int = "", startNextTime: str = "", endNextTime: str = "",
                          startLastCommunicateTime: str = "", endLastCommunicateTime: str = ""):
         """
         查询意向
@@ -738,43 +731,14 @@
                 "endTime": end_date,
                 "creatorIds": [],
                 "comeFroms": [],
                 "phone": ""
             }
         )
 
-    # 查询收支明细-支出
-    @loop_pages("paymentRefundDtos")
-    def payments_query_refund(self, page, size, startdate: str = "", enddate: str = ""):
-        """
-        列出指定操作日期范围的所有订单记录
-        :param size: 每次取数据的分片量
-        :param page: 从第几页开始取数据
-        :param enddate: YY-MM-DD
-        :param startdate: YY-MM-DD
-        :return:
-        """
-        return self.request(
-            method="post",
-            url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentRefundList",
-            json={
-                "_t_": timestamp(),
-                "page": {"pageNum": page, "pageSize": size},
-                "campusIds": self.campus,
-                "refundFinishStartTime": startdate,
-                "refundFinishEndTime": enddate,
-                "orderNo": "",
-                "paymentAccountCustomIds": [],
-                "cardName": "",
-                "refundMethodList": [],
-                "confirmStatusList": [],
-                "phone": ""
-            }
-        )
-
     # 查询收支明细-账户明细
     @loop_pages()
     def payments_account_record(self, page, size, startdate: str = "", enddate: str = "", displayInvalidOrder=False,
                                 typeList: tuple = (), paymentAccountCustomIds: tuple = ()):
         return self.request(
             method="post",
             url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentAccountCustomRecord",
@@ -815,32 +779,14 @@
             url=f"https://{self.host}/api/cs-edu/orderInfo/get",
             params={
                 "orderInfoId": orderinfo_id,
                 "_t_": timestamp()
             }
         )["data"]
 
-    # 查询签单业绩
-    def achievements_query(self, payload: AchievementsQueryPayload) -> Achievements:
-        """
-        查询业绩。
-        """
-        return self._loop_pages(
-            f"https://{self.host}/api/cs-pc-report/cs-report/reports/findAchievementBelongerDetail",
-            payload, Achievements)
-
-    # 查询收入明细
-    def payments_query(self, payload: PaymentsQueryPayload) -> Payments:
-        """
-        查询业绩。
-        """
-        return self._loop_pages(
-            f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentList",
-            payload, Payments)
-
     # 查询招生来源
     def comefroms_query(self):
         return self.request(
             method="get",
             url=f"https://{self.host}/api/cs-crm/customField/get",
             params={"_t_": timestamp(), "customFieldId": "26118419"}
         )["data"]["selectItemList"]
```

