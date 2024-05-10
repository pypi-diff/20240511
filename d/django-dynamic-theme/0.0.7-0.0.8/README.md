# Comparing `tmp/django_dynamic_theme-0.0.7.tar.gz` & `tmp/django_dynamic_theme-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_theme-0.0.7.tar", max compression
+gzip compressed data, was "django_dynamic_theme-0.0.8.tar", max compression
```

## Comparing `django_dynamic_theme-0.0.7.tar` & `django_dynamic_theme-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1068 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/LICENSE
--rw-r--r--   0        0        0     1738 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/admin.py
--rw-r--r--   0        0        0      498 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/apps.py
--rw-r--r--   0        0        0      475 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/context_processor.py
--rw-r--r--   0        0        0      141 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/errors.py
--rw-r--r--   0        0        0     1243 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/middleware.py
--rw-r--r--   0        0        0      516 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0001_initial.py
--rw-r--r--   0        0        0      436 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0002_background_name.py
--rw-r--r--   0        0        0      484 2024-05-04 17:46:14.443807 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
--rw-r--r--   0        0        0     1241 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
--rw-r--r--   0        0        0      733 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
--rw-r--r--   0        0        0      526 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0006_alter_theme_background.py
--rw-r--r--   0        0        0      664 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
--rw-r--r--   0        0        0      434 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0008_alter_theme_default.py
--rw-r--r--   0        0        0      976 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0009_navbar.py
--rw-r--r--   0        0        0      507 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0010_theme_navbar.py
--rw-r--r--   0        0        0      612 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0011_navbar_font_size.py
--rw-r--r--   0        0        0      479 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0012_navbar_text_color.py
--rw-r--r--   0        0        0      566 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
--rw-r--r--   0        0        0      604 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
--rw-r--r--   0        0        0      940 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0015_mediagallery.py
--rw-r--r--   0        0        0      529 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0016_theme_media_gallery.py
--rw-r--r--   0        0        0        0 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/__init__.py
--rw-r--r--   0        0        0     6297 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/models.py
--rw-r--r--   0        0        0      582 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/signals.py
--rw-r--r--   0        0        0        0 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/utill/__init__.py
--rw-r--r--   0        0        0      506 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/utill/color_converter.py
--rw-r--r--   0        0        0      740 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/django_dynamic_theme/utill/scss_editor.py
--rw-r--r--   0        0        0      743 2024-05-04 17:46:14.447808 django_dynamic_theme-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1830 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/admin.py
+-rw-r--r--   0        0        0      498 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/apps.py
+-rw-r--r--   0        0        0      475 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/context_processor.py
+-rw-r--r--   0        0        0      292 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/errors.py
+-rw-r--r--   0        0        0     1243 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/middleware.py
+-rw-r--r--   0        0        0      516 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0001_initial.py
+-rw-r--r--   0        0        0      436 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0002_background_name.py
+-rw-r--r--   0        0        0      484 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0003_alter_background_primary_bg.py
+-rw-r--r--   0        0        0     1241 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py
+-rw-r--r--   0        0        0      733 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py
+-rw-r--r--   0        0        0      526 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0006_alter_theme_background.py
+-rw-r--r--   0        0        0      664 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py
+-rw-r--r--   0        0        0      434 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0008_alter_theme_default.py
+-rw-r--r--   0        0        0      976 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0009_navbar.py
+-rw-r--r--   0        0        0      507 2024-05-10 23:28:48.275073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0010_theme_navbar.py
+-rw-r--r--   0        0        0      612 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0011_navbar_font_size.py
+-rw-r--r--   0        0        0      479 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0012_navbar_text_color.py
+-rw-r--r--   0        0        0      566 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0013_navbar_text_opacity.py
+-rw-r--r--   0        0        0      604 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py
+-rw-r--r--   0        0        0      940 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0015_mediagallery.py
+-rw-r--r--   0        0        0      529 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0016_theme_media_gallery.py
+-rw-r--r--   0        0        0      704 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0017_alter_mediagallery_options_alter_theme_navbar.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/__init__.py
+-rw-r--r--   0        0        0     6741 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/models.py
+-rw-r--r--   0        0        0      581 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/signals.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/util/__init__.py
+-rw-r--r--   0        0        0     1332 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/util/color_converter.py
+-rw-r--r--   0        0        0      740 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/django_dynamic_theme/util/scss_editor.py
+-rw-r--r--   0        0        0     1054 2024-05-10 23:28:48.279073 django_dynamic_theme-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 django_dynamic_theme-0.0.8/PKG-INFO
```

### Comparing `django_dynamic_theme-0.0.7/LICENSE` & `django_dynamic_theme-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/README.md` & `django_dynamic_theme-0.0.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-dynamic-theme)
 [![](https://img.shields.io/pypi/djversions/django-dynamic-theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
+![GitHub Release](https://img.shields.io/github/v/release/segelzwerg/django-dynamic-theme)
+
 
 [![Documentation Status](https://readthedocs.org/projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-theme.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-theme)
 
 # Django Dynamic Theme
 This allows an administrator of a django website to change the theme on the fly.
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-dynamic-
 theme) [![](https://img.shields.io/pypi/djversions/django-dynamic-
 theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://
-www.djangoproject.com/) [![Documentation Status](https://readthedocs.org/
-projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-
-theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
-gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://
-codecov.io/gh/Segelzwerg/django-dynamic-theme) # Django Dynamic Theme This
-allows an administrator of a django website to change the theme on the fly. ##
-Installation ```sh pip install django-dynamic-theme ``` ## Quickstart 1. Add
-the following settings:: ```python INSTALLED_APPS = [ ...,
-"django_dynamic_theme", "compressor", ] ... # Default setting but you can set
-it to some other path. STATIC_URL = "static/" STATIC_ROOT = "static"
-STATICFILES_FINDERS = [ ..., "compressor.finders.CompressorFinder", ]
-COMPRESS_PRECOMPILERS = (("text/x-scss", "django_libsass.SassCompiler"),)
-MIDDLEWARE = [ ...,
+www.djangoproject.com/) ![GitHub Release](https://img.shields.io/github/v/
+release/segelzwerg/django-dynamic-theme) [![Documentation Status](https://
+readthedocs.org/projects/django-dynamic-theme/badge/?version=latest)](https://
+django-dynamic-theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https:
+//codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/
+badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-
+theme) # Django Dynamic Theme This allows an administrator of a django website
+to change the theme on the fly. ## Installation ```sh pip install django-
+dynamic-theme ``` ## Quickstart 1. Add the following settings:: ```python
+INSTALLED_APPS = [ ..., "django_dynamic_theme", "compressor", ] ... # Default
+setting but you can set it to some other path. STATIC_URL = "static/
+" STATIC_ROOT = "static" STATICFILES_FINDERS = [ ...,
+"compressor.finders.CompressorFinder", ] COMPRESS_PRECOMPILERS = (("text/x-
+scss", "django_libsass.SassCompiler"),) MIDDLEWARE = [ ...,
 "django_dynamic_theme.middleware.MissingThemeHandleMiddleware", ] TEMPLATES =
 { "OPTIONS": { "context_processors": [ ..., "django_dynamic_theme-
 context_processor.theme", ] } } ``` 2. Run `python manage.py migrate` 3.
 Assuming you have `base.html` add this to it before the `
 ` tag: ```html
 ... {% load compress %} {% load static %} {% compress css %}
 ...
```

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/admin.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/admin.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/middleware.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/middleware.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0001_initial.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0004_alter_background_primary_bg_theme.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0005_remove_theme_background_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0006_alter_theme_background.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0006_alter_theme_background.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0007_theme_default_theme_only_one_theme_can_be_default_.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0009_navbar.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0009_navbar.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0011_navbar_font_size.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0011_navbar_font_size.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0013_navbar_text_opacity.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0013_navbar_text_opacity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0014_alter_navbar_opacity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0015_mediagallery.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0015_mediagallery.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/migrations/0016_theme_media_gallery.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/migrations/0016_theme_media_gallery.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/models.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from abc import ABCMeta, abstractmethod
 from decimal import Decimal
 from colorfield.fields import ColorField
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 
 
-from django_dynamic_theme.utill.color_converter import hex_to_rgb_tuple
-from django_dynamic_theme.utill.scss_editor import ScssEditor
+from django_dynamic_theme.util.color_converter import hex_to_rgb_tuple
+from django_dynamic_theme.util.scss_editor import ScssEditor
 
 
 # pylint: disable=too-many-ancestors
 class FontSizeChoice(models.TextChoices):
     """
     List of pre defined css font sizes.
     Or px or em or % see https://developer.mozilla.org/en-US/docs/Web/CSS/font-size
@@ -98,14 +98,20 @@
 
     margin_left = models.CharField(max_length=50)
     margin_right = models.CharField(max_length=50)
     max_width = models.CharField(max_length=50)
     item_align = models.CharField(max_length=50)
     row_margin_top = models.CharField(max_length=50)
 
+    # pylint: disable=too-few-public-methods
+    class Meta:
+        """Meta definitions of Media Gallery"""
+        verbose_name = "Media Gallery"
+        verbose_name_plural = "Media Galleries"
+
     def export(self) -> str:
         margin_left = f"margin-left: {self.margin_left};"
         margin_right = f"margin-right: {self.margin_right};"
         max_width = f"max-width: {self.max_width};"
         text_align = f"text-align: {self.item_align};"
         row = f".row {{margin-top: {self.row_margin_top};}}"
         media_gallery = f""".mediagallery {{{margin_left}
@@ -159,15 +165,15 @@
     name = models.CharField(max_length=50)
     default = models.BooleanField(default=False)
     background: Background = models.ForeignKey(Background, on_delete=models.CASCADE)
     media_gallery: MediaGallery = models.ForeignKey(
         MediaGallery, default=None, null=True, on_delete=models.DO_NOTHING
     )
     navbar: Navbar = models.ForeignKey(
-        Navbar, default=None, null=True, on_delete=models.CASCADE
+        Navbar, default=None, null=True, on_delete=models.DO_NOTHING
     )
 
     # pylint: disable=too-few-public-methods
     class Meta:
         """Meta class of the Theme."""
 
         constraints = [
@@ -186,17 +192,27 @@
         return f"static/{self.name}.scss"
 
     # pylint: disable=no-member
     def export(self) -> str:
         """
         Exports all listed configurations as string in SCSS format.
         """
-        return f"""body {{{self.background.export()}}}
-{self.media_gallery.export()}
-{self.navbar.export()}"""
+        background = self.background.export()
+        if not self.media_gallery:
+            mediagallery = ''
+        else:
+            mediagallery = self.media_gallery.export()
+        if not self.navbar:
+            navbar = ''
+        else:
+            navbar = self.navbar.export()
+
+        return f"""body {{{background}}}
+{mediagallery}
+{navbar}"""
 
     def write_export(self) -> None:
         """Writes the content of the export to the file."""
         scss_editor = ScssEditor(self.path)
         scss_editor.write(self.export())
 
     def save(self, *args, **kwargs) -> None:
```

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/signals.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/signals.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Defines the signals for this app.
 """
 
 from django.dispatch import receiver
 from django.db.models.signals import post_delete
 
 from django_dynamic_theme.models import Theme
-from django_dynamic_theme.utill.scss_editor import ScssEditor
+from django_dynamic_theme.util.scss_editor import ScssEditor
 
 
 @receiver(post_delete, sender=Theme)
 def delete_file(
     sender, instance, *args, **kwargs  # pylint: disable=unused-argument
 ) -> None:
     """
```

### Comparing `django_dynamic_theme-0.0.7/django_dynamic_theme/utill/scss_editor.py` & `django_dynamic_theme-0.0.8/django_dynamic_theme/util/scss_editor.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_theme-0.0.7/PKG-INFO` & `django_dynamic_theme-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-theme
-Version: 0.0.7
+Version: 0.0.8
 Summary: This enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg
 Author-email: 25705862+Segelzwerg@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,16 @@
 Requires-Dist: django-compressor (>=4.4,<5.0)
 Requires-Dist: django-libsass (>=0.9,<0.10)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-dynamic-theme)
 [![](https://img.shields.io/pypi/djversions/django-dynamic-theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
+![GitHub Release](https://img.shields.io/github/v/release/segelzwerg/django-dynamic-theme)
+
 
 [![Documentation Status](https://readthedocs.org/projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-theme.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-theme)
 
 # Django Dynamic Theme
 This allows an administrator of a django website to change the theme on the fly.
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.7 Summary: This
+Metadata-Version: 2.1 Name: django-dynamic-theme Version: 0.0.8 Summary: This
 enables the administrator of a django website to change the theme on the fly.
 Author: Segelzwerg Author-email: 25705862+Segelzwerg@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=5.0,<6.0) Requires-Dist: django-colorfield
 (>=0.11.0,<0.12.0) Requires-Dist: django-compressor (>=4.4,<5.0) Requires-Dist:
 django-libsass (>=0.9,<0.10) Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Description-Content-Type: text/markdown ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/django-dynamic-theme) [![](https://
 img.shields.io/pypi/djversions/django-dynamic-
 theme?color=0C4B33&logo=django&logoColor=white&label=django)](https://
-www.djangoproject.com/) [![Documentation Status](https://readthedocs.org/
-projects/django-dynamic-theme/badge/?version=latest)](https://django-dynamic-
-theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https://codecov.io/
-gh/Segelzwerg/django-dynamic-theme/graph/badge.svg?token=YBTYAESSWE)](https://
-codecov.io/gh/Segelzwerg/django-dynamic-theme) # Django Dynamic Theme This
-allows an administrator of a django website to change the theme on the fly. ##
-Installation ```sh pip install django-dynamic-theme ``` ## Quickstart 1. Add
-the following settings:: ```python INSTALLED_APPS = [ ...,
-"django_dynamic_theme", "compressor", ] ... # Default setting but you can set
-it to some other path. STATIC_URL = "static/" STATIC_ROOT = "static"
-STATICFILES_FINDERS = [ ..., "compressor.finders.CompressorFinder", ]
-COMPRESS_PRECOMPILERS = (("text/x-scss", "django_libsass.SassCompiler"),)
-MIDDLEWARE = [ ...,
+www.djangoproject.com/) ![GitHub Release](https://img.shields.io/github/v/
+release/segelzwerg/django-dynamic-theme) [![Documentation Status](https://
+readthedocs.org/projects/django-dynamic-theme/badge/?version=latest)](https://
+django-dynamic-theme.readthedocs.io/en/latest/?badge=latest) [![codecov](https:
+//codecov.io/gh/Segelzwerg/django-dynamic-theme/graph/
+badge.svg?token=YBTYAESSWE)](https://codecov.io/gh/Segelzwerg/django-dynamic-
+theme) # Django Dynamic Theme This allows an administrator of a django website
+to change the theme on the fly. ## Installation ```sh pip install django-
+dynamic-theme ``` ## Quickstart 1. Add the following settings:: ```python
+INSTALLED_APPS = [ ..., "django_dynamic_theme", "compressor", ] ... # Default
+setting but you can set it to some other path. STATIC_URL = "static/
+" STATIC_ROOT = "static" STATICFILES_FINDERS = [ ...,
+"compressor.finders.CompressorFinder", ] COMPRESS_PRECOMPILERS = (("text/x-
+scss", "django_libsass.SassCompiler"),) MIDDLEWARE = [ ...,
 "django_dynamic_theme.middleware.MissingThemeHandleMiddleware", ] TEMPLATES =
 { "OPTIONS": { "context_processors": [ ..., "django_dynamic_theme-
 context_processor.theme", ] } } ``` 2. Run `python manage.py migrate` 3.
 Assuming you have `base.html` add this to it before the `
 ` tag: ```html
 ... {% load compress %} {% load static %} {% compress css %}
 ...
```

