# Comparing `tmp/django_unfold_admin_list_filter_dropdown-1.0.4.tar.gz` & `tmp/django_unfold_admin_list_filter_dropdown-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_unfold_admin_list_filter_dropdown-1.0.4.tar", last modified: Fri Apr 26 14:41:33 2024, max compression
+gzip compressed data, was "django_unfold_admin_list_filter_dropdown-1.0.5.tar", last modified: Sat May 11 15:23:21 2024, max compression
```

## Comparing `django_unfold_admin_list_filter_dropdown-1.0.4.tar` & `django_unfold_admin_list_filter_dropdown-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:41:33.690832 django_unfold_admin_list_filter_dropdown-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 14:41:33.690832 django_unfold_admin_list_filter_dropdown-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:41:33.690832 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_list_filter_dropdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-26 14:41:33.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 14:41:33.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_list_filter_dropdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:41:33.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_list_filter_dropdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-26 14:41:33.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_list_filter_dropdown.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:41:33.690832 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:41:33.686833 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:41:33.690832 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/dropdown_filter.html
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:41:33.690832 django_unfold_admin_list_filter_dropdown-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-26 14:41:30.000000 django_unfold_admin_list_filter_dropdown-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:23:21.132197 django_unfold_admin_list_filter_dropdown-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-11 15:23:21.132197 django_unfold_admin_list_filter_dropdown-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:23:21.132197 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_list_filter_dropdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-11 15:23:21.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-11 15:23:21.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_list_filter_dropdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:23:21.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_list_filter_dropdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 15:23:21.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_list_filter_dropdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:23:21.132197 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:23:21.128197 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:23:21.132197 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/dropdown_filter.html
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:23:21.132197 django_unfold_admin_list_filter_dropdown-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-11 15:23:14.000000 django_unfold_admin_list_filter_dropdown-1.0.5/setup.py
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/LICENSE` & `django_unfold_admin_list_filter_dropdown-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/PKG-INFO` & `django_unfold_admin_list_filter_dropdown-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-unfold-admin-list-filter-dropdown
-Version: 1.0.4
+Version: 1.0.5
 Summary: Use dropdowns in Django admin list filter
 Home-page: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdown
-Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.4.zip
+Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.5.zip
 Author: Franco Borrelli
 Author-email: francoborrelli96@gmail.com
 License: MIT License
 Keywords: django,admin,filter,dropdown,unfold,django-unfold
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/README.md` & `django_unfold_admin_list_filter_dropdown-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO` & `django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_list_filter_dropdown.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-unfold-admin-list-filter-dropdown
-Version: 1.0.4
+Version: 1.0.5
 Summary: Use dropdowns in Django admin list filter
 Home-page: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdown
-Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.4.zip
+Download-URL: https://github.com/francoborrelli/django-unfold-admin-list-filter-dropdow/archive/1.0.5.zip
 Author: Franco Borrelli
 Author-email: francoborrelli96@gmail.com
 License: MIT License
 Keywords: django,admin,filter,dropdown,unfold,django-unfold
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/filters.py` & `django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/filters.py`

 * *Files identical despite different names*

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/dropdown_filter.html` & `django_unfold_admin_list_filter_dropdown-1.0.5/django_unfold_admin_listfilter_dropdown/templates/django_unfold_admin_listfilter_dropdown/dropdown_filter.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 {% load i18n %}
 <div class="mb-6">
     <script type="text/javascript">var go_from_select = function(opt) { window.location = window.location.pathname + opt };</script>
-    <h3>{% blocktrans with title as filter_title %} By {{ filter_title }} {% endblocktrans %}</h3>
+    <h3 class="font-medium mb-4 text-gray-700 text-sm dark:text-gray-200">{% blocktrans with title as filter_title %} By {{ filter_title }} {% endblocktrans %}</h3>
     <ul class="admin-filter-{{ title|cut:' ' }}">
-    {% if choices|slice:"4:" %}
-        <li>
-        <select
-            style="background: none !important; padding: 10px;"
-            class="select2 select2-container select2-container--admin-autocomplete border bg-white font-medium rounded-md shadow-sm text-gray-500 text-sm focus:ring focus:ring-primary-300 focus:border-primary-600 focus:outline-none group-[.errors]:border-red-600 group-[.errors]:focus:ring-red-200"
-            onchange="go_from_select(this.options[this.selectedIndex].value)">
-        {% for choice in choices %}
-            <option{% if choice.selected %} selected="selected"{% endif %}
-            value="{{ choice.query_string|iriencode }}">{{ choice.display }}</option>
-        {% endfor %}
-        </select>
-        </li>
-    {% else %}
-        {% for choice in choices %}
-                <li{% if choice.selected %} class="selected"{% endif %}>
-                <a href="{{ choice.query_string|iriencode }}">{{ choice.display }}</a></li>
-        {% endfor %}
-    {% endif %}
+    <li>
+    <select
+        style="background: none !important; padding: 10px;"
+        class="select2 select2-container select2-container--admin-autocomplete border bg-white font-medium rounded-md shadow-sm text-gray-500 text-sm focus:ring focus:ring-primary-300 focus:border-primary-600 focus:outline-none group-[.errors]:border-red-600 group-[.errors]:focus:ring-red-200"
+        onchange="go_from_select(this.options[this.selectedIndex].value)">
+    {% for choice in choices %}
+        <option{% if choice.selected %} selected="selected"{% endif %}
+        value="{{ choice.query_string|iriencode }}">{{ choice.display }}</option>
+    {% endfor %}
+    </select>
+    </li>
     </ul>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
 {% load i18n %}
 ******** {{%% bblloocckkttrraannss wwiitthh ttiittllee aass ffiilltteerr__ttiittllee %%}} BByy {{{{ ffiilltteerr__ttiittllee }}}} {{%%
 eennddbblloocckkttrraannss %%}} ********
-    * {% if choices|slice:"4:" %}
     * {% for choice in choices %}
     * % if choice.selected %} selected="selected"{% endif %} value="{
       { choice.query_string|iriencode }}">{{ choice.display }}
     * {% endfor %}
-{% else %} {% for choice in choices %}
-% if choice.selected %} class="selected"{% endif %}> _{_{_ _c_h_o_i_c_e_._d_i_s_p_l_a_y_ _}_}
-{% endfor %} {% endif %}
```

### Comparing `django_unfold_admin_list_filter_dropdown-1.0.4/setup.py` & `django_unfold_admin_list_filter_dropdown-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encoding: utf-8
 
 import os
 from setuptools import find_packages, setup
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 description = 'Use dropdowns in Django admin list filter'
 
 setup(
```

