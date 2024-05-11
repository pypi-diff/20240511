# Comparing `tmp/FreeBack-4.6.1b0.tar.gz` & `tmp/FreeBack-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-4.6.1b0.tar", last modified: Thu Apr 25 13:12:33 2024, max compression
+gzip compressed data, was "FreeBack-4.6.3.tar", last modified: Sat May 11 10:18:07 2024, max compression
```

## Comparing `FreeBack-4.6.1b0.tar` & `FreeBack-4.6.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-25 13:12:33.687811 FreeBack-4.6.1b0/
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-25 13:12:33.686634 FreeBack-4.6.1b0/FreeBack/
--rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.6.1b0/FreeBack/__init__.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    39718 2024-04-25 03:13:09.000000 FreeBack-4.6.1b0/FreeBack/alpha.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    33139 2024-04-25 03:13:09.000000 FreeBack-4.6.1b0/FreeBack/barbybar.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    14423 2024-04-25 03:13:09.000000 FreeBack-4.6.1b0/FreeBack/display.py
--rw-r--r--   0 h1nlee     (501) staff       (20)     9918 2024-04-25 03:13:09.000000 FreeBack-4.6.1b0/FreeBack/event.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    15861 2024-04-25 09:13:18.000000 FreeBack-4.6.1b0/FreeBack/my_pd.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    37065 2024-04-25 13:03:14.000000 FreeBack-4.6.1b0/FreeBack/post.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    10240 2024-04-25 12:59:25.000000 FreeBack-4.6.1b0/FreeBack/strat.py
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-25 13:12:33.687388 FreeBack-4.6.1b0/FreeBack.egg-info/
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-25 13:12:33.000000 FreeBack-4.6.1b0/FreeBack.egg-info/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-25 13:12:33.000000 FreeBack-4.6.1b0/FreeBack.egg-info/SOURCES.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-25 13:12:33.000000 FreeBack-4.6.1b0/FreeBack.egg-info/dependency_links.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)       74 2024-04-25 13:12:33.000000 FreeBack-4.6.1b0/FreeBack.egg-info/requires.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-25 13:12:33.000000 FreeBack-4.6.1b0/FreeBack.egg-info/top_level.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.6.1b0/LICENSE
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-25 13:12:33.687570 FreeBack-4.6.1b0/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.6.1b0/README.md
--rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-25 13:12:33.687860 FreeBack-4.6.1b0/setup.cfg
--rw-r--r--   0 h1nlee     (501) staff       (20)     1268 2024-04-25 13:12:24.000000 FreeBack-4.6.1b0/setup.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-05-11 10:18:07.947171 FreeBack-4.6.3/
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-05-11 10:18:07.946011 FreeBack-4.6.3/FreeBack/
+-rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.6.3/FreeBack/__init__.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    39718 2024-04-25 03:13:09.000000 FreeBack-4.6.3/FreeBack/alpha.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    33139 2024-04-25 03:13:09.000000 FreeBack-4.6.3/FreeBack/barbybar.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    15152 2024-05-09 16:37:18.000000 FreeBack-4.6.3/FreeBack/display.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     9918 2024-04-25 03:13:09.000000 FreeBack-4.6.3/FreeBack/event.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    15861 2024-04-25 13:13:23.000000 FreeBack-4.6.3/FreeBack/my_pd.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    37428 2024-05-11 09:07:36.000000 FreeBack-4.6.3/FreeBack/post.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    11504 2024-05-11 10:03:35.000000 FreeBack-4.6.3/FreeBack/strat.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-05-11 10:18:07.946710 FreeBack-4.6.3/FreeBack.egg-info/
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1046 2024-05-11 10:18:07.000000 FreeBack-4.6.3/FreeBack.egg-info/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      305 2024-05-11 10:18:07.000000 FreeBack-4.6.3/FreeBack.egg-info/SOURCES.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-05-11 10:18:07.000000 FreeBack-4.6.3/FreeBack.egg-info/dependency_links.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-05-11 10:18:07.000000 FreeBack-4.6.3/FreeBack.egg-info/top_level.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.6.3/LICENSE
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1046 2024-05-11 10:18:07.946894 FreeBack-4.6.3/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      622 2024-04-25 13:23:42.000000 FreeBack-4.6.3/README.md
+-rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-05-11 10:18:07.947215 FreeBack-4.6.3/setup.cfg
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1271 2024-05-11 10:17:57.000000 FreeBack-4.6.3/setup.py
```

### Comparing `FreeBack-4.6.1b0/FreeBack/alpha.py` & `FreeBack-4.6.3/FreeBack/alpha.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.6.1b0/FreeBack/barbybar.py` & `FreeBack-4.6.3/FreeBack/barbybar.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.6.1b0/FreeBack/display.py` & `FreeBack-4.6.3/FreeBack/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,39 @@
     fig,ax = plt.subplots(r,c,sharex=sharex, sharey=sharey,figsize=(w,d))
     plt.subplots_adjust(left=None, bottom=None, right=None, top=None, hspace = None, wspace=0.5)
         
     plt.gcf().autofmt_xdate()
 
     return plt, fig, ax
 
+# 获取月度统计量
+# method， 
+# total_return 一般收益率总收益
+# total_lr 对数收益率的总收益
+# sum 求和
+# mul 乘积 
+def get_month(ser, method='total_return'):
+    if ser.name == None:
+        name = 0 
+    else:
+        name = ser.name
+    df = ser.reset_index()
+    # 筛出同月数据
+    df['month'] = df['date'].apply(lambda x: x - datetime.timedelta(x.day-1))
+    df = df.set_index('month')[name]
+    # 月度统计量
+    if method=='total_return':
+        return (((df+1).groupby('month')).prod()-1)*100
+    elif method=='total_lr':
+        return (np.exp(df.groupby('month').sum()) - 1)*100
+    elif method=='sum':
+        return df.groupby('month').sum()
+    elif method=='mul':
+        return df.groupby('month').prod()
+
 # 月度数据热力图  
 # period_value 为pd.Series index month ‘2023-7-1’  value  0: ***
 # color_threshold 为红绿色分界点
 def month_thermal(period_value, color_threshold=0):   
     # 数值>0红色，<0为绿色。转化为颜色[R,G,B]
     def color_map(x, max_r):
         if x>0:
@@ -86,17 +111,15 @@
     i = np.array(list(set(i)))
     i.sort()
     ax.set(yticks=i)
     # 年份
     years = sorted(list(set([i.year for i in period_value.index])))
     ax.set_yticklabels(years)
     # 设置横坐标 月份
-    j = np.array(list(set(j)))
-    j.sort()
-    ax.set(xticks=j)
+    ax.set(xticks=list(range(12)))
     ax.set_xticklabels(['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
                                 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'])
     # 关闭网格
     ax.grid(False)
     # 显示数值
     for i_ in i:
         for j_ in j:
```

### Comparing `FreeBack-4.6.1b0/FreeBack/event.py` & `FreeBack-4.6.3/FreeBack/event.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.6.1b0/FreeBack/my_pd.py` & `FreeBack-4.6.3/FreeBack/my_pd.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.6.1b0/FreeBack/post.py` & `FreeBack-4.6.3/FreeBack/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,20 +378,23 @@
         # 持仓表(名称，代码，持仓量，持仓额)
         result_hold = pd.DataFrame()
         for date in self.held.index.get_level_values(0).unique():
             temp = self.held.loc[date].sort_values(by='amount', ascending=False)
             iamount = 0
             for idx,val in temp.iterrows():
                 if 'name' in self.market.columns:
-                    keystring = val['name']+'('+str(idx)+')'+ ', 持仓量：'+str(val['hold'])+', 持仓额：'+str(val['amount'])
+                    #keystring = val['name']+'('+str(idx)+')'+ ', 持仓量：'+str(val['hold'])+', 持仓额：'+str(val['amount'])
+                    keystring = val['name']+'('+str(idx)+')'+ ', 仓位：'+str(round(100*val['amount']/self.net.loc[date], 2))+'%'
                 else:
-                    keystring = str(idx) + ', 持仓量：'+str(round(val['hold'],0))+', 持仓额：'+str(round(val['amount'],1))
+                    #keystring = str(idx) + ', 持仓量：'+str(round(val['hold'],0))+', 持仓额：'+str(round(val['amount'],1))
+                    keystring = str(idx) + ', 仓位：'+str(round(100*val['amount']/self.net.loc[date], 2))+'%'
                 result_hold.loc[date, 'hold%s'%iamount] = keystring
                 iamount += 1
         result_hold = result_hold.join(pd.DataFrame(10000*self.returns).rename(columns={0:'收益率(万)'}))
+        result_hold = result_hold.join(pd.DataFrame(round(100*self.turnover,2)).rename(columns={0:'换手率(%)'}))
         result_hold.index.name = '日期'
         self.result_hold = result_hold
 
         FB.display.write_df(result_hold , "./output/持仓表", col_width={'A':10})
 
         #self.result_hold = pd.Series(result_hold)
         #self.result_hold.to_excel('./output/hold.xlsx')
```

### Comparing `FreeBack-4.6.1b0/FreeBack/strat.py` & `FreeBack-4.6.3/FreeBack/strat.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ###################################################################
 
 
 
 # 择股策略、元策略
 class MetaStrat():
     # 'inexclude':,
-        # 当格式为('bool', False)时， 'bool'列为筛选条件, True为符合条件的证券
-        # 格式为（False, 'bool'), 'bool'列为排除条件, False为符合条件的证券
+        # 当格式为('bool', False)时， 'bool'列为筛选条件, 'bool'为True为符合条件的证券
+        # 格式为（False, 'bool'), 'bool'列为排除条件, 'bool'为False为符合条件的证券
         # 格式为 ['code0', 'code1', ] 时为等权持有固定证券组合，'cash'表示持有现金
     # 'score':float,   按score列由大到小选取证券,等权持有
     # 'hold_num':float,    取前hold_num（大于1表示数量，小于1小于百分比）只
     # market，pd.DataFrame, 需要包括策略需要调取的列，可以先不加
     # price，当前日期可以获得的价格数据,可以使用 'close'收盘价（有一点未来信息），或者下根bar开盘价/TWAP/VWAP
     def __init__(self, inexclude, score=None, hold_num=None, market=None, price='close', interval=1):
         self.inexclude = inexclude
@@ -31,15 +31,15 @@
     def add_cash(self):
         cash = pd.DataFrame(index=self.market.index.get_level_values(0).unique())
         cash['code']  = 'cash'
         cash['name'] = '现金'
         cash[self.price] = 1
         cash = cash.reset_index().set_index(['date', 'code'])
         self.market = pd.concat([self.market, cash]).sort_values('date')
-    # 获得持仓表(持仓张数)
+    # 获得虚拟持仓表(价格每一时刻货值都为1的持仓张数)
     def get_hold(self):
         # 按列表持股
         if type(self.inexclude)==list:
             if 'cash' in (self.inexclude):
                 self.add_cash()
             df_hold = self.market.loc[:, self.inexclude, :]
         # 按排除、排序规则持股
@@ -55,53 +55,77 @@
                 df_hold = pd.concat([self.market.loc[lost_bars, 'cash', :], df_hold])
         # 等权（总账户市值1块钱）
         df_hold = (1/df_hold[self.price].unstack()).fillna(0)
         df_hold = df_hold.apply(lambda x: x/(x!=0).sum(), axis=1)
         # 去掉一直持仓为0的品种
         always_not_hold = (df_hold==0).all()
         self.df_hold = df_hold[always_not_hold[~always_not_hold].index].copy()
+    ## 调仓间隔不为1时，需考虑调仓问题
+    #def get_interval(self):
+    #    if self.interval!=1:
+    #        # 以interval为周期 调整持仓的持仓表
+    #        # 选取的index  interval = 3  0,0,0,3,3,3,6...
+    #        take_hold = [self.df_hold.index[int(i/self.interval)*self.interval]\
+    #                            for i in range(len(self.df_hold.index))]
+    #        real_hold = self.df_hold.loc[take_hold].copy()
+    #        ## 提取的index非连续，复原到原来的连续交易日index
+    #        real_hold.index = self.df_hold.index
+    #        # 去掉一直持仓为0的品种
+    #        always_not_hold = (real_hold==0).all()
+    #        self.df_hold = real_hold[always_not_hold[~always_not_hold].index].copy()
     # 调仓间隔不为1时，需考虑调仓问题
-    def get_interval(self):
+    def get_interval(self, df):
         if self.interval!=1:
-            # 以interval为周期 调整持仓的持仓表
+            # 以interval为周期 获取df 
             # 选取的index  interval = 3  0,0,0,3,3,3,6...
-            take_hold = [self.df_hold.index[int(i/self.interval)*self.interval]\
-                                for i in range(len(self.df_hold.index))]
-            real_hold = self.df_hold.loc[take_hold].copy()
+            take_df = [df.index[int(i/self.interval)*self.interval]\
+                                for i in range(len(df.index))]
+            real_df = df.loc[take_df].copy()
             ## 提取的index非连续，复原到原来的连续交易日index
-            real_hold.index = self.df_hold.index
-            # 去掉一直持仓为0的品种
-            always_not_hold = (real_hold==0).all()
-            self.df_hold = real_hold[always_not_hold[~always_not_hold].index].copy()
+            real_df.index = df.index
+            return real_df
+        return False
     # 运行策略
     def run(self):
         self.get_hold()
-        self.get_interval()
+        #self.get_interval()
+        df_hold = self.get_interval(self.df_hold)
+        if df_hold:
+            # 如果不是每日再平衡的话，可能会有品种一只持仓为0，去掉一直持仓为0的品种
+            always_not_hold = (df_hold==0).all()
+            self.df_hold = df_hold[always_not_hold[~always_not_hold].index].copy()
         # 判断cash是否在持仓，如果在的话避免price没有cash列
         if 'cash' in self.df_hold.columns:
             self.add_cash()
         # 价格矩阵，去掉全是0的列
         self.df_price = pd.DataFrame(self.market[self.price]).\
             pivot_table(self.price, 'date' ,'code')[self.df_hold.columns].copy()
-        # 货值矩阵
+        # 虚拟货值矩阵
         self.df_amount = (self.df_hold*self.df_price).fillna(0)
         # 权重矩阵
         self.df_weight = (self.df_amount.apply(lambda x: (x/x.sum()).fillna(0), axis=1))
         # 净值贡献矩阵
         returns = (self.df_price/self.df_price.shift() - 1).fillna(0)
         self.df_contri = (self.df_weight.shift()*returns).fillna(0)
-        self.returns = self.df_contri.sum(axis=1)    
+        self.returns = self.df_contri.sum(axis=1)
+        self.net = (self.returns+1).cumprod()
+        # 获得真实持仓市值与持仓张数(净值需要interval)
+        net = self.get_interval(self.net)
+        if not net:
+            net = self.net
+        self.df_amount = self.df_amount.mul(list(net.values), axis=0)
+        self.df_hold = self.df_hold.mul(list(net.values), axis=0)
         # 交易金额
         delta_hold = self.df_hold-self.df_hold.shift().fillna(0)
         self.delta_amount = (delta_hold*self.df_price).fillna(0)
         # cash的变化不会带来换手，可能没有‘cash'列
         if 'cash' in self.df_hold.columns:
-            self.turnover = abs(self.delta_amount.drop(columns='cash').sum(axis=1))/self.df_amount.sum(axis=1)
+            self.turnover = abs(self.delta_amount).drop(columns='cash').sum(axis=1)/self.net
         else:
-            self.turnover = abs(self.delta_amount.sum(axis=1))/self.df_amount.sum(axis=1)
+            self.turnover = abs(self.delta_amount).sum(axis=1)/self.net
 
 
 
 # 组合策略、择时策略
 # 根据择时条件选择陪着不同的择股策略
 # conds = [满足条件0的交易日（index或lsit），满足条件1的交易日, ..., 满足条件n的交易日]
 # strats =[条件0对应策略0（MetaStrat）,   非条件0且条件1对应策略1, ... , 非条件0到条件n-1且条件n对应策略n， 剩余时间执行条件n+1]
```

### Comparing `FreeBack-4.6.1b0/FreeBack.egg-info/PKG-INFO` & `FreeBack-4.6.3/FreeBack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.6.1b0
+Version: 4.6.3
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # -----------------------Module------------------------
 
-**barbybar**： 逐k线，逐笔成交的事件驱动回测
+**strat**： 择股和择时策略的快速回测框架
 
-**alpha**: 因子测试
+**barbybar**：逐k线，逐笔成交的事件驱动回测
+
+**alpha**：因子测试
 
 **event**：事件信号测试
 
 **post**： 后处理模块
 
 **display**： 可视化模块
```

### Comparing `FreeBack-4.6.1b0/LICENSE` & `FreeBack-4.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeBack-4.6.1b0/PKG-INFO` & `FreeBack-4.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.6.1b0
+Version: 4.6.3
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # -----------------------Module------------------------
 
-**barbybar**： 逐k线，逐笔成交的事件驱动回测
+**strat**： 择股和择时策略的快速回测框架
 
-**alpha**: 因子测试
+**barbybar**：逐k线，逐笔成交的事件驱动回测
+
+**alpha**：因子测试
 
 **event**：事件信号测试
 
 **post**： 后处理模块
 
 **display**： 可视化模块
```

### Comparing `FreeBack-4.6.1b0/README.md` & `FreeBack-4.6.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -----------------------Module------------------------
 
-**barbybar**： 逐k线，逐笔成交的事件驱动回测
+**strat**： 择股和择时策略的快速回测框架
 
-**alpha**: 因子测试
+**barbybar**：逐k线，逐笔成交的事件驱动回测
+
+**alpha**：因子测试
 
 **event**：事件信号测试
 
 **post**： 后处理模块
 
 **display**： 可视化模块
```

### Comparing `FreeBack-4.6.1b0/setup.py` & `FreeBack-4.6.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,32 +5,32 @@
     long_description = fh.read()
 
 setup(
     name="FreeBack",
     # 版本号: 第几次模块增加，第几次函数增加，第几次函数功能修改
     # (每次高级别序号增加后,低级别序号归0)
     # alpha为调试版,beta为测试版,stable为稳定版 
-    version="4.6.1-beta",
+    version="4.6.3",
     author="LH.Li,zzq",
     author_email="lh98lee@zju.edu.cn",  
     description='Package for backtest',
     long_description=long_description, 
     # 描述文件为md格式
     long_description_content_type="text/markdown",
     url="https://github.com/LHanLi/FreeBack",
     packages=find_packages(),
     install_requires = [
-        'pandas',
-        'scipy',
-        'statsmodels',
-        'seaborn',
-        'plottable',
-        'pyecharts',
-        'numpy_ext',
-        'xlsxwriter'
+        #'pandas',
+        #'scipy',
+        #'statsmodels',
+        #'seaborn',
+        #'plottable',
+        #'pyecharts',
+        #'numpy_ext',
+        #'xlsxwriter'
     ],
     classifiers=[
          # 该软件包仅与Python3兼容
         "Programming Language :: Python :: 3",
         # 根据GPL 3.0许可证开源
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         # 与操作系统无关
```

