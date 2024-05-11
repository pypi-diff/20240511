# Comparing `tmp/aa_drifters-0.4.2a0.tar.gz` & `tmp/aa_drifters-0.4.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_drifters-0.4.2a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_drifters-0.4.3a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_drifters-0.4.2a0.tar` & `aa_drifters-0.4.3a0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1069 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/LICENSE
--rw-r--r--   0        0        0     2419 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/README.md
--rw-r--r--   0        0        0      113 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/__init__.py
--rw-r--r--   0        0        0      705 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/admin.py
--rw-r--r--   0        0        0    10989 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/app_settings.py
--rw-r--r--   0        0        0     1015 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/auth_hooks.py
--rw-r--r--   0        0        0    16660 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/cogs/drifters.py
--rw-r--r--   0        0        0      953 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/forms.py
--rw-r--r--   0        0        0      400 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/locale/da_DK/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2267 2023-11-15 02:31:45.809410 aa_drifters-0.4.2a0/drifters/locale/da_DK/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      384 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2251 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3673 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2395 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4667 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2316 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2305 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2246 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2258 2023-11-15 02:31:45.810410 aa_drifters-0.4.2a0/drifters/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      523 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2390 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3101 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5364 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      399 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2266 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2480 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0001_initial.py
--rw-r--r--   0        0        0     1413 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0002_clear.py
--rw-r--r--   0        0        0      999 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0003_wormhole_archived_wormhole_archived_at_and_more.py
--rw-r--r--   0        0        0     1319 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0004_wormhole_bookmarked_k_wormhole_bookmarked_w_and_more.py
--rw-r--r--   0        0        0      616 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0005_alter_wormhole_archived_at_and_more.py
--rw-r--r--   0        0        0      831 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0006_alter_clear_system_alter_wormhole_system.py
--rw-r--r--   0        0        0     1151 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0007_alter_clear_options_driftersconfiguration.py
--rw-r--r--   0        0        0     3292 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0008_driftersconfiguration_motd_systems_and_more.py
--rw-r--r--   0        0        0      487 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0009_wormhole_reserved.py
--rw-r--r--   0        0        0    12222 2023-11-15 02:31:45.811410 aa_drifters-0.4.2a0/drifters/migrations/0010_general_alter_wormhole_eol_changed_at_and_more.py
--rw-r--r--   0        0        0        0 2023-11-15 02:31:45.840410 aa_drifters-0.4.2a0/drifters/migrations/__init__.py
--rw-r--r--   0        0        0    10356 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/models.py
--rw-r--r--   0        0        0      906 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/routing.py
--rw-r--r--   0        0        0      755 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/tasks.py
--rw-r--r--   0        0        0     1634 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/base.html
--rw-r--r--   0        0        0     1068 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/blocks/complex.html
--rw-r--r--   0        0        0     1249 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/blocks/wormhole.html
--rw-r--r--   0        0        0      217 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/index.html
--rw-r--r--   0        0        0     1226 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/motd.html
--rw-r--r--   0        0        0     1257 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/scout/blocks/scout_complex.html
--rw-r--r--   0        0        0     1259 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/scout/blocks/scout_region.html
--rw-r--r--   0        0        0      204 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/scout/blocks/scout_system.html
--rw-r--r--   0        0        0      329 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/scout/index.html
--rw-r--r--   0        0        0      647 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/scout/scout_complex.html
--rw-r--r--   0        0        0      416 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templates/drifters/scout/scout_region.html
--rw-r--r--   0        0        0        0 2023-11-15 02:31:45.841410 aa_drifters-0.4.2a0/drifters/templatetags/__init__.py
--rw-r--r--   0        0        0      587 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/templatetags/drifters.py
--rw-r--r--   0        0        0      391 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/urls.py
--rw-r--r--   0        0        0    10447 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/drifters/views.py
--rw-r--r--   0        0        0     2022 2023-11-15 02:31:45.812410 aa_drifters-0.4.2a0/pyproject.toml
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 aa_drifters-0.4.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/LICENSE
+-rw-r--r--   0        0        0     2419 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/README.md
+-rw-r--r--   0        0        0      113 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/drifters/__init__.py
+-rw-r--r--   0        0        0      705 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/drifters/admin.py
+-rw-r--r--   0        0        0    10989 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/drifters/app_settings.py
+-rw-r--r--   0        0        0     1015 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/drifters/auth_hooks.py
+-rw-r--r--   0        0        0    16660 2024-05-11 11:07:51.650077 aa_drifters-0.4.3a0/drifters/cogs/drifters.py
+-rw-r--r--   0        0        0      953 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/forms.py
+-rw-r--r--   0        0        0      400 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/locale/da_DK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2267 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/locale/da_DK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      739 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3825 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3675 2024-05-11 11:07:51.651077 aa_drifters-0.4.3a0/drifters/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2423 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4669 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2316 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2305 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2246 2024-05-11 11:07:51.652077 aa_drifters-0.4.3a0/drifters/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2258 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      523 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2390 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3120 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5366 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      399 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2266 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2480 2024-05-11 11:07:51.653077 aa_drifters-0.4.3a0/drifters/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1413 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0002_clear.py
+-rw-r--r--   0        0        0      999 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0003_wormhole_archived_wormhole_archived_at_and_more.py
+-rw-r--r--   0        0        0     1319 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0004_wormhole_bookmarked_k_wormhole_bookmarked_w_and_more.py
+-rw-r--r--   0        0        0      616 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0005_alter_wormhole_archived_at_and_more.py
+-rw-r--r--   0        0        0      831 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0006_alter_clear_system_alter_wormhole_system.py
+-rw-r--r--   0        0        0     1151 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0007_alter_clear_options_driftersconfiguration.py
+-rw-r--r--   0        0        0     3292 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0008_driftersconfiguration_motd_systems_and_more.py
+-rw-r--r--   0        0        0      487 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0009_wormhole_reserved.py
+-rw-r--r--   0        0        0    12222 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0010_general_alter_wormhole_eol_changed_at_and_more.py
+-rw-r--r--   0        0        0      480 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/migrations/0011_alter_wormhole_managers.py
+-rw-r--r--   0        0        0        0 2024-05-11 11:07:51.690077 aa_drifters-0.4.3a0/drifters/migrations/__init__.py
+-rw-r--r--   0        0        0    10356 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/models.py
+-rw-r--r--   0        0        0      906 2024-05-11 11:07:51.654077 aa_drifters-0.4.3a0/drifters/routing.py
+-rw-r--r--   0        0        0      755 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/tasks.py
+-rw-r--r--   0        0        0     1634 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/base.html
+-rw-r--r--   0        0        0     1068 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/blocks/complex.html
+-rw-r--r--   0        0        0     1249 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/blocks/wormhole.html
+-rw-r--r--   0        0        0      217 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/index.html
+-rw-r--r--   0        0        0     1226 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/motd.html
+-rw-r--r--   0        0        0     1257 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/scout/blocks/scout_complex.html
+-rw-r--r--   0        0        0     1259 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/scout/blocks/scout_region.html
+-rw-r--r--   0        0        0      204 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/scout/blocks/scout_system.html
+-rw-r--r--   0        0        0      329 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/scout/index.html
+-rw-r--r--   0        0        0      647 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/scout/scout_complex.html
+-rw-r--r--   0        0        0      416 2024-05-11 11:07:51.655077 aa_drifters-0.4.3a0/drifters/templates/drifters/scout/scout_region.html
+-rw-r--r--   0        0        0        0 2024-05-11 11:07:51.692077 aa_drifters-0.4.3a0/drifters/templatetags/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-11 11:07:51.656077 aa_drifters-0.4.3a0/drifters/templatetags/drifters.py
+-rw-r--r--   0        0        0      391 2024-05-11 11:07:51.656077 aa_drifters-0.4.3a0/drifters/urls.py
+-rw-r--r--   0        0        0    10447 2024-05-11 11:07:51.656077 aa_drifters-0.4.3a0/drifters/views.py
+-rw-r--r--   0        0        0     2102 2024-05-11 11:07:51.656077 aa_drifters-0.4.3a0/pyproject.toml
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 aa_drifters-0.4.3a0/PKG-INFO
```

### Comparing `aa_drifters-0.4.2a0/LICENSE` & `aa_drifters-0.4.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/README.md` & `aa_drifters-0.4.3a0/README.md`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/admin.py` & `aa_drifters-0.4.3a0/drifters/admin.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/app_settings.py` & `aa_drifters-0.4.3a0/drifters/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/auth_hooks.py` & `aa_drifters-0.4.3a0/drifters/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/cogs/drifters.py` & `aa_drifters-0.4.3a0/drifters/cogs/drifters.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/forms.py` & `aa_drifters-0.4.3a0/drifters/forms.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/da_DK/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/da_DK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/de/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-05-31 12:59+1000\n"
 "PO-Revision-Date: 2023-05-31 03:17+0000\n"
-"Language-Team: German (https://app.transifex.com/alliance-auth/teams/107430/de/)\n"
+"Language-Team: Korean (Korea) (https://app.transifex.com/alliance-auth/teams/107430/ko_KR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ko_KR\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: drifters/models.py:16
 msgid "Barbican"
 msgstr ""
 
 #: drifters/models.py:17
 msgid "Conflux"
```

### Comparing `aa_drifters-0.4.2a0/drifters/locale/en/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,166 +1,169 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
+# Translators:
+# Peter Pfeufer, 2023
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 21:57+1000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-05-11 20:57+1000\n"
+"PO-Revision-Date: 2023-10-08 10:25+0000\n"
+"Last-Translator: Peter Pfeufer, 2023\n"
+"Language-Team: German (https://app.transifex.com/alliance-auth/teams/107430/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: drifters/auth_hooks.py:21 drifters/templates/drifters/base.html:6
 #: drifters/templates/drifters/base.html:23
 msgid "Drifters"
 msgstr ""
 
-#: drifters/models.py:38
+#: drifters/models.py:43
 msgid "Barbican"
-msgstr ""
+msgstr "Barbican"
 
-#: drifters/models.py:39
+#: drifters/models.py:44
 msgid "Conflux"
-msgstr ""
+msgstr "Conflux"
 
-#: drifters/models.py:40
+#: drifters/models.py:45
 msgid "Redoubt"
-msgstr ""
+msgstr "Redoubt"
 
-#: drifters/models.py:41
+#: drifters/models.py:46
 msgid "Sentinel"
-msgstr ""
+msgstr "Sentinel"
 
-#: drifters/models.py:42
+#: drifters/models.py:47
 msgid "Vidette"
-msgstr ""
+msgstr "Vidette"
 
-#: drifters/models.py:43
+#: drifters/models.py:48
 msgid "Thera"
 msgstr ""
 
-#: drifters/models.py:44
+#: drifters/models.py:49
 msgid "Turnur"
 msgstr ""
 
-#: drifters/models.py:51
+#: drifters/models.py:56
 msgid ""
-"This wormhole has not yet had its stability significantly disrupted by ships "
-"passing through it"
+"This wormhole has not yet had its stability significantly disrupted by ships"
+" passing through it"
 msgstr ""
 
-#: drifters/models.py:53
+#: drifters/models.py:58
 msgid ""
-"This wormhole has had its stability reduced by ships passing through it, but "
-"not to a critical degree yet"
+"This wormhole has had its stability reduced by ships passing through it, but"
+" not to a critical degree yet"
 msgstr ""
 
-#: drifters/models.py:55
+#: drifters/models.py:60
 msgid ""
 "This wormhole has had its stability critically disrupted by the mass of "
 "numerous ships passing through and is on the verge of collapse"
 msgstr ""
 
-#: drifters/models.py:62
+#: drifters/models.py:67
 msgid ""
 "This wormhole has not yet begun its natural cycle of decay and should last "
 "at least another day"
 msgstr ""
 
-#: drifters/models.py:64
+#: drifters/models.py:69
 msgid ""
 "This wormhole is beginning to decay, and probably won't last another day"
 msgstr ""
 
-#: drifters/models.py:65
+#: drifters/models.py:70
 msgid "This wormhole is reaching the end of its natural lifetime"
 msgstr ""
 
-#: drifters/models.py:67 drifters/models.py:188
+#: drifters/models.py:72 drifters/models.py:218
 msgid "Solar System"
-msgstr ""
+msgstr "Sonnensystem"
 
-#: drifters/models.py:68
+#: drifters/models.py:73
 msgid "Complex"
 msgstr ""
 
-#: drifters/models.py:69
+#: drifters/models.py:74
 msgid "Mass Remaining"
 msgstr ""
 
-#: drifters/models.py:70
+#: drifters/models.py:75
 msgid "K Space Bookmarked"
 msgstr ""
 
-#: drifters/models.py:71
+#: drifters/models.py:76
 msgid "W Space Bookmarked"
 msgstr ""
 
-#: drifters/models.py:73
+#: drifters/models.py:78
 msgid "Lifetime Remaining"
 msgstr ""
 
-#: drifters/models.py:78 drifters/models.py:192
+#: drifters/models.py:83 drifters/models.py:222
 msgid "Created By User"
 msgstr ""
 
-#: drifters/models.py:82
+#: drifters/models.py:87
 msgid "Update By User"
 msgstr ""
 
-#: drifters/models.py:84
+#: drifters/models.py:89
 msgid "Archived"
 msgstr ""
 
-#: drifters/models.py:85
+#: drifters/models.py:90
 msgid "Not Published / Reserved for Fleets and WH Team Usage"
 msgstr ""
 
-#: drifters/models.py:88
+#: drifters/models.py:93
 msgid "Archived By User"
 msgstr ""
 
-#: drifters/models.py:91
+#: drifters/models.py:100
 msgid "Wormhole"
-msgstr ""
+msgstr "Wurmloch"
 
-#: drifters/models.py:92
+#: drifters/models.py:101
 msgid "Wormholes"
-msgstr ""
+msgstr "Wurmlöcher"
 
-#: drifters/models.py:196
+#: drifters/models.py:226
 msgid "Updated By User"
 msgstr ""
 
-#: drifters/models.py:199
+#: drifters/models.py:229
 msgid "Clear System"
 msgstr ""
 
-#: drifters/models.py:200
+#: drifters/models.py:230
 msgid "Clear Systems"
 msgstr ""
 
-#: drifters/models.py:215
+#: drifters/models.py:245
 msgid "POI Regions to be highlighted in the Web UI"
 msgstr ""
 
-#: drifters/models.py:216
+#: drifters/models.py:246
 msgid "POI Systems to be highlighted in the Web UI"
 msgstr ""
 
-#: drifters/models.py:217
+#: drifters/models.py:247
 msgid "Systems to be included in the MOTD Generation"
 msgstr ""
 
 #: drifters/templates/drifters/base.html:18
 msgid "Toggle navigation"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_drifters-0.4.2a0/drifters/locale/es/LC_MESSAGES/django.mo` & `aa_drifters-0.4.3a0/drifters/locale/es/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-05-31 03:17+0000\n"
-"Last-Translator: trenus, 2023\n"
+"PO-Revision-Date: 2023-10-08 10:25+0000\n"
+"Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2023\n"
 "Language-Team: Spanish (https://app.transifex.com/alliance-auth/teams/107430/"
 "es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
```

### Comparing `aa_drifters-0.4.2a0/drifters/locale/es/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,173 +7,173 @@
 # Joel Falknau <ozirascal@gmail.com>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 21:57+1000\n"
+"POT-Creation-Date: 2024-05-11 20:57+1000\n"
 "PO-Revision-Date: 2023-10-08 10:25+0000\n"
 "Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2023\n"
 "Language-Team: Spanish (https://app.transifex.com/alliance-auth/teams/107430/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: drifters/auth_hooks.py:21 drifters/templates/drifters/base.html:6
 #: drifters/templates/drifters/base.html:23
 msgid "Drifters"
 msgstr ""
 
-#: drifters/models.py:38
+#: drifters/models.py:43
 msgid "Barbican"
 msgstr "Barbican"
 
-#: drifters/models.py:39
+#: drifters/models.py:44
 msgid "Conflux"
 msgstr "Conflux"
 
-#: drifters/models.py:40
+#: drifters/models.py:45
 msgid "Redoubt"
 msgstr "Redoubt"
 
-#: drifters/models.py:41
+#: drifters/models.py:46
 msgid "Sentinel"
 msgstr "Sentinel"
 
-#: drifters/models.py:42
+#: drifters/models.py:47
 msgid "Vidette"
 msgstr "Vidette"
 
-#: drifters/models.py:43
+#: drifters/models.py:48
 msgid "Thera"
 msgstr ""
 
-#: drifters/models.py:44
+#: drifters/models.py:49
 msgid "Turnur"
 msgstr ""
 
-#: drifters/models.py:51
+#: drifters/models.py:56
 msgid ""
 "This wormhole has not yet had its stability significantly disrupted by ships"
 " passing through it"
 msgstr ""
 "La estabilidad de este agujero de gusano no se ha visto significativamente "
 "alterada por las naves que lo atraviesan"
 
-#: drifters/models.py:53
+#: drifters/models.py:58
 msgid ""
 "This wormhole has had its stability reduced by ships passing through it, but"
 " not to a critical degree yet"
 msgstr ""
 "La estabilidad de este agujero de gusano ha disminuido por las naves que lo "
 "cruzan, pero aún no ha alcanzado un punto crítico"
 
-#: drifters/models.py:55
+#: drifters/models.py:60
 msgid ""
 "This wormhole has had its stability critically disrupted by the mass of "
 "numerous ships passing through and is on the verge of collapse"
 msgstr ""
 "La estabilidad de este agujero de gusano se ha visto gravemente alterada por"
 " la masa de numerosas naves que lo atraviesan y está al borde del colapso."
 
-#: drifters/models.py:62
+#: drifters/models.py:67
 msgid ""
 "This wormhole has not yet begun its natural cycle of decay and should last "
 "at least another day"
 msgstr ""
 "Este agujero de gusano aun no empieza su ciclo natural de deterioro y "
 "debería durar al menos otro día"
 
-#: drifters/models.py:64
+#: drifters/models.py:69
 msgid ""
 "This wormhole is beginning to decay, and probably won't last another day"
 msgstr ""
 "Este agujero de gusano empieza a deteriorarse y probablemente no durará otro"
 " día"
 
-#: drifters/models.py:65
+#: drifters/models.py:70
 msgid "This wormhole is reaching the end of its natural lifetime"
 msgstr "Este agujero de gusano está llegando al final de su vida útil"
 
-#: drifters/models.py:67 drifters/models.py:188
+#: drifters/models.py:72 drifters/models.py:218
 msgid "Solar System"
 msgstr ""
 
-#: drifters/models.py:68
+#: drifters/models.py:73
 msgid "Complex"
 msgstr "Complejo"
 
-#: drifters/models.py:69
+#: drifters/models.py:74
 msgid "Mass Remaining"
 msgstr "Masa restante"
 
-#: drifters/models.py:70
+#: drifters/models.py:75
 msgid "K Space Bookmarked"
 msgstr "Espacio K marcado"
 
-#: drifters/models.py:71
+#: drifters/models.py:76
 msgid "W Space Bookmarked"
 msgstr "Espacio W marcado"
 
-#: drifters/models.py:73
+#: drifters/models.py:78
 msgid "Lifetime Remaining"
 msgstr "Tiempo de vida restante"
 
-#: drifters/models.py:78 drifters/models.py:192
+#: drifters/models.py:83 drifters/models.py:222
 msgid "Created By User"
 msgstr ""
 
-#: drifters/models.py:82
+#: drifters/models.py:87
 msgid "Update By User"
 msgstr ""
 
-#: drifters/models.py:84
+#: drifters/models.py:89
 msgid "Archived"
 msgstr "Archivado"
 
-#: drifters/models.py:85
+#: drifters/models.py:90
 msgid "Not Published / Reserved for Fleets and WH Team Usage"
 msgstr ""
 
-#: drifters/models.py:88
+#: drifters/models.py:93
 msgid "Archived By User"
 msgstr ""
 
-#: drifters/models.py:91
+#: drifters/models.py:100
 msgid "Wormhole"
 msgstr "Agujero de gusano"
 
-#: drifters/models.py:92
+#: drifters/models.py:101
 msgid "Wormholes"
 msgstr "Agujeros de Gusano"
 
-#: drifters/models.py:196
+#: drifters/models.py:226
 msgid "Updated By User"
 msgstr ""
 
-#: drifters/models.py:199
+#: drifters/models.py:229
 msgid "Clear System"
 msgstr ""
 
-#: drifters/models.py:200
+#: drifters/models.py:230
 msgid "Clear Systems"
 msgstr ""
 
-#: drifters/models.py:215
+#: drifters/models.py:245
 msgid "POI Regions to be highlighted in the Web UI"
 msgstr ""
 
-#: drifters/models.py:216
+#: drifters/models.py:246
 msgid "POI Systems to be highlighted in the Web UI"
 msgstr ""
 
-#: drifters/models.py:217
+#: drifters/models.py:247
 msgid "Systems to be included in the MOTD Generation"
 msgstr ""
 
 #: drifters/templates/drifters/base.html:18
 msgid "Toggle navigation"
 msgstr ""
```

### Comparing `aa_drifters-0.4.2a0/drifters/locale/fr_FR/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/it_IT/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/ja/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/ko_KR/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-05-31 12:59+1000\n"
 "PO-Revision-Date: 2023-05-31 03:17+0000\n"
-"Language-Team: Korean (Korea) (https://app.transifex.com/alliance-auth/teams/107430/ko_KR/)\n"
+"Language-Team: Chinese Simplified (https://app.transifex.com/alliance-auth/teams/107430/zh-Hans/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ko_KR\n"
+"Language: zh-Hans\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: drifters/models.py:16
 msgid "Barbican"
 msgstr ""
 
 #: drifters/models.py:17
```

### Comparing `aa_drifters-0.4.2a0/drifters/locale/ru/LC_MESSAGES/django.mo` & `aa_drifters-0.4.3a0/drifters/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/ru/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/locale/uk/LC_MESSAGES/django.mo` & `aa_drifters-0.4.3a0/drifters/locale/uk/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-05-31 03:17+0000\n"
-"Last-Translator: Kristof Swensen, 2023\n"
+"PO-Revision-Date: 2023-10-08 10:25+0000\n"
+"Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2023\n"
 "Language-Team: Ukrainian (https://app.transifex.com/alliance-auth/"
 "teams/107430/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
```

### Comparing `aa_drifters-0.4.2a0/drifters/locale/uk/LC_MESSAGES/django.po` & `aa_drifters-0.4.3a0/drifters/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,173 +7,173 @@
 # Joel Falknau <ozirascal@gmail.com>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 21:57+1000\n"
+"POT-Creation-Date: 2024-05-11 20:57+1000\n"
 "PO-Revision-Date: 2023-10-08 10:25+0000\n"
 "Last-Translator: Joel Falknau <ozirascal@gmail.com>, 2023\n"
 "Language-Team: Ukrainian (https://app.transifex.com/alliance-auth/teams/107430/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: drifters/auth_hooks.py:21 drifters/templates/drifters/base.html:6
 #: drifters/templates/drifters/base.html:23
 msgid "Drifters"
 msgstr ""
 
-#: drifters/models.py:38
+#: drifters/models.py:43
 msgid "Barbican"
 msgstr "Barbican"
 
-#: drifters/models.py:39
+#: drifters/models.py:44
 msgid "Conflux"
 msgstr "Conflux"
 
-#: drifters/models.py:40
+#: drifters/models.py:45
 msgid "Redoubt"
 msgstr "Redoubt"
 
-#: drifters/models.py:41
+#: drifters/models.py:46
 msgid "Sentinel"
 msgstr "Sentinel"
 
-#: drifters/models.py:42
+#: drifters/models.py:47
 msgid "Vidette"
 msgstr "Vidette"
 
-#: drifters/models.py:43
+#: drifters/models.py:48
 msgid "Thera"
 msgstr ""
 
-#: drifters/models.py:44
+#: drifters/models.py:49
 msgid "Turnur"
 msgstr ""
 
-#: drifters/models.py:51
+#: drifters/models.py:56
 msgid ""
 "This wormhole has not yet had its stability significantly disrupted by ships"
 " passing through it"
 msgstr ""
 "Ця червоточина ще не зазнала суттєвого порушення стабільності від кораблів, "
 "що проходили через неї."
 
-#: drifters/models.py:53
+#: drifters/models.py:58
 msgid ""
 "This wormhole has had its stability reduced by ships passing through it, but"
 " not to a critical degree yet"
 msgstr ""
 "Ця червоточина отримала зниження стабільності від кораблів, що проходили "
 "через неї, але ще не до критичного ступеня."
 
-#: drifters/models.py:55
+#: drifters/models.py:60
 msgid ""
 "This wormhole has had its stability critically disrupted by the mass of "
 "numerous ships passing through and is on the verge of collapse"
 msgstr ""
 "Стабільність цієї червоточини була критично порушена масою численних "
 "кораблів, які проходили через неї, і вона на межі руйнування."
 
-#: drifters/models.py:62
+#: drifters/models.py:67
 msgid ""
 "This wormhole has not yet begun its natural cycle of decay and should last "
 "at least another day"
 msgstr ""
 "Ця червоточина ще не розпочала свій природний цикл розпаду і повинна "
 "існувати щонайменше ще один день."
 
-#: drifters/models.py:64
+#: drifters/models.py:69
 msgid ""
 "This wormhole is beginning to decay, and probably won't last another day"
 msgstr ""
 "Ця червоточина починає розпадатися і, ймовірно, не протримається і дня."
 
-#: drifters/models.py:65
+#: drifters/models.py:70
 msgid "This wormhole is reaching the end of its natural lifetime"
 msgstr ""
 "Ця червоточина наближається до завершення свого природного життєвого циклу."
 
-#: drifters/models.py:67 drifters/models.py:188
+#: drifters/models.py:72 drifters/models.py:218
 msgid "Solar System"
 msgstr ""
 
-#: drifters/models.py:68
+#: drifters/models.py:73
 msgid "Complex"
 msgstr "Комплекс"
 
-#: drifters/models.py:69
+#: drifters/models.py:74
 msgid "Mass Remaining"
 msgstr "Залишкова маса"
 
-#: drifters/models.py:70
+#: drifters/models.py:75
 msgid "K Space Bookmarked"
 msgstr "Закладки K-Space"
 
-#: drifters/models.py:71
+#: drifters/models.py:76
 msgid "W Space Bookmarked"
 msgstr "Закладки W-Space"
 
-#: drifters/models.py:73
+#: drifters/models.py:78
 msgid "Lifetime Remaining"
 msgstr "Залишок життя"
 
-#: drifters/models.py:78 drifters/models.py:192
+#: drifters/models.py:83 drifters/models.py:222
 msgid "Created By User"
 msgstr ""
 
-#: drifters/models.py:82
+#: drifters/models.py:87
 msgid "Update By User"
 msgstr ""
 
-#: drifters/models.py:84
+#: drifters/models.py:89
 msgid "Archived"
 msgstr "Архівовано"
 
-#: drifters/models.py:85
+#: drifters/models.py:90
 msgid "Not Published / Reserved for Fleets and WH Team Usage"
 msgstr ""
 
-#: drifters/models.py:88
+#: drifters/models.py:93
 msgid "Archived By User"
 msgstr ""
 
-#: drifters/models.py:91
+#: drifters/models.py:100
 msgid "Wormhole"
 msgstr "Червоточина"
 
-#: drifters/models.py:92
+#: drifters/models.py:101
 msgid "Wormholes"
 msgstr "Червоточини"
 
-#: drifters/models.py:196
+#: drifters/models.py:226
 msgid "Updated By User"
 msgstr ""
 
-#: drifters/models.py:199
+#: drifters/models.py:229
 msgid "Clear System"
 msgstr ""
 
-#: drifters/models.py:200
+#: drifters/models.py:230
 msgid "Clear Systems"
 msgstr ""
 
-#: drifters/models.py:215
+#: drifters/models.py:245
 msgid "POI Regions to be highlighted in the Web UI"
 msgstr ""
 
-#: drifters/models.py:216
+#: drifters/models.py:246
 msgid "POI Systems to be highlighted in the Web UI"
 msgstr ""
 
-#: drifters/models.py:217
+#: drifters/models.py:247
 msgid "Systems to be included in the MOTD Generation"
 msgstr ""
 
 #: drifters/templates/drifters/base.html:18
 msgid "Toggle navigation"
 msgstr ""
```

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0001_initial.py` & `aa_drifters-0.4.3a0/drifters/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0002_clear.py` & `aa_drifters-0.4.3a0/drifters/migrations/0002_clear.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0003_wormhole_archived_wormhole_archived_at_and_more.py` & `aa_drifters-0.4.3a0/drifters/migrations/0003_wormhole_archived_wormhole_archived_at_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0004_wormhole_bookmarked_k_wormhole_bookmarked_w_and_more.py` & `aa_drifters-0.4.3a0/drifters/migrations/0004_wormhole_bookmarked_k_wormhole_bookmarked_w_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0005_alter_wormhole_archived_at_and_more.py` & `aa_drifters-0.4.3a0/drifters/migrations/0005_alter_wormhole_archived_at_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0006_alter_clear_system_alter_wormhole_system.py` & `aa_drifters-0.4.3a0/drifters/migrations/0006_alter_clear_system_alter_wormhole_system.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0007_alter_clear_options_driftersconfiguration.py` & `aa_drifters-0.4.3a0/drifters/migrations/0007_alter_clear_options_driftersconfiguration.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0008_driftersconfiguration_motd_systems_and_more.py` & `aa_drifters-0.4.3a0/drifters/migrations/0008_driftersconfiguration_motd_systems_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/migrations/0010_general_alter_wormhole_eol_changed_at_and_more.py` & `aa_drifters-0.4.3a0/drifters/migrations/0010_general_alter_wormhole_eol_changed_at_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/models.py` & `aa_drifters-0.4.3a0/drifters/models.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/routing.py` & `aa_drifters-0.4.3a0/drifters/routing.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/tasks.py` & `aa_drifters-0.4.3a0/drifters/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/base.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/base.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/blocks/complex.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/blocks/complex.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/blocks/wormhole.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/blocks/wormhole.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/motd.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/motd.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/scout/blocks/scout_complex.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/scout/blocks/scout_complex.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/scout/blocks/scout_region.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/scout/blocks/scout_region.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templates/drifters/scout/scout_complex.html` & `aa_drifters-0.4.3a0/drifters/templates/drifters/scout/scout_complex.html`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/templatetags/drifters.py` & `aa_drifters-0.4.3a0/drifters/templatetags/drifters.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/drifters/views.py` & `aa_drifters-0.4.3a0/drifters/views.py`

 * *Files identical despite different names*

### Comparing `aa_drifters-0.4.2a0/pyproject.toml` & `aa_drifters-0.4.3a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     "eveonline",
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Celery",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content"
 ]
 dependencies = [
     "allianceauth>=3.0.0,<5.0.0",
     "django-eveuniverse",
```

### Comparing `aa_drifters-0.4.2a0/PKG-INFO` & `aa_drifters-0.4.3a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: aa_drifters
-Version: 0.4.2a0
+Version: 0.4.3a0
 Summary: Drifter wormhole tracker/manager plugin for Alliance Auth.
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: allianceauth>=3.0.0,<5.0.0
 Requires-Dist: django-eveuniverse
 Requires-Dist: django-solo>=2.0.0,<3.0.0
 Requires-Dist: py-cord>=2.0.0,<3.0.0
```

