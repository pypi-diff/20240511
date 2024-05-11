# Comparing `tmp/types-Pillow-9.5.0.5.tar.gz` & `tmp/types-Pillow-9.5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Pillow-9.5.0.5.tar", last modified: Wed Jun 28 21:14:21 2023, max compression
+gzip compressed data, was "types-Pillow-9.5.0.6.tar", last modified: Wed Jul  5 09:17:35 2023, max compression
```

## Comparing `types-Pillow-9.5.0.5.tar` & `types-Pillow-9.5.0.6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:21.239046 types-Pillow-9.5.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-28 21:14:18.000000 types-Pillow-9.5.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 21:14:18.000000 types-Pillow-9.5.0.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:21.239046 types-Pillow-9.5.0.5/PIL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/BdfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/BlpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/BmpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/BufrStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ContainerIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/CurImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/DcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/DdsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/EpsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ExifTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/FitsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/FitsStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/FliImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/FontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/FpxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/FtexImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/GbrImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/GdImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/GifImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/GimpGradientFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/GimpPaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/GribStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/Hdf5StubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/IcnsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/IcoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/Image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageChops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageCms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageColor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageDraw2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageEnhance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageFilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageFont.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageGrab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageMath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageMode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageMorph.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageOps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImagePalette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImagePath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageQt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageSequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageShow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageStat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageTk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageTransform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImageWin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/ImtImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/IptcImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/Jpeg2KImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/JpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/JpegPresets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-28 21:14:18.000000 types-Pillow-9.5.0.5/PIL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/McIdasImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/MicImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/MpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/MpoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/MspImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PSDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PalmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PcdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PcfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PdfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PdfParser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PixarImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PngImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PsdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/PyAccess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/QoiImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/SgiImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/SpiderImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/SunImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/TarIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/TgaImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/TiffImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/TiffTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/WalImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/WebPImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/WmfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/XVThumbImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/XbmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/XpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/_binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/_imaging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/_tkinter_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-28 21:14:02.000000 types-Pillow-9.5.0.5/PIL-stubs/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-28 21:14:21.239046 types-Pillow-9.5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 21:14:21.239046 types-Pillow-9.5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-28 21:14:18.000000 types-Pillow-9.5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:14:21.239046 types-Pillow-9.5.0.5/types_Pillow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-28 21:14:21.000000 types-Pillow-9.5.0.5/types_Pillow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-28 21:14:21.000000 types-Pillow-9.5.0.5/types_Pillow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 21:14:21.000000 types-Pillow-9.5.0.5/types_Pillow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-28 21:14:21.000000 types-Pillow-9.5.0.5/types_Pillow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:17:35.901533 types-Pillow-9.5.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-07-05 09:17:34.000000 types-Pillow-9.5.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 09:17:34.000000 types-Pillow-9.5.0.6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:17:35.901533 types-Pillow-9.5.0.6/PIL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/BdfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/BlpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/BmpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/BufrStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ContainerIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/CurImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/DcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/DdsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/EpsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ExifTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/FitsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/FitsStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/FliImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/FontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/FpxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/FtexImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/GbrImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/GdImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/GifImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/GimpGradientFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/GimpPaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/GribStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/Hdf5StubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/IcnsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/IcoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/Image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageChops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageCms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageColor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageDraw2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageEnhance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageFilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageFont.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageGrab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageMath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageMode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageMorph.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageOps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImagePalette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImagePath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageQt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageSequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageShow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageStat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageTk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageTransform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImageWin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/ImtImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/IptcImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/Jpeg2KImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/JpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/JpegPresets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 09:17:34.000000 types-Pillow-9.5.0.6/PIL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/McIdasImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/MicImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/MpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/MpoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/MspImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PSDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PalmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PcdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PcfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PdfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PdfParser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PixarImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PngImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PsdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/PyAccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/QoiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/SgiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/SpiderImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/SunImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/TarIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/TgaImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/TiffImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/TiffTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/WalImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/WebPImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/WmfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/XVThumbImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/XbmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/XpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/_binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/_imaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/_tkinter_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-05 09:17:20.000000 types-Pillow-9.5.0.6/PIL-stubs/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-05 09:17:35.901533 types-Pillow-9.5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:17:35.901533 types-Pillow-9.5.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-05 09:17:34.000000 types-Pillow-9.5.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:17:35.901533 types-Pillow-9.5.0.6/types_Pillow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-05 09:17:35.000000 types-Pillow-9.5.0.6/types_Pillow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-05 09:17:35.000000 types-Pillow-9.5.0.6/types_Pillow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:17:35.000000 types-Pillow-9.5.0.6/types_Pillow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 09:17:35.000000 types-Pillow-9.5.0.6/types_Pillow.egg-info/top_level.txt
```

### Comparing `types-Pillow-9.5.0.5/CHANGELOG.md` & `types-Pillow-9.5.0.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 9.5.0.6 (2023-07-05)
+
+Pillow: Add `tuple[int, int]` to `_Color` TypeAlias (#10407)
+
 ## 9.5.0.5 (2023-06-28)
 
 [PIL] Make return type of PyDecoder.decode a tuple (#10381)
 
 ## 9.5.0.4 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
```

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/BlpImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/BlpImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/BmpImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/BmpImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/DdsImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/DdsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/EpsImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/EpsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ExifTags.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ExifTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/FpxImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/FpxImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/GifImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/GifImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/IcnsImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/IcnsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/IcoImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/IcoImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/Image.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/Image.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 _ConversionMatrix: TypeAlias = (
     tuple[float, float, float, float] | tuple[float, float, float, float, float, float, float, float, float, float, float, float]
 )
 # `str` values are only accepted if mode="RGB" for an `Image` object
 # `float` values are only accepted for certain modes such as "F"
 # See https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.new
-_Color: TypeAlias = int | tuple[int] | tuple[int, int, int] | tuple[int, int, int, int] | str | float | tuple[float]
+_Color: TypeAlias = (
+    int | tuple[int] | tuple[int, int] | tuple[int, int, int] | tuple[int, int, int, int] | str | float | tuple[float]
+)
 
 class _Writeable(SupportsWrite[bytes], Protocol):
     def seek(self, __offset: int) -> Any: ...
 
 NORMAL: Literal[0]  # deprecated
 SEQUENCE: Literal[1]  # deprecated
 CONTAINER: Literal[2]  # deprecated
```

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageChops.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageChops.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageCms.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageCms.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageDraw.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageDraw2.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageDraw2.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageEnhance.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageEnhance.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageFile.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageFile.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageFilter.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageFilter.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageFont.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageFont.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageGrab.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageGrab.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageMath.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageMath.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageMorph.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageMorph.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageOps.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageOps.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImagePalette.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImagePalette.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageQt.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageQt.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageShow.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageShow.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageTk.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageTk.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/ImageWin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/ImageWin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/Jpeg2KImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/Jpeg2KImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/JpegImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/JpegImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/MicImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/MicImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/PSDraw.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/PSDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/PdfParser.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/PdfParser.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/PngImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/PngImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/PyAccess.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/PyAccess.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/SpiderImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/SpiderImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/TiffImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/TiffImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/TiffTags.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/TiffTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/WmfImagePlugin.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/WmfImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/_imaging.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/_imaging.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PIL-stubs/features.pyi` & `types-Pillow-9.5.0.6/PIL-stubs/features.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.5/PKG-INFO` & `types-Pillow-9.5.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.5
+Version: 9.5.0.6
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `aab9fdd86ad316f4459dd06b7a29fdafea296ff3` and was tested
+This package was generated from typeshed commit `65a6a195f2f1e4c38feeea4c4721f6c53e16fdca` and was tested
 with mypy 1.4.1, pyright 1.1.316, and
 pytype 2023.6.16.
```

### Comparing `types-Pillow-9.5.0.5/setup.py` & `types-Pillow-9.5.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `aab9fdd86ad316f4459dd06b7a29fdafea296ff3` and was tested
+This package was generated from typeshed commit `65a6a195f2f1e4c38feeea4c4721f6c53e16fdca` and was tested
 with mypy 1.4.1, pyright 1.1.316, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="9.5.0.5",
+      version="9.5.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md",
```

### Comparing `types-Pillow-9.5.0.5/types_Pillow.egg-info/PKG-INFO` & `types-Pillow-9.5.0.6/types_Pillow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.5
+Version: 9.5.0.6
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `aab9fdd86ad316f4459dd06b7a29fdafea296ff3` and was tested
+This package was generated from typeshed commit `65a6a195f2f1e4c38feeea4c4721f6c53e16fdca` and was tested
 with mypy 1.4.1, pyright 1.1.316, and
 pytype 2023.6.16.
```

### Comparing `types-Pillow-9.5.0.5/types_Pillow.egg-info/SOURCES.txt` & `types-Pillow-9.5.0.6/types_Pillow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

