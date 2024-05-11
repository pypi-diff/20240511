# Comparing `tmp/csv2notion_neo-1.2.4.tar.gz` & `tmp/csv2notion_neo-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2notion_neo-1.2.4.tar", max compression
+gzip compressed data, was "csv2notion_neo-1.2.5.tar", max compression
```

## Comparing `csv2notion_neo-1.2.4.tar` & `csv2notion_neo-1.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     2573 2024-02-12 01:35:19.401038 csv2notion_neo-1.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     1068 2024-02-12 01:35:19.401038 csv2notion_neo-1.2.4/LICENSE
--rw-r--r--   0        0        0    27880 2024-02-12 01:35:19.405038 csv2notion_neo-1.2.4/README.md
--rw-r--r--   0        0        0        0 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/__init__.py
--rw-r--r--   0        0        0      119 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/__main__.py
--rw-r--r--   0        0        0     3195 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/cli.py
--rw-r--r--   0        0        0    11825 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/cli_args.py
--rw-r--r--   0        0        0     2348 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/cli_steps.py
--rw-r--r--   0        0        0     5499 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/local_data.py
--rw-r--r--   0        0        0        0 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/__init__.py
--rw-r--r--   0        0        0    24687 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/block.py
--rw-r--r--   0        0        0    16883 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/client.py
--rw-r--r--   0        0        0    27149 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/collection.py
--rw-r--r--   0        0        0      108 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/logger.py
--rw-r--r--   0        0        0     3693 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/maps.py
--rw-r--r--   0        0        0     9350 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/markdown.py
--rw-r--r--   0        0        0     8200 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/monitor.py
--rw-r--r--   0        0        0      997 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/operations.py
--rw-r--r--   0        0        0     4480 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/records.py
--rw-r--r--   0        0        0      290 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/settings.py
--rw-r--r--   0        0        0     9398 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/smoke_test.py
--rw-r--r--   0        0        0     1636 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/space.py
--rw-r--r--   0        0        0    15012 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/store.py
--rw-r--r--   0        0        0     1258 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/user.py
--rw-r--r--   0        0        0     2851 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/utils.py
--rw-r--r--   0        0        0     2279 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion/utils_ssl.py
--rw-r--r--   0        0        0    12252 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_convert.py
--rw-r--r--   0        0        0     1922 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_convert_map.py
--rw-r--r--   0        0        0     6699 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_db.py
--rw-r--r--   0        0        0     2072 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_db_client.py
--rw-r--r--   0        0        0     5074 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_db_collection.py
--rw-r--r--   0        0        0     9697 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_preparator.py
--rw-r--r--   0        0        0     9775 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_row.py
--rw-r--r--   0        0        0     4147 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_row_image_block.py
--rw-r--r--   0        0        0     2775 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_row_upload_file.py
--rw-r--r--   0        0        0     1126 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_type_guess.py
--rw-r--r--   0        0        0     1766 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/notion_uploader.py
--rw-r--r--   0        0        0     1276 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/utils_db.py
--rw-r--r--   0        0        0      305 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/utils_exceptions.py
--rw-r--r--   0        0        0      331 2024-02-12 01:35:19.845037 csv2notion_neo-1.2.4/csv2notion_neo/utils_file.py
--rw-r--r--   0        0        0      679 2024-02-12 01:35:19.849037 csv2notion_neo-1.2.4/csv2notion_neo/utils_rand_id.py
--rw-r--r--   0        0        0     1792 2024-02-12 01:35:19.849037 csv2notion_neo-1.2.4/csv2notion_neo/utils_static.py
--rw-r--r--   0        0        0      249 2024-02-12 01:35:19.849037 csv2notion_neo-1.2.4/csv2notion_neo/utils_str.py
--rw-r--r--   0        0        0     1387 2024-02-12 01:35:19.849037 csv2notion_neo-1.2.4/csv2notion_neo/utils_threading.py
--rw-r--r--   0        0        0       22 2024-02-12 01:35:19.849037 csv2notion_neo-1.2.4/csv2notion_neo/version.py
--rw-r--r--   0        0        0     5334 2024-02-12 01:35:19.849037 csv2notion_neo-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    29844 1970-01-01 00:00:00.000000 csv2notion_neo-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2933 2024-05-11 07:26:46.563915 csv2notion_neo-1.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1068 2024-05-11 07:26:46.563915 csv2notion_neo-1.2.5/LICENSE
+-rw-r--r--   0        0        0    27658 2024-05-11 07:26:46.563915 csv2notion_neo-1.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/__main__.py
+-rw-r--r--   0        0        0     3195 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/cli.py
+-rw-r--r--   0        0        0    11825 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/cli_args.py
+-rw-r--r--   0        0        0     2348 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/cli_steps.py
+-rw-r--r--   0        0        0     5533 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/local_data.py
+-rw-r--r--   0        0        0        0 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/__init__.py
+-rw-r--r--   0        0        0    24846 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/block.py
+-rw-r--r--   0        0        0    16051 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/client.py
+-rw-r--r--   0        0        0    27147 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/collection.py
+-rw-r--r--   0        0        0     1107 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/logger.py
+-rw-r--r--   0        0        0     3725 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/maps.py
+-rw-r--r--   0        0        0     9350 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/markdown.py
+-rw-r--r--   0        0        0     8200 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/monitor.py
+-rw-r--r--   0        0        0     1021 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/operations.py
+-rw-r--r--   0        0        0     4898 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/records.py
+-rw-r--r--   0        0        0      671 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/settings.py
+-rw-r--r--   0        0        0     9398 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/smoke_test.py
+-rw-r--r--   0        0        0     1636 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/space.py
+-rw-r--r--   0        0        0    14842 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/store.py
+-rw-r--r--   0        0        0      546 2024-05-11 07:26:47.003920 csv2notion_neo-1.2.5/csv2notion_neo/notion/user.py
+-rw-r--r--   0        0        0     2851 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion/utils.py
+-rw-r--r--   0        0        0     2279 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion/utils_ssl.py
+-rw-r--r--   0        0        0    12437 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_convert.py
+-rw-r--r--   0        0        0     1922 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_convert_map.py
+-rw-r--r--   0        0        0     6697 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_db.py
+-rw-r--r--   0        0        0     2072 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_db_client.py
+-rw-r--r--   0        0        0     5092 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_db_collection.py
+-rw-r--r--   0        0        0     9697 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_preparator.py
+-rw-r--r--   0        0        0     9799 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_row.py
+-rw-r--r--   0        0        0     4151 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_row_image_block.py
+-rw-r--r--   0        0        0     2908 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_row_upload_file.py
+-rw-r--r--   0        0        0     1126 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_type_guess.py
+-rw-r--r--   0        0        0     1759 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/notion_uploader.py
+-rw-r--r--   0        0        0     1276 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_db.py
+-rw-r--r--   0        0        0      305 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_exceptions.py
+-rw-r--r--   0        0        0      331 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_file.py
+-rw-r--r--   0        0        0      679 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_rand_id.py
+-rw-r--r--   0        0        0     1792 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_static.py
+-rw-r--r--   0        0        0      249 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_str.py
+-rw-r--r--   0        0        0     1387 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/utils_threading.py
+-rw-r--r--   0        0        0       22 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/csv2notion_neo/version.py
+-rw-r--r--   0        0        0     5334 2024-05-11 07:26:47.007920 csv2notion_neo-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    29622 1970-01-01 00:00:00.000000 csv2notion_neo-1.2.5/PKG-INFO
```

### Comparing `csv2notion_neo-1.2.4/CHANGELOG.md` & `csv2notion_neo-1.2.5/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+### 1.2.5
+
+**🎉 Released:**
+- 10th May 2024
+
+**🔨 Improvements:**
+- Improved image and icon upload logic (#32)
+- Improved `--payload-key-column` logic (#33)
+- Updated dependencies packages
+
+**🐞 Bug Fix:**
+- Fixed can't able to upload images due to Notion API changes (#32)
+- Fixed can't duplicate item within Notion when using CSV2Notion Neo (#3)
+
+---
+
 ### 1.2.4
 
 **🎉 Released:**
 - 12th February 2024
 
 **🔨 Improvements:**
 - Added logic for `--merge-only-column` for `.json` data (#27)
```

### Comparing `csv2notion_neo-1.2.4/LICENSE` & `csv2notion_neo-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/README.md` & `csv2notion_neo-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-<a href="https://github.com/TheAcharya/csv2notion-neo"><img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/CSV2Notion Neo_Icon.png?raw=true" width="200" alt="App icon" align="left"/>
+<p align="center">
+  <a href="https://github.com/TheAcharya/csv2notion-neo"><img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/CSV2Notion Neo_Icon.png?raw=true" height="200">
+  <h1 align="center">CSV2Notion Neo</h1>
+</p>
+
 
-<div>
-<h1>CSV2Notion Neo</h1>
-<!-- PyPI -->
-<a href="https://pypi.python.org/pypi/csv2notion-neo">
-<img src="https://img.shields.io/pypi/v/csv2notion-neo?label=version" alt="PyPI"/>
-</a>
-<!-- Python -->
-<a href="https://pypi.org/project/csv2notion-neo/">
-<img src="https://img.shields.io/pypi/pyversions/csv2notion-neo.svg" alt="Python"/>
-</a>
-<!-- release_github -->
-<a href="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml">
-<img src="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml/badge.svg" alt="release_github"/>
-</a>
-<p>
-<p>An advance method to upload & merge *.csv or *.json files with images to <a href="https://notion.so/" target="_blank">Notion</a> database.
-
-<br>
-<br>
-</div>
+<p align="center">
+  <a href="https://github.com/TheAcharya/csv2notion-neo/blob/main/LICENSE">
+    <img src="http://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat" alt="license"/>
+  </a>
+  <a href="https://pypi.python.org/pypi/csv2notion-neo">
+    <img src="https://img.shields.io/pypi/v/csv2notion-neo?label=version" alt="PyPI"/>
+  </a>
+  <a href="https://pypi.org/project/csv2notion-neo/">
+    <img src="https://img.shields.io/pypi/pyversions/csv2notion-neo.svg" alt="Python"/>
+  </a>
+  <a href="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml">
+    <img src="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml/badge.svg" alt="release_github"/>
+  </a>
+</p>
+
+An advance method to upload & merge *.csv or *.json files with images to <a href="https://notion.so/" target="_blank">Notion</a> database.
 
 ## Core Features
 
 ### Advantages over native import
 
 - Merge CSV or JSON with the existing database, using the first column as a key to combine existing rows
 - Choose column types manually instead of letting Notion detecting them automatically
@@ -54,15 +54,14 @@
   - [Column Types](#column-types)
   - [Mergin](#merging)
   - [Relation Columns](#relation-columns)
   - [Cover Image & Embedded Image](#cover-image--embedded-image)
   - [Icons](#icons)
   - [Mandatory Columns](#mandatory-columns)
 - [Examples](#examples)
-- [Known Issues](#known-issues)
 - [Credits](#credits)
 - [License](#license)
 - [Reporting Bugs](#reporting-bugs)
 
 ## Background
 
 Originally, we developed [csv2notion](https://github.com/vzhd1701/csv2notion) to address the lack of advanced importing support for `*.csv` files in [Notion](https://notion.so). We took inspiration from [Airtable](https://www.airtable.com)’s [CSV import extension](https://support.airtable.com/docs/csv-import-extension).
@@ -523,19 +522,14 @@
 ```
 
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_10.gif?raw=true"> </p>
 
 </p>
 </details>
 
-## Known Issues
-
-- Users would not be able to duplicate entries/records there where uploaded using **CSV2Notion Neo** in Notion.
-  - **Workaround:** Simply [duplicate](https://www.notion.so/help/duplicate-delete-and-restore-content) the database directly in Notion. You would be able to duplicate your entries/records in the duplicated database.
-  
 ## Utilised By
 
 ### [CommandPost](https://commandpost.io)
 
 <details><summary>CommandPost's Notion Toolbox</summary>
 <p>
```

#### html2text {}

```diff
@@ -1,112 +1,111 @@
-_[_A_p_p_ _i_c_o_n_]
-_**_**_**_**_**_**_ _CC_SS_VV_22_NN_oo_tt_ii_oo_nn_ _NN_ee_oo_ _**_**_**_**_**_**
-_[_P_y_P_I_]_[_P_y_t_h_o_n_]_[_r_e_l_e_a_s_e___g_i_t_h_u_b_]
-_A_n_ _a_d_v_a_n_c_e_ _m_e_t_h_o_d_ _t_o_ _u_p_l_o_a_d_ _&_ _m_e_r_g_e_ _*_._c_s_v_ _o_r_ _*_._j_s_o_n_ _f_i_l_e_s_ _w_i_t_h_ _i_m_a_g_e_s_ _t_o_ _N_o_t_i_o_n
-_d_a_t_a_b_a_s_e_.
-
-_#_#_ _C_o_r_e_ _F_e_a_t_u_r_e_s_ _#_#_#_ _A_d_v_a_n_t_a_g_e_s_ _o_v_e_r_ _n_a_t_i_v_e_ _i_m_p_o_r_t_ _-_ _M_e_r_g_e_ _C_S_V_ _o_r_ _J_S_O_N_ _w_i_t_h_ _t_h_e
-_e_x_i_s_t_i_n_g_ _d_a_t_a_b_a_s_e_,_ _u_s_i_n_g_ _t_h_e_ _f_i_r_s_t_ _c_o_l_u_m_n_ _a_s_ _a_ _k_e_y_ _t_o_ _c_o_m_b_i_n_e_ _e_x_i_s_t_i_n_g_ _r_o_w_s_ _-
-_C_h_o_o_s_e_ _c_o_l_u_m_n_ _t_y_p_e_s_ _m_a_n_u_a_l_l_y_ _i_n_s_t_e_a_d_ _o_f_ _l_e_t_t_i_n_g_ _N_o_t_i_o_n_ _d_e_t_e_c_t_i_n_g_ _t_h_e_m
-_a_u_t_o_m_a_t_i_c_a_l_l_y_ _-_ _L_i_n_k_ _o_r_ _c_r_e_a_t_e_ _n_e_w_ _e_n_t_r_i_e_s_ _i_n_ _r_e_l_a_t_i_o_n_ _c_o_l_u_m_n_s_ _b_a_s_e_d_ _o_n_ _t_h_e_i_r
-_v_a_l_u_e_s_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _-_ _E_a_s_i_l_y_ _u_p_l_o_a_d_ _f_i_l_e_s_ _i_n_t_o_ _t_h_e_ _d_e_s_i_g_n_a_t_e_d_ _"_F_i_l_e_s_ _&_ _M_e_d_i_a_"
-_c_o_l_u_m_n_ _-_ _A_s_s_i_g_n_ _a_ _i_c_o_n_ _f_o_r_ _e_a_c_h_ _r_o_w_ _f_o_r_ _q_u_i_c_k_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_ _-_ _S_e_t_ _a_ _c_o_v_e_r_ _o_r
-_e_m_b_e_d_ _a_n_ _i_m_a_g_e_ _f_o_r_ _e_a_c_h_ _r_o_w_ _t_o_ _e_n_h_a_n_c_e_ _v_i_s_u_a_l_ _r_e_p_r_e_s_e_n_t_a_t_i_o_n_ _-_ _U_p_l_o_a_d_ _i_m_a_g_e
-_f_i_l_e_s_ _f_o_r_ _c_o_v_e_r_s_ _o_r_ _i_c_o_n_s_ _-_ _A_p_p_l_y_ _v_a_l_i_d_a_t_i_o_n_ _o_p_t_i_o_n_s_ _f_o_r_ _i_n_p_u_t_ _d_a_t_a_ _t_o_ _e_n_s_u_r_e
-_a_c_c_u_r_a_c_y_ _#_#_#_ _D_i_s_a_d_v_a_n_t_a_g_e_s_ _o_v_e_r_ _n_a_t_i_v_e_ _i_m_p_o_r_t_ _-_ _I_m_p_o_r_t_i_n_g_ _e_a_c_h_ _r_o_w_ _s_e_p_a_r_a_t_e_l_y
-_m_i_g_h_t_ _l_e_a_d_ _t_o_ _s_l_o_w_e_r_ _s_p_e_e_d_ _-_ _T_o_ _a_d_d_r_e_s_s_ _t_h_i_s_,_ _u_t_i_l_i_s_e_ _m_u_l_t_i_t_h_r_e_a_d_e_d_ _u_p_l_o_a_d_ _#_#
-_T_a_b_l_e_ _o_f_ _c_o_n_t_e_n_t_s_ _-_ _[_B_a_c_k_g_r_o_u_n_d_]_(_#_b_a_c_k_g_r_o_u_n_d_)_ _-_ _[_I_n_s_t_a_l_l_a_t_i_o_n_]_(_#_i_n_s_t_a_l_l_a_t_i_o_n_)_ _-
-_[_P_r_e_-_c_o_m_p_i_l_e_d_ _B_i_n_a_r_y_ _(_R_e_c_o_m_m_e_n_d_e_d_)_]_(_#_p_r_e_-_c_o_m_p_i_l_e_d_-_b_i_n_a_r_y_-_r_e_c_o_m_m_e_n_d_e_d_)_ _-_ _[_F_r_o_m
-_S_o_u_r_c_e_]_(_#_f_r_o_m_-_s_o_u_r_c_e_)_ _-_ _[_G_u_i_d_e_]_(_#_g_u_i_d_e_)_ _-_ _[_m_a_c_O_S_ _R_e_l_e_a_s_e_]_(_#_m_a_c_o_s_-_r_e_l_e_a_s_e_)_ _-
-_[_P_r_e_r_e_q_u_i_s_i_t_e_]_(_#_p_r_e_r_e_q_u_i_s_i_t_e_)_ _-_ _[_U_p_l_o_a_d_ _S_p_e_e_d_]_(_#_u_p_l_o_a_d_-_s_p_e_e_d_)_ _-_ _[_D_u_p_l_i_c_a_t_e_ _C_S_V
-_C_o_l_u_m_n_s_]_(_#_d_u_p_l_i_c_a_t_e_-_c_s_v_-_c_o_l_u_m_n_s_)_ _-_ _[_M_i_s_s_i_n_g_ _C_o_l_u_m_n_s_]_(_#_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_)_ _-
-_[_C_o_l_u_m_n_ _T_y_p_e_s_]_(_#_c_o_l_u_m_n_-_t_y_p_e_s_)_ _-_ _[_M_e_r_g_i_n_]_(_#_m_e_r_g_i_n_g_)_ _-_ _[_R_e_l_a_t_i_o_n_ _C_o_l_u_m_n_s_]
-_(_#_r_e_l_a_t_i_o_n_-_c_o_l_u_m_n_s_)_ _-_ _[_C_o_v_e_r_ _I_m_a_g_e_ _&_ _E_m_b_e_d_d_e_d_ _I_m_a_g_e_]_(_#_c_o_v_e_r_-_i_m_a_g_e_-_-_e_m_b_e_d_d_e_d_-
-_i_m_a_g_e_)_ _-_ _[_I_c_o_n_s_]_(_#_i_c_o_n_s_)_ _-_ _[_M_a_n_d_a_t_o_r_y_ _C_o_l_u_m_n_s_]_(_#_m_a_n_d_a_t_o_r_y_-_c_o_l_u_m_n_s_)_ _-_ _[_E_x_a_m_p_l_e_s_]
-_(_#_e_x_a_m_p_l_e_s_)_ _-_ _[_K_n_o_w_n_ _I_s_s_u_e_s_]_(_#_k_n_o_w_n_-_i_s_s_u_e_s_)_ _-_ _[_C_r_e_d_i_t_s_]_(_#_c_r_e_d_i_t_s_)_ _-_ _[_L_i_c_e_n_s_e_]
-_(_#_l_i_c_e_n_s_e_)_ _-_ _[_R_e_p_o_r_t_i_n_g_ _B_u_g_s_]_(_#_r_e_p_o_r_t_i_n_g_-_b_u_g_s_)_ _#_#_ _B_a_c_k_g_r_o_u_n_d_ _O_r_i_g_i_n_a_l_l_y_,_ _w_e
-_d_e_v_e_l_o_p_e_d_ _[_c_s_v_2_n_o_t_i_o_n_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_v_z_h_d_1_7_0_1_/_c_s_v_2_n_o_t_i_o_n_)_ _t_o_ _a_d_d_r_e_s_s_ _t_h_e
-_l_a_c_k_ _o_f_ _a_d_v_a_n_c_e_d_ _i_m_p_o_r_t_i_n_g_ _s_u_p_p_o_r_t_ _f_o_r_ _`_*_._c_s_v_`_ _f_i_l_e_s_ _i_n_ _[_N_o_t_i_o_n_]_(_h_t_t_p_s_:_/_/
-_n_o_t_i_o_n_._s_o_)_._ _W_e_ _t_o_o_k_ _i_n_s_p_i_r_a_t_i_o_n_ _f_r_o_m_ _[_A_i_r_t_a_b_l_e_]_(_h_t_t_p_s_:_/_/_w_w_w_._a_i_r_t_a_b_l_e_._c_o_m_)_â___s
-_[_C_S_V_ _i_m_p_o_r_t_ _e_x_t_e_n_s_i_o_n_]_(_h_t_t_p_s_:_/_/_s_u_p_p_o_r_t_._a_i_r_t_a_b_l_e_._c_o_m_/_d_o_c_s_/_c_s_v_-_i_m_p_o_r_t_-_e_x_t_e_n_s_i_o_n_)_.
-_*_*_C_S_V_2_N_o_t_i_o_n_ _N_e_o_*_*_ _w_a_s_ _c_r_e_a_t_e_d_ _a_s_ _a_ _s_p_i_n_-_o_f_f_ _p_r_o_j_e_c_t_ _t_o_ _a_d_d_r_e_s_s_ _i_n_a_c_t_i_v_i_t_y_ _i_n
-_t_h_e_ _o_r_i_g_i_n_a_l_ _r_e_p_o_s_i_t_o_r_y_ _a_n_d_ _m_a_i_n_t_a_i_n_ _c_o_m_p_a_t_i_b_i_l_i_t_y_ _w_i_t_h_ _N_o_t_i_o_n_._ _A_s_ _N_o_t_i_o_n
-_c_h_a_n_g_e_s_ _o_r_ _u_p_d_a_t_e_s_ _i_t_s_ _b_a_c_k_e_n_d_ _A_P_I_ _p_e_r_i_o_d_i_c_a_l_l_y_,_ _w_e_ _a_i_m_ _t_o_ _f_i_x_,_ _u_p_d_a_t_e_ _a_n_d_ _a_d_d
-_n_e_w_ _f_e_a_t_u_r_e_s_ _t_o_ _t_h_e_ _t_o_o_l_ _i_n_ _a_ _t_i_m_e_l_y_ _m_a_n_n_e_r_._ _A_n_y_ _d_e_p_e_n_d_e_n_t_ _t_o_o_l_s_ _o_r_ _p_r_o_j_e_c_t
-_t_h_a_t_ _r_e_l_i_e_d_ _o_n_ _[_c_s_v_2_n_o_t_i_o_n_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_v_z_h_d_1_7_0_1_/_c_s_v_2_n_o_t_i_o_n_)_,_ _c_a_n_ _u_s_e
-_o_u_r_ _*_*_C_S_V_2_N_o_t_i_o_n_ _N_e_o_*_*_ _t_o_o_l_ _i_n_t_e_r_c_h_a_n_g_e_a_b_l_y_ _r_e_q_u_i_r_i_n_g_ _a_d_d_i_t_i_o_n_a_l_ _a_u_g_m_e_n_t_s_._ _#_#
-_I_n_s_t_a_l_l_a_t_i_o_n_ _#_#_#_ _P_r_e_-_c_o_m_p_i_l_e_d_ _B_i_n_a_r_y_ _(_R_e_c_o_m_m_e_n_d_e_d_)_ _D_o_w_n_l_o_a_d_ _t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e
-_o_f_ _t_h_e_ _l_a_t_e_s_t_ _b_i_n_a_r_y_ _r_e_l_e_a_s_e_ _[_h_e_r_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-
-_n_e_o_/_r_e_l_e_a_s_e_s_)_._ _#_#_#_ _W_i_t_h_ _[_H_o_m_e_b_r_e_w_]_(_h_t_t_p_s_:_/_/_b_r_e_w_._s_h_/_)_ _(_R_e_c_o_m_m_e_n_d_e_d_ _f_o_r_ _m_a_c_O_S_)
-_`_`_`_b_a_s_h_ _$_ _b_r_e_w_ _i_n_s_t_a_l_l_ _T_h_e_A_c_h_a_r_y_a_/_h_o_m_e_b_r_e_w_-_t_a_p_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_ _`_`_`_ _`_`_`_b_a_s_h_ _$
-_b_r_e_w_ _u_n_i_n_s_t_a_l_l_ _-_-_c_a_s_k_ _c_s_v_2_n_o_t_i_o_n_-_n_e_o_ _`_`_`_ _#_#_#_ _W_i_t_h_ _P_I_P_ _`_`_`_b_a_s_h_ _$_ _p_i_p_ _i_n_s_t_a_l_l_ _-_-
-_u_s_e_r_ _c_s_v_2_n_o_t_i_o_n___n_e_o_ _`_`_`_ _*_*_P_y_t_h_o_n_ _3_._7_ _o_r_ _l_a_t_e_r_ _r_e_q_u_i_r_e_d_._*_*_ _#_#_#_ _F_r_o_m_ _s_o_u_r_c_e_ _T_h_i_s
-_p_r_o_j_e_c_t_ _u_s_e_s_ _[_p_o_e_t_r_y_]_(_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_p_o_e_t_r_y_._o_r_g_/_)_ _f_o_r_ _d_e_p_e_n_d_e_n_c_y_ _m_a_n_a_g_e_m_e_n_t_ _a_n_d
-_p_a_c_k_a_g_i_n_g_._ _Y_o_u_ _w_i_l_l_ _h_a_v_e_ _t_o_ _i_n_s_t_a_l_l_ _i_t_ _f_i_r_s_t_._ _S_e_e_ _[_p_o_e_t_r_y_ _o_f_f_i_c_i_a_l
-_d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_p_o_e_t_r_y_._o_r_g_/_d_o_c_s_/_)_ _f_o_r_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _`_`_`_s_h_e_l_l_ _$
-_g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_._g_i_t_ _$_ _c_d_ _c_s_v_2_n_o_t_i_o_n___n_e_o_/
-_$_ _p_o_e_t_r_y_ _i_n_s_t_a_l_l_ _-_-_n_o_-_d_e_v_ _$_ _p_o_e_t_r_y_ _r_u_n_ _c_s_v_2_n_o_t_i_o_n___n_e_o_ _`_`_`_ _#_#_ _G_u_i_d_e_ _`_`_`_p_l_a_i_n_ _$
-_c_s_v_2_n_o_t_i_o_n___n_e_o_ _-_-_h_e_l_p_ _u_s_a_g_e_:_ _c_s_v_2_n_o_t_i_o_n___n_e_o_ _[_-_h_]_ _-_-_t_o_k_e_n_ _T_O_K_E_N_ _[_-_-_u_r_l_ _U_R_L_]
-_[_O_P_T_I_O_N_]_._._._ _F_I_L_E_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_ _U_p_l_o_a_d_ _&_ _M_e_r_g_e
-_C_S_V_ _o_r_ _J_S_O_N_ _D_a_t_a_ _w_i_t_h_ _I_m_a_g_e_s_ _t_o_ _N_o_t_i_o_n_ _D_a_t_a_b_a_s_e_ _p_o_s_i_t_i_o_n_a_l_ _a_r_g_u_m_e_n_t_s_:_ _F_I_L_E_ _C_S_V
-_o_r_ _J_S_O_N_ _f_i_l_e_ _t_o_ _u_p_l_o_a_d_ _g_e_n_e_r_a_l_ _o_p_t_i_o_n_s_:_ _-_-_w_o_r_k_s_p_a_c_e_ _a_c_t_i_v_e_ _N_o_t_i_o_n_ _w_o_r_k_s_p_a_c_e
-_n_a_m_e_ _-_-_t_o_k_e_n_ _N_o_t_i_o_n_ _t_o_k_e_n_,_ _s_t_o_r_e_d_ _i_n_ _t_o_k_e_n___v_2_ _c_o_o_k_i_e_ _f_o_r_ _n_o_t_i_o_n_._s_o_ _-_-_u_r_l_ _U_R_L
-_N_o_t_i_o_n_ _d_a_t_a_b_a_s_e_ _U_R_L_;_ _i_f_ _n_o_n_e_ _i_s_ _p_r_o_v_i_d_e_d_,_ _w_i_l_l_ _c_r_e_a_t_e_ _a_ _n_e_w_ _d_a_t_a_b_a_s_e_ _-_-_m_a_x_-
-_t_h_r_e_a_d_s_ _u_p_l_o_a_d_ _t_h_r_e_a_d_s_ _(_d_e_f_a_u_l_t_:_ _5_)_ _-_-_l_o_g_ _F_I_L_E_ _f_i_l_e_ _t_o_ _s_t_o_r_e_ _p_r_o_g_r_a_m_ _l_o_g_ _-_-
-_v_e_r_b_o_s_e_ _o_u_t_p_u_t_ _d_e_b_u_g_ _i_n_f_o_r_m_a_t_i_o_n_ _-_-_v_e_r_s_i_o_n_ _s_h_o_w_ _p_r_o_g_r_a_m_'_s_ _v_e_r_s_i_o_n_ _n_u_m_b_e_r_ _a_n_d
-_e_x_i_t_ _-_h_,_ _-_-_h_e_l_p_ _s_h_o_w_ _t_h_i_s_ _h_e_l_p_ _m_e_s_s_a_g_e_ _a_n_d_ _e_x_i_t_ _c_o_l_u_m_n_ _o_p_t_i_o_n_s_:_ _-_-_c_o_l_u_m_n_-_t_y_p_e_s
-_c_o_m_m_a_-_s_e_p_a_r_a_t_e_d_ _l_i_s_t_ _o_f_ _c_o_l_u_m_n_ _t_y_p_e_s_ _t_o_ _u_s_e_ _f_o_r_ _n_o_n_-_k_e_y_ _c_o_l_u_m_n_s_;_ _i_f_ _n_o_n_e_ _i_s
-_p_r_o_v_i_d_e_d_,_ _t_y_p_e_s_ _w_i_l_l_ _b_e_ _g_u_e_s_s_e_d_ _f_r_o_m_ _C_S_V_ _v_a_l_u_e_s_ _(_c_a_n_ _a_l_s_o_ _b_e_ _u_s_e_d_ _w_i_t_h_ _-_-_a_d_d_-
-_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_ _f_l_a_g_)_ _-_-_a_d_d_-_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_ _i_f_ _c_o_l_u_m_n_s_ _a_r_e_ _p_r_e_s_e_n_t_ _i_n_ _C_S_V_ _b_u_t
-_n_o_t_ _i_n_ _N_o_t_i_o_n_ _D_B_,_ _a_d_d_ _t_h_e_m_ _t_o_ _N_o_t_i_o_n_ _D_B_ _-_-_r_e_n_a_m_e_-_n_o_t_i_o_n_-_k_e_y_-_c_o_l_u_m_n_ _r_e_n_a_m_e_ _t_h_e
-_k_e_y_ _c_o_l_u_m_n_ _i_n_ _t_h_e_ _f_i_l_e_ _t_o_ _a_ _d_i_f_f_e_r_e_n_t_ _k_e_y_ _c_o_l_u_m_n_ _i_n_ _A_i_r_t_a_b_l_e_ _-_-_r_a_n_d_o_m_i_z_e_-
-_s_e_l_e_c_t_-_c_o_l_o_r_s_ _r_a_n_d_o_m_i_z_e_ _c_o_l_o_r_s_ _f_o_r_ _a_d_d_e_d_ _o_p_t_i_o_n_s_ _i_n_ _s_e_l_e_c_t_ _a_n_d_ _m_u_l_t_i_ _s_e_l_e_c_t
-_c_o_l_u_m_n_s_ _m_e_r_g_e_ _o_p_t_i_o_n_s_:_ _-_-_m_e_r_g_e_ _m_e_r_g_e_ _C_S_V_ _o_r_ _J_S_O_N_ _w_i_t_h_ _e_x_i_s_t_i_n_g_ _N_o_t_i_o_n_ _D_B_ _r_o_w_s_,
-_f_i_r_s_t_ _c_o_l_u_m_n_ _w_i_l_l_ _b_e_ _u_s_e_d_ _a_s_ _a_ _k_e_y_ _-_-_m_e_r_g_e_-_o_n_l_y_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t
-_s_h_o_u_l_d_ _b_e_ _u_p_d_a_t_e_d_ _o_n_ _m_e_r_g_e_;_ _w_h_e_n_ _p_r_o_v_i_d_e_d_,_ _o_t_h_e_r_ _c_o_l_u_m_n_s_ _w_i_l_l_ _b_e_ _i_g_n_o_r_e_d_ _(_u_s_e
-_m_u_l_t_i_p_l_e_ _t_i_m_e_s_ _f_o_r_ _m_u_l_t_i_p_l_e_ _c_o_l_u_m_n_s_)_ _-_-_m_e_r_g_e_-_s_k_i_p_-_n_e_w_ _s_k_i_p_ _n_e_w_ _r_o_w_s_ _i_n_ _C_S_V_ _o_r
-_J_S_O_N_ _t_h_a_t_ _a_r_e_ _n_o_t_ _a_l_r_e_a_d_y_ _i_n_ _N_o_t_i_o_n_ _D_B_ _d_u_r_i_n_g_ _m_e_r_g_e_ _r_e_l_a_t_i_o_n_s_ _o_p_t_i_o_n_s_:_ _-_-_a_d_d_-
-_m_i_s_s_i_n_g_-_r_e_l_a_t_i_o_n_s_ _a_d_d_ _m_i_s_s_i_n_g_ _e_n_t_r_i_e_s_ _i_n_t_o_ _l_i_n_k_e_d_ _N_o_t_i_o_n_ _D_B_ _p_a_g_e_ _c_o_v_e_r_ _o_p_t_i_o_n_s_:
-_-_-_i_m_a_g_e_-_c_o_l_u_m_n_ _C_O_L_U_M_N_ _o_n_e_ _o_r_ _m_o_r_e_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _p_o_i_n_t_s_ _t_o_ _U_R_L_ _o_r
-_i_m_a_g_e_ _f_i_l_e_ _t_h_a_t_ _w_i_l_l_ _b_e_ _e_m_b_e_d_d_e_d_ _f_o_r_ _t_h_a_t_ _r_o_w_ _-_-_i_m_a_g_e_-_c_o_l_u_m_n_-_k_e_e_p_ _k_e_e_p_ _i_m_a_g_e
-_C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _a_s_ _a_ _N_o_t_i_o_n_ _D_B_ _c_o_l_u_m_n_ _-_-_i_m_a_g_e_-_c_o_l_u_m_n_-_m_o_d_e_ _{_c_o_v_e_r_,_b_l_o_c_k_}
-_u_p_l_o_a_d_ _i_m_a_g_e_ _a_s_ _[_c_o_v_e_r_]_ _o_r_ _i_n_s_e_r_t_ _i_t_ _a_s_ _[_b_l_o_c_k_]_ _(_d_e_f_a_u_l_t_:_ _b_l_o_c_k_)_ _-_-_i_m_a_g_e_-
-_c_a_p_t_i_o_n_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _p_o_i_n_t_s_ _t_o_ _t_e_x_t_ _c_a_p_t_i_o_n_ _t_h_a_t_ _w_i_l_l_ _b_e
-_a_d_d_e_d_ _t_o_ _t_h_e_ _i_m_a_g_e_ _b_l_o_c_k_ _i_f_ _-_-_i_m_a_g_e_-_c_o_l_u_m_n_-_m_o_d_e_ _i_s_ _s_e_t_ _t_o_ _'_b_l_o_c_k_'_ _-_-_i_m_a_g_e_-
-_c_a_p_t_i_o_n_-_c_o_l_u_m_n_-_k_e_e_p_ _k_e_e_p_ _i_m_a_g_e_ _c_a_p_t_i_o_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _a_s_ _a_ _N_o_t_i_o_n_ _D_B_ _c_o_l_u_m_n
-_p_a_g_e_ _i_c_o_n_ _o_p_t_i_o_n_s_:_ _-_-_i_c_o_n_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _p_o_i_n_t_s_ _t_o_ _e_m_o_j_i_,_ _U_R_L
-_o_r_ _i_m_a_g_e_ _f_i_l_e_ _t_h_a_t_ _w_i_l_l_ _b_e_ _u_s_e_d_ _a_s_ _p_a_g_e_ _i_c_o_n_ _f_o_r_ _t_h_a_t_ _r_o_w_ _-_-_i_c_o_n_-_c_o_l_u_m_n_-_k_e_e_p
-_k_e_e_p_ _i_c_o_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _a_s_ _a_ _N_o_t_i_o_n_ _D_B_ _c_o_l_u_m_n_ _-_-_d_e_f_a_u_l_t_-_i_c_o_n_ _I_C_O_N_ _E_m_o_j_i_,
-_U_R_L_ _o_r_ _i_m_a_g_e_ _f_i_l_e_ _t_h_a_t_ _w_i_l_l_ _b_e_ _u_s_e_d_ _a_s_ _p_a_g_e_ _i_c_o_n_ _f_o_r_ _e_v_e_r_y_ _r_o_w_ _b_y_ _d_e_f_a_u_l_t
-_v_a_l_i_d_a_t_i_o_n_ _o_p_t_i_o_n_s_:_ _-_-_m_a_n_d_a_t_o_r_y_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _c_a_n_n_o_t_ _b_e_ _e_m_p_t_y
-_(_u_s_e_ _m_u_l_t_i_p_l_e_ _t_i_m_e_s_ _f_o_r_ _m_u_l_t_i_p_l_e_ _c_o_l_u_m_n_s_)_ _-_-_p_a_y_l_o_a_d_-_k_e_y_-_c_o_l_u_m_n_ _J_S_O_N_ _o_b_j_e_c_t_ _t_h_a_t
-_i_s_ _t_h_e_ _k_e_y_ _i_n_ _N_o_t_i_o_n_ _D_B_;_ _i_f_ _J_S_O_N_ _f_i_l_e_ _i_s_ _u_s_e_d_,_ _t_h_i_s_ _c_a_n_n_o_t_ _b_e_ _e_m_p_t_y_ _-_-_f_a_i_l_-_o_n_-
-_r_e_l_a_t_i_o_n_-_d_u_p_l_i_c_a_t_e_s_ _f_a_i_l_ _i_f_ _a_n_y_ _l_i_n_k_e_d_ _D_B_s_ _i_n_ _r_e_l_a_t_i_o_n_ _c_o_l_u_m_n_s_ _h_a_v_e_ _d_u_p_l_i_c_a_t_e
-_e_n_t_r_i_e_s_;_ _o_t_h_e_r_w_i_s_e_,_ _f_i_r_s_t_ _e_n_t_r_y_ _i_n_ _a_l_p_h_a_b_e_t_i_c_a_l_ _o_r_d_e_r_ _w_i_l_l_ _b_e_ _t_r_e_a_t_e_d_ _a_s_ _u_n_i_q_u_e
-_w_h_e_n_ _l_o_o_k_i_n_g_ _u_p_ _r_e_l_a_t_i_o_n_s_ _-_-_f_a_i_l_-_o_n_-_d_u_p_l_i_c_a_t_e_s_ _f_a_i_l_ _i_f_ _N_o_t_i_o_n_ _D_B_ _o_r_ _C_S_V_ _o_r_ _J_S_O_N
-_h_a_s_ _d_u_p_l_i_c_a_t_e_s_ _i_n_ _k_e_y_ _c_o_l_u_m_n_,_ _u_s_e_f_u_l_ _w_h_e_n_ _s_a_n_i_t_i_z_i_n_g_ _b_e_f_o_r_e_ _m_e_r_g_e_ _t_o_ _a_v_o_i_d
-_a_m_b_i_g_u_o_u_s_ _m_a_p_p_i_n_g_ _-_-_f_a_i_l_-_o_n_-_d_u_p_l_i_c_a_t_e_-_c_s_v_-_c_o_l_u_m_n_s_ _f_a_i_l_ _i_f_ _C_S_V_ _o_r_ _J_S_O_N_ _h_a_s
-_d_u_p_l_i_c_a_t_e_ _c_o_l_u_m_n_s_;_ _o_t_h_e_r_w_i_s_e_ _l_a_s_t_ _c_o_l_u_m_n_ _w_i_l_l_ _b_e_ _u_s_e_d_ _-_-_f_a_i_l_-_o_n_-_c_o_n_v_e_r_s_i_o_n_-
-_e_r_r_o_r_ _f_a_i_l_ _i_f_ _a_n_y_ _c_o_l_u_m_n_ _t_y_p_e_ _c_o_n_v_e_r_s_i_o_n_ _e_r_r_o_r_ _o_c_c_u_r_s_;_ _o_t_h_e_r_w_i_s_e_ _e_r_r_o_r_s_ _w_i_l_l_ _b_e
-_r_e_p_l_a_c_e_d_ _w_i_t_h_ _e_m_p_t_y_ _s_t_r_i_n_g_s_ _-_-_f_a_i_l_-_o_n_-_i_n_a_c_c_e_s_s_i_b_l_e_-_r_e_l_a_t_i_o_n_s_ _f_a_i_l_ _i_f_ _a_n_y
-_r_e_l_a_t_i_o_n_ _c_o_l_u_m_n_ _p_o_i_n_t_s_ _t_o_ _a_ _N_o_t_i_o_n_ _D_B_ _t_h_a_t_ _i_s_ _n_o_t_ _a_c_c_e_s_s_i_b_l_e_ _t_o_ _t_h_e_ _c_u_r_r_e_n_t
-_u_s_e_r_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _c_o_l_u_m_n_s_ _w_i_l_l_ _b_e_ _i_g_n_o_r_e_d_ _-_-_f_a_i_l_-_o_n_-_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_ _f_a_i_l_ _i_f
-_c_o_l_u_m_n_s_ _a_r_e_ _p_r_e_s_e_n_t_ _i_n_ _C_S_V_ _b_u_t_ _n_o_t_ _i_n_ _N_o_t_i_o_n_ _D_B_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _c_o_l_u_m_n_s_ _w_i_l_l
-_b_e_ _i_g_n_o_r_e_d_ _-_-_f_a_i_l_-_o_n_-_u_n_s_e_t_t_a_b_l_e_-_c_o_l_u_m_n_s_ _f_a_i_l_ _i_f_ _D_B_ _h_a_s_ _c_o_l_u_m_n_s_ _t_h_a_t_ _d_o_n_'_t
-_s_u_p_p_o_r_t_ _a_s_s_i_g_n_i_n_g_ _v_a_l_u_e_ _t_o_ _t_h_e_m_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _c_o_l_u_m_n_s_ _w_i_l_l_ _b_e_ _i_g_n_o_r_e_d
-_(_c_o_l_u_m_n_s_ _w_i_t_h_ _t_y_p_e_ _c_r_e_a_t_e_d___b_y_,_ _l_a_s_t___e_d_i_t_e_d___b_y_,_ _r_o_l_l_u_p_ _o_r_ _f_o_r_m_u_l_a_)_ _-_-_f_a_i_l_-_o_n_-
-_w_r_o_n_g_-_s_t_a_t_u_s_-_v_a_l_u_e_s_ _f_a_i_l_ _i_f_ _v_a_l_u_e_s_ _f_o_r_ _'_s_t_a_t_u_s_'_ _c_o_l_u_m_n_s_ _d_o_n_'_t_ _h_a_v_e_ _m_a_t_c_h_i_n_g
-_o_p_t_i_o_n_ _i_n_ _D_B_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _v_a_l_u_e_s_ _w_i_l_l_ _b_e_ _r_e_p_l_a_c_e_d_ _w_i_t_h_ _d_e_f_a_u_l_t_ _s_t_a_t_u_s_ _`_`_`
-_#_#_#_ _m_a_c_O_S_ _R_e_l_e_a_s_e_ _P_r_i_v_a_c_y_ _&_ _S_e_c_u_r_i_t_y
-_F_o_r_ _m_a_c_O_S_,_ _y_o_u_ _h_a_v_e_ _t_h_e_ _o_p_t_i_o_n_ _o_f_ _t_w_o_ _d_i_s_t_i_n_c_t_ _r_e_l_e_a_s_e_s_:_ _o_n_e_ _p_a_c_k_a_g_e_d_ _w_i_t_h_i_n_ _a
-_`_._z_i_p_`_ _a_r_c_h_i_v_e_ _a_n_d_ _t_h_e_ _o_t_h_e_r_ _i_n_ _a_ _`_._p_k_g_`_ _f_o_r_m_a_t_._ _N_a_v_i_g_a_t_e_ _t_o_ _t_h_e_ _`_P_r_i_v_a_c_y_ _&
-_S_e_c_u_r_i_t_y_`_ _s_e_t_t_i_n_g_s_ _a_n_d_ _s_e_t_ _y_o_u_r_ _p_r_e_f_e_r_e_n_c_e_ _t_o_ _`_A_p_p_ _S_t_o_r_e_ _a_n_d_ _i_d_e_n_t_i_f_i_e_d
-_d_e_v_e_l_o_p_e_r_s_`_.
-    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_/_b_l_o_b_/_m_a_s_t_e_r_/_a_s_s_e_t_s_/_m_a_c_O_S_-
-                             _p_r_i_v_a_c_y_._p_n_g_?_r_a_w_=_t_r_u_e_]
+  _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_/_b_l_o_b_/_m_a_s_t_e_r_/_a_s_s_e_t_s_/_C_S_V_2_N_o_t_i_o_n
+                            _N_e_o___I_c_o_n_._p_n_g_?_r_a_w_=_t_r_u_e_]
+                         _**_**_**_**_**_**_ _CC_SS_VV_22_NN_oo_tt_ii_oo_nn_ _NN_ee_oo_ _**_**_**_**_**_**
+                    _[_l_i_c_e_n_s_e_]_[_P_y_P_I_]_[_P_y_t_h_o_n_]_[_r_e_l_e_a_s_e___g_i_t_h_u_b_]
+An advance method to upload & merge *.csv or *.json files with images to _N_o_t_i_o_n
+database. ## Core Features ### Advantages over native import - Merge CSV or
+JSON with the existing database, using the first column as a key to combine
+existing rows - Choose column types manually instead of letting Notion
+detecting them automatically - Link or create new entries in relation columns
+based on their values automatically - Easily upload files into the designated
+"Files & Media" column - Assign a icon for each row for quick identification -
+Set a cover or embed an image for each row to enhance visual representation -
+Upload image files for covers or icons - Apply validation options for input
+data to ensure accuracy ### Disadvantages over native import - Importing each
+row separately might lead to slower speed - To address this, utilise
+multithreaded upload ## Table of contents - [Background](#background) -
+[Installation](#installation) - [Pre-compiled Binary (Recommended)](#pre-
+compiled-binary-recommended) - [From Source](#from-source) - [Guide](#guide) -
+[macOS Release](#macos-release) - [Prerequisite](#prerequisite) - [Upload
+Speed](#upload-speed) - [Duplicate CSV Columns](#duplicate-csv-columns) -
+[Missing Columns](#missing-columns) - [Column Types](#column-types) - [Mergin]
+(#merging) - [Relation Columns](#relation-columns) - [Cover Image & Embedded
+Image](#cover-image--embedded-image) - [Icons](#icons) - [Mandatory Columns]
+(#mandatory-columns) - [Examples](#examples) - [Credits](#credits) - [License]
+(#license) - [Reporting Bugs](#reporting-bugs) ## Background Originally, we
+developed [csv2notion](https://github.com/vzhd1701/csv2notion) to address the
+lack of advanced importing support for `*.csv` files in [Notion](https://
+notion.so). We took inspiration from [Airtable](https://www.airtable.com)âs
+[CSV import extension](https://support.airtable.com/docs/csv-import-extension).
+**CSV2Notion Neo** was created as a spin-off project to address inactivity in
+the original repository and maintain compatibility with Notion. As Notion
+changes or updates its backend API periodically, we aim to fix, update and add
+new features to the tool in a timely manner. Any dependent tools or project
+that relied on [csv2notion](https://github.com/vzhd1701/csv2notion), can use
+our **CSV2Notion Neo** tool interchangeably requiring additional augments. ##
+Installation ### Pre-compiled Binary (Recommended) Download the latest release
+of the latest binary release [here](https://github.com/TheAcharya/csv2notion-
+neo/releases). ### With [Homebrew](https://brew.sh/) (Recommended for macOS)
+```bash $ brew install TheAcharya/homebrew-tap/csv2notion-neo ``` ```bash $
+brew uninstall --cask csv2notion-neo ``` ### With PIP ```bash $ pip install --
+user csv2notion_neo ``` **Python 3.7 or later required.** ### From source This
+project uses [poetry](https://python-poetry.org/) for dependency management and
+packaging. You will have to install it first. See [poetry official
+documentation](https://python-poetry.org/docs/) for instructions. ```shell $
+git clone https://github.com/TheAcharya/csv2notion-neo.git $ cd csv2notion_neo/
+$ poetry install --no-dev $ poetry run csv2notion_neo ``` ## Guide ```plain $
+csv2notion_neo --help usage: csv2notion_neo [-h] --token TOKEN [--url URL]
+[OPTION]... FILE https://github.com/TheAcharya/csv2notion-neo Upload & Merge
+CSV or JSON Data with Images to Notion Database positional arguments: FILE CSV
+or JSON file to upload general options: --workspace active Notion workspace
+name --token Notion token, stored in token_v2 cookie for notion.so --url URL
+Notion database URL; if none is provided, will create a new database --max-
+threads upload threads (default: 5) --log FILE file to store program log --
+verbose output debug information --version show program's version number and
+exit -h, --help show this help message and exit column options: --column-types
+comma-separated list of column types to use for non-key columns; if none is
+provided, types will be guessed from CSV values (can also be used with --add-
+missing-columns flag) --add-missing-columns if columns are present in CSV but
+not in Notion DB, add them to Notion DB --rename-notion-key-column rename the
+key column in the file to a different key column in Airtable --randomize-
+select-colors randomize colors for added options in select and multi select
+columns merge options: --merge merge CSV or JSON with existing Notion DB rows,
+first column will be used as a key --merge-only-column CSV or JSON column that
+should be updated on merge; when provided, other columns will be ignored (use
+multiple times for multiple columns) --merge-skip-new skip new rows in CSV or
+JSON that are not already in Notion DB during merge relations options: --add-
+missing-relations add missing entries into linked Notion DB page cover options:
+--image-column COLUMN one or more CSV or JSON column that points to URL or
+image file that will be embedded for that row --image-column-keep keep image
+CSV or JSON column as a Notion DB column --image-column-mode {cover,block}
+upload image as [cover] or insert it as [block] (default: block) --image-
+caption-column CSV or JSON column that points to text caption that will be
+added to the image block if --image-column-mode is set to 'block' --image-
+caption-column-keep keep image caption CSV or JSON column as a Notion DB column
+page icon options: --icon-column CSV or JSON column that points to emoji, URL
+or image file that will be used as page icon for that row --icon-column-keep
+keep icon CSV or JSON column as a Notion DB column --default-icon ICON Emoji,
+URL or image file that will be used as page icon for every row by default
+validation options: --mandatory-column CSV or JSON column that cannot be empty
+(use multiple times for multiple columns) --payload-key-column JSON object that
+is the key in Notion DB; if JSON file is used, this cannot be empty --fail-on-
+relation-duplicates fail if any linked DBs in relation columns have duplicate
+entries; otherwise, first entry in alphabetical order will be treated as unique
+when looking up relations --fail-on-duplicates fail if Notion DB or CSV or JSON
+has duplicates in key column, useful when sanitizing before merge to avoid
+ambiguous mapping --fail-on-duplicate-csv-columns fail if CSV or JSON has
+duplicate columns; otherwise last column will be used --fail-on-conversion-
+error fail if any column type conversion error occurs; otherwise errors will be
+replaced with empty strings --fail-on-inaccessible-relations fail if any
+relation column points to a Notion DB that is not accessible to the current
+user; otherwise those columns will be ignored --fail-on-missing-columns fail if
+columns are present in CSV but not in Notion DB; otherwise those columns will
+be ignored --fail-on-unsettable-columns fail if DB has columns that don't
+support assigning value to them; otherwise those columns will be ignored
+(columns with type created_by, last_edited_by, rollup or formula) --fail-on-
+wrong-status-values fail if values for 'status' columns don't have matching
+option in DB; otherwise those values will be replaced with default status ```
+### macOS Release Privacy & Security
+For macOS, you have the option of two distinct releases: one packaged within a
+`.zip` archive and the other in a `.pkg` format. Navigate to the `Privacy &
+Security` settings and set your preference to `App Store and identified
+developers`.
+    [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/macOS-
+                             privacy.png?raw=true]
 Utilise the `CSV2Notion Neo.pkg` installer to install the command-line binary
 into your system. Upon completion, find the installed binary `csv2notion_neo`
 located within `/usr/local/bin`. To uninstall, you can utalise this terminal
 command. ```plain sudo rm /usr/local/bin/csv2notion_neo ```
     [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/macOS-
                             installer.png?raw=true]
 ### Prerequisite You must pass a single `*.csv` file for upload. The CSV file
@@ -309,20 +308,16 @@
 Importing JSON into Existing Database with a Different Key Column
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
 YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
 column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-
 Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_10.gif?raw=true]
-## Known Issues - Users would not be able to duplicate entries/records there
-where uploaded using **CSV2Notion Neo** in Notion. - **Workaround:** Simply
-[duplicate](https://www.notion.so/help/duplicate-delete-and-restore-content)
-the database directly in Notion. You would be able to duplicate your entries/
-records in the duplicated database. ## Utilised By ### [CommandPost](https://
-commandpost.io) CommandPost's Notion Toolbox
+## Utilised By ### [CommandPost](https://commandpost.io) CommandPost's Notion
+Toolbox
   [https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/
                          toolbox-notion.png?raw=true]
 ## Credits Original Idea and Workflow Architecture by [Vigneswaran Rajkumar]
 (https://twitter.com/IAmVigneswaran) Maintained by [Arjun Prakash](https://
 github.com/arjunprakash027) (1.0.0 ...) Original Work by [Vladilen Zhdanov]
 (https://github.com/vzhd1701) Icon Design by [Bor Jen Goh](https://
 www.artstation.com/borjengoh) ## License Licensed under the MIT license. See
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/cli.py` & `csv2notion_neo-1.2.5/csv2notion_neo/cli.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/cli_args.py` & `csv2notion_neo-1.2.5/csv2notion_neo/cli_args.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/cli_steps.py` & `csv2notion_neo-1.2.5/csv2notion_neo/cli_steps.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/local_data.py` & `csv2notion_neo-1.2.5/csv2notion_neo/local_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 CSVRowType = Dict[str, str]
 
 logger = logging.getLogger(__name__)
 
 
 def data_read(file_path: Path, fail_on_duplicate_columns: bool) -> List[CSVRowType]:
+    print("file extbn",file_path)
     suffix = Path(file_path).suffix
 
     if "csv" in suffix:
         try:
             with open(file_path, "r", encoding="utf-8-sig") as csv_file:
                 return _csv_read_rows(csv_file, fail_on_duplicate_columns)
         except FileNotFoundError as e:
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/block.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import mimetypes
 import os
 import random
 import requests
 import time
 import uuid
+from icecream import ic
 
 from cached_property import cached_property
 from copy import deepcopy
 
 from .logger import logger
 from .maps import property_map, field_map, mapper
 from .markdown import plaintext_to_notion, notion_to_plaintext
@@ -382,15 +383,15 @@
         list_args = {"id": self.id}
         if position in ["before", "after"]:
             list_args[position] = target_block.id
 
         with self._client.as_atomic_transaction():
 
             # First, remove the node, before we re-insert and re-activate it at the target location
-            self.remove()
+            #self.remove()
 
             if not self.is_alias:
                 # Set the parent_id of the moving block to the new parent, and mark it as active again
                 self._client.submit_transaction(
                     build_operation(
                         id=self.id,
                         path=[],
@@ -401,30 +402,33 @@
                         },
                         command="update",
                     )
                 )
             else:
                 self._alias_parent = new_parent_id
 
-            # Add the moving block's ID to the "content" list of the new parent
+            # Add the moving block's ID to the "content" list of the new paren
             self._client.submit_transaction(
                 build_operation(
                     id=new_parent_id,
                     path=["content"],
                     args=list_args,
                     command=list_command,
                 )
             )
 
-        # Parent block can be a collection, which will cause API error on refresh
-        refresh_blocks = [self, self.parent, target_block, target_block.parent]
-        refresh_blocks_ids = [b.id for b in refresh_blocks if isinstance(b, Block)]
-
         # update the local block cache to reflect the updates
-        self._client.refresh_records(block=refresh_blocks_ids)
+        self._client.refresh_records(
+            block=[
+                self.id,
+                self.get("parent_id"),
+                target_block.id,
+                target_block.get("parent_id"),
+            ]
+        )
 
 
 class DividerBlock(Block):
 
     _type = "divider"
 
 
@@ -630,18 +634,27 @@
 
     file_id = field_map(["file_ids", 0])
 
     def upload_file(self, path):
 
         mimetype = mimetypes.guess_type(path)[0] or "text/plain"
         filename = os.path.split(path)[-1]
-
+        
         data = self._client.post(
             "getUploadFileUrl",
-            {"bucket": "secure", "name": filename, "contentType": mimetype},
+            {
+                "bucket": "secure",
+                "name": filename,
+                "contentType": mimetype,
+                "record": {
+                    "id": self.id,
+                    "spaceId": self.space_info["spaceId"],
+                    "table": "block"
+                },
+            },
         ).json()
 
         with open(path, "rb") as f:
             response = requests.put(
                 data["signedPutUrl"], data=f, headers={"Content-type": mimetype}
             )
             response.raise_for_status()
@@ -707,26 +720,26 @@
 
 class CollectionViewBlock(MediaBlock):
 
     _type = "collection_view"
 
     @property
     def collection(self):
-        collection_id = self.get("format.collection_pointer.id")
+        collection_id = self.get("collection_id")
         if not collection_id:
             return None
         if not hasattr(self, "_collection"):
             self._collection = self._client.get_collection(collection_id)
         return self._collection
 
     @collection.setter
     def collection(self, val):
         if hasattr(self, "_collection"):
             del self._collection
-        self.set("format.collection_pointer.id", val.id)
+        self.set("collection_id", val.id)
 
     @property
     def views(self):
         if not hasattr(self, "_views"):
             self._views = CollectionViewBlockViews(parent=self)
         return self._views
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/client.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import hashlib
 import json
 import re
 import uuid
-import time
-from icecream import ic
 
 from requests import Session, HTTPError
 from requests.cookies import cookiejar_from_dict
 from urllib.parse import urljoin
+from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from getpass import getpass
-from ratelimit import limits, sleep_and_retry
 
 from .block import Block, BLOCK_TYPES
 from .collection import (
     Collection,
     CollectionView,
     CollectionRowBlock,
     COLLECTION_VIEW_TYPES,
@@ -24,31 +22,22 @@
 from .monitor import Monitor
 from .operations import operation_update_last_edited, build_operation
 from .settings import API_BASE_URL
 from .space import Space
 from .store import RecordStore
 from .user import User
 from .utils import extract_id, now
-from .utils_ssl import HTTPAdapterTLS
 
 from icecream import ic
 
-CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.7113.93 Safari/537.36"
-
-
-class HTTPRateLimitException(Exception):
-    pass
-
-
 def create_session(client_specified_retry=None):
     """
     retry on 502
     """
     session = Session()
-
     if client_specified_retry:
         retry = client_specified_retry
     else:
         retry = Retry(
             5,
             backoff_factor=0.3,
             status_forcelist=(502, 503, 504),
@@ -59,18 +48,16 @@
                 "TRACE",
                 "GET",
                 "PUT",
                 "OPTIONS",
                 "DELETE",
             ),
         )
-    adapter = HTTPAdapterTLS(max_retries=retry)
+    adapter = HTTPAdapter(max_retries=retry)
     session.mount("https://", adapter)
-    session.headers.update({"User-Agent": CHROME})
-    session.headers.update({"Content-Type": "application/json"})
     return session
 
 
 class NotionClient(object):
     """
     This is the entry point to using the API. Create an instance of this class, passing it the value of the
     "token_v2" cookie from a logged-in browser session on Notion.so. Most of the methods on here are primarily
@@ -80,61 +67,50 @@
     def __init__(
         self,
         token_v2=None,
         monitor=False,
         start_monitoring=False,
         enable_caching=False,
         cache_key=None,
-        cache_path=None,
         email=None,
         password=None,
         client_specified_retry=None,
-        workspace=None,
+        workspace=None
     ):
-        
         self.workspace = workspace
-
         self.session = create_session(client_specified_retry)
         if token_v2:
-            self.session.cookies.set(
-                "token_v2",
-                token_v2,
-                domain=".www.notion.so",
-                discard=False,
-                expires=int(time.time()) + 3600 * 24 * 365,
-                secure=True,
-            )
+            self.session.cookies = cookiejar_from_dict({"token_v2": token_v2})
         else:
             self._set_token(email=email, password=password)
 
         if enable_caching:
             cache_key = cache_key or hashlib.sha256(token_v2.encode()).hexdigest()
-            self._store = RecordStore(self, cache_key=cache_key, cache_path=cache_path)
+            self._store = RecordStore(self, cache_key=cache_key)
         else:
             self._store = RecordStore(self)
         if monitor:
             self._monitor = Monitor(self)
             if start_monitoring:
                 self.start_monitoring()
         else:
             self._monitor = None
 
         self._update_user_info()
 
     def start_monitoring(self):
         self._monitor.poll_async()
-
+    
     def _fetch_guest_space_data(self, records):
         """
         guest users have an empty `space` dict, so get the space_id from the `space_view` dict instead,
         and fetch the space data from the getPublicSpaceData endpoint.
 
         Note: This mutates the records dict
         """
-
         space_id = list(records["space_view"].values())[0]["value"]["space_id"]
 
         space_data = self.post(
             "getPublicSpaceData", {"type": "space-ids", "spaceIds": [space_id]}
         ).json()
 
         records["space"] = {
@@ -183,14 +159,15 @@
         response = self.post("getSpaces", {}).json()
         return {
             response[uid]["notion_user"][uid]["value"]["email"]: uid
             for uid in response.keys()
         }
 
     def set_user_by_uid(self, user_id):
+        self.session.headers.update({"x-notion-active-user-header": user_id})
         self._update_user_info()
 
     def set_user_by_email(self, email):
         email_uid_dict = self.get_email_uid()
         uid = email_uid_dict.get(email)
         if not uid:
             raise Exception(
@@ -251,15 +228,15 @@
         """
         Retrieve an instance of a subclass of CollectionView that maps to the appropriate type.
         The `url_or_id` argument can either be the URL for a database page, or the ID of a collection_view (in which case
         you must also pass the collection)
         """
         # if it's a URL for a database page, try extracting the collection and view IDs
         if url_or_id.startswith("http"):
-            match = re.search(r"([a-f0-9]{32})\?v=([a-f0-9]{32})", url_or_id)
+            match = re.search("([a-f0-9]{32})\?v=([a-f0-9]{32})", url_or_id)
             if not match:
                 raise Exception("Invalid collection view URL")
             block_id, view_id = match.groups()
             collection = self.get_block(
                 block_id, force_refresh=force_refresh
             ).collection
         else:
@@ -287,46 +264,33 @@
         """
         self._store.call_get_record_values(**kwargs)
 
     def refresh_collection_rows(self, collection_id):
         row_ids = [row.id for row in self.get_collection(collection_id).get_rows()]
         self._store.set_collection_rows(collection_id, row_ids)
 
-    @sleep_and_retry
-    @limits(calls=3000, period=60)
     def post(self, endpoint, data):
-        while True:
-            try:
-                return self._post(endpoint, data)
-            except HTTPRateLimitException:
-                time.sleep(1)
-    def _post(self, endpoint, data):
         """
         All API requests on Notion.so are done as POSTs (except the websocket communications).
         """
         url = urljoin(API_BASE_URL, endpoint)
-        
         response = self.session.post(url, json=data)
-
         if response.status_code == 400:
-            logger.error(
-                "Got 400 error attempting to POST to {}, with data: {}".format(
-                    endpoint, json.dumps(data, indent=2)
+            if endpoint != 'getRecordValues':
+                logger.error(
+                    "Got 400 error attempting to POST to {}, with data: {}".format(
+                        endpoint, json.dumps(data, indent=2)
+                    )
                 )
-            )
-            raise HTTPError(
-                response.json().get(
-                    "message", "There was an error (400) submitting the request."
+                raise HTTPError(
+                    response.json().get(
+                        "message", "There was an error (400) submitting the request."
+                    )
                 )
-            )
-        if response.status_code == 429:
-            raise HTTPRateLimitException
-
         response.raise_for_status()
-
         return response
 
     def submit_transaction(self, operations, update_last_edited=True):
 
         if not operations:
             return
 
@@ -343,19 +307,19 @@
             ]
 
         # if we're in a transaction, just add these operations to the list; otherwise, execute them right away
         if self.in_transaction():
             self._transaction_operations += operations
         else:
             data = {"operations": operations}
+            
             self.post("submitTransaction", data)
             self._store.run_local_operations(operations)
 
     def query_collection(self, *args, **kwargs):
-    
         return self._store.call_query_collection(*args, **kwargs)
 
     def as_atomic_transaction(self):
         """
         Returns a context manager that buffers up all calls to `submit_transaction` and sends them as one big transaction
         when the context manager exits.
         """
@@ -433,21 +397,20 @@
             "version": 1,
             "alive": True,
             "created_by_id": self.current_user.id,
             "created_by_table": "notion_user",
             "created_time": now(),
             "parent_id": parent.id,
             "parent_table": parent._table,
-            "space_id": self.current_space.id,
         }
 
         args.update(kwargs)
 
         with self.as_atomic_transaction():
-
+            
             # create the new record
             self.submit_transaction(
                 build_operation(
                     args=args, command="set", id=record_id, path=[], table=table
                 )
             )
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/collection.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,15 +734,15 @@
             for key, val in columns.items():
                 setattr(self.columns, key, val)
 
     def remove(self):
         # Mark the block as inactive
         self._client.submit_transaction(
             build_operation(
-                id=self.id, path=[], args={"alive": False}, command="update"
+                id=self.id, path=[], args={"alive": True}, command="update"
             )
         )
 
 
 class TemplateBlock(CollectionRowBlock):
     @property
     def is_template(self):
@@ -863,8 +863,8 @@
     if type(cls) == type and issubclass(cls, CollectionView) and hasattr(cls, "_type")
 }
 
 QUERY_RESULT_TYPES = {
     cls._type: cls
     for cls in locals().values()
     if type(cls) == type and issubclass(cls, QueryResult) and hasattr(cls, "_type")
-}
+}
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/maps.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             and "id" in signature(api_to_python).parameters
         ):
             kwargs["client"] = self._client
             kwargs["id"] = self.id
         return api_to_python(self.get(path), **kwargs)
 
     def fset(self, value):
+        from icecream import ic
         kwargs = {}
         if "client" in signature(python_to_api).parameters:
             kwargs["client"] = self._client
         self.set(path, python_to_api(value, **kwargs))
 
     return mapper(
         fget=fget,
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/markdown.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/markdown.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/monitor.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/monitor.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/operations.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .utils import now
+from icecream import ic
 
 
 def build_operation(id, path, args, command="set", table="block"):
     """
     Data updates sent to the submitTransaction endpoint consist of a sequence of "operations". This is a helper
     function that constructs one of these operations.
     """
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/records.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/records.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from copy import deepcopy
 
 from .logger import logger
 from .operations import build_operation
 from .utils import extract_id, get_by_path
-
+from icecream import ic
 
 class Record(object):
 
     # if a subclass has a list of ids that should be update when child records are removed, it should specify the key here
     child_list_key = None
 
     def __init__(self, client, id, *args, **kwargs):
@@ -108,17 +108,30 @@
             path, self._get_record_data(force_refresh=force_refresh), default=default
         )
 
     def set(self, path, value):
         """
         Set a specific `value` (under the specific `path`) on the record's data structure on the server.
         """
-        self._client.submit_transaction(
-            build_operation(id=self.id, path=path, args=value, table=self._table)
-        )
+        
+        command = 'set'
+        if 'cover_block' in path:
+            path = ['properties']
+            command = 'update'
+        elif 'icon' in path:
+            path = ['format','page_icon']
+        elif 'display_source' in path:
+            path = ['format']
+            value = {"display_source":value}
+            command = 'update'
+
+        if value:
+            self._client.submit_transaction(
+                build_operation(id=self.id, path=path, args=value, table=self._table,command=command)
+            )
 
     def __eq__(self, other):
         return self.id == other.id
 
     def __ne__(self, other):
         return self.id != other.id
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/smoke_test.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/smoke_test.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/space.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/space.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/store.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from dictdiffer import diff
 from inspect import signature
 from threading import Lock
 from pathlib import Path
 from tzlocal import get_localzone
 
 from .logger import logger
+from .settings import CACHE_DIR
 from .utils import extract_id
-
 from icecream import ic
 
 class MissingClass(object):
     def __bool__(self):
         return False
 
 
@@ -70,32 +70,25 @@
         elif isinstance(val, Callback):
             return self.callback_id == val.callback_id
         else:
             return False
 
 
 class RecordStore(object):
-    def __init__(self, client, cache_key=None, cache_path=None):
+    def __init__(self, client, cache_key=None):
         self._mutex = Lock()
         self._client = client
         self._cache_key = cache_key
-        self._cache_path = cache_path
         self._values = defaultdict(lambda: defaultdict(dict))
         self._role = defaultdict(lambda: defaultdict(str))
         self._collection_row_ids = {}
         self._callbacks = defaultdict(lambda: defaultdict(list))
         self._records_to_refresh = {}
         self._pages_to_refresh = []
-
         with self._mutex:
-            if self._cache_key:
-                if not self._cache_path or not isinstance(self._cache_path, Path):
-                    raise ValueError("You must provide directory for cache")
-                self._cache_path.mkdir(parents=True, exist_ok=True)
-
             self._load_cache()
 
     def _get(self, table, id):
         return self._values[table].get(id, Missing)
 
     def add_callback(self, record, callback, callback_id=None, extra_kwargs={}):
         assert callable(
@@ -116,15 +109,17 @@
         if callback_or_callback_id_prefix is None:
             return
         callbacks = self._callbacks[table][id]
         while callback_or_callback_id_prefix in callbacks:
             callbacks.remove(callback_or_callback_id_prefix)
 
     def _get_cache_path(self, attribute):
-        return self._cache_path / "{}{}.json".format(self._cache_key, attribute)
+        return str(
+            Path(CACHE_DIR).joinpath("{}{}.json".format(self._cache_key, attribute))
+        )
 
     def _load_cache(self, attributes=("_values", "_role", "_collection_row_ids")):
         if not self._cache_key:
             return
         for attr in attributes:
             try:
                 with open(self._get_cache_path(attr)) as f:
@@ -247,29 +242,32 @@
                     set(self._records_to_refresh.get(table, []) + ids)
                 )
                 continue
 
             requestlist += [{"table": table, "id": extract_id(id)} for id in ids]
 
         if requestlist:
-            logger.debug(
-                "Calling 'getRecordValues' endpoint for requests: {}".format(
-                    requestlist
-                )
-            )
-            results = self._client.post(
-                "getRecordValues", {"requests": requestlist}
-            ).json()["results"]
-            for request, result in zip(requestlist, results):
-                self._update_record(
-                    request["table"],
-                    request["id"],
-                    value=result.get("value"),
-                    role=result.get("role"),
+            try:
+                logger.debug(
+                    "Calling 'getRecordValues' endpoint for requests: {}".format(
+                        requestlist
+                    )
                 )
+                results = self._client.post(
+                    "getRecordValues", {"requests": requestlist}
+                ).json()["results"]
+                for request, result in zip(requestlist, results):
+                    self._update_record(
+                        request["table"],
+                        request["id"],
+                        value=result.get("value"),
+                        role=result.get("role"),
+                    )
+            except Exception as e:
+                pass
 
     def get_current_version(self, table, id):
         values = self._get(table, id)
         if values and "version" in values:
             return values["version"]
         else:
             return -1
@@ -277,17 +275,15 @@
     def call_load_page_chunk(self, page_id, limit=100):
 
         if self._client.in_transaction():
             self._pages_to_refresh.append(page_id)
             return
 
         data = {
-            "page": {
-                "id": page_id,
-            },
+            "pageId": page_id,
             "limit": limit,
             "cursor": {"stack": []},
             "chunkNumber": 0,
             "verticalColumns": False,
         }
 
         recordmap = self._client.post("loadPageChunk", data).json()["recordMap"]
@@ -309,14 +305,15 @@
         self,
         collection_id,
         collection_view_id,
         search="",
         type="table",
         aggregate=[],
         aggregations=[],
+        filter={},
         sort=[],
         calendar_by="",
         group_by="",
         limit=50
     ):
 
         assert not (
@@ -352,16 +349,14 @@
             },
         }
 
         response = self._client.post("queryCollection", data).json()
 
         self.store_recordmap(response["recordMap"])
 
-        from icecream import ic
-
         return response["result"]
 
     def handle_post_transaction_refreshing(self):
 
         for block_id in self._pages_to_refresh:
             self.call_load_page_chunk(block_id)
         self._pages_to_refresh = []
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/utils.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/utils.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion/utils_ssl.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion/utils_ssl.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_convert.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,47 +35,49 @@
 
     def convert_to_notion_rows(self, csv_data: LocalData) -> List[NotionUploadRow]:
         notion_rows = []
         # starting with 2nd row, because first is header
         self._current_row = 2
 
         for row in csv_data:
-     
             if self.rules.rename_notion_key_column:
                 new_id = self.rules.rename_notion_key_column[1]
                 old_id = self.rules.rename_notion_key_column[0]
                 row[new_id] = row[old_id]
                 del row[old_id]
 
             try:
                 notion_rows.append(self._convert_row(row))
             except NotionError as e:
                 raise NotionError(f"CSV [{self._current_row}]: {e}")
             self._current_row += 1
-    
+
         return notion_rows
 
     def _error(self, error: str) -> None:
         logger.error(f"CSV [{self._current_row}]: {error}")
 
         if self.rules.fail_on_conversion_error:
             raise NotionError("Error during conversion.")
 
     def _convert_row(self, row: CSVRowType) -> NotionUploadRow:
         properties = self._map_properties(row)
         columns = self._map_columns(row)
         
-
         return NotionUploadRow(columns=columns, properties=properties)
 
     def _map_properties(self, row: CSVRowType) -> Dict[str, Any]:
         properties = {}
 
         if self.rules.payload_key_column:
-            properties["payload_key_column"] = self.rules.payload_key_column
+            if self.rules.rename_notion_key_column:
+                new_id = self.rules.rename_notion_key_column[1]
+                properties["payload_key_column"] = new_id
+            else:
+                properties["payload_key_column"] = self.rules.payload_key_column
 
         if self.rules.image_column_mode == "block":
             properties["cover_block"] = self._map_image(row)
             properties["cover_block_caption"] = self._map_image_caption(row)
         else:
             properties["cover"] = self._map_image(row)
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_convert_map.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_convert_map.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_db.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,14 @@
 
     def add_row(
         self,
         properties: Optional[Dict[str, Any]] = None,
         columns: Optional[Dict[str, Any]] = None,
     ) -> CollectionRowBlockExtended:
         new_row = self.collection.add_row_block(properties=properties, columns=columns)
-
-
         key = columns.get(self.key_column) if columns else None
         if key:
             self.rows[key] = new_row
 
         return new_row
 
     def add_row_key(self, key: str) -> CollectionRowBlockExtended:
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_db_client.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_db_client.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_db_collection.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_db_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,17 +61,19 @@
         row_id = self._client.create_record("block", self, type="page")
         row = row_class(self._client, row_id)
 
         columns = {} if columns is None else columns
         properties = {} if properties is None else properties
 
         with self._client.as_atomic_transaction():
+        
             for key, val in properties.items():
                 setattr(row, key, val)
 
+        
             for key, val in columns.items():
                 setattr(row.columns, key, val)
 
             if update_views:
                 # make sure the new record is inserted at the end of each view
                 for view in self.parent.views:
                     if view is None or isinstance(view, CalendarView):
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_preparator.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_preparator.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_row.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
     @property
     def cover(self) -> Optional[str]:
         return super().cover  # type: ignore
 
     @cover.setter
     def cover(self, image: FileType) -> None:
+        
         new_image: Optional[FileType] = image if image else None
 
         if not self._is_meta_changed("cover_meta", new_image, self.cover):
             return
 
         if new_image is None:
             cover_meta = None
@@ -82,15 +83,14 @@
             cover_img = image.pop(0)
         else:
             cover_img = None
         if self._client.in_transaction():
             raise RuntimeError("Cannot set cover_block during atomic transaction")
 
         new_image: Optional[FileType] = cover_img if cover_img else None
-
      
         if not self._is_meta_changed("cover_block_meta", new_image, self.cover_block):
             return
 
         if new_image is None:
             cover_block_meta = None
         else:
@@ -115,15 +115,14 @@
             return
 
         attrs = {
             "display_source": image_url,
             "source": image_url,
         }
         
-
         file_id = get_file_id(image_url)
         if file_id:
             attrs["file_id"] = file_id
 
     @property
     def cover_block_caption(self) -> Optional[str]:
         return self.image_block.caption  # type: ignore
@@ -240,14 +239,16 @@
         self.set(f"properties.meta.file_columns.{column_id}", column_files_meta)
 
         return column_files_urls
 
     def _process_column_files(
         self, files: List[FileType]
     ) -> Tuple[List[Meta], NamedURLs]:
+        
+       
         column_files_meta: List[Meta] = []
         column_files_urls: NamedURLs = {}
 
         for filetype in files:
             file_url, file_meta = upload_filetype(self, filetype)
 
             column_files_urls[get_filetype_name(filetype)] = file_url
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_row_image_block.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_row_image_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from csv2notion_neo.notion_row_upload_file import get_file_id
 from icecream import ic
 
 
 class CoverImageBlock(ImageBlock):
     is_cover_block = field_map("properties.is_cover_block")
 
-
+    
     def update(self, **attrs: Any) -> None:
         with self._client.as_atomic_transaction():
             file_id = attrs.pop("file_id", None)
 
             for k, v in attrs.items():
                 setattr(self, k, v)
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_row_upload_file.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_row_upload_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,46 +23,53 @@
         url = filetype
         meta = {"type": "url", "url": filetype}
 
     return url, meta
 
 
 def upload_file(block: Block, file_path: Path) -> Tuple[str, Meta]:
+    
     file_url = _upload_file(block, file_path)
 
     file_id = get_file_id(file_url)
     if file_id is None:
         raise NotionError(f"Could not upload file {file_path}")
-
+    
     return file_url, {
-        "type": "file",
-        "file_id": file_id,
-        "sha256": get_file_sha256(file_path),
+        "source": [
+            [
+                file_url
+            ]
+        ]
     }
+    # return file_url, {
+    #     "type": "file",
+    #     "file_id": file_id,
+    #     "sha256": get_file_sha256(file_path),
+    # }
 
 
 def _upload_file(block: Block, file_path: Path) -> str:
     file_mime = mimetypes.guess_type(file_path.name)[0] or "application/octet-stream"
 
-
     post_data = {
         "bucket": "secure",
         "name": file_path.name,
         "contentType": file_mime,
         "record": {
             "table": "block",
             "id": block.id,
             "spaceId": block.space_info["spaceId"],
         },
     }
 
 
     upload_data = block._client.post("getUploadFileUrl", post_data).json()
 
-
+    
     with open(file_path, "rb") as f:
         requests.put(
             upload_data["signedPutUrl"],
             data=f,
             headers={"Content-type": file_mime},
         ).raise_for_status()
 
@@ -71,15 +78,14 @@
 
 def get_file_id(image_url: str) -> Optional[str]:
     # aws_host/space_id/file_id/filename
     aws_re = r"^https://(.*?\.amazonaws\.com)/([a-f0-9\-]+)/([a-f0-9\-]+)/(.*?)$"
 
     aws_match = re.search(aws_re, image_url)
 
-
     if aws_match:
         return aws_match.group(3)
 
     return None
 
 
 def is_meta_different(
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_type_guess.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_type_guess.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/notion_uploader.py` & `csv2notion_neo-1.2.5/csv2notion_neo/notion_uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 
 @dataclass
 class NotionUploadRow(object):
     columns: Dict[str, Any]
     properties: Dict[str, Any]
 
     def key(self) -> str:
-        
         if "payload_key_column" in self.properties:
             if self.properties["payload_key_column"]:
                 return str(self.columns[self.properties["payload_key_column"]])
         return str(list(self.columns.values())[0])
 
 
 class NotionRowUploader(object):
     def __init__(self, db: NotionDB):
         self.db = db
 
     def upload_row(self, row: NotionUploadRow, is_merge: bool) -> None:
+
         post_properties = _extract_post_properties(row.properties)
 
         db_row = self._get_db_row(row, is_merge)
 
         # these need to be updated after
         # because they can't be updated in atomic transaction
         for prop, prop_val in post_properties.items():
             setattr(db_row, prop, prop_val)
 
     def _get_db_row(
         self, row: NotionUploadRow, is_merge: bool
     ) -> CollectionRowBlockExtended:
       
         existing_row = self.db.rows.get(row.key()) if is_merge else None
+
         if is_merge and existing_row:       
             cur_row = existing_row
             cur_row.update(properties=row.properties, columns=row.columns)
         else:
             cur_row = self.db.add_row(properties=row.properties, columns=row.columns)
         return cur_row
```

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/utils_db.py` & `csv2notion_neo-1.2.5/csv2notion_neo/utils_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/utils_rand_id.py` & `csv2notion_neo-1.2.5/csv2notion_neo/utils_rand_id.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/utils_static.py` & `csv2notion_neo-1.2.5/csv2notion_neo/utils_static.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/csv2notion_neo/utils_threading.py` & `csv2notion_neo-1.2.5/csv2notion_neo/utils_threading.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.4/pyproject.toml` & `csv2notion_neo-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "csv2notion_neo"
-version = "1.2.4"
+version = "1.2.5"
 description = "Upload & Merge CSV Data with Images to Notion Database"
 authors = ["vzhd1701 <vzhd1701@gmail.com>", "Arjun <arjunprakash027@gmail.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md"]
 license = "MIT"
 homepage = "https://github.com/TheAcharya/csv2notion-neo"
 repository = "https://github.com/TheAcharya/csv2notion-neo"
```

### Comparing `csv2notion_neo-1.2.4/PKG-INFO` & `csv2notion_neo-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2notion-neo
-Version: 1.2.4
+Version: 1.2.5
 Summary: Upload & Merge CSV Data with Images to Notion Database
 Home-page: https://github.com/TheAcharya/csv2notion-neo
 License: MIT
 Keywords: csv,notion,import,merge
 Author: vzhd1701
 Author-email: vzhd1701@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -41,36 +41,36 @@
 Requires-Dist: types-requests (>=2.27.27,<3.0.0)
 Requires-Dist: tzlocal (>=5.2,<6.0)
 Project-URL: Changelog, https://github.com/TheAcharya/csv2notion-neo/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/TheAcharya/csv2notion-neo/blob/master/README.md
 Project-URL: Repository, https://github.com/TheAcharya/csv2notion-neo
 Description-Content-Type: text/markdown
 
-<a href="https://github.com/TheAcharya/csv2notion-neo"><img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/CSV2Notion Neo_Icon.png?raw=true" width="200" alt="App icon" align="left"/>
+<p align="center">
+  <a href="https://github.com/TheAcharya/csv2notion-neo"><img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/CSV2Notion Neo_Icon.png?raw=true" height="200">
+  <h1 align="center">CSV2Notion Neo</h1>
+</p>
+
 
-<div>
-<h1>CSV2Notion Neo</h1>
-<!-- PyPI -->
-<a href="https://pypi.python.org/pypi/csv2notion-neo">
-<img src="https://img.shields.io/pypi/v/csv2notion-neo?label=version" alt="PyPI"/>
-</a>
-<!-- Python -->
-<a href="https://pypi.org/project/csv2notion-neo/">
-<img src="https://img.shields.io/pypi/pyversions/csv2notion-neo.svg" alt="Python"/>
-</a>
-<!-- release_github -->
-<a href="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml">
-<img src="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml/badge.svg" alt="release_github"/>
-</a>
-<p>
-<p>An advance method to upload & merge *.csv or *.json files with images to <a href="https://notion.so/" target="_blank">Notion</a> database.
-
-<br>
-<br>
-</div>
+<p align="center">
+  <a href="https://github.com/TheAcharya/csv2notion-neo/blob/main/LICENSE">
+    <img src="http://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat" alt="license"/>
+  </a>
+  <a href="https://pypi.python.org/pypi/csv2notion-neo">
+    <img src="https://img.shields.io/pypi/v/csv2notion-neo?label=version" alt="PyPI"/>
+  </a>
+  <a href="https://pypi.org/project/csv2notion-neo/">
+    <img src="https://img.shields.io/pypi/pyversions/csv2notion-neo.svg" alt="Python"/>
+  </a>
+  <a href="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml">
+    <img src="https://github.com/TheAcharya/csv2notion-neo/actions/workflows/release_github.yml/badge.svg" alt="release_github"/>
+  </a>
+</p>
+
+An advance method to upload & merge *.csv or *.json files with images to <a href="https://notion.so/" target="_blank">Notion</a> database.
 
 ## Core Features
 
 ### Advantages over native import
 
 - Merge CSV or JSON with the existing database, using the first column as a key to combine existing rows
 - Choose column types manually instead of letting Notion detecting them automatically
@@ -101,15 +101,14 @@
   - [Column Types](#column-types)
   - [Mergin](#merging)
   - [Relation Columns](#relation-columns)
   - [Cover Image & Embedded Image](#cover-image--embedded-image)
   - [Icons](#icons)
   - [Mandatory Columns](#mandatory-columns)
 - [Examples](#examples)
-- [Known Issues](#known-issues)
 - [Credits](#credits)
 - [License](#license)
 - [Reporting Bugs](#reporting-bugs)
 
 ## Background
 
 Originally, we developed [csv2notion](https://github.com/vzhd1701/csv2notion) to address the lack of advanced importing support for `*.csv` files in [Notion](https://notion.so). We took inspiration from [Airtable](https://www.airtable.com)’s [CSV import extension](https://support.airtable.com/docs/csv-import-extension).
@@ -570,19 +569,14 @@
 ```
 
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_10.gif?raw=true"> </p>
 
 </p>
 </details>
 
-## Known Issues
-
-- Users would not be able to duplicate entries/records there where uploaded using **CSV2Notion Neo** in Notion.
-  - **Workaround:** Simply [duplicate](https://www.notion.so/help/duplicate-delete-and-restore-content) the database directly in Notion. You would be able to duplicate your entries/records in the duplicated database.
-  
 ## Utilised By
 
 ### [CommandPost](https://commandpost.io)
 
 <details><summary>CommandPost's Notion Toolbox</summary>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csv2notion-neo Version: 1.2.4 Summary: Upload &
+Metadata-Version: 2.1 Name: csv2notion-neo Version: 1.2.5 Summary: Upload &
 Merge CSV Data with Images to Notion Database Home-page: https://github.com/
 TheAcharya/csv2notion-neo License: MIT Keywords: csv,notion,import,merge
 Author: vzhd1701 Author-email: vzhd1701@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft Classifier:
@@ -20,119 +20,118 @@
 (>=2.27.1,<2.29) Requires-Dist: tqdm (>=4.64.0,<5.0.0) Requires-Dist: types-
 emoji (>=1.2.8,<2.0.0) Requires-Dist: types-python-dateutil (>=2.8.16,<3.0.0)
 Requires-Dist: types-requests (>=2.27.27,<3.0.0) Requires-Dist: tzlocal
 (>=5.2,<6.0) Project-URL: Changelog, https://github.com/TheAcharya/csv2notion-
 neo/blob/master/CHANGELOG.md Project-URL: Documentation, https://github.com/
 TheAcharya/csv2notion-neo/blob/master/README.md Project-URL: Repository, https:
 //github.com/TheAcharya/csv2notion-neo Description-Content-Type: text/markdown
-_[_A_p_p_ _i_c_o_n_]
-_**_**_**_**_**_**_ _CC_SS_VV_22_NN_oo_tt_ii_oo_nn_ _NN_ee_oo_ _**_**_**_**_**_**
-_[_P_y_P_I_]_[_P_y_t_h_o_n_]_[_r_e_l_e_a_s_e___g_i_t_h_u_b_]
-_A_n_ _a_d_v_a_n_c_e_ _m_e_t_h_o_d_ _t_o_ _u_p_l_o_a_d_ _&_ _m_e_r_g_e_ _*_._c_s_v_ _o_r_ _*_._j_s_o_n_ _f_i_l_e_s_ _w_i_t_h_ _i_m_a_g_e_s_ _t_o_ _N_o_t_i_o_n
-_d_a_t_a_b_a_s_e_.
-
-_#_#_ _C_o_r_e_ _F_e_a_t_u_r_e_s_ _#_#_#_ _A_d_v_a_n_t_a_g_e_s_ _o_v_e_r_ _n_a_t_i_v_e_ _i_m_p_o_r_t_ _-_ _M_e_r_g_e_ _C_S_V_ _o_r_ _J_S_O_N_ _w_i_t_h_ _t_h_e
-_e_x_i_s_t_i_n_g_ _d_a_t_a_b_a_s_e_,_ _u_s_i_n_g_ _t_h_e_ _f_i_r_s_t_ _c_o_l_u_m_n_ _a_s_ _a_ _k_e_y_ _t_o_ _c_o_m_b_i_n_e_ _e_x_i_s_t_i_n_g_ _r_o_w_s_ _-
-_C_h_o_o_s_e_ _c_o_l_u_m_n_ _t_y_p_e_s_ _m_a_n_u_a_l_l_y_ _i_n_s_t_e_a_d_ _o_f_ _l_e_t_t_i_n_g_ _N_o_t_i_o_n_ _d_e_t_e_c_t_i_n_g_ _t_h_e_m
-_a_u_t_o_m_a_t_i_c_a_l_l_y_ _-_ _L_i_n_k_ _o_r_ _c_r_e_a_t_e_ _n_e_w_ _e_n_t_r_i_e_s_ _i_n_ _r_e_l_a_t_i_o_n_ _c_o_l_u_m_n_s_ _b_a_s_e_d_ _o_n_ _t_h_e_i_r
-_v_a_l_u_e_s_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _-_ _E_a_s_i_l_y_ _u_p_l_o_a_d_ _f_i_l_e_s_ _i_n_t_o_ _t_h_e_ _d_e_s_i_g_n_a_t_e_d_ _"_F_i_l_e_s_ _&_ _M_e_d_i_a_"
-_c_o_l_u_m_n_ _-_ _A_s_s_i_g_n_ _a_ _i_c_o_n_ _f_o_r_ _e_a_c_h_ _r_o_w_ _f_o_r_ _q_u_i_c_k_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_ _-_ _S_e_t_ _a_ _c_o_v_e_r_ _o_r
-_e_m_b_e_d_ _a_n_ _i_m_a_g_e_ _f_o_r_ _e_a_c_h_ _r_o_w_ _t_o_ _e_n_h_a_n_c_e_ _v_i_s_u_a_l_ _r_e_p_r_e_s_e_n_t_a_t_i_o_n_ _-_ _U_p_l_o_a_d_ _i_m_a_g_e
-_f_i_l_e_s_ _f_o_r_ _c_o_v_e_r_s_ _o_r_ _i_c_o_n_s_ _-_ _A_p_p_l_y_ _v_a_l_i_d_a_t_i_o_n_ _o_p_t_i_o_n_s_ _f_o_r_ _i_n_p_u_t_ _d_a_t_a_ _t_o_ _e_n_s_u_r_e
-_a_c_c_u_r_a_c_y_ _#_#_#_ _D_i_s_a_d_v_a_n_t_a_g_e_s_ _o_v_e_r_ _n_a_t_i_v_e_ _i_m_p_o_r_t_ _-_ _I_m_p_o_r_t_i_n_g_ _e_a_c_h_ _r_o_w_ _s_e_p_a_r_a_t_e_l_y
-_m_i_g_h_t_ _l_e_a_d_ _t_o_ _s_l_o_w_e_r_ _s_p_e_e_d_ _-_ _T_o_ _a_d_d_r_e_s_s_ _t_h_i_s_,_ _u_t_i_l_i_s_e_ _m_u_l_t_i_t_h_r_e_a_d_e_d_ _u_p_l_o_a_d_ _#_#
-_T_a_b_l_e_ _o_f_ _c_o_n_t_e_n_t_s_ _-_ _[_B_a_c_k_g_r_o_u_n_d_]_(_#_b_a_c_k_g_r_o_u_n_d_)_ _-_ _[_I_n_s_t_a_l_l_a_t_i_o_n_]_(_#_i_n_s_t_a_l_l_a_t_i_o_n_)_ _-
-_[_P_r_e_-_c_o_m_p_i_l_e_d_ _B_i_n_a_r_y_ _(_R_e_c_o_m_m_e_n_d_e_d_)_]_(_#_p_r_e_-_c_o_m_p_i_l_e_d_-_b_i_n_a_r_y_-_r_e_c_o_m_m_e_n_d_e_d_)_ _-_ _[_F_r_o_m
-_S_o_u_r_c_e_]_(_#_f_r_o_m_-_s_o_u_r_c_e_)_ _-_ _[_G_u_i_d_e_]_(_#_g_u_i_d_e_)_ _-_ _[_m_a_c_O_S_ _R_e_l_e_a_s_e_]_(_#_m_a_c_o_s_-_r_e_l_e_a_s_e_)_ _-
-_[_P_r_e_r_e_q_u_i_s_i_t_e_]_(_#_p_r_e_r_e_q_u_i_s_i_t_e_)_ _-_ _[_U_p_l_o_a_d_ _S_p_e_e_d_]_(_#_u_p_l_o_a_d_-_s_p_e_e_d_)_ _-_ _[_D_u_p_l_i_c_a_t_e_ _C_S_V
-_C_o_l_u_m_n_s_]_(_#_d_u_p_l_i_c_a_t_e_-_c_s_v_-_c_o_l_u_m_n_s_)_ _-_ _[_M_i_s_s_i_n_g_ _C_o_l_u_m_n_s_]_(_#_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_)_ _-
-_[_C_o_l_u_m_n_ _T_y_p_e_s_]_(_#_c_o_l_u_m_n_-_t_y_p_e_s_)_ _-_ _[_M_e_r_g_i_n_]_(_#_m_e_r_g_i_n_g_)_ _-_ _[_R_e_l_a_t_i_o_n_ _C_o_l_u_m_n_s_]
-_(_#_r_e_l_a_t_i_o_n_-_c_o_l_u_m_n_s_)_ _-_ _[_C_o_v_e_r_ _I_m_a_g_e_ _&_ _E_m_b_e_d_d_e_d_ _I_m_a_g_e_]_(_#_c_o_v_e_r_-_i_m_a_g_e_-_-_e_m_b_e_d_d_e_d_-
-_i_m_a_g_e_)_ _-_ _[_I_c_o_n_s_]_(_#_i_c_o_n_s_)_ _-_ _[_M_a_n_d_a_t_o_r_y_ _C_o_l_u_m_n_s_]_(_#_m_a_n_d_a_t_o_r_y_-_c_o_l_u_m_n_s_)_ _-_ _[_E_x_a_m_p_l_e_s_]
-_(_#_e_x_a_m_p_l_e_s_)_ _-_ _[_K_n_o_w_n_ _I_s_s_u_e_s_]_(_#_k_n_o_w_n_-_i_s_s_u_e_s_)_ _-_ _[_C_r_e_d_i_t_s_]_(_#_c_r_e_d_i_t_s_)_ _-_ _[_L_i_c_e_n_s_e_]
-_(_#_l_i_c_e_n_s_e_)_ _-_ _[_R_e_p_o_r_t_i_n_g_ _B_u_g_s_]_(_#_r_e_p_o_r_t_i_n_g_-_b_u_g_s_)_ _#_#_ _B_a_c_k_g_r_o_u_n_d_ _O_r_i_g_i_n_a_l_l_y_,_ _w_e
-_d_e_v_e_l_o_p_e_d_ _[_c_s_v_2_n_o_t_i_o_n_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_v_z_h_d_1_7_0_1_/_c_s_v_2_n_o_t_i_o_n_)_ _t_o_ _a_d_d_r_e_s_s_ _t_h_e
-_l_a_c_k_ _o_f_ _a_d_v_a_n_c_e_d_ _i_m_p_o_r_t_i_n_g_ _s_u_p_p_o_r_t_ _f_o_r_ _`_*_._c_s_v_`_ _f_i_l_e_s_ _i_n_ _[_N_o_t_i_o_n_]_(_h_t_t_p_s_:_/_/
-_n_o_t_i_o_n_._s_o_)_._ _W_e_ _t_o_o_k_ _i_n_s_p_i_r_a_t_i_o_n_ _f_r_o_m_ _[_A_i_r_t_a_b_l_e_]_(_h_t_t_p_s_:_/_/_w_w_w_._a_i_r_t_a_b_l_e_._c_o_m_)_â___s
-_[_C_S_V_ _i_m_p_o_r_t_ _e_x_t_e_n_s_i_o_n_]_(_h_t_t_p_s_:_/_/_s_u_p_p_o_r_t_._a_i_r_t_a_b_l_e_._c_o_m_/_d_o_c_s_/_c_s_v_-_i_m_p_o_r_t_-_e_x_t_e_n_s_i_o_n_)_.
-_*_*_C_S_V_2_N_o_t_i_o_n_ _N_e_o_*_*_ _w_a_s_ _c_r_e_a_t_e_d_ _a_s_ _a_ _s_p_i_n_-_o_f_f_ _p_r_o_j_e_c_t_ _t_o_ _a_d_d_r_e_s_s_ _i_n_a_c_t_i_v_i_t_y_ _i_n
-_t_h_e_ _o_r_i_g_i_n_a_l_ _r_e_p_o_s_i_t_o_r_y_ _a_n_d_ _m_a_i_n_t_a_i_n_ _c_o_m_p_a_t_i_b_i_l_i_t_y_ _w_i_t_h_ _N_o_t_i_o_n_._ _A_s_ _N_o_t_i_o_n
-_c_h_a_n_g_e_s_ _o_r_ _u_p_d_a_t_e_s_ _i_t_s_ _b_a_c_k_e_n_d_ _A_P_I_ _p_e_r_i_o_d_i_c_a_l_l_y_,_ _w_e_ _a_i_m_ _t_o_ _f_i_x_,_ _u_p_d_a_t_e_ _a_n_d_ _a_d_d
-_n_e_w_ _f_e_a_t_u_r_e_s_ _t_o_ _t_h_e_ _t_o_o_l_ _i_n_ _a_ _t_i_m_e_l_y_ _m_a_n_n_e_r_._ _A_n_y_ _d_e_p_e_n_d_e_n_t_ _t_o_o_l_s_ _o_r_ _p_r_o_j_e_c_t
-_t_h_a_t_ _r_e_l_i_e_d_ _o_n_ _[_c_s_v_2_n_o_t_i_o_n_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_v_z_h_d_1_7_0_1_/_c_s_v_2_n_o_t_i_o_n_)_,_ _c_a_n_ _u_s_e
-_o_u_r_ _*_*_C_S_V_2_N_o_t_i_o_n_ _N_e_o_*_*_ _t_o_o_l_ _i_n_t_e_r_c_h_a_n_g_e_a_b_l_y_ _r_e_q_u_i_r_i_n_g_ _a_d_d_i_t_i_o_n_a_l_ _a_u_g_m_e_n_t_s_._ _#_#
-_I_n_s_t_a_l_l_a_t_i_o_n_ _#_#_#_ _P_r_e_-_c_o_m_p_i_l_e_d_ _B_i_n_a_r_y_ _(_R_e_c_o_m_m_e_n_d_e_d_)_ _D_o_w_n_l_o_a_d_ _t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e
-_o_f_ _t_h_e_ _l_a_t_e_s_t_ _b_i_n_a_r_y_ _r_e_l_e_a_s_e_ _[_h_e_r_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-
-_n_e_o_/_r_e_l_e_a_s_e_s_)_._ _#_#_#_ _W_i_t_h_ _[_H_o_m_e_b_r_e_w_]_(_h_t_t_p_s_:_/_/_b_r_e_w_._s_h_/_)_ _(_R_e_c_o_m_m_e_n_d_e_d_ _f_o_r_ _m_a_c_O_S_)
-_`_`_`_b_a_s_h_ _$_ _b_r_e_w_ _i_n_s_t_a_l_l_ _T_h_e_A_c_h_a_r_y_a_/_h_o_m_e_b_r_e_w_-_t_a_p_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_ _`_`_`_ _`_`_`_b_a_s_h_ _$
-_b_r_e_w_ _u_n_i_n_s_t_a_l_l_ _-_-_c_a_s_k_ _c_s_v_2_n_o_t_i_o_n_-_n_e_o_ _`_`_`_ _#_#_#_ _W_i_t_h_ _P_I_P_ _`_`_`_b_a_s_h_ _$_ _p_i_p_ _i_n_s_t_a_l_l_ _-_-
-_u_s_e_r_ _c_s_v_2_n_o_t_i_o_n___n_e_o_ _`_`_`_ _*_*_P_y_t_h_o_n_ _3_._7_ _o_r_ _l_a_t_e_r_ _r_e_q_u_i_r_e_d_._*_*_ _#_#_#_ _F_r_o_m_ _s_o_u_r_c_e_ _T_h_i_s
-_p_r_o_j_e_c_t_ _u_s_e_s_ _[_p_o_e_t_r_y_]_(_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_p_o_e_t_r_y_._o_r_g_/_)_ _f_o_r_ _d_e_p_e_n_d_e_n_c_y_ _m_a_n_a_g_e_m_e_n_t_ _a_n_d
-_p_a_c_k_a_g_i_n_g_._ _Y_o_u_ _w_i_l_l_ _h_a_v_e_ _t_o_ _i_n_s_t_a_l_l_ _i_t_ _f_i_r_s_t_._ _S_e_e_ _[_p_o_e_t_r_y_ _o_f_f_i_c_i_a_l
-_d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/_p_y_t_h_o_n_-_p_o_e_t_r_y_._o_r_g_/_d_o_c_s_/_)_ _f_o_r_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _`_`_`_s_h_e_l_l_ _$
-_g_i_t_ _c_l_o_n_e_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_._g_i_t_ _$_ _c_d_ _c_s_v_2_n_o_t_i_o_n___n_e_o_/
-_$_ _p_o_e_t_r_y_ _i_n_s_t_a_l_l_ _-_-_n_o_-_d_e_v_ _$_ _p_o_e_t_r_y_ _r_u_n_ _c_s_v_2_n_o_t_i_o_n___n_e_o_ _`_`_`_ _#_#_ _G_u_i_d_e_ _`_`_`_p_l_a_i_n_ _$
-_c_s_v_2_n_o_t_i_o_n___n_e_o_ _-_-_h_e_l_p_ _u_s_a_g_e_:_ _c_s_v_2_n_o_t_i_o_n___n_e_o_ _[_-_h_]_ _-_-_t_o_k_e_n_ _T_O_K_E_N_ _[_-_-_u_r_l_ _U_R_L_]
-_[_O_P_T_I_O_N_]_._._._ _F_I_L_E_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_ _U_p_l_o_a_d_ _&_ _M_e_r_g_e
-_C_S_V_ _o_r_ _J_S_O_N_ _D_a_t_a_ _w_i_t_h_ _I_m_a_g_e_s_ _t_o_ _N_o_t_i_o_n_ _D_a_t_a_b_a_s_e_ _p_o_s_i_t_i_o_n_a_l_ _a_r_g_u_m_e_n_t_s_:_ _F_I_L_E_ _C_S_V
-_o_r_ _J_S_O_N_ _f_i_l_e_ _t_o_ _u_p_l_o_a_d_ _g_e_n_e_r_a_l_ _o_p_t_i_o_n_s_:_ _-_-_w_o_r_k_s_p_a_c_e_ _a_c_t_i_v_e_ _N_o_t_i_o_n_ _w_o_r_k_s_p_a_c_e
-_n_a_m_e_ _-_-_t_o_k_e_n_ _N_o_t_i_o_n_ _t_o_k_e_n_,_ _s_t_o_r_e_d_ _i_n_ _t_o_k_e_n___v_2_ _c_o_o_k_i_e_ _f_o_r_ _n_o_t_i_o_n_._s_o_ _-_-_u_r_l_ _U_R_L
-_N_o_t_i_o_n_ _d_a_t_a_b_a_s_e_ _U_R_L_;_ _i_f_ _n_o_n_e_ _i_s_ _p_r_o_v_i_d_e_d_,_ _w_i_l_l_ _c_r_e_a_t_e_ _a_ _n_e_w_ _d_a_t_a_b_a_s_e_ _-_-_m_a_x_-
-_t_h_r_e_a_d_s_ _u_p_l_o_a_d_ _t_h_r_e_a_d_s_ _(_d_e_f_a_u_l_t_:_ _5_)_ _-_-_l_o_g_ _F_I_L_E_ _f_i_l_e_ _t_o_ _s_t_o_r_e_ _p_r_o_g_r_a_m_ _l_o_g_ _-_-
-_v_e_r_b_o_s_e_ _o_u_t_p_u_t_ _d_e_b_u_g_ _i_n_f_o_r_m_a_t_i_o_n_ _-_-_v_e_r_s_i_o_n_ _s_h_o_w_ _p_r_o_g_r_a_m_'_s_ _v_e_r_s_i_o_n_ _n_u_m_b_e_r_ _a_n_d
-_e_x_i_t_ _-_h_,_ _-_-_h_e_l_p_ _s_h_o_w_ _t_h_i_s_ _h_e_l_p_ _m_e_s_s_a_g_e_ _a_n_d_ _e_x_i_t_ _c_o_l_u_m_n_ _o_p_t_i_o_n_s_:_ _-_-_c_o_l_u_m_n_-_t_y_p_e_s
-_c_o_m_m_a_-_s_e_p_a_r_a_t_e_d_ _l_i_s_t_ _o_f_ _c_o_l_u_m_n_ _t_y_p_e_s_ _t_o_ _u_s_e_ _f_o_r_ _n_o_n_-_k_e_y_ _c_o_l_u_m_n_s_;_ _i_f_ _n_o_n_e_ _i_s
-_p_r_o_v_i_d_e_d_,_ _t_y_p_e_s_ _w_i_l_l_ _b_e_ _g_u_e_s_s_e_d_ _f_r_o_m_ _C_S_V_ _v_a_l_u_e_s_ _(_c_a_n_ _a_l_s_o_ _b_e_ _u_s_e_d_ _w_i_t_h_ _-_-_a_d_d_-
-_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_ _f_l_a_g_)_ _-_-_a_d_d_-_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_ _i_f_ _c_o_l_u_m_n_s_ _a_r_e_ _p_r_e_s_e_n_t_ _i_n_ _C_S_V_ _b_u_t
-_n_o_t_ _i_n_ _N_o_t_i_o_n_ _D_B_,_ _a_d_d_ _t_h_e_m_ _t_o_ _N_o_t_i_o_n_ _D_B_ _-_-_r_e_n_a_m_e_-_n_o_t_i_o_n_-_k_e_y_-_c_o_l_u_m_n_ _r_e_n_a_m_e_ _t_h_e
-_k_e_y_ _c_o_l_u_m_n_ _i_n_ _t_h_e_ _f_i_l_e_ _t_o_ _a_ _d_i_f_f_e_r_e_n_t_ _k_e_y_ _c_o_l_u_m_n_ _i_n_ _A_i_r_t_a_b_l_e_ _-_-_r_a_n_d_o_m_i_z_e_-
-_s_e_l_e_c_t_-_c_o_l_o_r_s_ _r_a_n_d_o_m_i_z_e_ _c_o_l_o_r_s_ _f_o_r_ _a_d_d_e_d_ _o_p_t_i_o_n_s_ _i_n_ _s_e_l_e_c_t_ _a_n_d_ _m_u_l_t_i_ _s_e_l_e_c_t
-_c_o_l_u_m_n_s_ _m_e_r_g_e_ _o_p_t_i_o_n_s_:_ _-_-_m_e_r_g_e_ _m_e_r_g_e_ _C_S_V_ _o_r_ _J_S_O_N_ _w_i_t_h_ _e_x_i_s_t_i_n_g_ _N_o_t_i_o_n_ _D_B_ _r_o_w_s_,
-_f_i_r_s_t_ _c_o_l_u_m_n_ _w_i_l_l_ _b_e_ _u_s_e_d_ _a_s_ _a_ _k_e_y_ _-_-_m_e_r_g_e_-_o_n_l_y_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t
-_s_h_o_u_l_d_ _b_e_ _u_p_d_a_t_e_d_ _o_n_ _m_e_r_g_e_;_ _w_h_e_n_ _p_r_o_v_i_d_e_d_,_ _o_t_h_e_r_ _c_o_l_u_m_n_s_ _w_i_l_l_ _b_e_ _i_g_n_o_r_e_d_ _(_u_s_e
-_m_u_l_t_i_p_l_e_ _t_i_m_e_s_ _f_o_r_ _m_u_l_t_i_p_l_e_ _c_o_l_u_m_n_s_)_ _-_-_m_e_r_g_e_-_s_k_i_p_-_n_e_w_ _s_k_i_p_ _n_e_w_ _r_o_w_s_ _i_n_ _C_S_V_ _o_r
-_J_S_O_N_ _t_h_a_t_ _a_r_e_ _n_o_t_ _a_l_r_e_a_d_y_ _i_n_ _N_o_t_i_o_n_ _D_B_ _d_u_r_i_n_g_ _m_e_r_g_e_ _r_e_l_a_t_i_o_n_s_ _o_p_t_i_o_n_s_:_ _-_-_a_d_d_-
-_m_i_s_s_i_n_g_-_r_e_l_a_t_i_o_n_s_ _a_d_d_ _m_i_s_s_i_n_g_ _e_n_t_r_i_e_s_ _i_n_t_o_ _l_i_n_k_e_d_ _N_o_t_i_o_n_ _D_B_ _p_a_g_e_ _c_o_v_e_r_ _o_p_t_i_o_n_s_:
-_-_-_i_m_a_g_e_-_c_o_l_u_m_n_ _C_O_L_U_M_N_ _o_n_e_ _o_r_ _m_o_r_e_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _p_o_i_n_t_s_ _t_o_ _U_R_L_ _o_r
-_i_m_a_g_e_ _f_i_l_e_ _t_h_a_t_ _w_i_l_l_ _b_e_ _e_m_b_e_d_d_e_d_ _f_o_r_ _t_h_a_t_ _r_o_w_ _-_-_i_m_a_g_e_-_c_o_l_u_m_n_-_k_e_e_p_ _k_e_e_p_ _i_m_a_g_e
-_C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _a_s_ _a_ _N_o_t_i_o_n_ _D_B_ _c_o_l_u_m_n_ _-_-_i_m_a_g_e_-_c_o_l_u_m_n_-_m_o_d_e_ _{_c_o_v_e_r_,_b_l_o_c_k_}
-_u_p_l_o_a_d_ _i_m_a_g_e_ _a_s_ _[_c_o_v_e_r_]_ _o_r_ _i_n_s_e_r_t_ _i_t_ _a_s_ _[_b_l_o_c_k_]_ _(_d_e_f_a_u_l_t_:_ _b_l_o_c_k_)_ _-_-_i_m_a_g_e_-
-_c_a_p_t_i_o_n_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _p_o_i_n_t_s_ _t_o_ _t_e_x_t_ _c_a_p_t_i_o_n_ _t_h_a_t_ _w_i_l_l_ _b_e
-_a_d_d_e_d_ _t_o_ _t_h_e_ _i_m_a_g_e_ _b_l_o_c_k_ _i_f_ _-_-_i_m_a_g_e_-_c_o_l_u_m_n_-_m_o_d_e_ _i_s_ _s_e_t_ _t_o_ _'_b_l_o_c_k_'_ _-_-_i_m_a_g_e_-
-_c_a_p_t_i_o_n_-_c_o_l_u_m_n_-_k_e_e_p_ _k_e_e_p_ _i_m_a_g_e_ _c_a_p_t_i_o_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _a_s_ _a_ _N_o_t_i_o_n_ _D_B_ _c_o_l_u_m_n
-_p_a_g_e_ _i_c_o_n_ _o_p_t_i_o_n_s_:_ _-_-_i_c_o_n_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _p_o_i_n_t_s_ _t_o_ _e_m_o_j_i_,_ _U_R_L
-_o_r_ _i_m_a_g_e_ _f_i_l_e_ _t_h_a_t_ _w_i_l_l_ _b_e_ _u_s_e_d_ _a_s_ _p_a_g_e_ _i_c_o_n_ _f_o_r_ _t_h_a_t_ _r_o_w_ _-_-_i_c_o_n_-_c_o_l_u_m_n_-_k_e_e_p
-_k_e_e_p_ _i_c_o_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _a_s_ _a_ _N_o_t_i_o_n_ _D_B_ _c_o_l_u_m_n_ _-_-_d_e_f_a_u_l_t_-_i_c_o_n_ _I_C_O_N_ _E_m_o_j_i_,
-_U_R_L_ _o_r_ _i_m_a_g_e_ _f_i_l_e_ _t_h_a_t_ _w_i_l_l_ _b_e_ _u_s_e_d_ _a_s_ _p_a_g_e_ _i_c_o_n_ _f_o_r_ _e_v_e_r_y_ _r_o_w_ _b_y_ _d_e_f_a_u_l_t
-_v_a_l_i_d_a_t_i_o_n_ _o_p_t_i_o_n_s_:_ _-_-_m_a_n_d_a_t_o_r_y_-_c_o_l_u_m_n_ _C_S_V_ _o_r_ _J_S_O_N_ _c_o_l_u_m_n_ _t_h_a_t_ _c_a_n_n_o_t_ _b_e_ _e_m_p_t_y
-_(_u_s_e_ _m_u_l_t_i_p_l_e_ _t_i_m_e_s_ _f_o_r_ _m_u_l_t_i_p_l_e_ _c_o_l_u_m_n_s_)_ _-_-_p_a_y_l_o_a_d_-_k_e_y_-_c_o_l_u_m_n_ _J_S_O_N_ _o_b_j_e_c_t_ _t_h_a_t
-_i_s_ _t_h_e_ _k_e_y_ _i_n_ _N_o_t_i_o_n_ _D_B_;_ _i_f_ _J_S_O_N_ _f_i_l_e_ _i_s_ _u_s_e_d_,_ _t_h_i_s_ _c_a_n_n_o_t_ _b_e_ _e_m_p_t_y_ _-_-_f_a_i_l_-_o_n_-
-_r_e_l_a_t_i_o_n_-_d_u_p_l_i_c_a_t_e_s_ _f_a_i_l_ _i_f_ _a_n_y_ _l_i_n_k_e_d_ _D_B_s_ _i_n_ _r_e_l_a_t_i_o_n_ _c_o_l_u_m_n_s_ _h_a_v_e_ _d_u_p_l_i_c_a_t_e
-_e_n_t_r_i_e_s_;_ _o_t_h_e_r_w_i_s_e_,_ _f_i_r_s_t_ _e_n_t_r_y_ _i_n_ _a_l_p_h_a_b_e_t_i_c_a_l_ _o_r_d_e_r_ _w_i_l_l_ _b_e_ _t_r_e_a_t_e_d_ _a_s_ _u_n_i_q_u_e
-_w_h_e_n_ _l_o_o_k_i_n_g_ _u_p_ _r_e_l_a_t_i_o_n_s_ _-_-_f_a_i_l_-_o_n_-_d_u_p_l_i_c_a_t_e_s_ _f_a_i_l_ _i_f_ _N_o_t_i_o_n_ _D_B_ _o_r_ _C_S_V_ _o_r_ _J_S_O_N
-_h_a_s_ _d_u_p_l_i_c_a_t_e_s_ _i_n_ _k_e_y_ _c_o_l_u_m_n_,_ _u_s_e_f_u_l_ _w_h_e_n_ _s_a_n_i_t_i_z_i_n_g_ _b_e_f_o_r_e_ _m_e_r_g_e_ _t_o_ _a_v_o_i_d
-_a_m_b_i_g_u_o_u_s_ _m_a_p_p_i_n_g_ _-_-_f_a_i_l_-_o_n_-_d_u_p_l_i_c_a_t_e_-_c_s_v_-_c_o_l_u_m_n_s_ _f_a_i_l_ _i_f_ _C_S_V_ _o_r_ _J_S_O_N_ _h_a_s
-_d_u_p_l_i_c_a_t_e_ _c_o_l_u_m_n_s_;_ _o_t_h_e_r_w_i_s_e_ _l_a_s_t_ _c_o_l_u_m_n_ _w_i_l_l_ _b_e_ _u_s_e_d_ _-_-_f_a_i_l_-_o_n_-_c_o_n_v_e_r_s_i_o_n_-
-_e_r_r_o_r_ _f_a_i_l_ _i_f_ _a_n_y_ _c_o_l_u_m_n_ _t_y_p_e_ _c_o_n_v_e_r_s_i_o_n_ _e_r_r_o_r_ _o_c_c_u_r_s_;_ _o_t_h_e_r_w_i_s_e_ _e_r_r_o_r_s_ _w_i_l_l_ _b_e
-_r_e_p_l_a_c_e_d_ _w_i_t_h_ _e_m_p_t_y_ _s_t_r_i_n_g_s_ _-_-_f_a_i_l_-_o_n_-_i_n_a_c_c_e_s_s_i_b_l_e_-_r_e_l_a_t_i_o_n_s_ _f_a_i_l_ _i_f_ _a_n_y
-_r_e_l_a_t_i_o_n_ _c_o_l_u_m_n_ _p_o_i_n_t_s_ _t_o_ _a_ _N_o_t_i_o_n_ _D_B_ _t_h_a_t_ _i_s_ _n_o_t_ _a_c_c_e_s_s_i_b_l_e_ _t_o_ _t_h_e_ _c_u_r_r_e_n_t
-_u_s_e_r_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _c_o_l_u_m_n_s_ _w_i_l_l_ _b_e_ _i_g_n_o_r_e_d_ _-_-_f_a_i_l_-_o_n_-_m_i_s_s_i_n_g_-_c_o_l_u_m_n_s_ _f_a_i_l_ _i_f
-_c_o_l_u_m_n_s_ _a_r_e_ _p_r_e_s_e_n_t_ _i_n_ _C_S_V_ _b_u_t_ _n_o_t_ _i_n_ _N_o_t_i_o_n_ _D_B_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _c_o_l_u_m_n_s_ _w_i_l_l
-_b_e_ _i_g_n_o_r_e_d_ _-_-_f_a_i_l_-_o_n_-_u_n_s_e_t_t_a_b_l_e_-_c_o_l_u_m_n_s_ _f_a_i_l_ _i_f_ _D_B_ _h_a_s_ _c_o_l_u_m_n_s_ _t_h_a_t_ _d_o_n_'_t
-_s_u_p_p_o_r_t_ _a_s_s_i_g_n_i_n_g_ _v_a_l_u_e_ _t_o_ _t_h_e_m_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _c_o_l_u_m_n_s_ _w_i_l_l_ _b_e_ _i_g_n_o_r_e_d
-_(_c_o_l_u_m_n_s_ _w_i_t_h_ _t_y_p_e_ _c_r_e_a_t_e_d___b_y_,_ _l_a_s_t___e_d_i_t_e_d___b_y_,_ _r_o_l_l_u_p_ _o_r_ _f_o_r_m_u_l_a_)_ _-_-_f_a_i_l_-_o_n_-
-_w_r_o_n_g_-_s_t_a_t_u_s_-_v_a_l_u_e_s_ _f_a_i_l_ _i_f_ _v_a_l_u_e_s_ _f_o_r_ _'_s_t_a_t_u_s_'_ _c_o_l_u_m_n_s_ _d_o_n_'_t_ _h_a_v_e_ _m_a_t_c_h_i_n_g
-_o_p_t_i_o_n_ _i_n_ _D_B_;_ _o_t_h_e_r_w_i_s_e_ _t_h_o_s_e_ _v_a_l_u_e_s_ _w_i_l_l_ _b_e_ _r_e_p_l_a_c_e_d_ _w_i_t_h_ _d_e_f_a_u_l_t_ _s_t_a_t_u_s_ _`_`_`
-_#_#_#_ _m_a_c_O_S_ _R_e_l_e_a_s_e_ _P_r_i_v_a_c_y_ _&_ _S_e_c_u_r_i_t_y
-_F_o_r_ _m_a_c_O_S_,_ _y_o_u_ _h_a_v_e_ _t_h_e_ _o_p_t_i_o_n_ _o_f_ _t_w_o_ _d_i_s_t_i_n_c_t_ _r_e_l_e_a_s_e_s_:_ _o_n_e_ _p_a_c_k_a_g_e_d_ _w_i_t_h_i_n_ _a
-_`_._z_i_p_`_ _a_r_c_h_i_v_e_ _a_n_d_ _t_h_e_ _o_t_h_e_r_ _i_n_ _a_ _`_._p_k_g_`_ _f_o_r_m_a_t_._ _N_a_v_i_g_a_t_e_ _t_o_ _t_h_e_ _`_P_r_i_v_a_c_y_ _&
-_S_e_c_u_r_i_t_y_`_ _s_e_t_t_i_n_g_s_ _a_n_d_ _s_e_t_ _y_o_u_r_ _p_r_e_f_e_r_e_n_c_e_ _t_o_ _`_A_p_p_ _S_t_o_r_e_ _a_n_d_ _i_d_e_n_t_i_f_i_e_d
-_d_e_v_e_l_o_p_e_r_s_`_.
-    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_/_b_l_o_b_/_m_a_s_t_e_r_/_a_s_s_e_t_s_/_m_a_c_O_S_-
-                             _p_r_i_v_a_c_y_._p_n_g_?_r_a_w_=_t_r_u_e_]
+  _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_T_h_e_A_c_h_a_r_y_a_/_c_s_v_2_n_o_t_i_o_n_-_n_e_o_/_b_l_o_b_/_m_a_s_t_e_r_/_a_s_s_e_t_s_/_C_S_V_2_N_o_t_i_o_n
+                            _N_e_o___I_c_o_n_._p_n_g_?_r_a_w_=_t_r_u_e_]
+                         _**_**_**_**_**_**_ _CC_SS_VV_22_NN_oo_tt_ii_oo_nn_ _NN_ee_oo_ _**_**_**_**_**_**
+                    _[_l_i_c_e_n_s_e_]_[_P_y_P_I_]_[_P_y_t_h_o_n_]_[_r_e_l_e_a_s_e___g_i_t_h_u_b_]
+An advance method to upload & merge *.csv or *.json files with images to _N_o_t_i_o_n
+database. ## Core Features ### Advantages over native import - Merge CSV or
+JSON with the existing database, using the first column as a key to combine
+existing rows - Choose column types manually instead of letting Notion
+detecting them automatically - Link or create new entries in relation columns
+based on their values automatically - Easily upload files into the designated
+"Files & Media" column - Assign a icon for each row for quick identification -
+Set a cover or embed an image for each row to enhance visual representation -
+Upload image files for covers or icons - Apply validation options for input
+data to ensure accuracy ### Disadvantages over native import - Importing each
+row separately might lead to slower speed - To address this, utilise
+multithreaded upload ## Table of contents - [Background](#background) -
+[Installation](#installation) - [Pre-compiled Binary (Recommended)](#pre-
+compiled-binary-recommended) - [From Source](#from-source) - [Guide](#guide) -
+[macOS Release](#macos-release) - [Prerequisite](#prerequisite) - [Upload
+Speed](#upload-speed) - [Duplicate CSV Columns](#duplicate-csv-columns) -
+[Missing Columns](#missing-columns) - [Column Types](#column-types) - [Mergin]
+(#merging) - [Relation Columns](#relation-columns) - [Cover Image & Embedded
+Image](#cover-image--embedded-image) - [Icons](#icons) - [Mandatory Columns]
+(#mandatory-columns) - [Examples](#examples) - [Credits](#credits) - [License]
+(#license) - [Reporting Bugs](#reporting-bugs) ## Background Originally, we
+developed [csv2notion](https://github.com/vzhd1701/csv2notion) to address the
+lack of advanced importing support for `*.csv` files in [Notion](https://
+notion.so). We took inspiration from [Airtable](https://www.airtable.com)âs
+[CSV import extension](https://support.airtable.com/docs/csv-import-extension).
+**CSV2Notion Neo** was created as a spin-off project to address inactivity in
+the original repository and maintain compatibility with Notion. As Notion
+changes or updates its backend API periodically, we aim to fix, update and add
+new features to the tool in a timely manner. Any dependent tools or project
+that relied on [csv2notion](https://github.com/vzhd1701/csv2notion), can use
+our **CSV2Notion Neo** tool interchangeably requiring additional augments. ##
+Installation ### Pre-compiled Binary (Recommended) Download the latest release
+of the latest binary release [here](https://github.com/TheAcharya/csv2notion-
+neo/releases). ### With [Homebrew](https://brew.sh/) (Recommended for macOS)
+```bash $ brew install TheAcharya/homebrew-tap/csv2notion-neo ``` ```bash $
+brew uninstall --cask csv2notion-neo ``` ### With PIP ```bash $ pip install --
+user csv2notion_neo ``` **Python 3.7 or later required.** ### From source This
+project uses [poetry](https://python-poetry.org/) for dependency management and
+packaging. You will have to install it first. See [poetry official
+documentation](https://python-poetry.org/docs/) for instructions. ```shell $
+git clone https://github.com/TheAcharya/csv2notion-neo.git $ cd csv2notion_neo/
+$ poetry install --no-dev $ poetry run csv2notion_neo ``` ## Guide ```plain $
+csv2notion_neo --help usage: csv2notion_neo [-h] --token TOKEN [--url URL]
+[OPTION]... FILE https://github.com/TheAcharya/csv2notion-neo Upload & Merge
+CSV or JSON Data with Images to Notion Database positional arguments: FILE CSV
+or JSON file to upload general options: --workspace active Notion workspace
+name --token Notion token, stored in token_v2 cookie for notion.so --url URL
+Notion database URL; if none is provided, will create a new database --max-
+threads upload threads (default: 5) --log FILE file to store program log --
+verbose output debug information --version show program's version number and
+exit -h, --help show this help message and exit column options: --column-types
+comma-separated list of column types to use for non-key columns; if none is
+provided, types will be guessed from CSV values (can also be used with --add-
+missing-columns flag) --add-missing-columns if columns are present in CSV but
+not in Notion DB, add them to Notion DB --rename-notion-key-column rename the
+key column in the file to a different key column in Airtable --randomize-
+select-colors randomize colors for added options in select and multi select
+columns merge options: --merge merge CSV or JSON with existing Notion DB rows,
+first column will be used as a key --merge-only-column CSV or JSON column that
+should be updated on merge; when provided, other columns will be ignored (use
+multiple times for multiple columns) --merge-skip-new skip new rows in CSV or
+JSON that are not already in Notion DB during merge relations options: --add-
+missing-relations add missing entries into linked Notion DB page cover options:
+--image-column COLUMN one or more CSV or JSON column that points to URL or
+image file that will be embedded for that row --image-column-keep keep image
+CSV or JSON column as a Notion DB column --image-column-mode {cover,block}
+upload image as [cover] or insert it as [block] (default: block) --image-
+caption-column CSV or JSON column that points to text caption that will be
+added to the image block if --image-column-mode is set to 'block' --image-
+caption-column-keep keep image caption CSV or JSON column as a Notion DB column
+page icon options: --icon-column CSV or JSON column that points to emoji, URL
+or image file that will be used as page icon for that row --icon-column-keep
+keep icon CSV or JSON column as a Notion DB column --default-icon ICON Emoji,
+URL or image file that will be used as page icon for every row by default
+validation options: --mandatory-column CSV or JSON column that cannot be empty
+(use multiple times for multiple columns) --payload-key-column JSON object that
+is the key in Notion DB; if JSON file is used, this cannot be empty --fail-on-
+relation-duplicates fail if any linked DBs in relation columns have duplicate
+entries; otherwise, first entry in alphabetical order will be treated as unique
+when looking up relations --fail-on-duplicates fail if Notion DB or CSV or JSON
+has duplicates in key column, useful when sanitizing before merge to avoid
+ambiguous mapping --fail-on-duplicate-csv-columns fail if CSV or JSON has
+duplicate columns; otherwise last column will be used --fail-on-conversion-
+error fail if any column type conversion error occurs; otherwise errors will be
+replaced with empty strings --fail-on-inaccessible-relations fail if any
+relation column points to a Notion DB that is not accessible to the current
+user; otherwise those columns will be ignored --fail-on-missing-columns fail if
+columns are present in CSV but not in Notion DB; otherwise those columns will
+be ignored --fail-on-unsettable-columns fail if DB has columns that don't
+support assigning value to them; otherwise those columns will be ignored
+(columns with type created_by, last_edited_by, rollup or formula) --fail-on-
+wrong-status-values fail if values for 'status' columns don't have matching
+option in DB; otherwise those values will be replaced with default status ```
+### macOS Release Privacy & Security
+For macOS, you have the option of two distinct releases: one packaged within a
+`.zip` archive and the other in a `.pkg` format. Navigate to the `Privacy &
+Security` settings and set your preference to `App Store and identified
+developers`.
+    [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/macOS-
+                             privacy.png?raw=true]
 Utilise the `CSV2Notion Neo.pkg` installer to install the command-line binary
 into your system. Upon completion, find the installed binary `csv2notion_neo`
 located within `/usr/local/bin`. To uninstall, you can utalise this terminal
 command. ```plain sudo rm /usr/local/bin/csv2notion_neo ```
     [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/macOS-
                             installer.png?raw=true]
 ### Prerequisite You must pass a single `*.csv` file for upload. The CSV file
@@ -335,20 +334,16 @@
 Importing JSON into Existing Database with a Different Key Column
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
 YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
 column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-
 Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_10.gif?raw=true]
-## Known Issues - Users would not be able to duplicate entries/records there
-where uploaded using **CSV2Notion Neo** in Notion. - **Workaround:** Simply
-[duplicate](https://www.notion.so/help/duplicate-delete-and-restore-content)
-the database directly in Notion. You would be able to duplicate your entries/
-records in the duplicated database. ## Utilised By ### [CommandPost](https://
-commandpost.io) CommandPost's Notion Toolbox
+## Utilised By ### [CommandPost](https://commandpost.io) CommandPost's Notion
+Toolbox
   [https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/
                          toolbox-notion.png?raw=true]
 ## Credits Original Idea and Workflow Architecture by [Vigneswaran Rajkumar]
 (https://twitter.com/IAmVigneswaran) Maintained by [Arjun Prakash](https://
 github.com/arjunprakash027) (1.0.0 ...) Original Work by [Vladilen Zhdanov]
 (https://github.com/vzhd1701) Icon Design by [Bor Jen Goh](https://
 www.artstation.com/borjengoh) ## License Licensed under the MIT license. See
```

