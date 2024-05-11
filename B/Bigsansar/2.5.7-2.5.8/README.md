# Comparing `tmp/Bigsansar-2.5.7.tar.gz` & `tmp/bigsansar-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-2.5.7.tar", last modified: Sat Mar 23 13:32:51 2024, max compression
+gzip compressed data, was "bigsansar-2.5.8.tar", last modified: Sat May 11 15:09:32 2024, max compression
```

## Comparing `Bigsansar-2.5.7.tar` & `bigsansar-2.5.8.tar`

### file list

```diff
@@ -1,189 +1,196 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.860576 Bigsansar-2.5.7/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.860576 Bigsansar-2.5.7/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5335 2024-03-23 13:32:51.000000 Bigsansar-2.5.7/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     6882 2024-03-23 13:32:51.000000 Bigsansar-2.5.7/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2024-03-23 13:32:51.000000 Bigsansar-2.5.7/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       50 2024-03-23 13:32:51.000000 Bigsansar-2.5.7/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2024-03-23 13:32:51.000000 Bigsansar-2.5.7/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2024-03-23 13:32:51.000000 Bigsansar-2.5.7/Bigsansar.egg-info/top_level.txt
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5335 2024-03-23 13:32:51.860576 Bigsansar-2.5.7/PKG-INFO
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4410 2024-03-20 10:24:55.000000 Bigsansar-2.5.7/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.790577 Bigsansar-2.5.7/bigsansar/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.790577 Bigsansar-2.5.7/bigsansar/contrib/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.800577 Bigsansar-2.5.7/bigsansar/contrib/account/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.800577 Bigsansar-2.5.7/bigsansar/contrib/account/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/models.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.800577 Bigsansar-2.5.7/bigsansar/contrib/account/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.800577 Bigsansar-2.5.7/bigsansar/contrib/advance/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      167 2024-03-19 15:09:06.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3395 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.810577 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0003_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0005_delete_css.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0007_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      527 2024-03-17 14:08:34.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      631 2024-03-18 12:34:06.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      922 2024-03-18 12:32:25.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.810577 Bigsansar-2.5.7/bigsansar/contrib/advance/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-19 14:52:06.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-03-23 08:00:26.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/templatetags/nav_bar.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      659 2024-02-09 10:30:34.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     6566 2024-03-23 13:31:59.000000 Bigsansar-2.5.7/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.810577 Bigsansar-2.5.7/bigsansar/contrib/blogs/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.810577 Bigsansar-2.5.7/bigsansar/contrib/blogs/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.810577 Bigsansar-2.5.7/bigsansar/contrib/blogs/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/templatetags/blogs.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.820577 Bigsansar-2.5.7/bigsansar/contrib/sites/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1617 2024-02-12 08:59:23.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/admin.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/apps.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-03-08 12:27:07.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.820577 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0001_initial.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-02-09 11:54:41.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0002_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-02-12 05:36:07.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0003_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-02-12 05:50:44.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-02-12 05:54:39.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-02-12 05:59:18.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-02-12 06:24:52.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-02-12 07:22:55.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-02-12 07:58:58.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2024-03-08 11:54:46.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2398 2024-03-08 11:39:58.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.820577 Bigsansar-2.5.7/bigsansar/contrib/sites/templatetags/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/templatetags/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/templatetags/pages.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-02-12 08:27:38.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-03-23 08:21:22.000000 Bigsansar-2.5.7/bigsansar/contrib/sites/views.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/contrib/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.820577 Bigsansar-2.5.7/bigsansar/core/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-03-01 14:39:47.000000 Bigsansar-2.5.7/bigsansar/core/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/core/host.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-03-03 13:13:14.000000 Bigsansar-2.5.7/bigsansar/core/init.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-03-01 14:40:11.000000 Bigsansar-2.5.7/bigsansar/core/pip_package.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    16364 2024-03-16 12:02:48.000000 Bigsansar-2.5.7/bigsansar/core/ubuntu.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/etc/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/etc/apache2.conf
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/etc/config_chroot.sh
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-03-16 12:06:01.000000 Bigsansar-2.5.7/bigsansar/etc/db.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/etc/sshd_config
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/management/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/management/commands/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/management/commands/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-02-19 11:53:53.000000 Bigsansar-2.5.7/bigsansar/management/commands/createuser.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-02-19 11:56:02.000000 Bigsansar-2.5.7/bigsansar/management/commands/setup_server.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/migrations/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/migrations/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/static/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.780577 Bigsansar-2.5.7/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.780577 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.780577 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.830577 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.850576 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/logo.png
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.850576 Bigsansar-2.5.7/bigsansar/templates/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/404.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/__init__.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/acc_active_email.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-03-23 13:32:51.860576 Bigsansar-2.5.7/bigsansar/templates/admin/
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-03-23 13:20:20.000000 Bigsansar-2.5.7/bigsansar/templates/admin/account_info.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/admin_update.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/chpass.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/chuname.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/create_domain.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-02-09 12:33:05.000000 Bigsansar-2.5.7/bigsansar/templates/admin/domain_manage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/edit_domain.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/editprofile.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/login.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     5881 2024-03-23 13:26:08.000000 Bigsansar-2.5.7/bigsansar/templates/admin/nav.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/page_create.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/page_delete.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/admin/page_edit.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1619 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/base.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/blog_preview.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-03-09 11:06:44.000000 Bigsansar-2.5.7/bigsansar/templates/default.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/defaultpage.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/parking.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/script.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/sitemap.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/templates/styles.html
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/tests.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-02-08 10:55:16.000000 Bigsansar-2.5.7/bigsansar/urls.py
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-02-21 13:18:23.000000 Bigsansar-2.5.7/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-03-23 13:32:51.860576 Bigsansar-2.5.7/setup.cfg
--rwxrwxr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-03-23 13:32:28.000000 Bigsansar-2.5.7/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.588183 bigsansar-2.5.8/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.578183 bigsansar-2.5.8/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5363 2024-05-11 15:09:32.000000 bigsansar-2.5.8/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     7323 2024-05-11 15:09:32.000000 bigsansar-2.5.8/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2024-05-11 15:09:32.000000 bigsansar-2.5.8/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       50 2024-05-11 15:09:32.000000 bigsansar-2.5.8/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2024-05-11 15:09:32.000000 bigsansar-2.5.8/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2024-05-11 15:09:32.000000 bigsansar-2.5.8/Bigsansar.egg-info/top_level.txt
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1073 2024-04-10 03:12:24.000000 bigsansar-2.5.8/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     5363 2024-05-11 15:09:32.588183 bigsansar-2.5.8/PKG-INFO
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     4438 2024-05-11 15:06:57.000000 bigsansar-2.5.8/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.418183 bigsansar-2.5.8/bigsansar/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/admin.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.418183 bigsansar-2.5.8/bigsansar/contrib/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.428183 bigsansar-2.5.8/bigsansar/contrib/account/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      489 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/admin.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      275 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/apps.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1155 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.428183 bigsansar-2.5.8/bigsansar/contrib/account/migrations/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      969 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/migrations/0001_initial.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      400 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/migrations/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      539 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/models.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      340 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.428183 bigsansar-2.5.8/bigsansar/contrib/account/templates/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/templates/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/tests.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/urls.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.438183 bigsansar-2.5.8/bigsansar/contrib/advance/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      157 2024-04-10 05:15:54.000000 bigsansar-2.5.8/bigsansar/contrib/advance/admin.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      202 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      357 2024-05-11 07:59:27.000000 bigsansar-2.5.8/bigsansar/contrib/advance/cf_url.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     4583 2024-04-16 12:22:05.000000 bigsansar-2.5.8/bigsansar/contrib/advance/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.458183 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0001_initial.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1050 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      296 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0005_delete_css.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      289 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0006_delete_javascript.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1075 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0007_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      527 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      631 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2024-04-10 05:16:13.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      391 2024-04-13 11:41:57.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      637 2024-04-16 11:46:02.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/migrations/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1356 2024-04-16 11:46:06.000000 bigsansar-2.5.8/bigsansar/contrib/advance/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.458183 bigsansar-2.5.8/bigsansar/contrib/advance/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1797 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/templatetags/nav_bar.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/advance/tests.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      721 2024-04-16 11:03:13.000000 bigsansar-2.5.8/bigsansar/contrib/advance/urls.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)    20734 2024-05-11 15:08:03.000000 bigsansar-2.5.8/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.458183 bigsansar-2.5.8/bigsansar/contrib/blogs/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     2238 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/admin.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      188 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/apps.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      261 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.458183 bigsansar-2.5.8/bigsansar/contrib/blogs/migrations/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     2261 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      367 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/migrations/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     2028 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.458183 bigsansar-2.5.8/bigsansar/contrib/blogs/templatetags/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/templatetags/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1478 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/templatetags/blogs.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/tests.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       63 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.468183 bigsansar-2.5.8/bigsansar/contrib/sites/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1647 2024-04-20 13:27:20.000000 bigsansar-2.5.8/bigsansar/contrib/sites/admin.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      196 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/apps.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     4435 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.478183 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1847 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0001_initial.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      819 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0002_default_domain.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      385 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0003_domains_default.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      386 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      331 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      653 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      410 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      346 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      405 2024-05-09 10:32:01.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/migrations/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     2453 2024-05-09 10:31:51.000000 bigsansar-2.5.8/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.478183 bigsansar-2.5.8/bigsansar/contrib/sites/templatetags/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/templatetags/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      394 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/templatetags/pages.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/tests.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      547 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/sites/urls.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     9258 2024-04-10 10:36:13.000000 bigsansar-2.5.8/bigsansar/contrib/sites/views.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/urls.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/contrib/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.488183 bigsansar-2.5.8/bigsansar/core/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1018 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/core/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      402 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/core/host.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     9710 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/core/init.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      640 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/core/pip_package.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)    16727 2024-05-11 15:05:41.000000 bigsansar-2.5.8/bigsansar/core/ubuntu.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.488183 bigsansar-2.5.8/bigsansar/etc/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     7287 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/etc/apache2.conf
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1638 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/etc/config_chroot.sh
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     5123 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/etc/db.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     3236 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/etc/sshd_config
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.498183 bigsansar-2.5.8/bigsansar/management/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.498183 bigsansar-2.5.8/bigsansar/management/commands/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/management/commands/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1076 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/management/commands/createuser.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1023 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/management/commands/setup_server.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.498183 bigsansar-2.5.8/bigsansar/migrations/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/migrations/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       57 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.508183 bigsansar-2.5.8/bigsansar/static/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.398183 bigsansar-2.5.8/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.398183 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.408183 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.508183 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.508183 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1258 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1165 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.538183 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1337 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1654 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1184 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1078 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1514 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1024 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1084 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1079 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1161 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      960 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1051 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1226 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1166 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1081 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1171 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1229 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1035 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1022 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1040 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1120 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1151 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1153 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1539 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1173 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1206 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1538 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1067 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      916 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)    13371 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     9230 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/logo.png
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      551 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.558183 bigsansar-2.5.8/bigsansar/templates/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/404.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/__init__.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      164 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/acc_active_email.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2024-05-11 15:09:32.578183 bigsansar-2.5.8/bigsansar/templates/admin/
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)    10272 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/account_info.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      519 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/admin_update.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      878 2024-04-13 11:47:55.000000 bigsansar-2.5.8/bigsansar/templates/admin/cf_config.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/chpass.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      558 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/chuname.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4401 2024-05-11 07:58:01.000000 bigsansar-2.5.8/bigsansar/templates/admin/cloudflare.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      549 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/create_domain.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     8866 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/domain_manage.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1019 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/edit_domain.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      566 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/editprofile.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      979 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/login.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     6004 2024-04-16 11:03:44.000000 bigsansar-2.5.8/bigsansar/templates/admin/nav.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      947 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/page_create.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      948 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/page_delete.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      717 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/admin/page_edit.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1622 2024-05-11 07:51:33.000000 bigsansar-2.5.8/bigsansar/templates/base.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1898 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/blog_preview.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     2197 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/default.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     2200 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/defaultpage.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      719 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/parking.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/script.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      411 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/sitemap.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)      101 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/templates/styles.html
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)       60 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/tests.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1209 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/urls.py
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     4595 2024-04-10 03:12:24.000000 bigsansar-2.5.8/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2024-05-11 15:09:32.588183 bigsansar-2.5.8/setup.cfg
+-rwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)     1914 2024-05-11 15:06:06.000000 bigsansar-2.5.8/setup.py
```

### Comparing `Bigsansar-2.5.7/Bigsansar.egg-info/PKG-INFO` & `bigsansar-2.5.8/Bigsansar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.5.7
+Version: 2.5.8
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://github.com/pokhrelb9/bigsansar
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
@@ -19,14 +19,15 @@
 Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: fontawesomefree
 
 ## New update
+* Working in to cloudflare 
 * fixed some bugs
 * added new db table for nav always open or close.
 * now you can install bigsansar package in to ubuntu and all setup with on command lines
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
@@ -63,15 +64,15 @@
 # for full setup in to server 
 
 this is work only on ubuntu os 
 
 2) type ` python manage.py setup_server` commend for fully setup into server .
 
 [How to Setup a Full Server with BigSansar, Django, and Ubuntu
-](https://youtu.be/iEmI0HO_U0E)
+](https://youtu.be/j8YN6x9XdR4)
 
 # some usefull link 
 [sitemap.xml](http://localhost/sitemap.xml)
 [script.js](http://localhost/script.js)
 [styles.css](http://localhost/styles.css)
 
 # how to edit sitemap , js and css from pages
```

#### html2text {}

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.5.7 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.5.8 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: OS Independent Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: django Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor Requires-Dist: requests Requires-Dist: pillow
-Requires-Dist: fontawesomefree ## New update * fixed some bugs * added new db
-table for nav always open or close. * now you can install bigsansar package in
-to ubuntu and all setup with on command lines # How to get Bigsansar Bigsansar
-is available open-source under the [MIT](https://en.wikipedia.org/wiki/
-MIT_License) license. We recommend using the latest version of Python 3.
-Bigsansar is Fully based on django and linux ubuntu. You can use [bigsansar]
-(https://bigsansar.com) for install packaged. You can use [bigsansar](https://
-bigsansar.com) for install packaged. view our tutorials in [youtube](https://
-youtube.com/bigsansar) for playlist: [bigsansar for django](https://
-www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the
-latest development version The latest and greatest Bigsasnar version is the one
-thatâs in our Git repository (our revision-control system). This is only for
-experienced users who want to try incoming changes and help identify bugs
-before an official release. Get it using this shell command, which requires
-[Git](https://https://git-scm.com/): `git clone https://github.com/pokhrelb9/
-bigsansar.git` You can also download a [gzipped tarball](https://https://
-pypi.org/project/Bigsansar/#files) of the development version. This archive is
-updated every time we commit code. # After you install bigsansar 1) Type
-`bigsansar init` command for **automatically** setup server for internal
+Requires-Dist: fontawesomefree ## New update * Working in to cloudflare * fixed
+some bugs * added new db table for nav always open or close. * now you can
+install bigsansar package in to ubuntu and all setup with on command lines #
+How to get Bigsansar Bigsansar is available open-source under the [MIT](https:/
+/en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
+version of Python 3. Bigsansar is Fully based on django and linux ubuntu. You
+can use [bigsansar](https://bigsansar.com) for install packaged. You can use
+[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
+[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
+(https://www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) #
+Get the latest development version The latest and greatest Bigsasnar version is
+the one thatâs in our Git repository (our revision-control system). This is
+only for experienced users who want to try incoming changes and help identify
+bugs before an official release. Get it using this shell command, which
+requires [Git](https://https://git-scm.com/): `git clone https://github.com/
+pokhrelb9/bigsansar.git` You can also download a [gzipped tarball](https://
+https://pypi.org/project/Bigsansar/#files) of the development version. This
+archive is updated every time we commit code. # After you install bigsansar 1)
+Type `bigsansar init` command for **automatically** setup server for internal
 configurations. ** this command valid into vertualenv for developer # for full
 setup in to server this is work only on ubuntu os 2) type ` python manage.py
 setup_server` commend for fully setup into server . [How to Setup a Full Server
-with BigSansar, Django, and Ubuntu ](https://youtu.be/iEmI0HO_U0E) # some
+with BigSansar, Django, and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some
 usefull link [sitemap.xml](http://localhost/sitemap.xml) [script.js](http://
 localhost/script.js) [styles.css](http://localhost/styles.css) # how to edit
 sitemap , js and css from pages create a page **slug** name with sitemap,script
 , styles # How to change admin URL in server side with domain go to
 **VirtualHost.py** file and change **localhost** with your subdomain ## Some
 usefull commands: `python3 manage.py createuser` - get unlimited users. ##
 templatetags for extends and include {% extends '/.html' %} {% include '/.html'
```

### Comparing `Bigsansar-2.5.7/Bigsansar.egg-info/SOURCES.txt` & `bigsansar-2.5.8/Bigsansar.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,32 @@
 bigsansar/contrib/account/migrations/0001_initial.py
 bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
 bigsansar/contrib/account/migrations/__init__.py
 bigsansar/contrib/account/templates/__init__.py
 bigsansar/contrib/advance/__init__.py
 bigsansar/contrib/advance/admin.py
 bigsansar/contrib/advance/apps.py
+bigsansar/contrib/advance/cf_url.py
 bigsansar/contrib/advance/forms.py
 bigsansar/contrib/advance/models.py
 bigsansar/contrib/advance/tests.py
 bigsansar/contrib/advance/urls.py
 bigsansar/contrib/advance/views.py
 bigsansar/contrib/advance/migrations/0001_initial.py
 bigsansar/contrib/advance/migrations/0002_alter_css_options.py
 bigsansar/contrib/advance/migrations/0003_javascript.py
 bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
 bigsansar/contrib/advance/migrations/0005_delete_css.py
 bigsansar/contrib/advance/migrations/0006_delete_javascript.py
 bigsansar/contrib/advance/migrations/0007_initial.py
 bigsansar/contrib/advance/migrations/0008_sidebarsettings.py
 bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py
+bigsansar/contrib/advance/migrations/0010_cloudflare_api.py
+bigsansar/contrib/advance/migrations/0011_rename_account_global_api_key_cloudflare_api_global_api_key.py
+bigsansar/contrib/advance/migrations/0012_cloudflare_api_ip_address_cloudflare_api_ip_address2.py
 bigsansar/contrib/advance/migrations/__init__.py
 bigsansar/contrib/advance/templatetags/__init__.py
 bigsansar/contrib/advance/templatetags/nav_bar.py
 bigsansar/contrib/blogs/__init__.py
 bigsansar/contrib/blogs/admin.py
 bigsansar/contrib/blogs/apps.py
 bigsansar/contrib/blogs/forms.py
@@ -76,14 +80,15 @@
 bigsansar/contrib/sites/migrations/0004_alter_domains_default.py
 bigsansar/contrib/sites/migrations/0005_remove_domains_default.py
 bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py
 bigsansar/contrib/sites/migrations/0007_alter_default_domain_default_domain.py
 bigsansar/contrib/sites/migrations/0008_domains_primary_domain.py
 bigsansar/contrib/sites/migrations/0009_remove_default_domain_default_domain.py
 bigsansar/contrib/sites/migrations/0010_alter_domains_description.py
+bigsansar/contrib/sites/migrations/0011_domains_zone_id.py
 bigsansar/contrib/sites/migrations/__init__.py
 bigsansar/contrib/sites/templatetags/__init__.py
 bigsansar/contrib/sites/templatetags/pages.py
 bigsansar/core/__init__.py
 bigsansar/core/host.py
 bigsansar/core/init.py
 bigsansar/core/pip_package.py
@@ -140,16 +145,18 @@
 bigsansar/templates/defaultpage.html
 bigsansar/templates/parking.html
 bigsansar/templates/script.html
 bigsansar/templates/sitemap.html
 bigsansar/templates/styles.html
 bigsansar/templates/admin/account_info.html
 bigsansar/templates/admin/admin_update.html
+bigsansar/templates/admin/cf_config.html
 bigsansar/templates/admin/chpass.html
 bigsansar/templates/admin/chuname.html
+bigsansar/templates/admin/cloudflare.html
 bigsansar/templates/admin/create_domain.html
 bigsansar/templates/admin/domain_manage.html
 bigsansar/templates/admin/edit_domain.html
 bigsansar/templates/admin/editprofile.html
 bigsansar/templates/admin/login.html
 bigsansar/templates/admin/nav.html
 bigsansar/templates/admin/page_create.html
```

### Comparing `Bigsansar-2.5.7/LICENSE` & `bigsansar-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/PKG-INFO` & `bigsansar-2.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 2.5.7
+Version: 2.5.8
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://github.com/pokhrelb9/bigsansar
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
@@ -19,14 +19,15 @@
 Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: fontawesomefree
 
 ## New update
+* Working in to cloudflare 
 * fixed some bugs
 * added new db table for nav always open or close.
 * now you can install bigsansar package in to ubuntu and all setup with on command lines
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
@@ -63,15 +64,15 @@
 # for full setup in to server 
 
 this is work only on ubuntu os 
 
 2) type ` python manage.py setup_server` commend for fully setup into server .
 
 [How to Setup a Full Server with BigSansar, Django, and Ubuntu
-](https://youtu.be/iEmI0HO_U0E)
+](https://youtu.be/j8YN6x9XdR4)
 
 # some usefull link 
 [sitemap.xml](http://localhost/sitemap.xml)
 [script.js](http://localhost/script.js)
 [styles.css](http://localhost/styles.css)
 
 # how to edit sitemap , js and css from pages
```

#### html2text {}

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 2.5.7 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 2.5.8 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 github.com/pokhrelb9/bigsansar Author: Bikash Pokhrel Author-email:
 bigsansaroffice@gmail.com Project-URL: Bug Tracker, https://github.com/
 pokhrelb9/bigsansar/issues Project-URL: Documentations, https://
 docs.bigsansar.com/ Keywords: python,django host,bigsansar,django,django sites
 framework,django flatpages Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: OS Independent Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: django Requires-Dist: django-phonenumber-field[phonenumberslite]
 Requires-Dist: django-ckeditor Requires-Dist: requests Requires-Dist: pillow
-Requires-Dist: fontawesomefree ## New update * fixed some bugs * added new db
-table for nav always open or close. * now you can install bigsansar package in
-to ubuntu and all setup with on command lines # How to get Bigsansar Bigsansar
-is available open-source under the [MIT](https://en.wikipedia.org/wiki/
-MIT_License) license. We recommend using the latest version of Python 3.
-Bigsansar is Fully based on django and linux ubuntu. You can use [bigsansar]
-(https://bigsansar.com) for install packaged. You can use [bigsansar](https://
-bigsansar.com) for install packaged. view our tutorials in [youtube](https://
-youtube.com/bigsansar) for playlist: [bigsansar for django](https://
-www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the
-latest development version The latest and greatest Bigsasnar version is the one
-thatâs in our Git repository (our revision-control system). This is only for
-experienced users who want to try incoming changes and help identify bugs
-before an official release. Get it using this shell command, which requires
-[Git](https://https://git-scm.com/): `git clone https://github.com/pokhrelb9/
-bigsansar.git` You can also download a [gzipped tarball](https://https://
-pypi.org/project/Bigsansar/#files) of the development version. This archive is
-updated every time we commit code. # After you install bigsansar 1) Type
-`bigsansar init` command for **automatically** setup server for internal
+Requires-Dist: fontawesomefree ## New update * Working in to cloudflare * fixed
+some bugs * added new db table for nav always open or close. * now you can
+install bigsansar package in to ubuntu and all setup with on command lines #
+How to get Bigsansar Bigsansar is available open-source under the [MIT](https:/
+/en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
+version of Python 3. Bigsansar is Fully based on django and linux ubuntu. You
+can use [bigsansar](https://bigsansar.com) for install packaged. You can use
+[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
+[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
+(https://www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) #
+Get the latest development version The latest and greatest Bigsasnar version is
+the one thatâs in our Git repository (our revision-control system). This is
+only for experienced users who want to try incoming changes and help identify
+bugs before an official release. Get it using this shell command, which
+requires [Git](https://https://git-scm.com/): `git clone https://github.com/
+pokhrelb9/bigsansar.git` You can also download a [gzipped tarball](https://
+https://pypi.org/project/Bigsansar/#files) of the development version. This
+archive is updated every time we commit code. # After you install bigsansar 1)
+Type `bigsansar init` command for **automatically** setup server for internal
 configurations. ** this command valid into vertualenv for developer # for full
 setup in to server this is work only on ubuntu os 2) type ` python manage.py
 setup_server` commend for fully setup into server . [How to Setup a Full Server
-with BigSansar, Django, and Ubuntu ](https://youtu.be/iEmI0HO_U0E) # some
+with BigSansar, Django, and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some
 usefull link [sitemap.xml](http://localhost/sitemap.xml) [script.js](http://
 localhost/script.js) [styles.css](http://localhost/styles.css) # how to edit
 sitemap , js and css from pages create a page **slug** name with sitemap,script
 , styles # How to change admin URL in server side with domain go to
 **VirtualHost.py** file and change **localhost** with your subdomain ## Some
 usefull commands: `python3 manage.py createuser` - get unlimited users. ##
 templatetags for extends and include {% extends '/.html' %} {% include '/.html'
```

### Comparing `Bigsansar-2.5.7/README.md` & `bigsansar-2.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ## New update
+* Working in to cloudflare 
 * fixed some bugs
 * added new db table for nav always open or close.
 * now you can install bigsansar package in to ubuntu and all setup with on command lines
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
@@ -39,15 +40,15 @@
 # for full setup in to server 
 
 this is work only on ubuntu os 
 
 2) type ` python manage.py setup_server` commend for fully setup into server .
 
 [How to Setup a Full Server with BigSansar, Django, and Ubuntu
-](https://youtu.be/iEmI0HO_U0E)
+](https://youtu.be/j8YN6x9XdR4)
 
 # some usefull link 
 [sitemap.xml](http://localhost/sitemap.xml)
 [script.js](http://localhost/script.js)
 [styles.css](http://localhost/styles.css)
 
 # how to edit sitemap , js and css from pages
```

#### html2text {}

```diff
@@ -1,39 +1,39 @@
-## New update * fixed some bugs * added new db table for nav always open or
-close. * now you can install bigsansar package in to ubuntu and all setup with
-on command lines # How to get Bigsansar Bigsansar is available open-source
-under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We
-recommend using the latest version of Python 3. Bigsansar is Fully based on
-django and linux ubuntu. You can use [bigsansar](https://bigsansar.com) for
-install packaged. You can use [bigsansar](https://bigsansar.com) for install
-packaged. view our tutorials in [youtube](https://youtube.com/bigsansar) for
-playlist: [bigsansar for django](https://www.youtube.com/
-playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the latest development
-version The latest and greatest Bigsasnar version is the one thatâs in our
-Git repository (our revision-control system). This is only for experienced
-users who want to try incoming changes and help identify bugs before an
-official release. Get it using this shell command, which requires [Git](https:/
-/https://git-scm.com/): `git clone https://github.com/pokhrelb9/bigsansar.git`
-You can also download a [gzipped tarball](https://https://pypi.org/project/
-Bigsansar/#files) of the development version. This archive is updated every
-time we commit code. # After you install bigsansar 1) Type `bigsansar init`
-command for **automatically** setup server for internal configurations. ** this
-command valid into vertualenv for developer # for full setup in to server this
-is work only on ubuntu os 2) type ` python manage.py setup_server` commend for
-fully setup into server . [How to Setup a Full Server with BigSansar, Django,
-and Ubuntu ](https://youtu.be/iEmI0HO_U0E) # some usefull link [sitemap.xml]
-(http://localhost/sitemap.xml) [script.js](http://localhost/script.js)
-[styles.css](http://localhost/styles.css) # how to edit sitemap , js and css
-from pages create a page **slug** name with sitemap,script , styles # How to
-change admin URL in server side with domain go to **VirtualHost.py** file and
-change **localhost** with your subdomain ## Some usefull commands: `python3
-manage.py createuser` - get unlimited users. ## templatetags for extends and
-include {% extends '/.html' %} {% include '/.html' %} ## load blog list in
-templates `{% load blogs %} {% get_blog as bloglist %} {% for list in bloglist
-%}
+## New update * Working in to cloudflare * fixed some bugs * added new db table
+for nav always open or close. * now you can install bigsansar package in to
+ubuntu and all setup with on command lines # How to get Bigsansar Bigsansar is
+available open-source under the [MIT](https://en.wikipedia.org/wiki/
+MIT_License) license. We recommend using the latest version of Python 3.
+Bigsansar is Fully based on django and linux ubuntu. You can use [bigsansar]
+(https://bigsansar.com) for install packaged. You can use [bigsansar](https://
+bigsansar.com) for install packaged. view our tutorials in [youtube](https://
+youtube.com/bigsansar) for playlist: [bigsansar for django](https://
+www.youtube.com/playlist?list=PLbGzLu1WXrFUXw7qr6AMz5_iEkEAPV_Vs) # Get the
+latest development version The latest and greatest Bigsasnar version is the one
+thatâs in our Git repository (our revision-control system). This is only for
+experienced users who want to try incoming changes and help identify bugs
+before an official release. Get it using this shell command, which requires
+[Git](https://https://git-scm.com/): `git clone https://github.com/pokhrelb9/
+bigsansar.git` You can also download a [gzipped tarball](https://https://
+pypi.org/project/Bigsansar/#files) of the development version. This archive is
+updated every time we commit code. # After you install bigsansar 1) Type
+`bigsansar init` command for **automatically** setup server for internal
+configurations. ** this command valid into vertualenv for developer # for full
+setup in to server this is work only on ubuntu os 2) type ` python manage.py
+setup_server` commend for fully setup into server . [How to Setup a Full Server
+with BigSansar, Django, and Ubuntu ](https://youtu.be/j8YN6x9XdR4) # some
+usefull link [sitemap.xml](http://localhost/sitemap.xml) [script.js](http://
+localhost/script.js) [styles.css](http://localhost/styles.css) # how to edit
+sitemap , js and css from pages create a page **slug** name with sitemap,script
+, styles # How to change admin URL in server side with domain go to
+**VirtualHost.py** file and change **localhost** with your subdomain ## Some
+usefull commands: `python3 manage.py createuser` - get unlimited users. ##
+templatetags for extends and include {% extends '/.html' %} {% include '/.html'
+%} ## load blog list in templates `{% load blogs %} {% get_blog as bloglist %}
+{% for list in bloglist %}
 **** {{{{lliisstt..ttiittllee}}}} -- {{{{ lliisstt..ddoommaaiinn }}}} ****
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 _R_e_a_d_ _M_o_r_e
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
 { get_blog.publish_date }} {{ get_blog.domain }} {{ get_blog.id }} {
 { get_blog.slug }} {{ get_blog.body | safe }} {{ get_blog.visitor }} ` ## Count
```

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/account/forms.py` & `bigsansar-2.5.8/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/account/migrations/0001_initial.py` & `bigsansar-2.5.8/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/account/models.py` & `bigsansar-2.5.8/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0001_initial.py` & `bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0003_javascript.py` & `bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0007_initial.py` & `bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0007_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py` & `bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0008_sidebarsettings.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py` & `bigsansar-2.5.8/bigsansar/contrib/advance/migrations/0009_sidebarsettings_user.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/advance/templatetags/nav_bar.py` & `bigsansar-2.5.8/bigsansar/contrib/advance/templatetags/nav_bar.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/blogs/admin.py` & `bigsansar-2.5.8/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/blogs/migrations/0001_initial.py` & `bigsansar-2.5.8/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/blogs/models.py` & `bigsansar-2.5.8/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/blogs/templatetags/blogs.py` & `bigsansar-2.5.8/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/admin.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,7 +44,9 @@
             defaults['form'] = self.add_form
         defaults.update(kwargs)
         return super().get_form(request, obj, **defaults)
         
 
 
 admin.site.register(pages, pageadmin)
+
+admin.site.register(domains)
```

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/forms.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0001_initial.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0002_default_domain.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0002_default_domain.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/migrations/0006_default_domain_default_domain_and_more.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/models.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class domains(models.Model):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     domain = models.CharField(max_length=100, unique=True)
     Description = models.CharField(max_length=50, default=None)
     publish_date = models.DateField(auto_now_add=True)
     visitor = models.IntegerField(default=1)
     primary_domaIn = models.BooleanField(default=False)
-    
+    zone_id = models.CharField(max_length=1000, default='')
 
     def __str__(self):
         return self.domain
 
     class Meta:
         verbose_name = 'Domain'
         verbose_name_plural = 'Custom Domain'
```

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/urls.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/contrib/sites/views.py` & `bigsansar-2.5.8/bigsansar/contrib/sites/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/core/__init__.py` & `bigsansar-2.5.8/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/core/init.py` & `bigsansar-2.5.8/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/core/pip_package.py` & `bigsansar-2.5.8/bigsansar/core/pip_package.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/core/ubuntu.py` & `bigsansar-2.5.8/bigsansar/core/ubuntu.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,22 @@
                 os.makedirs('ssl')
                 
     else:
          print('already exit............')
 
     ssl_cert_snakeoil = 'ssl/ssl-cert-snakeoil.key'
     ssl_cert_pem = 'ssl/ssl-cert-snakeoil.pem'
+    ssl_req_csr = 'ssl/server.csr'
     full_url_for_cert_key = os.path.join(BASE_DIR, ssl_cert_snakeoil)
     get_pem_cert_url = os.path.join(BASE_DIR, ssl_cert_pem)
-    os.system('sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout %s -out %s' % (full_url_for_cert_key, get_pem_cert_url))
+    get_req_csr = os.path.join(BASE_DIR, ssl_req_csr)
+    os.system(f'sudo openssl genrsa -out {full_url_for_cert_key} 2048')
+    os.system(f'sudo openssl req -new -key server.key -out {get_req_csr}')
+    os.system(f'sudo openssl x509 -req -days 365 -in {get_req_csr} -signkey {full_url_for_cert_key} -out {get_pem_cert_url}')
+    #os.system('sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout %s -out %s' % (full_url_for_cert_key, get_pem_cert_url))
     os.system('sudo chown -R www-data %s && sudo chmod -R 775 %s' % (BASE_DIR, BASE_DIR))
 
     # for main setting of apache2
     lib_loc = site.getsitepackages()[0]
     
     # Construct the full path to the installed package directory
```

### Comparing `Bigsansar-2.5.7/bigsansar/etc/apache2.conf` & `bigsansar-2.5.8/bigsansar/etc/apache2.conf`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/etc/config_chroot.sh` & `bigsansar-2.5.8/bigsansar/etc/config_chroot.sh`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/etc/db.py` & `bigsansar-2.5.8/bigsansar/etc/db.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/etc/sshd_config` & `bigsansar-2.5.8/bigsansar/etc/sshd_config`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/management/commands/createuser.py` & `bigsansar-2.5.8/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/management/commands/setup_server.py` & `bigsansar-2.5.8/bigsansar/management/commands/setup_server.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `bigsansar-2.5.8/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/logo.png` & `bigsansar-2.5.8/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/static/style.css` & `bigsansar-2.5.8/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/404.html` & `bigsansar-2.5.8/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/account_info.html` & `bigsansar-2.5.8/bigsansar/templates/admin/account_info.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/admin_update.html` & `bigsansar-2.5.8/bigsansar/templates/admin/admin_update.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/chpass.html` & `bigsansar-2.5.8/bigsansar/templates/admin/chpass.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/chuname.html` & `bigsansar-2.5.8/bigsansar/templates/admin/chuname.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/create_domain.html` & `bigsansar-2.5.8/bigsansar/templates/admin/create_domain.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/domain_manage.html` & `bigsansar-2.5.8/bigsansar/templates/admin/domain_manage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/edit_domain.html` & `bigsansar-2.5.8/bigsansar/templates/admin/edit_domain.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/editprofile.html` & `bigsansar-2.5.8/bigsansar/templates/admin/editprofile.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/login.html` & `bigsansar-2.5.8/bigsansar/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/nav.html` & `bigsansar-2.5.8/bigsansar/templates/admin/nav.html`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
     hr {
    
     color: white;
 }
 
 .sidenav-menu-heading {
-    padding: 1.75rem 1rem 0.75rem;
-    font-size: 0.7rem;
+    padding: 0.05rem 1rem 0.05rem;
+    font-size: 0.75rem;
     font-weight: bold;
     text-transform: uppercase;
     letter-spacing: 0.05em;
     color: #fff;
 }
     </style>
 </head>
@@ -88,27 +88,28 @@
     
     {% domain_list_for_nav as domains %}
     {% for domains in domains %}
     <option value="/admin/domain/manage/{{ domains.id }}">{{ domains.domain }}</option>
     {% endfor %}
     </select>
     
-    <hr/>
     {% host_for_nav as per_domain %}
     {% if per_domain %}
-
+    <hr/>
     <a href="/admin/dashboard">Dashboard</a>
     <a href="/admin/changeuname">Change Username</a>
     <a href="">Settings</a>
 
-    {% else %}
-    <p>dfdfdsf</p>
-
     {% endif %}
     {% endif %}
+    {% if user.is_superuser %}
+    <hr/>
+    <div class="sidenav-menu-heading">Global Settings </div>
+    <a href="/admin/cf/">Cloudflare</a>
+    {% endif %}
 </div>
 
 <div id="main" class="content">
 <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
 
 	<div class="container-fluid">
 		{% if user.is_staff %}
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
 {% if user.is_staff %} {% load nav_bar %} {% post_is_sidebar_open %}
 {% csrf_token %}
 Websites
 ===============================================================================
 {% domain_list_for_nav as domains %} {% for domains in domains %}
 {{ domains.domain }}
 {% endfor %}
+{% host_for_nav as per_domain %} {% if per_domain %}
 ===============================================================================
-{% host_for_nav as per_domain %} {% if per_domain %} _D_a_s_h_b_o_a_r_d _C_h_a_n_g_e_ _U_s_e_r_n_a_m_e
-Settings {% else %}
-dfdfdsf
-{% endif %} {% endif %}
+_D_a_s_h_b_o_a_r_d _C_h_a_n_g_e_ _U_s_e_r_n_a_m_e Settings {% endif %} {% endif %} {% if
+user.is_superuser %}
+===============================================================================
+Global Settings
+_C_l_o_u_d_f_l_a_r_e {% endif %}
 {% if user.is_staff %}
 {% csrf_token %}
 {% else %} {% endif %} {% load static %}
 _B_I_G_S_A_N_S_A_R
 
       [Unknown INPUT type]Search
     * {% if user.is_authenticated %}
```

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/page_create.html` & `bigsansar-2.5.8/bigsansar/templates/admin/page_create.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/page_delete.html` & `bigsansar-2.5.8/bigsansar/templates/admin/page_delete.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/admin/page_edit.html` & `bigsansar-2.5.8/bigsansar/templates/admin/page_edit.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/base.html` & `bigsansar-2.5.8/bigsansar/templates/base.html`

 * *Files 20% similar despite different names*

```diff
@@ -20,20 +20,19 @@
     <link href="{% static 'fontawesomefree/css/solid.css' %}" rel="stylesheet" type="text/css">
 
 
         <title>{% block title %} Bigsansar - create your own site {% endblock %}</title>
 
         <!-- style for own customization -->
 
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor" crossorigin="anonymous">
-<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/js/bootstrap.bundle.min.js" integrity="sha384-pprn3073KE6tl6bjs2QrFaJGz5/SUsLqktiwsUTF55Jfv3qYSDhgCecCxMW52nD2" crossorigin="anonymous"></script>
-
+        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
+        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
         <!-- for head tag -->
 
-
+        
         {% block head %} {% endblock %}
 </head>
 <body>
 
 {% block body %} {% endblock %}
 </body>
 </html>
```

### Comparing `Bigsansar-2.5.7/bigsansar/templates/blog_preview.html` & `bigsansar-2.5.8/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/default.html` & `bigsansar-2.5.8/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/defaultpage.html` & `bigsansar-2.5.8/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/templates/parking.html` & `bigsansar-2.5.8/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/urls.py` & `bigsansar-2.5.8/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/bigsansar/views.py` & `bigsansar-2.5.8/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-2.5.7/setup.py` & `bigsansar-2.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="2.5.7",
+    version="2.5.8",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pokhrelb9/bigsansar",
     project_urls={
```

